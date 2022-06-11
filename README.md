scratch-ext.el
==============

scratch-ext.el is extensions for \*scratch\* buffer.

This enables you to dump \*scratch\* buffer automatically
when it is killed or Emacs quits.

In addition,

* killing \*scratch\* becomes simply `(erase-buffer)` it, so you can easily undo.
* after you save \*scratch\* to file by hand, new \*scratch\* buffer is created.


Usage
-----

Add following line to your start up file:

```elisp
(require 'scratch-ext)
```

Log file goes to ~/.scratch directory by default. You can change this
by customizing `scratch-ext-log-directory'.

You can bind a key for `scratch-ext-insert-newest-log` and
`scratch-ext-restore-last-scratch` if you prefer:

```elisp
(global-set-key (kbd "C-c i") 'scratch-ext-insert-newest-log)
(global-set-key (kbd "C-c r") 'scratch-ext-restore-last-scratch)
```

LICENSE
-------

This is licensed under the MIT License.


Author
------

Kouhei Yanagita \<yanagi at shakenbu.org\>
