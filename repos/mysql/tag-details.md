<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `mysql`

-	[`mysql:5`](#mysql5)
-	[`mysql:5.6`](#mysql56)
-	[`mysql:5.6.51`](#mysql5651)
-	[`mysql:5.7`](#mysql57)
-	[`mysql:5.7.35`](#mysql5735)
-	[`mysql:8`](#mysql8)
-	[`mysql:8.0`](#mysql80)
-	[`mysql:8.0.26`](#mysql8026)
-	[`mysql:latest`](#mysqllatest)

## `mysql:5`

```console
$ docker pull mysql@sha256:b8814059bbd9c80b78fe4b2b0b70cd70fe3772b3c5d8ee1edfa46791db3224f9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5` - linux; amd64

```console
$ docker pull mysql@sha256:748f9a853e97c01a8ea530946ad564d6fd0f5bf98fbdf3919920a066266f071e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.8 MB (154784589 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a8a506ccfdc7699b62e0818774fa06c7e1f30d17b4695d2c8be42848870e2ef`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 12 Oct 2021 01:21:05 GMT
ADD file:910392427fdf089bc26b64d6dc450ff3d020c7c1a474d85b2f9298134d0007bd in / 
# Tue, 12 Oct 2021 01:21:05 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 16:22:41 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 12 Oct 2021 16:22:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 16:22:48 GMT
ENV GOSU_VERSION=1.12
# Tue, 12 Oct 2021 16:22:57 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 12 Oct 2021 16:22:58 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 12 Oct 2021 16:23:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		pwgen 		openssl 		perl 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 16:23:15 GMT
RUN set -ex; 	key='A4A9406876FCBD3C456770C88C718D3B5072E1F5'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list > /dev/null
# Tue, 12 Oct 2021 16:23:38 GMT
ENV MYSQL_MAJOR=5.7
# Tue, 12 Oct 2021 16:23:38 GMT
ENV MYSQL_VERSION=5.7.35-1debian10
# Tue, 12 Oct 2021 16:23:39 GMT
RUN echo 'deb http://repo.mysql.com/apt/debian/ buster mysql-5.7' > /etc/apt/sources.list.d/mysql.list
# Tue, 12 Oct 2021 16:24:00 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-server="${MYSQL_VERSION}" 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 12 Oct 2021 16:24:00 GMT
VOLUME [/var/lib/mysql]
# Tue, 12 Oct 2021 16:24:00 GMT
COPY file:345a22fe55d3e6783a17075612415413487e7dba27fbf1000a67c7870364b739 in /usr/local/bin/ 
# Tue, 12 Oct 2021 16:24:01 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 12 Oct 2021 16:24:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Oct 2021 16:24:02 GMT
EXPOSE 3306 33060
# Tue, 12 Oct 2021 16:24:02 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:b380bbd43752f83945df8b5d1074fef8dd044820e7d3aef33b655a2483e030c7`  
		Last Modified: Tue, 12 Oct 2021 01:26:51 GMT  
		Size: 27.1 MB (27139510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f23cbf2ecc5d6ad68efaf326f8ff1c8b4adfab8faad61315440d21c396dd0160`  
		Last Modified: Tue, 12 Oct 2021 16:25:22 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30cfc6c29c0af103c07adaa5e3ee70ffbd8de71ca7b9155079c9769f45fb9aa4`  
		Last Modified: Tue, 12 Oct 2021 16:25:22 GMT  
		Size: 4.2 MB (4179263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b38609286cbe5e62cb8a5a9cb7ed553050e6fc1fa4c537b46c54b6d81a527a7b`  
		Last Modified: Tue, 12 Oct 2021 16:25:20 GMT  
		Size: 1.4 MB (1419434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8211d9e66cd658ab45002b3fa5f8558cd8c13d2f07ba492d7ea1520718d32cff`  
		Last Modified: Tue, 12 Oct 2021 16:25:19 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2313f9eeca4a60533540741b85137033831959ae5a9c4ea652fa4605c9a14bae`  
		Last Modified: Tue, 12 Oct 2021 16:25:23 GMT  
		Size: 13.4 MB (13448689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eb487d00da0bfa9e36634d8c6ceae1e2116f2b56da6b272bec5233966f989e8`  
		Last Modified: Tue, 12 Oct 2021 16:25:19 GMT  
		Size: 1.9 KB (1879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb9cc5c700e7fb7e0ca9db042b78b50e144da72defc9ddbf857f86d060910694`  
		Last Modified: Tue, 12 Oct 2021 16:25:53 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88676eb32344873441c993c766bd6b35cb18662b1c02838ba5afebaf244a8791`  
		Last Modified: Tue, 12 Oct 2021 16:26:09 GMT  
		Size: 108.6 MB (108588045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fea0b38a34855016edc5fc573eede479e4fcb0cecdd87872a9b38aa33b16c98`  
		Last Modified: Tue, 12 Oct 2021 16:25:52 GMT  
		Size: 5.5 KB (5542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dc585bfc69349e8092a6e6e66c66562a344178408b2bd607cbb064e084894f7`  
		Last Modified: Tue, 12 Oct 2021 16:25:53 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.6`

```console
$ docker pull mysql@sha256:cdb7b3a69c0f36ce61dda653cdbe1bf086b6a98c1bf6fa023f7a37bc8325dc98
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.6` - linux; amd64

```console
$ docker pull mysql@sha256:6ba9428c3fbac40577e86367043c044f1edad9738629300ba0602d05bd1b12d1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **103.0 MB (102970747 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3b364958c233566bff03ad2a44a417c7efe192a08a0ceebbb9b75316ca831d7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 12 Oct 2021 01:22:52 GMT
ADD file:1220579e31585dec45ca8e35874eb689018ed026a1f23b7906f791c0279671e0 in / 
# Tue, 12 Oct 2021 01:22:53 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 16:24:07 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 12 Oct 2021 16:24:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 16:24:13 GMT
ENV GOSU_VERSION=1.12
# Tue, 12 Oct 2021 16:24:25 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 12 Oct 2021 16:24:26 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 12 Oct 2021 16:24:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		pwgen 		perl 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 16:24:41 GMT
RUN set -ex; 	key='A4A9406876FCBD3C456770C88C718D3B5072E1F5'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list > /dev/null
# Tue, 12 Oct 2021 16:24:41 GMT
ENV MYSQL_MAJOR=5.6
# Tue, 12 Oct 2021 16:24:42 GMT
ENV MYSQL_VERSION=5.6.51-1debian9
# Tue, 12 Oct 2021 16:24:42 GMT
RUN echo 'deb http://repo.mysql.com/apt/debian/ stretch mysql-5.6' > /etc/apt/sources.list.d/mysql.list
# Tue, 12 Oct 2021 16:24:58 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-server="${MYSQL_VERSION}" 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 12 Oct 2021 16:24:58 GMT
VOLUME [/var/lib/mysql]
# Tue, 12 Oct 2021 16:24:58 GMT
COPY file:345a22fe55d3e6783a17075612415413487e7dba27fbf1000a67c7870364b739 in /usr/local/bin/ 
# Tue, 12 Oct 2021 16:24:59 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 12 Oct 2021 16:24:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Oct 2021 16:25:00 GMT
EXPOSE 3306
# Tue, 12 Oct 2021 16:25:00 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:eec53b8a5053c739b5b685cb372b38eea3286ab6626532bad963291f76357c5f`  
		Last Modified: Tue, 12 Oct 2021 01:29:50 GMT  
		Size: 22.5 MB (22527572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0f71fe48852c9b99183aa3fb3e2b06a3f7ed3be6a80daa334d50d699967569b`  
		Last Modified: Tue, 12 Oct 2021 16:26:28 GMT  
		Size: 1.7 KB (1740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0bdbff3130a5d3a456985fa0aa55dff7e2fa29ef25cb4a27d02fb2576a4f655`  
		Last Modified: Tue, 12 Oct 2021 16:26:27 GMT  
		Size: 4.5 MB (4503783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10b14d18e3a15974a3fb11ed8cfbc1581b366778c499fec9b942cb527d8f04a5`  
		Last Modified: Tue, 12 Oct 2021 16:26:26 GMT  
		Size: 1.4 MB (1412168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45ba66db8ef39763b31bb58f3a00350ecb0ce1bb2576b8a3b5a66d519fd97806`  
		Last Modified: Tue, 12 Oct 2021 16:26:25 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7c7e25beebfaaab4021d84aa09b67939daa38760fd93fe201332e1e0bd94809`  
		Last Modified: Tue, 12 Oct 2021 16:26:28 GMT  
		Size: 10.2 MB (10225752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d69efd6c310472dc45954a35daea0d44580e6f56a9a0d7c91008f0496d98e27`  
		Last Modified: Tue, 12 Oct 2021 16:26:23 GMT  
		Size: 19.5 KB (19458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef665230f46f036e65cac1d260bb2b46a2d1e12a16733d0823f210ee42fbc99c`  
		Last Modified: Tue, 12 Oct 2021 16:26:23 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f26c5841884ece34d2701091a7188d2a21b63f62d41c4dd39a165a71551e345`  
		Last Modified: Tue, 12 Oct 2021 16:26:34 GMT  
		Size: 64.3 MB (64274226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc57157e768b6b8cfc4aaf8579aa43a1f3239fca95eee1361b7224d4d4190f31`  
		Last Modified: Tue, 12 Oct 2021 16:26:23 GMT  
		Size: 5.6 KB (5559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:934b60bbc78c93ed4a3eb1d513c8ff2d592e66ce1e27f2faf233ff3a3a90155c`  
		Last Modified: Tue, 12 Oct 2021 16:26:23 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.6.51`

```console
$ docker pull mysql@sha256:cdb7b3a69c0f36ce61dda653cdbe1bf086b6a98c1bf6fa023f7a37bc8325dc98
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.6.51` - linux; amd64

```console
$ docker pull mysql@sha256:6ba9428c3fbac40577e86367043c044f1edad9738629300ba0602d05bd1b12d1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **103.0 MB (102970747 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3b364958c233566bff03ad2a44a417c7efe192a08a0ceebbb9b75316ca831d7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 12 Oct 2021 01:22:52 GMT
ADD file:1220579e31585dec45ca8e35874eb689018ed026a1f23b7906f791c0279671e0 in / 
# Tue, 12 Oct 2021 01:22:53 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 16:24:07 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 12 Oct 2021 16:24:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 16:24:13 GMT
ENV GOSU_VERSION=1.12
# Tue, 12 Oct 2021 16:24:25 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 12 Oct 2021 16:24:26 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 12 Oct 2021 16:24:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		pwgen 		perl 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 16:24:41 GMT
RUN set -ex; 	key='A4A9406876FCBD3C456770C88C718D3B5072E1F5'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list > /dev/null
# Tue, 12 Oct 2021 16:24:41 GMT
ENV MYSQL_MAJOR=5.6
# Tue, 12 Oct 2021 16:24:42 GMT
ENV MYSQL_VERSION=5.6.51-1debian9
# Tue, 12 Oct 2021 16:24:42 GMT
RUN echo 'deb http://repo.mysql.com/apt/debian/ stretch mysql-5.6' > /etc/apt/sources.list.d/mysql.list
# Tue, 12 Oct 2021 16:24:58 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-server="${MYSQL_VERSION}" 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 12 Oct 2021 16:24:58 GMT
VOLUME [/var/lib/mysql]
# Tue, 12 Oct 2021 16:24:58 GMT
COPY file:345a22fe55d3e6783a17075612415413487e7dba27fbf1000a67c7870364b739 in /usr/local/bin/ 
# Tue, 12 Oct 2021 16:24:59 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 12 Oct 2021 16:24:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Oct 2021 16:25:00 GMT
EXPOSE 3306
# Tue, 12 Oct 2021 16:25:00 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:eec53b8a5053c739b5b685cb372b38eea3286ab6626532bad963291f76357c5f`  
		Last Modified: Tue, 12 Oct 2021 01:29:50 GMT  
		Size: 22.5 MB (22527572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0f71fe48852c9b99183aa3fb3e2b06a3f7ed3be6a80daa334d50d699967569b`  
		Last Modified: Tue, 12 Oct 2021 16:26:28 GMT  
		Size: 1.7 KB (1740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0bdbff3130a5d3a456985fa0aa55dff7e2fa29ef25cb4a27d02fb2576a4f655`  
		Last Modified: Tue, 12 Oct 2021 16:26:27 GMT  
		Size: 4.5 MB (4503783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10b14d18e3a15974a3fb11ed8cfbc1581b366778c499fec9b942cb527d8f04a5`  
		Last Modified: Tue, 12 Oct 2021 16:26:26 GMT  
		Size: 1.4 MB (1412168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45ba66db8ef39763b31bb58f3a00350ecb0ce1bb2576b8a3b5a66d519fd97806`  
		Last Modified: Tue, 12 Oct 2021 16:26:25 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7c7e25beebfaaab4021d84aa09b67939daa38760fd93fe201332e1e0bd94809`  
		Last Modified: Tue, 12 Oct 2021 16:26:28 GMT  
		Size: 10.2 MB (10225752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d69efd6c310472dc45954a35daea0d44580e6f56a9a0d7c91008f0496d98e27`  
		Last Modified: Tue, 12 Oct 2021 16:26:23 GMT  
		Size: 19.5 KB (19458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef665230f46f036e65cac1d260bb2b46a2d1e12a16733d0823f210ee42fbc99c`  
		Last Modified: Tue, 12 Oct 2021 16:26:23 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f26c5841884ece34d2701091a7188d2a21b63f62d41c4dd39a165a71551e345`  
		Last Modified: Tue, 12 Oct 2021 16:26:34 GMT  
		Size: 64.3 MB (64274226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc57157e768b6b8cfc4aaf8579aa43a1f3239fca95eee1361b7224d4d4190f31`  
		Last Modified: Tue, 12 Oct 2021 16:26:23 GMT  
		Size: 5.6 KB (5559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:934b60bbc78c93ed4a3eb1d513c8ff2d592e66ce1e27f2faf233ff3a3a90155c`  
		Last Modified: Tue, 12 Oct 2021 16:26:23 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7`

```console
$ docker pull mysql@sha256:b8814059bbd9c80b78fe4b2b0b70cd70fe3772b3c5d8ee1edfa46791db3224f9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7` - linux; amd64

```console
$ docker pull mysql@sha256:748f9a853e97c01a8ea530946ad564d6fd0f5bf98fbdf3919920a066266f071e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.8 MB (154784589 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a8a506ccfdc7699b62e0818774fa06c7e1f30d17b4695d2c8be42848870e2ef`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 12 Oct 2021 01:21:05 GMT
ADD file:910392427fdf089bc26b64d6dc450ff3d020c7c1a474d85b2f9298134d0007bd in / 
# Tue, 12 Oct 2021 01:21:05 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 16:22:41 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 12 Oct 2021 16:22:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 16:22:48 GMT
ENV GOSU_VERSION=1.12
# Tue, 12 Oct 2021 16:22:57 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 12 Oct 2021 16:22:58 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 12 Oct 2021 16:23:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		pwgen 		openssl 		perl 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 16:23:15 GMT
RUN set -ex; 	key='A4A9406876FCBD3C456770C88C718D3B5072E1F5'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list > /dev/null
# Tue, 12 Oct 2021 16:23:38 GMT
ENV MYSQL_MAJOR=5.7
# Tue, 12 Oct 2021 16:23:38 GMT
ENV MYSQL_VERSION=5.7.35-1debian10
# Tue, 12 Oct 2021 16:23:39 GMT
RUN echo 'deb http://repo.mysql.com/apt/debian/ buster mysql-5.7' > /etc/apt/sources.list.d/mysql.list
# Tue, 12 Oct 2021 16:24:00 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-server="${MYSQL_VERSION}" 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 12 Oct 2021 16:24:00 GMT
VOLUME [/var/lib/mysql]
# Tue, 12 Oct 2021 16:24:00 GMT
COPY file:345a22fe55d3e6783a17075612415413487e7dba27fbf1000a67c7870364b739 in /usr/local/bin/ 
# Tue, 12 Oct 2021 16:24:01 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 12 Oct 2021 16:24:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Oct 2021 16:24:02 GMT
EXPOSE 3306 33060
# Tue, 12 Oct 2021 16:24:02 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:b380bbd43752f83945df8b5d1074fef8dd044820e7d3aef33b655a2483e030c7`  
		Last Modified: Tue, 12 Oct 2021 01:26:51 GMT  
		Size: 27.1 MB (27139510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f23cbf2ecc5d6ad68efaf326f8ff1c8b4adfab8faad61315440d21c396dd0160`  
		Last Modified: Tue, 12 Oct 2021 16:25:22 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30cfc6c29c0af103c07adaa5e3ee70ffbd8de71ca7b9155079c9769f45fb9aa4`  
		Last Modified: Tue, 12 Oct 2021 16:25:22 GMT  
		Size: 4.2 MB (4179263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b38609286cbe5e62cb8a5a9cb7ed553050e6fc1fa4c537b46c54b6d81a527a7b`  
		Last Modified: Tue, 12 Oct 2021 16:25:20 GMT  
		Size: 1.4 MB (1419434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8211d9e66cd658ab45002b3fa5f8558cd8c13d2f07ba492d7ea1520718d32cff`  
		Last Modified: Tue, 12 Oct 2021 16:25:19 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2313f9eeca4a60533540741b85137033831959ae5a9c4ea652fa4605c9a14bae`  
		Last Modified: Tue, 12 Oct 2021 16:25:23 GMT  
		Size: 13.4 MB (13448689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eb487d00da0bfa9e36634d8c6ceae1e2116f2b56da6b272bec5233966f989e8`  
		Last Modified: Tue, 12 Oct 2021 16:25:19 GMT  
		Size: 1.9 KB (1879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb9cc5c700e7fb7e0ca9db042b78b50e144da72defc9ddbf857f86d060910694`  
		Last Modified: Tue, 12 Oct 2021 16:25:53 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88676eb32344873441c993c766bd6b35cb18662b1c02838ba5afebaf244a8791`  
		Last Modified: Tue, 12 Oct 2021 16:26:09 GMT  
		Size: 108.6 MB (108588045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fea0b38a34855016edc5fc573eede479e4fcb0cecdd87872a9b38aa33b16c98`  
		Last Modified: Tue, 12 Oct 2021 16:25:52 GMT  
		Size: 5.5 KB (5542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dc585bfc69349e8092a6e6e66c66562a344178408b2bd607cbb064e084894f7`  
		Last Modified: Tue, 12 Oct 2021 16:25:53 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7.35`

```console
$ docker pull mysql@sha256:b8814059bbd9c80b78fe4b2b0b70cd70fe3772b3c5d8ee1edfa46791db3224f9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7.35` - linux; amd64

```console
$ docker pull mysql@sha256:748f9a853e97c01a8ea530946ad564d6fd0f5bf98fbdf3919920a066266f071e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.8 MB (154784589 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a8a506ccfdc7699b62e0818774fa06c7e1f30d17b4695d2c8be42848870e2ef`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 12 Oct 2021 01:21:05 GMT
ADD file:910392427fdf089bc26b64d6dc450ff3d020c7c1a474d85b2f9298134d0007bd in / 
# Tue, 12 Oct 2021 01:21:05 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 16:22:41 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 12 Oct 2021 16:22:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 16:22:48 GMT
ENV GOSU_VERSION=1.12
# Tue, 12 Oct 2021 16:22:57 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 12 Oct 2021 16:22:58 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 12 Oct 2021 16:23:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		pwgen 		openssl 		perl 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 16:23:15 GMT
RUN set -ex; 	key='A4A9406876FCBD3C456770C88C718D3B5072E1F5'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list > /dev/null
# Tue, 12 Oct 2021 16:23:38 GMT
ENV MYSQL_MAJOR=5.7
# Tue, 12 Oct 2021 16:23:38 GMT
ENV MYSQL_VERSION=5.7.35-1debian10
# Tue, 12 Oct 2021 16:23:39 GMT
RUN echo 'deb http://repo.mysql.com/apt/debian/ buster mysql-5.7' > /etc/apt/sources.list.d/mysql.list
# Tue, 12 Oct 2021 16:24:00 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-server="${MYSQL_VERSION}" 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 12 Oct 2021 16:24:00 GMT
VOLUME [/var/lib/mysql]
# Tue, 12 Oct 2021 16:24:00 GMT
COPY file:345a22fe55d3e6783a17075612415413487e7dba27fbf1000a67c7870364b739 in /usr/local/bin/ 
# Tue, 12 Oct 2021 16:24:01 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 12 Oct 2021 16:24:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Oct 2021 16:24:02 GMT
EXPOSE 3306 33060
# Tue, 12 Oct 2021 16:24:02 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:b380bbd43752f83945df8b5d1074fef8dd044820e7d3aef33b655a2483e030c7`  
		Last Modified: Tue, 12 Oct 2021 01:26:51 GMT  
		Size: 27.1 MB (27139510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f23cbf2ecc5d6ad68efaf326f8ff1c8b4adfab8faad61315440d21c396dd0160`  
		Last Modified: Tue, 12 Oct 2021 16:25:22 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30cfc6c29c0af103c07adaa5e3ee70ffbd8de71ca7b9155079c9769f45fb9aa4`  
		Last Modified: Tue, 12 Oct 2021 16:25:22 GMT  
		Size: 4.2 MB (4179263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b38609286cbe5e62cb8a5a9cb7ed553050e6fc1fa4c537b46c54b6d81a527a7b`  
		Last Modified: Tue, 12 Oct 2021 16:25:20 GMT  
		Size: 1.4 MB (1419434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8211d9e66cd658ab45002b3fa5f8558cd8c13d2f07ba492d7ea1520718d32cff`  
		Last Modified: Tue, 12 Oct 2021 16:25:19 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2313f9eeca4a60533540741b85137033831959ae5a9c4ea652fa4605c9a14bae`  
		Last Modified: Tue, 12 Oct 2021 16:25:23 GMT  
		Size: 13.4 MB (13448689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eb487d00da0bfa9e36634d8c6ceae1e2116f2b56da6b272bec5233966f989e8`  
		Last Modified: Tue, 12 Oct 2021 16:25:19 GMT  
		Size: 1.9 KB (1879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb9cc5c700e7fb7e0ca9db042b78b50e144da72defc9ddbf857f86d060910694`  
		Last Modified: Tue, 12 Oct 2021 16:25:53 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88676eb32344873441c993c766bd6b35cb18662b1c02838ba5afebaf244a8791`  
		Last Modified: Tue, 12 Oct 2021 16:26:09 GMT  
		Size: 108.6 MB (108588045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fea0b38a34855016edc5fc573eede479e4fcb0cecdd87872a9b38aa33b16c98`  
		Last Modified: Tue, 12 Oct 2021 16:25:52 GMT  
		Size: 5.5 KB (5542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dc585bfc69349e8092a6e6e66c66562a344178408b2bd607cbb064e084894f7`  
		Last Modified: Tue, 12 Oct 2021 16:25:53 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8`

```console
$ docker pull mysql@sha256:5d52dc010398db422949f079c76e98f6b62230e5b59c0bf7582409d2c85abacb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:8` - linux; amd64

```console
$ docker pull mysql@sha256:882e55f40d61034a2bb8a1abab1353571ad2a33866f382350788eb34740528b5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **150.6 MB (150587534 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9da615fced53bc1bc11e3d7f20a37873362e1d5354354238f0b63c6d549f7f66`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 12 Oct 2021 01:21:05 GMT
ADD file:910392427fdf089bc26b64d6dc450ff3d020c7c1a474d85b2f9298134d0007bd in / 
# Tue, 12 Oct 2021 01:21:05 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 16:22:41 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 12 Oct 2021 16:22:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 16:22:48 GMT
ENV GOSU_VERSION=1.12
# Tue, 12 Oct 2021 16:22:57 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 12 Oct 2021 16:22:58 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 12 Oct 2021 16:23:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		pwgen 		openssl 		perl 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 16:23:15 GMT
RUN set -ex; 	key='A4A9406876FCBD3C456770C88C718D3B5072E1F5'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list > /dev/null
# Tue, 12 Oct 2021 16:23:15 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 12 Oct 2021 16:23:16 GMT
ENV MYSQL_VERSION=8.0.26-1debian10
# Tue, 12 Oct 2021 16:23:16 GMT
RUN echo 'deb http://repo.mysql.com/apt/debian/ buster mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Tue, 12 Oct 2021 16:23:31 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 12 Oct 2021 16:23:32 GMT
VOLUME [/var/lib/mysql]
# Tue, 12 Oct 2021 16:23:32 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Tue, 12 Oct 2021 16:23:32 GMT
COPY file:345a22fe55d3e6783a17075612415413487e7dba27fbf1000a67c7870364b739 in /usr/local/bin/ 
# Tue, 12 Oct 2021 16:23:33 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 12 Oct 2021 16:23:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Oct 2021 16:23:34 GMT
EXPOSE 3306 33060
# Tue, 12 Oct 2021 16:23:34 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:b380bbd43752f83945df8b5d1074fef8dd044820e7d3aef33b655a2483e030c7`  
		Last Modified: Tue, 12 Oct 2021 01:26:51 GMT  
		Size: 27.1 MB (27139510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f23cbf2ecc5d6ad68efaf326f8ff1c8b4adfab8faad61315440d21c396dd0160`  
		Last Modified: Tue, 12 Oct 2021 16:25:22 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30cfc6c29c0af103c07adaa5e3ee70ffbd8de71ca7b9155079c9769f45fb9aa4`  
		Last Modified: Tue, 12 Oct 2021 16:25:22 GMT  
		Size: 4.2 MB (4179263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b38609286cbe5e62cb8a5a9cb7ed553050e6fc1fa4c537b46c54b6d81a527a7b`  
		Last Modified: Tue, 12 Oct 2021 16:25:20 GMT  
		Size: 1.4 MB (1419434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8211d9e66cd658ab45002b3fa5f8558cd8c13d2f07ba492d7ea1520718d32cff`  
		Last Modified: Tue, 12 Oct 2021 16:25:19 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2313f9eeca4a60533540741b85137033831959ae5a9c4ea652fa4605c9a14bae`  
		Last Modified: Tue, 12 Oct 2021 16:25:23 GMT  
		Size: 13.4 MB (13448689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eb487d00da0bfa9e36634d8c6ceae1e2116f2b56da6b272bec5233966f989e8`  
		Last Modified: Tue, 12 Oct 2021 16:25:19 GMT  
		Size: 1.9 KB (1879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5d2b117a9385bafc1761e043905b1e9a4b603a52a47b2e6f80fe92621530a95`  
		Last Modified: Tue, 12 Oct 2021 16:25:17 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f6cb474cd1c8a589d731f3aba876196cd5ad15fc04363d07e00998953d8bccc`  
		Last Modified: Tue, 12 Oct 2021 16:25:36 GMT  
		Size: 104.4 MB (104390152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:896b3fd2ab079ed6501a2ddab191810f6e6a91a296a0600451bd5f15eb3be680`  
		Last Modified: Tue, 12 Oct 2021 16:25:17 GMT  
		Size: 842.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:532e67ebb3762ad33b4ffb25848be0166d216f456f7f91c4afff201419f24870`  
		Last Modified: Tue, 12 Oct 2021 16:25:17 GMT  
		Size: 5.5 KB (5541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:233c7958b33f5f424cd93ade1de9ab2c2e26fd7363a99d8b33d5d01ce57bd509`  
		Last Modified: Tue, 12 Oct 2021 16:25:17 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0`

```console
$ docker pull mysql@sha256:5d52dc010398db422949f079c76e98f6b62230e5b59c0bf7582409d2c85abacb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:8.0` - linux; amd64

```console
$ docker pull mysql@sha256:882e55f40d61034a2bb8a1abab1353571ad2a33866f382350788eb34740528b5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **150.6 MB (150587534 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9da615fced53bc1bc11e3d7f20a37873362e1d5354354238f0b63c6d549f7f66`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 12 Oct 2021 01:21:05 GMT
ADD file:910392427fdf089bc26b64d6dc450ff3d020c7c1a474d85b2f9298134d0007bd in / 
# Tue, 12 Oct 2021 01:21:05 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 16:22:41 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 12 Oct 2021 16:22:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 16:22:48 GMT
ENV GOSU_VERSION=1.12
# Tue, 12 Oct 2021 16:22:57 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 12 Oct 2021 16:22:58 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 12 Oct 2021 16:23:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		pwgen 		openssl 		perl 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 16:23:15 GMT
RUN set -ex; 	key='A4A9406876FCBD3C456770C88C718D3B5072E1F5'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list > /dev/null
# Tue, 12 Oct 2021 16:23:15 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 12 Oct 2021 16:23:16 GMT
ENV MYSQL_VERSION=8.0.26-1debian10
# Tue, 12 Oct 2021 16:23:16 GMT
RUN echo 'deb http://repo.mysql.com/apt/debian/ buster mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Tue, 12 Oct 2021 16:23:31 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 12 Oct 2021 16:23:32 GMT
VOLUME [/var/lib/mysql]
# Tue, 12 Oct 2021 16:23:32 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Tue, 12 Oct 2021 16:23:32 GMT
COPY file:345a22fe55d3e6783a17075612415413487e7dba27fbf1000a67c7870364b739 in /usr/local/bin/ 
# Tue, 12 Oct 2021 16:23:33 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 12 Oct 2021 16:23:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Oct 2021 16:23:34 GMT
EXPOSE 3306 33060
# Tue, 12 Oct 2021 16:23:34 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:b380bbd43752f83945df8b5d1074fef8dd044820e7d3aef33b655a2483e030c7`  
		Last Modified: Tue, 12 Oct 2021 01:26:51 GMT  
		Size: 27.1 MB (27139510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f23cbf2ecc5d6ad68efaf326f8ff1c8b4adfab8faad61315440d21c396dd0160`  
		Last Modified: Tue, 12 Oct 2021 16:25:22 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30cfc6c29c0af103c07adaa5e3ee70ffbd8de71ca7b9155079c9769f45fb9aa4`  
		Last Modified: Tue, 12 Oct 2021 16:25:22 GMT  
		Size: 4.2 MB (4179263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b38609286cbe5e62cb8a5a9cb7ed553050e6fc1fa4c537b46c54b6d81a527a7b`  
		Last Modified: Tue, 12 Oct 2021 16:25:20 GMT  
		Size: 1.4 MB (1419434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8211d9e66cd658ab45002b3fa5f8558cd8c13d2f07ba492d7ea1520718d32cff`  
		Last Modified: Tue, 12 Oct 2021 16:25:19 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2313f9eeca4a60533540741b85137033831959ae5a9c4ea652fa4605c9a14bae`  
		Last Modified: Tue, 12 Oct 2021 16:25:23 GMT  
		Size: 13.4 MB (13448689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eb487d00da0bfa9e36634d8c6ceae1e2116f2b56da6b272bec5233966f989e8`  
		Last Modified: Tue, 12 Oct 2021 16:25:19 GMT  
		Size: 1.9 KB (1879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5d2b117a9385bafc1761e043905b1e9a4b603a52a47b2e6f80fe92621530a95`  
		Last Modified: Tue, 12 Oct 2021 16:25:17 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f6cb474cd1c8a589d731f3aba876196cd5ad15fc04363d07e00998953d8bccc`  
		Last Modified: Tue, 12 Oct 2021 16:25:36 GMT  
		Size: 104.4 MB (104390152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:896b3fd2ab079ed6501a2ddab191810f6e6a91a296a0600451bd5f15eb3be680`  
		Last Modified: Tue, 12 Oct 2021 16:25:17 GMT  
		Size: 842.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:532e67ebb3762ad33b4ffb25848be0166d216f456f7f91c4afff201419f24870`  
		Last Modified: Tue, 12 Oct 2021 16:25:17 GMT  
		Size: 5.5 KB (5541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:233c7958b33f5f424cd93ade1de9ab2c2e26fd7363a99d8b33d5d01ce57bd509`  
		Last Modified: Tue, 12 Oct 2021 16:25:17 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0.26`

```console
$ docker pull mysql@sha256:5d52dc010398db422949f079c76e98f6b62230e5b59c0bf7582409d2c85abacb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:8.0.26` - linux; amd64

```console
$ docker pull mysql@sha256:882e55f40d61034a2bb8a1abab1353571ad2a33866f382350788eb34740528b5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **150.6 MB (150587534 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9da615fced53bc1bc11e3d7f20a37873362e1d5354354238f0b63c6d549f7f66`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 12 Oct 2021 01:21:05 GMT
ADD file:910392427fdf089bc26b64d6dc450ff3d020c7c1a474d85b2f9298134d0007bd in / 
# Tue, 12 Oct 2021 01:21:05 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 16:22:41 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 12 Oct 2021 16:22:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 16:22:48 GMT
ENV GOSU_VERSION=1.12
# Tue, 12 Oct 2021 16:22:57 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 12 Oct 2021 16:22:58 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 12 Oct 2021 16:23:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		pwgen 		openssl 		perl 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 16:23:15 GMT
RUN set -ex; 	key='A4A9406876FCBD3C456770C88C718D3B5072E1F5'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list > /dev/null
# Tue, 12 Oct 2021 16:23:15 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 12 Oct 2021 16:23:16 GMT
ENV MYSQL_VERSION=8.0.26-1debian10
# Tue, 12 Oct 2021 16:23:16 GMT
RUN echo 'deb http://repo.mysql.com/apt/debian/ buster mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Tue, 12 Oct 2021 16:23:31 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 12 Oct 2021 16:23:32 GMT
VOLUME [/var/lib/mysql]
# Tue, 12 Oct 2021 16:23:32 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Tue, 12 Oct 2021 16:23:32 GMT
COPY file:345a22fe55d3e6783a17075612415413487e7dba27fbf1000a67c7870364b739 in /usr/local/bin/ 
# Tue, 12 Oct 2021 16:23:33 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 12 Oct 2021 16:23:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Oct 2021 16:23:34 GMT
EXPOSE 3306 33060
# Tue, 12 Oct 2021 16:23:34 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:b380bbd43752f83945df8b5d1074fef8dd044820e7d3aef33b655a2483e030c7`  
		Last Modified: Tue, 12 Oct 2021 01:26:51 GMT  
		Size: 27.1 MB (27139510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f23cbf2ecc5d6ad68efaf326f8ff1c8b4adfab8faad61315440d21c396dd0160`  
		Last Modified: Tue, 12 Oct 2021 16:25:22 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30cfc6c29c0af103c07adaa5e3ee70ffbd8de71ca7b9155079c9769f45fb9aa4`  
		Last Modified: Tue, 12 Oct 2021 16:25:22 GMT  
		Size: 4.2 MB (4179263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b38609286cbe5e62cb8a5a9cb7ed553050e6fc1fa4c537b46c54b6d81a527a7b`  
		Last Modified: Tue, 12 Oct 2021 16:25:20 GMT  
		Size: 1.4 MB (1419434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8211d9e66cd658ab45002b3fa5f8558cd8c13d2f07ba492d7ea1520718d32cff`  
		Last Modified: Tue, 12 Oct 2021 16:25:19 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2313f9eeca4a60533540741b85137033831959ae5a9c4ea652fa4605c9a14bae`  
		Last Modified: Tue, 12 Oct 2021 16:25:23 GMT  
		Size: 13.4 MB (13448689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eb487d00da0bfa9e36634d8c6ceae1e2116f2b56da6b272bec5233966f989e8`  
		Last Modified: Tue, 12 Oct 2021 16:25:19 GMT  
		Size: 1.9 KB (1879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5d2b117a9385bafc1761e043905b1e9a4b603a52a47b2e6f80fe92621530a95`  
		Last Modified: Tue, 12 Oct 2021 16:25:17 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f6cb474cd1c8a589d731f3aba876196cd5ad15fc04363d07e00998953d8bccc`  
		Last Modified: Tue, 12 Oct 2021 16:25:36 GMT  
		Size: 104.4 MB (104390152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:896b3fd2ab079ed6501a2ddab191810f6e6a91a296a0600451bd5f15eb3be680`  
		Last Modified: Tue, 12 Oct 2021 16:25:17 GMT  
		Size: 842.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:532e67ebb3762ad33b4ffb25848be0166d216f456f7f91c4afff201419f24870`  
		Last Modified: Tue, 12 Oct 2021 16:25:17 GMT  
		Size: 5.5 KB (5541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:233c7958b33f5f424cd93ade1de9ab2c2e26fd7363a99d8b33d5d01ce57bd509`  
		Last Modified: Tue, 12 Oct 2021 16:25:17 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:latest`

```console
$ docker pull mysql@sha256:5d52dc010398db422949f079c76e98f6b62230e5b59c0bf7582409d2c85abacb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:latest` - linux; amd64

```console
$ docker pull mysql@sha256:882e55f40d61034a2bb8a1abab1353571ad2a33866f382350788eb34740528b5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **150.6 MB (150587534 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9da615fced53bc1bc11e3d7f20a37873362e1d5354354238f0b63c6d549f7f66`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 12 Oct 2021 01:21:05 GMT
ADD file:910392427fdf089bc26b64d6dc450ff3d020c7c1a474d85b2f9298134d0007bd in / 
# Tue, 12 Oct 2021 01:21:05 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 16:22:41 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 12 Oct 2021 16:22:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 16:22:48 GMT
ENV GOSU_VERSION=1.12
# Tue, 12 Oct 2021 16:22:57 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 12 Oct 2021 16:22:58 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 12 Oct 2021 16:23:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		pwgen 		openssl 		perl 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 16:23:15 GMT
RUN set -ex; 	key='A4A9406876FCBD3C456770C88C718D3B5072E1F5'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list > /dev/null
# Tue, 12 Oct 2021 16:23:15 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 12 Oct 2021 16:23:16 GMT
ENV MYSQL_VERSION=8.0.26-1debian10
# Tue, 12 Oct 2021 16:23:16 GMT
RUN echo 'deb http://repo.mysql.com/apt/debian/ buster mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Tue, 12 Oct 2021 16:23:31 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 12 Oct 2021 16:23:32 GMT
VOLUME [/var/lib/mysql]
# Tue, 12 Oct 2021 16:23:32 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Tue, 12 Oct 2021 16:23:32 GMT
COPY file:345a22fe55d3e6783a17075612415413487e7dba27fbf1000a67c7870364b739 in /usr/local/bin/ 
# Tue, 12 Oct 2021 16:23:33 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 12 Oct 2021 16:23:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Oct 2021 16:23:34 GMT
EXPOSE 3306 33060
# Tue, 12 Oct 2021 16:23:34 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:b380bbd43752f83945df8b5d1074fef8dd044820e7d3aef33b655a2483e030c7`  
		Last Modified: Tue, 12 Oct 2021 01:26:51 GMT  
		Size: 27.1 MB (27139510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f23cbf2ecc5d6ad68efaf326f8ff1c8b4adfab8faad61315440d21c396dd0160`  
		Last Modified: Tue, 12 Oct 2021 16:25:22 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30cfc6c29c0af103c07adaa5e3ee70ffbd8de71ca7b9155079c9769f45fb9aa4`  
		Last Modified: Tue, 12 Oct 2021 16:25:22 GMT  
		Size: 4.2 MB (4179263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b38609286cbe5e62cb8a5a9cb7ed553050e6fc1fa4c537b46c54b6d81a527a7b`  
		Last Modified: Tue, 12 Oct 2021 16:25:20 GMT  
		Size: 1.4 MB (1419434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8211d9e66cd658ab45002b3fa5f8558cd8c13d2f07ba492d7ea1520718d32cff`  
		Last Modified: Tue, 12 Oct 2021 16:25:19 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2313f9eeca4a60533540741b85137033831959ae5a9c4ea652fa4605c9a14bae`  
		Last Modified: Tue, 12 Oct 2021 16:25:23 GMT  
		Size: 13.4 MB (13448689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eb487d00da0bfa9e36634d8c6ceae1e2116f2b56da6b272bec5233966f989e8`  
		Last Modified: Tue, 12 Oct 2021 16:25:19 GMT  
		Size: 1.9 KB (1879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5d2b117a9385bafc1761e043905b1e9a4b603a52a47b2e6f80fe92621530a95`  
		Last Modified: Tue, 12 Oct 2021 16:25:17 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f6cb474cd1c8a589d731f3aba876196cd5ad15fc04363d07e00998953d8bccc`  
		Last Modified: Tue, 12 Oct 2021 16:25:36 GMT  
		Size: 104.4 MB (104390152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:896b3fd2ab079ed6501a2ddab191810f6e6a91a296a0600451bd5f15eb3be680`  
		Last Modified: Tue, 12 Oct 2021 16:25:17 GMT  
		Size: 842.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:532e67ebb3762ad33b4ffb25848be0166d216f456f7f91c4afff201419f24870`  
		Last Modified: Tue, 12 Oct 2021 16:25:17 GMT  
		Size: 5.5 KB (5541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:233c7958b33f5f424cd93ade1de9ab2c2e26fd7363a99d8b33d5d01ce57bd509`  
		Last Modified: Tue, 12 Oct 2021 16:25:17 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
