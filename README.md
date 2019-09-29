# Things To Pushbullet Instructions
[Things to Pushbullet Page](https://omarshahine.github.io/things-to-pushbullet/Things-to-Pushbullet.html) is a simple static web page that lets you contruct a Things To-Do and send it to an iOS device. I wrote this because I use Windows Devices at work and wanted an easy way to send To-Dos to Things that was more powerful and capable than [Mail to Things](https://support.culturedcode.com/customer/en/portal/articles/2908262-using-mail-to-things).

## Set up Pushbullet
1. Get a  [Pushbullet Account](https://www.pushbullet.com/) 
2. Install the  [Pushbullet App](https://apps.apple.com/us/app/pushbullet/id810352052)  on your iOS device
3. Sign into Pushbullet on your iOS device (note if Push notifications don’t work, sign out and sign in again on the iOS device)

## Get your Pushbullet Access Token
1. Go to the  [Pushbullet Account Page](https://www.pushbullet.com/#settings/account) 
2. Click **Create Access Token**
3. Make note of your access token


## Get your Things Authentication Token
**on iOS**
1. Launch Things
2. Go to Settings (bottom of screen)
3. Go to General
4. Select Things URLs
5. Make note of your authentication token

## Try it out
1. Navigate to the [Things to Pushbullet Page](https://omarshahine.github.io/things-to-pushbullet/Things-to-Pushbullet.html) 
2. Enter the Things Authentication token into the **auth-token** field on the page and click **Save**
3. Enter the Pushbullet Access token into the **pushbullet-auth-token** field on the page and click **Save**
4. Enter a title and any other data you like and click **Send to Pushbullet**

You should get a notification
![Notification](resources/IMG_0096.jpeg)
tapping the notification will display this
![To-Do](resources/IMG_0097.jpeg)

## Details
This page was built using the [Things URL-Scheme](https://support.culturedcode.com/customer/en/portal/articles/2803573) documentation page. I forked the HTML and CSS and stripped anything unecessary to create a simple page to generate the correct URL scheme for things. Feel free to customize or simplify this page further.

That URL is then sent to Pusbhullet which in turn will push the URL to your iOS device.

The auth-token and pushbullet access tokens are stored in your browser local storage for re-use.

You can bookmark the [Things to Pushbullet Page](https://omarshahine.github.io/things-to-pushbullet/Things-to-Pushbullet.html) on any web browser and send to-dos to your iOS devices.

The [Things to Pushbullet Page](https://omarshahine.github.io/things-to-pushbullet/Things-to-Pushbullet.html) is hosted on GitHub in this repository. You can [view the source here](https://github.com/omarshahine/things-to-pushbullet).
