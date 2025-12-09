<!DOCTYPE html>
<html xmlns="http://www.w3.org/1999/xhtml" lang="" xml:lang="">
<head>
  <meta charset="utf-8" />
  <meta name="generator" content="pandoc" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0, user-scalable=yes" />
  <title>SMB Patches to Be Reviewed</title>
  <style>
    code{white-space: pre-wrap;}
    span.smallcaps{font-variant: small-caps;}
    span.underline{text-decoration: underline;}
    div.column{display: inline-block; vertical-align: top; width: 50%;}
    div.hanging-indent{margin-left: 1.5em; text-indent: -1.5em;}
    ul.task-list{list-style: none;}
  </style>
  <link rel="stylesheet" href="https://chenxiaosong.com/stylesheet.css" />
</head>
<body>
<header id="title-block-header">
<ul>
<li>Author: 陈孝松 (ChenXiaoSong)</li>
<li><a href="https://chenxiaosong.com/">Chinese Homepage: chenxiaosong.com</a></li>
<li><a href="https://chenxiaosong.com/en/">English Homepage: chenxiaosong.com/en</a></li>
<li>Email: <a href="mailto:chenxiaosong@chenxiaosong.com" class="email">chenxiaosong@chenxiaosong.com</a></li>
</ul>
<h1 class="title">SMB Patches to Be Reviewed</h1>
</header>
<nav id="TOC" role="doc-toc">
<ul>
<li><a href="#safest-patches-for-6.19-rc1"><span class="toc-section-number">1</span> “Safest” Patches for 6.19-rc1</a></li>
<li><a href="#patches-to-be-reviewed"><span class="toc-section-number">2</span> Patches to Be Reviewed</a></li>
<li><a href="#patches-applied-to-cifs-2.6.git-for-next"><span class="toc-section-number">3</span> Patches Applied to cifs-2.6.git for-next</a></li>
</ul>
</nav>
<h1 data-number="1" id="safest-patches-for-6.19-rc1"><span class="header-section-number">1</span> “Safest” Patches for 6.19-rc1</h1>
<p><a href="https://github.com/chenxiaosonggithub/tmp/tree/master/gnu-linux/smb/patch/safest">Click here to see the patches on GitHub that I consider the “safest” and suitable as targets for 6.19-rc1.</a>(Conflicts have been resolved).</p>
<ul>
<li>[PATCH v4 00/10] smb: improve search speed of SMB2 maperror
<ul>
<li>[PATCH v4 10/10] smb/server: rename include guard in smb_common.h</li>
</ul></li>
<li>[PATCH 00/30] smb: improve search speed of SMB1 maperror
<ul>
<li>[PATCH 01/30] smb/client: fix NT_STATUS_NO_DATA_DETECTED value</li>
<li>[PATCH 02/30] smb/client: fix NT_STATUS_DEVICE_DOOR_OPEN value</li>
<li>[PATCH 03/30] smb/client: fix NT_STATUS_UNABLE_TO_FREE_VM value</li>
<li>[PATCH 04/30] smb/server: remove unused nterr.h</li>
<li>[PATCH 05/30] smb/client: add 4 NT error code definitions</li>
<li>[PATCH 06/30] smb/client: add parentheses to NT error code definitions containing bitwise OR operator</li>
</ul></li>
<li>[PATCH 00/13] smb: move duplicate definitions into common header file, part 2
<ul>
<li>[PATCH 01/13] smb: add documentation references for smb2 change notify definitions</li>
<li>[PATCH 02/13] smb: move notify completion filter flags into common/smb2pdu.h</li>
<li>[PATCH 03/13] smb: move SMB2 Notify Action Flags into common/smb2pdu.h</li>
<li>[PATCH 04/13] smb: move file_notify_information to common/fscc.h</li>
<li>[PATCH 05/13] smb: move File Attributes definitions into common/fscc.h</li>
<li>[PATCH 06/13] smb: update struct duplicate_extents_to_file_ex</li>
<li>[PATCH 07/13] smb/server: add comment to FileSystemName of FileFsAttributeInformation</li>
<li>[PATCH 10/13] smb/client: remove DeviceType Flags and Device Characteristics definitions</li>
<li>[PATCH 13/13] smb: move some SMB1 definitions into common/smb1pdu.h</li>
</ul></li>
</ul>
<h1 data-number="2" id="patches-to-be-reviewed"><span class="header-section-number">2</span> Patches to Be Reviewed</h1>
<p>Besides the patches above that are the “safest” and suitable for 6.19-rc1, the other patches to be reviewed on GitHub are as follows:</p>
<ul>
<li><a href="https://github.com/chenxiaosonggithub/tmp/tree/master/gnu-linux/smb/patch/smb2maperror">[PATCH v4 00/10] smb: improve search speed of SMB2 maperror</a>
<ul>
<li>#0005 ~ #0008</li>
</ul></li>
<li><a href="https://github.com/chenxiaosonggithub/tmp/tree/master/gnu-linux/smb/patch/smb1maperror">[PATCH 00/30] smb: improve search speed of SMB1 maperror</a>
<ul>
<li>#0007 ~ #0030</li>
</ul></li>
<li><a href="https://github.com/chenxiaosonggithub/tmp/tree/master/gnu-linux/smb/patch/remove-duplicate-definitions">[PATCH 00/13] smb: move duplicate definitions into common header file, part 2</a>
<ul>
<li>#0008, #0009, #0011, #0012</li>
</ul></li>
</ul>
<h1 data-number="3" id="patches-applied-to-cifs-2.6.git-for-next"><span class="header-section-number">3</span> Patches Applied to cifs-2.6.git for-next</h1>
<p>The following patches have been applied to <a href="https://git.samba.org/sfrench/?p=sfrench/cifs-2.6.git;a=shortlog;h=refs/heads/for-next">cifs-2.6.git for-next</a>:</p>
<ul>
<li>smb/client: update some SMB2 status strings</li>
<li>smb/client: add two elements to smb2_error_map_table array</li>
<li>smb: rename to STATUS_SMB_NO_PREAUTH_INTEGRITY_HASH_OVERLAP</li>
<li>smb/client: remove unused elements from smb2_error_map_table array</li>
<li>smb/client: reduce loop count in map_smb2_to_linux_error() by half</li>
</ul>
</body>
</html>
