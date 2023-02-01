## `mysql:5-debian`

```console
$ docker pull mysql@sha256:1a74dd3703a9e08a4f86f2f3ca0fc5c583ed70d14ce51c0810214a49a9356728
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5-debian` - linux; amd64

```console
$ docker pull mysql@sha256:ceeb9aae2f08123530c07c9892ee07fef679cd385dc12de67945100c327c9d2c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **162.7 MB (162697097 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cdc0da91e4b1905ceb995dd7a40aedb53ff2a547121bebcfc9958a0963e7401c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 11 Jan 2023 02:35:07 GMT
ADD file:67ceb946e54c26c505b5f9f393d77befbd5e9b3b5c069ca301e314ecc74456b0 in / 
# Wed, 11 Jan 2023 02:35:07 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 06:20:12 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 11 Jan 2023 06:20:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 04:25:01 GMT
ENV GOSU_VERSION=1.16
# Wed, 01 Feb 2023 04:25:13 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 01 Feb 2023 04:25:13 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 01 Feb 2023 04:25:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 04:25:23 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Wed, 01 Feb 2023 04:25:23 GMT
ENV MYSQL_MAJOR=5.7
# Wed, 01 Feb 2023 04:25:23 GMT
ENV MYSQL_VERSION=5.7.41-1debian10
# Wed, 01 Feb 2023 04:25:24 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-5.7' > /etc/apt/sources.list.d/mysql.list
# Wed, 01 Feb 2023 04:25:42 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-server="${MYSQL_VERSION}" 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Wed, 01 Feb 2023 04:25:43 GMT
VOLUME [/var/lib/mysql]
# Wed, 01 Feb 2023 04:25:43 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 01 Feb 2023 04:25:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 01 Feb 2023 04:25:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Feb 2023 04:25:44 GMT
EXPOSE 3306 33060
# Wed, 01 Feb 2023 04:25:44 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:548fcab5fe888f589dd092c68b813bfd65359878bd1950d6b753f749e82ebd7c`  
		Last Modified: Wed, 11 Jan 2023 02:39:48 GMT  
		Size: 27.1 MB (27140352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:702e45a0d0fab46740d0cf404969001dc0537dd564973fa6f31da2a00cfe5ef8`  
		Last Modified: Wed, 11 Jan 2023 06:22:03 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad96d17a23a7cff619709675f8981274e6a4ff7a9fb99590f0a837511e69a50b`  
		Last Modified: Wed, 11 Jan 2023 06:22:03 GMT  
		Size: 4.2 MB (4182274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce23bd8e19cbf46dca11c58364da8cae841721eb6ec6e59b5b64366b92b71c60`  
		Last Modified: Wed, 01 Feb 2023 04:27:43 GMT  
		Size: 1.4 MB (1441737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75f410a04b48d8f13ee66006c76284a85219773b56a7a3917c7278e76910d15b`  
		Last Modified: Wed, 01 Feb 2023 04:27:43 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d9d2a4035b33745414d5b00e226fd586f1b79b41c922746a2950ec302854714`  
		Last Modified: Wed, 01 Feb 2023 04:27:45 GMT  
		Size: 14.1 MB (14089526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d914f26e38d92043c13c7ac16c4034ee50d83195ac73832cde6ba5cb7c74dd7`  
		Last Modified: Wed, 01 Feb 2023 04:27:41 GMT  
		Size: 2.5 KB (2548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b578ab58d644b756e0807fcff7ca7d3875dd58ce88ae3f3ec826285f18df1e1a`  
		Last Modified: Wed, 01 Feb 2023 04:27:41 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6e9911a3a0f7bf66493311483809b24e311912328abd044d7374e0a1c7005d3`  
		Last Modified: Wed, 01 Feb 2023 04:27:56 GMT  
		Size: 115.8 MB (115833016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b5516c1cc32a00e699d90cbafb5aec186382a49ff7862ad1c077ec3623beb1c`  
		Last Modified: Wed, 01 Feb 2023 04:27:41 GMT  
		Size: 5.4 KB (5392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcb4433c89ce7ae2f55ea90016bc0c183373fbbb78ab19257b0b753e8cdca160`  
		Last Modified: Wed, 01 Feb 2023 04:27:41 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
