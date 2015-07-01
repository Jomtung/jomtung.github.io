---
layout: post
title:  "vim wins all the files, but emacs is cooler"
date:   2015-07-01
categories: firstpost, flametopic, vim, emacs, configuration
--

I still remember when I decided to choose between vim and emacs.  I didn't have many requirements to choose the winner, but I knew what had to be done.  I had a 4 GB (maybe I forgot the exact size but it was larger than normal) csv file that had to be used to create another csv file for a mass update (millions of system records needed to be modified).  At the time I was a Data Quality Specialist and a former Excel Wizard who was also proficient in MS Access, so I thought it was no sweat.  So I ran the query to get the data and looked at the file.

Then the csv file wouldn't load.  At.  All.

So I googled it.

I then discovered notepad++, but it was an early version (1.x or something) and couldn't handle the file size without crashing.

I then discovered bash, but decided I couldn't learn the proper sed or awk command quick enough to finish the thing before next week.

I then found emacs and vim were options, but it seems they had to be chosen between.  I did not get this and chose to understand why while choosing.

In my former life I had done some software purchasing due diligence.  This means trying out company apps and telling your boss if it sucks or not.  During my stint in due diligence I noticed that most company or organization level apps sucked (it was 2009) and nobody really noticed or cared.  It's a tremendous market opportunity that I should revisit at some point to see if it still exists.  Anyways, I took my experience in software due diligence and put it to use determing which text editor to use.  Using my single requirement to load the large file and do the thing, I set out to experiment upon these two editors (in Windows Xp back in 2009) and decide who the victor would become.

So I downloaded emacs and vim, then I started reading the wikipedia artile dedicated to the flamewar between the two editors(https://en.wikipedia.org/wiki/Editor_war).  I was now amused and even more curious.  Why the fuck does anyone care about a couple of text editors?  Looking over the options between the two I quickly decided on emacs (unicode support or not?  didn't seem like a choice) and started.  And it loaded!  And then I started doing the thing!  And then... that's when emacs crashed.

I was dissappointed, but since I had no skin in the editor wars I really didn't give a fuck.  What do I care if the choice with unicode support and some sort of macro engine that seemed promising didn't work.  I don't give a fuck about any of that.  I just want to do my thing and go home.

I installed gVim and ran the thing.  I expected all text editors to crash at this point.  Vim reminded me of notepad when I started it.  Just a tiny little box that didn't look promising.  As I opened the csv file thinking it might crash already, I was already thinking of how to cut the file into peices and work on the separate parts.  I was not liking the amount of work I had to do for this thing at this point.  Then there was this wierd modal editing in vim that was harder to use than emacs.  The frustration at my workstation was palpable in the back of my mouth.

That's when I loaded the file with vim and ran the thing, and it worked like a fucking beast!  Fuck ya for the old school editor I'd never heard of before today!  However, doing the thing was tricky on vim and it seemed like it shouldn't have been.  Emacs was easy as shit, but vim was tricky.  However, vim did the thing and emacs told me to fuck off.  So I chose vim.

The next week I found I needed bash too, but vim held it's own for the thing at the time and many other things since.

Oh and to describe what the thing was; a tranformation that changed field values and isolated that field value and row id from the entire data table.  I had a regex and wanted to use it to extract the new field values for update on the data directly.  So my requirements for text editors were that they could use regex for replacements, and that they could open a large file.

A grep command would have made my life easier, but would have not given me an interesting introdcution to the wonderful world of modal text editing.  The next week when I learned grep with bash I made that realization.
