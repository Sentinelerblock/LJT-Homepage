# LJT-Homepage

Junteng Liu's personal homepage, forked from [AcademicPages](https://github.com/academicpages/academicpages.github.io). Personal content uses only the supplied memory.

## Content

- `_pages/about.md`: biography, education, research internships, all six publications, research background and interests, the Zhiyuan Honor Scholarship, and contact information.
- `_pages/publications.html`: the same six publications on the template's existing Publications page.
- `_data/navigation.yml`: links to sections of the homepage.
- `_config.yml`: profile settings and project-site configuration.

No new content pages were added. Unrelated template pages, sample posts, and sample collections are excluded from the published build. No photograph, unrecorded programming-language or framework skills, or guessed publication URLs have been added.

## Build and deployment

The existing `.github/workflows/jekyll.yml` workflow builds the site and checks that only the two existing content pages are generated, that all six publication titles appear on both pages, and that saved contact links and homepage navigation are present.

Configured project-site URL: `https://sentinelerblock.github.io/LJT-Homepage/`.

GitHub Pages must be enabled for the repository with **Settings → Pages → Source → GitHub Actions**. GitHub's workflow token cannot perform initial Pages enablement. When Pages is not enabled, the workflow uploads the verified build artifact and explicitly skips deployment. Once Pages is enabled, the same workflow can deploy on a push to `master` or a manual run.

Local build:

```sh
bundle install
bundle exec jekyll build
```

The original theme license is retained in `LICENSE`.
