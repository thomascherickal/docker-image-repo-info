## `mysql:5-debian`

```console
$ docker pull mysql@sha256:1e637483dfa9e3f2027357f1e8fc566f5c01b7c0a7da1f2408a8b2e8661c785d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5-debian` - linux; amd64

```console
$ docker pull mysql@sha256:ce9f3f34ced66d8f1134cae332db346b99eac57fe98151b66d332273ad37e0a4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **162.7 MB (162697008 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:098b17901f722f8abb61238c31204b90b65986117f25b494725bb3a580346a0f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 04 Feb 2023 06:52:07 GMT
ADD file:4fbe1e3712cf37c85529cc81e0d03c82085203de00d64b0d669b5996e975925a in / 
# Sat, 04 Feb 2023 06:52:07 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 14:48:23 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Sat, 04 Feb 2023 14:48:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 14:48:28 GMT
ENV GOSU_VERSION=1.16
# Sat, 04 Feb 2023 14:48:37 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 04 Feb 2023 14:48:38 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 04 Feb 2023 14:48:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 14:48:45 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Sat, 04 Feb 2023 14:48:45 GMT
ENV MYSQL_MAJOR=5.7
# Sat, 04 Feb 2023 14:48:45 GMT
ENV MYSQL_VERSION=5.7.41-1debian10
# Sat, 04 Feb 2023 14:48:46 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-5.7' > /etc/apt/sources.list.d/mysql.list
# Sat, 04 Feb 2023 14:49:04 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-server="${MYSQL_VERSION}" 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Sat, 04 Feb 2023 14:49:05 GMT
VOLUME [/var/lib/mysql]
# Sat, 04 Feb 2023 14:49:05 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Sat, 04 Feb 2023 14:49:06 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Sat, 04 Feb 2023 14:49:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 04 Feb 2023 14:49:06 GMT
EXPOSE 3306 33060
# Sat, 04 Feb 2023 14:49:06 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:0cf508b37688dca559387b506062329202aaf08b48be5f55f9278b2a818ad2c9`  
		Last Modified: Sat, 04 Feb 2023 06:56:58 GMT  
		Size: 27.1 MB (27140353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa52c08f6d64c27c8bbc7f78f8368224b99c37b48e8343a9d0364d33d779de21`  
		Last Modified: Sat, 04 Feb 2023 14:50:13 GMT  
		Size: 1.7 KB (1729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47f717ed1938dd429e6bf1387feb8f1365db34cc1e17ae307ed79d89cfef28f8`  
		Last Modified: Sat, 04 Feb 2023 14:50:12 GMT  
		Size: 4.2 MB (4182319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a135a3b62b02e7b6e0becd2e51dab4b8d1c0c0fc1d8bfb45dba78e63e5c9bd4`  
		Last Modified: Sat, 04 Feb 2023 14:50:12 GMT  
		Size: 1.4 MB (1441725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cd96155287dc7fa118c3ef4c5b929337571a489a4e01a879313dd1e53c25612`  
		Last Modified: Sat, 04 Feb 2023 14:50:11 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:139136d0303f40fe184d71465c0d8eaad987d48ceb1dba15bd99d77d8e1a11ad`  
		Last Modified: Sat, 04 Feb 2023 14:50:14 GMT  
		Size: 14.1 MB (14089433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89eaaf4eeed62dee382967f65959afb060a8e0ed386be7ad8038a98548075ece`  
		Last Modified: Sat, 04 Feb 2023 14:50:10 GMT  
		Size: 2.5 KB (2549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d277fa21096ee1963f0dbd04bedb91574e4eb14db48230f23b6158828b685575`  
		Last Modified: Sat, 04 Feb 2023 14:50:10 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5a4d032701adf22ae19c0ca5e82bd887758807d9557541db8039a699b120ca0`  
		Last Modified: Sat, 04 Feb 2023 14:50:25 GMT  
		Size: 115.8 MB (115832990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce4f39afc4d329d98aa5f9d8c441455b653db63f99e280f36a58363618988837`  
		Last Modified: Sat, 04 Feb 2023 14:50:10 GMT  
		Size: 5.4 KB (5391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39b6afcd59994a6e603ab93368f70455a849f21899602cd7f2fab9292be534b6`  
		Last Modified: Sat, 04 Feb 2023 14:50:10 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
