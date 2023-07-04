+++
title = "Disable Ligatures in Powershell 7"
date = "2023-07-04T15:11:29-06:00"
author = "Bryce Guinta"
authorTwitter = "" #do not include @
cover = ""
tags = ["", ""]
keywords = ["", ""]
description = ""
showFullContent = false
readingTime = false
hideComments = false
color = "" #color from the theme settings
+++

Adding a font with extended icons automatically enables ligatures for powershell. This example shows CaskaydiaCove Nerd Font installed.

Here's how to do it for powershell 7.x (`pwsh`)

# How to disable Ligatures for Windows 11 Powershell 7
`$settings = (Get-Item "C:\users\$env:UserName\AppData\Local\Packages\Microsoft.WindowsTerminal_*\LocalState\settings.json")`
`notepad $settings.DirectoryName`
search for "font"
add the below "features" section into the json in your file:
```
         "font":
         {
             "face": "CaskaydiaCove Nerd Font",
             "features": {
                 "liga": 0,
                 "calt": 0
             }
         },
```
Start a new shell to check
