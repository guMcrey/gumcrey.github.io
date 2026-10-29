# 游戏隐私政策网站

本仓库通过 GitHub Pages 发布静态 HTML，无需构建依赖。

## Tiro Total

- 游戏：**Tiro Total**，Android 包名 `com.tirototal.app`。
- 开发者：**gumeracy**，联系邮箱 `gumeracy@gmail.com`。
- 目标玩家：**13 岁及以上**。
- 巴西葡语（默认）：`tiro-total/privacy/index.html`。
- 英语：`tiro-total/privacy/en.html`。
- 最近修订：**2026-10-29**。

发布后可在 Google Play 的隐私政策字段填写：

```text
https://gumcrey.github.io/tiro-total/privacy/
```

英语版地址：

```text
https://gumcrey.github.io/tiro-total/privacy/en.html
```

新增文件必须进入 GitHub Pages 的实际发布来源才会在线生效。在仓库 Settings → Pages 确认当前发布分支和目录，提交并推送文件到对应来源；等 Pages 部署完成后，检查两个地址均可在未登录状态下打开。以上地址是发布目标，创建本地文件本身不会让它们上线。

页面复用根目录的 `policy.css`。原有 Photo Luck / Pomar Zen 条款位于 `index.html` 和 `en.html`，仅在页脚增加 Tiro Total 政策入口。根目录 `app-ads.txt` 保持原路径。

本地预览：

```sh
python3 -m http.server 8765 --bind 127.0.0.1
```

随后访问 `http://127.0.0.1:8765/tiro-total/privacy/`。

## 广告声明与实际版本

已核对 Tiro Total 当前 Android 源码和版本代码 2 的合并清单：没有原生广告 SDK、独立分析 SDK 或广告 ID 权限。进度、奖励、道具和偏好由游戏本地保存；Android 配置允许系统备份。

按用户要求参考现有 Pomar Zen 政策，两种语言已采用正式的 AdMob 广告声明，不再以「未来广告」或「尚未接入」作为网页内容。声明涵盖数据类别、处理目的、广告形式、激励奖励条件、个性化与非个性化广告、UMP 隐私选择、第三方链接、国际处理、保留与删除、数据主体权利和未成年人保护。广告内容明确适用于提供广告的版本和功能，避免将声明写成某个无广告安装包的实际 SDK 状态。

这次修改的是政策文案，不等于接入广告 SDK、创建同意弹窗或更改 Play Console 的数据声明。

### 接入广告前的维护清单

1. 核对实际选择的 Google Mobile Ads SDK、UMP 和任何中介网络的最新数据披露。广告条款已提前包含 AdMob；如果实际服务、数据或功能与条款有差异，补充实际启用的提供商与广告形式，并同时更新两种语言和修订日期。
2. 按地区和年龄接入必要的同意流程，在依赖同意的处理之前取得有效同意；使用 UMP 的当前状态决定是否可以请求广告，并在要求时提供可重新打开的隐私选项入口。阅读隐私政策或点击游戏的通用「同意」不能代替广告同意。
3. 面向 13 岁以上仍可能包括未成年人。条款承诺不向已识别为未满 18 岁的用户请求个性化广告；实际广告配置、适用的年龄判断、监护人授权和当地数字同意年龄必须与此一致。UMP 的未达同意年龄标记与广告请求的年龄标记分别核对，不能只设置其中一个。
4. 同步核对 Play Console 的「包含广告」「广告 ID」「数据安全」「目标受众和内容」声明与当次安装包。未接入广告的当前版本按当前行为填写，不因政策预留未来广告就声明已经使用广告 ID。SDK 在非个性化广告下仍可能处理数据。
5. 在游戏内的适当位置提供此政策的可访问入口。当前游戏仍有测试版隐私文案，网站新增页面不会自动替换应用内文字；正式发布前需要移除旧测试文案，并连接正式政策。
6. 验证拒绝和撤回同意、未成年人限制、广告关闭或失败、奖励发放等行为与条款一致；若提供广告中介或其他收集服务，在启用前补充披露。

官方参考：

- [Google Play 用户数据政策](https://support.google.com/googleplay/android-developer/answer/10144311)
- [Google Mobile Ads SDK 数据披露](https://developers.google.com/admob/android/privacy/play-data-disclosure)
- [Google Mobile Ads 下一代 SDK 数据披露](https://developers.google.com/admob/android/next-gen/privacy/play-data-disclosure)
- [UMP 隐私选择](https://developers.google.com/admob/android/privacy)
- [广告请求及未达同意年龄设置](https://developers.google.com/admob/android/targeting)
- [GitHub Pages 及访问日志](https://docs.github.com/en/pages/getting-started-with-github-pages/what-is-github-pages)
- [Android 系统备份](https://developer.android.com/identity/data/autobackup)
