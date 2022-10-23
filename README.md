# Privacy Guides Blog

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
