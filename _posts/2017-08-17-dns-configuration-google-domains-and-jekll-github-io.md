---
layout: post
title:  "DNS Configuration: Google Domains and Jekll @ github.io"
date:   2017-08-16
categories: operations dns configuration
---

The setup and configuration process for a Domain managed by [Google Domains](http://domains.google.com) running a [Jekyll Blog](https://jekyllrb.com/) hosted on [GitHub Pages](https://pages.github.com/).

---
### Step 1 - Fork and update a GitHub repo.
- I forked this quickstart [Jekyll now](https://github.com/barryclark/jekyll-now) repo, by [Barry Clark](https://github.com/barryclark).
- Inside your fork, rename the repo using the following format `{githubusername}.github.io`
- In the settings section of the repo, goto the GitHub Pages section and point it to your naked domain, IE: `http://example.com` - without the `www.` canonical name alias.
- Update the CNAME file in the root directory, as follows:

```
tinkr.design
www.tinkr.design
```
That is all it takes to configure your blog in [GitHub](http://www.gituhb.com). Now you will need to configure the domain itself.

---
### Step 2 - Configure the DNS records for your domain.

Login to [Google Domains](http://domains.google.com/) and navigate to the DNS configuration section of the domain you wish to configure.
- Custom resource records: 

| Name | Type  | Time To Live | Data                       |
|------|-------|--------------|----------------------------|
| @    | A     | 1H           | 192.30.252.153             |
|      |       |              | 192.30.252.154             |
| www  | CNAME | 1H           | {githubusername}.github.io |

Thats all. Be warned that it may take a bit to propagate the records across the globe ( up to a day ), but generally this happens in less than 5 minutes for most locations.

You can visual the propagation [using various online tools](https://www.google.com/search?q=dns+propagation+checker) while you wait.

--
[t. payne](http://www.tpayne.net/) @ [tinkr.deisgn](http://www.tinker.deisgn/)
