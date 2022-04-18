---
title: "Google Apps Script to automate mundane tasks"
description: "The power of google apps script and how I used it to get more free time"
date: 2022-04-18
publishDate: 2022-04-18
author: "Lorna Jacob"
images: []
draft: false
tags: ["google-apps-script", "javascript"]
---

Google Apps Script is a cloud-based JavaScript platform that lets you integrate with and automate tasks across Google products. It has built-in libraries for Google Workspace applications like Sheets, Gmail, Calendar, Drive, and more. You don't need to install anything to get started — Google gives you a code editor in the browser, and the scripts you write runs on Google's servers.

What can Apps Script do?

Apps Script is versatile. Among other things, you can:
- Add custom menus, dialogs, and sidebars to Google Docs, Sheets, and Forms.
- Write custom functions and macros for Google Sheets.
- Publish web apps — either standalone or embedded in Google Sites.
- Interact with other Google services, including AdSense, Analytics, Calendar, Drive, Gmail, and Maps.
- Build add-ons and publish them to the Google Workspace Marketplace.

If you are interested to learn more 👉 [read from Google overview page itself.](https://developers.google.com/apps-script/overview)

I wrote a mini side project to use the apps script for automating my monthly budget monitoring task. Every month, I download my Credit Card statements in CSV format from my bank, open up my Google Sheet, paste the transactions there, and then categorise my expenses one by one, generate nice charts and pivot tables, and compare how I did financially vs last month. On a nice day, it would take me about an hour to finish this. Early this year, instead of spending an hour doing the same thing again, I instead googled how I can automate this mundane task using Google Sheets. In my good ol' days, I used to write macros in MS Excel to do same stuff, so I thought what are the odds Sheets has the same functionality. And alas, I discovered Google Apps Script.

In a nutshell, here's what I did:
- In my budget sheet, I added a custom menu to allow me to import the Credit Card statements from my Drive. (Now, getting the CSV from bank to Google Drive is still manually done by me :D) 
- I then written functions that will extract the data from csv file once the import is successful and present the data nicely in a new sheet.
- Then it iterates each row and categorizes them based on the merchant name.
- Voila! It's done in about a minute or less.

If you want to see the code (warning! it's a bit rubbish), you can checkout my Github repository. I hope you learn something and get inspired to start exploring the Google Apps Script too.