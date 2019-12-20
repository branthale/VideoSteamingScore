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
  
  Drone streaming 
  
  web cams - USB
  

Priorities
1. Stream Video with Graphics layers 
      Completed 
2. Have multiple video sources and switch between them while keeping graphic layers
3. Utilize dedicated buttons to allow easy switching
      Keyboard mapped
      USB keypad mapped
      External dock - andriod app
4. Scoring - ability to update scores or leaderboard
    something like soorecounter.com
    
Ideas being tested

RTMP - server local or remote, maybe run RTMP server on laptop or PI,  remote run it on Amazon instance or private youtube/facebook
  local eliminates lots of up and down bandwidth, but may require local wifi gear that can use a seperate wifi connection to cell service.   Cell service may solve the wifi issue, but range may be limited.
  http://nginx-win.ecsds.eu/download/nginx%201.7.12.1%20Lizard.zip
  Well this worked - thanks Jordan
  

Scoreboards - web page, executable or python window capture, some text based solution
  web pages are not updating in OBS - user error ?
  Window sources need chroma/green screen work
  
Video feed switching - need a press 1 for cam 1, 2 for cam 2, etc
  Each scene has all the video feeds 

