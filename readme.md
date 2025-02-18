# custom-msvc-buildtools-version

自定义使用指定版本的 MSVC BuildTools

详见 [patch](./patch) 目录

## 修改说明

核心是修改了 [vcvars.bat](./patch/BuildTools/Common7/Tools/vsdevcmd/ext/vcvars.bat?L723~L750) 文件，增加了对 `__VCVARS_CUSTOM_CONFIG_FILE_NAME` 环境变量的支持。