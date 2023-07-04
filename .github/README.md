# Steam's Miniprofile

_Fork of [gamer2810/steam-miniprofile](https://github.com/gamer2810/steam-miniprofile)_

This is a tool that loads your miniprofile(_with animated background and frame_) as a HTML entity so that you can feature it on your website.  
Preview:

<iframe src="https://akrista.github.io/steam-miniprofile/" style="border:0px #ffffff none;" name="myiFrame" scrolling="no" frameborder="1" marginheight="0px" marginwidth="0px" height="400px" width="600px" allowfullscreen></iframe>

## Guide

1. Get your Steam's **AccountID**, you can use [SteamDB](https://steamdb.info/calculator/) or google how to find it yourself.
2. Access `https://akrista.github.io/steam-miniprofile/?accountId=YOUR_ACCOUNTID_HERE`

Example: https://akrista.github.io/steam-miniprofile/?accountId=238158335

### To add this to your site

1.  You can load it into any div with JQuery or Javascript. [Jquery's Load() guide](https://www.tutorialspoint.com/How-to-load-external-HTML-into-a-div-using-jQuery).
2.  You can also load it as an _iframe_

```html
<iframe
  src="https://akrista.github.io/steam-miniprofile/?accountId=YOUR_ACCOUNTID_HERE"
  style="border:0px #ffffff none;"
  name="myiFrame"
  scrolling="no"
  frameborder="1"
  marginheight="0px"
  marginwidth="0px"
  height="400px"
  width="600px"
  allowfullscreen
></iframe>
```

- Once it's loaded, you can mod it however you like using CSS. - A working
  example can be found at my [Github Profile](https://github.com/akrista).

#### Notes:

- This works by calling Steam's API and render the response with Steam's CSS. _This site is not affiliated with Steam or Valve_.
- Your profile will need to be public for this to work.
- It will track your _public_ status (Online, Offline), but it _wont_ track your _friend-only_ status (Away, Snooze,...).
- If your AccountID is invalid, it will instead load _MINE_ (as in the one writing this) miniprofile).
- You might have to disable caching of the _iframe_ on your web, or changes on Steam won't be reflected immediately.

## Why a fork?

The original repo seems to have issues when calling the CORS API, so I forked it and changed the API used to load the miniprofile. In any case this project eventually happens to fail you when loading, as it happened to me with gamer2810's repo, try changing the API to one of this [LIST](https://gist.github.com/jimmywarting/ac1be6ea0297c16c477e17f8fbe51347)

_*Have a good day*_ and <sub>~~Please feed me a star if you are feeling generous. I'm _humgry_~~</sub>
