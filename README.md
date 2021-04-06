# buildopencv

## [How_to_setup_Qt_and_openCV_on_Windows](https://wiki.qt.io/How_to_setup_Qt_and_openCV_on_Windows)

### Cmake
```bash
cd C:\
cd C:\LIB\build_opencv 
cmake -DCMAKE_BUILD_TYPE=Release -DCMAKE_INSTALL_PREFIX=. -G "MinGW Makefiles" -DOPENCV_ENABLE_ALLOCATOR_STATS:BOOL="0" -DWITH_QT:BOOL="1" -DWITH_OPENGL:BOOL="1" -D PYTHON_DEFAULT_EXECUTABLE=C:\Python38\python.exe ../opencv-4.5.0
```

<details><summary>cmake Configuration</summary> 

* MinGW-x64-810
* Windows-10-64bit
* CMake-3.19.2

```
General configuration for OpenCV 4.5.0 =====================================
  Version control:               unknown

  Platform:
    Timestamp:                   2021-04-05T16:35:08Z
    Host:                        Windows 10.0.19042 AMD64
    CMake:                       3.19.2
    CMake generator:             MinGW Makefiles
    CMake build tool:            C:/Qt/Tools/mingw810_64/bin/mingw32-make.exe
    Configuration:               Release

  CPU/HW features:
    Baseline:                    SSE SSE2 SSE3
      requested:                 SSE3
    Dispatched code generation:  SSE4_1 SSE4_2 FP16 AVX AVX2
      requested:                 SSE4_1 SSE4_2 AVX FP16 AVX2 AVX512_SKX
      SSE4_1 (17 files):         + SSSE3 SSE4_1
      SSE4_2 (2 files):          + SSSE3 SSE4_1 POPCNT SSE4_2
      FP16 (1 files):            + SSSE3 SSE4_1 POPCNT SSE4_2 FP16 AVX
      AVX (5 files):             + SSSE3 SSE4_1 POPCNT SSE4_2 AVX
      AVX2 (31 files):           + SSSE3 SSE4_1 POPCNT SSE4_2 FP16 FMA3 AVX AVX2

  C/C++:
    Built as dynamic libs?:      YES
    C++ standard:                11
    C++ Compiler:                C:/Qt/Tools/mingw810_64/bin/g++.exe  (ver 8.1.0)
    C++ flags (Release):         -fsigned-char -W -Wall -Werror=return-type -Werror=non-virtual-dtor -Werror=address -Werror=sequence-point -Wformat -Werror=format-security -Wmissing-declarations -Wundef -Winit-self -Wpointer-arith -Wshadow -Wsign-promo -Wuninitialized -Winit-self -Wsuggest-override -Wno-delete-non-virtual-dtor -Wno-comment -Wimplicit-fallthrough=3 -Wno-strict-overflow -fdiagnostics-show-option -Wno-long-long -fomit-frame-pointer -ffunction-sections -fdata-sections  -msse -msse2 -msse3 -fvisibility=hidden -fvisibility-inlines-hidden -O3 -DNDEBUG  -DNDEBUG
    C++ flags (Debug):           -fsigned-char -W -Wall -Werror=return-type -Werror=non-virtual-dtor -Werror=address -Werror=sequence-point -Wformat -Werror=format-security -Wmissing-declarations -Wundef -Winit-self -Wpointer-arith -Wshadow -Wsign-promo -Wuninitialized -Winit-self -Wsuggest-override -Wno-delete-non-virtual-dtor -Wno-comment -Wimplicit-fallthrough=3 -Wno-strict-overflow -fdiagnostics-show-option -Wno-long-long -fomit-frame-pointer -ffunction-sections -fdata-sections  -msse -msse2 -msse3 -fvisibility=hidden -fvisibility-inlines-hidden -g  -O0 -DDEBUG -D_DEBUG
    C Compiler:                  C:/Qt/Tools/mingw810_64/bin/gcc.exe
    C flags (Release):           -fsigned-char -W -Wall -Werror=return-type -Werror=non-virtual-dtor -Werror=address -Werror=sequence-point -Wformat -Werror=format-security -Wmissing-declarations -Wmissing-prototypes -Wstrict-prototypes -Wundef -Winit-self -Wpointer-arith -Wshadow -Wuninitialized -Winit-self -Wno-comment -Wimplicit-fallthrough=3 -Wno-strict-overflow -fdiagnostics-show-option -Wno-long-long -fomit-frame-pointer -ffunction-sections -fdata-sections  -msse -msse2 -msse3 -fvisibility=hidden -O3 -DNDEBUG  -DNDEBUG
    C flags (Debug):             -fsigned-char -W -Wall -Werror=return-type -Werror=non-virtual-dtor -Werror=address -Werror=sequence-point -Wformat -Werror=format-security -Wmissing-declarations -Wmissing-prototypes -Wstrict-prototypes -Wundef -Winit-self -Wpointer-arith -Wshadow -Wuninitialized -Winit-self -Wno-comment -Wimplicit-fallthrough=3 -Wno-strict-overflow -fdiagnostics-show-option -Wno-long-long -fomit-frame-pointer -ffunction-sections -fdata-sections  -msse -msse2 -msse3 -fvisibility=hidden -g  -O0 -DDEBUG -D_DEBUG
    Linker flags (Release):      -Wl,--gc-sections  
    Linker flags (Debug):        -Wl,--gc-sections  
    ccache:                      NO
    Precompiled headers:         NO
    Extra dependencies:          opengl32 glu32
    3rdparty dependencies:

  OpenCV modules:
    To be built:                 calib3d core dnn features2d flann gapi highgui imgcodecs imgproc ml objdetect photo stitching ts video videoio
    Disabled:                    world
    Disabled by dependency:      -
    Unavailable:                 java js python2 python3
    Applications:                tests perf_tests apps
    Documentation:               NO
    Non-free algorithms:         NO

  Windows RT support:            NO

  GUI: 
    QT:                          YES (ver 5.15.2)
      QT OpenGL support:         YES (Qt5::OpenGL 5.15.2)
    Win32 UI:                    YES
    OpenGL support:              YES (opengl32 glu32)
    VTK support:                 NO

  Media I/O: 
    ZLib:                        build (ver 1.2.11)
    JPEG:                        build-libjpeg-turbo (ver 2.0.5-62)
    WEBP:                        build (ver encoder: 0x020f)
    PNG:                         build (ver 1.6.37)
    TIFF:                        build (ver 42 - 4.0.10)
    JPEG 2000:                   build (ver 2.3.1)
    OpenEXR:                     build (ver 2.3.0)
    HDR:                         YES
    SUNRASTER:                   YES
    PXM:                         YES
    PFM:                         YES

  Video I/O:
    DC1394:                      NO
    FFMPEG:                      YES (prebuilt binaries)
      avcodec:                   YES (58.91.100)
      avformat:                  YES (58.45.100)
      avutil:                    YES (56.51.100)
      swscale:                   YES (5.7.100)
      avresample:                YES (4.0.0)
    GStreamer:                   YES (1.18.4)
    DirectShow:                  YES

  Parallel framework:            none

  Trace:                         YES (built-in)

  Other third-party libraries:
    Lapack:                      NO
    Eigen:                       NO
    Custom HAL:                  NO
    Protobuf:                    build (3.5.1)

  OpenCL:                        YES (no extra features)
    Include path:                C:/LIB/opencv-4.5.0/3rdparty/include/opencl/1.2
    Link libraries:              Dynamic load

  Python (for build):            C:/Python38/python.exe

  Java:                          
    ant:                         NO
    JNI:                         C:/Program Files/AdoptOpenJDK/jdk-11.0.10.9-hotspot/include C:/Program Files/AdoptOpenJDK/jdk-11.0.10.9-hotspot/include/win32 C:/Program Files/AdoptOpenJDK/jdk-11.0.10.9-hotspot/include
    Java wrappers:               NO
    Java tests:                  NO

  Install to:                    C:/LIB/build_opencv/install
-----------------------------------------------------------------
```
</details>

