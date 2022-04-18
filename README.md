# hugo-theme-qiuqiu

一款精简的博客主题

### 博客页面结构

博客页面结构如下所示：
- 首页
- 归档页
- 文章页
- 分类汇总页
- 分类页
- 标签汇总页
- 标签页
- 关于页
- 个人简历页面

### 公共结构

- header模块
- footer模块

##### 首页结构拆解

首页分为左右两栏，左侧是近期文章列表及简要内容，右侧是搜索

### 待办事项
- [x] LOGO，要求640px * 160px
- [x] 确认主题颜色，暂定Taptap蓝
- [x] 添加favicon.ico
- [x] 首页文章卡片样式选择
- [x] 首页文章列表分页
- [x] 各页面title问题
- [x] 各页面meta和关键字问题
- [x] 文章图片问题（图床）
- [ ] 文章目录，参考https://gohugo.io/content-management/toc/
- [x] 首页样式美观问题
- [x] header顶部吸附问题
- [x] 不同设备间响应式布局问题
- [x] 归档页面样式问题
- [x] taxonomy list页面样式问题
- [x] taxonomy term页面样式问题
- [x] 标签和分类样式优化，改为颜色随机
- [x] 关于页面完善和补充
- [x] 404页面优化
- [x] 支持数学公式
- [x] 社交媒体链接支持
- [x] 微信公众号icon增加划过展示二维码功能
- [x] 自定义样式加载问题
- [ ] 研究下站内搜索，可参考algolia
- [ ] 研究下站内评论，可参考discus，gitalk
- [ ] 增加网站访问统计分析
- [ ] 增加简历页面
- [ ] 增加赞助页面
- [x] 调整文章标题，一级标题用h1，二级标题用h3（使用Typora时注意）
- [x] 首页文章列表的三个tag，日期，字数，阅读时间
- [x] 文章支持slug，提升网站可检索性
- [x] 修改content样式下的img样式，使得图片居中展示
- [x] 文章头图去掉默认的16x9，因为会导致图像变形失真
- [ ] 在文章页面底部，增加默认版权声明区域，如“转载本站文章请注明作者和出处”，可参考message展示形式
- [ ] 在文章页面底部，增加公众号二维码引流板块
- [ ] 在文章页面增加悬浮分享图标，引导用户分享到微信朋友圈，方案：使用qrcode插件，或对接微信公众号JSSDK
- [ ] 在文章页面底部增加打赏功能，可以考虑将关注，分享，打赏放到一个板块里面来展示
- [x] 首页文章列表，如果未分页，则去掉水平分隔线
- [x] 为了支持sticky footer设置，把footer标签上的都用div包起来，取一个id=wrapper
- [ ] 文章列表（归档页）增加分页支持，待调研
- [x] 标题太长的问题，需要做缩略处理，15个字以内
- [x] 在文章页面底部，增加标签和分类显示
- [x] 在文章归档页面，增加每年文章数量显示，共xxx篇
- [x] 站点首页，阅读更多 改为 阅读全文
- [x] 解决tags/categories的大写英文在连接中自动转小写的问题
- [x] 统一用{{ $.Site.Title }}代替硬编码方式的站点命名
- [x] Categories和Tags页面，标签组后面的数字，取消超链接