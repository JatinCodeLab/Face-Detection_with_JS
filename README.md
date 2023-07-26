IMPORTANT: Bug Fixes
Deprecation of navigator.getUserMedia
In order to resolve the issue, it is essential to update all instances of navigator.getUserMedia to the new navigator.mediaDevices.getUserMedia method. This update is crucial as navigator.getUserMedia has been deprecated. Please make sure to modify all occurrences of the deprecated method to the new one, navigator.mediaDevices.getUserMedia.

Low-end Devices Issue
On low-end machines, the play event listener triggers prematurely, before the video is fully loaded. This premature firing causes errors to emerge from the Face API, resulting in script termination. To tackle this problem, replace the play event with the playing event, which is activated when the media has enough data to begin playing. Implementing this change will mitigate the errors and ensure smoother performance, especially on low-end devices.

Code Lab Jatin Organization https://github.com/JatinCodeLab
Copyright © Jatin009V
