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
$ docker pull php-zendserver@sha256:949c7200c172b9ea11cb72837d11ce483145e2c68483cbde7f9816b6706ff6e8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `php-zendserver:2019.0` - linux; amd64

```console
$ docker pull php-zendserver@sha256:edc31ba72cc8bf226a0f7768ae1a9709273fcb8fe27343dd6d982b32974e2590
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **492.1 MB (492084438 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c04f6940be5a2fef39c5261b0af64efa48732b58738b71969e26deac15e1b2f`
-	Default Command: `["\/usr\/local\/bin\/run"]`

```dockerfile
# Mon, 06 Jul 2020 21:56:08 GMT
ADD file:0b40d881e3e00d68de1f1df0a565385bb838144b83814df891c994f466e9efa2 in / 
# Mon, 06 Jul 2020 21:56:09 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Mon, 06 Jul 2020 21:56:10 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 06 Jul 2020 21:56:11 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 06 Jul 2020 21:56:11 GMT
CMD ["/bin/bash"]
# Tue, 07 Jul 2020 01:36:35 GMT
RUN apt-get update && apt-get install -y       gnupg
# Tue, 07 Jul 2020 01:36:36 GMT
RUN apt-key adv --keyserver keyserver.ubuntu.com --recv-key 799058698E65316A2E7A4FF42EAE1437F7D2C623
# Tue, 07 Jul 2020 01:36:36 GMT
COPY file:23f8c2a96f087277b95ebfd7f401f5c1b95ec7f3443fa9231607566f1d8e7270 in /etc/apt/sources.list.d/zend-server.list 
# Tue, 07 Jul 2020 01:38:22 GMT
RUN apt-get update && apt-get install -y       iproute2       curl       libmysqlclient20       unzip       git       zend-server-nginx=2019.0.4+b392     && rm -rf /var/lib/apt/lists/*     && /usr/local/zend/bin/zendctl.sh stop
# Tue, 07 Jul 2020 01:38:23 GMT
ENV ZS_INIT_VERSION=0.3
# Tue, 07 Jul 2020 01:38:23 GMT
ENV ZS_INIT_SHA256=e8d441d8503808e9fc0fafc762b2cb80d4a6e68b94fede0fe41efdeac10800cb
# Tue, 07 Jul 2020 01:38:24 GMT
COPY file:ad21ce0b2dc8345be0ef63836774934d6b2045ddc3685411221a07dd10b649d1 in /tmp/zs-init.patch 
# Tue, 07 Jul 2020 01:38:24 GMT
RUN curl -fSL -o zs-init.tar.gz "http://repos.zend.com/zs-init/zs-init-docker-${ZS_INIT_VERSION}.tar.gz"     && echo "${ZS_INIT_SHA256} *zs-init.tar.gz" | sha256sum -c -     && mkdir /usr/local/zs-init     && tar xzf zs-init.tar.gz --strip-components=1 -C /usr/local/zs-init     && rm zs-init.tar.gz     && patch -u /usr/local/zs-init/src/Init/Steps/AbstractStep.php -i /tmp/zs-init.patch     && rm /tmp/zs-init.patch
# Tue, 07 Jul 2020 01:38:25 GMT
WORKDIR /usr/local/zs-init
# Wed, 08 Jul 2020 18:29:24 GMT
RUN /usr/local/zend/bin/php -r "readfile('https://getcomposer.org/installer');" | /usr/local/zend/bin/php     && /usr/local/zend/bin/php composer.phar update
# Wed, 08 Jul 2020 18:29:24 GMT
COPY dir:7937a6223a1e7805720eca1fbf8c2ccd37938f8f8aa175ae003d409459d49380 in /usr/local/bin 
# Wed, 08 Jul 2020 18:29:25 GMT
COPY dir:80bde0d50316e7c9350262fe3b75826a91d075303027787e759d703b60df13d6 in /usr/local/zend/var/plugins/ 
# Wed, 08 Jul 2020 18:29:25 GMT
RUN rm /var/www/html/index.nginx-debian.html
# Wed, 08 Jul 2020 18:29:25 GMT
COPY dir:d174a5d34625889b4356c566972566e0ca7da618b01ea42276562f8186517a67 in /var/www/html 
# Wed, 08 Jul 2020 18:29:26 GMT
EXPOSE 80
# Wed, 08 Jul 2020 18:29:26 GMT
EXPOSE 443
# Wed, 08 Jul 2020 18:29:26 GMT
EXPOSE 10081
# Wed, 08 Jul 2020 18:29:26 GMT
EXPOSE 10082
# Wed, 08 Jul 2020 18:29:26 GMT
WORKDIR /var/www/html
# Wed, 08 Jul 2020 18:29:27 GMT
CMD ["/usr/local/bin/run"]
```

