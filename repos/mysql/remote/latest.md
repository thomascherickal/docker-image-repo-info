## `mysql:latest`

```console
$ docker pull mysql@sha256:d0507b008897c39f6cbc76285af1171d4551988475e00e91344060023cd9c553
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:latest` - linux; amd64

```console
$ docker pull mysql@sha256:d256fd79a3d25784996b2d6a188a6bd83e3b3b32fa554366f033d1354dfc5c00
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.0 MB (153984058 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b4c624c7fe1acde563bdc41b5479d8e7bb1433dd4b259fca90c1a3d92aeb9a7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 21 Dec 2021 01:23:04 GMT
ADD file:bd5c9e0e0145fe33beee9d73615cc89b5c5459bb84ea164cb1bbd8c999f0c2e4 in / 
# Tue, 21 Dec 2021 01:23:04 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:55:02 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 21 Dec 2021 02:55:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Thu, 20 Jan 2022 04:32:57 GMT
ENV GOSU_VERSION=1.14
# Thu, 20 Jan 2022 04:33:08 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 20 Jan 2022 04:33:09 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 20 Jan 2022 04:33:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		pwgen 		openssl 		perl 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Thu, 20 Jan 2022 04:33:27 GMT
RUN set -ex; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list > /dev/null
# Thu, 20 Jan 2022 04:33:27 GMT
ENV MYSQL_MAJOR=8.0
# Thu, 20 Jan 2022 04:33:27 GMT
ENV MYSQL_VERSION=8.0.28-1debian10
# Thu, 20 Jan 2022 04:33:28 GMT
RUN echo 'deb http://repo.mysql.com/apt/debian/ buster mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Thu, 20 Jan 2022 04:33:44 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Thu, 20 Jan 2022 04:33:45 GMT
VOLUME [/var/lib/mysql]
# Thu, 20 Jan 2022 04:33:45 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Thu, 20 Jan 2022 04:33:45 GMT
COPY file:c112ec3a02a7b818421f8613e69e548ad2ee644304066708204abb684d77664a in /usr/local/bin/ 
# Thu, 20 Jan 2022 04:33:46 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 20 Jan 2022 04:33:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 20 Jan 2022 04:33:46 GMT
EXPOSE 3306 33060
# Thu, 20 Jan 2022 04:33:46 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:72a69066d2febc34d8f3dbcb645f7b851a57e9681322ece7ad8007503b783c19`  
		Last Modified: Tue, 21 Dec 2021 01:28:32 GMT  
		Size: 27.2 MB (27153723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93619dbc5b36fe839e30a055a373bb628be3c22109abcb483cc56c8dd5f8cf47`  
		Last Modified: Tue, 21 Dec 2021 02:58:24 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99da31dd61422c9b6ce417b189ebaf568e6cfa7a5343f7db4ad7c2ae2127a238`  
		Last Modified: Tue, 21 Dec 2021 02:58:25 GMT  
		Size: 4.2 MB (4179263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5c707858ec02a0d102d6306913ed8ad74365dc284cb513fbff51879d7783f5d`  
		Last Modified: Thu, 20 Jan 2022 04:34:35 GMT  
		Size: 1.4 MB (1386720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc41578cbf60e53a23966a1bd9fee191e68ac08563fdfc9c9a6c9725d56af582`  
		Last Modified: Thu, 20 Jan 2022 04:34:34 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4785d896ef103951a64f67d0e91b7b43fdae6919bd8f7846c75ccc962f2f1f68`  
		Last Modified: Thu, 20 Jan 2022 04:34:38 GMT  
		Size: 13.4 MB (13448671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d250cdc93be0b7d74514ff98186bcf28d622b80023b3d55e6fcaf4071da20c3`  
		Last Modified: Thu, 20 Jan 2022 04:34:34 GMT  
		Size: 2.5 KB (2534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:309700f4198397acc0e961b62a62b9e50b44d65920c5a4579fc71b5a1867ef6f`  
		Last Modified: Thu, 20 Jan 2022 04:34:32 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45fd33301836fd93b35c08f60f90d4d5b9c50734c767cab500f901e18b17a3d5`  
		Last Modified: Thu, 20 Jan 2022 04:34:49 GMT  
		Size: 107.8 MB (107804978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92f970c68b71c579a97aca2b3dd47e6d9f79a1a7ea72c1a75277afa201f93079`  
		Last Modified: Thu, 20 Jan 2022 04:34:32 GMT  
		Size: 845.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb3544339a9e02b647179786399d1a65f445e93c57622e1fba60953ab539e3d0`  
		Last Modified: Thu, 20 Jan 2022 04:34:32 GMT  
		Size: 5.1 KB (5097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f66ddf4c43fa729d20b71510a0b192032858839cf98e79557838de2942a4d08f`  
		Last Modified: Thu, 20 Jan 2022 04:34:32 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
