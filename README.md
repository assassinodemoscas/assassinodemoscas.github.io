# luisencerrabodes.me

Static website hosted via github pages and available at [luisencerrabodes.me](https://luisencerrabodes.me).


## Development

Setup heavily based on [Henrik Nyh](https://henrik.nyh.se/).

Assuming ruby and bundler are already installed:

```ruby
# Install dependencies with bundler.
bundle install

# Watch SCSS directory and recompile on change.
./script/watch
```

Build with:
```
./script/build
```

The content is built in `./public` so simply open up `./public/index.html` on your browser thereafter.

## Deploy

To deploy changes, build the page with `scripts/build`, push the changes to `public` directory to the `main` branch.

Then, update the `gh-pages` branch with:

```bash
git push origin `git subtree split --prefix public main`:gh-pages --force
```
