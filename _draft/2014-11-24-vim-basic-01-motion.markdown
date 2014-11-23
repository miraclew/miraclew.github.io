---
layout:     post
title:      "Vim 基础 1"
subtitle:   "移动光标"
date:       2014-11-24 12:00:00
author:     "miraclew"
header-img: "img/post-bg-06.jpg"
---

<h2>移动光标</h2>

<h3>慢移动</h3>
* C-j: 下
* C-k: 上
* C-l: 右
* C-h: 左

<h3>行中移动</h3>
 * 行首，行尾 0 和 $
 * 单词移动(向前) w, W, e, E
 * 单词移动(向后) b,B, ge, gE

<h3>翻页</h3>

<p>
    Paging - Moving the page up and down by full pages with CTRL-f and CTRL-b and by half pages with CTRL-u and CTRL-d.

Cursor jumping to screen parts - Moving to the head, middle and last line of a screen with H, M and L respectively.

Top and Bottom of the buffer - Jumping to the top line of the entire buffer with gg and the bottom of the entire buffer with G.

Jumping to a particular line - Get to a specific line number with <number>G.

Easy regular expression searching - The famous '*' and '#' keys for jumping by bounded regular expression.

Manual regular expression searching - Using '/' and '?' to manually search.

</p>

<p>
    Start of Function or Class Jumping - Moving to the beginning of functions and classes backwards through the buffer with [[ and the beginning of functions and classes forwards through the buffer with ]] (assuming you code properly and put braces for these things in column 0 (hanging brace?? Come on! :D).

End of Function or Class Jumping - Forwards to the end of a function or class definition with ][ and backwards to the end of a function or class definition with [].

Jumping to Matching Braces - The fantastic % characters.

Marks - Basic mark functionality and how it works with m, ' and `.
</p>
