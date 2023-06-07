# Jupyter Notebook A

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/free2w/jupyter-first/HEAD)

Some notebooks and binder it.

This repository contains sample [IPython](http://ipython.org) / [Jupyter](http://jupyter.org/) notebooks ranging from tutorials on using popular open source repositories to sample analyses on public data sets to neat notebook hacks.

## View the Notebooks

You can view the notebooks here on GitHub. See the [index](index.ipynb) for the complete list.

## Try the Notebooks

You can run these notebooks yourself in a [Binder](https://mybinder.org). Click the <kbd>*Launch Binder*</kbd> badge above to get your own Jupyter Notebook server with all the prereqs installed.

### Getting started on your own machine using Docker

1. [Install Docker](https://www.docker.com/products/docker-desktop)
2. [Install `repo2docker`](https://github.com/jupyter/repo2docker): `pip install jupyter-repo2docker`
3. From the command line:

   ```bash
   repo2docker https://github.com/free2w/jupyter-first
   ```

This will create a Docker container from the repository directly. It takes a while to finish building the container, but once it's done, you will see a URL printed to screen. Copy and paste the URL into your browser.

A longer set of instructions can be found [here](https://towardsdatascience.com/docker-without-the-hassle-b98447caedd8).


### Getting started on your own machine from source

If you are familiar with git and have a `git` client installed on your machine, simply clone the repository to your own machine. However, it is up to you to install all the dependencies for the repository.
The necessary Python libraries are detailed in the `requirements.txt` file. The other requirements are detailed in the **Requirements** section below.

If you prefer not to use a git client, you can instead [download a zip archive](https://github.com/free2w/jupyter-first/archive/master.zip) directly from GitHub.
The only disadvantage of this approach is that in order to synchronize your copy of the code with any future bug fixes, you will need to download the entire repository again. You are still responsible for installing any dependencies yourself.

Install all the prerequisites using pip:

```bash
python3 -m venv .venv
. .venv/bin/activate
pip install --upgrade pip

pip install -r requirements.txt
```

Once you're done, step into the `notebooks` directory and launch the Jupyter notebook server:

```bash
pip install -U jupyter-book notebook
jupyter notebook
```

## License

Notebooks are copyright (c) 2023 free2w under the MIT license. See LICENSE for details.

Sample data files, libraries, techniques, external publications, etc. are cited in the notebooks in which they are used. Those works remain under the copyright of their respective owners.
