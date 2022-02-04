# Magpylib-Sandbox

This repository is an environment sanbox for testing the magpylib master branch.

The purpose of this repository is to de-couple the content of a repository from the environment that is needed to run it. This allows us to update the content of a repo without needing to re-build the Binder needed for it. (More infos [here](https://discourse.jupyter.org/t/tip-speed-up-binder-launches-by-pulling-github-content-in-a-binder-link-with-nbgitpuller/922))

Any other repo containing jupyter notebooks (as `*.ipynb` or `*.md`) can be linked to this repository via [nbgitpuller](https://github.com/jupyterhub/nbgitpuller) and use the environment created by this repo.

The environment dependencies are defined [here](https://github.com/Alexboiboi/Magpylib-Sandbox/blob/main/.binder/environment.yml)

You can use [nbgitpuller link generator](https://jupyterhub.github.io/nbgitpuller/link) to create a custom Binder link that points to the content of your own repo.
