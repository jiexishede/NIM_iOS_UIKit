# 手动集成 NIMKit

### 导入代码

将 `NIMKit/NIMKit` 下的所有源代码导入你的工程


### 导入资源文件

将 `NIMKit/Resources/` 下的资源文件导入你的工程，包括

* `NIMKitResource.bundle` （主要资源文件） 
* `NIMKitEmoticon.bundle`	  (表情资源文件）
* `NIMKitSettings.bundle`  (配置资源文件)

### 手动添加 NIMSDK

`NIMKit` 主要依赖于 `NIMSDK` 以提供 IM 服务，所以需要相应添加 `NIMSDK`。手动导入 `NIMSDK` 的教程参考[这里](http://dev.netease.im/docs?doc=iOS)。

### 手动添加第三方库

除 `NIMSDK` 外，`NIMKit` 还依赖如下第三方库，需要手动进行添加

* [SDWebImage](https://github.com/rs/SDWebImage) v3.8.2
* [Toast](https://github.com/scalessec/Toast) v3.0
* [SVProgressHUD](https://github.com/SVProgressHUD/SVProgressHUD) v2.0.3
* [M80AttributedLabel](https://github.com/xiangwangfeng/M80AttributedLabel) v1.6.2
* [CTAsstsPickerController](https://github.com/chiunam/CTAssetsPickerController) v3.3.2-alpha

为防止文档更新不够及时，推荐在导入第三方库时参考当前的 [podspec](https://github.com/netease-im/NIM_iOS_UIKit/blob/master/NIMKit.podspec) 内指定的版本号。

**注:** 导入 `CTAsstsPickerController` 时需要同时添加它的 `bundle` 文件


### 添加系统依赖项

* `CoreText.framework`

### 设置额外链接选项

设置 `Other Linker Flags` 为 `-ObjC`

### 开始使用
在需要使用 `NIMKit` 组件的地方 `#import "NIMKit.h"`

