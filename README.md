# [pchoi.me](https://pchoi.me)

[![Netlify Status](https://api.netlify.com/api/v1/badges/2ca40221-5ca7-4763-bc13-e18013c32bc0/deploy-status)](https://app.netlify.com/sites/pchoi-me/deploys)

A personal URL shortener, inspired by [Kent C Dodds](https://github.com/kentcdodds/netlify-shortener)

Basic steps to get your own shortlinks up and running:

1. Pick up a custom domain from a domain registrar like [namecheap.com](https://namecheap.com) or [iwantmyname.com](https://iwantmyname.com)
2. Init a repo with a `_redirect` file, with a line like `/slug   http://example.com`, where the 1st arg is the relative path, and 2nd is where you want to redirect to
3. Setup a new site in [Netlify](https://app.netlify.com/start) and link your repo
4. Add your custom domain in "Domain Settings"

And thats it!

If you get some 'site not secure' errors, just wait a few hours for the domains and SSL certs to fully propgate thru DNS, but you should otherwise be good!

Bonus steps:

- add `netlify-shortener` as a dev dependency to be able to auto-format when adding new links
- add `netlify-shortener` as a shell alias to be enable creating quick short links from the cli
