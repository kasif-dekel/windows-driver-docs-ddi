---
UID: NF:dbgeng.IDebugClient3.AbandonCurrentProcess
title: IDebugClient3::AbandonCurrentProcess
description: The AbandonCurrentProcess method removes the current process from the debugger engine's process list without detaching or terminating the process.
old-location: debugger\abandoncurrentprocess.htm
tech.root: debugger
ms.assetid: a6abbdb8-8d19-4ae0-8272-8faa87b8e409
ms.date: 05/03/2018
ms.keywords: AbandonCurrentProcess, AbandonCurrentProcess method [Windows Debugging], AbandonCurrentProcess method [Windows Debugging],IDebugClient2 interface, AbandonCurrentProcess method [Windows Debugging],IDebugClient3 interface, AbandonCurrentProcess method [Windows Debugging],IDebugClient4 interface, AbandonCurrentProcess method [Windows Debugging],IDebugClient5 interface, IDebugClient2 interface [Windows Debugging],AbandonCurrentProcess method, IDebugClient2::AbandonCurrentProcess, IDebugClient3 interface [Windows Debugging],AbandonCurrentProcess method, IDebugClient3.AbandonCurrentProcess, IDebugClient3::AbandonCurrentProcess, IDebugClient4 interface [Windows Debugging],AbandonCurrentProcess method, IDebugClient4::AbandonCurrentProcess, IDebugClient5 interface [Windows Debugging],AbandonCurrentProcess method, IDebugClient5::AbandonCurrentProcess, IDebugClient_2a3f34d6-591b-4cae-bc28-2da5f05a9548.xml, dbgeng/IDebugClient2::AbandonCurrentProcess, dbgeng/IDebugClient3::AbandonCurrentProcess, dbgeng/IDebugClient4::AbandonCurrentProcess, dbgeng/IDebugClient5::AbandonCurrentProcess, debugger.abandoncurrentprocess
ms.topic: method
req.header: dbgeng.h
req.include-header: Dbgeng.h
req.target-type: Desktop
req.target-min-winverclnt: 
req.target-min-winversvr: 
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: 
req.dll: 
req.irql: 
topic_type:
-	APIRef
-	kbSyntax
api_type:
-	COM
api_location:
-	dbgeng.h
api_name:
-	IDebugClient2.AbandonCurrentProcess
-	IDebugClient3.AbandonCurrentProcess
-	IDebugClient4.AbandonCurrentProcess
-	IDebugClient5.AbandonCurrentProcess
product:
- Windows
targetos: Windows
req.typenames: 
---

# IDebugClient3::AbandonCurrentProcess


## -description


The <b>AbandonCurrentProcess</b> method removes the <a href="https://msdn.microsoft.com/295b05a3-e27f-4761-a562-7e87e25bfd3b">current process</a> from the debugger engine's process list without detaching or terminating the process.


## -parameters






## -returns



This method may also return error values.  See <a href="https://msdn.microsoft.com/713f3ee2-2f5b-415e-9908-90f5ae428b43">Return Values</a> for more details.

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>S_OK</b></dt>
</dl>
</td>
<td width="60%">
The method was successful.

</td>
</tr>
</table>
 




## -remarks



This method is only available for live user-mode debugging.  The target must be running on Windows XP or a later version of Windows.

Windows will continue to consider this process as being debugged, and so the process will remain suspended.  This method allows the debugger to be shut down and a new debugger to attach to the process.  See <a href="https://msdn.microsoft.com/library/windows/hardware/ff552020">Live User-Mode Targets</a> and <a href="https://msdn.microsoft.com/cc137185-58a7-44bf-b262-2698c46730f6">Re-attaching to the Target Application</a> for more information.




## -see-also




<a href="https://msdn.microsoft.com/library/windows/hardware/ff561508">.abandon (Abandon Process)</a>



<a href="https://msdn.microsoft.com/library/windows/hardware/ff538150">AttachProcess</a>



<a href="https://msdn.microsoft.com/library/windows/hardware/ff540055">CreateProcessAndAttach2</a>



<a href="https://msdn.microsoft.com/library/windows/hardware/ff541846">DetachCurrentProcess</a>



<a href="https://msdn.microsoft.com/library/windows/hardware/ff550481">IDebugClient2</a>



<a href="https://msdn.microsoft.com/library/windows/hardware/ff550488">IDebugClient3</a>



<a href="https://msdn.microsoft.com/library/windows/hardware/ff550494">IDebugClient4</a>



<a href="https://msdn.microsoft.com/library/windows/hardware/ff550497">IDebugClient5</a>



<a href="https://msdn.microsoft.com/library/windows/hardware/ff558866">TerminateCurrentProcess</a>
 

 

