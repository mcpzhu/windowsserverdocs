---
title: ksetup:dumpstate
description: Reference topic for **** - 

ms.prod: windows-server


ms.technology: manage-windows-commands

ms.topic: article
ms.assetid: 3ef2f7b8-97af-4f42-9542-cff324840637
author: coreyp-at-msft
ms.author: coreyp
manager: dongill
ms.date: 10/16/2017
---

# ksetup:dumpstate



Displays the current state of realm settings for all realms that are defined on the computer.

## Syntax

```
ksetup /dumpstate
```

#### Parameters

None

## Remarks

The output of this command includes the default realm (the domain that the computer is a member of) and all the realms that are defined on this computer. The following is included for each realm:
-   All the Key Distribution Centers (KDCs) that are associated with this realm
-   All the **set realm** flags for this realm
-   The KDC password

This command does not display the domain name that is specified by DNS detection or by the command **ksetup /domain**.

This command does not display the computer password that is set by using the command **ksetup /setcomputerpassword**.

**Ksetup** produces the same output as **ksetup /dumpstate**.

## Examples

Find most of the Kerberos realm configurations on a computer:
```
ksetup /dumpstate
```

## Additional References

-   [Ksetup](ksetup.md)
-   - [Command-Line Syntax Key](command-line-syntax-key.md)