<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `mysql`

-	[`mysql:5`](#mysql5)
-	[`mysql:5.6`](#mysql56)
-	[`mysql:5.6.49`](#mysql5649)
-	[`mysql:5.7`](#mysql57)
-	[`mysql:5.7.31`](#mysql5731)
-	[`mysql:8`](#mysql8)
-	[`mysql:8.0`](#mysql80)
-	[`mysql:8.0.21`](#mysql8021)
-	[`mysql:latest`](#mysqllatest)

## `mysql:5`

```console
$ docker pull mysql@sha256:da58f943b94721d46e87d5de208dc07302a8b13e638cd1d24285d222376d6d84
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mysql:5` - linux; amd64

```console
$ docker pull mysql@sha256:d3418a353847c7b34e3b082d1ea35a9d12fd1244d3d841d8cfe076e72c216b00
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.5 MB (154474259 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:718a6da099d82183c064a964523c0deca80619cb033aadd15854771fe592a480`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 04 Aug 2020 15:42:51 GMT
ADD file:3af3091e7d2bb40bc1e6550eb5ea290badc6bbf3339105626f245a963cc11450 in / 
# Tue, 04 Aug 2020 15:42:51 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 23:19:19 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 04 Aug 2020 23:19:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 23:19:26 GMT
ENV GOSU_VERSION=1.12
# Tue, 04 Aug 2020 23:19:34 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 04 Aug 2020 23:19:35 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 04 Aug 2020 23:19:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		pwgen 		openssl 		perl 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 23:19:45 GMT
RUN set -ex; 	key='A4A9406876FCBD3C456770C88C718D3B5072E1F5'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list > /dev/null
# Tue, 04 Aug 2020 23:20:14 GMT
ENV MYSQL_MAJOR=5.7
# Tue, 04 Aug 2020 23:20:14 GMT
ENV MYSQL_VERSION=5.7.31-1debian10
# Tue, 04 Aug 2020 23:20:15 GMT
RUN echo "deb http://repo.mysql.com/apt/debian/ buster mysql-${MYSQL_MAJOR}" > /etc/apt/sources.list.d/mysql.list
# Tue, 04 Aug 2020 23:20:38 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update && apt-get install -y mysql-server="${MYSQL_VERSION}" && rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 777 /var/run/mysqld 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Tue, 04 Aug 2020 23:20:38 GMT
VOLUME [/var/lib/mysql]
# Tue, 04 Aug 2020 23:20:39 GMT
COPY file:7cbb26bbdb8e71b36aafda38dbac08caa641714a19991b86cde77daf3286ec11 in /usr/local/bin/ 
# Tue, 04 Aug 2020 23:20:39 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 04 Aug 2020 23:20:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Aug 2020 23:20:40 GMT
EXPOSE 3306 33060
# Tue, 04 Aug 2020 23:20:40 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:bf59529304463f62efa7179fa1a32718a611528cc4ce9f30c0d1bbc6724ec3fb`  
		Last Modified: Tue, 04 Aug 2020 15:49:09 GMT  
		Size: 27.1 MB (27092121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8254623a9871b825936fce675bd714b26e4291b14f382b88d36ae9d85e304ed4`  
		Last Modified: Tue, 04 Aug 2020 23:21:49 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:938e3e06dac451f904a36d49c72fb11a2366176eb3b9bd7e8a71153028a9cfd3`  
		Last Modified: Tue, 04 Aug 2020 23:21:51 GMT  
		Size: 4.2 MB (4178123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea28ebf28884e64ac7e9d560727639795015425e5ea74f69a2101f6e16a43826`  
		Last Modified: Tue, 04 Aug 2020 23:21:49 GMT  
		Size: 1.4 MB (1419232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3cef38785c27cc0ccfd16a582f888fa88b0a31e390a0b99b432478370b176e4`  
		Last Modified: Tue, 04 Aug 2020 23:21:49 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:894f9792565ae2b3bbf93a31e6370772714c1a63d40b5636bb1a8c8491e564fb`  
		Last Modified: Tue, 04 Aug 2020 23:21:53 GMT  
		Size: 13.4 MB (13446959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d8a57523420f36ec3d5a5fff355c7b1424481c745e2a88eb5cffd9ff340c835`  
		Last Modified: Tue, 04 Aug 2020 23:21:48 GMT  
		Size: 2.4 KB (2388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f09bf1d31c1ccc04b380ab4dbe9d709958e8e6e1426ad0a37b3167c3a202f10`  
		Last Modified: Tue, 04 Aug 2020 23:22:18 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b6ff254abe738cfb27e4ee7ce6b41d6602d30dc212d5991ef27b5b308a1f516`  
		Last Modified: Tue, 04 Aug 2020 23:22:39 GMT  
		Size: 108.3 MB (108328095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74310a0bf42d0339c4034fb2565df7c3d71defeff25865e254edaaf3a0592b78`  
		Last Modified: Tue, 04 Aug 2020 23:22:18 GMT  
		Size: 5.1 KB (5146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d398726627fd8783de92c0559d7898852523d524f5c204eb92ef2b7bfcdacea1`  
		Last Modified: Tue, 04 Aug 2020 23:22:18 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.6`

```console
$ docker pull mysql@sha256:857113744fa24df5837dacc9786dae9c7a3d4913ac5cdfcf6ce1016e5b226e12
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mysql:5.6` - linux; amd64

```console
$ docker pull mysql@sha256:41a78a6be57572d8fb09558775e34b487ea2cfd9355fc78b106d5fa9e0bf115c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.9 MB (102930004 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d3d3845393d685eed9321927f1b026ba1bfdfe618d2494e708003efb437c685`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 04 Aug 2020 15:45:49 GMT
ADD file:16a1ddc40c95b14f8d6c79795047776270ee399f36979aaca45978a67bfee134 in / 
# Tue, 04 Aug 2020 15:45:49 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 23:20:48 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 04 Aug 2020 23:20:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 23:20:54 GMT
ENV GOSU_VERSION=1.12
# Tue, 04 Aug 2020 23:21:06 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 04 Aug 2020 23:21:07 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 04 Aug 2020 23:21:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		pwgen 		perl 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 23:21:18 GMT
RUN set -ex; 	key='A4A9406876FCBD3C456770C88C718D3B5072E1F5'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list > /dev/null
# Tue, 04 Aug 2020 23:21:18 GMT
ENV MYSQL_MAJOR=5.6
# Tue, 04 Aug 2020 23:21:18 GMT
ENV MYSQL_VERSION=5.6.49-1debian9
# Tue, 04 Aug 2020 23:21:19 GMT
RUN echo "deb http://repo.mysql.com/apt/debian/ stretch mysql-${MYSQL_MAJOR}" > /etc/apt/sources.list.d/mysql.list
# Tue, 04 Aug 2020 23:21:36 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update && apt-get install -y mysql-server="${MYSQL_VERSION}" && rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 777 /var/run/mysqld 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Tue, 04 Aug 2020 23:21:36 GMT
VOLUME [/var/lib/mysql]
# Tue, 04 Aug 2020 23:21:36 GMT
COPY file:7cbb26bbdb8e71b36aafda38dbac08caa641714a19991b86cde77daf3286ec11 in /usr/local/bin/ 
# Tue, 04 Aug 2020 23:21:37 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 04 Aug 2020 23:21:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Aug 2020 23:21:37 GMT
EXPOSE 3306
# Tue, 04 Aug 2020 23:21:38 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:75cb2ebf3b3cb9c601a22edc7d9a120749da33999b30fba22b6cf2b90ee92823`  
		Last Modified: Tue, 04 Aug 2020 15:52:18 GMT  
		Size: 22.5 MB (22522276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fdc75a292689e27cc814ddfee710b59b82ddac5b27532ba541cec812670aa2c`  
		Last Modified: Tue, 04 Aug 2020 23:22:46 GMT  
		Size: 1.7 KB (1745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ba1844b09a58316ebab76519983bfe7b01779de739fad9cc7ba5af68330c05a`  
		Last Modified: Tue, 04 Aug 2020 23:22:46 GMT  
		Size: 4.5 MB (4502039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8927406e4559511f9783afdbb512ec12329112e63cda5eafe1200fefb53ba9f4`  
		Last Modified: Tue, 04 Aug 2020 23:22:45 GMT  
		Size: 1.4 MB (1412097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41f2a683960c2eb8b4c29ec450b1dcd7eb66232bd0dca67832aeb5ca217bd82c`  
		Last Modified: Tue, 04 Aug 2020 23:22:45 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fe760d556adc88adfb6878448473d9b9889648bfb2b916093fb5d213b610fba`  
		Last Modified: Tue, 04 Aug 2020 23:22:48 GMT  
		Size: 10.2 MB (10224930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ded99153be233624ef4cb4fc93c93d3bd71af690724e46ecd5efc42da1aa1f2e`  
		Last Modified: Tue, 04 Aug 2020 23:22:44 GMT  
		Size: 28.3 KB (28325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f80b2192fcccd55ea8a1e07609884d4fe4999899f995ba8f2c30fe186cb4000`  
		Last Modified: Tue, 04 Aug 2020 23:22:44 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caa61e980546c2df04c4c7ef70abd591f5b0f63c91011c59642701945221883f`  
		Last Modified: Tue, 04 Aug 2020 23:22:58 GMT  
		Size: 64.2 MB (64232971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d5c4dc713afb0904ebfcfc615943f14915f006389f6f65a1ea6825639763a99`  
		Last Modified: Tue, 04 Aug 2020 23:22:44 GMT  
		Size: 5.2 KB (5159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cada58ccc6268c3a354c5f32d728f51ff0175665e1a389d11a25f1a4aef5c451`  
		Last Modified: Tue, 04 Aug 2020 23:22:44 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.6.49`

```console
$ docker pull mysql@sha256:857113744fa24df5837dacc9786dae9c7a3d4913ac5cdfcf6ce1016e5b226e12
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mysql:5.6.49` - linux; amd64

```console
$ docker pull mysql@sha256:41a78a6be57572d8fb09558775e34b487ea2cfd9355fc78b106d5fa9e0bf115c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.9 MB (102930004 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d3d3845393d685eed9321927f1b026ba1bfdfe618d2494e708003efb437c685`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 04 Aug 2020 15:45:49 GMT
ADD file:16a1ddc40c95b14f8d6c79795047776270ee399f36979aaca45978a67bfee134 in / 
# Tue, 04 Aug 2020 15:45:49 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 23:20:48 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 04 Aug 2020 23:20:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 23:20:54 GMT
ENV GOSU_VERSION=1.12
# Tue, 04 Aug 2020 23:21:06 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 04 Aug 2020 23:21:07 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 04 Aug 2020 23:21:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		pwgen 		perl 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 23:21:18 GMT
RUN set -ex; 	key='A4A9406876FCBD3C456770C88C718D3B5072E1F5'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list > /dev/null
# Tue, 04 Aug 2020 23:21:18 GMT
ENV MYSQL_MAJOR=5.6
# Tue, 04 Aug 2020 23:21:18 GMT
ENV MYSQL_VERSION=5.6.49-1debian9
# Tue, 04 Aug 2020 23:21:19 GMT
RUN echo "deb http://repo.mysql.com/apt/debian/ stretch mysql-${MYSQL_MAJOR}" > /etc/apt/sources.list.d/mysql.list
# Tue, 04 Aug 2020 23:21:36 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update && apt-get install -y mysql-server="${MYSQL_VERSION}" && rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 777 /var/run/mysqld 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Tue, 04 Aug 2020 23:21:36 GMT
VOLUME [/var/lib/mysql]
# Tue, 04 Aug 2020 23:21:36 GMT
COPY file:7cbb26bbdb8e71b36aafda38dbac08caa641714a19991b86cde77daf3286ec11 in /usr/local/bin/ 
# Tue, 04 Aug 2020 23:21:37 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 04 Aug 2020 23:21:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Aug 2020 23:21:37 GMT
EXPOSE 3306
# Tue, 04 Aug 2020 23:21:38 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:75cb2ebf3b3cb9c601a22edc7d9a120749da33999b30fba22b6cf2b90ee92823`  
		Last Modified: Tue, 04 Aug 2020 15:52:18 GMT  
		Size: 22.5 MB (22522276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fdc75a292689e27cc814ddfee710b59b82ddac5b27532ba541cec812670aa2c`  
		Last Modified: Tue, 04 Aug 2020 23:22:46 GMT  
		Size: 1.7 KB (1745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ba1844b09a58316ebab76519983bfe7b01779de739fad9cc7ba5af68330c05a`  
		Last Modified: Tue, 04 Aug 2020 23:22:46 GMT  
		Size: 4.5 MB (4502039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8927406e4559511f9783afdbb512ec12329112e63cda5eafe1200fefb53ba9f4`  
		Last Modified: Tue, 04 Aug 2020 23:22:45 GMT  
		Size: 1.4 MB (1412097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41f2a683960c2eb8b4c29ec450b1dcd7eb66232bd0dca67832aeb5ca217bd82c`  
		Last Modified: Tue, 04 Aug 2020 23:22:45 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fe760d556adc88adfb6878448473d9b9889648bfb2b916093fb5d213b610fba`  
		Last Modified: Tue, 04 Aug 2020 23:22:48 GMT  
		Size: 10.2 MB (10224930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ded99153be233624ef4cb4fc93c93d3bd71af690724e46ecd5efc42da1aa1f2e`  
		Last Modified: Tue, 04 Aug 2020 23:22:44 GMT  
		Size: 28.3 KB (28325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f80b2192fcccd55ea8a1e07609884d4fe4999899f995ba8f2c30fe186cb4000`  
		Last Modified: Tue, 04 Aug 2020 23:22:44 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caa61e980546c2df04c4c7ef70abd591f5b0f63c91011c59642701945221883f`  
		Last Modified: Tue, 04 Aug 2020 23:22:58 GMT  
		Size: 64.2 MB (64232971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d5c4dc713afb0904ebfcfc615943f14915f006389f6f65a1ea6825639763a99`  
		Last Modified: Tue, 04 Aug 2020 23:22:44 GMT  
		Size: 5.2 KB (5159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cada58ccc6268c3a354c5f32d728f51ff0175665e1a389d11a25f1a4aef5c451`  
		Last Modified: Tue, 04 Aug 2020 23:22:44 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7`

```console
$ docker pull mysql@sha256:da58f943b94721d46e87d5de208dc07302a8b13e638cd1d24285d222376d6d84
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mysql:5.7` - linux; amd64

```console
$ docker pull mysql@sha256:d3418a353847c7b34e3b082d1ea35a9d12fd1244d3d841d8cfe076e72c216b00
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.5 MB (154474259 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:718a6da099d82183c064a964523c0deca80619cb033aadd15854771fe592a480`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 04 Aug 2020 15:42:51 GMT
ADD file:3af3091e7d2bb40bc1e6550eb5ea290badc6bbf3339105626f245a963cc11450 in / 
# Tue, 04 Aug 2020 15:42:51 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 23:19:19 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 04 Aug 2020 23:19:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 23:19:26 GMT
ENV GOSU_VERSION=1.12
# Tue, 04 Aug 2020 23:19:34 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 04 Aug 2020 23:19:35 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 04 Aug 2020 23:19:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		pwgen 		openssl 		perl 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 23:19:45 GMT
RUN set -ex; 	key='A4A9406876FCBD3C456770C88C718D3B5072E1F5'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list > /dev/null
# Tue, 04 Aug 2020 23:20:14 GMT
ENV MYSQL_MAJOR=5.7
# Tue, 04 Aug 2020 23:20:14 GMT
ENV MYSQL_VERSION=5.7.31-1debian10
# Tue, 04 Aug 2020 23:20:15 GMT
RUN echo "deb http://repo.mysql.com/apt/debian/ buster mysql-${MYSQL_MAJOR}" > /etc/apt/sources.list.d/mysql.list
# Tue, 04 Aug 2020 23:20:38 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update && apt-get install -y mysql-server="${MYSQL_VERSION}" && rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 777 /var/run/mysqld 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Tue, 04 Aug 2020 23:20:38 GMT
VOLUME [/var/lib/mysql]
# Tue, 04 Aug 2020 23:20:39 GMT
COPY file:7cbb26bbdb8e71b36aafda38dbac08caa641714a19991b86cde77daf3286ec11 in /usr/local/bin/ 
# Tue, 04 Aug 2020 23:20:39 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 04 Aug 2020 23:20:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Aug 2020 23:20:40 GMT
EXPOSE 3306 33060
# Tue, 04 Aug 2020 23:20:40 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:bf59529304463f62efa7179fa1a32718a611528cc4ce9f30c0d1bbc6724ec3fb`  
		Last Modified: Tue, 04 Aug 2020 15:49:09 GMT  
		Size: 27.1 MB (27092121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8254623a9871b825936fce675bd714b26e4291b14f382b88d36ae9d85e304ed4`  
		Last Modified: Tue, 04 Aug 2020 23:21:49 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:938e3e06dac451f904a36d49c72fb11a2366176eb3b9bd7e8a71153028a9cfd3`  
		Last Modified: Tue, 04 Aug 2020 23:21:51 GMT  
		Size: 4.2 MB (4178123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea28ebf28884e64ac7e9d560727639795015425e5ea74f69a2101f6e16a43826`  
		Last Modified: Tue, 04 Aug 2020 23:21:49 GMT  
		Size: 1.4 MB (1419232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3cef38785c27cc0ccfd16a582f888fa88b0a31e390a0b99b432478370b176e4`  
		Last Modified: Tue, 04 Aug 2020 23:21:49 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:894f9792565ae2b3bbf93a31e6370772714c1a63d40b5636bb1a8c8491e564fb`  
		Last Modified: Tue, 04 Aug 2020 23:21:53 GMT  
		Size: 13.4 MB (13446959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d8a57523420f36ec3d5a5fff355c7b1424481c745e2a88eb5cffd9ff340c835`  
		Last Modified: Tue, 04 Aug 2020 23:21:48 GMT  
		Size: 2.4 KB (2388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f09bf1d31c1ccc04b380ab4dbe9d709958e8e6e1426ad0a37b3167c3a202f10`  
		Last Modified: Tue, 04 Aug 2020 23:22:18 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b6ff254abe738cfb27e4ee7ce6b41d6602d30dc212d5991ef27b5b308a1f516`  
		Last Modified: Tue, 04 Aug 2020 23:22:39 GMT  
		Size: 108.3 MB (108328095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74310a0bf42d0339c4034fb2565df7c3d71defeff25865e254edaaf3a0592b78`  
		Last Modified: Tue, 04 Aug 2020 23:22:18 GMT  
		Size: 5.1 KB (5146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d398726627fd8783de92c0559d7898852523d524f5c204eb92ef2b7bfcdacea1`  
		Last Modified: Tue, 04 Aug 2020 23:22:18 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7.31`

```console
$ docker pull mysql@sha256:da58f943b94721d46e87d5de208dc07302a8b13e638cd1d24285d222376d6d84
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mysql:5.7.31` - linux; amd64

```console
$ docker pull mysql@sha256:d3418a353847c7b34e3b082d1ea35a9d12fd1244d3d841d8cfe076e72c216b00
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.5 MB (154474259 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:718a6da099d82183c064a964523c0deca80619cb033aadd15854771fe592a480`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 04 Aug 2020 15:42:51 GMT
ADD file:3af3091e7d2bb40bc1e6550eb5ea290badc6bbf3339105626f245a963cc11450 in / 
# Tue, 04 Aug 2020 15:42:51 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 23:19:19 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 04 Aug 2020 23:19:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 23:19:26 GMT
ENV GOSU_VERSION=1.12
# Tue, 04 Aug 2020 23:19:34 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 04 Aug 2020 23:19:35 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 04 Aug 2020 23:19:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		pwgen 		openssl 		perl 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 23:19:45 GMT
RUN set -ex; 	key='A4A9406876FCBD3C456770C88C718D3B5072E1F5'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list > /dev/null
# Tue, 04 Aug 2020 23:20:14 GMT
ENV MYSQL_MAJOR=5.7
# Tue, 04 Aug 2020 23:20:14 GMT
ENV MYSQL_VERSION=5.7.31-1debian10
# Tue, 04 Aug 2020 23:20:15 GMT
RUN echo "deb http://repo.mysql.com/apt/debian/ buster mysql-${MYSQL_MAJOR}" > /etc/apt/sources.list.d/mysql.list
# Tue, 04 Aug 2020 23:20:38 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update && apt-get install -y mysql-server="${MYSQL_VERSION}" && rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 777 /var/run/mysqld 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf
# Tue, 04 Aug 2020 23:20:38 GMT
VOLUME [/var/lib/mysql]
# Tue, 04 Aug 2020 23:20:39 GMT
COPY file:7cbb26bbdb8e71b36aafda38dbac08caa641714a19991b86cde77daf3286ec11 in /usr/local/bin/ 
# Tue, 04 Aug 2020 23:20:39 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 04 Aug 2020 23:20:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Aug 2020 23:20:40 GMT
EXPOSE 3306 33060
# Tue, 04 Aug 2020 23:20:40 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:bf59529304463f62efa7179fa1a32718a611528cc4ce9f30c0d1bbc6724ec3fb`  
		Last Modified: Tue, 04 Aug 2020 15:49:09 GMT  
		Size: 27.1 MB (27092121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8254623a9871b825936fce675bd714b26e4291b14f382b88d36ae9d85e304ed4`  
		Last Modified: Tue, 04 Aug 2020 23:21:49 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:938e3e06dac451f904a36d49c72fb11a2366176eb3b9bd7e8a71153028a9cfd3`  
		Last Modified: Tue, 04 Aug 2020 23:21:51 GMT  
		Size: 4.2 MB (4178123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea28ebf28884e64ac7e9d560727639795015425e5ea74f69a2101f6e16a43826`  
		Last Modified: Tue, 04 Aug 2020 23:21:49 GMT  
		Size: 1.4 MB (1419232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3cef38785c27cc0ccfd16a582f888fa88b0a31e390a0b99b432478370b176e4`  
		Last Modified: Tue, 04 Aug 2020 23:21:49 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:894f9792565ae2b3bbf93a31e6370772714c1a63d40b5636bb1a8c8491e564fb`  
		Last Modified: Tue, 04 Aug 2020 23:21:53 GMT  
		Size: 13.4 MB (13446959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d8a57523420f36ec3d5a5fff355c7b1424481c745e2a88eb5cffd9ff340c835`  
		Last Modified: Tue, 04 Aug 2020 23:21:48 GMT  
		Size: 2.4 KB (2388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f09bf1d31c1ccc04b380ab4dbe9d709958e8e6e1426ad0a37b3167c3a202f10`  
		Last Modified: Tue, 04 Aug 2020 23:22:18 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b6ff254abe738cfb27e4ee7ce6b41d6602d30dc212d5991ef27b5b308a1f516`  
		Last Modified: Tue, 04 Aug 2020 23:22:39 GMT  
		Size: 108.3 MB (108328095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74310a0bf42d0339c4034fb2565df7c3d71defeff25865e254edaaf3a0592b78`  
		Last Modified: Tue, 04 Aug 2020 23:22:18 GMT  
		Size: 5.1 KB (5146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d398726627fd8783de92c0559d7898852523d524f5c204eb92ef2b7bfcdacea1`  
		Last Modified: Tue, 04 Aug 2020 23:22:18 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8`

```console
$ docker pull mysql@sha256:c358e72e100ab493a0304bda35e6f239db2ec8c9bb836d8a427ac34307d074ed
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mysql:8` - linux; amd64

```console
$ docker pull mysql@sha256:5f7620b5dfa7982adb8127e047b3ade838b9621487f085bc3c004f8387cfe14d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **158.6 MB (158633211 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d64f46acfd1af4ee6a162f80c6e07e843761bf14d412060023bf0e69e720fb4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 04 Aug 2020 15:42:51 GMT
ADD file:3af3091e7d2bb40bc1e6550eb5ea290badc6bbf3339105626f245a963cc11450 in / 
# Tue, 04 Aug 2020 15:42:51 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 23:19:19 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 04 Aug 2020 23:19:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 23:19:26 GMT
ENV GOSU_VERSION=1.12
# Tue, 04 Aug 2020 23:19:34 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 04 Aug 2020 23:19:35 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 04 Aug 2020 23:19:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		pwgen 		openssl 		perl 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 23:19:45 GMT
RUN set -ex; 	key='A4A9406876FCBD3C456770C88C718D3B5072E1F5'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list > /dev/null
# Tue, 04 Aug 2020 23:19:45 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 04 Aug 2020 23:19:45 GMT
ENV MYSQL_VERSION=8.0.21-1debian10
# Tue, 04 Aug 2020 23:19:46 GMT
RUN echo "deb http://repo.mysql.com/apt/debian/ buster mysql-${MYSQL_MAJOR}" > /etc/apt/sources.list.d/mysql.list
# Tue, 04 Aug 2020 23:20:02 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update && apt-get install -y mysql-community-client="${MYSQL_VERSION}" mysql-community-server-core="${MYSQL_VERSION}" && rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 777 /var/run/mysqld
# Tue, 04 Aug 2020 23:20:02 GMT
VOLUME [/var/lib/mysql]
# Tue, 04 Aug 2020 23:20:02 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Tue, 04 Aug 2020 23:20:03 GMT
COPY file:7cbb26bbdb8e71b36aafda38dbac08caa641714a19991b86cde77daf3286ec11 in /usr/local/bin/ 
# Tue, 04 Aug 2020 23:20:04 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 04 Aug 2020 23:20:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Aug 2020 23:20:04 GMT
EXPOSE 3306 33060
# Tue, 04 Aug 2020 23:20:04 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:bf59529304463f62efa7179fa1a32718a611528cc4ce9f30c0d1bbc6724ec3fb`  
		Last Modified: Tue, 04 Aug 2020 15:49:09 GMT  
		Size: 27.1 MB (27092121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8254623a9871b825936fce675bd714b26e4291b14f382b88d36ae9d85e304ed4`  
		Last Modified: Tue, 04 Aug 2020 23:21:49 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:938e3e06dac451f904a36d49c72fb11a2366176eb3b9bd7e8a71153028a9cfd3`  
		Last Modified: Tue, 04 Aug 2020 23:21:51 GMT  
		Size: 4.2 MB (4178123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea28ebf28884e64ac7e9d560727639795015425e5ea74f69a2101f6e16a43826`  
		Last Modified: Tue, 04 Aug 2020 23:21:49 GMT  
		Size: 1.4 MB (1419232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3cef38785c27cc0ccfd16a582f888fa88b0a31e390a0b99b432478370b176e4`  
		Last Modified: Tue, 04 Aug 2020 23:21:49 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:894f9792565ae2b3bbf93a31e6370772714c1a63d40b5636bb1a8c8491e564fb`  
		Last Modified: Tue, 04 Aug 2020 23:21:53 GMT  
		Size: 13.4 MB (13446959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d8a57523420f36ec3d5a5fff355c7b1424481c745e2a88eb5cffd9ff340c835`  
		Last Modified: Tue, 04 Aug 2020 23:21:48 GMT  
		Size: 2.4 KB (2388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c676912929ff9a4e5de0447f551251488ed2e45d3490ac396a5226c7508093b`  
		Last Modified: Tue, 04 Aug 2020 23:21:48 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff39fdb566b404b45698e49c4715854df72ec79dc1ea82d927e1225cb6fcd9fc`  
		Last Modified: Tue, 04 Aug 2020 23:22:12 GMT  
		Size: 112.5 MB (112486199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fff872988abad185b4016457f19fe136c31f862c5eb983a539bede3a181a9468`  
		Last Modified: Tue, 04 Aug 2020 23:21:47 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d34e365ae6873ddeca72598974553f5825b05831164d8574fd888faf021e40b`  
		Last Modified: Tue, 04 Aug 2020 23:21:47 GMT  
		Size: 5.1 KB (5147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7886ee20621e64f2ef86225ba06d16ccede5dd283939ea6959ca30b03e13460b`  
		Last Modified: Tue, 04 Aug 2020 23:21:48 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0`

```console
$ docker pull mysql@sha256:c358e72e100ab493a0304bda35e6f239db2ec8c9bb836d8a427ac34307d074ed
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mysql:8.0` - linux; amd64

```console
$ docker pull mysql@sha256:5f7620b5dfa7982adb8127e047b3ade838b9621487f085bc3c004f8387cfe14d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **158.6 MB (158633211 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d64f46acfd1af4ee6a162f80c6e07e843761bf14d412060023bf0e69e720fb4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 04 Aug 2020 15:42:51 GMT
ADD file:3af3091e7d2bb40bc1e6550eb5ea290badc6bbf3339105626f245a963cc11450 in / 
# Tue, 04 Aug 2020 15:42:51 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 23:19:19 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 04 Aug 2020 23:19:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 23:19:26 GMT
ENV GOSU_VERSION=1.12
# Tue, 04 Aug 2020 23:19:34 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 04 Aug 2020 23:19:35 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 04 Aug 2020 23:19:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		pwgen 		openssl 		perl 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 23:19:45 GMT
RUN set -ex; 	key='A4A9406876FCBD3C456770C88C718D3B5072E1F5'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list > /dev/null
# Tue, 04 Aug 2020 23:19:45 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 04 Aug 2020 23:19:45 GMT
ENV MYSQL_VERSION=8.0.21-1debian10
# Tue, 04 Aug 2020 23:19:46 GMT
RUN echo "deb http://repo.mysql.com/apt/debian/ buster mysql-${MYSQL_MAJOR}" > /etc/apt/sources.list.d/mysql.list
# Tue, 04 Aug 2020 23:20:02 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update && apt-get install -y mysql-community-client="${MYSQL_VERSION}" mysql-community-server-core="${MYSQL_VERSION}" && rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 777 /var/run/mysqld
# Tue, 04 Aug 2020 23:20:02 GMT
VOLUME [/var/lib/mysql]
# Tue, 04 Aug 2020 23:20:02 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Tue, 04 Aug 2020 23:20:03 GMT
COPY file:7cbb26bbdb8e71b36aafda38dbac08caa641714a19991b86cde77daf3286ec11 in /usr/local/bin/ 
# Tue, 04 Aug 2020 23:20:04 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 04 Aug 2020 23:20:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Aug 2020 23:20:04 GMT
EXPOSE 3306 33060
# Tue, 04 Aug 2020 23:20:04 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:bf59529304463f62efa7179fa1a32718a611528cc4ce9f30c0d1bbc6724ec3fb`  
		Last Modified: Tue, 04 Aug 2020 15:49:09 GMT  
		Size: 27.1 MB (27092121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8254623a9871b825936fce675bd714b26e4291b14f382b88d36ae9d85e304ed4`  
		Last Modified: Tue, 04 Aug 2020 23:21:49 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:938e3e06dac451f904a36d49c72fb11a2366176eb3b9bd7e8a71153028a9cfd3`  
		Last Modified: Tue, 04 Aug 2020 23:21:51 GMT  
		Size: 4.2 MB (4178123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea28ebf28884e64ac7e9d560727639795015425e5ea74f69a2101f6e16a43826`  
		Last Modified: Tue, 04 Aug 2020 23:21:49 GMT  
		Size: 1.4 MB (1419232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3cef38785c27cc0ccfd16a582f888fa88b0a31e390a0b99b432478370b176e4`  
		Last Modified: Tue, 04 Aug 2020 23:21:49 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:894f9792565ae2b3bbf93a31e6370772714c1a63d40b5636bb1a8c8491e564fb`  
		Last Modified: Tue, 04 Aug 2020 23:21:53 GMT  
		Size: 13.4 MB (13446959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d8a57523420f36ec3d5a5fff355c7b1424481c745e2a88eb5cffd9ff340c835`  
		Last Modified: Tue, 04 Aug 2020 23:21:48 GMT  
		Size: 2.4 KB (2388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c676912929ff9a4e5de0447f551251488ed2e45d3490ac396a5226c7508093b`  
		Last Modified: Tue, 04 Aug 2020 23:21:48 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff39fdb566b404b45698e49c4715854df72ec79dc1ea82d927e1225cb6fcd9fc`  
		Last Modified: Tue, 04 Aug 2020 23:22:12 GMT  
		Size: 112.5 MB (112486199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fff872988abad185b4016457f19fe136c31f862c5eb983a539bede3a181a9468`  
		Last Modified: Tue, 04 Aug 2020 23:21:47 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d34e365ae6873ddeca72598974553f5825b05831164d8574fd888faf021e40b`  
		Last Modified: Tue, 04 Aug 2020 23:21:47 GMT  
		Size: 5.1 KB (5147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7886ee20621e64f2ef86225ba06d16ccede5dd283939ea6959ca30b03e13460b`  
		Last Modified: Tue, 04 Aug 2020 23:21:48 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0.21`

```console
$ docker pull mysql@sha256:c358e72e100ab493a0304bda35e6f239db2ec8c9bb836d8a427ac34307d074ed
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mysql:8.0.21` - linux; amd64

```console
$ docker pull mysql@sha256:5f7620b5dfa7982adb8127e047b3ade838b9621487f085bc3c004f8387cfe14d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **158.6 MB (158633211 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d64f46acfd1af4ee6a162f80c6e07e843761bf14d412060023bf0e69e720fb4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 04 Aug 2020 15:42:51 GMT
ADD file:3af3091e7d2bb40bc1e6550eb5ea290badc6bbf3339105626f245a963cc11450 in / 
# Tue, 04 Aug 2020 15:42:51 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 23:19:19 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 04 Aug 2020 23:19:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 23:19:26 GMT
ENV GOSU_VERSION=1.12
# Tue, 04 Aug 2020 23:19:34 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 04 Aug 2020 23:19:35 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 04 Aug 2020 23:19:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		pwgen 		openssl 		perl 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 23:19:45 GMT
RUN set -ex; 	key='A4A9406876FCBD3C456770C88C718D3B5072E1F5'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list > /dev/null
# Tue, 04 Aug 2020 23:19:45 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 04 Aug 2020 23:19:45 GMT
ENV MYSQL_VERSION=8.0.21-1debian10
# Tue, 04 Aug 2020 23:19:46 GMT
RUN echo "deb http://repo.mysql.com/apt/debian/ buster mysql-${MYSQL_MAJOR}" > /etc/apt/sources.list.d/mysql.list
# Tue, 04 Aug 2020 23:20:02 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update && apt-get install -y mysql-community-client="${MYSQL_VERSION}" mysql-community-server-core="${MYSQL_VERSION}" && rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 777 /var/run/mysqld
# Tue, 04 Aug 2020 23:20:02 GMT
VOLUME [/var/lib/mysql]
# Tue, 04 Aug 2020 23:20:02 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Tue, 04 Aug 2020 23:20:03 GMT
COPY file:7cbb26bbdb8e71b36aafda38dbac08caa641714a19991b86cde77daf3286ec11 in /usr/local/bin/ 
# Tue, 04 Aug 2020 23:20:04 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 04 Aug 2020 23:20:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Aug 2020 23:20:04 GMT
EXPOSE 3306 33060
# Tue, 04 Aug 2020 23:20:04 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:bf59529304463f62efa7179fa1a32718a611528cc4ce9f30c0d1bbc6724ec3fb`  
		Last Modified: Tue, 04 Aug 2020 15:49:09 GMT  
		Size: 27.1 MB (27092121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8254623a9871b825936fce675bd714b26e4291b14f382b88d36ae9d85e304ed4`  
		Last Modified: Tue, 04 Aug 2020 23:21:49 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:938e3e06dac451f904a36d49c72fb11a2366176eb3b9bd7e8a71153028a9cfd3`  
		Last Modified: Tue, 04 Aug 2020 23:21:51 GMT  
		Size: 4.2 MB (4178123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea28ebf28884e64ac7e9d560727639795015425e5ea74f69a2101f6e16a43826`  
		Last Modified: Tue, 04 Aug 2020 23:21:49 GMT  
		Size: 1.4 MB (1419232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3cef38785c27cc0ccfd16a582f888fa88b0a31e390a0b99b432478370b176e4`  
		Last Modified: Tue, 04 Aug 2020 23:21:49 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:894f9792565ae2b3bbf93a31e6370772714c1a63d40b5636bb1a8c8491e564fb`  
		Last Modified: Tue, 04 Aug 2020 23:21:53 GMT  
		Size: 13.4 MB (13446959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d8a57523420f36ec3d5a5fff355c7b1424481c745e2a88eb5cffd9ff340c835`  
		Last Modified: Tue, 04 Aug 2020 23:21:48 GMT  
		Size: 2.4 KB (2388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c676912929ff9a4e5de0447f551251488ed2e45d3490ac396a5226c7508093b`  
		Last Modified: Tue, 04 Aug 2020 23:21:48 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff39fdb566b404b45698e49c4715854df72ec79dc1ea82d927e1225cb6fcd9fc`  
		Last Modified: Tue, 04 Aug 2020 23:22:12 GMT  
		Size: 112.5 MB (112486199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fff872988abad185b4016457f19fe136c31f862c5eb983a539bede3a181a9468`  
		Last Modified: Tue, 04 Aug 2020 23:21:47 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d34e365ae6873ddeca72598974553f5825b05831164d8574fd888faf021e40b`  
		Last Modified: Tue, 04 Aug 2020 23:21:47 GMT  
		Size: 5.1 KB (5147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7886ee20621e64f2ef86225ba06d16ccede5dd283939ea6959ca30b03e13460b`  
		Last Modified: Tue, 04 Aug 2020 23:21:48 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:latest`

```console
$ docker pull mysql@sha256:c358e72e100ab493a0304bda35e6f239db2ec8c9bb836d8a427ac34307d074ed
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mysql:latest` - linux; amd64

```console
$ docker pull mysql@sha256:5f7620b5dfa7982adb8127e047b3ade838b9621487f085bc3c004f8387cfe14d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **158.6 MB (158633211 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d64f46acfd1af4ee6a162f80c6e07e843761bf14d412060023bf0e69e720fb4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 04 Aug 2020 15:42:51 GMT
ADD file:3af3091e7d2bb40bc1e6550eb5ea290badc6bbf3339105626f245a963cc11450 in / 
# Tue, 04 Aug 2020 15:42:51 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 23:19:19 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 04 Aug 2020 23:19:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 23:19:26 GMT
ENV GOSU_VERSION=1.12
# Tue, 04 Aug 2020 23:19:34 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 04 Aug 2020 23:19:35 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 04 Aug 2020 23:19:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		pwgen 		openssl 		perl 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 23:19:45 GMT
RUN set -ex; 	key='A4A9406876FCBD3C456770C88C718D3B5072E1F5'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list > /dev/null
# Tue, 04 Aug 2020 23:19:45 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 04 Aug 2020 23:19:45 GMT
ENV MYSQL_VERSION=8.0.21-1debian10
# Tue, 04 Aug 2020 23:19:46 GMT
RUN echo "deb http://repo.mysql.com/apt/debian/ buster mysql-${MYSQL_MAJOR}" > /etc/apt/sources.list.d/mysql.list
# Tue, 04 Aug 2020 23:20:02 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update && apt-get install -y mysql-community-client="${MYSQL_VERSION}" mysql-community-server-core="${MYSQL_VERSION}" && rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 777 /var/run/mysqld
# Tue, 04 Aug 2020 23:20:02 GMT
VOLUME [/var/lib/mysql]
# Tue, 04 Aug 2020 23:20:02 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Tue, 04 Aug 2020 23:20:03 GMT
COPY file:7cbb26bbdb8e71b36aafda38dbac08caa641714a19991b86cde77daf3286ec11 in /usr/local/bin/ 
# Tue, 04 Aug 2020 23:20:04 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 04 Aug 2020 23:20:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Aug 2020 23:20:04 GMT
EXPOSE 3306 33060
# Tue, 04 Aug 2020 23:20:04 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:bf59529304463f62efa7179fa1a32718a611528cc4ce9f30c0d1bbc6724ec3fb`  
		Last Modified: Tue, 04 Aug 2020 15:49:09 GMT  
		Size: 27.1 MB (27092121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8254623a9871b825936fce675bd714b26e4291b14f382b88d36ae9d85e304ed4`  
		Last Modified: Tue, 04 Aug 2020 23:21:49 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:938e3e06dac451f904a36d49c72fb11a2366176eb3b9bd7e8a71153028a9cfd3`  
		Last Modified: Tue, 04 Aug 2020 23:21:51 GMT  
		Size: 4.2 MB (4178123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea28ebf28884e64ac7e9d560727639795015425e5ea74f69a2101f6e16a43826`  
		Last Modified: Tue, 04 Aug 2020 23:21:49 GMT  
		Size: 1.4 MB (1419232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3cef38785c27cc0ccfd16a582f888fa88b0a31e390a0b99b432478370b176e4`  
		Last Modified: Tue, 04 Aug 2020 23:21:49 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:894f9792565ae2b3bbf93a31e6370772714c1a63d40b5636bb1a8c8491e564fb`  
		Last Modified: Tue, 04 Aug 2020 23:21:53 GMT  
		Size: 13.4 MB (13446959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d8a57523420f36ec3d5a5fff355c7b1424481c745e2a88eb5cffd9ff340c835`  
		Last Modified: Tue, 04 Aug 2020 23:21:48 GMT  
		Size: 2.4 KB (2388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c676912929ff9a4e5de0447f551251488ed2e45d3490ac396a5226c7508093b`  
		Last Modified: Tue, 04 Aug 2020 23:21:48 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff39fdb566b404b45698e49c4715854df72ec79dc1ea82d927e1225cb6fcd9fc`  
		Last Modified: Tue, 04 Aug 2020 23:22:12 GMT  
		Size: 112.5 MB (112486199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fff872988abad185b4016457f19fe136c31f862c5eb983a539bede3a181a9468`  
		Last Modified: Tue, 04 Aug 2020 23:21:47 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d34e365ae6873ddeca72598974553f5825b05831164d8574fd888faf021e40b`  
		Last Modified: Tue, 04 Aug 2020 23:21:47 GMT  
		Size: 5.1 KB (5147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7886ee20621e64f2ef86225ba06d16ccede5dd283939ea6959ca30b03e13460b`  
		Last Modified: Tue, 04 Aug 2020 23:21:48 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
