# luisencerrabodes.me

Static website hosted via github pages and available at [luisencerrabodes.me](https://luisencerrabodes.me).


## Development

Setup and layout based on [Henrik Nyh](https://henrik.nyh.se/).

Assuming ruby and bundler are already installed:

```ruby
# Install dependencies with bundler.
bundle install

# Watch sass directory and recompile on change.
./script/watch
```

Build SASS with:
```
./script/build
```

The CSS is built in `./docs` since this is the default directory used by github pages. To run locally simply open
up `./docs/index.html` on your browser.

## Deploy

To deploy changes, build the CSS with `scripts/build`, push the changes to `docs` directory to the `main` branch.
