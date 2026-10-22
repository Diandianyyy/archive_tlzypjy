# TL 回收站源备份

上游：https://tlzypjy.github.io/jb-repo/

添加到 Cydia、Sileo、Zebra：https://diandianyyy.github.io/archive_tlzypjy/

每 6 小时检查更新，保留已备份的历史版本，按 SHA256 去重。
下载后校验 SHA256、大小和 dpkg-deb 格式；坏包跳过并记录到 bad-packages.log，下次运行重试。
索引下载失败或发布失败会使任务失败，不会冒充同步成功。

可在 Actions 手动运行同步；摘要显示本轮成功及跳过数量。
