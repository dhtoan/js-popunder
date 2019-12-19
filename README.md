# Javascript Popunder Maker
* This Javascript class being used to make a popunder easier (avoid blocked by Google Chrome)
* You can make multiple windows/tabs
* Have more options for setting popunder

***

* Author: Do Huy Toan
* Contact: do@doligo.net
* Home: https://www.doligo.net/author/dhtoan
* Copyright: (c) 2014 David Lab.
* Version: 2.0

**Note**: 
* The popunders will open all at the same time with Firefox, IE
But in Google Chrome, i have been try to avoid blocked by Chrome popunder-blocker therefore the popunders will be open in order clicked
* Default: popunder work for session of browser, but you can change it by `cookieExpires` options

### Options
#### Main Options
* 'onNewTab' `true` or `false` default: `true`, this decide the popunder will open on newtab or new window
* 'eventType' `1` or `2` - default: `1` (window onclick), `2` (document.body onclick)
* 'cookieExpires' type float, day of cookie (if not set, popup will work by session), you can use `0.5` for 12 hours
* 'alwaysPop' `true` or `false` - default: `false`, if `true`, refresh = new popunder

#### Other Options
There are all defaul options of popunder (if onNewTab = false)

* width:        window.screen.width,
* height:	window.screen.height,
* left:		0,
* top:		0,
* location:	1,
* tollbar:	1,
* status:	1,
* menubar:	1,
* scrollbars:	1,
* resizable:	1

### Usage

    <script type="text/javascript" src="popup.js"></script>
    <script type="text/javascript">
    // make pop on new tab
    Light.Popup.create('site1.com', {onNewTab: true});
    // make pop on new window with size 100x100
    Light.Popup.create('site1.com', {width: 100, height: 100, onNewTab: false});
    // refresh = new popup
    Light.Popup.create('site3.com', {alwaysPop: true});
    </script>

P/s: I haven't updated it for a long time, if it don't working, Please email for me :)
