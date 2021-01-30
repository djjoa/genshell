# genshell
genshell: A bash copy-and-paste oneline reverse shell generator.
<!--
*** LOGO !![vmplayer_bx33YLqLcn](https://user-images.githubusercontent.com/68730121/106347752-dc8c6a80-628e-11eb-91e9-3e2d510b2172.png)
-->

<!-- ABOUT THE PROJECT -->
## About The Project

![Banner](https://user-images.githubusercontent.com/68730121/106348443-58d57c80-6294-11eb-8aa0-b93806259f58.png)




<!-- GETTING STARTED -->
## Installation
Multiple ways to install / use the script: 

1. Use the github repo  
   ```sh
   git clone https://github.com/djjoa/genshell.git
   cd genshell
   chmod +x gennshell
   ./genshell 
   ```
   
2. Grab the standalone script
   ```sh
   wget https://raw.githubusercontent.com/djjoa/genshell/main/genshell && chmod +x genshell && ./genshell
   #OR 
   curl https://raw.githubusercontent.com/djjoa/genshell/main/genshell -o genshell && chmod +x genshell && ./genshell
   ```

<!-- USAGE EXAMPLES -->
## Usage

```sh
./genshell -u
Usage: genshell [-h|--help] -p|--port [args] [-l|--LHOST [args]] [-t|--RHOST [args]] [-b|--banner]
```

## Help

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


<!-- CONTRIBUTING -->
## Contributing

Contributions are what make the open source community such an amazing place to be learn, inspire, and create. Any contributions you make are **greatly appreciated**.

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

<!-- CONTACT -->
## Contact

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
