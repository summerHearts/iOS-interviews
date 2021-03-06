## 性能优化[卡顿、崩溃、app启动]
---
### 性能优化 - cpu、gpu
核心：减少cpu、gpu的资源消耗

cpu的作用：
- 对象管理(销毁与创建);
- 对象的维护(属性调整、布局计算、文本计算和排版、图片格式转换和解码)
- 图像的绘制(CG)

gpu的作用：
- 纹理渲染
- 视图合成

### 崩溃
unrecognized selector、KVO、NSTimer、Container、Bad Access

### app启动
通过环境变量DYLD_PRINT_STATISTICS查看启动时间

1> 冷启动 - 首次启动
- dyld
- runtime
- main

2> 热启动 - 后台激活

[官方资料一](https://developer.apple.com/videos/play/wwdc2017/413/)
[官方资料二](https://developer.apple.com/videos/play/wwdc2016/406/)

### 参考
- [25 iOS App Performance Tips & Tricks](https://www.raywenderlich.com/2752-25-ios-app-performance-tips-tricks) [**中文翻译**](https://blog.csdn.net/github_34613936/article/details/51302547)
- [iOS 保持界面流畅的技巧](https://blog.ibireme.com/2015/11/12/smooth_user_interfaces_for_ios/)
- [iOS启动优化](https://juejin.im/entry/5b63fb115188257bca291fbc)
- [阿里数据iOS端启动速度优化的一些经验](https://www.jianshu.com/p/f29b59f4c2b9)
- [iOS App 启动性能优化](https://chars.tech/blog/ios-app-launch-time-optimize/)
- [深入理解iOS App的启动过程](https://blog.csdn.net/Hello_Hwc/article/details/78317863)
- [iOS 浅谈GPU及“App渲染流程”](https://juejin.im/post/5e80b49751882573be11b138)