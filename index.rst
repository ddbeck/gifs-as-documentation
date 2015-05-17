*********************
GIFs as Documentation
*********************

This is a short guide to using GIFs *in* documentation and *as* documentation.
Animated GIFs are a great tool for making documentation, but it takes some special care and attention to make them work.

This guide was started on May 16, 2015 by Daniel D. Beck on his flight to Portland, Oregon
en route to attend the Write the Docs conference.
Your contributions to this guide are welcome!
If you have a suggestion to improve this guide, please `open an issue on GitHub`__ or `tweet @ddbeck`__.

.. __: https://www.github.org/ddbeck/gifs-as-documentation/issues
.. __: https://twitter.com/ddbeck

.. note::

   This guide will use "animated GIF" and "GIF" interchangeably.
   GIFs aren't necessarily animated, but this guide is only considering GIFs that are animated.


Why GIFs?
=========

.. figure:: tumblr.gif

   As Tumblr knows, GIFs are a lot of fun.

Despite "animated GIF" conjuring up something frivolous, animation in general has a long history of being used to
to do everything from `telling fairy tales`__ to helping people understand `complicated technical subjects`__.
GIFs, as a specific form of short animation, have many strengths that make them a good tool for technical communicators:

.. __: http://en.wikipedia.org/wiki/Snow_White_and_the_Seven_Dwarfs_(1937_film)
.. __: https://www.youtube.com/watch?v=aW5ozq4Tqew

* GIFs are much easier to make than high definition video.
  GIFs have lower audience expectations, because GIFs are silent and often grainy, short, and low-resolution.
  A series of animated GIFs can be made at lower cost than making a full-length video.

* GIFs can be used for numerous contexts.
  GIFs can instruct users, illustrate problems for customer support, or mockup a new idea for the design process.

* GIFs support content reuse.
  A GIF made for documentation can be reused in marketing or support contexts (and vice-versa).

