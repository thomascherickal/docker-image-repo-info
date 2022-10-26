<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `php-zendserver`

-	[`php-zendserver:2019.0`](#php-zendserver20190)
-	[`php-zendserver:2021.0`](#php-zendserver20210)
-	[`php-zendserver:5.6`](#php-zendserver56)
-	[`php-zendserver:8.5`](#php-zendserver85)
-	[`php-zendserver:8.5-php5.6`](#php-zendserver85-php56)
-	[`php-zendserver:9.1`](#php-zendserver91)
-	[`php-zendserver:latest`](#php-zendserverlatest)

## `php-zendserver:2019.0`

```console
$ docker pull php-zendserver@sha256:408c6fcbe87de8e5f6d7b518cb0f4df0e1e25dfec2698047cf6c6c57df8a11af
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `php-zendserver:2019.0` - linux; amd64

```console
$ docker pull php-zendserver@sha256:c8e5e21d98feffe68d7ae15afaad59f1a55a1f53038345a66efdb78e198b6428
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **486.9 MB (486862018 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b8578bdb85e7de3dad36622433c1f8bad252b7bfd11f0e2be9c1989856f0cfe`
-	Default Command: `["\/usr\/local\/bin\/run"]`

```dockerfile
# Tue, 25 Oct 2022 01:53:28 GMT
ADD file:fc5d658c47ede58827812b75a311353be776e41e2dd339b8906839527c9b5247 in / 
# Tue, 25 Oct 2022 01:53:28 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 17:19:21 GMT
RUN apt-get update && apt-get install -y       gnupg
# Tue, 25 Oct 2022 17:19:22 GMT
RUN apt-key adv --keyserver keyserver.ubuntu.com --recv-key 799058698E65316A2E7A4FF42EAE1437F7D2C623
# Tue, 25 Oct 2022 17:19:23 GMT
COPY file:23f8c2a96f087277b95ebfd7f401f5c1b95ec7f3443fa9231607566f1d8e7270 in /etc/apt/sources.list.d/zend-server.list 
# Tue, 25 Oct 2022 17:21:09 GMT
RUN apt-get update && apt-get install -y       iproute2       curl       libmysqlclient20       unzip       git       zend-server-nginx=2019.0.7+b403     && rm -rf /var/lib/apt/lists/*     && /usr/local/zend/bin/zendctl.sh stop
# Tue, 25 Oct 2022 17:21:13 GMT
ENV ZS_INIT_VERSION=0.3
# Tue, 25 Oct 2022 17:21:13 GMT
ENV ZS_INIT_SHA256=e8d441d8503808e9fc0fafc762b2cb80d4a6e68b94fede0fe41efdeac10800cb
# Tue, 25 Oct 2022 17:21:13 GMT
COPY file:ad21ce0b2dc8345be0ef63836774934d6b2045ddc3685411221a07dd10b649d1 in /tmp/zs-init.patch 
# Tue, 25 Oct 2022 17:21:14 GMT
RUN curl -fSL -o zs-init.tar.gz "http://repos.zend.com/zs-init/zs-init-docker-${ZS_INIT_VERSION}.tar.gz"     && echo "${ZS_INIT_SHA256} *zs-init.tar.gz" | sha256sum -c -     && mkdir /usr/local/zs-init     && tar xzf zs-init.tar.gz --strip-components=1 -C /usr/local/zs-init     && rm zs-init.tar.gz     && patch -u /usr/local/zs-init/src/Init/Steps/AbstractStep.php -i /tmp/zs-init.patch     && rm /tmp/zs-init.patch
# Tue, 25 Oct 2022 17:21:14 GMT
WORKDIR /usr/local/zs-init
# Tue, 25 Oct 2022 17:21:19 GMT
RUN /usr/local/zend/bin/php -r "readfile('https://getcomposer.org/installer');" | /usr/local/zend/bin/php     && /usr/local/zend/bin/php composer.phar update
# Tue, 25 Oct 2022 17:21:20 GMT
COPY dir:eecd98e9ebf1c61a12ae67558eb2a6ce846b9ebfadabbf08503e90b3e30d9496 in /usr/local/bin 
# Tue, 25 Oct 2022 17:21:20 GMT
COPY dir:80bde0d50316e7c9350262fe3b75826a91d075303027787e759d703b60df13d6 in /usr/local/zend/var/plugins/ 
# Tue, 25 Oct 2022 17:21:20 GMT
RUN rm /var/www/html/index.nginx-debian.html
# Tue, 25 Oct 2022 17:21:21 GMT
COPY dir:d174a5d34625889b4356c566972566e0ca7da618b01ea42276562f8186517a67 in /var/www/html 
# Tue, 25 Oct 2022 17:21:21 GMT
EXPOSE 80
# Tue, 25 Oct 2022 17:21:21 GMT
EXPOSE 443
# Tue, 25 Oct 2022 17:21:21 GMT
EXPOSE 10081
# Tue, 25 Oct 2022 17:21:21 GMT
EXPOSE 10082
# Tue, 25 Oct 2022 17:21:21 GMT
WORKDIR /var/www/html
# Tue, 25 Oct 2022 17:21:21 GMT
CMD ["/usr/local/bin/run"]
```

-	Layers:
	-	`sha256:a404e54162968593b8d92b571f3cdd673e4c9eab5d9be28d7c494595c0aa6682`  
		Last Modified: Wed, 19 Oct 2022 22:03:02 GMT  
		Size: 26.7 MB (26712500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fbb3fae8f00f5b0fb4cf5a677d7131fad36431423e10e2c243ce245cfb22808`  
		Last Modified: Wed, 26 Oct 2022 15:47:38 GMT  
		Size: 36.7 MB (36676854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfef197f4322d6a3bde0d88fdf96a99f095d982900906520ae117a39f658a0c3`  
		Last Modified: Wed, 26 Oct 2022 15:47:34 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dceb556d3c3fd0e6af78dcbc65bdc9f7412be26940c713e30d8b51a3d66521e`  
		Last Modified: Wed, 26 Oct 2022 15:47:33 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb8686314f0a0d425a096e91268709de89132e79b1bcce3c8d977581a3f015a2`  
		Last Modified: Wed, 26 Oct 2022 15:48:36 GMT  
		Size: 418.1 MB (418118157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd78ce86c18f55f7a5fc2d1218d1388d1a00e39fbba3a1b31748a0777988f776`  
		Last Modified: Tue, 25 Oct 2022 17:24:35 GMT  
		Size: 446.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:985510284fa5ce11b26d7c15077afa4938b2b92d49efbe768123fb3d2229e568`  
		Last Modified: Tue, 25 Oct 2022 17:23:56 GMT  
		Size: 18.9 KB (18929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd9f8c743e9f056678aefd74d0aa94ff5f1daa7e072fa0f338510562a5b5e63f`  
		Last Modified: Tue, 25 Oct 2022 17:23:37 GMT  
		Size: 5.3 MB (5315208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e80ec5e4ffa3f6a5816478a3cd44e6919805d22aa439e4b85109957afba9c3c`  
		Last Modified: Tue, 25 Oct 2022 17:23:36 GMT  
		Size: 14.3 KB (14294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d66c9007e6deefe0bb5df8d4d8e55a10880ed52c5c5c8a22d31baeca07a5b3e7`  
		Last Modified: Tue, 25 Oct 2022 17:23:36 GMT  
		Size: 2.6 KB (2559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9439f9756c4c8ceab379f46baea3b47134e88a8e03c637e80892331f1e5a5fd`  
		Last Modified: Tue, 25 Oct 2022 17:23:36 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:397a32ccf9d44a07f1d0ff06fd2a8ac7a9fa6ebc87e5357553347b2ddbceb833`  
		Last Modified: Tue, 25 Oct 2022 17:23:36 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `php-zendserver:2021.0`

```console
$ docker pull php-zendserver@sha256:882235663fae8f55986e7666a1caeaba4841a1a385f2647f91cf288e6d358095
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `php-zendserver:2021.0` - linux; amd64

```console
$ docker pull php-zendserver@sha256:38c703709692c1f2a37518dc3f6ad9cb5f59dab6aa39b7f3c72fe7b51dd9bf21
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **394.8 MB (394750601 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fcc5df54322f7d81a8081f5a073a650fd506da09c6b29e526e927f7d04b3baf3`
-	Default Command: `["\/usr\/local\/bin\/run"]`

```dockerfile
# Tue, 25 Oct 2022 01:53:28 GMT
ADD file:fc5d658c47ede58827812b75a311353be776e41e2dd339b8906839527c9b5247 in / 
# Tue, 25 Oct 2022 01:53:28 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 17:19:21 GMT
RUN apt-get update && apt-get install -y       gnupg
# Tue, 25 Oct 2022 17:19:22 GMT
RUN apt-key adv --keyserver keyserver.ubuntu.com --recv-key 799058698E65316A2E7A4FF42EAE1437F7D2C623
# Tue, 25 Oct 2022 17:21:29 GMT
COPY file:1e70d8fd6f9643bffb703528edddba0aa02a58e95cc53e92f58a86cde29e732a in /etc/apt/sources.list.d/zend-server.list 
# Tue, 25 Oct 2022 17:23:03 GMT
RUN apt-get update && apt-get install -y       iproute2       curl       libmysqlclient20       unzip       git       zend-server-nginx=2021.0.0+b74     && rm -rf /var/lib/apt/lists/*     && /usr/local/zend/bin/zendctl.sh stop
# Tue, 25 Oct 2022 17:23:06 GMT
ENV ZS_INIT_VERSION=0.3
# Tue, 25 Oct 2022 17:23:06 GMT
ENV ZS_INIT_SHA256=e8d441d8503808e9fc0fafc762b2cb80d4a6e68b94fede0fe41efdeac10800cb
# Tue, 25 Oct 2022 17:23:06 GMT
COPY file:ad21ce0b2dc8345be0ef63836774934d6b2045ddc3685411221a07dd10b649d1 in /tmp/zs-init.patch 
# Tue, 25 Oct 2022 17:23:08 GMT
RUN curl -fSL -o zs-init.tar.gz "http://repos.zend.com/zs-init/zs-init-docker-${ZS_INIT_VERSION}.tar.gz"     && echo "${ZS_INIT_SHA256} *zs-init.tar.gz" | sha256sum -c -     && mkdir /usr/local/zs-init     && tar xzf zs-init.tar.gz --strip-components=1 -C /usr/local/zs-init     && rm zs-init.tar.gz     && patch -u /usr/local/zs-init/src/Init/Steps/AbstractStep.php -i /tmp/zs-init.patch     && rm /tmp/zs-init.patch
# Tue, 25 Oct 2022 17:23:08 GMT
WORKDIR /usr/local/zs-init
# Tue, 25 Oct 2022 17:23:13 GMT
RUN /usr/local/zend/bin/php -r "readfile('https://getcomposer.org/installer');" | /usr/local/zend/bin/php     && /usr/local/zend/bin/php composer.phar update
# Tue, 25 Oct 2022 17:23:14 GMT
COPY dir:eecd98e9ebf1c61a12ae67558eb2a6ce846b9ebfadabbf08503e90b3e30d9496 in /usr/local/bin 
# Tue, 25 Oct 2022 17:23:14 GMT
COPY dir:80bde0d50316e7c9350262fe3b75826a91d075303027787e759d703b60df13d6 in /usr/local/zend/var/plugins/ 
# Tue, 25 Oct 2022 17:23:14 GMT
RUN rm /var/www/html/index.nginx-debian.html
# Tue, 25 Oct 2022 17:23:14 GMT
COPY dir:d174a5d34625889b4356c566972566e0ca7da618b01ea42276562f8186517a67 in /var/www/html 
# Tue, 25 Oct 2022 17:23:14 GMT
EXPOSE 80
# Tue, 25 Oct 2022 17:23:15 GMT
EXPOSE 443
# Tue, 25 Oct 2022 17:23:15 GMT
EXPOSE 10081
# Tue, 25 Oct 2022 17:23:15 GMT
EXPOSE 10082
# Tue, 25 Oct 2022 17:23:15 GMT
WORKDIR /var/www/html
# Tue, 25 Oct 2022 17:23:15 GMT
CMD ["/usr/local/bin/run"]
```

-	Layers:
	-	`sha256:a404e54162968593b8d92b571f3cdd673e4c9eab5d9be28d7c494595c0aa6682`  
		Last Modified: Wed, 19 Oct 2022 22:03:02 GMT  
		Size: 26.7 MB (26712500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fbb3fae8f00f5b0fb4cf5a677d7131fad36431423e10e2c243ce245cfb22808`  
		Last Modified: Wed, 26 Oct 2022 15:47:38 GMT  
		Size: 36.7 MB (36676854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfef197f4322d6a3bde0d88fdf96a99f095d982900906520ae117a39f658a0c3`  
		Last Modified: Wed, 26 Oct 2022 15:47:34 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8ee2927be8bc9d8db274aa85650c006f8ec987d85aa3dd85e3278da02144502`  
		Last Modified: Wed, 26 Oct 2022 15:48:50 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07fbe6b63324df1effc044b8e838ae9c928632a765c2d3efa5d380786f324ab0`  
		Last Modified: Wed, 26 Oct 2022 15:49:43 GMT  
		Size: 326.0 MB (326006802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26925d52cd07bde840512fa2026ea1e75ebbd5abd2fe22673ab9773e6ac63328`  
		Last Modified: Wed, 26 Oct 2022 15:48:50 GMT  
		Size: 446.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37c8d761f31ae9946acc1bcdd2fa95e12095724f83117d222140f91ec007bf9f`  
		Last Modified: Wed, 26 Oct 2022 15:48:50 GMT  
		Size: 18.9 KB (18926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00d53c3a35228079dcfe72aa875a6b69de67b6a86050b3a0449330cbb33f785b`  
		Last Modified: Wed, 26 Oct 2022 15:48:50 GMT  
		Size: 5.3 MB (5315156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1054edbca2de70c30f494fde04969dfe94ea2c415a5727391357f26f973fe18b`  
		Last Modified: Wed, 26 Oct 2022 15:48:48 GMT  
		Size: 14.3 KB (14293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24bf534882f3d908757d2f91a520575226f452bebb5567c0f8b7b7f61850ec3f`  
		Last Modified: Wed, 26 Oct 2022 15:48:48 GMT  
		Size: 2.6 KB (2558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:442235a0cc8ddeec20cc48b51ac49181891e510211e0b1f3ac739b7fcd2485e8`  
		Last Modified: Wed, 26 Oct 2022 15:48:48 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff3ee1cceacb8560da402eb62ea8c3bc49e67a6489817e12f24f84d7c73beca2`  
		Last Modified: Wed, 26 Oct 2022 15:48:48 GMT  
		Size: 1.3 KB (1255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `php-zendserver:5.6`

```console
$ docker pull php-zendserver@sha256:46087476dd829477b235937b1b774e539c67177fb9c637bde91b28b2e6cf9299
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `php-zendserver:5.6` - linux; amd64

```console
$ docker pull php-zendserver@sha256:5393691a9d8617643c002a7ec19c90639a480868ae335ab538499d1a05865d4d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **315.6 MB (315608578 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:513ed7b8cb626435a0c10f51c07b1631f83e70f06549e79357644c19c6d30670`
-	Default Command: `["\/usr\/local\/bin\/run"]`

```dockerfile
# Tue, 31 Aug 2021 01:21:27 GMT
ADD file:11b425d4c08e81a3e0cb2e0345d27cd5fc844dd83f1096af4cc05f635824ff5d in / 
# Tue, 31 Aug 2021 01:21:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 31 Aug 2021 01:21:29 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 01:21:30 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 31 Aug 2021 01:21:30 GMT
CMD ["/bin/bash"]
# Tue, 31 Aug 2021 04:02:14 GMT
RUN apt-key adv --keyserver keyserver.ubuntu.com --recv-key 799058698E65316A2E7A4FF42EAE1437F7D2C623
# Tue, 31 Aug 2021 04:02:15 GMT
COPY file:6f0a5450842ae9c3e06d131c7180961d773ca33754e17af8ea2ac258fd0c6054 in /etc/apt/sources.list.d/zend-server.list 
# Tue, 31 Aug 2021 04:02:15 GMT
COPY file:7a9d81c6298f71cfad4408c8b3d7c3bf53bf90083221ec55686e12b2eb6f16a4 in /etc/apt/sources.list.d/ubuntu-trusty.list 
# Tue, 31 Aug 2021 04:04:03 GMT
RUN apt-get update     && apt-get install -y         curl         libmysqlclient18         unzip         git         zend-server-php-5.6=8.5.17+b19     && rm -rf /var/lib/apt/lists/*     && /usr/local/zend/bin/zendctl.sh stop
# Tue, 31 Aug 2021 04:04:06 GMT
COPY file:def46bbc651bcb61f92bcaa2f8d6edec0c22e51e86132fabd2e47542dcbec0bf in /etc/apache2/conf-available 
# Tue, 31 Aug 2021 04:04:06 GMT
RUN /usr/sbin/a2enconf drop-http-proxy-header
# Tue, 31 Aug 2021 04:04:07 GMT
RUN /usr/sbin/a2enmod headers
# Tue, 31 Aug 2021 04:04:07 GMT
ENV ZS_INIT_VERSION=0.3
# Tue, 31 Aug 2021 04:04:08 GMT
ENV ZS_INIT_SHA256=e8d441d8503808e9fc0fafc762b2cb80d4a6e68b94fede0fe41efdeac10800cb
# Tue, 31 Aug 2021 04:04:09 GMT
RUN curl -fSL -o zs-init.tar.gz "http://repos.zend.com/zs-init/zs-init-docker-${ZS_INIT_VERSION}.tar.gz"     && echo "${ZS_INIT_SHA256} *zs-init.tar.gz" | sha256sum -c -     && mkdir /usr/local/zs-init     && tar xzf zs-init.tar.gz --strip-components=1 -C /usr/local/zs-init     && rm zs-init.tar.gz
# Tue, 31 Aug 2021 04:04:09 GMT
WORKDIR /usr/local/zs-init
# Tue, 31 Aug 2021 04:04:16 GMT
RUN /usr/local/zend/bin/php -r "readfile('https://getcomposer.org/installer');" | /usr/local/zend/bin/php     && /usr/local/zend/bin/php composer.phar self-update && /usr/local/zend/bin/php composer.phar update
# Tue, 31 Aug 2021 04:04:16 GMT
COPY dir:b75978d6e77900379bb898c52c86c408d7f6fcd06b5c66439d594a1a3dcca0b4 in /usr/local/bin 
# Tue, 31 Aug 2021 04:04:16 GMT
COPY dir:80bde0d50316e7c9350262fe3b75826a91d075303027787e759d703b60df13d6 in /usr/local/zend/var/plugins/ 
# Tue, 31 Aug 2021 04:04:17 GMT
RUN rm /var/www/html/index.html
# Tue, 31 Aug 2021 04:04:17 GMT
COPY dir:d174a5d34625889b4356c566972566e0ca7da618b01ea42276562f8186517a67 in /var/www/html 
# Tue, 31 Aug 2021 04:04:17 GMT
EXPOSE 80
# Tue, 31 Aug 2021 04:04:18 GMT
EXPOSE 443
# Tue, 31 Aug 2021 04:04:18 GMT
EXPOSE 10081
# Tue, 31 Aug 2021 04:04:18 GMT
EXPOSE 10082
# Tue, 31 Aug 2021 04:04:18 GMT
WORKDIR /var/www/html
# Tue, 31 Aug 2021 04:04:18 GMT
CMD ["/usr/local/bin/run"]
```

-	Layers:
	-	`sha256:58690f9b18fca6469a14da4e212c96849469f9b1be6661d2342a4bf01774aa50`  
		Last Modified: Thu, 05 Aug 2021 00:25:05 GMT  
		Size: 46.5 MB (46497548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b51569e7c50720acf6860327847fe342a1afbe148d24c529fb81df105e3eed01`  
		Last Modified: Tue, 31 Aug 2021 01:23:09 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da8ef40b9ecabc2679fe2419957220c0272a965c5cf7e0269fa1aeeb8c56f2e1`  
		Last Modified: Tue, 31 Aug 2021 01:23:08 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb15d46c38dcd1ea0b1990006c3366ecd10c79d374f341687eb2cb23a2c8672e`  
		Last Modified: Tue, 31 Aug 2021 01:23:08 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2102dd9376f61b14df18139d78a96caeb38426131bb6a85847a5733f84d83c32`  
		Last Modified: Tue, 31 Aug 2021 04:11:12 GMT  
		Size: 14.7 KB (14704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae050479344fbb7ea0f86b97e8c772b7ae45103fa5cfc2bea2a4b79c631a1534`  
		Last Modified: Tue, 31 Aug 2021 04:11:11 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7d990e63418cea6828a1754a0cfd88662fe780fa88dd2de23528d624ab6bc35`  
		Last Modified: Tue, 31 Aug 2021 04:11:11 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e78264dffd8afd8084e307db7cfd44f971f55d76534559ccd72b50b64108726`  
		Last Modified: Tue, 31 Aug 2021 04:11:40 GMT  
		Size: 263.9 MB (263910611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd783101a133a035071fca065237130e373e2f4cc4151957c9c461ae9a79cdf2`  
		Last Modified: Tue, 31 Aug 2021 04:11:09 GMT  
		Size: 263.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d19cbd07b1b667393092b9d2df1833f0b331cfe1eb5e6ad304f4acbda03136ab`  
		Last Modified: Tue, 31 Aug 2021 04:11:09 GMT  
		Size: 336.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c21aeee9b83798ca4fd42d7e5aa46ecd288c027160673f1be4f3d9d57b70a383`  
		Last Modified: Tue, 31 Aug 2021 04:11:09 GMT  
		Size: 307.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf7e05a640abfb3d3865705d1a482da844acc818d5c32089ee78ec8ba477136d`  
		Last Modified: Tue, 31 Aug 2021 04:11:09 GMT  
		Size: 18.9 KB (18859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be58af708ccc85c876f8148b3f7af699d37b1d23a25d76c1c8eaedd03b6dcc9b`  
		Last Modified: Tue, 31 Aug 2021 04:11:08 GMT  
		Size: 5.1 MB (5146536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb1df10206b55b2eb8839919bb0d056e7256e1dd2bb398a492c5b8317235fe6d`  
		Last Modified: Tue, 31 Aug 2021 04:11:07 GMT  
		Size: 13.4 KB (13357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:703d37b5f26f094cbc47c55b9abf4e3fe103e96208d7e102c579384ffe6add64`  
		Last Modified: Tue, 31 Aug 2021 04:11:06 GMT  
		Size: 2.6 KB (2566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15716512d8f97648b13d29fdbc7df5b8f6ec04e2ca06aa9447b31525f08c1c2c`  
		Last Modified: Tue, 31 Aug 2021 04:11:06 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b72ae8545d8a1d76de6aadb8a94a839c2d60e2f164e0323e0ad4cc73a1853110`  
		Last Modified: Tue, 31 Aug 2021 04:11:06 GMT  
		Size: 1.2 KB (1250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `php-zendserver:8.5`

```console
$ docker pull php-zendserver@sha256:46087476dd829477b235937b1b774e539c67177fb9c637bde91b28b2e6cf9299
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `php-zendserver:8.5` - linux; amd64

```console
$ docker pull php-zendserver@sha256:5393691a9d8617643c002a7ec19c90639a480868ae335ab538499d1a05865d4d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **315.6 MB (315608578 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:513ed7b8cb626435a0c10f51c07b1631f83e70f06549e79357644c19c6d30670`
-	Default Command: `["\/usr\/local\/bin\/run"]`

```dockerfile
# Tue, 31 Aug 2021 01:21:27 GMT
ADD file:11b425d4c08e81a3e0cb2e0345d27cd5fc844dd83f1096af4cc05f635824ff5d in / 
# Tue, 31 Aug 2021 01:21:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 31 Aug 2021 01:21:29 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 01:21:30 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 31 Aug 2021 01:21:30 GMT
CMD ["/bin/bash"]
# Tue, 31 Aug 2021 04:02:14 GMT
RUN apt-key adv --keyserver keyserver.ubuntu.com --recv-key 799058698E65316A2E7A4FF42EAE1437F7D2C623
# Tue, 31 Aug 2021 04:02:15 GMT
COPY file:6f0a5450842ae9c3e06d131c7180961d773ca33754e17af8ea2ac258fd0c6054 in /etc/apt/sources.list.d/zend-server.list 
# Tue, 31 Aug 2021 04:02:15 GMT
COPY file:7a9d81c6298f71cfad4408c8b3d7c3bf53bf90083221ec55686e12b2eb6f16a4 in /etc/apt/sources.list.d/ubuntu-trusty.list 
# Tue, 31 Aug 2021 04:04:03 GMT
RUN apt-get update     && apt-get install -y         curl         libmysqlclient18         unzip         git         zend-server-php-5.6=8.5.17+b19     && rm -rf /var/lib/apt/lists/*     && /usr/local/zend/bin/zendctl.sh stop
# Tue, 31 Aug 2021 04:04:06 GMT
COPY file:def46bbc651bcb61f92bcaa2f8d6edec0c22e51e86132fabd2e47542dcbec0bf in /etc/apache2/conf-available 
# Tue, 31 Aug 2021 04:04:06 GMT
RUN /usr/sbin/a2enconf drop-http-proxy-header
# Tue, 31 Aug 2021 04:04:07 GMT
RUN /usr/sbin/a2enmod headers
# Tue, 31 Aug 2021 04:04:07 GMT
ENV ZS_INIT_VERSION=0.3
# Tue, 31 Aug 2021 04:04:08 GMT
ENV ZS_INIT_SHA256=e8d441d8503808e9fc0fafc762b2cb80d4a6e68b94fede0fe41efdeac10800cb
# Tue, 31 Aug 2021 04:04:09 GMT
RUN curl -fSL -o zs-init.tar.gz "http://repos.zend.com/zs-init/zs-init-docker-${ZS_INIT_VERSION}.tar.gz"     && echo "${ZS_INIT_SHA256} *zs-init.tar.gz" | sha256sum -c -     && mkdir /usr/local/zs-init     && tar xzf zs-init.tar.gz --strip-components=1 -C /usr/local/zs-init     && rm zs-init.tar.gz
# Tue, 31 Aug 2021 04:04:09 GMT
WORKDIR /usr/local/zs-init
# Tue, 31 Aug 2021 04:04:16 GMT
RUN /usr/local/zend/bin/php -r "readfile('https://getcomposer.org/installer');" | /usr/local/zend/bin/php     && /usr/local/zend/bin/php composer.phar self-update && /usr/local/zend/bin/php composer.phar update
# Tue, 31 Aug 2021 04:04:16 GMT
COPY dir:b75978d6e77900379bb898c52c86c408d7f6fcd06b5c66439d594a1a3dcca0b4 in /usr/local/bin 
# Tue, 31 Aug 2021 04:04:16 GMT
COPY dir:80bde0d50316e7c9350262fe3b75826a91d075303027787e759d703b60df13d6 in /usr/local/zend/var/plugins/ 
# Tue, 31 Aug 2021 04:04:17 GMT
RUN rm /var/www/html/index.html
# Tue, 31 Aug 2021 04:04:17 GMT
COPY dir:d174a5d34625889b4356c566972566e0ca7da618b01ea42276562f8186517a67 in /var/www/html 
# Tue, 31 Aug 2021 04:04:17 GMT
EXPOSE 80
# Tue, 31 Aug 2021 04:04:18 GMT
EXPOSE 443
# Tue, 31 Aug 2021 04:04:18 GMT
EXPOSE 10081
# Tue, 31 Aug 2021 04:04:18 GMT
EXPOSE 10082
# Tue, 31 Aug 2021 04:04:18 GMT
WORKDIR /var/www/html
# Tue, 31 Aug 2021 04:04:18 GMT
CMD ["/usr/local/bin/run"]
```

-	Layers:
	-	`sha256:58690f9b18fca6469a14da4e212c96849469f9b1be6661d2342a4bf01774aa50`  
		Last Modified: Thu, 05 Aug 2021 00:25:05 GMT  
		Size: 46.5 MB (46497548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b51569e7c50720acf6860327847fe342a1afbe148d24c529fb81df105e3eed01`  
		Last Modified: Tue, 31 Aug 2021 01:23:09 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da8ef40b9ecabc2679fe2419957220c0272a965c5cf7e0269fa1aeeb8c56f2e1`  
		Last Modified: Tue, 31 Aug 2021 01:23:08 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb15d46c38dcd1ea0b1990006c3366ecd10c79d374f341687eb2cb23a2c8672e`  
		Last Modified: Tue, 31 Aug 2021 01:23:08 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2102dd9376f61b14df18139d78a96caeb38426131bb6a85847a5733f84d83c32`  
		Last Modified: Tue, 31 Aug 2021 04:11:12 GMT  
		Size: 14.7 KB (14704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae050479344fbb7ea0f86b97e8c772b7ae45103fa5cfc2bea2a4b79c631a1534`  
		Last Modified: Tue, 31 Aug 2021 04:11:11 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7d990e63418cea6828a1754a0cfd88662fe780fa88dd2de23528d624ab6bc35`  
		Last Modified: Tue, 31 Aug 2021 04:11:11 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e78264dffd8afd8084e307db7cfd44f971f55d76534559ccd72b50b64108726`  
		Last Modified: Tue, 31 Aug 2021 04:11:40 GMT  
		Size: 263.9 MB (263910611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd783101a133a035071fca065237130e373e2f4cc4151957c9c461ae9a79cdf2`  
		Last Modified: Tue, 31 Aug 2021 04:11:09 GMT  
		Size: 263.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d19cbd07b1b667393092b9d2df1833f0b331cfe1eb5e6ad304f4acbda03136ab`  
		Last Modified: Tue, 31 Aug 2021 04:11:09 GMT  
		Size: 336.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c21aeee9b83798ca4fd42d7e5aa46ecd288c027160673f1be4f3d9d57b70a383`  
		Last Modified: Tue, 31 Aug 2021 04:11:09 GMT  
		Size: 307.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf7e05a640abfb3d3865705d1a482da844acc818d5c32089ee78ec8ba477136d`  
		Last Modified: Tue, 31 Aug 2021 04:11:09 GMT  
		Size: 18.9 KB (18859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be58af708ccc85c876f8148b3f7af699d37b1d23a25d76c1c8eaedd03b6dcc9b`  
		Last Modified: Tue, 31 Aug 2021 04:11:08 GMT  
		Size: 5.1 MB (5146536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb1df10206b55b2eb8839919bb0d056e7256e1dd2bb398a492c5b8317235fe6d`  
		Last Modified: Tue, 31 Aug 2021 04:11:07 GMT  
		Size: 13.4 KB (13357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:703d37b5f26f094cbc47c55b9abf4e3fe103e96208d7e102c579384ffe6add64`  
		Last Modified: Tue, 31 Aug 2021 04:11:06 GMT  
		Size: 2.6 KB (2566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15716512d8f97648b13d29fdbc7df5b8f6ec04e2ca06aa9447b31525f08c1c2c`  
		Last Modified: Tue, 31 Aug 2021 04:11:06 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b72ae8545d8a1d76de6aadb8a94a839c2d60e2f164e0323e0ad4cc73a1853110`  
		Last Modified: Tue, 31 Aug 2021 04:11:06 GMT  
		Size: 1.2 KB (1250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `php-zendserver:8.5-php5.6`

```console
$ docker pull php-zendserver@sha256:46087476dd829477b235937b1b774e539c67177fb9c637bde91b28b2e6cf9299
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `php-zendserver:8.5-php5.6` - linux; amd64

```console
$ docker pull php-zendserver@sha256:5393691a9d8617643c002a7ec19c90639a480868ae335ab538499d1a05865d4d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **315.6 MB (315608578 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:513ed7b8cb626435a0c10f51c07b1631f83e70f06549e79357644c19c6d30670`
-	Default Command: `["\/usr\/local\/bin\/run"]`

```dockerfile
# Tue, 31 Aug 2021 01:21:27 GMT
ADD file:11b425d4c08e81a3e0cb2e0345d27cd5fc844dd83f1096af4cc05f635824ff5d in / 
# Tue, 31 Aug 2021 01:21:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 31 Aug 2021 01:21:29 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 01:21:30 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 31 Aug 2021 01:21:30 GMT
CMD ["/bin/bash"]
# Tue, 31 Aug 2021 04:02:14 GMT
RUN apt-key adv --keyserver keyserver.ubuntu.com --recv-key 799058698E65316A2E7A4FF42EAE1437F7D2C623
# Tue, 31 Aug 2021 04:02:15 GMT
COPY file:6f0a5450842ae9c3e06d131c7180961d773ca33754e17af8ea2ac258fd0c6054 in /etc/apt/sources.list.d/zend-server.list 
# Tue, 31 Aug 2021 04:02:15 GMT
COPY file:7a9d81c6298f71cfad4408c8b3d7c3bf53bf90083221ec55686e12b2eb6f16a4 in /etc/apt/sources.list.d/ubuntu-trusty.list 
# Tue, 31 Aug 2021 04:04:03 GMT
RUN apt-get update     && apt-get install -y         curl         libmysqlclient18         unzip         git         zend-server-php-5.6=8.5.17+b19     && rm -rf /var/lib/apt/lists/*     && /usr/local/zend/bin/zendctl.sh stop
# Tue, 31 Aug 2021 04:04:06 GMT
COPY file:def46bbc651bcb61f92bcaa2f8d6edec0c22e51e86132fabd2e47542dcbec0bf in /etc/apache2/conf-available 
# Tue, 31 Aug 2021 04:04:06 GMT
RUN /usr/sbin/a2enconf drop-http-proxy-header
# Tue, 31 Aug 2021 04:04:07 GMT
RUN /usr/sbin/a2enmod headers
# Tue, 31 Aug 2021 04:04:07 GMT
ENV ZS_INIT_VERSION=0.3
# Tue, 31 Aug 2021 04:04:08 GMT
ENV ZS_INIT_SHA256=e8d441d8503808e9fc0fafc762b2cb80d4a6e68b94fede0fe41efdeac10800cb
# Tue, 31 Aug 2021 04:04:09 GMT
RUN curl -fSL -o zs-init.tar.gz "http://repos.zend.com/zs-init/zs-init-docker-${ZS_INIT_VERSION}.tar.gz"     && echo "${ZS_INIT_SHA256} *zs-init.tar.gz" | sha256sum -c -     && mkdir /usr/local/zs-init     && tar xzf zs-init.tar.gz --strip-components=1 -C /usr/local/zs-init     && rm zs-init.tar.gz
# Tue, 31 Aug 2021 04:04:09 GMT
WORKDIR /usr/local/zs-init
# Tue, 31 Aug 2021 04:04:16 GMT
RUN /usr/local/zend/bin/php -r "readfile('https://getcomposer.org/installer');" | /usr/local/zend/bin/php     && /usr/local/zend/bin/php composer.phar self-update && /usr/local/zend/bin/php composer.phar update
# Tue, 31 Aug 2021 04:04:16 GMT
COPY dir:b75978d6e77900379bb898c52c86c408d7f6fcd06b5c66439d594a1a3dcca0b4 in /usr/local/bin 
# Tue, 31 Aug 2021 04:04:16 GMT
COPY dir:80bde0d50316e7c9350262fe3b75826a91d075303027787e759d703b60df13d6 in /usr/local/zend/var/plugins/ 
# Tue, 31 Aug 2021 04:04:17 GMT
RUN rm /var/www/html/index.html
# Tue, 31 Aug 2021 04:04:17 GMT
COPY dir:d174a5d34625889b4356c566972566e0ca7da618b01ea42276562f8186517a67 in /var/www/html 
# Tue, 31 Aug 2021 04:04:17 GMT
EXPOSE 80
# Tue, 31 Aug 2021 04:04:18 GMT
EXPOSE 443
# Tue, 31 Aug 2021 04:04:18 GMT
EXPOSE 10081
# Tue, 31 Aug 2021 04:04:18 GMT
EXPOSE 10082
# Tue, 31 Aug 2021 04:04:18 GMT
WORKDIR /var/www/html
# Tue, 31 Aug 2021 04:04:18 GMT
CMD ["/usr/local/bin/run"]
```

-	Layers:
	-	`sha256:58690f9b18fca6469a14da4e212c96849469f9b1be6661d2342a4bf01774aa50`  
		Last Modified: Thu, 05 Aug 2021 00:25:05 GMT  
		Size: 46.5 MB (46497548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b51569e7c50720acf6860327847fe342a1afbe148d24c529fb81df105e3eed01`  
		Last Modified: Tue, 31 Aug 2021 01:23:09 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da8ef40b9ecabc2679fe2419957220c0272a965c5cf7e0269fa1aeeb8c56f2e1`  
		Last Modified: Tue, 31 Aug 2021 01:23:08 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb15d46c38dcd1ea0b1990006c3366ecd10c79d374f341687eb2cb23a2c8672e`  
		Last Modified: Tue, 31 Aug 2021 01:23:08 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2102dd9376f61b14df18139d78a96caeb38426131bb6a85847a5733f84d83c32`  
		Last Modified: Tue, 31 Aug 2021 04:11:12 GMT  
		Size: 14.7 KB (14704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae050479344fbb7ea0f86b97e8c772b7ae45103fa5cfc2bea2a4b79c631a1534`  
		Last Modified: Tue, 31 Aug 2021 04:11:11 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7d990e63418cea6828a1754a0cfd88662fe780fa88dd2de23528d624ab6bc35`  
		Last Modified: Tue, 31 Aug 2021 04:11:11 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e78264dffd8afd8084e307db7cfd44f971f55d76534559ccd72b50b64108726`  
		Last Modified: Tue, 31 Aug 2021 04:11:40 GMT  
		Size: 263.9 MB (263910611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd783101a133a035071fca065237130e373e2f4cc4151957c9c461ae9a79cdf2`  
		Last Modified: Tue, 31 Aug 2021 04:11:09 GMT  
		Size: 263.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d19cbd07b1b667393092b9d2df1833f0b331cfe1eb5e6ad304f4acbda03136ab`  
		Last Modified: Tue, 31 Aug 2021 04:11:09 GMT  
		Size: 336.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c21aeee9b83798ca4fd42d7e5aa46ecd288c027160673f1be4f3d9d57b70a383`  
		Last Modified: Tue, 31 Aug 2021 04:11:09 GMT  
		Size: 307.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf7e05a640abfb3d3865705d1a482da844acc818d5c32089ee78ec8ba477136d`  
		Last Modified: Tue, 31 Aug 2021 04:11:09 GMT  
		Size: 18.9 KB (18859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be58af708ccc85c876f8148b3f7af699d37b1d23a25d76c1c8eaedd03b6dcc9b`  
		Last Modified: Tue, 31 Aug 2021 04:11:08 GMT  
		Size: 5.1 MB (5146536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb1df10206b55b2eb8839919bb0d056e7256e1dd2bb398a492c5b8317235fe6d`  
		Last Modified: Tue, 31 Aug 2021 04:11:07 GMT  
		Size: 13.4 KB (13357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:703d37b5f26f094cbc47c55b9abf4e3fe103e96208d7e102c579384ffe6add64`  
		Last Modified: Tue, 31 Aug 2021 04:11:06 GMT  
		Size: 2.6 KB (2566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15716512d8f97648b13d29fdbc7df5b8f6ec04e2ca06aa9447b31525f08c1c2c`  
		Last Modified: Tue, 31 Aug 2021 04:11:06 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b72ae8545d8a1d76de6aadb8a94a839c2d60e2f164e0323e0ad4cc73a1853110`  
		Last Modified: Tue, 31 Aug 2021 04:11:06 GMT  
		Size: 1.2 KB (1250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `php-zendserver:9.1`

```console
$ docker pull php-zendserver@sha256:cc80372d5dcac564f69bb3c8c066a46638ee40115142f5247079084a5ddc1179
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `php-zendserver:9.1` - linux; amd64

```console
$ docker pull php-zendserver@sha256:7b079ac3a11ceab944593ab3fbfbbac482a4d6611fa431c710e2bd0472c87888
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **399.3 MB (399260011 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78ac8051a5f543e6f729a4fc404e53a1f68ef6dc6c6443b992634a95664429c3`
-	Default Command: `["\/usr\/local\/bin\/run"]`

```dockerfile
# Tue, 31 Aug 2021 01:21:27 GMT
ADD file:11b425d4c08e81a3e0cb2e0345d27cd5fc844dd83f1096af4cc05f635824ff5d in / 
# Tue, 31 Aug 2021 01:21:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 31 Aug 2021 01:21:29 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 01:21:30 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 31 Aug 2021 01:21:30 GMT
CMD ["/bin/bash"]
# Tue, 31 Aug 2021 04:02:14 GMT
RUN apt-key adv --keyserver keyserver.ubuntu.com --recv-key 799058698E65316A2E7A4FF42EAE1437F7D2C623
# Tue, 31 Aug 2021 04:04:22 GMT
COPY file:0d4830b5060fb75cec6a47b30d343d82f9c3d6f95f20c11635618b93dedb5720 in /etc/apt/sources.list.d/zend-server.list 
# Tue, 31 Aug 2021 04:05:46 GMT
RUN apt-get update     && apt-get install -y       curl       libmysqlclient20       unzip       git       zend-server-php-7.1=9.1.12+b211     && rm -rf /var/lib/apt/lists/*     && /usr/local/zend/bin/zendctl.sh stop
# Tue, 31 Aug 2021 04:05:50 GMT
COPY file:def46bbc651bcb61f92bcaa2f8d6edec0c22e51e86132fabd2e47542dcbec0bf in /etc/apache2/conf-available 
# Tue, 31 Aug 2021 04:05:51 GMT
RUN /usr/sbin/a2enconf drop-http-proxy-header
# Tue, 31 Aug 2021 04:05:52 GMT
RUN /usr/sbin/a2enmod headers
# Tue, 31 Aug 2021 04:05:52 GMT
ENV ZS_INIT_VERSION=0.3
# Tue, 31 Aug 2021 04:05:52 GMT
ENV ZS_INIT_SHA256=e8d441d8503808e9fc0fafc762b2cb80d4a6e68b94fede0fe41efdeac10800cb
# Tue, 31 Aug 2021 04:05:53 GMT
RUN curl -fSL -o zs-init.tar.gz "http://repos.zend.com/zs-init/zs-init-docker-${ZS_INIT_VERSION}.tar.gz"     && echo "${ZS_INIT_SHA256} *zs-init.tar.gz" | sha256sum -c -     && mkdir /usr/local/zs-init     && tar xzf zs-init.tar.gz --strip-components=1 -C /usr/local/zs-init     && rm zs-init.tar.gz
# Tue, 31 Aug 2021 04:05:53 GMT
WORKDIR /usr/local/zs-init
# Tue, 31 Aug 2021 04:06:00 GMT
RUN /usr/local/zend/bin/php -r "readfile('https://getcomposer.org/installer');" | /usr/local/zend/bin/php     && /usr/local/zend/bin/php composer.phar self-update && /usr/local/zend/bin/php composer.phar update
# Tue, 31 Aug 2021 04:06:00 GMT
COPY dir:5966ca4828c37f68d48d11da814350a590451453f42aa83ef2eab6893db3e4cc in /usr/local/bin 
# Tue, 31 Aug 2021 04:06:01 GMT
COPY dir:80bde0d50316e7c9350262fe3b75826a91d075303027787e759d703b60df13d6 in /usr/local/zend/var/plugins/ 
# Tue, 31 Aug 2021 04:06:01 GMT
RUN rm /var/www/html/index.html
# Tue, 31 Aug 2021 04:06:02 GMT
COPY dir:d174a5d34625889b4356c566972566e0ca7da618b01ea42276562f8186517a67 in /var/www/html 
# Tue, 31 Aug 2021 04:06:02 GMT
EXPOSE 80
# Tue, 31 Aug 2021 04:06:02 GMT
EXPOSE 443
# Tue, 31 Aug 2021 04:06:02 GMT
EXPOSE 10081
# Tue, 31 Aug 2021 04:06:02 GMT
EXPOSE 10082
# Tue, 31 Aug 2021 04:06:03 GMT
WORKDIR /var/www/html
# Tue, 31 Aug 2021 04:06:03 GMT
CMD ["/usr/local/bin/run"]
```

-	Layers:
	-	`sha256:58690f9b18fca6469a14da4e212c96849469f9b1be6661d2342a4bf01774aa50`  
		Last Modified: Thu, 05 Aug 2021 00:25:05 GMT  
		Size: 46.5 MB (46497548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b51569e7c50720acf6860327847fe342a1afbe148d24c529fb81df105e3eed01`  
		Last Modified: Tue, 31 Aug 2021 01:23:09 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da8ef40b9ecabc2679fe2419957220c0272a965c5cf7e0269fa1aeeb8c56f2e1`  
		Last Modified: Tue, 31 Aug 2021 01:23:08 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb15d46c38dcd1ea0b1990006c3366ecd10c79d374f341687eb2cb23a2c8672e`  
		Last Modified: Tue, 31 Aug 2021 01:23:08 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2102dd9376f61b14df18139d78a96caeb38426131bb6a85847a5733f84d83c32`  
		Last Modified: Tue, 31 Aug 2021 04:11:12 GMT  
		Size: 14.7 KB (14704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ef9ee709ba9d99042fc4eae3385479692614cfd72cbc83c98522170944f9f1a`  
		Last Modified: Tue, 31 Aug 2021 04:12:01 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:837980bcf5c021764e8ff0b5e1826fa0d23d4d4bbd2fe02962a470f7d8df8f11`  
		Last Modified: Tue, 31 Aug 2021 04:12:43 GMT  
		Size: 347.6 MB (347557251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f311d7aa89c09f28fce59942e782699474050c73dc60b2c0570f5eb2fe64c4fc`  
		Last Modified: Tue, 31 Aug 2021 04:11:59 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8c9384096c8027661058200d5dd435498203ae6cea4ffada13ffcc34a17f730`  
		Last Modified: Tue, 31 Aug 2021 04:11:59 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a391773894550b0dcf95133d7a0ebfc325acd5a660c35f96c77133e3fd8f740c`  
		Last Modified: Tue, 31 Aug 2021 04:11:59 GMT  
		Size: 308.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e99104e97158863a1815e4b564104f84c3c0671a3ef2a49ddf935cb20a41e537`  
		Last Modified: Tue, 31 Aug 2021 04:11:59 GMT  
		Size: 18.9 KB (18859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dc404237abddc7a47d1e606dc92470e0035dcd32745c3c0bf383528304c96d7`  
		Last Modified: Tue, 31 Aug 2021 04:11:58 GMT  
		Size: 5.2 MB (5150653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63099d2783ee41f72d28cc95ab35ba28c5674108eead4fba7719574ecddb2c99`  
		Last Modified: Tue, 31 Aug 2021 04:11:57 GMT  
		Size: 14.3 KB (14320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16df2874073685e8fadc4aa9c04fc75132336de6749145d708e7d664cc03a03f`  
		Last Modified: Tue, 31 Aug 2021 04:11:57 GMT  
		Size: 2.6 KB (2559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b978107de3a3767f2ffe65e620f34ce62d93b74cbd20b77b1821327e7458539b`  
		Last Modified: Tue, 31 Aug 2021 04:11:57 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc3a81a9d2085d59971d4608251a552a6c9631466fcac109142e49c26602cf12`  
		Last Modified: Tue, 31 Aug 2021 04:11:57 GMT  
		Size: 1.2 KB (1249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `php-zendserver:latest`

```console
$ docker pull php-zendserver@sha256:882235663fae8f55986e7666a1caeaba4841a1a385f2647f91cf288e6d358095
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `php-zendserver:latest` - linux; amd64

```console
$ docker pull php-zendserver@sha256:38c703709692c1f2a37518dc3f6ad9cb5f59dab6aa39b7f3c72fe7b51dd9bf21
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **394.8 MB (394750601 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fcc5df54322f7d81a8081f5a073a650fd506da09c6b29e526e927f7d04b3baf3`
-	Default Command: `["\/usr\/local\/bin\/run"]`

```dockerfile
# Tue, 25 Oct 2022 01:53:28 GMT
ADD file:fc5d658c47ede58827812b75a311353be776e41e2dd339b8906839527c9b5247 in / 
# Tue, 25 Oct 2022 01:53:28 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 17:19:21 GMT
RUN apt-get update && apt-get install -y       gnupg
# Tue, 25 Oct 2022 17:19:22 GMT
RUN apt-key adv --keyserver keyserver.ubuntu.com --recv-key 799058698E65316A2E7A4FF42EAE1437F7D2C623
# Tue, 25 Oct 2022 17:21:29 GMT
COPY file:1e70d8fd6f9643bffb703528edddba0aa02a58e95cc53e92f58a86cde29e732a in /etc/apt/sources.list.d/zend-server.list 
# Tue, 25 Oct 2022 17:23:03 GMT
RUN apt-get update && apt-get install -y       iproute2       curl       libmysqlclient20       unzip       git       zend-server-nginx=2021.0.0+b74     && rm -rf /var/lib/apt/lists/*     && /usr/local/zend/bin/zendctl.sh stop
# Tue, 25 Oct 2022 17:23:06 GMT
ENV ZS_INIT_VERSION=0.3
# Tue, 25 Oct 2022 17:23:06 GMT
ENV ZS_INIT_SHA256=e8d441d8503808e9fc0fafc762b2cb80d4a6e68b94fede0fe41efdeac10800cb
# Tue, 25 Oct 2022 17:23:06 GMT
COPY file:ad21ce0b2dc8345be0ef63836774934d6b2045ddc3685411221a07dd10b649d1 in /tmp/zs-init.patch 
# Tue, 25 Oct 2022 17:23:08 GMT
RUN curl -fSL -o zs-init.tar.gz "http://repos.zend.com/zs-init/zs-init-docker-${ZS_INIT_VERSION}.tar.gz"     && echo "${ZS_INIT_SHA256} *zs-init.tar.gz" | sha256sum -c -     && mkdir /usr/local/zs-init     && tar xzf zs-init.tar.gz --strip-components=1 -C /usr/local/zs-init     && rm zs-init.tar.gz     && patch -u /usr/local/zs-init/src/Init/Steps/AbstractStep.php -i /tmp/zs-init.patch     && rm /tmp/zs-init.patch
# Tue, 25 Oct 2022 17:23:08 GMT
WORKDIR /usr/local/zs-init
# Tue, 25 Oct 2022 17:23:13 GMT
RUN /usr/local/zend/bin/php -r "readfile('https://getcomposer.org/installer');" | /usr/local/zend/bin/php     && /usr/local/zend/bin/php composer.phar update
# Tue, 25 Oct 2022 17:23:14 GMT
COPY dir:eecd98e9ebf1c61a12ae67558eb2a6ce846b9ebfadabbf08503e90b3e30d9496 in /usr/local/bin 
# Tue, 25 Oct 2022 17:23:14 GMT
COPY dir:80bde0d50316e7c9350262fe3b75826a91d075303027787e759d703b60df13d6 in /usr/local/zend/var/plugins/ 
# Tue, 25 Oct 2022 17:23:14 GMT
RUN rm /var/www/html/index.nginx-debian.html
# Tue, 25 Oct 2022 17:23:14 GMT
COPY dir:d174a5d34625889b4356c566972566e0ca7da618b01ea42276562f8186517a67 in /var/www/html 
# Tue, 25 Oct 2022 17:23:14 GMT
EXPOSE 80
# Tue, 25 Oct 2022 17:23:15 GMT
EXPOSE 443
# Tue, 25 Oct 2022 17:23:15 GMT
EXPOSE 10081
# Tue, 25 Oct 2022 17:23:15 GMT
EXPOSE 10082
# Tue, 25 Oct 2022 17:23:15 GMT
WORKDIR /var/www/html
# Tue, 25 Oct 2022 17:23:15 GMT
CMD ["/usr/local/bin/run"]
```

-	Layers:
	-	`sha256:a404e54162968593b8d92b571f3cdd673e4c9eab5d9be28d7c494595c0aa6682`  
		Last Modified: Wed, 19 Oct 2022 22:03:02 GMT  
		Size: 26.7 MB (26712500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fbb3fae8f00f5b0fb4cf5a677d7131fad36431423e10e2c243ce245cfb22808`  
		Last Modified: Wed, 26 Oct 2022 15:47:38 GMT  
		Size: 36.7 MB (36676854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfef197f4322d6a3bde0d88fdf96a99f095d982900906520ae117a39f658a0c3`  
		Last Modified: Wed, 26 Oct 2022 15:47:34 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8ee2927be8bc9d8db274aa85650c006f8ec987d85aa3dd85e3278da02144502`  
		Last Modified: Wed, 26 Oct 2022 15:48:50 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07fbe6b63324df1effc044b8e838ae9c928632a765c2d3efa5d380786f324ab0`  
		Last Modified: Wed, 26 Oct 2022 15:49:43 GMT  
		Size: 326.0 MB (326006802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26925d52cd07bde840512fa2026ea1e75ebbd5abd2fe22673ab9773e6ac63328`  
		Last Modified: Wed, 26 Oct 2022 15:48:50 GMT  
		Size: 446.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37c8d761f31ae9946acc1bcdd2fa95e12095724f83117d222140f91ec007bf9f`  
		Last Modified: Wed, 26 Oct 2022 15:48:50 GMT  
		Size: 18.9 KB (18926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00d53c3a35228079dcfe72aa875a6b69de67b6a86050b3a0449330cbb33f785b`  
		Last Modified: Wed, 26 Oct 2022 15:48:50 GMT  
		Size: 5.3 MB (5315156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1054edbca2de70c30f494fde04969dfe94ea2c415a5727391357f26f973fe18b`  
		Last Modified: Wed, 26 Oct 2022 15:48:48 GMT  
		Size: 14.3 KB (14293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24bf534882f3d908757d2f91a520575226f452bebb5567c0f8b7b7f61850ec3f`  
		Last Modified: Wed, 26 Oct 2022 15:48:48 GMT  
		Size: 2.6 KB (2558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:442235a0cc8ddeec20cc48b51ac49181891e510211e0b1f3ac739b7fcd2485e8`  
		Last Modified: Wed, 26 Oct 2022 15:48:48 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff3ee1cceacb8560da402eb62ea8c3bc49e67a6489817e12f24f84d7c73beca2`  
		Last Modified: Wed, 26 Oct 2022 15:48:48 GMT  
		Size: 1.3 KB (1255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
