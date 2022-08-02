---
# multilingual page pair id, this must pair with translations of this page. (This name must be unique)
lng_pair: id_homelab_essay
title: "Homelabbing as a hobby"

# post specific
# if not specified, .name will be used from _data/owner/[language].yml
author: Sean Rettig
# multiple category is not supported
category: homelab
# multiple tag entries are possible
tags: [homelab, infrastructure]
# thumbnail image for post
img: ":homelab_pic.jpeg"
# disable comments on this page
#comments_disable: true

# publish date
date: 2022-08-02 10:04:30 -0500

# seo
# if not specified, date will be used.
#meta_modify_date: 2022-01-01 10:04:30 +0900
# check the meta_common_description in _data/owner/[language].yml
#meta_description: ""

# optional
# if you enabled image_viewer_posts you don't need to enable this. This is only if image_viewer_posts = false
#image_viewer_on: true
# if you enabled image_lazy_loader_posts you don't need to enable this. This is only if image_lazy_loader_posts = false
#image_lazy_loader_on: true
# exclude from on site search
#on_site_search_exclude: true
# exclude from search engines
#search_engine_exclude: true
# to disable this page, simply set published: false or delete this file
#published: false
---
<!-- outline-start -->

###### Preface
This essay was written for an English class in response to the prompt of describing a hobby.

<br>
<br>
Turning the key to your car and hearing your engine turn is such a mundane thing, isn’t it? Its such a common activity, you might not notice doing it. But imagine you had just spent hours putting together the engine in that car, and this was the test to see if your hard work has paid off. Perhaps you had saved that car from being trashed, bringing it back to your garage to spend some time on it. This was your project, and something you could reliably go out and work on. When it all comes together in the end, and you unveil your masterpiece, you feel proud, accomplished, and finally have something to show for all your hard work. Luckily, this journey isn’t exclusive to cars. In a similar way, a computer is a mundane thing to most people, and going to a website is a simple task. Yet, if you had designed that website, written the code, put together the services behind it, and deployed it, you would have that same feeling. The lifecycle of a website demonstrates one of the more complex things you can achieve through a homelab, as there are many more things you can do with one. 


The term homelab doesn’t obviously exemplify its meaning. One may think it is a place for science experiments at home, or maybe some crazy movie villain’s base, but it is much simpler than that. A raspberry pi is an extremely small computer that can be bought for around $35, and it qualifies to be the only thing that makes up your homelab. So does spending thousands of dollars on enterprise grade hardware to have fancy features such as high availability, remote management, and power redundancy. These are all part of the joy of having a homelab, as it can be anything you want. 


Many articles about homelabbing are geared towards someone unfamiliar with system administration, and talk about common services that people like to run. One such service is Shinobi, an NVR solution to connect cameras from around your house for monitoring. Another would be Nextcloud, a personal cloud similar to OneDrive or Google Drive, but hosted on your own equipment. These articles also detail how if you are new to Linux, an operating system commonly used in homelabs, you can use this opportunity for learning or breaking things. If, however, you are a sys admin or IT person for your career, you may be familiar with many concepts in a homelab and want to have something at home to practice with. This way, you do not have to worry about messing up anything critical in the infrastructure set up at your workplace. There are also many certifications that you can get for working with Linux or networking such as the GIAC Certified Unix Security Administrator or Cisco CCNA certification. Preparing for the certification exams can be made easier by setting up suitable environments within a homelab These few descriptions of a homelab’s use have been very broad, as what constitutes a homelab can vary widely, but I can get specific with what I do in mine. 


My homelab has changed a lot over the years as I have learned more about what I want to do with it. My idea of a homelab has gone through the same evolution as the hardware that makes it up, but we’ll focus on the former for now and go over the specifics of the infrastructure in a later section. When I first started, I didn’t exactly have any idea of what a homelab was; I simply wanted to host a Minecraft server to play with friends. I really enjoyed being of some sort of service to my friends, especially when it came to technology. I had always offered to fix computers and various devices for them, but it felt good to orchestrate some kind of magic for friends to have fun- not to mention I could join them! Soon after setting up the server, I found out about the hobby itself, and my eyes were opened to all the possibilities. There were so many services that you could run I was overwhelmed, but that’s one thing that’s amazing about it: you can do anything! Another part I enjoy about setting up the services, is the feeling of pride. I may have followed a tutorial, but I put together all the pieces and created something amazing. I set up a Plex server (detailed later) after the Minecraft server, and boy am I proud of the product. After that, my interpretation of a homelab has culminated into a desire to take control of my privacy. If I stored a file on a cloud server, I have no idea who or what also has access to it, despite what the company might say. I would rather keep all my data close at hand. These have combined with my desire to create things by myself to form my understanding and appreciation of a homelab.


