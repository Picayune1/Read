# Ocean Life VR: Beneath The Waves
## Developed by the Do it for the Fish team, in collaboration with the Flying Fish Technologies team

### Description 
This project is a simulation of an underwater environment using VR. The simulation is built using Unreal Engine, and the main point of the project is to use real data, to educate people about the reefs and fishes. Currently this version of the project only has one environment model loaded. The environment model was built using the photogrammetry software Reality Capture and images of the environment. The purpose of this project is to be deployed in environments like an aquarium in order to educate users about reef and fishes.

### Requirements to run this program
- Unreal Engine (version 5.4 or later) link : https://www.unrealengine.com/en-US/download
- Meta Quest Link app : https://www.meta.com/en-gb/help/quest/articles/headsets-and-accessories/oculus-rift-s/install-app-for-link/
- Meta Quest VR headset

## Setup Instructions

### 1. Install Unreal Engine
1. Download and install the **Epic Games Launcher** from [this link](https://www.epicgames.com/store/en-US/download).
2. Once installed, open the Epic Games Launcher and either **sign in** or **create an account**.
3. On the left sidebar of the launcher, click on **Unreal Engine** to go to the Unreal Engine page.
4. In the top-right corner, click the **Install Engine** button to install Unreal Engine.
5. Once the installation is complete, you'll be able to launch Unreal Engine.

### 2. Download the Project
1. Unzip the project file (`Ocean_Life_VR.zip`).
2. Navigate to the folder where you unzipped the file.
3. Look for the Unreal Engine project file called `Ocean_Life_VR.uproject` and double-click it to open the project in Unreal Engine.

   - Alternatively, you can move the unzipped project folder into your `Unreal Projects` folder (which was created when Unreal Engine was first installed). Then launch the Epic Games Launcher and you should see the `Ocean_Life_VR` project listed. Click on it to open.

### 3. Set Up VR for Meta Quest
1. Set up your **VR headset** following the instructions that come with your device.
2. For Meta Quest:
   1. Download and install the **Meta Quest Link** app on your PC.
   2. Sign in to your Meta Quest account on the PC app.
   3. Connect your Meta Quest headset to your PC using a cable or Air Link through the Meta Quest app.
   4. Go to **Settings > General** in the Meta Quest PC app and set **Meta Quest Link as OpenXR runtime**.
      - This allows Unreal Engine to connect directly to the VR headset without using third-party software like SteamVR.

### 4. Configure the Project for VR in Unreal Engine
1. Open the `Ocean_Life_VR` project in Unreal Engine.
2. In the top-right corner, click **Settings** and select **Project Settings**.
3. Scroll to the **Maps & Modes** section under the **Project** tab.
   - In the **Default GameMode** section, set the game mode to **VRGameMode**.
4. If your VR headset is connected, click the **3 dots** menu at the top of the screen and select **VR Preview**.

### 5. Load the Ocean Environment Level
1. In Unreal Engine, click on the **Content Drawer** at the bottom left of the screen.
2. Navigate to the folder called **Stage**.
3. Double-click the **level** file in this folder to load the ocean environment.
4. To start playing the sample environment in VR, click the **green play button** (triangle icon) in the top menu.

Also note that if you do not have a VR headset, you can also experience this project in first person - but some features will not be designed for it.
 
### Files in the codebase
Once you have opened the project in Unreal Engine, You can click the content drawer in the bottom left to see the files in the content folder: 
- **Character** : Contains animations, meshes and materials for the movement and animations of a VR character's hands 
- **FirstPerson** : Contains the blueprints, and inputs for the controls of a first person character. Though not used in the final prototype, can still be used to test debugging
- **FirstPersonArms** : Contains the animation and character models for the first person character
- **Fishes** : Contains the materials, textures and static meshes used for the fishes
- **FX** : Contains any special FX used in the project, in this case, the schooling system
- **LevelPrototyping** : Some basic shapes and materials used to build levels.
- **PhotoModels** : Contains the static meshes, materials and textures for the photogrammetric models used in the project
- **PickupFish** : Interface and UI used to interact with fishes in first person. Not used in final project
- **Scenery** : Contains sand, water and other materials and textures used in the stage
- **Stage** : Contains the prototype level. Double click to see the prototype and run to test out
- **View_items** : Contains the items used in the stages, as well as the view interface and UI's. This includes fish items and coral arrows placed near corals on the map. The interface which all these items use to be able to be viewed and display information to the users and the UI's that display this information
- **VRTemplate** : The blueprints, FX, materials and inputs for the VR character and its controls

### Code we've implemented or changed: 
To look at the Blueprints of an asset, double click it 
- **FirstPerson/Blueprints** : Added some code to pickup fish with pickup interface. Added the function Looking.
- **VRTemplate/Blueprints/VRPawn** : Added code to check area for items like coral or fishes. Also to show information if fish picked up. Added functions looking, AreaCheck, stopInspect, ToggleInspect.
- **View_items** : All assets in this folder added by us. The items are the things users interact with on stage. The UI is the displays the user sees. The interface is the interaction interface which all items implement in order to be able to be interacted with. 
For the UI widgets look at the top right and click Graph to view the blueprint

Stage designed with inspiration from this video : https://www.youtube.com/watch?v=xHH1R7VPcTA

### Credits for the 3d model: 
- Fish Collection by shedmon : https://sketchfab.com/3d-models/fish-collection-84a4238a77e541f0ae7db54ccf9f6d8e No changes made
- Yellow tang by JayNme : https://sketchfab.com/3d-models/oxidane-yellow-tang-5750f70ac6734728b0eb3ed81de9bb2d No changes made
- Triggerfish by Jivo3dAssets : https://3dexport.com/3dmodel-triggerfish-416259.htm Some changes made
- Coral beauty fish : https://free3d.com/3d-model/coral-beauty-angelfish-v1--473554.html No changes made
- Underwater environment made in photogrammetry software Reality Capture using images provided by the Flying Fish Technologies team. 

### Privacy concerns
Unreal Engine does collect data from users such as hardware performance, usage statistics and other information about what users do on the platform. If you are uncomfortable with this you can disable it. To do this open the project and in the top menu click edit. This will show a dropdown menu, where you will want to click editor preferences. Click this and scroll down to privacy. Then click both bug reports and user data and click don't send. This will stop any personal data from being sent to Epic Games. None of our written blueprints collect data, and you can read through the whole project to check if you're still concerned.

### Security concerns
If one is concerned about the project zip file, like if it has been changed malicously, remove the readme file and check the hash. The MD5 checksum hash of the project should be :  
ece0f2f5b701f7205f5e722df7ffdb72

### Ethical concerns
All models and information were created with thorough research and an aim to show the true data as it is. None of the images were edited in a way to display a false narrative before the models were formed, and the models were created to the best of our ability to show the data as accurate as possible. 

### Troubleshooting videos and guides:
- If you are having trouble installing Unreal Engine watch this video : https://www.youtube.com/watch?v=ODxm8iuOVak
- If you are having trouble creating an Epic Games account watch this video : https://www.youtube.com/watch?v=5h2h7_232y0
- If you are having trouble linking your VR headset to your PC, follow the guide on the official Meta Quest page here : https://www.meta.com/en-gb/help/quest/articles/headsets-and-accessories/oculus-link/connect-with-air-link/
- If you are having trouble changing to VR gamemode or setting to VR preview follow along with this video : https://www.youtube.com/watch?v=Qoa6hdxGOL8

Once again thanks to the team at Flying Fish Technologies.
