# VideoSteamingScore

Some sites to check out
https://scorecounter.com/tournament/

Priorities

OBS Studio is the platform
Facebook Live and video hosting

Platform - Windows Laptop

Cameras / Video sources 
  GoPro streaming https://gopro.com/help/articles/block/getting-started-with-live-streaming
  Live streaming currently supports RTMP and RTMPS URLs only. RTSP, HLS and other URLs are not supported. 
  
  Drone streaming - should be RMTP
  
  HDMI output cameras - old gopro, pro cams   - need HDMI video capture
  
  web cams - USB - "Garbage" - Larry 
  

Priorities
1. Stream Video with Graphics layers 
      
      Can place images and web page elements in each scene
      
      Lowerthirds plugins seem to be the way to go - still investigating which ones are any good
      
2. Have multiple video sources and switch between them while keeping graphic layers

      Having an RTMP server is a huge win for multiple RTMP streaming cameras - using NGINX for windows 
      
      http://nginx-win.ecsds.eu/download/nginx%201.7.12.1%20Lizard.zip
      
      Sample nginx.conf on this site setup for 4 cameras on 4 seperate ports (same port had some issues, but should work)
      
      
3. Utilize dedicated buttons to allow easy switching
      
      Keyboard mapped
      
      USB keypad mapped 
      
      External dock - andriod app

4. Scoring - ability to update scores or leaderboard - part of the lower thirds from 1
    
    something like soorecounter.com
    
Ideas being tested

RTMP - server local or remote, maybe run RTMP server on laptop or PI,  remote run it on Amazon instance or private youtube/facebook
  local eliminates lots of up and down bandwidth, but may require local wifi gear that can use a seperate wifi connection to cell service.   Cell service may solve the wifi issue, but range may be limited.
 
 http://nginx-win.ecsds.eu/download/nginx%201.7.12.1%20Lizard.zip
  Well this worked - thanks Jordan
  

Scoreboards - web page, executable or python window capture, some text based solution
  
  Web pages do not auto refresh in OBS - you have to do some fancy web page refresh on the web site side
  
  Window sources need chroma/green screen work
  
Video feed switching - need a press 1 for cam 1, 2 for cam 2, etc
  
  Manual way - Each scene has all the video feeds - cons is not flexible and whole deck needs to be prebuilt 

  Some lower third plugin - need to find one you like - 90% are garbage or cost money
