# laravel-admin 通用后台系统

#### laravel-admin v2.0版本，基于laravel优雅风格的特性，以及服务设计模式，已重构，考虑到laravel的优雅灵活性，去除了1.0版本中的代码生成功能。

git clone https://github.com/moho110/laravel-admin-2.0


## laravel-admin安装

#### 运行环境
```
php7.4版本
```

#### clone 项目到本地
```
GitHub:   git clone git@github.com:moho110/laravel-admin.git
```
或
```
码云:   git clone git@gitee.com:moho110/laravel-admin.git
```

#### 安装项目依赖
```
composer install
```

#### 配置数据库
```
更改 `.env` 文件内的数据库配置选项,数据库编码推荐`utf8mb4`。
```

#### 运行数据库迁移
```
php artisan migrate
``` 
#### 菜单生成数据填充
```
php artisan db:seed
``` 
#### 公共磁盘创建
```
php artisan storage:link

如果是docker容器部署,则需要到nginx容器中,手动创建软连接：
例如: ln -s /usr/share/nginx/html/temp/laravel-admin-temp/storage/app/public/ /usr/share/nginx/html/temp/laravel-admin-temp/public/storage
``` 

#### 最后一步，别忘了把项目设置为程序运行用户哟
```
例如我的程序运行用户是www用户:  chown -R www:www ./laravel-admin/
``` 

#### 服务器配置
可参考[Laravel 7 安装配置](https://learnku.com/docs/laravel/7.x/installation/7447)

#### Docker容器部署
可参考[docker-lnmp环境部署](https://github.com/yuxingfei/docker-lnmp)

#### 访问后台
访问`/admin`，默认超级管理员的账号密码都为`super_admin`。
