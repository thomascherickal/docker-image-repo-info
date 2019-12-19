<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `php-zendserver`

-	[`php-zendserver:2019.0`](#php-zendserver20190)
-	[`php-zendserver:9.1`](#php-zendserver91)
-	[`php-zendserver:latest`](#php-zendserverlatest)

## `php-zendserver:2019.0`

```console
$ docker pull php-zendserver@sha256:82eb9b5c0ed354984c693bc51427265b4f9091e347010b5a250434a772e6cd70
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `php-zendserver:2019.0` - linux; amd64

```console
$ docker pull php-zendserver@sha256:893ce8b1bb78271ea5991c4df2efa900eab4556a3c564370b3faded61f298bea
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **450.4 MB (450421477 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:564ff968430192fc59be9a0760ba68cd8839a9a5b4786ecf7a9696fa4cb74887`
-	Default Command: `["\/usr\/local\/bin\/run"]`

```dockerfile
# Thu, 19 Dec 2019 04:24:35 GMT
ADD file:f0b8eaa718bc3965b1e8395f5a6bea97c16651b50614e676bb3eaf31335a0045 in / 
# Thu, 19 Dec 2019 04:24:36 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 19 Dec 2019 04:24:37 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 19 Dec 2019 04:24:38 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 19 Dec 2019 04:24:38 GMT
CMD ["/bin/bash"]
# Thu, 19 Dec 2019 09:25:36 GMT
RUN apt-key adv --keyserver keyserver.ubuntu.com --recv-key 799058698E65316A2E7A4FF42EAE1437F7D2C623
# Thu, 19 Dec 2019 09:27:36 GMT
COPY file:64f63be6042521a7e257b6755c9344694bbe4c59cd3c677e8df3dc06c795a802 in /etc/apt/sources.list.d/zend-server.list 
# Thu, 19 Dec 2019 09:29:13 GMT
RUN apt-get update     && apt-get install -y       curl       libmysqlclient20       unzip       git       zend-server=2019.0.3+b345     && rm -rf /var/lib/apt/lists/*     && /usr/local/zend/bin/zendctl.sh stop
# Thu, 19 Dec 2019 09:29:14 GMT
COPY file:26009fd1b91c8a82cfe83d983f9357a5914e70e1b464baf9d4d99dd284c5f310 in /etc/zend.lic 
# Thu, 19 Dec 2019 09:29:14 GMT
COPY file:def46bbc651bcb61f92bcaa2f8d6edec0c22e51e86132fabd2e47542dcbec0bf in /etc/apache2/conf-available 
# Thu, 19 Dec 2019 09:29:15 GMT
RUN /usr/sbin/a2enconf drop-http-proxy-header
# Thu, 19 Dec 2019 09:29:16 GMT
RUN /usr/sbin/a2enmod headers
# Thu, 19 Dec 2019 09:29:17 GMT
ENV ZS_INIT_VERSION=0.3
# Thu, 19 Dec 2019 09:29:20 GMT
ENV ZS_INIT_SHA256=e8d441d8503808e9fc0fafc762b2cb80d4a6e68b94fede0fe41efdeac10800cb
# Thu, 19 Dec 2019 09:29:21 GMT
RUN curl -fSL -o zs-init.tar.gz "http://repos.zend.com/zs-init/zs-init-docker-${ZS_INIT_VERSION}.tar.gz"     && echo "${ZS_INIT_SHA256} *zs-init.tar.gz" | sha256sum -c -     && mkdir /usr/local/zs-init     && tar xzf zs-init.tar.gz --strip-components=1 -C /usr/local/zs-init     && rm zs-init.tar.gz
# Thu, 19 Dec 2019 09:29:21 GMT
WORKDIR /usr/local/zs-init
# Thu, 19 Dec 2019 09:29:31 GMT
RUN /usr/local/zend/bin/php -r "readfile('https://getcomposer.org/installer');" | /usr/local/zend/bin/php     && /usr/local/zend/bin/php composer.phar self-update && /usr/local/zend/bin/php composer.phar update
# Thu, 19 Dec 2019 09:29:31 GMT
COPY dir:2503294e06c787d82d501853381aa61cd4a7bf7e5f082292d4aba573b9bbf2e2 in /usr/local/bin 
# Thu, 19 Dec 2019 09:29:31 GMT
COPY dir:80bde0d50316e7c9350262fe3b75826a91d075303027787e759d703b60df13d6 in /usr/local/zend/var/plugins/ 
# Thu, 19 Dec 2019 09:29:32 GMT
RUN rm /var/www/html/index.html
# Thu, 19 Dec 2019 09:29:32 GMT
COPY dir:d174a5d34625889b4356c566972566e0ca7da618b01ea42276562f8186517a67 in /var/www/html 
# Thu, 19 Dec 2019 09:29:32 GMT
EXPOSE 80
# Thu, 19 Dec 2019 09:29:32 GMT
EXPOSE 443
# Thu, 19 Dec 2019 09:29:32 GMT
EXPOSE 10081
# Thu, 19 Dec 2019 09:29:33 GMT
EXPOSE 10082
# Thu, 19 Dec 2019 09:29:33 GMT
WORKDIR /var/www/html
# Thu, 19 Dec 2019 09:29:33 GMT
CMD ["/usr/local/bin/run"]
```

-	Layers:
	-	`sha256:3386e6af03b043219225367632569465e5ecd47391d1f99a6d265e51bd463a83`  
		Last Modified: Thu, 12 Dec 2019 08:26:09 GMT  
		Size: 44.1 MB (44123254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49ac0bbe6c8eeb959337b336ceaa5c3bbbae81e316025f9b94ede453540f2377`  
		Last Modified: Thu, 19 Dec 2019 04:26:00 GMT  
		Size: 529.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1983a67e104e801fceb1850a375a71fe6b62636ba7a8403d9644f308a6a43f9`  
		Last Modified: Thu, 19 Dec 2019 04:26:00 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a0f3a523f04f61db942018321ae122f90d8e3303e243b005e8de9817daf7028`  
		Last Modified: Thu, 19 Dec 2019 04:25:59 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dee51a57715f0b1489f9c52a40655d476868a88c0d5af35e59d4d7bb0cc44c1`  
		Last Modified: Thu, 19 Dec 2019 09:29:56 GMT  
		Size: 13.1 KB (13068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53c1cbda829149cf1be4af1b326df822a7fbb3b839ee55962854050801559e05`  
		Last Modified: Thu, 19 Dec 2019 09:30:53 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff27fdaf3774595a509ee20a150d04af9b7f499a27b83fa89a6b5c92881fbc3f`  
		Last Modified: Thu, 19 Dec 2019 09:31:52 GMT  
		Size: 388.3 MB (388254215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48c7fde5eb485f10cb0b920b940b91f8182612ed40107afc502add6d1559ac5f`  
		Last Modified: Thu, 19 Dec 2019 09:30:52 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39773e5112066147ed2120422a84ded27ecf897452f8fa59533f0d0f76c31899`  
		Last Modified: Thu, 19 Dec 2019 09:30:51 GMT  
		Size: 262.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:453bf8d8fb4403524aa7e8092e7a0f96aee73941d824a5f9a452c96b5d924878`  
		Last Modified: Thu, 19 Dec 2019 09:30:52 GMT  
		Size: 315.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5760a384e5682e602608eb9e5d7b7d5f170d112de455b39fc8537cad681ebf7`  
		Last Modified: Thu, 19 Dec 2019 09:30:51 GMT  
		Size: 307.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78e6b9084fc16df83a5c215c0a6447e1a263c235155d2dfff3a69eebd5d99589`  
		Last Modified: Thu, 19 Dec 2019 09:30:51 GMT  
		Size: 18.8 KB (18831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:621c9d7d8f57105573f03d8b44c8e2e74922871d2ef69b73de6979cc5ea4d7c1`  
		Last Modified: Thu, 19 Dec 2019 09:30:53 GMT  
		Size: 18.0 MB (17990978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e2c5314bb4742ba440bc6362e57741d9c0358eb3bfc280b8ba536c3d27e258d`  
		Last Modified: Thu, 19 Dec 2019 09:30:50 GMT  
		Size: 14.3 KB (14296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c246510189e7e62eab4fff2b67e827be7ec0c586e99da70628d8018e87d0cf7`  
		Last Modified: Thu, 19 Dec 2019 09:30:50 GMT  
		Size: 2.5 KB (2531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb621c58f9c92a3789aedd9d9b49dfc6d9be9ac5cdc9a39665966c384d3cd549`  
		Last Modified: Thu, 19 Dec 2019 09:30:50 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c0f5e4f3e8069d678ea9f1d80552a9d3d16378b5c90328fedc3f4749048034f`  
		Last Modified: Thu, 19 Dec 2019 09:30:50 GMT  
		Size: 1.2 KB (1248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `php-zendserver:9.1`

```console
$ docker pull php-zendserver@sha256:f6bf2695cdad4940913081a1491dd3e96aa68c1ff634e456f24c09163a3d497c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `php-zendserver:9.1` - linux; amd64

```console
$ docker pull php-zendserver@sha256:6bd99c420a7595579dbd1ae59c14f7fc0253eb71f02cccfbeb4cb99cfa231729
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **409.7 MB (409719210 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19ecc74ba65ca696fd5858b57584cd290c30517f1827a1857e55965afba954e1`
-	Default Command: `["\/usr\/local\/bin\/run"]`

```dockerfile
# Thu, 19 Dec 2019 04:24:35 GMT
ADD file:f0b8eaa718bc3965b1e8395f5a6bea97c16651b50614e676bb3eaf31335a0045 in / 
# Thu, 19 Dec 2019 04:24:36 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 19 Dec 2019 04:24:37 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 19 Dec 2019 04:24:38 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 19 Dec 2019 04:24:38 GMT
CMD ["/bin/bash"]
# Thu, 19 Dec 2019 09:25:36 GMT
RUN apt-key adv --keyserver keyserver.ubuntu.com --recv-key 799058698E65316A2E7A4FF42EAE1437F7D2C623
# Thu, 19 Dec 2019 09:25:36 GMT
COPY file:0d4830b5060fb75cec6a47b30d343d82f9c3d6f95f20c11635618b93dedb5720 in /etc/apt/sources.list.d/zend-server.list 
# Thu, 19 Dec 2019 09:27:07 GMT
RUN apt-get update     && apt-get install -y       curl       libmysqlclient20       unzip       git       zend-server-php-7.1=9.1.10+b202     && rm -rf /var/lib/apt/lists/*     && /usr/local/zend/bin/zendctl.sh stop
# Thu, 19 Dec 2019 09:27:08 GMT
COPY file:26009fd1b91c8a82cfe83d983f9357a5914e70e1b464baf9d4d99dd284c5f310 in /etc/zend.lic 
# Thu, 19 Dec 2019 09:27:09 GMT
COPY file:def46bbc651bcb61f92bcaa2f8d6edec0c22e51e86132fabd2e47542dcbec0bf in /etc/apache2/conf-available 
# Thu, 19 Dec 2019 09:27:09 GMT
RUN /usr/sbin/a2enconf drop-http-proxy-header
# Thu, 19 Dec 2019 09:27:10 GMT
RUN /usr/sbin/a2enmod headers
# Thu, 19 Dec 2019 09:27:10 GMT
ENV ZS_INIT_VERSION=0.3
# Thu, 19 Dec 2019 09:27:10 GMT
ENV ZS_INIT_SHA256=e8d441d8503808e9fc0fafc762b2cb80d4a6e68b94fede0fe41efdeac10800cb
# Thu, 19 Dec 2019 09:27:11 GMT
RUN curl -fSL -o zs-init.tar.gz "http://repos.zend.com/zs-init/zs-init-docker-${ZS_INIT_VERSION}.tar.gz"     && echo "${ZS_INIT_SHA256} *zs-init.tar.gz" | sha256sum -c -     && mkdir /usr/local/zs-init     && tar xzf zs-init.tar.gz --strip-components=1 -C /usr/local/zs-init     && rm zs-init.tar.gz
# Thu, 19 Dec 2019 09:27:11 GMT
WORKDIR /usr/local/zs-init
# Thu, 19 Dec 2019 09:27:21 GMT
RUN /usr/local/zend/bin/php -r "readfile('https://getcomposer.org/installer');" | /usr/local/zend/bin/php     && /usr/local/zend/bin/php composer.phar self-update && /usr/local/zend/bin/php composer.phar update
# Thu, 19 Dec 2019 09:27:21 GMT
COPY dir:864637d3fa0817ce3be0c7e34e1298851fa2ea4cfb86583e2ec811f00c6a95fd in /usr/local/bin 
# Thu, 19 Dec 2019 09:27:21 GMT
COPY dir:80bde0d50316e7c9350262fe3b75826a91d075303027787e759d703b60df13d6 in /usr/local/zend/var/plugins/ 
# Thu, 19 Dec 2019 09:27:22 GMT
RUN rm /var/www/html/index.html
# Thu, 19 Dec 2019 09:27:22 GMT
COPY dir:d174a5d34625889b4356c566972566e0ca7da618b01ea42276562f8186517a67 in /var/www/html 
# Thu, 19 Dec 2019 09:27:22 GMT
EXPOSE 80
# Thu, 19 Dec 2019 09:27:22 GMT
EXPOSE 443
# Thu, 19 Dec 2019 09:27:23 GMT
EXPOSE 10081
# Thu, 19 Dec 2019 09:27:23 GMT
EXPOSE 10082
# Thu, 19 Dec 2019 09:27:23 GMT
WORKDIR /var/www/html
# Thu, 19 Dec 2019 09:27:23 GMT
CMD ["/usr/local/bin/run"]
```

-	Layers:
	-	`sha256:3386e6af03b043219225367632569465e5ecd47391d1f99a6d265e51bd463a83`  
		Last Modified: Thu, 12 Dec 2019 08:26:09 GMT  
		Size: 44.1 MB (44123254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49ac0bbe6c8eeb959337b336ceaa5c3bbbae81e316025f9b94ede453540f2377`  
		Last Modified: Thu, 19 Dec 2019 04:26:00 GMT  
		Size: 529.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1983a67e104e801fceb1850a375a71fe6b62636ba7a8403d9644f308a6a43f9`  
		Last Modified: Thu, 19 Dec 2019 04:26:00 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a0f3a523f04f61db942018321ae122f90d8e3303e243b005e8de9817daf7028`  
		Last Modified: Thu, 19 Dec 2019 04:25:59 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dee51a57715f0b1489f9c52a40655d476868a88c0d5af35e59d4d7bb0cc44c1`  
		Last Modified: Thu, 19 Dec 2019 09:29:56 GMT  
		Size: 13.1 KB (13068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b96d3fc0273a6faaac2b3c32eca6a371925c82575307f6f86e41c066dc5b9276`  
		Last Modified: Thu, 19 Dec 2019 09:29:56 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b79dcbbafe91ae3a658710c8bdab43402b6b191e9105fa6ab4d0c8f6e8b809e`  
		Last Modified: Thu, 19 Dec 2019 09:30:45 GMT  
		Size: 347.6 MB (347552079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c39fcf10d221953fb422428911c78ca9011981c22a17f2aa9d4e890ae20697c4`  
		Last Modified: Thu, 19 Dec 2019 09:29:55 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94ae8aa4721020f76a7e425a7309de03a032c5039878d9a4db4238dc4fc0650f`  
		Last Modified: Thu, 19 Dec 2019 09:29:55 GMT  
		Size: 263.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23a43f5754abdf8e218acb55508e916c39dc227481f1a331486f1ae6016dbcd8`  
		Last Modified: Thu, 19 Dec 2019 09:29:54 GMT  
		Size: 315.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ce038913745fd1b88fab31c030678f9ede7d08163d497d0959fe5668a68e9eb`  
		Last Modified: Thu, 19 Dec 2019 09:29:54 GMT  
		Size: 309.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84d2313b4dfbf787112926e42c1790001c4e326779598c69cc4ee9a19f4bea30`  
		Last Modified: Thu, 19 Dec 2019 09:29:54 GMT  
		Size: 18.8 KB (18832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6888a6afdb2ee914ca2fa6f3454bb77259fcb3f7016d5dc73bb3ded046bb5be1`  
		Last Modified: Thu, 19 Dec 2019 09:29:56 GMT  
		Size: 18.0 MB (17990846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52f1be142f167de7a289399ebc955e8d8ec1be80ef83a05e11d6749ec07bd0dd`  
		Last Modified: Thu, 19 Dec 2019 09:29:53 GMT  
		Size: 14.3 KB (14298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13ec644c2b7b663967a331c427efcb40a75869d210fbaf0388ab92f802d04d9c`  
		Last Modified: Thu, 19 Dec 2019 09:29:53 GMT  
		Size: 2.5 KB (2530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11acead17010886fa662c1fd69c728b46c4ac6d9bce556ae45d9062fef9c19aa`  
		Last Modified: Thu, 19 Dec 2019 09:29:53 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f369c9645a2058099f040f80b2c29156e678d672a389566f78a8b821e22ec6c`  
		Last Modified: Thu, 19 Dec 2019 09:29:53 GMT  
		Size: 1.2 KB (1250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `php-zendserver:latest`

```console
$ docker pull php-zendserver@sha256:82eb9b5c0ed354984c693bc51427265b4f9091e347010b5a250434a772e6cd70
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `php-zendserver:latest` - linux; amd64

```console
$ docker pull php-zendserver@sha256:893ce8b1bb78271ea5991c4df2efa900eab4556a3c564370b3faded61f298bea
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **450.4 MB (450421477 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:564ff968430192fc59be9a0760ba68cd8839a9a5b4786ecf7a9696fa4cb74887`
-	Default Command: `["\/usr\/local\/bin\/run"]`

```dockerfile
# Thu, 19 Dec 2019 04:24:35 GMT
ADD file:f0b8eaa718bc3965b1e8395f5a6bea97c16651b50614e676bb3eaf31335a0045 in / 
# Thu, 19 Dec 2019 04:24:36 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 19 Dec 2019 04:24:37 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 19 Dec 2019 04:24:38 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 19 Dec 2019 04:24:38 GMT
CMD ["/bin/bash"]
# Thu, 19 Dec 2019 09:25:36 GMT
RUN apt-key adv --keyserver keyserver.ubuntu.com --recv-key 799058698E65316A2E7A4FF42EAE1437F7D2C623
# Thu, 19 Dec 2019 09:27:36 GMT
COPY file:64f63be6042521a7e257b6755c9344694bbe4c59cd3c677e8df3dc06c795a802 in /etc/apt/sources.list.d/zend-server.list 
# Thu, 19 Dec 2019 09:29:13 GMT
RUN apt-get update     && apt-get install -y       curl       libmysqlclient20       unzip       git       zend-server=2019.0.3+b345     && rm -rf /var/lib/apt/lists/*     && /usr/local/zend/bin/zendctl.sh stop
# Thu, 19 Dec 2019 09:29:14 GMT
COPY file:26009fd1b91c8a82cfe83d983f9357a5914e70e1b464baf9d4d99dd284c5f310 in /etc/zend.lic 
# Thu, 19 Dec 2019 09:29:14 GMT
COPY file:def46bbc651bcb61f92bcaa2f8d6edec0c22e51e86132fabd2e47542dcbec0bf in /etc/apache2/conf-available 
# Thu, 19 Dec 2019 09:29:15 GMT
RUN /usr/sbin/a2enconf drop-http-proxy-header
# Thu, 19 Dec 2019 09:29:16 GMT
RUN /usr/sbin/a2enmod headers
# Thu, 19 Dec 2019 09:29:17 GMT
ENV ZS_INIT_VERSION=0.3
# Thu, 19 Dec 2019 09:29:20 GMT
ENV ZS_INIT_SHA256=e8d441d8503808e9fc0fafc762b2cb80d4a6e68b94fede0fe41efdeac10800cb
# Thu, 19 Dec 2019 09:29:21 GMT
RUN curl -fSL -o zs-init.tar.gz "http://repos.zend.com/zs-init/zs-init-docker-${ZS_INIT_VERSION}.tar.gz"     && echo "${ZS_INIT_SHA256} *zs-init.tar.gz" | sha256sum -c -     && mkdir /usr/local/zs-init     && tar xzf zs-init.tar.gz --strip-components=1 -C /usr/local/zs-init     && rm zs-init.tar.gz
# Thu, 19 Dec 2019 09:29:21 GMT
WORKDIR /usr/local/zs-init
# Thu, 19 Dec 2019 09:29:31 GMT
RUN /usr/local/zend/bin/php -r "readfile('https://getcomposer.org/installer');" | /usr/local/zend/bin/php     && /usr/local/zend/bin/php composer.phar self-update && /usr/local/zend/bin/php composer.phar update
# Thu, 19 Dec 2019 09:29:31 GMT
COPY dir:2503294e06c787d82d501853381aa61cd4a7bf7e5f082292d4aba573b9bbf2e2 in /usr/local/bin 
# Thu, 19 Dec 2019 09:29:31 GMT
COPY dir:80bde0d50316e7c9350262fe3b75826a91d075303027787e759d703b60df13d6 in /usr/local/zend/var/plugins/ 
# Thu, 19 Dec 2019 09:29:32 GMT
RUN rm /var/www/html/index.html
# Thu, 19 Dec 2019 09:29:32 GMT
COPY dir:d174a5d34625889b4356c566972566e0ca7da618b01ea42276562f8186517a67 in /var/www/html 
# Thu, 19 Dec 2019 09:29:32 GMT
EXPOSE 80
# Thu, 19 Dec 2019 09:29:32 GMT
EXPOSE 443
# Thu, 19 Dec 2019 09:29:32 GMT
EXPOSE 10081
# Thu, 19 Dec 2019 09:29:33 GMT
EXPOSE 10082
# Thu, 19 Dec 2019 09:29:33 GMT
WORKDIR /var/www/html
# Thu, 19 Dec 2019 09:29:33 GMT
CMD ["/usr/local/bin/run"]
```

-	Layers:
	-	`sha256:3386e6af03b043219225367632569465e5ecd47391d1f99a6d265e51bd463a83`  
		Last Modified: Thu, 12 Dec 2019 08:26:09 GMT  
		Size: 44.1 MB (44123254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49ac0bbe6c8eeb959337b336ceaa5c3bbbae81e316025f9b94ede453540f2377`  
		Last Modified: Thu, 19 Dec 2019 04:26:00 GMT  
		Size: 529.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1983a67e104e801fceb1850a375a71fe6b62636ba7a8403d9644f308a6a43f9`  
		Last Modified: Thu, 19 Dec 2019 04:26:00 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a0f3a523f04f61db942018321ae122f90d8e3303e243b005e8de9817daf7028`  
		Last Modified: Thu, 19 Dec 2019 04:25:59 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dee51a57715f0b1489f9c52a40655d476868a88c0d5af35e59d4d7bb0cc44c1`  
		Last Modified: Thu, 19 Dec 2019 09:29:56 GMT  
		Size: 13.1 KB (13068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53c1cbda829149cf1be4af1b326df822a7fbb3b839ee55962854050801559e05`  
		Last Modified: Thu, 19 Dec 2019 09:30:53 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff27fdaf3774595a509ee20a150d04af9b7f499a27b83fa89a6b5c92881fbc3f`  
		Last Modified: Thu, 19 Dec 2019 09:31:52 GMT  
		Size: 388.3 MB (388254215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48c7fde5eb485f10cb0b920b940b91f8182612ed40107afc502add6d1559ac5f`  
		Last Modified: Thu, 19 Dec 2019 09:30:52 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39773e5112066147ed2120422a84ded27ecf897452f8fa59533f0d0f76c31899`  
		Last Modified: Thu, 19 Dec 2019 09:30:51 GMT  
		Size: 262.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:453bf8d8fb4403524aa7e8092e7a0f96aee73941d824a5f9a452c96b5d924878`  
		Last Modified: Thu, 19 Dec 2019 09:30:52 GMT  
		Size: 315.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5760a384e5682e602608eb9e5d7b7d5f170d112de455b39fc8537cad681ebf7`  
		Last Modified: Thu, 19 Dec 2019 09:30:51 GMT  
		Size: 307.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78e6b9084fc16df83a5c215c0a6447e1a263c235155d2dfff3a69eebd5d99589`  
		Last Modified: Thu, 19 Dec 2019 09:30:51 GMT  
		Size: 18.8 KB (18831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:621c9d7d8f57105573f03d8b44c8e2e74922871d2ef69b73de6979cc5ea4d7c1`  
		Last Modified: Thu, 19 Dec 2019 09:30:53 GMT  
		Size: 18.0 MB (17990978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e2c5314bb4742ba440bc6362e57741d9c0358eb3bfc280b8ba536c3d27e258d`  
		Last Modified: Thu, 19 Dec 2019 09:30:50 GMT  
		Size: 14.3 KB (14296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c246510189e7e62eab4fff2b67e827be7ec0c586e99da70628d8018e87d0cf7`  
		Last Modified: Thu, 19 Dec 2019 09:30:50 GMT  
		Size: 2.5 KB (2531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb621c58f9c92a3789aedd9d9b49dfc6d9be9ac5cdc9a39665966c384d3cd549`  
		Last Modified: Thu, 19 Dec 2019 09:30:50 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c0f5e4f3e8069d678ea9f1d80552a9d3d16378b5c90328fedc3f4749048034f`  
		Last Modified: Thu, 19 Dec 2019 09:30:50 GMT  
		Size: 1.2 KB (1248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
