# flowgorithm_linux
Installation instructions to use [Flowgorithm](http://flowgorithm.org) on Linux / Ubuntu 20.04

According to [Wikipedia](https://en.wikipedia.org/wiki/Flowgorithm)
> Flowgorithm is a graphical authoring tool which allows users to write and execute programs using flowcharts.

It is sometimes used in schools to introduce computer science. Unfortunately it is available only for Windows, which is a problem for students using Linux or MacOS. Luckily, using [Wine](https://winehq.org) and [`wine-mono`](https://wiki.winehq.org/Mono), you can make it work. You need to use some commands in the terminal. If you find error or inaccuracies, feel free to open an issue here on GitHub.

## Installation instructions for Linux (Ubuntu 20.04)

1. Install `wine` to get several new commands in the terminal, like `wine` and `wine64`:
```
sudo apt install wine
```


2. Dowload `wine-mono`. At the time of writing, the latest version is `7.4.0`, that you can find from here:

  https://dl.winehq.org/wine/wine-mono/7.4.0/
  
  https://dl.winehq.org/wine/wine-mono/7.4.0/wine-mono-7.4.0-x86.msi

3. Install `wine-mono`
```
wine64 uninstaller
```
(then click on *install* and choose the file you just downloaded `wine-mono-7.4.0-x86.msi`, and press *OK*)

4. Download Flowgorithm. I used the *Executable Only* version `3.31` because it does not require any installation. The *Windows Installer* version should work as well (untested). You can find the file at:

http://flowgorithm.org/download/index.html


5. Unzip the downloaded file `Flowgorithm-exe-only.zip` to get `Flowgorithm.exe`
```
  unzip Flowgorithm-exe-only.zip
```

6. Run Flowgorithm.exe via `wine64`
```
  wine64 Flowgorithm.exe
```

Next time, you just just need to execute the last step to run Flowgorithm on Linux.
