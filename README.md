# PilferShush Jammer
Android microphone checker and passive jamming application.  

Test application for low battery requirement microphone jamming.

Calls audioRecord.startRecording() but DOES NOT READ THE AUDIO BUFFER.

Claims audio focus and should block user apps from gaining focus of microphone.

System apps (telephony) should override and bump the Jammer from the microphone. 

Adds a notification as a reminder for running while in background .

Responds (stop and restart jammer) to telephony audio focus LOSS_TRANSIENT and GAIN.

Handle music player audio focus gain.

   vers. 1.1.02
   - min API 18 (4.3)
   - target API 23 (6.x)
   - compiled API 26 (8.x)

   testing devices
   - EMU : Galaxy Nexus API 18 (Android Studio AVD, no GApps)
   - EMU : Nexus 5X API 24 (Android Studio AVD, GApps)
   - LOW : s4 I9195 (deprecated) 4.3.1 (18)(CyanogenMod 10.2, F-Droid)
   - SLO : Mts 5045D (tainted) 6.0.1 (23) (CyanogenMod 13.0, GApps)
   - DEV : s5 G900I (tainted) 7.1.2 (25)(LineageOS 14.1, GApps)
 
 TODO:
 - full and proper testing ( incl. VOIP ? )
 - active jamming

# 2018 Kaputnik Go


Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

   http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.