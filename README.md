# 二维码工具箱（com.example.qrtool）

纯本地工具：生成二维码、相机扫码、从图片识别二维码。不上传任何内容。

- minSdk 24 / targetSdk 34
- 依赖：ZXing core 3.5.3（见 libs/zxing-core.jar，编译时随 dex 打进 APK）
- 签名：secrets/qrtool-release.keystore（别名 qrtoolrelease）
- 在线更新：dist/update.json（单文件自包含签名，RSA-SHA256）

## 构建
```bash
./build.sh   # 产物 build/app-debug.apk（release 密钥已签）
```

## 发布
```bash
python3 publish/publish_ota.py 1.0.1 "更新说明\n第二行"
```
