﻿---
Description: 'Opens a specified folder in a Windows Explorer window.'
ms.assetid: 'DB434D02-56B2-4e8f-9E43-BBF47C7BE377'
title: 'IShellDispatch.Explore method'
---

# IShellDispatch.Explore method

Opens a specified folder in a Windows Explorer window.

## Syntax


```JScript
IShellDispatch.Explore(
  vDir
)
```

<span codelanguage="VisualBasic"></span>

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr class="header">
<th>VB</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><pre><code>IShellDispatch.Explore( _
  ByVal vDir As Variant _
)</code></pre></td>
</tr>
</tbody>
</table>



## Parameters

<dl> <dt>

*vDir* \[in\]
</dt> <dd>

Type: **Variant**

The folder to be displayed. This can be a string that specifies the path of the folder or one of the [**ShellSpecialFolderConstants**](shellspecialfolderconstants.md) values. Note that the constant names found in **ShellSpecialFolderConstants** are available in Visual Basic, but not in VBScript or JScript. In those cases, the numeric values must be used in their place.

</dd> </dl>

## Return value

### JScript

This method does not return a value.

### VB

This method does not return a value.

## Remarks

This method is implemented and accessed through the [**Shell.Explore**](shell-explore.md) method.

## Examples

The following examples show the use of **Explore** in JScript, VBScript, and Visual Basic.

JScript:


```JScript
<script language="JScript">
    function fnShellExploreJ()
    {
        var objShell = new ActiveXObject("shell.application");
        
        objshell.Explore("C:\\");
    }
</script>
```



VBScript:


```VB
<script language="VBScript">
    function fnShellExploreVB()
        dim objShell
        dim ssfWINDOWS
        ssfWINDOWS = 36

        set objShell = CreateObject("shell.application")
        objshell.Explore(ssfWINDOWS)

        set objShell = nothing
    end function
 </script>
```



Visual Basic:


```VB
Private Sub fnShellExploreVB()
    Dim objShell As Shell

    Set objShell = New Shell
    objshell.Explore (ssfPERSONAL)

    Set objShell = Nothing
End Sub
```



## Requirements



|                                     |                                                                                                                |
|-------------------------------------|----------------------------------------------------------------------------------------------------------------|
| Minimum supported client<br/> | Windows 2000 Professional, Windows XP \[desktop apps only\]<br/>                                         |
| Minimum supported server<br/> | Windows 2000 Server \[desktop apps only\]<br/>                                                           |
| Header<br/>                   | <dl> <dt>Shldisp.h</dt> </dl>                           |
| IDL<br/>                      | <dl> <dt>Shldisp.idl</dt> </dl>                         |
| DLL<br/>                      | <dl> <dt>Shell32.dll (version 4.71 or later)</dt> </dl> |



 

 



