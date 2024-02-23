## Pubishing to Github Pages from Quatro in RStudio

This document describes how to publish a Quatro document to Github Pages.
The assumption is that you have already published to GitHub as you have copied one of the templates that we have, which are already set up to publish to Github Pages automatically.

**More documentation will be added to publish to Github Pages from scratch at a later time.**


## Workflow

1. Do a `git pull` on the project, either through the terminal or RStudio's Git pane.
2. Then, run `renv::restore()` in the R console (in case someone else has edited the files).
3. Make your edits, building the site occassionaly to see that it can be rendered properly.
4. Once you are ready to publish, do a `renv::snapshot()` to update the `renv.lock` file.
5. Commit and push your changes to Github.
6. Wait for the changes to be reflected on the Github website.


## Worst case scenario

If the site does not render and you are *out of time* to troubleshoot, you can do a manual update of the website. 

In the terminal tab, run:

```bash
quarto publish gh-pages
```
The command will automatically commit and push the changes to the `gh-pages` branch. Then, when you have free time, you can troubleshoot the issue so that you can resume the normal workflow.
