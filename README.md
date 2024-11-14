
# RaspberryPi - Ngrok connection

I wanted to find a way to connect to my home network from anywhere in the world using a wifi connection (works on a mobile device as well using a VPN). 

#### *Requirements*
- RaspberryPI that supports a wired ethernet connection (wifi works but not ideal).
- Thats it honestly

> How it works
> The pi is connected to your router using an ethernet cable. You install ngrok onto the pi and start the service on startup in the background. It opens a TCP connection just like the image below.
> ![Screenshot from 2024-11-14 14-43-35](https://github.com/user-attachments/assets/03a2b650-6120-437e-aac6-dbe95c8eb154)
> You then will curl the webserver to get the information on where to connect to and will email yourself the content. You can then use the content to ssh into PI. ex: ssh pi@example -p <portnumber>
> Once remoted in, if you have your PC connected to the ethernet you can setup WakeOnLan and power on your desktop using the PC mac address. And use it to remote into the PC from anywhere.
> If you have 



1. Install RaspberryOS onto your PI (haven't tested with other linux distro's)
2. Enable ssh
3. Install ngrok [Ngrok](https://download.ngrok.com/linux)
4. 