* Animated GIFs do not have the negative associations of auto-playing video (because they're intrinsically silent).
  With a GIF, you can get away with showing something to a viewer that they might not otherwise have been receptive to.

* Compared to traditional web video, GIFs are relatively frictionless from the perspective of your audience.
  Unlike a YouTube video, there's no need to click play, because browsers automatically load and run GIFs.
  GIFs are natively supported by effectively all browsers, unlike many video formats and players,
  so your audience doesn't need to install a plugin to see it.

* Compared to a sequence of still images, GIFs are less cognitively demanding.
  Your viewer doesn't have to mentally interpolate frames between still images, because the frames actually exist.
  For example, trying to follow step-by-step drawings of how to tie a knot can be much more challenging than watching
  an animated equivalent.

* GIFs can be embedded pretty much anywhere and be reasonably expected to work.
  So you can use a GIF in a technical document just as easily as in a tweet or an email.

* GIFs can be used as prototypes or storyboards for full-scale video production.
  You can use GIFs to make a proof-of-concept for a video or as part of the script writing process.

* Finally, GIFs are fun.
  They can add a dash of excitement, action, or texture that static text and graphics can't.

Of course, GIFs aren't ideal for every situation.
At least for the time being, they're useless in print media.
And for many applications and audiences, they cannot replace traditional video or well-placed still images.
But with judicious use, you may find that animated GIFs complement your existing documentation tools and skills.



Guidelines for Using GIFs
=========================

If you're convinced to give GIFs a try, don't just start littering your docs with memes and scrolling text.
Consider these guidelines for using GIFs:

* GIFs should be **supplementary to** other kinds of documentation
  or be **supplemented by** other kinds of documentation.
  GIFs are rarely a substitute for writing things down.
  Also remember that members of your audience may have reduced vision or blindness.
  An over-dependence on GIFs and video poses serious accessibility problems.
  Screen readers can't read images (yet) and it can be difficult to write meaningful alt text for animations.

* GIFs should be used sparingly.
  Many animations visible on screen can be distracting or confusing, especially if they're mixed with other text.
  Too much visual noise from competing animations can hinder your audience's ability to appreciate anything on screen.

* GIFs should be small.
  GIF isn't an efficient image format and GIFs don't load particularly gracefully, so keep your file sizes in check.
  If overused, GIFs can cause your page size to balloon out of control,
  to the point that your audience may give up and leave your documentation rather than waiting on your page to load.

* GIFs should be short.
  If you can't quickly tell where in the action the animation is (i.e. beginning, middle, or end),
  it's hard to learn anything from the animation.
  You can get away with longer animations if you add some kind of signposting
  (e.g., numbered steps, a time stamp, or a pause at the beginning of the sequence),
  but at some point the lack of playback control (e.g., play, pause, and rewind) proves too frustrating,
  even if the GIF's file size doesn't catch up with you first.



Kinds of GIFs
=============

I've identified or conceived of a few ways GIFs may be used in documentation and as documentation:
decorative, demonstrative, familiarizing, instructional, and narrative.
This is probably not comprehensive, but it might help you get started.


Decorative
----------

Decorative GIFs that don't add anything to the subject matter of the documentation per se,
but serve to connect you and your audience through shared cultural touchstones, jokes, and enthusiasm.
This is by far the most common way GIFs are used in documentation, but they're rarely ever used *as* documentation
(except in this document, go figure).

**Patterns:**

* Success or failure intensifiers
* In-jokes
* Memes

**Examples:**

.. figure:: riker_deal_with_it.gif

   "Deal With It" featuring Commander Riker

.. figure:: ron_paul_happening.gif

   "It's happening!" featuring American politician Ron Paul



Demonstrative
-------------

Demonstrative GIFs show what something is or what it does,
but without the expectation that the viewer is meant to be able to reproduce the demonstration themselves.
This is the most common kind of GIF as documentation that I've seen.

**Patterns:**

*  Showing the behavior of the end result of a process that your documentation teaches.
*  Showing a 360-degree walk around of a product

**Examples:**

*  The documentation for a Python library I wrote, `Oraide`__, shows how the library simulates someone typing text.
   The GIF doesn't show the the interface to produce the results, just the result.
   The GIF alone provides insufficient information for the viewer to do the same.

   .. __: http://oraide.rtfd.org/

   .. figure:: oraide.gif

      Oraide's simulated typing demo GIF

*  The Node.js library `blessed`__ provides an interface for
   generating a graphical user interface (GUI) similar to `curses`__.
   Their README contains a long animated GIF that shows what the library produces (that is to say, the GUI),
   but not the code to produce the interface.
   There's no way that a viewer could produce the same results themselves by watching the GIF alone,
   but it does show what the library is capable of doing.

   .. __: https://github.com/chjj/blessed#blessed
   .. __: http://en.wikipedia.org/wiki/Curses_%28programming_library%29

   .. figure:: blessed.gif

      `blessed` Node.js library demo GIF.
      Thanks to `Beau Gunderson`__ for this example.

      .. __: https://twitter.com/beaugunderson/status/590677562831024130


Familiarizing
-------------

Acquainting the the viewer with something that they're going to do themselves,
but with the expectation that more detail is forthcoming.

**Patterns:**

*  The preview GIF that shows the performance of complicated task as an introduction to step-by-step instructions
*  The screencast in miniature

**Examples:**

* The `Learn to Crochet`_ tumblog uses a familiarization GIF to introduce a detailed series of instructions.
  It shows a process, but not each of the steps needed to do it (that comes in subsequent parts).

  .. _Learn to Crochet: http://crochet-gifs.tumblr.com/

  .. figure:: crochet_familiar.gif

     *Learn to Crochet*'s familiarization GIF.
     Thanks to Jaime Margalotti for this example.


Instructional
-------------

Instructional GIFs show something that the viewer is meant to do themselves.

**Patterns**:

*  Showing a single step of a task with or without annotations
*  Showing multiple steps of a task with or without annotations
*  The screencast in miniature

**Examples**:

* The `Learn to Crochet`_ tumblog uses GIFs to show how to complete each individual step in crocheting.
  Note its effective use of the pause at the end of the GIF.

  .. figure:: crochet_step.gif

     A *Learn to Crochet* GIF illustrating a single step.
     Thanks to Jaime Margalotti for this example.


Narrative
---------

Narrative GIFs tell a story.
Telling a story with a GIF can connect the thing you're trying to teach your user on a personal level.
Narratives help contextualize your documentation in the world that your audience lives in.

**Patterns**:

*  A before-and-after sequence
*  Warnings or cautions by showing an incorrect action followed by a negative consequence

**Examples**:

.. todo:: I don't actually have an example of this yet, though I do have an idea for doing one myself.


How to Make a GIF
=================

There's generally three ways to make a GIF:

* Record directly to the GIF format
* Record video and convert to GIF
* Convert two or more still images into a GIF animation

This section attempts to suggest tools and other resources for using such


Recording directly to GIF
-------------------------

* `LICEcap`__ captures part of your screen, like other screencasting software, and saves the result as an animated GIF.
  This is quite possibly the easiest way to make an animated GIF,
  though it's only useful for making software-related documentation.

  Platforms: Mac OS X, Windows.

  .. __: http://www.cockos.com/licecap/

.. todo:: Get recommendations for an iOS GIF camera
.. todo:: Test some Android GIF cameras


Converting video to GIF
-----------------------

* `ffmpeg`__ is a command-line tool that can convert existing video formats (e.g., MP4, QuickTime) to GIF,
  with the option to select specific time sequences and other features.
  `This guide`__ (for Mac OS X, but useful for all platforms) illustrates how you might use ffmpeg for making GIFs.

  Platforms: Linux, Mac OS X, Windows

  .. __: https://www.ffmpeg.org
  .. __: https://gist.github.com/dergachev/4627207



Converting still images to GIF
------------------------------

* `ImageMagick`__ is a suite of tools for creating and manipulating images.
  The `animate`__ command can be used to stitch together many individual still images
  (e.g., a series of screenshots or photos) into an animated GIF.
  ImageMagick bindings for many programming languages are also available.

  Platforms: Linux, Mac OS X, Windows

  .. __: http://www.imagemagick.org/script/index.php
  .. __: http://www.imagemagick.org/script/animate.php



Additional resources
====================

Tools
-----

* Gifsicle__ is a useful tool for optimizing GIFs.
  It can significantly reduce your GIF's file size,
  enabling you to use it bandwidth or file-sized constrained contexts like mobile browsers and Twitter.
  (which imposes a somewhat draconian file size limitation).
  It's especially useful in conjuction with other tools that make GIFs,
  because many of them do no optimization of their own.

  .. __: http://www.lcdf.org/gifsicle/

* `Giphy`__ is a search engine for GIFs.
  It's great for finding inspiration and decorative GIFs.

  .. __: http://giphy.com/


Reading
-------

* `Using Animated GIF Images for Library Instruction`__ by Karl Suhr
  examines using GIFs in the context of information literacy and library instruction.

  .. __: http://www.inthelibrarywiththeleadpipe.org/2014/using-animated-gif-images-for-library-instruction/


