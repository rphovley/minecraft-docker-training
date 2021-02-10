# Minecraft - Docker

# Part 1

## Why do this?
Git gud at dev ops, networking and docker bruh

[POWERPOINT! (Part 1)](https://docs.google.com/presentation/d/16L7liqKqTfs161wQUxcd1Dp97tZNQeYBsvnLHHkPkO8/edit?usp=sharing)

## Let's make a minecraft docker image!

I followed [this wiki](https://minecraft.gamepedia.com/Tutorials/Setting_up_a_server) to set this up.

1) We need to make our minecraft server "blueprint" or image. Create a `Dockerfile` by making a new file with the name `Dockerfile` in the root of your project.
2) Add Java FROM statement: [What version?](Installing_Java.png)
3) *[Potential Optimization](JRE_vs_JDK.png)*
4) Add command to add curl to image (for minecraft server download)
5) Add command to download minecraft server app [Download](https://www.minecraft.net/en-us/download/server/)
6) Add command to copy minecraft config files 
7) Add command to run minecraft server app
8) Test!

## Make a docker-compose file!
1) Add version and services blocks to yml
2) Add name 
3) Add build path (could use image name for things we don't need to build locally)
4) Add volume (what does this do for us? Won't do this today)
5) Run it!

But, if we open up minecraft, could we connect to this server?


# Part 2


## Concepts
- Linux Users
- SSH
- Docker
- Docker-compose
- Server (script/program bound to a port or set of ports)

##
- Infrastructure highlights two skills of programming
  - Memorization: language syntax, library/tool function calls and how they work, infrastructure/environment impact (errors related to operating system you're running)
    - What tools do I have available to solve problems? (node, python, docker, routers, google cloud)
    - How do those tools work?
    - How do those tools work with each other? (How does node interact with redis? How does Angular work with local storage)
    - What environments do they work within? (Firefox on mac vs ie11 on windows)
  - Patience
- Infrastructure
  - Why should I care?
    - When we talk about our programming "environment" what are we talking about?
      - "os and version, libraries/packages and their version, networing, even data (db, caching, etc...)
    - Development is a creative process. It's important to know how your process might change as the 'canvas' you create on changes. (i.e. different package versions, os, etc...)
    - Infrastructure bugs (believe or not, they write bugs too)
    
- Docker
  - Why?
    - Works on my machine
    - [vs VM](containers-vs-virtual-machines.jpg)
    - Create the same "environment" or infrastructure your code runs on every single time
      - Imagine writing a feature using a package that isn't supported by the OS the server runs on and not finding that out until it gets merged
  - Image
    - Blueprint:Dockerfile
  - Container
    - House:Container
  
- Networking
  - [Protocol Stack](https://en.wikipedia.org/wiki/Protocol_stack#:~:text=The%20protocol%20stack%20or%20network,the%20software%20implementation%20of%20them.)
    - Physical layer (not important)
    - Data Link (not important)
    - Network (Focus, focus)
      - ip addressing
      - ports
      - routers
      - domain name servers

