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
        Documentation
=============

It's a fact that one of the biggest problems with today's software is lack of
good documentation, or any documentation for that matter. Programmers generally
don't have a lot of time to document their work, and the things they do
document are usually oriented towards other programmers. While we can
appreciate the programmers point of view, we feel it's necessary to cater to a
larger audience (i.e our users) by providing clear, concise information on how
to use our software. The sections below will bring all of these pieces of
information together for you.

Before you get started with Window Maker, you need to have an understanding of
how to make use of the documentation that comes with the source distribution.
The main objective to using documentation is to **understand** it, which
coincidentally requires that you **read** it. A common mistake is for new or
novice users to overlook this information, leading them to frustration and a
bad first impression. Please take a moment to peruse the sections below, which
should make the experience of learning Window Maker a more pleasant one.

.. class:: contents

- `Installation Basics <installation.html>`_
- `Window Maker Compilation and Installation <wmaker_install.html>`_
- `Window Maker Internationalisation <wmaker_i18n.html>`_
- `Guided Tour <guidedtour/index.html>`_
- `User Guide <guide_toc.html>`_
- `FAQ <FAQ.html>`_
- `WINGs <wings.html>`_

.. - `Desktop/X Integration <desktop.php>`_

Very frequently asked question
------------------------------

- **Can I easily mount my external drives or connect to the internet with
  Window Maker?**

  Yes, you can. Mounting external media is not the problem of a window manager
  to solve, but a tipical Window Maker user can mount external media just as
  easily as any other desktop user.  If you use a dockapp like
  `wmvolman <https://github.com/raorn/wmvolman>`_ or
  `wmudmount <http://sourceforge.net/projects/wmudmount>`_ you are just a
  click away from having your external media mounted on `/media/VOLUME_LABEL`.

  And you can just as easily manage your network connections using the standard
  `nm-applet` running in a system tray like `wmsystemtray
  <http://sourceforge.net/projects/wmsystemtray>`_ on your dock.

  .. figure:: /img/essential_dockapps.png
     :alt: essential dockapps

     wmvolman and wmsystemtray with nm-applet

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
