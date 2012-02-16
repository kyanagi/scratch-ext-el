scratch-ext.el
==============

scratch-ext.el is extensions for \*scratch\* buffer.

This enables you to dump \*scratch\* buffer automatically
when it is killed or Emacs quits.

In addition,

* killing \*scratch\* becomes simply (erase-buffer) it, so you can easily undo.
* after you save \*scratch\* to file by hand, new \*scratch\* buffer is created.


Usage
-----

Add following line to your start up file:

    (require 'scratch-ext)

Log file goes to ~/.scratch directory by default. You can change this
by customizing `scratch-ext-log-file-format'.


LICENSE
-------

This is licensed under the MIT License.


Author
------

Kouhei Yanagita \<yanagi at shakenbu.org\>
