# pamasol.github.io source code
Source code of [pamasol.github.io](https://pamasol.github.io/) website, based on Hugo, which is a [static site](https://en.wikipedia.org/wiki/Static_web_page) generator.

## Installation

1. Create following folders on your machine:
    ```
    C:\Hugo\bin
    C:\Hugo\Sites
    ```

2. Download the latest zipped Hugo executable (`*.exe`) from [Hugo Releases](https://github.com/gohugoio/hugo/releases/).

3. Extract all contents to your `C:\Hugo\bin` folder.

4. In [CMD](https://en.wikipedia.org/wiki/Cmd.exe), add the `hugo.exe` executable to your `PATH` with the following command (you need administrator privileges):
    ```
    set PATH=%PATH%;C:\Hugo\bin
    ```

5. Reboot your PC.

6. Now you can use hugo with your prefered CLI

Following commands are helpful:
* `hugo help` gives you a command overview
* `hugo server -D` runs a local server with drafts enabled.
* `hugo -D` builds static pages


# Base theme

Update git submodule as follows.

```
git submodule update --remote --merge
```
