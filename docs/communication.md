# Communication :id=communication

The communication window is use to make the link between the Architect's I/O, and the PLC. 

![Middle](Images/First_scheme.png ':size=500')

Before testing your simulation with a PLC, make sure that your simulation works without it.

To make the good communication you need to follow those four step :

- [Communication](#communication)
	- [Tagging](#tagging)
	- [Aliasing](#aliasing)
	- [Link](#link)
	- [Play](#play)




## Tagging :id=tagging

A Tag is the address for the I/O in the simulation, and Tagging is the action to give a Tag to an I/O.

>Adding a PLC

To add a new PLC to the simulation, you just have to click on the "+" button, and choose your PLC.

![Middle](Images/Arrow.png ':size=500')

>Attaching a PLC

You can attach a I/O to your PLC more easily by using the Alias_Element from the "Inspector" window. It allow you to give a name at all I/O from this group, in order to find them directly. 

Then with the "Connection_Id", you need to link the groups with the PLC that you have create earlier in the "Communication" Window.

>Tagging a PLC

To tag an I/O, you can just write the tag you want, in the Data monitor, in the #Tag column. It will directly impact the full tag of the I/O, that is the combination of the Alias_element of the parent groups, and the I/O tag.


## Aliasing :id=aliasing

>Manually

You are able to aliasing your tag, by filling up the address column in the communication windows, with the corresponding address in your PLC.

>Automatically

You can also make the aliasing automatically, with a .csv file, by excel.

## Link :id=link

In order to link correctly Architect software with a PLC, you need to use a link software.

It exist three main software, IESA Link, KEP and RSLink.

![Middle](Images/IESA_Link.png ':size=500')

To establish a connection between IESA Link Client and Architect, you need to ensure that they are configured with the same IP address and path. The IP address corresponds to your computer's standard IP address, while the path refers to the slot number of your CPU. By matching these settings, you can successfully link IESA Link Client with Architect.

Once you have entered the IP and Path information, you can select the specific PLC you are using in IESA Link Client. This allows you to perform read and write operations on tags associated with the PLC. To access a particular tag, you need to provide its address, which will enable you to interact with it.


## Play :id=play

After Tagging your I/O, Aliasing correctly and link Architect with your PLC, you can now turn on the Run mode, and see your simulation in action. 


