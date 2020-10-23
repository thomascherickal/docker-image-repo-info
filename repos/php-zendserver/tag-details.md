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
$ docker pull php-zendserver@sha256:cb395da0d7905552f1ce7565c7e1868db998d8a8fe8acfd9b9a56a59603bdf34
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `php-zendserver:2019.0` - linux; amd64

```console
$ docker pull php-zendserver@sha256:d75325f9a5f40459077e8ac9b820d30af19c751bafdf56d7237ea6ebb18a8d4b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **492.5 MB (492497209 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:edb441f9ef1883978a1e5bb228b3e0f3542aed948c492dcfa39cb81c113840f0`
-	Default Command: `["\/usr\/local\/bin\/run"]`

```dockerfile
# Fri, 25 Sep 2020 22:33:49 GMT
ADD file:4974bb5483c392fb54a35f3799802d623d14632747493dce5feb4d435634b4ac in / 
# Fri, 25 Sep 2020 22:33:50 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 22:33:51 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 22:33:52 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 22:33:52 GMT
CMD ["/bin/bash"]
# Sat, 26 Sep 2020 01:14:21 GMT
RUN apt-get update && apt-get install -y       gnupg
# Sat, 26 Sep 2020 01:14:21 GMT
RUN apt-key adv --keyserver keyserver.ubuntu.com --recv-key 799058698E65316A2E7A4FF42EAE1437F7D2C623
# Sat, 26 Sep 2020 01:14:22 GMT
COPY file:23f8c2a96f087277b95ebfd7f401f5c1b95ec7f3443fa9231607566f1d8e7270 in /etc/apt/sources.list.d/zend-server.list 
# Sat, 26 Sep 2020 01:16:01 GMT
RUN apt-get update && apt-get install -y       iproute2       curl       libmysqlclient20       unzip       git       zend-server-nginx=2019.0.4+b392     && rm -rf /var/lib/apt/lists/*     && /usr/local/zend/bin/zendctl.sh stop
# Sat, 26 Sep 2020 01:16:01 GMT
ENV ZS_INIT_VERSION=0.3
# Sat, 26 Sep 2020 01:16:02 GMT
ENV ZS_INIT_SHA256=e8d441d8503808e9fc0fafc762b2cb80d4a6e68b94fede0fe41efdeac10800cb
# Sat, 26 Sep 2020 01:16:02 GMT
COPY file:ad21ce0b2dc8345be0ef63836774934d6b2045ddc3685411221a07dd10b649d1 in /tmp/zs-init.patch 
# Sat, 26 Sep 2020 01:16:02 GMT
RUN curl -fSL -o zs-init.tar.gz "http://repos.zend.com/zs-init/zs-init-docker-${ZS_INIT_VERSION}.tar.gz"     && echo "${ZS_INIT_SHA256} *zs-init.tar.gz" | sha256sum -c -     && mkdir /usr/local/zs-init     && tar xzf zs-init.tar.gz --strip-components=1 -C /usr/local/zs-init     && rm zs-init.tar.gz     && patch -u /usr/local/zs-init/src/Init/Steps/AbstractStep.php -i /tmp/zs-init.patch     && rm /tmp/zs-init.patch
# Sat, 26 Sep 2020 01:16:03 GMT
WORKDIR /usr/local/zs-init
# Sat, 26 Sep 2020 01:16:12 GMT
RUN /usr/local/zend/bin/php -r "readfile('https://getcomposer.org/installer');" | /usr/local/zend/bin/php     && /usr/local/zend/bin/php composer.phar update
# Sat, 26 Sep 2020 01:16:12 GMT
COPY dir:7937a6223a1e7805720eca1fbf8c2ccd37938f8f8aa175ae003d409459d49380 in /usr/local/bin 
# Sat, 26 Sep 2020 01:16:12 GMT
COPY dir:80bde0d50316e7c9350262fe3b75826a91d075303027787e759d703b60df13d6 in /usr/local/zend/var/plugins/ 
# Sat, 26 Sep 2020 01:16:13 GMT
RUN rm /var/www/html/index.nginx-debian.html
# Sat, 26 Sep 2020 01:16:13 GMT
COPY dir:d174a5d34625889b4356c566972566e0ca7da618b01ea42276562f8186517a67 in /var/www/html 
# Sat, 26 Sep 2020 01:16:13 GMT
EXPOSE 80
# Sat, 26 Sep 2020 01:16:14 GMT
EXPOSE 443
# Sat, 26 Sep 2020 01:16:14 GMT
EXPOSE 10081
# Sat, 26 Sep 2020 01:16:14 GMT
EXPOSE 10082
# Sat, 26 Sep 2020 01:16:14 GMT
WORKDIR /var/www/html
# Sat, 26 Sep 2020 01:16:14 GMT
CMD ["/usr/local/bin/run"]
```

