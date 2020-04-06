<!DOCTYPE html>
<html>
  <head>
    <title>Window Maker: Documentation</title>
    <meta charset="utf-8">
    <link rel="stylesheet" href="/style.css" media="screen">
    <meta name="HandheldFriendly" content="True">
    <meta name="MobileOptimized" content="320">
    <meta name="viewport"
      content="width=device-width, minimumscale=1.0, maximum-scale=1.0">
  </head>
  <body>
    <div id="wrapper">
      <header>
        <h1>
          <a href="/">
            <span class="first">Window</span><span class="second">Maker</span>
          </a>
        </h1>
      </header>
      <aside>
        <nav class="menu">
          <ul>
            <li id="dock">
            <a href="#"></a>
            </li>
            <li id="home" title="Home">
              <a href="/">Home</a>
            </li>
            <li id="news" title="News">
              <a href="/news">News</a>
            </li>
            <li id="docs" title="Documentation">
              <a href="/docs">Documentation</a>
            </li>
            <li id="mail" title="Mailing lists">
              <a href="/lists">Mailing</a>
            </li>
            <li id="devel" title="Development">
              <a href="/dev">Development</a>
            </li>
            <li id="screenshots" title="Screenshots">
              <a href="/screenshots">Screenshots</a>
            </li>
            <li id="themes" title="Themes">
              <a href="/themes">Themes</a>
            </li>
            <li id="links" title="Links">
              <a href="/links">Links</a>
            </li>
          </ul>
        </nav>
      </aside>
      <article>
        Installation Basics
===================

Downloading and Extracting
--------------------------

The first necessary step is to `download
<http://windowmaker.org/pub/source/release/WindowMaker-0.95.5.tar.gz>`_ the
Window Maker source distribution. From this point on, we'll assume it has been
retrieved and is residing on the local hard disk. The next step is to extract
it, and change into the source directory.

.. code:: console
   :class: highlight

   # cd /path/to/your/download
   # gunzip WindowMaker-0.xx.xx.tar.gz
   # tar -xf WindowMaker-0.xx.xx.tar
   # cd WindowMaker-0.xx.xx

Now that things are extracted, it's time to look at the relevant pieces of
documentation. Most UNIX oriented free software packages come with a README
file, and Window Maker is no exception. The README file contains a summary
overview of what the distribution is, what the various directories contain, and
other general information.

Moving along, we have the NEWS file. For now, we just want to point out its
existence. It will become more useful to novice users over time. Veteran Window
Maker users will find it handy for keeping their configuration files up to
date, and learning about various changes which affect Window Maker's behavior.

The two remaining files we need to look at are INSTALL and BUGS. The INSTALL
file provides additional information that is necessary to install Window Maker
successfully. The BUGS file contains a list of known Window Maker bugs. If a
user feels they've found a bug in Window Maker, they should consult the BUGS
file first. If the bug isn't listed, proceed to the Bug Tracker and see if its
there.

Compiling
---------

After extracting the latest version of Window Maker using the previous
instructions, the next step is to compile it.  First of all, the configure
script should be run. It will test to make sure all the necessary libraries,
compilers and build tools are available on the local system. The configure
script allows for various arguments to be passed to it which relate to Window
Maker's installation. For a complete list of all configurable settings, enter:

.. code:: console
   :class: highlight

   $ ./configure --help

Commonly used configuration options are:

.. code:: console
   :class: highlight

   --prefix=DIR --enable-modelock --enable-xinerama --enable-silent-rules

The first configuration option lets Window Maker be installed into a
non-default installation directory (e.g if Window Maker cannot be installed
system wide for some reason, a user can specify a path under his/her home
directory).  The default installation directory is /usr/local/bin. Note that
root access will be needed later on during the installation process if the
defaults were used.

So if a user johndoe would like to install the wmaker binary into
/home/johndoe/wmaker/bin instead of the default /usr/local/bin, the following
argument would be passed to the configure script:

.. code:: console
   :class: highlight

   $ ./configure --prefix=/home/johndoe/wmaker

After the configure script has been successfully executed, Window Maker can now
be compiled with the make command; simply enter:

.. code:: console
   :class: highlight

   $ make

The final step is to install the binaries and other support files. This is
accomplished by entering:

.. code:: console
   :class: highlight

   # make install

Note that this is the step that needs to be performed by root if the default
installation directory was used, or if a directory was specified that the
running user cannot write to. If the installing user has root access, they
should first become root by issuing ``su - root``. Otherwise, reconfigure and
recompile Window Maker by specifying a different installation directory, or
kindly ask the local system administator to install it system wide.

Once Window Maker is installed system-wide, a default configuration can be
installed on a per-user basis, through the bundled installation script,
``wmaker.inst``. Enter ``wmaker.inst`` in a terminal emulator to configure
Window Maker for your user.

This script copies the default Window Maker configuration to your user's home
directory and sets Window Maker as the default window manager. It is
recommended to create ``~/GNUstep`` before executing the script.

Final tweaks
------------

Edit your ~/.xinitrc to load your newly installed Window Maker using the line
``exec /usr/local/bin/wmaker``.

Generate a new root menu (accessible with F12) with ``wmgenmenu``, for example

.. code:: console
   :class: highlight

   $ wmgenmenu > $HOME/GNUstep/Defaults/WMRootMenu

Another recommended step is to install a few dockapps like wmvolman, wmmixer
and wmsystemtray which allow one to easily mount external media on /media among
other things. Visit `dockapps <http://www.dockapps.net>`_ for many more
choices.

      </article>
      <div id="titlebar">
        <div id="minimize"></div>
        <div id="titlebar-inner">Window Maker: Documentation</div>
        <div id="close"></div>
      </div>
      <div id="resizebar">
        <div id="resizel"></div>
        <div id="resizebar-inner">
        </div>
        <div id="resizer"></div>
      </div>
    </div>
  </body>
</html>
