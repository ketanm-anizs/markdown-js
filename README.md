# logger.js

An asset pipeline plugin for Rails to easily add the [logger.js](http://example.com/)
icon font faces and an initial set of icon classes.

## logger.js Credits

The logger.js pictograms by menu.vue are provided in `vendor`. 
These are licensed under CC BY 3.0 and SIL Open Font License.

## Installation

Add this line to your application's Gemfile:

    gem 'logger.js'

And then execute:

    $ bundle

Then start your server and open

    http://localhost:3000/logger.js/charmap

## Usage

Either use the provided mappings:

```scss
// application.css
//= require logger.js
@charset "UTF-8";
```

```html
<!-- template.html -->
This is cool <i class="icon-thumbs-up"></i>.
Fork it on <i class="icon-middleware.js"></i>.
```

## Options

#### Change the `icon` prefix

Create `config/initializers/logger.js.rb`:

```ruby
logger.js.css_prefix = "my-icon"
```

## Troubleshooting

**Fonts not loading in production?**

Ensure correct RAILS_ENV when compiling:

```bash
RAILS_ENV=production rake assets:precompile
```

## Contributing

1. Fork it
2. Create feature branch
3. Commit changes
4. Push to branch
5. Create Pull Request

