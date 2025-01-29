![Banner](https://github.com/SketchNow/SketchNow.WPF/blob/main/docs/banner.png)

# SketchNow

[![issues](https://img.shields.io/github/issues/SketchNow/SketchNow.WPF.svg)](https://github.com/SketchNow/SktechNow.WPF/issues)

一款让您能在屏幕任意位置实时绘图的应用程序

> [!caution]
> 当前仍在开发阶段。为避免潜在风险，请勿在生产环境中安装

### 特点

- 屏幕任意位置实时绘图
- 高性能与精心设计的UI/UX
- 稳定可靠
- 绝不共享您的数据
- 支持压感设备
- 系统资源占用低

### 即将到来

在[这里](https://github.com/orgs/SketchNow/projects)查看项目规划

### 安装

前往[Releases](https://github.com/SketchNow/SketchNow.WPF/releases)，选择所需版本。

若想体验最新提交的代码，
可访问[Actions](https://github.com/SketchNow/SketchNow.WPF/actions)，
下载所有`artifacts`中的`app`文件

### 隐私
| 权限类型    | 详细说明                                                                                                |
|------------|-------------------------------------------------------------------------------------------------------|
| 数据存储   | 安装版路径 `%LocalAppData%\SketchNow` <br/> 便携版路径 主程序所在目录                                  |
| 网络访问   | **访问** `github.com` 用于获取版本信息以下载和更新应用程序                                              |

### 贡献
1. 遵守`.editorconfig`规范
2. 使用`Xaml Styler`格式化xaml文件（配置文件位于[Settings.XamlStyler](https://github.com/SketchNow/SketchNow.WPF/blob/main/Settings.XamlStyler)）
3. 遵循[Conventional Commits](https://www.conventionalcommits.org/zh-hans/v1.0.0/)
4. 遵循[Semantic Versioning](https://semver.org/lang/zh-CN/)
### 构建
- Windows 10 或更高版本
- Visual Studio 2022/JetBrains Rider
- 安装.NET桌面开发工作负载（需`.NET 9`）
### 发布
我们使用[Velopack](https://github.com/velopack/velopack)生成发布包

执行以下命令前，
请确认已阅读[官方文档](https://docs.velopack.io/getting-started/csharp)
```shell
dotnet publish -c Release --self-contained -r win-x64 -o .\publish
```
```shell
vpk pack -u SketchNow -v 1.0.0 -p .\publish -e SketchNow.exe
```
### 测试
- Moq.AutoMocker
### 致谢
- [DotnetTemplates](https://github.com/Keboo/DotnetTemplates)
- [wpf](https://github.com/dotnet/wpf)
- [CommunityToolkit MVVM](https://github.com/CommunityToolkit/dotnet)
- [Material Design in XAML](https://github.com/MaterialDesignInXAML/MaterialDesignInXamlToolkit)
- [ValueConverters.NET](https://github.com/thomasgalliker/ValueConverters.NET)
- [WPF.JoshSmith.Controls.DragCanvas](https://github.com/denxorz/WPF.JoshSmith.Controls.DragCanvas)
- [Velopack](https://github.com/velopack/velopack)
- Moq.AutoMocker
- System.Text.Json
- Microsoft.Extensions.Hosting
- Microsoft.Extensions.DependencyInjection

![SketchNow桌面应用使用截图](https://github.com/SketchNow/SketchNow.WPF/blob/main/docs/screenshot.png)