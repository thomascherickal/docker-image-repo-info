## `php-zendserver:latest`

```console
$ docker pull php-zendserver@sha256:22202e7a06ea9e6dc0b71816a8bb57f0cce285f46162df709f3cc142d3f74efb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `php-zendserver:latest` - linux; amd64

```console
$ docker pull php-zendserver@sha256:78c50b694d76ea6cef8b7eb2380743c3988d02b3c74460c3f2bfd6109ce65aa1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **391.4 MB (391393272 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a801ad603282e150468e7f1c5ce93b595cfa1ff8f54125fcaf18cb71f5b4d24b`
-	Default Command: `["\/usr\/local\/bin\/run"]`

```dockerfile
# Tue, 13 Jul 2021 22:29:15 GMT
ADD file:7274ece1917848683250bbeda9eacf6eb7510481cbaa177880e3a60b4133e35b in / 
# Tue, 13 Jul 2021 22:29:15 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 01:12:31 GMT
RUN apt-get update && apt-get install -y       gnupg
# Wed, 14 Jul 2021 01:12:34 GMT
RUN apt-key adv --keyserver keyserver.ubuntu.com --recv-key 799058698E65316A2E7A4FF42EAE1437F7D2C623
# Wed, 14 Jul 2021 01:14:33 GMT
COPY file:1e70d8fd6f9643bffb703528edddba0aa02a58e95cc53e92f58a86cde29e732a in /etc/apt/sources.list.d/zend-server.list 
# Wed, 14 Jul 2021 01:16:08 GMT
RUN apt-get update && apt-get install -y       iproute2       curl       libmysqlclient20       unzip       git       zend-server-nginx=2021.0.0+b74     && rm -rf /var/lib/apt/lists/*     && /usr/local/zend/bin/zendctl.sh stop
# Wed, 14 Jul 2021 01:16:11 GMT
ENV ZS_INIT_VERSION=0.3
# Wed, 14 Jul 2021 01:16:11 GMT
ENV ZS_INIT_SHA256=e8d441d8503808e9fc0fafc762b2cb80d4a6e68b94fede0fe41efdeac10800cb
# Wed, 14 Jul 2021 01:16:12 GMT
COPY file:ad21ce0b2dc8345be0ef63836774934d6b2045ddc3685411221a07dd10b649d1 in /tmp/zs-init.patch 
# Wed, 14 Jul 2021 01:16:13 GMT
RUN curl -fSL -o zs-init.tar.gz "http://repos.zend.com/zs-init/zs-init-docker-${ZS_INIT_VERSION}.tar.gz"     && echo "${ZS_INIT_SHA256} *zs-init.tar.gz" | sha256sum -c -     && mkdir /usr/local/zs-init     && tar xzf zs-init.tar.gz --strip-components=1 -C /usr/local/zs-init     && rm zs-init.tar.gz     && patch -u /usr/local/zs-init/src/Init/Steps/AbstractStep.php -i /tmp/zs-init.patch     && rm /tmp/zs-init.patch
# Wed, 14 Jul 2021 01:16:13 GMT
WORKDIR /usr/local/zs-init
# Wed, 14 Jul 2021 01:16:19 GMT
RUN /usr/local/zend/bin/php -r "readfile('https://getcomposer.org/installer');" | /usr/local/zend/bin/php     && /usr/local/zend/bin/php composer.phar update
# Wed, 14 Jul 2021 01:16:19 GMT
COPY dir:eecd98e9ebf1c61a12ae67558eb2a6ce846b9ebfadabbf08503e90b3e30d9496 in /usr/local/bin 
# Wed, 14 Jul 2021 01:16:19 GMT
COPY dir:80bde0d50316e7c9350262fe3b75826a91d075303027787e759d703b60df13d6 in /usr/local/zend/var/plugins/ 
# Wed, 14 Jul 2021 01:16:20 GMT
RUN rm /var/www/html/index.nginx-debian.html
# Wed, 14 Jul 2021 01:16:20 GMT
COPY dir:d174a5d34625889b4356c566972566e0ca7da618b01ea42276562f8186517a67 in /var/www/html 
# Wed, 14 Jul 2021 01:16:21 GMT
EXPOSE 80
# Wed, 14 Jul 2021 01:16:21 GMT
EXPOSE 443
# Wed, 14 Jul 2021 01:16:21 GMT
EXPOSE 10081
# Wed, 14 Jul 2021 01:16:21 GMT
EXPOSE 10082
# Wed, 14 Jul 2021 01:16:21 GMT
WORKDIR /var/www/html
# Wed, 14 Jul 2021 01:16:21 GMT
CMD ["/usr/local/bin/run"]
```

-	Layers:
	-	`sha256:e7ae86ffe2df0787131a4c49ace1b018fd38d62929b007d86bdd1f825e56a852`  
		Last Modified: Tue, 13 Jul 2021 22:31:03 GMT  
		Size: 26.7 MB (26706145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8de183e035e709c1e5fed2938e70420b7979e30238eb0de17f0a39068d0883cb`  
		Last Modified: Wed, 14 Jul 2021 01:16:50 GMT  
		Size: 33.0 MB (33012271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6f5a0de9e1fd7cf67635fcdcda6e01047403e83bbc17b37113789995422a5c9`  
		Last Modified: Wed, 14 Jul 2021 01:16:46 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff4b2d2466f74e6c1d163757e6e30dc57303b1f59a662ad0e6537568b19c0410`  
		Last Modified: Wed, 14 Jul 2021 01:17:53 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48be3b7ead7b80e2a96c975ca815e6bcec16d1612490e72f0c1ac6479aee5ffd`  
		Last Modified: Wed, 14 Jul 2021 01:18:38 GMT  
		Size: 326.5 MB (326487592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:006bb9907fcb2fb5318a5175aea53d6c6a1b662a743fc49f09b777fbf0f524a2`  
		Last Modified: Wed, 14 Jul 2021 01:17:52 GMT  
		Size: 446.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3fb07b13da720ac14fa595803b85b9d73edb29ad78af8f7920fefafa5508ba6`  
		Last Modified: Wed, 14 Jul 2021 01:17:52 GMT  
		Size: 18.9 KB (18927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a40c39b850bd96b83eff14a79b34b10a1bfb2ab584e7c6559e497f0ada4d289f`  
		Last Modified: Wed, 14 Jul 2021 01:17:51 GMT  
		Size: 5.1 MB (5147953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75836954c4ac76fb31d97ca91c4bd92af4f0885e25722a8084c1098e31a5c2d3`  
		Last Modified: Wed, 14 Jul 2021 01:17:50 GMT  
		Size: 14.3 KB (14298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef3c4cd48ccb9fee1cde4f1b305561806ca63f516e95f0d85f259686243edde3`  
		Last Modified: Wed, 14 Jul 2021 01:17:49 GMT  
		Size: 2.6 KB (2568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e66c16476b52b88d850567e5ef0220b4c3cc64b1c6aa619dffddef822ad8aebf`  
		Last Modified: Wed, 14 Jul 2021 01:17:49 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b56ee74df91be6a97cc1c7b5809d4c09941151b002ed5ff33c8c0a66ea2e7de`  
		Last Modified: Wed, 14 Jul 2021 01:17:50 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
