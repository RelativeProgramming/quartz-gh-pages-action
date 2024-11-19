# Quartz GitHub Pages Deployment Action
GitHub Action for minimal configuration deployment of [Quartz](https://github.com/jackyzha0/quartz) sites to GitHub Pages.

See `action.yml` for parameters.

**Example Configuration:**
```yml
jobs:
  publish_job:
    runs-on: ubuntu-latest
    steps:
    - name: Checkout repository
      uses: actions/checkout@v4

    - uses: RelativeProgramming/quartz-gh-pages-deploy@main
      with:
        quartz-version: v4.4.0
```
- documentation Markdown files are placed under `./docs/`
- modified `quartz.config.ts` is placed under `./docs/.quartz-config/`