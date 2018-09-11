coloremoji.sty
==============
Style package for directly including color emojis in latex documents

Installation

    mkdir -p ~/Library/texmf/tex/latex/local
    cd ~/Library/texmf/tex/latex/local
    git clone git@github.com:alecjacobson/coloremoji.sty.git
    texhash coloremoji.sty

[Related blog entry](http://www.alecjacobson.com/weblog/?p=4018)

## Examples

The following LaTeX code:

    \documentclass{article}
    \usepackage{coloremoji}
    \begin{document}
    Hello, 🌎.
    \end{document}

produces something like:

![Hello, world.](http://alecjacobson.com/weblog/media/hello-world-emoji.png)

You can even use emojis in math. The following LaTeX code:

    \[
    🐊^{🐊^{🐊}} = ∫_{🎃} 🙊 \ d🍀
    \]

produces something like:

![Emojis in math
mode.](http://alecjacobson.com/weblog/media/alligator-power-integral-jack-o-lantern.png)

## Image source for this version

This style sheet creates a PDF where each emoji is an embedded image
(rather than a character). The images are Twitter Emoji, copyright Twitter, Inc. - v2.3.1 2017-10-31. Twitter Emoji are available under the Creative Commons Attribution 4.0 license, and were obtained from https://github.com/iamcal/emoji-data. This is a change from Alec Jacobson's original style package, which used the Apple Color Emoji typeface.

## Known issues

The emoji_images directory contains over 2600 Twitter emoji, but fewer than 900 of these are currently defined in the style package. 

The encoding of the `.tex` must support emoji's, that is unicode characters. So switch your encoding to something like UTF-8.
