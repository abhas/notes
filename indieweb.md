---
date: 2020-08-06
tags:
  - indieweb
---

# IndieWeb Links

> "We should all own the content we're creating, rather than just posting to third-party content silos. Publish on your own domain, and syndicate out to silos. This is the basis of the "Indie Web" movement."

I chanced upon the world of IndieWeb and microformats while trying to search for a system to publish short notes (neuron is something I discovered in this process). Here is a summary of the research:

## What is the IndieWeb?

The [IndieWeb website and wiki](https://indieweb.org/) is very thorough and detailed. Though a bit difficult to read at first *(its full of outbound links and so requires patience to really get a feel of the while field)*, it is a great resource.

### Steps to get started:
*(Borrowed from the IndieWeb wiki)*

1. [Get a personal domain](https://indieweb.org/Getting_Started#Get_a_personal_domain):
	Builds identity, makes it easy to search for you.
2. [Find a place to host your content](https://indieweb.org/Getting_Started#Get_a_place_for_your_content):
  	You can host on a git repo (eg. github, gitlab etc), on a virtual server, a single-board computer or anywhere else.    
3. [Set up your home page](https://indieweb.org/Getting_Started#Set_up_your_home_page)
    - Mainly: [Set up web sign-in on your own domain](https://indieweb.org/How_to_set_up_web_sign-in_on_your_own_domain)  ... so that you can use your own identity on the IndieWeb
4. [Add info about yourself](https://indieweb.org/Getting_Started#Add_info_about_yourself): You can use microformats to add information about yourself so that when someone mentions you, they get it all in a structured / standard manner.
5. [Add links to existing social media](https://indieweb.org/Getting_Started#Add_links_to_existing_social_media): So that you can cross-post, hyperlink your posts and most importantly, own and self-host your content and not hold it captive to a 3rd party silo.
6. [Publish content on your domain and add microformats to your content](https://indieweb.org/Getting_Started#Add_microformats_to_your_content)
7. [Syndicate your content](https://indieweb.org/Getting_Started#Syndicate_Elsewhere): You can now post only to your own domain and have that content reach your existing social media accounts.

## [Microformats](https://microformats.io/)

> Microformats are a simple way to add more meaning to your HTML.

<http://microformats.org/wiki/Main_Page>

## Tools

Implementing these steps is a lot of very tough work. Using tools that do these things makes it simpler.

### [Transformative](https://github.com/barryf/transformative)

- IndieWeb personal website software
- written in Ruby
- Supports "notes, articles, bookmarks, photos and more"
- Developed by [Barry Frost](https://barryfrost.com)

This is one of the best tools I found. You can see it live on the developer's website. It handles most things for you so you can focus on the content.

### [Micro.blog](https://micro.blog/)

Micro.Blog is unique service that enables you to post to the IndieWeb. MicroBlogs can be mirrored to our own domains and they provide an interface to do the posting.

As an additional feature, [MicroBlog supports ActivityPub](https://help.micro.blog/2018/activitypub/) as well. So while you post using microformats, you can also federate your content via ActivityPub and have people follow you from Mastodon, for example.

They are also writing a [book about "microblogging"](https://book.micro.blog/). Read [the drafts here](https://github.com/microdotblog/indie-microblogging).

- Source code: <https://github.com/microdotblog>

### [Microblg.pub](https://docs.microblog.pub/)

Microblog.pub is unique: It serves ActivityPub primarily but supports the IndieWeb equally. It is designed as single-user tool and does not use javascript **ANYWHERE** (very very unique).

- <https://a4.io/>: The developers' own MicroBlog.pub instance

### <https://micropub.rocks/>

This website gives you a comparitive report about the status of micropub implementation status on servers and clients. Good way to discover servers & clients that you could use!

### [Sitewriter](http://sitewriter.net/)

Sitewriter is a tool that helps you add IndieWeb services to your static webite. Check out the documentation, [service](http://sitewriter.net/) and [source code](https://github.com/gerwitz/sitewriter).

### [Bridgy](https://brid.gy/)

Bridgy is a service (and software) that helps you connect your website to your social media accounts.

### [Quill](https://quill.p3k.io/)

Quill is a simple tool that support IndiaAuth and then lets you compose and make posts to your website.

### [Wordpress with IndieWeb](https://wordpress.org/plugins/indieweb/)

Wordpress is said to have one of the best and most mature IndieWeb implementations. If you use Wordpress, check it out.

- [Source Code](https://github.com/indieweb/wordpress-indieweb)

### [IndieWebify](https://indiewebify.me/)

This website and tool walks you through the process of IndieWeb-enabling your website. Its a great way to not just understand the steps involed but also test out if you have implemented them correctly on your website.

## Lets try this out together...

I am yet to try this out myself... but, at least, now I have some clarity on what to do and why and what to expect out of that process. So lets try this out together...