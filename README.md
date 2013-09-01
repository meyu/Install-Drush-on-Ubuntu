所為何來
=
於 Ubuntu 上安裝 Drush 命令列工具後，便能於終端機中直接進行 Drupal 的安裝與管理，替代部分網頁介面的操作需求。
   
   
使用環境
=
Ubuntu 12.04 Server  
Drush 6.0
   

推薦安裝方式
=
請先確保主機可使用 PEAR 套裝函式庫，並載入 Drush 的安裝頻道：
```bash
sudo apt-get install php-pear && 
sudo pear channel-discover pear.drush.org 
```
安裝 Drush 及 PHP-GD Graphics Library，並更新 Drush：
```bash
sudo apt-get install drush php5-gd && 
sudo pear install drush/drush
```
   
DONE.
<br>
<br>

補充說明
=
* Ubuntu 12.04 預設是安裝 Drush 4.5，但官方建議使用 5.6 以上的版本，故請務必進行更新。
* 欲查詢所安裝的 Drush 版本，可使用：<code>drush --version</code>
* 日後要更新 Drush 時，使用 <code>sudo pear install drush/drush</code> 即可。
* PHP-GD Graphics Library 為一圖像工具，亦為 Drush 在架設 Drupal 網站時的需求套件之一，故建議一併安裝。
   
參考資源
=
* [Drush | drupal.org](https://drupal.org/project/drush)
* [Drush.org](http://www.drush.org/)
* [drush-ops/drush](https://github.com/drush-ops/drush)
* [Installing/Upgrading Drush on Ubuntu | drupal.org](https://drupal.org/node/1248790)
* [How to Install Drush on a Cloud Server Running Ubuntu 12.04 | DigitalOcean](https://www.digitalocean.com/community/articles/how-to-install-drush-on-a-cloud-server-running-ubuntu-12-04)
