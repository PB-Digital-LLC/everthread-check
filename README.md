# EverThread site check · GitHub Action

Runs EverThread's free, plain-English security check against a site after you deploy, writes the report card to the job summary, and comments it on the pull request.

```yaml
- uses: everthread/check@v1
  with:
    url: https://preview-${{ github.event.number }}.yourhost.app   # or yourbakery.com
    fail-on: urgent          # urgent | attention | none
```

Needs `permissions: pull-requests: write` for the comment. No key, no account. Observation only: it loads the home page the way a browser does. Check only sites you own or have permission to check.

Docs: https://everthread.live/api
