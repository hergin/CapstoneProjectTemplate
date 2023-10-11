# Domain Model
  
[./image1.png](image)

Note that many of these components are likely already specified by the existing software. Our design will be adapted once we have access to the code.

Recorder: The software responsible for connecting to and reading sensor data from the VRDevice.

VRDevice: The VR headset itself, accessed via the applicable SDK.
MomentaryData: A generic representation of a sensor reading at a single moment in time. The data it contains may be a frame of video, the current heart rate, or whatever else is being collected.

WebUI: The frontend through which users and analysts may log in to access session data.

Database: The storage method for collected session data. The database is hosted on AWS and thus is accessed over the network.

Session: An aggregation of all the data collected over a single VR session. This class is associated with a six-digit access code, which is required for access by users. Each session is uniquely identified by its start time; this behavior may be adjusted in the case of collisions.

User: A person who may log in to the WebUI in order to access session visualizations. They differ from analysts in that they must have the appropriate access code for any session they wish to access.

Analyst: A person who may log in to the WebUI in order to access visualizations. They may access any session without the need for its access code, and may also access the session's raw data in addition to visualizations.