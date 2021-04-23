# cpp-opencv-cmake-superbuild
Automatically download, build and use OpenCV with OpenCV contrib for C++ application using CMake

# How to use
clone the repo in your desired folder ex: cvdemo
> git clone https://github.com/BBO-repo/cpp-opencv-cmake-superbuild.git cvdemo</br>
> cd cvdemo

run the cmake configuration to generate makefiles in the folder cvdemo/build 
> cmake -S . -B build

run cmake to build your app
> cmake --build build --target all

That's it you're done! You can enjoy developing OpenCV wonderful stuffs<br/><br/>
Notes: Downloading opencv and opencv-contrib may take some time.. fortunately you only do it once</br>
Comments: You could also using previous cmake commands
> mkdir build<br/>
> cd build<br/>
> cmake ..<br/>
> make

P.S: Building opencv may take some time .. you could increase number of threads
> cmake --build build --target all -j12

Or if using the previous cmake commands</br>
> ...</br>
> make -j12

P.P.S: You may want to udpate OPENCV_LIBS with your additionnal required linked libs and as opencv build as dynamic library make sure te LD_LIBRARY_PATH is updated while running your exectable in the bin/ folder 

