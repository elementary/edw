# edw

Mini-site and public resources for elementary Developer Weekend. For private planning resources, see: [@elementary/edw-planning](https://github.com/elementary/edw-planning)

**See, vote on, and submit [Talk Proposals](https://github.com/elementary/edw/discussions/categories/talk-proposals).**

<details markdown="1">
<summary><strong>Building & Running Locally</strong></summary>

This repo is a simple Jekyll-powered site hosted by GitHub Pages. To run it locally, see [the GitHub docs](https://help.github.com/articles/setting-up-your-github-pages-site-locally-with-jekyll/).

### Dependencies

This guide assumes you're on elementary OS or a similar Ubuntu-based environment.

#### Packages

- `ruby-full` (should include `ruby` and `ruby-dev`)
- `build-essential`
- `zlib1g-dev`

#### Ruby Stuff

- `jekyll` and `bundler`

We recommend installing gems to a (hidden) directory in your home folder:

```shell
echo '' >> ~/.bashrc
echo '# Install Ruby Gems to ~/.gems' >> ~/.bashrc
echo 'export GEM_HOME="$HOME/.gems"' >> ~/.bashrc
echo 'export PATH="$HOME/.gems/bin:$PATH"' >> ~/.bashrc
echo '' >> ~/.bashrc
source ~/.bashrc
```

Install jekyll and bundler:

```shell
gem install jekyll bundler
```

Install gems:

```shell
bundle install
```

(Adapted from https://jekyllrb.com/docs/installation/)

### Serve

```shell
bundle exec jekyll serve --host 0.0.0.0
```

The site should now be available at http://0.0.0.0:4000/ on your local machine, and your local machine's IP address on your network—great for testing on mobile OSes.
</details>
