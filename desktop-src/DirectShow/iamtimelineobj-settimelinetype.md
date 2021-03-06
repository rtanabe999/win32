---
description: Not supported. Call the IAMTimeline::CreateEmptyNode method to create a new timeline object. Once an object is created, you cannot change its type.
ms.assetid: 127b7435-84b0-46c4-b072-bb8eb54b6a4f
title: IAMTimelineObj::SetTimelineType method (Qedit.h)
ms.topic: reference
ms.date: 05/31/2018
topic_type: 
- APIRef
- kbSyntax
api_name: 
- IAMTimelineObj.SetTimelineType
api_type: 
- COM
api_location: 
- strmiids.lib
- strmiids.dll
---

# IAMTimelineObj::SetTimelineType method

> [!Note]  
> \[Deprecated. This API may be removed from future releases of Windows.\]

 

Not supported. Call the [**IAMTimeline::CreateEmptyNode**](iamtimeline-createemptynode.md) method to create a new timeline object. Once an object is created, you cannot change its type.

## Syntax


```C++
HRESULT SetTimelineType(
   TIMELINE_MAJOR_TYPE newVal
);
```



## Parameters

<dl> <dt>

*newVal* 
</dt> <dd>

Reserved.

</dd> </dl>

## Return value

If this method succeeds, it returns **S\_OK**. Otherwise, it returns an **HRESULT** error code.

## Remarks

> [!Note]  
> The header file Qedit.h is not compatible with Direct3D headers later than version 7.

 

> [!Note]  
> To obtain Qedit.h, download the [Microsoft Windows SDK Update for Windows Vista and .NET Framework 3.0](https://msdn.microsoft.com/windowsvista/bb980924.aspx). Qedit.h is not available in the Microsoft Windows SDK for Windows 7 and .NET Framework 3.5 Service Pack 1.

 

## Requirements



|                    |                                                                                         |
|--------------------|-----------------------------------------------------------------------------------------|
| Header<br/>  | <dl> <dt>Qedit.h</dt> </dl>      |
| Library<br/> | <dl> <dt>Strmiids.lib</dt> </dl> |



## See also

<dl> <dt>

[**IAMTimelineObj Interface**](iamtimelineobj.md)
</dt> </dl>

 

 




