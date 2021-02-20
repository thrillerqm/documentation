=====================
Storage quota 存储配额
=====================

Your Nextcloud admin has the option to set a storage quota on users. Look at
your the Personal page to see what your quota is, and how much you have used.

你的 Nextcloud 管理员可以选择设置用户的存储配额。看看你的个人页面，看看你的配额是多少，你已经使用了多少。

.. figure:: ../images/quota1.png

It may be helpful to understand how your quota is calculated. 

了解如何计算配额可能会有帮助。

Metadata (thumbnails, temporary files, cache, and encryption keys) takes up 
about 10% of disk space, but is not counted against user quotas. Some apps 
store information in the database, such as the Calendar and Contacts apps. This 
data is excluded from your quota.

元数据(缩略图、临时文件、缓存和加密密钥)占用约 10% 的磁盘空间，但不计入用户配额。一些应用程序在数据库中存储信息，如日历和联系人应用程序。此数据不包括在您的配额之内。

When other users share files with you, the shared files count against the 
original share owner's quota. When you share a folder and allow other users or 
groups to upload files to it, all uploaded and edited files count against your 
quota. When you re-share files shared with you, the re-share still counts 
against the quota of the original share owner.

当其他用户与您共享文件时，共享文件计入原始共享所有者的配额。当您共享一个文件夹并允许其他用户或组向其上传文件时，所有上传和编辑的文件都将计入您的配额。当您重新共享与您共享的文件时，重新共享仍然计入原共享所有者的配额。

Encrypted files are a little larger than unencrypted files; the unencrypted size 
is calculated against your quota.

加密的文件比未加密的文件稍大; 未加密的大小是根据您的配额计算的。

Deleted files that are still in the trash bin do not count against quotas. The 
trash bin is set at 50% of quota. Deleted file aging is set at 30 days. When 
deleted files exceed 50% of quota then the oldest files are removed until the 
total is below 50%.

已删除但仍然在回收桶中的文件不计入配额。垃圾桶设置为配额的50% 。删除的文件过期设置为30天。当删除的文件超过配额的50% 时，最旧的文件将被删除，直到总数低于50% 。

.. note:: Your administrator may have configured the trash bin retention period 
   to override the storage space management. See `admin documentation <https://docs.nextcloud.com/server/latest/admin_manual/configuration_server/config_sample_php_parameters.html#deleted-items-trash-bin>`_ for more details.
   
.. note:: 管理员可能已经配置了垃圾桶保留期以覆盖存储空间管理。
详细信息请参阅 `admin documentation <https://docs.nextcloud.com/server/latest/admin_manual/configuration_server/config_sample_php_parameters.html#deleted-items-trash-bin>`_ 。

When version control is enabled, the older file versions are not counted against 
quotas.

当启用版本控制时，旧的文件版本不计入配额。

If you create a public share via URL and allow uploads, any uploaded files 
count against your quota.

如果你通过 URL 创建了一个公共共享并允许上传，任何上传的文件都会计入你的配额。
