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
$ docker pull php-zendserver@sha256:7362e00616bf1e3b2c664aee72c85712440087d859618a24b6f6a92da25736a1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `php-zendserver:2019.0` - linux; amd64

```console
$ docker pull php-zendserver@sha256:d457a37eab208f4c5336fca61b3876010aa7aa41fbee92561cd1ebf78d0a3601
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **482.7 MB (482668751 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:043227d79d1e8e4821a15b229b57a8781ccf7199402f5deaca7ac8b645b5ebda`
-	Default Command: `["\/usr\/local\/bin\/run"]`

```dockerfile
# Wed, 19 May 2021 19:44:30 GMT
ADD file:e05689b5b0d51a2316f8a87b1a9d6cbf90d98b19a424dbb924ee3d0b1cc17bfc in / 
# Wed, 19 May 2021 19:44:31 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 May 2021 19:44:32 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 May 2021 19:44:33 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 May 2021 19:44:33 GMT
CMD ["/bin/bash"]
# Wed, 19 May 2021 21:27:54 GMT
RUN apt-get update && apt-get install -y       gnupg
# Wed, 19 May 2021 21:27:56 GMT
RUN apt-key adv --keyserver keyserver.ubuntu.com --recv-key 799058698E65316A2E7A4FF42EAE1437F7D2C623
# Wed, 19 May 2021 21:27:56 GMT
COPY file:23f8c2a96f087277b95ebfd7f401f5c1b95ec7f3443fa9231607566f1d8e7270 in /etc/apt/sources.list.d/zend-server.list 
# Wed, 19 May 2021 21:29:42 GMT
RUN apt-get update && apt-get install -y       iproute2       curl       libmysqlclient20       unzip       git       zend-server-nginx=2019.0.7+b403     && rm -rf /var/lib/apt/lists/*     && /usr/local/zend/bin/zendctl.sh stop
# Wed, 19 May 2021 21:29:46 GMT
ENV ZS_INIT_VERSION=0.3
# Wed, 19 May 2021 21:29:46 GMT
ENV ZS_INIT_SHA256=e8d441d8503808e9fc0fafc762b2cb80d4a6e68b94fede0fe41efdeac10800cb
# Wed, 19 May 2021 21:29:46 GMT
COPY file:ad21ce0b2dc8345be0ef63836774934d6b2045ddc3685411221a07dd10b649d1 in /tmp/zs-init.patch 
# Wed, 19 May 2021 21:29:47 GMT
RUN curl -fSL -o zs-init.tar.gz "http://repos.zend.com/zs-init/zs-init-docker-${ZS_INIT_VERSION}.tar.gz"     && echo "${ZS_INIT_SHA256} *zs-init.tar.gz" | sha256sum -c -     && mkdir /usr/local/zs-init     && tar xzf zs-init.tar.gz --strip-components=1 -C /usr/local/zs-init     && rm zs-init.tar.gz     && patch -u /usr/local/zs-init/src/Init/Steps/AbstractStep.php -i /tmp/zs-init.patch     && rm /tmp/zs-init.patch
# Wed, 19 May 2021 21:29:47 GMT
WORKDIR /usr/local/zs-init
# Wed, 19 May 2021 21:29:52 GMT
RUN /usr/local/zend/bin/php -r "readfile('https://getcomposer.org/installer');" | /usr/local/zend/bin/php     && /usr/local/zend/bin/php composer.phar update
# Wed, 19 May 2021 21:29:53 GMT
COPY dir:eecd98e9ebf1c61a12ae67558eb2a6ce846b9ebfadabbf08503e90b3e30d9496 in /usr/local/bin 
# Wed, 19 May 2021 21:29:53 GMT
COPY dir:80bde0d50316e7c9350262fe3b75826a91d075303027787e759d703b60df13d6 in /usr/local/zend/var/plugins/ 
# Wed, 19 May 2021 21:29:54 GMT
RUN rm /var/www/html/index.nginx-debian.html
# Wed, 19 May 2021 21:29:54 GMT
COPY dir:d174a5d34625889b4356c566972566e0ca7da618b01ea42276562f8186517a67 in /var/www/html 
# Wed, 19 May 2021 21:29:54 GMT
EXPOSE 80
# Wed, 19 May 2021 21:29:55 GMT
EXPOSE 443
# Wed, 19 May 2021 21:29:55 GMT
EXPOSE 10081
# Wed, 19 May 2021 21:29:55 GMT
EXPOSE 10082
# Wed, 19 May 2021 21:29:55 GMT
WORKDIR /var/www/html
# Wed, 19 May 2021 21:29:55 GMT
CMD ["/usr/local/bin/run"]
```

