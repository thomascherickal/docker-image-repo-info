## `mysql:debian`

```console
$ docker pull mysql@sha256:6d49fc540dac15528491aed83c7127b0c5874e87b5c81d0e89437d9aca413e75
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:debian` - linux; amd64

```console
$ docker pull mysql@sha256:7f9819035b5bfa7cabfca5ccc0d49542bd4635af204c6d354752fb62c3aa8f76
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **157.9 MB (157850867 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be9f4e078ca4997f3bf63e26e4bfa0802c5b83ce8298fb03b56770642e123482`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 23 Aug 2022 00:20:50 GMT
ADD file:7726efb0e0eb5003dbcf2967ec29364479eec8b41f2569ff189372153115b54b in / 
# Tue, 23 Aug 2022 00:20:51 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 03:38:21 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 23 Aug 2022 03:38:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 03:38:26 GMT
ENV GOSU_VERSION=1.14
# Tue, 23 Aug 2022 03:38:35 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 23 Aug 2022 03:38:36 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 23 Aug 2022 03:38:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 03:38:42 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Tue, 23 Aug 2022 03:38:42 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 23 Aug 2022 03:38:42 GMT
ENV MYSQL_VERSION=8.0.30-1debian11
# Tue, 23 Aug 2022 03:38:43 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ bullseye mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Tue, 23 Aug 2022 03:38:56 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 23 Aug 2022 03:38:57 GMT
VOLUME [/var/lib/mysql]
# Tue, 23 Aug 2022 03:38:57 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Wed, 24 Aug 2022 23:03:17 GMT
COPY file:5e84598933ec95c9918378d8dde5be8d5f80b0e1fc321a029f840f313201ebce in /usr/local/bin/ 
# Wed, 24 Aug 2022 23:03:17 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 24 Aug 2022 23:03:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 24 Aug 2022 23:03:17 GMT
EXPOSE 3306 33060
# Wed, 24 Aug 2022 23:03:17 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:7a6db449b51b92eac5c81cdbd82917785343f1664b2be57b22337b0a40c5b29d`  
		Last Modified: Tue, 23 Aug 2022 00:24:59 GMT  
		Size: 31.4 MB (31381485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63b23008bc872644b3493308929a67cefe09bcc825a15028af9b65d2b86b8154`  
		Last Modified: Tue, 23 Aug 2022 03:40:21 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82fdf48499dbc8cadd345c9a461bee300ec7f328fd970ea456ad13582f974b22`  
		Last Modified: Tue, 23 Aug 2022 03:40:22 GMT  
		Size: 4.4 MB (4414801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c75d7f84228a2f19e49b9a70c960e1b9fe6eceb637a24727ed6ec6c574b584d`  
		Last Modified: Tue, 23 Aug 2022 03:40:19 GMT  
		Size: 1.4 MB (1418466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61089f488e727e34e9b1c515a769ea0f63e4178b9f1f8a4b697f8345cd6a2fab`  
		Last Modified: Tue, 23 Aug 2022 03:40:19 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c82b0badc95c597bc8fa0c39ee975457037cb54ecafb310b75368ebaf1ea1c8`  
		Last Modified: Tue, 23 Aug 2022 03:40:21 GMT  
		Size: 12.7 MB (12661891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:245253769f71d25434c6c23a35770f5a993727fa9396802f45d5c41bf69ef18f`  
		Last Modified: Tue, 23 Aug 2022 03:40:19 GMT  
		Size: 2.5 KB (2549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7459b3c285350cb2e864e202e4a6ce674fe99d2338698d8aba402dca9be2a3f`  
		Last Modified: Tue, 23 Aug 2022 03:40:16 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e669258b3f94cee1da8b0e384ee0e8461fcaadff509b2929f9c2b45e684d674`  
		Last Modified: Tue, 23 Aug 2022 03:40:33 GMT  
		Size: 108.0 MB (107963194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7db97a7c2c85d65c31c5ecfaf632608190d8bd998f012fa7e7888fb4b9bd562`  
		Last Modified: Tue, 23 Aug 2022 03:40:16 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e8bfbb8075a7ee12fbb23a5666748e5aa6572bb00d4e501791376b3073dd85c`  
		Last Modified: Wed, 24 Aug 2022 23:05:29 GMT  
		Size: 5.4 KB (5381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8947074e030f3c5598671716911f7110c5aa82c49630824924d6dddcace90b14`  
		Last Modified: Wed, 24 Aug 2022 23:05:29 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
