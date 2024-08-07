# 前言
由于 Windows 占用过于的大，所以性能差的童鞋只能装低版本 Windows
蛋柿，只要把 Windows 的一些用不上功能砍掉，不就变得流畅了吗？
# 准备工作
你需要：
[MSMG Toolkit汉化版](https://sige666.lanzoul.com/iBKmb259l37i) 提取码：hvax
[一个原版 Windows 映像](https://hellowindows.cn/)
一双灵巧的手以及一个聪明的大脑
# 挂载映像
关闭杀毒软件或者将 MSMG Toolkit 所在的文件夹设置为白名单，随后双击挂载你下载的原版 Windows 映像，如果不成功，则可以使用软碟通等软件
复制这个映像里所有的文件，将它们复制到 MSMG Toolkit 文件夹中的 DVD 文件夹
右击 MSMG Toolkit 中的 Start.cmd 或者 Toolkit.cmd，选择以管理员身份运行，弹出的蓝色框框中按 A 同意协议，随后，工具箱就跑起来了
在跳转的工具箱首页中选择 1 ，随后再按一次 1，按自己需要选择需要精简的 Windows 版本，若有多个版本，用空格隔开
第一个问题按 Y ，随后都按 N
等待进度条跑完，我们就可以开始精简了
# 精简系统
我们在首页按 3 选择移除，再按 1，最后按 C 选择兼容性，不先移除这里的选项，会导致后面的依赖项无法移除
这里的选项都可以精简，但是全精简了，非常影响系统使用体验，建议按我的来
![兼容性](https://github.com/user-attachments/assets/792287de-9c02-4f36-a80e-0accd7366b76)
退出以后我们去选择移除的 Windows 组件
首先是 Internet，这里建议精简掉 Internet Explorer，但是你精简掉 Edge 也行，但注意必须保留 Edge WebView，别问我怎么知道的
然后是多媒体，只要你有替代品都可以精简
网络？都可以精简
隐私？ emm，预览体验计划你用得上可以留着
远程处理建议全干掉，系统建议留 WSL、防火墙、如果没有记事本的替代品的话，建议留着记事本，有个第三方安全软件的嘛……那安全中心也别留了
系统应用如果要登微软账号就别删 Content Delivery Manager 和设置同步
如果有第三方杀毒软件 就精简掉 SmartScreen 和 Windows Defender + Windows 安全中心，如果你不用 Start11 或者 Startallback ，也没有 Explorer Patcher ，那就别管”开始“菜单，打印服务如果要用，也留着
文件资源管理器切记不要精简，除非你有第三方的
最后一个如果你玩游戏也不要精简
Windows 应用建议全干掉
返回到移除系统组件那里，按 2，等待个几分钟，精简就完成了
# 集成功能
可能有人会问：”你不是说精简系统吗？怎么还要集成功能？“
但是，你装过了系统默认是不带 .NET 框架的，有一些软件就跑不起来了，所以这就需要我们去主页按 2 集成 .NET 框架
# 保存映像
首页按 6，再按 2，问你要不要剔除没有修改的那些版本，如果需要剔除，那么工具箱就会剔除掉映像里那些没有修改过的版本，随后下面一个问题就按 Y，等待精简完成
但是现在只有 install.wim，还无法直接安装，所以我们就需要把它打包成 ISO 格式
首页按 7，再按 1
ISO 卷标就是映像挂载到电脑里后显示的名称
ISO 名称就是映像的文件名
等待进度条跑完，这个系统就已经打包完成了
按任意键回到首页，再按一次 x 退出，这时候你就会发现在 MSMG Toolkit 工具箱的 ISO 文件夹内就有你刚才精简的映像
# 结束语
事实上，只用 MSMG Toolkit 来精简系统是不够的，还需要配合 NTLite 之类的专业软件，不过……你现在精简好的这个系统，是可以拿来当做日常系统用的
我自己做的这个成品，我以后会发布的：）