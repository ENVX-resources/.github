## Contribution Guidelines

This is a draft of the contribution guidelines for the various repositories under the SOLES OER organisation. It will change, perhaps frequently and drastically, as we learn more about the needs of the community (staff and students) and the best ways to support them. We may even separate the guidelines into different documents or repositories. But for now, let's go through the pressing issues.

## How to set up Quarto projects for publishing to GitHub Pages

In general most Quarto templates and documents in our repositories have been set up for *automatic* publishing to GitHub Pages. This means that when you push changes to the `main` branch, the document will be built and published to the `gh-pages` branch. This is a great feature, but it can be a bit tricky to set up. Here's a step-by-step guide.

### Checks

First of all, depending on how you copied a template or started a new project, you may need to check a few things to see if automated publishing has been set up. In most cases if you have a `.github/workflows` directory in your repository, you're good to go as either

- someone has set up the publishing for you, or
- you have copied a template that has the publishing set up, and you remembered to "Include all branches" when you created the repository.

![](images/include-all-branches.png)