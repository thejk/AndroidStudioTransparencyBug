Example project for Android Studio bug converting PNG images to lossless WEBP and removing transparency

Reproduction steps:
1. Check out this project.
2. Open project in Android Studio.
3. Start tool for converting images to webp.
   (right-click on res directory and select "Convert to WebP...")
4. Select lossless encoding.
   Make sure "Skip images with transparency/alpha channel" is NOT checked.
   Select all suggested images.

Expected result:  
All images continue to look exactly the same and some/all are converted
to webp.

Actual result:  
These are converted to web without transparency:  
drawable-xxxhdpi/ic_pause_white_36dp.webp  
drawable-xxxhdpi/ic_stop_white_36dp.webp  
drawable-xxhdpi/ic_stop_white_36dp.webp  
drawable-xhdpi/ic_pause_white_36dp.webp  
drawable-xhdpi/ic_stop_white_36dp.webp  
drawable-mdpi/ic_stop_white_36dp.webp  

These are converted to web correctly:  
drawable-hdpi/ic_pause_white_36dp.webp  
drawable-hdpi/ic_stop_white_36dp.webp  
drawable-mdpi/ic_pause_white_36dp.webp  
drawable-xxdpi/ic_pause_white_36dp.webp  
