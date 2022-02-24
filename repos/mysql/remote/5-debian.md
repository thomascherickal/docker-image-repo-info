## `mysql:5-debian`

```console
$ docker pull mysql@sha256:ea24ddf1116d6e5053919748d2c27c8200e39ac0dbe9540f213a2d9141b66167
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5-debian` - linux; amd64

```console
$ docker pull mysql@sha256:5adbbb05d43e67a7ed5f4856d3831b22ece5178d23c565b31cef61f92e3467ea
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.8 MB (154804997 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:538ec2c8721c073370299bf83ae46b940c83899f44cc90d89799a046afc5816b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:59 GMT
ADD file:c51141702f568a28a7e3e7a2748f5ead5754e32d7b1cf7ebc8f4326273d05206 in / 
# Wed, 26 Jan 2022 01:40:59 GMT
CMD ["bash"]
# Thu, 27 Jan 2022 00:56:31 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Thu, 27 Jan 2022 00:56:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Thu, 27 Jan 2022 00:56:43 GMT
ENV GOSU_VERSION=1.14
# Thu, 27 Jan 2022 00:57:05 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 27 Jan 2022 00:57:07 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 23 Feb 2022 22:25:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		openssl 		perl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Feb 2022 22:25:52 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Wed, 23 Feb 2022 22:27:54 GMT
ENV MYSQL_MAJOR=5.7
# Wed, 23 Feb 2022 22:27:54 GMT
ENV MYSQL_VERSION=5.7.37-1debian10
# Wed, 23 Feb 2022 22:27:55 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-5.7' > /etc/apt/sources.list.d/mysql.list
# Wed, 23 Feb 2022 22:28:14 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-server="${MYSQL_VERSION}" 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Wed, 23 Feb 2022 22:28:15 GMT
VOLUME [/var/lib/mysql]
# Wed, 23 Feb 2022 22:28:15 GMT
COPY file:baf57873956bd59e060e26b6c80f401272ee89005e3d62d008bf3de68c4c7545 in /usr/local/bin/ 
# Wed, 23 Feb 2022 22:28:16 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 23 Feb 2022 22:28:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Feb 2022 22:28:16 GMT
EXPOSE 3306 33060
# Wed, 23 Feb 2022 22:28:17 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:6552179c3509e3c4314b4065e0d2790563d01cd474e2fdd58be4d46acd48af6a`  
		Last Modified: Wed, 26 Jan 2022 01:47:31 GMT  
		Size: 27.2 MB (27153731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d69aa66e4482016fae7907ce17f46b3f7588c5ee17cc5c7dff11324e05c92bd5`  
		Last Modified: Thu, 27 Jan 2022 00:59:07 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b19465b002b6638a15647e41bd6bff7d4cabc190c35b5a50025e0c4370a2794`  
		Last Modified: Thu, 27 Jan 2022 00:59:08 GMT  
		Size: 4.2 MB (4179346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b0d0cfe99a1632d64b2986e131d8dd95ddb8b8bef124c690ab1958c961b8d20`  
		Last Modified: Thu, 27 Jan 2022 00:59:05 GMT  
		Size: 1.4 MB (1386744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ccd5a5c898747a41e6e4498e0c4a9c034ee1fb06c94f48e580de8521f668670`  
		Last Modified: Thu, 27 Jan 2022 00:59:04 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44f5f7765d10dffc8825a89c30cddc2c753bde7435445ff55a5baaff1fe97654`  
		Last Modified: Wed, 23 Feb 2022 22:29:13 GMT  
		Size: 13.4 MB (13438692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e8f1dd5efbe2ac5e563ea686d55f58b8dcedf32c1434304652c549fdf299c88`  
		Last Modified: Wed, 23 Feb 2022 22:29:10 GMT  
		Size: 2.5 KB (2549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab45b9a309e746ae5e6074efb8d35490146b3188f1375fd6abe60763a4b13b79`  
		Last Modified: Wed, 23 Feb 2022 22:30:15 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90242da46c5709e3df233b61e042de5002a59567de7c18a68c75935d386195d9`  
		Last Modified: Wed, 23 Feb 2022 22:30:30 GMT  
		Size: 108.6 MB (108636729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a8d822d1293bf6661e4e6c69c425a5e9fca7b43bbf1201c1c66effbebd275d4`  
		Last Modified: Wed, 23 Feb 2022 22:30:15 GMT  
		Size: 5.0 KB (4954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1704bf9fa7759625eeda74bcf484357dd06e4ef8d46319f09b59d4fd4c154eab`  
		Last Modified: Wed, 23 Feb 2022 22:30:15 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
