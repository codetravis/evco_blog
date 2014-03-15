#Read the Source

I have read and heard this quite a bit in my short time as a programmer.  It really hit me today as I was working on a little project that incorporated the useful little [Chartjs](http://www.chartjs.org) library.

This was my first time using this library and usually when using something for the first time I try to follow a tutorial or two to get familiar with it a little bit.  The tutorial/documentation on this website was a little limited and I couldn't see where I needed to add the change I wanted to make. I was making a little line chart for two different sets of numbers and wanted to remove the dots that appeared for each datapoint, but I could not see how.

The documentation showed that there were some line defaults and one of those defaults was <code>pointDot</code> which was set to true.  What it did not show was how to change it to false.  I tried a couple of different guesses but they didn't work.

## An Epitome
I remembered at this point that I had full access to see how the code worked (it is an open source project).  It couldn't hurt to understand how this thing worked by looking at its guts.

It was not hard to find the answer to my question once I found the function I was caling. An optional parameter was passed that could containg the list of changes to the default options.  A few seconds later I had a beautiful line chart without any little dots on it.

## The Takeaway
It's usually more beneficial to answer your questions by really getting into the code that you are using than to try to find the answer on a forum somewhere.  Not to say forums are a bad way to go, sometimes you need an explanation from someone else who has been there before. In general though, you should probably start by taking a peek into the source so you can understand what is going on.
