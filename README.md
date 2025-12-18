# Bluetooth-Packet-Sniffing
This Wireshark project analyzes HTTP and Bluetooth HCI protocols. I performed forensic data extraction by filtering for 200 OK codes to reconstruct JPEG images from raw packet bytes. I also compared 113 Bluetooth frames to Ethernet to contrast local wireless logic with TCP/IP.

## Part 1 HTTP
Open A2HTTP.cap in Wireshark. You should see mostly TCP and HTTP (green) packets.

How many packets are in this capture file?
Some packets show an error. What kind of error is this? HINT: The background of those packets is dark.
Use this filter.
http.response.code==200
What does the 200 access code mean?
Find a packet, the right click on ‘JPEG File Interchange Format’. Pick Export Packet Bytes to save a .bin file to your computer.
Next, change the file extension on the .bin file to .jpeg. You should now be able to open the image. Paste the JPEG (not a screenshot of wireshark) into the answers document!
Repeat this for a second image. (There are five total, but two will suffice for the assignment!)
 image.png

 

## Part 2 - bluetooth
Open A2BLUETOOTH.cap For this part, there are no steps or detailed instructions. This is the Bluetooth Host Controller Interface protocol.

There are 113 frames in here. go through them and write two paragraphs on what you found interesting. Describe some of the differences between these Bluetooth frames and the Ethernet frames we’ve seen.

Below is what you should see:

 

image.png

 

Remember, Bluetooth isn’t based in TCP/IP, it’s local wireless!

If you would like some more context, you can open the link below, but you don’t need to visit it or write a highly detailed response for full credit. Layman’s terms will suffice for this part of the lab. Feel free to work in a group for this part and discuss with your classmates!

Bluetooth Protocol DetailedLinks to an external site.
