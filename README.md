# TwitchStreamInfoPage
Replicating the feel of the channel info under the channel player, this is made out to be an html file so that it can be docked within OBS. It shows title, category, box art, viewer count and stream uptime, and has both light and dark modes.

You must have a client ID (acquired from Twitch Developers website) to use this.

For example, when you are offline:
![Demo1](https://raw.githubusercontent.com/janumeke/assets/master/TwitchStreamInfoPage/demo1.png)
When you go online:
![Demo2](https://raw.githubusercontent.com/janumeke/assets/master/TwitchStreamInfoPage/demo2.png)
Then when you go offline:
![Demo3](https://raw.githubusercontent.com/janumeke/assets/master/TwitchStreamInfoPage/demo3.png)

Note that this refreshes itself every 30 seconds, so the info may be as late as 30 seconds ago.

### Usage:
<pre>StreamInfo.html?clientId=&lt;Your Client ID&gt;&username=&lt;Target Channel's Username&gt;&dark=true</pre>
Last argument is optional. Default is light theme.

So for example, if you put the file under D:\\, you put the following in OBS &gt; View &gt; Docks &gt; Custom Browser Docks &gt; URL:
<pre>D:\StreamInfo.html?clientId=...&username=...</pre>

# 繁體中文版
請參考上圖，只是換成中文。

你需要有 Client ID 才能使用。可以在 Twitch Developers 網站取得。

這每30秒更新一次，所以最多會是30秒前的資料。
### 使用方式:
<pre>StreamInfo_zhtw.html?clientId=&lt;Client ID&gt;&username=&lt;頻道帳號&gt;&dark=true</pre>
最後一個參數可以不填，預設是淺色模式。

例如你把檔案放在D:\，到 OBS &gt; 檢視 &gt; 停駐視窗 &gt; 自訂瀏覽器停駐視窗 &gt; URL 填入：
<pre>D:\StreamInfo_zhtw.html?clientId=...&username=...</pre>
