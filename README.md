# Jekyll Blue

All-in-one easy Jekyll solution.

## Setting up the environment

1 - Easily install all Jekyll required software with ``` gem install github-pages ``` (Ruby needed!)


## Quick Start

1 - Fork this repo and rename it to yourgithubusername.github.io (yes, '.github.io' is included)

2 - Clone the fork locally (git clone ...)

3 - Edit it as you like and view it using ``` jekyll serve ```

4 - Write your first blog post and...

5 - ...publish it pushing it to the github remote!

Your website is available at yourgithubusername.github.io (for free, yay!)

Easy, isn't it?


## Custom Domain

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


## Credits

*cover.jpg* is licensed under a Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International License. You can read the license text [here](http://creativecommons.org/licenses/by-nc-nd/4.0/).
<br>Owner: Francesco Pira
<br>Title: Etna view from the Ancient Theatre of Taormina.
