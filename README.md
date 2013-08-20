所為何來
=
於 Ubuntu 上安裝 Drush 命令列工具後，便能於終端機中直接進行 Drupal 的安裝與管理，替代部分網頁介面的操作需求。


使用環境
=
Ubuntu 12.04 Server  
Drush 5.9


推薦安裝方式
=
於終端機中，輸入以下指令來安裝 Drush 及 PHP-GD Graphics Library，並更新 Drush：
```bash
sudo aptitude install drush php5-gd && 
sudo drush dl drush --destination='/usr/share'
```
DONE.
<br>
<br>

補充說明
=
* Ubuntu 12.04 預設是安裝 Drush 4.5，但官方建議使用 5.6 以上的版本，故請務必進行更新。
* 欲查詢所安裝的 Drush 版本，可使用：<code>drush --version</code>
* 日後要更新 Drush 時，使用 <code>sudo drush dl drush --destination='/usr/share'</code> 即可。
* PHP-GD Graphics Library

參考資源
=
* [Drush | drupal.org](https://drupal.org/project/drush)
* [Drush.org](http://www.drush.org/)
* [Installing/Upgrading Drush on Ubuntu | drupal.org](https://drupal.org/node/1248790)
