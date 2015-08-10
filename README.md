# Jekyll Blue

[![Gitter](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/pirafrank/Jekyll-Blue?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge)

![Imgur](http://i.imgur.com/UDLHJKT.png)

All-in-one easy Jekyll solution.

## Features

- All features of Jekyll-Now (credits to the author and contributors)

Plus:

- Completely redesigned home page
- Dedicated page for all blog posts
  - Sort posts by date or by category
- Automatic urls creation with redirect to enabled social networks
  - e.g. yourwebsite.com/twitter automatically redirects to your twitter account, yourwebsite.com/facebook to your facebook profile, and so on. Just you set up your social networks in _config.yml file
- Reach all articles of the same category of the post you're reading with a single click
- CSS class to support tablets and similar-sized screens
- Sass variables overhaul: easily apply your favourite colors!
  - embedded bootstrap color palette
- variables to easily change fonts site-wide
- New fonts!
  - Go the Google way with Roboto for sans-serif
  - Posts are written in beautiful Merriweather for better reading
- Improved font handling: ttf and woff2 fonts are embedded so your site displays the same on a wide range of devices
- Support for post sharing on Twitter, Facebook, LinkedIn, Google+
- Improved footer
- ...more I forgot!


## Quick start

### Setting up the environment

Easily install all Jekyll required software with ``` gem install github-pages ``` (Ruby needed!)

Already done? Skip to 'Make it yours'!

#### Troubleshooting

If you stuble across error *Could not find a JavaScript runtime. (ExecJS::RuntimeUnavailable)*, solve it with ``` gem install therubyracer ```.

### Make it yours

1 - Fork this repo and rename it to yourgithubusername.github.io (yes, '.github.io' is included)

2 - Clone the fork locally (git clone ...)

3 - Edit it as you like and view it using ``` jekyll serve ```

4 - Write your first blog post and...

5 - ...publish it pushing it to the github remote!

Your website is available at yourgithubusername.github.io (for free, yay!)

Easy, isn't it?


## Use your custom domain

You could buy a domain and setup a redirect or better setup a DNS redirect.

#### DNS redirect

1 - Buy the domain you like

2 - Create a free cloudflare account

3 - Add your custom domain to cloudflare and follow the procedure

4 - Add your custom domain to CNAME file in repository root

5 - Create an A record on cloudflare to point to github servers (follow [this guide](https://help.github.com/articles/tips-for-configuring-an-a-record-with-your-dns-provider/))


#### Get free HTTPS

**Please note that this solution is just palliative for the user.** Github Pages dosen't support HTTPS connection for custom domains. The furthest you can go is to use cloudflare as proxy and encrypt connection between the user and cloudflare. Thus Cloudflare to Github connection will remain not encrypted.

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

Copyright (c) 2015 Francesco Pira <dev@fpira.com>.

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
    along with Jekyll Blue.  If not, see <http://www.gnu.org/licenses/>.


## Credits

- [Jekyll Now](https://github.com/barryclark/jekyll-now), its contributors and third-part projects who made it possible
- Google Fonts
- [labs.jonsuh.com/](http://labs.jonsuh.com/responsive-video-embed/) for responsive video support

*cover.jpg* is a photo I took in 2014 and it's entitled "*Etna view from the Ancient Theatre of Taormina*". I license it under a [Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International License](http://creativecommons.org/licenses/by-nc-nd/4.0/). Feel free to use it under the license terms. You can read the full license text [here](http://creativecommons.org/licenses/by-nc-nd/4.0/legalcode).
