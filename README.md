# blockprint
Blockprint helps you turn your Raspberry Pi into a 3D printing design machine using Minecraft Pi.

This is the first program I wrote in Python. It is for Rasperry Pi users and works with the game Minecraft Pi that comes with the Raspbian, the Raspberry Pi OS.

To begin, download the minecraft-printing.py file and unzip it. 

You will also need to download OpenSCAD. This program is compatible with Raspbian and will be used to turn the output file from minecraft-printing into a .stl file that your 3D printing software will understand.

The 3D printing software I use is Repetier and the slicing program Slic3r. You can use whatever you like, but these instructions will be for those programs.

Instructions:

Open Minecraft Pi and create a world.

Hide Minecraft and open minecraft-printing.py in Python 3 or Geany and run the code. This can usually be done by hitting F5 on your keyboard or finding the “Run” command.

Now return to Minecraft and go build something awesome! The program will run quietly in the background.

Once you have something in Minecraft that you would like to print, build a cube cage around it made out of Gold blocks. You are essentially building a Minecraft version of a transporter from Star Trek and will be beaming your Minecraft object out of the game and into the real world! I chose Gold because transporters take a lot of energy to work and Gold is the best conductor of electricity.

This cube cage should not be a full cube, just the edges of a cube. Make sure that the length, width, and height are all the same. The program will check this and give you an error message if your transporter is not a perfect cube.

Once your object is ready to print, go and hit any part of the gold transporter with your sword. This will activate the transporter. It will first inspect itself to make sure you built a transporter that is a cube.

When the inspection is complete, the transporter will make a copy of your object right next to the transporter out of Wool. Look around after you activate your transporter with your sword and you should see the copy being built out of thin air.

When the copy is complete, you are given a chance to look at the copy and make sure it is what you want. Sometimes seeing your object all in one color highlights changes you want to make. If you want to make changes, go back to your object and edit it. You can hit the transporter with your sword to start the copy process over again. If you like how the Wool copy looks and want to print it, hit it with your sword.

The program will now export the coordinates of the object in a format that OpenSCAD will understand. Look on your desktop for a file called “Minecraft_object.scad”

Open Minecraft_object.scad in OpenSCAD and hit F6 to render it. If you created a very large object then this process can take up to 20 minutes. Sometimes the rendering process can get stuck at 99%. Don’t worry – just give it more time.

Once your object has rendered, go to File > Export to STL. This file will work in Repetier. When you slice it, check the scale of the object. It may be that the object is quite small and you need to scale it up. This is fine - it will not affect the quality of the print since it is made up of all cubes.

Tweet me any photos of successful prints or of questions on the code. @ThaneRichard.
