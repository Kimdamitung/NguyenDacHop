# Cài môi trường cần thiết

- [MinGW](https://github.com/niXman/mingw-builds-binaries/releases)

> Chọn x65 hoặc x86_64

> PATH môi trường lun nha

- [CMake](https://cmake.org/download/)

- [Make GNU](https://sourceforge.net/projects/gnuwin32/files/make/3.81/make-3.81.exe/download?use_mirror=onboardcloud&download=)

> PATH môi trường lun nha

- [Curl](https://curl.se/windows/)

> Chọn x65 hoặc x86_64

> PATH môi trường lun nha

# Cài Git bash

# Thiết lập llama.cpp

> https://github.com/ggml-org/llama.cpp.git

> cd llama.cpp

> mkdir build

> cd build

> cmake .. -G "MinGW Makefiles" -DCURL_INCLUDE_DIR=C:/nguyenduytung/curl-8.13.0_4-win64a-mingw/include -DCURL_LIBRARY=C:/nguyenduytung/curl-8.13.0_4-win64a-mingw/lib/libcurl.dll.a

> mingw32-make

> cd bin

> llama-server -hf ngxson/Vintern-1B-v3_5-GGUF --chat-template vicuna

- Chờ nó chạy hiện ra url localhost r mở index.html rồi chèn url vào