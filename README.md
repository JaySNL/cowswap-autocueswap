# cowswap-autocueswap
Cue a swap below a certain gas and token price.

Cowswap is great. It offers small fish to do trades without fronting the Gas, which at the time or writing, is absurd (150-200+$).  
If you dont have enough fund or if you want to do a trade that's favourable in Gas, you can wait all day with the window open or use this script to set a trade for token x to y and set a target GasFee you want it to initiate on.  
If this hits, it will play a "MOO" sound and hit "SWAP" for you. Now all you have to do is confirm the action.

# How to load: 
Copy paste in console. Because CowSwap does not use JQUERY, you need to paste it twice.

# Commands you can change: 
var **TargetGas** = xx.xx; Set this to the gas fee you want it to initiate BELOW.  
In console, type: ```TargetGas = [yourvalue]``` I.e ```TargetGas = 50.00```. This will hit Swap as soon as the GasFee is below $50.00  

var **TargetPrice** = xx.xx; Set this to the MAXIMUM value you want to token to be.  
In console, type: ```TargetPrice = [yourvalue]```. I.e ```TargetPrice = 4.69```. This will only buy the token when it is **below** $4.69  

var **TimeOut** = 20000; Increase or reduce the time the interval checks for the GasPrice to update.  
var **ConsoleClearCount** = x; Set to value after how many lines in console you want it to auto clear. Set equaly on line 18 and 71.  
var **BuyIt** = new Audio('https://www.myinstants.com/media/sounds/cow-moo-sound.mp3'); replace the url with something you want it to play as a sound que.

# Console Debug
![consoledebug](https://user-images.githubusercontent.com/7669379/148093306-ae765f52-d218-4da7-bd3e-c7a610eb2542.png)  
Set your console to "Warnings" only. It will print the current, lowest and highest gas prices recorded. If certain settings arent set, it will remind you to do so. It will also alert if certain conditions are met (or aren't. i.e tokenPrice is higher than your TargetPrice).

# Example of Proof Of Concept (older version)


https://user-images.githubusercontent.com/7669379/148092900-c2bf1241-c084-4d59-9eff-f3f2d31ed3e9.mp4

