# Gettings Started :id=gettingstarted

# Files Description :id=fliesdescription

It exist 3 types of files use by Architect software :

<table>
        <tbody><tr>
            <th>Files</th>
            <th>Description</th>
        </tr>
        
            <tr><td>.XMC3</td>
            <td>This file is the main file of your project, with 3D models and more.</td>
        </tr>
        <tr>
            <td>.alias</td>
            <td>This file is a text file, use for the communication between Architect and a PLC</td>
        </tr>
        <tr>
            <td>.config</td>
            <td>This file is is useful to fully configure your project.</td>
        </tr>
        <tr>
            <td>.PNTPackage</td>
            <td>This file is a file which contain a bundle of 3D object, to implant in your 3D Project. </td>
        </tr>
</tbody></table>

# Open an existing project :id=openproject
> Open a project

Click on File>Open

![Open](Images/Open.png)

Disable unused sections and click Load.

![Open2](Images/Open2.png ':size=600')

Let's start

![Opened](Images/Opened.png ':size=1024')

By default, you have access to the different demos for Architect listed below :

**Formation_VDemo**, is a project where all the most use objects and function are presented.

**Crochets_VDemo**, is a project with a hook chain, as conveyor.

**Carcass_VDemo**, is a project with an unique way to move product.

**Magasin_VDemo**, is a project, with an interface to stock the product in shell.

Each of them, explain how Architect work, and how you have to use the tools.

# 3D Navigation :id=nav
>Move camera

In order to navigate freely in the 3D viewer, you need to move.

You can use the middle click on your mouse or the keybindings "Arrows".

![Middle](Images/middle.png ':size=200') ![Arrows](Images/Arrows.png ':size=200')

This video show you how to use Button 3 to move your camera in the 3D viewer.

<video width="800" controls>
  <source src="Medias/Button3.mp4" type="video/mp4">
</video>

>Rotate camera

You can also rotate your camera by using the right click on your mouse.

![Middle](Images/right_click.png ':size=200')

This video show you how to use right click to rotate your camera in the 3D viewer.

<video width="800" controls>
  <source src="Medias/ClicDroit.mp4" type="video/mp4">
</video>

>Zoom

Finalmy, you can zoom in and out, by using your mouse wheel on the keybindings "+/-"

![Middle](Images/zoom.png ':size=200') ![Arrows](Images/minus.png ':size=200') ![Arrows](Images/plus.png ':size=200')

This video show you how to use mouse wheel to zoom in and out your camera in the 3D viewer.

<video width="800" controls>
  <source src="Medias/Wheel.mp4" type="video/mp4">
</video>


# Creating your first simulation :id=firstsim

>Creating a new scene

To start a brand new project, you need to click on File>New. Within seconds, a blank project will open and be ready for use.

You can also use the keybinding : ![Middle](Images/CtrlN.png ':size=130'), in order to open a new scene.

![Middle](Images/New.png ':size=130')

![Middle](Images/New2.png ':size=900')

>Adding a Conveyor

To add a conveyor to your scene, you can simply right click on the scene, and select Create>New Object>Transitique>Conveyor. The way to do it is described in the video just below.

<video width="800" controls>
  <source src="Medias/Adding.mp4" type="video/mp4">
</video>

If you want to move and rotate your conveyor, you can use the moving tools on the top bar. Have in mind that the arrow on the conveyor described the direction of the conveyor.

![Middle](Images/Gizmo.png ':size=200')

<video width="800" controls>
  <source src="Medias/Move.mp4" type="video/mp4">
</video>

>Adding a Sensor

In order to fully use a conveyor, you need to add a cell to it. To know when an object is on the conveyor, and when the object is not on it anymore.

To add a conveyor to your scene, you can simply right click on the scene, and select Create>New Object>Capteurs>Cellule. The way to do it is described in the video just below.

<video width="800" controls>
  <source src="Medias/Cell.mp4" type="video/mp4">
</video>

Then you will need to place your cell on the conveyor. In order to do that, you need to simply move the cell on the conveyor with the moving tools. The way to do it is described in the video just below.

<video width="800" controls>
  <source src="Medias/Move_Cell.mp4" type="video/mp4">
</video>

You can attach a cell to a conveyor, in order to move them together, to do not have to replace the cell at the right place all the time. The way to do it is described in the video just below.

<video width="800" controls>
  <source src="Medias/Attach.mp4" type="video/mp4">
</video>

>Duplicate Object

You can regroup objects together. In order to do it, simply right click on the scene, and select Create>New Groups>Standar. And drag your object in the groups. The way to do it is described in the video just below.

<video width="800" controls>
  <source src="Medias/Group.mp4" type="video/mp4">
</video>