-	Layers:
	-	`sha256:a1125296b23d78a3585a7910d649fbf0cc56284f9d2066e3243e8bc18f90b308`  
		Last Modified: Wed, 01 Jul 2020 12:21:40 GMT  
		Size: 26.7 MB (26696193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c742a4a0f38c95e690ad2dad8909c0cb232911418ac94a73da2a28becc7b734`  
		Last Modified: Mon, 06 Jul 2020 21:57:18 GMT  
		Size: 35.4 KB (35365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c5ea3b329965bf7239f4e4f484915a444ec6d78b532ae12525934d4f6f7ac9a`  
		Last Modified: Mon, 06 Jul 2020 21:57:19 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b4be91ead68299f53759fd80c135e0dde0eb797e91eb8fbc5a708a506e0c433`  
		Last Modified: Mon, 06 Jul 2020 21:57:19 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21a7132c9d77a7cd18c82b13e833b73aa5e638151300faffbb4b9eb3966a69e7`  
		Last Modified: Tue, 07 Jul 2020 01:40:59 GMT  
		Size: 28.1 MB (28081644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:befa7845b54db3885d58f9968b7a27ca3f22f8f826f271ab2608451fd0bb72d7`  
		Last Modified: Tue, 07 Jul 2020 01:40:56 GMT  
		Size: 1.4 KB (1385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0204dca8ce9ee79c5c0075bfebfa1b17282916808bc7917475b65ace22b12d02`  
		Last Modified: Tue, 07 Jul 2020 01:40:54 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b80c024b88fd7428da60d49c46f8188906d865dd0dee5a51ece18ec788597716`  
		Last Modified: Tue, 07 Jul 2020 01:42:01 GMT  
		Size: 417.6 MB (417550237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08cf6b5e1d6bf95cc3b5b494bddd2b75a24f308215ea4675eb018cac0812dee8`  
		Last Modified: Tue, 07 Jul 2020 01:40:54 GMT  
		Size: 445.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a654e5180bbb6a34cfff2526c4fbe5a95447e0b51deaea08717087b6881ee6ee`  
		Last Modified: Tue, 07 Jul 2020 01:40:54 GMT  
		Size: 18.9 KB (18905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f667a905d4577163b4aa9a28ec3b3517b40283571bff66de6236e799ee77719`  
		Last Modified: Wed, 08 Jul 2020 18:29:42 GMT  
		Size: 19.7 MB (19680767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c612a903487277dbc0ba78cf5566e91ddb67e38c1c69fb658a672504890b18b`  
		Last Modified: Wed, 08 Jul 2020 18:29:39 GMT  
		Size: 14.3 KB (14261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dbccc6524f2b3f202b83a2cce7ea56b6c4b587c07803534992d0b30aa83cfc5`  
		Last Modified: Wed, 08 Jul 2020 18:29:41 GMT  
		Size: 2.5 KB (2537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1569a19f8f158b5c4ff21d50d933719f55579a217671c47f86fd91a6c72241c4`  
		Last Modified: Wed, 08 Jul 2020 18:29:39 GMT  
		Size: 190.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04e8a94a8c598f71f2aad50ec084c06ecd5785bf3ce3ac3eaf226b146c30ee4e`  
		Last Modified: Wed, 08 Jul 2020 18:29:39 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `php-zendserver:5.6`

```console
$ docker pull php-zendserver@sha256:2ee1806734257df2d2f0c800991f447f0f7b17a65df3d80eae61a37b5f174456
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `php-zendserver:5.6` - linux; amd64

```console
$ docker pull php-zendserver@sha256:880499084b28721ebdf7ba4aeb8405b793f60ae74e6b07c61ff025327509b5d0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **328.0 MB (327957642 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c8191acf1602d0e8f79027b73229eae8d72afe77fa07e8ab4f712dce82d95b2`
-	Default Command: `["\/usr\/local\/bin\/run"]`

```dockerfile
# Mon, 06 Jul 2020 21:57:02 GMT
ADD file:47805a69cb7dd669e357d291ce27735c2d514348468b2d3e69c66161a4f80abd in / 
# Mon, 06 Jul 2020 21:57:03 GMT
RUN rm -rf /var/lib/apt/lists/*
# Mon, 06 Jul 2020 21:57:04 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 06 Jul 2020 21:57:04 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 06 Jul 2020 21:57:05 GMT
CMD ["/bin/bash"]
# Tue, 07 Jul 2020 01:31:29 GMT
RUN apt-key adv --keyserver keyserver.ubuntu.com --recv-key 799058698E65316A2E7A4FF42EAE1437F7D2C623
# Tue, 07 Jul 2020 01:31:30 GMT
COPY file:6f0a5450842ae9c3e06d131c7180961d773ca33754e17af8ea2ac258fd0c6054 in /etc/apt/sources.list.d/zend-server.list 
# Tue, 07 Jul 2020 01:31:30 GMT
COPY file:7a9d81c6298f71cfad4408c8b3d7c3bf53bf90083221ec55686e12b2eb6f16a4 in /etc/apt/sources.list.d/ubuntu-trusty.list 
# Tue, 07 Jul 2020 01:33:37 GMT
RUN apt-get update     && apt-get install -y         curl         libmysqlclient18         unzip         git         zend-server-php-5.6=8.5.15+b8     && rm -rf /var/lib/apt/lists/*     && /usr/local/zend/bin/zendctl.sh stop
# Tue, 07 Jul 2020 01:33:38 GMT
COPY file:def46bbc651bcb61f92bcaa2f8d6edec0c22e51e86132fabd2e47542dcbec0bf in /etc/apache2/conf-available 
# Tue, 07 Jul 2020 01:33:38 GMT
RUN /usr/sbin/a2enconf drop-http-proxy-header
# Tue, 07 Jul 2020 01:33:39 GMT
RUN /usr/sbin/a2enmod headers
# Tue, 07 Jul 2020 01:33:39 GMT
ENV ZS_INIT_VERSION=0.3
# Tue, 07 Jul 2020 01:33:40 GMT
ENV ZS_INIT_SHA256=e8d441d8503808e9fc0fafc762b2cb80d4a6e68b94fede0fe41efdeac10800cb
# Tue, 07 Jul 2020 01:33:40 GMT
RUN curl -fSL -o zs-init.tar.gz "http://repos.zend.com/zs-init/zs-init-docker-${ZS_INIT_VERSION}.tar.gz"     && echo "${ZS_INIT_SHA256} *zs-init.tar.gz" | sha256sum -c -     && mkdir /usr/local/zs-init     && tar xzf zs-init.tar.gz --strip-components=1 -C /usr/local/zs-init     && rm zs-init.tar.gz
# Tue, 07 Jul 2020 01:33:41 GMT
WORKDIR /usr/local/zs-init
# Tue, 07 Jul 2020 01:33:54 GMT
RUN /usr/local/zend/bin/php -r "readfile('https://getcomposer.org/installer');" | /usr/local/zend/bin/php     && /usr/local/zend/bin/php composer.phar self-update && /usr/local/zend/bin/php composer.phar update
# Tue, 07 Jul 2020 01:33:54 GMT
COPY dir:b75978d6e77900379bb898c52c86c408d7f6fcd06b5c66439d594a1a3dcca0b4 in /usr/local/bin 
# Tue, 07 Jul 2020 01:33:55 GMT
COPY dir:80bde0d50316e7c9350262fe3b75826a91d075303027787e759d703b60df13d6 in /usr/local/zend/var/plugins/ 
# Tue, 07 Jul 2020 01:33:55 GMT
RUN rm /var/www/html/index.html
# Tue, 07 Jul 2020 01:33:56 GMT
COPY dir:d174a5d34625889b4356c566972566e0ca7da618b01ea42276562f8186517a67 in /var/www/html 
# Tue, 07 Jul 2020 01:33:56 GMT
EXPOSE 80
# Tue, 07 Jul 2020 01:33:56 GMT
EXPOSE 443
# Tue, 07 Jul 2020 01:33:56 GMT
EXPOSE 10081
# Tue, 07 Jul 2020 01:33:56 GMT
EXPOSE 10082
# Tue, 07 Jul 2020 01:33:56 GMT
WORKDIR /var/www/html
# Tue, 07 Jul 2020 01:33:57 GMT
CMD ["/usr/local/bin/run"]
```

-	Layers:
	-	`sha256:6aa38bd67045d3ed7e7a73ca42e06fadbfd139a26693bf2dc8b9ccc318d87c3c`  
		Last Modified: Sat, 20 Jun 2020 13:20:13 GMT  
		Size: 44.4 MB (44374155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:981ae4862c056451e69578c614f07a5b552995d3fc1cf17d5dc78a26e8455d5a`  
		Last Modified: Mon, 06 Jul 2020 21:57:46 GMT  
		Size: 529.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bad8949dcb16a7693551042e056cef1e767ac0a23625a2eb9ae33ac44ac80f9`  
		Last Modified: Mon, 06 Jul 2020 21:57:46 GMT  
		Size: 846.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca9461589e708efab1c30577ec50f06db05714523e2976c7da421b0b418312e0`  
		Last Modified: Mon, 06 Jul 2020 21:57:46 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ee778a5819934066aed949f956cd3b8a649f7cee1b262c2b80ebff0dcb9e577`  
		Last Modified: Tue, 07 Jul 2020 01:38:57 GMT  
		Size: 14.7 KB (14705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:641c253ed31468457688c396343ae6a9ef7e907427979970a7e4358af9d48b49`  
		Last Modified: Tue, 07 Jul 2020 01:38:57 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:494020c078563b8a01e1038c676777db6764be607b1747e4733af5fd67fc4eda`  
		Last Modified: Tue, 07 Jul 2020 01:38:56 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26a5d4186e3c60801eb950647ebae4c74f5cb80e171025dd83e0f709eadda64c`  
		Last Modified: Tue, 07 Jul 2020 01:39:44 GMT  
		Size: 263.9 MB (263867509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2b155b0c7377f3747e29fc14cd3be7296b4484dc2bd3a27fdf3050c94ee76bb`  
		Last Modified: Tue, 07 Jul 2020 01:38:55 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fa3973e05b69c35d216761947623d0fab7e9a82b3b19bd100b2a839509f5c70`  
		Last Modified: Tue, 07 Jul 2020 01:38:55 GMT  
		Size: 317.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12a00468abadbafee8dee5b509c9d94ec2c0ab5ad1100b2b67f3716a3bb2c9db`  
		Last Modified: Tue, 07 Jul 2020 01:38:55 GMT  
		Size: 309.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a8bef849725a2d28227c2304892cba7ddc93e7bf91264824a721bcc900b1fcc`  
		Last Modified: Tue, 07 Jul 2020 01:38:54 GMT  
		Size: 18.8 KB (18832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:270fb4ef814f297ef013839a1b5ea9623266fb2abaa6a79fc89a757d630c1b46`  
		Last Modified: Tue, 07 Jul 2020 01:39:00 GMT  
		Size: 19.7 MB (19662183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b95cc201eee4775b93df891a0322aab2a03c08fbb39009efb47f510abf046c0a`  
		Last Modified: Tue, 07 Jul 2020 01:38:52 GMT  
		Size: 13.4 KB (13358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:865923cc5e44e2da0a7aba47bae4fb7a842a6e647aa8806c0203816c39aeeaa0`  
		Last Modified: Tue, 07 Jul 2020 01:38:52 GMT  
		Size: 2.5 KB (2536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcf75322260be1986fc0bcad5aa9f5adead34e666a1d4314814349d52053fab6`  
		Last Modified: Tue, 07 Jul 2020 01:38:53 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57644d6b3345e74d4e6c58afd254b2c4c9c226dcd11f15327280916b96195e95`  
		Last Modified: Tue, 07 Jul 2020 01:38:52 GMT  
		Size: 1.2 KB (1249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `php-zendserver:8.5`

```console
$ docker pull php-zendserver@sha256:2ee1806734257df2d2f0c800991f447f0f7b17a65df3d80eae61a37b5f174456
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `php-zendserver:8.5` - linux; amd64

```console
$ docker pull php-zendserver@sha256:880499084b28721ebdf7ba4aeb8405b793f60ae74e6b07c61ff025327509b5d0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **328.0 MB (327957642 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c8191acf1602d0e8f79027b73229eae8d72afe77fa07e8ab4f712dce82d95b2`
-	Default Command: `["\/usr\/local\/bin\/run"]`

```dockerfile
# Mon, 06 Jul 2020 21:57:02 GMT
ADD file:47805a69cb7dd669e357d291ce27735c2d514348468b2d3e69c66161a4f80abd in / 
# Mon, 06 Jul 2020 21:57:03 GMT
RUN rm -rf /var/lib/apt/lists/*
# Mon, 06 Jul 2020 21:57:04 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 06 Jul 2020 21:57:04 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 06 Jul 2020 21:57:05 GMT
CMD ["/bin/bash"]
# Tue, 07 Jul 2020 01:31:29 GMT
RUN apt-key adv --keyserver keyserver.ubuntu.com --recv-key 799058698E65316A2E7A4FF42EAE1437F7D2C623
# Tue, 07 Jul 2020 01:31:30 GMT
COPY file:6f0a5450842ae9c3e06d131c7180961d773ca33754e17af8ea2ac258fd0c6054 in /etc/apt/sources.list.d/zend-server.list 
# Tue, 07 Jul 2020 01:31:30 GMT
COPY file:7a9d81c6298f71cfad4408c8b3d7c3bf53bf90083221ec55686e12b2eb6f16a4 in /etc/apt/sources.list.d/ubuntu-trusty.list 
# Tue, 07 Jul 2020 01:33:37 GMT
RUN apt-get update     && apt-get install -y         curl         libmysqlclient18         unzip         git         zend-server-php-5.6=8.5.15+b8     && rm -rf /var/lib/apt/lists/*     && /usr/local/zend/bin/zendctl.sh stop
# Tue, 07 Jul 2020 01:33:38 GMT
COPY file:def46bbc651bcb61f92bcaa2f8d6edec0c22e51e86132fabd2e47542dcbec0bf in /etc/apache2/conf-available 
# Tue, 07 Jul 2020 01:33:38 GMT
RUN /usr/sbin/a2enconf drop-http-proxy-header
# Tue, 07 Jul 2020 01:33:39 GMT
RUN /usr/sbin/a2enmod headers
# Tue, 07 Jul 2020 01:33:39 GMT
ENV ZS_INIT_VERSION=0.3
# Tue, 07 Jul 2020 01:33:40 GMT
ENV ZS_INIT_SHA256=e8d441d8503808e9fc0fafc762b2cb80d4a6e68b94fede0fe41efdeac10800cb
# Tue, 07 Jul 2020 01:33:40 GMT
RUN curl -fSL -o zs-init.tar.gz "http://repos.zend.com/zs-init/zs-init-docker-${ZS_INIT_VERSION}.tar.gz"     && echo "${ZS_INIT_SHA256} *zs-init.tar.gz" | sha256sum -c -     && mkdir /usr/local/zs-init     && tar xzf zs-init.tar.gz --strip-components=1 -C /usr/local/zs-init     && rm zs-init.tar.gz
# Tue, 07 Jul 2020 01:33:41 GMT
WORKDIR /usr/local/zs-init
# Tue, 07 Jul 2020 01:33:54 GMT
RUN /usr/local/zend/bin/php -r "readfile('https://getcomposer.org/installer');" | /usr/local/zend/bin/php     && /usr/local/zend/bin/php composer.phar self-update && /usr/local/zend/bin/php composer.phar update
# Tue, 07 Jul 2020 01:33:54 GMT
COPY dir:b75978d6e77900379bb898c52c86c408d7f6fcd06b5c66439d594a1a3dcca0b4 in /usr/local/bin 
# Tue, 07 Jul 2020 01:33:55 GMT
COPY dir:80bde0d50316e7c9350262fe3b75826a91d075303027787e759d703b60df13d6 in /usr/local/zend/var/plugins/ 
# Tue, 07 Jul 2020 01:33:55 GMT
RUN rm /var/www/html/index.html
# Tue, 07 Jul 2020 01:33:56 GMT
COPY dir:d174a5d34625889b4356c566972566e0ca7da618b01ea42276562f8186517a67 in /var/www/html 
# Tue, 07 Jul 2020 01:33:56 GMT
EXPOSE 80
# Tue, 07 Jul 2020 01:33:56 GMT
EXPOSE 443
# Tue, 07 Jul 2020 01:33:56 GMT
EXPOSE 10081
# Tue, 07 Jul 2020 01:33:56 GMT
EXPOSE 10082
# Tue, 07 Jul 2020 01:33:56 GMT
WORKDIR /var/www/html
# Tue, 07 Jul 2020 01:33:57 GMT
CMD ["/usr/local/bin/run"]
```

-	Layers:
	-	`sha256:6aa38bd67045d3ed7e7a73ca42e06fadbfd139a26693bf2dc8b9ccc318d87c3c`  
		Last Modified: Sat, 20 Jun 2020 13:20:13 GMT  
		Size: 44.4 MB (44374155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:981ae4862c056451e69578c614f07a5b552995d3fc1cf17d5dc78a26e8455d5a`  
		Last Modified: Mon, 06 Jul 2020 21:57:46 GMT  
		Size: 529.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bad8949dcb16a7693551042e056cef1e767ac0a23625a2eb9ae33ac44ac80f9`  
		Last Modified: Mon, 06 Jul 2020 21:57:46 GMT  
		Size: 846.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca9461589e708efab1c30577ec50f06db05714523e2976c7da421b0b418312e0`  
		Last Modified: Mon, 06 Jul 2020 21:57:46 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ee778a5819934066aed949f956cd3b8a649f7cee1b262c2b80ebff0dcb9e577`  
		Last Modified: Tue, 07 Jul 2020 01:38:57 GMT  
		Size: 14.7 KB (14705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:641c253ed31468457688c396343ae6a9ef7e907427979970a7e4358af9d48b49`  
		Last Modified: Tue, 07 Jul 2020 01:38:57 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:494020c078563b8a01e1038c676777db6764be607b1747e4733af5fd67fc4eda`  
		Last Modified: Tue, 07 Jul 2020 01:38:56 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26a5d4186e3c60801eb950647ebae4c74f5cb80e171025dd83e0f709eadda64c`  
		Last Modified: Tue, 07 Jul 2020 01:39:44 GMT  
		Size: 263.9 MB (263867509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2b155b0c7377f3747e29fc14cd3be7296b4484dc2bd3a27fdf3050c94ee76bb`  
		Last Modified: Tue, 07 Jul 2020 01:38:55 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fa3973e05b69c35d216761947623d0fab7e9a82b3b19bd100b2a839509f5c70`  
		Last Modified: Tue, 07 Jul 2020 01:38:55 GMT  
		Size: 317.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12a00468abadbafee8dee5b509c9d94ec2c0ab5ad1100b2b67f3716a3bb2c9db`  
		Last Modified: Tue, 07 Jul 2020 01:38:55 GMT  
		Size: 309.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a8bef849725a2d28227c2304892cba7ddc93e7bf91264824a721bcc900b1fcc`  
		Last Modified: Tue, 07 Jul 2020 01:38:54 GMT  
		Size: 18.8 KB (18832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:270fb4ef814f297ef013839a1b5ea9623266fb2abaa6a79fc89a757d630c1b46`  
		Last Modified: Tue, 07 Jul 2020 01:39:00 GMT  
		Size: 19.7 MB (19662183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b95cc201eee4775b93df891a0322aab2a03c08fbb39009efb47f510abf046c0a`  
		Last Modified: Tue, 07 Jul 2020 01:38:52 GMT  
		Size: 13.4 KB (13358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:865923cc5e44e2da0a7aba47bae4fb7a842a6e647aa8806c0203816c39aeeaa0`  
		Last Modified: Tue, 07 Jul 2020 01:38:52 GMT  
		Size: 2.5 KB (2536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcf75322260be1986fc0bcad5aa9f5adead34e666a1d4314814349d52053fab6`  
		Last Modified: Tue, 07 Jul 2020 01:38:53 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57644d6b3345e74d4e6c58afd254b2c4c9c226dcd11f15327280916b96195e95`  
		Last Modified: Tue, 07 Jul 2020 01:38:52 GMT  
		Size: 1.2 KB (1249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `php-zendserver:8.5-php5.6`

```console
$ docker pull php-zendserver@sha256:2ee1806734257df2d2f0c800991f447f0f7b17a65df3d80eae61a37b5f174456
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `php-zendserver:8.5-php5.6` - linux; amd64

```console
$ docker pull php-zendserver@sha256:880499084b28721ebdf7ba4aeb8405b793f60ae74e6b07c61ff025327509b5d0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **328.0 MB (327957642 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c8191acf1602d0e8f79027b73229eae8d72afe77fa07e8ab4f712dce82d95b2`
-	Default Command: `["\/usr\/local\/bin\/run"]`

```dockerfile
# Mon, 06 Jul 2020 21:57:02 GMT
ADD file:47805a69cb7dd669e357d291ce27735c2d514348468b2d3e69c66161a4f80abd in / 
# Mon, 06 Jul 2020 21:57:03 GMT
RUN rm -rf /var/lib/apt/lists/*
# Mon, 06 Jul 2020 21:57:04 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 06 Jul 2020 21:57:04 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 06 Jul 2020 21:57:05 GMT
CMD ["/bin/bash"]
# Tue, 07 Jul 2020 01:31:29 GMT
RUN apt-key adv --keyserver keyserver.ubuntu.com --recv-key 799058698E65316A2E7A4FF42EAE1437F7D2C623
# Tue, 07 Jul 2020 01:31:30 GMT
COPY file:6f0a5450842ae9c3e06d131c7180961d773ca33754e17af8ea2ac258fd0c6054 in /etc/apt/sources.list.d/zend-server.list 
# Tue, 07 Jul 2020 01:31:30 GMT
COPY file:7a9d81c6298f71cfad4408c8b3d7c3bf53bf90083221ec55686e12b2eb6f16a4 in /etc/apt/sources.list.d/ubuntu-trusty.list 
# Tue, 07 Jul 2020 01:33:37 GMT
RUN apt-get update     && apt-get install -y         curl         libmysqlclient18         unzip         git         zend-server-php-5.6=8.5.15+b8     && rm -rf /var/lib/apt/lists/*     && /usr/local/zend/bin/zendctl.sh stop
# Tue, 07 Jul 2020 01:33:38 GMT
COPY file:def46bbc651bcb61f92bcaa2f8d6edec0c22e51e86132fabd2e47542dcbec0bf in /etc/apache2/conf-available 
# Tue, 07 Jul 2020 01:33:38 GMT
RUN /usr/sbin/a2enconf drop-http-proxy-header
# Tue, 07 Jul 2020 01:33:39 GMT
RUN /usr/sbin/a2enmod headers
# Tue, 07 Jul 2020 01:33:39 GMT
ENV ZS_INIT_VERSION=0.3
# Tue, 07 Jul 2020 01:33:40 GMT
ENV ZS_INIT_SHA256=e8d441d8503808e9fc0fafc762b2cb80d4a6e68b94fede0fe41efdeac10800cb
# Tue, 07 Jul 2020 01:33:40 GMT
RUN curl -fSL -o zs-init.tar.gz "http://repos.zend.com/zs-init/zs-init-docker-${ZS_INIT_VERSION}.tar.gz"     && echo "${ZS_INIT_SHA256} *zs-init.tar.gz" | sha256sum -c -     && mkdir /usr/local/zs-init     && tar xzf zs-init.tar.gz --strip-components=1 -C /usr/local/zs-init     && rm zs-init.tar.gz
# Tue, 07 Jul 2020 01:33:41 GMT
WORKDIR /usr/local/zs-init
# Tue, 07 Jul 2020 01:33:54 GMT
RUN /usr/local/zend/bin/php -r "readfile('https://getcomposer.org/installer');" | /usr/local/zend/bin/php     && /usr/local/zend/bin/php composer.phar self-update && /usr/local/zend/bin/php composer.phar update
# Tue, 07 Jul 2020 01:33:54 GMT
COPY dir:b75978d6e77900379bb898c52c86c408d7f6fcd06b5c66439d594a1a3dcca0b4 in /usr/local/bin 
# Tue, 07 Jul 2020 01:33:55 GMT
COPY dir:80bde0d50316e7c9350262fe3b75826a91d075303027787e759d703b60df13d6 in /usr/local/zend/var/plugins/ 
# Tue, 07 Jul 2020 01:33:55 GMT
RUN rm /var/www/html/index.html
# Tue, 07 Jul 2020 01:33:56 GMT
COPY dir:d174a5d34625889b4356c566972566e0ca7da618b01ea42276562f8186517a67 in /var/www/html 
# Tue, 07 Jul 2020 01:33:56 GMT
EXPOSE 80
# Tue, 07 Jul 2020 01:33:56 GMT
EXPOSE 443
# Tue, 07 Jul 2020 01:33:56 GMT
EXPOSE 10081
# Tue, 07 Jul 2020 01:33:56 GMT
EXPOSE 10082
# Tue, 07 Jul 2020 01:33:56 GMT
WORKDIR /var/www/html
# Tue, 07 Jul 2020 01:33:57 GMT
CMD ["/usr/local/bin/run"]
```

-	Layers:
	-	`sha256:6aa38bd67045d3ed7e7a73ca42e06fadbfd139a26693bf2dc8b9ccc318d87c3c`  
		Last Modified: Sat, 20 Jun 2020 13:20:13 GMT  
		Size: 44.4 MB (44374155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:981ae4862c056451e69578c614f07a5b552995d3fc1cf17d5dc78a26e8455d5a`  
		Last Modified: Mon, 06 Jul 2020 21:57:46 GMT  
		Size: 529.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bad8949dcb16a7693551042e056cef1e767ac0a23625a2eb9ae33ac44ac80f9`  
		Last Modified: Mon, 06 Jul 2020 21:57:46 GMT  
		Size: 846.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca9461589e708efab1c30577ec50f06db05714523e2976c7da421b0b418312e0`  
		Last Modified: Mon, 06 Jul 2020 21:57:46 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ee778a5819934066aed949f956cd3b8a649f7cee1b262c2b80ebff0dcb9e577`  
		Last Modified: Tue, 07 Jul 2020 01:38:57 GMT  
		Size: 14.7 KB (14705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:641c253ed31468457688c396343ae6a9ef7e907427979970a7e4358af9d48b49`  
		Last Modified: Tue, 07 Jul 2020 01:38:57 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:494020c078563b8a01e1038c676777db6764be607b1747e4733af5fd67fc4eda`  
		Last Modified: Tue, 07 Jul 2020 01:38:56 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26a5d4186e3c60801eb950647ebae4c74f5cb80e171025dd83e0f709eadda64c`  
		Last Modified: Tue, 07 Jul 2020 01:39:44 GMT  
		Size: 263.9 MB (263867509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2b155b0c7377f3747e29fc14cd3be7296b4484dc2bd3a27fdf3050c94ee76bb`  
		Last Modified: Tue, 07 Jul 2020 01:38:55 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fa3973e05b69c35d216761947623d0fab7e9a82b3b19bd100b2a839509f5c70`  
		Last Modified: Tue, 07 Jul 2020 01:38:55 GMT  
		Size: 317.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12a00468abadbafee8dee5b509c9d94ec2c0ab5ad1100b2b67f3716a3bb2c9db`  
		Last Modified: Tue, 07 Jul 2020 01:38:55 GMT  
		Size: 309.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a8bef849725a2d28227c2304892cba7ddc93e7bf91264824a721bcc900b1fcc`  
		Last Modified: Tue, 07 Jul 2020 01:38:54 GMT  
		Size: 18.8 KB (18832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:270fb4ef814f297ef013839a1b5ea9623266fb2abaa6a79fc89a757d630c1b46`  
		Last Modified: Tue, 07 Jul 2020 01:39:00 GMT  
		Size: 19.7 MB (19662183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b95cc201eee4775b93df891a0322aab2a03c08fbb39009efb47f510abf046c0a`  
		Last Modified: Tue, 07 Jul 2020 01:38:52 GMT  
		Size: 13.4 KB (13358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:865923cc5e44e2da0a7aba47bae4fb7a842a6e647aa8806c0203816c39aeeaa0`  
		Last Modified: Tue, 07 Jul 2020 01:38:52 GMT  
		Size: 2.5 KB (2536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcf75322260be1986fc0bcad5aa9f5adead34e666a1d4314814349d52053fab6`  
		Last Modified: Tue, 07 Jul 2020 01:38:53 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57644d6b3345e74d4e6c58afd254b2c4c9c226dcd11f15327280916b96195e95`  
		Last Modified: Tue, 07 Jul 2020 01:38:52 GMT  
		Size: 1.2 KB (1249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `php-zendserver:9.1`

```console
$ docker pull php-zendserver@sha256:6dac2e5f7265760a4424cae3c326beb91659921f431f626e54560d8954710e13
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `php-zendserver:9.1` - linux; amd64

```console
$ docker pull php-zendserver@sha256:05f32138c57772e9cbaee67425495bffe4c494b355d2a4d2edca84359fd64657
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **415.9 MB (415932540 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95b5183194ec189b94c7d41d85022420186162fa687bbdfe8646e6e22a25b67a`
-	Default Command: `["\/usr\/local\/bin\/run"]`

```dockerfile
# Mon, 06 Jul 2020 21:57:02 GMT
ADD file:47805a69cb7dd669e357d291ce27735c2d514348468b2d3e69c66161a4f80abd in / 
# Mon, 06 Jul 2020 21:57:03 GMT
RUN rm -rf /var/lib/apt/lists/*
# Mon, 06 Jul 2020 21:57:04 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 06 Jul 2020 21:57:04 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 06 Jul 2020 21:57:05 GMT
CMD ["/bin/bash"]
# Tue, 07 Jul 2020 01:31:29 GMT
RUN apt-key adv --keyserver keyserver.ubuntu.com --recv-key 799058698E65316A2E7A4FF42EAE1437F7D2C623
# Tue, 07 Jul 2020 01:34:15 GMT
COPY file:0d4830b5060fb75cec6a47b30d343d82f9c3d6f95f20c11635618b93dedb5720 in /etc/apt/sources.list.d/zend-server.list 
# Tue, 07 Jul 2020 01:35:40 GMT
RUN apt-get update     && apt-get install -y       curl       libmysqlclient20       unzip       git       zend-server-php-7.1=9.1.10+b202     && rm -rf /var/lib/apt/lists/*     && /usr/local/zend/bin/zendctl.sh stop
# Tue, 07 Jul 2020 01:35:41 GMT
COPY file:def46bbc651bcb61f92bcaa2f8d6edec0c22e51e86132fabd2e47542dcbec0bf in /etc/apache2/conf-available 
# Tue, 07 Jul 2020 01:35:42 GMT
RUN /usr/sbin/a2enconf drop-http-proxy-header
# Tue, 07 Jul 2020 01:35:43 GMT
RUN /usr/sbin/a2enmod headers
# Tue, 07 Jul 2020 01:35:43 GMT
ENV ZS_INIT_VERSION=0.3
# Tue, 07 Jul 2020 01:35:43 GMT
ENV ZS_INIT_SHA256=e8d441d8503808e9fc0fafc762b2cb80d4a6e68b94fede0fe41efdeac10800cb
# Tue, 07 Jul 2020 01:35:44 GMT
RUN curl -fSL -o zs-init.tar.gz "http://repos.zend.com/zs-init/zs-init-docker-${ZS_INIT_VERSION}.tar.gz"     && echo "${ZS_INIT_SHA256} *zs-init.tar.gz" | sha256sum -c -     && mkdir /usr/local/zs-init     && tar xzf zs-init.tar.gz --strip-components=1 -C /usr/local/zs-init     && rm zs-init.tar.gz
# Tue, 07 Jul 2020 01:35:44 GMT
WORKDIR /usr/local/zs-init
# Tue, 07 Jul 2020 01:35:56 GMT
RUN /usr/local/zend/bin/php -r "readfile('https://getcomposer.org/installer');" | /usr/local/zend/bin/php     && /usr/local/zend/bin/php composer.phar self-update && /usr/local/zend/bin/php composer.phar update
# Tue, 07 Jul 2020 01:35:56 GMT
COPY dir:864637d3fa0817ce3be0c7e34e1298851fa2ea4cfb86583e2ec811f00c6a95fd in /usr/local/bin 
# Tue, 07 Jul 2020 01:35:56 GMT
COPY dir:80bde0d50316e7c9350262fe3b75826a91d075303027787e759d703b60df13d6 in /usr/local/zend/var/plugins/ 
# Tue, 07 Jul 2020 01:35:57 GMT
RUN rm /var/www/html/index.html
# Tue, 07 Jul 2020 01:35:57 GMT
COPY dir:d174a5d34625889b4356c566972566e0ca7da618b01ea42276562f8186517a67 in /var/www/html 
# Tue, 07 Jul 2020 01:35:57 GMT
EXPOSE 80
# Tue, 07 Jul 2020 01:35:58 GMT
EXPOSE 443
# Tue, 07 Jul 2020 01:35:58 GMT
EXPOSE 10081
# Tue, 07 Jul 2020 01:35:58 GMT
EXPOSE 10082
# Tue, 07 Jul 2020 01:35:58 GMT
WORKDIR /var/www/html
# Tue, 07 Jul 2020 01:35:58 GMT
CMD ["/usr/local/bin/run"]
```

-	Layers:
	-	`sha256:6aa38bd67045d3ed7e7a73ca42e06fadbfd139a26693bf2dc8b9ccc318d87c3c`  
		Last Modified: Sat, 20 Jun 2020 13:20:13 GMT  
		Size: 44.4 MB (44374155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:981ae4862c056451e69578c614f07a5b552995d3fc1cf17d5dc78a26e8455d5a`  
		Last Modified: Mon, 06 Jul 2020 21:57:46 GMT  
		Size: 529.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bad8949dcb16a7693551042e056cef1e767ac0a23625a2eb9ae33ac44ac80f9`  
		Last Modified: Mon, 06 Jul 2020 21:57:46 GMT  
		Size: 846.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca9461589e708efab1c30577ec50f06db05714523e2976c7da421b0b418312e0`  
		Last Modified: Mon, 06 Jul 2020 21:57:46 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ee778a5819934066aed949f956cd3b8a649f7cee1b262c2b80ebff0dcb9e577`  
		Last Modified: Tue, 07 Jul 2020 01:38:57 GMT  
		Size: 14.7 KB (14705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67ac65d575aeda9e6fb90811ba5f6fe372684c8c6a0d95f6cd2c6c533b9a3e67`  
		Last Modified: Tue, 07 Jul 2020 01:39:53 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf9b801e9a4e4e6156f13d2b6228189a83ca9e108a650756fda06035d7ee7a97`  
		Last Modified: Tue, 07 Jul 2020 01:40:49 GMT  
		Size: 351.8 MB (351837241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a71ea59bf391bf695643cb53c3c73b5cb7da1514f227f789a0b1cfb6ce00651`  
		Last Modified: Tue, 07 Jul 2020 01:39:52 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59ce921977304a7cf997001b0269ae5351045fd33ea84e10a071426d9b7bc239`  
		Last Modified: Tue, 07 Jul 2020 01:39:52 GMT  
		Size: 319.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:debbff512aa01943db0f4e13f4dbeedb2fd61294bac773561e4ca0d730026651`  
		Last Modified: Tue, 07 Jul 2020 01:39:51 GMT  
		Size: 307.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d89777d8f2f11956c9bd43bc5802e951a9e07ad9b4139a3ce24f3081c5690172`  
		Last Modified: Tue, 07 Jul 2020 01:39:52 GMT  
		Size: 18.8 KB (18832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c436183296503d839f0c08b21cb197820c4841f33a8cb4072cafbb3ae2d4e6d`  
		Last Modified: Tue, 07 Jul 2020 01:39:53 GMT  
		Size: 19.7 MB (19666685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59924b8605e86d8dad4b3582b00a6c4fe69446b95dd9aed008d7f023dd7eb901`  
		Last Modified: Tue, 07 Jul 2020 01:39:50 GMT  
		Size: 14.3 KB (14303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bba6bcb00630019296e47d604fe4f2214ce8e5739ddf8cb84227c0191a7bfb2`  
		Last Modified: Tue, 07 Jul 2020 01:39:50 GMT  
		Size: 2.5 KB (2532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5648bdb5e5516e0a313808db0714ad8cd97fff880b98636fbeba2a062a5b778c`  
		Last Modified: Tue, 07 Jul 2020 01:39:51 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc851927e8ea7ad033828c06c866910331abe38f05816b51f1ee34c7cbf4d8d7`  
		Last Modified: Tue, 07 Jul 2020 01:39:50 GMT  
		Size: 1.2 KB (1250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `php-zendserver:latest`

```console
$ docker pull php-zendserver@sha256:949c7200c172b9ea11cb72837d11ce483145e2c68483cbde7f9816b6706ff6e8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `php-zendserver:latest` - linux; amd64

```console
$ docker pull php-zendserver@sha256:edc31ba72cc8bf226a0f7768ae1a9709273fcb8fe27343dd6d982b32974e2590
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **492.1 MB (492084438 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c04f6940be5a2fef39c5261b0af64efa48732b58738b71969e26deac15e1b2f`
-	Default Command: `["\/usr\/local\/bin\/run"]`

```dockerfile
# Mon, 06 Jul 2020 21:56:08 GMT
ADD file:0b40d881e3e00d68de1f1df0a565385bb838144b83814df891c994f466e9efa2 in / 
# Mon, 06 Jul 2020 21:56:09 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Mon, 06 Jul 2020 21:56:10 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 06 Jul 2020 21:56:11 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 06 Jul 2020 21:56:11 GMT
CMD ["/bin/bash"]
# Tue, 07 Jul 2020 01:36:35 GMT
RUN apt-get update && apt-get install -y       gnupg
# Tue, 07 Jul 2020 01:36:36 GMT
RUN apt-key adv --keyserver keyserver.ubuntu.com --recv-key 799058698E65316A2E7A4FF42EAE1437F7D2C623
# Tue, 07 Jul 2020 01:36:36 GMT
COPY file:23f8c2a96f087277b95ebfd7f401f5c1b95ec7f3443fa9231607566f1d8e7270 in /etc/apt/sources.list.d/zend-server.list 
# Tue, 07 Jul 2020 01:38:22 GMT
RUN apt-get update && apt-get install -y       iproute2       curl       libmysqlclient20       unzip       git       zend-server-nginx=2019.0.4+b392     && rm -rf /var/lib/apt/lists/*     && /usr/local/zend/bin/zendctl.sh stop
# Tue, 07 Jul 2020 01:38:23 GMT
ENV ZS_INIT_VERSION=0.3
# Tue, 07 Jul 2020 01:38:23 GMT
ENV ZS_INIT_SHA256=e8d441d8503808e9fc0fafc762b2cb80d4a6e68b94fede0fe41efdeac10800cb
# Tue, 07 Jul 2020 01:38:24 GMT
COPY file:ad21ce0b2dc8345be0ef63836774934d6b2045ddc3685411221a07dd10b649d1 in /tmp/zs-init.patch 
# Tue, 07 Jul 2020 01:38:24 GMT
RUN curl -fSL -o zs-init.tar.gz "http://repos.zend.com/zs-init/zs-init-docker-${ZS_INIT_VERSION}.tar.gz"     && echo "${ZS_INIT_SHA256} *zs-init.tar.gz" | sha256sum -c -     && mkdir /usr/local/zs-init     && tar xzf zs-init.tar.gz --strip-components=1 -C /usr/local/zs-init     && rm zs-init.tar.gz     && patch -u /usr/local/zs-init/src/Init/Steps/AbstractStep.php -i /tmp/zs-init.patch     && rm /tmp/zs-init.patch
# Tue, 07 Jul 2020 01:38:25 GMT
WORKDIR /usr/local/zs-init
# Wed, 08 Jul 2020 18:29:24 GMT
RUN /usr/local/zend/bin/php -r "readfile('https://getcomposer.org/installer');" | /usr/local/zend/bin/php     && /usr/local/zend/bin/php composer.phar update
# Wed, 08 Jul 2020 18:29:24 GMT
COPY dir:7937a6223a1e7805720eca1fbf8c2ccd37938f8f8aa175ae003d409459d49380 in /usr/local/bin 
# Wed, 08 Jul 2020 18:29:25 GMT
COPY dir:80bde0d50316e7c9350262fe3b75826a91d075303027787e759d703b60df13d6 in /usr/local/zend/var/plugins/ 
# Wed, 08 Jul 2020 18:29:25 GMT
RUN rm /var/www/html/index.nginx-debian.html
# Wed, 08 Jul 2020 18:29:25 GMT
COPY dir:d174a5d34625889b4356c566972566e0ca7da618b01ea42276562f8186517a67 in /var/www/html 
# Wed, 08 Jul 2020 18:29:26 GMT
EXPOSE 80
# Wed, 08 Jul 2020 18:29:26 GMT
EXPOSE 443
# Wed, 08 Jul 2020 18:29:26 GMT
EXPOSE 10081
# Wed, 08 Jul 2020 18:29:26 GMT
EXPOSE 10082
# Wed, 08 Jul 2020 18:29:26 GMT
WORKDIR /var/www/html
# Wed, 08 Jul 2020 18:29:27 GMT
CMD ["/usr/local/bin/run"]
```

-	Layers:
	-	`sha256:a1125296b23d78a3585a7910d649fbf0cc56284f9d2066e3243e8bc18f90b308`  
		Last Modified: Wed, 01 Jul 2020 12:21:40 GMT  
		Size: 26.7 MB (26696193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c742a4a0f38c95e690ad2dad8909c0cb232911418ac94a73da2a28becc7b734`  
		Last Modified: Mon, 06 Jul 2020 21:57:18 GMT  
		Size: 35.4 KB (35365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c5ea3b329965bf7239f4e4f484915a444ec6d78b532ae12525934d4f6f7ac9a`  
		Last Modified: Mon, 06 Jul 2020 21:57:19 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b4be91ead68299f53759fd80c135e0dde0eb797e91eb8fbc5a708a506e0c433`  
		Last Modified: Mon, 06 Jul 2020 21:57:19 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21a7132c9d77a7cd18c82b13e833b73aa5e638151300faffbb4b9eb3966a69e7`  
		Last Modified: Tue, 07 Jul 2020 01:40:59 GMT  
		Size: 28.1 MB (28081644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:befa7845b54db3885d58f9968b7a27ca3f22f8f826f271ab2608451fd0bb72d7`  
		Last Modified: Tue, 07 Jul 2020 01:40:56 GMT  
		Size: 1.4 KB (1385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0204dca8ce9ee79c5c0075bfebfa1b17282916808bc7917475b65ace22b12d02`  
		Last Modified: Tue, 07 Jul 2020 01:40:54 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b80c024b88fd7428da60d49c46f8188906d865dd0dee5a51ece18ec788597716`  
		Last Modified: Tue, 07 Jul 2020 01:42:01 GMT  
		Size: 417.6 MB (417550237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08cf6b5e1d6bf95cc3b5b494bddd2b75a24f308215ea4675eb018cac0812dee8`  
		Last Modified: Tue, 07 Jul 2020 01:40:54 GMT  
		Size: 445.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a654e5180bbb6a34cfff2526c4fbe5a95447e0b51deaea08717087b6881ee6ee`  
		Last Modified: Tue, 07 Jul 2020 01:40:54 GMT  
		Size: 18.9 KB (18905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f667a905d4577163b4aa9a28ec3b3517b40283571bff66de6236e799ee77719`  
		Last Modified: Wed, 08 Jul 2020 18:29:42 GMT  
		Size: 19.7 MB (19680767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c612a903487277dbc0ba78cf5566e91ddb67e38c1c69fb658a672504890b18b`  
		Last Modified: Wed, 08 Jul 2020 18:29:39 GMT  
		Size: 14.3 KB (14261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dbccc6524f2b3f202b83a2cce7ea56b6c4b587c07803534992d0b30aa83cfc5`  
		Last Modified: Wed, 08 Jul 2020 18:29:41 GMT  
		Size: 2.5 KB (2537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1569a19f8f158b5c4ff21d50d933719f55579a217671c47f86fd91a6c72241c4`  
		Last Modified: Wed, 08 Jul 2020 18:29:39 GMT  
		Size: 190.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04e8a94a8c598f71f2aad50ec084c06ecd5785bf3ce3ac3eaf226b146c30ee4e`  
		Last Modified: Wed, 08 Jul 2020 18:29:39 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
