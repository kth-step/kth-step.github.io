# KTH STEP website

This README intends to give short instructions about how to manage and update
this website. If you just want to visit the website, here it is:

https://kth-step.github.io/

## Important notes

When copy-pasting configuration files from around the Internet, (try to keep it legal, and) try to keep documentation and comments. No need to remove it, because that's likely that (the next-)you will have forgotten about all of this the next time that a change will have to be made. Also, try to write short comments for everything.

In order to update the website, just push to `master`. In other words, GitHub automatically deploys the website from the `master` branch.

## Running locally

In order to update the website, you can either create direct Pull Requests here on GitHub or clone the repository and commit locally. The second option gives the ability to see changes before pushing the code. Please read the official documentation (links below) for installation instructions and how-to pages.

```
# Only once, or when changing plugins
bundle install

# Rerun this when changing `_config.yml`, otherwise it's live-reloading
bundle exec jekyll serve
```

## Documentation links

This website tries to use the minimal configuration and "technical" changes possible. That's possible thanks to this combination of tools:
 - GitHub pages: https://pages.github.com/
 - Jekyll (static website generator): https://jekyllrb.com/
 - Minimal Mistakes (theme): https://mmistakes.github.io/minimal-mistakes/docs/

Basically, if you want to update the site content or structure, go to the theme's documentation.

