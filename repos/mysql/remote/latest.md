## `mysql:latest`

```console
$ docker pull mysql@sha256:5d1d733f32c28d47061e9d5c2b1fb49b4628c4432901632a70019ec950eda491
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mysql:latest` - linux; amd64

```console
$ docker pull mysql@sha256:d5ba356f580dce71bebfc9fb0cd29b446cfb3aedff699fa9a1e34c2ffc88dd13
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **159.3 MB (159284777 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:26d0ac143221341c36402a139826e938d2ea6f2e458005a71699975c84e96ade`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 12 Mar 2021 02:20:40 GMT
ADD file:3c32f1cd03198e141dd233a7ffd13444157d4150ad917d548f3ee9bf5953ce22 in / 
# Fri, 12 Mar 2021 02:20:41 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 11:18:35 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 12 Mar 2021 11:18:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 11:18:45 GMT
ENV GOSU_VERSION=1.12
# Fri, 12 Mar 2021 11:19:01 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 12 Mar 2021 11:19:02 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 12 Mar 2021 11:19:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		pwgen 		openssl 		perl 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 11:19:15 GMT
RUN set -ex; 	key='A4A9406876FCBD3C456770C88C718D3B5072E1F5'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list > /dev/null
# Fri, 12 Mar 2021 11:19:16 GMT
ENV MYSQL_MAJOR=8.0
# Fri, 12 Mar 2021 11:19:16 GMT
ENV MYSQL_VERSION=8.0.23-1debian10
# Fri, 12 Mar 2021 11:19:18 GMT
RUN echo 'deb http://repo.mysql.com/apt/debian/ buster mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Fri, 12 Mar 2021 11:19:41 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Fri, 12 Mar 2021 11:19:42 GMT
VOLUME [/var/lib/mysql]
# Fri, 12 Mar 2021 11:19:42 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Fri, 19 Mar 2021 17:20:33 GMT
COPY file:2c6221a2517649db2e9dd27098cc9ae1bdaff205f8d6f0299b20a41b86084d77 in /usr/local/bin/ 
# Fri, 19 Mar 2021 17:20:34 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 19 Mar 2021 17:20:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 19 Mar 2021 17:20:34 GMT
EXPOSE 3306 33060
# Fri, 19 Mar 2021 17:20:34 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:6f28985ad1843afd6fd4fe0b42a30bfab63c27d302362e7341e3316e8ba25ced`  
		Last Modified: Fri, 12 Mar 2021 02:26:11 GMT  
		Size: 27.1 MB (27101001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7cd18945cf60a3c6a78b9c4bfa556f8102fc69dbabd02c73442456e41f21c4a`  
		Last Modified: Fri, 12 Mar 2021 11:22:31 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee91068b931316c5a1dc661e51dbb43e9701e0a540a6097f0dcd88b346ea1d9f`  
		Last Modified: Fri, 12 Mar 2021 11:22:33 GMT  
		Size: 4.2 MB (4179167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4efa1a4f93bfb6b664d8b2038fcbe5f97a5bf33e68d524aeb307be7a8f6ed59`  
		Last Modified: Fri, 12 Mar 2021 11:22:29 GMT  
		Size: 1.4 MB (1419384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f220edfa5893f04a8e21d9d0e546b88b64a31cf99d3668dfb8421a8f2071c84e`  
		Last Modified: Fri, 12 Mar 2021 11:22:28 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74a27d3460f8bb426b613d1251422cc9767b0819dd26b77c55ee997bf25e44c9`  
		Last Modified: Fri, 12 Mar 2021 11:22:35 GMT  
		Size: 13.4 MB (13447253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e11e23b75427419602a05481e4d0e9e73062e9cabe942e38d1a3b4de47d29ce`  
		Last Modified: Fri, 12 Mar 2021 11:22:29 GMT  
		Size: 2.4 KB (2395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbce32c99761cb062cf7038b113761c6dcbc21547c30b19579ec369b13a733de`  
		Last Modified: Fri, 12 Mar 2021 11:22:26 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08545fb3966fb7696a72260f0fcf9bf71f106050f391d72679ca18a5c6badd56`  
		Last Modified: Fri, 12 Mar 2021 11:22:54 GMT  
		Size: 113.1 MB (113126986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b9c076841dcf52a412440d8ab44431372735edafb0f4b44bffb716b248016ab`  
		Last Modified: Fri, 12 Mar 2021 11:22:26 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef8b369352ae528672fd3c53de6054268aee4b4a9b0b34ba08ed79c4b4326d42`  
		Last Modified: Fri, 19 Mar 2021 17:21:06 GMT  
		Size: 5.5 KB (5519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebd210f0917d0f2635be71c1f9dba8dfc4c5325e159c32ff1206aab9f0c2d9a4`  
		Last Modified: Fri, 19 Mar 2021 17:21:06 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
