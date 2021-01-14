---
layout: post
title: "Figuring Out Hostinger VPS"
subtitle: "Pretty sure I'm making progress."
date: 2021-01-13 09:25:13 -0400
# background: '/img/posts/01.jpg'
---

<p>So I'm not sure I'm all the way there, but I think I'm making progress. I reinstalled the OS on the hostinger vps. I used Ubuntu 18.04 with the LAMP stack, Webmin and Virtualmin already installed. When it finished installing, I tried creating another user terry, but then figured out that hostinger's install had already created a user called terryinfcco. This user has a public_html directory already created and the permissions, etc. all set. So all I have to do is connect with FileZilla to sftp, user terryinfcco. Then uploading to that directory makes everything work. </p>
<p>I also set up ssl. I never got the ssl cert that I bought to work, but I did follow a guide they set up to install a free certificate from Let's Encrypt. Only problem is that it only lasts 3 months, so I'm going to have to regularly re-install it. But better than nothing!!</p>
<p>Working on customizing jekyll with the minima theme. But much of what I want is in the newest version of the minima theme (3.0) and the newest version I can get is 2.5.1 from rubygems. So tomorrow I think I'll work on forking the minima github repository and see if that gets me version 3.0.

