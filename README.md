# DNVOD-AD-Block

1. install ```uBlock``` plugin in your browser.
2. go to the settings menu of ```uBlock``` and select ```My filters``` Tab
3. Paste the following content in the input block <br> 
```
public.dnvod.tv/upload/public/*.jpg

! block all video type ads
http://s1-a1.dnvod.tv/*

! block the ad images, which is not in the same folder as the movie pictures
!/http:\/\/[\w|\-]+\.dnvod\.tv\/(?:\w+\/(?!video))+\d+(?:\w+)\.(jpg|JPG|gif|GIF){1}/
/http:\/\/[\w|\-]+\.dnvod\.tv\/(?:\w+\/(?!video))+\w+\.(jpg|JPG|gif|GIF){1}/

! block those ad images, which is in the same folder as the movie pictures
/http:\/\/[\w|\-]+\.dnvod\.tv\/[\w+|\/]+\d+[a-zA-Z]+\.(JPG|GIF){1}/

! block the git ads besides show section
www.dnvod.tv###form1 > .main > .i-cp > ul >.i-cp2

www.dnvod.tv###form1 > .main > .left > .dnpub.ggw-l
www.dnvod.tv###form1 > .main > .left > .product > .dnpub.ggw-l
www.dnvod.tv###form1 > .dnpub
www.dnvod.tv###form1 > .main > .left > .dnpub.ggw-l

! block the fucking side ads
www.dnvod.tv##body > .whole > .dnpub 

! block the fucking side ads
www.dnvod.tv##div[data-code*="SSS"]

! block the popup
www.dnvod.tv##div[data-type*="popup"]

! block stream ads
www.dnvod.tv##div[data-code*="D"]

! block stream ads
www.dnvod.tv##div[data-code*="B"]

! block stream ads
www.dnvod.tv##div[data-code*="I"]

! block stream ads
www.dnvod.tv##div[data-code*="L"]

! block stream ads
www.dnvod.tv##.ggw-r,.gsd,.float-right

www.dnvod.tv###form1 > .whole > .bfq > .bfq-l-2

www.dnvod.tv##body > .dnpub 
```

4. click ```Apply changes``` button in the upleft corner.
5. Enjoy!
