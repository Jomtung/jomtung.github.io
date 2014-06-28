---
layout: post
title:  "paragraphs and sentences"
date:   2014-06-28 12:56:10
categories: jekyll update
---

I started building a python module to split text files into paragraphs the other day.  Turns out that this "is not
an interesting NLP problem" and so there are no standard algorithms to approach the task.  Although I may have just
trusted that website too much, I took this to mean anything I could come up with for the job might be half decent.

As I'm using python to build a class module to get this done, it dawns on me that I'll have to also split each
paragraph into sentences and build the entire structure of paragraphs and sentences into referenced objects.  Not a
bad problem, but I can't help thinking someone has done most of the work already.  So I started by googling and
coming up with the usual text file i/o results.  I started to debate conveting the text file into a single string
to split by empty line versus using a list of lines to do the same.  As I'm steadily building out the problems and
have a simple solution, I can't help but think of how many other people must have solved the same problem and that
it would be around.  So I googled the full "python text file into paragraphs" instead of googling each way to read
text files and crunch string lists into strings (''.join(str) >> str += line) and finally found an awesome [post on
the subject](http://code.activestate.com/recipes/66063-read-a-text-file-by-paragraph/) with a full explanation and
even a generator solution in the comments.  Glory to google!

###Problems with pasting
Now I just have to use one of those bad ass looking methods and apply them to my problem of paragraph parsing and
sentence parsing within the paragraph object. Fun!