You can duplicate any object or groups, in order to do not repeat the creation process. To do it you need to right click on the object or groups you want to duplicate, and choose duplicate. The way to do it is described in the video just below.

<video width="800" controls>
  <source src="Medias/Duplicate.mp4" type="video/mp4">
</video>

To attach together two conveyors, it exist on the 3D Tools, a visual helper, to well link together object, such as conveyor. Make sure that the arrow are facing the same way, to have your two conveyor with the same direction. The way to do it is described in the video just below.

<video width="800" controls>
  <source src="Medias/Link.mp4" type="video/mp4">
</video>

[Resources](https://github.com/HaroldPX/PntArchitect/blob/main/docs/xmc3%20Exemple/)


# Running your first simulation :id=runfirstsim

>Switching Edit & Run

To initiate the simulation, simply toggle the run/pause button. The simulation will start, and the conveyor will start moving in accordance with the code programmed within the controller. If you wish to halt the simulation and reset the environment, you can click the run/pause button again followed by the reset button.

For the next sections, we will used the simulate created previously in [creating your first simulation](#firstsim)

>Adding a product

![Middle](Images/StopReset.png ':size=310') ![Middle](Images/Run.png ':size=300')

To generate a product within the 3D viewer, you must first define the product in the product resources window. Afterward, click on "Add product mode" and position the product anywhere you desire within the simulation. You are able to remove any of the product by using "Remover Product Mode". 

<video width="800" controls>
  <source src="Medias/Add_Remove.mp4" type="video/mp4">
</video>

>Testing without PLC

You can force the data to take specific values to observe how your object or simulation functions. An icon will appear at the top ![Middle](Images/ForcedIcon.png ':size=20') whenever a single data point is forced. In order to reset all the data, right click on that icon, and choose "reset all forced data". The process for forcing data is described in the video located just below this section.

<video width="800" controls>
  <source src="Medias/Forced.mp4" type="video/mp4">
</video>

You can see that the cell detect well, when a product cross the red laser trait, in the video just below.

<video width="800" controls>
  <source src="Medias/Run_Cell.mp4" type="video/mp4">
</video>

First, make sure you use the "Tapis" Conveyor, in order to command them correcly. If you are not sure that , your conveyor are "Tapis" one, you can convert them. The way to do it is described in the video just below.

<video width="800" controls>
  <source src="Medias/ToTapis.mp4" type="video/mp4">
</video>

You can forced the data to take specific value, in order to see how functions your object or simulation. You can reset all the forced data with an icon that will appear on top, whenever a single data is forced. The way to forced data is described in the video just below.

<video width="800" controls>
  <source src="Medias/Forced.mp4" type="video/mp4">
</video>

You can see that the cell detect well, when a product cross the red laser trait, in the video just below.

>Testing with PLC

In order to do not use, controller or forcing data, you can use a PLC, in order to monitor the simulation. In this page, as an example, we are going to use  a Siemens PLC.

![Middle](Images/Second_scheme.png ':size=800')

>Aliasing I/O

First, in order to correctly link your PLC to the simulation, you need to add an automate to the communication window.

<video width="800" controls>
  <source src="Medias/PLC.mp4" type="video/mp4">
</video>

Then, you can name a data with a tag, in order to find them, in the communication window in one sight.

<video width="800" controls>
  <source src="Medias/tag.mp4" type="video/mp4">
</video>

Then, to fully link the data with the PLC, you have to address an automate to the group, then address your PLC alias to the tag you want.

<video width="800" controls>
  <source src="Medias/Alais.mp4" type="video/mp4">
</video>

>Connecting PLC

To connect our automate to the simulation, we will use IESA Link client.

# External Software :id=externalsoftware

>Virtual commissioning PLC

<table>
        <tbody><tr>
            <th>Software</th>
            <th>Uses</th>
        </tr>
        
            <tr><td>IESA Link</td>
            <td>Siemens PLC</td>
        </tr>
        <tr>
            <td>KEP Server</td>
            <td>Siemens PLC</td>
        </tr>
        <tr>
            <td>RSLink</td>
            <td>Rockwell PLC</td>
        </tr>
        <tr>
            <td>Twincat</td>
            <td>Beckroff PLC</td>
        </tr>
    </tbody></table>

>Training VR

<table>
        <tbody><tr>
            <th>Software</th>
            <th>VR Headset</th>
        </tr>
        
            <tr><td>Steam VR</td>
            <td>HTC Vive Pro 2</td>
        </tr>
        <tr>
            <td>Vive Business Streaming</td>
            <td>HTC Vive Focus 3</td>
        </tr>
        <tr>
            <td>Oculus software</td>
            <td>Oculus headset</td>
        </tr>
        <tr>
            <td>Twincat</td>
            <td>Beckroff PLC</td>
        </tr>
    </tbody></table>














