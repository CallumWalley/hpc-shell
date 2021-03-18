# Introduction to using the shell in a High-Performance Computing context

This lesson provides an introduction to the bash shell aimed at researchers who
will be using the command line to use remote, high-performance computing (HPC)
systems. The material is also suitable for teaching the use of the shell for
any remote, advanced computing resources.


## Using this material

1. Follow the instructions found in the [Software Carpentry example lesson
   source](https://github.com/carpentries/lesson-example/) to create a
   repository for your lesson.
2. Create any host specific `.yml` files in the directory [_includes](_includes)
3. Create any required host-specific code snippets in the subdirectory
   [_includes/snippets](_includes/snippets). These snippets provide inputs and
   outputs that are host-specific and that are included automatically based on
   the configuration in the `_config.yml` file.
   1. Code snippets are in files named `snippet_name.host_id` and are included
      automatically when the lesson is built. For example, if the
      `snippet_name` was `login_output` and the `host_id` was
      `ComputeCanada_Graham`, then the snippet file would be called
      `login_output.ComputeCanada_Graham`.
   2. Code snippets are placed in subdirectories that are named according to
      the episode they appear in. For example, if the snippet is for episode
      01, then it will be in a subdirectory called `01`.
4. Set the environment variable `HPC_JEKYLL_CONFIG` to a comma delimited list of the localized configs you plan on using from [_includes](_includes), e.g. `siteSpecific.yml,clusterSpecific.yml`. They are ordered in increasing precedence.

## Lesson writing instructions

This is a fast overview of the Software Carpentry lesson template. This won't
cover lesson style or formatting (address that during review?).

For a full guide to the lesson template, see the [Software Carpentry example
lesson](http://swcarpentry.github.io/lesson-example/).

### Lesson structure

Software Carpentry lessons are generally episodic, with one clear concept for
each episode ([example](http://swcarpentry.github.io/r-novice-gapminder/)).

An episode is a markdown file that lives under the `_episodes` folder. Here is
a link to a [markdown
cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)
with most markdown syntax. Additionally, the Software Carpentry lesson template
uses several extra bits of formatting- see here for a [full
guide](http://swcarpentry.github.io/lesson-example/04-formatting/). The most
significant change is the addition of a YAML header that adds metadata (key
questions, lesson teaching times, etc.) and special syntax for code blocks,
exercises, and the like.

Episode names should be prefixed with a number of their section plus the number
of their episode within that section. This is important because the Software
Carpentry lesson template will auto-post our lessons in the order that they
would sort in. As long as your lesson sorts into the correct order, it will
appear in the correct order on the website.

### Publishing changes to GitHub + the GitHub pages website

The lesson website is viewable at <https://hpc-carpentry.github.io/hpc-shell/>.

The lesson website itself is auto-generated from the `gh-pages` branch of this
repository. GitHub pages will rebuild the website as soon as you push to the
GitHub `gh-pages` branch. Because of this `gh-pages` is considered the "master"
branch.

### Previewing changes locally

Obviously having to push to GitHub every time you want to view your changes to
the website isn't very convenient. To preview the lesson locally, run `make
serve`. You can then view the website at `localhost:4000` in your browser.
Pages will be automatically regenerated every time you write to them.

Note that the autogenerated website lives under the `_site` directory (and
doesn't get pushed to GitHub).

This process requires Ruby, Make, and Jekyll. You can find setup instructions
[here](http://swcarpentry.github.io/lesson-example/setup/).

## Example lessons

Some links to example SWC workshop lessons for reference:

* [Example Bash lesson](https://github.com/swcarpentry/shell-novice)
* [Example Python lesson](
  https://github.com/swcarpentry/python-novice-inflammation)
* [Example R lesson](https://github.com/swcarpentry/r-novice-gapminder)
  (uses R markdown files instead of markdown)


[_includes](_includes)