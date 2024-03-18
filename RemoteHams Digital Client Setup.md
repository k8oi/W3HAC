### RemoteHams Digital Setup
#### VAC Install and Sound Device Config
1. Install VAC 7 Full
1. VAC Control Panel (Run as Administrator)
    1. Set "Cables" to 1
    1. Ensure "Volume control" is enabled
1. System -> Sound
    * Set default audio device drivers to your preference
1. System -> Sound -> More Sound Settings -> Playback Tab -> Line 1 Properties -> Levels Tab
    1. Line 1 Set to 95%
    1. Main Volume Set to 25%
1. System -> Sound -> More Sound Settings -> Playback Tab -> Line 1 Properties -> Advanced Tab
    * Disable "Enable audio enhancements"
1. System -> Sound -> More Sound Settings -> Playback Tab -> Line 1 Properties -> "Spacial Sound" Tab
    * Line 1 Set to "Off"
1. System -> Sound -> More Sound Settings -> Recording Tab -> Line 1 Properties -> Levels Tab
    * Line 1 VAC Recording is set to 5%
1. System -> Sound -> More Sound Settings -> Recording Tab -> Line 1 Properties -> Advanced Tab
    * Disable "Enable audio enhancements"
---
#### White Noise Application Install & Volume Mixer Config
1. Install preferred White Noise Application
    * I used "TMSoft White Noise App" https://www.tmsoft.com/
1. Start White Noise App
1. System -> Sound -> Volume Mixer
    1. Set White Noise app to 10%
    1. Set White Noise "Output device" to Line 1
    1. Set White Noise "Input device" to Default
---
#### RCFOrb Client Install & Configuration
1. Install RCFOrbClient
    1. http://download.remotehams.com/
    1. NOTE
        1. I used v0.9.309
        1. The later versions have some kind of Virtual Serial Port latency which affects WSJT-X PTT keying and I haven't figured out a way to fix it
1. Start RCFOrbClient
    1. Audio Tab
        * Set SPKR and MIC are connected to "Line 1"
    1. Virtual Devices Tab
        1. Virtual K3: Select a Com Port & Set to "On"
        1. Virtual Rotator: Select a Com Port & Set to "On"
1. Connect to RemoteHams Server
    1. Search for W3HAC
    1. Select HacDC ... W3HAC and right mouse click to Add Favorite
    1. Double Click and Connect
---
#### WSJT-X Install & Configuration
1. Install WSJT-X
    1. https://wsjt.sourceforge.io/wsjtx.html
    1. NOTE: I used 32bit v2.6.1
    1. Install the updated HamLib: https://wsjt.sourceforge.io/support.html
    1. NOTE: I used 32bit Hamlib DLL
1. Start WSJT-X
1. File -> Settings -> Radio Tab
    1. Rig: Elecraft K3
    1. Cat Control: Serial Port -> Select the RCFOrbClient Virtual K3 COM Port
    1. Data Bits: 8
    1. Stop Bits: 1
    1. Handshake: None
    1. PTT Method: CAT
    1. Mode: USB
    1. Split Operation: Fake It
1. File -> Settings -> Audio Tab
    1. Soundcard Input: Line 1
    1. Soundcard Output: Line 1
---
#### PstRotator Install & Configuration
1. Install PstRotator
    1. https://pstrotator.com/
    1. NOTE: I installed PstRotatorAz
1. Setup -> Controller: DCU-1 Hy-Gain
1. Setup -> My Location: My Locator FM18JW (W3HAC Remote Site Grid)
1. Communication -> Azimuth COM Port: Select the RCFOrbClient Virtual Rotator COM Port
1. Setup -> Trackers Setup -> Test & Save Setup
    * NOTE: WSJT-X must be running for this test to work
1. Set Tracker -> WSJT-X
