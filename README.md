# Civic Tech DC Website

Welcome! This is the repository for the website for Civic Tech DC. It is a static site built with [Jekyll](https://jekyllrb.com/). It is mostly HTML, Javascript, and CSS.

## Getting Started

1. First, make sure that you have <a href="https://git-scm.com/downloads">git</a> on your computer. Create your own <a href="https://docs.github.com/en/get-started/quickstart/contributing-to-projects">fork</a> of the repository, then clone it to your computer:

`git clone git@github.com:[YOUR GITHUB NAME]/codefordc-website`

2. Now, install the correct version of Ruby.

We use [asdf](https://asdf-vm.com/) and its [ruby plugin](https://github.com/asdf-vm/asdf-ruby) to configure Ruby for this project. You can see which version of Ruby we're using in the [.tool-versions](.tool-versions) file.
#### For Windows Users
Since [asdf](https://asdf-vm.com/) relies on shell scripts that are not natively compatible with Windows command-line environments, a workable way for Windows users is through the Windows Subsystem Linux(WSL). To install WSL, open command prompt on windows and run:
```
wsl --install
```
Then restart the computer and install Remote Development on VScode.
Now, if you're on Ubuntu, you may need to install some dependencies. If the `install` step doesn't work, try one or both of these commands:
```
sudo apt install libyaml-dev
sudo apt install libffi-dev
```

To install the Ruby plugin, run the following commands inside the project's directory:

```
asdf plugin add ruby https://github.com/asdf-vm/asdf-ruby.git
asdf install
```
If you are on Ubuntu and the above `asdf install` fails to build. Try:
```
export RUBY_CONFIGURE_OPTS="--with-openssl-dir=/home/linuxbrew/.linuxbrew/Cellar/openssl@3/3.1.0"
asdf install ruby 3.2.0
```
3. Install required gems.

`bundle install`

4. Run a local version of the website.

`bundle exec jekyll serve`

5. Open a web browser page at `localhost:4000`

## Issues

If you notice a problem or have an idea for an improvement you can submit an [issue](https://github.com/civictechdc/codefordc-website/issues).

## Contributing

Refer to the [contribution instructions](CONTRIBUTING.md) to contribute to this project. We have a [project board](https://github.com/orgs/civictechdc/projects/3) where we track issues and ideas to be implemented.

Let us know if you get stuck in the Civic Tech DC Slack channel #civictechdc-website. Happy coding!
