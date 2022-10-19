## `mysql:8-debian`

```console
$ docker pull mysql@sha256:6da07a43b1ca31cb3e7e3d420de6a91682f0b8f4231888eafb11d86a3806d9e1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:8-debian` - linux; amd64

```console
$ docker pull mysql@sha256:e6fb4c622766a92a7f2eda90f5208b863c206511504e77d805971f1944103212
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **177.6 MB (177571480 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56ffa4b21891e5a2ed6c1af823d9981d52d3a6d68dff7cc3d544760fb5815215`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:39 GMT
ADD file:b78b777208be08edd8f297035cdfbacddb45170ad778fd643c792ee045187e39 in / 
# Tue, 04 Oct 2022 23:26:39 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 04:21:45 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 05 Oct 2022 04:21:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 04:21:51 GMT
ENV GOSU_VERSION=1.14
# Wed, 05 Oct 2022 04:22:00 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 05 Oct 2022 04:22:00 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 05 Oct 2022 04:22:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 04:22:07 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Wed, 05 Oct 2022 04:22:07 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 11 Oct 2022 20:29:30 GMT
ENV MYSQL_VERSION=8.0.31-1debian11
# Tue, 11 Oct 2022 20:29:31 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ bullseye mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Tue, 11 Oct 2022 20:29:47 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 11 Oct 2022 20:29:48 GMT
VOLUME [/var/lib/mysql]
# Tue, 11 Oct 2022 20:29:48 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Wed, 19 Oct 2022 19:24:29 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 19 Oct 2022 19:24:30 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 19 Oct 2022 19:24:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 19 Oct 2022 19:24:30 GMT
EXPOSE 3306 33060
# Wed, 19 Oct 2022 19:24:30 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:bd159e379b3b1bc0134341e4ffdeab5f966ec422ae04818bb69ecef08a823b05`  
		Last Modified: Tue, 04 Oct 2022 23:30:54 GMT  
		Size: 31.4 MB (31420102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f498ba1a3ae2dfa82359e0fb959af536134a1360d33dfa87638e409b70b3fa3`  
		Last Modified: Wed, 05 Oct 2022 04:23:52 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c224eff0af51a4254bf410ca8f6cab7044171639fc6e7b29cd55248bb609d02`  
		Last Modified: Wed, 05 Oct 2022 04:23:52 GMT  
		Size: 4.4 MB (4414808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acdd40c1260704addfdb3a21bf71ae5c14567100f98acd4d8dfec303294e1c5f`  
		Last Modified: Wed, 05 Oct 2022 04:23:50 GMT  
		Size: 1.4 MB (1418452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21c3ece0305cbf295220adfdacf8c9e9fdf5de35ea07e505913ea4ee6e1f4f74`  
		Last Modified: Wed, 05 Oct 2022 04:23:49 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a10286651685e256e36f218063406728987d0f36c285adf41d41f8665661b74`  
		Last Modified: Wed, 05 Oct 2022 04:23:52 GMT  
		Size: 12.7 MB (12661783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77a34b42ee331888b70b38f6c96cacce54fe2bb4cf6e2ccefdd7add2144d5a3e`  
		Last Modified: Wed, 05 Oct 2022 04:23:49 GMT  
		Size: 2.5 KB (2546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e5d04bddbd0c7caeacce07fffaa07f1b523fe80e9415cc5c88fe8387468c2ec`  
		Last Modified: Tue, 11 Oct 2022 20:32:24 GMT  
		Size: 258.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d01b2bd56df6d823af6ff936600b456e3a7e94bbab1df9a52b59df7ed84c832d`  
		Last Modified: Tue, 11 Oct 2022 20:32:43 GMT  
		Size: 127.6 MB (127645294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39ca09d481ffc70add23e3d81c2a8d0bf7c30928edf8650a3cd3464c14022eb6`  
		Last Modified: Tue, 11 Oct 2022 20:32:24 GMT  
		Size: 846.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd5bd9407260ce1a7ee0cd4090756c9dea74c7ff2e0f9f67707bcd3a0afedea5`  
		Last Modified: Wed, 19 Oct 2022 19:25:32 GMT  
		Size: 5.4 KB (5386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5227be166f712520b21a76c9ed1e61648494703fa3c3b55d0d3fcaeabe32547f`  
		Last Modified: Wed, 19 Oct 2022 19:25:32 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
