---
layout: post
read_time: true
show_date: true
title: "solve Gitalk not found error"
date: 2022-01-11
img: posts/20210420/post8-rembrandt.jpg
tags: [general blogging, thoughts]
author: openedger
description: "how to handle with not found error when you deployed Gitalk for comment feature on your blogs"
---
I chose the Jekyll theme: [Adam Blog 2.0](https://github.com/the-mvm/the-mvm.github.io) as my github blog pages.The official guide is very clear and simple so that I can deploy my blog very fast.

![my new blog](./assets/img/template_screenshots/homepage-responsive.jpg)

![night theme toggle](./assets/img/template_screenshots/light-toggle.png)

But the original comment plug-in:Disqus is a paid service, so I tried another popular comment tool:[GiTalk](https://gitalk.github.io/).Everything is fine until I met with "Not Found" Error when I deployed.

![not found error](./assets/img/posts/20220111/GiTalk_error.png)

The followings are the steps to solve this "Not Found" error when activating gitalk on your webpage:
- Create a new github repo for comments storage

![create comment repo](./assets/img/posts/20220111/create_new_repo_comment.png)

- Enabling the "issues" of this repo,and activate the "issues" with first comment

![issues enabled](./assets/img/posts/20220111/issues_enabled.png)
![first comment](./assets/img/posts/20220111/create_first_comment.png)

- Configure the OAuth Apps in Github Apps setting

![app kid key](./assets/img/posts/20220111/clientID_key.png)
![set Oauth](./assets/img/posts/20220111/set_OAuth.png)

- Configure the "repo" of gitalk js code without "https://" prefix ,
just set it like this:  repo: blog-comments(repo name)

![Set repo name](./assets/img/posts/20220111/set repo.png)

Finally, you can see the perfect GiTalk tool on your webpage.

![enjoy](./assets/img/posts/20220111/correct_GiTalk.png)

Enjoy GiTalk!
