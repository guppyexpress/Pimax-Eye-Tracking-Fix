# Eye tracking Fix
> if you have the Pimax Eye tracking module, and you are not satisfied with how it performs. use this instead! it increases performance (a little bit) i am still working out the bugs and kinks in it. but for the most part, it does improve the eye tracking

# Instructons

> if you are like me and saw the Droolon Pi1 eye tracking module and thought. wow, eye tracking on a Pimax! that must be great! and you buy it. and low and behold. it is barely usable. it can not track properly, it gets very hot etc. well I got fed up with that. so I went out and made my own software/firmware for it. (the firmware is a branch of an official 7invensun firmware that 7i has provided to me through an email)

well, what does this that you made do? how can it improve on a product that seems hopeless?

as long as you follow the instructions I listed on the github repository, the Eye tracker becomes

more accurate

less hot less

power draw

still runs at 120 hertz*

and no longer a need for an external cable to the pc

it performs best directly connected to the headset, with the 15mm foam. please be aware, the cable thing has only been tested by 2 people, both with the same results, that might not be the case for you, as well as the size of the facial interface.

I will continue to try to update this as time goes on to better improve upon the code.

make sure to download the full code it will not work unless you do so.
![firstimg](https://community.openmr.ai/uploads/default/original/3X/f/0/f001d743b122f7a68d706430d4210539876ec131.png)

also make sure. you followed Pimax’s original instructions for the Eye Tracking module. as that is required for this to work.

once you have done that, the files are listed in numerical order of what to do
![secondimg](https://community.openmr.ai/uploads/default/original/3X/b/6/b6bb85dfba8456752fd0aaa29829bd68ad65459a.png)
start by running the firmware upgrader. then run the runtime .exe
after that, make sure to run the AMCap that comes with the files on the top right you will see the words “capture” click that, and in the drop down click “Set Frame Rate”
![thirdimg](https://community.openmr.ai/uploads/default/original/3X/5/9/59a6fd74dc800ac46aab951ccda939c0a914d229.png)
set your frame rate to look like mine. it should say “10000” and the “Use Frame Rate” box should be checked.
![4thimg](https://community.openmr.ai/uploads/default/original/3X/4/d/4de3e3e33c8eff1dd44bfe933ee3f3d530fe6b75.png)
once that is done, click OK

if you click on “options” in the drop down, click “Video Capture Pin”
![fithimg](https://community.openmr.ai/uploads/default/original/3X/a/a/aa5b632281f7842fb1516f0e5199260b9a075f06.png)
have that match these settings. this will provide it with 120 hertz at the default resolution.
once you are done click “Apply” then click “OK”
![sixthimg](https://community.openmr.ai/uploads/default/original/3X/f/4/f4df7e1dd23fe36007db50f254a13dd493b83de7.png)

it should now say 120 fps as shown below
![7thimg](https://community.openmr.ai/uploads/default/original/3X/e/f/efb2bf48aebb5e257ed1976087617964f777999f.png)
Next up you will need the file called “lib”
replace the files in the AseeVR runtime with these. this will make the tracking more accurate.
![firstimg](https://community.openmr.ai/uploads/default/original/3X/0/b/0b6ccfbfca6bcf444b58c0155f73e66f3e62db7c.png)


close AseeVR with task manager (or right click and select exit) same goes for the program called “Forward” power down the vr headset by holding the power button. wait roughly 10 seconds and turn the Pimax headset back on. and start AseeVR.

you will notice the eye tracking is now significantly more accurate and slightly smoother. i am still working out the bugs as it is still not fully done. but as of now. it changes the eye tracker from “functional” to “usable”

thanks so much for your time! and i hope you enjoy the eye tracking! any questions comments or concerns, please message me on discord @guppyexpress#0001


<br>
make sure you are using the ET on 2.0 mode where it is connected directly to the headset. there is no longer a need for an external cable with this new fix


<br> <br> <br> 
# if you are having a hard time getting to calibrate. make sure AMcap is closed, if you are still having a hard time calibrating, kill AseeVr with task manager, and kill forward with task manager. hold down powerbutton on the HMD until it shuts off wait 30 seconds, turn it back on, restart AseeVR and try again. (might have to repeat multiple times) if it still doesnt work, open device manager, and uninstall the DroolonF1 (located in cameras) and re install everything. restart computer. and try again.
<br>
make sure you are using the AMCap located in the files downloaded. on the right hand side you will see a button called capture. click that, then in the dropdown click set frame rate. under that, make sure the box is checked, and type in "10000" (without the quotes) and make sure that is applied. also make sure to follow the amcap instructions to change it to the default resolution + frames. it should show similar to the image in step 3. any questions? feel free to shoot me a dm on discord @guppyexpress#0001

# For More Detailed Instructions, Visit This OpenMR Link.
https://community.openmr.ai/t/eye-tracking-software-fix/37292
