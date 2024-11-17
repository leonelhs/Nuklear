# Nuklear Android demos

## Building for SDL beginners

This folder contains two **Nuklear** implementations for **Android** based on JNI/C and SDL2.

The **SDL2** source code is required in order to build the demos. You can get a copy at <https://github.com/libsdl-org/SDL>. Clone it wherever you want and check out the latest SDL2 release tag, currently `release-2.30.9`.

The build script (`build.sh`) requires the environment variables `SDLPATH`, `ANDROID_HOME` and `ANDROID_NDK_HOME` to be set.

### Implemenations

### sdl\_opengl2

This folder contains all the dependencies for building a project based on **OpenGL ES2**. To build the demo just execute `./build.sh`. If everything goes ok, you will see your demo in `build/com.demogles2.nuklear/`.

### sdl2surface\_rawfb

This folder contains all the dependencies for building a project based on **Raw SDL Surface**. OpenGL context will not be accessible inside this project. Anyways under the hood SDL works with OpenGL. Just like the previous demo you will find the project build result in `build/com.sdl2rawfb.nuklear/`.

## Building for SDL experts

If you already are familiar with SDL, you can create your own build script based on SDL's original [androidbuild.sh](https://github.com/libsdl-org/SDL/blob/release-2.30.9/build-scripts/androidbuild.sh).
