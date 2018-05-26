---
title: DL\_DROPPED notification code
description: Signals that the user has completed a drag operation by releasing the left mouse button. A drag list box sends this notification code to its parent window in the form of a drag list message. For more information, see Drag List Box Messages.
ms.assetid: 81b9b424-2735-407d-bac9-f03ea2f48b4e
keywords:
- DL_DROPPED notification code Windows Controls
topic_type:
- apiref
api_name:
- DL_DROPPED
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.date: 05/31/2018
ms.topic: article
ms.author: windowssdkdev
ms.prod: windows
ms.technology: desktop
---

# DL\_DROPPED notification code

Signals that the user has completed a drag operation by releasing the left mouse button. A drag list box sends this notification code to its parent window in the form of a drag list message. For more information, see [Drag List Box Messages](about-list-boxes.md#drag-list-box-messages).


```C++
DL_DROPPED

    pDragInfo = (LPARAM)(LPDRAGLISTINFO) lParam;
```



## Parameters

<dl> <dt>

*lParam* 
</dt> <dd>

A pointer to a [**DRAGLISTINFO**](/windows/win32/Commctrl/ns-commctrl-tagdraglistinfo?branch=master) structure that contains the DL\_DROPPED notification code, the handle to the drag list box, and the cursor position.

</dd> </dl>

## Return value

No return value.

## Remarks

This notification code is normally processed by inserting the item being dragged into the list in front of the item under the cursor. To retrieve the index of the item at the cursor position, use the [**LBItemFromPt**](/windows/win32/Commctrl/nf-commctrl-lbitemfrompt?branch=master) function. Note that the DL\_DROPPED notification code is sent even if the cursor is not on a list item. In that case, **LBItemFromPt** returns -1.

## Requirements



|                                     |                                                                                       |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Minimum supported client<br/> | Windows Vista \[desktop apps only\]<br/>                                        |
| Minimum supported server<br/> | Windows Server 2003 \[desktop apps only\]<br/>                                  |
| Header<br/>                   | <dl> <dt>Commctrl.h</dt> </dl> |



 

 




