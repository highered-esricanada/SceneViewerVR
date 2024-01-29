## Scene Viewer VR
The Scene Viewer VR application lets users view ArcGIS Online hosted web scenes with the Unity game engine and in virtual reality.

![intro](/intro.png)

## Features
The following web scene features have been included in the app:
- Global and local scenes
- Slides (including layer visibility, camera, and sun position)
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
The application has been developed and tested on Windows 10. It can be used with or without VR heasdsets. Windows Mixed Reality headsets and the Meta Quest with the link cable are supported. 

The app was created using the [ArcGIS Maps SDK for Unity](https://developers.arcgis.com/unity/) and requires an internet connection.   

## Instructions

### Getting Started
1. Download the application [here](https://github.com/highered-esricanada/SceneViewerVR/releases/download/1.0/Scene.Viewer.VR.zip).
1. Unzip to a local folder on your machine.
1. Double click on the Scene Viewer.exe file.
1. If you are using a headset, press the menu button on the controller to toggle the display of the main menu (You can press the left thumbstick in to show tooltips on the controllers to identify the menu button). You can press the escape key on the keyboard if you are not using a headset.
1. Use the ray coming out of the right controller and the right trigger button to select items on the menu. You can use your mouse if you are not using a headset to select menu items.

The menu lets you choose the scene you would like to load:

![menu](/main_menu.png)

Once selected, you can use the arrow buttons to browse the bookmarks if available.

![bookmarks](/bookmark.png)

You can also change the time of day or year in the Options menu:

![lighting](/lighting.png)

Select the Controls Help button to see the headset or keyboard/mouse controls.

### Updating the application's web scenes
The application currently works with publicly accessible web scenes. These web scenes are defined in a scenes.json file in the "global view_Data\StreamingAssets" directory. Follow the format of specifying web scene ids and the scale. The scale property is used when in VR. For example, a scale of 5 will set the model scale to 1:5. Objects in the scene will be one fifth of the real-world size.  

The following web scenes are included when you download the app:

|Name|id|
| --- | --- |
|3D BAG WGS|[586e62704afc441ead838a4abfafc2f8](https://www.arcgis.com/home/item.html?id=586e62704afc441ead838a4abfafc2f8)|
|Mountain Biking in Bavaria|[1b787e0335af4929a4a5267ebfa58a20](https://www.arcgis.com/home/item.html?id=1b787e0335af4929a4a5267ebfa58a20)|
|Visualize New Developments|[19dcff93eeb64f208d09d328656dd492](https://www.arcgis.com/home/item.html?id=19dcff93eeb64f208d09d328656dd492)|
|Everest 1953 Sagarmatha Chomolungma|[cb67c8d220ef44b7a359d207f2df2fd4](https://www.arcgis.com/home/item.html?id=cb67c8d220ef44b7a359d207f2df2fd4)|
|Montreal, Canada Scene|[63a16e0c9f364d0fab9d55f40bf71771](https://www.arcgis.com/home/item.html?id=63a16e0c9f364d0fab9d55f40bf71771)|
|Copy of Reality Mesh Examples by bconnolly_IVT|[aae50a6ccf5c484a917750897a1d59a9](https://www.arcgis.com/home/item.html?id=aae50a6ccf5c484a917750897a1d59a9)|
|Mountains|[9c6384f5003a4008b1819c212c5a9105](https://www.arcgis.com/home/item.html?id=9c6384f5003a4008b1819c212c5a9105)|
|Turanga Library|[543648a92446497db8a92c06ce1ad0b1](https://www.arcgis.com/home/item.html?id=543648a92446497db8a92c06ce1ad0b1)|
|Scene of Vancouver, Canada Scene|[e4781c19442d40d580637cde7ca87937](https://www.arcgis.com/home/item.html?id=e4781c19442d40d580637cde7ca87937)|
|NGA New York City NY 3D Buildings and Trees 2013|[919277d789a641f5a580ddc1d5903640](https://www.arcgis.com/home/item.html?id=919277d789a641f5a580ddc1d5903640)|
|NGA Philadelphia - Trenton - Wilmington|[942d42a494874057bc20395afe2828cb](https://www.arcgis.com/home/item.html?id=942d42a494874057bc20395afe2828cb)|
|Buildings Philadelphia|[db2f366cc8c64549a7a5f74fa8cd1460](https://www.arcgis.com/home/item.html?id=db2f366cc8c64549a7a5f74fa8cd1460)|
|Linz, Austria|[5e3f870f59ca4d9da5ca4184c99b5edb](https://www.arcgis.com/home/item.html?id=5e3f870f59ca4d9da5ca4184c99b5edb)|
|San Francisco Styled|[85cbe6113ce64edca7696c6104481b87](https://www.arcgis.com/home/item.html?id=85cbe6113ce64edca7696c6104481b87)|
|Toronto Massing Scene|[a0031de092324a4d9ef5da4bf627502d](https://www.arcgis.com/home/item.html?id=a0031de092324a4d9ef5da4bf627502d)|

## Troubleshooting

### Cannot see the globe when launching the app
1. Check that your internet connection is working, followed by checking the [ArcGIS Online Health Dashboard](https://status.arcgis.com/) for any service disruptions on ArcGIS Online.
1. If you are still unable to see the globe, there may be an issue with the API key. You can create your own API key [here](https://developers.arcgis.com/documentation/mapping-apis-and-services/security/tutorials/create-and-manage-an-api-key/) and copy it into the apikey.txt file in the "global view_Data\StreamingAssets" directory.

### VR Controllers do not move in the app
1. Make sure the Unity preview windows that appears on your desktop has focus by clicking on the window.
