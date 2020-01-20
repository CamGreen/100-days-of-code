# 100 Days Of Code - Log for Cameron Green

### Day 1: 15 January 2020

**Today's Progress:** Today I decided to fix an internet GIS application I developed back in 2018 using OpenLayers for production. First thing I did was reinstall Node.js & npm with OpenLayers, this took a little longer than expected because I could remember how to do it correctly so had to spend a bit of time reading. Eventually got it to work when I selected the correct directory using `mkdir new-project && cd new-project`. Once this was correctly installed, the code worked. 

The first thing I tried to fix was the spatial layers that were no longer being displayed. The error came from the url being used to call the layers was incorrect. I fixed this and discovered a new error. The new error I was getting is a `net::ERR_NAME_NOT_RESOLVED`. To resolve this I needed to to update my nameservers with my domain registrar. This didn't happen as I could not log into my domain registrar account, don't know why. Trying to fix that now. 

**Thoughts:** A little annoyed about this, took me longer than it should have to figure it out but now I know for next time in case I get the same error one day in the future. Hopefully will get to fixing this issue in the next 100 days. Feel I reconnected with OpenLayers again today which is a big plus for an aspiring GIS Developer. 

**Useful Link(s):** OpenLayers - Basic project setup using NPM and Parcel: https://openlayers.org/en/latest/doc/tutorials/bundle.html 

**Link(s) to work:** Coming soon. 

### Day 2: 16 January 2020
**Today's Progress:** The first thing I did today was finally get round to encrypting my server. Have been putting that off for some reason but fianlly did that and it was easy enough. 

Later I worked yet again on the OSM application I worked on yesterday. Managed to fix the net::ERR_NAME_NOT_RESOLVED error and managed to get into my domain registrar account. Fixed the error of the spatial layers not displaying as they are displayed in development. The problem now comes in where I package the code for production and load it onto my server. 

The error I am getting is a `Mixed Content: The page was loaded over HTTPS, but requested an insecure XMLHttpRequest endpoint. This request has been blocked; the content must be served over HTTPS`. I sort of understand why I am getting the error I got. My server is HTTPS and the code I used to call my layers is `http://camcode.xzy.......`. When I changed the code to `https://camcode.xzy.......` I got another error which didn't understand. The error was `Failed to load resource: net::ERR_SSL_PROTOCOL_ERROR`. Another twist to the story is since my server is now HTTPS none of the layers in my GeoServer are displaying under Layer Preview. No idea how to fix any of this.  

Mixed Content Error:

![HTTPS_Error](https://github.com/CamGreen/100-days-of-code/blob/master/images/HTTPS_Error.png)

SSL Protocol Error:

![SSL_Error](https://github.com/CamGreen/100-days-of-code/blob/master/images/SSL_Error.png)

**Thoughts:** A little disappointed with all of this but at the same timw, I am okay with it because I am learning. Hoping to find some GeoServer experts that can help me. If you are reading this and know what the issue is or have any suggestions/comments, please let me know. Really would like to work this out. 

**Link(s) to work:** https://camcode.xyz/osm_visualise/

**Side Note:** Learning how to write in Markup more and more each day. 

### Day 3: 20 January 2020

**Today's Progress:** Took the weekend off to regroup myself. Started again fresh today. 

Decided I would start from the basics and relearn GitHub. I did a course on it a while ago but couldn't remember a thing so I needed to do it again to be able to use it again properly. Did a simple FreeCodeCamp.org course that was divided into three sections. 

In section 1, I covered creating a repo, connecting it to my VS Code, cloned my repo, edited it and pushed it to my repo. In section 2, I covered branching and then in section 3 I covered creating and managing pull requests. 

Pushed this change in the log file based on everything I just learnt. 

**Thoughts:** Happy with myself about this. Something that is really imporant in coding and such a basic. Mastered it and now working towards bigger things. This video explained it very well and was easy to follow. 

**Useful Link(s):** YouTube Video from FreeCodeCamp.org on GitHub - https://www.youtube.com/watch?v=x0EYpi38Yp4&feature=youtu.be