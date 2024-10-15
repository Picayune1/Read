# Ocean Life VR: Beneath The Waves
## Developed by the do it for the fish team, in collaboration with the flying fish technology team

### Description 
This project is a simulation of an underwater environmet using VR. the simulation is built using Unreal engine, and the main point of the project is to use real data, to educate people about the reefs. Currently this version of the project only has one environment model loaded. The environment model was built using the photogrammetry software reality capture and images of the environment. The purpose of this project is to be deployed in environments like an aquarium in order to educate users about reef and fishes.

### Requirements to run this program
- Unreal Engine (version 5.4 or later) link : https://www.unrealengine.com/en-US/download
- Meta Quest Link app : https://www.meta.com/en-gb/help/quest/articles/headsets-and-accessories/oculus-rift-s/install-app-for-link/
- Meta Quest VR headset

Before you begin you will want to install Unreal engine. To do this you should first download the epic games launcher from the link above. Once you have installed the launcher, run it. Once the epic games 
launcher is installed, open it and either sign in or create an account. Once that's done, you should be taken to the main page for the launcher. If you look to the left of your screen you will see a link to the Unreal engine. If you click this, you will be taken to the unreal engine page. Then in the top right, you will see a button to install unreal engine. Click this and onces the install is done, you should now be able to launch the engine. The only way to view the blueprints of an unreal engine project is inside the unreal engine. If you want to make your own models, you can also download reality capture from this page. 

### If you're just reading the codebase, and not running the full code, 
Unzip the codebase and open the file, then double click the Unreal engine project file. Now click the content drawer to find all the files. The files we made changes to or created are : 
- FirstPerson/Blueprints/BP_FirstPersonCharacter : Contains code for the first person pov, how it interacts with items. Changes made, Crated funcion looking. 
- View_fish/Items/Item_1 : A grabbable fish item that has code on how the user interacts with it and what it should do if interacted with. Created by us
- View_fish/UI/Display_help : Widget code. Created by us
- View_fish/UI/Inspection : Widget for first person POV. Created by us
- View_fish/UI/InspectionVR : Widget for VR POV. Created by us
- VRTemplate/Blueprints/VRPawn : Contains code controlling the VR pov as well as actions and functions. Changes made, Created funcitons are looking, toggleinspect, areacheck, stopinsepct

For the UI widgets look at the top right and click Graph to view the blueprint

### If you are running and compiling the full version, follow the steps below
If you are having trouble installing steam watch this guide here : https://www.youtube.com/watch?v=zkETI3ITNHc

Make sure your Meta Quest VR headset is already setup before beginning

You will have to link your PC Meta Quest Link app to your Meta Quest VR headset using either a cable or air link. First you will have to download and setup the Meta Quest Link app on your PC. Make sure to use the same account that you use for your actual Meta Quest VR headset on the Meta Quest Link app. If your struggling heres a video : https://www.youtube.com/watch?v=BTCtMrEbZQo&t=20s

Then you can link your Meta Quest VR headset to your PC using either air link or a cable. If you are having trouble linking your VR headset to your PC, follow the guide on the official Meta Quest page here : https://www.meta.com/en-gb/help/quest/articles/headsets-and-accessories/oculus-link/connect-with-air-link/

Now download the unreal engine file and unzip. Now open the file and double click the Unreal engine project file

In order to setup the Meta Quest VR headset in order to link with the unreal engine, You will need to set it up in the Unreal engine file. This guide gives a good breakdown of what you should do to setup the file so it can be previewed in VR : https://www.youtube.com/watch?v=Z4sClxhgsxk

Once thats all done, click the content browser in the bottom left of the unreal engine and open the file called Stage. Then click on the file called level. This should open the currently setup VR environment. If you setup the link level beforehand so that you could run the level in VR, You should see the green triangle in the top. Click this to then run the enviroment, allowing you to test and experience the prototype.

Credits for the 3d model: 
- Fish Collection by shedmon : https://sketchfab.com/3d-models/fish-collection-84a4238a77e541f0ae7db54ccf9f6d8e No changes made
- Yellow tang by JayNme : https://sketchfab.com/3d-models/oxidane-yellow-tang-5750f70ac6734728b0eb3ed81de9bb2d No changes made
- Triggerfish by Jivo3dAssets : https://3dexport.com/3dmodel-triggerfish-416259.htm Some changes made
- Coral beauty fish : https://free3d.com/3d-model/coral-beauty-angelfish-v1--473554.html No changes made
- Underwater environment made in photogrammetry software reality capture using images provided by the Flying fish technologies team. 

### Privacy concerns
Unreal engine does collect data from users such as hardware performance, usage statistics and other information about what users do on the platform. If you are uncomfortable with this you can disable it. To do this open the project and in the top menu click edit. This will show a dropdown menu, where you will want to click editor preferences. Click this and scroll down to privacy. Then click both bug reports and user data and click dont send. This will stop any personal data from being sent to Epic games. None of our written blueprints collect data, and you can read through the whole project to check if your still concerned.

### Security concerns
If one is concerned about the project zip file, like if it has been changed malicously, remove the readme file and check the hash. The MD5 checksum hash of the project should be : 

### Ethical concerns
All models and information were created with throurogh research and an aim to show the true data as it is. None of the images were edited in a way to display a flase narrative before the models were formed, and the models were created to the best of our ability to show the data as accurate as possible. 

Troubleshooting videos and guides:
If your having trouble installing unreal engine watch this video : https://www.youtube.com/watch?v=ODxm8iuOVak
If your having trouble creating an epic games account watch this video : https://www.youtube.com/watch?v=5h2h7_232y0
