## `mysql:5-debian`

```console
$ docker pull mysql@sha256:849a8e87076f75717e1f98102ed1545396faab1cb2c99c768bf2b5b430571604
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5-debian` - linux; amd64

```console
$ docker pull mysql@sha256:2bbef75b058643f5a747c13661a88ee3301df9e25f0eaeb358587cc37da86afc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **162.7 MB (162693934 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:88338e85f040d97b75f2d43518736f4af9e52fa4c4c577cd34b134273a079266`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 23 Mar 2023 01:30:50 GMT
ADD file:52316aa7d631242cd16337be337e57187ef07d3965e6284321fbdcd5b4f92b64 in / 
# Thu, 23 Mar 2023 01:30:51 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 11:00:21 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 23 Mar 2023 11:00:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 11:00:28 GMT
ENV GOSU_VERSION=1.16
# Thu, 23 Mar 2023 11:00:37 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Mar 2023 11:00:37 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 23 Mar 2023 11:00:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 11:00:45 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Thu, 23 Mar 2023 11:00:45 GMT
ENV MYSQL_MAJOR=5.7
# Thu, 23 Mar 2023 11:00:45 GMT
ENV MYSQL_VERSION=5.7.41-1debian10
# Thu, 23 Mar 2023 11:00:46 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-5.7' > /etc/apt/sources.list.d/mysql.list
# Thu, 23 Mar 2023 11:01:03 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-server="${MYSQL_VERSION}" 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Thu, 23 Mar 2023 11:01:04 GMT
VOLUME [/var/lib/mysql]
# Thu, 23 Mar 2023 11:01:04 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Thu, 23 Mar 2023 11:01:05 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 23 Mar 2023 11:01:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Mar 2023 11:01:05 GMT
EXPOSE 3306 33060
# Thu, 23 Mar 2023 11:01:05 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:3689b8de819b48387712c6d4d62d26a52a04c9e88afc68fb9d1dbe48bfa9e21d`  
		Last Modified: Thu, 23 Mar 2023 01:35:01 GMT  
		Size: 27.1 MB (27139869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27ac63a14e4479941312ab4b314bbd36b8eed13e848b7446b33d62d1cf387c14`  
		Last Modified: Thu, 23 Mar 2023 11:01:59 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17a94b43bbfe3822fc0a3c87da156138a81cec71bf1b9a2e00f3acc1b9819eca`  
		Last Modified: Thu, 23 Mar 2023 11:01:58 GMT  
		Size: 4.2 MB (4182339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38763e84573623aeb1cff67387112f2d0b31e5ed0b899e3b3a126770e46d8b94`  
		Last Modified: Thu, 23 Mar 2023 11:01:58 GMT  
		Size: 1.4 MB (1441745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bcbc7fd4a2d7d18a737618196f4d75de0a316eaf5c125b2d4d35a7eb037426d`  
		Last Modified: Thu, 23 Mar 2023 11:01:57 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19764d7bd70a9eea88bec2db9d035ffe9224b9dcd7c0613e42f63b775f8f75d3`  
		Last Modified: Thu, 23 Mar 2023 11:02:00 GMT  
		Size: 14.1 MB (14086905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8a2769597f7f726053839c80035384b62ea02c2f3dafa473e5200c96236b67c`  
		Last Modified: Thu, 23 Mar 2023 11:01:55 GMT  
		Size: 2.5 KB (2550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55969b3a4225bf2037f3ccfc7930ed5b0cfed7aeee036deb0d7aee144dfbc425`  
		Last Modified: Thu, 23 Mar 2023 11:01:55 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f4898aaf83c5d2f75aa7c90e3936fb2faf0f565889f5973fb820f1330cff028`  
		Last Modified: Thu, 23 Mar 2023 11:02:10 GMT  
		Size: 115.8 MB (115832889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae9972a98a4d99007516b2303bc1ca8e06d9696adff985ac28b4f52bbb086738`  
		Last Modified: Thu, 23 Mar 2023 11:01:55 GMT  
		Size: 5.4 KB (5385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9b8313553fddc90f14c25b3007f8f77459244ac46fbcd5580f9f3c31ba6a0d1`  
		Last Modified: Thu, 23 Mar 2023 11:01:55 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
