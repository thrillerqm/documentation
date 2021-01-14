=================
Nextcloud Web界面
=================

You can connect to your Nextcloud server using any Web browser. Just point it to
your Nextcloud server URL (e.g. cloud.example.com) and enter your username and password:

您可以使用任何 Web 浏览器连接到 Nextcloud 服务器。只需将其指向你的 Nextcloud 服务器 URL (例如 cloud.example.com 服务器) ，然后输入你的用户名和密码:

.. figure:: images/login_page.png
     :alt: Nextcloud login screen.

Web browser requirements | Web浏览器要求
---------------------------------------

For the best experience with the Nextcloud web interface, we recommend that you use the 
latest and supported version of a browser from this list:

为了获得使用 Nextcloud Web界面的最佳体验，我们建议您使用以下列表中最新的、支持的浏览器版本:

* Microsoft **Internet Explorer**
* Microsoft **Edge**
* Mozilla **Firefox**
* Google **Chrome**/Chromium
* Apple **Safari**

.. note:: If you want to use Nextcloud Talk you need to run Mozilla **Firefox** 52+
   or Google **Chrome**/Chromium 49+ to have the full experience with video calls and 
   screensharing. Google **Chrome**/Chromium requires a additional plugin for screensharing.

.. note:: 如果你想使用Nextcloud Talk， 你需要运行Mozilla **Firefox** 52+
   或 Google **Chrome**/Chromium 49+ 来获得完整的视频通化和屏幕分享体验. Google **Chrome**/Chromium 需要一个额外的屏幕分享插件。 

Navigating the main user interface | 浏览用户主界面
--------------------------------------------------

By default, the Nextcloud Web interface opens to your Dashboard or Files page:

默认情况下，Nextcloud Web 界面会打开你的看板（Dashboard）或文件（Files）页面：

.. figure:: images/files_page.png
     :scale: 75%
     :alt: The main Files view.
     
In Files you can add, remove, and share files, and make changes based on the access privileges
set by you (if you are administering the server) or by your server administrator.

在“文件（Files）”中，您可以添加、删除和共享文件，并根据您（如果您正在管理服务器）或服务器管理员设置的访问权限进行更改。

The Nextcloud user interface contains the following fields and functions:

Nextcloud用户界面包括以下区域和功能：

* **Apps Selection Menu** (1): Located in the upper left corner, you'll find all
  your apps which are available on your instance of Nextcloud. Clicking on an
  apps icon will redirect you to the app.

* **应用选择菜单** (1): 位于左上角，你可以找到所有在 Nextcloud 实例中可用的应用。点击应用图标会将你重定向到该应用。

* **Apps Information** field (2): Located in the left sidebar, this provides
  filters and tasks associated with your selected app. For example, when you
  are using the Files apps you have a special set of filters for quickly
  finding your files, such as files that have been shared with you, and files
  that you have shared with others. You'll see different items for other apps.

* **应用信息** 区域 (2): 位于左侧边栏，提供了与您选定的应用相关过滤器和任务。例如，当你使用文件应用时，你有一套特殊的过滤器用于快速查找你的文件，比如与你共享的文件，以及与他人共享的文件。你会看到其他应用程序的不同条目。

* **Application View** (3): The main central field in the Nextcloud user interface.
  This field displays the contents or user features of your selected app.

* **应用程序视图** (3): Nextcloud 用户界面的主要中心区域。此区域显示所选应用的内容或用户特性。

* **Navigation Bar** (4): Located over the main viewing window (the Application
  View), this bar provides a type of breadcrumbs navigation that enables you to
  migrate to higher levels of the folder hierarchy up to the root level (home).

* **导航栏** (4): 位于主视窗（应用程序视图）上方, 工具栏提供了一种面包屑导航，使您可以迁移到文件夹层次结构的更高级别（主页）。

* **New** button (5): Located in the Navigation Bar, the ``New`` button
  enables you to create new files, new folders, or upload files.

* **新建** 按钮 (5): 位于导航栏内, 通过“新建” 按钮您可以创建新文件、新文件夹或上传文件。

.. note:: You can also drag and drop files from your file manager into the
   Files Application View to upload them to your instance. Currently,
   the only Web browsers that support drag-and-drop folders are Chrome and
   Chromium.

.. note:: 您还可以将文件从文件管理器拖放到“文件应用程序视图”中，以将文件上传到实例。目前，唯一支持拖放文件夹的浏览器是 Chrome 和 Chromium。

* **Search** field (6): Click on the magnifier in the upper right hand corner of
  to search for files.
  
* **搜索** 区域 (6): 单击右上角的放大镜以搜索文件。

* **Contacts Menu** (7): Gives you an overview about your contacts and users on
  your server. Dependent on the given details and available apps, you can
  directly start a video call with them or send emails.
  
* **联系人菜单** (7): 提供关于服务器上联系人和用户的概况。 根据提供的细节和可用的应用情况，你可以直接与他们启动视频电话或发送电子邮件。

* **Grid view** button (8). This looks like four little squares, which toggles
  the grid view for folders and files.
  
* **网格视图** 按钮 (8). 这看起来像四个小方块，用于切换文件夹和文件的网格视图。
  
* **Settings** menu (9): Click on your profile picture,
  located to the right of the Search field, to open your Settings
  dropdown menu. Your Settings page provides the following settings and features:
  
* **设置** 菜单 (9): 点击您的个人资料图片，位于搜索区域的右侧，以打开您的设置下拉菜单。你的设置页面提供了以下设置和功能:

  * Links to download desktop and mobile apps
  * Server usage and space availability
  * Password management
  * Name, email, and profile picture settings
  * Manage connected browsers and devices
  * Group memberships
  * Interface language settings
  * Manage notifications
  * Federated Cloud ID and social media-sharing buttons
  
  * 下载桌面和移动应用的链接
  * 服务器使用情况和可用空间
  * 密码管理
  * 用户名、电子邮件和个人资料图片设置
  * 管理已连接的浏览器和设备
  * 团体成员资格
  * 界面语言设置
  * 管理通知
  * 联合云 ID 和社交媒体分享按钮
  * 用于外部存储的 SSL/TLS 证书管理器
  * 你的双因子验证
  * Nextcloud 版本

See :doc:`userpreferences` section to learn more about these settings.

参见 :doc:`userpreferences` 部分以了解有关这些设置的更多信息。
