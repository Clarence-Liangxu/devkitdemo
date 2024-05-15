# **kaezip & gzip demo**

English | [简体中文](README.md)

## Introduction
1. [KAEzip](https://www.hikunpeng.com/document/detail/en/kunpengaccel/compress/devg-kaezip/kunpengaccel_kaezip_0001.html) is the compression module of the Kunpeng Accelerator Engine (KAE). It uses the Kunpeng hardware acceleration module to implement the deflate algorithm and works with the lossless user-mode driver framework to provide an interface for high-performance compression in gzip or zlib format.
## KAEzip demo dependency
1. Ensure **KAEdriver** has been installed;
2. Ensure **KAEzip** has been installed;

[Download KAEdriver](https://gitee.com/kunpengcompute/KAE/tree/kae1/)
[Download KAEzip](https://gitee.com/kunpengcompute/KAE/tree/kae1/)
[Reference](https://www.hikunpeng.com/document/detail/en/kunpengaccel/compress/devg-kaezip/kunpengaccel_kaezip_0005.html)

2. Or install **kunpeng-gpc** and **kunpeng-gpc-devle** SDK

## Guidance
1. Obtain the code.

   ```shell
   git clone https://github.com/kunpengcompute/devkitdemo.git
   ```

2. Switch to the project root path.

   ```shell
   cd ./devkitdemo/Development_framework/gpc-sdk/examples/kaezip/
   ```

3. Compile the KAEzip demo.

   ```shell
   mkdir build
   cd build
   cmake ..
   make
   ```

4. Run KAEzip demo

   ```shell
   ./kaezip_demo -h // help
   ./kaezip_demo -czf filename.tar.gz filename // compress
   ./kaezip_demo -xzf filename.tar.gz // decompress
   ```

5. 清理demo

   ```shell
   cd ..
   rm -rf build
   ```
