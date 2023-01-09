# JobControl Walkthrough

**Before getting in line for the lasers:** use one of our laser templates to prepare your file following the instructions and styleguide included in the template. If you need help, don't be afraid to come in during our open hours and check your file with shop staff!

Once your file is ready, get in line for the lasers and put your file on a flash drive. When your turn comes, go to an open laser and open up your file. This walkthrough will only include instructions for AutoCAD and Illustrator, but files can be sent from other software such as Inkscape, using the same styleguide and a similar printing process. 

## AutoCAD to JobControl
To start, either into the commandline `plot`, or go to File -> Plot. This will open what is essentially AutoCAD's printing function. The following window should open.

![starter](https://raw.githubusercontent.com/theLadyStardust/scd-shop/main/images/autocadplotstart.JPG)

This may look like a lot, but we only need to worry about 3 main things, shown in the image below.

![starter_highlighted](https://raw.githubusercontent.com/theLadyStardust/scd-shop/main/images/starter_highlighted.png)

1. Plotter: This is the printer output. Select `Trotec Engraver vXX.X.X` from the plotter dropdown. 

![plotter](https://raw.githubusercontent.com/theLadyStardust/scd-shop/main/images/autocadplotter.JPG)

2. Plot Area: This is what will be plotted. First, select `Window` from the `What to Plot` dropdown

![plotareaselect](https://raw.githubusercontent.com/theLadyStardust/scd-shop/main/images/autocadplotareaselect.JPG)

Then select the area you want to laser. 

![windowareaselect](https://raw.githubusercontent.com/theLadyStardust/scd-shop/main/images/autocadwindowselect.JPG)

If you want to reselect this area, you can hit the `Window<` button this is now next to the `What to Plot` 

![windowreselect](https://github.com/theLadyStardust/scd-shop/blob/main/images/windowreselect.JPG)

3. Plot Scale: This is the scale at which this will be plotted. All of The Shop's templates are 1 plot unit = 1 inch, so generally you'll select 1:1, and inches here. To do this, first deselect the `fit to paper` box, then change the `Scale` dropdown to 1:1 with the units in inches.

![plotscale](https://raw.githubusercontent.com/theLadyStardust/scd-shop/main/images/plotscale.JPG)


Once you have this, you can select `Apply to Layout` in order to save these settings to your file. When you go to plot next time, it will have these same settings. Then, hit `Ok` to send to JobControl.

## Illustrator to JobControl
To start, print by using Control + P or going to File -> Print. It should open up the following window. 

![image](https://user-images.githubusercontent.com/63514508/211379006-8bd3fbd2-85d4-40d8-968b-7376a6dc4640.png)

Select `Trotec Engraver vXX.X.X` from the printer dropdown.

![image](https://user-images.githubusercontent.com/63514508/211379360-220ee3e7-54b8-4870-bf48-a1ffd1de8c8d.png)

Under Options, find the Scaling dropdown and select `Do Not Scale.` This will ensure that hairline strokes for cut and engrave lines will stay as such in the printing process. 

![image](https://user-images.githubusercontent.com/63514508/211379758-92075bff-691f-4799-9d34-eb6e739370af.png)

From here, you can just print to send it to JobControl.

### Dithering and Images

If you're wanting to print images from Illustrator to have a grayscale effect with the laser, you may want to check out the various dithering algorithms included with JobControl. To do this, from the print dialogue, hit `Setup...`, then `Preferences` after selecting the printer. You'll then find them in the `Halftone` dropdown under `Process Options`. 

![image](https://user-images.githubusercontent.com/63514508/211381203-76200651-5043-430f-9ced-33ead08f2762.png)

Each algorithm is optimized for different uses, and [this article](https://tannerhelland.com/2012/12/28/dithering-eleven-algorithms-source-code.html) does a pretty good job of covering them. Once you've selected the one you want, hit the JobControl button at the bottom of the dialogue box, then `Print`, and `Print` again to send it. 

![image](https://user-images.githubusercontent.com/63514508/211381073-d959d84c-9491-44cb-b2c3-ec596436f235.png)


## JobControl
Once you've sent your file to JobControl, it will either open JobControl if it wasn't open yet, or it will start it flashing. Either way, navigate to JobControl.

![jobcontrolbreakdown](https://user-images.githubusercontent.com/63514508/211382921-615a3231-91f6-4e24-beed-a2a12ec8199f.png)

1. Jobs Panel. This is where your job will show up after you send it to JobControl. You can drag jobs from here to the bed, and back. Selecting a job here will display a preview beneath this panel that will show your job as the set of instructions the laser will follow.

![image](https://user-images.githubusercontent.com/63514508/211383427-051e52ae-90a0-4eb2-8253-a3a74c4751c3.png)

2. Bed. This is the bed of the laser, and placing and positioning jobs here will tell the laser what to do, and where. 

3. Material Settings. This is what settings the laser will use to interpret your file. The left dropdown is the category of material, and the right is the specific material, with width. You can also change the material by double clicking on the bed. 

4. What you see is what you get. This is a toggleable option that lets you see what the laser will do given your file. This is used mostly for checking that your file is set up correctly before sending it to the laser. Notably, not all materials use all settings, and changing the material can change how the laser will interpret your file. So, if not all of your file is showing up correctly, check that you have the correct material first. 

5. Placement coordinates. This is the position, in inches, of the upper left corner of the job. You can move the job by either dragging it in the bed, or by using these. Generally, you want to place your job where your material will be, and you'll have the best results the closer to the upper left corner of the bed your job is. However, in order to ensure that the entirety of the job is on your material, you'll want to offset it by a tenth or so of an inch. 

6. Machine status and connection. This shows the status of the laser, it's connection to JobControl, and the controls to manage that. By clicking the USB button when the laser is on, you'll initiate a connection to the laser. Once this connection is set, this button will change to a play button, which allows you to send the jobs on the bed to the laser with the current material settings. This will also have controls to pause and stop the laser while a job is running. 

## Laser Controls

![lasercontrols](https://user-images.githubusercontent.com/63514508/211396845-d25b42a2-c2a1-4f4b-a182-e86c9e345639.png)

1. On/Off Switch. Turn the key all the way to the left to startup, then release to let turn on. Turning on will initiate a homing sequence, which must be done before anything else can be done with the machine. 
2. Emergency Stop. Use only in an emergency, i.e. a self-sustaining fire in the bed.
3. Stop and Start/Pause controls. Pressing start/pause will run the current bed in JobControl, and will pause operation after the machine completes the current operation. This will keep the job and where it is in the job in memory, allowing you to unpause and restart by pressing the start/pause button again. Stop will stop operation, and throw out the current job. 
4. X-Y Axes Controls. Controls position of the head in the X and Y (horizontal) plane. When connected, the head's position will show in the bed in JobControl and can be locked onto to place files. 
5. Z Axis Controls. Controls vertical position of bed. Pressing both at once with the head over the material will do an autofocus operation, setting the bed's position to the correct height for that material depth. 

Not pictured: GRIT card reader, towards front of machine. When red, laser will be locked out. When green, laser is able to be operated.

## Sending to Laser
To start, have your job prepped and sent to JobControl.

1. Place on bed by either double-clicking your job in the jobs tab or dragging it onto the bed in JobControl.

![image](https://user-images.githubusercontent.com/63514508/211392195-b04e4eb0-a2e6-49d9-9bd7-0f22abab3984.png)

2. If the laser is off, turn on the laser by tapping your Grit card to the card reader, then turning the key all the way to the left, and letting it go back, similar to starting a car. The laser will begin a homing sequence, and will beep when finished.

3. Place your material on the laser bed where you have your job in JobControl. If you need to move the laser down to fit your material, use the Z axis controls to move the bed to fit your material.

5. Using the XY axes arrows on the laser controls to place the head over your material, hit both Z arrows to home the Z position. The laser needs to be a certain depth from the material to home correctly, and this does that automatically. 

6. Initiate a connection to the laser by hitting the USB button in JobControl. 

6. Select your material by double-clicking the bed outside of your job, then finding the material category and the specific material. If you accidently double-click on your job,  you can hit escape to get back to the main view. Note that the specific material settings can't be changed without Shop Supervisor permission. 

![image](https://user-images.githubusercontent.com/63514508/211390466-bb73d001-0bf5-4587-9483-770902c8a730.png)

7. Using the what you see is what you get tool shown above, check the position and operations done by the laser. Blacks, greens and greys will engrave, reds will cut. 

![image](https://user-images.githubusercontent.com/63514508/211390869-3f604771-1df0-4980-b617-89ffc9438515.png)

8. After checking to ensure correct placement, size, position, and operations of your job, hit the play button in the laser status area in the bottom right of JobControl or the Play/Pause button on the laser to start the job. 
