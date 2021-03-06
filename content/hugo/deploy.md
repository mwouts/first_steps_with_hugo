---
title: Hosting the site
---

There are [many ways to deploy](https://gohugo.io/hosting-and-deployment) the resulting site.

I gave a try to Netlify as that method offers continuous integration. I followed Hugo's documentation about
[Hosting on Netlify](https://gohugo.io/hosting-and-deployment/hosting-on-netlify/), and used `hugo -D` as the 
command to build the site, and `public` as the publish directory:

![](../netlify_build.png)

Then, all I had to do was to change the site domain to [https://my-first-steps-with-hugo.netlify.com/](https://my-first-steps-with-hugo.netlify.com/)

![](../netlify_domain.png)

Then I realized that the rendering of the website on Netlify was not exactly matching the one I was seeing locally. Thus I fixed the version of Hugo used by Netlify with
a `netlify.toml` file with the following content:
```
[context.production.environment]
  HUGO_VERSION = "0.62.2"
```
