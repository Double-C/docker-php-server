# docker-php-server

由于之前都是用的 homestead 来做本地开发环境，安装php扩展过于麻烦，再接着是启动慢

于是改为使用 docker 定制属于自己的本地开发环境

主要包括

* php
  * pdo_mysql
  * pdo_sqlsrv
  * sqlsrv
  * swoole
  * redis
* mysql
* redis
* nginx

> 由于公司还有很多老项目在使用 mssql，所以还要装相关扩展  T . T

docker可以随时更新对应服务版本，启动又快，真香！

体验真的是完爆以前的虚拟机。