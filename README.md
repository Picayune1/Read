# Ocean Life VR: Beneath The Waves
## Developed by the do it for the fish team, in collaboration with the flying fish technology team

### Description 
This project is a simulation of an underwater environment using VR. The simulation is built using Unreal Engine, and the main point of the project is to use real data, to educate people about the reefs and fishes. Currently this version of the project only has one environment model loaded. The environment model was built using the photogrammetry software reality capture and images of the environment. The purpose of this project is to be deployed in environments like an aquarium in order to educate users about reef and fishes.

### Requirements to run this program
- Unreal Engine (version 5.4 or later) link : https://www.unrealengine.com/en-US/download
- Meta Quest Link app : https://www.meta.com/en-gb/help/quest/articles/headsets-and-accessories/oculus-rift-s/install-app-for-link/
- Meta Quest VR headset

### Setup
Before you begin you will want to install Unreal engine. To do this you should first download the epic games launcher from the link above. Once you have installed the launcher, run it. Once the epic games 
launcher is installed, open it and either sign in or create an account. Once that's done, you should be taken to the main page for the launcher. If you look to the left of your screen you will see a link to the Unreal engine. If you click this, you will be taken to the unreal engine page. Then in the top right, you will see a button to install unreal engine. Click this and onces the install is done, you should now be able to launch the engine. The only way to view the blueprints of an unreal engine project is inside the unreal engine. If you want to make your own models, you can also download reality capture from this page. 

Once you have unreal engine installed and working, you can now open the file. To do this first unzip the file. Then open it and look for the unreal engine project file called Ocean_Life_VR. Then double click this file to open the project in Unreal engine. You can also, take the unzipped file and place it in the Unreal_projects file that should have been created once you installed and opened the Unreal engine. Drop the unzipped file into the unreal projects file. Then you can launch unreal engine from the epic games launcher. You will see a project called Ocean_Life_VR, which you can then open to see the project.

Now you will want to get VR setup so you can run it in the Unreal engine. To do this first you will want to setup the VR. This can be done by following the instructions of the VR when you first turn it on. Once you have set up your VR you will want to connect it to your PC. To do this for a Meta Quest VR, You will want to download the Meta Quest link app on your PC. Then sign into your Meta Quest account on the PC app. You will then want to connect your Meta Quest to your PC through the app either using a cable or air link. Once your VR headset is connected you want to go to settings in your Meta Quest PC app and go to General and set Meta Quest link as OpenXR runtime. This will mean you wont have to use third party software like Steam to connect to the unreal engine. 

Now that your VR headset is connected to your PC, you now need to set up the project so you can start it in VR. To do this, open the project in Unreal engine. Then in the top right of the screen click the settings button. This will show a dropdown. Click the project settings. Then click Maps and Models underneath the Project section. You will see a section to select the Default gamemode. Click this and set it to the VRGameMode. If your VR headset is connected, you should now be able to click the 3 dots in the menu at the top of the screen and select VR preview. Once thats done your almost ready to play the level in VR. 

For the final step, click the content drawer in the bottom left and click the folder called Stage. You will see an item in the folder called level. Click this twice to open the ocean environment. Finally click the green triangle in the top menu to begin playing the sample environment in VR. 

### Files in the codebase
Once you have opened the project in Unreal engine, You can click the content drawer in the bottom left to see the files in the content foleder: 
- Character : Contains animations, meshes and materials for the movement and animations of a VR character's hands 
- FirstPerson : Contains the blueprints, and inputs for the controls of a first person character. Though not used in the final prototype, can still be used to test debugging
- FirstPersonArms : Contains the animation and character models for the first person character
- Fishes : Contains the materials, textures and static meshes used for the fishes
- FX : Contains any special FX used in the project, in this case, the schooling system
- LevelPrototyping : Some basic shapes and materials used to build levels.
- PhotoModels : Contains the static meshes, materials and textures for the photogrammetric models used in the project
- PickupFish : Interface and UI used to interact with fishes in first person. Not used in final project
- Scenery : Contains sand, water and other materials and textures used in the stage
- Stage : Contains the prototype level. Double click to see the prototype and run to test out
- View_items : Contains the items used in the stages, as well as the view interface and UI's. This includes fish items and coral arrows placed near corals on the map. The interface which all these items use to be able to be viewed and display information to the users and the UI's that display this information
- VRTemplate : The blueprints, FX, materials and inputs for the VR character and its controls

### Code we've implemented or changed: 
To look at the Blueprints of an asset, double click it 
- FirstPerson/Blueprints : Added some code to pickup fish with pickup interface. Added the function Looking.
- VRTemplate/Blueprints/VRPawn : Added code to check area for items like coral or fishes. Also to show information if fish picked up. Added functions looking, AreaCheck, stopInspect, ToggleInspect.
- View_items : All assets in this folder added by us. The items are the things users interact with on stage. The UI is the displays the user see's. The interface is the interact interface which all items implement in order to be able to be interacted with. 
For the UI widgets look at the top right and click Graph to view the blueprint

Stage designed with inspiration from this video : https://www.youtube.com/watch?v=xHH1R7VPcTA

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
All models and information were created with throurogh research and an aim to show the true data as it is. None of the images were edited in a way to display a false narrative before the models were formed, and the models were created to the best of our ability to show the data as accurate as possible. 

### Troubleshooting videos and guides:
- If you are having trouble installing unreal engine watch this video : https://www.youtube.com/watch?v=ODxm8iuOVak
- If you are having trouble creating an epic games account watch this video : https://www.youtube.com/watch?v=5h2h7_232y0
- If you are having trouble linking your VR headset to your PC, follow the guide on the official Meta Quest page here : https://www.meta.com/en-gb/help/quest/articles/headsets-and-accessories/oculus-link/connect-with-air-link/
- If you are having trouble changing to VR gamemode or setting to VR preview follow along with this video : https://www.youtube.com/watch?v=Qoa6hdxGOL8
