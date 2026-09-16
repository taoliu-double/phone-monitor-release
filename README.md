# phone-monitor-release

通话录音监控 App（包名 `com.phone.monitor`）的测试安装包发布仓库。

## 下载

**国内加速地址（推荐，实测约 4 MB/s）**

```
https://gh-proxy.com/https://github.com/taoliu-double/phone-monitor-release/releases/latest/download/phone-monitor-2.2.0.apk
```

**GitHub 直连**

```
https://github.com/taoliu-double/phone-monitor-release/releases/latest/download/phone-monitor-2.2.0.apk
```

> 直连在部分国内网络下只有几 KB/s，建议用上面的加速地址。加速镜像只是反向代理，文件与原站逐字节一致（已比对 SHA256）。

| 版本 | 说明 | 大小 | SHA256 |
|------|------|------|--------|
| 2.2.0 (220) | 测试版，debug 签名 | 11480331 字节 | `d92356674977a6563cb179a3650225243824eb8617ad16446e480f5001f8608a` |

## 首次运行必须配置

1. 关闭本应用的电池优化（设置 → 电池 → 应用耗电管理 → 不优化）
2. 允许精确闹钟权限（App 会弹 SnackBar 引导）
3. 授予电话、通讯录、存储、录音权限
4. 微信消息同步功能依赖 Root（Magisk + Shamiko + DenyList），详见项目文档

## 注意事项

- 这是 **debug 构建**：使用公开的 debug keystore 签名，且 `android:debuggable=true`，仅供内部测试。
- APK 内含编译期注入的 `APP_SECRET` 常量，用 `strings` 即可提取。本仓库已设为 public，**该密钥应视为已公开**；若后续要长期对外分发，建议轮换密钥并改用正式签名构建。