As said before, my actual homelab has changed just as much as my idea of it. The start of my journey is difficult to remember exactly, but I believe the first computer I used to host something on was my friend’s old computer he sold me around February of 2019. My interest in computers started much before then, but that was when I first had a device I wasn’t actively using with Windows. It was then I was introduced to Proxmox, an operating system I use to manage and deploy virtual machines on my computers without them having a monitor attached to them. A virtual machine is essentially a virtualized computer within a computer, so, for example, I could have windows running on a machine without it actually being installed on that computer. As opposed to a “bare metal” install, virtual machines are useful because you can run many of them on a single computer. Proxmox allows me to see these virtual machines on a webpage, making it easy to manage what is running. When I speak of running a service, I mean that I have a virtual machine going with that specific service running. What makes a computer a server, is that it is (mostly) always on and ready for anything to connect to it to use its computing power. I had also acquired a small rack that would allow me to store these servers in a better looking way than a bunch of computers piled in a corner. These racks have special places in the front and back to bolt in servers depending on if they support the ability to be rackmount. Then, in June of 2020, I bought 2 older but still quite capable enterprise-grade servers to add to my infrastructure to upgrade from the consumer computer I had before. Unfortunately, they were too big for the server rack, and sat atop it for the better part of a year, until I finally found a full-sized server rack at Purdue salvage. It was quite a task to get it home and into the house, as this is not a small piece of kit. It was almost too big, but I prefer to see it as future proof, meaning however much more equipment I acquired, it would fit in the rack. I still ran the Minecraft server, but I also set up something called Plex, a program that allows you to stream video files from home in a Netflix style fashion. I realized I could copy all the DVDs and Blu-rays I had so I could watch them from anywhere. Eventually, I had ripped so many movies that I realized I needed more storage, so I got one of my dad’s old work computers, put some hard drives in it, and created my first NAS (Network Attached Storage). It is a storage server that I can write to and read from over the network, and if I turn my computer off, I can still access the storage from a different computer. However, I soon realized that I was going to need more storage with the ever-increasing number of movies I had, so I bought a few more hard drives and new server to hold them all. I also realized a while ago that I should buy a UPS (uninterruptable power supply) to provide battery backup to my servers if the power goes out. A power outage can be damaging to computers, so it is a good idea to restrict their occurrence as much as possible. As of right now I have not installed the UPS, but it is waiting at home for me to do so. My journey is specific compared to how I have previously described homelabbing, but that perfectly exemplifies the seemingly endless possibilities of a homelab. 


As I progress towards the future, I have been looking into deploying what’s called a Kubernetes cluster. It’s something I don’t fully understand yet, but it is basically a distributed, self-healing, self-scaling deployment system. If I needed more computing power, it would scale itself up, and if one of the deployments broke, no services would be interrupted. I also have many other services that I would like to get up and running. One of these services is home assistant, an open-source automation tool that can connect all of the smart devices in your home so they can communicate with each other. Another service is called Paperless-ng, a solution for going paperless at home and storing as many of your former paper documents within the reach of any device. I have many more things that I want to get up and running, but it is difficult to work on this while also getting schoolwork done. I do as much of it as I can in my free time.


It can be hard to see why having a homelab is important at all, especially if you don’t necessarily lend yourself to being too technical. This is definitely true for some people, and that points out the fact that a homelab isn’t for everyone, but it doesn’t discount the importance of the hobby itself. I have already outlined a few uses of a homelab, but that list goes on and on for the multitude of things that people have done with their own computers. You may think that all of these things can be handled by buying it from some company and having them handle all of this for you. And you can, but the same can be said for painting a room in your house, DIYing the backsplash in your kitchen, or even cooking your own food. Some people may not have the money to pay for those services, and others just feel like learning and doing something themselves. That is what is important about this hobby. It can teach many skills that can be used in the real world with so many cool applications. Yet, if you still find having a homelab not exactly for you, that’s ok! However, you can still benefit from having a friend interested in all of this. Maybe they can run your website for you, or at the very least help you out when a computer of yours just broke while outside of its warranty.


Homelabbing is an extremely expansive hobby, which lends itself to having something for almost everyone. You can go as deep or as shallow as you want and you wouldn’t receive much judgement. No matter how small your homelab might be, there are people online who respect it for what it is and want to help you learn enough to get to your end goal. I think that is one of the important parts of this hobby, if you feel stuck, it is incredibly easy to ask for help. Many people say that the only real limits are the power bill and spousal approval, but being single and living at my parent’ house exempts me from that. There is something to be said about DIY, but I feel this hobby takes it to the extreme because of the possibilities, transferrable skills, and opportunity for fulfillment. Working on my homelab has been a big part of my life, and I firmly believe I will do it until I die.