======================================
Managing deleted files 管理已删除的文件
======================================

When you delete a file in Nextcloud, it is not immediately deleted permanently,
only moved into the trash bin. It is not permanently deleted until you manually
delete it, or when the Deleted Files app deletes it to make room for new files.

当你在 Nextcloud 删除一个文件时，它不会立即被永久删除，只是移动到垃圾桶中。除非您手动删除它，或删除文件应用程序删除它以为新文件腾出空间，否则它不会被永久删除。

Find your deleted files by clicking on the **Deleted files**
button on the Files page of the Nextcloud Web interface. You'll have options to
either restore or permanently delete files.

通过点击 Nextcloud Web 界面的文件页面上的 **Deleted Files** 按钮找到您删除的文件。您可以选择恢复或永久删除文件。

Quotas 配额
-----------

Deleted files are not counted against your storage quota. Only your personal
files count against your quota, not files which were shared with you.
(See :doc:`quota` to learn more about quotas.)

删除的文件不计入你的存储配额。只有您的个人文件计算在您的配额，与您共享的文件不会计算。(请参阅:doc:`quota` 以了解更多关于配额的信息。)

What happens when shared files are deleted 删除共享文件时会发生什么
-----------------------------------------------------------------

Deleting files gets a little complicated when they are shared files, as this
scenario illustrates:

当文件是共享文件时，删除文件会变得有点复杂，描述如下:

1. User1 shares a folder "test" with User2 and User3
2. User2 (the recipient) deletes a file/folder "sub" inside of "test"
3. The folder "sub" will be moved to the trash bin of both User1 (owner) and
   User2 (recipient)
4. But User3 will not have a copy of "sub" in their trash bin

1. 用户1 共享一个文件夹 “test” 给 用户2 和 用户3
2. 用户2 (接收者) 删除 “test” 中的一个文件/文件夹“sub”
3. 文件夹“sub” 将会被移动至 用户1 (所有者) 和 用户2 (接收者)的垃圾桶
4. 但是 用户3 的垃圾桶里不会有“sub”的一个副本

When User1 deletes "sub" then it is moved to User1's trash bin. It is
deleted from User2 and User3, but not placed in their trash bins.

当 用户1 删除“sub”，它会移动到 用户1 的垃圾桶。它会从 User2和 User3中删除，但不会被放到垃圾箱中。

When you share files, other users may copy, rename, move, and share them with
other people, just as they can for any computer files; Nextcloud does not have
magic powers to prevent this.

当你共享文件时，其他用户可能会复制、重命名、移动并与其他人共享，就像他们可以共享任何计算机文件一样; Nextcloud 没有魔力来阻止这种情况。

How the deleted files app manages storage space 删除文件应用如何管理存储空间
--------------------------------------------------------------------------

To ensure that users do not run over their storage quotas, the Deleted Files
app allocates a maximum of 50% of their currently available free space to
deleted files. If your deleted files exceed this limit, Nextcloud deletes the
oldest files (files with the oldest timestamps from when they were deleted)
until it meets the memory usage limit again.

为了确保用户不会超过他们的存储配额，删除文件应用分配最多50% 的当前可用空闲空间给删除的文件。如果您删除的文件超过这个限制，Nextcloud 将删除最旧的文件(从删除文件时开始计时的最旧时间戳的文件) ，直到它再次达到存储使用限制。

Nextcloud checks the age of deleted files every time new files are added to the
deleted files. By default, deleted files stay in the trash bin for 30 days. The
Nextcloud server administrator can adjust this value in the ``config.php`` file
by setting the ``trashbin_retention_obligation`` value. Files older than the
``trashbin_retention_obligation`` value will be deleted permanently.
Additionally, Nextcloud calculates the maximum available space every time a new
file is added. If the deleted files exceed the new maximum allowed space
Nextcloud will permanently delete those trashed files with the soonest expiration
until the space limit is met again.

每次新文件添加到被删除的文件时，Nextcloud 都会检查被删除文件的已删除时间。默认情况下，删除的文件会在垃圾桶中保留30天。服务器管理员可以通过设置config.php 文件中的 trashbin retention obligation 值来调整这个值。已删除时间超过 trashbin_retention_obligation 值的文件将被永久删除。此外，Nextcloud 计算每次添加新文件时的最大可用空间。如果删除的文件超过新的最大允许空间 Nextcloud 将永久删除那些删除文件的最快期限，直到再次满足空间限制。

.. note:: Your administrator may have configured the trash bin retention period 
   to override the storage space management. See `admin documentation <https://docs.nextcloud.com/server/latest/admin_manual/configuration_server/config_sample_php_parameters.html#deleted-items-trash-bin>`_ for more details.
   
.. note:: 管理员可能已经配置了垃圾桶保留期以覆盖存储空间管理。 参见 `admin documentation <https://docs.nextcloud.com/server/latest/admin_manual/configuration_server/config_sample_php_parameters.html#deleted-items-trash-bin>`_ 获取更多细节。
