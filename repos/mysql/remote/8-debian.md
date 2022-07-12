## `mysql:8-debian`

```console
$ docker pull mysql@sha256:5ef1130b5a6ebd5c2f31f0244c25027c47fb5a7279ad747026b495414adaaf27
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:8-debian` - linux; amd64

```console
$ docker pull mysql@sha256:3a7e864bc88458911fa598065fe027736fa63495f5780ee0618caeb4a52bbc4c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **157.4 MB (157380412 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0fc0e2322d42dbab9448b7af63601f09cbd916193afec376675bf32fdbca5203`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 12 Jul 2022 01:20:10 GMT
ADD file:d978f6d3025a06f5142a0c13c98bf12fbd47cdf9162ed31fbc05c86983b0a679 in / 
# Tue, 12 Jul 2022 01:20:10 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 01:49:49 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 12 Jul 2022 01:49:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 01:49:56 GMT
ENV GOSU_VERSION=1.14
# Tue, 12 Jul 2022 01:50:05 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 12 Jul 2022 01:50:05 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 12 Jul 2022 01:50:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 01:50:12 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Tue, 12 Jul 2022 01:50:12 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 12 Jul 2022 01:50:12 GMT
ENV MYSQL_VERSION=8.0.29-1debian11
# Tue, 12 Jul 2022 01:50:13 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ bullseye mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Tue, 12 Jul 2022 01:50:28 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 12 Jul 2022 01:50:29 GMT
VOLUME [/var/lib/mysql]
# Tue, 12 Jul 2022 01:50:29 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Tue, 12 Jul 2022 01:50:29 GMT
COPY file:d27cf504fa76fb5a4038020a01eaaf52723b17b751566119de311adacb043752 in /usr/local/bin/ 
# Tue, 12 Jul 2022 01:50:29 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 12 Jul 2022 01:50:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Jul 2022 01:50:30 GMT
EXPOSE 3306 33060
# Tue, 12 Jul 2022 01:50:30 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:461246efe0a75316d99afdbf348f7063b57b0caeee8daab775f1f08152ea36f4`  
		Last Modified: Tue, 12 Jul 2022 01:24:34 GMT  
		Size: 31.4 MB (31366610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1cd5bb1f5de5503f17b383d7c62078467389f82828ac46a41db64289ecf9880`  
		Last Modified: Tue, 12 Jul 2022 01:52:26 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd9d402d85bd06018ec1a89d3298f4d88f3c4d06c2cd93c8951d8bbb19596ace`  
		Last Modified: Tue, 12 Jul 2022 01:52:26 GMT  
		Size: 4.4 MB (4414786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33a04621f5daa2ee95b4484e11cb963f929686d8f77511d9e31d8cf63d2a491b`  
		Last Modified: Tue, 12 Jul 2022 01:52:24 GMT  
		Size: 1.4 MB (1418425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2eef8024049f6e7f8a7769c0ed43bc5ddab7c1b3dbc772a3ba1b71a039bff03`  
		Last Modified: Tue, 12 Jul 2022 01:52:23 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a021c48082a6778bc62f96a17b8202ad24185d41b54fad0c4788d55e18a106b1`  
		Last Modified: Tue, 12 Jul 2022 01:52:26 GMT  
		Size: 12.7 MB (12661669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a27a84090d2f2cc8e7bc9db5098fe5f2c61aaf38e003421fab9630fdf6541c2`  
		Last Modified: Tue, 12 Jul 2022 01:52:23 GMT  
		Size: 2.5 KB (2547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7ddfbeb275b283abe3dfc3de542ebdcc701c4c996a96c2be39ed59e5137ac83`  
		Last Modified: Tue, 12 Jul 2022 01:52:21 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29fbdc9d2624616a1188b80790c80688aba8f17538b784d1ec937ba763d0caca`  
		Last Modified: Tue, 12 Jul 2022 01:52:38 GMT  
		Size: 107.5 MB (107508121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87a306bac37ec6ca492ea124d5aab4a2015656c9bbcf1d82aa693a2df13241d1`  
		Last Modified: Tue, 12 Jul 2022 01:52:21 GMT  
		Size: 845.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3396c7604c38680b49a32a26d9e55ae095981acb8d33fd75c844fa5b6b0edc39`  
		Last Modified: Tue, 12 Jul 2022 01:52:21 GMT  
		Size: 5.2 KB (5157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:832af0332a2a6d268d5173bf633da9f00789d1970b6992fba3a7c49b208aca38`  
		Last Modified: Tue, 12 Jul 2022 01:52:21 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
