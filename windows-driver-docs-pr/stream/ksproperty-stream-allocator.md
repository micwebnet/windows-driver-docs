---
title: KSPROPERTY\_STREAM\_ALLOCATOR
description: The KSPROPERTY\_STREAM\_ALLOCATOR property is an optional property that should be implemented if the pin allocates stream buffers or can provide an allocator
ms.assetid: 9a13efe6-4ad4-49bc-b9f1-10c22b47d9d0
keywords: ["KSPROPERTY_STREAM_ALLOCATOR Streaming Media Devices"]
topic_type:
- apiref
api_name:
- KSPROPERTY_STREAM_ALLOCATOR
api_location:
- ks.h
api_type:
- HeaderDef
ms.author: windowsdriverdev
ms.date: 11/28/2017
ms.topic: article
ms.prod: windows-hardware
ms.technology: windows-devices
---

# KSPROPERTY\_STREAM\_ALLOCATOR


The KSPROPERTY\_STREAM\_ALLOCATOR property is an optional property that should be implemented if the pin allocates stream buffers or can provide an allocator

## <span id="ddk_ksproperty_stream_allocator_ks"></span><span id="DDK_KSPROPERTY_STREAM_ALLOCATOR_KS"></span>


### <span id="Usage_Summary_Table"></span><span id="usage_summary_table"></span><span id="USAGE_SUMMARY_TABLE"></span>Usage Summary Table

<table>
<colgroup>
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
</colgroup>
<thead>
<tr class="header">
<th>Get</th>
<th>Set</th>
<th>Target</th>
<th>Property Descriptor Type</th>
<th>Property Value Type</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p>Yes</p></td>
<td><p>Yes</p></td>
<td><p>Pin</p></td>
<td><p>[<strong>KSPROPERTY</strong>](https://msdn.microsoft.com/library/windows/hardware/ff564262)</p></td>
<td><p>HANDLE</p></td>
</tr>
</tbody>
</table>

 

Remarks
-------

The returned value is always a **NULL** handle. However, support is determined by whether the call returns successfully.

The property sets the handle of the allocator assigned to the stream connection point. A connection point for KSPIN\_COMMUNICATION\_SOURCE checks the property to determine the handle of the allocator that should be used for data allocations. This property is typically set by a graph manager such as DirectShow.

An allocator handle is obtained and can be used to set the allocator for another filter pin. A filter using the allocator must reference the object to obtain a pointer to a file object and dereference the file object when a new allocator is assigned or when the connection is closed. The property can also be queried to determine if this connection point supports providing an allocator.

Requirements
------------

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p>Header</p></td>
<td>Ks.h (include Ks.h)</td>
</tr>
</tbody>
</table>

## <span id="see_also"></span>See also


[**KSPROPERTY**](https://msdn.microsoft.com/library/windows/hardware/ff564262)

 

 

[Send comments about this topic to Microsoft](mailto:wsddocfb@microsoft.com?subject=Documentation%20feedback%20%5Bstream\stream%5D:%20KSPROPERTY_STREAM_ALLOCATOR%20%20RELEASE:%20%2811/22/2017%29&body=%0A%0APRIVACY%20STATEMENT%0A%0AWe%20use%20your%20feedback%20to%20improve%20the%20documentation.%20We%20don't%20use%20your%20email%20address%20for%20any%20other%20purpose,%20and%20we'll%20remove%20your%20email%20address%20from%20our%20system%20after%20the%20issue%20that%20you're%20reporting%20is%20fixed.%20While%20we're%20working%20to%20fix%20this%20issue,%20we%20might%20send%20you%20an%20email%20message%20to%20ask%20for%20more%20info.%20Later,%20we%20might%20also%20send%20you%20an%20email%20message%20to%20let%20you%20know%20that%20we've%20addressed%20your%20feedback.%0A%0AFor%20more%20info%20about%20Microsoft's%20privacy%20policy,%20see%20http://privacy.microsoft.com/default.aspx. "Send comments about this topic to Microsoft")





