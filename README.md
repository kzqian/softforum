# softforum
<details>
  <summary>BC4 MAC Unlimited</summary>
  
  
1 . goto `beyond compare` folder
```
 cd "/Applications/Beyond Compare.app/Contents/MacOS/"
```

2 . rename `BCompare` to `BCompare.real`
```
 mv BCompare BCompare.real
```

3 . new a file named BCompare
```
 touch BCompare
```
4 . write following code into `BCompare`
```
#! /bin/bash
if [ -f $HOME/Library/Application\ Support/Beyond\ Compare/registry.dat ]
then
    rm $HOME/Library/Application\ Support/Beyond\ Compare/registry.dat
fi
"/Applications/Beyond Compare.app/Contents/MacOS/BCompare.real" &
```

5 . make `BCompare` executable.
```
chmod +x BCompare
```

refer to:
 [beyond-compare-4-for-mac-unlimited](http://tutandtips.blogspot.com/2015/10/beyond-compare-4-for-mac-unlimited.html)
</details>

<details>
  <summary>BC4 WIN Unlimited</summary>
  
  
1 . run command
```
 reg.exe delete "HKCU\Software\Scooter Software\Beyond Compare 4" /v CacheID /f
```
</details>
