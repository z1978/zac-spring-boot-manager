#zac-spring-boot-manager
application.properties
filemanager.html -> depository
management.html
manager.html
大家会发现前端难道就只有两个文件，jQuery、bootstrap、angularjs这些依赖难道又不需要？当然不是，这里我们为了精简（ZB），用到了webjars，webjars把常用的第三方js插件和类库打包成了jar包的形式，我们可以通过引用jar包的方式引用第三方js插件 首先得配置依赖，官方支持多种构建工具maven、gradle等，这里我们使用Maven方式


#spring-boot-filemanager
方便有文件管理功能的项目集成,不依赖后端,目前只集成了SpringBoot实现

###功能介绍
* 前后端分离,方便集成到自己的熟悉语言项目中
* 支持选择回调,如弹框文件选择
* 多语言支持
* 支持多种文件列表布局（图标/详细列表）
* 多文件上传
* 支持文件搜索
* 复制、移动、重命名
* 删除、修改、预览、下载
* 直接压缩、解压缩zip文件(支持解压zip、tar.gz、rar)
* 支持设置文件权限(UNIX chmod格式)
* 移动端支持
* 支持 OFFICE 等文档在线预览 (原生 HTML，非转码成 PDF)
* 即将支持 OFFICE 等文档在线编辑以及协同写作 (估计下一版本吧)


#[更多介绍请访问](http://shaofan.org/angular-filemanager/)

#截图

<a href="http://alexphoto.b0.upaiyun.com/ghost/angular-filemanager/screenshot.gif" target="_blank"><img src="http://alexphoto.b0.upaiyun.com/ghost/angular-filemanager/screenshot.gif" ></a>


<a href="http://alexphoto.b0.upaiyun.com/ghost/angular-filemanager/screenshot.gif" target="_blank"><img src="http://alexphoto.b0.upaiyun.com/ghost/angular-filemanager/office.gif" ></a>

#运行

* 检出项目 <code class="code-normal">git clone https://git.oschina.net/alexyang/spring-boot-filemanager.git</code>
* 再项目根目录执行 <code class="code-normal">mvn spring-boot:run</code> 或运行<code class="code-normal">SpringBootFileManagerApplication</code>

#编译angular-filemanager

> 其实利用webjars可以做到用java去编译，以后空了再弄吧。

* 编译需要用到<code class="code-normal">node.js</code>和<code class="code-normal">gulp</code>模块
* 先安装全局gulp模块 <code class="code-normal">npm install -g gulp</code>
* 然后在项目根目录执行<code class="code-normal">npm install</code>
* 最后打包编译到dist目录下 <code class="code-normal">gulp build</code>



