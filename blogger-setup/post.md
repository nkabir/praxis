## Blogger Setup for Markdown

This blog is now hosted on GitHub: 

    https://github.com/nkabir/praxis

It's a collection of [Markdown](http://daringfireball.net/projects/markdown/) pages along with links to images hosted in a [public Dropbox folder](https://www.dropbox.com/sh/r9qw876n8teix61/ZYDcDxLTn4/praxis). This enables me to edit everything in [vim](http://www.vim.org/)

## Project Layout

The `praxis` project is laid out with a folder per article. Each folder (e.g. `praxis/blogger-setup`) has a file named `post.md` that represents the article. There is a corresponding folder `Dropbox/Public/praxis/blogger-setup` that contains all images associated with the article.

## Conversion to Blogger 

Following instructions from [here](http://notely.blogspot.com/2011/08/how-to-use-markdown-in-blogspot-posts.html), make sure that `Edit HTML Line Breaks` is set to `Use <br /> tags` and that `Compose Settings` is set to `Interpret typed HTML`.

<img src="https://dl.dropbox.com/u/59707331/praxis/blogger-setup/blogger-configuration.png" width="100%" />

The following steps convert Markdown to HTML for Blogger:

    $ pandoc --no-wrap --from=markdown --to=html post.md | xclip


