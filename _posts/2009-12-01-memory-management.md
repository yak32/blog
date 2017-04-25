---
layout: post
title: Memory management
date: 2009-12-01 09:47
author: admin
comments: true
categories: [engine]
---
<a href="http://2.bp.blogspot.com/_LfYx03jjmdk/SxTmMikpqMI/AAAAAAAAAus/R4ZYOjH9OsE/s1600/LIttleZombieSusie2.jpg">

<img class="image featured" border="3" alt="" src="http://2.bp.blogspot.com/_LfYx03jjmdk/SxTmMikpqMI/AAAAAAAAAus/R4ZYOjH9OsE/s320/LIttleZombieSusie2.jpg" id="BLOGGER_PHOTO_ID_5410202155492157634" /></a>

Usually C++ uses linked list to holding free memory chunks, so searching for free chunk is not fast. Especially for small objects. So I decided to optimize allocating of memory using special pool allocator. All small objects in engine have base class, which  get and release memory from pool allocator. 3x times optimization for memory allocation (small objects)  Look Andrei Alexandrescu <a href="http://www.amazon.com/exec/obidos/ASIN/0201704315/modecdesi-20" target="_top">Modern C++ Design</a> and in details <a href="http://books.google.com/books?id=aJ1av7UFBPwC&amp;pg=PA78&amp;lpg=PA78&amp;dq=Andrei+Alexandrescu+pool+allocator&amp;source=bl&amp;ots=YQfM1pOh7_&amp;sig=reCULuBCidrVZX9rJNgwdH-fiRE&amp;hl=en&amp;ei=ds8VS4vtD5CTkAWZgZWABw&amp;sa=X&amp;oi=book_result&amp;ct=result&amp;resnum=1&amp;ved=0CAgQ6AEwAA#v=onepage&amp;q=&amp;f=false">here</a></span>
