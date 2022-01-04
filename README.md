# cowswap-autocueswap
Cue a swap below a certain gas and token price.

Cowswap is great. It offers small fish to do trades without fronting the Gas, which at the time or writing, is absurd (150-200+$).  
If you dont have enough fund or if you want to do a trade that's favourable in Gas, you can wait all day with the window open or use this script to set a trade for token x to y and set a target GasFee you want it to initiate on.  
If this hits, it will play a "MOO" sound and hit "SWAP" for you. Now all you have to do is confirm the action.

# How to load: 
Copy paste in console. Because CowSwap does not use JQUERY, you need to paste it twice.

# Commands you can change: 
var TargetGas = xx.xx; Set this to the gas fee you want it to initiate BELOW.  
var TargetPrice = xx.xx; Set this to the MAXIMUM value you want to token to be.  
var TimeOut = 20000; Increase or reduce the time the interval checks for the GasPrice to update.
var BuyIt = new Audio('https://www.myinstants.com/media/sounds/cow-moo-sound.mp3'); replace the url with something you want it to play as a sound que.

Console Debug Set your console to "Warnings" only. It will print the current, lowest and highest gas prices recorded. If certain settings arent set, it will remind you to do so. It will also alert if certain conditions are met (or aren't. i.e tokenPrice is higher than your TargetPrice).
