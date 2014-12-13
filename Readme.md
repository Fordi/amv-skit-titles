What is this?
=============

This is the output of my work - using [Skitter](https://github.com/Fordi/skitter) - to skit-title [AMV Hell](http://www.amvhell.com/).  

What is skit-titling?
---------------------

AMV Hell and other compilations are comprised of sets of vignettes, skits, or other types of clips.  Skit-titling is therefore, titling those clips so that the viewer has some context.  It's kind of like when a music video shows the song/artist/album in the lower-right corner of the screen.  In fact, it's exactly like that.

How do I use these?
-------------------
First you'll need to download [a copy](https://github.com/Fordi/amv-skit-titles/archive/master.zip).  Github's doing zips of the master branch now, so that's easy.  If you don't know what to do with a .zip file, I don't understand what you're saying.

If you're familiar with [git](http://msysgit.github.com/), you know the drill.

You can also just right-click / save as... the "raw" link next to a file if you only want one.

Once you've got the subs, just place them in the same directory as your copies of [AMV Hell](http://www.amvhell.com/), and open the video using a player that supports ASS files, such as [VLC Media Player](http://www.videolan.org/vlc/index.html).

ASS Files?
----------
ASS is the file extension used for Advanced Substation Alpha - a widely-used subtitling spec that supports basic styling and positioning.  It's actually one of the few that does this consistently, and was for this reason selected for the project.

How did you make these?
-----------------------

1. I deployed [Skitter](https://github.com/Fordi/skitter) on my local machine's [webserver](http://www.wampserver.com/en/)
2. I copied the [AMV Hell](http://www.amvhell.com/) videos into a subfolder of skitter
3. One by one, I configured Skitter to point to an appropriate video, acquired the credits listing page from the AMV Hell site, and built a CSS selector to point to each of the credits.
    * For AMV Hell 1-3 and CE, I had to use [VLC](http://www.videolan.org/vlc/index.html) to convert them to webm format, so that Chrome could play them.
4. I pointed my browser to my local machine, and started creating the ASS file using Skitter's interface.
5. For AMV Hell 0 and /0, I was lucky enough to find someone had already created a skit-log with times.  A quick PHP script translated those into ASS.  They're to-the-second resolution, so they're a little off one way or the other, but frankly, I'm glad to not have to watch them.

Can you do {insert compilation here}?
--------------------------------------------

Totally can.  Requests to [amvhell@codemonkeybryan.com](mailto:amvhell@codemonkeybryan.com).  I'll get to it as free time allows.  New AMV Hells will update on this page.