---
layout: post
title:  "Homekit Send a notification from the IFTTT"
date:   2022-08-28 10:56:00 -0800
categories: Homekit automation 
---

Open the [Contoller](https://controllerforhomekit.com/) Application and click on `Add Automation` - 

![add Automation](/images/Controller_add.jpg)


Name the New Automation and select `Event-Based` or `Time-Based`.   
![select event-based](/images/eventbased.jpg)

Here I am going to trigger on motion and select `If one of these events`
![select one of these events](/images/ifOneofTheseevents.jpg)


Find and select the accessory.
![select an accessory](/images/selectAccessory.jpg)


Add conditions for the selected the accessory.
![add conditions](/images/addConditions.jpg)


Select an existing scene as a placeholder.  This in only to compelte the automation to be able to save it.  We will update this later.
![select scene](/images/selectScene.jpg)

Click the `Close` button.
![temp scene](/images/placeholderScene.jpg)

`Save` automation.
![save button](/images/saveautomation.jpg)

Since Apple has not exposed `convert to shortcut` feature we need to switchback to Apple Home application and go to `Select Accessories and Scenes.`
![select accessories and scens](/images/selectAccesScenes.jpg)


And then unselect the scene we initially selected as a placeholder.  Go all the way to the bottom and click `Convert to Shortcut`.
![connvToshortcut](/images/connvToshortcut.jpg)


Delete scene listed:
![connvToshortcut](/images/connvToshortcut.jpg)

Add Web action - 
![selectWeb](/images/selectWeb.jpg)

Select url for webhook url
![selectURL](/images/selectURL.jpg)

Go to IFTTT and create the webhook.
![createbuttonIFTTT](/images/createbuttonIFTTT.jpg)

![webhookAdd](/images/webhookAdd.jpg)

![webRequest](/images/webRequest.jpg)

![triggerMotionDetected](/images/triggerMotionDetected.jpg)

![ThenThat](/images/ThenThat.jpg)

![notifications](/images/notifications.jpg)

![notificationSimple](/images/notificationSimple.jpg)

![createAction](/images/createAction.jpg)

![notificationSimple](/images/notificationSimple.jpg)

You should endup with a url for the webhook like this - 
>curl -X POST https://maker.ifttt.com/trigger/{event}/with/key/your{key-here}


Back in Home app add url
![webhooookURL](/images/webhooookURL.jpg)


get contents of url:
![getContents](/images/getContents.jpg)





maker.ifttt.com/trigger/GR_LowTempWarning/with/key/XXXXXXXX


 




