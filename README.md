
# GStreamer with Python - TEKEVER CHALLENGE

For this challenge was requested to create an simple pipeline using GStreamer. Fot that I used an tutorial from youtube (https://www.youtube.com/watch?v=HDY8pf-b1nA&t=166s), because it's a really new technologie for me. 

Assumptions:

1) The source of the video it's just an webcam image.
2) The OS is Windows





## Install and run
As I mentioned, I will consider that you are trying to run the GStreamer through an Windows Machine.
The GStreamer doesn't have a native compatibility with Windows and Python,  so will be necessary emulate that.
For that, we will use MSYS2, download with the link: https://github.com/msys2/msys2-installer/releases/download/2020-09-03/msys2-x86_64-20200903.exe

Once it's installed, start "MSYS2 MinGW 64-bit" from the Start Menu. This will open up the MSYS2 terminal.

Once you are in MSYS2 MinGW Terminal, you can run these commands to install all the dependencies that we need:

Clone the project using git:
```bash
  pacman -Syu
```
Then:

```bash
  pacman -S mingw-w64-x86_64-gstreamer mingw-w64-x86_64-gst-devtools mingw-w64-x86_64-gst-plugins-{base,good,bad,ugly} mingw-w64-x86_64-python3 mingw-w64-x86_64-python3-gobject
```
After that, open the msys64 folder and navigate to home/<name_of_your_profile>/:
In my case the name of my profile are luizg, so the path are msys64/home/luizg
```bash
  cd home
  cd name_of_your_profile
```
Then just create an folder called gstreamer
```bash
  mkdir gstreamer
```

Now you have the structure to receive our main.py, so you can download it of clone:
```bash
  git clone https://github.com/luizgtvsilva/tekever-task_one.git
```

Copy our 'main.py' file and paste into your gstreamer folder.

Start "MSYS2 MinGW 64-bit" from the Start Menu.

Navigate to our gstreamer folder:
```bash
  cd gstreamer
```

Then run:
```bash
  python3 main.py
```

The objective of this pipeline are just show your webcam video.

