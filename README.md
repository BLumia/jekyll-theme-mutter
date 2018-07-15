# jekyll-theme-mutter

A jekyll theme. 

## Installation

Add this line to your Jekyll site's `Gemfile`:

```ruby
gem "jekyll-theme-mutter"
```

And add this line to your Jekyll site's `_config.yml`:

```yaml
theme: jekyll-theme-mutter
```

And then execute:

    $ bundle

Or install it yourself as:

    $ gem install jekyll-theme-mutter

## Usage

You can directly take a look at the [jekyll-theme-mutter](https://github.com/BLumia/jekyll-theme-mutter)'s source code so you can check out some example usage about how we get [the example site](https://blumia.github.io/jekyll-theme-mutter/) works.

### Layouts

Refers to files within the `_layouts` directory, that define the markup for your theme.

 - default.html — The base layout that lays the foundation for subsequent layouts. The derived layouts inject their contents into this file at the line that says `{{ content }}` and are linked to this file via FrontMatter declaration layout: default.
 - `home.html` — Don't use it.
 - `page.html` — The layout for your documents that contain FrontMatter, but are not posts.
 - `post.html` — The layout for your posts.
 - `posts.html` — The layout for your post list. 

### Customization

We got some useful attr for customization the site.

 - `header_pages` - You probably want some pages display in the navbar, then provide a list in your `_config.yml`
 - `nav-title` - If you use the navigation bar, Set this in front-matter so the value you've set will be display in the navbar instead of the page title.
 - `subtitle` - All web pages in this theme got a subtitle, you can set a subtitle in every single page and also in `_config.yml` for a global default subtitle.

## Contributing

Bug reports and pull requests are welcome on GitHub at https://github.com/BLumia/jekyll-theme-mutter. This project is intended to be a safe, welcoming space for collaboration, and contributors are expected to adhere to the [Contributor Covenant](http://contributor-covenant.org) code of conduct.

## Development

To set up your environment to develop this theme, run `bundle install`.

Your theme is setup just like a normal Jekyll site! To test your theme, run `bundle exec jekyll serve` and open your browser at `http://localhost:4000`. This starts a Jekyll server using your theme. Add pages, documents, data, etc. like normal to test your theme's contents. As you make modifications to your theme and to your content, your site will regenerate and you should see the changes in the browser after a refresh, just like normal.

When your theme is released, only the files in `_layouts`, `_includes`, `_sass` and `assets` tracked with Git will be bundled.
To add a custom directory to your theme-gem, please edit the regexp in `jekyll-theme-mutter.gemspec` accordingly.

## License

The theme is available as open source under the terms of the [MIT License](https://opensource.org/licenses/MIT).

