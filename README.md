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

> [!WARNING]

> Có thể khi chạy nhưng lệnh dưới sẽ lỗi, do máy tính tao cài nhiều môi trường Command line interface cho nhiều thứ bruh nên đề phòng nếu lỗi sẽ tính tiếp, bậy giờ thì cài vậy

# Cài Git bash

# Thiết lập llama.cpp

```bash
https://github.com/ggml-org/llama.cpp.git
```

```bash
cd llama.cpp
```

```bash
mkdir build
```

```bash
cd build
```

```bash
cmake .. -G "MinGW Makefiles" -DCURL_INCLUDE_DIR=C:/nguyenduytung/curl-8.13.0_4-win64a-mingw/include -DCURL_LIBRARY=C:/nguyenduytung/curl-8.13.0_4-win64a-mingw/lib/libcurl.dll.a
```

```bash
mingw32-make
```

```bash
cd bin
```

```bash
llama-server -hf ngxson/Vintern-1B-v3_5-GGUF --chat-template vicuna
```

- Chờ nó chạy hiện ra url localhost r mở index.html rồi chèn url vào