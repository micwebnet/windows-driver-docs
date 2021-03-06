---
title: GUID_61883_CLASS
description: GUID_61883_CLASS
ms.assetid: 3380c42c-3ac4-4d71-9a1b-581ef8c7b57a
keywords: ["GUID_61883_CLASS Device and Driver Installation"]
topic_type:
- apiref
api_name:
- GUID_61883_CLASS
api_location:
- 61883.h
api_type:
- HeaderDef
---

# GUID_61883_CLASS


The GUID_61883_CLASS [device interface class](https://msdn.microsoft.com/library/windows/hardware/ff541339) is defined for devices in the 61883 [device setup class](https://msdn.microsoft.com/library/windows/hardware/ff541509).

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th align="left">Attribute</th>
<th align="left">Setting</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td align="left"><p>Identifier</p></td>
<td align="left"><p>GUID_61883_CLASS</p></td>
</tr>
<tr class="even">
<td align="left"><p>Class GUID</p></td>
<td align="left"><p>{7EBEFBC0-3200-11d2-B4C2-00A0C9697D07}</p></td>
</tr>
</tbody>
</table>

 

Remarks
-------

Drivers for devices in the 61883 device setup class register instances of this device interface class to notify the operating system and applications of the presence of 61883 devices. The 61883 device interface class includes IEEE 1394 devices that support the IEC-61883 protocol. For information about 61883 devices and drivers, see [IEC-61883 Client Drivers](https://msdn.microsoft.com/library/windows/hardware/ff537188).

For information about the device setup class for 1394 bus devices, see [**BUS1394_CLASS_GUID**](bus1394-class-guid.md).

Requirements
------------

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td align="left"><p>Version</p></td>
<td align="left"><p>Available in Windows XP and later versions of Windows.</p></td>
</tr>
<tr class="even">
<td align="left"><p>Header</p></td>
<td align="left">61883.h (include 61883.h)</td>
</tr>
</tbody>
</table>

## See also


[**BUS1394_CLASS_GUID**](bus1394-class-guid.md)

 

 

[Send comments about this topic to Microsoft](mailto:wsddocfb@microsoft.com?subject=Documentation%20feedback%20%5Bdevinst\devinst%5D:%20GUID_61883_CLASS%20%20RELEASE:%20%2810/9/2017%29&body=%0A%0APRIVACY%20STATEMENT%0A%0AWe%20use%20your%20feedback%20to%20improve%20the%20documentation.%20We%20don't%20use%20your%20email%20address%20for%20any%20other%20purpose,%20and%20we'll%20remove%20your%20email%20address%20from%20our%20system%20after%20the%20issue%20that%20you're%20reporting%20is%20fixed.%20While%20we're%20working%20to%20fix%20this%20issue,%20we%20might%20send%20you%20an%20email%20message%20to%20ask%20for%20more%20info.%20Later,%20we%20might%20also%20send%20you%20an%20email%20message%20to%20let%20you%20know%20that%20we've%20addressed%20your%20feedback.%0A%0AFor%20more%20info%20about%20Microsoft's%20privacy%20policy,%20see%20http://privacy.microsoft.com/default.aspx. "Send comments about this topic to Microsoft")





