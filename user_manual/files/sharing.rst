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

作为一个共享参与者，您可以配置是否自动接受所有传入的共享并将它们添加到根文件夹，或者是否每次都需要询问您是否接受或拒绝共享。

.. figure:: ../images/sharing_internal_acceptNotification.png

For adjusting the acceptance setting, go to **Settings** > **Personal** > **Sharing**:

要调整验收设置，请进入**设置** > **个人** > **共享**:

.. figure:: ../images/sharing_autoAcceptSetting.png


Others with access 其他具有访问权限的人
-------------------------------------

In order to find out if a file or folder is accessible to others through sharing of a superior folder 
hierarchy level, click on **Others with access** in the sharing tab:

为了找出一个文件或者文件夹是否可以被其他人通过共享一个更高的文件夹层级来访问，点击共享标签中的 **其他具有访问权限的人**:

.. figure:: ../images/sharing_others-with-access__collapsed.png

The list shows all users, groups, chats etc. that the current object has been given access to through
sharing of a superior folder in the hierarchy:

该列表显示当前对象通过共享层次结构中的上级文件夹而获得的访问权限的用户、组、聊天等:

.. figure:: ../images/sharing_others-with-access__details.png

Click on the three dots to:

点击三个点可以：

* see who initiated the share
* see where the share was initiated (click to navigate to the folder, as far as you have access there)
* unshare the initial share (only accessible for the share owner)

* 查看是谁邀请的共享
* 查看共享开始的位置 （只要你要访问文件夹的权限就可以通过单击导航至这个文件夹）
* 取消初始的共享 （只有共享的拥有者可以访问）


.. note:: This information is only visible to the owner of a file/folder or sharees with resharing rights.

.. note:: 此信息仅对文件/文件夹的拥有者或具有二次共享权限的用户可见。

==========================
Federated Shares 联合云共享
==========================

Federation Sharing allows you to mount file shares from remote Nextcloud servers, in effect 
creating your own cloud of Nextclouds. You can create direct share links with 
users on other Nextcloud servers.

联合云共享允许你挂载从远程 Nextcloud 服务器上共享的文件， 相当于你创建了自己的 Nextcloud 云。 您可以创建一个直接的共享连接给其他Nextcloud服务器上的用户。

Creating a new Federation Share 创建新的联合云共享
-------------------------------------------------

Federation sharing is enabled by default. Follow these steps to create a new share with other Nextcloud or ownCloud servers:

默认情况下联合共享是启用的。 按照下面的步骤创建一个与其他 Nextcloud 或 ownCloud 服务器的新共享：

Go to your ``Files`` page and click the Share icon on the file or directory 
you want to share. In the sidebar enter the username and URL of the remote user
in this form: ``<username>@<nc-server-url>``. In this example, that is
``bob@cloud.example.com``:

转到 ``Files`` 页 并单击你要共享的文件或文件夹的共享图标。 在侧边栏输入如 ``<username>@<nc-server-url>`` 形式的远程用户的用户名和URL。 在这个例子中，是``bob@cloud.example.com``：

.. figure:: ../images/share-federation-1.png

The sharee is receiving a notification in their Nextcloud, allowing them to either accept or decline the incoming share:

共享参与者在他们的 Nextcloud 中将收到了一个通知，允许他们接受或拒绝收到的共享:

.. figure:: ../images/share-federation-2-notification.png


Adding a public share to your Nextcloud 为你的Nextcloud添加一个公共共享
---------------------------------------------------------------------

Nextcloud public link share pages offer an option to add that file or folder as a federated share into your own Nextcloud instance.
Just enter your ``<username>@<nc-server-url>`` just like shown for outbound shares above:

Nextcloud 公共共享链接页面提供了一个选项，可以将该文件或文件夹作为联合云共享添加到自己的 Nextcloud 实例中。
只要输入你的 ``<username>@<nc-server-url>`` 就像上面显示的出站共享。

.. figure:: ../images/share-federation-3-public.png
