### RemoteHams Digital Setup
VAC Install and Sound Device Config
1. Install VAC 7 Full
2. VAC Control Panel (Run as Administrator)
    1. Set "Cables" to 1
    2. Ensure "Volume control" is enabled
3. System -> Sound
    1. Set default audio device drivers to your preference
4. System -> Sound -> More Sound Settings -> Playback Tab -> Line 1 Properties -> Levels Tab
    1. Line 1 Set to 95%
    2. Main Volume Set to 25%
5. System -> Sound -> More Sound Settings -> Playback Tab -> Line 1 Properties -> Advanced Tab
    1. Disable "Enable audio enhancements"
6. System -> Sound -> More Sound Settings -> Playback Tab -> Line 1 Properties -> "Spacial Sound" Tab
    1. Line 1 Set to "Off"
7. System -> Sound -> More Sound Settings -> Recording Tab -> Line 1 Properties -> Levels Tab
    1. Line 1 VAC Recording is set to 5%
8. System -> Sound -> More Sound Settings -> Recording Tab -> Line 1 Properties -> Advanced Tab
    1. Disable "Enable audio enhancements"

White Noise Application Install & Volume Mixer Config
1. Install preferred White Noise Application
    1. I used "TMSoft White Noise App" https://www.tmsoft.com/
2. Start White Noise App
3. System -> Sound -> Volume Mixer
    1. Set White Noise app to 10%
    2. Set White Noise "Output device" to Line 1
    3. Set White Noise "Input device" to Default

RCFOrb Client Install & Configuration
1. Install RCFOrbClient
    1. http://download.remotehams.com/
    2. NOTE
        1. I used v0.9.309
        2. The later versions have some kind of Virtual Serial Port latency which affects WSJT-X PTT keying and I haven't figured out a way to fix it
2. Start RCFOrbClient
    1. Audio Tab
        1. Set SPKR and MIC are connected to "Line 1"
    2. Virtual Devices Tab
        1. Virtual K3: Select a Com Port & Set to "On"
        2. Virtual Rotator: Select a Com Port & Set to "On"
3. Connect to RemoteHams Server
    1. Search for W3HAC
    2. Select HacDC ... W3HAC and right mouse click to Add Favorite
    3. Double Click and Connect

WSJT-X Install & Configuration
1. Install WSJT-X
    1. https://wsjt.sourceforge.io/wsjtx.html
    2. NOTE: I used 32bit v2.6.1
    3. Install the updated HamLib: https://wsjt.sourceforge.io/support.html
    4. NOTE: I used 32bit Hamlib DLL
2. Start WSJT-X
3. File -> Settings -> Radio Tab
    1. Rig: Elecraft K3
    2. Cat Control: Serial Port -> Select the RCFOrbClient Virtual K3 COM Port
    3. Data Bits: 8
    4. Stop Bits: 1
    5. Handshake: None
    6. PTT Method: CAT
    7. Mode: USB
    8. Split Operation: Fake It
4. File -> Settings -> Audio Tab
    1. Soundcard Input: Line 1
    2. Soundcard Output: Line 1

PstRotator Install & Configuration
1. Install PstRotator
    1. https://pstrotator.com/
    2. NOTE: I installed PstRotatorAz
2. Setup -> Controller: DCU-1 Hy-Gain
3. Setup -> My Location: My Locator FM18JW (W3HAC Remote Site Grid)
4. Communication -> Azimuth COM Port: Select the RCFOrbClient Virtual Rotator COM Port
5. Setup -> Trackers Setup -> Test & Save Setup
    1. NOTE: WSJT-X must be running for this test to work
6. Set Tracker -> WSJT-X
Now


