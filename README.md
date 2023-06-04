# BxMCTF 2023

![ctflogo](https://github.com/cosmoshivani/BxMCTF-23/assets/47838688/785587b6-2ac5-46ca-991b-315efb103d05)

:mushroom: [BxMCTF 2023](https://ctfmgci.jonathanw.dev/contest/bxmctf2023) 

Hi! :wave:

## 1. Selfie [Forensics]

### Author: clides
### One day, clides secretly plugged a rubber ducky into Claudio Pacheco's laptop and gained control. While browsing through his files, he found this selfie which contains some secret information.

>We have a zip file and after extracting it, we get the following image for this challenge --

![BxMCTF-Foren-1](https://github.com/cosmoshivani/BxMCTF-23/assets/47838688/fe844a74-17bd-47c2-8291-f42ae63850a0)

>Let's first check the file using an online Exif Tool

:mushroom: [Exif Tool](https://exif.tools/)

![exif](https://github.com/cosmoshivani/BxMCTF-23/assets/47838688/0f879c61-7992-4323-b8b2-a69c1ec6ad7a)


>You will find that there is, what seems like an ecoded string in the License section ```Y3Rme25xaUoyQnQyaVZEa2d6fQ```. We can use CyberChef to decode

:mushroom: [CyberChef](https://gchq.github.io/CyberChef/)

>Using the Base64 decoder, we get the flag

```ctf{nqiJ2Bt2iVDkgz}```

>Probably the string in the braces also means something but I couldn't decode it, and the flag already works. But it would have been better if it meant something
 
 ---
 
 ## 2. Blank Space - I mean Page [Web]
 ### Author: Mani
 ### Have fun finding the flag…regardless if you're capable of solving CAPTCHAs or not.

>given web address --  ```https://bxmweb1.jonathanw.dev/```

>The description is hinting towards whether you are a Robot or not. Which indicates that its referring to the robots.txt file that most websites have. Basically, it comes under the Robot Exclusion Protocol, which ensures that the bots will always look for the robots.txt file for the information they are not allowed to access. For example, during web crawling the bot will exclude the information that are not allowed to be indexed. But this disalllowence can easily be bypassed. And some web crawlers might use this file as a guide to get forbidden informations. So, if you go to ```https://bxmweb1.jonathanw.dev/robots.txt``` you will find this- ```Disallow: /very-secretly-hidden```. Now this web address - ```https://bxmweb1.jonathanw.dev/very-secretly-hidden/``` will lead you to the flag ```ctf{sdh57349857243fkhkwAklkAH} ```



 
