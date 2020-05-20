# Real-World-Federated-Learning

<p>Exploring the use of Federated Learning on a set of Raspberry PI's. The goal is to develop a distributed recommender system that will give individual users a recommendation on movies they might like.
Using a neural collaborative filtering model on the latest Raspberry PI to date to provide the recommendations.</p>

<h2>Raspberry Pi setup</h2>
<ul>
	<li>Installing raspbian buster lite</li>
	<p>With the formatted SD card we need to install the Raspbian image.
	I will be using balenaEtcher, which is available for Windows, Mac and Linux.
	<a href="https://www.balena.io/etcher/">Link</a></p>
	<li>Download the Raspbian Buster Lite image <a href="https://www.raspberrypi.org/downloads/raspbian/">Link</a></li>	
	<li>Use balenaEtcher to select the image and drive and then flash the image to the drive.</li>
	<li>Enable SSH on the Raspberry Pi</li>
	<p>Insert the SD card into your computer<br>
	Navigate to the boot directory on the SD card.<br> 
	Create a file called “ssh”<br>
	SSH is now enabled. You can now insert the SD card back into the pi.<br>
	</p>
	<li>How to connect to the pi</li>
	<p>Turn on the pi.<br>
	You will need to connect both your computer and the pi to the same router. Connect the raspberry pi to the router via the ethernet cable and connect your computer to the router via WIFI.
	Now you will need to find out what devices are on the network. I will be using Linksys’ router page. I accessed this webpage by typing in the IP address into my browser, 
	for example my router’s IP was 10.1.1.1.<br>
	Navigate to the status tab and click on Local Network in the sub menu. Click on DCHP table to find other devices connected to the router.<br>
	<img src="linksystable.png" />
	In a terminal on the connected pc type <br>
	<code>ssh pi@<device ip></code>
	For example:
	My Raspberry Pi’s IP: 10.1.1.141 (As seen in the DCHP table)
	ssh pi@10.1.1.141
	</p>
</ul>

