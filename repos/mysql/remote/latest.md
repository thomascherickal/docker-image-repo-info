## `mysql:latest`

```console
$ docker pull mysql@sha256:345ccdb5028d5719425b7798a2519d5cd069f9191f47acb18a04d9a138c09f86
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mysql:latest` - linux; amd64

```console
$ docker pull mysql@sha256:9cd5e9b89460a80ce4612f4440f77fdf496885c839882158e700b115044547b6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **159.1 MB (159104687 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d1e1a2546718391644cf7cbb66a391e45ef170a764b46331eb75acb0ee9d612`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 16 Apr 2020 03:22:36 GMT
ADD file:865f9041e12eb341f0a394764ddc11db49cbc8b91d4fb57c6fb1960b68b1bb41 in / 
# Thu, 16 Apr 2020 03:22:36 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 10:04:13 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 16 Apr 2020 10:04:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Fri, 17 Apr 2020 16:56:29 GMT
ENV GOSU_VERSION=1.12
# Fri, 17 Apr 2020 16:56:37 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 17 Apr 2020 16:56:38 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 17 Apr 2020 16:56:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		pwgen 		openssl 		perl 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Fri, 17 Apr 2020 16:56:46 GMT
RUN set -ex; 	key='A4A9406876FCBD3C456770C88C718D3B5072E1F5'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list > /dev/null
# Fri, 17 Apr 2020 16:56:46 GMT
ENV MYSQL_MAJOR=8.0
# Fri, 17 Apr 2020 16:56:46 GMT
ENV MYSQL_VERSION=8.0.19-1debian10
# Fri, 17 Apr 2020 16:56:47 GMT
RUN echo "deb http://repo.mysql.com/apt/debian/ buster mysql-${MYSQL_MAJOR}" > /etc/apt/sources.list.d/mysql.list
# Fri, 17 Apr 2020 16:57:04 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update && apt-get install -y mysql-community-client="${MYSQL_VERSION}" mysql-community-server-core="${MYSQL_VERSION}" && rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 777 /var/run/mysqld
# Fri, 17 Apr 2020 16:57:04 GMT
VOLUME [/var/lib/mysql]
# Fri, 17 Apr 2020 16:57:05 GMT
COPY dir:478f098f3681084f7493af1f04cbcd3eeda6f10e0dd2f5c740acd25328a73455 in /etc/mysql/ 
# Wed, 22 Apr 2020 23:39:17 GMT
COPY file:b09451ebd8fb98d90335352b9649da1b3336a789513bb4ae725c9eadafd519b6 in /usr/local/bin/ 
# Wed, 22 Apr 2020 23:39:18 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 22 Apr 2020 23:39:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Apr 2020 23:39:18 GMT
EXPOSE 3306 33060
# Wed, 22 Apr 2020 23:39:18 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:123275d6e508d282237a22fefa5aef822b719a06496444ea89efa65da523fc4b`  
		Last Modified: Thu, 16 Apr 2020 03:31:44 GMT  
		Size: 27.1 MB (27098147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27cddf5c7140b7596d94da456329ec66b76241f435e586f4390362a57d7b26ab`  
		Last Modified: Thu, 16 Apr 2020 10:07:32 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c17d442e14c91a582a572491492c59628829de516e8372b06ab961a10618d92a`  
		Last Modified: Thu, 16 Apr 2020 10:07:33 GMT  
		Size: 4.2 MB (4178047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eb72ffed068adb89481349a9567db21d4db73857b43a5f1998fb39b5cb91dbd`  
		Last Modified: Fri, 17 Apr 2020 16:58:49 GMT  
		Size: 1.4 MB (1419257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4aa125eb616aacd4ccd43ea64e2c9f00018c68353ba7c554b3372263e403917`  
		Last Modified: Fri, 17 Apr 2020 16:58:49 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52560afb169c1c6ad2d041db598538c1e2e488dacd6aa151611af1e82f024666`  
		Last Modified: Fri, 17 Apr 2020 16:58:53 GMT  
		Size: 13.4 MB (13442923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68190f37a1d2753e3d0d552f60fe63c8620cbc28a2dc72400cb3710da7fc428f`  
		Last Modified: Fri, 17 Apr 2020 16:58:49 GMT  
		Size: 2.4 KB (2393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dc788993ca17123a6c2f14276242dcb1bf8342d87ac632dee9fd09ce5362750`  
		Last Modified: Fri, 17 Apr 2020 16:58:48 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a69f7038d031ebfe4a43347e722c2fea87c7877b0694580731554e82390ba5ca`  
		Last Modified: Fri, 17 Apr 2020 16:59:13 GMT  
		Size: 113.0 MB (112955694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:354e8f26557174eebb5947ea0d8e3ed41755ec9dba095e3ed92769cba4f62459`  
		Last Modified: Fri, 17 Apr 2020 16:58:48 GMT  
		Size: 898.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5474d95704d1845ee6d1806d26be96b026aac0edb7fc928fe40bcc11a4fcc160`  
		Last Modified: Wed, 22 Apr 2020 23:39:37 GMT  
		Size: 5.1 KB (5131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11a4858de488b1fafbca2f1df01a7ab4451b1b7327adfdcd942106471fcd3e0d`  
		Last Modified: Wed, 22 Apr 2020 23:39:37 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
