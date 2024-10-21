
# HTBUSTER
 HTBUSTER is a utility for the Dombusters team to use for HackTheBox. It draws heavy inspiration, and is built based on [Celesian's Styx tool](https://github.com/c3l3si4n/styx)   
 (Currently just copied, changes are intended!)
  
 ## Purpose
 HTBUSTER was built for the sole purpose of levelling the playing field during HTB seasons. With the speed at which the usual few complete easy machines, we need to save seconds where ever we can.
 To save reinventing the wheel, Celesian's tool was cloned and modified to better suit our use cases.

 ##
 HTBUSTER will be further built on to bring new features and enhancements to the team. 
 
 
## Usage
1. `sudo apt install -y libxcursor-dev libxrandr-dev libxinerama-dev libxi-dev libxxf86vm-dev`
2. `go install github.com/DOMBUSTERS/HTBUSTER@HEAD`
3. Create an app token on your HTB profile (any duration you want)
4. Set the `HTB_TOKEN` environment variable with the value containing your generated token
5. Run styx

-OR- clone this repo and run `go build`
