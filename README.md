# phpredis-from-php5.4


RHEL 7 用の EPEL リリースパッケージをインストールし、EPEL リポジトリを有効にします。

sudo amazon-linux-extras install epel -y

このリポジトリを有効にする

sudo yum-config-manager --enable epel

yum -y install php-pecl-redis --enablerepo=epel

確認

yum list installed | grep php*

redis.soの確認

ll /usr/lib64/php/modules/

php.iniにredis.soを追加

extension=redis.so







