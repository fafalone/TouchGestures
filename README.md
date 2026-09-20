# TouchGestures
Using touchscreen gestures to manipulate images


<img width="564" height="591" alt="TouchGest" src="https://github.com/user-attachments/assets/d16504a6-b0ea-4f74-8476-a7b86a69e7f4" />

This project shows how to implement touchscreen gesture handling in order to manipulate an image that is rendered by Direct2D.\
It supports Pinch-to-zoom, Rotate, Pan (with two fingers), and 2-finger taps.

There's two versions:

TouchGesturesEffects.twinproj - Uses `WM_GESTURE`/`GetGestureInfo` to process gestures. Less advanced but suitable for Windows 7.

TouchGesturesManip.twinproj - Uses `WM_POINTERUP/UPDATE/DOWN` and the system `ManipulationProcessor` class to process gestures. Offers a lot more advanced features (though only pinch-to-zoom/rotate/pan are implemented), as-is though requires Win8+. 

**Requires Windows Development Library for twinBASIC v9.4.730+** - Updated specifically for this project. References->Available packages. If you uncheck 'Embed', it will be available to all projects that link to it.

**Update - TouchGesturesManip v2.1:** Added InertiaProcessor class so you can now flick the image and it will slowly decelerate and bounce off the sides.

<img width="745" height="604" alt="TouchGest2" src="https://github.com/user-attachments/assets/b73f776b-d3f9-4324-82e9-8683d52937f5" />

**Update - TouchGesturesManip v1.1:** Added two-finger tap functionality like the other project. Also of interest, this shows how to track the number of touch points for advanced multitouch features.
