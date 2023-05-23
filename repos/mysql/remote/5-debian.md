## `mysql:5-debian`

```console
$ docker pull mysql@sha256:11aea01c02f457f6c67e2037caa5e004e015ee94293aac224c0beb13459ee9db
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5-debian` - linux; amd64

```console
$ docker pull mysql@sha256:26504dc8b79b5b0bf60d9e7e043b7a2b1a9895b390382cf7ceab3792d8aa2e34
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **162.8 MB (162758554 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f270218b50ff2e08bc03cde8f0ba99dfef35758ef84f3c93e9c64d25b027be5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 23 May 2023 01:20:37 GMT
ADD file:2058e04b33179527a56999678c1c62dfcf76944675afcd77b5163141fb025f8c in / 
# Tue, 23 May 2023 01:20:37 GMT
CMD ["bash"]
# Tue, 23 May 2023 04:16:31 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 23 May 2023 04:16:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg && rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 04:16:37 GMT
ENV GOSU_VERSION=1.16
# Tue, 23 May 2023 04:16:45 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 23 May 2023 04:16:45 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 23 May 2023 04:16:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 04:16:52 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Tue, 23 May 2023 04:16:52 GMT
ENV MYSQL_MAJOR=5.7
# Tue, 23 May 2023 04:16:52 GMT
ENV MYSQL_VERSION=5.7.42-1debian10
# Tue, 23 May 2023 04:16:53 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-5.7' > /etc/apt/sources.list.d/mysql.list
# Tue, 23 May 2023 04:17:12 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-server="${MYSQL_VERSION}" 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 23 May 2023 04:17:13 GMT
VOLUME [/var/lib/mysql]
# Tue, 23 May 2023 04:17:13 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Tue, 23 May 2023 04:17:13 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 23 May 2023 04:17:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 May 2023 04:17:14 GMT
EXPOSE 3306 33060
# Tue, 23 May 2023 04:17:14 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:99bf4787315b60d97d860ac6d006b7835b2241a601e93c2da4af6ca554be8704`  
		Last Modified: Tue, 23 May 2023 01:24:47 GMT  
		Size: 27.1 MB (27138577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35ca486d93f7aa513f34a5fadffd81c536ce4ac5de719145803c6829aea16397`  
		Last Modified: Tue, 23 May 2023 04:18:10 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a60f1b29379d4ba9ab2dabb338ac075c86cc37e5fdfcae5ae96dbbd6457cf089`  
		Last Modified: Tue, 23 May 2023 04:18:08 GMT  
		Size: 4.2 MB (4182401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5a7f35f9a601ec927d75159dea2103af466efa76425e85420e4478dd4245c24`  
		Last Modified: Tue, 23 May 2023 04:18:08 GMT  
		Size: 1.4 MB (1441855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1256d8a34742417f317fd61b3b0a979ba9899c2a1fe1a41e0af44e91540db169`  
		Last Modified: Tue, 23 May 2023 04:18:07 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec41b788488c21b7d482ff0f0bfbb022be4e32813795b01d9cecafa83a0be8f9`  
		Last Modified: Tue, 23 May 2023 04:18:10 GMT  
		Size: 14.1 MB (14087083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4314d2e9e62de6d9176830e185d701028a984e0c7553787dbe701721a5e5afdb`  
		Last Modified: Tue, 23 May 2023 04:18:05 GMT  
		Size: 2.5 KB (2548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c051de3bff5e78a684c15f282bcd6df4cf3867917812ac522b6e71d5c8db794b`  
		Last Modified: Tue, 23 May 2023 04:18:05 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d7f78bab28293fb999acd01969a1c1200e3709605dd6b165f2c04dcddc9f413`  
		Last Modified: Tue, 23 May 2023 04:18:20 GMT  
		Size: 115.9 MB (115898446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:011807ab1ea4c4daaa35ce94fb51df9b7e3184e9207f6e8522441d2d2053abc1`  
		Last Modified: Tue, 23 May 2023 04:18:05 GMT  
		Size: 5.4 KB (5391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5146016c0e9ff625ac285f603f05082728c2895cdf869378f6bcfcf5ed9963d`  
		Last Modified: Tue, 23 May 2023 04:18:06 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
