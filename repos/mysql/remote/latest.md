## `mysql:latest`

```console
$ docker pull mysql@sha256:dc3cdcf3025c3257e8047bb0eaee9d5a42d9f694f84fc5e7b6d12710ba7f6fcb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:latest` - linux; amd64

```console
$ docker pull mysql@sha256:dc7738aabdbd169a07e473ced756abfc6f873ce607e9437914071c90e0a0f51f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.9 MB (155885566 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b2500a44757fb9f9eef2089840ea3d7f1f53f36000e500853904786a291a7093`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 11 May 2022 01:20:37 GMT
ADD file:76b454ddb7dfe4d22afae844a7e67e7e5fb4570dae2e21bbd259a1f2e5839f33 in / 
# Wed, 11 May 2022 01:20:37 GMT
CMD ["bash"]
# Wed, 11 May 2022 05:01:23 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 11 May 2022 05:01:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 05:01:29 GMT
ENV GOSU_VERSION=1.14
# Wed, 11 May 2022 05:01:38 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 11 May 2022 05:01:39 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 11 May 2022 05:01:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 05:01:46 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Wed, 11 May 2022 05:01:46 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 11 May 2022 05:01:46 GMT
ENV MYSQL_VERSION=8.0.29-1debian10
# Wed, 11 May 2022 05:01:47 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Wed, 11 May 2022 05:02:01 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Wed, 11 May 2022 05:02:02 GMT
VOLUME [/var/lib/mysql]
# Wed, 11 May 2022 05:02:02 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Mon, 23 May 2022 23:37:51 GMT
COPY file:d27cf504fa76fb5a4038020a01eaaf52723b17b751566119de311adacb043752 in /usr/local/bin/ 
# Mon, 23 May 2022 23:37:52 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 23 May 2022 23:37:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 23 May 2022 23:37:52 GMT
EXPOSE 3306 33060
# Mon, 23 May 2022 23:37:52 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:c32ce6654453d35d0b3dde45d195adeee586ffba0a683006ee06748c077c01fa`  
		Last Modified: Wed, 11 May 2022 01:25:58 GMT  
		Size: 27.1 MB (27140722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:415d08ee031ab3bffe8c0db6b82f2cde88049eda62a50801eb6d8aa68bb0e12c`  
		Last Modified: Wed, 11 May 2022 05:03:03 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a38fec2542ffcfa6247f2992d1ec422b38e00ed5ca998bc5b890ca1a97ab1d5`  
		Last Modified: Wed, 11 May 2022 05:03:04 GMT  
		Size: 4.2 MB (4179283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:352881ee8fe9b63edbd90eb3a1ffa035c72b7edfbcad6fda55db516c2a2b2cb9`  
		Last Modified: Wed, 11 May 2022 05:03:02 GMT  
		Size: 1.4 MB (1386677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8e20da291b6c92de4aa28a02fe8845045ec68d9b9ad1497e921fa42e8303650`  
		Last Modified: Wed, 11 May 2022 05:03:01 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66c2a8cc1999eedaa968d140339f25947e1faf8b3f2084c7eb5eee68455d6295`  
		Last Modified: Wed, 11 May 2022 05:03:03 GMT  
		Size: 14.1 MB (14064393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3a3a8e49878cc1f98a4927704e4fdc191bcc2cc80fbf7470b36fe1b44b7596d`  
		Last Modified: Wed, 11 May 2022 05:03:01 GMT  
		Size: 2.5 KB (2548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e33a48832bec0e74023cbd16a908bc440f32f292f7db67c91de8114199145984`  
		Last Modified: Wed, 11 May 2022 05:02:58 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:410b942b8b28385f3aa8f160e5cfa770f39b81c059e6842d17ac37a75aa573c5`  
		Last Modified: Wed, 11 May 2022 05:03:15 GMT  
		Size: 109.1 MB (109103697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5323c9dd265c14ee05d2fef4d1a2116eeb2199a40af1ffbd3895f282b7aac05`  
		Last Modified: Wed, 11 May 2022 05:02:59 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e51041021063c0c624c5f6ffcf317a1be857f75442a44d706603e4c03a595cc7`  
		Last Modified: Mon, 23 May 2022 23:38:38 GMT  
		Size: 5.2 KB (5152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b68b4cbc496eaf65ee90a5c221bc53000a1ce7995d42d85b57e69e6350a584c8`  
		Last Modified: Mon, 23 May 2022 23:38:38 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
