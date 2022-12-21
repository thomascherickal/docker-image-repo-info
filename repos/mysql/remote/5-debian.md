## `mysql:5-debian`

```console
$ docker pull mysql@sha256:c134741fc67355f1f57939624ff3e117bc0a2b0e6566fca60f85bce847a04ace
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5-debian` - linux; amd64

```console
$ docker pull mysql@sha256:c7f71d444e2a3434aede4594672722dd2e2f4e886882f5133cb2b7ee23d0e5a7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **162.6 MB (162596962 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94165850af50f5fc2c2cdf49a5c0d6e71d1408c3817eae97a681ae86b15fab19`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 21 Dec 2022 01:20:52 GMT
ADD file:660e0093a3da49e4ca41260d09d585754ccb1eff8974c4b0dd4456b76ddbbc9a in / 
# Wed, 21 Dec 2022 01:20:52 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 11:32:39 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 21 Dec 2022 11:32:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 11:32:45 GMT
ENV GOSU_VERSION=1.14
# Wed, 21 Dec 2022 11:32:54 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 21 Dec 2022 11:32:54 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 21 Dec 2022 11:33:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 11:33:02 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Wed, 21 Dec 2022 11:33:02 GMT
ENV MYSQL_MAJOR=5.7
# Wed, 21 Dec 2022 11:33:02 GMT
ENV MYSQL_VERSION=5.7.40-1debian10
# Wed, 21 Dec 2022 11:33:03 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-5.7' > /etc/apt/sources.list.d/mysql.list
# Wed, 21 Dec 2022 11:33:22 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-server="${MYSQL_VERSION}" 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Wed, 21 Dec 2022 11:33:23 GMT
VOLUME [/var/lib/mysql]
# Wed, 21 Dec 2022 11:33:23 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 21 Dec 2022 11:33:23 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 21 Dec 2022 11:33:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Dec 2022 11:33:24 GMT
EXPOSE 3306 33060
# Wed, 21 Dec 2022 11:33:24 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:b52ebda398ed2c4602ea06056f78d45a59474ee4e2a020967251ba082424e7e2`  
		Last Modified: Wed, 21 Dec 2022 01:25:17 GMT  
		Size: 27.1 MB (27140331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ce9a79d5155fd4711289385da53044c809d4e3c678327ca6d45fb6a9f4cf987`  
		Last Modified: Wed, 21 Dec 2022 11:34:31 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e261668310f535cff440b65def4e46639ea51e56eb7e29f3dcd0d2bc789dc16`  
		Last Modified: Wed, 21 Dec 2022 11:34:30 GMT  
		Size: 4.2 MB (4182322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3123e9b617f90c63e401b61f20202da262ba291624f9cf582382b6606266d4f`  
		Last Modified: Wed, 21 Dec 2022 11:34:30 GMT  
		Size: 1.4 MB (1388870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f0c53d4059e024752565a418a176ee322c7975e3573daac8543596533034c0d`  
		Last Modified: Wed, 21 Dec 2022 11:34:29 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a769258f8c5aae1218e004f37090ebf203889beee192d48cef2bc63238e41bdb`  
		Last Modified: Wed, 21 Dec 2022 11:34:32 GMT  
		Size: 14.1 MB (14089454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6478aa5af16e1946961ac5a640d2dd50637ef7f6f5a19546baf2add23b9f0930`  
		Last Modified: Wed, 21 Dec 2022 11:34:27 GMT  
		Size: 2.5 KB (2545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86a4405a4c9e0921b9c4f114716117465cab4932d55dd832a73ef363f18e4f75`  
		Last Modified: Wed, 21 Dec 2022 11:34:27 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eae9863c382483c9a8a0bc99c315132f7b91a2abdd9c8e6c4854e15a5f8770b2`  
		Last Modified: Wed, 21 Dec 2022 11:34:43 GMT  
		Size: 115.8 MB (115785799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a741ea6ad10a9767f461430b7c34fbe4cd65ce41bcd26837e7a0a32d5144aae4`  
		Last Modified: Wed, 21 Dec 2022 11:34:27 GMT  
		Size: 5.4 KB (5389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62548f9fac91770f96cdf945c008bf822f27efacd5d895c9643be71f8555485a`  
		Last Modified: Wed, 21 Dec 2022 11:34:27 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
