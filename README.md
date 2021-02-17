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

## [POWERPOINT](https://docs.google.com/presentation/d/1Y5Di3UIOWMp6MSwGh2IKszgQE4hC50w12RURRtDXv6U/edit)

## Compare Dockerfile/Dockercompose file to previous
- "EXPOSE 25565" 
  - need to bind minecraft server app to the container port. If it doesn't get a port assigned, it will not be available in the network
    - lsof -i tcp:25565
    - Why isn't it showing?
  - port forwarding
    - Add -p 25565 to docker run command

## Digital Ocean Server

-


##

