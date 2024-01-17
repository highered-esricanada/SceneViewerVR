## Scene Viewer VR
The Scene Viewer VR application lets users view web scenes hosted on ArcGIS Online with the high quality rendering of the Unity game engine and in virtual reality.

## Demo
![demo](/demo.gif) (Video using the headset)

## Features
The following web scene features have been included in the app:
- Global and local scenes
- Slides (including layer visibility settings, camera, and sun position)
- Layer opacity
- Coloured object scene layers
- Layers supported (based on support in the ArcGIS Maps SDK)
    - Image tile layer
    - Vector tile layer
    - Elevation tile layer
    - 3D object scene layer 
    - Building scene layer
    - Integrated mesh layer

## Requirements
The application has been developed and tested on Windows 10. It can be used with or without VR heasdsets. Windows Mixed Reality headsets and the Quest from Oculus using the link cable are supported. 

The app was created using the [ArcGIS Maps SDK for Unity](https://developers.arcgis.com/unity/) and requires an internet connection.   

## Instructions

### Getting Started
1. Download the application [here](https://github.com/highered-esricanada/SceneViwerVR/releases/download/SceneViewer.zip).
1. Unzip to a local folder on your machine.
1. Double click on the Scene Viewer.exe file.
1. If you are on a headset, press the menu button on the controller to toggle the display of the main menu (You can press the left thumbstick in to show tooltips on the controllers to identify the menu button). You can press the escape key on the keyboard if you are not using a headset.
1. Use the ray coming out of the right controller and the right trigger button to select items on the menu. You can use your mouse if you are not using a headset to select menu items.

The menu lets you choose the scene you would like to load:

![menu](/main_menu.png)

Once selected, you can use the arrow buttons to browse the bookmarks if available

![bookmarks](/bookmark.png)

You can also change the time of day or year in the Options menu:

![lighting](/lighting.png)

Select the controls button to see the headset or keyboard/mouse controls.

### Updating the application's web scenes
The Scene Viewer VR currently only works with publicly accessible web scenes. These web scenes are defined in a scenes.json file in the "global view_Data\StreamingAssets" directory. Follow the format of specifying web scene ids and the scale. The scale property is used when in VR to set the default 

## Troubleshooting

### Cannot see globe view when launching app
1. Make sure the Unity preview windows that appears on your desktop has focus by clicking on the window.
1. Check that your internet connection is working, followed by checking the [ArcGIS Online Health Dashboard](https://status.arcgis.com/) for any service disruptions to ArcGIS Online.
1. If you are still unable to see the globe, there may be an issue with the API key. You can create your own API key [here](https://developers.arcgis.com/documentation/mapping-apis-and-services/security/tutorials/create-and-manage-an-api-key/) and copy it into the apikey.txt file in the "global view_Data\StreamingAssets" directory.
