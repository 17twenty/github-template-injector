# Github Template Injector

Simple script that relies on having [personal access tokens](https://help.github.com/articles/creating-a-personal-access-token-for-the-command-line/)
for your account.

## Getting Started

Really simple. Grab the script. Set the params. Run the script. Cleanup anything
that didn't push.

```bash
$ export GITHUB_AUTH_TOKEN=XXXXXX
$ export GITHUB_ORG=migrated-things
$ export GITHUB_URI=git.private.domain
$ bash gh-templater.sh
...
```

## Issues

- Currently only really works against Github Enterprise due to the fact Github.com exposes different URIs for API and I'm lazy.
- Only deals with the first 100 pages... You'd need to get it to do `&page=2` or filter out the 'next' link in the JSON but see point 1.

PRs welcome.
