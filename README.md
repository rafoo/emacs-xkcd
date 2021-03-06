emacs-xkcd
==========

[![Build Status](https://travis-ci.org/vibhavp/emacs-xkcd.png?branch=master)](https://travis-ci.org/vibhavp/emacs-xkcd)

Implementation of an xkcd (http://xkcd.com/) reader for Emacs.

#Installation

## Via package.el (Melpa)
emacs-xkcd is now available on [Melpa](http://melpa.milkbox.net). If you have added Melpa as a repository, the package can be installed by a simple `M-x package-install xkcd`.

## Via Github
Clone this repository to a desired location, and add the following snippet to your .emacs:
```lisp
(add-to-list 'load-path (expand-file-name "/path/to/emacs-xkcd.el"))
(require 'xkcd)
```
#Screenshot:
![alt text][screen]
[screen]: http://i.imgur.com/x08oyQm.png "Screenshot of emacs-xkcd"
#Loading up comics:
`xkcd-get` loads up a user-specified comic.

Files are cached by default to ~/.emacs.d/xkcd/. This can be changed by changing `xkcd-cache-dir` in the group "xkcd". (customize-group xkcd)

`xkcd` loads up the latest xkcd.
# Current keybindings:
| Keybinding | Use                            |  Function      |
|:----------:|:------------------------------:|:--------------:|
| `r`        | Load a random xkcd             | (xkcd-rand)    |
| `t`        | Show alt-text in the minibuffer| (xkcd-alt-text)|
| `<right>`  | Load next xkcd                 | (xkcd-next)    |
| `<left>`   | Load previous xkcd             | (xkcd-prev)    |

#TODO
Add support for custom faces.
