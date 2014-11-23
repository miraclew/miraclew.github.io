---
layout:     post
title:      "Vim 基础 2"
subtitle:   "移动光标"
date:       2014-11-24 12:00:00
author:     "miraclew"
header-img: "img/post-bg-06.jpg"
---



<p>
    Starting an Insert - The main keys for getting into Insert Mode are i and I.

Starting an Insert with a New Line - Another way to get into Insert Mode is with o and O for creating new lines.

Starting an Insert with Append - You can also get into Insert Mode with a and A.

Replacing Characters - You can replace characters (like turning off "insert" in Notepad) with r and R.

Changing Things - You can change characters or motion related things using c and C.

Deleting Characters - Delete a single character under the cursor with x and before the cursor with X.

Deleting Lines - Delete a single line with dd.

Repeat - One of the absolutely core and biggest features of Vi is something very simple: the '.' operator. Repeat the last command by hitting '.'.
</p>


<p>
    Yanking - Yanking is "copying" in the "lousy editor" vernacular and it's done with the y key and Y key.

Putting - Putting is the inverse of yanking, and once you've yanked, you can put with the p key and P key.

Joining - You can join lines with the J key but it will put a space at the join position, so if you don't want that to happen you need to use gJ.

Visual Mode - We cover the three Visual Modes using the v key for character-wise visual selection, V for line-wise selection and CTRL-v for block-mode selection. The all-important gv sequence is also covered to help you re-select an area you just selected.
</p>