## `mysql:8-debian`

```console
$ docker pull mysql@sha256:504760f722770e8554c40e7ea6b803ae9e0c19e21e25b94d0b8a03bab20541ff
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:8-debian` - linux; amd64

```console
$ docker pull mysql@sha256:9a16d88a3410a326a082261a64db5624902fc763775410663cc44420968831a3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **157.8 MB (157835607 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c2ee58f241ef6265fbc87840afec971c52938a5bcc38259e71bb0ad0363e827e`
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
# Tue, 26 Jul 2022 23:28:31 GMT
ENV MYSQL_VERSION=8.0.30-1debian11
# Tue, 26 Jul 2022 23:28:31 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ bullseye mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Tue, 26 Jul 2022 23:28:45 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 26 Jul 2022 23:28:45 GMT
VOLUME [/var/lib/mysql]
# Tue, 26 Jul 2022 23:28:45 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Tue, 26 Jul 2022 23:28:46 GMT
COPY file:d27cf504fa76fb5a4038020a01eaaf52723b17b751566119de311adacb043752 in /usr/local/bin/ 
# Tue, 26 Jul 2022 23:28:46 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 26 Jul 2022 23:28:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 26 Jul 2022 23:28:46 GMT
EXPOSE 3306 33060
# Tue, 26 Jul 2022 23:28:46 GMT
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
	-	`sha256:40bc66f09ecd05d38547cb872afb8703d21702dcbd68f1688e69c1fa899b9bfe`  
		Last Modified: Tue, 26 Jul 2022 23:31:05 GMT  
		Size: 256.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57a0b87a3f7d2dd5b0a2ba39b526929f321b90da90a2249caf4da175b9b19e70`  
		Last Modified: Tue, 26 Jul 2022 23:31:22 GMT  
		Size: 108.0 MB (107963313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44e82ef1aa7cd91168ba63bd5724afa619590e17c79d641515a3a0f23bf75839`  
		Last Modified: Tue, 26 Jul 2022 23:31:05 GMT  
		Size: 842.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f04800ad7ccd34e26a26464cfa045c9030672e0bc018c05b370e55acce1d02e`  
		Last Modified: Tue, 26 Jul 2022 23:31:05 GMT  
		Size: 5.2 KB (5157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6593ab5ec7351b0dba0042dd7086bb2ae362d26cd4c7be288dfc618a7884ea15`  
		Last Modified: Tue, 26 Jul 2022 23:31:05 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
