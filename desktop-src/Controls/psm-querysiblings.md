---
title: PSM\_QUERYSIBLINGS message
description: Sent to a property sheet, which then forwards the message to each of its pages. You can send this message explicitly or by using the PropSheet\_QuerySiblings macro.
ms.assetid: '96f48847-b7b8-4d6f-8bde-ada915b7c962'
keywords: ["PSM_QUERYSIBLINGS message Windows Controls"]
topic_type:
- apiref
api_name:
- PSM_QUERYSIBLINGS
api_location:
- Prsht.h
api_type:
- HeaderDef
---

# PSM\_QUERYSIBLINGS message

Sent to a property sheet, which then forwards the message to each of its pages. You can send this message explicitly or by using the [**PropSheet\_QuerySiblings**](propsheet-querysiblings.md) macro.

## Parameters

<dl> <dt>

*wParam* 
</dt> <dd>

First application-defined parameter.

</dd> <dt>

*lParam* 
</dt> <dd>

Second application-defined parameter.

</dd> </dl>

## Return value

Returns the nonzero value from a page in the property sheet, or zero if no page returns a nonzero value.

## Remarks

If a page returns a nonzero value, the property sheet does not send the message to subsequent pages.

## Requirements



|                                     |                                                                                    |
|-------------------------------------|------------------------------------------------------------------------------------|
| Minimum supported client<br/> | Windows�Vista \[desktop apps only\]<br/>                                     |
| Minimum supported server<br/> | Windows Server�2003 \[desktop apps only\]<br/>                               |
| Header<br/>                   | <dl> <dt>Prsht.h</dt> </dl> |



�

�




