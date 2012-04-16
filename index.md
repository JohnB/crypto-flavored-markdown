---
title: Crypto-Flavored Markdown
layout: default
---

#Introduction to CFM

CFM is an extension of GFM ([GitHub Flavored](http://github.github.com/github-flavored-markdown/) [Markdown](http://daringfireball.net/projects/markdown/syntax)) that also allows you to specify portions of the document that are encryped, along with the encryption method.

The initially supported tags are Crypto.rot(n=13) and Crypto.substitution(style=:morse). Eventually, I could see adding Crypto.rsa for public-key encrypting a section of text.

Differences from traditional Markdown
-------------------------------------

### Syntax highlighting

Each supported encryption is a "language block" defining what should happen in the block

    ```rot(13)
    This text will be encrypted for reading but plaintext when editing
    ```


