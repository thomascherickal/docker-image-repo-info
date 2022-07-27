## `mysql:5-debian`

```console
$ docker pull mysql@sha256:d150c2e5269349200254d3fddb6bb00b6d3f3b4f301c8b050193ce02235e2bd1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5-debian` - linux; amd64

```console
$ docker pull mysql@sha256:7d71e364a747cdf4c564a78c439e28b831d1b4013937c925a63b6502c4bb03e1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **162.5 MB (162535672 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96e7464ce3a1541cd7c305635158e6965c7aa939595b401b918d878ab8e8110e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 12 Jul 2022 01:20:32 GMT
ADD file:7f2320197e75c5169402827ce0c47d93629331875d76b9f0ddd389244747eccd in / 
# Tue, 12 Jul 2022 01:20:33 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 01:50:41 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 12 Jul 2022 01:50:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 01:50:48 GMT
ENV GOSU_VERSION=1.14
# Tue, 12 Jul 2022 01:50:57 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 12 Jul 2022 01:50:57 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 12 Jul 2022 01:51:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 01:51:05 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Tue, 12 Jul 2022 01:51:05 GMT
ENV MYSQL_MAJOR=5.7
# Tue, 26 Jul 2022 23:29:39 GMT
ENV MYSQL_VERSION=5.7.39-1debian10
# Tue, 26 Jul 2022 23:29:39 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-5.7' > /etc/apt/sources.list.d/mysql.list
# Tue, 26 Jul 2022 23:29:58 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-server="${MYSQL_VERSION}" 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 26 Jul 2022 23:29:59 GMT
VOLUME [/var/lib/mysql]
# Tue, 26 Jul 2022 23:29:59 GMT
COPY file:d27cf504fa76fb5a4038020a01eaaf52723b17b751566119de311adacb043752 in /usr/local/bin/ 
# Tue, 26 Jul 2022 23:30:00 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 26 Jul 2022 23:30:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 26 Jul 2022 23:30:00 GMT
EXPOSE 3306 33060
# Tue, 26 Jul 2022 23:30:00 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:ac2fb615420c18b61e0693f2569a3d38e3b9b58456b691bac44405e08389a591`  
		Last Modified: Tue, 12 Jul 2022 01:25:22 GMT  
		Size: 27.1 MB (27139850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c67721b86bd696950ee55207c50a132ffea3fd315ce65340a9364aa2b0a28b71`  
		Last Modified: Tue, 12 Jul 2022 01:53:21 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a459e3867bf64a340f900e39d7bcaa2e41acc1a1bbf6534a5f808dc821c198d`  
		Last Modified: Tue, 12 Jul 2022 01:53:19 GMT  
		Size: 4.2 MB (4179193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4146b33aaf1f61e1e653cc708bd8aca2aba92bc9de0ed003536be939c133e815`  
		Last Modified: Tue, 12 Jul 2022 01:53:19 GMT  
		Size: 1.4 MB (1386646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01dc4ff4603c80ddf6552e8a571530056427fcadc9eeda2864926afb0bcfb04c`  
		Last Modified: Tue, 12 Jul 2022 01:53:18 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eae6e50dbb1b5a2203bce53487d118136572c3b462597c0c55400cad43cf359`  
		Last Modified: Tue, 12 Jul 2022 01:53:21 GMT  
		Size: 14.1 MB (14086975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba7a8db4d7e220d8a84874391bc45a74f1482d62ffd0ba285904d5d0280ba290`  
		Last Modified: Tue, 12 Jul 2022 01:53:16 GMT  
		Size: 2.5 KB (2548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8fd0393c8403efcb77e99b1edc7a90b98ceac858a821e21704a4f48f10d4b98`  
		Last Modified: Tue, 26 Jul 2022 23:32:11 GMT  
		Size: 255.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61755fb54b19fb7c2751fa8c64fd26d43621cce235c36793339e494c768c39f0`  
		Last Modified: Tue, 26 Jul 2022 23:32:26 GMT  
		Size: 115.7 MB (115733043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4cdf50400e14a83af72628ac5bdd68b13c9a5b5f33e1b471c962277e79795cd`  
		Last Modified: Tue, 26 Jul 2022 23:32:11 GMT  
		Size: 5.2 KB (5158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b2b65322bb3e6ec927486d764cc71e9fd17af86fcc3acd9b63214438d84f356`  
		Last Modified: Tue, 26 Jul 2022 23:32:11 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
