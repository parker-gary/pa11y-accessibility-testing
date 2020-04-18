# pa11y-accessibility-testing

A build template to run Pa11y accessibility testing on your webpages via the command line.

## Variables

In the settings for your repository, set a 'Secret' environment variable with name 'target_url', and value of the url you want to run tests against.

```sh
- shell: cmd
  name: Run Accessibility Tests
  env:
    target_url: ${{ secrets.target_url }}
  run: pa11y "%target_url%"
```
