# DNVOD-AD-Block

1. install ```uBlock``` plugin in your browser.
2. go to the settings menu of ```uBlock``` and select ```My filters``` Tab
3. Paste the following content in the input block <br> 
```
  public.dnvod.tv/upload/public/*.jpg<br>

  http://s1-a1.dnvod.tv/vod/*

  ! block the fucking ad images.
  /http:\/\/\w+\.dnvod\.tv\/(?:\w+\/(?!video))+\d+(?:\w+)\.[jpg|JPG|gif|GIF]{1}/

  www.dnvod.tv###form1 > .main > .left > .dnpub.ggw-l
  www.dnvod.tv###form1 > .main > .left > .product > .dnpub.ggw-l
  www.dnvod.tv###form1 > .dnpub
  www.dnvod.tv###form1 > .main > .left > .dnpub.ggw-l

  ! block the fucking side ads
  www.dnvod.tv##body > .whole > .dnpub 

  www.dnvod.tv##body > .dnpub 
```

4. click ```Apply changes``` button in the upleft corner.
5. Enjoy!
