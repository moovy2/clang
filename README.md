# PowerTech Clang
>We care about Developers, so we create Simple, Powerful and Convenient tools for them. This Compiler fork is intended for C/C++ Developers. We believe that the most functional, modern and promising compiler today is Clang (LLVM project), so we built our tools relative to the Clang/LLVM infrastructure.

*Please note that the compiler is under active development, we will update this article as new functionality becomes available. We will be glad for your participation in the development, testing and voicing of proposals. Feel free in [Issues](https://github.com/powertech-center/clang/issues), [Discussions](https://github.com/powertech-center/clang/discussions) or in the telegram group [PowerTech C/C++ Beta](https://t.me/powercpp_beta).*

### Installation
Now you can freely download the **Beta** version of the compiler, unpack the archive corresponding to your operating system and use it. Using our scripts you can easily change the `PATH` environment variable or create the necessary symlinks, more details in the [Portable Installation](/docs/portable-installation.md) page.
* Windows x64: [powerclang-windows-x64.7z](https://powertech.center/data/clang/beta/powerclang-windows-x64.7z)
* Linux x64: [powerclang-linux-x64.7z](https://powertech.center/data/clang/beta/powerclang-linux-x64.7z)
* Linux ARM64: [powerclang-linux-arm64.7z](https://powertech.center/data/clang/beta/powerclang-linux-arm64.7z)
* macOS x64: [powerclang-macos-x64.7z](https://powertech.center/data/clang/beta/powerclang-macos-x64.7z)
* macOS ARM64: [powerclang-macos-arm64.7z](https://powertech.center/data/clang/beta/powerclang-macos-arm64.7z)

### Features
* [[C] Language Extensions](/docs/features/language-extensions.md)
* [[C] VSCode Integration](/docs/features/vscode-integration.md)
* [[C] Cross Compilation](/docs/features/cross-compilation.md)
* [[P] Build Speed Boost](/docs/features/build-speed-boost.md)

### Notes
* Unlike canonical Clang where the default linker is `ld`, in our fork the default linker is `lld`. This approach is motivated by the fact that developers in the iterative build process spend a lot of time on linking, which `lld` performs faster, especially with our optimizations. You can change the linker in the standard way, for example `-fuse-ld=ld`.

### IDE
Our fork can be freely used in all IDEs that work with standard Clang, such as CLion, Eclipse or VSCode. But we recommend using our Extensions for VSCode: [PowerTech C/C++](https://marketplace.visualstudio.com/items?itemName=PowerTech.powercpp) and [PowerTech Themes](https://marketplace.visualstudio.com/items?itemName=PowerTech.powerthemes). It's fast, free and convenient! In the extension settings, you can explicitly specify the path to the compiler.

![](https://github.com/powertech-center/vscode-cpp/raw/master/images/settings_path.png)
![](https://github.com/powertech-center/vscode-cpp/raw/master/images/quick-start.gif)
![](https://github.com/powertech-center/vscode-themes/raw/master/images/overview.png)