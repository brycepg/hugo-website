+++
title = "Install Lua Language Server for Neovim"
date = "2023-07-04T15:14:48-06:00"
author = ""
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

# Install lua language server on windows for Neovim

`Set-ExecutionPolicy RemoteSigned -Scope CurrentUser` # Optional: Needed to run a remote script the first time

`irm get.scoop.sh | iex`  
`scoop bucket add extras`  
`scoop install lua-language-server`[

