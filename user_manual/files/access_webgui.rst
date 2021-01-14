=================================
使用 Nextcloud Web 界面访问你的文件
=================================

You can access your Nextcloud files with the Nextcloud Web interface and create,
preview, edit, delete, share, and re-share files. Your Nextcloud administrator
has the option to disable these features, so if any of them are missing on your
system ask your server administrator.

您可以通过 Nextcloud Web 界面访问 Nextcloud 文件，并创建、预览、编辑、删除、共享和重新共享文件。你的 Nextcloud 管理员可以选择禁用这些功能，所以如果你的系统缺少这些功能，请咨询你的服务器管理员。

.. figure:: ../images/users-files.png
   :alt: The Files view screen.

Tagging files | 为文件添加标签
-----------------------------

You can assign tags to files. To create tags, open a file to the Details view.
Then type your tags. To enter more than one tag press the return key after
creating each tag. All tags are system tags, and are shared by all users on your
Nextcloud server.

您可以为文件分配标签。若要创建标签，请在“详细信息”视图中打开一个文件。然后输入你的标签。若要输入多个标签，请在创建每个标签后按回车键。所有的标签都是系统标签，并由 Nextcloud 服务器上的所有用户共享。

.. figure:: ../images/files_page-7.png
   :alt: Creating file tags.

Then use the Tags filter on the left sidebar to filter files by tags:

然后使用左侧边栏的标签（Tags）过滤器通过标签过滤文件：

.. figure:: ../images/files_page-8.png
   :alt: Viewing file tags.

Comments | 评论
---------------

Use the Details view to add and read comments on any file or folder. Comments
are visible to everyone who has access to the file:

使用“详细信息”视图可以添加和读取对任何文件或文件夹的评论。每个可以访问该文件的人都可以看到评论：

.. figure:: ../images/file_menu_comments_2.png
   :alt: Creating and viewing comments.

Video player | 视频播放器
------------------------

You can play videos in Nextcloud with the Video Player app by simply clicking on
the file. Video streaming by the native Nextcloud video player depends on your Web browser
and the video format. If your Nextcloud administrator has enabled video
streaming, and it doesn't work in your Web browser, it may be a browser issue. See https://developer.mozilla.org/en-US/docs/Web/HTML/Supported_media_formats#Browser_compatibility for supported multimedia formats in Web browsers.

你可以通过视频播放器应用在 Nextcloud 播放视频，只需点击文件即可。本地 Nextcloud 视频播放器的视频流取决于您的 Web 浏览器和视频格式。如果你的 Nextcloud 管理员已经启用了视频流，但是它不能在你的 Web 浏览器中工作，这可能是一个浏览器问题。有关 Web 浏览器中支持的多媒体格式，请参阅 https://developer.mozilla.org/en-us/docs/Web/html/supported_media_formats#browser_compatibility。

.. figure:: ../images/video_player_2.png
   :alt: Watching a movie.

File controls | 文件控制
-----------------------

Nextcloud can display thumbnail previews for image files, MP3 covers,
and text files, if this enabled by your server administrator. Hover your cursor
over a file or folder to expose the controls for the following operations:

Nextcloud 可以显示图像文件、 MP3封面和文本文件的缩略图预览，这需要服务器管理员启用该功能。将光标悬停在文件或文件夹上，以公开下列操作的控件:

Favorites | 收藏夹
  Click the star to the left of the file icon to mark it as a favorite:
  
  点击文件图标左侧的星号，将其标记为收藏:
  
  .. figure:: ../images/files_page-1.png
   :alt: Marking Favorite files.
   
  You can also quickly find all of your favorites with the Favorites filter on the left
  sidebar.
  
  你也可以通过左侧边栏的收藏夹过滤器快速找到你所有的收藏夹。

Overflow Menu | 溢出菜单
  The Overflow menu (three dots) displays file details, and allows you to
  rename, download, or delete files:
  
  溢出菜单(三个点...)显示文件详细信息，并允许您重命名、移动、下载或删除文件:

  .. figure:: ../images/files_page-3.png
   :alt: Overflow menu.

  The Details view shows Activities, Sharing, and Versions information:
  
  详细信息视图显示活动、共享和版本信息：

.. figure:: ../images/files_page-4.png
   :alt: Details screen.

The **Settings** gear icon at the lower left allows you to show or hide hidden
files in your Nextcloud Web interface. These are also called dotfiles, because
they are prefixed with a dot, e.g. ``.mailfile``. The dot tells your operating
system to hide these files in your file browsers, unless you choose to display
them. Usually these are configuration files, so having the option to hide them
reduces clutter.

左下角的 **设置** 齿轮图标允许你在 Nextcloud Web 界面中显示或不显示隐藏文件。这些文件也称为 点文件，因为它们前面有一个点，例如``.mailfile``。点告诉你的操作系统在你的文件浏览器中隐藏这些文件，除非你选择显示它们。通常这些都是配置文件，因此可以选择隐藏它们以减少混乱。

.. figure:: ../images/hidden_files.png
   :alt: Hiding or displaying hidden files.

Previewing files | 预览文件
--------------------------

