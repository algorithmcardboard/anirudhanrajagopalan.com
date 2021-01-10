---
layout: post
title:  "Browser addons everyone should have"
date:   2020-11-09 23:44:33 -0600
tags: [privacy, firefox]
---

I like using Firefox more than Chrome as Firefox aligns more with my privacy outlook.  I also love Firefox just for the [major rewrite](https://bholley.net/blog/2017/stylo.html) they did using Rust.  I try to convince my friends to start using these addons and I thought it might be a good idea to start writing these down.  So here is a quick list.


## uBlock Origin
Note the name *uBlock Origin*.  Its not uBlock or Adblock Plus.  uBlock Origin is the one that is maintained by original author.  This is the addon that will actually protect you from ads and unwanted trackers.

## Privacy badger
Privacy badger went through a major rewrite recently.  (Read [Privacy Badger is Changing to Protect You Better](https://www.eff.org/deeplinks/2020/10/privacy-badger-changing-protect-you-better)).  Privacy badger has a list of known trackers and it helps you browse the web while securing your privacy as well.  I am yet to figure out if Privacy Badger with the new rewrite is still required when you have ublock origin.


## Decentraleyes
This addon emulates the CDN.  Remember when web-developers used to link jQuery and other libraries from Google CDN.  Using the Referrer header, Google can track which website you visit and which resource (url) within a site you visit due to the link the site's developer injected on his site.  Arguably, this makes the web faster, but it also provides more information to a centralized provider.  The solution Decentraleyes provides is to cache these common libaries in your browser and serve the files locally.

## Bitwarden
Remembering passwords is hard!  On top of that, saving yourself from Phishing is even harder.  Check [https://www.apple.com/](https://www.apple.com/) vs [https://www.xn--80ak6aa92e.com/](https://www.xn--80ak6aa92e.com/) and you can see that these go to very different websites but the URLs in FF reads apple.com.  Using password managers such as bitwarden not only helps you use strong passwords, it also helps you from phishing attacks as your spidy senses can be triggered when you visit a phishing website where no password is displayed in bitwarden.

## Firefox Multi-Account Container
Finally containers for browsers!!.  This addon provides you better separation of cookies and tracking info across websites.  If you have a work github and personal github, then using Multi-Account Container will help you use them both on the same browser.  Note that Firefox history is shared across all the containers into a single FF account.

## Facebook container
This is built on top of Multi-Account Containers.  I use this to sepatare out FF domains automatically.

## Temporary Containers
Temporary containers are built on top of Multi-Account conatiners.  This addon creates separate container context for things you browser quickly.  Think of random links you click.  It would be good to reduce your tracking by opening these links in separate containers.

## HTTPS everywhere
Its 2020.  But a lot of websites still use http:// by default even when a https:// url is available.  HTTPS Everywhere addon automatically makes you use https url if available.

## Certainly Something
Crtainly something is a certificate viewer.  Provides the details of the certificate and the certificate chain in greater detail