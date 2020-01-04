# TwitchStreamInfoPage
Replicating the feel of the stream info under the channel player, this is made out to be an html file so that it can be docked within OBS. It shows title, category, box art, viewer count and stream uptime, and has both light and dark modes.

You must have a client ID (acquired from Twitch Developers website) to use this.

For example, when you are offline:
![Demo1](https://raw.githubusercontent.com/janumeke/assets/master/TwitchStreamInfoPage/demo1.png)
When you go online:
![Demo2](https://raw.githubusercontent.com/janumeke/assets/master/TwitchStreamInfoPage/demo2.png)
Then when you go offline:
![Demo3](https://raw.githubusercontent.com/janumeke/assets/master/TwitchStreamInfoPage/demo3.png)

Note that this refreshes itself every 30 seconds, so the info may be as late as 30 seconds (plus latency) ago.

### Usage:
<pre>StreamInfo.html?clientId=&lt;Your Client ID&gt;&username=&lt;Target Channel's Username&gt;&dark=true</pre>
Last argument is optional. Default is light theme.

So for example, if you put the file under D:\\, you put the following in OBS &gt; View &gt; Docks &gt; Custom Browser Docks &gt; URL:
<pre>D:\StreamInfo.html?clientId=...&username=...</pre>

## How To Localize
1. Translate the strings in line 66-76.
2. Use the appropriate fonts in line 11.
