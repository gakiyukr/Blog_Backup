这个 UI 2021 年就有报道加入 Beta 计划了，然而 2023 了还没实装，这里分享一个办法，通过修改注册表强行开启云母效果。

个人认为这个效果相比 2019 2016 的原版效果还是很好看的。

## 效果图

![](https://s3-jp-ap-3.040407.xyz/oss/photos/Snipaste_07-22_19-44-00.png)

![](https://s3-jp-ap-3.040407.xyz/oss/photos/Snipaste_07-22_19-44-30.png)

![](https://s3-jp-ap-3.040407.xyz/oss/photos/Snipaste_07-22_19-44-57.png)

## 启用方法

将以下代码，保存为 .reg 注册表编辑器格式，然后运行即可。

```
Windows Registry Editor Version 5.00
[HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\ExperimentConfigs\ExternalFeatureOverrides]
[HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\ExperimentConfigs\ExternalFeatureOverrides\access]
"Microsoft.Office.UXPlatform.FluentSVRefresh"="true"
"Microsoft.Office.UXPlatform.RibbonTouchOptimization"="true"
"Microsoft.Office.UXPlatform.FluentSVRibbonOptionsMenu"="true"
[HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\ExperimentConfigs\ExternalFeatureOverrides\excel]
"Microsoft.Office.UXPlatform.FluentSVRefresh"="true"
"Microsoft.Office.UXPlatform.RibbonTouchOptimization"="true"
"Microsoft.Office.UXPlatform.FluentSVRibbonOptionsMenu"="true"
[HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\ExperimentConfigs\ExternalFeatureOverrides\onenote]
"Microsoft.Office.UXPlatform.FluentSVRefresh"="true"
"Microsoft.Office.UXPlatform.RibbonTouchOptimization"="true"
"Microsoft.Office.UXPlatform.FluentSVRibbonOptionsMenu"="true"
[HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\ExperimentConfigs\ExternalFeatureOverrides\outlook]
"Microsoft.Office.UXPlatform.FluentSVRefresh"="true"
"Microsoft.Office.UXPlatform.RibbonTouchOptimization"="true"
"Microsoft.Office.UXPlatform.FluentSVRibbonOptionsMenu"="true"
[HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\ExperimentConfigs\ExternalFeatureOverrides\powerpoint]
"Microsoft.Office.UXPlatform.FluentSVRefresh"="true"
"Microsoft.Office.UXPlatform.RibbonTouchOptimization"="true"
"Microsoft.Office.UXPlatform.FluentSVRibbonOptionsMenu"="true"
[HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\ExperimentConfigs\ExternalFeatureOverrides\project]
"Microsoft.Office.UXPlatform.FluentSVRefresh"="true"
"Microsoft.Office.UXPlatform.RibbonTouchOptimization"="true"
"Microsoft.Office.UXPlatform.FluentSVRibbonOptionsMenu"="true"
[HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\ExperimentConfigs\ExternalFeatureOverrides\publisher]
"Microsoft.Office.UXPlatform.FluentSVRefresh"="true"
"Microsoft.Office.UXPlatform.RibbonTouchOptimization"="true"
"Microsoft.Office.UXPlatform.FluentSVRibbonOptionsMenu"="true"
[HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\ExperimentConfigs\ExternalFeatureOverrides\visio]
"Microsoft.Office.UXPlatform.FluentSVRefresh"="true"
"Microsoft.Office.UXPlatform.RibbonTouchOptimization"="true"
"Microsoft.Office.UXPlatform.FluentSVRibbonOptionsMenu"="true"
[HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\ExperimentConfigs\ExternalFeatureOverrides\word]
"Microsoft.Office.UXPlatform.FluentSVRefresh"="true"
"Microsoft.Office.UXPlatform.RibbonTouchOptimization"="true"
"Microsoft.Office.UXPlatform.FluentSVRibbonOptionsMenu"="true"
```

