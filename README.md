# Privacy Guides Blog

## Post Metadata

- `date` (**required**): Post date
- `categories`: List of post categories. Allowed categories: `Announcements`, `Opinion`, `Software`, `Hardware`, `Android`, `iOS`, `Linux`, `macOS`, `Windows`, `Qubes OS`, `Providers`
- `authors`: List of post authors. Authors must exist in [`.authors.yml`](/docs/.authors.yml). Only the first author will be displayed on the blog index.
- `links`: Related links shown on post sidebar. May be internal or external links.
- `tags`: List of post tags. Reuse [existing tags](https://blog.privacyguides.org/tags/) if applicable, but feel free to add any as-needed.
- `license`: Post license. May be one of `BY`, `BY-SA`, `BY-NC`, `BY-NC-SA`, `BY-SA`, `BY-ND`, `BY-NC-ND`, or `CC0` to be automatically linked, or set to any HTML string. Defaults to "All rights reserved" if not set.

Example:

```
---
date: 2021-09-14
categories:
    - Announcements
authors:
    - jonaharagon
    - dngray
    - freddy-m
links:
    - 'About Privacy Guides': "https://www.privacyguides.org/about/"
    - posts/weve-joined-the-open-collective-foundation.md
tags:
    - Privacy Guides
license: CC0
---
```

## Developing

Committing to this repository requires [signing your commits](https://docs.github.com/en/authentication/managing-commit-signature-verification/signing-commits) (`git config commit.gpgsign true`) unless you are making edits via the GitHub.com text editor interface. As of August 2022 the preferred signing method is [SSH commit signatures](https://docs.github.com/en/authentication/managing-commit-signature-verification/about-commit-signature-verification#ssh-commit-signature-verification), but GPG signing is also acceptable. You should add your signing key to your GitHub profile.

This website uses [`mkdocs-material-insiders`](https://squidfunk.github.io/mkdocs-material/insiders/) which offers additional functionality over the open-source `mkdocs-material` project. For obvious reasons we cannot distribute access to the insiders repository. 

**Team members** should clone the repository with `mkdocs-material-insiders` directly. This method is identical to production:

1. Clone this repository and submodules: `git clone --recurse-submodules https://github.com/privacyguides/privacyguides.org.git`
2. Enable SSH commit verification with our local [`.allowed_signers`](/.allowed_signers) file: `git config gpg.ssh.allowedSignersFile .allowed_signers`
3. Install Python **3.10**
4. Install **pipenv**: `pip install pipenv`
5. Install dependencies: `pipenv install --dev` (install [Pillow and CairoSVG](https://squidfunk.github.io/mkdocs-material/setup/setting-up-social-cards/#dependencies) as well to generate social cards)
6. Serve the site locally: `pipenv run mkdocs serve`
    - The site will be available at `http://localhost:8000`
    - You can build the site locally with `pipenv run mkdocs build`
    - This version of the site should be identical to the live, production version

If you commit to `main` with commits signed with your SSH key, you should add your SSH key to [`.allowed_signers`](/.allowed_signers) in this repo.
