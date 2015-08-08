# emscripten-KJPBS

This repository serves as a checkout point for the Emscripten and Emscripten-Qt pieces needed to successfully build King James Pure Bible Search (KJPBS) for Emscripten.  This was done because not every combination of those repositories works for building KJPBS.  In fact, when I was first porting KJPBS to Emscripten, I went through over 30 different release versions of Emscripten before finding one that would actually work.

That was 1-1/2 years ago and Emscripten itself has gotten a lot of work since then and will likely work better now with Emscripten-Qt in general, but at least having a known working starting point will hopefully make your life easier.

Rather than manually pulling the 'emscripten' and 'emscripten-qt' repositories, you should clone this 'emscripten-KJPBS' repository and pass the '--recursive' option to 'git clone' or do a 'git submodule init' and 'git submodule update' after you have cloned the repository.

If you are looking to build KJPBS for any other platform other than Emscripten (such as for Windows, Linux, Mac, Android, iOS, embedded-Linux, etc), you do not need this repository or any of the Emscripten pieces at all.  That's why this repository was kept completely separate from the main 'KingJamesPureBibleSearch' repository.

If you wish to try a compiled version of KJPBS for Emscripten, visit the [PureBibleSearch.com Online](http://www.purebiblesearch.com/online/) page to launch it.  Note that KJPBS is an ultra-heavy target for Emscripten and many browsers struggle with loading it.  I've had the best luck with Firefox, but even it will occasionally give 'script is busy' warnings, with which you can safely select 'continue' until it loads.  Other browsers tend to either not be compatible at all (such as older versions of IE) or timeout completely, as I've seen on newer versions of Chrome (though older versions worked fine).  There should be settings buried somewhere deep in the browser to let you control those things.

And while you are at [PureBibleSearch.com Online](http://www.purebiblesearch.com/online/), if the Emscripten version isn't working well in your browser, then try the VNC Embedded-Linux target if you are looking at using KJPBS online in your browser.  In all honesty, "emscripten-KJPBS" is more of a novelty for computer nerds who are enamored by the fact that a C++ application can be cross-compiled to javascript than it is a useful target of KJPBS.
