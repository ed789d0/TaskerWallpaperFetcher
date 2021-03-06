# TaskerWallpaperFetcher
2 tasks for Tasker that can fetch and set a wallpaper from Bing or Unsplash. Inspired by https://www.reddit.com/r/tasker/comments/f2taxl/ and https://forum.joaoapps.com/index.php?resources/wallpaper-daily-changer-unsplash-images.417/

NOTE: Bing Wallpapers are capped to 1920x1080 or 1080x1920. I don't know if it's possible to fetch a higher-res version.
## How to use
1. [Download the ZIP](https://github.com/ed789d0/TaskerWallpaperFetcher/archive/main.zip) and extract it. (You can do this directly on your Android device, or on your computer and then transfer the .tsk.xml files.)
2. In Tasker long press the *TASKS* tab at the top and select Import Task.
3. Find the .tsk.xml file you extracted in step 1.
4. The task is now imported.
5. To make it run every day, make a new profile and use the Time option. If you want every day, then make sure the To button is deactivated and select a time to run every day. If you want an interval (up to 12 hours), deactivate both the From and the To buttons and select Every.
## Get landscape photos (Bing only)
By default, the bing task gets portrait photos. To get landscape photos, 
go to the task in tasker and in the JavaScriptlet action, remove the `.replace(/1920x1080/g, "1080x1920")` part of the code.
## Change Search Term (Unsplash only)
After importing the Unsplash task, you can change the search term. 
Go to the Set Unsplash Wallpaper task, and in the HTTP Request action change the word "landscape" (in the url field) to something else.
Use %20 for a space.

See https://source.unsplash.com/ for all the URL options for getting the picture. (You can use %RESOLUTION wherever it asks for a resolution.)
