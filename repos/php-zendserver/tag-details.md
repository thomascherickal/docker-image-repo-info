<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `php-zendserver`

-	[`php-zendserver:2019.0`](#php-zendserver20190)
-	[`php-zendserver:5.6`](#php-zendserver56)
-	[`php-zendserver:8.5`](#php-zendserver85)
-	[`php-zendserver:8.5-php5.6`](#php-zendserver85-php56)
-	[`php-zendserver:9.1`](#php-zendserver91)
-	[`php-zendserver:latest`](#php-zendserverlatest)

## `php-zendserver:2019.0`

```console
$ docker pull php-zendserver@sha256:48502759e5ba39d563a18c5e59721346367e60182151a062d052ed9e796613b2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `php-zendserver:2019.0` - linux; amd64

```console
$ docker pull php-zendserver@sha256:451493593ea52b67771e890f7e1bda545f1349e1bd6af7fdd57469a3f89ac3bf
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **451.1 MB (451059936 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f17c59a2778aa6a54dd80d1f13b1e7e9af2c159204f093d7a6443184449fc5b7`
-	Default Command: `["\/usr\/local\/bin\/run"]`

```dockerfile
# Fri, 21 Feb 2020 22:22:27 GMT
ADD file:1f70668251e2e58cee0ff0c22ee805f8a269ac6f8934c07f7e89dca6cc1de3aa in / 
# Fri, 21 Feb 2020 22:22:27 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:22:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:22:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:22:30 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 23:10:37 GMT
RUN apt-key adv --keyserver keyserver.ubuntu.com --recv-key 799058698E65316A2E7A4FF42EAE1437F7D2C623
# Fri, 21 Feb 2020 23:12:39 GMT
COPY file:64f63be6042521a7e257b6755c9344694bbe4c59cd3c677e8df3dc06c795a802 in /etc/apt/sources.list.d/zend-server.list 
# Fri, 21 Feb 2020 23:14:06 GMT
RUN apt-get update     && apt-get install -y       curl       libmysqlclient20       unzip       git       zend-server=2019.0.3+b345     && rm -rf /var/lib/apt/lists/*     && /usr/local/zend/bin/zendctl.sh stop
# Fri, 21 Feb 2020 23:14:07 GMT
COPY file:26009fd1b91c8a82cfe83d983f9357a5914e70e1b464baf9d4d99dd284c5f310 in /etc/zend.lic 
# Fri, 21 Feb 2020 23:14:07 GMT
COPY file:def46bbc651bcb61f92bcaa2f8d6edec0c22e51e86132fabd2e47542dcbec0bf in /etc/apache2/conf-available 
# Fri, 21 Feb 2020 23:14:08 GMT
RUN /usr/sbin/a2enconf drop-http-proxy-header
# Fri, 21 Feb 2020 23:14:09 GMT
RUN /usr/sbin/a2enmod headers
# Fri, 21 Feb 2020 23:14:09 GMT
ENV ZS_INIT_VERSION=0.3
# Fri, 21 Feb 2020 23:14:09 GMT
ENV ZS_INIT_SHA256=e8d441d8503808e9fc0fafc762b2cb80d4a6e68b94fede0fe41efdeac10800cb
# Fri, 21 Feb 2020 23:14:10 GMT
RUN curl -fSL -o zs-init.tar.gz "http://repos.zend.com/zs-init/zs-init-docker-${ZS_INIT_VERSION}.tar.gz"     && echo "${ZS_INIT_SHA256} *zs-init.tar.gz" | sha256sum -c -     && mkdir /usr/local/zs-init     && tar xzf zs-init.tar.gz --strip-components=1 -C /usr/local/zs-init     && rm zs-init.tar.gz
# Fri, 21 Feb 2020 23:14:10 GMT
WORKDIR /usr/local/zs-init
# Fri, 21 Feb 2020 23:14:19 GMT
RUN /usr/local/zend/bin/php -r "readfile('https://getcomposer.org/installer');" | /usr/local/zend/bin/php     && /usr/local/zend/bin/php composer.phar self-update && /usr/local/zend/bin/php composer.phar update
# Fri, 21 Feb 2020 23:14:19 GMT
COPY dir:2503294e06c787d82d501853381aa61cd4a7bf7e5f082292d4aba573b9bbf2e2 in /usr/local/bin 
# Fri, 21 Feb 2020 23:14:19 GMT
COPY dir:80bde0d50316e7c9350262fe3b75826a91d075303027787e759d703b60df13d6 in /usr/local/zend/var/plugins/ 
# Fri, 21 Feb 2020 23:14:20 GMT
RUN rm /var/www/html/index.html
# Fri, 21 Feb 2020 23:14:20 GMT
COPY dir:d174a5d34625889b4356c566972566e0ca7da618b01ea42276562f8186517a67 in /var/www/html 
# Fri, 21 Feb 2020 23:14:20 GMT
EXPOSE 80
# Fri, 21 Feb 2020 23:14:21 GMT
EXPOSE 443
# Fri, 21 Feb 2020 23:14:21 GMT
EXPOSE 10081
# Fri, 21 Feb 2020 23:14:21 GMT
EXPOSE 10082
# Fri, 21 Feb 2020 23:14:21 GMT
WORKDIR /var/www/html
# Fri, 21 Feb 2020 23:14:21 GMT
CMD ["/usr/local/bin/run"]
```

-	Layers:
	-	`sha256:fe703b657a32e0046dce0ad2cb17172cbec8ba302edf370f5f28962bdb6216a9`  
		Last Modified: Thu, 13 Feb 2020 00:25:54 GMT  
		Size: 44.2 MB (44191726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9df1fafd224fae3ba34a68dfc401f75bf6bc0c016fe36c61661ca5c7ad729ee`  
		Last Modified: Fri, 21 Feb 2020 22:23:12 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a645a4b887f9613f80fae43432e46423f196a9952d11bb620bef2add7c4ed4ee`  
		Last Modified: Fri, 21 Feb 2020 22:23:12 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57db7fe0b522b7a6069e769606e5ed0913a64e1e0d0030382a922ccf9449211e`  
		Last Modified: Fri, 21 Feb 2020 22:23:13 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b204d6c7313832d2fbd9d1bfcf5d6a080fbf7d9de9ecc28a267c8007577b71a8`  
		Last Modified: Fri, 21 Feb 2020 23:14:45 GMT  
		Size: 13.1 KB (13067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba2aba748bb9dfe89848070a5e6ad0dffff34a55a08aa898b7b6839819efcad7`  
		Last Modified: Fri, 21 Feb 2020 23:15:43 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e37fdb70d677ce5352ea1824a9f3ab255773a42c5a19b71339b25b5dfc4c6484`  
		Last Modified: Fri, 21 Feb 2020 23:16:42 GMT  
		Size: 388.3 MB (388274707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64ba0e9d2fc1f5b9b1e324ab97787a7d075b22eb7813168fe8ec1ff2de89d68e`  
		Last Modified: Fri, 21 Feb 2020 23:15:42 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93c0c1865f99c35bc58204479b99e54bc159f91b6452dd8fc1366903a66e1155`  
		Last Modified: Fri, 21 Feb 2020 23:15:42 GMT  
		Size: 261.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef11124aab853c24b171bb20f1f07175ee199616829a8c067779fa17aaf0274c`  
		Last Modified: Fri, 21 Feb 2020 23:15:41 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71802188d7e47f533e47f54f2eb797a19a96f7a4dbae115195888e95f5bae228`  
		Last Modified: Fri, 21 Feb 2020 23:15:41 GMT  
		Size: 309.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb70b45dfd6effaef6ba44b617515cffd3650ef4862034d5f7dc64d256e1b129`  
		Last Modified: Fri, 21 Feb 2020 23:15:41 GMT  
		Size: 18.8 KB (18830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77852d4170347dc2b048255b88894139c2287131c122cb574c413130843cc11c`  
		Last Modified: Fri, 21 Feb 2020 23:15:43 GMT  
		Size: 18.5 MB (18540471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41e1714d7dc5b9a46a896048f55450973c0b71c9cca2ef69e7bbf48bb08d0650`  
		Last Modified: Fri, 21 Feb 2020 23:15:40 GMT  
		Size: 14.3 KB (14297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c3afc73e381496b2f024f0a0f00c11d8bf36ab6cb3dec0cdfbf297375218508`  
		Last Modified: Fri, 21 Feb 2020 23:15:40 GMT  
		Size: 2.5 KB (2532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aba2ee3f1f05cff5b558bfe1aaa35997f558328287ada889b10ff0508e6c0dfb`  
		Last Modified: Fri, 21 Feb 2020 23:15:40 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c39ad01e225f02f840c8aa1c1fe39faa1c376756b7693a7053fab87f9ce09d22`  
		Last Modified: Fri, 21 Feb 2020 23:15:40 GMT  
		Size: 1.2 KB (1248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `php-zendserver:5.6`

```console
$ docker pull php-zendserver@sha256:bbb9a7491a390922c950cd098d811a17f48797833edceed333e53a00f26745b3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `php-zendserver:5.6` - linux; amd64

```console
$ docker pull php-zendserver@sha256:b80aff13fc04d6836765e0b3bf0d119e28bcbd873a17825c869b5ab258a1cd09
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **326.8 MB (326798099 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:65c51148750e1461de43d0754330bfa7246f3cfd15b4386b837eaaa81e111b66`
-	Default Command: `["\/usr\/local\/bin\/run"]`

```dockerfile
# Thu, 31 Oct 2019 22:21:27 GMT
ADD file:9511990749b593a6f98fcc4d7dfe03df7b2c79be69f7a9ea96b52a6a8065829d in / 
# Thu, 31 Oct 2019 22:21:28 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 22:21:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 31 Oct 2019 22:21:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 31 Oct 2019 22:21:29 GMT
CMD ["/bin/bash"]
# Thu, 31 Oct 2019 23:20:40 GMT
RUN apt-key adv --keyserver keyserver.ubuntu.com --recv-key 799058698E65316A2E7A4FF42EAE1437F7D2C623
# Thu, 14 Nov 2019 00:20:20 GMT
COPY file:6f0a5450842ae9c3e06d131c7180961d773ca33754e17af8ea2ac258fd0c6054 in /etc/apt/sources.list.d/zend-server.list 
# Thu, 14 Nov 2019 00:22:27 GMT
RUN apt-get update     && apt-get install -y         curl         libmysqlclient20         unzip         git         zend-server-php-5.6=8.5.15+b8     && rm -rf /var/lib/apt/lists/*     && /usr/local/zend/bin/zendctl.sh stop
# Thu, 14 Nov 2019 00:22:28 GMT
COPY file:26009fd1b91c8a82cfe83d983f9357a5914e70e1b464baf9d4d99dd284c5f310 in /etc/zend.lic 
# Thu, 14 Nov 2019 00:22:28 GMT
COPY file:def46bbc651bcb61f92bcaa2f8d6edec0c22e51e86132fabd2e47542dcbec0bf in /etc/apache2/conf-available 
# Thu, 14 Nov 2019 00:22:28 GMT
RUN /usr/sbin/a2enconf drop-http-proxy-header
# Thu, 14 Nov 2019 00:22:29 GMT
RUN /usr/sbin/a2enmod headers
# Thu, 14 Nov 2019 00:22:29 GMT
ENV ZS_INIT_VERSION=0.3
# Thu, 14 Nov 2019 00:22:29 GMT
ENV ZS_INIT_SHA256=e8d441d8503808e9fc0fafc762b2cb80d4a6e68b94fede0fe41efdeac10800cb
# Thu, 14 Nov 2019 00:22:30 GMT
RUN curl -fSL -o zs-init.tar.gz "http://repos.zend.com/zs-init/zs-init-docker-${ZS_INIT_VERSION}.tar.gz"     && echo "${ZS_INIT_SHA256} *zs-init.tar.gz" | sha256sum -c -     && mkdir /usr/local/zs-init     && tar xzf zs-init.tar.gz --strip-components=1 -C /usr/local/zs-init     && rm zs-init.tar.gz
# Thu, 14 Nov 2019 00:22:30 GMT
WORKDIR /usr/local/zs-init
# Thu, 14 Nov 2019 00:22:43 GMT
RUN /usr/local/zend/bin/php -r "readfile('https://getcomposer.org/installer');" | /usr/local/zend/bin/php     && /usr/local/zend/bin/php composer.phar self-update && /usr/local/zend/bin/php composer.phar update
# Thu, 14 Nov 2019 00:22:43 GMT
COPY dir:b75978d6e77900379bb898c52c86c408d7f6fcd06b5c66439d594a1a3dcca0b4 in /usr/local/bin 
# Thu, 14 Nov 2019 00:22:43 GMT
COPY dir:80bde0d50316e7c9350262fe3b75826a91d075303027787e759d703b60df13d6 in /usr/local/zend/var/plugins/ 
# Thu, 14 Nov 2019 00:22:44 GMT
RUN rm /var/www/html/index.html
# Thu, 14 Nov 2019 00:22:44 GMT
COPY dir:d174a5d34625889b4356c566972566e0ca7da618b01ea42276562f8186517a67 in /var/www/html 
# Thu, 14 Nov 2019 00:22:44 GMT
EXPOSE 80
# Thu, 14 Nov 2019 00:22:44 GMT
EXPOSE 443
# Thu, 14 Nov 2019 00:22:45 GMT
EXPOSE 10081
# Thu, 14 Nov 2019 00:22:45 GMT
EXPOSE 10082
# Thu, 14 Nov 2019 00:22:45 GMT
WORKDIR /var/www/html
# Thu, 14 Nov 2019 00:22:45 GMT
CMD ["/usr/local/bin/run"]
```

-	Layers:
	-	`sha256:e80174c8b43b97abb6bf8901cc5dade4897f16eb53b12674bef1eae6ae847451`  
		Last Modified: Fri, 25 Oct 2019 13:19:57 GMT  
		Size: 44.1 MB (44144090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1072db285cc5eb2f3415891381631501b3ad9b1a10da20ca2e932d7d8799988`  
		Last Modified: Thu, 31 Oct 2019 22:22:11 GMT  
		Size: 529.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:858453671e6769806e0374869acce1d9e5d97f5020f86139e0862c7ada6da621`  
		Last Modified: Thu, 31 Oct 2019 22:22:11 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d07b1124f982f6c5da7f1b85a0a12f9574d6ce7e8a84160cda939e5b3a1faad`  
		Last Modified: Thu, 31 Oct 2019 22:22:12 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dd3bbfd00fc5ebd5580e5dfd7dc67648bbcc3cbc8f8586a394d4b89969aa0c6`  
		Last Modified: Thu, 31 Oct 2019 23:23:59 GMT  
		Size: 13.1 KB (13063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd7972c5c39e76a6fdbdc6d5e90d930cccb5aa1e0e9f8529690b98eb280d0b26`  
		Last Modified: Thu, 14 Nov 2019 00:26:44 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfe8dd0f16945d688c966dec9449ef3f73a319a9dbd6ccd3f2e28326ca637493`  
		Last Modified: Thu, 14 Nov 2019 00:27:29 GMT  
		Size: 264.9 MB (264904384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcd4d7480dbc2d58ef5f8c4a69b6de56d692f59963d30158e1a899fe72a41120`  
		Last Modified: Thu, 14 Nov 2019 00:26:43 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b155b3f501aaeb3cc3871015dff62f7b49f5b9928548ddadc795a3b492db9de`  
		Last Modified: Thu, 14 Nov 2019 00:26:42 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af2f02cc12ca4f17b2825985d493a5a9a95125d6ff5262a6572f0122bb460c25`  
		Last Modified: Thu, 14 Nov 2019 00:26:42 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64ca72af1425b49468aa1fae6a9a91cde43a5e896d2b9c16c5656f909732391c`  
		Last Modified: Thu, 14 Nov 2019 00:26:41 GMT  
		Size: 311.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06f1d93fc7adaf787aa32bbccb68c90913a77b7bbde22db778828bcbd9d73265`  
		Last Modified: Thu, 14 Nov 2019 00:26:41 GMT  
		Size: 18.8 KB (18833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dbf33622c3d1f3e246893576f0151054aed62f7864d61008eff7a83ca82e4db`  
		Last Modified: Thu, 14 Nov 2019 00:26:47 GMT  
		Size: 17.7 MB (17697521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4af76157de133e460fba6e093ed9fc74c05479db62927c2f76751121f5e5061`  
		Last Modified: Thu, 14 Nov 2019 00:26:39 GMT  
		Size: 13.4 KB (13357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c06bff2bb16526527cc8ec197bec93c56cbe184c29dd52d6e170f05444154a9`  
		Last Modified: Thu, 14 Nov 2019 00:26:39 GMT  
		Size: 2.5 KB (2535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:336d2aba8e1ea88e8aef42f6901a3d1a092a0e94c330038d6ef3997ce4c87cfc`  
		Last Modified: Thu, 14 Nov 2019 00:26:39 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3da0598932e21f2fd138c2b6f79e3a559ecd8411b17cc5904e518ae24ff9bd39`  
		Last Modified: Thu, 14 Nov 2019 00:26:39 GMT  
		Size: 1.2 KB (1249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `php-zendserver:8.5`

```console
$ docker pull php-zendserver@sha256:bbb9a7491a390922c950cd098d811a17f48797833edceed333e53a00f26745b3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `php-zendserver:8.5` - linux; amd64

```console
$ docker pull php-zendserver@sha256:b80aff13fc04d6836765e0b3bf0d119e28bcbd873a17825c869b5ab258a1cd09
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **326.8 MB (326798099 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:65c51148750e1461de43d0754330bfa7246f3cfd15b4386b837eaaa81e111b66`
-	Default Command: `["\/usr\/local\/bin\/run"]`

```dockerfile
# Thu, 31 Oct 2019 22:21:27 GMT
ADD file:9511990749b593a6f98fcc4d7dfe03df7b2c79be69f7a9ea96b52a6a8065829d in / 
# Thu, 31 Oct 2019 22:21:28 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 22:21:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 31 Oct 2019 22:21:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 31 Oct 2019 22:21:29 GMT
CMD ["/bin/bash"]
# Thu, 31 Oct 2019 23:20:40 GMT
RUN apt-key adv --keyserver keyserver.ubuntu.com --recv-key 799058698E65316A2E7A4FF42EAE1437F7D2C623
# Thu, 14 Nov 2019 00:20:20 GMT
COPY file:6f0a5450842ae9c3e06d131c7180961d773ca33754e17af8ea2ac258fd0c6054 in /etc/apt/sources.list.d/zend-server.list 
# Thu, 14 Nov 2019 00:22:27 GMT
RUN apt-get update     && apt-get install -y         curl         libmysqlclient20         unzip         git         zend-server-php-5.6=8.5.15+b8     && rm -rf /var/lib/apt/lists/*     && /usr/local/zend/bin/zendctl.sh stop
# Thu, 14 Nov 2019 00:22:28 GMT
COPY file:26009fd1b91c8a82cfe83d983f9357a5914e70e1b464baf9d4d99dd284c5f310 in /etc/zend.lic 
# Thu, 14 Nov 2019 00:22:28 GMT
COPY file:def46bbc651bcb61f92bcaa2f8d6edec0c22e51e86132fabd2e47542dcbec0bf in /etc/apache2/conf-available 
# Thu, 14 Nov 2019 00:22:28 GMT
RUN /usr/sbin/a2enconf drop-http-proxy-header
# Thu, 14 Nov 2019 00:22:29 GMT
RUN /usr/sbin/a2enmod headers
# Thu, 14 Nov 2019 00:22:29 GMT
ENV ZS_INIT_VERSION=0.3
# Thu, 14 Nov 2019 00:22:29 GMT
ENV ZS_INIT_SHA256=e8d441d8503808e9fc0fafc762b2cb80d4a6e68b94fede0fe41efdeac10800cb
# Thu, 14 Nov 2019 00:22:30 GMT
RUN curl -fSL -o zs-init.tar.gz "http://repos.zend.com/zs-init/zs-init-docker-${ZS_INIT_VERSION}.tar.gz"     && echo "${ZS_INIT_SHA256} *zs-init.tar.gz" | sha256sum -c -     && mkdir /usr/local/zs-init     && tar xzf zs-init.tar.gz --strip-components=1 -C /usr/local/zs-init     && rm zs-init.tar.gz
# Thu, 14 Nov 2019 00:22:30 GMT
WORKDIR /usr/local/zs-init
# Thu, 14 Nov 2019 00:22:43 GMT
RUN /usr/local/zend/bin/php -r "readfile('https://getcomposer.org/installer');" | /usr/local/zend/bin/php     && /usr/local/zend/bin/php composer.phar self-update && /usr/local/zend/bin/php composer.phar update
# Thu, 14 Nov 2019 00:22:43 GMT
COPY dir:b75978d6e77900379bb898c52c86c408d7f6fcd06b5c66439d594a1a3dcca0b4 in /usr/local/bin 
# Thu, 14 Nov 2019 00:22:43 GMT
COPY dir:80bde0d50316e7c9350262fe3b75826a91d075303027787e759d703b60df13d6 in /usr/local/zend/var/plugins/ 
# Thu, 14 Nov 2019 00:22:44 GMT
RUN rm /var/www/html/index.html
# Thu, 14 Nov 2019 00:22:44 GMT
COPY dir:d174a5d34625889b4356c566972566e0ca7da618b01ea42276562f8186517a67 in /var/www/html 
# Thu, 14 Nov 2019 00:22:44 GMT
EXPOSE 80
# Thu, 14 Nov 2019 00:22:44 GMT
EXPOSE 443
# Thu, 14 Nov 2019 00:22:45 GMT
EXPOSE 10081
# Thu, 14 Nov 2019 00:22:45 GMT
EXPOSE 10082
# Thu, 14 Nov 2019 00:22:45 GMT
WORKDIR /var/www/html
# Thu, 14 Nov 2019 00:22:45 GMT
CMD ["/usr/local/bin/run"]
```

-	Layers:
	-	`sha256:e80174c8b43b97abb6bf8901cc5dade4897f16eb53b12674bef1eae6ae847451`  
		Last Modified: Fri, 25 Oct 2019 13:19:57 GMT  
		Size: 44.1 MB (44144090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1072db285cc5eb2f3415891381631501b3ad9b1a10da20ca2e932d7d8799988`  
		Last Modified: Thu, 31 Oct 2019 22:22:11 GMT  
		Size: 529.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:858453671e6769806e0374869acce1d9e5d97f5020f86139e0862c7ada6da621`  
		Last Modified: Thu, 31 Oct 2019 22:22:11 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d07b1124f982f6c5da7f1b85a0a12f9574d6ce7e8a84160cda939e5b3a1faad`  
		Last Modified: Thu, 31 Oct 2019 22:22:12 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dd3bbfd00fc5ebd5580e5dfd7dc67648bbcc3cbc8f8586a394d4b89969aa0c6`  
		Last Modified: Thu, 31 Oct 2019 23:23:59 GMT  
		Size: 13.1 KB (13063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd7972c5c39e76a6fdbdc6d5e90d930cccb5aa1e0e9f8529690b98eb280d0b26`  
		Last Modified: Thu, 14 Nov 2019 00:26:44 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfe8dd0f16945d688c966dec9449ef3f73a319a9dbd6ccd3f2e28326ca637493`  
		Last Modified: Thu, 14 Nov 2019 00:27:29 GMT  
		Size: 264.9 MB (264904384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcd4d7480dbc2d58ef5f8c4a69b6de56d692f59963d30158e1a899fe72a41120`  
		Last Modified: Thu, 14 Nov 2019 00:26:43 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b155b3f501aaeb3cc3871015dff62f7b49f5b9928548ddadc795a3b492db9de`  
		Last Modified: Thu, 14 Nov 2019 00:26:42 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af2f02cc12ca4f17b2825985d493a5a9a95125d6ff5262a6572f0122bb460c25`  
		Last Modified: Thu, 14 Nov 2019 00:26:42 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64ca72af1425b49468aa1fae6a9a91cde43a5e896d2b9c16c5656f909732391c`  
		Last Modified: Thu, 14 Nov 2019 00:26:41 GMT  
		Size: 311.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06f1d93fc7adaf787aa32bbccb68c90913a77b7bbde22db778828bcbd9d73265`  
		Last Modified: Thu, 14 Nov 2019 00:26:41 GMT  
		Size: 18.8 KB (18833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dbf33622c3d1f3e246893576f0151054aed62f7864d61008eff7a83ca82e4db`  
		Last Modified: Thu, 14 Nov 2019 00:26:47 GMT  
		Size: 17.7 MB (17697521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4af76157de133e460fba6e093ed9fc74c05479db62927c2f76751121f5e5061`  
		Last Modified: Thu, 14 Nov 2019 00:26:39 GMT  
		Size: 13.4 KB (13357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c06bff2bb16526527cc8ec197bec93c56cbe184c29dd52d6e170f05444154a9`  
		Last Modified: Thu, 14 Nov 2019 00:26:39 GMT  
		Size: 2.5 KB (2535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:336d2aba8e1ea88e8aef42f6901a3d1a092a0e94c330038d6ef3997ce4c87cfc`  
		Last Modified: Thu, 14 Nov 2019 00:26:39 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3da0598932e21f2fd138c2b6f79e3a559ecd8411b17cc5904e518ae24ff9bd39`  
		Last Modified: Thu, 14 Nov 2019 00:26:39 GMT  
		Size: 1.2 KB (1249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `php-zendserver:8.5-php5.6`

```console
$ docker pull php-zendserver@sha256:bbb9a7491a390922c950cd098d811a17f48797833edceed333e53a00f26745b3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `php-zendserver:8.5-php5.6` - linux; amd64

```console
$ docker pull php-zendserver@sha256:b80aff13fc04d6836765e0b3bf0d119e28bcbd873a17825c869b5ab258a1cd09
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **326.8 MB (326798099 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:65c51148750e1461de43d0754330bfa7246f3cfd15b4386b837eaaa81e111b66`
-	Default Command: `["\/usr\/local\/bin\/run"]`

```dockerfile
# Thu, 31 Oct 2019 22:21:27 GMT
ADD file:9511990749b593a6f98fcc4d7dfe03df7b2c79be69f7a9ea96b52a6a8065829d in / 
# Thu, 31 Oct 2019 22:21:28 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 22:21:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 31 Oct 2019 22:21:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 31 Oct 2019 22:21:29 GMT
CMD ["/bin/bash"]
# Thu, 31 Oct 2019 23:20:40 GMT
RUN apt-key adv --keyserver keyserver.ubuntu.com --recv-key 799058698E65316A2E7A4FF42EAE1437F7D2C623
# Thu, 14 Nov 2019 00:20:20 GMT
COPY file:6f0a5450842ae9c3e06d131c7180961d773ca33754e17af8ea2ac258fd0c6054 in /etc/apt/sources.list.d/zend-server.list 
# Thu, 14 Nov 2019 00:22:27 GMT
RUN apt-get update     && apt-get install -y         curl         libmysqlclient20         unzip         git         zend-server-php-5.6=8.5.15+b8     && rm -rf /var/lib/apt/lists/*     && /usr/local/zend/bin/zendctl.sh stop
# Thu, 14 Nov 2019 00:22:28 GMT
COPY file:26009fd1b91c8a82cfe83d983f9357a5914e70e1b464baf9d4d99dd284c5f310 in /etc/zend.lic 
# Thu, 14 Nov 2019 00:22:28 GMT
COPY file:def46bbc651bcb61f92bcaa2f8d6edec0c22e51e86132fabd2e47542dcbec0bf in /etc/apache2/conf-available 
# Thu, 14 Nov 2019 00:22:28 GMT
RUN /usr/sbin/a2enconf drop-http-proxy-header
# Thu, 14 Nov 2019 00:22:29 GMT
RUN /usr/sbin/a2enmod headers
# Thu, 14 Nov 2019 00:22:29 GMT
ENV ZS_INIT_VERSION=0.3
# Thu, 14 Nov 2019 00:22:29 GMT
ENV ZS_INIT_SHA256=e8d441d8503808e9fc0fafc762b2cb80d4a6e68b94fede0fe41efdeac10800cb
# Thu, 14 Nov 2019 00:22:30 GMT
RUN curl -fSL -o zs-init.tar.gz "http://repos.zend.com/zs-init/zs-init-docker-${ZS_INIT_VERSION}.tar.gz"     && echo "${ZS_INIT_SHA256} *zs-init.tar.gz" | sha256sum -c -     && mkdir /usr/local/zs-init     && tar xzf zs-init.tar.gz --strip-components=1 -C /usr/local/zs-init     && rm zs-init.tar.gz
# Thu, 14 Nov 2019 00:22:30 GMT
WORKDIR /usr/local/zs-init
# Thu, 14 Nov 2019 00:22:43 GMT
RUN /usr/local/zend/bin/php -r "readfile('https://getcomposer.org/installer');" | /usr/local/zend/bin/php     && /usr/local/zend/bin/php composer.phar self-update && /usr/local/zend/bin/php composer.phar update
# Thu, 14 Nov 2019 00:22:43 GMT
COPY dir:b75978d6e77900379bb898c52c86c408d7f6fcd06b5c66439d594a1a3dcca0b4 in /usr/local/bin 
# Thu, 14 Nov 2019 00:22:43 GMT
COPY dir:80bde0d50316e7c9350262fe3b75826a91d075303027787e759d703b60df13d6 in /usr/local/zend/var/plugins/ 
# Thu, 14 Nov 2019 00:22:44 GMT
RUN rm /var/www/html/index.html
# Thu, 14 Nov 2019 00:22:44 GMT
COPY dir:d174a5d34625889b4356c566972566e0ca7da618b01ea42276562f8186517a67 in /var/www/html 
# Thu, 14 Nov 2019 00:22:44 GMT
EXPOSE 80
# Thu, 14 Nov 2019 00:22:44 GMT
EXPOSE 443
# Thu, 14 Nov 2019 00:22:45 GMT
EXPOSE 10081
# Thu, 14 Nov 2019 00:22:45 GMT
EXPOSE 10082
# Thu, 14 Nov 2019 00:22:45 GMT
WORKDIR /var/www/html
# Thu, 14 Nov 2019 00:22:45 GMT
CMD ["/usr/local/bin/run"]
```

-	Layers:
	-	`sha256:e80174c8b43b97abb6bf8901cc5dade4897f16eb53b12674bef1eae6ae847451`  
		Last Modified: Fri, 25 Oct 2019 13:19:57 GMT  
		Size: 44.1 MB (44144090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1072db285cc5eb2f3415891381631501b3ad9b1a10da20ca2e932d7d8799988`  
		Last Modified: Thu, 31 Oct 2019 22:22:11 GMT  
		Size: 529.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:858453671e6769806e0374869acce1d9e5d97f5020f86139e0862c7ada6da621`  
		Last Modified: Thu, 31 Oct 2019 22:22:11 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d07b1124f982f6c5da7f1b85a0a12f9574d6ce7e8a84160cda939e5b3a1faad`  
		Last Modified: Thu, 31 Oct 2019 22:22:12 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dd3bbfd00fc5ebd5580e5dfd7dc67648bbcc3cbc8f8586a394d4b89969aa0c6`  
		Last Modified: Thu, 31 Oct 2019 23:23:59 GMT  
		Size: 13.1 KB (13063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd7972c5c39e76a6fdbdc6d5e90d930cccb5aa1e0e9f8529690b98eb280d0b26`  
		Last Modified: Thu, 14 Nov 2019 00:26:44 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfe8dd0f16945d688c966dec9449ef3f73a319a9dbd6ccd3f2e28326ca637493`  
		Last Modified: Thu, 14 Nov 2019 00:27:29 GMT  
		Size: 264.9 MB (264904384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcd4d7480dbc2d58ef5f8c4a69b6de56d692f59963d30158e1a899fe72a41120`  
		Last Modified: Thu, 14 Nov 2019 00:26:43 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b155b3f501aaeb3cc3871015dff62f7b49f5b9928548ddadc795a3b492db9de`  
		Last Modified: Thu, 14 Nov 2019 00:26:42 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af2f02cc12ca4f17b2825985d493a5a9a95125d6ff5262a6572f0122bb460c25`  
		Last Modified: Thu, 14 Nov 2019 00:26:42 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64ca72af1425b49468aa1fae6a9a91cde43a5e896d2b9c16c5656f909732391c`  
		Last Modified: Thu, 14 Nov 2019 00:26:41 GMT  
		Size: 311.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06f1d93fc7adaf787aa32bbccb68c90913a77b7bbde22db778828bcbd9d73265`  
		Last Modified: Thu, 14 Nov 2019 00:26:41 GMT  
		Size: 18.8 KB (18833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dbf33622c3d1f3e246893576f0151054aed62f7864d61008eff7a83ca82e4db`  
		Last Modified: Thu, 14 Nov 2019 00:26:47 GMT  
		Size: 17.7 MB (17697521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4af76157de133e460fba6e093ed9fc74c05479db62927c2f76751121f5e5061`  
		Last Modified: Thu, 14 Nov 2019 00:26:39 GMT  
		Size: 13.4 KB (13357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c06bff2bb16526527cc8ec197bec93c56cbe184c29dd52d6e170f05444154a9`  
		Last Modified: Thu, 14 Nov 2019 00:26:39 GMT  
		Size: 2.5 KB (2535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:336d2aba8e1ea88e8aef42f6901a3d1a092a0e94c330038d6ef3997ce4c87cfc`  
		Last Modified: Thu, 14 Nov 2019 00:26:39 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3da0598932e21f2fd138c2b6f79e3a559ecd8411b17cc5904e518ae24ff9bd39`  
		Last Modified: Thu, 14 Nov 2019 00:26:39 GMT  
		Size: 1.2 KB (1249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `php-zendserver:9.1`

```console
$ docker pull php-zendserver@sha256:2440b411fbdd7cf8dd61622a3a63a9eea06a6467e0f30d28029786c271121992
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `php-zendserver:9.1` - linux; amd64

```console
$ docker pull php-zendserver@sha256:bb2e68dafa405da79e834b7d3e355eaa5905ebe009ebf2e6003212ae489d1ea3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **407.5 MB (407505489 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9aec08bd35c3f88042f7e728a78f69a9172b415476374572f5c204304b0b01b`
-	Default Command: `["\/usr\/local\/bin\/run"]`

```dockerfile
# Fri, 24 Apr 2020 01:08:29 GMT
ADD file:4fe14d9555e739e4d006eecb273a2f4a53e6dbe93bd0db26d5f999168b5d4114 in / 
# Fri, 24 Apr 2020 01:08:31 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 01:08:33 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Apr 2020 01:08:35 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Apr 2020 01:08:35 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 20:36:11 GMT
RUN apt-key adv --keyserver keyserver.ubuntu.com --recv-key 799058698E65316A2E7A4FF42EAE1437F7D2C623
# Fri, 24 Apr 2020 20:36:11 GMT
COPY file:0d4830b5060fb75cec6a47b30d343d82f9c3d6f95f20c11635618b93dedb5720 in /etc/apt/sources.list.d/zend-server.list 
# Fri, 24 Apr 2020 20:37:43 GMT
RUN apt-get update     && apt-get install -y       curl       libmysqlclient20       unzip       git       zend-server-php-7.1=9.1.10+b202     && rm -rf /var/lib/apt/lists/*     && /usr/local/zend/bin/zendctl.sh stop
# Fri, 24 Apr 2020 20:37:44 GMT
COPY file:26009fd1b91c8a82cfe83d983f9357a5914e70e1b464baf9d4d99dd284c5f310 in /etc/zend.lic 
# Fri, 24 Apr 2020 20:37:44 GMT
COPY file:def46bbc651bcb61f92bcaa2f8d6edec0c22e51e86132fabd2e47542dcbec0bf in /etc/apache2/conf-available 
# Fri, 24 Apr 2020 20:37:45 GMT
RUN /usr/sbin/a2enconf drop-http-proxy-header
# Fri, 24 Apr 2020 20:37:46 GMT
RUN /usr/sbin/a2enmod headers
# Fri, 24 Apr 2020 20:37:46 GMT
ENV ZS_INIT_VERSION=0.3
# Fri, 24 Apr 2020 20:37:46 GMT
ENV ZS_INIT_SHA256=e8d441d8503808e9fc0fafc762b2cb80d4a6e68b94fede0fe41efdeac10800cb
# Fri, 24 Apr 2020 20:37:47 GMT
RUN curl -fSL -o zs-init.tar.gz "http://repos.zend.com/zs-init/zs-init-docker-${ZS_INIT_VERSION}.tar.gz"     && echo "${ZS_INIT_SHA256} *zs-init.tar.gz" | sha256sum -c -     && mkdir /usr/local/zs-init     && tar xzf zs-init.tar.gz --strip-components=1 -C /usr/local/zs-init     && rm zs-init.tar.gz
# Fri, 24 Apr 2020 20:37:47 GMT
WORKDIR /usr/local/zs-init
# Fri, 24 Apr 2020 20:37:57 GMT
RUN /usr/local/zend/bin/php -r "readfile('https://getcomposer.org/installer');" | /usr/local/zend/bin/php     && /usr/local/zend/bin/php composer.phar self-update && /usr/local/zend/bin/php composer.phar update
# Fri, 24 Apr 2020 20:37:58 GMT
COPY dir:864637d3fa0817ce3be0c7e34e1298851fa2ea4cfb86583e2ec811f00c6a95fd in /usr/local/bin 
# Fri, 24 Apr 2020 20:37:58 GMT
COPY dir:80bde0d50316e7c9350262fe3b75826a91d075303027787e759d703b60df13d6 in /usr/local/zend/var/plugins/ 
# Fri, 24 Apr 2020 20:37:59 GMT
RUN rm /var/www/html/index.html
# Fri, 24 Apr 2020 20:37:59 GMT
COPY dir:d174a5d34625889b4356c566972566e0ca7da618b01ea42276562f8186517a67 in /var/www/html 
# Fri, 24 Apr 2020 20:37:59 GMT
EXPOSE 80
# Fri, 24 Apr 2020 20:37:59 GMT
EXPOSE 443
# Fri, 24 Apr 2020 20:37:59 GMT
EXPOSE 10081
# Fri, 24 Apr 2020 20:37:59 GMT
EXPOSE 10082
# Fri, 24 Apr 2020 20:38:00 GMT
WORKDIR /var/www/html
# Fri, 24 Apr 2020 20:38:00 GMT
CMD ["/usr/local/bin/run"]
```

-	Layers:
	-	`sha256:e92ed755c008afc1863a616a5ba743b670c09c1698f7328f05591932452a425f`  
		Last Modified: Fri, 27 Mar 2020 14:20:10 GMT  
		Size: 44.2 MB (44247132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9fd7cb1ff8f489cf082781b0e1fe0c13b840e20147e8fc8204b4592da7c2f70`  
		Last Modified: Fri, 24 Apr 2020 01:09:44 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee690f2d57a128744cf4c5b52646ad0ba7a5af113d9d7e0e02b62c06d35fd14c`  
		Last Modified: Fri, 24 Apr 2020 01:09:45 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53e3366ec435596bed2563cc882ba47ec25df6be2b1027e3243e83589c667c1e`  
		Last Modified: Fri, 24 Apr 2020 01:09:44 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57dd6efaf2106877d2c05041b9f5e7fe7da7805d9d6a416a1f30d6758d387463`  
		Last Modified: Fri, 24 Apr 2020 20:38:38 GMT  
		Size: 13.1 KB (13062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77646021918b7f46ddfe78991a6d14d2e5477d25d4325bfe689f56a3756c10c4`  
		Last Modified: Fri, 24 Apr 2020 20:38:39 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3017c8a79c77d56bebc576d9f08bd9a38a5380210344a302f6e4b3b3ee2b3bd`  
		Last Modified: Fri, 24 Apr 2020 20:39:43 GMT  
		Size: 344.1 MB (344115440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df7b0427e618e493a76d718903e012de367de6b347a14a642daf4852495b0c73`  
		Last Modified: Fri, 24 Apr 2020 20:38:38 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9ee9701de9ddd316e515a7ce7068658b213c39784dbfde63ca4ef6152ba7ab3`  
		Last Modified: Fri, 24 Apr 2020 20:38:37 GMT  
		Size: 262.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c83755288ea1de0d17060e8f5bd6245ab14db1c13530a3eac8cf44a9d93aa94a`  
		Last Modified: Fri, 24 Apr 2020 20:38:37 GMT  
		Size: 317.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c4cfc80228a7961482b1af0cf8a86fbb5c2f351c25e9a97ff73b0cb0f1cf9ca`  
		Last Modified: Fri, 24 Apr 2020 20:38:36 GMT  
		Size: 309.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c8f07f3fbe44dc20f70970813dae213cae7c17c7dd8176a0002eece435a0d3e`  
		Last Modified: Fri, 24 Apr 2020 20:38:37 GMT  
		Size: 18.8 KB (18836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ab931a89a6514956a081dde1aaa10d587c24dac57286e9947c57a16dd13608a`  
		Last Modified: Fri, 24 Apr 2020 20:38:39 GMT  
		Size: 19.1 MB (19089874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12a67962acc90a8e0daab7a044023cb5a8efda0972014b007b75040d524ac632`  
		Last Modified: Fri, 24 Apr 2020 20:38:35 GMT  
		Size: 14.3 KB (14300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6727cfad62969d5765a26d25270335bcffe56ac1c08b68b7b9444821866152d9`  
		Last Modified: Fri, 24 Apr 2020 20:38:36 GMT  
		Size: 2.5 KB (2535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1637965a8be9e1f05730e23aff3d2bc67988b6ed63c8cd58e5a9a2e3e681ecd2`  
		Last Modified: Fri, 24 Apr 2020 20:38:35 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12cf94f0851715fdbe9a83f756f91cea5f27af1ae69fccaffa5f4d41f2a00803`  
		Last Modified: Fri, 24 Apr 2020 20:38:35 GMT  
		Size: 1.3 KB (1252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `php-zendserver:latest`

```console
$ docker pull php-zendserver@sha256:48502759e5ba39d563a18c5e59721346367e60182151a062d052ed9e796613b2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `php-zendserver:latest` - linux; amd64

```console
$ docker pull php-zendserver@sha256:451493593ea52b67771e890f7e1bda545f1349e1bd6af7fdd57469a3f89ac3bf
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **451.1 MB (451059936 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f17c59a2778aa6a54dd80d1f13b1e7e9af2c159204f093d7a6443184449fc5b7`
-	Default Command: `["\/usr\/local\/bin\/run"]`

```dockerfile
# Fri, 21 Feb 2020 22:22:27 GMT
ADD file:1f70668251e2e58cee0ff0c22ee805f8a269ac6f8934c07f7e89dca6cc1de3aa in / 
# Fri, 21 Feb 2020 22:22:27 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:22:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:22:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:22:30 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 23:10:37 GMT
RUN apt-key adv --keyserver keyserver.ubuntu.com --recv-key 799058698E65316A2E7A4FF42EAE1437F7D2C623
# Fri, 21 Feb 2020 23:12:39 GMT
COPY file:64f63be6042521a7e257b6755c9344694bbe4c59cd3c677e8df3dc06c795a802 in /etc/apt/sources.list.d/zend-server.list 
# Fri, 21 Feb 2020 23:14:06 GMT
RUN apt-get update     && apt-get install -y       curl       libmysqlclient20       unzip       git       zend-server=2019.0.3+b345     && rm -rf /var/lib/apt/lists/*     && /usr/local/zend/bin/zendctl.sh stop
# Fri, 21 Feb 2020 23:14:07 GMT
COPY file:26009fd1b91c8a82cfe83d983f9357a5914e70e1b464baf9d4d99dd284c5f310 in /etc/zend.lic 
# Fri, 21 Feb 2020 23:14:07 GMT
COPY file:def46bbc651bcb61f92bcaa2f8d6edec0c22e51e86132fabd2e47542dcbec0bf in /etc/apache2/conf-available 
# Fri, 21 Feb 2020 23:14:08 GMT
RUN /usr/sbin/a2enconf drop-http-proxy-header
# Fri, 21 Feb 2020 23:14:09 GMT
RUN /usr/sbin/a2enmod headers
# Fri, 21 Feb 2020 23:14:09 GMT
ENV ZS_INIT_VERSION=0.3
# Fri, 21 Feb 2020 23:14:09 GMT
ENV ZS_INIT_SHA256=e8d441d8503808e9fc0fafc762b2cb80d4a6e68b94fede0fe41efdeac10800cb
# Fri, 21 Feb 2020 23:14:10 GMT
RUN curl -fSL -o zs-init.tar.gz "http://repos.zend.com/zs-init/zs-init-docker-${ZS_INIT_VERSION}.tar.gz"     && echo "${ZS_INIT_SHA256} *zs-init.tar.gz" | sha256sum -c -     && mkdir /usr/local/zs-init     && tar xzf zs-init.tar.gz --strip-components=1 -C /usr/local/zs-init     && rm zs-init.tar.gz
# Fri, 21 Feb 2020 23:14:10 GMT
WORKDIR /usr/local/zs-init
# Fri, 21 Feb 2020 23:14:19 GMT
RUN /usr/local/zend/bin/php -r "readfile('https://getcomposer.org/installer');" | /usr/local/zend/bin/php     && /usr/local/zend/bin/php composer.phar self-update && /usr/local/zend/bin/php composer.phar update
# Fri, 21 Feb 2020 23:14:19 GMT
COPY dir:2503294e06c787d82d501853381aa61cd4a7bf7e5f082292d4aba573b9bbf2e2 in /usr/local/bin 
# Fri, 21 Feb 2020 23:14:19 GMT
COPY dir:80bde0d50316e7c9350262fe3b75826a91d075303027787e759d703b60df13d6 in /usr/local/zend/var/plugins/ 
# Fri, 21 Feb 2020 23:14:20 GMT
RUN rm /var/www/html/index.html
# Fri, 21 Feb 2020 23:14:20 GMT
COPY dir:d174a5d34625889b4356c566972566e0ca7da618b01ea42276562f8186517a67 in /var/www/html 
# Fri, 21 Feb 2020 23:14:20 GMT
EXPOSE 80
# Fri, 21 Feb 2020 23:14:21 GMT
EXPOSE 443
# Fri, 21 Feb 2020 23:14:21 GMT
EXPOSE 10081
# Fri, 21 Feb 2020 23:14:21 GMT
EXPOSE 10082
# Fri, 21 Feb 2020 23:14:21 GMT
WORKDIR /var/www/html
# Fri, 21 Feb 2020 23:14:21 GMT
CMD ["/usr/local/bin/run"]
```

-	Layers:
	-	`sha256:fe703b657a32e0046dce0ad2cb17172cbec8ba302edf370f5f28962bdb6216a9`  
		Last Modified: Thu, 13 Feb 2020 00:25:54 GMT  
		Size: 44.2 MB (44191726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9df1fafd224fae3ba34a68dfc401f75bf6bc0c016fe36c61661ca5c7ad729ee`  
		Last Modified: Fri, 21 Feb 2020 22:23:12 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a645a4b887f9613f80fae43432e46423f196a9952d11bb620bef2add7c4ed4ee`  
		Last Modified: Fri, 21 Feb 2020 22:23:12 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57db7fe0b522b7a6069e769606e5ed0913a64e1e0d0030382a922ccf9449211e`  
		Last Modified: Fri, 21 Feb 2020 22:23:13 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b204d6c7313832d2fbd9d1bfcf5d6a080fbf7d9de9ecc28a267c8007577b71a8`  
		Last Modified: Fri, 21 Feb 2020 23:14:45 GMT  
		Size: 13.1 KB (13067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba2aba748bb9dfe89848070a5e6ad0dffff34a55a08aa898b7b6839819efcad7`  
		Last Modified: Fri, 21 Feb 2020 23:15:43 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e37fdb70d677ce5352ea1824a9f3ab255773a42c5a19b71339b25b5dfc4c6484`  
		Last Modified: Fri, 21 Feb 2020 23:16:42 GMT  
		Size: 388.3 MB (388274707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64ba0e9d2fc1f5b9b1e324ab97787a7d075b22eb7813168fe8ec1ff2de89d68e`  
		Last Modified: Fri, 21 Feb 2020 23:15:42 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93c0c1865f99c35bc58204479b99e54bc159f91b6452dd8fc1366903a66e1155`  
		Last Modified: Fri, 21 Feb 2020 23:15:42 GMT  
		Size: 261.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef11124aab853c24b171bb20f1f07175ee199616829a8c067779fa17aaf0274c`  
		Last Modified: Fri, 21 Feb 2020 23:15:41 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71802188d7e47f533e47f54f2eb797a19a96f7a4dbae115195888e95f5bae228`  
		Last Modified: Fri, 21 Feb 2020 23:15:41 GMT  
		Size: 309.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb70b45dfd6effaef6ba44b617515cffd3650ef4862034d5f7dc64d256e1b129`  
		Last Modified: Fri, 21 Feb 2020 23:15:41 GMT  
		Size: 18.8 KB (18830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77852d4170347dc2b048255b88894139c2287131c122cb574c413130843cc11c`  
		Last Modified: Fri, 21 Feb 2020 23:15:43 GMT  
		Size: 18.5 MB (18540471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41e1714d7dc5b9a46a896048f55450973c0b71c9cca2ef69e7bbf48bb08d0650`  
		Last Modified: Fri, 21 Feb 2020 23:15:40 GMT  
		Size: 14.3 KB (14297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c3afc73e381496b2f024f0a0f00c11d8bf36ab6cb3dec0cdfbf297375218508`  
		Last Modified: Fri, 21 Feb 2020 23:15:40 GMT  
		Size: 2.5 KB (2532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aba2ee3f1f05cff5b558bfe1aaa35997f558328287ada889b10ff0508e6c0dfb`  
		Last Modified: Fri, 21 Feb 2020 23:15:40 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c39ad01e225f02f840c8aa1c1fe39faa1c376756b7693a7053fab87f9ce09d22`  
		Last Modified: Fri, 21 Feb 2020 23:15:40 GMT  
		Size: 1.2 KB (1248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
