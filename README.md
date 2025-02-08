# LabelML
Software specifically for object annotation for macOS’s CreateML

# Object Detection on iOS/MacOS with Create ML

Recently, I’ve been working on implementing object detection functionality on iOS, specifically to train a model for fuel dispenser information extraction. Since it’s an iOS project, my first choice was to use **Create ML**, which is built into macOS, to train the model. However, after looking at several mainstream data annotation tools, I found that most don’t directly support Create ML. After refining my search keywords multiple times, I discovered the native macOS app [LabelML](https://apps.apple.com/cn/app/labelml/id6478145989?mt=12), which directly supports Create ML training datasets.

---

### Conclusion First:  
The functionality is not complicated, and the app has native interaction with fast speed. If it's just for simple object annotation, I would highly recommend it—it’s practically ready to use out of the box.

### Main Features:
* Once you open the app, you can directly select a folder—no extra pages.
* Interaction is convenient (similar to Photoshop interaction):
  * Scroll the mouse = Zoom in and out of the image.
  * Hold the spacebar = Drag the image with the mouse.
  * Command + S to save anytime (native interaction).
  * Command + Z to undo actions (native interaction).

Since the functionality is relatively simple, here are some screenshots of the usage:

1. **Click the menu to activate folder selection, ensuring that the folder contains images:**

   ![image.png](https://upload-images.jianshu.io/upload_images/695270-a289d5b475215243.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

2. **Annotation:**

   ![image.png](https://upload-images.jianshu.io/upload_images/695270-0dd14766d536e341.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)  
   ![image.png](https://upload-images.jianshu.io/upload_images/695270-d94edaaf9cba69b7.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)  
   ![image.png](https://upload-images.jianshu.io/upload_images/695270-6f52f3772688f6d8.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

3. **Create a new ObjectDetector in CreateML:**

   ![image.png](https://upload-images.jianshu.io/upload_images/695270-2266eb79cdc36e01.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

4. **Choose the folder that you just annotated in the TrainingData:**

   ![image.png](https://upload-images.jianshu.io/upload_images/695270-1533218fcc84f322.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

5. **Click the 'Train' button in the top menu to start training:**

   ![image.png](https://upload-images.jianshu.io/upload_images/695270-652b497c80bdee95.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

   ![image.png](https://upload-images.jianshu.io/upload_images/695270-f36839db365c1ab0.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

6. **Once training is complete, drag the trained model into your iOS project for integration.**
