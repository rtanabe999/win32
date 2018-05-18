---
title: GetErrorEx method of the Msvm\_NetworkJob class
description: When the job is executing or has terminated without error, then this method returns no Msvm\_Error instance.
ms.assetid: 'af2f23ed-026c-4154-b910-53aefc2cb71c'
keywords: ["GetErrorEx method Hyper-V", "GetErrorEx method Hyper-V , Msvm_NetworkJob class", "Msvm_NetworkJob class Hyper-V , GetErrorEx method"]
topic_type:
- apiref
api_name:
- Msvm_NetworkJob.GetErrorEx
api_location:
- Root\Virtualization
api_type:
- COM
---

# GetErrorEx method of the Msvm\_NetworkJob class

When the job is executing or has terminated without error, then this method returns no [**Msvm\_Error**](msvm-error.md) instance. However, if the job has failed because of some internal problem or because the job has been terminated by a client, then one or more **Msvm\_Error** instances are returned.

## Syntax


```mof
uint32 GetErrorEx(
  [out]�string Errors[]
);
```



## Parameters

<dl> <dt>

*Errors* \[out\]
</dt> <dd>

Type: **string\[\]**

If the operational status on the job is not "OK", this method returns an array of CIM error instances. Otherwise, if the job is "OK", this method returns **NULL**.

</dd> </dl>

## Return value

Type: **uint32**

This method returns one of the following values.

<dl> <dt>

**Completed with No Error** (0)
</dt> <dt>

**Failed** (32768)
</dt> <dt>

**Access Denied** (32769)
</dt> <dt>

**Not Supported** (32770)
</dt> <dt>

**Status is unknown** (32771)
</dt> <dt>

**Timeout** (32772)
</dt> <dt>

**Invalid parameter** (32773)
</dt> <dt>

**System is in used** (32774)
</dt> <dt>

**Invalid state for this operation** (32775)
</dt> <dt>

**Incorrect data type** (32776)
</dt> <dt>

**System is not available** (32777)
</dt> <dt>

**Out of memory** (32778)
</dt> </dl>

## Remarks

Access to the [**Msvm\_NetworkJob**](msvm-networkjob.md) class might be restricted by UAC Filtering. For more information, see [User Account Control and WMI](https://msdn.microsoft.com/library/aa826699).

## Requirements



|                                     |                                                                                                      |
|-------------------------------------|------------------------------------------------------------------------------------------------------|
| Minimum supported client<br/> | None supported<br/>                                                                            |
| Minimum supported server<br/> | Windows Server�2008<br/>                                                                       |
| End of client support<br/>    | None supported<br/>                                                                            |
| End of server support<br/>    | Windows Server�2012<br/>                                                                       |
| Namespace<br/>                | Root\\Virtualization<br/>                                                                      |
| MOF<br/>                      | <dl> <dt>WindowsVirtualization.mof</dt> </dl> |



## See also

<dl> <dt>

[**Msvm\_NetworkJob**](msvm-networkjob.md)
</dt> </dl>

�

�




