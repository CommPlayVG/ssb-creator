# ssb-creator
  A simple Chromium site-specific browser creation tool

# What is an SSB?
  Glad you asked!

  An SSB is essentially a stripped down version of a web browser that's designed to have little to nothing of its interface visible, and only view one site. The
  reason this is useful is that given the right setup, you can run webapps as if they were installed on your local drive, with slightly improved performance over a
  regular web browser. This tool aims to do as much of that work for you as possible!

# How to use ssb-creator
  Straightforward and to the point.
  To install, just `git clone https://github.com/SaphiraKai/ssb-creator` and move `ssb-creator` into `/usr/bin`, or download the .zip and do the same.

  1. Use `sudo ssb-creator https://www.example.com # just example.com works too` to "install" a webapp
  2. Use `sudo ssb-creator remove example.com` to "uninstall" a webapp

# NOTES:
  1. This tool is ONLY compatible with Chromium and Chromium-based browsers (Chrome, Edge, Vivaldi, Brave, etc)
     While Firefox and some other browsers DO support SSBs, it's not compatible with the code I have written. If there are requests to make ssb-creator 
     Firefox(or other)-compatible, I'll look into it!

  2. When removing a webapp, you CANNOT use the full URL, as `remove` refers to the local files and not the site itself.
  
  3. I haven't thoroughly bug-checked this tool, and one known issue I have confirmation of is that the `remove` option is capable of removing regular executables
     as well as webapps if used improperly. Just try to be careful with `remove`, and I am accepting commits if anyone has a lightweight solution to this or other
     issues.
