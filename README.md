### Sublime Text 2/3 输入法修复[Ubuntu(Debian)]

主要目的:

+ 安装 Sublime Text 3
+ 安装 Fcitx 输入法 + 皮肤
+ 修复 Sublime Text 2/3's 在 Ubuntu(Debian) 系统下的无法输入中文输入法的问题

### 使用方法 ###

+ 更新并升级系统为最新(较新的系统会解决很多可能出现的问题)

```bash
sudo apt-get update && sudo apt-get upgrade
```

+ 克隆项目到本地 : 

```bash
git clone https://github.com/Moonshile/sublime-text-imfix
```

+ 运行脚本 : 

```bash
cd sublime-text-imfix && ./sublime-imfix
```

+ 完成! 重新启动后就可以在Sublime Text 2/3 中 使用Fcitx了! 注意: 皮肤可能需要自己选择 ^_^

### 效果图:

![Fcitx](image/fcitx.png)

### 重要提示:

+ **这个修复仅当在终端中使用 `subl .` 调用Sublime Text的时候有效, 具体原因请看源代码[src/subl](https://github.com/lyfeyaj/sublime-text-imfix/blob/master/src/subl)**

### 补充
比较纠结的是我重新登录之后切换输入法非常麻烦。解决方案是

1. 点击任务栏右上角的键盘图案，选择“配置”，然后把多余的都删掉，只留下“拼音”和“键盘 - 英(美国)”两项。这是通过手动选择就已经可以输入中文了。
2. 还是在这个对话框，选择“全局配置”选项卡，点击“切换激活/非激活输入法”旁边的第一个按钮，然后按shift。这是就可以使用shift切换输入法了！
