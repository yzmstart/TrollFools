# TrollFools 3.3-34 去广告改动

修改文件：`TrollFools/AppListView.swift`

1. 移除首页 `advertisementSection` 的插入与视图定义，广告卡片及“广告”标题不再显示。
2. 移除 `isAdvertisementHidden` 与 `shouldShowAdvertisement` 状态和判断。
3. 移除每次首页出现时 10% 概率重新启用广告的代码。
4. 移除相关动画依赖。其他页面、App 模型、注入功能、构建设置均未修改。

编译：使用仓库 `.github/workflows/compile.yml` 或 `.github/workflows/release.yml`，必要时在 GitHub Actions 中给 Release 工作流 `contents: write` 权限。

验证：源码差异及 ZIP 校验通过；未在 macOS/Xcode 上编译或在手机上安装测试。
