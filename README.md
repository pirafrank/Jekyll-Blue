# Jekyll Blue

[![Gitter](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/pirafrank/Jekyll-Blue?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge)

![Imgur](http://i.imgur.com/UDLHJKT.png)

All-in-one easy Jekyll solution.

**Already downloaded? Check the [customisation](#customisation) section!**

## Changelog

Please check [release notes](https://github.com/pirafrank/Jekyll-Blue/releases).

## Features

- All features of Jekyll-Now (credits to its author and its contributors)

### Plus

- Completely redesigned home page
- Full-width navbar
- Website search
  - Powered by duckduckgo, so you don't have to worry about being tracked
- Automatic urls creation with redirect to enabled social networks
  - e.g. yourwebsite.com/twitter automatically redirects to your twitter account, yourwebsite.com/facebook to your facebook profile, and so on. Just you set up your social networks in _config.yml file
- Choose whether to display social icons in footer or just in home
- Email obfuscation, so you don't get spam (yay!).
  - *BONUS:* your email is displayed correctly
  - ```mailto``` link works
  - mobile is supported
  - ..and it's easy to use, too. Please read how to use it below.
- Dedicated page for all blog posts
  - Sort posts by date or by category
- Choose whether to display or not page titles on a per-page basis.
- Reach all articles of the same category of the post you're reading with a single click
- Evernote Web Clipper and Evernote Clearly support: your articles are displayed beautifully
- Responsive support for videos (HTML5, embedded, YouTube and Vimeo)
- 'Back to top' button in post pages
- CSS class to support tablets and similar-sized screens
  - Use ```@include smallscreen``` in your Sass code
- Sass variables overhaul: easily apply your favourite colors!
- Bootstrap color palette ready to use
- Variables to easily change fonts site-wide
- Great fonts!
  - Go the Google way with Roboto for sans-serif
  - Posts are written in beautiful Merriweather for better reading
- Improved font handling: ttf and woff2 fonts are embedded so your site displays the same on a wide range of devices
- Support for post sharing on Twitter, Facebook, LinkedIn, Google+
- Improved footer
- ...more I forgot!

Looking how to use one or more features? Please, check the [customisation](#customisation) section.

## Quick start

### Setting up the environment

Easily install all Jekyll required software with ``` gem install github-pages ``` (Ruby needed!)

Already done? Skip to 'Make it yours'!

#### Troubleshooting

If you stuble across error *Could not find a JavaScript runtime. (ExecJS::RuntimeUnavailable)*, solve it with ``` gem install therubyracer ```.

### Use it

1 - Fork this repo and rename it to yourgithubusername.github.io (yes, '.github.io' is included)

2 - Clone the fork locally (git clone ...)

3 - Edit it as you like and view it using ``` jekyll serve ```

4 - Write your first blog post and...

5 - ...publish it pushing it to the github remote!

Your website is available at yourgithubusername.github.io (for free, yay!)

Easy, isn't it?

## Customisation

#### Website-wide

**Style**

Check ```styles.scss``` in root folder.

**Colors and Fonts**

Jekyll-Blue is designed to use a scale of colors and only two font families, one Serif and one Sans-Serif. Go to ```_sass/_variables.scss``` to customise all of them. If you add/change fonts, remeber to edit ```_sass/_fonts.scss``` accordingly.

#### Search results page

You can customise colors of result page in ```_includes/searchbox.html```

#### Display page title

This setting is related to pages, not posts.

To display the title in page, set ```show_title``` to ```true``` or ```false``` in Liquid header.

#### Using email obfuscation

Make your email secure in 2 steps:

1 - Go to ```_config.yml``` 

2 - In *encryptedemail* type your email with **1 space** between each character (don't worry, it will be displayed correctly :smiley:). You're done!

**Example**

If your email is *myawesome@email.com*, then type *m y a w e s o m e @ e m a i l . c o m*.

**Note**

If you don't use *encryptedemail*, your plain email will be used (if in _config.yml).

**Always-secure email**

Use the code below wherever you want (even in markdown pages!) to secure your email.

```html
<div class="safe-email">
    <a href="mailto:{{ site.encryptedemail }}" onclick="this.href=this.href.replace(/ /g,'')">{{ site.encryptedemail }}</a>
</div>
```

## Use your custom domain

You could buy a domain and setup a redirect or better setup a DNS redirect.

#### DNS redirect

1 - Buy the domain you like

2 - Create a free cloudflare account

3 - Add your custom domain to cloudflare and follow the procedure

4 - Add your custom domain to CNAME file in repository root

5 - Create an A record on cloudflare to point to github servers (follow [this guide](https://help.github.com/articles/tips-for-configuring-an-a-record-with-your-dns-provider/))


#### Get free HTTPS

**Please note that this solution is just palliative for your website visitors.** Github Pages dosen't support HTTPS connection for custom domains. The furthest you can go is to use cloudflare as proxy and encrypt connection between the user and cloudflare. Thus Cloudflare to Github connection will remain not encrypted.

If you still want to have this facade security, follow the procedure below.

1 - Go to cloudflare and enable it (just be sure you have an orange cloud near the DNS entry, if not click the cloud to make it orange)

2 - In *Crypto*, enable *Flexible SSL*

3 - In *Page Rules*, create rules to *always use HTTPS*. You need to create two of those: one for yourcustomdomain.com and one for www.yourcustomdomain.com.

4 - Wait a could of hours

You're done!

## Contribute

Got a great feature it's missing? 

Fork this repo, clone, code the feature and send me a pull-request!

## License

Copyright (c) 2015 Francesco Pira < fpira.com >.

Jekyll Blue is a fork of Jekyll Now. Jekyll Now is released under MIT license, copyright (c) 2015 Barry Clark.

    Jekyll Blue is free software: you can redistribute it and/or modify
    it under the terms of the GNU General Public License as published by
    the Free Software Foundation, either version 3 of the License, or
    (at your option) any later version.

    Jekyll Blue is distributed in the hope that it will be useful,
    but WITHOUT ANY WARRANTY; without even the implied warranty of
    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
    GNU General Public License for more details.

    You should have received a copy of the GNU General Public License
    along with Jekyll Blue. If not, see <http://www.gnu.org/licenses/>.


## Credits

- [Jekyll Now](https://github.com/barryclark/jekyll-now), its contributors and third-part projects who made it possible
- Google Fonts
- [responsivegridsystem](http://www.responsivegridsystem.com/) for the CSS grid code
- [labs.jonsuh.com/](http://labs.jonsuh.com/responsive-video-embed/) for responsive video support
- [This guy](http://stackoverflow.com/users/27009/pornel) on StackOverflow for [email obfuscation code](http://stackoverflow.com/questions/163628/making-email-addresses-safe-from-bots-on-a-webpage)
- Hardik Pandya for [his great article](http://hardik.org/blog/2013/stylising-duckduckgo-site-search/) about website search

*cover.jpg* is a photo I took in 2014 and it's entitled "*Etna view from the Ancient Theatre of Taormina*". I license it under a [Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International License](http://creativecommons.org/licenses/by-nc-nd/4.0/). Feel free to use it under the license terms. You can read the full license text [here](http://creativecommons.org/licenses/by-nc-nd/4.0/legalcode).
