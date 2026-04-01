---
layout: post
title:  "Latest Website Changes"
date:   2026-03-31 10:20:00 -0500
categories: [homelab, website]
tags: [homelab, website, jekyll]
---

So I have released a new version of my website. It has a brand new design and feel along with some significant backend changes. Let's discuss how this site began, how it was configured in the past, and where we are now.

## The Beginning

This website began as a little side project that I had made for myself. I had just finished an intro to web design course and wanted to test my skills with hosting the files on my own. I had been using proxmox for a while at that point, so I spun up an LXC container, installed NGINX, looked up some hardening guides and got to work.

After setting my domain up with Cloudflare and changing some port forwarding settings on my college apartment router, I was hosting the website I had created for class on a sub-domain. I quickly found an HTML template for a "Quick Links" style of page that pointed to various things, like my GitHub and LinkedIn, and put it up on my domain. I went from zero hosting experience to hosting 2 different websites on the same web server.

## Progression

The next semester I had another course in which the major project we were tasked with was creating and publishing an interactive version of our resumes. This had to be something public facing that people could interact with, and I already had the base I needed to get going. While others were attempting to find a solution, I was working on improving my website.

I made some major changes. I found a more advanced HTML/CSS/JavaScript template that incorporated smooth scrolling and responsive design. I filled things out within the template, and wasn't completely happy with what I made, so I made some modifications to the template to more fit my style. Also, after a move, I had to move the webserver off my personal infrastructure and onto a VPS service as I had lost the ability to port forward due to CGNAT.

## The Present

As time has progressed, I have had less and less time to focus on managing my website front-ends and its constant progressing changes. Even though I was using a template, it was still becoming rather difficult to keep up with modifications. As a result, the website stayed in a similar state for a couple of years with no changes.

As I got more and more into cybersecurity, I realized how important it is to keep track of all systems to ensure that they stay up-to-date with the patches to mitigate any vulnerabilities, especially with something that is web-facing and open to the internet. I also realize that logs need to be looked at consistently to ensure that nothing nefarious is occurring. This is something that I have been severely lacking on in my personal life.

So here we are with a change. I decided to start using the static site generator [Jekyll](https://jekyllrb.com/), more specifically the [Chirpy](https://github.com/cotes2020/jekyll-theme-chirpy) theme to resolve my issues with managing my frontend. This also works really well with my decision to use [GitHub Pages](https://docs.github.com/en/pages) for my backend. By moving to GitHub Pages, I am offloading the backend infrastructure to a platform that handles security and maintenance for me. This aligns with the cybersecurity risk management principle of transference — shifting the burden of risk to a third party better equipped to handle it.

I am excited to use the blog to showcase things I am working on and to keep this site updated.
