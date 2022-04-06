# Onboarding content repository

This is the repository for content for the Onboarding portal. All files should be written in markdown, preferably adhering to the [CommonMark](https://commonmark.org/help/) specification.

You can use all markdown features when writing content, except for the H1 heading level. H1 heading level is generated automatically based on the frontmatter title field described below. Any H1 content present in the markdown files will be ignored and will NOT be displayed on portal pages.

Visual Studio Code comes with a markdown preview utility - you can use it to preview the documents you are writing before pushing them.

The content repository utilizes two branches ``develop`` and ``master``. All new and updated content is introduced by pull requests from feature branches to ``develop`` branch. Master branch will be used for production-ready content.

- Workflow for contributor:
  - Introduce changes in the file
  - Create a pull request to ``develop`` branch
- Workflow for maintainer
  - Review pull requests
  - Create pull requests from ``develop`` to ``master`` when it's time for release

*All content in develop is automatically updated to https://onboarding-new.mediusflow.com*
