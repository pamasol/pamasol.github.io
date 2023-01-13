# pamasol.github.io source code
Source code of [pamasol.github.io](https://pamasol.github.io/) website, based on Hugo, which is a [static site](https://en.wikipedia.org/wiki/Static_web_page) generator.

## Installation and local development

1. Create following folders on your machine:

    ```bash
    C:\Hugo\bin
    C:\Hugo\Sites
    ```

2. Download the latest zipped Hugo executable (`*.exe`) from [Hugo Releases](https://github.com/gohugoio/hugo/releases/).

3. Extract all contents to your `C:\Hugo\bin` folder.

4. In [CMD](https://en.wikipedia.org/wiki/Cmd.exe), add the `hugo.exe` executable to your `PATH` with the following command (you need administrator privileges):

    ```bash
    set PATH=%PATH%;C:\Hugo\bin
    ```

5. Reboot your PC.

6. Go to `C:\Hugo\Sites` and run ([Git](https://git-scm.com/downloads) must be installed on your machine):

    ```bash
    git clone https://github.com/pamasol/pamasol.github.io.git
    ```

7. Cd into the project folder as follows:

    ```bash
    cd pamasol.github.io
    ```

8. This template is based on the [Hugo Relearn Theme](https://github.com/McShelby/hugo-theme-relearn) from [@McShelby](https://github.com/McShelby). Many thanks to him for this great piece of code. The submodule can be downloaded as follows:

    ```bash
    git submodule init
    git submodule update --remote
    ```

9. Now you can run hugo comands. Following commands are helpful:
    * `hugo help` gives you a command overview
    * `hugo server -D` runs a local server with drafts enabled.
    * `hugo -D` builds static pages and puts into folder `docs`. Not needed in this repo since build and deployment realized with GitHub actions.
    * `git status` calls for the status of your local file, for example to check on untracked files
    * `git add --all` Adds everything up for the commit, such as untracked files etc.
    * `git commit -m "text" ` Commits everything, the text can be changed to a commentary of the changes
    * `git push` Pushes everything up to the server

## Deployment

When pushing to `master` branch following pipeline gets triggered that builds the static pages in a first step. The static pages are placed in th `gh-pages` branch and will be moved from there to [https://pamasol.github.io](https://pamasol.github.io/) in a second step:

1. `create-static-page` is defined in [`.github/workflows/gh-pages.yml`](https://github.com/pamasol/pamasol.github.io/blob/main/.github/workflows/gh-pages.yml). It creates the static content and places it in the `gh-pages` branch.

2. `pages-build-deployment` takes the static pages and pushes them on GitHub Pages. There is no `*.yml` file for this procedure, it is defined in [settings > pages](https://github.com/pamasol/pamasol.github.io/settings/pages).
