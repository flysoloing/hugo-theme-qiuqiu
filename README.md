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
- [x] 确认主题颜色，暂定Taptap蓝，或者类似颜色
- [x] 添加favicon.ico
- [x] 首页文章卡片样式选择
- [x] 首页文章列表分页
- [x] 各页面title问题
- [x] 各页面meta和关键字问题，具体文章页面的关键字使用Front Matter里的keyword填充，或者将tags转换为keywords
- [x] 文章图片问题（图床）
- [ ] 在文章页面，增加文章目录，在移动端打开时隐藏，具体实现参考https://gohugo.io/content-management/toc/
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
- [x] 考虑增加图片和图注的增强实现，figure，有两种途径，一是在hugo action中，二是在页面加载时JS异步处理dom元素
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
- [ ] 增加相关文章列表
- [ ] 增加最近更新文章列表，在归档页，或者在首页右边栏，在移动端打开时隐藏
- [x] page页面最下面，去掉“分类：”和“标签：”
- [x] 国内外访问性能优化，使用CDN加速，如Cloudflare，vercel，netlify等
- [x] 优化数学公式相关JS加载性能，根据hasMathFormula进行判断，true or false
- [x] 优化qiuqiu.css，精简不必要元素组件，同时采用压缩编译，head.html已改为qiuqiu.min.css引用
- [x] 若文章有更新，在文章内增加文章更新于X年X月X日的提示
- [x] 是否展示封面图片，由cover_image，改为coverImage进行判断，统一名命风格
- [ ] 文章页面侧边栏，增加悬浮按钮，快速回到顶部
- [x] 文章页面底部，增加一两行空行，避免文章内容离分类和标签太近
- [x] 减少第三方JS库的依赖，如jQuery的用途不多，可以用原生JavaScript脚本替换，提升页面加载速度
- [x] img图片元素增加alt属性，优化SEO效率
- [ ] 考虑文章标题过短过长时，确保分页展示保持一致，在移动端时表现为上下堆叠？
- [x] 将标题格式从之前的“Site Title | Page Title”改为“Page Title - Site Title”
- [x] SEO，增加百度/Google等搜索引擎的收录
- [x] fontawesome实在太慢，准备用本地引用方式替换线上引用
- [x] 之前使用的fontawesome是5.15.4版本，当前版本为6.2.1版本
- [ ] 增加阅读次数统计，阅读排行列表
- [x] 图片上传时增加水印，基于PicGo的水印插件实现，watermark
- [ ] 文章底部标签模式更换为breadcrumb格式
- [x] 标签云展示优化，根据每个标签的数值，分为3档，is-normal，is-medium和is-large
- [ ] copyright年份改为实时动态展示，年份相同则不更改，否则更新为最新
- [x] 增加自定义站点统计脚本，包括站点PV和文章PV展示
- [ ] 锚链接定位问题，由于目前菜单栏遮挡，需重新定位，包括PC端和移动端
- [ ] 基于Midjourney修改博客logo，基于自己的照片，定制专属个人头像
- [x] 在文章内容页面，使用<div class="main"></div>来包装正文，便于后续自动化提取
- [x] 若文章由AI辅助创作，在文章正文前增加文章AI辅助创作的声明