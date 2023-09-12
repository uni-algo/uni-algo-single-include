This repository contains single include version of [uni-algo library](https://github.com/uni-algo/uni-algo).

Just drop `uni_algo.h` or `uni_algo_ext.h` file into your project and include it.

The file `uni_algo_ext.h` contains extensions (files from `include/uni_algo/ext` directory in the main repository) file `uni_algo.h` does not.
You need to use only one of them not both.

Be aware that it is not recommended to use the single include version in production and include it to more than one `.cpp` file because the file is big and compiles slowly.

Current limitations of the single include version:
- System locale facilities: uni::locale::system() function etc. are disabled in this version for now
- Config defines that start with `UNI_ALGO_ENABLE/DISABLE` except `UNI_ALGO_ENABLE_SAFE_LAYER` will break compilation i.e. must not be used
- The single include version is less tested
