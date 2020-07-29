# qtter
A TouchDesigner patch to detect images from a paper sheet


29/07/2020

Qtter beta 0.1
by
Simone Murtas

web: 
	www.amartist.it
facebook: 
	simone "simplo" murtas
	amartist multimedia
	

This patch extracts parts of a paper sheet and converts them in cropped TOPs to be used as you want. 

It was inspired by the work from @Owen Lowery. 
He made an installation of moving puppets for childrens. 2D characters are animated by Kinect and childrens can draw their avatars on a paper sheet, each part on a rectangle (head, body, arms...) 
The sheet is then inserted in a scanner and the patch cuts the rectangles and biuld the characters. 

This project is intended to create the image to be printed and the system to detect and retrieve the rectangles using a simple webcam (or other live image sources) and placing the sheet in front of it.

You can define all rectangles size in a simple TABLE, the system will automatically cut them from the paper sheet.
Detection is based on the TOE qrCodeTracker by "pdubost" link: https://forum.derivative.ca/uploads/short-url/oThaZRwiV2VD5YHw3M92JEfltoK.tox Forum reference: https://forum.derivative.ca/t/recognize-moving-qr-code/3291
https://github.com/simplo/qtter




TO BE DONE
1) compensate horizontale deformation (x rotatoin of the sheet on the camera plane) evaluating difference in size between upper and lower QRcode    
2) line guides on the screen and positoin detection in real time to be sure the image is captured at maximum size
3) use a better webcam (4k?) or drive a reflex camera    
4) integrate kinect camera to cut parts of real body and face    
5) put the QRdetectioncode outside in engine to avoid TD freezing while computing
		
	
	
PYTHON HELP:	
	HOW TO INSTALL THE PYZBAR LIBRARY!
	
	open the CMD with administrator privileges
	go in the folder: 
	C:\Program Files\Derivative\TouchDesigner\bin\Scripts
		(or where TD is installed)
	enter: 	pip install pyzbar --target=“C:\Program Files\Derivative\TouchDesignerpip \bin\Lib”
		(verify the path correspond to where TD is installed)

	if you don't have pip installed:
		download https://bootstrap.pypa.io/get-pip.py 
		go to 
		C:\Program Files\Derivative\TouchDesigner\bin
			(or where TD is installed)
		enter python get-pip.py
		

This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License
along with this program.  If not, see <http://www.gnu.org/licenses/>.		
			