### Build
```bash
mingw32-make -j 8
mingw32-make install
```

### Test(small special modification)
```pro
# more correct variant, how set includepath and libs for mingw
# add system variable: OPENCV_SDK_DIR=C:/LIB/build_opencv/install
# read http://doc.qt.io/qt-5/qmake-variable-reference.html#libs

INCLUDEPATH += $$(OPENCV_SDK_DIR)/include
LIBS += -L$$(OPENCV_SDK_DIR)/x64/mingw/lib \
        -lopencv_core450        \
        -lopencv_highgui450     \
        -lopencv_imgcodecs450   \
        -lopencv_imgproc450     \
        -lopencv_features2d450  \
        -lopencv_calib3d450
```

```pro
cv::Mat image = cv::imread("C:/Users/61240/Pictures/logo_blue.png", 1);
```
### pkg-config
```bash
$ cat C:/Qt/5.15.2/mingw81_64/lib/pkgconfig/opencv.pc
# Package Information for pkg-config
prefix=C:/LIB/build_opencv/install
exec_prefix=${prefix}/x64/mingw/bin

libdir=C:/LIB/build_opencv/install/x64/mingw/lib
includedir=C:/LIB/build_opencv/install/include

Name: OpenCV
Description: Open Source Computer Vision Library
Version: 4.5.0
Libs: -LC:/LIB/build_opencv/install/x64/mingw/lib -lopencv_gapi450 -lopencv_stitching450 -lopencv_dnn450 -lopencv_photo450 -lopencv_objdetect450 -lopencv_ml450 -lopencv_video450 -lopencv_calib3d450 -lopencv_features2d450 -lopencv_highgui450 -lopencv_videoio450 -lopencv_imgcodecs450 -lopencv_imgproc450 -lopencv_flann450 -lopencv_core450
Libs.private: -ldl -lm -lpthread -lrt
Cflags: -I${includedir}

$ export PKG_CONFIG_PATH="C:/Qt/5.15.2/mingw81_64/lib/pkgconfig"
$ pkg-config --modversion opencv
4.5.0
```

```pro
CONFIG += link_pkgconfig
PKGCONFIG += opencv
#INCLUDEPATH += $$(OPENCV_SDK_DIR)/include
#LIBS += -L$$(OPENCV_SDK_DIR)/x64/mingw/lib \
#        -lopencv_core450        \
#        -lopencv_highgui450     \
#        -lopencv_imgcodecs450   \
#        -lopencv_imgproc450     \
#        -lopencv_features2d450  \
#        -lopencv_calib3d450
```

