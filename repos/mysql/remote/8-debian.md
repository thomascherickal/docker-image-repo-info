## `mysql:8-debian`

```console
$ docker pull mysql@sha256:ee1e7bf1a6c7f7fc26abbbed04b6e0ab6f202b48c50ef8f418324901420b207e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:8-debian` - linux; amd64

```console
$ docker pull mysql@sha256:8dd2269034dd8680a2d90403977c9604bbaeb0e30364d105340a50241245785c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **179.7 MB (179716143 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a7faa2f9a3fde46c5e8c2d1b5c8d0fb9372a5707162e3b2826fe59478a54cce`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 12 Jun 2023 23:21:07 GMT
ADD file:5ab44909c2983e19ab6596e7e4ee9ad80e48afeb9dfe0e7224afdae7cafd25ef in / 
# Mon, 12 Jun 2023 23:21:08 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 07:06:11 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 13 Jun 2023 07:06:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg && rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 07:06:17 GMT
ENV GOSU_VERSION=1.16
# Tue, 13 Jun 2023 07:06:25 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Jun 2023 07:06:25 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Jun 2023 07:06:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 07:06:32 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Tue, 13 Jun 2023 07:06:32 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 13 Jun 2023 07:06:32 GMT
ENV MYSQL_VERSION=8.0.33-1debian11
# Tue, 13 Jun 2023 07:06:33 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ bullseye mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Tue, 13 Jun 2023 07:06:47 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 13 Jun 2023 07:06:48 GMT
VOLUME [/var/lib/mysql]
# Tue, 13 Jun 2023 07:06:48 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Tue, 13 Jun 2023 07:06:48 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Tue, 13 Jun 2023 07:06:49 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 13 Jun 2023 07:06:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Jun 2023 07:06:49 GMT
EXPOSE 3306 33060
# Tue, 13 Jun 2023 07:06:49 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:759700526b7894aa9c150feb2ebfcd00cf06d2890df739e71555edcfd13669e3`  
		Last Modified: Mon, 12 Jun 2023 23:26:30 GMT  
		Size: 31.4 MB (31417410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe03a6bd2ae95b6630c019ae5bf8e7351c8f27095d7fa0fb9a0deb3a6a56d515`  
		Last Modified: Tue, 13 Jun 2023 07:07:58 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fe98fd0054daa6f38d2c1aaeff6b257d29ba86de74067a273764fb9801b4df9`  
		Last Modified: Tue, 13 Jun 2023 07:07:59 GMT  
		Size: 4.4 MB (4414989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17b46f788fa0e3949eb16f96da627627fef28391e6788017828fdc59d85e1e47`  
		Last Modified: Tue, 13 Jun 2023 07:07:57 GMT  
		Size: 1.5 MB (1471490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a574d9be7097a3158569d7be3fe8f58245d2a1160a02322df42cc21ed4da6305`  
		Last Modified: Tue, 13 Jun 2023 07:07:57 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c32a1a43aaf90ecca1eaecc5cbdade060ae64eb3ad5c0164d3f7fdfa6df36c22`  
		Last Modified: Tue, 13 Jun 2023 07:07:59 GMT  
		Size: 12.7 MB (12662026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1168cde172f4894d8388f45337512f3c50e31b0052297b85690542a846df34f6`  
		Last Modified: Tue, 13 Jun 2023 07:07:57 GMT  
		Size: 2.5 KB (2548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7db9de6fbb6e12066dfb465bb744c8874637465cb32df5af3b7bdc1853d1f07e`  
		Last Modified: Tue, 13 Jun 2023 07:07:55 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7597d1f876243f8e8f404c3f283ef6cbbdba1f7a9e6dd0382d87b0c52a1c7286`  
		Last Modified: Tue, 13 Jun 2023 07:08:13 GMT  
		Size: 129.7 MB (129739199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c90525318623af863af49636e05796881027a61b6c6f6f673755105a58f6e1ff`  
		Last Modified: Tue, 13 Jun 2023 07:07:55 GMT  
		Size: 845.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:569dbc33ff4adc1218e4182f4ef79c728b2ece52f04ab884388496922b9c38f5`  
		Last Modified: Tue, 13 Jun 2023 07:07:55 GMT  
		Size: 5.4 KB (5388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:765dd48ed85e84d520ae837a9e4fa93353bff6066721a0b41e484f1baeaa4194`  
		Last Modified: Tue, 13 Jun 2023 07:07:55 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
