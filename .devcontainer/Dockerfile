FROM mcr.microsoft.com/devcontainers/base:bullseye
RUN apt-get update \
    && export DEBIAN_FRONTEND=noninteractive \
    && apt-get -y install build-essential \
                            scons \
                            pkg-config \
                            libx11-dev \
                            libxcursor-dev \
                            libxinerama-dev \
                            libgl1-mesa-dev \
                            libglu-dev \
                            libasound2-dev \
                            libpulse-dev \
                            libudev-dev \
                            libxi-dev \
                            libxrandr-dev \
                            yasm \
                            mingw-w64
RUN update-alternatives --set x86_64-w64-mingw32-gcc /usr/bin/x86_64-w64-mingw32-gcc-posix
RUN update-alternatives --set x86_64-w64-mingw32-g++ /usr/bin/x86_64-w64-mingw32-g++-posix