# CS:GO case stats viewer

## How does it work?

This Java Application loads your whole CS:GO <a href=https://steamcommunity.com/my/inventoryhistory>inventory history</a> by emulation the view more button.
To avoid rate limiting it loads 50 transactions per ~2.5 seconds. Which mean if you have a large history it will take longer to load.
After the inventory history is dumped it will search for every unboxed case.

## Usage

1. Download the latest compiled version via the <a href=https://github.com/cantryDev/CSGOCaseStatsViewer/files/5939123/CSGOCaseStatsViewer-Release1.0.0.zip>latest release</a> or compile it yourself with maven.
2. Execute the execute.bat 
3. Follow the steps in the commandline which just got opened
4. Get disappointed.

## Example result

<a href=https://github.com/cantryDev/CSGOCaseStatsViewer/blob/master/result_07_02_2021_14_54.txt>click</a>

## Requirements
- Java 8 or higher

## FAQ

### It crashed
Just restart it. It will continue where it crashed.

### Why does it need my cookies?
It needs your cookies to request your <a href=https://steamcommunity.com/my/inventoryhistory>inventory history</a>

### How do I get my cookies?

#### Chrome

1. Visit your steam profile.
2. Press F12 or right click(anywhere on the website) and press inspect element. 
3. Select the network tab
4. Reload the page
5. Go back to the network tab and scroll to the top and select the first entry. On the right side it should say Request Url: Your steam profile url
6. Scroll down on the right side till you see Cookie:
7. Right click on Cookie: and select copy value

#### Firefox
1. Visit your steam profile.
2. Press F12 or right click(anywhere on the website) and press inspect element.
3. Select the network tab
4. Reload the page
5. Go back to the network tab and scroll to the top and select the first entry. On the right side it should say GET: Your steam profile url
6. Scroll down on the right side till you see Cookie:
7. Right click on Cookie: and select copy
