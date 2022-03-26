# Beacon Guide

These guides relate to the following products: USB, Short Range, Long Range, Avvel X

## Configuring the UUID

The default iBeacon UUID is: EBEFD083-70A2-47C8-9837-E7B5634DF524

This is not to be confused with the Peripheral UUID which is seen in the 'searching peripherals' screen. The peripheral UUID is unique to the device and cannot be changed using the eBeacon configuration utility. Some BLE scanners, such as LightBlue, identify the beacon initially by its peripheral Name and peripheral UUID.

1. Open the eBeacon App

2. Tap the 'Central' tab

3. Tap the 'jaalee' device

4. Tap Beacon 'Config' (0xFFF0)

5. Tap Beacon 'UUID' (0xFFF2)

6. Tap 'Write'. Now put in the new UUID, make sure that the line begins with "0x".

7. Tap 'Send'. Confirmation of sent Hex value appears as a box below the 'write value box' with the comment 'Select to write'.

8. Tap 'Config' which will take you to a screen containing all the characteristics about the iBeacon. The UUID value box should now contain a different value.

## Modifying the Transmission Power

The output Transmission Power level is measured in dBm. The default level is set to the maximum of 0dBm. Use the table below to find the corresponding write values.

1. Open the eBeacon App

2. Tap the ‘Central’ tab

3. Tap the ‘jaalee' device

4. Tap Tx Power (0x1804)

5. Tap Tx Power Level (0x2A07)

6. Tap Write

The hex value to be entered comprises of the password and new power level value.

## Changing the Password

A password is required every time the iBeacon is configured. We recommend that the password is changed upon receiving the iBeacon for security reasons.

The default password is: 666666

1. Open the eBeacon App.

2. Connect to your beacon.

3. Tap 'Beacon Config' (0xFFF0).

4. Tap '0xFFF8'.

5. Tap 'Write'.

6. In the 'Write HEX' box enter your desired password preceded by '0x'. i.e '0x123456'.

7. Tap 'Send;

The setup should now be complete. You can go back to the previous page to see the new password you have set.

**THERE IS NO HARD RESET - Remember your password.**

If you have entered set the password to be automatically remembered then you may need to change this. In the Home menu go to 'More' > 'Central Setting' > 'Automatically Input Password'.

## Configuring the Major Value 

The Major and Minor values are very useful in narrowing down the location of the iBeacon to a more specific location. The Major is a value between 0 and 65535. The default Major value is 1 (0x0001).

1. Open the eBeacon App.

2. Tap the 'Central' tab.

3. Tap the 'jaalee' device.

4. Tap 'Beacon Config' (0xFFF0).

5. Tap 'Beacon Major Value' (0xFFF3).

6. Tap 'Write’.

7. Enter the new Major Value following this format: 0x0005, if you want the Major Value to be 5.

8. Tap 'Send' - A Confirmation of sent hex values appears as a box below the write value box with the comment 'Select to write'.
 
9. Tap 'Config' which will take you to a screen containing all the characteristics about the iBeacon. 

10. To check that the write was successful, tap 'Config' and check that the correct value is in the Major field.

## Configuring the Minor Value

The Major and Minor values are very useful in narrowing down the location of the iBeacon to a specific location. The Minor is a value between 0 and 65535. The default Minor value is 1 (0x0001).

1. Open the eBeacon App.

2. Tap the 'Central' tab.

3. Tap the 'jaalee' device.

4. Tap 'Beacon Config' (0xFFF0).

5. Tap 'Beacon Minor Value' (0xFFF4).

6. Tap 'Write’.

7. Enter the new Minor value following this format: 0x0005, if you want the Minor Value to be 5.

8. Tap 'Send' - A Confirmation of sent hex values appears as a box below the write value box with the comment 'Select to write'.
 
9. Tap 'Config' which will take you to a screen containing all the characteristics about the iBeacon. 

10. To check that the write was successful, tap 'Config' and check that the correct value is in the Minor field.

## Changing the Beacons Name

Once you have successfully changed the name of the beacons it may take a few attempts to moments to the beacon before you will see the change made when searching for the beacons. Wait for the beacon to refresh its self (a few minutes) then you should see the changes made.

TO CONFIGURE THE UUID
1. Open the eBeacon App

2. Tap the 'Central' tab

3. Tap the 'jaalee' device - await connection.

4. Scroll down to and tap '0xFF80'.

5. Tap '0x2A90'

6. Tap 'Write'

7. In the 'Write Text' field enter the name you would like to use.

8. Tap 'Send' on the keyboard.

9. Tap 'Select to Write'

10. The changes should now have been made.

## Opening Up Your Long Range iBeacon

1. Turn the iBeacon upside down until you can see the faint lines around the sides.

2. Use a thin screwdriver or plastic card to open the back housing.

3. Slowly use a screwdriver to prize the circuit board out of the housing, there is a buzzer loosely stuck on to the housing, take this off carefully.

4. Slide the new battery in, with the positive terminal facing down (Test the iBeacon before putting it back into the housing.)

5. Put the circuit board back into the iBeacon housing, circuit board facing up, and make sure it fits into the two plastic pins.

6. Put the closing lid back on.

## Avvel X ONLY- Eddystone URL Setup Guide

This guide will walk you though the setup process of the Eddystone functionality. You will need to put the device in connectable mode, please click here to see how to do this, if you haven't already done so when configuring the iBeacon functionality.

![Stage 0](/images/Eddystone/Stage+0.png)
![Stage 1](/images/Eddystone/Stage+1.png)
![Stage 2](/images/Eddystone/Stage+2.png)
![Stage 3](/images/Eddystone/Stage+3.png)
![Stage 4](/images/Eddystone/Stage+4.png)
![Stage 5](/images/Eddystone/Stage+5.png)
![Stage 6](/images/Eddystone/Stage+6.png)
![Stage 7](/images/Eddystone/Stage+7.png)
![Stage 8](/images/Eddystone/Stage+8.png)
![Stage 9](/images/Eddystone/Stage+9+Update.png)
![Stage 10](/images/Eddystone/Stage+10.png)
![Stage 11](/images/Eddystone/Stage+11.png)

