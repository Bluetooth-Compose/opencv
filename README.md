## Bluetooth-Compose additional notes:

We built OpenCV for Android and iOS, as follows:

```cd ~/``` [Enter]

```pwd```  [Enter]

```/Users/developer```

```git clone https://github.com/Bluetooth-Compose/opencv.git```  [Enter] i.e. opencv repo

```git clone https://github.com/Bluetooth-Compose/opencv_contrib.git```  [Enter] i.e. opencv_contrib repo

we also ensured that the following paths DID NOT exist:

- /Users/developer/android
- /Users/developer/ios

we then ran the following two commands:

- ```python opencv/platforms/ios/build_framework.py ios --contrib ./opencv_contrib```
- ```python opencv/platforms/android/build_sdk.py android opencv  --extra_modules_path ./opencv_contrib/modules --sdk_path /Users/developer/Library/Android/sdk --ndk_path /Users/developer/Library/Android/sdk/ndk/24.0.8215888```

The rest of this ReadMe is the original fiorked ReadMe

## OpenCV: Open Source Computer Vision Library

### Resources

* Homepage: <https://opencv.org>
  * Courses: <https://opencv.org/courses>
* Docs: <https://docs.opencv.org/4.x/>
* Q&A forum: <https://forum.opencv.org>
  * previous forum (read only): <http://answers.opencv.org>
* Issue tracking: <https://github.com/opencv/opencv/issues>
* Additional OpenCV functionality: <https://github.com/opencv/opencv_contrib> 


### Contributing

Please read the [contribution guidelines](https://github.com/opencv/opencv/wiki/How_to_contribute) before starting work on a pull request.

#### Summary of the guidelines:

* One pull request per issue;
* Choose the right base branch;
* Include tests and documentation;
* Clean up "oops" commits before submitting;
* Follow the [coding style guide](https://github.com/opencv/opencv/wiki/Coding_Style_Guide).
