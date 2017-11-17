---
title: "Context Free Art"
date: 2017-11-02T11:24:15+01:00
draft: false
categories: ["note"]
tags: ["visual", "generative"]
---

[Context Free Art](https://www.contextfreeart.org/) is program that generate graphics from instruction called grammar.

> The program follows the instructions in a few seconds to create images that can contain millions of shapes.

Context Free is useful program for people interested in generative art. Unfortunately it's little known.

## Linux usage

There is no GUI for Linux, but there is command line program - *cfdg*. Some useful commands:

``` sh
# generate image
# -s size
cfdg -s 1600x900 script.cfdg -o walpaper.png

# pipe directly into feh
cfdg -s 512 script.cfdg | feh -

# generat animation as png frames
# -a ammount of frames or TIMExFPS
cfdg -s 1024 -a 256 script.cfdg -o some_dir/frm%f.png

```


## Links

- [website](https://www.contextfreeart.org/)
- [documentation](https://github.com/MtnViewJohn/context-free/wiki)
- [gallery](https://www.contextfreeart.org/gallery2/#popular/0/48) of user's works

## Some of my works

{{< ig "/images/cfdg1.png" "" >}}

<!-- {{< ig "/images/MVXIBFy.png" "" >}} -->

{{< ig "/images/cfdg5.png" "" >}}

{{< ig "/images/cfdg3.png" "" >}}

{{< ig "/images/cfdg4.png" "" >}}

{{< ig "/images/cfdg2.png" "" >}}

<!-- {{< ig "/images/Jg2QFC8.png" "" >}} -->

<!-- {{< ig "/images/96t5VQB.png" "" >}} -->
