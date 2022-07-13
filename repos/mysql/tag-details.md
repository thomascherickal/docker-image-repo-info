<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `mysql`

-	[`mysql:5`](#mysql5)
-	[`mysql:5-debian`](#mysql5-debian)
-	[`mysql:5-oracle`](#mysql5-oracle)
-	[`mysql:5.7`](#mysql57)
-	[`mysql:5.7-debian`](#mysql57-debian)
-	[`mysql:5.7-oracle`](#mysql57-oracle)
-	[`mysql:5.7.38`](#mysql5738)
-	[`mysql:5.7.38-debian`](#mysql5738-debian)
-	[`mysql:5.7.38-oracle`](#mysql5738-oracle)
-	[`mysql:8`](#mysql8)
-	[`mysql:8-debian`](#mysql8-debian)
-	[`mysql:8-oracle`](#mysql8-oracle)
-	[`mysql:8.0`](#mysql80)
-	[`mysql:8.0-debian`](#mysql80-debian)
-	[`mysql:8.0-oracle`](#mysql80-oracle)
-	[`mysql:8.0.29`](#mysql8029)
-	[`mysql:8.0.29-debian`](#mysql8029-debian)
-	[`mysql:8.0.29-oracle`](#mysql8029-oracle)
-	[`mysql:debian`](#mysqldebian)
-	[`mysql:latest`](#mysqllatest)
-	[`mysql:oracle`](#mysqloracle)

## `mysql:5`

```console
$ docker pull mysql@sha256:bbe0e2b0a33ef5c3a983e490dcb3c1a42d623db1d5679e82f65cce3f32c8f254
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5` - linux; amd64

```console
$ docker pull mysql@sha256:f6f459b960b1c09270dcf6a0b48130ce321754ed85f91340a38bfd0a2bfaa9fd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.8 MB (127835314 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:459651132a1115239f7370765464a0737d028ae7e74c68360740d81751fbae7e`
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
# Wed, 13 Jul 2022 06:46:49 GMT
ENV MYSQL_VERSION=5.7.38-1.el7
# Wed, 13 Jul 2022 06:46:50 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql5.7-server-minimal]'; 		echo 'name=MySQL 5.7 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-5.7-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 13 Jul 2022 06:47:07 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-community-server-minimal-$MYSQL_VERSION"; 	yum clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	{ echo '!includedir /etc/mysql/mysql.conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/mysql.conf.d; 		find /etc/my.cnf /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/'; 		mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 13 Jul 2022 06:47:08 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 13 Jul 2022 06:47:08 GMT
ENV MYSQL_SHELL_VERSION=8.0.29-1.el7
# Wed, 13 Jul 2022 06:47:29 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-shell-$MYSQL_SHELL_VERSION"; 	yum clean all; 		mysqlsh --version
# Wed, 13 Jul 2022 06:47:29 GMT
VOLUME [/var/lib/mysql]
# Wed, 13 Jul 2022 06:47:30 GMT
COPY file:d27cf504fa76fb5a4038020a01eaaf52723b17b751566119de311adacb043752 in /usr/local/bin/ 
# Wed, 13 Jul 2022 06:47:30 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 13 Jul 2022 06:47:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 Jul 2022 06:47:30 GMT
EXPOSE 3306 33060
# Wed, 13 Jul 2022 06:47:30 GMT
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
	-	`sha256:3da2c95cac2f2be8de53134b47fffb71f3d257008a21469515bc369365d80cab`  
		Last Modified: Wed, 13 Jul 2022 06:48:47 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af7913db289ca759b26340e40246245818235665507ec4b07e217e00def9339d`  
		Last Modified: Wed, 13 Jul 2022 06:48:50 GMT  
		Size: 25.5 MB (25495451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77f552f93c12a44977e352279f7cf9e424bed23f5593b9f150ac1de660c28100`  
		Last Modified: Wed, 13 Jul 2022 06:48:46 GMT  
		Size: 317.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ed53edb61abcac629dfed63948829313b0af1321c2ac4a33eb69e6cd64fd0ab`  
		Last Modified: Wed, 13 Jul 2022 06:48:55 GMT  
		Size: 48.1 MB (48087801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67e1c6839f08f71f146139560a0cea2c9999d9c468e67df57b0df499ca968d45`  
		Last Modified: Wed, 13 Jul 2022 06:48:45 GMT  
		Size: 5.2 KB (5162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abcdaaf08d0fddb2dd29500c74a9d51e6878618e456a44a34dc767b2dacf4973`  
		Last Modified: Wed, 13 Jul 2022 06:48:45 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5-debian`

```console
$ docker pull mysql@sha256:367d1dbfd4483258ef7a652728e5b9952fbcecb85279e402aa9e5d87de8231a0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5-debian` - linux; amd64

```console
$ docker pull mysql@sha256:df28187b545543c0a69383e7cce38e826309e6748b2cfe7f55283d4e6a9e7d45
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **162.5 MB (162479117 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c39b1bfebc659bb3c491762610ea952ae3387c2674bb733ba1ee89db28f49aca`
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
# Tue, 12 Jul 2022 01:51:05 GMT
ENV MYSQL_VERSION=5.7.38-1debian10
# Tue, 12 Jul 2022 01:51:06 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-5.7' > /etc/apt/sources.list.d/mysql.list
# Tue, 12 Jul 2022 01:51:24 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-server="${MYSQL_VERSION}" 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 12 Jul 2022 01:51:25 GMT
VOLUME [/var/lib/mysql]
# Tue, 12 Jul 2022 01:51:25 GMT
COPY file:d27cf504fa76fb5a4038020a01eaaf52723b17b751566119de311adacb043752 in /usr/local/bin/ 
# Tue, 12 Jul 2022 01:51:26 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 12 Jul 2022 01:51:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Jul 2022 01:51:26 GMT
EXPOSE 3306 33060
# Tue, 12 Jul 2022 01:51:26 GMT
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
	-	`sha256:54cbb2253505e560148ca1bd7a17143efba2418fbbc1972bd42772a826d62b91`  
		Last Modified: Tue, 12 Jul 2022 01:53:16 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fa6b64c13ff24c36e9041128849079e53c4b4a69b686608b93076c32fa27198`  
		Last Modified: Tue, 12 Jul 2022 01:53:32 GMT  
		Size: 115.7 MB (115676498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29961c6b0e8435d5d91d49f4fae0b47a965f2ee658312354feb91dfe8f63a51e`  
		Last Modified: Tue, 12 Jul 2022 01:53:16 GMT  
		Size: 5.2 KB (5154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9a7e69ecd8e754a1cd222382eedd50b0d31d8f1a3aded65f478093be9f424ad`  
		Last Modified: Tue, 12 Jul 2022 01:53:16 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5-oracle`

```console
$ docker pull mysql@sha256:bbe0e2b0a33ef5c3a983e490dcb3c1a42d623db1d5679e82f65cce3f32c8f254
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:f6f459b960b1c09270dcf6a0b48130ce321754ed85f91340a38bfd0a2bfaa9fd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.8 MB (127835314 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:459651132a1115239f7370765464a0737d028ae7e74c68360740d81751fbae7e`
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
# Wed, 13 Jul 2022 06:46:49 GMT
ENV MYSQL_VERSION=5.7.38-1.el7
# Wed, 13 Jul 2022 06:46:50 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql5.7-server-minimal]'; 		echo 'name=MySQL 5.7 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-5.7-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 13 Jul 2022 06:47:07 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-community-server-minimal-$MYSQL_VERSION"; 	yum clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	{ echo '!includedir /etc/mysql/mysql.conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/mysql.conf.d; 		find /etc/my.cnf /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/'; 		mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 13 Jul 2022 06:47:08 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 13 Jul 2022 06:47:08 GMT
ENV MYSQL_SHELL_VERSION=8.0.29-1.el7
# Wed, 13 Jul 2022 06:47:29 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-shell-$MYSQL_SHELL_VERSION"; 	yum clean all; 		mysqlsh --version
# Wed, 13 Jul 2022 06:47:29 GMT
VOLUME [/var/lib/mysql]
# Wed, 13 Jul 2022 06:47:30 GMT
COPY file:d27cf504fa76fb5a4038020a01eaaf52723b17b751566119de311adacb043752 in /usr/local/bin/ 
# Wed, 13 Jul 2022 06:47:30 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 13 Jul 2022 06:47:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 Jul 2022 06:47:30 GMT
EXPOSE 3306 33060
# Wed, 13 Jul 2022 06:47:30 GMT
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
	-	`sha256:3da2c95cac2f2be8de53134b47fffb71f3d257008a21469515bc369365d80cab`  
		Last Modified: Wed, 13 Jul 2022 06:48:47 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af7913db289ca759b26340e40246245818235665507ec4b07e217e00def9339d`  
		Last Modified: Wed, 13 Jul 2022 06:48:50 GMT  
		Size: 25.5 MB (25495451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77f552f93c12a44977e352279f7cf9e424bed23f5593b9f150ac1de660c28100`  
		Last Modified: Wed, 13 Jul 2022 06:48:46 GMT  
		Size: 317.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ed53edb61abcac629dfed63948829313b0af1321c2ac4a33eb69e6cd64fd0ab`  
		Last Modified: Wed, 13 Jul 2022 06:48:55 GMT  
		Size: 48.1 MB (48087801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67e1c6839f08f71f146139560a0cea2c9999d9c468e67df57b0df499ca968d45`  
		Last Modified: Wed, 13 Jul 2022 06:48:45 GMT  
		Size: 5.2 KB (5162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abcdaaf08d0fddb2dd29500c74a9d51e6878618e456a44a34dc767b2dacf4973`  
		Last Modified: Wed, 13 Jul 2022 06:48:45 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7`

```console
$ docker pull mysql@sha256:bbe0e2b0a33ef5c3a983e490dcb3c1a42d623db1d5679e82f65cce3f32c8f254
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7` - linux; amd64

```console
$ docker pull mysql@sha256:f6f459b960b1c09270dcf6a0b48130ce321754ed85f91340a38bfd0a2bfaa9fd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.8 MB (127835314 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:459651132a1115239f7370765464a0737d028ae7e74c68360740d81751fbae7e`
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
# Wed, 13 Jul 2022 06:46:49 GMT
ENV MYSQL_VERSION=5.7.38-1.el7
# Wed, 13 Jul 2022 06:46:50 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql5.7-server-minimal]'; 		echo 'name=MySQL 5.7 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-5.7-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 13 Jul 2022 06:47:07 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-community-server-minimal-$MYSQL_VERSION"; 	yum clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	{ echo '!includedir /etc/mysql/mysql.conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/mysql.conf.d; 		find /etc/my.cnf /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/'; 		mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 13 Jul 2022 06:47:08 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 13 Jul 2022 06:47:08 GMT
ENV MYSQL_SHELL_VERSION=8.0.29-1.el7
# Wed, 13 Jul 2022 06:47:29 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-shell-$MYSQL_SHELL_VERSION"; 	yum clean all; 		mysqlsh --version
# Wed, 13 Jul 2022 06:47:29 GMT
VOLUME [/var/lib/mysql]
# Wed, 13 Jul 2022 06:47:30 GMT
COPY file:d27cf504fa76fb5a4038020a01eaaf52723b17b751566119de311adacb043752 in /usr/local/bin/ 
# Wed, 13 Jul 2022 06:47:30 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 13 Jul 2022 06:47:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 Jul 2022 06:47:30 GMT
EXPOSE 3306 33060
# Wed, 13 Jul 2022 06:47:30 GMT
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
	-	`sha256:3da2c95cac2f2be8de53134b47fffb71f3d257008a21469515bc369365d80cab`  
		Last Modified: Wed, 13 Jul 2022 06:48:47 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af7913db289ca759b26340e40246245818235665507ec4b07e217e00def9339d`  
		Last Modified: Wed, 13 Jul 2022 06:48:50 GMT  
		Size: 25.5 MB (25495451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77f552f93c12a44977e352279f7cf9e424bed23f5593b9f150ac1de660c28100`  
		Last Modified: Wed, 13 Jul 2022 06:48:46 GMT  
		Size: 317.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ed53edb61abcac629dfed63948829313b0af1321c2ac4a33eb69e6cd64fd0ab`  
		Last Modified: Wed, 13 Jul 2022 06:48:55 GMT  
		Size: 48.1 MB (48087801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67e1c6839f08f71f146139560a0cea2c9999d9c468e67df57b0df499ca968d45`  
		Last Modified: Wed, 13 Jul 2022 06:48:45 GMT  
		Size: 5.2 KB (5162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abcdaaf08d0fddb2dd29500c74a9d51e6878618e456a44a34dc767b2dacf4973`  
		Last Modified: Wed, 13 Jul 2022 06:48:45 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7-debian`

```console
$ docker pull mysql@sha256:367d1dbfd4483258ef7a652728e5b9952fbcecb85279e402aa9e5d87de8231a0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7-debian` - linux; amd64

```console
$ docker pull mysql@sha256:df28187b545543c0a69383e7cce38e826309e6748b2cfe7f55283d4e6a9e7d45
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **162.5 MB (162479117 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c39b1bfebc659bb3c491762610ea952ae3387c2674bb733ba1ee89db28f49aca`
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
# Tue, 12 Jul 2022 01:51:05 GMT
ENV MYSQL_VERSION=5.7.38-1debian10
# Tue, 12 Jul 2022 01:51:06 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-5.7' > /etc/apt/sources.list.d/mysql.list
# Tue, 12 Jul 2022 01:51:24 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-server="${MYSQL_VERSION}" 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 12 Jul 2022 01:51:25 GMT
VOLUME [/var/lib/mysql]
# Tue, 12 Jul 2022 01:51:25 GMT
COPY file:d27cf504fa76fb5a4038020a01eaaf52723b17b751566119de311adacb043752 in /usr/local/bin/ 
# Tue, 12 Jul 2022 01:51:26 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 12 Jul 2022 01:51:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Jul 2022 01:51:26 GMT
EXPOSE 3306 33060
# Tue, 12 Jul 2022 01:51:26 GMT
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
	-	`sha256:54cbb2253505e560148ca1bd7a17143efba2418fbbc1972bd42772a826d62b91`  
		Last Modified: Tue, 12 Jul 2022 01:53:16 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fa6b64c13ff24c36e9041128849079e53c4b4a69b686608b93076c32fa27198`  
		Last Modified: Tue, 12 Jul 2022 01:53:32 GMT  
		Size: 115.7 MB (115676498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29961c6b0e8435d5d91d49f4fae0b47a965f2ee658312354feb91dfe8f63a51e`  
		Last Modified: Tue, 12 Jul 2022 01:53:16 GMT  
		Size: 5.2 KB (5154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9a7e69ecd8e754a1cd222382eedd50b0d31d8f1a3aded65f478093be9f424ad`  
		Last Modified: Tue, 12 Jul 2022 01:53:16 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7-oracle`

```console
$ docker pull mysql@sha256:bbe0e2b0a33ef5c3a983e490dcb3c1a42d623db1d5679e82f65cce3f32c8f254
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:f6f459b960b1c09270dcf6a0b48130ce321754ed85f91340a38bfd0a2bfaa9fd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.8 MB (127835314 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:459651132a1115239f7370765464a0737d028ae7e74c68360740d81751fbae7e`
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
# Wed, 13 Jul 2022 06:46:49 GMT
ENV MYSQL_VERSION=5.7.38-1.el7
# Wed, 13 Jul 2022 06:46:50 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql5.7-server-minimal]'; 		echo 'name=MySQL 5.7 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-5.7-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 13 Jul 2022 06:47:07 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-community-server-minimal-$MYSQL_VERSION"; 	yum clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	{ echo '!includedir /etc/mysql/mysql.conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/mysql.conf.d; 		find /etc/my.cnf /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/'; 		mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 13 Jul 2022 06:47:08 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 13 Jul 2022 06:47:08 GMT
ENV MYSQL_SHELL_VERSION=8.0.29-1.el7
# Wed, 13 Jul 2022 06:47:29 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-shell-$MYSQL_SHELL_VERSION"; 	yum clean all; 		mysqlsh --version
# Wed, 13 Jul 2022 06:47:29 GMT
VOLUME [/var/lib/mysql]
# Wed, 13 Jul 2022 06:47:30 GMT
COPY file:d27cf504fa76fb5a4038020a01eaaf52723b17b751566119de311adacb043752 in /usr/local/bin/ 
# Wed, 13 Jul 2022 06:47:30 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 13 Jul 2022 06:47:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 Jul 2022 06:47:30 GMT
EXPOSE 3306 33060
# Wed, 13 Jul 2022 06:47:30 GMT
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
	-	`sha256:3da2c95cac2f2be8de53134b47fffb71f3d257008a21469515bc369365d80cab`  
		Last Modified: Wed, 13 Jul 2022 06:48:47 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af7913db289ca759b26340e40246245818235665507ec4b07e217e00def9339d`  
		Last Modified: Wed, 13 Jul 2022 06:48:50 GMT  
		Size: 25.5 MB (25495451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77f552f93c12a44977e352279f7cf9e424bed23f5593b9f150ac1de660c28100`  
		Last Modified: Wed, 13 Jul 2022 06:48:46 GMT  
		Size: 317.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ed53edb61abcac629dfed63948829313b0af1321c2ac4a33eb69e6cd64fd0ab`  
		Last Modified: Wed, 13 Jul 2022 06:48:55 GMT  
		Size: 48.1 MB (48087801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67e1c6839f08f71f146139560a0cea2c9999d9c468e67df57b0df499ca968d45`  
		Last Modified: Wed, 13 Jul 2022 06:48:45 GMT  
		Size: 5.2 KB (5162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abcdaaf08d0fddb2dd29500c74a9d51e6878618e456a44a34dc767b2dacf4973`  
		Last Modified: Wed, 13 Jul 2022 06:48:45 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7.38`

```console
$ docker pull mysql@sha256:bbe0e2b0a33ef5c3a983e490dcb3c1a42d623db1d5679e82f65cce3f32c8f254
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7.38` - linux; amd64

```console
$ docker pull mysql@sha256:f6f459b960b1c09270dcf6a0b48130ce321754ed85f91340a38bfd0a2bfaa9fd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.8 MB (127835314 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:459651132a1115239f7370765464a0737d028ae7e74c68360740d81751fbae7e`
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
# Wed, 13 Jul 2022 06:46:49 GMT
ENV MYSQL_VERSION=5.7.38-1.el7
# Wed, 13 Jul 2022 06:46:50 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql5.7-server-minimal]'; 		echo 'name=MySQL 5.7 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-5.7-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 13 Jul 2022 06:47:07 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-community-server-minimal-$MYSQL_VERSION"; 	yum clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	{ echo '!includedir /etc/mysql/mysql.conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/mysql.conf.d; 		find /etc/my.cnf /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/'; 		mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 13 Jul 2022 06:47:08 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 13 Jul 2022 06:47:08 GMT
ENV MYSQL_SHELL_VERSION=8.0.29-1.el7
# Wed, 13 Jul 2022 06:47:29 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-shell-$MYSQL_SHELL_VERSION"; 	yum clean all; 		mysqlsh --version
# Wed, 13 Jul 2022 06:47:29 GMT
VOLUME [/var/lib/mysql]
# Wed, 13 Jul 2022 06:47:30 GMT
COPY file:d27cf504fa76fb5a4038020a01eaaf52723b17b751566119de311adacb043752 in /usr/local/bin/ 
# Wed, 13 Jul 2022 06:47:30 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 13 Jul 2022 06:47:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 Jul 2022 06:47:30 GMT
EXPOSE 3306 33060
# Wed, 13 Jul 2022 06:47:30 GMT
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
	-	`sha256:3da2c95cac2f2be8de53134b47fffb71f3d257008a21469515bc369365d80cab`  
		Last Modified: Wed, 13 Jul 2022 06:48:47 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af7913db289ca759b26340e40246245818235665507ec4b07e217e00def9339d`  
		Last Modified: Wed, 13 Jul 2022 06:48:50 GMT  
		Size: 25.5 MB (25495451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77f552f93c12a44977e352279f7cf9e424bed23f5593b9f150ac1de660c28100`  
		Last Modified: Wed, 13 Jul 2022 06:48:46 GMT  
		Size: 317.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ed53edb61abcac629dfed63948829313b0af1321c2ac4a33eb69e6cd64fd0ab`  
		Last Modified: Wed, 13 Jul 2022 06:48:55 GMT  
		Size: 48.1 MB (48087801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67e1c6839f08f71f146139560a0cea2c9999d9c468e67df57b0df499ca968d45`  
		Last Modified: Wed, 13 Jul 2022 06:48:45 GMT  
		Size: 5.2 KB (5162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abcdaaf08d0fddb2dd29500c74a9d51e6878618e456a44a34dc767b2dacf4973`  
		Last Modified: Wed, 13 Jul 2022 06:48:45 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7.38-debian`

```console
$ docker pull mysql@sha256:367d1dbfd4483258ef7a652728e5b9952fbcecb85279e402aa9e5d87de8231a0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7.38-debian` - linux; amd64

```console
$ docker pull mysql@sha256:df28187b545543c0a69383e7cce38e826309e6748b2cfe7f55283d4e6a9e7d45
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **162.5 MB (162479117 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c39b1bfebc659bb3c491762610ea952ae3387c2674bb733ba1ee89db28f49aca`
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
# Tue, 12 Jul 2022 01:51:05 GMT
ENV MYSQL_VERSION=5.7.38-1debian10
# Tue, 12 Jul 2022 01:51:06 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-5.7' > /etc/apt/sources.list.d/mysql.list
# Tue, 12 Jul 2022 01:51:24 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-server="${MYSQL_VERSION}" 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 12 Jul 2022 01:51:25 GMT
VOLUME [/var/lib/mysql]
# Tue, 12 Jul 2022 01:51:25 GMT
COPY file:d27cf504fa76fb5a4038020a01eaaf52723b17b751566119de311adacb043752 in /usr/local/bin/ 
# Tue, 12 Jul 2022 01:51:26 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 12 Jul 2022 01:51:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Jul 2022 01:51:26 GMT
EXPOSE 3306 33060
# Tue, 12 Jul 2022 01:51:26 GMT
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
	-	`sha256:54cbb2253505e560148ca1bd7a17143efba2418fbbc1972bd42772a826d62b91`  
		Last Modified: Tue, 12 Jul 2022 01:53:16 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fa6b64c13ff24c36e9041128849079e53c4b4a69b686608b93076c32fa27198`  
		Last Modified: Tue, 12 Jul 2022 01:53:32 GMT  
		Size: 115.7 MB (115676498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29961c6b0e8435d5d91d49f4fae0b47a965f2ee658312354feb91dfe8f63a51e`  
		Last Modified: Tue, 12 Jul 2022 01:53:16 GMT  
		Size: 5.2 KB (5154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9a7e69ecd8e754a1cd222382eedd50b0d31d8f1a3aded65f478093be9f424ad`  
		Last Modified: Tue, 12 Jul 2022 01:53:16 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7.38-oracle`

```console
$ docker pull mysql@sha256:bbe0e2b0a33ef5c3a983e490dcb3c1a42d623db1d5679e82f65cce3f32c8f254
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7.38-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:f6f459b960b1c09270dcf6a0b48130ce321754ed85f91340a38bfd0a2bfaa9fd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.8 MB (127835314 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:459651132a1115239f7370765464a0737d028ae7e74c68360740d81751fbae7e`
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
# Wed, 13 Jul 2022 06:46:49 GMT
ENV MYSQL_VERSION=5.7.38-1.el7
# Wed, 13 Jul 2022 06:46:50 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql5.7-server-minimal]'; 		echo 'name=MySQL 5.7 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-5.7-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 13 Jul 2022 06:47:07 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-community-server-minimal-$MYSQL_VERSION"; 	yum clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	{ echo '!includedir /etc/mysql/mysql.conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/mysql.conf.d; 		find /etc/my.cnf /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/'; 		mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 13 Jul 2022 06:47:08 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 13 Jul 2022 06:47:08 GMT
ENV MYSQL_SHELL_VERSION=8.0.29-1.el7
# Wed, 13 Jul 2022 06:47:29 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-shell-$MYSQL_SHELL_VERSION"; 	yum clean all; 		mysqlsh --version
# Wed, 13 Jul 2022 06:47:29 GMT
VOLUME [/var/lib/mysql]
# Wed, 13 Jul 2022 06:47:30 GMT
COPY file:d27cf504fa76fb5a4038020a01eaaf52723b17b751566119de311adacb043752 in /usr/local/bin/ 
# Wed, 13 Jul 2022 06:47:30 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 13 Jul 2022 06:47:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 Jul 2022 06:47:30 GMT
EXPOSE 3306 33060
# Wed, 13 Jul 2022 06:47:30 GMT
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
	-	`sha256:3da2c95cac2f2be8de53134b47fffb71f3d257008a21469515bc369365d80cab`  
		Last Modified: Wed, 13 Jul 2022 06:48:47 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af7913db289ca759b26340e40246245818235665507ec4b07e217e00def9339d`  
		Last Modified: Wed, 13 Jul 2022 06:48:50 GMT  
		Size: 25.5 MB (25495451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77f552f93c12a44977e352279f7cf9e424bed23f5593b9f150ac1de660c28100`  
		Last Modified: Wed, 13 Jul 2022 06:48:46 GMT  
		Size: 317.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ed53edb61abcac629dfed63948829313b0af1321c2ac4a33eb69e6cd64fd0ab`  
		Last Modified: Wed, 13 Jul 2022 06:48:55 GMT  
		Size: 48.1 MB (48087801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67e1c6839f08f71f146139560a0cea2c9999d9c468e67df57b0df499ca968d45`  
		Last Modified: Wed, 13 Jul 2022 06:48:45 GMT  
		Size: 5.2 KB (5162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abcdaaf08d0fddb2dd29500c74a9d51e6878618e456a44a34dc767b2dacf4973`  
		Last Modified: Wed, 13 Jul 2022 06:48:45 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8`

```console
$ docker pull mysql@sha256:152cf187a3efc56afb0b3877b4d21e231d1d6eb828ca9221056590b0ac834c75
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8` - linux; amd64

```console
$ docker pull mysql@sha256:44f98f4dd825a945d2a6a4b7b2f14127b5d07c5aaa07d9d232c2b58936fb76dc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.8 MB (131789857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33037edcac9b155a185e9555a5da711d754c88cb244e3d13e214db029c3b28ed`
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
# Wed, 13 Jul 2022 06:45:09 GMT
ENV MYSQL_VERSION=8.0.29-1.el8
# Wed, 13 Jul 2022 06:45:10 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 13 Jul 2022 06:45:38 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 13 Jul 2022 06:45:39 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 13 Jul 2022 06:45:39 GMT
ENV MYSQL_SHELL_VERSION=8.0.29-1.el8
# Wed, 13 Jul 2022 06:46:10 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Wed, 13 Jul 2022 06:46:10 GMT
VOLUME [/var/lib/mysql]
# Wed, 13 Jul 2022 06:46:11 GMT
COPY file:d27cf504fa76fb5a4038020a01eaaf52723b17b751566119de311adacb043752 in /usr/local/bin/ 
# Wed, 13 Jul 2022 06:46:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 13 Jul 2022 06:46:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 Jul 2022 06:46:11 GMT
EXPOSE 3306 33060
# Wed, 13 Jul 2022 06:46:11 GMT
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
	-	`sha256:7d1cc1ea1b3d8d62693939510193ad4b1c95748bcdcbb85e4a865555416fa2ce`  
		Last Modified: Wed, 13 Jul 2022 06:48:11 GMT  
		Size: 337.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d48f3c15cb803b81492348c7b8c160e9a9d3957dc0cc567b76893ec9dd3afd78`  
		Last Modified: Wed, 13 Jul 2022 06:48:16 GMT  
		Size: 47.3 MB (47260752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94c3d7b2c9ae878ae450aab764713dca9f718d37c21407ee84f36ce15c4f28d8`  
		Last Modified: Wed, 13 Jul 2022 06:48:09 GMT  
		Size: 318.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6cfbf240ed7196ec43fc009b344e17a6c84451079f19efea7b3fd2dab9bd65e`  
		Last Modified: Wed, 13 Jul 2022 06:48:16 GMT  
		Size: 39.8 MB (39780528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e12b159b2a12d49839093db700fe67feaa672b5461c59fda8c886799561195b5`  
		Last Modified: Wed, 13 Jul 2022 06:48:08 GMT  
		Size: 5.2 KB (5163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e93c6fd777f87eef9811f067b652a8d38e533ad87901fcd9648a3091f8b3a13`  
		Last Modified: Wed, 13 Jul 2022 06:48:08 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:12cf01a51f803d0ad49ee0dbbb3025a6eef3341e24757c2ed8150b6654c3fb07
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.7 MB (138716495 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02662e079c08f45f90a837cf583cfb18bc58a400342d4fefde11199f3d1f4102`
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
# Wed, 13 Jul 2022 07:47:56 GMT
ENV MYSQL_VERSION=8.0.29-1.el8
# Wed, 13 Jul 2022 07:47:57 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 13 Jul 2022 07:48:22 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 13 Jul 2022 07:48:23 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 13 Jul 2022 07:48:24 GMT
ENV MYSQL_SHELL_VERSION=8.0.29-1.el8
# Wed, 13 Jul 2022 07:48:52 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Wed, 13 Jul 2022 07:48:52 GMT
VOLUME [/var/lib/mysql]
# Wed, 13 Jul 2022 07:48:54 GMT
COPY file:d27cf504fa76fb5a4038020a01eaaf52723b17b751566119de311adacb043752 in /usr/local/bin/ 
# Wed, 13 Jul 2022 07:48:54 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 13 Jul 2022 07:48:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 Jul 2022 07:48:56 GMT
EXPOSE 3306 33060
# Wed, 13 Jul 2022 07:48:57 GMT
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
	-	`sha256:a0c96e0313eb60e8210c676750efcb4e81ee7fa7f03d25753a285f1099d6ea2a`  
		Last Modified: Wed, 13 Jul 2022 07:49:26 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abbb3361f75b7791da51c4da9574c17f2c5bcf091461d36ae7c0f28b04a29360`  
		Last Modified: Wed, 13 Jul 2022 07:49:31 GMT  
		Size: 53.3 MB (53324981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:857f6a6ae5074bea540b73b0b8be220f0ff784d5de971d89bfac6374807c760c`  
		Last Modified: Wed, 13 Jul 2022 07:49:24 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ac3d9a78b39cb7d140f50375303fca9c8f7635c31377217dd93b494d5a3bced`  
		Last Modified: Wed, 13 Jul 2022 07:49:32 GMT  
		Size: 42.1 MB (42075330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a07911c3362fc1fbaa9b5018facd4ea2e98408f9923338d8fea847048357b30e`  
		Last Modified: Wed, 13 Jul 2022 07:49:24 GMT  
		Size: 5.2 KB (5158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fce3f4951dffafbeebe224f95703722f1f44783a530c658ecd594a3f32252a3f`  
		Last Modified: Wed, 13 Jul 2022 07:49:24 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8-debian`

```console
$ docker pull mysql@sha256:5ef1130b5a6ebd5c2f31f0244c25027c47fb5a7279ad747026b495414adaaf27
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:8-debian` - linux; amd64

```console
$ docker pull mysql@sha256:3a7e864bc88458911fa598065fe027736fa63495f5780ee0618caeb4a52bbc4c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **157.4 MB (157380412 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0fc0e2322d42dbab9448b7af63601f09cbd916193afec376675bf32fdbca5203`
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
# Tue, 12 Jul 2022 01:50:12 GMT
ENV MYSQL_VERSION=8.0.29-1debian11
# Tue, 12 Jul 2022 01:50:13 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ bullseye mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Tue, 12 Jul 2022 01:50:28 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 12 Jul 2022 01:50:29 GMT
VOLUME [/var/lib/mysql]
# Tue, 12 Jul 2022 01:50:29 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Tue, 12 Jul 2022 01:50:29 GMT
COPY file:d27cf504fa76fb5a4038020a01eaaf52723b17b751566119de311adacb043752 in /usr/local/bin/ 
# Tue, 12 Jul 2022 01:50:29 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 12 Jul 2022 01:50:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Jul 2022 01:50:30 GMT
EXPOSE 3306 33060
# Tue, 12 Jul 2022 01:50:30 GMT
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
	-	`sha256:a7ddfbeb275b283abe3dfc3de542ebdcc701c4c996a96c2be39ed59e5137ac83`  
		Last Modified: Tue, 12 Jul 2022 01:52:21 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29fbdc9d2624616a1188b80790c80688aba8f17538b784d1ec937ba763d0caca`  
		Last Modified: Tue, 12 Jul 2022 01:52:38 GMT  
		Size: 107.5 MB (107508121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87a306bac37ec6ca492ea124d5aab4a2015656c9bbcf1d82aa693a2df13241d1`  
		Last Modified: Tue, 12 Jul 2022 01:52:21 GMT  
		Size: 845.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3396c7604c38680b49a32a26d9e55ae095981acb8d33fd75c844fa5b6b0edc39`  
		Last Modified: Tue, 12 Jul 2022 01:52:21 GMT  
		Size: 5.2 KB (5157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:832af0332a2a6d268d5173bf633da9f00789d1970b6992fba3a7c49b208aca38`  
		Last Modified: Tue, 12 Jul 2022 01:52:21 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8-oracle`

```console
$ docker pull mysql@sha256:152cf187a3efc56afb0b3877b4d21e231d1d6eb828ca9221056590b0ac834c75
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:44f98f4dd825a945d2a6a4b7b2f14127b5d07c5aaa07d9d232c2b58936fb76dc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.8 MB (131789857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33037edcac9b155a185e9555a5da711d754c88cb244e3d13e214db029c3b28ed`
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
# Wed, 13 Jul 2022 06:45:09 GMT
ENV MYSQL_VERSION=8.0.29-1.el8
# Wed, 13 Jul 2022 06:45:10 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 13 Jul 2022 06:45:38 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 13 Jul 2022 06:45:39 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 13 Jul 2022 06:45:39 GMT
ENV MYSQL_SHELL_VERSION=8.0.29-1.el8
# Wed, 13 Jul 2022 06:46:10 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Wed, 13 Jul 2022 06:46:10 GMT
VOLUME [/var/lib/mysql]
# Wed, 13 Jul 2022 06:46:11 GMT
COPY file:d27cf504fa76fb5a4038020a01eaaf52723b17b751566119de311adacb043752 in /usr/local/bin/ 
# Wed, 13 Jul 2022 06:46:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 13 Jul 2022 06:46:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 Jul 2022 06:46:11 GMT
EXPOSE 3306 33060
# Wed, 13 Jul 2022 06:46:11 GMT
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
	-	`sha256:7d1cc1ea1b3d8d62693939510193ad4b1c95748bcdcbb85e4a865555416fa2ce`  
		Last Modified: Wed, 13 Jul 2022 06:48:11 GMT  
		Size: 337.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d48f3c15cb803b81492348c7b8c160e9a9d3957dc0cc567b76893ec9dd3afd78`  
		Last Modified: Wed, 13 Jul 2022 06:48:16 GMT  
		Size: 47.3 MB (47260752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94c3d7b2c9ae878ae450aab764713dca9f718d37c21407ee84f36ce15c4f28d8`  
		Last Modified: Wed, 13 Jul 2022 06:48:09 GMT  
		Size: 318.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6cfbf240ed7196ec43fc009b344e17a6c84451079f19efea7b3fd2dab9bd65e`  
		Last Modified: Wed, 13 Jul 2022 06:48:16 GMT  
		Size: 39.8 MB (39780528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e12b159b2a12d49839093db700fe67feaa672b5461c59fda8c886799561195b5`  
		Last Modified: Wed, 13 Jul 2022 06:48:08 GMT  
		Size: 5.2 KB (5163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e93c6fd777f87eef9811f067b652a8d38e533ad87901fcd9648a3091f8b3a13`  
		Last Modified: Wed, 13 Jul 2022 06:48:08 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8-oracle` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:12cf01a51f803d0ad49ee0dbbb3025a6eef3341e24757c2ed8150b6654c3fb07
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.7 MB (138716495 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02662e079c08f45f90a837cf583cfb18bc58a400342d4fefde11199f3d1f4102`
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
# Wed, 13 Jul 2022 07:47:56 GMT
ENV MYSQL_VERSION=8.0.29-1.el8
# Wed, 13 Jul 2022 07:47:57 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 13 Jul 2022 07:48:22 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 13 Jul 2022 07:48:23 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 13 Jul 2022 07:48:24 GMT
ENV MYSQL_SHELL_VERSION=8.0.29-1.el8
# Wed, 13 Jul 2022 07:48:52 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Wed, 13 Jul 2022 07:48:52 GMT
VOLUME [/var/lib/mysql]
# Wed, 13 Jul 2022 07:48:54 GMT
COPY file:d27cf504fa76fb5a4038020a01eaaf52723b17b751566119de311adacb043752 in /usr/local/bin/ 
# Wed, 13 Jul 2022 07:48:54 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 13 Jul 2022 07:48:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 Jul 2022 07:48:56 GMT
EXPOSE 3306 33060
# Wed, 13 Jul 2022 07:48:57 GMT
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
	-	`sha256:a0c96e0313eb60e8210c676750efcb4e81ee7fa7f03d25753a285f1099d6ea2a`  
		Last Modified: Wed, 13 Jul 2022 07:49:26 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abbb3361f75b7791da51c4da9574c17f2c5bcf091461d36ae7c0f28b04a29360`  
		Last Modified: Wed, 13 Jul 2022 07:49:31 GMT  
		Size: 53.3 MB (53324981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:857f6a6ae5074bea540b73b0b8be220f0ff784d5de971d89bfac6374807c760c`  
		Last Modified: Wed, 13 Jul 2022 07:49:24 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ac3d9a78b39cb7d140f50375303fca9c8f7635c31377217dd93b494d5a3bced`  
		Last Modified: Wed, 13 Jul 2022 07:49:32 GMT  
		Size: 42.1 MB (42075330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a07911c3362fc1fbaa9b5018facd4ea2e98408f9923338d8fea847048357b30e`  
		Last Modified: Wed, 13 Jul 2022 07:49:24 GMT  
		Size: 5.2 KB (5158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fce3f4951dffafbeebe224f95703722f1f44783a530c658ecd594a3f32252a3f`  
		Last Modified: Wed, 13 Jul 2022 07:49:24 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0`

```console
$ docker pull mysql@sha256:152cf187a3efc56afb0b3877b4d21e231d1d6eb828ca9221056590b0ac834c75
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8.0` - linux; amd64

```console
$ docker pull mysql@sha256:44f98f4dd825a945d2a6a4b7b2f14127b5d07c5aaa07d9d232c2b58936fb76dc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.8 MB (131789857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33037edcac9b155a185e9555a5da711d754c88cb244e3d13e214db029c3b28ed`
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
# Wed, 13 Jul 2022 06:45:09 GMT
ENV MYSQL_VERSION=8.0.29-1.el8
# Wed, 13 Jul 2022 06:45:10 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 13 Jul 2022 06:45:38 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 13 Jul 2022 06:45:39 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 13 Jul 2022 06:45:39 GMT
ENV MYSQL_SHELL_VERSION=8.0.29-1.el8
# Wed, 13 Jul 2022 06:46:10 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Wed, 13 Jul 2022 06:46:10 GMT
VOLUME [/var/lib/mysql]
# Wed, 13 Jul 2022 06:46:11 GMT
COPY file:d27cf504fa76fb5a4038020a01eaaf52723b17b751566119de311adacb043752 in /usr/local/bin/ 
# Wed, 13 Jul 2022 06:46:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 13 Jul 2022 06:46:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 Jul 2022 06:46:11 GMT
EXPOSE 3306 33060
# Wed, 13 Jul 2022 06:46:11 GMT
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
	-	`sha256:7d1cc1ea1b3d8d62693939510193ad4b1c95748bcdcbb85e4a865555416fa2ce`  
		Last Modified: Wed, 13 Jul 2022 06:48:11 GMT  
		Size: 337.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d48f3c15cb803b81492348c7b8c160e9a9d3957dc0cc567b76893ec9dd3afd78`  
		Last Modified: Wed, 13 Jul 2022 06:48:16 GMT  
		Size: 47.3 MB (47260752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94c3d7b2c9ae878ae450aab764713dca9f718d37c21407ee84f36ce15c4f28d8`  
		Last Modified: Wed, 13 Jul 2022 06:48:09 GMT  
		Size: 318.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6cfbf240ed7196ec43fc009b344e17a6c84451079f19efea7b3fd2dab9bd65e`  
		Last Modified: Wed, 13 Jul 2022 06:48:16 GMT  
		Size: 39.8 MB (39780528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e12b159b2a12d49839093db700fe67feaa672b5461c59fda8c886799561195b5`  
		Last Modified: Wed, 13 Jul 2022 06:48:08 GMT  
		Size: 5.2 KB (5163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e93c6fd777f87eef9811f067b652a8d38e533ad87901fcd9648a3091f8b3a13`  
		Last Modified: Wed, 13 Jul 2022 06:48:08 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8.0` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:12cf01a51f803d0ad49ee0dbbb3025a6eef3341e24757c2ed8150b6654c3fb07
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.7 MB (138716495 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02662e079c08f45f90a837cf583cfb18bc58a400342d4fefde11199f3d1f4102`
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
# Wed, 13 Jul 2022 07:47:56 GMT
ENV MYSQL_VERSION=8.0.29-1.el8
# Wed, 13 Jul 2022 07:47:57 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 13 Jul 2022 07:48:22 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 13 Jul 2022 07:48:23 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 13 Jul 2022 07:48:24 GMT
ENV MYSQL_SHELL_VERSION=8.0.29-1.el8
# Wed, 13 Jul 2022 07:48:52 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Wed, 13 Jul 2022 07:48:52 GMT
VOLUME [/var/lib/mysql]
# Wed, 13 Jul 2022 07:48:54 GMT
COPY file:d27cf504fa76fb5a4038020a01eaaf52723b17b751566119de311adacb043752 in /usr/local/bin/ 
# Wed, 13 Jul 2022 07:48:54 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 13 Jul 2022 07:48:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 Jul 2022 07:48:56 GMT
EXPOSE 3306 33060
# Wed, 13 Jul 2022 07:48:57 GMT
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
	-	`sha256:a0c96e0313eb60e8210c676750efcb4e81ee7fa7f03d25753a285f1099d6ea2a`  
		Last Modified: Wed, 13 Jul 2022 07:49:26 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abbb3361f75b7791da51c4da9574c17f2c5bcf091461d36ae7c0f28b04a29360`  
		Last Modified: Wed, 13 Jul 2022 07:49:31 GMT  
		Size: 53.3 MB (53324981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:857f6a6ae5074bea540b73b0b8be220f0ff784d5de971d89bfac6374807c760c`  
		Last Modified: Wed, 13 Jul 2022 07:49:24 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ac3d9a78b39cb7d140f50375303fca9c8f7635c31377217dd93b494d5a3bced`  
		Last Modified: Wed, 13 Jul 2022 07:49:32 GMT  
		Size: 42.1 MB (42075330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a07911c3362fc1fbaa9b5018facd4ea2e98408f9923338d8fea847048357b30e`  
		Last Modified: Wed, 13 Jul 2022 07:49:24 GMT  
		Size: 5.2 KB (5158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fce3f4951dffafbeebe224f95703722f1f44783a530c658ecd594a3f32252a3f`  
		Last Modified: Wed, 13 Jul 2022 07:49:24 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0-debian`

```console
$ docker pull mysql@sha256:5ef1130b5a6ebd5c2f31f0244c25027c47fb5a7279ad747026b495414adaaf27
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:8.0-debian` - linux; amd64

```console
$ docker pull mysql@sha256:3a7e864bc88458911fa598065fe027736fa63495f5780ee0618caeb4a52bbc4c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **157.4 MB (157380412 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0fc0e2322d42dbab9448b7af63601f09cbd916193afec376675bf32fdbca5203`
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
# Tue, 12 Jul 2022 01:50:12 GMT
ENV MYSQL_VERSION=8.0.29-1debian11
# Tue, 12 Jul 2022 01:50:13 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ bullseye mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Tue, 12 Jul 2022 01:50:28 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 12 Jul 2022 01:50:29 GMT
VOLUME [/var/lib/mysql]
# Tue, 12 Jul 2022 01:50:29 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Tue, 12 Jul 2022 01:50:29 GMT
COPY file:d27cf504fa76fb5a4038020a01eaaf52723b17b751566119de311adacb043752 in /usr/local/bin/ 
# Tue, 12 Jul 2022 01:50:29 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 12 Jul 2022 01:50:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Jul 2022 01:50:30 GMT
EXPOSE 3306 33060
# Tue, 12 Jul 2022 01:50:30 GMT
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
	-	`sha256:a7ddfbeb275b283abe3dfc3de542ebdcc701c4c996a96c2be39ed59e5137ac83`  
		Last Modified: Tue, 12 Jul 2022 01:52:21 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29fbdc9d2624616a1188b80790c80688aba8f17538b784d1ec937ba763d0caca`  
		Last Modified: Tue, 12 Jul 2022 01:52:38 GMT  
		Size: 107.5 MB (107508121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87a306bac37ec6ca492ea124d5aab4a2015656c9bbcf1d82aa693a2df13241d1`  
		Last Modified: Tue, 12 Jul 2022 01:52:21 GMT  
		Size: 845.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3396c7604c38680b49a32a26d9e55ae095981acb8d33fd75c844fa5b6b0edc39`  
		Last Modified: Tue, 12 Jul 2022 01:52:21 GMT  
		Size: 5.2 KB (5157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:832af0332a2a6d268d5173bf633da9f00789d1970b6992fba3a7c49b208aca38`  
		Last Modified: Tue, 12 Jul 2022 01:52:21 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0-oracle`

```console
$ docker pull mysql@sha256:152cf187a3efc56afb0b3877b4d21e231d1d6eb828ca9221056590b0ac834c75
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8.0-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:44f98f4dd825a945d2a6a4b7b2f14127b5d07c5aaa07d9d232c2b58936fb76dc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.8 MB (131789857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33037edcac9b155a185e9555a5da711d754c88cb244e3d13e214db029c3b28ed`
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
# Wed, 13 Jul 2022 06:45:09 GMT
ENV MYSQL_VERSION=8.0.29-1.el8
# Wed, 13 Jul 2022 06:45:10 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 13 Jul 2022 06:45:38 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 13 Jul 2022 06:45:39 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 13 Jul 2022 06:45:39 GMT
ENV MYSQL_SHELL_VERSION=8.0.29-1.el8
# Wed, 13 Jul 2022 06:46:10 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Wed, 13 Jul 2022 06:46:10 GMT
VOLUME [/var/lib/mysql]
# Wed, 13 Jul 2022 06:46:11 GMT
COPY file:d27cf504fa76fb5a4038020a01eaaf52723b17b751566119de311adacb043752 in /usr/local/bin/ 
# Wed, 13 Jul 2022 06:46:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 13 Jul 2022 06:46:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 Jul 2022 06:46:11 GMT
EXPOSE 3306 33060
# Wed, 13 Jul 2022 06:46:11 GMT
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
	-	`sha256:7d1cc1ea1b3d8d62693939510193ad4b1c95748bcdcbb85e4a865555416fa2ce`  
		Last Modified: Wed, 13 Jul 2022 06:48:11 GMT  
		Size: 337.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d48f3c15cb803b81492348c7b8c160e9a9d3957dc0cc567b76893ec9dd3afd78`  
		Last Modified: Wed, 13 Jul 2022 06:48:16 GMT  
		Size: 47.3 MB (47260752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94c3d7b2c9ae878ae450aab764713dca9f718d37c21407ee84f36ce15c4f28d8`  
		Last Modified: Wed, 13 Jul 2022 06:48:09 GMT  
		Size: 318.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6cfbf240ed7196ec43fc009b344e17a6c84451079f19efea7b3fd2dab9bd65e`  
		Last Modified: Wed, 13 Jul 2022 06:48:16 GMT  
		Size: 39.8 MB (39780528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e12b159b2a12d49839093db700fe67feaa672b5461c59fda8c886799561195b5`  
		Last Modified: Wed, 13 Jul 2022 06:48:08 GMT  
		Size: 5.2 KB (5163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e93c6fd777f87eef9811f067b652a8d38e533ad87901fcd9648a3091f8b3a13`  
		Last Modified: Wed, 13 Jul 2022 06:48:08 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8.0-oracle` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:12cf01a51f803d0ad49ee0dbbb3025a6eef3341e24757c2ed8150b6654c3fb07
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.7 MB (138716495 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02662e079c08f45f90a837cf583cfb18bc58a400342d4fefde11199f3d1f4102`
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
# Wed, 13 Jul 2022 07:47:56 GMT
ENV MYSQL_VERSION=8.0.29-1.el8
# Wed, 13 Jul 2022 07:47:57 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 13 Jul 2022 07:48:22 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 13 Jul 2022 07:48:23 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 13 Jul 2022 07:48:24 GMT
ENV MYSQL_SHELL_VERSION=8.0.29-1.el8
# Wed, 13 Jul 2022 07:48:52 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Wed, 13 Jul 2022 07:48:52 GMT
VOLUME [/var/lib/mysql]
# Wed, 13 Jul 2022 07:48:54 GMT
COPY file:d27cf504fa76fb5a4038020a01eaaf52723b17b751566119de311adacb043752 in /usr/local/bin/ 
# Wed, 13 Jul 2022 07:48:54 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 13 Jul 2022 07:48:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 Jul 2022 07:48:56 GMT
EXPOSE 3306 33060
# Wed, 13 Jul 2022 07:48:57 GMT
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
	-	`sha256:a0c96e0313eb60e8210c676750efcb4e81ee7fa7f03d25753a285f1099d6ea2a`  
		Last Modified: Wed, 13 Jul 2022 07:49:26 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abbb3361f75b7791da51c4da9574c17f2c5bcf091461d36ae7c0f28b04a29360`  
		Last Modified: Wed, 13 Jul 2022 07:49:31 GMT  
		Size: 53.3 MB (53324981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:857f6a6ae5074bea540b73b0b8be220f0ff784d5de971d89bfac6374807c760c`  
		Last Modified: Wed, 13 Jul 2022 07:49:24 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ac3d9a78b39cb7d140f50375303fca9c8f7635c31377217dd93b494d5a3bced`  
		Last Modified: Wed, 13 Jul 2022 07:49:32 GMT  
		Size: 42.1 MB (42075330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a07911c3362fc1fbaa9b5018facd4ea2e98408f9923338d8fea847048357b30e`  
		Last Modified: Wed, 13 Jul 2022 07:49:24 GMT  
		Size: 5.2 KB (5158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fce3f4951dffafbeebe224f95703722f1f44783a530c658ecd594a3f32252a3f`  
		Last Modified: Wed, 13 Jul 2022 07:49:24 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0.29`

```console
$ docker pull mysql@sha256:152cf187a3efc56afb0b3877b4d21e231d1d6eb828ca9221056590b0ac834c75
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8.0.29` - linux; amd64

```console
$ docker pull mysql@sha256:44f98f4dd825a945d2a6a4b7b2f14127b5d07c5aaa07d9d232c2b58936fb76dc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.8 MB (131789857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33037edcac9b155a185e9555a5da711d754c88cb244e3d13e214db029c3b28ed`
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
# Wed, 13 Jul 2022 06:45:09 GMT
ENV MYSQL_VERSION=8.0.29-1.el8
# Wed, 13 Jul 2022 06:45:10 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 13 Jul 2022 06:45:38 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 13 Jul 2022 06:45:39 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 13 Jul 2022 06:45:39 GMT
ENV MYSQL_SHELL_VERSION=8.0.29-1.el8
# Wed, 13 Jul 2022 06:46:10 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Wed, 13 Jul 2022 06:46:10 GMT
VOLUME [/var/lib/mysql]
# Wed, 13 Jul 2022 06:46:11 GMT
COPY file:d27cf504fa76fb5a4038020a01eaaf52723b17b751566119de311adacb043752 in /usr/local/bin/ 
# Wed, 13 Jul 2022 06:46:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 13 Jul 2022 06:46:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 Jul 2022 06:46:11 GMT
EXPOSE 3306 33060
# Wed, 13 Jul 2022 06:46:11 GMT
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
	-	`sha256:7d1cc1ea1b3d8d62693939510193ad4b1c95748bcdcbb85e4a865555416fa2ce`  
		Last Modified: Wed, 13 Jul 2022 06:48:11 GMT  
		Size: 337.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d48f3c15cb803b81492348c7b8c160e9a9d3957dc0cc567b76893ec9dd3afd78`  
		Last Modified: Wed, 13 Jul 2022 06:48:16 GMT  
		Size: 47.3 MB (47260752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94c3d7b2c9ae878ae450aab764713dca9f718d37c21407ee84f36ce15c4f28d8`  
		Last Modified: Wed, 13 Jul 2022 06:48:09 GMT  
		Size: 318.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6cfbf240ed7196ec43fc009b344e17a6c84451079f19efea7b3fd2dab9bd65e`  
		Last Modified: Wed, 13 Jul 2022 06:48:16 GMT  
		Size: 39.8 MB (39780528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e12b159b2a12d49839093db700fe67feaa672b5461c59fda8c886799561195b5`  
		Last Modified: Wed, 13 Jul 2022 06:48:08 GMT  
		Size: 5.2 KB (5163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e93c6fd777f87eef9811f067b652a8d38e533ad87901fcd9648a3091f8b3a13`  
		Last Modified: Wed, 13 Jul 2022 06:48:08 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8.0.29` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:12cf01a51f803d0ad49ee0dbbb3025a6eef3341e24757c2ed8150b6654c3fb07
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.7 MB (138716495 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02662e079c08f45f90a837cf583cfb18bc58a400342d4fefde11199f3d1f4102`
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
# Wed, 13 Jul 2022 07:47:56 GMT
ENV MYSQL_VERSION=8.0.29-1.el8
# Wed, 13 Jul 2022 07:47:57 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 13 Jul 2022 07:48:22 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 13 Jul 2022 07:48:23 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 13 Jul 2022 07:48:24 GMT
ENV MYSQL_SHELL_VERSION=8.0.29-1.el8
# Wed, 13 Jul 2022 07:48:52 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Wed, 13 Jul 2022 07:48:52 GMT
VOLUME [/var/lib/mysql]
# Wed, 13 Jul 2022 07:48:54 GMT
COPY file:d27cf504fa76fb5a4038020a01eaaf52723b17b751566119de311adacb043752 in /usr/local/bin/ 
# Wed, 13 Jul 2022 07:48:54 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 13 Jul 2022 07:48:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 Jul 2022 07:48:56 GMT
EXPOSE 3306 33060
# Wed, 13 Jul 2022 07:48:57 GMT
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
	-	`sha256:a0c96e0313eb60e8210c676750efcb4e81ee7fa7f03d25753a285f1099d6ea2a`  
		Last Modified: Wed, 13 Jul 2022 07:49:26 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abbb3361f75b7791da51c4da9574c17f2c5bcf091461d36ae7c0f28b04a29360`  
		Last Modified: Wed, 13 Jul 2022 07:49:31 GMT  
		Size: 53.3 MB (53324981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:857f6a6ae5074bea540b73b0b8be220f0ff784d5de971d89bfac6374807c760c`  
		Last Modified: Wed, 13 Jul 2022 07:49:24 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ac3d9a78b39cb7d140f50375303fca9c8f7635c31377217dd93b494d5a3bced`  
		Last Modified: Wed, 13 Jul 2022 07:49:32 GMT  
		Size: 42.1 MB (42075330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a07911c3362fc1fbaa9b5018facd4ea2e98408f9923338d8fea847048357b30e`  
		Last Modified: Wed, 13 Jul 2022 07:49:24 GMT  
		Size: 5.2 KB (5158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fce3f4951dffafbeebe224f95703722f1f44783a530c658ecd594a3f32252a3f`  
		Last Modified: Wed, 13 Jul 2022 07:49:24 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0.29-debian`

```console
$ docker pull mysql@sha256:5ef1130b5a6ebd5c2f31f0244c25027c47fb5a7279ad747026b495414adaaf27
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:8.0.29-debian` - linux; amd64

```console
$ docker pull mysql@sha256:3a7e864bc88458911fa598065fe027736fa63495f5780ee0618caeb4a52bbc4c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **157.4 MB (157380412 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0fc0e2322d42dbab9448b7af63601f09cbd916193afec376675bf32fdbca5203`
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
# Tue, 12 Jul 2022 01:50:12 GMT
ENV MYSQL_VERSION=8.0.29-1debian11
# Tue, 12 Jul 2022 01:50:13 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ bullseye mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Tue, 12 Jul 2022 01:50:28 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 12 Jul 2022 01:50:29 GMT
VOLUME [/var/lib/mysql]
# Tue, 12 Jul 2022 01:50:29 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Tue, 12 Jul 2022 01:50:29 GMT
COPY file:d27cf504fa76fb5a4038020a01eaaf52723b17b751566119de311adacb043752 in /usr/local/bin/ 
# Tue, 12 Jul 2022 01:50:29 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 12 Jul 2022 01:50:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Jul 2022 01:50:30 GMT
EXPOSE 3306 33060
# Tue, 12 Jul 2022 01:50:30 GMT
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
	-	`sha256:a7ddfbeb275b283abe3dfc3de542ebdcc701c4c996a96c2be39ed59e5137ac83`  
		Last Modified: Tue, 12 Jul 2022 01:52:21 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29fbdc9d2624616a1188b80790c80688aba8f17538b784d1ec937ba763d0caca`  
		Last Modified: Tue, 12 Jul 2022 01:52:38 GMT  
		Size: 107.5 MB (107508121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87a306bac37ec6ca492ea124d5aab4a2015656c9bbcf1d82aa693a2df13241d1`  
		Last Modified: Tue, 12 Jul 2022 01:52:21 GMT  
		Size: 845.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3396c7604c38680b49a32a26d9e55ae095981acb8d33fd75c844fa5b6b0edc39`  
		Last Modified: Tue, 12 Jul 2022 01:52:21 GMT  
		Size: 5.2 KB (5157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:832af0332a2a6d268d5173bf633da9f00789d1970b6992fba3a7c49b208aca38`  
		Last Modified: Tue, 12 Jul 2022 01:52:21 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0.29-oracle`

```console
$ docker pull mysql@sha256:152cf187a3efc56afb0b3877b4d21e231d1d6eb828ca9221056590b0ac834c75
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8.0.29-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:44f98f4dd825a945d2a6a4b7b2f14127b5d07c5aaa07d9d232c2b58936fb76dc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.8 MB (131789857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33037edcac9b155a185e9555a5da711d754c88cb244e3d13e214db029c3b28ed`
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
# Wed, 13 Jul 2022 06:45:09 GMT
ENV MYSQL_VERSION=8.0.29-1.el8
# Wed, 13 Jul 2022 06:45:10 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 13 Jul 2022 06:45:38 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 13 Jul 2022 06:45:39 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 13 Jul 2022 06:45:39 GMT
ENV MYSQL_SHELL_VERSION=8.0.29-1.el8
# Wed, 13 Jul 2022 06:46:10 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Wed, 13 Jul 2022 06:46:10 GMT
VOLUME [/var/lib/mysql]
# Wed, 13 Jul 2022 06:46:11 GMT
COPY file:d27cf504fa76fb5a4038020a01eaaf52723b17b751566119de311adacb043752 in /usr/local/bin/ 
# Wed, 13 Jul 2022 06:46:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 13 Jul 2022 06:46:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 Jul 2022 06:46:11 GMT
EXPOSE 3306 33060
# Wed, 13 Jul 2022 06:46:11 GMT
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
	-	`sha256:7d1cc1ea1b3d8d62693939510193ad4b1c95748bcdcbb85e4a865555416fa2ce`  
		Last Modified: Wed, 13 Jul 2022 06:48:11 GMT  
		Size: 337.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d48f3c15cb803b81492348c7b8c160e9a9d3957dc0cc567b76893ec9dd3afd78`  
		Last Modified: Wed, 13 Jul 2022 06:48:16 GMT  
		Size: 47.3 MB (47260752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94c3d7b2c9ae878ae450aab764713dca9f718d37c21407ee84f36ce15c4f28d8`  
		Last Modified: Wed, 13 Jul 2022 06:48:09 GMT  
		Size: 318.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6cfbf240ed7196ec43fc009b344e17a6c84451079f19efea7b3fd2dab9bd65e`  
		Last Modified: Wed, 13 Jul 2022 06:48:16 GMT  
		Size: 39.8 MB (39780528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e12b159b2a12d49839093db700fe67feaa672b5461c59fda8c886799561195b5`  
		Last Modified: Wed, 13 Jul 2022 06:48:08 GMT  
		Size: 5.2 KB (5163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e93c6fd777f87eef9811f067b652a8d38e533ad87901fcd9648a3091f8b3a13`  
		Last Modified: Wed, 13 Jul 2022 06:48:08 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8.0.29-oracle` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:12cf01a51f803d0ad49ee0dbbb3025a6eef3341e24757c2ed8150b6654c3fb07
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.7 MB (138716495 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02662e079c08f45f90a837cf583cfb18bc58a400342d4fefde11199f3d1f4102`
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
# Wed, 13 Jul 2022 07:47:56 GMT
ENV MYSQL_VERSION=8.0.29-1.el8
# Wed, 13 Jul 2022 07:47:57 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 13 Jul 2022 07:48:22 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 13 Jul 2022 07:48:23 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 13 Jul 2022 07:48:24 GMT
ENV MYSQL_SHELL_VERSION=8.0.29-1.el8
# Wed, 13 Jul 2022 07:48:52 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Wed, 13 Jul 2022 07:48:52 GMT
VOLUME [/var/lib/mysql]
# Wed, 13 Jul 2022 07:48:54 GMT
COPY file:d27cf504fa76fb5a4038020a01eaaf52723b17b751566119de311adacb043752 in /usr/local/bin/ 
# Wed, 13 Jul 2022 07:48:54 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 13 Jul 2022 07:48:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 Jul 2022 07:48:56 GMT
EXPOSE 3306 33060
# Wed, 13 Jul 2022 07:48:57 GMT
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
	-	`sha256:a0c96e0313eb60e8210c676750efcb4e81ee7fa7f03d25753a285f1099d6ea2a`  
		Last Modified: Wed, 13 Jul 2022 07:49:26 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abbb3361f75b7791da51c4da9574c17f2c5bcf091461d36ae7c0f28b04a29360`  
		Last Modified: Wed, 13 Jul 2022 07:49:31 GMT  
		Size: 53.3 MB (53324981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:857f6a6ae5074bea540b73b0b8be220f0ff784d5de971d89bfac6374807c760c`  
		Last Modified: Wed, 13 Jul 2022 07:49:24 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ac3d9a78b39cb7d140f50375303fca9c8f7635c31377217dd93b494d5a3bced`  
		Last Modified: Wed, 13 Jul 2022 07:49:32 GMT  
		Size: 42.1 MB (42075330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a07911c3362fc1fbaa9b5018facd4ea2e98408f9923338d8fea847048357b30e`  
		Last Modified: Wed, 13 Jul 2022 07:49:24 GMT  
		Size: 5.2 KB (5158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fce3f4951dffafbeebe224f95703722f1f44783a530c658ecd594a3f32252a3f`  
		Last Modified: Wed, 13 Jul 2022 07:49:24 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:debian`

```console
$ docker pull mysql@sha256:5ef1130b5a6ebd5c2f31f0244c25027c47fb5a7279ad747026b495414adaaf27
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:debian` - linux; amd64

```console
$ docker pull mysql@sha256:3a7e864bc88458911fa598065fe027736fa63495f5780ee0618caeb4a52bbc4c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **157.4 MB (157380412 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0fc0e2322d42dbab9448b7af63601f09cbd916193afec376675bf32fdbca5203`
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
# Tue, 12 Jul 2022 01:50:12 GMT
ENV MYSQL_VERSION=8.0.29-1debian11
# Tue, 12 Jul 2022 01:50:13 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ bullseye mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Tue, 12 Jul 2022 01:50:28 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 12 Jul 2022 01:50:29 GMT
VOLUME [/var/lib/mysql]
# Tue, 12 Jul 2022 01:50:29 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Tue, 12 Jul 2022 01:50:29 GMT
COPY file:d27cf504fa76fb5a4038020a01eaaf52723b17b751566119de311adacb043752 in /usr/local/bin/ 
# Tue, 12 Jul 2022 01:50:29 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 12 Jul 2022 01:50:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Jul 2022 01:50:30 GMT
EXPOSE 3306 33060
# Tue, 12 Jul 2022 01:50:30 GMT
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
	-	`sha256:a7ddfbeb275b283abe3dfc3de542ebdcc701c4c996a96c2be39ed59e5137ac83`  
		Last Modified: Tue, 12 Jul 2022 01:52:21 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29fbdc9d2624616a1188b80790c80688aba8f17538b784d1ec937ba763d0caca`  
		Last Modified: Tue, 12 Jul 2022 01:52:38 GMT  
		Size: 107.5 MB (107508121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87a306bac37ec6ca492ea124d5aab4a2015656c9bbcf1d82aa693a2df13241d1`  
		Last Modified: Tue, 12 Jul 2022 01:52:21 GMT  
		Size: 845.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3396c7604c38680b49a32a26d9e55ae095981acb8d33fd75c844fa5b6b0edc39`  
		Last Modified: Tue, 12 Jul 2022 01:52:21 GMT  
		Size: 5.2 KB (5157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:832af0332a2a6d268d5173bf633da9f00789d1970b6992fba3a7c49b208aca38`  
		Last Modified: Tue, 12 Jul 2022 01:52:21 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:latest`

```console
$ docker pull mysql@sha256:152cf187a3efc56afb0b3877b4d21e231d1d6eb828ca9221056590b0ac834c75
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:latest` - linux; amd64

```console
$ docker pull mysql@sha256:44f98f4dd825a945d2a6a4b7b2f14127b5d07c5aaa07d9d232c2b58936fb76dc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.8 MB (131789857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33037edcac9b155a185e9555a5da711d754c88cb244e3d13e214db029c3b28ed`
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
# Wed, 13 Jul 2022 06:45:09 GMT
ENV MYSQL_VERSION=8.0.29-1.el8
# Wed, 13 Jul 2022 06:45:10 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 13 Jul 2022 06:45:38 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 13 Jul 2022 06:45:39 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 13 Jul 2022 06:45:39 GMT
ENV MYSQL_SHELL_VERSION=8.0.29-1.el8
# Wed, 13 Jul 2022 06:46:10 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Wed, 13 Jul 2022 06:46:10 GMT
VOLUME [/var/lib/mysql]
# Wed, 13 Jul 2022 06:46:11 GMT
COPY file:d27cf504fa76fb5a4038020a01eaaf52723b17b751566119de311adacb043752 in /usr/local/bin/ 
# Wed, 13 Jul 2022 06:46:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 13 Jul 2022 06:46:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 Jul 2022 06:46:11 GMT
EXPOSE 3306 33060
# Wed, 13 Jul 2022 06:46:11 GMT
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
	-	`sha256:7d1cc1ea1b3d8d62693939510193ad4b1c95748bcdcbb85e4a865555416fa2ce`  
		Last Modified: Wed, 13 Jul 2022 06:48:11 GMT  
		Size: 337.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d48f3c15cb803b81492348c7b8c160e9a9d3957dc0cc567b76893ec9dd3afd78`  
		Last Modified: Wed, 13 Jul 2022 06:48:16 GMT  
		Size: 47.3 MB (47260752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94c3d7b2c9ae878ae450aab764713dca9f718d37c21407ee84f36ce15c4f28d8`  
		Last Modified: Wed, 13 Jul 2022 06:48:09 GMT  
		Size: 318.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6cfbf240ed7196ec43fc009b344e17a6c84451079f19efea7b3fd2dab9bd65e`  
		Last Modified: Wed, 13 Jul 2022 06:48:16 GMT  
		Size: 39.8 MB (39780528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e12b159b2a12d49839093db700fe67feaa672b5461c59fda8c886799561195b5`  
		Last Modified: Wed, 13 Jul 2022 06:48:08 GMT  
		Size: 5.2 KB (5163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e93c6fd777f87eef9811f067b652a8d38e533ad87901fcd9648a3091f8b3a13`  
		Last Modified: Wed, 13 Jul 2022 06:48:08 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:latest` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:12cf01a51f803d0ad49ee0dbbb3025a6eef3341e24757c2ed8150b6654c3fb07
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.7 MB (138716495 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02662e079c08f45f90a837cf583cfb18bc58a400342d4fefde11199f3d1f4102`
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
# Wed, 13 Jul 2022 07:47:56 GMT
ENV MYSQL_VERSION=8.0.29-1.el8
# Wed, 13 Jul 2022 07:47:57 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 13 Jul 2022 07:48:22 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 13 Jul 2022 07:48:23 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 13 Jul 2022 07:48:24 GMT
ENV MYSQL_SHELL_VERSION=8.0.29-1.el8
# Wed, 13 Jul 2022 07:48:52 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Wed, 13 Jul 2022 07:48:52 GMT
VOLUME [/var/lib/mysql]
# Wed, 13 Jul 2022 07:48:54 GMT
COPY file:d27cf504fa76fb5a4038020a01eaaf52723b17b751566119de311adacb043752 in /usr/local/bin/ 
# Wed, 13 Jul 2022 07:48:54 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 13 Jul 2022 07:48:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 Jul 2022 07:48:56 GMT
EXPOSE 3306 33060
# Wed, 13 Jul 2022 07:48:57 GMT
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
	-	`sha256:a0c96e0313eb60e8210c676750efcb4e81ee7fa7f03d25753a285f1099d6ea2a`  
		Last Modified: Wed, 13 Jul 2022 07:49:26 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abbb3361f75b7791da51c4da9574c17f2c5bcf091461d36ae7c0f28b04a29360`  
		Last Modified: Wed, 13 Jul 2022 07:49:31 GMT  
		Size: 53.3 MB (53324981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:857f6a6ae5074bea540b73b0b8be220f0ff784d5de971d89bfac6374807c760c`  
		Last Modified: Wed, 13 Jul 2022 07:49:24 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ac3d9a78b39cb7d140f50375303fca9c8f7635c31377217dd93b494d5a3bced`  
		Last Modified: Wed, 13 Jul 2022 07:49:32 GMT  
		Size: 42.1 MB (42075330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a07911c3362fc1fbaa9b5018facd4ea2e98408f9923338d8fea847048357b30e`  
		Last Modified: Wed, 13 Jul 2022 07:49:24 GMT  
		Size: 5.2 KB (5158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fce3f4951dffafbeebe224f95703722f1f44783a530c658ecd594a3f32252a3f`  
		Last Modified: Wed, 13 Jul 2022 07:49:24 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:oracle`

```console
$ docker pull mysql@sha256:152cf187a3efc56afb0b3877b4d21e231d1d6eb828ca9221056590b0ac834c75
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:oracle` - linux; amd64

```console
$ docker pull mysql@sha256:44f98f4dd825a945d2a6a4b7b2f14127b5d07c5aaa07d9d232c2b58936fb76dc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.8 MB (131789857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33037edcac9b155a185e9555a5da711d754c88cb244e3d13e214db029c3b28ed`
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
# Wed, 13 Jul 2022 06:45:09 GMT
ENV MYSQL_VERSION=8.0.29-1.el8
# Wed, 13 Jul 2022 06:45:10 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 13 Jul 2022 06:45:38 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 13 Jul 2022 06:45:39 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 13 Jul 2022 06:45:39 GMT
ENV MYSQL_SHELL_VERSION=8.0.29-1.el8
# Wed, 13 Jul 2022 06:46:10 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Wed, 13 Jul 2022 06:46:10 GMT
VOLUME [/var/lib/mysql]
# Wed, 13 Jul 2022 06:46:11 GMT
COPY file:d27cf504fa76fb5a4038020a01eaaf52723b17b751566119de311adacb043752 in /usr/local/bin/ 
# Wed, 13 Jul 2022 06:46:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 13 Jul 2022 06:46:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 Jul 2022 06:46:11 GMT
EXPOSE 3306 33060
# Wed, 13 Jul 2022 06:46:11 GMT
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
	-	`sha256:7d1cc1ea1b3d8d62693939510193ad4b1c95748bcdcbb85e4a865555416fa2ce`  
		Last Modified: Wed, 13 Jul 2022 06:48:11 GMT  
		Size: 337.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d48f3c15cb803b81492348c7b8c160e9a9d3957dc0cc567b76893ec9dd3afd78`  
		Last Modified: Wed, 13 Jul 2022 06:48:16 GMT  
		Size: 47.3 MB (47260752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94c3d7b2c9ae878ae450aab764713dca9f718d37c21407ee84f36ce15c4f28d8`  
		Last Modified: Wed, 13 Jul 2022 06:48:09 GMT  
		Size: 318.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6cfbf240ed7196ec43fc009b344e17a6c84451079f19efea7b3fd2dab9bd65e`  
		Last Modified: Wed, 13 Jul 2022 06:48:16 GMT  
		Size: 39.8 MB (39780528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e12b159b2a12d49839093db700fe67feaa672b5461c59fda8c886799561195b5`  
		Last Modified: Wed, 13 Jul 2022 06:48:08 GMT  
		Size: 5.2 KB (5163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e93c6fd777f87eef9811f067b652a8d38e533ad87901fcd9648a3091f8b3a13`  
		Last Modified: Wed, 13 Jul 2022 06:48:08 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:oracle` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:12cf01a51f803d0ad49ee0dbbb3025a6eef3341e24757c2ed8150b6654c3fb07
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.7 MB (138716495 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02662e079c08f45f90a837cf583cfb18bc58a400342d4fefde11199f3d1f4102`
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
# Wed, 13 Jul 2022 07:47:56 GMT
ENV MYSQL_VERSION=8.0.29-1.el8
# Wed, 13 Jul 2022 07:47:57 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 13 Jul 2022 07:48:22 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 13 Jul 2022 07:48:23 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 13 Jul 2022 07:48:24 GMT
ENV MYSQL_SHELL_VERSION=8.0.29-1.el8
# Wed, 13 Jul 2022 07:48:52 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Wed, 13 Jul 2022 07:48:52 GMT
VOLUME [/var/lib/mysql]
# Wed, 13 Jul 2022 07:48:54 GMT
COPY file:d27cf504fa76fb5a4038020a01eaaf52723b17b751566119de311adacb043752 in /usr/local/bin/ 
# Wed, 13 Jul 2022 07:48:54 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 13 Jul 2022 07:48:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 Jul 2022 07:48:56 GMT
EXPOSE 3306 33060
# Wed, 13 Jul 2022 07:48:57 GMT
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
	-	`sha256:a0c96e0313eb60e8210c676750efcb4e81ee7fa7f03d25753a285f1099d6ea2a`  
		Last Modified: Wed, 13 Jul 2022 07:49:26 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abbb3361f75b7791da51c4da9574c17f2c5bcf091461d36ae7c0f28b04a29360`  
		Last Modified: Wed, 13 Jul 2022 07:49:31 GMT  
		Size: 53.3 MB (53324981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:857f6a6ae5074bea540b73b0b8be220f0ff784d5de971d89bfac6374807c760c`  
		Last Modified: Wed, 13 Jul 2022 07:49:24 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ac3d9a78b39cb7d140f50375303fca9c8f7635c31377217dd93b494d5a3bced`  
		Last Modified: Wed, 13 Jul 2022 07:49:32 GMT  
		Size: 42.1 MB (42075330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a07911c3362fc1fbaa9b5018facd4ea2e98408f9923338d8fea847048357b30e`  
		Last Modified: Wed, 13 Jul 2022 07:49:24 GMT  
		Size: 5.2 KB (5158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fce3f4951dffafbeebe224f95703722f1f44783a530c658ecd594a3f32252a3f`  
		Last Modified: Wed, 13 Jul 2022 07:49:24 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
