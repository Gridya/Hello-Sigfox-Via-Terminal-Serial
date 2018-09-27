# Tutorial for nanofox IoT KiT activation.

This page presents a step by step procedure to connect 

## Step 1: Getting Device ID and PAC of the WISOL Modem

The default firmware loaded with Nanofox initialises the WISOL modem, and prints out the DEVICE ID and PAC codes every 20 seconds. PAC and DEVICE ID will be required in the next step for device activation. 
Follow this steps to get Device ID and PAC:

1.  Connect Nanofox kit in the PC via USB port. The device should be recognized as a serial Com port. 
2.  Open a serial terminal and set communication to 9600, 1
3.  You should see every 20 secondos the DEVICE ID and PAC printed out in your serial terminal. You can click in the Arduino Nano Reset button and watch the initialization procedure.
3.  Take note of DEVICE ID and PAC.


## Step 2: Kit activation in Sigfox Backend

Note: In case your kit was alread activated by the manufacturer, you can skip this step and jump to step 3.

Follow the Step-by-step guide:

1.  Browse to https://buy.sigfox.com
2.  Click on Activate my devkit
3.  Pick your country
4.  Click on Next
5.  Enter Device ID (HEX) and PAC and click on Next
6.  Enter account details and click on Subscribe
7.  Your subscription is active!

## Step 3: Sigfox Backend Login

Before sending the first message, we will login in the Sigfox Backend and make sure our device has been registered, and that we are in the correct screen to monitor the incomming data.
Follow this steps:

1.  Browse to http://backend.sigfox.com and login with your credentials.
2.  Click in DEVICE on top of the screen. 
  Now you should see a list of your devices, and you should be able to identify your Nanofox kit by the DEVICE ID
3.  Click in the ID code of the Nanofox Kit
4.  Click in the MESSAGE on the left menu
  Now you should see a list of the latest messages received from your device. You are ready now to send the first message using the Nanofox kit.
  
  ## Step 4: Sending the first Sigfox uplink message

Now we will send the first message througt the Sigfox network and check if it has reached backend database. 
Follow this steps:

1.  Make sure your Nanofox kit is still powered up. (If you did not removed it from USB port you should be good to go!) 
2.  In the Nanofox Board, click in the user button and monitor the serial console. You should see some messages indicating the button has been pressed and an uplink message is underway. 
3.  Now monitor the Sigfox Backend. In a few seconds a message should pop up in the list.

You are now read to start experimenting with Nanofox IoT kit!
  
 

### Small image

![](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTkjhLm6R7bwG9y7iMMeMtIUKWINpmo8ylEEMSOtePWr9hX8Wo_zQ)

### Large image

![](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSx8MWT1jHI4aEOd2-OQAzRDAEMEilM6Ltvyf7275fITItqHSQq)

  



