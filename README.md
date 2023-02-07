This repository contains single include version of [uni-algo library](https://github.com/uni-algo/uni-algo).

Just drop `uni_algo.h` file into your project and include it.

Note that system locale facilities: uni::locale::system() function etc. are disabled in the single include version for now.

Be aware that it is not recommended to use the single include version in production because the file is big and compiles slowly.
