# Source @ Coveo
## A technical blog by the fine people at Coveo

See our blog posts at [source.coveo.com](https://source.coveo.com)

This blog uses [Jekyll](http://jekyllrb.com/) and is hosted by [github pages](https://pages.github.com/)

# Create a post

## Quick start (if you know how to use Git and GitHub already)

Fork this repository, and add your blog post on your fork. You'll be able to preview your changes at [youruser.github.io/source.coveo.com](youruser.github.io/source.coveo.com). Note however that if the date in the file name of your post is in the future, you won't be able to see it.

Blogposts in Jekyll are written in markdown. The posts themselves are under `_posts`, and the images are under `images`.

Posts expect a [front-matter](http://jekyllrb.com/docs/frontmatter/). We ask that you minimally add:
  * A title for your blog post
  * Your name
  * Your role within Coveo (in bio)
  * A picture of you

Tags are not mandatory, but can be helpful. You can also add your Twitter handle to your discretion.

Here is a sample front matter:

```markdown
---
layout: post

title: "Integrating Coveo with Jekyll"

tags: [JavaScript Search Framework, Jekyll, Coveo integration]

author:
  name: Harry Potter
  bio: Software Developer
  twitter: coveo
  image: hpotter.jpg

---
```

The file name of your posts need to be prefixed by the date your post is meant to be published on (e.g., `2021-10-05-mypost.md` would be for October 5th, 2021).

You should also add a `<!-- more -->` tag towards the beginning of your post, typically after the first paragraph. Everything before that tag will be used to create the post preview on (source.coveo.com)[https://source.coveo.com/], before the `Read more...` link.

To preview your post locally, you can install [Ruby and Jekyll](https://jekyllrb.com/docs/), and run the `bundle exec jekyll serve` command from your folder. The site will be available on your [localhost:4000](http://localhost:4000). Alternatively, with docker you can host a local Jekyll server using `docker run --volume=$(pwd):/srv/jekyll -p 4000:4000 jekyll/jekyll jekyll server` from the root of your repository. Note that if the date in the file name of your post is in the future, you won't be able to see it.

## Detailed Steps

To properly create a blog post, you'll need a [GitHub account](https://github.com/join), as well as [git](https://git-scm.com/downloads) on your computer.

1. Using your GitHub account, [fork this repository](https://github.com/Coveo/source.coveo.com/fork). This creates a copy of this repository on your account at [https://github.com/youruser/source.coveo.com](https://github.com/youruser/source.coveo.com).
2. On your forked repository, use git to clone it on your computer. For this, open a command line tool (like Terminal on Mac or cmd on Windows) on your computer, and run `git clone https://github.com/youruser/source.coveo.com.git`, changing `youruser` with your own username. Running this creates files in the folder your terminal is open to, so make sure you first get the terminal where you want your files to be in.
3. Open your newly created folder using your favourite code editor. If you're new, we recommend using [VS Code](https://code.visualstudio.com/), which is free, full featured (for what you'll need), and relatively easy to use.
4. In the `_posts` folder, create a new markdown file, prefixed by the date you want to publish your post on (e.g., `2021-10-05-mypost.md` would be for October 5th, 2021). You might alternatively want to duplicate an existing post instead and rename the file, to get a better idea of the markdown syntax.
5. Blogposts in Jekyll are written in [markdown](https://www.markdownguide.org/). Posts expect a [front-matter](http://jekyllrb.com/docs/frontmatter/). We ask that you minimally add:
  * A title for your blog post
  * Your name
  * Your role within Coveo (in bio)
  * A picture of you (to add in the `images` folder)
  Tags are not mandatory, but can be helpful. You can also add your Twitter handle to your discretion.
6. Add a `<!-- more -->` tag towards the beginning of your post, typically after the first paragraph. Everything before that tag will be used to create the post preview on [source.coveo.com](https://source.coveo.com/), before the `Read more...` link.
7. You can preview your post locally by following the documentation on [Jekyll's website](https://jekyllrb.com/docs/), installing Ruby, Jekyll, and running `bundle exec jekyll serve`.
8. Once you feel satisfied with your post, you can push it to your fork. This requires a git commit. If you are new to git, we recommend using the [VS Code git tools](https://code.visualstudio.com/docs/editor/versioncontrol#_commit).
9. Once you have pushed your post to your fork, you can preview your changes at [youruser.github.io/source.coveo.com](youruser.github.io/source.coveo.com).
10. Change and repush any other changes you might want to make.
11. Once you are satisfied with your article, [create a pull request](https://docs.github.com/en/github/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request-from-a-fork) form your fork to the main source.coveo.com repo.

This alerts us in the #technical_blog Slack channel. We will then review your changes, make comments, and eventually approve your request. You can typically expect comments/approval to roll in within the first week.
