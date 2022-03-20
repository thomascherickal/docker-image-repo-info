## `php-zendserver:latest`

```console
$ docker pull php-zendserver@sha256:f11d1d4605879a1293437a733f9ed9fe29c5d2fbb72a22d4449850c196b36a1a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `php-zendserver:latest` - linux; amd64

```console
$ docker pull php-zendserver@sha256:d926b94439d727a19ee18e2efe2516daef6ab7195e28e4251c513b3679098006
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **392.6 MB (392644811 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13cd6c8ece1ebefe1b2f6f60d5c070859a9fce2cb2410f39f51498adbdf1d990`
-	Default Command: `["\/usr\/local\/bin\/run"]`

```dockerfile
# Fri, 18 Mar 2022 05:30:26 GMT
ADD file:f554512cb0acad99508554656767804e4821ece488fac0e46fd2c643a39f7021 in / 
# Fri, 18 Mar 2022 05:30:27 GMT
CMD ["bash"]
# Sat, 19 Mar 2022 23:16:22 GMT
RUN apt-get update && apt-get install -y       gnupg
# Sat, 19 Mar 2022 23:16:51 GMT
RUN apt-key adv --keyserver keyserver.ubuntu.com --recv-key 799058698E65316A2E7A4FF42EAE1437F7D2C623
# Sat, 19 Mar 2022 23:18:38 GMT
COPY file:1e70d8fd6f9643bffb703528edddba0aa02a58e95cc53e92f58a86cde29e732a in /etc/apt/sources.list.d/zend-server.list 
# Sat, 19 Mar 2022 23:20:03 GMT
RUN apt-get update && apt-get install -y       iproute2       curl       libmysqlclient20       unzip       git       zend-server-nginx=2021.0.0+b74     && rm -rf /var/lib/apt/lists/*     && /usr/local/zend/bin/zendctl.sh stop
# Sat, 19 Mar 2022 23:20:06 GMT
ENV ZS_INIT_VERSION=0.3
# Sat, 19 Mar 2022 23:20:06 GMT
ENV ZS_INIT_SHA256=e8d441d8503808e9fc0fafc762b2cb80d4a6e68b94fede0fe41efdeac10800cb
# Sat, 19 Mar 2022 23:20:06 GMT
COPY file:ad21ce0b2dc8345be0ef63836774934d6b2045ddc3685411221a07dd10b649d1 in /tmp/zs-init.patch 
# Sat, 19 Mar 2022 23:20:07 GMT
RUN curl -fSL -o zs-init.tar.gz "http://repos.zend.com/zs-init/zs-init-docker-${ZS_INIT_VERSION}.tar.gz"     && echo "${ZS_INIT_SHA256} *zs-init.tar.gz" | sha256sum -c -     && mkdir /usr/local/zs-init     && tar xzf zs-init.tar.gz --strip-components=1 -C /usr/local/zs-init     && rm zs-init.tar.gz     && patch -u /usr/local/zs-init/src/Init/Steps/AbstractStep.php -i /tmp/zs-init.patch     && rm /tmp/zs-init.patch
# Sat, 19 Mar 2022 23:20:07 GMT
WORKDIR /usr/local/zs-init
# Sat, 19 Mar 2022 23:20:13 GMT
RUN /usr/local/zend/bin/php -r "readfile('https://getcomposer.org/installer');" | /usr/local/zend/bin/php     && /usr/local/zend/bin/php composer.phar update
# Sat, 19 Mar 2022 23:20:13 GMT
COPY dir:eecd98e9ebf1c61a12ae67558eb2a6ce846b9ebfadabbf08503e90b3e30d9496 in /usr/local/bin 
# Sat, 19 Mar 2022 23:20:13 GMT
COPY dir:80bde0d50316e7c9350262fe3b75826a91d075303027787e759d703b60df13d6 in /usr/local/zend/var/plugins/ 
# Sat, 19 Mar 2022 23:20:13 GMT
RUN rm /var/www/html/index.nginx-debian.html
# Sat, 19 Mar 2022 23:20:14 GMT
COPY dir:d174a5d34625889b4356c566972566e0ca7da618b01ea42276562f8186517a67 in /var/www/html 
# Sat, 19 Mar 2022 23:20:14 GMT
EXPOSE 80
# Sat, 19 Mar 2022 23:20:14 GMT
EXPOSE 443
# Sat, 19 Mar 2022 23:20:14 GMT
EXPOSE 10081
# Sat, 19 Mar 2022 23:20:14 GMT
EXPOSE 10082
# Sat, 19 Mar 2022 23:20:14 GMT
WORKDIR /var/www/html
# Sat, 19 Mar 2022 23:20:14 GMT
CMD ["/usr/local/bin/run"]
```

-	Layers:
	-	`sha256:11323ed2c65349758e68a03a8e43825ec263dc9790daea93cf83b18ad0703109`  
		Last Modified: Thu, 17 Mar 2022 11:55:05 GMT  
		Size: 26.7 MB (26708634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c5715f36ae1f077308f21070ba121637d1ab1c740a7960c7d7e5bec8f90bc1e`  
		Last Modified: Sat, 19 Mar 2022 23:20:52 GMT  
		Size: 34.8 MB (34766913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be743ad723a813773ebec8e400a8d4df8ddb305f06111a5936bff5f904c7a98d`  
		Last Modified: Sat, 19 Mar 2022 23:20:47 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57c58dc6559c0afa2ce7977343979de6ff3988c48d63a3f442116385a526e538`  
		Last Modified: Sat, 19 Mar 2022 23:21:49 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6823e781efd13bd938cd7c573f0ea60500033c2bfae34b11ce8d184ee96ea49e`  
		Last Modified: Sat, 19 Mar 2022 23:22:32 GMT  
		Size: 325.9 MB (325942293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e840f491b983d347100da8b6ad12a8a8552f310851a5b280fd054adac7fcd52`  
		Last Modified: Sat, 19 Mar 2022 23:21:48 GMT  
		Size: 445.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b83cbb4382785c2a2550cc66f574453c023d9e280e3424d72f76744d163e4862`  
		Last Modified: Sat, 19 Mar 2022 23:21:48 GMT  
		Size: 18.9 KB (18926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4278e27443887bb47bd2931e664ebd9458288afbeadbb7f18ead693a9d0c1f1`  
		Last Modified: Sat, 19 Mar 2022 23:21:48 GMT  
		Size: 5.2 MB (5187685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de37f63080d1e8a55ddafa4d6edeba7b774b559510ea4eb949f4be3cf294abf6`  
		Last Modified: Sat, 19 Mar 2022 23:21:46 GMT  
		Size: 14.3 KB (14293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1830b9819c223674b56e0bddc9b1738a959837455ed0b8ad72ae66e58e5ec09b`  
		Last Modified: Sat, 19 Mar 2022 23:21:46 GMT  
		Size: 2.6 KB (2559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16b5f8536def455a5675fc37d8fbb7fc64c8983b653183a208204ae08abd8d87`  
		Last Modified: Sat, 19 Mar 2022 23:21:46 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5da6f5aebab796803c667b1bba016d46ee00f2b8a93dcd8fbc136df3e9dbdd6f`  
		Last Modified: Sat, 19 Mar 2022 23:21:46 GMT  
		Size: 1.3 KB (1251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
