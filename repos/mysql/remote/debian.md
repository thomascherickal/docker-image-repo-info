## `mysql:debian`

```console
$ docker pull mysql@sha256:3cebdc40926f61eaac83b5ea26388f8fa770e7636c2ea930421cc5604a41a247
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:debian` - linux; amd64

```console
$ docker pull mysql@sha256:3463914132e73c14c172cd4a94da9c66d0baa1a315b16161f462921193e36aa6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **177.8 MB (177751835 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf20690ccd77820231956c3b7385b477bcd57afe216412e84b5c0166e04cab52`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 04 Feb 2023 06:51:41 GMT
ADD file:1d256392bb7afe6942d157db84ca62774ac4114f8a3816fd50bace8d73130b57 in / 
# Sat, 04 Feb 2023 06:51:41 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 14:47:32 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 04 Feb 2023 14:47:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 14:47:38 GMT
ENV GOSU_VERSION=1.16
# Sat, 04 Feb 2023 14:47:45 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 04 Feb 2023 14:47:46 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 04 Feb 2023 14:47:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 14:47:53 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Sat, 04 Feb 2023 14:47:53 GMT
ENV MYSQL_MAJOR=8.0
# Sat, 04 Feb 2023 14:47:53 GMT
ENV MYSQL_VERSION=8.0.32-1debian11
# Sat, 04 Feb 2023 14:47:54 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ bullseye mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Sat, 04 Feb 2023 14:48:09 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Sat, 04 Feb 2023 14:48:10 GMT
VOLUME [/var/lib/mysql]
# Sat, 04 Feb 2023 14:48:10 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Sat, 04 Feb 2023 14:48:10 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Sat, 04 Feb 2023 14:48:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Sat, 04 Feb 2023 14:48:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 04 Feb 2023 14:48:11 GMT
EXPOSE 3306 33060
# Sat, 04 Feb 2023 14:48:11 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:01b5b2efb836d74b8b49da819514eca52e25290d1688db59420ffb9c6b65a03c`  
		Last Modified: Sat, 04 Feb 2023 06:56:17 GMT  
		Size: 31.4 MB (31396919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4957656d4d97b158dafcf9f7ea1e52ce85827e65d97a1fce33f22b024e0d659f`  
		Last Modified: Sat, 04 Feb 2023 14:49:37 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6013719e001ed5ce0cbc7cdff4ae1f79c141597caa27a8006e92a6326e53345a`  
		Last Modified: Sat, 04 Feb 2023 14:49:38 GMT  
		Size: 4.4 MB (4414927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1aa6814d598d5914d9926ec0a5a04fcc6e790afabc91f4766372af106c17acd2`  
		Last Modified: Sat, 04 Feb 2023 14:49:36 GMT  
		Size: 1.5 MB (1471342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62c8eaab45d1b1d84217a009b1ed704b791e724afbf410b70e19cccba16330e7`  
		Last Modified: Sat, 04 Feb 2023 14:49:35 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf5f646a9bb01ef05b95b959b0aa365de8bfd5b41ee6f963d2f9f053a176ac2d`  
		Last Modified: Sat, 04 Feb 2023 14:49:38 GMT  
		Size: 12.7 MB (12662023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74f77555863007461c120a08bff5a4064950f9480c943803faeab52ce0195ecd`  
		Last Modified: Sat, 04 Feb 2023 14:49:35 GMT  
		Size: 2.5 KB (2547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f26b2b4e771728df08c074cb278d9d41dd87e6048ec1eccfb1206e01d5e4f8f`  
		Last Modified: Sat, 04 Feb 2023 14:49:33 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b587ff3b05d9015e5d9471aceedbbdff6e371c2b9ae923af273addce00abfbd1`  
		Last Modified: Sat, 04 Feb 2023 14:49:53 GMT  
		Size: 127.8 MB (127795588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58f0c92d7ddeafcc2949667f9fbf63dfaff447ad17cff156957fe4e38ca45aac`  
		Last Modified: Sat, 04 Feb 2023 14:49:33 GMT  
		Size: 845.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5690a3da4b66efa9e50222b88182474283b4dda3ddd5e7bfee83568005657562`  
		Last Modified: Sat, 04 Feb 2023 14:49:33 GMT  
		Size: 5.4 KB (5390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23b8d1d871af097f1efb61a6f8f1c623aa6b6201969f6367182c8d03aab0186e`  
		Last Modified: Sat, 04 Feb 2023 14:49:33 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
