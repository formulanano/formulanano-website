All contributions, including merge requests, feature requests, ideas, design tweaks, etc. are welcome. 
I welcome all input, from sharing your own implementations of code to general thoughts and ideas. Just open a new issue!

## Feature Requests

Feature requests are always welcome! If Jekyll can do it and if the theme's design would work well with it, then I would love to add it. Of course, 
code submission via a merge/pull request is great, but not necessary.

## Bug Reports

If you encounter any issues with these themes on any devices, please submit a bug report with the device type and a detailed description of what 
the issue that you're encountering is.
<br /><br />

## How to contribute

### 1. Fork the repo
Visit this link if you have any confusion:  https://help.github.com/en/articles/fork-a-repo#fork-an-example-repository

### 2. Clone your forked repo to your machine
Visit this link if you have any confusion:  https://help.github.com/en/articles/cloning-a-repository

### 3. Install Dependencies to Serve Website Locally [*]

In order deploy the website locally we need Ruby and some "gems" installed on our machines.

#### 3.1. Windows

1. Download and Install a Ruby+Devkit version from [RubyInstaller Downloads](https://rubyinstaller.org/downloads/). Use default options for installation.
2. Run the `ridk install` step on the last stage of the installation wizard. This is needed for installing gems with native extensions. You can find additional information regarding this in the [RubyInstaller Documentation](https://github.com/oneclick/rubyinstaller2#using-the-installer-on-a-target-system).
3. Open a new command prompt window from the start menu, so that changes to the PATH environment variable becomes effective. Install Jekyll via `gem install jekyll` and for compatibility install Bundler v1.12 via `gem install bundler -v 1.12`
4. Check if Jekyll and Bundler are installed properly: `jekyll -v` and `bundler -v`
5. Go to the directiory of your forked repository and run `jekyll serve`. In your browser open "127.0.0.1:4000".

#### 3.2. Fedora
1. Run `sudo dnf install ruby ruby-devel @development-tools`
2. To avoid install gems as root user add following lines to your ".bashrc" or related configuration file that is used by your shell (for example ".zshrc" if tou use zsh). This lines tells your system to install gem files to "~/gems"
```
export GEM_HOME="$HOME/gems"
export PATH="$HOME/gems/bin:$PATH"
```
3. Install Jekyll via `gem install jekyll`
* If you get an error that says
`gcc: error: /usr/lib/rpm/redhat/redhat-hardened-cc1: No such file or directory`
Run : `sudo dnf install redhat-rpm-config`
* If you get an error that says `make: g++: Command not found`
Run: `dnf install gcc-c++`
4. Install Bundler v1.12 for compatibility via `gem install bundler -v 1.12`
5. Go to the directiory of your forked repository and run `jekyll serve`. In your browser open "127.0.0.1:4000".


#### 3.3. Ubuntu

1. Run `sudo apt-get install ruby-full build-essential zlib1g-dev`
2. To avoid install gems as root user add following lines to your ".bashrc" or related configuration file that is used by your shell (for example ".zshrc" if tou use zsh). This lines tells your system to install gem files to "~/gems"
```
export GEM_HOME="$HOME/gems"
export PATH="$HOME/gems/bin:$PATH"
```
3. Install Jekyll via `gem install jekyll` and for compatibility install Bundler v1.12 via `gem install bundler -v 1.12`
4. Go to the directiory of your forked repository and run `jekyll serve`. In your browser open "127.0.0.1:4000".

### 4. Make the changes you want
### 5. Go to GitHub page of your forked repo and create a pull request
Visit this link if you have any confusion: https://help.github.com/en/articles/creating-a-pull-request

*Thank you*

[*] Source: https://jekyllrb.com/docs/installation/
