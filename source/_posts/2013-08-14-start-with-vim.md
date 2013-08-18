---
layout: post
title: "Start with VIM"
date: 2013-08-14 22:24
comments: true
categories: VIM
---

#### Basic Vim

`j` Move down one line

`G` Go to bottom of file 

H | J | K | L |
--|
left|down|up|right|

`yy` Yank line  
`p` Paste above cursor  
`i` Insert text before cursor
`a` Append text after cursor  
`fN` Jump forward to first 'N'  
`3fN` Jump forward to third 'N'  
`6l` Forward 6 letters  
`2j` Down 2 lines  
`w` Forward one word  
`cw` Change word  
`u` Undo
`Ctrl-R` Redo
`vim -N ` Use newer Vim mode not compatible with original vi  
`:w !sudo tee %` with root permissions
#### Edit












`d$` Delete through end of line 

`c2/end<Return>` Change text from cursor through next two occurrences of "end"

`i` Insert text at cursor(activates Insert mode)在光标前  
`I` Insert text at start of line  
`w` Move forward by one word
`b` Move backward by one word