---
title: SM\_RemovePort function
description: The SM\_RemovePort WMI method configures the WMI provider so that it stops passing events that are associated with the indicated port to the WMI client.
keywords: ["SM_RemovePort function Storage Devices"]
topic_type:
- apiref
api_name:
- SM_RemovePort
api_location:
- Hbapiwmi.h
api_type:
- HeaderDef
ms.date: 10/17/2018
---

# SM\_RemovePort function


The SM\_RemovePort WMI method configures the WMI provider so that it stops passing events that are associated with the indicated port to the WMI client.

## Syntax

```ManagedCPlusPlus
void SM_RemovePort(
   [in, HBAType("HBA_WWN")] uint8          PortWWN[8],
   [in, EVENT_TYPES_QUALIFIERS] uint32     EventType,
   [out, HBA_STATUS_QUALIFIERS] HBA_STATUS HBAStatus
);
```

## Parameters

*PortWWN*   
A worldwide name (WWN) that indicates the port that should be removed from the list of ports whose events are reported to the WMI client.

*EventType*   
The type of the event. The values that can be assigned to this member are defined by the EVENT\_TYPES\_QUALIFIERS WMI class qualifier.

*HBAStatus*   
The status of the operation. For a list of allowed values and their descriptions, see [HBA\_STATUS](hba-status.md). The miniport driver returns this information in the HBAStatus member of a SM\_RemovePort\_OUT structure.

## Return value

Not applicable to WMI methods.

## Remarks

This WMI method belongs to the MS\_SM\_EventControl WMI Class.

## Requirements

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td align="left"><p>Target platform</p></td>
<td align="left">Desktop</td>
</tr>
<tr class="even">
<td align="left"><p>Header</p></td>
<td align="left">Hbapiwmi.h</td>
</tr>
</tbody>
</table>

## <span id="see_also"></span>See also


[HBA\_STATUS](hba-status.md)

[**SM\_RemovePort\_IN**](/windows-hardware/drivers/ddi/hbapiwmi/ns-hbapiwmi-_sm_removeport_in)

[**SM\_RemovePort\_OUT**](/windows-hardware/drivers/ddi/hbapiwmi/ns-hbapiwmi-_sm_removeport_out)

 

