# CHV Specialized Solution DEF 2018

[Website](http://www.specsolns.com/defcon) with additional info
[**SDK**](http://www.specsolns.com/uploads/9/4/8/7/94871222/dc2018_sdk.zip)
-Check the website for up to date information

![alt text](https://raw.githubusercontent.com/username/projectname/branch/path/asset/img.png)


## Quick how-to for compiling & downloading code to the 2018 Defcon 26 car hacking village badge:

[Reddit link I got from](https://www.reddit.com/r/Defcon/comments/97c57z/chv_badge_hello_wolrd/)

1. Download and extract the SDK from [http://www.specsolns.com/uploads/9/4/8/7/94871222/dc2018_sdk.zip](http://www.specsolns.com/uploads/9/4/8/7/94871222/dc2018_sdk.zip)

2. Install the windows driver from ``` SDK\bin\Win7 QCM USB Driver\USB Driver```

 Note that it isn't digitally signed so you will need to manually install the "QCM.inf" file by attaching the CHV badge via USB and installing the driver via Device Manager

 For an example of how to manually install, see [https://www.tp-link.com/us/faq-228.html](https://www.tp-link.com/us/faq-228.html)

3. Check Device Manager to see if the badge is properly recognized as a QCM device

4. Update Windows PATH variable to include SDK\bin directory : [https://www.computerhope.com/issues/ch000549.htm](https://www.computerhope.com/issues/ch000549.htm)

5. To compile the sample 'default' badge application, open a command window in SDK\default

To make a sample code change for testing, use your favorite text editor to modify the name of one of the menu items on line 24 of badge_default.p, e.g. from "BOX" to "BIZ"

6. Now ```pawncc.exe badge_default.p```

This will generate **badge_default.amx** file

7. ```Run QCM.exe```

8. Select Load Script and then browse to **badge_default.amx**

9. It should download the code to the badge

10. Rinse and repeat until you achieve desired results


