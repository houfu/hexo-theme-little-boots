# Little Boots Hexo Blog Theme

A Hexo Blog Theme which implements [the latest Bootstrap 4 (v 4.1.1)](https://getbootstrap.com/) and [the latest Font-Awesome (v 5.0.13)](https://fontawesome.com).

Several aspects of this theme were inspired by [Clean Blog Hexo](https://github.com/klugjo/hexo-theme-clean-blog).

## Why Little Boots?

Several themes for Hexo (like Clean Blog) used  previous versions of Bootstrap and Font Awesome. While there is nothing wrong with that, I used Bootstrap 4 (since Beta 1) and I have never looked back, so the loss of some of the more recent features like scss mixins etc were not available on such themes. Not to mention, folks who are using this for the first time would need to refer to older docs in order to customise their themes.

## Installation

The dependency `hexo-renderer-scss`is required to compile Bootstrap 4 SASS files.

```
npm install hexo-renderer-scss --save
```

Clone the latest version to your themes directory:

```
git clone https://github.com/houfu/hexo-theme-little-boots.git themes/little-boots
```

Update your blog's main `_config.yml` to set the theme to `little-boots`:

```yaml
# Extensions
## Plugins: http://hexo.io/plugins/
## Themes: http://hexo.io/themes/
theme: little-boots
```

## Configuration

### Additional Theming

As in [Bootstrap 4](https://getbootstrap.com/docs/4.1/getting-started/theming/), you can use Bootstrap 4's built in SASS variables for global style preferences for easy theming and components changes. Simply modify `little_boots.scss`.

### Introduction Jumbotron

The Index Page can feature a jumbotron right below the banner if you would like to hlighlight some content before going on to the blog posts (originally I wanted to mention something about my CV at this point). Edit the following section in the `_config.yml`to have some content there. You will need at least the title and the lead or text in order for the jumbotron to show. Leaving these fields blank will remove the jumbotron from the layout.

```yaml
# Intro
intro_title:  #This is the title of the Jumbotron
intro_lead:   #This is the text that appears under the title, which is larger than normal text
intro_text:   #This appears below the title and lead, and appears like normal text.
intro_btn_caption:  #This is the text that appears on the button under the intro_text.
intro_btn_link:  #This is the link that activates when the button is clicked. 
```

### Other Features

Several features that are available in [Clean Blog Hexo](https://github.com/klugjo/hexo-theme-clean-blog) are also available in `little_boots`:

- Disqus and Facebook comments
- Google Analytics
- Addthis
- Cover image for posts and pages
- Tags and Categories Support

Please read the ReadMe in Clean Blog Hexo](https://github.com/klugjo/hexo-theme-clean-blog) for further details on how to support them in your blog.

**Note:** In Font Awesome 5, Brand icons (like FaceBook, Github etc) are categorised in its own separate category. This means that in the Navigation Menu, only brand icons are supported. For example, email icons (like fa-envelope-open) *will not work* in the Navigation Menu. Will spend some time thinking of the best way to deal with this in a separate release.

## License

MIT
