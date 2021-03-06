---
title: Symbol Status Abbreviations
description: Symbol Status Abbreviations
ms.assetid: 198453f2-fc9a-4313-875e-ac963b843df9
keywords: ["symbols, symbol status abbreviations", "deferred (symbol status abbreviation)", "(symbol status abbreviation)", "T (symbol status abbreviation)", "C (symbol status abbreviation)", "DIA (symbol status abbreviation)", "Export (symbol status abbreviation)", "PERF (symbol status abbreviation)", "PDB (symbol status abbreviation)"]
ms.author: domars
ms.date: 05/23/2017
ms.topic: article
ms.prod: windows-hardware
ms.technology: windows-devices
---

# Symbol Status Abbreviations


## <span id="ddk_symbol_status_abbreviations_dbg"></span><span id="DDK_SYMBOL_STATUS_ABBREVIATIONS_DBG"></span>


Symbol file types and their loading status can be determined by using the [**lm (List Loaded Modules)**](lm--list-loaded-modules-.md) command, the [**!lmi**](-lmi.md) extension, or WinDbg's [Debug | Modules](debug---modules.md) menu command.

Each of these displays information about loaded modules and their symbols.

The following abbreviations are used in the displays generated by these commands:

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th align="left">Abbreviation</th>
<th align="left">Meaning</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td align="left"><p><strong>deferred</strong></p></td>
<td align="left"><p>The module has been loaded, but the debugger has not attempted to load the symbols. Symbols will be loaded when needed. See [Deferred Symbol Loading](deferred-symbol-loading.md) for details.</p></td>
</tr>
<tr class="even">
<td align="left"><p><strong>#</strong></p></td>
<td align="left"><p>There is a mismatch between the symbol file and the executable, either in their timestamps or in their checksums.</p></td>
</tr>
<tr class="odd">
<td align="left"><p><strong>T</strong></p></td>
<td align="left"><p>The timestamp is missing, not accessible, or equal to zero.</p></td>
</tr>
<tr class="even">
<td align="left"><p><strong>C</strong></p></td>
<td align="left"><p>The checksum is missing, not accessible, or equal to zero.</p></td>
</tr>
<tr class="odd">
<td align="left"><p><strong>DIA</strong></p></td>
<td align="left"><p>Symbol files were loaded through Debug Interface Access (DIA).</p></td>
</tr>
<tr class="even">
<td align="left"><p><strong>Export</strong></p></td>
<td align="left"><p>No actual symbol files were found, so symbol information was extracted from the binary file's export table.</p></td>
</tr>
<tr class="odd">
<td align="left"><p><strong>M</strong></p></td>
<td align="left"><p>There is a mismatch between the symbol file and the executable, either in their timestamps or in their checksums. However, symbol files have been loaded anyway due to the symbol option settings.</p></td>
</tr>
<tr class="even">
<td align="left"><p><strong>PERF</strong></p></td>
<td align="left"><p>This binary contains [performance-optimized code](debugging-performance-optimized-code.md). Standard address arithmetic may not produce correct results.</p></td>
</tr>
<tr class="odd">
<td align="left"><p><strong>Stripped</strong></p></td>
<td align="left"><p>Debug information was stripped from the image file.</p></td>
</tr>
<tr class="even">
<td align="left"><p><strong>PDB</strong></p></td>
<td align="left"><p>The symbols are in .pdb format.</p></td>
</tr>
<tr class="odd">
<td align="left"><p><strong>COFF</strong></p></td>
<td align="left"><p>The symbols are in common object file format (COFF) symbol format.</p></td>
</tr>
</tbody>
</table>

 

 

 

[Send comments about this topic to Microsoft](mailto:wsddocfb@microsoft.com?subject=Documentation%20feedback%20[debugger\debugger]:%20Symbol%20Status%20Abbreviations%20%20RELEASE:%20%285/15/2017%29&body=%0A%0APRIVACY%20STATEMENT%0A%0AWe%20use%20your%20feedback%20to%20improve%20the%20documentation.%20We%20don't%20use%20your%20email%20address%20for%20any%20other%20purpose,%20and%20we'll%20remove%20your%20email%20address%20from%20our%20system%20after%20the%20issue%20that%20you're%20reporting%20is%20fixed.%20While%20we're%20working%20to%20fix%20this%20issue,%20we%20might%20send%20you%20an%20email%20message%20to%20ask%20for%20more%20info.%20Later,%20we%20might%20also%20send%20you%20an%20email%20message%20to%20let%20you%20know%20that%20we've%20addressed%20your%20feedback.%0A%0AFor%20more%20info%20about%20Microsoft's%20privacy%20policy,%20see%20http://privacy.microsoft.com/default.aspx. "Send comments about this topic to Microsoft")