-	Layers:
	-	`sha256:171857c49d0f5e2ebf623e6cb36a8bcad585ed0c2aa99c87a055df034c1e5848`  
		Last Modified: Tue, 22 Sep 2020 12:21:27 GMT  
		Size: 26.7 MB (26701612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:419640447d267f068d2f84a093cb13a56ce77e130877f5b8bdb4294f4a90a84f`  
		Last Modified: Fri, 25 Sep 2020 22:36:49 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61e52f862619ab016d3bcfbd78e5c7aaaa1989b4c295e6dbcacddd2d7b93e1f5`  
		Last Modified: Fri, 25 Sep 2020 22:36:49 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d25ea472f1de12f80e58430b1b7f3f00d4bc8e869d7a2936049a748508899d4`  
		Last Modified: Sat, 26 Sep 2020 01:18:37 GMT  
		Size: 28.5 MB (28531625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1aa4a20a4688fda442a588ed4d1e4ebe5e84282b635b39c7c5b845d93cf5e7c7`  
		Last Modified: Sat, 26 Sep 2020 01:18:34 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cee0e3fb707955145a7f055ecf9477f1054eec3c648fadb7607c43b28abf898c`  
		Last Modified: Sat, 26 Sep 2020 01:18:33 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:067f6ec87d1a0921a2e201d14bc871de38a28f732249323a61cfc7f7d17084a0`  
		Last Modified: Sat, 26 Sep 2020 01:19:37 GMT  
		Size: 418.1 MB (418117003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:964778aa7557739bc53d9237c77300baf80cf7325b2c7448f47a1d77f331eac0`  
		Last Modified: Sat, 26 Sep 2020 01:18:33 GMT  
		Size: 447.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d70852fa4a26d14e8fae00524ae46be5e02524d41b3de324866eabd752b4e81`  
		Last Modified: Sat, 26 Sep 2020 01:18:33 GMT  
		Size: 18.9 KB (18902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77e0177886aaf1f949cb435cc14b60fd396a5425c503020b86cf1bc645ab577f`  
		Last Modified: Sat, 26 Sep 2020 01:18:35 GMT  
		Size: 19.1 MB (19106769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:896f79fecbb3e25efe648cc2772ee81b289154679bba55316bc100b6ac0a7fc9`  
		Last Modified: Sat, 26 Sep 2020 01:18:32 GMT  
		Size: 14.3 KB (14252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cba471bd014c4ccd8e970aaa4ba565ca1ff341200a3eb2c940f062cd4fc33c36`  
		Last Modified: Sat, 26 Sep 2020 01:18:32 GMT  
		Size: 2.5 KB (2527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a18f139f66e26c7937f9ac5fa431af4460309617848cfd61ff67bcf26cf4c30a`  
		Last Modified: Sat, 26 Sep 2020 01:18:32 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4796c9744ddf7d7875ae51305b478ff0bf18021b2fdb55c352a536c1e01fda3`  
		Last Modified: Sat, 26 Sep 2020 01:18:32 GMT  
		Size: 1.3 KB (1255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `php-zendserver:5.6`

```console
$ docker pull php-zendserver@sha256:02d9d14201e1946d7dffc840a936281acc716b831bf9f53b81c2af1365dc232c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `php-zendserver:5.6` - linux; amd64

```console
$ docker pull php-zendserver@sha256:e3b5f8218d03264c98cd39297b8a068e750f0fe600da7631d686b461800dbc65
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **329.0 MB (329032990 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc39d52f0d52dca7e7b2a9eca43aa7498538cd8dba8f2f2bc756f7c992ed086e`
-	Default Command: `["\/usr\/local\/bin\/run"]`

```dockerfile
# Fri, 23 Oct 2020 17:33:08 GMT
ADD file:c1f3147c7b6710af5affd417ff822ee28df872d716003858d3d2e23d2277c981 in / 
# Fri, 23 Oct 2020 17:33:09 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 17:33:09 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 17:33:10 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 17:33:10 GMT
CMD ["/bin/bash"]
# Fri, 23 Oct 2020 18:10:30 GMT
RUN apt-key adv --keyserver keyserver.ubuntu.com --recv-key 799058698E65316A2E7A4FF42EAE1437F7D2C623
# Fri, 23 Oct 2020 18:10:30 GMT
COPY file:6f0a5450842ae9c3e06d131c7180961d773ca33754e17af8ea2ac258fd0c6054 in /etc/apt/sources.list.d/zend-server.list 
# Fri, 23 Oct 2020 18:10:30 GMT
COPY file:7a9d81c6298f71cfad4408c8b3d7c3bf53bf90083221ec55686e12b2eb6f16a4 in /etc/apt/sources.list.d/ubuntu-trusty.list 
# Fri, 23 Oct 2020 18:12:14 GMT
RUN apt-get update     && apt-get install -y         curl         libmysqlclient18         unzip         git         zend-server-php-5.6=8.5.15+b8     && rm -rf /var/lib/apt/lists/*     && /usr/local/zend/bin/zendctl.sh stop
# Fri, 23 Oct 2020 18:12:15 GMT
COPY file:def46bbc651bcb61f92bcaa2f8d6edec0c22e51e86132fabd2e47542dcbec0bf in /etc/apache2/conf-available 
# Fri, 23 Oct 2020 18:12:15 GMT
RUN /usr/sbin/a2enconf drop-http-proxy-header
# Fri, 23 Oct 2020 18:12:16 GMT
RUN /usr/sbin/a2enmod headers
# Fri, 23 Oct 2020 18:12:16 GMT
ENV ZS_INIT_VERSION=0.3
# Fri, 23 Oct 2020 18:12:17 GMT
ENV ZS_INIT_SHA256=e8d441d8503808e9fc0fafc762b2cb80d4a6e68b94fede0fe41efdeac10800cb
# Fri, 23 Oct 2020 18:12:17 GMT
RUN curl -fSL -o zs-init.tar.gz "http://repos.zend.com/zs-init/zs-init-docker-${ZS_INIT_VERSION}.tar.gz"     && echo "${ZS_INIT_SHA256} *zs-init.tar.gz" | sha256sum -c -     && mkdir /usr/local/zs-init     && tar xzf zs-init.tar.gz --strip-components=1 -C /usr/local/zs-init     && rm zs-init.tar.gz
# Fri, 23 Oct 2020 18:12:18 GMT
WORKDIR /usr/local/zs-init
# Fri, 23 Oct 2020 18:12:49 GMT
RUN /usr/local/zend/bin/php -r "readfile('https://getcomposer.org/installer');" | /usr/local/zend/bin/php     && /usr/local/zend/bin/php composer.phar self-update && /usr/local/zend/bin/php composer.phar update
# Fri, 23 Oct 2020 18:12:49 GMT
COPY dir:b75978d6e77900379bb898c52c86c408d7f6fcd06b5c66439d594a1a3dcca0b4 in /usr/local/bin 
# Fri, 23 Oct 2020 18:12:49 GMT
COPY dir:80bde0d50316e7c9350262fe3b75826a91d075303027787e759d703b60df13d6 in /usr/local/zend/var/plugins/ 
# Fri, 23 Oct 2020 18:12:50 GMT
RUN rm /var/www/html/index.html
# Fri, 23 Oct 2020 18:12:50 GMT
COPY dir:d174a5d34625889b4356c566972566e0ca7da618b01ea42276562f8186517a67 in /var/www/html 
# Fri, 23 Oct 2020 18:12:50 GMT
EXPOSE 80
# Fri, 23 Oct 2020 18:12:50 GMT
EXPOSE 443
# Fri, 23 Oct 2020 18:12:51 GMT
EXPOSE 10081
# Fri, 23 Oct 2020 18:12:51 GMT
EXPOSE 10082
# Fri, 23 Oct 2020 18:12:51 GMT
WORKDIR /var/www/html
# Fri, 23 Oct 2020 18:12:51 GMT
CMD ["/usr/local/bin/run"]
```

-	Layers:
	-	`sha256:2c11b7cecaa5d3e2a57e290921ababbfb8572b549015168d4cbd91c340d2c566`  
		Last Modified: Wed, 14 Oct 2020 13:20:30 GMT  
		Size: 45.8 MB (45825714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04637fa562525a9366f00e8f4b08d04a347bded1ee513738451ef9d42b4dfc4e`  
		Last Modified: Fri, 23 Oct 2020 17:33:48 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6e6af23a0f38c4a6511147d2a9dc06a07a7afa0669000cb62720c7eafe031ae`  
		Last Modified: Fri, 23 Oct 2020 17:33:49 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4a424de92ad71639c5cabadcdab0493e4067eb2f9cf109ffef40db178349238`  
		Last Modified: Fri, 23 Oct 2020 17:33:49 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:187900b9f5f13fb354da4f570ead845eacbb1aa0f6fdd1ae6d3d3a3b3106dfc0`  
		Last Modified: Fri, 23 Oct 2020 18:15:32 GMT  
		Size: 14.7 KB (14703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:676f83f63a0a417e40969f230d43e70c3eb83eb1ef481e9a2d0cd7397cab6631`  
		Last Modified: Fri, 23 Oct 2020 18:15:31 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c26e9146cd406ba8c90243d90c7f669ee630423114d2ec648c37fe3a45adb51a`  
		Last Modified: Fri, 23 Oct 2020 18:15:30 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac0d7203e494582d8fa0ed8b3e4ebe26bdd243f9994fb0a09588cc9f6abdeeba`  
		Last Modified: Fri, 23 Oct 2020 18:16:19 GMT  
		Size: 263.9 MB (263863822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3129050734a7a34221e974fd5193003a36564c064bf4e8e1875352f8e5ec4e3`  
		Last Modified: Fri, 23 Oct 2020 18:15:29 GMT  
		Size: 263.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e53c26463e55af085f0285fd18b726af23ce2dc6c2b517a448aa446326695109`  
		Last Modified: Fri, 23 Oct 2020 18:15:29 GMT  
		Size: 315.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e2de3b257c9fcafe0dbfe449f343940c63dfecd1e00164db2b21a270416ff0f`  
		Last Modified: Fri, 23 Oct 2020 18:15:28 GMT  
		Size: 310.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26aa21347da39e4773dc5aba77ff3e4d622a23d540c7923d5b1e77b378d4af18`  
		Last Modified: Fri, 23 Oct 2020 18:15:28 GMT  
		Size: 18.8 KB (18832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a68c462f618a65e527a6ea19fd31dc357e8739c863775324b9180c804ae208b`  
		Last Modified: Fri, 23 Oct 2020 18:15:31 GMT  
		Size: 19.3 MB (19289666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5b8d8782e321c77064ac88328f20d57a126d77534eb8d306ce0df6d3ca09af1`  
		Last Modified: Fri, 23 Oct 2020 18:15:27 GMT  
		Size: 13.4 KB (13355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b708c93363fbb698c763535e45d4149f12cab110c9d759992007f9ab3dce4e97`  
		Last Modified: Fri, 23 Oct 2020 18:15:27 GMT  
		Size: 2.5 KB (2538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e22e13156c07e9949cfe6266dcabd660b0523bc5fc2cb0634151f4617d020c8`  
		Last Modified: Fri, 23 Oct 2020 18:15:27 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7da5121ccf5f79a515c740acbb142c2c53ec789955ca5e63a5f33352ef1ae893`  
		Last Modified: Fri, 23 Oct 2020 18:15:28 GMT  
		Size: 1.2 KB (1249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `php-zendserver:8.5`

```console
$ docker pull php-zendserver@sha256:02d9d14201e1946d7dffc840a936281acc716b831bf9f53b81c2af1365dc232c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `php-zendserver:8.5` - linux; amd64

```console
$ docker pull php-zendserver@sha256:e3b5f8218d03264c98cd39297b8a068e750f0fe600da7631d686b461800dbc65
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **329.0 MB (329032990 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc39d52f0d52dca7e7b2a9eca43aa7498538cd8dba8f2f2bc756f7c992ed086e`
-	Default Command: `["\/usr\/local\/bin\/run"]`

```dockerfile
# Fri, 23 Oct 2020 17:33:08 GMT
ADD file:c1f3147c7b6710af5affd417ff822ee28df872d716003858d3d2e23d2277c981 in / 
# Fri, 23 Oct 2020 17:33:09 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 17:33:09 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 17:33:10 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 17:33:10 GMT
CMD ["/bin/bash"]
# Fri, 23 Oct 2020 18:10:30 GMT
RUN apt-key adv --keyserver keyserver.ubuntu.com --recv-key 799058698E65316A2E7A4FF42EAE1437F7D2C623
# Fri, 23 Oct 2020 18:10:30 GMT
COPY file:6f0a5450842ae9c3e06d131c7180961d773ca33754e17af8ea2ac258fd0c6054 in /etc/apt/sources.list.d/zend-server.list 
# Fri, 23 Oct 2020 18:10:30 GMT
COPY file:7a9d81c6298f71cfad4408c8b3d7c3bf53bf90083221ec55686e12b2eb6f16a4 in /etc/apt/sources.list.d/ubuntu-trusty.list 
# Fri, 23 Oct 2020 18:12:14 GMT
RUN apt-get update     && apt-get install -y         curl         libmysqlclient18         unzip         git         zend-server-php-5.6=8.5.15+b8     && rm -rf /var/lib/apt/lists/*     && /usr/local/zend/bin/zendctl.sh stop
# Fri, 23 Oct 2020 18:12:15 GMT
COPY file:def46bbc651bcb61f92bcaa2f8d6edec0c22e51e86132fabd2e47542dcbec0bf in /etc/apache2/conf-available 
# Fri, 23 Oct 2020 18:12:15 GMT
RUN /usr/sbin/a2enconf drop-http-proxy-header
# Fri, 23 Oct 2020 18:12:16 GMT
RUN /usr/sbin/a2enmod headers
# Fri, 23 Oct 2020 18:12:16 GMT
ENV ZS_INIT_VERSION=0.3
# Fri, 23 Oct 2020 18:12:17 GMT
ENV ZS_INIT_SHA256=e8d441d8503808e9fc0fafc762b2cb80d4a6e68b94fede0fe41efdeac10800cb
# Fri, 23 Oct 2020 18:12:17 GMT
RUN curl -fSL -o zs-init.tar.gz "http://repos.zend.com/zs-init/zs-init-docker-${ZS_INIT_VERSION}.tar.gz"     && echo "${ZS_INIT_SHA256} *zs-init.tar.gz" | sha256sum -c -     && mkdir /usr/local/zs-init     && tar xzf zs-init.tar.gz --strip-components=1 -C /usr/local/zs-init     && rm zs-init.tar.gz
# Fri, 23 Oct 2020 18:12:18 GMT
WORKDIR /usr/local/zs-init
# Fri, 23 Oct 2020 18:12:49 GMT
RUN /usr/local/zend/bin/php -r "readfile('https://getcomposer.org/installer');" | /usr/local/zend/bin/php     && /usr/local/zend/bin/php composer.phar self-update && /usr/local/zend/bin/php composer.phar update
# Fri, 23 Oct 2020 18:12:49 GMT
COPY dir:b75978d6e77900379bb898c52c86c408d7f6fcd06b5c66439d594a1a3dcca0b4 in /usr/local/bin 
# Fri, 23 Oct 2020 18:12:49 GMT
COPY dir:80bde0d50316e7c9350262fe3b75826a91d075303027787e759d703b60df13d6 in /usr/local/zend/var/plugins/ 
# Fri, 23 Oct 2020 18:12:50 GMT
RUN rm /var/www/html/index.html
# Fri, 23 Oct 2020 18:12:50 GMT
COPY dir:d174a5d34625889b4356c566972566e0ca7da618b01ea42276562f8186517a67 in /var/www/html 
# Fri, 23 Oct 2020 18:12:50 GMT
EXPOSE 80
# Fri, 23 Oct 2020 18:12:50 GMT
EXPOSE 443
# Fri, 23 Oct 2020 18:12:51 GMT
EXPOSE 10081
# Fri, 23 Oct 2020 18:12:51 GMT
EXPOSE 10082
# Fri, 23 Oct 2020 18:12:51 GMT
WORKDIR /var/www/html
# Fri, 23 Oct 2020 18:12:51 GMT
CMD ["/usr/local/bin/run"]
```

-	Layers:
	-	`sha256:2c11b7cecaa5d3e2a57e290921ababbfb8572b549015168d4cbd91c340d2c566`  
		Last Modified: Wed, 14 Oct 2020 13:20:30 GMT  
		Size: 45.8 MB (45825714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04637fa562525a9366f00e8f4b08d04a347bded1ee513738451ef9d42b4dfc4e`  
		Last Modified: Fri, 23 Oct 2020 17:33:48 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6e6af23a0f38c4a6511147d2a9dc06a07a7afa0669000cb62720c7eafe031ae`  
		Last Modified: Fri, 23 Oct 2020 17:33:49 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4a424de92ad71639c5cabadcdab0493e4067eb2f9cf109ffef40db178349238`  
		Last Modified: Fri, 23 Oct 2020 17:33:49 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:187900b9f5f13fb354da4f570ead845eacbb1aa0f6fdd1ae6d3d3a3b3106dfc0`  
		Last Modified: Fri, 23 Oct 2020 18:15:32 GMT  
		Size: 14.7 KB (14703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:676f83f63a0a417e40969f230d43e70c3eb83eb1ef481e9a2d0cd7397cab6631`  
		Last Modified: Fri, 23 Oct 2020 18:15:31 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c26e9146cd406ba8c90243d90c7f669ee630423114d2ec648c37fe3a45adb51a`  
		Last Modified: Fri, 23 Oct 2020 18:15:30 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac0d7203e494582d8fa0ed8b3e4ebe26bdd243f9994fb0a09588cc9f6abdeeba`  
		Last Modified: Fri, 23 Oct 2020 18:16:19 GMT  
		Size: 263.9 MB (263863822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3129050734a7a34221e974fd5193003a36564c064bf4e8e1875352f8e5ec4e3`  
		Last Modified: Fri, 23 Oct 2020 18:15:29 GMT  
		Size: 263.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e53c26463e55af085f0285fd18b726af23ce2dc6c2b517a448aa446326695109`  
		Last Modified: Fri, 23 Oct 2020 18:15:29 GMT  
		Size: 315.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e2de3b257c9fcafe0dbfe449f343940c63dfecd1e00164db2b21a270416ff0f`  
		Last Modified: Fri, 23 Oct 2020 18:15:28 GMT  
		Size: 310.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26aa21347da39e4773dc5aba77ff3e4d622a23d540c7923d5b1e77b378d4af18`  
		Last Modified: Fri, 23 Oct 2020 18:15:28 GMT  
		Size: 18.8 KB (18832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a68c462f618a65e527a6ea19fd31dc357e8739c863775324b9180c804ae208b`  
		Last Modified: Fri, 23 Oct 2020 18:15:31 GMT  
		Size: 19.3 MB (19289666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5b8d8782e321c77064ac88328f20d57a126d77534eb8d306ce0df6d3ca09af1`  
		Last Modified: Fri, 23 Oct 2020 18:15:27 GMT  
		Size: 13.4 KB (13355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b708c93363fbb698c763535e45d4149f12cab110c9d759992007f9ab3dce4e97`  
		Last Modified: Fri, 23 Oct 2020 18:15:27 GMT  
		Size: 2.5 KB (2538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e22e13156c07e9949cfe6266dcabd660b0523bc5fc2cb0634151f4617d020c8`  
		Last Modified: Fri, 23 Oct 2020 18:15:27 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7da5121ccf5f79a515c740acbb142c2c53ec789955ca5e63a5f33352ef1ae893`  
		Last Modified: Fri, 23 Oct 2020 18:15:28 GMT  
		Size: 1.2 KB (1249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `php-zendserver:8.5-php5.6`

```console
$ docker pull php-zendserver@sha256:02d9d14201e1946d7dffc840a936281acc716b831bf9f53b81c2af1365dc232c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `php-zendserver:8.5-php5.6` - linux; amd64

```console
$ docker pull php-zendserver@sha256:e3b5f8218d03264c98cd39297b8a068e750f0fe600da7631d686b461800dbc65
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **329.0 MB (329032990 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc39d52f0d52dca7e7b2a9eca43aa7498538cd8dba8f2f2bc756f7c992ed086e`
-	Default Command: `["\/usr\/local\/bin\/run"]`

```dockerfile
# Fri, 23 Oct 2020 17:33:08 GMT
ADD file:c1f3147c7b6710af5affd417ff822ee28df872d716003858d3d2e23d2277c981 in / 
# Fri, 23 Oct 2020 17:33:09 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 17:33:09 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 17:33:10 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 17:33:10 GMT
CMD ["/bin/bash"]
# Fri, 23 Oct 2020 18:10:30 GMT
RUN apt-key adv --keyserver keyserver.ubuntu.com --recv-key 799058698E65316A2E7A4FF42EAE1437F7D2C623
# Fri, 23 Oct 2020 18:10:30 GMT
COPY file:6f0a5450842ae9c3e06d131c7180961d773ca33754e17af8ea2ac258fd0c6054 in /etc/apt/sources.list.d/zend-server.list 
# Fri, 23 Oct 2020 18:10:30 GMT
COPY file:7a9d81c6298f71cfad4408c8b3d7c3bf53bf90083221ec55686e12b2eb6f16a4 in /etc/apt/sources.list.d/ubuntu-trusty.list 
# Fri, 23 Oct 2020 18:12:14 GMT
RUN apt-get update     && apt-get install -y         curl         libmysqlclient18         unzip         git         zend-server-php-5.6=8.5.15+b8     && rm -rf /var/lib/apt/lists/*     && /usr/local/zend/bin/zendctl.sh stop
# Fri, 23 Oct 2020 18:12:15 GMT
COPY file:def46bbc651bcb61f92bcaa2f8d6edec0c22e51e86132fabd2e47542dcbec0bf in /etc/apache2/conf-available 
# Fri, 23 Oct 2020 18:12:15 GMT
RUN /usr/sbin/a2enconf drop-http-proxy-header
# Fri, 23 Oct 2020 18:12:16 GMT
RUN /usr/sbin/a2enmod headers
# Fri, 23 Oct 2020 18:12:16 GMT
ENV ZS_INIT_VERSION=0.3
# Fri, 23 Oct 2020 18:12:17 GMT
ENV ZS_INIT_SHA256=e8d441d8503808e9fc0fafc762b2cb80d4a6e68b94fede0fe41efdeac10800cb
# Fri, 23 Oct 2020 18:12:17 GMT
RUN curl -fSL -o zs-init.tar.gz "http://repos.zend.com/zs-init/zs-init-docker-${ZS_INIT_VERSION}.tar.gz"     && echo "${ZS_INIT_SHA256} *zs-init.tar.gz" | sha256sum -c -     && mkdir /usr/local/zs-init     && tar xzf zs-init.tar.gz --strip-components=1 -C /usr/local/zs-init     && rm zs-init.tar.gz
# Fri, 23 Oct 2020 18:12:18 GMT
WORKDIR /usr/local/zs-init
# Fri, 23 Oct 2020 18:12:49 GMT
RUN /usr/local/zend/bin/php -r "readfile('https://getcomposer.org/installer');" | /usr/local/zend/bin/php     && /usr/local/zend/bin/php composer.phar self-update && /usr/local/zend/bin/php composer.phar update
# Fri, 23 Oct 2020 18:12:49 GMT
COPY dir:b75978d6e77900379bb898c52c86c408d7f6fcd06b5c66439d594a1a3dcca0b4 in /usr/local/bin 
# Fri, 23 Oct 2020 18:12:49 GMT
COPY dir:80bde0d50316e7c9350262fe3b75826a91d075303027787e759d703b60df13d6 in /usr/local/zend/var/plugins/ 
# Fri, 23 Oct 2020 18:12:50 GMT
RUN rm /var/www/html/index.html
# Fri, 23 Oct 2020 18:12:50 GMT
COPY dir:d174a5d34625889b4356c566972566e0ca7da618b01ea42276562f8186517a67 in /var/www/html 
# Fri, 23 Oct 2020 18:12:50 GMT
EXPOSE 80
# Fri, 23 Oct 2020 18:12:50 GMT
EXPOSE 443
# Fri, 23 Oct 2020 18:12:51 GMT
EXPOSE 10081
# Fri, 23 Oct 2020 18:12:51 GMT
EXPOSE 10082
# Fri, 23 Oct 2020 18:12:51 GMT
WORKDIR /var/www/html
# Fri, 23 Oct 2020 18:12:51 GMT
CMD ["/usr/local/bin/run"]
```

-	Layers:
	-	`sha256:2c11b7cecaa5d3e2a57e290921ababbfb8572b549015168d4cbd91c340d2c566`  
		Last Modified: Wed, 14 Oct 2020 13:20:30 GMT  
		Size: 45.8 MB (45825714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04637fa562525a9366f00e8f4b08d04a347bded1ee513738451ef9d42b4dfc4e`  
		Last Modified: Fri, 23 Oct 2020 17:33:48 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6e6af23a0f38c4a6511147d2a9dc06a07a7afa0669000cb62720c7eafe031ae`  
		Last Modified: Fri, 23 Oct 2020 17:33:49 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4a424de92ad71639c5cabadcdab0493e4067eb2f9cf109ffef40db178349238`  
		Last Modified: Fri, 23 Oct 2020 17:33:49 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:187900b9f5f13fb354da4f570ead845eacbb1aa0f6fdd1ae6d3d3a3b3106dfc0`  
		Last Modified: Fri, 23 Oct 2020 18:15:32 GMT  
		Size: 14.7 KB (14703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:676f83f63a0a417e40969f230d43e70c3eb83eb1ef481e9a2d0cd7397cab6631`  
		Last Modified: Fri, 23 Oct 2020 18:15:31 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c26e9146cd406ba8c90243d90c7f669ee630423114d2ec648c37fe3a45adb51a`  
		Last Modified: Fri, 23 Oct 2020 18:15:30 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac0d7203e494582d8fa0ed8b3e4ebe26bdd243f9994fb0a09588cc9f6abdeeba`  
		Last Modified: Fri, 23 Oct 2020 18:16:19 GMT  
		Size: 263.9 MB (263863822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3129050734a7a34221e974fd5193003a36564c064bf4e8e1875352f8e5ec4e3`  
		Last Modified: Fri, 23 Oct 2020 18:15:29 GMT  
		Size: 263.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e53c26463e55af085f0285fd18b726af23ce2dc6c2b517a448aa446326695109`  
		Last Modified: Fri, 23 Oct 2020 18:15:29 GMT  
		Size: 315.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e2de3b257c9fcafe0dbfe449f343940c63dfecd1e00164db2b21a270416ff0f`  
		Last Modified: Fri, 23 Oct 2020 18:15:28 GMT  
		Size: 310.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26aa21347da39e4773dc5aba77ff3e4d622a23d540c7923d5b1e77b378d4af18`  
		Last Modified: Fri, 23 Oct 2020 18:15:28 GMT  
		Size: 18.8 KB (18832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a68c462f618a65e527a6ea19fd31dc357e8739c863775324b9180c804ae208b`  
		Last Modified: Fri, 23 Oct 2020 18:15:31 GMT  
		Size: 19.3 MB (19289666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5b8d8782e321c77064ac88328f20d57a126d77534eb8d306ce0df6d3ca09af1`  
		Last Modified: Fri, 23 Oct 2020 18:15:27 GMT  
		Size: 13.4 KB (13355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b708c93363fbb698c763535e45d4149f12cab110c9d759992007f9ab3dce4e97`  
		Last Modified: Fri, 23 Oct 2020 18:15:27 GMT  
		Size: 2.5 KB (2538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e22e13156c07e9949cfe6266dcabd660b0523bc5fc2cb0634151f4617d020c8`  
		Last Modified: Fri, 23 Oct 2020 18:15:27 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7da5121ccf5f79a515c740acbb142c2c53ec789955ca5e63a5f33352ef1ae893`  
		Last Modified: Fri, 23 Oct 2020 18:15:28 GMT  
		Size: 1.2 KB (1249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `php-zendserver:9.1`

```console
$ docker pull php-zendserver@sha256:356afc9dd799eaf23bf68920139750f1a0c1a221bdf728ca95486532fe10c83c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `php-zendserver:9.1` - linux; amd64

```console
$ docker pull php-zendserver@sha256:05230b5fb41f82a4d6012ccaa7d495013b5c747931af5179a23427a003dd40fc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **412.7 MB (412694509 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8fcc9f51e619ed2018df72ef360cc591f3fa07abc43919844f529297410dc179`
-	Default Command: `["\/usr\/local\/bin\/run"]`

```dockerfile
# Fri, 23 Oct 2020 17:33:08 GMT
ADD file:c1f3147c7b6710af5affd417ff822ee28df872d716003858d3d2e23d2277c981 in / 
# Fri, 23 Oct 2020 17:33:09 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 17:33:09 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 17:33:10 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 17:33:10 GMT
CMD ["/bin/bash"]
# Fri, 23 Oct 2020 18:10:30 GMT
RUN apt-key adv --keyserver keyserver.ubuntu.com --recv-key 799058698E65316A2E7A4FF42EAE1437F7D2C623
# Fri, 23 Oct 2020 18:13:00 GMT
COPY file:0d4830b5060fb75cec6a47b30d343d82f9c3d6f95f20c11635618b93dedb5720 in /etc/apt/sources.list.d/zend-server.list 
# Fri, 23 Oct 2020 18:14:28 GMT
RUN apt-get update     && apt-get install -y       curl       libmysqlclient20       unzip       git       zend-server-php-7.1=9.1.10+b202     && rm -rf /var/lib/apt/lists/*     && /usr/local/zend/bin/zendctl.sh stop
# Fri, 23 Oct 2020 18:14:29 GMT
COPY file:def46bbc651bcb61f92bcaa2f8d6edec0c22e51e86132fabd2e47542dcbec0bf in /etc/apache2/conf-available 
# Fri, 23 Oct 2020 18:14:30 GMT
RUN /usr/sbin/a2enconf drop-http-proxy-header
# Fri, 23 Oct 2020 18:14:31 GMT
RUN /usr/sbin/a2enmod headers
# Fri, 23 Oct 2020 18:14:31 GMT
ENV ZS_INIT_VERSION=0.3
# Fri, 23 Oct 2020 18:14:31 GMT
ENV ZS_INIT_SHA256=e8d441d8503808e9fc0fafc762b2cb80d4a6e68b94fede0fe41efdeac10800cb
# Fri, 23 Oct 2020 18:14:32 GMT
RUN curl -fSL -o zs-init.tar.gz "http://repos.zend.com/zs-init/zs-init-docker-${ZS_INIT_VERSION}.tar.gz"     && echo "${ZS_INIT_SHA256} *zs-init.tar.gz" | sha256sum -c -     && mkdir /usr/local/zs-init     && tar xzf zs-init.tar.gz --strip-components=1 -C /usr/local/zs-init     && rm zs-init.tar.gz
# Fri, 23 Oct 2020 18:14:32 GMT
WORKDIR /usr/local/zs-init
# Fri, 23 Oct 2020 18:14:59 GMT
RUN /usr/local/zend/bin/php -r "readfile('https://getcomposer.org/installer');" | /usr/local/zend/bin/php     && /usr/local/zend/bin/php composer.phar self-update && /usr/local/zend/bin/php composer.phar update
# Fri, 23 Oct 2020 18:15:00 GMT
COPY dir:864637d3fa0817ce3be0c7e34e1298851fa2ea4cfb86583e2ec811f00c6a95fd in /usr/local/bin 
# Fri, 23 Oct 2020 18:15:00 GMT
COPY dir:80bde0d50316e7c9350262fe3b75826a91d075303027787e759d703b60df13d6 in /usr/local/zend/var/plugins/ 
# Fri, 23 Oct 2020 18:15:02 GMT
RUN rm /var/www/html/index.html
# Fri, 23 Oct 2020 18:15:02 GMT
COPY dir:d174a5d34625889b4356c566972566e0ca7da618b01ea42276562f8186517a67 in /var/www/html 
# Fri, 23 Oct 2020 18:15:03 GMT
EXPOSE 80
# Fri, 23 Oct 2020 18:15:03 GMT
EXPOSE 443
# Fri, 23 Oct 2020 18:15:03 GMT
EXPOSE 10081
# Fri, 23 Oct 2020 18:15:03 GMT
EXPOSE 10082
# Fri, 23 Oct 2020 18:15:03 GMT
WORKDIR /var/www/html
# Fri, 23 Oct 2020 18:15:04 GMT
CMD ["/usr/local/bin/run"]
```

-	Layers:
	-	`sha256:2c11b7cecaa5d3e2a57e290921ababbfb8572b549015168d4cbd91c340d2c566`  
		Last Modified: Wed, 14 Oct 2020 13:20:30 GMT  
		Size: 45.8 MB (45825714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04637fa562525a9366f00e8f4b08d04a347bded1ee513738451ef9d42b4dfc4e`  
		Last Modified: Fri, 23 Oct 2020 17:33:48 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6e6af23a0f38c4a6511147d2a9dc06a07a7afa0669000cb62720c7eafe031ae`  
		Last Modified: Fri, 23 Oct 2020 17:33:49 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4a424de92ad71639c5cabadcdab0493e4067eb2f9cf109ffef40db178349238`  
		Last Modified: Fri, 23 Oct 2020 17:33:49 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:187900b9f5f13fb354da4f570ead845eacbb1aa0f6fdd1ae6d3d3a3b3106dfc0`  
		Last Modified: Fri, 23 Oct 2020 18:15:32 GMT  
		Size: 14.7 KB (14703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:087aaa13b90e037978995cf3b435f89f242e37028668b99c6e265e25561c38dd`  
		Last Modified: Fri, 23 Oct 2020 18:16:31 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee3d141e906e01e6e2c76f20dfe73785b50e4e9d52e570144a5063fe1f3074b1`  
		Last Modified: Fri, 23 Oct 2020 18:17:30 GMT  
		Size: 347.5 MB (347518346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1814a3e1883d68be1940e6750bd53b0943fe8a4e6b8d42ac0b889e70978a2ec`  
		Last Modified: Fri, 23 Oct 2020 18:16:30 GMT  
		Size: 263.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f3666474e8ec9321a446df4bd85d8431df8e9330dbf6a1d7e36b5808a8ad943`  
		Last Modified: Fri, 23 Oct 2020 18:16:29 GMT  
		Size: 317.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb42071938b44c08503fe59207bd3c2dd14f9c19a437ed058ed79c34b7732790`  
		Last Modified: Fri, 23 Oct 2020 18:16:29 GMT  
		Size: 306.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdcd2765bb967c5d10d05d3a6ef9c3a7bf62d227c425a5c31527907b724114d1`  
		Last Modified: Fri, 23 Oct 2020 18:16:29 GMT  
		Size: 18.8 KB (18834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72a86de8c615e5ed43502f348e264309a63c3e2998cc37c8719e3a90bb6414dc`  
		Last Modified: Fri, 23 Oct 2020 18:16:31 GMT  
		Size: 19.3 MB (19295993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82ab6517db25e11f457203e3fc0a75c228b6633f1558f3c07fc704192f36d998`  
		Last Modified: Fri, 23 Oct 2020 18:16:28 GMT  
		Size: 14.3 KB (14300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6240e92bc5372564e9d48516f1e3da684f7f2233ec844c6744269d2b6d384f66`  
		Last Modified: Fri, 23 Oct 2020 18:16:28 GMT  
		Size: 2.5 KB (2534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ef8155693ba99aecf0ce5d1cb575281267b31e4f4fe2a9cee9ad9b3203c2f67`  
		Last Modified: Fri, 23 Oct 2020 18:16:28 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc8ed68e459d808d2cb00ab28d2a656d4ce29c5ea3fddc494c9ea34b7b79e069`  
		Last Modified: Fri, 23 Oct 2020 18:16:28 GMT  
		Size: 1.2 KB (1250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `php-zendserver:latest`

```console
$ docker pull php-zendserver@sha256:cb395da0d7905552f1ce7565c7e1868db998d8a8fe8acfd9b9a56a59603bdf34
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `php-zendserver:latest` - linux; amd64

```console
$ docker pull php-zendserver@sha256:d75325f9a5f40459077e8ac9b820d30af19c751bafdf56d7237ea6ebb18a8d4b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **492.5 MB (492497209 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:edb441f9ef1883978a1e5bb228b3e0f3542aed948c492dcfa39cb81c113840f0`
-	Default Command: `["\/usr\/local\/bin\/run"]`

```dockerfile
# Fri, 25 Sep 2020 22:33:49 GMT
ADD file:4974bb5483c392fb54a35f3799802d623d14632747493dce5feb4d435634b4ac in / 
# Fri, 25 Sep 2020 22:33:50 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 22:33:51 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 22:33:52 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 22:33:52 GMT
CMD ["/bin/bash"]
# Sat, 26 Sep 2020 01:14:21 GMT
RUN apt-get update && apt-get install -y       gnupg
# Sat, 26 Sep 2020 01:14:21 GMT
RUN apt-key adv --keyserver keyserver.ubuntu.com --recv-key 799058698E65316A2E7A4FF42EAE1437F7D2C623
# Sat, 26 Sep 2020 01:14:22 GMT
COPY file:23f8c2a96f087277b95ebfd7f401f5c1b95ec7f3443fa9231607566f1d8e7270 in /etc/apt/sources.list.d/zend-server.list 
# Sat, 26 Sep 2020 01:16:01 GMT
RUN apt-get update && apt-get install -y       iproute2       curl       libmysqlclient20       unzip       git       zend-server-nginx=2019.0.4+b392     && rm -rf /var/lib/apt/lists/*     && /usr/local/zend/bin/zendctl.sh stop
# Sat, 26 Sep 2020 01:16:01 GMT
ENV ZS_INIT_VERSION=0.3
# Sat, 26 Sep 2020 01:16:02 GMT
ENV ZS_INIT_SHA256=e8d441d8503808e9fc0fafc762b2cb80d4a6e68b94fede0fe41efdeac10800cb
# Sat, 26 Sep 2020 01:16:02 GMT
COPY file:ad21ce0b2dc8345be0ef63836774934d6b2045ddc3685411221a07dd10b649d1 in /tmp/zs-init.patch 
# Sat, 26 Sep 2020 01:16:02 GMT
RUN curl -fSL -o zs-init.tar.gz "http://repos.zend.com/zs-init/zs-init-docker-${ZS_INIT_VERSION}.tar.gz"     && echo "${ZS_INIT_SHA256} *zs-init.tar.gz" | sha256sum -c -     && mkdir /usr/local/zs-init     && tar xzf zs-init.tar.gz --strip-components=1 -C /usr/local/zs-init     && rm zs-init.tar.gz     && patch -u /usr/local/zs-init/src/Init/Steps/AbstractStep.php -i /tmp/zs-init.patch     && rm /tmp/zs-init.patch
# Sat, 26 Sep 2020 01:16:03 GMT
WORKDIR /usr/local/zs-init
# Sat, 26 Sep 2020 01:16:12 GMT
RUN /usr/local/zend/bin/php -r "readfile('https://getcomposer.org/installer');" | /usr/local/zend/bin/php     && /usr/local/zend/bin/php composer.phar update
# Sat, 26 Sep 2020 01:16:12 GMT
COPY dir:7937a6223a1e7805720eca1fbf8c2ccd37938f8f8aa175ae003d409459d49380 in /usr/local/bin 
# Sat, 26 Sep 2020 01:16:12 GMT
COPY dir:80bde0d50316e7c9350262fe3b75826a91d075303027787e759d703b60df13d6 in /usr/local/zend/var/plugins/ 
# Sat, 26 Sep 2020 01:16:13 GMT
RUN rm /var/www/html/index.nginx-debian.html
# Sat, 26 Sep 2020 01:16:13 GMT
COPY dir:d174a5d34625889b4356c566972566e0ca7da618b01ea42276562f8186517a67 in /var/www/html 
# Sat, 26 Sep 2020 01:16:13 GMT
EXPOSE 80
# Sat, 26 Sep 2020 01:16:14 GMT
EXPOSE 443
# Sat, 26 Sep 2020 01:16:14 GMT
EXPOSE 10081
# Sat, 26 Sep 2020 01:16:14 GMT
EXPOSE 10082
# Sat, 26 Sep 2020 01:16:14 GMT
WORKDIR /var/www/html
# Sat, 26 Sep 2020 01:16:14 GMT
CMD ["/usr/local/bin/run"]
```

-	Layers:
	-	`sha256:171857c49d0f5e2ebf623e6cb36a8bcad585ed0c2aa99c87a055df034c1e5848`  
		Last Modified: Tue, 22 Sep 2020 12:21:27 GMT  
		Size: 26.7 MB (26701612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:419640447d267f068d2f84a093cb13a56ce77e130877f5b8bdb4294f4a90a84f`  
		Last Modified: Fri, 25 Sep 2020 22:36:49 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61e52f862619ab016d3bcfbd78e5c7aaaa1989b4c295e6dbcacddd2d7b93e1f5`  
		Last Modified: Fri, 25 Sep 2020 22:36:49 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d25ea472f1de12f80e58430b1b7f3f00d4bc8e869d7a2936049a748508899d4`  
		Last Modified: Sat, 26 Sep 2020 01:18:37 GMT  
		Size: 28.5 MB (28531625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1aa4a20a4688fda442a588ed4d1e4ebe5e84282b635b39c7c5b845d93cf5e7c7`  
		Last Modified: Sat, 26 Sep 2020 01:18:34 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cee0e3fb707955145a7f055ecf9477f1054eec3c648fadb7607c43b28abf898c`  
		Last Modified: Sat, 26 Sep 2020 01:18:33 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:067f6ec87d1a0921a2e201d14bc871de38a28f732249323a61cfc7f7d17084a0`  
		Last Modified: Sat, 26 Sep 2020 01:19:37 GMT  
		Size: 418.1 MB (418117003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:964778aa7557739bc53d9237c77300baf80cf7325b2c7448f47a1d77f331eac0`  
		Last Modified: Sat, 26 Sep 2020 01:18:33 GMT  
		Size: 447.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d70852fa4a26d14e8fae00524ae46be5e02524d41b3de324866eabd752b4e81`  
		Last Modified: Sat, 26 Sep 2020 01:18:33 GMT  
		Size: 18.9 KB (18902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77e0177886aaf1f949cb435cc14b60fd396a5425c503020b86cf1bc645ab577f`  
		Last Modified: Sat, 26 Sep 2020 01:18:35 GMT  
		Size: 19.1 MB (19106769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:896f79fecbb3e25efe648cc2772ee81b289154679bba55316bc100b6ac0a7fc9`  
		Last Modified: Sat, 26 Sep 2020 01:18:32 GMT  
		Size: 14.3 KB (14252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cba471bd014c4ccd8e970aaa4ba565ca1ff341200a3eb2c940f062cd4fc33c36`  
		Last Modified: Sat, 26 Sep 2020 01:18:32 GMT  
		Size: 2.5 KB (2527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a18f139f66e26c7937f9ac5fa431af4460309617848cfd61ff67bcf26cf4c30a`  
		Last Modified: Sat, 26 Sep 2020 01:18:32 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4796c9744ddf7d7875ae51305b478ff0bf18021b2fdb55c352a536c1e01fda3`  
		Last Modified: Sat, 26 Sep 2020 01:18:32 GMT  
		Size: 1.3 KB (1255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
