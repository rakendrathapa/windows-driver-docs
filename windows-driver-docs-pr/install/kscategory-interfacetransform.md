---
title: KSCATEGORY_INTERFACETRANSFORM
description: KSCATEGORY_INTERFACETRANSFORM
keywords: ["KSCATEGORY_INTERFACETRANSFORM Device and Driver Installation"]
topic_type:
- apiref
api_name:
- KSCATEGORY_INTERFACETRANSFORM
api_location:
- Ks.h
api_type:
- HeaderDef
ms.date: 10/17/2018
---

# KSCATEGORY_INTERFACETRANSFORM


The KSCATEGORY_INTERFACETRANSFORM [device interface class](./overview-of-device-interface-classes.md) is defined for the [kernel streaming](../stream/streaming-minidrivers2.md) (KS) functional category that transforms the interface of a device.

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
<td align="left"><p>KSCATEGORY_INTERFACETRANSFORM</p></td>
</tr>
<tr class="even">
<td align="left"><p>Class GUID</p></td>
<td align="left"><p>{CF1DDA2D-9743-11D0-A3EE-00A0C9223196}</p></td>
</tr>
</tbody>
</table>

 

## Remarks

Drivers for KS devices register instances of KSCATEGORY_INTERFACETRANSFORM to indicate to the operating system that the devices support the KSCATEGORY_INTERFACETRANSFORM functional category.

The KSCATEGORY_INTERFACETRANSFORM functional category is one of the [**KSPROPERTY_TOPOLOGY_CATEGORIES**](../stream/ksproperty-topology-categories.md) functional categories.

## Requirements

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td align="left"><p>Header</p></td>
<td align="left">Ks.h (include Ks.h)</td>
</tr>
</tbody>
</table>

## See also


[**KSPROPERTY_TOPOLOGY_CATEGORIES**](../stream/ksproperty-topology-categories.md)

 

