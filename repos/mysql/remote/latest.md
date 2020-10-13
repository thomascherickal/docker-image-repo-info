## `mysql:latest`

```console
$ docker pull mysql@sha256:86b7c83e24c824163927db1016d5ab153a9a04358951be8b236171286e3289a4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mysql:latest` - linux; amd64

```console
$ docker pull mysql@sha256:77b7e09c906615c1bb59b2e9d7703f728b1186a5a70e547ce2f1079ef4c1c5ca
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **158.6 MB (158633522 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e85dd5c32558ea5c22cc4786cff512c1940270a50e7dbc21ad2df42f0637de4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 13 Oct 2020 01:39:05 GMT
ADD file:0dc53e7886c35bc21ae6c4f6cedda54d56ae9c9e9cd367678f1a72e68b3c43d4 in / 
# Tue, 13 Oct 2020 01:39:05 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 08:01:49 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 13 Oct 2020 08:01:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 08:01:59 GMT
ENV GOSU_VERSION=1.12
# Tue, 13 Oct 2020 08:02:13 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Oct 2020 08:02:14 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 13 Oct 2020 08:02:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		pwgen 		openssl 		perl 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 08:02:28 GMT
RUN set -ex; 	key='A4A9406876FCBD3C456770C88C718D3B5072E1F5'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list > /dev/null
# Tue, 13 Oct 2020 08:02:29 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 13 Oct 2020 08:02:29 GMT
ENV MYSQL_VERSION=8.0.21-1debian10
# Tue, 13 Oct 2020 08:02:30 GMT
RUN echo "deb http://repo.mysql.com/apt/debian/ buster mysql-${MYSQL_MAJOR}" > /etc/apt/sources.list.d/mysql.list
# Tue, 13 Oct 2020 08:02:57 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update && apt-get install -y mysql-community-client="${MYSQL_VERSION}" mysql-community-server-core="${MYSQL_VERSION}" && rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 13 Oct 2020 08:02:57 GMT
VOLUME [/var/lib/mysql]
# Tue, 13 Oct 2020 08:02:58 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Tue, 13 Oct 2020 08:02:58 GMT
COPY file:7cbb26bbdb8e71b36aafda38dbac08caa641714a19991b86cde77daf3286ec11 in /usr/local/bin/ 
# Tue, 13 Oct 2020 08:03:00 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 13 Oct 2020 08:03:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Oct 2020 08:03:00 GMT
EXPOSE 3306 33060
# Tue, 13 Oct 2020 08:03:01 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:bb79b6b2107fea8e8a47133a660b78e3a546998fcf0427be39ac9a0af4a97e90`  
		Last Modified: Tue, 13 Oct 2020 01:48:17 GMT  
		Size: 27.1 MB (27092228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49e22f6fb9f7713028f8ed9b0beaa2ebac38d73ff6fd60532031e4a257f314c0`  
		Last Modified: Tue, 13 Oct 2020 08:05:18 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:842b1255668c99365efe9cf8367baf458ad590033cfbe73c03e67a961d34a288`  
		Last Modified: Tue, 13 Oct 2020 08:05:18 GMT  
		Size: 4.2 MB (4178100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f48d1f430002d35f5766b2ba9cfbe0c624a705a542622a94e5b86e2132aba7b`  
		Last Modified: Tue, 13 Oct 2020 08:05:17 GMT  
		Size: 1.4 MB (1419213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c693f0615bcee7154070df04d6cce10562437d69ee98d469252e950cd79e0d7f`  
		Last Modified: Tue, 13 Oct 2020 08:05:17 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a621b9dbed2309be1806a0a750a6deef7c2558f25ceee4fcfc06ec421fad097`  
		Last Modified: Tue, 13 Oct 2020 08:05:21 GMT  
		Size: 13.4 MB (13447145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0807d32aef130f157419493647a5b252b6560b5385f14f102f388e576aeb1e98`  
		Last Modified: Tue, 13 Oct 2020 08:05:17 GMT  
		Size: 2.4 KB (2395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9eb4355ba4508252590eb497a480a1d154529cff1ccdada2c60e628aaa73dc18`  
		Last Modified: Tue, 13 Oct 2020 08:05:16 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6879faad3b6c70e300c1ad96cf752b85e4a54ade54b8e4d370600a57e617c439`  
		Last Modified: Tue, 13 Oct 2020 08:05:39 GMT  
		Size: 112.5 MB (112486256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:164ef92f3887884a8e93d96f0a4cdfe88912f0dc4a257b857c1aa63c7ee5e00f`  
		Last Modified: Tue, 13 Oct 2020 08:05:16 GMT  
		Size: 843.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e4a6e666228dc751782155f2b3af56ed7c5e9ba56ef35c36f03587b6242065d`  
		Last Modified: Tue, 13 Oct 2020 08:05:16 GMT  
		Size: 5.1 KB (5145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d45dea7731adeb126e6275444517123fc75f817c1949722f608d1eedef8ce475`  
		Last Modified: Tue, 13 Oct 2020 08:05:16 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
