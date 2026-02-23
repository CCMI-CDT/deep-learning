# Training week site template

This repository is a template that can be used to create a site for resources for a training week.

## Setting up a new site

1. [Fork this repository](https://github.com/CCMI-CDT/training-week-site-template/fork)

2. In the settings of the new repository, click on "Pages" and set source to "GitHub Actions".

3. In the "Actions" tab of the repository, click "I understand and want to activate Actions"

4. Update the title and authors in [book.toml](book.toml)

## Editing a site

The pages of your site should be markdown files in the [src/](src/) directory.
In order to appear on your site, each page should be listed in the file [SUMMARY.md](src/SUMMARY.md).

More details about how mdbooks work can be found [here](https://rust-lang.github.io/mdBook/guide/creating.html).
