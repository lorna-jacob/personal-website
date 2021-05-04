---
title: "Deploy static website using Netlify"
description: "Learn how to automatically deploy your website with every push to the Github repo."
date: 2021-05-01T15:00:00+01:00
publishDate: 2021-05-01T15:00:00+01:00
author: "Lorna Jacob"
images: []
draft: false
tags: ["web-development", "ci-cd"]
---

I have been using [cPanel](https://cpanel.net/) for hosting and editing my personal website in the past few years. It comes with a clean text editor for editing html and css files. The hosting fee for cPanel is also relatively cheap. Since my website's just for "fun", I chose the cheapest shared hosting plan from Namecheap. I do enjoy cPanel's editor because I prefer writing code rather than using the drag/drop functionality that other popular website content management systems offer. I just feel like I have more control over my website when I write the code. The only downside is that I am missing the source code history. I realised that this is very important for me since I enjoy experimenting on my website. So when my webhosting plan expired, I searched for other solutions and then I found [Netlify](https://www.netlify.com/).

Netlify is an all-in-one platform for automating modern web projects. You can use it to replace your hosting infrastructure, continuous integration, and deployment pipeline with a single workflow. It also allows you to integrate dynamic functionality like serverless functions, user authentication, and form handling as your projects grow.

Provided you already have uploaded your website's codebase in Github and created a free Netlify account, then automating the deployment is a breeze. 

How to use Netlify to deploy your websites:

1. Click 'New Site from Git' button in the Team Overview's page.
{{< figure src="/posts/images/new-site-button.png">}}

2. Connect to Git provider. 
Choose your provider and then a pop-up window will appear to authorize Netlify's access to your source control.
{{< figure src="/posts/images/pick-source-control.png">}}

3. Pick the repository which contains your website's codebase.
Use the handy search bar if you have a lot of repos
{{< figure src="/posts/images/choose-repo.png">}}

4. Configure site settings and deploy.
Configure settings like branch to deploy, build command, publish directory. Once done, click 'Deploy' button.

5. Push changes to repo and see a deploy triggers automatically in Netlify. Congrats! You just created a Continuous Deployment pipeline for your website.

Github commit:
{{< figure src="/posts/images/github-commit.png" >}}

Netlify build and deploy progress:
{{< figure src="/posts/images/netlify-deploy.png">}}