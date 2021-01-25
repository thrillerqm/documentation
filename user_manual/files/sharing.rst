=====================
File Sharing 文件共享
=====================

Nextcloud users can share files and folders. Possible targets are:

Nextcloud 用户可以共享文件和文件夹，可能的目标有:

* public links 公共链接
* users 用户
* groups 用户组
* circles 圈子
* talk conversations 会话
* users or groups on federated Nextcloud servers 联合云上的用户或用户组

.. note:: Some options may note be available due to administrative configuration.
   See :doc:`admin documentation <file_sharing_configuration>` for details.

.. note:: 可用选项依赖于管理的配置
   参见 :doc:`admin documentation <file_sharing_configuration>` 获取细节。

Public link shares 公共链接共享
------------------------------

You can share files and folders via public links.

您可以通过公共链接共享文件和文件夹。

A random 15-digit token will be created. The link will look like ``https://cloud.example.com/s/yxcFKRWBJqYYzp4``.

将创建一个随机的15位令牌。这个链接像 ``https://cloud.example.com/s/yxcFKRWBJqYYzp4``。

A number of options are available for public *folder* shares:

公共 *文件夹* 共享有多个：

.. figure:: ../images/sharing_public_folder.png

* **Read only** to allow viewing and downloading
* **Allow upload and editing**
* With **File drop**, the sharee can only upload files to a folder without seeing the files that are already in that folder.
* **Hide download** prevents the sharee from downloading
* **Password protect**
* **Set expiration date** will automatically disable the share
* **Note to recipient**
* **Unshare** to revert the share
* **Add another link** to create multiple public links with different rights

* **只读** 允许浏览和下载
* **允许上传和编辑**
* 使用 **文件拖拽**, 共享者只能将文件上传到文件夹，而不会看到该文件夹中已经存在的文件。
* **隐藏下载** 防止共享者下载
* **密码保护**
* **设置过期时间** 将自动关闭该共享
* **接收人备注**
* **取消共享** 以收回共享
* **添加其他链接** 以创建多个具有不同权限的链接

For public *file* shares, you may allow editing the file with one of Nextcloud's collaborative editing solutions:

对于公共 *文件* 共享, 你可以使用 Nextcloud 的协同编辑解决方案来编辑文件:

.. figure:: ../images/sharing_public_file.png


Internal shares with users and groups 用户和用户组之间的内部共享
--------------------------------------------------------------

When sharing with users, groups, circles or members of a Talk conversation, rights for the files or folder contents are adjustable:

当与用户、用户组、圈子或 Talk 对话成员共享时，文件或文件夹的共享权限可以调整:

.. figure:: ../images/sharing_internal.png

As a sharee, you can configure if you automatically want to accept all incoming shares and have them added to your root folder, or if you 
want to be asked each time if you want to accept or decline the share.



.. figure:: ../images/sharing_internal_acceptNotification.png

For adjusting the acceptance setting, go to **Settings** > **Personal** > **Sharing**:

.. figure:: ../images/sharing_autoAcceptSetting.png


Others with access
------------------

In order to find out if a file or folder is accessible to others through sharing of a superior folder 
hierarchy level, click on **Others with access** in the sharing tab:

.. figure:: ../images/sharing_others-with-access__collapsed.png

The list shows all users, groups, chats etc. that the current object has been given access to through
sharing of a superior folder in the hierarchy:

.. figure:: ../images/sharing_others-with-access__details.png

Click on the three dots to:

* see who initiated the share
* see where the share was initiated (click to navigate to the folder, as far as you have access there)
* unshare the initial share (only accessible for the share owner)


.. note:: This information is only visible to the owner of a file/folder or sharees with resharing rights.


================
Federated Shares
================

Federation Sharing allows you to mount file shares from remote Nextcloud servers, in effect 
creating your own cloud of Nextclouds. You can create direct share links with 
users on other Nextcloud servers.

Creating a new Federation Share
-------------------------------

Federation sharing is enabled by default. Follow these steps to create a new share with other Nextcloud or ownCloud servers:

Go to your ``Files`` page and click the Share icon on the file or directory 
you want to share. In the sidebar enter the username and URL of the remote user
in this form: ``<username>@<nc-server-url>``. In this example, that is
``bob@cloud.example.com``:

.. figure:: ../images/share-federation-1.png

The sharee is receiving a notification in their Nextcloud, allowing them to either accept or decline the incoming share:

.. figure:: ../images/share-federation-2-notification.png


Adding a public share to your Nextcloud
---------------------------------------

Nextcloud public link share pages offer an option to add that file or folder as a federated share into your own Nextcloud instance.
Just enter your ``<username>@<nc-server-url>`` just like shown for outbound shares above:

.. figure:: ../images/share-federation-3-public.png
