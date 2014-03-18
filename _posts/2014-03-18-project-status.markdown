---
layout: post
title:  "Project status"
date:   2014-03-18 20:10:38
categories:
---

## Our projects

We now have quite a few projects in the [vim-erlang organization][vim-erlang]:

- [vim-erlang-runtime][vim-erlang-runtime] is the Erlang syntax and indentation
  built into Vim.
- [vim-erlang-compiler][vim-erlang-compiler] is an Erlang syntax checking and
  compiler plugin for Vim. It can perform on-the-fly syntax checks (utilising
  signs) and gives Erlang support to the `:make` command.
- [vim-erlang-omnicomplete][vim-erlang-omnicomplete] is an Erlang autocomplete
  plugin which gives Erlang support to the `i_CTRL-X_CTRL-O` keystroke.
- [vim-erlang-tags][vim-erlang-tags] is Erlang ctags-file generator plugin which
  makes Vim able to jump to definitions of functions, records, etc. by using the
  `CTRL-]`, `:tags`, and other commands.

## Installing all projects

1. Install the Vim plugin called [pathogen][pathogen], which helps installing
   further plugins.

2. Clone all repositories:

{% highlight bash %}
cd ~/.vim/bundle
git clone git@github.com:vim-erlang/vim-erlang-runtime.git
git clone git@github.com:vim-erlang/vim-erlang-compiler.git
git clone git@github.com:vim-erlang/vim-erlang-omnicomplete.git
git clone git@github.com:vim-erlang/vim-erlang-tags.git
{% endhighlight %}

3. Generate help files:

{% highlight vim %}
:Helptags
{% endhighlight %}

Help pages are available via the `:help` command, e.g. `:help
vim-erlang-compiler`.

[vim-erlang]: https://github.com/vim-erlang
[vim-erlang-runtime]: https://github.com/vim-erlang/vim-erlang-runtime
[vim-erlang-compiler]: https://github.com/vim-erlang/vim-erlang-compiler
[vim-erlang-omnicomplete]: https://github.com/vim-erlang/vim-erlang-omnicomplete
[vim-erlang-tags]: https://github.com/vim-erlang/vim-erlang-tags
[pathogen]: https://github.com/tpope/vim-pathogen#installation
