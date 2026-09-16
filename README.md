# phone-monitor-release

通话录音监控 App（包名 `com.phone.monitor`）的测试安装包发布仓库。

## 下载

最新版直链（点开即下载）：

```
https://github.com/taoliu-double/phone-monitor-release/releases/latest/download/phone-monitor-2.2.0.apk
```

| 版本 | 说明 | 大小 |
|------|------|------|
| 2.2.0 (220) | 测试版，debug 签名 | 11480331 字节 |

## 注意事项

- 这是 **debug 构建**，APK 内含编译期注入的 `APP_SECRET` 常量，属于内部测试包，请勿公开分发。
- 安装后首次运行需要：关闭本应用电池优化、允许精确闹钟、授予电话/通讯录/存储/录音权限。
- 微信消息同步功能依赖 Root（Magisk + Shamiko + DenyList），详见项目文档。