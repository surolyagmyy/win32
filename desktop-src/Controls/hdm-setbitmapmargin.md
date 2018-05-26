---
title: HDM\_SETBITMAPMARGIN message
description: Sets the width of the margin, specified in pixels, of a bitmap in an existing header control. You can send this message explicitly or use the Header\_SetBitmapMargin macro.
ms.assetid: 5ac04701-18c8-42d4-9850-fe6eb813672c
keywords:
- HDM_SETBITMAPMARGIN message Windows Controls
topic_type:
- apiref
api_name:
- HDM_SETBITMAPMARGIN
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

# HDM\_SETBITMAPMARGIN message

Sets the width of the margin, specified in pixels, of a bitmap in an existing header control. You can send this message explicitly or use the [**Header\_SetBitmapMargin**](/windows/win32/Commctrl/nf-commctrl-header_setbitmapmargin?branch=master) macro.

## Parameters

<dl> <dt>

*wParam* 
</dt> <dd>

The width, specified in pixels, of the margin that surrounds a bitmap within an existing header control.

</dd> <dt>

*lParam* 
</dt> <dd>Must be zero.</dd> </dl>

## Return value

Returns the width of the bitmap margin, in pixels. If the bitmap margin was not previously specified, the default value of 3\* [**GetSystemMetrics**](https://msdn.microsoft.com/library/windows/desktop/ms724385) (*SM\_CXEDGE*) is returned.

## Requirements



|                                     |                                                                                       |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Minimum supported client<br/> | Windows Vista \[desktop apps only\]<br/>                                        |
| Minimum supported server<br/> | Windows Server 2003 \[desktop apps only\]<br/>                                  |
| Header<br/>                   | <dl> <dt>Commctrl.h</dt> </dl> |



## See also

<dl> <dt>

[**HDM\_GETBITMAPMARGIN**](hdm-getbitmapmargin.md)
</dt> </dl>

 

 




