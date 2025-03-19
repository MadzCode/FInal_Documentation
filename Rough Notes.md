
https://github.com/user-attachments/assets/60b2b5eb-a4bd-4225-b121-49758a91f6a7
### Rough Notes

## Cam System
https://www.youtube.com/watch?v=ZmIzHtglnMM&t=96s
![image](https://github.com/user-attachments/assets/d3ca7b75-539e-434f-8013-84629ff47b8e)
![image](https://github.com/user-attachments/assets/465ede1f-908d-4379-b19a-1c536208e991)


The camera is not looking at the correct location, cannot rotate camera


https://github.com/user-attachments/assets/faa4f62b-b49c-48fb-84ef-cf13d31d1323


https://github.com/user-attachments/assets/1eeab146-34ec-4e6c-ae24-a434e9e8f8a5
- fixed direction but the movement is too smooth

https://blueprintue.com/blueprint/d6-zmgms/
- to help stop the player from turning the camera I disabled the camera movement by always having the mouse on screen

https://blueprintue.com/blueprint/eknuf5e9/ 
- Spline Movement

I went for more of a resident evil feel but it feels a bit sudden
https://www.youtube.com/watch?v=O7SjrIrY_io

https://github.com/user-attachments/assets/884cf8c0-9d5a-4080-8d93-a591b34ba2d4

https://github.com/user-attachments/assets/cf017509-7dea-4670-a708-345a69fa9988

I made the Camera not follow the player and It looks better I will research more into animating the camera





## Light System
![image](https://github.com/user-attachments/assets/d7466631-da96-4a7f-bf13-882bddc76d77)
![image](https://github.com/user-attachments/assets/62b50042-5fd6-4962-8b75-e4960928e555)
used copilot to help with this


https://github.com/user-attachments/assets/6d8c1599-a92c-4676-a710-48d32220e92a


https://github.com/user-attachments/assets/79d63893-3249-482c-aa5e-a6df6513ac5b



## 2 Player System

## 2D Character movement
- I decided to completly remake the character movement to allow me to create better 3d movement
- my artist James Davies created some rough sprites to allow me to make sure the movement looks correct
https://www.youtube.com/watch?v=0f1_qSXbqAI
![Idle](https://github.com/user-attachments/assets/9ae707b5-522d-446e-b81f-570db16941b3)
![Jumping](https://github.com/user-attachments/assets/8121c110-4142-409d-a37f-df4e9cbf5ff4)
![Walking Transition](https://github.com/user-attachments/assets/e7842da4-34b3-4cf6-a773-08b211b06062)
![Walk 1](https://github.com/user-attachments/assets/30576ac0-5e46-43ce-8c65-45d1fd019bde)
![Walk 2](https://github.com/user-attachments/assets/eb8e19f2-8828-4c4a-b3d1-98b7be93e38c)



-Added PaperZD
https://www.fab.com/listings/6664e3b5-e376-47aa-a0dd-f7bbbd5b93c0
https://www.youtube.com/watch?v=0f1_qSXbqAI
![image](https://github.com/user-attachments/assets/da6a5260-5478-4a76-8043-0c865821c29c)

- Made Player_BP
![image](https://github.com/user-attachments/assets/58286c68-50f8-4232-bc31-f4bd49cb2c21)

- Made Player Controller
![image](https://github.com/user-attachments/assets/a6df1f63-ed60-41e1-8ce8-af23628dd670)

- Added Animation Source
![image](https://github.com/user-attachments/assets/964e1dde-a7b2-4fdb-a4ba-78d792f2439c)

- Added PaperZD AnimBP
![image](https://github.com/user-attachments/assets/a9f8575b-dbc0-439a-9168-cfebbdc325eb)

- Imported the Sprites
![image](https://github.com/user-attachments/assets/211283cd-c94f-4d13-9f1a-215a36b72cc7)
![image](https://github.com/user-attachments/assets/777ac99c-a964-407f-9355-750105bcbec3)

- then I turned them all into sprites using the create sprite menu
![image](https://github.com/user-attachments/assets/6c3197dd-1a04-40ae-aaef-4f3a46ac20bf)

- Then I turned all of the sprites into Flipbooks
![image](https://github.com/user-attachments/assets/4175dd69-13f8-4a3b-bbee-fc2538ee736c)
![image](https://github.com/user-attachments/assets/cde3c1f2-fb43-4a08-910f-b9c985024b5e)

- Animation Preview
![Early Walking Anim](https://github.com/user-attachments/assets/ea1b6d52-dc67-4891-ab60-ce0b2eef51b2)

- Added sprit to player bp
![image](https://github.com/user-attachments/assets/f6ae2c97-509f-4d64-a4c5-750dc0b28d6e)

- casting a shadow
 ![image](https://github.com/user-attachments/assets/fce2366e-a86a-48cf-8867-8aa29326f3f6)

- I made it a MaskedLitSpriteMaterial to make sure the character can have light shine on it to   
![image](https://github.com/user-attachments/assets/fd46c3b4-35a7-49ac-a57c-1346c44bf092)

- overwrote the old gamemode with my new one so it work
![image](https://github.com/user-attachments/assets/a930a011-25ca-4ed3-acf4-a9597f081fe8)

- Finished Animations and added a jump

https://www.youtube.com/watch?v=aWkgOr5U-zI

- The code worked fine until I tried to use a flip flop to deal with the animations, trying state machines instead
  
https://blueprintue.com/blueprint/o0i6lbe8/
- Reworking the movement

![image](https://github.com/user-attachments/assets/9468fd03-1a60-4d18-a002-09ab43a55c3b)

![image](https://github.com/user-attachments/assets/0f4f6302-f984-4f10-81e0-5ad34f5903af)

https://www.youtube.com/watch?v=KZWybxR46-4

https://github.com/user-attachments/assets/6d6cf995-6812-4653-82d7-826e06ff5a99

https://github.com/user-attachments/assets/39ba90dc-81fc-468d-9d50-9dc6a16e37e9

https://github.com/user-attachments/assets/a8201d14-5b2f-47e4-a656-f36e4832b93c




https://github.com/user-attachments/assets/eb4b25b6-87b9-4951-a73c-77c19b8a1aeb




### Cursor Mechanic
![image](https://github.com/user-attachments/assets/bca8ea41-f575-4122-ae6f-75db2460fd18)
https://www.youtube.com/watch?v=8VZtDdKApeM

### UI
<img width="1252" alt="{08FFB487-965C-4603-8FBF-8B7FBAAA8412}" src="https://github.com/user-attachments/assets/565679bd-121d-4e01-abcd-b12c5a2ec5a1" />


https://github.com/user-attachments/assets/6129a141-02ff-4d4a-9e4f-22ea746900cc


https://github.com/user-attachments/assets/f3d6e354-b03e-40bf-b741-49ba13dc9b69



https://github.com/user-attachments/assets/0cb821bd-9a7e-4488-a9f6-08b8f938bad7



https://www.youtube.com/watch?v=kumZj_mov58&t=266s

https://www.youtube.com/watch?v=Ff67XtqgSxc&t=103s

Overwrote the esc shortcut so there is a pause menu
![image](https://github.com/user-attachments/assets/35b11460-27e0-4150-b284-166cf00179f5)

https://www.youtube.com/watch?v=lacx5J8FoXI

I was having issues of the pause code not unpausing but I fixed it using this forum
https://forums.unrealengine.com/t/trying-to-get-the-game-to-pause-unpause-with-the-same-button-messes-with-my-controls/253670

issue with the dialogue doing the print string but not the text of the dialogue


https://github.com/user-attachments/assets/f1de46bc-05a7-46ea-9ad1-47cea7af8cc2

this video for dialogue
https://www.youtube.com/watch?v=Z8q1eMU2Gjo

### Shadow Character powers
https://blueprintue.com/blueprint/41-2dd55/

- Got help from AI Still Broken but closer to goal
  Spawning an Object at Mouse Location When Pressing "E" in Unreal Engine (Using Blueprints)

Create the Spawnable Object Blueprint:

Create a new Blueprint class named BP_SpawnableObject.

Set Up Player Controller:

Open your PlayerController Blueprint.

Add an "InputKey" event for the "E" key.

Add a "Get Player Controller" node.

Get Mouse Position:

Use the "Get Hit Result Under Cursor by Channel" node.

Connect it to "Get Player Controller".

Set the "Trace Channel" to Visibility.

Promote the "Hit Result" to a variable (HitResult).

Break Hit Result:

Drag the HitResult variable and break it using "Break Hit Result".

Access the Location pin.

Set Up Transform:

Connect the Location to the Location input of a "Make Transform" node.

Set Rotation to 0,0,0 and Scale to 1,1,1.

Spawn the Actor:

Connect the "Make Transform" node to the Spawn Transform input of "Spawn Actor from Class".

Ensure the "Spawn Actor from Class" node is set to spawn your BP_SpawnableObject.

https://github.com/user-attachments/assets/2219d771-c042-4e6b-a59a-d5daed33b345

![image](https://github.com/user-attachments/assets/ec3c3114-fcad-4fc0-926f-ed5614994348)


https://github.com/user-attachments/assets/8ae8b5cb-ad89-4769-8c19-c79b689509e6

https://www.youtube.com/watch?v=T3Vou11FGss


https://github.com/user-attachments/assets/786b0a97-5f8f-48e2-8d3f-0aef5a3ab4a3


https://www.youtube.com/watch?v=rF_oIaDvtJ4
### CSV File (Dialogue)
https://gdcvault.com/play/1025055/Audio-Asset-Management-Tips-and
https://dev.epicgames.com/documentation/en-us/unreal-engine/data-driven-gameplay-elements-in-unreal-engine?application_version=5.4
https://docs.google.com/spreadsheets/d/1-5I0bgjq7tCaSo0pwK05oLpwlT2uFYdOTOCDr0gBt6o/edit?gid=0#gid=0
