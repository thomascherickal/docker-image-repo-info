## `mysql:5-debian`

```console
$ docker pull mysql@sha256:16e159331007eccc069822f7b731272043ed572a79a196a05ffa2ea127caaf67
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5-debian` - linux; amd64

```console
$ docker pull mysql@sha256:368c1258fb7330eece5a0fbe2c9801d666bb0f26d7a82c78c431fbcb8f5fd191
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **162.5 MB (162456671 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3d35804fa376a141b9a9dad8f5534c3179f4c328d6efc67c5c5145d257c291a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 11 May 2022 01:20:37 GMT
ADD file:76b454ddb7dfe4d22afae844a7e67e7e5fb4570dae2e21bbd259a1f2e5839f33 in / 
# Wed, 11 May 2022 01:20:37 GMT
CMD ["bash"]
# Wed, 11 May 2022 05:01:23 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 11 May 2022 05:01:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 05:01:29 GMT
ENV GOSU_VERSION=1.14
# Wed, 11 May 2022 05:01:38 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 11 May 2022 05:01:39 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 11 May 2022 05:01:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 05:01:46 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Wed, 11 May 2022 05:02:12 GMT
ENV MYSQL_MAJOR=5.7
# Wed, 11 May 2022 05:02:12 GMT
ENV MYSQL_VERSION=5.7.38-1debian10
# Wed, 11 May 2022 05:02:13 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-5.7' > /etc/apt/sources.list.d/mysql.list
# Wed, 11 May 2022 05:02:31 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-server="${MYSQL_VERSION}" 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Wed, 11 May 2022 05:02:32 GMT
VOLUME [/var/lib/mysql]
# Wed, 11 May 2022 05:02:32 GMT
COPY file:e9a583a365264f0f565259ffd0f19e5199ef4351d098f75af32f633c0d6cbe73 in /usr/local/bin/ 
# Wed, 11 May 2022 05:02:32 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 11 May 2022 05:02:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 05:02:32 GMT
EXPOSE 3306 33060
# Wed, 11 May 2022 05:02:33 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:c32ce6654453d35d0b3dde45d195adeee586ffba0a683006ee06748c077c01fa`  
		Last Modified: Wed, 11 May 2022 01:25:58 GMT  
		Size: 27.1 MB (27140722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:415d08ee031ab3bffe8c0db6b82f2cde88049eda62a50801eb6d8aa68bb0e12c`  
		Last Modified: Wed, 11 May 2022 05:03:03 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a38fec2542ffcfa6247f2992d1ec422b38e00ed5ca998bc5b890ca1a97ab1d5`  
		Last Modified: Wed, 11 May 2022 05:03:04 GMT  
		Size: 4.2 MB (4179283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:352881ee8fe9b63edbd90eb3a1ffa035c72b7edfbcad6fda55db516c2a2b2cb9`  
		Last Modified: Wed, 11 May 2022 05:03:02 GMT  
		Size: 1.4 MB (1386677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8e20da291b6c92de4aa28a02fe8845045ec68d9b9ad1497e921fa42e8303650`  
		Last Modified: Wed, 11 May 2022 05:03:01 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66c2a8cc1999eedaa968d140339f25947e1faf8b3f2084c7eb5eee68455d6295`  
		Last Modified: Wed, 11 May 2022 05:03:03 GMT  
		Size: 14.1 MB (14064393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3a3a8e49878cc1f98a4927704e4fdc191bcc2cc80fbf7470b36fe1b44b7596d`  
		Last Modified: Wed, 11 May 2022 05:03:01 GMT  
		Size: 2.5 KB (2548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:172aabfba65cfce5cfcc754b562da5a55e6328ca9c02b005fdf40d07b0e6cfcd`  
		Last Modified: Wed, 11 May 2022 05:03:45 GMT  
		Size: 254.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fea17d0b1d1ec95b127efcb443db4ffe3c6bbc890efa5754602b9d49691a567d`  
		Last Modified: Wed, 11 May 2022 05:04:00 GMT  
		Size: 115.7 MB (115675657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fff7f5411ca9049d62e30c6a523c27a914994bcb1750bcef101daf61db3f42c4`  
		Last Modified: Wed, 11 May 2022 05:03:45 GMT  
		Size: 5.1 KB (5135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c33d43428e07b9c9c4d69f30ad3287c01be6f5938dca2821207281bd6927d026`  
		Last Modified: Wed, 11 May 2022 05:03:45 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
