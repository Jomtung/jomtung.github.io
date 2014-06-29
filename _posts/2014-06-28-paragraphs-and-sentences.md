---
layout: post
title:  "paragraphs and sentences"
date:   2014-06-28 12:56:10
categories: first
---

I started building a python module to split text files into paragraphs the other day.  Turns out "how to divide texts into paragraphs is not considered as a significant problem in natural language processing" according to the NLTK folks.
So I can't use their work.  Although I may have trusted the good guys at NLTK too much about paragraph parsing , I took this to mean anything I could come up with for the job might be half decent.

As I'm building the module, it dawns on me that I'll have to also split each paragraph into sentences and build the
entire structure of paragraphs and sentences into referenced objects.  Not a bad problem, but I can't help thinking
someone has done most of the work already.  Instead of googling each way to read text files and transform strings into strings (''.join(str) >> str += line) I found an awesome [post on the subject](http://code.activestate.com/recipes/66063-read-a-text-file-by-paragraph/) with a full explanation and even a generator solution in the comments.  Glory to google!

###Problems with pasting
Now I just have to use one of those bad ass looking methods and apply them to my problem of paragraph parsing and
sentence parsing within the paragraph object. Fun!  Two awesome algorithms to do some awesome things.  That's when
I realized I didn't know exactly how paragraphs should be defined.  

So I decided that markdown as the base format keeps the complications simple with paragraph definitions and I could worry about sentence definitions later since those are standard punctuation delimiters.  Then I paste and throw the test text file into these awesome functions and start to actually read the code.  

Of course that didn't work.  I need to read the code first.  

I need to read the code and find out that both of these guys have an awesome solution that I would have to apply to my specific problem of crunching a text file into a list of strings which are paragraphs.  I need to read and find it would be faster to write a simple version.  So I write the simple version and now there's a third way to do it and I still haven't read through  either awesome method.  Once I get to that I'll decide that mine is the most awesome of course.  Because it's simple.  Simply awesome.

###Adventures -n- sentences
Now that I have paragraph lists for the text files in my head I, I should start to make the paragraph list
ready for cool things like semantic operations, autonomous categorization, learning to talk shit like a teenager, and other things a granular text object should be able to facilitate.  This meant taking paragraphs, counting them as a base object, then splitting them up into sentence units.  Furthermore, to achieve the teenage mouthing I'd need to build context awareness dictionaries (which are two separate things really) based on each word.  That meant taking sentences, counting them as another object (child to paragraph), then splitting them up into word units.  Thanks to Python, lists and regex patterns make this somewhat bearable.

So after a while I have a pretty cool set of functions that are able to parse a text file into words listed by
sentences listed by paragraphs.  I've push it to the [ResOnMe gitub repo](https://github.com/Jomtung/ResOnMe-Core) since this is part of the core engine used for input to markdown and markdown to output.  The only thing left is to make the class into a single readable generator function.  I might put that question on [Stack Overflow](http://stackoverflow.com/) if I can't figure it out.
