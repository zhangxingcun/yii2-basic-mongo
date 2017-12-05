以 yii2 basic为基础搭建项目基础:包括权限管理,用户,mongodb

1)下载
composer create-project zhangxingcun/yii2-basic-mongo:dev-master

2)配置参数
权限管理可以用mongodb也可以用文件,默认用mongodb
**管理员权限默认开放,增加完超级用户后,记得关闭**

3)运行php yii init/user  增加超级用户

4)配置完超级用户,关闭管理员权限web.php
//'admin/*', // add or remove allowed actions to this list


说明:用户和权限管理没有挂接,先增加用户,再配置权限
