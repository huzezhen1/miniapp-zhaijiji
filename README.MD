# 接口
使用宅社 CLUB 接口：[点击查看](https://juejin.im/post/5bae4f6ae51d450e664b633e)

# 开发记录
1. 图片接口每天凌晨5点左右才更新一次，所以建议做适当缓存，关于数据存储方面知识，[点击查看](https://developers.weixin.qq.com/miniprogram/dev/api/storage/wx.setStorage.html)
2. 上拉触底加载使用Page的onReachBottom事件，[点击查看](https://developers.weixin.qq.com/miniprogram/dev/framework/app-service/page.html#%E9%A1%B5%E9%9D%A2%E4%BA%8B%E4%BB%B6%E5%A4%84%E7%90%86%E5%87%BD%E6%95%B0)
3. 可滑动的Tab选项卡，参考网上数据，[1.点击查看](https://blog.csdn.net/sophie_u/article/details/71745125)，[2.点击查看](https://blog.csdn.net/hanxue_tyc/article/details/78673172)，[3.点击查看](https://blog.csdn.net/an_xinyu/article/details/80226270)

# 问题记录
1. 执行 `gulp dev` 报错：`Cannot find module '@babel/core'`
答：版本搭配问题，`gulp-babel` 版本是最新的 `8`，最后回退到 `7`，`npm install --save-dev gulp-babel@7` (参考：[点击查看](https://www.cnblogs.com/soyxiaobi/p/9554565.html))

2. 执行 `gulp dev` 报错：`Task function must be specified`
答：`gulp` 版本问题，通过 `gulp -v` 发现本地 `gulp` 版本是 `4.0`，`gulp4` 和 `gulp3` 的写法不同，所以回退下版本（参考：[点击查看](https://www.cnblogs.com/evaxtt/p/9561091.html)）

