---
title: ftp send_1
description: Reference topic for **** - 

ms.prod: windows-server


ms.technology: manage-windows-commands

ms.topic: article
ms.assetid: 000aa80a-60a0-4b51-815f-3237a4f3e0f4 vhorne
author: coreyp-at-msft
ms.author: coreyp
manager: dongill
ms.date: 10/16/2017
---
# ftp: send_1

> Applies to: Windows Server (Semi-Annual Channel), Windows Server 2019, Windows Server 2016, Windows Server 2012 R2, Windows Server 2012

Copies a local file to the remote computer using the current file transfer type.   
## Syntax  
```  
send <LocalFile> [<remoteFile>]  
```  
#### Parameters  

|  Parameter   |                    Description                    |
|--------------|---------------------------------------------------|
| <LocalFile>  |         Specifies the local file to copy.         |
| <remoteFile> | Specifies the name to use on the remote computer. |

## Remarks  
- The **send** command is identical to the **put** command.  
- if *remoteFile* is not specified, the file is given the *LocalFile* name.  
  ## Examples  
  copy the local file **test.txt** and name it **test1.txt** on the remote computer.  
  ```  
  send test.txt test1.txt  
  ```  
  copy the local file **program.exe** to the remote computer.  
  ```  
  send program.exe  
  ```  
  ## Additional References  
- - [Command-Line Syntax Key](command-line-syntax-key.md)  
