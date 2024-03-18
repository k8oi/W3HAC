### RH Digital Client Operation Procedure
1. Start Remote Hams
	1. Check Audio: SPKR & MIC to Line 1
	1. Check Virtual Devices
	1. Connect to W3HAC
	1. System -> Sound -> More Sound Settings
		1. Playback -> Line 1 -> Levels: Line 1 95%, Main Vol 25%
		1. Recording -> Line 1 -> Levels: Set to 5%
1. Start White Noise App
	* Select "White Noise" Sounds and click "Play"
1. System -> Sound -> Volume Mixer
	1. Set White Noise app to 10%
	1. Set White Noise "Output device" to Line 1
	1. Set White Noise "Input device" to Default
---
### Start RemoteHams, White Noise, PstRotator, & WSJTX
1. Connect to RemoteHams Server
	1. Search for W3HAC
	1. Select HacDC ... W3HAC and right mouse click to Add Favorite
	1. Double Click and Connect
	1. Remote Sliders
		1. DSP Low Cut-Off: 0KHz
		1. DSP high Cut-Off: 5 KHz
		1. AF Gain: 255 (100%)
		1. RF Gain: 255 (100%)
		1. RF Power: 100W (100%)
	1. Drop Down (Left Options)
		1. Mode: USB
		1. AGC: Fast
		1. Tx Meter: ALC
	1. Buttons (Right Options)
		1. The ONLY button which should be ON is the PWR button
		1. Turn off all other buttons
1. KPA1500 (Amplifier)
	1. Select **STBY** to leave the amp OFF unless you REALLY think you need big power
    2. **IF You are planning to use the amp**; please ensure you set the ***RF Power*** Slider to a **10% level** as a starting point. *Too much RF Power will cause the amp to trip if you are not careful!!!*
1. Start White Noise
	1. Open Sound Mixer and ensure White Noise is about 10% and Output Device is set to Line 1 (The same as the RCF Orb Client)
	1. Start playing white noise
1. Start WSJTX
	1. Ensure the WSJTX Pwr level is about 18% (for K8OI) - you need to test and ensure no ALC movement and you are getting the power out that you want
1. Start PstRotator
1. WSTX - select band
1. RemoteHams - press Tune 3 times
#### NOTES
* WATCH the ALC on the RemoteHams display - you do NOT want it to MOVE at ALL
* WATCH the Power Out Meter on the KPA1500 box- aim for 25-35 watts out as a good starting point
