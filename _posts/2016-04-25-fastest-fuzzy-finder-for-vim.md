---
layout: post
title: Fastest Fuzzy Finder for Vim / Neovim
date: 2016-04-25 22:37:42.000000000 +05:45
type: post
published: true
status: publish
categories: []
tags: []
meta:
  _edit_last: '1'
  _yoast_wpseo_primary_category: ''
  _yoast_wpseo_focuskw_text_input: fastest fuzzy finder
  _yoast_wpseo_focuskw: fastest fuzzy finder
  _yoast_wpseo_linkdex: '69'
  _oembed_3c361fc64a0e448a1872dbe78a6aedbb: "{{unknown}}"
  dsq_thread_id: '4775817346'
  _wpcom_is_markdown: '1'
  _pingme: '1'
  _encloseme: '1'
---
When I started to use Vim I needed a fast way to go between files by hitting Ctrl+P and typing the file name just like in Sublime Text, Text Mate or any other text editor. Then I found [ctrlp](https://github.com/ctrlpvim/ctrlp.vim) plugin for vim which was ok. The main problem I had with ctrlp was speed. At my full time job I am working with a code base that contains 20,000+ files and it was very frustrating every-time I had to go to a file.  Even the caching did not help much. And some of the time the search result it returned was not matching the file (most probably due to very similar file naming).

After some search for its alternative I came across  [Command-T](https://github.com/wincent/command-t) and it was built for speed (much faster than CtrlP). And the search result was much accurate. I was happy with it for a long time but I had one problem with it as it would not work with  [neovim](https://neovim.io/). But I really wanted to switch to neovim and using CtrlP was out of question for me.

![Command-T](https://raw.githubusercontent.com/wincent/command-t/media/command-t.gif)

Then I found [fzf](https://github.com/junegunn/fzf) which would work in [neovim](https://neovim.io/). It was amazingly faster than [Command-T](https://github.com/wincent/command-t) as well. I heard of this quiet a while ago but did not tried it. This was really a holy experience for me haha, it blew away all fuzzy finder. In Github  page it says "*fzf is a general-purpose command-line fuzzy finder.*" so it can be used from command-line as well. Actually this plugin is rewritten in [Golang](https://golang.org/) which might be the reason of its speed.

![fzf](https://camo.githubusercontent.com/0b07def9e05309281212369b118fcf9b9fc7948e/68747470733a2f2f7261772e6769746875622e636f6d2f6a756e6567756e6e2f692f6d61737465722f667a662e676966)
