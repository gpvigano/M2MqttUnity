M2MQTT for Unity
====================
This is a simple [Unity3d](http://unity3d.com/) project for using [M2MQTT](https://github.com/eclipse/paho.mqtt.m2mqtt) with Unity.
The M2MQTT library was modified to run also on UWP/HoloLens.

An example scene is provided with a UI for controlling the connection to the broker and for testing messaging.

**Requires Unity 2017.1 or higher.**

 ![image](https://raw.githubusercontent.com/gpvigano/M2MqttUnity/master/images/M2MqttUnity_UI.png)

### Getting started
To try this project with Unity press the button **Clone or download** and choose [**Download ZIP**](https://github.com/gpvigano/M2MqttUnity/archive/master.zip). Save and unzip the archive to your hard disk and then you can open it with Unity.
An example scene is provided in M2MqttUnity/Examples/Scenes/M2MqttUnity_Test, with a UI for controlling the connection to a MQTT broker and to test publishing and receiving messages.
You can find in the same folder also a scene slightly changed to test the project in VR/AR/MR (M2MqttUnity_TestXR).

### Building on different platform and devices
This project was tested with different versions of Unity (2017.1.0, 2017.1.4, 2018.2) with the following platforms:
* Windows Standalone
* Android (as simple app and for GearVR)
* Universal Windows Platform (desktop and HoloLens, using Unity 2017.1.4 or higher).

These setting were used for all the platforms:
* Other settings:
  * *Scripting Define Symbols* = SSL
* Resolution
  * *Default is fullscreen* = no
  * *Run in Background* = yes

Specific settings for Android:
* Set the *Package Name*
* for **GearVR**:
  * check Virtual Reality Supported (or XR for newer versions of Unity)
  * add *Oculus* in *Virtual Reality SDKs*
  * set *Minimum API Level* to 19
  * put your "oculussig..." file(s) in Assets/Plugins/Android/Assets

Specific settings for Universal Windows Platform:
* build with Unity 2017.1.4 or newer
* set the *Package Name*
* *Other settings*: set *API Compatibility Level* to .NET 4.6
* *Publishing settings*: check *InternetClient* in *Capabilities*  
* *Scripting Backend* set to .NET (deprecated in 2018.2) or IL2CPP (not for 2017.1)
* for **HoloLens**:
  * check *Virtual Reality Supported* (or XR for newer versions of Unity)
  * add *Windows Holographic* (*Windows Mixed Reality* in newer versions) in *Virtual Reality SDKs*

SSL connection problems found with some combination of Unity versions/platforms.


### Contributing

Contributions from you are welcome!

If you find bugs or you have any new idea for improvements and new features you can raise an issue on GitHub (please follow the suggested template, filling the proper sections). To open issues or make pull requests please follow the instructions in [CONTRIBUTING.md](https://github.com/gpvigano/M2mqttUnity/blob/master/CONTRIBUTING.md).

### License

Released under the [MIT License](https://github.com/gpvigano/M2MqttUnity/blob/master/LICENSE.txt).

The included (slightly modified) [M2MQTT](https://github.com/eclipse/paho.mqtt.m2mqtt) library is licensed under [Eclipse Public License 1.0](https://github.com/eclipse/paho.mqtt.m2mqtt/blob/master/LICENSE).