#Blobs and stuff
An idea I had about parsing blobs.

##Description
When describing a page with text, there are usually lines.  Imagine that
the page or local space is counted into blobs.  Blobs are defined as line
groups or line blocks.  Now let's say that we want to count the different
properties of the blob.  One property might be the number of words.
Another would be the number of lines.  Still another might be the number of
characters, or average character count per line or word.  However, these
are just the metrics that count volume properties within the blob.

Let's count the properties that shape the blob itself.  What is the most
repeated character in the blob boundary lines?  Are there any other
noticable structures to look for in boundary lines?  Is there a noticable
structural boundary to make the blob into modular sub blobs?

Now that we've drawn attention to the boundaries and shape, we can describe
the blob in terms of it's edges.  Referring back to the various blob
metrics as types of volume, let's treat blobs as shapes which connect edges
over metrics instead of planes over volume.  In this way we can integrate
along the shapes made by multiple properties to evaluate the metric types
formed from the edge plane connections.

Looking at the blob as a shape, how are the edges formed?  What splits the
lines into a separate blob from below or above?  How do these splits or
edges affect the internal properties of the blob?  Also, what shape does te
metric take?  Is it mostly a numerical blob, focused on calculations or is
is part of a text paragraph in conversational nartural language?  How is
the metric describing the content in the blob volume?

The purpose of all this is to create a functional space that converts blob
shapes into text parsing notation.  With this notation I can then map out
algorithms along string forms without having to expand them into a single
line or hold them to a single type.  I've been finding that the basics for
the words and stuff are good, but grabbing and exporting anything in the
blob size is a freakin chore without hogging memory or wasting chunks of
unstable cpu time.  Probably the language.  Should try out HoTT.

##Roadmap
This thing is going to be a project