-	Layers:
	-	`sha256:4bbfd2c87b7524455f144a03bf387c88b6d4200e5e0df9139a9d5e79110f89ca`  
		Last Modified: Thu, 13 May 2021 14:54:04 GMT  
		Size: 26.7 MB (26696304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2e110be24e168b42c1a2ddbc4a476a217b73cccdba69cdcb212b812a88f5726`  
		Last Modified: Wed, 19 May 2021 19:45:43 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:889a7173dcfeb409f9d88054a97ab2445f5a799a823f719a5573365ee3662b6f`  
		Last Modified: Wed, 19 May 2021 19:45:43 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9144d071c4b85fa5ab5d409a9918aee04c54ec95cff0423fbff29bdc9685240e`  
		Last Modified: Wed, 19 May 2021 21:32:25 GMT  
		Size: 32.7 MB (32728064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e96ceb4f17e2df5b452408d60928be9a5e68b804d762d43789490bec62c03573`  
		Last Modified: Wed, 19 May 2021 21:32:19 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23f06e51a7176f2d7370c0f67890368831fe1670f1c65f587fc47341c3c46ef3`  
		Last Modified: Wed, 19 May 2021 21:32:19 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dc0121a0d0dbdd07bb296f16202ea79d90780b48945ad850386cfd112788fae`  
		Last Modified: Wed, 19 May 2021 21:33:14 GMT  
		Size: 418.1 MB (418060512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b7265a8e404536d6f7e6d6d32e8088bb911832a3882fd7e595979850f5092e2`  
		Last Modified: Wed, 19 May 2021 21:32:18 GMT  
		Size: 445.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:679884bd8552438dbe30af77b3053c5fd3795c2424c5d7223c247aa1763a20b9`  
		Last Modified: Wed, 19 May 2021 21:32:19 GMT  
		Size: 18.9 KB (18930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89f9163f0ddeccf25b6255c6a2b3cc00491e4e8fefba1d6ceae6c9774b101ef8`  
		Last Modified: Wed, 19 May 2021 21:32:17 GMT  
		Size: 5.1 MB (5143530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77df64a66d7863ba28403b9cb1f5b971e313a047ea9be4b8d198b6f87249cde7`  
		Last Modified: Wed, 19 May 2021 21:32:16 GMT  
		Size: 14.3 KB (14292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4aad3dbe0394293d86a2aad364a7c2fd4111a6b327f5b88434ea36bca293bdd`  
		Last Modified: Wed, 19 May 2021 21:32:16 GMT  
		Size: 2.6 KB (2560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62064f69a9ceac4bfd8f5727bf10cc6a786aae78216ab055074a4f7c1566cbea`  
		Last Modified: Wed, 19 May 2021 21:32:16 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dddfc9774448263cba901590d6e2e26ef8d98dcf433065cd7456263df6b1bbd`  
		Last Modified: Wed, 19 May 2021 21:32:16 GMT  
		Size: 1.3 KB (1253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `php-zendserver:2021.0`

```console
$ docker pull php-zendserver@sha256:75e1191b9be91d1373af83efd0a6cb523846811544dadaeb260762136284ceaa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `php-zendserver:2021.0` - linux; amd64

```console
$ docker pull php-zendserver@sha256:41adc32003329deca06ebf9b51e46e325244914ff57d9b4a77a8526e0fe86890
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **390.5 MB (390547905 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e1e318eee8bde745135f5b7573eb3c7dcf3e6c6f8f1540ea47bce4ad0a85073`
-	Default Command: `["\/usr\/local\/bin\/run"]`

```dockerfile
# Wed, 19 May 2021 19:44:30 GMT
ADD file:e05689b5b0d51a2316f8a87b1a9d6cbf90d98b19a424dbb924ee3d0b1cc17bfc in / 
# Wed, 19 May 2021 19:44:31 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 May 2021 19:44:32 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 May 2021 19:44:33 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 May 2021 19:44:33 GMT
CMD ["/bin/bash"]
# Wed, 19 May 2021 21:27:54 GMT
RUN apt-get update && apt-get install -y       gnupg
# Wed, 19 May 2021 21:27:56 GMT
RUN apt-key adv --keyserver keyserver.ubuntu.com --recv-key 799058698E65316A2E7A4FF42EAE1437F7D2C623
# Wed, 02 Jun 2021 05:26:18 GMT
COPY file:1e70d8fd6f9643bffb703528edddba0aa02a58e95cc53e92f58a86cde29e732a in /etc/apt/sources.list.d/zend-server.list 
# Wed, 02 Jun 2021 05:28:37 GMT
RUN apt-get update && apt-get install -y       iproute2       curl       libmysqlclient20       unzip       git       zend-server-nginx=2021.0.0+b74     && rm -rf /var/lib/apt/lists/*     && /usr/local/zend/bin/zendctl.sh stop
# Wed, 02 Jun 2021 05:28:40 GMT
ENV ZS_INIT_VERSION=0.3
# Wed, 02 Jun 2021 05:28:40 GMT
ENV ZS_INIT_SHA256=e8d441d8503808e9fc0fafc762b2cb80d4a6e68b94fede0fe41efdeac10800cb
# Wed, 02 Jun 2021 05:28:40 GMT
COPY file:ad21ce0b2dc8345be0ef63836774934d6b2045ddc3685411221a07dd10b649d1 in /tmp/zs-init.patch 
# Wed, 02 Jun 2021 05:28:42 GMT
RUN curl -fSL -o zs-init.tar.gz "http://repos.zend.com/zs-init/zs-init-docker-${ZS_INIT_VERSION}.tar.gz"     && echo "${ZS_INIT_SHA256} *zs-init.tar.gz" | sha256sum -c -     && mkdir /usr/local/zs-init     && tar xzf zs-init.tar.gz --strip-components=1 -C /usr/local/zs-init     && rm zs-init.tar.gz     && patch -u /usr/local/zs-init/src/Init/Steps/AbstractStep.php -i /tmp/zs-init.patch     && rm /tmp/zs-init.patch
# Wed, 02 Jun 2021 05:28:42 GMT
WORKDIR /usr/local/zs-init
# Wed, 02 Jun 2021 05:28:47 GMT
RUN /usr/local/zend/bin/php -r "readfile('https://getcomposer.org/installer');" | /usr/local/zend/bin/php     && /usr/local/zend/bin/php composer.phar update
# Wed, 02 Jun 2021 05:28:48 GMT
COPY dir:eecd98e9ebf1c61a12ae67558eb2a6ce846b9ebfadabbf08503e90b3e30d9496 in /usr/local/bin 
# Wed, 02 Jun 2021 05:28:48 GMT
COPY dir:80bde0d50316e7c9350262fe3b75826a91d075303027787e759d703b60df13d6 in /usr/local/zend/var/plugins/ 
# Wed, 02 Jun 2021 05:28:49 GMT
RUN rm /var/www/html/index.nginx-debian.html
# Wed, 02 Jun 2021 05:28:49 GMT
COPY dir:d174a5d34625889b4356c566972566e0ca7da618b01ea42276562f8186517a67 in /var/www/html 
# Wed, 02 Jun 2021 05:28:49 GMT
EXPOSE 80
# Wed, 02 Jun 2021 05:28:49 GMT
EXPOSE 443
# Wed, 02 Jun 2021 05:28:50 GMT
EXPOSE 10081
# Wed, 02 Jun 2021 05:28:50 GMT
EXPOSE 10082
# Wed, 02 Jun 2021 05:28:50 GMT
WORKDIR /var/www/html
# Wed, 02 Jun 2021 05:28:50 GMT
CMD ["/usr/local/bin/run"]
```

-	Layers:
	-	`sha256:4bbfd2c87b7524455f144a03bf387c88b6d4200e5e0df9139a9d5e79110f89ca`  
		Last Modified: Thu, 13 May 2021 14:54:04 GMT  
		Size: 26.7 MB (26696304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2e110be24e168b42c1a2ddbc4a476a217b73cccdba69cdcb212b812a88f5726`  
		Last Modified: Wed, 19 May 2021 19:45:43 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:889a7173dcfeb409f9d88054a97ab2445f5a799a823f719a5573365ee3662b6f`  
		Last Modified: Wed, 19 May 2021 19:45:43 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9144d071c4b85fa5ab5d409a9918aee04c54ec95cff0423fbff29bdc9685240e`  
		Last Modified: Wed, 19 May 2021 21:32:25 GMT  
		Size: 32.7 MB (32728064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e96ceb4f17e2df5b452408d60928be9a5e68b804d762d43789490bec62c03573`  
		Last Modified: Wed, 19 May 2021 21:32:19 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da8508419d7e817248be0bd87dee89c187aa3e2192cb6c7ad2960d83a0973c04`  
		Last Modified: Wed, 02 Jun 2021 05:29:14 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11874b19716c34cdc712011486d3d85b707d5148f637300e27ae0b2cd9da7296`  
		Last Modified: Wed, 02 Jun 2021 05:29:58 GMT  
		Size: 325.9 MB (325939344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d22002ca86e9fe54d9098dfae1be7184a94e635e0b2b22521cfce75d263ad58`  
		Last Modified: Wed, 02 Jun 2021 05:29:13 GMT  
		Size: 446.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89d86e4e78768ff2a28733e688274954ad50540901ec09edc416724ba54766c1`  
		Last Modified: Wed, 02 Jun 2021 05:29:14 GMT  
		Size: 18.9 KB (18933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c1f13a54a7eef1d4df4c30b2a6fe116ef9f5128d7458e4e480bbff3794b93de`  
		Last Modified: Wed, 02 Jun 2021 05:29:12 GMT  
		Size: 5.1 MB (5143845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6000bc0ffd7edcc58243e31eb96155e1ba001dc53af51045d58dd3091eb1c7e`  
		Last Modified: Wed, 02 Jun 2021 05:29:11 GMT  
		Size: 14.3 KB (14293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7556bf9fbff70fa59c442d318536dfe80b74b5e0b43465bacd26ba0a8582d9e`  
		Last Modified: Wed, 02 Jun 2021 05:29:11 GMT  
		Size: 2.6 KB (2558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:871ae199dc1048e94fb53ec87b9c3c043b51041043893abf2b60bf8435e9c4dc`  
		Last Modified: Wed, 02 Jun 2021 05:29:11 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76d2b9a5806a293d1c8405ee91f90cfb55050d8b97922ea6e47ea5a95c890c28`  
		Last Modified: Wed, 02 Jun 2021 05:29:11 GMT  
		Size: 1.3 KB (1255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `php-zendserver:5.6`

```console
$ docker pull php-zendserver@sha256:29f7a6caff28ff30727d39ae8f84f349647962e4ee1ed1b5ecaad3c7a4c49682
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `php-zendserver:5.6` - linux; amd64

```console
$ docker pull php-zendserver@sha256:35110784719156315d53f3eabd343864fe6d6918262320da2ee414b44aa70b7f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **315.6 MB (315562399 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0879dc1f9d2c49dbd786d23dbda5b85a51f1c2e696f4d7f1830936cea8bb626a`
-	Default Command: `["\/usr\/local\/bin\/run"]`

```dockerfile
# Wed, 19 May 2021 19:45:15 GMT
ADD file:5dd161b04353d3cbc2b258d66ef3c79a8307faa944953a1c7920a3d97468520c in / 
# Wed, 19 May 2021 19:45:16 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 May 2021 19:45:17 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 19 May 2021 19:45:18 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 May 2021 19:45:19 GMT
CMD ["/bin/bash"]
# Wed, 19 May 2021 21:23:26 GMT
RUN apt-key adv --keyserver keyserver.ubuntu.com --recv-key 799058698E65316A2E7A4FF42EAE1437F7D2C623
# Wed, 19 May 2021 21:23:26 GMT
COPY file:6f0a5450842ae9c3e06d131c7180961d773ca33754e17af8ea2ac258fd0c6054 in /etc/apt/sources.list.d/zend-server.list 
# Wed, 19 May 2021 21:23:26 GMT
COPY file:7a9d81c6298f71cfad4408c8b3d7c3bf53bf90083221ec55686e12b2eb6f16a4 in /etc/apt/sources.list.d/ubuntu-trusty.list 
# Wed, 19 May 2021 21:25:19 GMT
RUN apt-get update     && apt-get install -y         curl         libmysqlclient18         unzip         git         zend-server-php-5.6=8.5.17+b19     && rm -rf /var/lib/apt/lists/*     && /usr/local/zend/bin/zendctl.sh stop
# Wed, 19 May 2021 21:25:22 GMT
COPY file:def46bbc651bcb61f92bcaa2f8d6edec0c22e51e86132fabd2e47542dcbec0bf in /etc/apache2/conf-available 
# Wed, 19 May 2021 21:25:23 GMT
RUN /usr/sbin/a2enconf drop-http-proxy-header
# Wed, 19 May 2021 21:25:24 GMT
RUN /usr/sbin/a2enmod headers
# Wed, 19 May 2021 21:25:24 GMT
ENV ZS_INIT_VERSION=0.3
# Wed, 19 May 2021 21:25:24 GMT
ENV ZS_INIT_SHA256=e8d441d8503808e9fc0fafc762b2cb80d4a6e68b94fede0fe41efdeac10800cb
# Wed, 19 May 2021 21:25:26 GMT
RUN curl -fSL -o zs-init.tar.gz "http://repos.zend.com/zs-init/zs-init-docker-${ZS_INIT_VERSION}.tar.gz"     && echo "${ZS_INIT_SHA256} *zs-init.tar.gz" | sha256sum -c -     && mkdir /usr/local/zs-init     && tar xzf zs-init.tar.gz --strip-components=1 -C /usr/local/zs-init     && rm zs-init.tar.gz
# Wed, 19 May 2021 21:25:26 GMT
WORKDIR /usr/local/zs-init
# Wed, 19 May 2021 21:25:33 GMT
RUN /usr/local/zend/bin/php -r "readfile('https://getcomposer.org/installer');" | /usr/local/zend/bin/php     && /usr/local/zend/bin/php composer.phar self-update && /usr/local/zend/bin/php composer.phar update
# Wed, 19 May 2021 21:25:33 GMT
COPY dir:b75978d6e77900379bb898c52c86c408d7f6fcd06b5c66439d594a1a3dcca0b4 in /usr/local/bin 
# Wed, 19 May 2021 21:25:33 GMT
COPY dir:80bde0d50316e7c9350262fe3b75826a91d075303027787e759d703b60df13d6 in /usr/local/zend/var/plugins/ 
# Wed, 19 May 2021 21:25:34 GMT
RUN rm /var/www/html/index.html
# Wed, 19 May 2021 21:25:34 GMT
COPY dir:d174a5d34625889b4356c566972566e0ca7da618b01ea42276562f8186517a67 in /var/www/html 
# Wed, 19 May 2021 21:25:35 GMT
EXPOSE 80
# Wed, 19 May 2021 21:25:35 GMT
EXPOSE 443
# Wed, 19 May 2021 21:25:35 GMT
EXPOSE 10081
# Wed, 19 May 2021 21:25:35 GMT
EXPOSE 10082
# Wed, 19 May 2021 21:25:35 GMT
WORKDIR /var/www/html
# Wed, 19 May 2021 21:25:35 GMT
CMD ["/usr/local/bin/run"]
```

-	Layers:
	-	`sha256:80bce60046fa9e5ccbe54c9bd4bfa3f379ce7bc43bed493ae92389050de04024`  
		Last Modified: Thu, 29 Apr 2021 15:24:23 GMT  
		Size: 46.5 MB (46461779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55a738a1554069bc9050c0a60b57fc93e98069e59822677a483cc74cafaf2bf7`  
		Last Modified: Wed, 19 May 2021 19:46:37 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e19cf0706c6229033d11dbf952b3eb96ad70e1f32527960aeb3c83ad86f16551`  
		Last Modified: Wed, 19 May 2021 19:46:36 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de4cdd6c27d1f17cf5ff350e76b7efe80aceff4dc99fd518065bf048abd6494a`  
		Last Modified: Wed, 19 May 2021 19:46:36 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac40b437fbc4991a8140c95b7a0260f9712a5eaac51c8041da4eac49f84ad66f`  
		Last Modified: Wed, 19 May 2021 21:30:28 GMT  
		Size: 14.7 KB (14704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5733792fcd2f20c5795da034849032a7b96455bc03d2cf7b1c9a1721e169cd12`  
		Last Modified: Wed, 19 May 2021 21:30:28 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba4494029f725b281461477d7da1e4f81fd33255109e0519592e0dad92c3a4d9`  
		Last Modified: Wed, 19 May 2021 21:30:28 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:647437216dfaa70b6638abd53f5cb549b44197b5ae741ff1f680f8c9446d17d9`  
		Last Modified: Wed, 19 May 2021 21:30:58 GMT  
		Size: 263.9 MB (263908043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59b566b1ae3967eef5a9b2c36d981c7236e780248c80336b1b333294eac632e9`  
		Last Modified: Wed, 19 May 2021 21:30:25 GMT  
		Size: 261.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0cbdc785d56dba5ef10f8953ccca2311fb28079dd3ee76882e01bbf0b73b09a`  
		Last Modified: Wed, 19 May 2021 21:30:26 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f16eb159dd02187bcbdf6d2c852f31f5c3d1b90d072df66f793ad18925988e42`  
		Last Modified: Wed, 19 May 2021 21:30:25 GMT  
		Size: 309.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40304a32d57db74eb46651f2c13c784df1acb38bf9c33049dd6d00bdde03a705`  
		Last Modified: Wed, 19 May 2021 21:30:25 GMT  
		Size: 18.9 KB (18857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc26788b27ab0c3453fae2dede1847171b47dd85e8bd42df4a2597a34b4cdcd2`  
		Last Modified: Wed, 19 May 2021 21:30:24 GMT  
		Size: 5.1 MB (5138713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0f1c0f5cbc82d68742da0ab34d929531b111d992bfed087ade11cf5c32b5002`  
		Last Modified: Wed, 19 May 2021 21:30:23 GMT  
		Size: 13.4 KB (13352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30fd4a818ec8c10f951244c1c634c2b3c14beb420d0ce303e6e5af70a80dd2a2`  
		Last Modified: Wed, 19 May 2021 21:30:22 GMT  
		Size: 2.6 KB (2566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29a6e314138b090b0b7aa9704b3325fc8547a649f116a8d9ef6ad8653bc9655e`  
		Last Modified: Wed, 19 May 2021 21:30:23 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6953f3187a2a18cd98427f9c3bb9d61ae3022aabb3e45a1815c188c16b8228b7`  
		Last Modified: Wed, 19 May 2021 21:30:23 GMT  
		Size: 1.2 KB (1250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `php-zendserver:8.5`

```console
$ docker pull php-zendserver@sha256:29f7a6caff28ff30727d39ae8f84f349647962e4ee1ed1b5ecaad3c7a4c49682
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `php-zendserver:8.5` - linux; amd64

```console
$ docker pull php-zendserver@sha256:35110784719156315d53f3eabd343864fe6d6918262320da2ee414b44aa70b7f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **315.6 MB (315562399 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0879dc1f9d2c49dbd786d23dbda5b85a51f1c2e696f4d7f1830936cea8bb626a`
-	Default Command: `["\/usr\/local\/bin\/run"]`

```dockerfile
# Wed, 19 May 2021 19:45:15 GMT
ADD file:5dd161b04353d3cbc2b258d66ef3c79a8307faa944953a1c7920a3d97468520c in / 
# Wed, 19 May 2021 19:45:16 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 May 2021 19:45:17 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 19 May 2021 19:45:18 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 May 2021 19:45:19 GMT
CMD ["/bin/bash"]
# Wed, 19 May 2021 21:23:26 GMT
RUN apt-key adv --keyserver keyserver.ubuntu.com --recv-key 799058698E65316A2E7A4FF42EAE1437F7D2C623
# Wed, 19 May 2021 21:23:26 GMT
COPY file:6f0a5450842ae9c3e06d131c7180961d773ca33754e17af8ea2ac258fd0c6054 in /etc/apt/sources.list.d/zend-server.list 
# Wed, 19 May 2021 21:23:26 GMT
COPY file:7a9d81c6298f71cfad4408c8b3d7c3bf53bf90083221ec55686e12b2eb6f16a4 in /etc/apt/sources.list.d/ubuntu-trusty.list 
# Wed, 19 May 2021 21:25:19 GMT
RUN apt-get update     && apt-get install -y         curl         libmysqlclient18         unzip         git         zend-server-php-5.6=8.5.17+b19     && rm -rf /var/lib/apt/lists/*     && /usr/local/zend/bin/zendctl.sh stop
# Wed, 19 May 2021 21:25:22 GMT
COPY file:def46bbc651bcb61f92bcaa2f8d6edec0c22e51e86132fabd2e47542dcbec0bf in /etc/apache2/conf-available 
# Wed, 19 May 2021 21:25:23 GMT
RUN /usr/sbin/a2enconf drop-http-proxy-header
# Wed, 19 May 2021 21:25:24 GMT
RUN /usr/sbin/a2enmod headers
# Wed, 19 May 2021 21:25:24 GMT
ENV ZS_INIT_VERSION=0.3
# Wed, 19 May 2021 21:25:24 GMT
ENV ZS_INIT_SHA256=e8d441d8503808e9fc0fafc762b2cb80d4a6e68b94fede0fe41efdeac10800cb
# Wed, 19 May 2021 21:25:26 GMT
RUN curl -fSL -o zs-init.tar.gz "http://repos.zend.com/zs-init/zs-init-docker-${ZS_INIT_VERSION}.tar.gz"     && echo "${ZS_INIT_SHA256} *zs-init.tar.gz" | sha256sum -c -     && mkdir /usr/local/zs-init     && tar xzf zs-init.tar.gz --strip-components=1 -C /usr/local/zs-init     && rm zs-init.tar.gz
# Wed, 19 May 2021 21:25:26 GMT
WORKDIR /usr/local/zs-init
# Wed, 19 May 2021 21:25:33 GMT
RUN /usr/local/zend/bin/php -r "readfile('https://getcomposer.org/installer');" | /usr/local/zend/bin/php     && /usr/local/zend/bin/php composer.phar self-update && /usr/local/zend/bin/php composer.phar update
# Wed, 19 May 2021 21:25:33 GMT
COPY dir:b75978d6e77900379bb898c52c86c408d7f6fcd06b5c66439d594a1a3dcca0b4 in /usr/local/bin 
# Wed, 19 May 2021 21:25:33 GMT
COPY dir:80bde0d50316e7c9350262fe3b75826a91d075303027787e759d703b60df13d6 in /usr/local/zend/var/plugins/ 
# Wed, 19 May 2021 21:25:34 GMT
RUN rm /var/www/html/index.html
# Wed, 19 May 2021 21:25:34 GMT
COPY dir:d174a5d34625889b4356c566972566e0ca7da618b01ea42276562f8186517a67 in /var/www/html 
# Wed, 19 May 2021 21:25:35 GMT
EXPOSE 80
# Wed, 19 May 2021 21:25:35 GMT
EXPOSE 443
# Wed, 19 May 2021 21:25:35 GMT
EXPOSE 10081
# Wed, 19 May 2021 21:25:35 GMT
EXPOSE 10082
# Wed, 19 May 2021 21:25:35 GMT
WORKDIR /var/www/html
# Wed, 19 May 2021 21:25:35 GMT
CMD ["/usr/local/bin/run"]
```

-	Layers:
	-	`sha256:80bce60046fa9e5ccbe54c9bd4bfa3f379ce7bc43bed493ae92389050de04024`  
		Last Modified: Thu, 29 Apr 2021 15:24:23 GMT  
		Size: 46.5 MB (46461779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55a738a1554069bc9050c0a60b57fc93e98069e59822677a483cc74cafaf2bf7`  
		Last Modified: Wed, 19 May 2021 19:46:37 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e19cf0706c6229033d11dbf952b3eb96ad70e1f32527960aeb3c83ad86f16551`  
		Last Modified: Wed, 19 May 2021 19:46:36 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de4cdd6c27d1f17cf5ff350e76b7efe80aceff4dc99fd518065bf048abd6494a`  
		Last Modified: Wed, 19 May 2021 19:46:36 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac40b437fbc4991a8140c95b7a0260f9712a5eaac51c8041da4eac49f84ad66f`  
		Last Modified: Wed, 19 May 2021 21:30:28 GMT  
		Size: 14.7 KB (14704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5733792fcd2f20c5795da034849032a7b96455bc03d2cf7b1c9a1721e169cd12`  
		Last Modified: Wed, 19 May 2021 21:30:28 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba4494029f725b281461477d7da1e4f81fd33255109e0519592e0dad92c3a4d9`  
		Last Modified: Wed, 19 May 2021 21:30:28 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:647437216dfaa70b6638abd53f5cb549b44197b5ae741ff1f680f8c9446d17d9`  
		Last Modified: Wed, 19 May 2021 21:30:58 GMT  
		Size: 263.9 MB (263908043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59b566b1ae3967eef5a9b2c36d981c7236e780248c80336b1b333294eac632e9`  
		Last Modified: Wed, 19 May 2021 21:30:25 GMT  
		Size: 261.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0cbdc785d56dba5ef10f8953ccca2311fb28079dd3ee76882e01bbf0b73b09a`  
		Last Modified: Wed, 19 May 2021 21:30:26 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f16eb159dd02187bcbdf6d2c852f31f5c3d1b90d072df66f793ad18925988e42`  
		Last Modified: Wed, 19 May 2021 21:30:25 GMT  
		Size: 309.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40304a32d57db74eb46651f2c13c784df1acb38bf9c33049dd6d00bdde03a705`  
		Last Modified: Wed, 19 May 2021 21:30:25 GMT  
		Size: 18.9 KB (18857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc26788b27ab0c3453fae2dede1847171b47dd85e8bd42df4a2597a34b4cdcd2`  
		Last Modified: Wed, 19 May 2021 21:30:24 GMT  
		Size: 5.1 MB (5138713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0f1c0f5cbc82d68742da0ab34d929531b111d992bfed087ade11cf5c32b5002`  
		Last Modified: Wed, 19 May 2021 21:30:23 GMT  
		Size: 13.4 KB (13352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30fd4a818ec8c10f951244c1c634c2b3c14beb420d0ce303e6e5af70a80dd2a2`  
		Last Modified: Wed, 19 May 2021 21:30:22 GMT  
		Size: 2.6 KB (2566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29a6e314138b090b0b7aa9704b3325fc8547a649f116a8d9ef6ad8653bc9655e`  
		Last Modified: Wed, 19 May 2021 21:30:23 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6953f3187a2a18cd98427f9c3bb9d61ae3022aabb3e45a1815c188c16b8228b7`  
		Last Modified: Wed, 19 May 2021 21:30:23 GMT  
		Size: 1.2 KB (1250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `php-zendserver:8.5-php5.6`

```console
$ docker pull php-zendserver@sha256:29f7a6caff28ff30727d39ae8f84f349647962e4ee1ed1b5ecaad3c7a4c49682
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `php-zendserver:8.5-php5.6` - linux; amd64

```console
$ docker pull php-zendserver@sha256:35110784719156315d53f3eabd343864fe6d6918262320da2ee414b44aa70b7f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **315.6 MB (315562399 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0879dc1f9d2c49dbd786d23dbda5b85a51f1c2e696f4d7f1830936cea8bb626a`
-	Default Command: `["\/usr\/local\/bin\/run"]`

```dockerfile
# Wed, 19 May 2021 19:45:15 GMT
ADD file:5dd161b04353d3cbc2b258d66ef3c79a8307faa944953a1c7920a3d97468520c in / 
# Wed, 19 May 2021 19:45:16 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 May 2021 19:45:17 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 19 May 2021 19:45:18 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 May 2021 19:45:19 GMT
CMD ["/bin/bash"]
# Wed, 19 May 2021 21:23:26 GMT
RUN apt-key adv --keyserver keyserver.ubuntu.com --recv-key 799058698E65316A2E7A4FF42EAE1437F7D2C623
# Wed, 19 May 2021 21:23:26 GMT
COPY file:6f0a5450842ae9c3e06d131c7180961d773ca33754e17af8ea2ac258fd0c6054 in /etc/apt/sources.list.d/zend-server.list 
# Wed, 19 May 2021 21:23:26 GMT
COPY file:7a9d81c6298f71cfad4408c8b3d7c3bf53bf90083221ec55686e12b2eb6f16a4 in /etc/apt/sources.list.d/ubuntu-trusty.list 
# Wed, 19 May 2021 21:25:19 GMT
RUN apt-get update     && apt-get install -y         curl         libmysqlclient18         unzip         git         zend-server-php-5.6=8.5.17+b19     && rm -rf /var/lib/apt/lists/*     && /usr/local/zend/bin/zendctl.sh stop
# Wed, 19 May 2021 21:25:22 GMT
COPY file:def46bbc651bcb61f92bcaa2f8d6edec0c22e51e86132fabd2e47542dcbec0bf in /etc/apache2/conf-available 
# Wed, 19 May 2021 21:25:23 GMT
RUN /usr/sbin/a2enconf drop-http-proxy-header
# Wed, 19 May 2021 21:25:24 GMT
RUN /usr/sbin/a2enmod headers
# Wed, 19 May 2021 21:25:24 GMT
ENV ZS_INIT_VERSION=0.3
# Wed, 19 May 2021 21:25:24 GMT
ENV ZS_INIT_SHA256=e8d441d8503808e9fc0fafc762b2cb80d4a6e68b94fede0fe41efdeac10800cb
# Wed, 19 May 2021 21:25:26 GMT
RUN curl -fSL -o zs-init.tar.gz "http://repos.zend.com/zs-init/zs-init-docker-${ZS_INIT_VERSION}.tar.gz"     && echo "${ZS_INIT_SHA256} *zs-init.tar.gz" | sha256sum -c -     && mkdir /usr/local/zs-init     && tar xzf zs-init.tar.gz --strip-components=1 -C /usr/local/zs-init     && rm zs-init.tar.gz
# Wed, 19 May 2021 21:25:26 GMT
WORKDIR /usr/local/zs-init
# Wed, 19 May 2021 21:25:33 GMT
RUN /usr/local/zend/bin/php -r "readfile('https://getcomposer.org/installer');" | /usr/local/zend/bin/php     && /usr/local/zend/bin/php composer.phar self-update && /usr/local/zend/bin/php composer.phar update
# Wed, 19 May 2021 21:25:33 GMT
COPY dir:b75978d6e77900379bb898c52c86c408d7f6fcd06b5c66439d594a1a3dcca0b4 in /usr/local/bin 
# Wed, 19 May 2021 21:25:33 GMT
COPY dir:80bde0d50316e7c9350262fe3b75826a91d075303027787e759d703b60df13d6 in /usr/local/zend/var/plugins/ 
# Wed, 19 May 2021 21:25:34 GMT
RUN rm /var/www/html/index.html
# Wed, 19 May 2021 21:25:34 GMT
COPY dir:d174a5d34625889b4356c566972566e0ca7da618b01ea42276562f8186517a67 in /var/www/html 
# Wed, 19 May 2021 21:25:35 GMT
EXPOSE 80
# Wed, 19 May 2021 21:25:35 GMT
EXPOSE 443
# Wed, 19 May 2021 21:25:35 GMT
EXPOSE 10081
# Wed, 19 May 2021 21:25:35 GMT
EXPOSE 10082
# Wed, 19 May 2021 21:25:35 GMT
WORKDIR /var/www/html
# Wed, 19 May 2021 21:25:35 GMT
CMD ["/usr/local/bin/run"]
```

-	Layers:
	-	`sha256:80bce60046fa9e5ccbe54c9bd4bfa3f379ce7bc43bed493ae92389050de04024`  
		Last Modified: Thu, 29 Apr 2021 15:24:23 GMT  
		Size: 46.5 MB (46461779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55a738a1554069bc9050c0a60b57fc93e98069e59822677a483cc74cafaf2bf7`  
		Last Modified: Wed, 19 May 2021 19:46:37 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e19cf0706c6229033d11dbf952b3eb96ad70e1f32527960aeb3c83ad86f16551`  
		Last Modified: Wed, 19 May 2021 19:46:36 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de4cdd6c27d1f17cf5ff350e76b7efe80aceff4dc99fd518065bf048abd6494a`  
		Last Modified: Wed, 19 May 2021 19:46:36 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac40b437fbc4991a8140c95b7a0260f9712a5eaac51c8041da4eac49f84ad66f`  
		Last Modified: Wed, 19 May 2021 21:30:28 GMT  
		Size: 14.7 KB (14704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5733792fcd2f20c5795da034849032a7b96455bc03d2cf7b1c9a1721e169cd12`  
		Last Modified: Wed, 19 May 2021 21:30:28 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba4494029f725b281461477d7da1e4f81fd33255109e0519592e0dad92c3a4d9`  
		Last Modified: Wed, 19 May 2021 21:30:28 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:647437216dfaa70b6638abd53f5cb549b44197b5ae741ff1f680f8c9446d17d9`  
		Last Modified: Wed, 19 May 2021 21:30:58 GMT  
		Size: 263.9 MB (263908043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59b566b1ae3967eef5a9b2c36d981c7236e780248c80336b1b333294eac632e9`  
		Last Modified: Wed, 19 May 2021 21:30:25 GMT  
		Size: 261.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0cbdc785d56dba5ef10f8953ccca2311fb28079dd3ee76882e01bbf0b73b09a`  
		Last Modified: Wed, 19 May 2021 21:30:26 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f16eb159dd02187bcbdf6d2c852f31f5c3d1b90d072df66f793ad18925988e42`  
		Last Modified: Wed, 19 May 2021 21:30:25 GMT  
		Size: 309.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40304a32d57db74eb46651f2c13c784df1acb38bf9c33049dd6d00bdde03a705`  
		Last Modified: Wed, 19 May 2021 21:30:25 GMT  
		Size: 18.9 KB (18857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc26788b27ab0c3453fae2dede1847171b47dd85e8bd42df4a2597a34b4cdcd2`  
		Last Modified: Wed, 19 May 2021 21:30:24 GMT  
		Size: 5.1 MB (5138713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0f1c0f5cbc82d68742da0ab34d929531b111d992bfed087ade11cf5c32b5002`  
		Last Modified: Wed, 19 May 2021 21:30:23 GMT  
		Size: 13.4 KB (13352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30fd4a818ec8c10f951244c1c634c2b3c14beb420d0ce303e6e5af70a80dd2a2`  
		Last Modified: Wed, 19 May 2021 21:30:22 GMT  
		Size: 2.6 KB (2566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29a6e314138b090b0b7aa9704b3325fc8547a649f116a8d9ef6ad8653bc9655e`  
		Last Modified: Wed, 19 May 2021 21:30:23 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6953f3187a2a18cd98427f9c3bb9d61ae3022aabb3e45a1815c188c16b8228b7`  
		Last Modified: Wed, 19 May 2021 21:30:23 GMT  
		Size: 1.2 KB (1250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `php-zendserver:9.1`

```console
$ docker pull php-zendserver@sha256:62627094de4aae154c40789000bf365818c2110bc9febfbd1396277092c26684
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `php-zendserver:9.1` - linux; amd64

```console
$ docker pull php-zendserver@sha256:516da56f497293c59d096b2e2c57821568a9c96a4b219c7cdcd7284727d84560
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **399.2 MB (399219727 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f6bd0cad3115091603fce75193b622030a5d2127654524ceaa3a5216b731649a`
-	Default Command: `["\/usr\/local\/bin\/run"]`

```dockerfile
# Wed, 19 May 2021 19:45:15 GMT
ADD file:5dd161b04353d3cbc2b258d66ef3c79a8307faa944953a1c7920a3d97468520c in / 
# Wed, 19 May 2021 19:45:16 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 May 2021 19:45:17 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 19 May 2021 19:45:18 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 May 2021 19:45:19 GMT
CMD ["/bin/bash"]
# Wed, 19 May 2021 21:23:26 GMT
RUN apt-key adv --keyserver keyserver.ubuntu.com --recv-key 799058698E65316A2E7A4FF42EAE1437F7D2C623
# Wed, 19 May 2021 21:25:51 GMT
COPY file:0d4830b5060fb75cec6a47b30d343d82f9c3d6f95f20c11635618b93dedb5720 in /etc/apt/sources.list.d/zend-server.list 
# Wed, 19 May 2021 21:27:23 GMT
RUN apt-get update     && apt-get install -y       curl       libmysqlclient20       unzip       git       zend-server-php-7.1=9.1.12+b211     && rm -rf /var/lib/apt/lists/*     && /usr/local/zend/bin/zendctl.sh stop
# Wed, 19 May 2021 21:27:26 GMT
COPY file:def46bbc651bcb61f92bcaa2f8d6edec0c22e51e86132fabd2e47542dcbec0bf in /etc/apache2/conf-available 
# Wed, 19 May 2021 21:27:27 GMT
RUN /usr/sbin/a2enconf drop-http-proxy-header
# Wed, 19 May 2021 21:27:28 GMT
RUN /usr/sbin/a2enmod headers
# Wed, 19 May 2021 21:27:28 GMT
ENV ZS_INIT_VERSION=0.3
# Wed, 19 May 2021 21:27:28 GMT
ENV ZS_INIT_SHA256=e8d441d8503808e9fc0fafc762b2cb80d4a6e68b94fede0fe41efdeac10800cb
# Wed, 19 May 2021 21:27:30 GMT
RUN curl -fSL -o zs-init.tar.gz "http://repos.zend.com/zs-init/zs-init-docker-${ZS_INIT_VERSION}.tar.gz"     && echo "${ZS_INIT_SHA256} *zs-init.tar.gz" | sha256sum -c -     && mkdir /usr/local/zs-init     && tar xzf zs-init.tar.gz --strip-components=1 -C /usr/local/zs-init     && rm zs-init.tar.gz
# Wed, 19 May 2021 21:27:30 GMT
WORKDIR /usr/local/zs-init
# Wed, 19 May 2021 21:27:36 GMT
RUN /usr/local/zend/bin/php -r "readfile('https://getcomposer.org/installer');" | /usr/local/zend/bin/php     && /usr/local/zend/bin/php composer.phar self-update && /usr/local/zend/bin/php composer.phar update
# Wed, 19 May 2021 21:27:36 GMT
COPY dir:5966ca4828c37f68d48d11da814350a590451453f42aa83ef2eab6893db3e4cc in /usr/local/bin 
# Wed, 19 May 2021 21:27:37 GMT
COPY dir:80bde0d50316e7c9350262fe3b75826a91d075303027787e759d703b60df13d6 in /usr/local/zend/var/plugins/ 
# Wed, 19 May 2021 21:27:38 GMT
RUN rm /var/www/html/index.html
# Wed, 19 May 2021 21:27:38 GMT
COPY dir:d174a5d34625889b4356c566972566e0ca7da618b01ea42276562f8186517a67 in /var/www/html 
# Wed, 19 May 2021 21:27:38 GMT
EXPOSE 80
# Wed, 19 May 2021 21:27:38 GMT
EXPOSE 443
# Wed, 19 May 2021 21:27:38 GMT
EXPOSE 10081
# Wed, 19 May 2021 21:27:39 GMT
EXPOSE 10082
# Wed, 19 May 2021 21:27:39 GMT
WORKDIR /var/www/html
# Wed, 19 May 2021 21:27:39 GMT
CMD ["/usr/local/bin/run"]
```

-	Layers:
	-	`sha256:80bce60046fa9e5ccbe54c9bd4bfa3f379ce7bc43bed493ae92389050de04024`  
		Last Modified: Thu, 29 Apr 2021 15:24:23 GMT  
		Size: 46.5 MB (46461779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55a738a1554069bc9050c0a60b57fc93e98069e59822677a483cc74cafaf2bf7`  
		Last Modified: Wed, 19 May 2021 19:46:37 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e19cf0706c6229033d11dbf952b3eb96ad70e1f32527960aeb3c83ad86f16551`  
		Last Modified: Wed, 19 May 2021 19:46:36 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de4cdd6c27d1f17cf5ff350e76b7efe80aceff4dc99fd518065bf048abd6494a`  
		Last Modified: Wed, 19 May 2021 19:46:36 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac40b437fbc4991a8140c95b7a0260f9712a5eaac51c8041da4eac49f84ad66f`  
		Last Modified: Wed, 19 May 2021 21:30:28 GMT  
		Size: 14.7 KB (14704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ac90c1e328daf1dcbfaaad77fe3279b6f409e8c3ab5efac3136159372add55c`  
		Last Modified: Wed, 19 May 2021 21:31:19 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0164e8ebb2b7dca4e7498e7b45d84509d8d5ea5479d0e9d211bcc44f76a59f5b`  
		Last Modified: Wed, 19 May 2021 21:32:02 GMT  
		Size: 347.6 MB (347559876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d67e229845786af18a87a4b2c56dd61f5af3b29ce0c7612cffb6ac83ff3af08d`  
		Last Modified: Wed, 19 May 2021 21:31:17 GMT  
		Size: 261.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8acf74b7136246758096c67ced6ab6d4efb4e0205c071c75aabe38b7a0061e4b`  
		Last Modified: Wed, 19 May 2021 21:31:17 GMT  
		Size: 337.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a65f1a05d3e7d6c957a7691dcfce6225b3876b4789df0d1dc9839eba37446a47`  
		Last Modified: Wed, 19 May 2021 21:31:17 GMT  
		Size: 309.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da28f2ef237f957f1e8cdf7061732fd0b65fafc2cac74b500073f55d644d5505`  
		Last Modified: Wed, 19 May 2021 21:31:17 GMT  
		Size: 18.9 KB (18857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b09f7e865cce47ba1dc72bcfdb99f994b327956cbee5009983f721d4f25e4f4`  
		Last Modified: Wed, 19 May 2021 21:31:15 GMT  
		Size: 5.1 MB (5143533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e23b15d85b85e4e2b93eba2c6d934dd76bdd88c46ff38301b5bf78d32aedb4a`  
		Last Modified: Wed, 19 May 2021 21:31:14 GMT  
		Size: 14.3 KB (14316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a838f1687396ee0c9138791935ec885105a6d1e1044657a321618b9a2b94593`  
		Last Modified: Wed, 19 May 2021 21:31:14 GMT  
		Size: 2.6 KB (2556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d71ab5c15f002dfcccf27b838dd6153a403532202fc317ad013eb23d0a8f85f`  
		Last Modified: Wed, 19 May 2021 21:31:14 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4fd28e94312c2a9cfb55e70d73a5b390435585ca07a803e989d1873b0e71684`  
		Last Modified: Wed, 19 May 2021 21:31:14 GMT  
		Size: 1.2 KB (1249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `php-zendserver:latest`

```console
$ docker pull php-zendserver@sha256:75e1191b9be91d1373af83efd0a6cb523846811544dadaeb260762136284ceaa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `php-zendserver:latest` - linux; amd64

```console
$ docker pull php-zendserver@sha256:41adc32003329deca06ebf9b51e46e325244914ff57d9b4a77a8526e0fe86890
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **390.5 MB (390547905 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e1e318eee8bde745135f5b7573eb3c7dcf3e6c6f8f1540ea47bce4ad0a85073`
-	Default Command: `["\/usr\/local\/bin\/run"]`

```dockerfile
# Wed, 19 May 2021 19:44:30 GMT
ADD file:e05689b5b0d51a2316f8a87b1a9d6cbf90d98b19a424dbb924ee3d0b1cc17bfc in / 
# Wed, 19 May 2021 19:44:31 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 May 2021 19:44:32 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 May 2021 19:44:33 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 May 2021 19:44:33 GMT
CMD ["/bin/bash"]
# Wed, 19 May 2021 21:27:54 GMT
RUN apt-get update && apt-get install -y       gnupg
# Wed, 19 May 2021 21:27:56 GMT
RUN apt-key adv --keyserver keyserver.ubuntu.com --recv-key 799058698E65316A2E7A4FF42EAE1437F7D2C623
# Wed, 02 Jun 2021 05:26:18 GMT
COPY file:1e70d8fd6f9643bffb703528edddba0aa02a58e95cc53e92f58a86cde29e732a in /etc/apt/sources.list.d/zend-server.list 
# Wed, 02 Jun 2021 05:28:37 GMT
RUN apt-get update && apt-get install -y       iproute2       curl       libmysqlclient20       unzip       git       zend-server-nginx=2021.0.0+b74     && rm -rf /var/lib/apt/lists/*     && /usr/local/zend/bin/zendctl.sh stop
# Wed, 02 Jun 2021 05:28:40 GMT
ENV ZS_INIT_VERSION=0.3
# Wed, 02 Jun 2021 05:28:40 GMT
ENV ZS_INIT_SHA256=e8d441d8503808e9fc0fafc762b2cb80d4a6e68b94fede0fe41efdeac10800cb
# Wed, 02 Jun 2021 05:28:40 GMT
COPY file:ad21ce0b2dc8345be0ef63836774934d6b2045ddc3685411221a07dd10b649d1 in /tmp/zs-init.patch 
# Wed, 02 Jun 2021 05:28:42 GMT
RUN curl -fSL -o zs-init.tar.gz "http://repos.zend.com/zs-init/zs-init-docker-${ZS_INIT_VERSION}.tar.gz"     && echo "${ZS_INIT_SHA256} *zs-init.tar.gz" | sha256sum -c -     && mkdir /usr/local/zs-init     && tar xzf zs-init.tar.gz --strip-components=1 -C /usr/local/zs-init     && rm zs-init.tar.gz     && patch -u /usr/local/zs-init/src/Init/Steps/AbstractStep.php -i /tmp/zs-init.patch     && rm /tmp/zs-init.patch
# Wed, 02 Jun 2021 05:28:42 GMT
WORKDIR /usr/local/zs-init
# Wed, 02 Jun 2021 05:28:47 GMT
RUN /usr/local/zend/bin/php -r "readfile('https://getcomposer.org/installer');" | /usr/local/zend/bin/php     && /usr/local/zend/bin/php composer.phar update
# Wed, 02 Jun 2021 05:28:48 GMT
COPY dir:eecd98e9ebf1c61a12ae67558eb2a6ce846b9ebfadabbf08503e90b3e30d9496 in /usr/local/bin 
# Wed, 02 Jun 2021 05:28:48 GMT
COPY dir:80bde0d50316e7c9350262fe3b75826a91d075303027787e759d703b60df13d6 in /usr/local/zend/var/plugins/ 
# Wed, 02 Jun 2021 05:28:49 GMT
RUN rm /var/www/html/index.nginx-debian.html
# Wed, 02 Jun 2021 05:28:49 GMT
COPY dir:d174a5d34625889b4356c566972566e0ca7da618b01ea42276562f8186517a67 in /var/www/html 
# Wed, 02 Jun 2021 05:28:49 GMT
EXPOSE 80
# Wed, 02 Jun 2021 05:28:49 GMT
EXPOSE 443
# Wed, 02 Jun 2021 05:28:50 GMT
EXPOSE 10081
# Wed, 02 Jun 2021 05:28:50 GMT
EXPOSE 10082
# Wed, 02 Jun 2021 05:28:50 GMT
WORKDIR /var/www/html
# Wed, 02 Jun 2021 05:28:50 GMT
CMD ["/usr/local/bin/run"]
```

-	Layers:
	-	`sha256:4bbfd2c87b7524455f144a03bf387c88b6d4200e5e0df9139a9d5e79110f89ca`  
		Last Modified: Thu, 13 May 2021 14:54:04 GMT  
		Size: 26.7 MB (26696304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2e110be24e168b42c1a2ddbc4a476a217b73cccdba69cdcb212b812a88f5726`  
		Last Modified: Wed, 19 May 2021 19:45:43 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:889a7173dcfeb409f9d88054a97ab2445f5a799a823f719a5573365ee3662b6f`  
		Last Modified: Wed, 19 May 2021 19:45:43 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9144d071c4b85fa5ab5d409a9918aee04c54ec95cff0423fbff29bdc9685240e`  
		Last Modified: Wed, 19 May 2021 21:32:25 GMT  
		Size: 32.7 MB (32728064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e96ceb4f17e2df5b452408d60928be9a5e68b804d762d43789490bec62c03573`  
		Last Modified: Wed, 19 May 2021 21:32:19 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da8508419d7e817248be0bd87dee89c187aa3e2192cb6c7ad2960d83a0973c04`  
		Last Modified: Wed, 02 Jun 2021 05:29:14 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11874b19716c34cdc712011486d3d85b707d5148f637300e27ae0b2cd9da7296`  
		Last Modified: Wed, 02 Jun 2021 05:29:58 GMT  
		Size: 325.9 MB (325939344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d22002ca86e9fe54d9098dfae1be7184a94e635e0b2b22521cfce75d263ad58`  
		Last Modified: Wed, 02 Jun 2021 05:29:13 GMT  
		Size: 446.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89d86e4e78768ff2a28733e688274954ad50540901ec09edc416724ba54766c1`  
		Last Modified: Wed, 02 Jun 2021 05:29:14 GMT  
		Size: 18.9 KB (18933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c1f13a54a7eef1d4df4c30b2a6fe116ef9f5128d7458e4e480bbff3794b93de`  
		Last Modified: Wed, 02 Jun 2021 05:29:12 GMT  
		Size: 5.1 MB (5143845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6000bc0ffd7edcc58243e31eb96155e1ba001dc53af51045d58dd3091eb1c7e`  
		Last Modified: Wed, 02 Jun 2021 05:29:11 GMT  
		Size: 14.3 KB (14293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7556bf9fbff70fa59c442d318536dfe80b74b5e0b43465bacd26ba0a8582d9e`  
		Last Modified: Wed, 02 Jun 2021 05:29:11 GMT  
		Size: 2.6 KB (2558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:871ae199dc1048e94fb53ec87b9c3c043b51041043893abf2b60bf8435e9c4dc`  
		Last Modified: Wed, 02 Jun 2021 05:29:11 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76d2b9a5806a293d1c8405ee91f90cfb55050d8b97922ea6e47ea5a95c890c28`  
		Last Modified: Wed, 02 Jun 2021 05:29:11 GMT  
		Size: 1.3 KB (1255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
