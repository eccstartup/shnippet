# Shnippet

## About

**Shnippet** is a collection of
[YASnippet](https://github.com/capitaomorte/yasnippet)
[Haskell](http://haskell.org/) snippets for Emacs.

## Usage

Clone repository:

    $ cd ~/.emacs.d/snippets

    $ git clone https://github.com/LukeHoersten/shnippet
    OR
    $ hg clone https://bitbucket.org/LukeHoersten/shnippet

Add the cloned repository to YASnippet's `yas-snippet-dirs`:

    (setq yas-snippet-dirs
          '("~/.emacs.d/snippets/shnippet"
            "/other/paths/"
            ))

Snippets may have to be recompiled and reloaded in Emacs if YASnippet
is already in use:

    M-x yas-recompile-all
    M-x yas-reload-all


The Haskell snippts should now be available to use! Try typing
`fn<TAB>` in an Emacs Haskell buffer to test.

## Notes

I **highly** recommend using YASnippet with
[ido-mode](http://www.emacswiki.org/emacs/InteractivelyDoThings). Configure
Emacs:

    (setq-default yas-prompt-functions '(yas-ido-prompt yas-dropdown-prompt))

This is important so that alternatives (like `import` vs. `import
qualified`) can quickly be selected with a single key stroke.

## Authors

This code is written and maintained by Luke Hoersten,
<luke@hoersten.org>.