You can display uncompressed text files, OpenDocument files, videos, and image
files in the Nextcloud embedded viewers by clicking on the file name. There may
be other file types you can preview if your Nextcloud administrator has enabled
them. If Nextcloud cannot display a file, it starts a download process and
downloads the file to your computer.

通过点击文件名，你可以在 Nextcloud 嵌入的查看器中显示未压缩的文本文件、 OpenDocument 文件、视频和图像文件。如果 Nextcloud 管理员启用了其他类型文件的支持，您也可以预览它们。如果 Nextcloud 不能显示一个文件，它会启动一个下载进程并将该文件下载到您的计算机。

Navigating inside your Nextcloud | 在Nextcloud中导航
-------------------------------------------------------

Navigating through folders in Nextcloud is as simple as clicking on a folder to
open it and using the back button on your browser to move to a previous level.
Nextcloud also provides a navigation bar at the top of the Files field for quick
navigation.

在 Nextcloud 中浏览文件夹很简单，只需通过点击就可以打开文件夹，然后使用浏览器的后退按钮就可以返回上一级。Nextcloud 还在文件区域顶部提供了一个导航栏，用于快速导航。

Sharing status icons | 共享状态图标
----------------------------------

Any folder that has been shared is marked with the ``Shared`` overlay icon.
Public link shares are marked with a chain link. Unshared folders are not marked:

任何已经被共享的文件夹都用“共享”覆盖图标标记。公共链接共享使用“链”标记。非共享文件夹没有标记：

.. figure:: ../images/files_page-5.png
   :alt: Share status icons.

Creating or uploading files and directories | 创建或上传文件和文件夹
------------------------------------------------------------------

Upload or create new files or folders directly in a Nextcloud folder by clicking
on the *New* button in the Files app:

点击文件应用中的 *新建* 按钮，直接在 Nextcloud 文件夹中上传或创建新文件或文件夹:

.. figure:: ../images/files_page-6.png
   :alt: The New file/folder/upload menu.

The *New* button provides the following options:

*新建* 按钮提供以下选项:

Up arrow | 上传
  Upload files from your computer into Nextcloud. You can also upload files by
  dragging and dropping them from your file manager.
  
  从你的电脑上传文件到 Nextcloud。还可以通过从文件管理器中拖放文件来上传文件。

Text file | 文本文件
  Creates a new text file and adds the file to your current folder.
  
  创建一个新的文本文件并将该文件添加到当前文件夹中。

Folder | 文件夹
  Creates a new folder in the current folder.
  
  在当前文件夹中创建一个新文件夹。

Selecting files or folders | 选择文件或文件夹
--------------------------------------------

You can select one or more files or folders by clicking on their checkboxes. To
select all files in the current directory, click on the checkbox located at the
top of the files listing.

您可以通过单击复选框来选择一个或多个文件或文件夹。要选择当前目录中的所有文件，请单击文件列表顶部的复选框。

When you select multiple files, you can delete all of them, or download them as
a ZIP file by using the ``Delete`` or ``Download`` buttons that appear at the
top.

当您选择多个文件时，您可以使用顶部的 ``删除``按钮删除所有文件，或者使用``下载`` 按钮将它们作为 ZIP 文件下载。

.. note:: If the ``Download`` button is not visible, the administrator has
   disabled this feature.
   
.. note:: 如果 ``下载`` 按钮无效, 则是管理员已禁用该功能。

Filtering the files view | 过滤文件视图
--------------------------------------

The left sidebar on the Files page contains several filters for quickly sorting
and managing your files.

文件页面的左侧边栏包含几个用于快速排序和管理文件的过滤器。

All files | 所有文件
  The default view; displays all files that you have access to.
  
  默认视图；显示所有你可以访问的文件。

Favorites | 收藏夹
  Files or folders marked with the yellow star.
  
  使用黄星标记的文件或文件夹。

Shared with you | 你共享的文件
  Displays all files shared with you by another user or group.
  
  显示所有你共享给其他用户或用户组的文件。

Shared with others | 别人共享的文件
  Displays all files that you have shared with other users or groups.
  
  显示所有其他用户或用户组共享给你的文件。

Shared by link | 使用链接共享的文件
  Displays all files that are shared by you via public link.
  
  显示所有你通过公共链接共享出的文件。

External Storage (optional) | 外部存储（可选）
  Files that you have access to on external storage devices and services such
  as Amazon S3, SMB/CIFS, FTP…
  
  您可以访问外部存储设备和服务上的文件，如 Amazon S3、 SMB/CIFS、 FTP等。

Moving files | 移动文件
----------------------

You can move files and folders by dragging and dropping them into any directory.

你可以通过拖拽至其他目录来移动文件或文件夹

Creating or connecting to a Federation Share link | 创建或连接到联合共享链接
--------------------------------------------------------------------------

Federated Cloud Sharing allows you to mount file shares from remote Nextcloud
servers, and manage them just like a local share. See :doc:`federated_cloud_sharing` 
to learn to how to create and connect to new Federated Cloud shares.

联合云共享允许您从远程 Nextcloud 服务器挂载文件共享，并像管理本地共享一样管理它们。请参阅 :doc:`federated_cloud_sharing` 来学习如何创建和连接到新的联合云共享。
