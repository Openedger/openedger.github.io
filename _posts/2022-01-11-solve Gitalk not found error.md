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

But the original comment plug-in:Disqus is a paid service, so I tried another popular comment tool:[GiTalk](https://gitalk.github.io/).Everything is fine until I met with "Not Found" Error when I deployed.

The followings are the steps to solve this "Not Found" error when activating gitalk on your webpage:
1. Create a new github repo for comments storage
2. Enabling the "issues" of this repo,and activate the "issue"
3. Configure the OAuth Apps in Github Apps setting
4. Configure the "repo" of gitalk js code without "https://" ,
like this:  repo: blog-comments   
