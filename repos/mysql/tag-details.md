<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `mysql`

-	[`mysql:5`](#mysql5)
-	[`mysql:5-debian`](#mysql5-debian)
-	[`mysql:5-oracle`](#mysql5-oracle)
-	[`mysql:5.7`](#mysql57)
-	[`mysql:5.7-debian`](#mysql57-debian)
-	[`mysql:5.7-oracle`](#mysql57-oracle)
-	[`mysql:5.7.39`](#mysql5739)
-	[`mysql:5.7.39-debian`](#mysql5739-debian)
-	[`mysql:5.7.39-oracle`](#mysql5739-oracle)
-	[`mysql:8`](#mysql8)
-	[`mysql:8-debian`](#mysql8-debian)
-	[`mysql:8-oracle`](#mysql8-oracle)
-	[`mysql:8.0`](#mysql80)
-	[`mysql:8.0-debian`](#mysql80-debian)
-	[`mysql:8.0-oracle`](#mysql80-oracle)
-	[`mysql:8.0.30`](#mysql8030)
-	[`mysql:8.0.30-debian`](#mysql8030-debian)
-	[`mysql:8.0.30-oracle`](#mysql8030-oracle)
-	[`mysql:debian`](#mysqldebian)
-	[`mysql:latest`](#mysqllatest)
-	[`mysql:oracle`](#mysqloracle)

## `mysql:5`

```console
$ docker pull mysql@sha256:b3a86578a582617214477d91e47e850f9e18df0b5d1644fb2d96d91a340b8972
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5` - linux; amd64

```console
$ docker pull mysql@sha256:5ecf646122c4fcbda81983c9e93e81a011b0593c9c19fbfc55b48bd1c23bc790
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.4 MB (128373606 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3147495b3a5ce957dee2319099a8808c1418e0b0a2c82c9b2396c5fb4b688509`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 05 Jul 2022 22:20:58 GMT
ADD file:50fb7d83a9d57e5a0a6af5e5daf27e464ae8a28c196ce6bad6c254dfc1774cdd in / 
# Tue, 05 Jul 2022 22:20:58 GMT
CMD ["/bin/bash"]
# Wed, 13 Jul 2022 06:46:23 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 13 Jul 2022 06:46:23 GMT
ENV GOSU_VERSION=1.14
# Wed, 13 Jul 2022 06:46:26 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 13 Jul 2022 06:46:48 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False oracle-epel-release-el7; 	yum install -y --setopt=skip_missing_names_on_install=False 		bzip2 		gzip 		openssl 		xz 		zstd 	; 	yum clean all
# Wed, 13 Jul 2022 06:46:49 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 13 Jul 2022 06:46:49 GMT
ENV MYSQL_MAJOR=5.7
# Tue, 26 Jul 2022 23:28:50 GMT
ENV MYSQL_VERSION=5.7.39-1.el7
# Tue, 26 Jul 2022 23:28:51 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql5.7-server-minimal]'; 		echo 'name=MySQL 5.7 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-5.7-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Tue, 26 Jul 2022 23:29:09 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-community-server-minimal-$MYSQL_VERSION"; 	yum clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	{ echo '!includedir /etc/mysql/mysql.conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/mysql.conf.d; 		find /etc/my.cnf /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/'; 		mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Tue, 26 Jul 2022 23:29:10 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Tue, 26 Jul 2022 23:29:10 GMT
ENV MYSQL_SHELL_VERSION=8.0.30-1.el7
# Tue, 26 Jul 2022 23:29:31 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-shell-$MYSQL_SHELL_VERSION"; 	yum clean all; 		mysqlsh --version
# Tue, 26 Jul 2022 23:29:32 GMT
VOLUME [/var/lib/mysql]
# Tue, 26 Jul 2022 23:29:32 GMT
COPY file:d27cf504fa76fb5a4038020a01eaaf52723b17b751566119de311adacb043752 in /usr/local/bin/ 
# Tue, 26 Jul 2022 23:29:32 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 26 Jul 2022 23:29:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 26 Jul 2022 23:29:33 GMT
EXPOSE 3306 33060
# Tue, 26 Jul 2022 23:29:33 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:66fb3478003364657ac7751c40e41a135e02975f9459f652b1df23e3896b5fac`  
		Last Modified: Tue, 05 Jul 2022 22:22:18 GMT  
		Size: 48.8 MB (48762895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef4ccd63cdb4ccb21c25d292be05bf37ee54a40a0746acdfa962a45a29a08b51`  
		Last Modified: Wed, 13 Jul 2022 06:48:50 GMT  
		Size: 870.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f28a94c51f0d4090e9d6792e3ac48d318cc96056520dd0d7f6e6d2db851891`  
		Last Modified: Wed, 13 Jul 2022 06:48:50 GMT  
		Size: 930.2 KB (930231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7feea2a503b5e8b906b70f33abda7cc47dd30cb72363f804838831a48fdc8a74`  
		Last Modified: Wed, 13 Jul 2022 06:48:49 GMT  
		Size: 4.5 MB (4549473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71dd5852ecd934862db097d1380b3c2fe6471908610bbc2ac0b10f3daf59a183`  
		Last Modified: Wed, 13 Jul 2022 06:48:47 GMT  
		Size: 2.7 KB (2659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ff5c3b24fd570d47fbe75cbe51b9f8428d58446368bf07022c42c52d943a9bb`  
		Last Modified: Tue, 26 Jul 2022 23:31:41 GMT  
		Size: 336.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88a546386a618f1071083b0d9d357cceff83aa39db239224f71a97968e35fff2`  
		Last Modified: Tue, 26 Jul 2022 23:31:43 GMT  
		Size: 25.5 MB (25512706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65b18297cf83f401e9641ba48cc9948ea3593821b42cae5990bacffd230c5ae5`  
		Last Modified: Tue, 26 Jul 2022 23:31:39 GMT  
		Size: 319.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d64f23335fb87ecace32a157428c706c308e2b71a97f9038204e208cf838bea6`  
		Last Modified: Tue, 26 Jul 2022 23:31:48 GMT  
		Size: 48.6 MB (48608834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ba4171261fac245494f48f61a9a3392736658b7c31f707783b796d952008ebb`  
		Last Modified: Tue, 26 Jul 2022 23:31:39 GMT  
		Size: 5.2 KB (5162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96dcc6c8de93eee9106fbbff2915b00236e56b1bf820f724d87daae33cb57e8d`  
		Last Modified: Tue, 26 Jul 2022 23:31:39 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

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

## `mysql:5-oracle`

```console
$ docker pull mysql@sha256:b3a86578a582617214477d91e47e850f9e18df0b5d1644fb2d96d91a340b8972
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:5ecf646122c4fcbda81983c9e93e81a011b0593c9c19fbfc55b48bd1c23bc790
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.4 MB (128373606 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3147495b3a5ce957dee2319099a8808c1418e0b0a2c82c9b2396c5fb4b688509`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 05 Jul 2022 22:20:58 GMT
ADD file:50fb7d83a9d57e5a0a6af5e5daf27e464ae8a28c196ce6bad6c254dfc1774cdd in / 
# Tue, 05 Jul 2022 22:20:58 GMT
CMD ["/bin/bash"]
# Wed, 13 Jul 2022 06:46:23 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 13 Jul 2022 06:46:23 GMT
ENV GOSU_VERSION=1.14
# Wed, 13 Jul 2022 06:46:26 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 13 Jul 2022 06:46:48 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False oracle-epel-release-el7; 	yum install -y --setopt=skip_missing_names_on_install=False 		bzip2 		gzip 		openssl 		xz 		zstd 	; 	yum clean all
# Wed, 13 Jul 2022 06:46:49 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 13 Jul 2022 06:46:49 GMT
ENV MYSQL_MAJOR=5.7
# Tue, 26 Jul 2022 23:28:50 GMT
ENV MYSQL_VERSION=5.7.39-1.el7
# Tue, 26 Jul 2022 23:28:51 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql5.7-server-minimal]'; 		echo 'name=MySQL 5.7 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-5.7-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Tue, 26 Jul 2022 23:29:09 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-community-server-minimal-$MYSQL_VERSION"; 	yum clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	{ echo '!includedir /etc/mysql/mysql.conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/mysql.conf.d; 		find /etc/my.cnf /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/'; 		mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Tue, 26 Jul 2022 23:29:10 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Tue, 26 Jul 2022 23:29:10 GMT
ENV MYSQL_SHELL_VERSION=8.0.30-1.el7
# Tue, 26 Jul 2022 23:29:31 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-shell-$MYSQL_SHELL_VERSION"; 	yum clean all; 		mysqlsh --version
# Tue, 26 Jul 2022 23:29:32 GMT
VOLUME [/var/lib/mysql]
# Tue, 26 Jul 2022 23:29:32 GMT
COPY file:d27cf504fa76fb5a4038020a01eaaf52723b17b751566119de311adacb043752 in /usr/local/bin/ 
# Tue, 26 Jul 2022 23:29:32 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 26 Jul 2022 23:29:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 26 Jul 2022 23:29:33 GMT
EXPOSE 3306 33060
# Tue, 26 Jul 2022 23:29:33 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:66fb3478003364657ac7751c40e41a135e02975f9459f652b1df23e3896b5fac`  
		Last Modified: Tue, 05 Jul 2022 22:22:18 GMT  
		Size: 48.8 MB (48762895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef4ccd63cdb4ccb21c25d292be05bf37ee54a40a0746acdfa962a45a29a08b51`  
		Last Modified: Wed, 13 Jul 2022 06:48:50 GMT  
		Size: 870.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f28a94c51f0d4090e9d6792e3ac48d318cc96056520dd0d7f6e6d2db851891`  
		Last Modified: Wed, 13 Jul 2022 06:48:50 GMT  
		Size: 930.2 KB (930231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7feea2a503b5e8b906b70f33abda7cc47dd30cb72363f804838831a48fdc8a74`  
		Last Modified: Wed, 13 Jul 2022 06:48:49 GMT  
		Size: 4.5 MB (4549473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71dd5852ecd934862db097d1380b3c2fe6471908610bbc2ac0b10f3daf59a183`  
		Last Modified: Wed, 13 Jul 2022 06:48:47 GMT  
		Size: 2.7 KB (2659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ff5c3b24fd570d47fbe75cbe51b9f8428d58446368bf07022c42c52d943a9bb`  
		Last Modified: Tue, 26 Jul 2022 23:31:41 GMT  
		Size: 336.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88a546386a618f1071083b0d9d357cceff83aa39db239224f71a97968e35fff2`  
		Last Modified: Tue, 26 Jul 2022 23:31:43 GMT  
		Size: 25.5 MB (25512706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65b18297cf83f401e9641ba48cc9948ea3593821b42cae5990bacffd230c5ae5`  
		Last Modified: Tue, 26 Jul 2022 23:31:39 GMT  
		Size: 319.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d64f23335fb87ecace32a157428c706c308e2b71a97f9038204e208cf838bea6`  
		Last Modified: Tue, 26 Jul 2022 23:31:48 GMT  
		Size: 48.6 MB (48608834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ba4171261fac245494f48f61a9a3392736658b7c31f707783b796d952008ebb`  
		Last Modified: Tue, 26 Jul 2022 23:31:39 GMT  
		Size: 5.2 KB (5162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96dcc6c8de93eee9106fbbff2915b00236e56b1bf820f724d87daae33cb57e8d`  
		Last Modified: Tue, 26 Jul 2022 23:31:39 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7`

```console
$ docker pull mysql@sha256:b3a86578a582617214477d91e47e850f9e18df0b5d1644fb2d96d91a340b8972
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7` - linux; amd64

```console
$ docker pull mysql@sha256:5ecf646122c4fcbda81983c9e93e81a011b0593c9c19fbfc55b48bd1c23bc790
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.4 MB (128373606 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3147495b3a5ce957dee2319099a8808c1418e0b0a2c82c9b2396c5fb4b688509`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 05 Jul 2022 22:20:58 GMT
ADD file:50fb7d83a9d57e5a0a6af5e5daf27e464ae8a28c196ce6bad6c254dfc1774cdd in / 
# Tue, 05 Jul 2022 22:20:58 GMT
CMD ["/bin/bash"]
# Wed, 13 Jul 2022 06:46:23 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 13 Jul 2022 06:46:23 GMT
ENV GOSU_VERSION=1.14
# Wed, 13 Jul 2022 06:46:26 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 13 Jul 2022 06:46:48 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False oracle-epel-release-el7; 	yum install -y --setopt=skip_missing_names_on_install=False 		bzip2 		gzip 		openssl 		xz 		zstd 	; 	yum clean all
# Wed, 13 Jul 2022 06:46:49 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 13 Jul 2022 06:46:49 GMT
ENV MYSQL_MAJOR=5.7
# Tue, 26 Jul 2022 23:28:50 GMT
ENV MYSQL_VERSION=5.7.39-1.el7
# Tue, 26 Jul 2022 23:28:51 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql5.7-server-minimal]'; 		echo 'name=MySQL 5.7 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-5.7-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Tue, 26 Jul 2022 23:29:09 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-community-server-minimal-$MYSQL_VERSION"; 	yum clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	{ echo '!includedir /etc/mysql/mysql.conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/mysql.conf.d; 		find /etc/my.cnf /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/'; 		mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Tue, 26 Jul 2022 23:29:10 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Tue, 26 Jul 2022 23:29:10 GMT
ENV MYSQL_SHELL_VERSION=8.0.30-1.el7
# Tue, 26 Jul 2022 23:29:31 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-shell-$MYSQL_SHELL_VERSION"; 	yum clean all; 		mysqlsh --version
# Tue, 26 Jul 2022 23:29:32 GMT
VOLUME [/var/lib/mysql]
# Tue, 26 Jul 2022 23:29:32 GMT
COPY file:d27cf504fa76fb5a4038020a01eaaf52723b17b751566119de311adacb043752 in /usr/local/bin/ 
# Tue, 26 Jul 2022 23:29:32 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 26 Jul 2022 23:29:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 26 Jul 2022 23:29:33 GMT
EXPOSE 3306 33060
# Tue, 26 Jul 2022 23:29:33 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:66fb3478003364657ac7751c40e41a135e02975f9459f652b1df23e3896b5fac`  
		Last Modified: Tue, 05 Jul 2022 22:22:18 GMT  
		Size: 48.8 MB (48762895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef4ccd63cdb4ccb21c25d292be05bf37ee54a40a0746acdfa962a45a29a08b51`  
		Last Modified: Wed, 13 Jul 2022 06:48:50 GMT  
		Size: 870.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f28a94c51f0d4090e9d6792e3ac48d318cc96056520dd0d7f6e6d2db851891`  
		Last Modified: Wed, 13 Jul 2022 06:48:50 GMT  
		Size: 930.2 KB (930231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7feea2a503b5e8b906b70f33abda7cc47dd30cb72363f804838831a48fdc8a74`  
		Last Modified: Wed, 13 Jul 2022 06:48:49 GMT  
		Size: 4.5 MB (4549473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71dd5852ecd934862db097d1380b3c2fe6471908610bbc2ac0b10f3daf59a183`  
		Last Modified: Wed, 13 Jul 2022 06:48:47 GMT  
		Size: 2.7 KB (2659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ff5c3b24fd570d47fbe75cbe51b9f8428d58446368bf07022c42c52d943a9bb`  
		Last Modified: Tue, 26 Jul 2022 23:31:41 GMT  
		Size: 336.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88a546386a618f1071083b0d9d357cceff83aa39db239224f71a97968e35fff2`  
		Last Modified: Tue, 26 Jul 2022 23:31:43 GMT  
		Size: 25.5 MB (25512706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65b18297cf83f401e9641ba48cc9948ea3593821b42cae5990bacffd230c5ae5`  
		Last Modified: Tue, 26 Jul 2022 23:31:39 GMT  
		Size: 319.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d64f23335fb87ecace32a157428c706c308e2b71a97f9038204e208cf838bea6`  
		Last Modified: Tue, 26 Jul 2022 23:31:48 GMT  
		Size: 48.6 MB (48608834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ba4171261fac245494f48f61a9a3392736658b7c31f707783b796d952008ebb`  
		Last Modified: Tue, 26 Jul 2022 23:31:39 GMT  
		Size: 5.2 KB (5162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96dcc6c8de93eee9106fbbff2915b00236e56b1bf820f724d87daae33cb57e8d`  
		Last Modified: Tue, 26 Jul 2022 23:31:39 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7-debian`

```console
$ docker pull mysql@sha256:d150c2e5269349200254d3fddb6bb00b6d3f3b4f301c8b050193ce02235e2bd1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7-debian` - linux; amd64

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

## `mysql:5.7-oracle`

```console
$ docker pull mysql@sha256:b3a86578a582617214477d91e47e850f9e18df0b5d1644fb2d96d91a340b8972
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:5ecf646122c4fcbda81983c9e93e81a011b0593c9c19fbfc55b48bd1c23bc790
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.4 MB (128373606 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3147495b3a5ce957dee2319099a8808c1418e0b0a2c82c9b2396c5fb4b688509`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 05 Jul 2022 22:20:58 GMT
ADD file:50fb7d83a9d57e5a0a6af5e5daf27e464ae8a28c196ce6bad6c254dfc1774cdd in / 
# Tue, 05 Jul 2022 22:20:58 GMT
CMD ["/bin/bash"]
# Wed, 13 Jul 2022 06:46:23 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 13 Jul 2022 06:46:23 GMT
ENV GOSU_VERSION=1.14
# Wed, 13 Jul 2022 06:46:26 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 13 Jul 2022 06:46:48 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False oracle-epel-release-el7; 	yum install -y --setopt=skip_missing_names_on_install=False 		bzip2 		gzip 		openssl 		xz 		zstd 	; 	yum clean all
# Wed, 13 Jul 2022 06:46:49 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 13 Jul 2022 06:46:49 GMT
ENV MYSQL_MAJOR=5.7
# Tue, 26 Jul 2022 23:28:50 GMT
ENV MYSQL_VERSION=5.7.39-1.el7
# Tue, 26 Jul 2022 23:28:51 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql5.7-server-minimal]'; 		echo 'name=MySQL 5.7 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-5.7-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Tue, 26 Jul 2022 23:29:09 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-community-server-minimal-$MYSQL_VERSION"; 	yum clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	{ echo '!includedir /etc/mysql/mysql.conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/mysql.conf.d; 		find /etc/my.cnf /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/'; 		mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Tue, 26 Jul 2022 23:29:10 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Tue, 26 Jul 2022 23:29:10 GMT
ENV MYSQL_SHELL_VERSION=8.0.30-1.el7
# Tue, 26 Jul 2022 23:29:31 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-shell-$MYSQL_SHELL_VERSION"; 	yum clean all; 		mysqlsh --version
# Tue, 26 Jul 2022 23:29:32 GMT
VOLUME [/var/lib/mysql]
# Tue, 26 Jul 2022 23:29:32 GMT
COPY file:d27cf504fa76fb5a4038020a01eaaf52723b17b751566119de311adacb043752 in /usr/local/bin/ 
# Tue, 26 Jul 2022 23:29:32 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 26 Jul 2022 23:29:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 26 Jul 2022 23:29:33 GMT
EXPOSE 3306 33060
# Tue, 26 Jul 2022 23:29:33 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:66fb3478003364657ac7751c40e41a135e02975f9459f652b1df23e3896b5fac`  
		Last Modified: Tue, 05 Jul 2022 22:22:18 GMT  
		Size: 48.8 MB (48762895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef4ccd63cdb4ccb21c25d292be05bf37ee54a40a0746acdfa962a45a29a08b51`  
		Last Modified: Wed, 13 Jul 2022 06:48:50 GMT  
		Size: 870.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f28a94c51f0d4090e9d6792e3ac48d318cc96056520dd0d7f6e6d2db851891`  
		Last Modified: Wed, 13 Jul 2022 06:48:50 GMT  
		Size: 930.2 KB (930231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7feea2a503b5e8b906b70f33abda7cc47dd30cb72363f804838831a48fdc8a74`  
		Last Modified: Wed, 13 Jul 2022 06:48:49 GMT  
		Size: 4.5 MB (4549473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71dd5852ecd934862db097d1380b3c2fe6471908610bbc2ac0b10f3daf59a183`  
		Last Modified: Wed, 13 Jul 2022 06:48:47 GMT  
		Size: 2.7 KB (2659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ff5c3b24fd570d47fbe75cbe51b9f8428d58446368bf07022c42c52d943a9bb`  
		Last Modified: Tue, 26 Jul 2022 23:31:41 GMT  
		Size: 336.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88a546386a618f1071083b0d9d357cceff83aa39db239224f71a97968e35fff2`  
		Last Modified: Tue, 26 Jul 2022 23:31:43 GMT  
		Size: 25.5 MB (25512706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65b18297cf83f401e9641ba48cc9948ea3593821b42cae5990bacffd230c5ae5`  
		Last Modified: Tue, 26 Jul 2022 23:31:39 GMT  
		Size: 319.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d64f23335fb87ecace32a157428c706c308e2b71a97f9038204e208cf838bea6`  
		Last Modified: Tue, 26 Jul 2022 23:31:48 GMT  
		Size: 48.6 MB (48608834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ba4171261fac245494f48f61a9a3392736658b7c31f707783b796d952008ebb`  
		Last Modified: Tue, 26 Jul 2022 23:31:39 GMT  
		Size: 5.2 KB (5162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96dcc6c8de93eee9106fbbff2915b00236e56b1bf820f724d87daae33cb57e8d`  
		Last Modified: Tue, 26 Jul 2022 23:31:39 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7.39`

```console
$ docker pull mysql@sha256:b3a86578a582617214477d91e47e850f9e18df0b5d1644fb2d96d91a340b8972
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7.39` - linux; amd64

```console
$ docker pull mysql@sha256:5ecf646122c4fcbda81983c9e93e81a011b0593c9c19fbfc55b48bd1c23bc790
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.4 MB (128373606 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3147495b3a5ce957dee2319099a8808c1418e0b0a2c82c9b2396c5fb4b688509`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 05 Jul 2022 22:20:58 GMT
ADD file:50fb7d83a9d57e5a0a6af5e5daf27e464ae8a28c196ce6bad6c254dfc1774cdd in / 
# Tue, 05 Jul 2022 22:20:58 GMT
CMD ["/bin/bash"]
# Wed, 13 Jul 2022 06:46:23 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 13 Jul 2022 06:46:23 GMT
ENV GOSU_VERSION=1.14
# Wed, 13 Jul 2022 06:46:26 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 13 Jul 2022 06:46:48 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False oracle-epel-release-el7; 	yum install -y --setopt=skip_missing_names_on_install=False 		bzip2 		gzip 		openssl 		xz 		zstd 	; 	yum clean all
# Wed, 13 Jul 2022 06:46:49 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 13 Jul 2022 06:46:49 GMT
ENV MYSQL_MAJOR=5.7
# Tue, 26 Jul 2022 23:28:50 GMT
ENV MYSQL_VERSION=5.7.39-1.el7
# Tue, 26 Jul 2022 23:28:51 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql5.7-server-minimal]'; 		echo 'name=MySQL 5.7 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-5.7-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Tue, 26 Jul 2022 23:29:09 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-community-server-minimal-$MYSQL_VERSION"; 	yum clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	{ echo '!includedir /etc/mysql/mysql.conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/mysql.conf.d; 		find /etc/my.cnf /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/'; 		mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Tue, 26 Jul 2022 23:29:10 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Tue, 26 Jul 2022 23:29:10 GMT
ENV MYSQL_SHELL_VERSION=8.0.30-1.el7
# Tue, 26 Jul 2022 23:29:31 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-shell-$MYSQL_SHELL_VERSION"; 	yum clean all; 		mysqlsh --version
# Tue, 26 Jul 2022 23:29:32 GMT
VOLUME [/var/lib/mysql]
# Tue, 26 Jul 2022 23:29:32 GMT
COPY file:d27cf504fa76fb5a4038020a01eaaf52723b17b751566119de311adacb043752 in /usr/local/bin/ 
# Tue, 26 Jul 2022 23:29:32 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 26 Jul 2022 23:29:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 26 Jul 2022 23:29:33 GMT
EXPOSE 3306 33060
# Tue, 26 Jul 2022 23:29:33 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:66fb3478003364657ac7751c40e41a135e02975f9459f652b1df23e3896b5fac`  
		Last Modified: Tue, 05 Jul 2022 22:22:18 GMT  
		Size: 48.8 MB (48762895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef4ccd63cdb4ccb21c25d292be05bf37ee54a40a0746acdfa962a45a29a08b51`  
		Last Modified: Wed, 13 Jul 2022 06:48:50 GMT  
		Size: 870.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f28a94c51f0d4090e9d6792e3ac48d318cc96056520dd0d7f6e6d2db851891`  
		Last Modified: Wed, 13 Jul 2022 06:48:50 GMT  
		Size: 930.2 KB (930231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7feea2a503b5e8b906b70f33abda7cc47dd30cb72363f804838831a48fdc8a74`  
		Last Modified: Wed, 13 Jul 2022 06:48:49 GMT  
		Size: 4.5 MB (4549473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71dd5852ecd934862db097d1380b3c2fe6471908610bbc2ac0b10f3daf59a183`  
		Last Modified: Wed, 13 Jul 2022 06:48:47 GMT  
		Size: 2.7 KB (2659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ff5c3b24fd570d47fbe75cbe51b9f8428d58446368bf07022c42c52d943a9bb`  
		Last Modified: Tue, 26 Jul 2022 23:31:41 GMT  
		Size: 336.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88a546386a618f1071083b0d9d357cceff83aa39db239224f71a97968e35fff2`  
		Last Modified: Tue, 26 Jul 2022 23:31:43 GMT  
		Size: 25.5 MB (25512706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65b18297cf83f401e9641ba48cc9948ea3593821b42cae5990bacffd230c5ae5`  
		Last Modified: Tue, 26 Jul 2022 23:31:39 GMT  
		Size: 319.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d64f23335fb87ecace32a157428c706c308e2b71a97f9038204e208cf838bea6`  
		Last Modified: Tue, 26 Jul 2022 23:31:48 GMT  
		Size: 48.6 MB (48608834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ba4171261fac245494f48f61a9a3392736658b7c31f707783b796d952008ebb`  
		Last Modified: Tue, 26 Jul 2022 23:31:39 GMT  
		Size: 5.2 KB (5162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96dcc6c8de93eee9106fbbff2915b00236e56b1bf820f724d87daae33cb57e8d`  
		Last Modified: Tue, 26 Jul 2022 23:31:39 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7.39-debian`

```console
$ docker pull mysql@sha256:d150c2e5269349200254d3fddb6bb00b6d3f3b4f301c8b050193ce02235e2bd1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7.39-debian` - linux; amd64

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

## `mysql:5.7.39-oracle`

```console
$ docker pull mysql@sha256:b3a86578a582617214477d91e47e850f9e18df0b5d1644fb2d96d91a340b8972
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7.39-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:5ecf646122c4fcbda81983c9e93e81a011b0593c9c19fbfc55b48bd1c23bc790
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.4 MB (128373606 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3147495b3a5ce957dee2319099a8808c1418e0b0a2c82c9b2396c5fb4b688509`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 05 Jul 2022 22:20:58 GMT
ADD file:50fb7d83a9d57e5a0a6af5e5daf27e464ae8a28c196ce6bad6c254dfc1774cdd in / 
# Tue, 05 Jul 2022 22:20:58 GMT
CMD ["/bin/bash"]
# Wed, 13 Jul 2022 06:46:23 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 13 Jul 2022 06:46:23 GMT
ENV GOSU_VERSION=1.14
# Wed, 13 Jul 2022 06:46:26 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 13 Jul 2022 06:46:48 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False oracle-epel-release-el7; 	yum install -y --setopt=skip_missing_names_on_install=False 		bzip2 		gzip 		openssl 		xz 		zstd 	; 	yum clean all
# Wed, 13 Jul 2022 06:46:49 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 13 Jul 2022 06:46:49 GMT
ENV MYSQL_MAJOR=5.7
# Tue, 26 Jul 2022 23:28:50 GMT
ENV MYSQL_VERSION=5.7.39-1.el7
# Tue, 26 Jul 2022 23:28:51 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql5.7-server-minimal]'; 		echo 'name=MySQL 5.7 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-5.7-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Tue, 26 Jul 2022 23:29:09 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-community-server-minimal-$MYSQL_VERSION"; 	yum clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	{ echo '!includedir /etc/mysql/mysql.conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/mysql.conf.d; 		find /etc/my.cnf /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/'; 		mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Tue, 26 Jul 2022 23:29:10 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Tue, 26 Jul 2022 23:29:10 GMT
ENV MYSQL_SHELL_VERSION=8.0.30-1.el7
# Tue, 26 Jul 2022 23:29:31 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-shell-$MYSQL_SHELL_VERSION"; 	yum clean all; 		mysqlsh --version
# Tue, 26 Jul 2022 23:29:32 GMT
VOLUME [/var/lib/mysql]
# Tue, 26 Jul 2022 23:29:32 GMT
COPY file:d27cf504fa76fb5a4038020a01eaaf52723b17b751566119de311adacb043752 in /usr/local/bin/ 
# Tue, 26 Jul 2022 23:29:32 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 26 Jul 2022 23:29:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 26 Jul 2022 23:29:33 GMT
EXPOSE 3306 33060
# Tue, 26 Jul 2022 23:29:33 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:66fb3478003364657ac7751c40e41a135e02975f9459f652b1df23e3896b5fac`  
		Last Modified: Tue, 05 Jul 2022 22:22:18 GMT  
		Size: 48.8 MB (48762895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef4ccd63cdb4ccb21c25d292be05bf37ee54a40a0746acdfa962a45a29a08b51`  
		Last Modified: Wed, 13 Jul 2022 06:48:50 GMT  
		Size: 870.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f28a94c51f0d4090e9d6792e3ac48d318cc96056520dd0d7f6e6d2db851891`  
		Last Modified: Wed, 13 Jul 2022 06:48:50 GMT  
		Size: 930.2 KB (930231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7feea2a503b5e8b906b70f33abda7cc47dd30cb72363f804838831a48fdc8a74`  
		Last Modified: Wed, 13 Jul 2022 06:48:49 GMT  
		Size: 4.5 MB (4549473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71dd5852ecd934862db097d1380b3c2fe6471908610bbc2ac0b10f3daf59a183`  
		Last Modified: Wed, 13 Jul 2022 06:48:47 GMT  
		Size: 2.7 KB (2659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ff5c3b24fd570d47fbe75cbe51b9f8428d58446368bf07022c42c52d943a9bb`  
		Last Modified: Tue, 26 Jul 2022 23:31:41 GMT  
		Size: 336.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88a546386a618f1071083b0d9d357cceff83aa39db239224f71a97968e35fff2`  
		Last Modified: Tue, 26 Jul 2022 23:31:43 GMT  
		Size: 25.5 MB (25512706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65b18297cf83f401e9641ba48cc9948ea3593821b42cae5990bacffd230c5ae5`  
		Last Modified: Tue, 26 Jul 2022 23:31:39 GMT  
		Size: 319.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d64f23335fb87ecace32a157428c706c308e2b71a97f9038204e208cf838bea6`  
		Last Modified: Tue, 26 Jul 2022 23:31:48 GMT  
		Size: 48.6 MB (48608834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ba4171261fac245494f48f61a9a3392736658b7c31f707783b796d952008ebb`  
		Last Modified: Tue, 26 Jul 2022 23:31:39 GMT  
		Size: 5.2 KB (5162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96dcc6c8de93eee9106fbbff2915b00236e56b1bf820f724d87daae33cb57e8d`  
		Last Modified: Tue, 26 Jul 2022 23:31:39 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8`

```console
$ docker pull mysql@sha256:657d78ee56e09101902673adcdd7d2bf03012e759c1aa525eeca28cb0fe1aa7d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8` - linux; amd64

```console
$ docker pull mysql@sha256:13b312e01e8c6eca35c0ff251c261ca2e52994b2a71890539ad31dce8978fa15
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.5 MB (132512841 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38643ad93215bedea00fedd3d6f2a1c8e1bff3b9a172aa2547fd8b4bac9cfee3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 05 Jul 2022 22:20:34 GMT
ADD file:69555d6633d88e50ab2ddecc8bc5002a8f79005d828a9093975d68ca05b023e9 in / 
# Tue, 05 Jul 2022 22:20:34 GMT
CMD ["/bin/bash"]
# Wed, 13 Jul 2022 06:44:43 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 13 Jul 2022 06:44:43 GMT
ENV GOSU_VERSION=1.14
# Wed, 13 Jul 2022 06:44:46 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 13 Jul 2022 06:45:08 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Wed, 13 Jul 2022 06:45:09 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 13 Jul 2022 06:45:09 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 26 Jul 2022 23:27:21 GMT
ENV MYSQL_VERSION=8.0.30-1.el8
# Tue, 26 Jul 2022 23:27:22 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Tue, 26 Jul 2022 23:27:50 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Tue, 26 Jul 2022 23:27:51 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Tue, 26 Jul 2022 23:27:51 GMT
ENV MYSQL_SHELL_VERSION=8.0.30-1.el8
# Tue, 26 Jul 2022 23:28:22 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Tue, 26 Jul 2022 23:28:23 GMT
VOLUME [/var/lib/mysql]
# Tue, 26 Jul 2022 23:28:23 GMT
COPY file:d27cf504fa76fb5a4038020a01eaaf52723b17b751566119de311adacb043752 in /usr/local/bin/ 
# Tue, 26 Jul 2022 23:28:24 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 26 Jul 2022 23:28:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 26 Jul 2022 23:28:24 GMT
EXPOSE 3306 33060
# Tue, 26 Jul 2022 23:28:24 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:e54b73e95ef388354463a761e4e93ce3dac29cb244b2dc0424f2f4afc6ddf5cd`  
		Last Modified: Tue, 05 Jul 2022 22:21:41 GMT  
		Size: 39.2 MB (39222121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:327840d38cb25a590bbb16c433f0e05aa20ff9396d364afa42a6e26d24c6191c`  
		Last Modified: Wed, 13 Jul 2022 06:48:13 GMT  
		Size: 888.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:642077275f5f571c8f25c08b96faa535499c0eda0abe5d31a1dd5652828833b6`  
		Last Modified: Wed, 13 Jul 2022 06:48:13 GMT  
		Size: 928.8 KB (928836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e077469d560d641c3611653814fff9b3ae082c7b9fbdfb388a77ea34e49bf80f`  
		Last Modified: Wed, 13 Jul 2022 06:48:12 GMT  
		Size: 4.6 MB (4588162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbf214d981a6cf5e7e8da61fc840f0f5500ea6b91512f990b91e2d1e8cd6bea1`  
		Last Modified: Wed, 13 Jul 2022 06:48:11 GMT  
		Size: 2.6 KB (2631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4fda5f8b9a827b60600963d317db9cc284863fae5a963ba443cf2bb238f66c1`  
		Last Modified: Tue, 26 Jul 2022 23:30:30 GMT  
		Size: 336.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a41c2763043bfe2e0ecad80d96d0a451f3ed7141c8241418f484cc787c12023c`  
		Last Modified: Tue, 26 Jul 2022 23:30:36 GMT  
		Size: 47.7 MB (47732516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f86b3df6abb1f7fd5fe173a37be422608072ee6ce831b964a3076473ac14105a`  
		Last Modified: Tue, 26 Jul 2022 23:30:29 GMT  
		Size: 319.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95b1c2ed2ecfddca85150fe3e619638d7f71bcca106ad427e1fe8d513285a2fd`  
		Last Modified: Tue, 26 Jul 2022 23:30:36 GMT  
		Size: 40.0 MB (40031753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0edcd52771b148165e0ca520d3e3981ca95e94e9abcc3c895586a0caf919d7f`  
		Last Modified: Tue, 26 Jul 2022 23:30:28 GMT  
		Size: 5.2 KB (5159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3d312b5c835845f301e964bb6bd231671dc089225f6d4457eb636b7fabfad5e`  
		Last Modified: Tue, 26 Jul 2022 23:30:28 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:2375bf5d81d54f400d6af809fe60c1af2e0252e7d5b65bb65a80ca844ee3338e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.2 MB (141223352 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a75af66873e7bc730c1934b1d7319e5c3cf1eb3f26c72653ebfaba0af229c25`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 05 Jul 2022 22:43:14 GMT
ADD file:e864e9187ff57bc1df9611a0990052f89611bfe7b6bc8e3d24b500b0886ec725 in / 
# Tue, 05 Jul 2022 22:43:14 GMT
CMD ["/bin/bash"]
# Wed, 13 Jul 2022 07:47:27 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 13 Jul 2022 07:47:27 GMT
ENV GOSU_VERSION=1.14
# Wed, 13 Jul 2022 07:47:31 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 13 Jul 2022 07:47:52 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Wed, 13 Jul 2022 07:47:54 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 13 Jul 2022 07:47:55 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 26 Jul 2022 23:55:24 GMT
ENV MYSQL_VERSION=8.0.30-1.el8
# Tue, 26 Jul 2022 23:55:25 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Tue, 26 Jul 2022 23:55:53 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Tue, 26 Jul 2022 23:55:54 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Tue, 26 Jul 2022 23:55:54 GMT
ENV MYSQL_SHELL_VERSION=8.0.30-1.el8
# Tue, 26 Jul 2022 23:56:24 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Tue, 26 Jul 2022 23:56:24 GMT
VOLUME [/var/lib/mysql]
# Tue, 26 Jul 2022 23:56:26 GMT
COPY file:d27cf504fa76fb5a4038020a01eaaf52723b17b751566119de311adacb043752 in /usr/local/bin/ 
# Tue, 26 Jul 2022 23:56:27 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 26 Jul 2022 23:56:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 26 Jul 2022 23:56:28 GMT
EXPOSE 3306 33060
# Tue, 26 Jul 2022 23:56:29 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:e5d41499b4049578ed8bbb14817cd79d4136a84899b65e4364b0125d4d1c792c`  
		Last Modified: Tue, 05 Jul 2022 22:44:31 GMT  
		Size: 38.0 MB (38027757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c14e53563050114db97e64919184751150f664c330508d7e443fb5408550cc04`  
		Last Modified: Wed, 13 Jul 2022 07:49:28 GMT  
		Size: 889.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:024772013ffd3205dc1717b60dc2ed89bb9953874fa53b4ee3d343be4e2db409`  
		Last Modified: Wed, 13 Jul 2022 07:49:29 GMT  
		Size: 857.2 KB (857153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e0914c16b380ff7a955c5cf1f69c21b835e52f6ac378a4b7323bfa168404007`  
		Last Modified: Wed, 13 Jul 2022 07:49:27 GMT  
		Size: 4.4 MB (4421847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71713f7372e7c03e17b0c0a4ef720ab6d7eb715efc80d2274f6e16588fbf0eae`  
		Last Modified: Wed, 13 Jul 2022 07:49:26 GMT  
		Size: 2.6 KB (2609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cad5804e4a57cfb046f1f19c286013ef3ffad8360b663613cad59978a512370`  
		Last Modified: Tue, 26 Jul 2022 23:56:57 GMT  
		Size: 333.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5308d3086645e729f0b6f0c42389abe0258a77941d250b2bdec734dcd408b41`  
		Last Modified: Tue, 26 Jul 2022 23:57:03 GMT  
		Size: 53.8 MB (53798288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5515cfa517579de894d15b5691fc09c6e6958e7a999a6dd419b9bb58a74c61d`  
		Last Modified: Tue, 26 Jul 2022 23:56:55 GMT  
		Size: 317.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44f33897b41dca1ed29f97e09e80baab85adc710313917c9164a9130f1cfc693`  
		Last Modified: Tue, 26 Jul 2022 23:57:03 GMT  
		Size: 44.1 MB (44108878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc195249cd1e03b936b46ede192667a7e83792b9f93f7ca837521293fb105494`  
		Last Modified: Tue, 26 Jul 2022 23:56:55 GMT  
		Size: 5.2 KB (5160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56ebae63daf8dd8c229ad24c897be15566d5416ab8bffe4f6d1719bf14e20b09`  
		Last Modified: Tue, 26 Jul 2022 23:56:55 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8-debian`

```console
$ docker pull mysql@sha256:504760f722770e8554c40e7ea6b803ae9e0c19e21e25b94d0b8a03bab20541ff
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:8-debian` - linux; amd64

```console
$ docker pull mysql@sha256:9a16d88a3410a326a082261a64db5624902fc763775410663cc44420968831a3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **157.8 MB (157835607 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c2ee58f241ef6265fbc87840afec971c52938a5bcc38259e71bb0ad0363e827e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 12 Jul 2022 01:20:10 GMT
ADD file:d978f6d3025a06f5142a0c13c98bf12fbd47cdf9162ed31fbc05c86983b0a679 in / 
# Tue, 12 Jul 2022 01:20:10 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 01:49:49 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 12 Jul 2022 01:49:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 01:49:56 GMT
ENV GOSU_VERSION=1.14
# Tue, 12 Jul 2022 01:50:05 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 12 Jul 2022 01:50:05 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 12 Jul 2022 01:50:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 01:50:12 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Tue, 12 Jul 2022 01:50:12 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 26 Jul 2022 23:28:31 GMT
ENV MYSQL_VERSION=8.0.30-1debian11
# Tue, 26 Jul 2022 23:28:31 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ bullseye mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Tue, 26 Jul 2022 23:28:45 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 26 Jul 2022 23:28:45 GMT
VOLUME [/var/lib/mysql]
# Tue, 26 Jul 2022 23:28:45 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Tue, 26 Jul 2022 23:28:46 GMT
COPY file:d27cf504fa76fb5a4038020a01eaaf52723b17b751566119de311adacb043752 in /usr/local/bin/ 
# Tue, 26 Jul 2022 23:28:46 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 26 Jul 2022 23:28:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 26 Jul 2022 23:28:46 GMT
EXPOSE 3306 33060
# Tue, 26 Jul 2022 23:28:46 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:461246efe0a75316d99afdbf348f7063b57b0caeee8daab775f1f08152ea36f4`  
		Last Modified: Tue, 12 Jul 2022 01:24:34 GMT  
		Size: 31.4 MB (31366610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1cd5bb1f5de5503f17b383d7c62078467389f82828ac46a41db64289ecf9880`  
		Last Modified: Tue, 12 Jul 2022 01:52:26 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd9d402d85bd06018ec1a89d3298f4d88f3c4d06c2cd93c8951d8bbb19596ace`  
		Last Modified: Tue, 12 Jul 2022 01:52:26 GMT  
		Size: 4.4 MB (4414786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33a04621f5daa2ee95b4484e11cb963f929686d8f77511d9e31d8cf63d2a491b`  
		Last Modified: Tue, 12 Jul 2022 01:52:24 GMT  
		Size: 1.4 MB (1418425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2eef8024049f6e7f8a7769c0ed43bc5ddab7c1b3dbc772a3ba1b71a039bff03`  
		Last Modified: Tue, 12 Jul 2022 01:52:23 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a021c48082a6778bc62f96a17b8202ad24185d41b54fad0c4788d55e18a106b1`  
		Last Modified: Tue, 12 Jul 2022 01:52:26 GMT  
		Size: 12.7 MB (12661669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a27a84090d2f2cc8e7bc9db5098fe5f2c61aaf38e003421fab9630fdf6541c2`  
		Last Modified: Tue, 12 Jul 2022 01:52:23 GMT  
		Size: 2.5 KB (2547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40bc66f09ecd05d38547cb872afb8703d21702dcbd68f1688e69c1fa899b9bfe`  
		Last Modified: Tue, 26 Jul 2022 23:31:05 GMT  
		Size: 256.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57a0b87a3f7d2dd5b0a2ba39b526929f321b90da90a2249caf4da175b9b19e70`  
		Last Modified: Tue, 26 Jul 2022 23:31:22 GMT  
		Size: 108.0 MB (107963313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44e82ef1aa7cd91168ba63bd5724afa619590e17c79d641515a3a0f23bf75839`  
		Last Modified: Tue, 26 Jul 2022 23:31:05 GMT  
		Size: 842.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f04800ad7ccd34e26a26464cfa045c9030672e0bc018c05b370e55acce1d02e`  
		Last Modified: Tue, 26 Jul 2022 23:31:05 GMT  
		Size: 5.2 KB (5157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6593ab5ec7351b0dba0042dd7086bb2ae362d26cd4c7be288dfc618a7884ea15`  
		Last Modified: Tue, 26 Jul 2022 23:31:05 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8-oracle`

```console
$ docker pull mysql@sha256:657d78ee56e09101902673adcdd7d2bf03012e759c1aa525eeca28cb0fe1aa7d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:13b312e01e8c6eca35c0ff251c261ca2e52994b2a71890539ad31dce8978fa15
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.5 MB (132512841 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38643ad93215bedea00fedd3d6f2a1c8e1bff3b9a172aa2547fd8b4bac9cfee3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 05 Jul 2022 22:20:34 GMT
ADD file:69555d6633d88e50ab2ddecc8bc5002a8f79005d828a9093975d68ca05b023e9 in / 
# Tue, 05 Jul 2022 22:20:34 GMT
CMD ["/bin/bash"]
# Wed, 13 Jul 2022 06:44:43 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 13 Jul 2022 06:44:43 GMT
ENV GOSU_VERSION=1.14
# Wed, 13 Jul 2022 06:44:46 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 13 Jul 2022 06:45:08 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Wed, 13 Jul 2022 06:45:09 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 13 Jul 2022 06:45:09 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 26 Jul 2022 23:27:21 GMT
ENV MYSQL_VERSION=8.0.30-1.el8
# Tue, 26 Jul 2022 23:27:22 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Tue, 26 Jul 2022 23:27:50 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Tue, 26 Jul 2022 23:27:51 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Tue, 26 Jul 2022 23:27:51 GMT
ENV MYSQL_SHELL_VERSION=8.0.30-1.el8
# Tue, 26 Jul 2022 23:28:22 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Tue, 26 Jul 2022 23:28:23 GMT
VOLUME [/var/lib/mysql]
# Tue, 26 Jul 2022 23:28:23 GMT
COPY file:d27cf504fa76fb5a4038020a01eaaf52723b17b751566119de311adacb043752 in /usr/local/bin/ 
# Tue, 26 Jul 2022 23:28:24 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 26 Jul 2022 23:28:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 26 Jul 2022 23:28:24 GMT
EXPOSE 3306 33060
# Tue, 26 Jul 2022 23:28:24 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:e54b73e95ef388354463a761e4e93ce3dac29cb244b2dc0424f2f4afc6ddf5cd`  
		Last Modified: Tue, 05 Jul 2022 22:21:41 GMT  
		Size: 39.2 MB (39222121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:327840d38cb25a590bbb16c433f0e05aa20ff9396d364afa42a6e26d24c6191c`  
		Last Modified: Wed, 13 Jul 2022 06:48:13 GMT  
		Size: 888.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:642077275f5f571c8f25c08b96faa535499c0eda0abe5d31a1dd5652828833b6`  
		Last Modified: Wed, 13 Jul 2022 06:48:13 GMT  
		Size: 928.8 KB (928836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e077469d560d641c3611653814fff9b3ae082c7b9fbdfb388a77ea34e49bf80f`  
		Last Modified: Wed, 13 Jul 2022 06:48:12 GMT  
		Size: 4.6 MB (4588162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbf214d981a6cf5e7e8da61fc840f0f5500ea6b91512f990b91e2d1e8cd6bea1`  
		Last Modified: Wed, 13 Jul 2022 06:48:11 GMT  
		Size: 2.6 KB (2631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4fda5f8b9a827b60600963d317db9cc284863fae5a963ba443cf2bb238f66c1`  
		Last Modified: Tue, 26 Jul 2022 23:30:30 GMT  
		Size: 336.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a41c2763043bfe2e0ecad80d96d0a451f3ed7141c8241418f484cc787c12023c`  
		Last Modified: Tue, 26 Jul 2022 23:30:36 GMT  
		Size: 47.7 MB (47732516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f86b3df6abb1f7fd5fe173a37be422608072ee6ce831b964a3076473ac14105a`  
		Last Modified: Tue, 26 Jul 2022 23:30:29 GMT  
		Size: 319.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95b1c2ed2ecfddca85150fe3e619638d7f71bcca106ad427e1fe8d513285a2fd`  
		Last Modified: Tue, 26 Jul 2022 23:30:36 GMT  
		Size: 40.0 MB (40031753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0edcd52771b148165e0ca520d3e3981ca95e94e9abcc3c895586a0caf919d7f`  
		Last Modified: Tue, 26 Jul 2022 23:30:28 GMT  
		Size: 5.2 KB (5159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3d312b5c835845f301e964bb6bd231671dc089225f6d4457eb636b7fabfad5e`  
		Last Modified: Tue, 26 Jul 2022 23:30:28 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8-oracle` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:2375bf5d81d54f400d6af809fe60c1af2e0252e7d5b65bb65a80ca844ee3338e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.2 MB (141223352 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a75af66873e7bc730c1934b1d7319e5c3cf1eb3f26c72653ebfaba0af229c25`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 05 Jul 2022 22:43:14 GMT
ADD file:e864e9187ff57bc1df9611a0990052f89611bfe7b6bc8e3d24b500b0886ec725 in / 
# Tue, 05 Jul 2022 22:43:14 GMT
CMD ["/bin/bash"]
# Wed, 13 Jul 2022 07:47:27 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 13 Jul 2022 07:47:27 GMT
ENV GOSU_VERSION=1.14
# Wed, 13 Jul 2022 07:47:31 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 13 Jul 2022 07:47:52 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Wed, 13 Jul 2022 07:47:54 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 13 Jul 2022 07:47:55 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 26 Jul 2022 23:55:24 GMT
ENV MYSQL_VERSION=8.0.30-1.el8
# Tue, 26 Jul 2022 23:55:25 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Tue, 26 Jul 2022 23:55:53 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Tue, 26 Jul 2022 23:55:54 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Tue, 26 Jul 2022 23:55:54 GMT
ENV MYSQL_SHELL_VERSION=8.0.30-1.el8
# Tue, 26 Jul 2022 23:56:24 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Tue, 26 Jul 2022 23:56:24 GMT
VOLUME [/var/lib/mysql]
# Tue, 26 Jul 2022 23:56:26 GMT
COPY file:d27cf504fa76fb5a4038020a01eaaf52723b17b751566119de311adacb043752 in /usr/local/bin/ 
# Tue, 26 Jul 2022 23:56:27 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 26 Jul 2022 23:56:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 26 Jul 2022 23:56:28 GMT
EXPOSE 3306 33060
# Tue, 26 Jul 2022 23:56:29 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:e5d41499b4049578ed8bbb14817cd79d4136a84899b65e4364b0125d4d1c792c`  
		Last Modified: Tue, 05 Jul 2022 22:44:31 GMT  
		Size: 38.0 MB (38027757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c14e53563050114db97e64919184751150f664c330508d7e443fb5408550cc04`  
		Last Modified: Wed, 13 Jul 2022 07:49:28 GMT  
		Size: 889.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:024772013ffd3205dc1717b60dc2ed89bb9953874fa53b4ee3d343be4e2db409`  
		Last Modified: Wed, 13 Jul 2022 07:49:29 GMT  
		Size: 857.2 KB (857153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e0914c16b380ff7a955c5cf1f69c21b835e52f6ac378a4b7323bfa168404007`  
		Last Modified: Wed, 13 Jul 2022 07:49:27 GMT  
		Size: 4.4 MB (4421847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71713f7372e7c03e17b0c0a4ef720ab6d7eb715efc80d2274f6e16588fbf0eae`  
		Last Modified: Wed, 13 Jul 2022 07:49:26 GMT  
		Size: 2.6 KB (2609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cad5804e4a57cfb046f1f19c286013ef3ffad8360b663613cad59978a512370`  
		Last Modified: Tue, 26 Jul 2022 23:56:57 GMT  
		Size: 333.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5308d3086645e729f0b6f0c42389abe0258a77941d250b2bdec734dcd408b41`  
		Last Modified: Tue, 26 Jul 2022 23:57:03 GMT  
		Size: 53.8 MB (53798288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5515cfa517579de894d15b5691fc09c6e6958e7a999a6dd419b9bb58a74c61d`  
		Last Modified: Tue, 26 Jul 2022 23:56:55 GMT  
		Size: 317.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44f33897b41dca1ed29f97e09e80baab85adc710313917c9164a9130f1cfc693`  
		Last Modified: Tue, 26 Jul 2022 23:57:03 GMT  
		Size: 44.1 MB (44108878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc195249cd1e03b936b46ede192667a7e83792b9f93f7ca837521293fb105494`  
		Last Modified: Tue, 26 Jul 2022 23:56:55 GMT  
		Size: 5.2 KB (5160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56ebae63daf8dd8c229ad24c897be15566d5416ab8bffe4f6d1719bf14e20b09`  
		Last Modified: Tue, 26 Jul 2022 23:56:55 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0`

```console
$ docker pull mysql@sha256:657d78ee56e09101902673adcdd7d2bf03012e759c1aa525eeca28cb0fe1aa7d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8.0` - linux; amd64

```console
$ docker pull mysql@sha256:13b312e01e8c6eca35c0ff251c261ca2e52994b2a71890539ad31dce8978fa15
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.5 MB (132512841 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38643ad93215bedea00fedd3d6f2a1c8e1bff3b9a172aa2547fd8b4bac9cfee3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 05 Jul 2022 22:20:34 GMT
ADD file:69555d6633d88e50ab2ddecc8bc5002a8f79005d828a9093975d68ca05b023e9 in / 
# Tue, 05 Jul 2022 22:20:34 GMT
CMD ["/bin/bash"]
# Wed, 13 Jul 2022 06:44:43 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 13 Jul 2022 06:44:43 GMT
ENV GOSU_VERSION=1.14
# Wed, 13 Jul 2022 06:44:46 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 13 Jul 2022 06:45:08 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Wed, 13 Jul 2022 06:45:09 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 13 Jul 2022 06:45:09 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 26 Jul 2022 23:27:21 GMT
ENV MYSQL_VERSION=8.0.30-1.el8
# Tue, 26 Jul 2022 23:27:22 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Tue, 26 Jul 2022 23:27:50 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Tue, 26 Jul 2022 23:27:51 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Tue, 26 Jul 2022 23:27:51 GMT
ENV MYSQL_SHELL_VERSION=8.0.30-1.el8
# Tue, 26 Jul 2022 23:28:22 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Tue, 26 Jul 2022 23:28:23 GMT
VOLUME [/var/lib/mysql]
# Tue, 26 Jul 2022 23:28:23 GMT
COPY file:d27cf504fa76fb5a4038020a01eaaf52723b17b751566119de311adacb043752 in /usr/local/bin/ 
# Tue, 26 Jul 2022 23:28:24 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 26 Jul 2022 23:28:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 26 Jul 2022 23:28:24 GMT
EXPOSE 3306 33060
# Tue, 26 Jul 2022 23:28:24 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:e54b73e95ef388354463a761e4e93ce3dac29cb244b2dc0424f2f4afc6ddf5cd`  
		Last Modified: Tue, 05 Jul 2022 22:21:41 GMT  
		Size: 39.2 MB (39222121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:327840d38cb25a590bbb16c433f0e05aa20ff9396d364afa42a6e26d24c6191c`  
		Last Modified: Wed, 13 Jul 2022 06:48:13 GMT  
		Size: 888.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:642077275f5f571c8f25c08b96faa535499c0eda0abe5d31a1dd5652828833b6`  
		Last Modified: Wed, 13 Jul 2022 06:48:13 GMT  
		Size: 928.8 KB (928836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e077469d560d641c3611653814fff9b3ae082c7b9fbdfb388a77ea34e49bf80f`  
		Last Modified: Wed, 13 Jul 2022 06:48:12 GMT  
		Size: 4.6 MB (4588162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbf214d981a6cf5e7e8da61fc840f0f5500ea6b91512f990b91e2d1e8cd6bea1`  
		Last Modified: Wed, 13 Jul 2022 06:48:11 GMT  
		Size: 2.6 KB (2631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4fda5f8b9a827b60600963d317db9cc284863fae5a963ba443cf2bb238f66c1`  
		Last Modified: Tue, 26 Jul 2022 23:30:30 GMT  
		Size: 336.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a41c2763043bfe2e0ecad80d96d0a451f3ed7141c8241418f484cc787c12023c`  
		Last Modified: Tue, 26 Jul 2022 23:30:36 GMT  
		Size: 47.7 MB (47732516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f86b3df6abb1f7fd5fe173a37be422608072ee6ce831b964a3076473ac14105a`  
		Last Modified: Tue, 26 Jul 2022 23:30:29 GMT  
		Size: 319.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95b1c2ed2ecfddca85150fe3e619638d7f71bcca106ad427e1fe8d513285a2fd`  
		Last Modified: Tue, 26 Jul 2022 23:30:36 GMT  
		Size: 40.0 MB (40031753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0edcd52771b148165e0ca520d3e3981ca95e94e9abcc3c895586a0caf919d7f`  
		Last Modified: Tue, 26 Jul 2022 23:30:28 GMT  
		Size: 5.2 KB (5159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3d312b5c835845f301e964bb6bd231671dc089225f6d4457eb636b7fabfad5e`  
		Last Modified: Tue, 26 Jul 2022 23:30:28 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8.0` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:2375bf5d81d54f400d6af809fe60c1af2e0252e7d5b65bb65a80ca844ee3338e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.2 MB (141223352 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a75af66873e7bc730c1934b1d7319e5c3cf1eb3f26c72653ebfaba0af229c25`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 05 Jul 2022 22:43:14 GMT
ADD file:e864e9187ff57bc1df9611a0990052f89611bfe7b6bc8e3d24b500b0886ec725 in / 
# Tue, 05 Jul 2022 22:43:14 GMT
CMD ["/bin/bash"]
# Wed, 13 Jul 2022 07:47:27 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 13 Jul 2022 07:47:27 GMT
ENV GOSU_VERSION=1.14
# Wed, 13 Jul 2022 07:47:31 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 13 Jul 2022 07:47:52 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Wed, 13 Jul 2022 07:47:54 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 13 Jul 2022 07:47:55 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 26 Jul 2022 23:55:24 GMT
ENV MYSQL_VERSION=8.0.30-1.el8
# Tue, 26 Jul 2022 23:55:25 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Tue, 26 Jul 2022 23:55:53 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Tue, 26 Jul 2022 23:55:54 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Tue, 26 Jul 2022 23:55:54 GMT
ENV MYSQL_SHELL_VERSION=8.0.30-1.el8
# Tue, 26 Jul 2022 23:56:24 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Tue, 26 Jul 2022 23:56:24 GMT
VOLUME [/var/lib/mysql]
# Tue, 26 Jul 2022 23:56:26 GMT
COPY file:d27cf504fa76fb5a4038020a01eaaf52723b17b751566119de311adacb043752 in /usr/local/bin/ 
# Tue, 26 Jul 2022 23:56:27 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 26 Jul 2022 23:56:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 26 Jul 2022 23:56:28 GMT
EXPOSE 3306 33060
# Tue, 26 Jul 2022 23:56:29 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:e5d41499b4049578ed8bbb14817cd79d4136a84899b65e4364b0125d4d1c792c`  
		Last Modified: Tue, 05 Jul 2022 22:44:31 GMT  
		Size: 38.0 MB (38027757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c14e53563050114db97e64919184751150f664c330508d7e443fb5408550cc04`  
		Last Modified: Wed, 13 Jul 2022 07:49:28 GMT  
		Size: 889.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:024772013ffd3205dc1717b60dc2ed89bb9953874fa53b4ee3d343be4e2db409`  
		Last Modified: Wed, 13 Jul 2022 07:49:29 GMT  
		Size: 857.2 KB (857153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e0914c16b380ff7a955c5cf1f69c21b835e52f6ac378a4b7323bfa168404007`  
		Last Modified: Wed, 13 Jul 2022 07:49:27 GMT  
		Size: 4.4 MB (4421847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71713f7372e7c03e17b0c0a4ef720ab6d7eb715efc80d2274f6e16588fbf0eae`  
		Last Modified: Wed, 13 Jul 2022 07:49:26 GMT  
		Size: 2.6 KB (2609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cad5804e4a57cfb046f1f19c286013ef3ffad8360b663613cad59978a512370`  
		Last Modified: Tue, 26 Jul 2022 23:56:57 GMT  
		Size: 333.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5308d3086645e729f0b6f0c42389abe0258a77941d250b2bdec734dcd408b41`  
		Last Modified: Tue, 26 Jul 2022 23:57:03 GMT  
		Size: 53.8 MB (53798288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5515cfa517579de894d15b5691fc09c6e6958e7a999a6dd419b9bb58a74c61d`  
		Last Modified: Tue, 26 Jul 2022 23:56:55 GMT  
		Size: 317.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44f33897b41dca1ed29f97e09e80baab85adc710313917c9164a9130f1cfc693`  
		Last Modified: Tue, 26 Jul 2022 23:57:03 GMT  
		Size: 44.1 MB (44108878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc195249cd1e03b936b46ede192667a7e83792b9f93f7ca837521293fb105494`  
		Last Modified: Tue, 26 Jul 2022 23:56:55 GMT  
		Size: 5.2 KB (5160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56ebae63daf8dd8c229ad24c897be15566d5416ab8bffe4f6d1719bf14e20b09`  
		Last Modified: Tue, 26 Jul 2022 23:56:55 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0-debian`

```console
$ docker pull mysql@sha256:504760f722770e8554c40e7ea6b803ae9e0c19e21e25b94d0b8a03bab20541ff
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:8.0-debian` - linux; amd64

```console
$ docker pull mysql@sha256:9a16d88a3410a326a082261a64db5624902fc763775410663cc44420968831a3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **157.8 MB (157835607 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c2ee58f241ef6265fbc87840afec971c52938a5bcc38259e71bb0ad0363e827e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 12 Jul 2022 01:20:10 GMT
ADD file:d978f6d3025a06f5142a0c13c98bf12fbd47cdf9162ed31fbc05c86983b0a679 in / 
# Tue, 12 Jul 2022 01:20:10 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 01:49:49 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 12 Jul 2022 01:49:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 01:49:56 GMT
ENV GOSU_VERSION=1.14
# Tue, 12 Jul 2022 01:50:05 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 12 Jul 2022 01:50:05 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 12 Jul 2022 01:50:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 01:50:12 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Tue, 12 Jul 2022 01:50:12 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 26 Jul 2022 23:28:31 GMT
ENV MYSQL_VERSION=8.0.30-1debian11
# Tue, 26 Jul 2022 23:28:31 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ bullseye mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Tue, 26 Jul 2022 23:28:45 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 26 Jul 2022 23:28:45 GMT
VOLUME [/var/lib/mysql]
# Tue, 26 Jul 2022 23:28:45 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Tue, 26 Jul 2022 23:28:46 GMT
COPY file:d27cf504fa76fb5a4038020a01eaaf52723b17b751566119de311adacb043752 in /usr/local/bin/ 
# Tue, 26 Jul 2022 23:28:46 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 26 Jul 2022 23:28:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 26 Jul 2022 23:28:46 GMT
EXPOSE 3306 33060
# Tue, 26 Jul 2022 23:28:46 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:461246efe0a75316d99afdbf348f7063b57b0caeee8daab775f1f08152ea36f4`  
		Last Modified: Tue, 12 Jul 2022 01:24:34 GMT  
		Size: 31.4 MB (31366610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1cd5bb1f5de5503f17b383d7c62078467389f82828ac46a41db64289ecf9880`  
		Last Modified: Tue, 12 Jul 2022 01:52:26 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd9d402d85bd06018ec1a89d3298f4d88f3c4d06c2cd93c8951d8bbb19596ace`  
		Last Modified: Tue, 12 Jul 2022 01:52:26 GMT  
		Size: 4.4 MB (4414786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33a04621f5daa2ee95b4484e11cb963f929686d8f77511d9e31d8cf63d2a491b`  
		Last Modified: Tue, 12 Jul 2022 01:52:24 GMT  
		Size: 1.4 MB (1418425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2eef8024049f6e7f8a7769c0ed43bc5ddab7c1b3dbc772a3ba1b71a039bff03`  
		Last Modified: Tue, 12 Jul 2022 01:52:23 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a021c48082a6778bc62f96a17b8202ad24185d41b54fad0c4788d55e18a106b1`  
		Last Modified: Tue, 12 Jul 2022 01:52:26 GMT  
		Size: 12.7 MB (12661669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a27a84090d2f2cc8e7bc9db5098fe5f2c61aaf38e003421fab9630fdf6541c2`  
		Last Modified: Tue, 12 Jul 2022 01:52:23 GMT  
		Size: 2.5 KB (2547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40bc66f09ecd05d38547cb872afb8703d21702dcbd68f1688e69c1fa899b9bfe`  
		Last Modified: Tue, 26 Jul 2022 23:31:05 GMT  
		Size: 256.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57a0b87a3f7d2dd5b0a2ba39b526929f321b90da90a2249caf4da175b9b19e70`  
		Last Modified: Tue, 26 Jul 2022 23:31:22 GMT  
		Size: 108.0 MB (107963313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44e82ef1aa7cd91168ba63bd5724afa619590e17c79d641515a3a0f23bf75839`  
		Last Modified: Tue, 26 Jul 2022 23:31:05 GMT  
		Size: 842.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f04800ad7ccd34e26a26464cfa045c9030672e0bc018c05b370e55acce1d02e`  
		Last Modified: Tue, 26 Jul 2022 23:31:05 GMT  
		Size: 5.2 KB (5157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6593ab5ec7351b0dba0042dd7086bb2ae362d26cd4c7be288dfc618a7884ea15`  
		Last Modified: Tue, 26 Jul 2022 23:31:05 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0-oracle`

```console
$ docker pull mysql@sha256:657d78ee56e09101902673adcdd7d2bf03012e759c1aa525eeca28cb0fe1aa7d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8.0-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:13b312e01e8c6eca35c0ff251c261ca2e52994b2a71890539ad31dce8978fa15
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.5 MB (132512841 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38643ad93215bedea00fedd3d6f2a1c8e1bff3b9a172aa2547fd8b4bac9cfee3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 05 Jul 2022 22:20:34 GMT
ADD file:69555d6633d88e50ab2ddecc8bc5002a8f79005d828a9093975d68ca05b023e9 in / 
# Tue, 05 Jul 2022 22:20:34 GMT
CMD ["/bin/bash"]
# Wed, 13 Jul 2022 06:44:43 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 13 Jul 2022 06:44:43 GMT
ENV GOSU_VERSION=1.14
# Wed, 13 Jul 2022 06:44:46 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 13 Jul 2022 06:45:08 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Wed, 13 Jul 2022 06:45:09 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 13 Jul 2022 06:45:09 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 26 Jul 2022 23:27:21 GMT
ENV MYSQL_VERSION=8.0.30-1.el8
# Tue, 26 Jul 2022 23:27:22 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Tue, 26 Jul 2022 23:27:50 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Tue, 26 Jul 2022 23:27:51 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Tue, 26 Jul 2022 23:27:51 GMT
ENV MYSQL_SHELL_VERSION=8.0.30-1.el8
# Tue, 26 Jul 2022 23:28:22 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Tue, 26 Jul 2022 23:28:23 GMT
VOLUME [/var/lib/mysql]
# Tue, 26 Jul 2022 23:28:23 GMT
COPY file:d27cf504fa76fb5a4038020a01eaaf52723b17b751566119de311adacb043752 in /usr/local/bin/ 
# Tue, 26 Jul 2022 23:28:24 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 26 Jul 2022 23:28:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 26 Jul 2022 23:28:24 GMT
EXPOSE 3306 33060
# Tue, 26 Jul 2022 23:28:24 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:e54b73e95ef388354463a761e4e93ce3dac29cb244b2dc0424f2f4afc6ddf5cd`  
		Last Modified: Tue, 05 Jul 2022 22:21:41 GMT  
		Size: 39.2 MB (39222121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:327840d38cb25a590bbb16c433f0e05aa20ff9396d364afa42a6e26d24c6191c`  
		Last Modified: Wed, 13 Jul 2022 06:48:13 GMT  
		Size: 888.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:642077275f5f571c8f25c08b96faa535499c0eda0abe5d31a1dd5652828833b6`  
		Last Modified: Wed, 13 Jul 2022 06:48:13 GMT  
		Size: 928.8 KB (928836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e077469d560d641c3611653814fff9b3ae082c7b9fbdfb388a77ea34e49bf80f`  
		Last Modified: Wed, 13 Jul 2022 06:48:12 GMT  
		Size: 4.6 MB (4588162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbf214d981a6cf5e7e8da61fc840f0f5500ea6b91512f990b91e2d1e8cd6bea1`  
		Last Modified: Wed, 13 Jul 2022 06:48:11 GMT  
		Size: 2.6 KB (2631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4fda5f8b9a827b60600963d317db9cc284863fae5a963ba443cf2bb238f66c1`  
		Last Modified: Tue, 26 Jul 2022 23:30:30 GMT  
		Size: 336.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a41c2763043bfe2e0ecad80d96d0a451f3ed7141c8241418f484cc787c12023c`  
		Last Modified: Tue, 26 Jul 2022 23:30:36 GMT  
		Size: 47.7 MB (47732516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f86b3df6abb1f7fd5fe173a37be422608072ee6ce831b964a3076473ac14105a`  
		Last Modified: Tue, 26 Jul 2022 23:30:29 GMT  
		Size: 319.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95b1c2ed2ecfddca85150fe3e619638d7f71bcca106ad427e1fe8d513285a2fd`  
		Last Modified: Tue, 26 Jul 2022 23:30:36 GMT  
		Size: 40.0 MB (40031753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0edcd52771b148165e0ca520d3e3981ca95e94e9abcc3c895586a0caf919d7f`  
		Last Modified: Tue, 26 Jul 2022 23:30:28 GMT  
		Size: 5.2 KB (5159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3d312b5c835845f301e964bb6bd231671dc089225f6d4457eb636b7fabfad5e`  
		Last Modified: Tue, 26 Jul 2022 23:30:28 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8.0-oracle` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:2375bf5d81d54f400d6af809fe60c1af2e0252e7d5b65bb65a80ca844ee3338e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.2 MB (141223352 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a75af66873e7bc730c1934b1d7319e5c3cf1eb3f26c72653ebfaba0af229c25`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 05 Jul 2022 22:43:14 GMT
ADD file:e864e9187ff57bc1df9611a0990052f89611bfe7b6bc8e3d24b500b0886ec725 in / 
# Tue, 05 Jul 2022 22:43:14 GMT
CMD ["/bin/bash"]
# Wed, 13 Jul 2022 07:47:27 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 13 Jul 2022 07:47:27 GMT
ENV GOSU_VERSION=1.14
# Wed, 13 Jul 2022 07:47:31 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 13 Jul 2022 07:47:52 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Wed, 13 Jul 2022 07:47:54 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 13 Jul 2022 07:47:55 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 26 Jul 2022 23:55:24 GMT
ENV MYSQL_VERSION=8.0.30-1.el8
# Tue, 26 Jul 2022 23:55:25 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Tue, 26 Jul 2022 23:55:53 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Tue, 26 Jul 2022 23:55:54 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Tue, 26 Jul 2022 23:55:54 GMT
ENV MYSQL_SHELL_VERSION=8.0.30-1.el8
# Tue, 26 Jul 2022 23:56:24 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Tue, 26 Jul 2022 23:56:24 GMT
VOLUME [/var/lib/mysql]
# Tue, 26 Jul 2022 23:56:26 GMT
COPY file:d27cf504fa76fb5a4038020a01eaaf52723b17b751566119de311adacb043752 in /usr/local/bin/ 
# Tue, 26 Jul 2022 23:56:27 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 26 Jul 2022 23:56:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 26 Jul 2022 23:56:28 GMT
EXPOSE 3306 33060
# Tue, 26 Jul 2022 23:56:29 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:e5d41499b4049578ed8bbb14817cd79d4136a84899b65e4364b0125d4d1c792c`  
		Last Modified: Tue, 05 Jul 2022 22:44:31 GMT  
		Size: 38.0 MB (38027757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c14e53563050114db97e64919184751150f664c330508d7e443fb5408550cc04`  
		Last Modified: Wed, 13 Jul 2022 07:49:28 GMT  
		Size: 889.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:024772013ffd3205dc1717b60dc2ed89bb9953874fa53b4ee3d343be4e2db409`  
		Last Modified: Wed, 13 Jul 2022 07:49:29 GMT  
		Size: 857.2 KB (857153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e0914c16b380ff7a955c5cf1f69c21b835e52f6ac378a4b7323bfa168404007`  
		Last Modified: Wed, 13 Jul 2022 07:49:27 GMT  
		Size: 4.4 MB (4421847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71713f7372e7c03e17b0c0a4ef720ab6d7eb715efc80d2274f6e16588fbf0eae`  
		Last Modified: Wed, 13 Jul 2022 07:49:26 GMT  
		Size: 2.6 KB (2609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cad5804e4a57cfb046f1f19c286013ef3ffad8360b663613cad59978a512370`  
		Last Modified: Tue, 26 Jul 2022 23:56:57 GMT  
		Size: 333.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5308d3086645e729f0b6f0c42389abe0258a77941d250b2bdec734dcd408b41`  
		Last Modified: Tue, 26 Jul 2022 23:57:03 GMT  
		Size: 53.8 MB (53798288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5515cfa517579de894d15b5691fc09c6e6958e7a999a6dd419b9bb58a74c61d`  
		Last Modified: Tue, 26 Jul 2022 23:56:55 GMT  
		Size: 317.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44f33897b41dca1ed29f97e09e80baab85adc710313917c9164a9130f1cfc693`  
		Last Modified: Tue, 26 Jul 2022 23:57:03 GMT  
		Size: 44.1 MB (44108878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc195249cd1e03b936b46ede192667a7e83792b9f93f7ca837521293fb105494`  
		Last Modified: Tue, 26 Jul 2022 23:56:55 GMT  
		Size: 5.2 KB (5160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56ebae63daf8dd8c229ad24c897be15566d5416ab8bffe4f6d1719bf14e20b09`  
		Last Modified: Tue, 26 Jul 2022 23:56:55 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0.30`

```console
$ docker pull mysql@sha256:657d78ee56e09101902673adcdd7d2bf03012e759c1aa525eeca28cb0fe1aa7d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8.0.30` - linux; amd64

```console
$ docker pull mysql@sha256:13b312e01e8c6eca35c0ff251c261ca2e52994b2a71890539ad31dce8978fa15
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.5 MB (132512841 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38643ad93215bedea00fedd3d6f2a1c8e1bff3b9a172aa2547fd8b4bac9cfee3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 05 Jul 2022 22:20:34 GMT
ADD file:69555d6633d88e50ab2ddecc8bc5002a8f79005d828a9093975d68ca05b023e9 in / 
# Tue, 05 Jul 2022 22:20:34 GMT
CMD ["/bin/bash"]
# Wed, 13 Jul 2022 06:44:43 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 13 Jul 2022 06:44:43 GMT
ENV GOSU_VERSION=1.14
# Wed, 13 Jul 2022 06:44:46 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 13 Jul 2022 06:45:08 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Wed, 13 Jul 2022 06:45:09 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 13 Jul 2022 06:45:09 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 26 Jul 2022 23:27:21 GMT
ENV MYSQL_VERSION=8.0.30-1.el8
# Tue, 26 Jul 2022 23:27:22 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Tue, 26 Jul 2022 23:27:50 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Tue, 26 Jul 2022 23:27:51 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Tue, 26 Jul 2022 23:27:51 GMT
ENV MYSQL_SHELL_VERSION=8.0.30-1.el8
# Tue, 26 Jul 2022 23:28:22 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Tue, 26 Jul 2022 23:28:23 GMT
VOLUME [/var/lib/mysql]
# Tue, 26 Jul 2022 23:28:23 GMT
COPY file:d27cf504fa76fb5a4038020a01eaaf52723b17b751566119de311adacb043752 in /usr/local/bin/ 
# Tue, 26 Jul 2022 23:28:24 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 26 Jul 2022 23:28:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 26 Jul 2022 23:28:24 GMT
EXPOSE 3306 33060
# Tue, 26 Jul 2022 23:28:24 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:e54b73e95ef388354463a761e4e93ce3dac29cb244b2dc0424f2f4afc6ddf5cd`  
		Last Modified: Tue, 05 Jul 2022 22:21:41 GMT  
		Size: 39.2 MB (39222121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:327840d38cb25a590bbb16c433f0e05aa20ff9396d364afa42a6e26d24c6191c`  
		Last Modified: Wed, 13 Jul 2022 06:48:13 GMT  
		Size: 888.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:642077275f5f571c8f25c08b96faa535499c0eda0abe5d31a1dd5652828833b6`  
		Last Modified: Wed, 13 Jul 2022 06:48:13 GMT  
		Size: 928.8 KB (928836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e077469d560d641c3611653814fff9b3ae082c7b9fbdfb388a77ea34e49bf80f`  
		Last Modified: Wed, 13 Jul 2022 06:48:12 GMT  
		Size: 4.6 MB (4588162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbf214d981a6cf5e7e8da61fc840f0f5500ea6b91512f990b91e2d1e8cd6bea1`  
		Last Modified: Wed, 13 Jul 2022 06:48:11 GMT  
		Size: 2.6 KB (2631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4fda5f8b9a827b60600963d317db9cc284863fae5a963ba443cf2bb238f66c1`  
		Last Modified: Tue, 26 Jul 2022 23:30:30 GMT  
		Size: 336.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a41c2763043bfe2e0ecad80d96d0a451f3ed7141c8241418f484cc787c12023c`  
		Last Modified: Tue, 26 Jul 2022 23:30:36 GMT  
		Size: 47.7 MB (47732516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f86b3df6abb1f7fd5fe173a37be422608072ee6ce831b964a3076473ac14105a`  
		Last Modified: Tue, 26 Jul 2022 23:30:29 GMT  
		Size: 319.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95b1c2ed2ecfddca85150fe3e619638d7f71bcca106ad427e1fe8d513285a2fd`  
		Last Modified: Tue, 26 Jul 2022 23:30:36 GMT  
		Size: 40.0 MB (40031753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0edcd52771b148165e0ca520d3e3981ca95e94e9abcc3c895586a0caf919d7f`  
		Last Modified: Tue, 26 Jul 2022 23:30:28 GMT  
		Size: 5.2 KB (5159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3d312b5c835845f301e964bb6bd231671dc089225f6d4457eb636b7fabfad5e`  
		Last Modified: Tue, 26 Jul 2022 23:30:28 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8.0.30` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:2375bf5d81d54f400d6af809fe60c1af2e0252e7d5b65bb65a80ca844ee3338e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.2 MB (141223352 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a75af66873e7bc730c1934b1d7319e5c3cf1eb3f26c72653ebfaba0af229c25`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 05 Jul 2022 22:43:14 GMT
ADD file:e864e9187ff57bc1df9611a0990052f89611bfe7b6bc8e3d24b500b0886ec725 in / 
# Tue, 05 Jul 2022 22:43:14 GMT
CMD ["/bin/bash"]
# Wed, 13 Jul 2022 07:47:27 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 13 Jul 2022 07:47:27 GMT
ENV GOSU_VERSION=1.14
# Wed, 13 Jul 2022 07:47:31 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 13 Jul 2022 07:47:52 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Wed, 13 Jul 2022 07:47:54 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 13 Jul 2022 07:47:55 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 26 Jul 2022 23:55:24 GMT
ENV MYSQL_VERSION=8.0.30-1.el8
# Tue, 26 Jul 2022 23:55:25 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Tue, 26 Jul 2022 23:55:53 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Tue, 26 Jul 2022 23:55:54 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Tue, 26 Jul 2022 23:55:54 GMT
ENV MYSQL_SHELL_VERSION=8.0.30-1.el8
# Tue, 26 Jul 2022 23:56:24 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Tue, 26 Jul 2022 23:56:24 GMT
VOLUME [/var/lib/mysql]
# Tue, 26 Jul 2022 23:56:26 GMT
COPY file:d27cf504fa76fb5a4038020a01eaaf52723b17b751566119de311adacb043752 in /usr/local/bin/ 
# Tue, 26 Jul 2022 23:56:27 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 26 Jul 2022 23:56:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 26 Jul 2022 23:56:28 GMT
EXPOSE 3306 33060
# Tue, 26 Jul 2022 23:56:29 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:e5d41499b4049578ed8bbb14817cd79d4136a84899b65e4364b0125d4d1c792c`  
		Last Modified: Tue, 05 Jul 2022 22:44:31 GMT  
		Size: 38.0 MB (38027757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c14e53563050114db97e64919184751150f664c330508d7e443fb5408550cc04`  
		Last Modified: Wed, 13 Jul 2022 07:49:28 GMT  
		Size: 889.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:024772013ffd3205dc1717b60dc2ed89bb9953874fa53b4ee3d343be4e2db409`  
		Last Modified: Wed, 13 Jul 2022 07:49:29 GMT  
		Size: 857.2 KB (857153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e0914c16b380ff7a955c5cf1f69c21b835e52f6ac378a4b7323bfa168404007`  
		Last Modified: Wed, 13 Jul 2022 07:49:27 GMT  
		Size: 4.4 MB (4421847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71713f7372e7c03e17b0c0a4ef720ab6d7eb715efc80d2274f6e16588fbf0eae`  
		Last Modified: Wed, 13 Jul 2022 07:49:26 GMT  
		Size: 2.6 KB (2609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cad5804e4a57cfb046f1f19c286013ef3ffad8360b663613cad59978a512370`  
		Last Modified: Tue, 26 Jul 2022 23:56:57 GMT  
		Size: 333.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5308d3086645e729f0b6f0c42389abe0258a77941d250b2bdec734dcd408b41`  
		Last Modified: Tue, 26 Jul 2022 23:57:03 GMT  
		Size: 53.8 MB (53798288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5515cfa517579de894d15b5691fc09c6e6958e7a999a6dd419b9bb58a74c61d`  
		Last Modified: Tue, 26 Jul 2022 23:56:55 GMT  
		Size: 317.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44f33897b41dca1ed29f97e09e80baab85adc710313917c9164a9130f1cfc693`  
		Last Modified: Tue, 26 Jul 2022 23:57:03 GMT  
		Size: 44.1 MB (44108878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc195249cd1e03b936b46ede192667a7e83792b9f93f7ca837521293fb105494`  
		Last Modified: Tue, 26 Jul 2022 23:56:55 GMT  
		Size: 5.2 KB (5160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56ebae63daf8dd8c229ad24c897be15566d5416ab8bffe4f6d1719bf14e20b09`  
		Last Modified: Tue, 26 Jul 2022 23:56:55 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0.30-debian`

```console
$ docker pull mysql@sha256:504760f722770e8554c40e7ea6b803ae9e0c19e21e25b94d0b8a03bab20541ff
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:8.0.30-debian` - linux; amd64

```console
$ docker pull mysql@sha256:9a16d88a3410a326a082261a64db5624902fc763775410663cc44420968831a3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **157.8 MB (157835607 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c2ee58f241ef6265fbc87840afec971c52938a5bcc38259e71bb0ad0363e827e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 12 Jul 2022 01:20:10 GMT
ADD file:d978f6d3025a06f5142a0c13c98bf12fbd47cdf9162ed31fbc05c86983b0a679 in / 
# Tue, 12 Jul 2022 01:20:10 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 01:49:49 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 12 Jul 2022 01:49:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 01:49:56 GMT
ENV GOSU_VERSION=1.14
# Tue, 12 Jul 2022 01:50:05 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 12 Jul 2022 01:50:05 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 12 Jul 2022 01:50:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 01:50:12 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Tue, 12 Jul 2022 01:50:12 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 26 Jul 2022 23:28:31 GMT
ENV MYSQL_VERSION=8.0.30-1debian11
# Tue, 26 Jul 2022 23:28:31 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ bullseye mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Tue, 26 Jul 2022 23:28:45 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 26 Jul 2022 23:28:45 GMT
VOLUME [/var/lib/mysql]
# Tue, 26 Jul 2022 23:28:45 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Tue, 26 Jul 2022 23:28:46 GMT
COPY file:d27cf504fa76fb5a4038020a01eaaf52723b17b751566119de311adacb043752 in /usr/local/bin/ 
# Tue, 26 Jul 2022 23:28:46 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 26 Jul 2022 23:28:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 26 Jul 2022 23:28:46 GMT
EXPOSE 3306 33060
# Tue, 26 Jul 2022 23:28:46 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:461246efe0a75316d99afdbf348f7063b57b0caeee8daab775f1f08152ea36f4`  
		Last Modified: Tue, 12 Jul 2022 01:24:34 GMT  
		Size: 31.4 MB (31366610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1cd5bb1f5de5503f17b383d7c62078467389f82828ac46a41db64289ecf9880`  
		Last Modified: Tue, 12 Jul 2022 01:52:26 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd9d402d85bd06018ec1a89d3298f4d88f3c4d06c2cd93c8951d8bbb19596ace`  
		Last Modified: Tue, 12 Jul 2022 01:52:26 GMT  
		Size: 4.4 MB (4414786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33a04621f5daa2ee95b4484e11cb963f929686d8f77511d9e31d8cf63d2a491b`  
		Last Modified: Tue, 12 Jul 2022 01:52:24 GMT  
		Size: 1.4 MB (1418425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2eef8024049f6e7f8a7769c0ed43bc5ddab7c1b3dbc772a3ba1b71a039bff03`  
		Last Modified: Tue, 12 Jul 2022 01:52:23 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a021c48082a6778bc62f96a17b8202ad24185d41b54fad0c4788d55e18a106b1`  
		Last Modified: Tue, 12 Jul 2022 01:52:26 GMT  
		Size: 12.7 MB (12661669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a27a84090d2f2cc8e7bc9db5098fe5f2c61aaf38e003421fab9630fdf6541c2`  
		Last Modified: Tue, 12 Jul 2022 01:52:23 GMT  
		Size: 2.5 KB (2547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40bc66f09ecd05d38547cb872afb8703d21702dcbd68f1688e69c1fa899b9bfe`  
		Last Modified: Tue, 26 Jul 2022 23:31:05 GMT  
		Size: 256.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57a0b87a3f7d2dd5b0a2ba39b526929f321b90da90a2249caf4da175b9b19e70`  
		Last Modified: Tue, 26 Jul 2022 23:31:22 GMT  
		Size: 108.0 MB (107963313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44e82ef1aa7cd91168ba63bd5724afa619590e17c79d641515a3a0f23bf75839`  
		Last Modified: Tue, 26 Jul 2022 23:31:05 GMT  
		Size: 842.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f04800ad7ccd34e26a26464cfa045c9030672e0bc018c05b370e55acce1d02e`  
		Last Modified: Tue, 26 Jul 2022 23:31:05 GMT  
		Size: 5.2 KB (5157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6593ab5ec7351b0dba0042dd7086bb2ae362d26cd4c7be288dfc618a7884ea15`  
		Last Modified: Tue, 26 Jul 2022 23:31:05 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0.30-oracle`

```console
$ docker pull mysql@sha256:657d78ee56e09101902673adcdd7d2bf03012e759c1aa525eeca28cb0fe1aa7d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8.0.30-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:13b312e01e8c6eca35c0ff251c261ca2e52994b2a71890539ad31dce8978fa15
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.5 MB (132512841 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38643ad93215bedea00fedd3d6f2a1c8e1bff3b9a172aa2547fd8b4bac9cfee3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 05 Jul 2022 22:20:34 GMT
ADD file:69555d6633d88e50ab2ddecc8bc5002a8f79005d828a9093975d68ca05b023e9 in / 
# Tue, 05 Jul 2022 22:20:34 GMT
CMD ["/bin/bash"]
# Wed, 13 Jul 2022 06:44:43 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 13 Jul 2022 06:44:43 GMT
ENV GOSU_VERSION=1.14
# Wed, 13 Jul 2022 06:44:46 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 13 Jul 2022 06:45:08 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Wed, 13 Jul 2022 06:45:09 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 13 Jul 2022 06:45:09 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 26 Jul 2022 23:27:21 GMT
ENV MYSQL_VERSION=8.0.30-1.el8
# Tue, 26 Jul 2022 23:27:22 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Tue, 26 Jul 2022 23:27:50 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Tue, 26 Jul 2022 23:27:51 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Tue, 26 Jul 2022 23:27:51 GMT
ENV MYSQL_SHELL_VERSION=8.0.30-1.el8
# Tue, 26 Jul 2022 23:28:22 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Tue, 26 Jul 2022 23:28:23 GMT
VOLUME [/var/lib/mysql]
# Tue, 26 Jul 2022 23:28:23 GMT
COPY file:d27cf504fa76fb5a4038020a01eaaf52723b17b751566119de311adacb043752 in /usr/local/bin/ 
# Tue, 26 Jul 2022 23:28:24 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 26 Jul 2022 23:28:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 26 Jul 2022 23:28:24 GMT
EXPOSE 3306 33060
# Tue, 26 Jul 2022 23:28:24 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:e54b73e95ef388354463a761e4e93ce3dac29cb244b2dc0424f2f4afc6ddf5cd`  
		Last Modified: Tue, 05 Jul 2022 22:21:41 GMT  
		Size: 39.2 MB (39222121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:327840d38cb25a590bbb16c433f0e05aa20ff9396d364afa42a6e26d24c6191c`  
		Last Modified: Wed, 13 Jul 2022 06:48:13 GMT  
		Size: 888.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:642077275f5f571c8f25c08b96faa535499c0eda0abe5d31a1dd5652828833b6`  
		Last Modified: Wed, 13 Jul 2022 06:48:13 GMT  
		Size: 928.8 KB (928836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e077469d560d641c3611653814fff9b3ae082c7b9fbdfb388a77ea34e49bf80f`  
		Last Modified: Wed, 13 Jul 2022 06:48:12 GMT  
		Size: 4.6 MB (4588162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbf214d981a6cf5e7e8da61fc840f0f5500ea6b91512f990b91e2d1e8cd6bea1`  
		Last Modified: Wed, 13 Jul 2022 06:48:11 GMT  
		Size: 2.6 KB (2631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4fda5f8b9a827b60600963d317db9cc284863fae5a963ba443cf2bb238f66c1`  
		Last Modified: Tue, 26 Jul 2022 23:30:30 GMT  
		Size: 336.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a41c2763043bfe2e0ecad80d96d0a451f3ed7141c8241418f484cc787c12023c`  
		Last Modified: Tue, 26 Jul 2022 23:30:36 GMT  
		Size: 47.7 MB (47732516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f86b3df6abb1f7fd5fe173a37be422608072ee6ce831b964a3076473ac14105a`  
		Last Modified: Tue, 26 Jul 2022 23:30:29 GMT  
		Size: 319.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95b1c2ed2ecfddca85150fe3e619638d7f71bcca106ad427e1fe8d513285a2fd`  
		Last Modified: Tue, 26 Jul 2022 23:30:36 GMT  
		Size: 40.0 MB (40031753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0edcd52771b148165e0ca520d3e3981ca95e94e9abcc3c895586a0caf919d7f`  
		Last Modified: Tue, 26 Jul 2022 23:30:28 GMT  
		Size: 5.2 KB (5159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3d312b5c835845f301e964bb6bd231671dc089225f6d4457eb636b7fabfad5e`  
		Last Modified: Tue, 26 Jul 2022 23:30:28 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8.0.30-oracle` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:2375bf5d81d54f400d6af809fe60c1af2e0252e7d5b65bb65a80ca844ee3338e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.2 MB (141223352 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a75af66873e7bc730c1934b1d7319e5c3cf1eb3f26c72653ebfaba0af229c25`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 05 Jul 2022 22:43:14 GMT
ADD file:e864e9187ff57bc1df9611a0990052f89611bfe7b6bc8e3d24b500b0886ec725 in / 
# Tue, 05 Jul 2022 22:43:14 GMT
CMD ["/bin/bash"]
# Wed, 13 Jul 2022 07:47:27 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 13 Jul 2022 07:47:27 GMT
ENV GOSU_VERSION=1.14
# Wed, 13 Jul 2022 07:47:31 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 13 Jul 2022 07:47:52 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Wed, 13 Jul 2022 07:47:54 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 13 Jul 2022 07:47:55 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 26 Jul 2022 23:55:24 GMT
ENV MYSQL_VERSION=8.0.30-1.el8
# Tue, 26 Jul 2022 23:55:25 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Tue, 26 Jul 2022 23:55:53 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Tue, 26 Jul 2022 23:55:54 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Tue, 26 Jul 2022 23:55:54 GMT
ENV MYSQL_SHELL_VERSION=8.0.30-1.el8
# Tue, 26 Jul 2022 23:56:24 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Tue, 26 Jul 2022 23:56:24 GMT
VOLUME [/var/lib/mysql]
# Tue, 26 Jul 2022 23:56:26 GMT
COPY file:d27cf504fa76fb5a4038020a01eaaf52723b17b751566119de311adacb043752 in /usr/local/bin/ 
# Tue, 26 Jul 2022 23:56:27 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 26 Jul 2022 23:56:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 26 Jul 2022 23:56:28 GMT
EXPOSE 3306 33060
# Tue, 26 Jul 2022 23:56:29 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:e5d41499b4049578ed8bbb14817cd79d4136a84899b65e4364b0125d4d1c792c`  
		Last Modified: Tue, 05 Jul 2022 22:44:31 GMT  
		Size: 38.0 MB (38027757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c14e53563050114db97e64919184751150f664c330508d7e443fb5408550cc04`  
		Last Modified: Wed, 13 Jul 2022 07:49:28 GMT  
		Size: 889.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:024772013ffd3205dc1717b60dc2ed89bb9953874fa53b4ee3d343be4e2db409`  
		Last Modified: Wed, 13 Jul 2022 07:49:29 GMT  
		Size: 857.2 KB (857153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e0914c16b380ff7a955c5cf1f69c21b835e52f6ac378a4b7323bfa168404007`  
		Last Modified: Wed, 13 Jul 2022 07:49:27 GMT  
		Size: 4.4 MB (4421847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71713f7372e7c03e17b0c0a4ef720ab6d7eb715efc80d2274f6e16588fbf0eae`  
		Last Modified: Wed, 13 Jul 2022 07:49:26 GMT  
		Size: 2.6 KB (2609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cad5804e4a57cfb046f1f19c286013ef3ffad8360b663613cad59978a512370`  
		Last Modified: Tue, 26 Jul 2022 23:56:57 GMT  
		Size: 333.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5308d3086645e729f0b6f0c42389abe0258a77941d250b2bdec734dcd408b41`  
		Last Modified: Tue, 26 Jul 2022 23:57:03 GMT  
		Size: 53.8 MB (53798288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5515cfa517579de894d15b5691fc09c6e6958e7a999a6dd419b9bb58a74c61d`  
		Last Modified: Tue, 26 Jul 2022 23:56:55 GMT  
		Size: 317.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44f33897b41dca1ed29f97e09e80baab85adc710313917c9164a9130f1cfc693`  
		Last Modified: Tue, 26 Jul 2022 23:57:03 GMT  
		Size: 44.1 MB (44108878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc195249cd1e03b936b46ede192667a7e83792b9f93f7ca837521293fb105494`  
		Last Modified: Tue, 26 Jul 2022 23:56:55 GMT  
		Size: 5.2 KB (5160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56ebae63daf8dd8c229ad24c897be15566d5416ab8bffe4f6d1719bf14e20b09`  
		Last Modified: Tue, 26 Jul 2022 23:56:55 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:debian`

```console
$ docker pull mysql@sha256:504760f722770e8554c40e7ea6b803ae9e0c19e21e25b94d0b8a03bab20541ff
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:debian` - linux; amd64

```console
$ docker pull mysql@sha256:9a16d88a3410a326a082261a64db5624902fc763775410663cc44420968831a3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **157.8 MB (157835607 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c2ee58f241ef6265fbc87840afec971c52938a5bcc38259e71bb0ad0363e827e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 12 Jul 2022 01:20:10 GMT
ADD file:d978f6d3025a06f5142a0c13c98bf12fbd47cdf9162ed31fbc05c86983b0a679 in / 
# Tue, 12 Jul 2022 01:20:10 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 01:49:49 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 12 Jul 2022 01:49:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 01:49:56 GMT
ENV GOSU_VERSION=1.14
# Tue, 12 Jul 2022 01:50:05 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 12 Jul 2022 01:50:05 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 12 Jul 2022 01:50:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 01:50:12 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Tue, 12 Jul 2022 01:50:12 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 26 Jul 2022 23:28:31 GMT
ENV MYSQL_VERSION=8.0.30-1debian11
# Tue, 26 Jul 2022 23:28:31 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ bullseye mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Tue, 26 Jul 2022 23:28:45 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 26 Jul 2022 23:28:45 GMT
VOLUME [/var/lib/mysql]
# Tue, 26 Jul 2022 23:28:45 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Tue, 26 Jul 2022 23:28:46 GMT
COPY file:d27cf504fa76fb5a4038020a01eaaf52723b17b751566119de311adacb043752 in /usr/local/bin/ 
# Tue, 26 Jul 2022 23:28:46 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 26 Jul 2022 23:28:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 26 Jul 2022 23:28:46 GMT
EXPOSE 3306 33060
# Tue, 26 Jul 2022 23:28:46 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:461246efe0a75316d99afdbf348f7063b57b0caeee8daab775f1f08152ea36f4`  
		Last Modified: Tue, 12 Jul 2022 01:24:34 GMT  
		Size: 31.4 MB (31366610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1cd5bb1f5de5503f17b383d7c62078467389f82828ac46a41db64289ecf9880`  
		Last Modified: Tue, 12 Jul 2022 01:52:26 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd9d402d85bd06018ec1a89d3298f4d88f3c4d06c2cd93c8951d8bbb19596ace`  
		Last Modified: Tue, 12 Jul 2022 01:52:26 GMT  
		Size: 4.4 MB (4414786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33a04621f5daa2ee95b4484e11cb963f929686d8f77511d9e31d8cf63d2a491b`  
		Last Modified: Tue, 12 Jul 2022 01:52:24 GMT  
		Size: 1.4 MB (1418425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2eef8024049f6e7f8a7769c0ed43bc5ddab7c1b3dbc772a3ba1b71a039bff03`  
		Last Modified: Tue, 12 Jul 2022 01:52:23 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a021c48082a6778bc62f96a17b8202ad24185d41b54fad0c4788d55e18a106b1`  
		Last Modified: Tue, 12 Jul 2022 01:52:26 GMT  
		Size: 12.7 MB (12661669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a27a84090d2f2cc8e7bc9db5098fe5f2c61aaf38e003421fab9630fdf6541c2`  
		Last Modified: Tue, 12 Jul 2022 01:52:23 GMT  
		Size: 2.5 KB (2547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40bc66f09ecd05d38547cb872afb8703d21702dcbd68f1688e69c1fa899b9bfe`  
		Last Modified: Tue, 26 Jul 2022 23:31:05 GMT  
		Size: 256.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57a0b87a3f7d2dd5b0a2ba39b526929f321b90da90a2249caf4da175b9b19e70`  
		Last Modified: Tue, 26 Jul 2022 23:31:22 GMT  
		Size: 108.0 MB (107963313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44e82ef1aa7cd91168ba63bd5724afa619590e17c79d641515a3a0f23bf75839`  
		Last Modified: Tue, 26 Jul 2022 23:31:05 GMT  
		Size: 842.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f04800ad7ccd34e26a26464cfa045c9030672e0bc018c05b370e55acce1d02e`  
		Last Modified: Tue, 26 Jul 2022 23:31:05 GMT  
		Size: 5.2 KB (5157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6593ab5ec7351b0dba0042dd7086bb2ae362d26cd4c7be288dfc618a7884ea15`  
		Last Modified: Tue, 26 Jul 2022 23:31:05 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:latest`

```console
$ docker pull mysql@sha256:657d78ee56e09101902673adcdd7d2bf03012e759c1aa525eeca28cb0fe1aa7d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:latest` - linux; amd64

```console
$ docker pull mysql@sha256:13b312e01e8c6eca35c0ff251c261ca2e52994b2a71890539ad31dce8978fa15
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.5 MB (132512841 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38643ad93215bedea00fedd3d6f2a1c8e1bff3b9a172aa2547fd8b4bac9cfee3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 05 Jul 2022 22:20:34 GMT
ADD file:69555d6633d88e50ab2ddecc8bc5002a8f79005d828a9093975d68ca05b023e9 in / 
# Tue, 05 Jul 2022 22:20:34 GMT
CMD ["/bin/bash"]
# Wed, 13 Jul 2022 06:44:43 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 13 Jul 2022 06:44:43 GMT
ENV GOSU_VERSION=1.14
# Wed, 13 Jul 2022 06:44:46 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 13 Jul 2022 06:45:08 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Wed, 13 Jul 2022 06:45:09 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 13 Jul 2022 06:45:09 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 26 Jul 2022 23:27:21 GMT
ENV MYSQL_VERSION=8.0.30-1.el8
# Tue, 26 Jul 2022 23:27:22 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Tue, 26 Jul 2022 23:27:50 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Tue, 26 Jul 2022 23:27:51 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Tue, 26 Jul 2022 23:27:51 GMT
ENV MYSQL_SHELL_VERSION=8.0.30-1.el8
# Tue, 26 Jul 2022 23:28:22 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Tue, 26 Jul 2022 23:28:23 GMT
VOLUME [/var/lib/mysql]
# Tue, 26 Jul 2022 23:28:23 GMT
COPY file:d27cf504fa76fb5a4038020a01eaaf52723b17b751566119de311adacb043752 in /usr/local/bin/ 
# Tue, 26 Jul 2022 23:28:24 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 26 Jul 2022 23:28:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 26 Jul 2022 23:28:24 GMT
EXPOSE 3306 33060
# Tue, 26 Jul 2022 23:28:24 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:e54b73e95ef388354463a761e4e93ce3dac29cb244b2dc0424f2f4afc6ddf5cd`  
		Last Modified: Tue, 05 Jul 2022 22:21:41 GMT  
		Size: 39.2 MB (39222121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:327840d38cb25a590bbb16c433f0e05aa20ff9396d364afa42a6e26d24c6191c`  
		Last Modified: Wed, 13 Jul 2022 06:48:13 GMT  
		Size: 888.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:642077275f5f571c8f25c08b96faa535499c0eda0abe5d31a1dd5652828833b6`  
		Last Modified: Wed, 13 Jul 2022 06:48:13 GMT  
		Size: 928.8 KB (928836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e077469d560d641c3611653814fff9b3ae082c7b9fbdfb388a77ea34e49bf80f`  
		Last Modified: Wed, 13 Jul 2022 06:48:12 GMT  
		Size: 4.6 MB (4588162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbf214d981a6cf5e7e8da61fc840f0f5500ea6b91512f990b91e2d1e8cd6bea1`  
		Last Modified: Wed, 13 Jul 2022 06:48:11 GMT  
		Size: 2.6 KB (2631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4fda5f8b9a827b60600963d317db9cc284863fae5a963ba443cf2bb238f66c1`  
		Last Modified: Tue, 26 Jul 2022 23:30:30 GMT  
		Size: 336.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a41c2763043bfe2e0ecad80d96d0a451f3ed7141c8241418f484cc787c12023c`  
		Last Modified: Tue, 26 Jul 2022 23:30:36 GMT  
		Size: 47.7 MB (47732516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f86b3df6abb1f7fd5fe173a37be422608072ee6ce831b964a3076473ac14105a`  
		Last Modified: Tue, 26 Jul 2022 23:30:29 GMT  
		Size: 319.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95b1c2ed2ecfddca85150fe3e619638d7f71bcca106ad427e1fe8d513285a2fd`  
		Last Modified: Tue, 26 Jul 2022 23:30:36 GMT  
		Size: 40.0 MB (40031753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0edcd52771b148165e0ca520d3e3981ca95e94e9abcc3c895586a0caf919d7f`  
		Last Modified: Tue, 26 Jul 2022 23:30:28 GMT  
		Size: 5.2 KB (5159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3d312b5c835845f301e964bb6bd231671dc089225f6d4457eb636b7fabfad5e`  
		Last Modified: Tue, 26 Jul 2022 23:30:28 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:latest` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:2375bf5d81d54f400d6af809fe60c1af2e0252e7d5b65bb65a80ca844ee3338e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.2 MB (141223352 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a75af66873e7bc730c1934b1d7319e5c3cf1eb3f26c72653ebfaba0af229c25`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 05 Jul 2022 22:43:14 GMT
ADD file:e864e9187ff57bc1df9611a0990052f89611bfe7b6bc8e3d24b500b0886ec725 in / 
# Tue, 05 Jul 2022 22:43:14 GMT
CMD ["/bin/bash"]
# Wed, 13 Jul 2022 07:47:27 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 13 Jul 2022 07:47:27 GMT
ENV GOSU_VERSION=1.14
# Wed, 13 Jul 2022 07:47:31 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 13 Jul 2022 07:47:52 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Wed, 13 Jul 2022 07:47:54 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 13 Jul 2022 07:47:55 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 26 Jul 2022 23:55:24 GMT
ENV MYSQL_VERSION=8.0.30-1.el8
# Tue, 26 Jul 2022 23:55:25 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Tue, 26 Jul 2022 23:55:53 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Tue, 26 Jul 2022 23:55:54 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Tue, 26 Jul 2022 23:55:54 GMT
ENV MYSQL_SHELL_VERSION=8.0.30-1.el8
# Tue, 26 Jul 2022 23:56:24 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Tue, 26 Jul 2022 23:56:24 GMT
VOLUME [/var/lib/mysql]
# Tue, 26 Jul 2022 23:56:26 GMT
COPY file:d27cf504fa76fb5a4038020a01eaaf52723b17b751566119de311adacb043752 in /usr/local/bin/ 
# Tue, 26 Jul 2022 23:56:27 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 26 Jul 2022 23:56:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 26 Jul 2022 23:56:28 GMT
EXPOSE 3306 33060
# Tue, 26 Jul 2022 23:56:29 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:e5d41499b4049578ed8bbb14817cd79d4136a84899b65e4364b0125d4d1c792c`  
		Last Modified: Tue, 05 Jul 2022 22:44:31 GMT  
		Size: 38.0 MB (38027757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c14e53563050114db97e64919184751150f664c330508d7e443fb5408550cc04`  
		Last Modified: Wed, 13 Jul 2022 07:49:28 GMT  
		Size: 889.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:024772013ffd3205dc1717b60dc2ed89bb9953874fa53b4ee3d343be4e2db409`  
		Last Modified: Wed, 13 Jul 2022 07:49:29 GMT  
		Size: 857.2 KB (857153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e0914c16b380ff7a955c5cf1f69c21b835e52f6ac378a4b7323bfa168404007`  
		Last Modified: Wed, 13 Jul 2022 07:49:27 GMT  
		Size: 4.4 MB (4421847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71713f7372e7c03e17b0c0a4ef720ab6d7eb715efc80d2274f6e16588fbf0eae`  
		Last Modified: Wed, 13 Jul 2022 07:49:26 GMT  
		Size: 2.6 KB (2609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cad5804e4a57cfb046f1f19c286013ef3ffad8360b663613cad59978a512370`  
		Last Modified: Tue, 26 Jul 2022 23:56:57 GMT  
		Size: 333.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5308d3086645e729f0b6f0c42389abe0258a77941d250b2bdec734dcd408b41`  
		Last Modified: Tue, 26 Jul 2022 23:57:03 GMT  
		Size: 53.8 MB (53798288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5515cfa517579de894d15b5691fc09c6e6958e7a999a6dd419b9bb58a74c61d`  
		Last Modified: Tue, 26 Jul 2022 23:56:55 GMT  
		Size: 317.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44f33897b41dca1ed29f97e09e80baab85adc710313917c9164a9130f1cfc693`  
		Last Modified: Tue, 26 Jul 2022 23:57:03 GMT  
		Size: 44.1 MB (44108878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc195249cd1e03b936b46ede192667a7e83792b9f93f7ca837521293fb105494`  
		Last Modified: Tue, 26 Jul 2022 23:56:55 GMT  
		Size: 5.2 KB (5160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56ebae63daf8dd8c229ad24c897be15566d5416ab8bffe4f6d1719bf14e20b09`  
		Last Modified: Tue, 26 Jul 2022 23:56:55 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:oracle`

```console
$ docker pull mysql@sha256:657d78ee56e09101902673adcdd7d2bf03012e759c1aa525eeca28cb0fe1aa7d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:oracle` - linux; amd64

```console
$ docker pull mysql@sha256:13b312e01e8c6eca35c0ff251c261ca2e52994b2a71890539ad31dce8978fa15
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.5 MB (132512841 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38643ad93215bedea00fedd3d6f2a1c8e1bff3b9a172aa2547fd8b4bac9cfee3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 05 Jul 2022 22:20:34 GMT
ADD file:69555d6633d88e50ab2ddecc8bc5002a8f79005d828a9093975d68ca05b023e9 in / 
# Tue, 05 Jul 2022 22:20:34 GMT
CMD ["/bin/bash"]
# Wed, 13 Jul 2022 06:44:43 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 13 Jul 2022 06:44:43 GMT
ENV GOSU_VERSION=1.14
# Wed, 13 Jul 2022 06:44:46 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 13 Jul 2022 06:45:08 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Wed, 13 Jul 2022 06:45:09 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 13 Jul 2022 06:45:09 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 26 Jul 2022 23:27:21 GMT
ENV MYSQL_VERSION=8.0.30-1.el8
# Tue, 26 Jul 2022 23:27:22 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Tue, 26 Jul 2022 23:27:50 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Tue, 26 Jul 2022 23:27:51 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Tue, 26 Jul 2022 23:27:51 GMT
ENV MYSQL_SHELL_VERSION=8.0.30-1.el8
# Tue, 26 Jul 2022 23:28:22 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Tue, 26 Jul 2022 23:28:23 GMT
VOLUME [/var/lib/mysql]
# Tue, 26 Jul 2022 23:28:23 GMT
COPY file:d27cf504fa76fb5a4038020a01eaaf52723b17b751566119de311adacb043752 in /usr/local/bin/ 
# Tue, 26 Jul 2022 23:28:24 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 26 Jul 2022 23:28:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 26 Jul 2022 23:28:24 GMT
EXPOSE 3306 33060
# Tue, 26 Jul 2022 23:28:24 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:e54b73e95ef388354463a761e4e93ce3dac29cb244b2dc0424f2f4afc6ddf5cd`  
		Last Modified: Tue, 05 Jul 2022 22:21:41 GMT  
		Size: 39.2 MB (39222121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:327840d38cb25a590bbb16c433f0e05aa20ff9396d364afa42a6e26d24c6191c`  
		Last Modified: Wed, 13 Jul 2022 06:48:13 GMT  
		Size: 888.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:642077275f5f571c8f25c08b96faa535499c0eda0abe5d31a1dd5652828833b6`  
		Last Modified: Wed, 13 Jul 2022 06:48:13 GMT  
		Size: 928.8 KB (928836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e077469d560d641c3611653814fff9b3ae082c7b9fbdfb388a77ea34e49bf80f`  
		Last Modified: Wed, 13 Jul 2022 06:48:12 GMT  
		Size: 4.6 MB (4588162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbf214d981a6cf5e7e8da61fc840f0f5500ea6b91512f990b91e2d1e8cd6bea1`  
		Last Modified: Wed, 13 Jul 2022 06:48:11 GMT  
		Size: 2.6 KB (2631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4fda5f8b9a827b60600963d317db9cc284863fae5a963ba443cf2bb238f66c1`  
		Last Modified: Tue, 26 Jul 2022 23:30:30 GMT  
		Size: 336.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a41c2763043bfe2e0ecad80d96d0a451f3ed7141c8241418f484cc787c12023c`  
		Last Modified: Tue, 26 Jul 2022 23:30:36 GMT  
		Size: 47.7 MB (47732516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f86b3df6abb1f7fd5fe173a37be422608072ee6ce831b964a3076473ac14105a`  
		Last Modified: Tue, 26 Jul 2022 23:30:29 GMT  
		Size: 319.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95b1c2ed2ecfddca85150fe3e619638d7f71bcca106ad427e1fe8d513285a2fd`  
		Last Modified: Tue, 26 Jul 2022 23:30:36 GMT  
		Size: 40.0 MB (40031753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0edcd52771b148165e0ca520d3e3981ca95e94e9abcc3c895586a0caf919d7f`  
		Last Modified: Tue, 26 Jul 2022 23:30:28 GMT  
		Size: 5.2 KB (5159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3d312b5c835845f301e964bb6bd231671dc089225f6d4457eb636b7fabfad5e`  
		Last Modified: Tue, 26 Jul 2022 23:30:28 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:oracle` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:2375bf5d81d54f400d6af809fe60c1af2e0252e7d5b65bb65a80ca844ee3338e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.2 MB (141223352 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a75af66873e7bc730c1934b1d7319e5c3cf1eb3f26c72653ebfaba0af229c25`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 05 Jul 2022 22:43:14 GMT
ADD file:e864e9187ff57bc1df9611a0990052f89611bfe7b6bc8e3d24b500b0886ec725 in / 
# Tue, 05 Jul 2022 22:43:14 GMT
CMD ["/bin/bash"]
# Wed, 13 Jul 2022 07:47:27 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 13 Jul 2022 07:47:27 GMT
ENV GOSU_VERSION=1.14
# Wed, 13 Jul 2022 07:47:31 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 13 Jul 2022 07:47:52 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Wed, 13 Jul 2022 07:47:54 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 13 Jul 2022 07:47:55 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 26 Jul 2022 23:55:24 GMT
ENV MYSQL_VERSION=8.0.30-1.el8
# Tue, 26 Jul 2022 23:55:25 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Tue, 26 Jul 2022 23:55:53 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Tue, 26 Jul 2022 23:55:54 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Tue, 26 Jul 2022 23:55:54 GMT
ENV MYSQL_SHELL_VERSION=8.0.30-1.el8
# Tue, 26 Jul 2022 23:56:24 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Tue, 26 Jul 2022 23:56:24 GMT
VOLUME [/var/lib/mysql]
# Tue, 26 Jul 2022 23:56:26 GMT
COPY file:d27cf504fa76fb5a4038020a01eaaf52723b17b751566119de311adacb043752 in /usr/local/bin/ 
# Tue, 26 Jul 2022 23:56:27 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 26 Jul 2022 23:56:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 26 Jul 2022 23:56:28 GMT
EXPOSE 3306 33060
# Tue, 26 Jul 2022 23:56:29 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:e5d41499b4049578ed8bbb14817cd79d4136a84899b65e4364b0125d4d1c792c`  
		Last Modified: Tue, 05 Jul 2022 22:44:31 GMT  
		Size: 38.0 MB (38027757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c14e53563050114db97e64919184751150f664c330508d7e443fb5408550cc04`  
		Last Modified: Wed, 13 Jul 2022 07:49:28 GMT  
		Size: 889.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:024772013ffd3205dc1717b60dc2ed89bb9953874fa53b4ee3d343be4e2db409`  
		Last Modified: Wed, 13 Jul 2022 07:49:29 GMT  
		Size: 857.2 KB (857153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e0914c16b380ff7a955c5cf1f69c21b835e52f6ac378a4b7323bfa168404007`  
		Last Modified: Wed, 13 Jul 2022 07:49:27 GMT  
		Size: 4.4 MB (4421847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71713f7372e7c03e17b0c0a4ef720ab6d7eb715efc80d2274f6e16588fbf0eae`  
		Last Modified: Wed, 13 Jul 2022 07:49:26 GMT  
		Size: 2.6 KB (2609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cad5804e4a57cfb046f1f19c286013ef3ffad8360b663613cad59978a512370`  
		Last Modified: Tue, 26 Jul 2022 23:56:57 GMT  
		Size: 333.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5308d3086645e729f0b6f0c42389abe0258a77941d250b2bdec734dcd408b41`  
		Last Modified: Tue, 26 Jul 2022 23:57:03 GMT  
		Size: 53.8 MB (53798288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5515cfa517579de894d15b5691fc09c6e6958e7a999a6dd419b9bb58a74c61d`  
		Last Modified: Tue, 26 Jul 2022 23:56:55 GMT  
		Size: 317.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44f33897b41dca1ed29f97e09e80baab85adc710313917c9164a9130f1cfc693`  
		Last Modified: Tue, 26 Jul 2022 23:57:03 GMT  
		Size: 44.1 MB (44108878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc195249cd1e03b936b46ede192667a7e83792b9f93f7ca837521293fb105494`  
		Last Modified: Tue, 26 Jul 2022 23:56:55 GMT  
		Size: 5.2 KB (5160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56ebae63daf8dd8c229ad24c897be15566d5416ab8bffe4f6d1719bf14e20b09`  
		Last Modified: Tue, 26 Jul 2022 23:56:55 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
