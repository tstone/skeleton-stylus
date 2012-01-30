
skeleton-stylus
---------------

A port of "Skeleton" into the Stylus language.  Free to use under the MIT license.  http://www.opensource.org/licenses/mit-license.php


Why
----

Skeleton (http://www.getskeleton.com) is a nicely designed responsive CSS framework.
It requires, however, the HTML to be altered in order to make sure of it.

    // index.html
    <div class="column eight sidebar"></div>

Chances are you already have a class or ID on the element (like ".sidebar").  Using
Stylus, the Skeleton classes can be mixed into the classes you already have setup,
or mixed into HTML5 tags.

    // style.styl
    .sidebar
        skeleton-columns(8)

    // index.html
    <div class="sidebar"></div>

This allows you to integrate Skeleton without ever needing to touch the site's HTML.

Base tags could also be globally extended.

    // style.styl
    body > aside
        skeleton-columns(5)

    // index.html
    <aside></aside>


Usage
-----

skeleton-stylus should be considered in "alpha" mode.  It hasn't yet been fully tested.
Additionally, skeleton-stylus makes use of Stylus bug fix #554 (https://github.com/LearnBoost/stylus/pull/554)
which at the time of writing (2/2/2012) wasn't yet part of Stylus.


Installation
------------

    git clone git://github.com/tsotne/skeleton-stylus.git
    cd skeleton-stylus
    mv skeleton.styl ~/path/to/your/project/public/css/skeleton.styl

Then in your main .styl file

    @import 'skeleton'


Functions
----------------

    skeleton-alpha
    skeleton-alphaomega
    skeleton-clearfix
    skeleton-container
    skeleton-offset(#)
    skeleton-column(#)
    skeleton-columns(#)
    skeleton-omega
