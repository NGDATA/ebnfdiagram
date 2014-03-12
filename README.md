# EBNF-Diagram

jQuery plugin that plots syntax diagrams (aka railroad diagrams) out of a formal syntax description.

# Building

There is no real automated build in place, sorry for that. What you need to do is:

0. Get a js interpreter you can operate from the command line.

We recommend rhino, the more interesting platforms have it on board or at least in the package repositories.

1. Build the parser

    ./build.sh

# Testing

Just point your browser to src/test/webenv/test.html.

Add some syntax in the textarea and push the buttons.

TODO: we think about providing some qunit testing. 

# Documentation

The code itself is currently your best source of documentation. 
Given the total size of the project source it might be hard to make a more condense variant :)

The default browser-testpage (see above) shows the diagram of the syntax the rendition expects as input.

Nevertheless, some extra simple usage documents might be wise about:
 * howto customize the vizuals
 * howto integrate its use on your own pages

Also: 
  * the src/desgin folder contains a scan of sketches that help explain how some of the internal drawing stuff is happening.
  * js/cc and jQuery provide more docs that might come around handy. Check the file CREDITS for pointers.

# Future Work

Next to the things you already thought of yourself, here is a short list of things to be added:
 * better build framework - and make it cross platform 
 * better jQuery usage: 
   * provide some automatic way to have pre/@class="ebnf" elements replaced with the diagram canvas
 * add support for the html5 impaired (ie) through explorercanvas (http://code.google.com/p/explorercanvas/)
