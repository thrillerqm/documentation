============================
Large file uploads 大文件上传
============================

When uploading files through the web client, Nextcloud is limited by PHP and
Apache configurations. By default, PHP is configured for only 2 megabyte
uploads. As this default upload limit is not entirely useful, we recommend that
your Nextcloud admin increase the Nextcloud variables to sizes appropriate for
users.

当通过 web 客户端上传文件时，Nextcloud 受到 PHP 和 Apache 配置的限制。
默认情况下，PHP 只配置为2MB的上传大小。
由于这个默认的上传限制并不完全够用，我们建议您的 Nextcloud 管理员将 Nextcloud 变量增加到适合用户的大小。



Modifying certain Nextcloud variables requires administrative access. If you
require larger upload limits than have been provided by the default (or already
set by your administrator):

修改某些 Nextcloud 变量需要管理员访问权限。如果您需要比默认设置(或管理员已经设置)更大的上传限制:

* Contact your administrator to request an increase in these variables

* Refer to the section in the `Admin Documentation
  <https://docs.nextcloud.org/server/latest/admin_manual/configuration_files/
  big_file_upload_configuration.html>`_ that describes how to manage file
  upload size limits.
  
* 请与管理员联系，请求增加这些变量的大小

* 参见 `Admin Documentation
  <https://docs.nextcloud.org/server/latest/admin_manual/configuration_files/
  big_file_upload_configuration.html>`_ ，该部分描述如何管理文件上传大小限制。

.. TODO ON RELEASE: Update version number above on release
