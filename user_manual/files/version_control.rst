=======================
Version control 版本控制
=======================

Nextcloud supports simple version control system for files. Versioning creates
backups of files which are accessible via the Versions tab on the Details
sidebar. This tab contains the history of the file where you can roll back a
file to any previous version. Changes made at intervals greater than two minutes
are saved in **data/[user]/files_versions**.

Nextcloud 支持简单的文件版本控制系统。版本控制创建文件的备份，这些文件可以通过 Details 侧边栏的 Versions 选项卡进行访问。此选项卡包含文件的历史记录，您可以将文件回滚到以前的任何版本。间隔大于两分钟的更改保存在 **data/[user]/files_versions** 。

.. figure:: ../images/files_versioning.png

To restore a specific version of a file, click the circular arrow to the left.
Click on the timestamp to download it.

若要还原文件的特定版本，请单击左侧的圆形箭头。点击时间戳下载。

The versioning app expires old versions automatically to make sure that
the user doesn't run out of space. This pattern is used to delete
old versions:

版本控制应用程序会自动终止旧版本，以确保用户不会用尽空间。这个模式用于删除旧版本:

* For the first second we keep one version
* For the first 10 seconds Nextcloud keeps one version every 2 seconds
* For the first minute Nextcloud keeps one version every 10 seconds
* For the first hour Nextcloud keeps one version every minute
* For the first 24 hours Nextcloud keeps one version every hour
* For the first 30 days Nextcloud keeps one version every day
* After the first 30 days Nextcloud keeps one version every week

* 第一秒我们保留一个版本
* 在开始的10秒内，Nextcloud 每2秒保留一个版本
* 前一分钟，Nextcloud 每10秒保留一个版本
* 在开始的一个小时里，Nextcloud 每分钟保留一个版本
* 在开始的24小时内，Nextcloud 每小时保存一个版本
* 在开始的30天里，Nextcloud 每天都保留一个版本
* 在前30天之后，Nextcloud 每周都会保留一个版本

The versions are adjusted along this pattern every time a new version gets
created.

每次创建新版本时，版本都会按照这个模式进行调整。

The version app never uses more that 50% of the user's currently available free
space. If the stored versions exceed this limit, Nextcloud deletes the oldest
versions until it meets the disk space limit again.

这个版本控制应用从来不会使用超过 50% 的用户当前可用的空闲空间。如果存储的版本超过此限制，Nextcloud 将删除最早的版本，直到它再次满足磁盘空间限制。
