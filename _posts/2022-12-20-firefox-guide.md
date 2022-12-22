---
layout: post
title:  "Firefox Tracking Protection Guide"
subtitle: "How to Protect Your Browser from Trackers"
date:   2022-12-20 12:00:00 -0700
categories: user-guides
---

This document was completed as the final requirement for the Technical Writing Certificate at Bellevue College, Technical Writing Capstone, Fall, 2022.

# Contents
[1  Introduction](#1-introduction)

[1.1	What Is tracking?](#11-what-is-tracking)

[1.2	Cookies](#12-cookies)

[1.2.1	Third Party Cookies](#121-third-party-cookies)

[2	Firefox Settings](#2-firefox-settings)

[2.1	Search](#21-search)

[2.2	Privacy and Security](#22-privacy-and-security)

[2.2.1	Permissions](#221-permissions)

[2.2.2	Security](#222-security)

[2.3	What Should I Do If Enhanced Tracking Protection Breaks a Site?](#23-what-should-i-do-if-enhanced-tracking-protection-breaks-a-site)

[3	Add-Ons](#3-add-ons)

[3.1	Can Add-ons Be Trusted?](#31-can-add-ons-be-trusted)

[3.2	How to Install an Add-On](#32-how-to-install-an-add-on)

[3.3	Disabling an Add-On](#33-disabling-an-add-on)

[3.4	uBlock Origin](#34-ublock-origin)

[3.4.1	Disable for Certain Websites](#341-disable-for-certain-websites)

[3.5	Facebook Container](#35-facebook-container)

[3.6	Firefox Multi-Account Containers](#36-firefox-multi-account-containers)

[3.7	Privacy Badger](#37-privacy-badger)

[3.7.1	Disable for Specific Sites](#371-disable-for-specific-sites)

[3.7.2	Adjust Blocked Domains on a Site](#372-adjust-blocked-domains-on-a-site)

[4	Browsing](#4-browsing)

[4.1	Rejecting Cookies from a Site](#41-rejecting-cookies-from-a-site)

[4.2	Requesting Sites not to Sell Data](#42-requesting-sites-not-to-sell-data)

[4.3	Browsing with Containers](#43-browsing-with-containers)

[5	Disclaimer](#5-disclaimer)

# 1 Introduction
In today’s internet-driven world, many major companies that do business online such as Google and Meta rely on collecting users’ browsing data for advertising. Websites can even collect data about your browsing after closing the site.

Mozilla Firefox is a web browser with features designed to prevent invasions of privacy. If you consider it an invasion of privacy to track your browsing habits for advertising purposes, this guide can demonstrate how to take advantage of these features to minimize the risk of websites tracking you.

## 1.1 What Is tracking?
“Tracking” refers to the methods websites use to collect data on users’ browsing habits. Generally, companies will use tracking to build user profiles, which allows them to show advertisements to users based on what the company think they want to see. These profiles include demographic information such as age, gender, and online activity. For instance, you might start to see more ads across all sites for an item after you search for that item on one site.

This guide focuses on protecting your browser from techniques some websites use to build profiles on their users.

## 1.2 Cookies
Cookies are small files a website stores on your device. The website can then use that information for various functions of the site. For example, online retailers use cookies to remember the items in your shopping cart. Other sites might use cookies remember your username and password when you click “Remember me” after logging into a website.

### 1.2.1 Third Party Cookies
Although most cookies are benign, some “third party” cookies can track your browsing activity across multiple websites. Third party cookies are cookies that come from domains other than the domain you logged into.

For example, suppose you log onto an online retailer who shows you an advertisement served by Google, the company that owns the search engine of the same name. Google can now install cookies on your device to learn about your browsing habits, even if you never directly logged on to any site owned by Google.

These cookies are the reason many websites will show advertisements for products the user has seen before, even if the user has not visited the website before.

# 2 Firefox Settings
This section will show which settings to change in the browser to get the most out of its built-in privacy features.

Click the application menu button (pictured below) in the top right corner and click “Settings” to open the settings.

![Application Menu Button](/images/firefox_images/application_menu.png)

The following sections will explain which settings to change in each of the categories on the left side of the screen. Categories that do not have a section do not need any changes.

## 2.1 Search
Change your **Default Search Engine** to DuckDuckGo.

![](/images/firefox_images/duckduckgo.png)

DuckDuckGo is a search engine that collects no personal information or search history. DuckDuckGo is the best choice for privacy because most search engines collect user data.

## 2.2 Privacy and Security
Under **Enhanced Tracking Protection**, choose **Strict.**

![](/images/firefox_images/enhanced_tracking_protection.png)

Under “Send websites a “Do Not Track” signal that you don’t want to be tracked,” choose “Always”.

Under **Cookies and Site Data,** check “Delete cookies and site data when Firefox is closed”.

Checking this box may make sites less convenient. For example, this will cause sites to delete your saved username and password even if you want the site to automatically log in. To allow Firefox to save cookies from trusted sites, click **Manage Exceptions…**

A new window will appear. In the “Address of website” bar, enter the name of the trusted website. Click “Allow.”

You can remove websites from the list by clicking the website’s name in the list and clicking **Remove Website.**

![](/images/firefox_images/cookie_exceptions.png)

### 2.2.1 Permissions
Ensure that “Block pop-up windows” and “Warn you when websites try to install add-ons” are checked.

![](/images/firefox_images/permissions.png)

By default, websites will not have access to location, camera, microphone, etc. unless you have explicitly granted it to the site.

### 2.2.2 Security
Check all three boxes under **Deceptive Content and Dangerous Software Protection**.

Check the box under **Certificates.**

Under **HTTPS-Only Mode**, check “Enable HTTPS-Only Mode in all windows.”

## 2.3 What Should I Do If Enhanced Tracking Protection Breaks a Site?
If you notice a site is not working properly because of Enhanced Tracking Protection, click the shield icon in the address bar. Then click the slider as shown below.

![](/images/firefox_images/disable_enhanced_tracking_protection.png)

# 3 Add-Ons
Some add-ons can boost the privacy of your browsing by blocking trackers in certain sites. This section will explain how to install and use add-ons. It will also suggest specific add-ons to block tracking.

Although many add-ons are available for privacy purposes, they often perform the same function as each other. Installing too many add-ons may be redundant. The add-ons suggested in this guide cover the most important vulnerabilities with minimal redundancy.

## 3.1 Can Add-ons Be Trusted?
Although some add-ons contain malware, this guide only recommends 100% open-source add-ons. This means anyone can view the source code, making it impossible for developers to slip trackers or other malware of their own into the add-on.

On Mozilla’s add-ons site, certain add-ons are marked with the symbols below. Respectively, these are Mozilla’s stamp of approval and a badge for add-ons made by Mozilla themselves. The organization only gives the former to add-ons they trust.

![](/images/firefox_images/recommended.png) | ![](/images/firefox_images/by_firefox.png)

## 3.2 How to Install an Add-On
Mozilla allows users to download add-ons from [addons.mozilla.org](https://addons.mozilla.org/).

To install an add-on:
1. Navigate to page of the add-on you want to install on addons.mozilla.org. Links are provided in the following sections.
2. Click on “Add to Firefox.” A dialogue box will appear that lists the permissions the add-on needs.
3. Click “Add” in the dialogue box.

![](/images/firefox_images/addon_page.png)

## 3.3 Disabling an Add-On
If you ever need to disable an add-on without uninstalling it,
1. Open the application menu, then click “Add-ons and themes”. Alternatively, press Control+Shift+A. A full list of installed add-ons should appear.
2. Click the slider next to an enabled add-on to disable it.

![](/images/firefox_images/disable_addon.png)

## 3.4 uBlock Origin
uBlock Origin (UBO) is an add-on that blocks advertisements, tracking cookies, and popups. Although many users know it as an ad blocker, it blocks a wide range of malicious or just annoying website elements.

To install, navigate to the [uBlock Origin page](https://addons.mozilla.org/en-US/firefox/addon/ublock-origin/) from Mozilla and install using the instructions in [3.2](#32-how-to-install-an-add-on).

UBO works immediately after installation, but you can optionally change settings for a better experience.

### 3.4.1 Disable for Certain Websites
Some websites, such as news sites will not work properly with UBO because they do not allow ad blockers on their site.

In these cases, UBO can be disabled by:
1. Navigate to the website you want to browse.
2. Click the UBO icon in the toolbar.
3. Click the power button in the UI as shown below. A refresh button will appear next to it.
4. Click the refresh button that appears.

![](/images/firefox_images/disable_ubo.png)

## 3.5 Facebook Container
Meta (formerly Facebook) uses trackers heavily across its services. Even the “like” widgets you see in non-Meta sites can get data about you.

This add-on makes it so that Meta services cannot interact with other tabs and blocks Meta content on non-Meta websites. It does not need any additional configuration once you install it.

Be aware that installing this add-on will immediately
- close all tabs of Meta sites,
- delete all cookies from Meta sites, and
- log you out of all Meta sites.

To install, navigate to the [Facebook Container add-on page](https://addons.mozilla.org/en-US/firefox/addon/facebook-container/) and install using the instructions in [3.2](#32-how-to-install-an-add-on).

## 3.6 Firefox Multi-Account Containers
Firefox has a built-in feature called containers that allow you to separate tabs with different purposes into different containers. Tabs in a container can only interact with tabs open in that same container. For example, if you have Amazon.com open in a container, the cookies installed by that tab cannot see tabs outside the container. This is a great feature to use when sites have necessary cookies to install but you do not want them to see your other browsing activity.

To install, navigate to the [Multi-Account Containers add-on page](https://addons.mozilla.org/en-US/firefox/addon/multi-account-containers/) and install using the instructions in [3.2](#32-how-to-install-an-add-on).

## 3.7 Privacy Badger
Privacy Badger locates and blocks trackers from sites you visit. While UBO draws on a fixed list of blocked domains, Privacy Badger detects and blocks tracking dynamically. In other words, it can catch what UBO misses.

Like UBO, Privacy Badger works immediately after installation, but can be adjusted based on your preferences.

To install, navigate to the [Privacy Badger add-on page](https://addons.mozilla.org/en-US/firefox/addon/privacy-badger17/) and install using the instructions in [3.2](#32-how-to-install-an-add-on).

### 3.7.1 Disable for Specific Sites
Some sites that do not allow ad blockers view Privacy Badger as an ad blocker. If you ever want to disable Privacy Badger for specific sites,

1. Click the Privacy Badger icon in the toolbar. The privacy badger widget will appear.
2. Click “Disable for this site” in the widget.

![](/images/firefox_images/privacy_badger.png)

### 3.7.2 Adjust Blocked Domains on a Site
If you open the Privacy Badger widget, you will notice a list of domains with sliders next to each domain. If you want to allow all content from a domain, move the slider to the right. To block cookies from a domain, move the slider to the middle. To block all content from a domain, move the slider to the left.

# 4 Browsing
This section explains how to browse securely using the features and add-ons in this guide.
## 4.1 Rejecting Cookies from a Site
According to European law, users must give consent to a website before it can collect data. This is why you’ve likely seen notices on websites that inform you on how they use cookies.

You may have seen banners at the bottom of certain sites asking you to accept or reject cookies. Each site’s banner will look different from the others, but generally they will have an option to accept all cookies and view more options.

As an example, see the screenshot below from Pocket.

![](/images/firefox_images/reject_cookies.png)

Click “Manage”. Accepting the cookies immediately might allow trackers.

![](/images/firefox_images/cookie_settings.png)

Click “Reject All”. This will reject all cookies except the ones necessary for the site to function.

Remember that this is only an example. Different sites will look different or use slightly different terms.

## 4.2 Browsing with Containers
Ensure that the Multi-Tab Containers extension is installed before using containers.

Using containers isolates tabs from each other, allowing you to have different online identities for different purposes. For example, you can keep all your shopping tabs in one container so that they cannot interact with tabs outside the container.

1. Right click on the new tab icon next to your open tabs. A menu of containers will open.
2. Select the container you would like to open the new tab in.

A new tab will open in the container, and you can now browse as normal.

# 5 Disclaimer
Following this guide does not guarantee complete privacy on the internet. This guide does not apply to mobile devices. Websites that you visit may still identify you and your device. To prevent this, a VPN can help.

Although the instructions above block third party cookies, they do not prevent first party cookies (or cookies that come directly from the sites you visit) from seeing your browsing.

This guide also does not protect against hackers or anyone who wants to steal passwords, credit card numbers, social security numbers, email addresses, etc. Always create strong passwords and never share personal information with a site you do not trust.

# References

“gorhill/uBlock.” GitHub. Accessed November 16, 2022. https://github.com/gorhill/uBlock/wiki.

“Multi-Account Containers.” Firefox Help. Accessed November 16, 2022. <https://support.mozilla.org/en-US/kb/containers>.

Privacy Badger. Accessed November 16, 2022. <https://privacybadger.org/>.

“Trackers and scripts Firefox blocks in Enhanced Tracking Protection.” Firefox Help. Accessed November 16, 2022. <https://support.mozilla.org/en-US/kb/trackers-and-scripts-firefox-blocks-enhanced-track>.
