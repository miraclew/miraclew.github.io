---
layout:     post
title:      "Vim 基础 3"
subtitle:   "移动光标"
date:       2014-11-24 12:00:00
author:     "miraclew"
header-img: "img/post-bg-06.jpg"
---


<p>
    Listing Buffers - Good ol' ls is your friend here.

Switching Buffers - The buffer command gets you there and it can be used a ton of different ways.

Buffer deletion - The bdelete command is used to delete buffers and it can be used in an equally vast number of ways.


</p>

<p>
    Splitting Windows - There's vertical splits and horizontal splits. Split horizontally with :split or CTRL-w s and vertically with :vsplit or CTRL-w v.

Closing Windows - You can close with :close or CTRL-w c.

Switching Windows - Change windows with CTRL-w h, CTRL-w j, CTRL-w k or CTRL-w l.

Switching Windows (continued) - You can also switch to the "previous" window with CTRL-w p.

Switching Windows (continued again) - If you want to jump around windows a bit quicker then you can pass a numeric argument to the CTRL-w {motion} command such as 5CTRL-w k to move up 5 windows.

Moving Windows - If you want to reposition a window to another spot, you can use the CTRL-w H, CTRL-w J, CTRL-w K or CTRL-w L commands.

Focusing a Window - If you want to de-clutter your workspace and make the current window the only visible window then you can hit CTRL-w o.

You can check out my mappings for dealing with windows in the vimrc section.
</p>