# **Proposal for GSOC 2019**

https://forum.kodi.tv/showthread.php?tid=342741

**PLAN:**

Building a website for submit addons to Kodi repo due to its convenience and accessibility on all sorts of devices. A command-line interface will encourage more errors and a Java UI is limited and I find it a bit clunky to implement with other tools.

**GOALS I wish to complete throughout this project**

Reduce the clutter of repos. This is probably the most important thing for me. I remember using Kodi through all of my years and always found the extra step of adding a repo to the File Manager tedious. Uploading the essential addons straight to the main Kodi repo will make the process more convenient and accessible.
Reduce the work load of developers by automating basic syntax checks. Not only developers will have less steps to worry about, this will encourage more people to create addons and give them a platform to share their hard work.
Better quality submissions. Since the website will also aim to offer suggestions to the code that will be committed on the client side, there are less chance of errors.

**IMPLEMENTATION**
1. I plan to use Django REST Framework for the back end, which will also be compatible with Android/iOS devices. For GitHub Authentication, according to my knowledge currently there is something like "social-auth-app-django" library which can be used to connect to GitHub and later branch it to Kodi's Github. 
1. I also seek to embed the Kodi add-on generator tool on the website as well and connect the folder to the user's personal github. The interface of the tool is very simple and I think with some knowledge and guidance, it can be easily implemented.
1. For the front end, theme wise I'm thinking about implementing something similar to Angular Material Starter SPA due to its simplistic look and interface, and obviously make it Kodi-themed  Wink

**CODE ANALYSIS**

I was thinking, wouldn't it be easier to use our very own Kodi's addon checker to check for new repository submissions? I'm sure it also includes code analysis as well, so it takes care of multiple issues all at once Smile I don't know how exactly I would go with implementing it, so any suggestions will be great Smile 
If not, I think someone mentioned in another thread CodeMirror is a great open source editor with syntax-highlighting so it is a great choice to implement!
    
**BONUS ADDITION**

Last thing I want to work on is having a list of addons from the Kodi repository displayed on the website. The website display should be very similar to the organization in the official repository, with categories and search query to search addons that are available for Kodi. I will most likely implement a Grid-view style with thumbnails from the repository itself and small descriptions listed underneath it. The database will update once every couple hours which will also push updates to the website with new lists.
    
**TL;DR** The website will be basically a display of Team Kodi addons, with an addition to PR author's repo and branch it to Team Kodi's repository.
