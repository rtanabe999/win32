---
title: IBackgroundCopyError interface
description: Use the IBackgroundCopyError interface to determine the cause of an error and if the transfer process can proceed.
ms.assetid: '7DCB63CF-4180-4DC3-9093-07C4F8CF7A8E'
keywords: ["IBackgroundCopyError interface", "IBackgroundCopyError interface, described"]
topic_type:
- apiref
api_name:
- IBackgroundCopyError
api_location:
- dosvc.dll
api_type:
- COM
---

# IBackgroundCopyError interface

Use the **IBackgroundCopyError** interface to determine the cause of an error and if the transfer process can proceed.

DO creates an error object only when the state of the job is BG\_JOB\_STATE\_ERROR or BG\_JOB\_STATE\_TRANSIENT\_ERROR. DO does not create an error object when an **IBackgroundCopyXXXX** interface method fails. The error object is available until DO begins transferring data (the state of the job changes to BG\_JOB\_STATE\_TRANSFERRING) for the job.

To get an **IBackgroundCopyError** object, call the [**IBackgroundCopyJob::GetError**](ibackgroundcopyjob-geterror.md) method.

## Members

The **IBackgroundCopyError** interface inherits from the [**IUnknown**](https://msdn.microsoft.com/library/windows/desktop/ms680509) interface. **IBackgroundCopyError** also has these types of members:

-   [Methods](#methods)

### Methods

The **IBackgroundCopyError** interface has these methods.



| Method                                                   | Description                                                                                 |
|:---------------------------------------------------------|:--------------------------------------------------------------------------------------------|
| [**GetError**](ibackgroundcopyerror-geterror-method.md) | Retrieves the error code and identifies the context in which the error occurred.<br/> |
| [**GetFile**](ibackgroundcopyerror-getfile-method.md)   | Retrieves an interface pointer to the file object associated with the error.<br/>     |



�

## Requirements



|                                     |                                                                                                     |
|-------------------------------------|-----------------------------------------------------------------------------------------------------|
| Minimum supported client<br/> | Windows�10, version 1709 \[desktop apps only\]<br/>                                           |
| Minimum supported server<br/> | Windows Server, version 1709 \[desktop apps only\]<br/>                                       |
| Header<br/>                   | <dl> <dt>Deliveryoptimization.h</dt> </dl>   |
| IDL<br/>                      | <dl> <dt>DeliveryOptimization.idl</dt> </dl> |
| Library<br/>                  | <dl> <dt>Dosvc.lib</dt> </dl>                |
| DLL<br/>                      | <dl> <dt>Dosvc.dll</dt> </dl>                |
| IID<br/>                      | IID\_IBackgroundCopyError is defined as 19C613A0-FCB8-4F28-81AE-897C3D078F81<br/>             |



## See also

<dl> <dt>

[**BG\_JOB\_STATE**](bg-job-state-.md)
</dt> <dt>

[**IBackgroundCopyJob::GetError**](ibackgroundcopyjob-geterror.md)
</dt> <dt>

[**IBackgroundCopyJob::GetState**](ibackgroundcopyjob-getstate.md)
</dt> <dt>

[**IBackgroundCopyCallback::JobError**](ibackgroundcopycallback-joberror-method.md)
</dt> </dl>

�

�




