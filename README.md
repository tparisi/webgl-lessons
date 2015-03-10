------------------------------------------------------------------
The official maintained repository for this project is now
https://github.com/tparisi/webgl-lessons -- please fork from 
and send pull requests to there rather than here.
------------------------------------------------------------------


Some lessons in WebGL
---------------------

This repository contains a series of simple lessons in WebGL, plus some
related examples.

The folders named lesson01, lesson02, and so on are a sequential tutorial and
are best understood using the explanatory text at:

    <http://learningwebgl.com/lessons/>

The form of the first ten lessons is *very* loosely based on NeHe Productions'
well-known OpenGL tutorial, which can be found here:

    <http://nehe.gamedev.net/>

The lessons from 11 onwards are not related to the NeHe ones.

The folders named example01 etc are example code for interesting stuff outside
the scope of the tutorial, and have their own README.txt files with details.


Problems seeing the lessons?
----------------------------

When experimenting with the lessons later than #5 you may encounter errors
resulting from "cross-origin" file access.  This is caused by the browsers'
security systems:

 * Browsers want to stop pages from one server ("origin") from gaining access
   to data from another origin except under closely-controlled circumstances.
   (For example, imagine if a hostile website tried to gain access to data
   from the online banking window you had open in another tab.)
 * Unfortunately, when files are loaded from the filesystem, the browser sees
   each file as a separate origin.  So when one of these examples tries to
   load, say, a texture to display on a cube, it will fail.

There are two ways you can work around this.  The best, safest way is to use
a local webserver, but an alternative if you're careful about it is to
temporarily disable the cross-origin restrictions. Here are [instructions for running things locally](https://github.com/mrdoob/three.js/wiki/How-to-run-things-locally).
