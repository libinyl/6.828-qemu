## 环境初始化 ( for MacOS)

1. 克隆此代码库
   
    ```
    git clone https://github.com/libinyl/6.828-qemu qemu
    ```

2. 安装命令行工具：
   
    ```
    xcode-select --install
    ```

3. 安装 qemu 依赖库

    ```
    brew install $(brew deps qemu)
    ```


4. 配置编译选项

    ```
    ./configure --disable-kvm --disable-werror --disable-sdl --target-list="i386-softmmu x86_64-softmmu"
    ```

5. 编译并安装
   
   ```
   PATH=${PATH}:/usr/local/opt/gettext/bin make install
   ```
