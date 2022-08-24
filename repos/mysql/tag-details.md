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
$ docker pull mysql@sha256:b92fae25c5d06050380903a38adb5965f8f19f1fb8f426b5940a34310e5498f6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5` - linux; amd64

```console
$ docker pull mysql@sha256:69d6aea96669a23edd9fdf8c98f2461ba7b0917dd5bdd22b98cd14e6718810ae
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.4 MB (128373820 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ebcbf7d9efcb14f59993708a14baa242efb6fa9417a1d64c4acc48d2b4c64e3c`
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
# Wed, 24 Aug 2022 00:36:56 GMT
COPY file:0362167b353388be7fb99432d9373f030ddd789bd27d57e183555c672530b303 in /usr/local/bin/ 
# Wed, 24 Aug 2022 00:36:56 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 24 Aug 2022 00:36:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 24 Aug 2022 00:36:57 GMT
EXPOSE 3306 33060
# Wed, 24 Aug 2022 00:36:57 GMT
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
	-	`sha256:1812e337741544527115d426c156181ac4635cb7afa49de63f68f2b583b638be`  
		Last Modified: Wed, 24 Aug 2022 00:38:08 GMT  
		Size: 5.4 KB (5376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69105ed9bd3515a09430faa732ee4ca74c9676f78f5075b92b948791de077eeb`  
		Last Modified: Wed, 24 Aug 2022 00:38:08 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5-debian`

```console
$ docker pull mysql@sha256:205e4668c88c3b25a32280ea91a3ff2ba90d89dd0f42ce11de3826cbbed58e3a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5-debian` - linux; amd64

```console
$ docker pull mysql@sha256:b81837e100796b465638fc10ec12f7002260b09f035e3d2e9419d235e343d760
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **162.5 MB (162534517 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c76ecb9ed4957423285a314df6e6f63688652616dc0c41c9e15d0a8fdd13e2e1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 23 Aug 2022 00:21:10 GMT
ADD file:baca493d7744d12304f6d9c7b6ec0800453a0ba02cbf4005ec35c7b921adf0c4 in / 
# Tue, 23 Aug 2022 00:21:10 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 03:39:04 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 23 Aug 2022 03:39:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 03:39:09 GMT
ENV GOSU_VERSION=1.14
# Tue, 23 Aug 2022 03:39:18 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 23 Aug 2022 03:39:18 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 23 Aug 2022 03:39:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 03:39:26 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Tue, 23 Aug 2022 03:39:26 GMT
ENV MYSQL_MAJOR=5.7
# Tue, 23 Aug 2022 03:39:26 GMT
ENV MYSQL_VERSION=5.7.39-1debian10
# Tue, 23 Aug 2022 03:39:26 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-5.7' > /etc/apt/sources.list.d/mysql.list
# Tue, 23 Aug 2022 03:39:45 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-server="${MYSQL_VERSION}" 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 23 Aug 2022 03:39:45 GMT
VOLUME [/var/lib/mysql]
# Wed, 24 Aug 2022 00:37:00 GMT
COPY file:0362167b353388be7fb99432d9373f030ddd789bd27d57e183555c672530b303 in /usr/local/bin/ 
# Wed, 24 Aug 2022 00:37:00 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 24 Aug 2022 00:37:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 24 Aug 2022 00:37:00 GMT
EXPOSE 3306 33060
# Wed, 24 Aug 2022 00:37:01 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:2238450926aa858e592e60bb5d68dd26eeab8a984eee45505ca89d2022e3b450`  
		Last Modified: Tue, 23 Aug 2022 00:25:43 GMT  
		Size: 27.1 MB (27138330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71c5f740138266af637c12e92100241c142f69f19afc2cdc08a8b88d8e15cc6f`  
		Last Modified: Tue, 23 Aug 2022 03:40:57 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04c7f3adca1d7944d8c4bc63ecc1b8c511277bd69708b6a03b25f1743af7407e`  
		Last Modified: Tue, 23 Aug 2022 03:40:56 GMT  
		Size: 4.2 MB (4179233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cfac0455131411929e3fe47e882af36deff875d8595e630528618f590043c64`  
		Last Modified: Tue, 23 Aug 2022 03:40:55 GMT  
		Size: 1.4 MB (1386663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92da0306d995cc66b0091fa6ccf90121d5191ea326140c7f4d3c8d22b161b20`  
		Last Modified: Tue, 23 Aug 2022 03:40:55 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4b7cacb26da7b4d5183a528f7546a036f892791f689774e3075769f3ecb8efc`  
		Last Modified: Tue, 23 Aug 2022 03:40:57 GMT  
		Size: 14.1 MB (14086922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2ecb04aa1e751586d9c53589b45644d0055a250206b6117f019282b755cb41f`  
		Last Modified: Tue, 23 Aug 2022 03:40:52 GMT  
		Size: 2.5 KB (2549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23d5c9ab78dc4df78482099775fb74be8fa52da67aaf1dae367fa4ac39a1338c`  
		Last Modified: Tue, 23 Aug 2022 03:40:52 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:780804703dd6fc54b6fe4c9bb3201e23ae222a1a5899fa23804bd1b8e205a578`  
		Last Modified: Tue, 23 Aug 2022 03:41:08 GMT  
		Size: 115.7 MB (115733196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d355f958aceb57647de7b16c6c52e724e941c44cf7dbda97092a2f13afe17f5`  
		Last Modified: Wed, 24 Aug 2022 00:38:30 GMT  
		Size: 5.4 KB (5370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab0da5240bdc1d44cc7e1ff164a950c1099639afbc1348ed78b1ae209052a330`  
		Last Modified: Wed, 24 Aug 2022 00:38:30 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5-oracle`

```console
$ docker pull mysql@sha256:b92fae25c5d06050380903a38adb5965f8f19f1fb8f426b5940a34310e5498f6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:69d6aea96669a23edd9fdf8c98f2461ba7b0917dd5bdd22b98cd14e6718810ae
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.4 MB (128373820 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ebcbf7d9efcb14f59993708a14baa242efb6fa9417a1d64c4acc48d2b4c64e3c`
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
# Wed, 24 Aug 2022 00:36:56 GMT
COPY file:0362167b353388be7fb99432d9373f030ddd789bd27d57e183555c672530b303 in /usr/local/bin/ 
# Wed, 24 Aug 2022 00:36:56 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 24 Aug 2022 00:36:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 24 Aug 2022 00:36:57 GMT
EXPOSE 3306 33060
# Wed, 24 Aug 2022 00:36:57 GMT
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
	-	`sha256:1812e337741544527115d426c156181ac4635cb7afa49de63f68f2b583b638be`  
		Last Modified: Wed, 24 Aug 2022 00:38:08 GMT  
		Size: 5.4 KB (5376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69105ed9bd3515a09430faa732ee4ca74c9676f78f5075b92b948791de077eeb`  
		Last Modified: Wed, 24 Aug 2022 00:38:08 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7`

```console
$ docker pull mysql@sha256:b92fae25c5d06050380903a38adb5965f8f19f1fb8f426b5940a34310e5498f6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7` - linux; amd64

```console
$ docker pull mysql@sha256:69d6aea96669a23edd9fdf8c98f2461ba7b0917dd5bdd22b98cd14e6718810ae
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.4 MB (128373820 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ebcbf7d9efcb14f59993708a14baa242efb6fa9417a1d64c4acc48d2b4c64e3c`
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
# Wed, 24 Aug 2022 00:36:56 GMT
COPY file:0362167b353388be7fb99432d9373f030ddd789bd27d57e183555c672530b303 in /usr/local/bin/ 
# Wed, 24 Aug 2022 00:36:56 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 24 Aug 2022 00:36:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 24 Aug 2022 00:36:57 GMT
EXPOSE 3306 33060
# Wed, 24 Aug 2022 00:36:57 GMT
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
	-	`sha256:1812e337741544527115d426c156181ac4635cb7afa49de63f68f2b583b638be`  
		Last Modified: Wed, 24 Aug 2022 00:38:08 GMT  
		Size: 5.4 KB (5376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69105ed9bd3515a09430faa732ee4ca74c9676f78f5075b92b948791de077eeb`  
		Last Modified: Wed, 24 Aug 2022 00:38:08 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7-debian`

```console
$ docker pull mysql@sha256:205e4668c88c3b25a32280ea91a3ff2ba90d89dd0f42ce11de3826cbbed58e3a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7-debian` - linux; amd64

```console
$ docker pull mysql@sha256:b81837e100796b465638fc10ec12f7002260b09f035e3d2e9419d235e343d760
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **162.5 MB (162534517 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c76ecb9ed4957423285a314df6e6f63688652616dc0c41c9e15d0a8fdd13e2e1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 23 Aug 2022 00:21:10 GMT
ADD file:baca493d7744d12304f6d9c7b6ec0800453a0ba02cbf4005ec35c7b921adf0c4 in / 
# Tue, 23 Aug 2022 00:21:10 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 03:39:04 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 23 Aug 2022 03:39:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 03:39:09 GMT
ENV GOSU_VERSION=1.14
# Tue, 23 Aug 2022 03:39:18 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 23 Aug 2022 03:39:18 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 23 Aug 2022 03:39:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 03:39:26 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Tue, 23 Aug 2022 03:39:26 GMT
ENV MYSQL_MAJOR=5.7
# Tue, 23 Aug 2022 03:39:26 GMT
ENV MYSQL_VERSION=5.7.39-1debian10
# Tue, 23 Aug 2022 03:39:26 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-5.7' > /etc/apt/sources.list.d/mysql.list
# Tue, 23 Aug 2022 03:39:45 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-server="${MYSQL_VERSION}" 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 23 Aug 2022 03:39:45 GMT
VOLUME [/var/lib/mysql]
# Wed, 24 Aug 2022 00:37:00 GMT
COPY file:0362167b353388be7fb99432d9373f030ddd789bd27d57e183555c672530b303 in /usr/local/bin/ 
# Wed, 24 Aug 2022 00:37:00 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 24 Aug 2022 00:37:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 24 Aug 2022 00:37:00 GMT
EXPOSE 3306 33060
# Wed, 24 Aug 2022 00:37:01 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:2238450926aa858e592e60bb5d68dd26eeab8a984eee45505ca89d2022e3b450`  
		Last Modified: Tue, 23 Aug 2022 00:25:43 GMT  
		Size: 27.1 MB (27138330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71c5f740138266af637c12e92100241c142f69f19afc2cdc08a8b88d8e15cc6f`  
		Last Modified: Tue, 23 Aug 2022 03:40:57 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04c7f3adca1d7944d8c4bc63ecc1b8c511277bd69708b6a03b25f1743af7407e`  
		Last Modified: Tue, 23 Aug 2022 03:40:56 GMT  
		Size: 4.2 MB (4179233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cfac0455131411929e3fe47e882af36deff875d8595e630528618f590043c64`  
		Last Modified: Tue, 23 Aug 2022 03:40:55 GMT  
		Size: 1.4 MB (1386663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92da0306d995cc66b0091fa6ccf90121d5191ea326140c7f4d3c8d22b161b20`  
		Last Modified: Tue, 23 Aug 2022 03:40:55 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4b7cacb26da7b4d5183a528f7546a036f892791f689774e3075769f3ecb8efc`  
		Last Modified: Tue, 23 Aug 2022 03:40:57 GMT  
		Size: 14.1 MB (14086922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2ecb04aa1e751586d9c53589b45644d0055a250206b6117f019282b755cb41f`  
		Last Modified: Tue, 23 Aug 2022 03:40:52 GMT  
		Size: 2.5 KB (2549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23d5c9ab78dc4df78482099775fb74be8fa52da67aaf1dae367fa4ac39a1338c`  
		Last Modified: Tue, 23 Aug 2022 03:40:52 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:780804703dd6fc54b6fe4c9bb3201e23ae222a1a5899fa23804bd1b8e205a578`  
		Last Modified: Tue, 23 Aug 2022 03:41:08 GMT  
		Size: 115.7 MB (115733196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d355f958aceb57647de7b16c6c52e724e941c44cf7dbda97092a2f13afe17f5`  
		Last Modified: Wed, 24 Aug 2022 00:38:30 GMT  
		Size: 5.4 KB (5370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab0da5240bdc1d44cc7e1ff164a950c1099639afbc1348ed78b1ae209052a330`  
		Last Modified: Wed, 24 Aug 2022 00:38:30 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7-oracle`

```console
$ docker pull mysql@sha256:b92fae25c5d06050380903a38adb5965f8f19f1fb8f426b5940a34310e5498f6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:69d6aea96669a23edd9fdf8c98f2461ba7b0917dd5bdd22b98cd14e6718810ae
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.4 MB (128373820 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ebcbf7d9efcb14f59993708a14baa242efb6fa9417a1d64c4acc48d2b4c64e3c`
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
# Wed, 24 Aug 2022 00:36:56 GMT
COPY file:0362167b353388be7fb99432d9373f030ddd789bd27d57e183555c672530b303 in /usr/local/bin/ 
# Wed, 24 Aug 2022 00:36:56 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 24 Aug 2022 00:36:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 24 Aug 2022 00:36:57 GMT
EXPOSE 3306 33060
# Wed, 24 Aug 2022 00:36:57 GMT
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
	-	`sha256:1812e337741544527115d426c156181ac4635cb7afa49de63f68f2b583b638be`  
		Last Modified: Wed, 24 Aug 2022 00:38:08 GMT  
		Size: 5.4 KB (5376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69105ed9bd3515a09430faa732ee4ca74c9676f78f5075b92b948791de077eeb`  
		Last Modified: Wed, 24 Aug 2022 00:38:08 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7.39`

```console
$ docker pull mysql@sha256:b92fae25c5d06050380903a38adb5965f8f19f1fb8f426b5940a34310e5498f6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7.39` - linux; amd64

```console
$ docker pull mysql@sha256:69d6aea96669a23edd9fdf8c98f2461ba7b0917dd5bdd22b98cd14e6718810ae
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.4 MB (128373820 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ebcbf7d9efcb14f59993708a14baa242efb6fa9417a1d64c4acc48d2b4c64e3c`
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
# Wed, 24 Aug 2022 00:36:56 GMT
COPY file:0362167b353388be7fb99432d9373f030ddd789bd27d57e183555c672530b303 in /usr/local/bin/ 
# Wed, 24 Aug 2022 00:36:56 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 24 Aug 2022 00:36:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 24 Aug 2022 00:36:57 GMT
EXPOSE 3306 33060
# Wed, 24 Aug 2022 00:36:57 GMT
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
	-	`sha256:1812e337741544527115d426c156181ac4635cb7afa49de63f68f2b583b638be`  
		Last Modified: Wed, 24 Aug 2022 00:38:08 GMT  
		Size: 5.4 KB (5376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69105ed9bd3515a09430faa732ee4ca74c9676f78f5075b92b948791de077eeb`  
		Last Modified: Wed, 24 Aug 2022 00:38:08 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7.39-debian`

```console
$ docker pull mysql@sha256:205e4668c88c3b25a32280ea91a3ff2ba90d89dd0f42ce11de3826cbbed58e3a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7.39-debian` - linux; amd64

```console
$ docker pull mysql@sha256:b81837e100796b465638fc10ec12f7002260b09f035e3d2e9419d235e343d760
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **162.5 MB (162534517 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c76ecb9ed4957423285a314df6e6f63688652616dc0c41c9e15d0a8fdd13e2e1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 23 Aug 2022 00:21:10 GMT
ADD file:baca493d7744d12304f6d9c7b6ec0800453a0ba02cbf4005ec35c7b921adf0c4 in / 
# Tue, 23 Aug 2022 00:21:10 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 03:39:04 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 23 Aug 2022 03:39:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 03:39:09 GMT
ENV GOSU_VERSION=1.14
# Tue, 23 Aug 2022 03:39:18 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 23 Aug 2022 03:39:18 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 23 Aug 2022 03:39:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 03:39:26 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Tue, 23 Aug 2022 03:39:26 GMT
ENV MYSQL_MAJOR=5.7
# Tue, 23 Aug 2022 03:39:26 GMT
ENV MYSQL_VERSION=5.7.39-1debian10
# Tue, 23 Aug 2022 03:39:26 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-5.7' > /etc/apt/sources.list.d/mysql.list
# Tue, 23 Aug 2022 03:39:45 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-server="${MYSQL_VERSION}" 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 23 Aug 2022 03:39:45 GMT
VOLUME [/var/lib/mysql]
# Wed, 24 Aug 2022 00:37:00 GMT
COPY file:0362167b353388be7fb99432d9373f030ddd789bd27d57e183555c672530b303 in /usr/local/bin/ 
# Wed, 24 Aug 2022 00:37:00 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 24 Aug 2022 00:37:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 24 Aug 2022 00:37:00 GMT
EXPOSE 3306 33060
# Wed, 24 Aug 2022 00:37:01 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:2238450926aa858e592e60bb5d68dd26eeab8a984eee45505ca89d2022e3b450`  
		Last Modified: Tue, 23 Aug 2022 00:25:43 GMT  
		Size: 27.1 MB (27138330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71c5f740138266af637c12e92100241c142f69f19afc2cdc08a8b88d8e15cc6f`  
		Last Modified: Tue, 23 Aug 2022 03:40:57 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04c7f3adca1d7944d8c4bc63ecc1b8c511277bd69708b6a03b25f1743af7407e`  
		Last Modified: Tue, 23 Aug 2022 03:40:56 GMT  
		Size: 4.2 MB (4179233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cfac0455131411929e3fe47e882af36deff875d8595e630528618f590043c64`  
		Last Modified: Tue, 23 Aug 2022 03:40:55 GMT  
		Size: 1.4 MB (1386663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92da0306d995cc66b0091fa6ccf90121d5191ea326140c7f4d3c8d22b161b20`  
		Last Modified: Tue, 23 Aug 2022 03:40:55 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4b7cacb26da7b4d5183a528f7546a036f892791f689774e3075769f3ecb8efc`  
		Last Modified: Tue, 23 Aug 2022 03:40:57 GMT  
		Size: 14.1 MB (14086922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2ecb04aa1e751586d9c53589b45644d0055a250206b6117f019282b755cb41f`  
		Last Modified: Tue, 23 Aug 2022 03:40:52 GMT  
		Size: 2.5 KB (2549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23d5c9ab78dc4df78482099775fb74be8fa52da67aaf1dae367fa4ac39a1338c`  
		Last Modified: Tue, 23 Aug 2022 03:40:52 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:780804703dd6fc54b6fe4c9bb3201e23ae222a1a5899fa23804bd1b8e205a578`  
		Last Modified: Tue, 23 Aug 2022 03:41:08 GMT  
		Size: 115.7 MB (115733196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d355f958aceb57647de7b16c6c52e724e941c44cf7dbda97092a2f13afe17f5`  
		Last Modified: Wed, 24 Aug 2022 00:38:30 GMT  
		Size: 5.4 KB (5370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab0da5240bdc1d44cc7e1ff164a950c1099639afbc1348ed78b1ae209052a330`  
		Last Modified: Wed, 24 Aug 2022 00:38:30 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7.39-oracle`

```console
$ docker pull mysql@sha256:b92fae25c5d06050380903a38adb5965f8f19f1fb8f426b5940a34310e5498f6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7.39-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:69d6aea96669a23edd9fdf8c98f2461ba7b0917dd5bdd22b98cd14e6718810ae
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.4 MB (128373820 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ebcbf7d9efcb14f59993708a14baa242efb6fa9417a1d64c4acc48d2b4c64e3c`
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
# Wed, 24 Aug 2022 00:36:56 GMT
COPY file:0362167b353388be7fb99432d9373f030ddd789bd27d57e183555c672530b303 in /usr/local/bin/ 
# Wed, 24 Aug 2022 00:36:56 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 24 Aug 2022 00:36:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 24 Aug 2022 00:36:57 GMT
EXPOSE 3306 33060
# Wed, 24 Aug 2022 00:36:57 GMT
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
	-	`sha256:1812e337741544527115d426c156181ac4635cb7afa49de63f68f2b583b638be`  
		Last Modified: Wed, 24 Aug 2022 00:38:08 GMT  
		Size: 5.4 KB (5376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69105ed9bd3515a09430faa732ee4ca74c9676f78f5075b92b948791de077eeb`  
		Last Modified: Wed, 24 Aug 2022 00:38:08 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8`

```console
$ docker pull mysql@sha256:3de4d9814b28e48f225e259cc3b2c77530296afcec20bae53e1c7a4892f2a98e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8` - linux; amd64

```console
$ docker pull mysql@sha256:930e762c3f185d55d96a65e0d6cb2f724ffc16a87270f85283ae099d75e92ad0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.5 MB (132502250 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c989cc040bcf09e776e701e0fb567045ee77ed8667daf1a506d898717011bfe5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 04 Aug 2022 00:36:37 GMT
ADD file:0a05a213ae66f556b2b320291ac58ec9f2f67554e29338a072f1347f22864a49 in / 
# Thu, 04 Aug 2022 00:36:37 GMT
CMD ["/bin/bash"]
# Thu, 04 Aug 2022 01:24:42 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Thu, 04 Aug 2022 01:24:43 GMT
ENV GOSU_VERSION=1.14
# Thu, 04 Aug 2022 01:24:46 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 04 Aug 2022 01:25:08 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Thu, 04 Aug 2022 01:25:10 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Thu, 04 Aug 2022 01:25:10 GMT
ENV MYSQL_MAJOR=8.0
# Thu, 04 Aug 2022 01:25:10 GMT
ENV MYSQL_VERSION=8.0.30-1.el8
# Thu, 04 Aug 2022 01:25:10 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Thu, 04 Aug 2022 01:25:38 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Thu, 04 Aug 2022 01:25:39 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Thu, 04 Aug 2022 01:25:39 GMT
ENV MYSQL_SHELL_VERSION=8.0.30-1.el8
# Thu, 04 Aug 2022 01:26:10 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Thu, 04 Aug 2022 01:26:11 GMT
VOLUME [/var/lib/mysql]
# Wed, 24 Aug 2022 00:36:48 GMT
COPY file:0362167b353388be7fb99432d9373f030ddd789bd27d57e183555c672530b303 in /usr/local/bin/ 
# Wed, 24 Aug 2022 00:36:48 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 24 Aug 2022 00:36:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 24 Aug 2022 00:36:49 GMT
EXPOSE 3306 33060
# Wed, 24 Aug 2022 00:36:49 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:32c1bf40aba1f372a057d3280b0b7cdacde9d8500a069004e6f243bc09cde806`  
		Last Modified: Thu, 04 Aug 2022 00:37:33 GMT  
		Size: 39.2 MB (39223952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ac22f3a638d1c75f850c6c7b189d746c1ec6c58ec618f9e4b928f045df1b79d`  
		Last Modified: Thu, 04 Aug 2022 01:26:53 GMT  
		Size: 890.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1e7273ed05ed3b0f6be1e9a202f93199d88428c9dff52d1edce8d965ad50f8e`  
		Last Modified: Thu, 04 Aug 2022 01:26:54 GMT  
		Size: 928.8 KB (928835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20be45a0c6abbfaf62bd02c40f3cff6bf4822711b339ebcd4e1b7d6b2764ca20`  
		Last Modified: Thu, 04 Aug 2022 01:26:52 GMT  
		Size: 4.6 MB (4581809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:410a229693ff98f0a019a180a655ad903a882367b72f78f0ac3c595c1434a65e`  
		Last Modified: Thu, 04 Aug 2022 01:26:51 GMT  
		Size: 2.6 KB (2628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ce71e3a9b8879afc4dce1dc74841ecbae7da28798b238c88f0322b7bdc82472`  
		Last Modified: Thu, 04 Aug 2022 01:26:51 GMT  
		Size: 335.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c93c823af05bbde448c0a889b94ef2d6279b9c595c9b1a1abcbd49f795f7631c`  
		Last Modified: Thu, 04 Aug 2022 01:26:56 GMT  
		Size: 47.7 MB (47726773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6752c4d09c7204097f7ecbf50885874b620e77263452bb581ed1f4d9681344d`  
		Last Modified: Thu, 04 Aug 2022 01:26:49 GMT  
		Size: 315.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7f2cfe3efcbd4b98bf44100e9f3fc095ca4a480fd75a0028bae61aedfb6298a`  
		Last Modified: Thu, 04 Aug 2022 01:26:57 GMT  
		Size: 40.0 MB (40031217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09e782dbb2c3f52fb09d97fee4689b382e3789e244c209fe81782420a19d1a2a`  
		Last Modified: Wed, 24 Aug 2022 00:37:25 GMT  
		Size: 5.4 KB (5375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01199f522543dd7f72aa6b05d1be8d67dc48483700d79db260348af7e69f2aaa`  
		Last Modified: Wed, 24 Aug 2022 00:37:24 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:54b1f5e74608236fe20d5dcdf39124a81244dd4d043b0798929614c1bc1ec602
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.2 MB (141193701 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1b9c6058e7a1b8f805b067ba9d4775d392fcfda1cdd601396716864c8f59e14`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 04 Aug 2022 00:40:43 GMT
ADD file:a68d82fa032efe6adc2926f7e745508f0541bba3f906e2702d34252353100747 in / 
# Thu, 04 Aug 2022 00:40:44 GMT
CMD ["/bin/bash"]
# Thu, 04 Aug 2022 00:57:16 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Thu, 04 Aug 2022 00:57:17 GMT
ENV GOSU_VERSION=1.14
# Thu, 04 Aug 2022 00:57:21 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 04 Aug 2022 00:57:44 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Thu, 04 Aug 2022 00:57:46 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Thu, 04 Aug 2022 00:57:47 GMT
ENV MYSQL_MAJOR=8.0
# Thu, 04 Aug 2022 00:57:48 GMT
ENV MYSQL_VERSION=8.0.30-1.el8
# Thu, 04 Aug 2022 00:57:49 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Thu, 04 Aug 2022 00:58:17 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Thu, 04 Aug 2022 00:58:17 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Thu, 04 Aug 2022 00:58:18 GMT
ENV MYSQL_SHELL_VERSION=8.0.30-1.el8
# Thu, 04 Aug 2022 00:58:50 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Thu, 04 Aug 2022 00:58:51 GMT
VOLUME [/var/lib/mysql]
# Wed, 24 Aug 2022 03:30:34 GMT
COPY file:0362167b353388be7fb99432d9373f030ddd789bd27d57e183555c672530b303 in /usr/local/bin/ 
# Wed, 24 Aug 2022 03:30:35 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 24 Aug 2022 03:30:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 24 Aug 2022 03:30:37 GMT
EXPOSE 3306 33060
# Wed, 24 Aug 2022 03:30:38 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:ecf56004177eb6ca162c88de29e84bc4ba3d2e7efd3703df9ecae51b89003d52`  
		Last Modified: Thu, 04 Aug 2022 00:41:51 GMT  
		Size: 38.0 MB (38023046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1091d9f012e1e44cf00d872494ff008feb11a824aa940f5fccaadcf0f043e951`  
		Last Modified: Thu, 04 Aug 2022 00:59:35 GMT  
		Size: 888.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fabd9779d4678f8577c74505cc31bd42788a9ffa1eba563340b8ef29946b3e55`  
		Last Modified: Thu, 04 Aug 2022 00:59:36 GMT  
		Size: 857.2 KB (857152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6278448e2e194f0e2e8e7d2f29495296d594f7bd2e63d0306037e5b4f5125eb`  
		Last Modified: Thu, 04 Aug 2022 00:59:34 GMT  
		Size: 4.4 MB (4404159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6050832741b8d8e4dfba20e0d31c88f56b9b645c97752c9bbec708740c3e6e15`  
		Last Modified: Thu, 04 Aug 2022 00:59:33 GMT  
		Size: 2.6 KB (2607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0be9d1181fe5f7d6c39819a56c680e5e010a7b808b96eb00eabdeacd66ee6c1`  
		Last Modified: Thu, 04 Aug 2022 00:59:33 GMT  
		Size: 335.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbdaffd3eb50f6880d4e27c2ba2a47193ba4e1959b4647e5e794b0872e981c5b`  
		Last Modified: Thu, 04 Aug 2022 00:59:38 GMT  
		Size: 53.8 MB (53784614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a74c1ad0f09fc99fb019bcbfebb1b57f4f7fcf7e968e6ece353a06d583cab8ed`  
		Last Modified: Thu, 04 Aug 2022 00:59:31 GMT  
		Size: 315.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad2b7db10f4eacccefc72231d395d9920b81dd4bba86be2a8994b8ee9161ec92`  
		Last Modified: Thu, 04 Aug 2022 00:59:38 GMT  
		Size: 44.1 MB (44115089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f6281129c7fb0746caa0023cec4db82b482c85d81752eaafcff70498537c82a`  
		Last Modified: Wed, 24 Aug 2022 03:31:04 GMT  
		Size: 5.4 KB (5375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49dcabdef3045b25265175bee4894568254c4b35b769d77a0afedc6fd7ec9a1d`  
		Last Modified: Wed, 24 Aug 2022 03:31:04 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8-debian`

```console
$ docker pull mysql@sha256:1b9a6291084f62abdcba3d057e6932e5419910c469f506f627eb31756e1b4666
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:8-debian` - linux; amd64

```console
$ docker pull mysql@sha256:ae245d06921e615701b017b2f6ac7aedaaf4cdf351bf57302cab7bc732ef3766
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **157.9 MB (157850853 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:960207ea9ac0c08b0485963dd531c0fcb4409c980661579f474af0119032a90a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 23 Aug 2022 00:20:50 GMT
ADD file:7726efb0e0eb5003dbcf2967ec29364479eec8b41f2569ff189372153115b54b in / 
# Tue, 23 Aug 2022 00:20:51 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 03:38:21 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 23 Aug 2022 03:38:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 03:38:26 GMT
ENV GOSU_VERSION=1.14
# Tue, 23 Aug 2022 03:38:35 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 23 Aug 2022 03:38:36 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 23 Aug 2022 03:38:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 03:38:42 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Tue, 23 Aug 2022 03:38:42 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 23 Aug 2022 03:38:42 GMT
ENV MYSQL_VERSION=8.0.30-1debian11
# Tue, 23 Aug 2022 03:38:43 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ bullseye mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Tue, 23 Aug 2022 03:38:56 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 23 Aug 2022 03:38:57 GMT
VOLUME [/var/lib/mysql]
# Tue, 23 Aug 2022 03:38:57 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Wed, 24 Aug 2022 00:36:52 GMT
COPY file:0362167b353388be7fb99432d9373f030ddd789bd27d57e183555c672530b303 in /usr/local/bin/ 
# Wed, 24 Aug 2022 00:36:53 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 24 Aug 2022 00:36:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 24 Aug 2022 00:36:53 GMT
EXPOSE 3306 33060
# Wed, 24 Aug 2022 00:36:53 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:7a6db449b51b92eac5c81cdbd82917785343f1664b2be57b22337b0a40c5b29d`  
		Last Modified: Tue, 23 Aug 2022 00:24:59 GMT  
		Size: 31.4 MB (31381485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63b23008bc872644b3493308929a67cefe09bcc825a15028af9b65d2b86b8154`  
		Last Modified: Tue, 23 Aug 2022 03:40:21 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82fdf48499dbc8cadd345c9a461bee300ec7f328fd970ea456ad13582f974b22`  
		Last Modified: Tue, 23 Aug 2022 03:40:22 GMT  
		Size: 4.4 MB (4414801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c75d7f84228a2f19e49b9a70c960e1b9fe6eceb637a24727ed6ec6c574b584d`  
		Last Modified: Tue, 23 Aug 2022 03:40:19 GMT  
		Size: 1.4 MB (1418466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61089f488e727e34e9b1c515a769ea0f63e4178b9f1f8a4b697f8345cd6a2fab`  
		Last Modified: Tue, 23 Aug 2022 03:40:19 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c82b0badc95c597bc8fa0c39ee975457037cb54ecafb310b75368ebaf1ea1c8`  
		Last Modified: Tue, 23 Aug 2022 03:40:21 GMT  
		Size: 12.7 MB (12661891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:245253769f71d25434c6c23a35770f5a993727fa9396802f45d5c41bf69ef18f`  
		Last Modified: Tue, 23 Aug 2022 03:40:19 GMT  
		Size: 2.5 KB (2549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7459b3c285350cb2e864e202e4a6ce674fe99d2338698d8aba402dca9be2a3f`  
		Last Modified: Tue, 23 Aug 2022 03:40:16 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e669258b3f94cee1da8b0e384ee0e8461fcaadff509b2929f9c2b45e684d674`  
		Last Modified: Tue, 23 Aug 2022 03:40:33 GMT  
		Size: 108.0 MB (107963194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7db97a7c2c85d65c31c5ecfaf632608190d8bd998f012fa7e7888fb4b9bd562`  
		Last Modified: Tue, 23 Aug 2022 03:40:16 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d96137de95c38044d259df48352ed8c80df7702fb6ee065be7cddcc1b0b3dc9`  
		Last Modified: Wed, 24 Aug 2022 00:37:52 GMT  
		Size: 5.4 KB (5367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eaa7d534011271dfaee8ae54a5c425d1e7913d687e2e33c5e4cab48dd813bc6`  
		Last Modified: Wed, 24 Aug 2022 00:37:52 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8-oracle`

```console
$ docker pull mysql@sha256:3de4d9814b28e48f225e259cc3b2c77530296afcec20bae53e1c7a4892f2a98e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:930e762c3f185d55d96a65e0d6cb2f724ffc16a87270f85283ae099d75e92ad0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.5 MB (132502250 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c989cc040bcf09e776e701e0fb567045ee77ed8667daf1a506d898717011bfe5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 04 Aug 2022 00:36:37 GMT
ADD file:0a05a213ae66f556b2b320291ac58ec9f2f67554e29338a072f1347f22864a49 in / 
# Thu, 04 Aug 2022 00:36:37 GMT
CMD ["/bin/bash"]
# Thu, 04 Aug 2022 01:24:42 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Thu, 04 Aug 2022 01:24:43 GMT
ENV GOSU_VERSION=1.14
# Thu, 04 Aug 2022 01:24:46 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 04 Aug 2022 01:25:08 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Thu, 04 Aug 2022 01:25:10 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Thu, 04 Aug 2022 01:25:10 GMT
ENV MYSQL_MAJOR=8.0
# Thu, 04 Aug 2022 01:25:10 GMT
ENV MYSQL_VERSION=8.0.30-1.el8
# Thu, 04 Aug 2022 01:25:10 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Thu, 04 Aug 2022 01:25:38 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Thu, 04 Aug 2022 01:25:39 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Thu, 04 Aug 2022 01:25:39 GMT
ENV MYSQL_SHELL_VERSION=8.0.30-1.el8
# Thu, 04 Aug 2022 01:26:10 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Thu, 04 Aug 2022 01:26:11 GMT
VOLUME [/var/lib/mysql]
# Wed, 24 Aug 2022 00:36:48 GMT
COPY file:0362167b353388be7fb99432d9373f030ddd789bd27d57e183555c672530b303 in /usr/local/bin/ 
# Wed, 24 Aug 2022 00:36:48 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 24 Aug 2022 00:36:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 24 Aug 2022 00:36:49 GMT
EXPOSE 3306 33060
# Wed, 24 Aug 2022 00:36:49 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:32c1bf40aba1f372a057d3280b0b7cdacde9d8500a069004e6f243bc09cde806`  
		Last Modified: Thu, 04 Aug 2022 00:37:33 GMT  
		Size: 39.2 MB (39223952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ac22f3a638d1c75f850c6c7b189d746c1ec6c58ec618f9e4b928f045df1b79d`  
		Last Modified: Thu, 04 Aug 2022 01:26:53 GMT  
		Size: 890.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1e7273ed05ed3b0f6be1e9a202f93199d88428c9dff52d1edce8d965ad50f8e`  
		Last Modified: Thu, 04 Aug 2022 01:26:54 GMT  
		Size: 928.8 KB (928835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20be45a0c6abbfaf62bd02c40f3cff6bf4822711b339ebcd4e1b7d6b2764ca20`  
		Last Modified: Thu, 04 Aug 2022 01:26:52 GMT  
		Size: 4.6 MB (4581809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:410a229693ff98f0a019a180a655ad903a882367b72f78f0ac3c595c1434a65e`  
		Last Modified: Thu, 04 Aug 2022 01:26:51 GMT  
		Size: 2.6 KB (2628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ce71e3a9b8879afc4dce1dc74841ecbae7da28798b238c88f0322b7bdc82472`  
		Last Modified: Thu, 04 Aug 2022 01:26:51 GMT  
		Size: 335.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c93c823af05bbde448c0a889b94ef2d6279b9c595c9b1a1abcbd49f795f7631c`  
		Last Modified: Thu, 04 Aug 2022 01:26:56 GMT  
		Size: 47.7 MB (47726773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6752c4d09c7204097f7ecbf50885874b620e77263452bb581ed1f4d9681344d`  
		Last Modified: Thu, 04 Aug 2022 01:26:49 GMT  
		Size: 315.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7f2cfe3efcbd4b98bf44100e9f3fc095ca4a480fd75a0028bae61aedfb6298a`  
		Last Modified: Thu, 04 Aug 2022 01:26:57 GMT  
		Size: 40.0 MB (40031217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09e782dbb2c3f52fb09d97fee4689b382e3789e244c209fe81782420a19d1a2a`  
		Last Modified: Wed, 24 Aug 2022 00:37:25 GMT  
		Size: 5.4 KB (5375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01199f522543dd7f72aa6b05d1be8d67dc48483700d79db260348af7e69f2aaa`  
		Last Modified: Wed, 24 Aug 2022 00:37:24 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8-oracle` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:54b1f5e74608236fe20d5dcdf39124a81244dd4d043b0798929614c1bc1ec602
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.2 MB (141193701 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1b9c6058e7a1b8f805b067ba9d4775d392fcfda1cdd601396716864c8f59e14`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 04 Aug 2022 00:40:43 GMT
ADD file:a68d82fa032efe6adc2926f7e745508f0541bba3f906e2702d34252353100747 in / 
# Thu, 04 Aug 2022 00:40:44 GMT
CMD ["/bin/bash"]
# Thu, 04 Aug 2022 00:57:16 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Thu, 04 Aug 2022 00:57:17 GMT
ENV GOSU_VERSION=1.14
# Thu, 04 Aug 2022 00:57:21 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 04 Aug 2022 00:57:44 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Thu, 04 Aug 2022 00:57:46 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Thu, 04 Aug 2022 00:57:47 GMT
ENV MYSQL_MAJOR=8.0
# Thu, 04 Aug 2022 00:57:48 GMT
ENV MYSQL_VERSION=8.0.30-1.el8
# Thu, 04 Aug 2022 00:57:49 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Thu, 04 Aug 2022 00:58:17 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Thu, 04 Aug 2022 00:58:17 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Thu, 04 Aug 2022 00:58:18 GMT
ENV MYSQL_SHELL_VERSION=8.0.30-1.el8
# Thu, 04 Aug 2022 00:58:50 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Thu, 04 Aug 2022 00:58:51 GMT
VOLUME [/var/lib/mysql]
# Wed, 24 Aug 2022 03:30:34 GMT
COPY file:0362167b353388be7fb99432d9373f030ddd789bd27d57e183555c672530b303 in /usr/local/bin/ 
# Wed, 24 Aug 2022 03:30:35 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 24 Aug 2022 03:30:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 24 Aug 2022 03:30:37 GMT
EXPOSE 3306 33060
# Wed, 24 Aug 2022 03:30:38 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:ecf56004177eb6ca162c88de29e84bc4ba3d2e7efd3703df9ecae51b89003d52`  
		Last Modified: Thu, 04 Aug 2022 00:41:51 GMT  
		Size: 38.0 MB (38023046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1091d9f012e1e44cf00d872494ff008feb11a824aa940f5fccaadcf0f043e951`  
		Last Modified: Thu, 04 Aug 2022 00:59:35 GMT  
		Size: 888.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fabd9779d4678f8577c74505cc31bd42788a9ffa1eba563340b8ef29946b3e55`  
		Last Modified: Thu, 04 Aug 2022 00:59:36 GMT  
		Size: 857.2 KB (857152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6278448e2e194f0e2e8e7d2f29495296d594f7bd2e63d0306037e5b4f5125eb`  
		Last Modified: Thu, 04 Aug 2022 00:59:34 GMT  
		Size: 4.4 MB (4404159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6050832741b8d8e4dfba20e0d31c88f56b9b645c97752c9bbec708740c3e6e15`  
		Last Modified: Thu, 04 Aug 2022 00:59:33 GMT  
		Size: 2.6 KB (2607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0be9d1181fe5f7d6c39819a56c680e5e010a7b808b96eb00eabdeacd66ee6c1`  
		Last Modified: Thu, 04 Aug 2022 00:59:33 GMT  
		Size: 335.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbdaffd3eb50f6880d4e27c2ba2a47193ba4e1959b4647e5e794b0872e981c5b`  
		Last Modified: Thu, 04 Aug 2022 00:59:38 GMT  
		Size: 53.8 MB (53784614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a74c1ad0f09fc99fb019bcbfebb1b57f4f7fcf7e968e6ece353a06d583cab8ed`  
		Last Modified: Thu, 04 Aug 2022 00:59:31 GMT  
		Size: 315.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad2b7db10f4eacccefc72231d395d9920b81dd4bba86be2a8994b8ee9161ec92`  
		Last Modified: Thu, 04 Aug 2022 00:59:38 GMT  
		Size: 44.1 MB (44115089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f6281129c7fb0746caa0023cec4db82b482c85d81752eaafcff70498537c82a`  
		Last Modified: Wed, 24 Aug 2022 03:31:04 GMT  
		Size: 5.4 KB (5375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49dcabdef3045b25265175bee4894568254c4b35b769d77a0afedc6fd7ec9a1d`  
		Last Modified: Wed, 24 Aug 2022 03:31:04 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0`

```console
$ docker pull mysql@sha256:3de4d9814b28e48f225e259cc3b2c77530296afcec20bae53e1c7a4892f2a98e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8.0` - linux; amd64

```console
$ docker pull mysql@sha256:930e762c3f185d55d96a65e0d6cb2f724ffc16a87270f85283ae099d75e92ad0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.5 MB (132502250 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c989cc040bcf09e776e701e0fb567045ee77ed8667daf1a506d898717011bfe5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 04 Aug 2022 00:36:37 GMT
ADD file:0a05a213ae66f556b2b320291ac58ec9f2f67554e29338a072f1347f22864a49 in / 
# Thu, 04 Aug 2022 00:36:37 GMT
CMD ["/bin/bash"]
# Thu, 04 Aug 2022 01:24:42 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Thu, 04 Aug 2022 01:24:43 GMT
ENV GOSU_VERSION=1.14
# Thu, 04 Aug 2022 01:24:46 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 04 Aug 2022 01:25:08 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Thu, 04 Aug 2022 01:25:10 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Thu, 04 Aug 2022 01:25:10 GMT
ENV MYSQL_MAJOR=8.0
# Thu, 04 Aug 2022 01:25:10 GMT
ENV MYSQL_VERSION=8.0.30-1.el8
# Thu, 04 Aug 2022 01:25:10 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Thu, 04 Aug 2022 01:25:38 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Thu, 04 Aug 2022 01:25:39 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Thu, 04 Aug 2022 01:25:39 GMT
ENV MYSQL_SHELL_VERSION=8.0.30-1.el8
# Thu, 04 Aug 2022 01:26:10 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Thu, 04 Aug 2022 01:26:11 GMT
VOLUME [/var/lib/mysql]
# Wed, 24 Aug 2022 00:36:48 GMT
COPY file:0362167b353388be7fb99432d9373f030ddd789bd27d57e183555c672530b303 in /usr/local/bin/ 
# Wed, 24 Aug 2022 00:36:48 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 24 Aug 2022 00:36:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 24 Aug 2022 00:36:49 GMT
EXPOSE 3306 33060
# Wed, 24 Aug 2022 00:36:49 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:32c1bf40aba1f372a057d3280b0b7cdacde9d8500a069004e6f243bc09cde806`  
		Last Modified: Thu, 04 Aug 2022 00:37:33 GMT  
		Size: 39.2 MB (39223952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ac22f3a638d1c75f850c6c7b189d746c1ec6c58ec618f9e4b928f045df1b79d`  
		Last Modified: Thu, 04 Aug 2022 01:26:53 GMT  
		Size: 890.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1e7273ed05ed3b0f6be1e9a202f93199d88428c9dff52d1edce8d965ad50f8e`  
		Last Modified: Thu, 04 Aug 2022 01:26:54 GMT  
		Size: 928.8 KB (928835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20be45a0c6abbfaf62bd02c40f3cff6bf4822711b339ebcd4e1b7d6b2764ca20`  
		Last Modified: Thu, 04 Aug 2022 01:26:52 GMT  
		Size: 4.6 MB (4581809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:410a229693ff98f0a019a180a655ad903a882367b72f78f0ac3c595c1434a65e`  
		Last Modified: Thu, 04 Aug 2022 01:26:51 GMT  
		Size: 2.6 KB (2628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ce71e3a9b8879afc4dce1dc74841ecbae7da28798b238c88f0322b7bdc82472`  
		Last Modified: Thu, 04 Aug 2022 01:26:51 GMT  
		Size: 335.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c93c823af05bbde448c0a889b94ef2d6279b9c595c9b1a1abcbd49f795f7631c`  
		Last Modified: Thu, 04 Aug 2022 01:26:56 GMT  
		Size: 47.7 MB (47726773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6752c4d09c7204097f7ecbf50885874b620e77263452bb581ed1f4d9681344d`  
		Last Modified: Thu, 04 Aug 2022 01:26:49 GMT  
		Size: 315.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7f2cfe3efcbd4b98bf44100e9f3fc095ca4a480fd75a0028bae61aedfb6298a`  
		Last Modified: Thu, 04 Aug 2022 01:26:57 GMT  
		Size: 40.0 MB (40031217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09e782dbb2c3f52fb09d97fee4689b382e3789e244c209fe81782420a19d1a2a`  
		Last Modified: Wed, 24 Aug 2022 00:37:25 GMT  
		Size: 5.4 KB (5375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01199f522543dd7f72aa6b05d1be8d67dc48483700d79db260348af7e69f2aaa`  
		Last Modified: Wed, 24 Aug 2022 00:37:24 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8.0` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:54b1f5e74608236fe20d5dcdf39124a81244dd4d043b0798929614c1bc1ec602
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.2 MB (141193701 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1b9c6058e7a1b8f805b067ba9d4775d392fcfda1cdd601396716864c8f59e14`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 04 Aug 2022 00:40:43 GMT
ADD file:a68d82fa032efe6adc2926f7e745508f0541bba3f906e2702d34252353100747 in / 
# Thu, 04 Aug 2022 00:40:44 GMT
CMD ["/bin/bash"]
# Thu, 04 Aug 2022 00:57:16 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Thu, 04 Aug 2022 00:57:17 GMT
ENV GOSU_VERSION=1.14
# Thu, 04 Aug 2022 00:57:21 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 04 Aug 2022 00:57:44 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Thu, 04 Aug 2022 00:57:46 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Thu, 04 Aug 2022 00:57:47 GMT
ENV MYSQL_MAJOR=8.0
# Thu, 04 Aug 2022 00:57:48 GMT
ENV MYSQL_VERSION=8.0.30-1.el8
# Thu, 04 Aug 2022 00:57:49 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Thu, 04 Aug 2022 00:58:17 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Thu, 04 Aug 2022 00:58:17 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Thu, 04 Aug 2022 00:58:18 GMT
ENV MYSQL_SHELL_VERSION=8.0.30-1.el8
# Thu, 04 Aug 2022 00:58:50 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Thu, 04 Aug 2022 00:58:51 GMT
VOLUME [/var/lib/mysql]
# Wed, 24 Aug 2022 03:30:34 GMT
COPY file:0362167b353388be7fb99432d9373f030ddd789bd27d57e183555c672530b303 in /usr/local/bin/ 
# Wed, 24 Aug 2022 03:30:35 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 24 Aug 2022 03:30:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 24 Aug 2022 03:30:37 GMT
EXPOSE 3306 33060
# Wed, 24 Aug 2022 03:30:38 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:ecf56004177eb6ca162c88de29e84bc4ba3d2e7efd3703df9ecae51b89003d52`  
		Last Modified: Thu, 04 Aug 2022 00:41:51 GMT  
		Size: 38.0 MB (38023046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1091d9f012e1e44cf00d872494ff008feb11a824aa940f5fccaadcf0f043e951`  
		Last Modified: Thu, 04 Aug 2022 00:59:35 GMT  
		Size: 888.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fabd9779d4678f8577c74505cc31bd42788a9ffa1eba563340b8ef29946b3e55`  
		Last Modified: Thu, 04 Aug 2022 00:59:36 GMT  
		Size: 857.2 KB (857152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6278448e2e194f0e2e8e7d2f29495296d594f7bd2e63d0306037e5b4f5125eb`  
		Last Modified: Thu, 04 Aug 2022 00:59:34 GMT  
		Size: 4.4 MB (4404159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6050832741b8d8e4dfba20e0d31c88f56b9b645c97752c9bbec708740c3e6e15`  
		Last Modified: Thu, 04 Aug 2022 00:59:33 GMT  
		Size: 2.6 KB (2607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0be9d1181fe5f7d6c39819a56c680e5e010a7b808b96eb00eabdeacd66ee6c1`  
		Last Modified: Thu, 04 Aug 2022 00:59:33 GMT  
		Size: 335.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbdaffd3eb50f6880d4e27c2ba2a47193ba4e1959b4647e5e794b0872e981c5b`  
		Last Modified: Thu, 04 Aug 2022 00:59:38 GMT  
		Size: 53.8 MB (53784614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a74c1ad0f09fc99fb019bcbfebb1b57f4f7fcf7e968e6ece353a06d583cab8ed`  
		Last Modified: Thu, 04 Aug 2022 00:59:31 GMT  
		Size: 315.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad2b7db10f4eacccefc72231d395d9920b81dd4bba86be2a8994b8ee9161ec92`  
		Last Modified: Thu, 04 Aug 2022 00:59:38 GMT  
		Size: 44.1 MB (44115089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f6281129c7fb0746caa0023cec4db82b482c85d81752eaafcff70498537c82a`  
		Last Modified: Wed, 24 Aug 2022 03:31:04 GMT  
		Size: 5.4 KB (5375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49dcabdef3045b25265175bee4894568254c4b35b769d77a0afedc6fd7ec9a1d`  
		Last Modified: Wed, 24 Aug 2022 03:31:04 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0-debian`

```console
$ docker pull mysql@sha256:1b9a6291084f62abdcba3d057e6932e5419910c469f506f627eb31756e1b4666
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:8.0-debian` - linux; amd64

```console
$ docker pull mysql@sha256:ae245d06921e615701b017b2f6ac7aedaaf4cdf351bf57302cab7bc732ef3766
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **157.9 MB (157850853 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:960207ea9ac0c08b0485963dd531c0fcb4409c980661579f474af0119032a90a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 23 Aug 2022 00:20:50 GMT
ADD file:7726efb0e0eb5003dbcf2967ec29364479eec8b41f2569ff189372153115b54b in / 
# Tue, 23 Aug 2022 00:20:51 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 03:38:21 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 23 Aug 2022 03:38:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 03:38:26 GMT
ENV GOSU_VERSION=1.14
# Tue, 23 Aug 2022 03:38:35 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 23 Aug 2022 03:38:36 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 23 Aug 2022 03:38:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 03:38:42 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Tue, 23 Aug 2022 03:38:42 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 23 Aug 2022 03:38:42 GMT
ENV MYSQL_VERSION=8.0.30-1debian11
# Tue, 23 Aug 2022 03:38:43 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ bullseye mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Tue, 23 Aug 2022 03:38:56 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 23 Aug 2022 03:38:57 GMT
VOLUME [/var/lib/mysql]
# Tue, 23 Aug 2022 03:38:57 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Wed, 24 Aug 2022 00:36:52 GMT
COPY file:0362167b353388be7fb99432d9373f030ddd789bd27d57e183555c672530b303 in /usr/local/bin/ 
# Wed, 24 Aug 2022 00:36:53 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 24 Aug 2022 00:36:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 24 Aug 2022 00:36:53 GMT
EXPOSE 3306 33060
# Wed, 24 Aug 2022 00:36:53 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:7a6db449b51b92eac5c81cdbd82917785343f1664b2be57b22337b0a40c5b29d`  
		Last Modified: Tue, 23 Aug 2022 00:24:59 GMT  
		Size: 31.4 MB (31381485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63b23008bc872644b3493308929a67cefe09bcc825a15028af9b65d2b86b8154`  
		Last Modified: Tue, 23 Aug 2022 03:40:21 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82fdf48499dbc8cadd345c9a461bee300ec7f328fd970ea456ad13582f974b22`  
		Last Modified: Tue, 23 Aug 2022 03:40:22 GMT  
		Size: 4.4 MB (4414801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c75d7f84228a2f19e49b9a70c960e1b9fe6eceb637a24727ed6ec6c574b584d`  
		Last Modified: Tue, 23 Aug 2022 03:40:19 GMT  
		Size: 1.4 MB (1418466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61089f488e727e34e9b1c515a769ea0f63e4178b9f1f8a4b697f8345cd6a2fab`  
		Last Modified: Tue, 23 Aug 2022 03:40:19 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c82b0badc95c597bc8fa0c39ee975457037cb54ecafb310b75368ebaf1ea1c8`  
		Last Modified: Tue, 23 Aug 2022 03:40:21 GMT  
		Size: 12.7 MB (12661891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:245253769f71d25434c6c23a35770f5a993727fa9396802f45d5c41bf69ef18f`  
		Last Modified: Tue, 23 Aug 2022 03:40:19 GMT  
		Size: 2.5 KB (2549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7459b3c285350cb2e864e202e4a6ce674fe99d2338698d8aba402dca9be2a3f`  
		Last Modified: Tue, 23 Aug 2022 03:40:16 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e669258b3f94cee1da8b0e384ee0e8461fcaadff509b2929f9c2b45e684d674`  
		Last Modified: Tue, 23 Aug 2022 03:40:33 GMT  
		Size: 108.0 MB (107963194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7db97a7c2c85d65c31c5ecfaf632608190d8bd998f012fa7e7888fb4b9bd562`  
		Last Modified: Tue, 23 Aug 2022 03:40:16 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d96137de95c38044d259df48352ed8c80df7702fb6ee065be7cddcc1b0b3dc9`  
		Last Modified: Wed, 24 Aug 2022 00:37:52 GMT  
		Size: 5.4 KB (5367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eaa7d534011271dfaee8ae54a5c425d1e7913d687e2e33c5e4cab48dd813bc6`  
		Last Modified: Wed, 24 Aug 2022 00:37:52 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0-oracle`

```console
$ docker pull mysql@sha256:3de4d9814b28e48f225e259cc3b2c77530296afcec20bae53e1c7a4892f2a98e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8.0-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:930e762c3f185d55d96a65e0d6cb2f724ffc16a87270f85283ae099d75e92ad0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.5 MB (132502250 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c989cc040bcf09e776e701e0fb567045ee77ed8667daf1a506d898717011bfe5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 04 Aug 2022 00:36:37 GMT
ADD file:0a05a213ae66f556b2b320291ac58ec9f2f67554e29338a072f1347f22864a49 in / 
# Thu, 04 Aug 2022 00:36:37 GMT
CMD ["/bin/bash"]
# Thu, 04 Aug 2022 01:24:42 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Thu, 04 Aug 2022 01:24:43 GMT
ENV GOSU_VERSION=1.14
# Thu, 04 Aug 2022 01:24:46 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 04 Aug 2022 01:25:08 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Thu, 04 Aug 2022 01:25:10 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Thu, 04 Aug 2022 01:25:10 GMT
ENV MYSQL_MAJOR=8.0
# Thu, 04 Aug 2022 01:25:10 GMT
ENV MYSQL_VERSION=8.0.30-1.el8
# Thu, 04 Aug 2022 01:25:10 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Thu, 04 Aug 2022 01:25:38 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Thu, 04 Aug 2022 01:25:39 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Thu, 04 Aug 2022 01:25:39 GMT
ENV MYSQL_SHELL_VERSION=8.0.30-1.el8
# Thu, 04 Aug 2022 01:26:10 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Thu, 04 Aug 2022 01:26:11 GMT
VOLUME [/var/lib/mysql]
# Wed, 24 Aug 2022 00:36:48 GMT
COPY file:0362167b353388be7fb99432d9373f030ddd789bd27d57e183555c672530b303 in /usr/local/bin/ 
# Wed, 24 Aug 2022 00:36:48 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 24 Aug 2022 00:36:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 24 Aug 2022 00:36:49 GMT
EXPOSE 3306 33060
# Wed, 24 Aug 2022 00:36:49 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:32c1bf40aba1f372a057d3280b0b7cdacde9d8500a069004e6f243bc09cde806`  
		Last Modified: Thu, 04 Aug 2022 00:37:33 GMT  
		Size: 39.2 MB (39223952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ac22f3a638d1c75f850c6c7b189d746c1ec6c58ec618f9e4b928f045df1b79d`  
		Last Modified: Thu, 04 Aug 2022 01:26:53 GMT  
		Size: 890.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1e7273ed05ed3b0f6be1e9a202f93199d88428c9dff52d1edce8d965ad50f8e`  
		Last Modified: Thu, 04 Aug 2022 01:26:54 GMT  
		Size: 928.8 KB (928835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20be45a0c6abbfaf62bd02c40f3cff6bf4822711b339ebcd4e1b7d6b2764ca20`  
		Last Modified: Thu, 04 Aug 2022 01:26:52 GMT  
		Size: 4.6 MB (4581809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:410a229693ff98f0a019a180a655ad903a882367b72f78f0ac3c595c1434a65e`  
		Last Modified: Thu, 04 Aug 2022 01:26:51 GMT  
		Size: 2.6 KB (2628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ce71e3a9b8879afc4dce1dc74841ecbae7da28798b238c88f0322b7bdc82472`  
		Last Modified: Thu, 04 Aug 2022 01:26:51 GMT  
		Size: 335.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c93c823af05bbde448c0a889b94ef2d6279b9c595c9b1a1abcbd49f795f7631c`  
		Last Modified: Thu, 04 Aug 2022 01:26:56 GMT  
		Size: 47.7 MB (47726773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6752c4d09c7204097f7ecbf50885874b620e77263452bb581ed1f4d9681344d`  
		Last Modified: Thu, 04 Aug 2022 01:26:49 GMT  
		Size: 315.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7f2cfe3efcbd4b98bf44100e9f3fc095ca4a480fd75a0028bae61aedfb6298a`  
		Last Modified: Thu, 04 Aug 2022 01:26:57 GMT  
		Size: 40.0 MB (40031217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09e782dbb2c3f52fb09d97fee4689b382e3789e244c209fe81782420a19d1a2a`  
		Last Modified: Wed, 24 Aug 2022 00:37:25 GMT  
		Size: 5.4 KB (5375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01199f522543dd7f72aa6b05d1be8d67dc48483700d79db260348af7e69f2aaa`  
		Last Modified: Wed, 24 Aug 2022 00:37:24 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8.0-oracle` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:54b1f5e74608236fe20d5dcdf39124a81244dd4d043b0798929614c1bc1ec602
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.2 MB (141193701 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1b9c6058e7a1b8f805b067ba9d4775d392fcfda1cdd601396716864c8f59e14`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 04 Aug 2022 00:40:43 GMT
ADD file:a68d82fa032efe6adc2926f7e745508f0541bba3f906e2702d34252353100747 in / 
# Thu, 04 Aug 2022 00:40:44 GMT
CMD ["/bin/bash"]
# Thu, 04 Aug 2022 00:57:16 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Thu, 04 Aug 2022 00:57:17 GMT
ENV GOSU_VERSION=1.14
# Thu, 04 Aug 2022 00:57:21 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 04 Aug 2022 00:57:44 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Thu, 04 Aug 2022 00:57:46 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Thu, 04 Aug 2022 00:57:47 GMT
ENV MYSQL_MAJOR=8.0
# Thu, 04 Aug 2022 00:57:48 GMT
ENV MYSQL_VERSION=8.0.30-1.el8
# Thu, 04 Aug 2022 00:57:49 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Thu, 04 Aug 2022 00:58:17 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Thu, 04 Aug 2022 00:58:17 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Thu, 04 Aug 2022 00:58:18 GMT
ENV MYSQL_SHELL_VERSION=8.0.30-1.el8
# Thu, 04 Aug 2022 00:58:50 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Thu, 04 Aug 2022 00:58:51 GMT
VOLUME [/var/lib/mysql]
# Wed, 24 Aug 2022 03:30:34 GMT
COPY file:0362167b353388be7fb99432d9373f030ddd789bd27d57e183555c672530b303 in /usr/local/bin/ 
# Wed, 24 Aug 2022 03:30:35 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 24 Aug 2022 03:30:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 24 Aug 2022 03:30:37 GMT
EXPOSE 3306 33060
# Wed, 24 Aug 2022 03:30:38 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:ecf56004177eb6ca162c88de29e84bc4ba3d2e7efd3703df9ecae51b89003d52`  
		Last Modified: Thu, 04 Aug 2022 00:41:51 GMT  
		Size: 38.0 MB (38023046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1091d9f012e1e44cf00d872494ff008feb11a824aa940f5fccaadcf0f043e951`  
		Last Modified: Thu, 04 Aug 2022 00:59:35 GMT  
		Size: 888.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fabd9779d4678f8577c74505cc31bd42788a9ffa1eba563340b8ef29946b3e55`  
		Last Modified: Thu, 04 Aug 2022 00:59:36 GMT  
		Size: 857.2 KB (857152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6278448e2e194f0e2e8e7d2f29495296d594f7bd2e63d0306037e5b4f5125eb`  
		Last Modified: Thu, 04 Aug 2022 00:59:34 GMT  
		Size: 4.4 MB (4404159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6050832741b8d8e4dfba20e0d31c88f56b9b645c97752c9bbec708740c3e6e15`  
		Last Modified: Thu, 04 Aug 2022 00:59:33 GMT  
		Size: 2.6 KB (2607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0be9d1181fe5f7d6c39819a56c680e5e010a7b808b96eb00eabdeacd66ee6c1`  
		Last Modified: Thu, 04 Aug 2022 00:59:33 GMT  
		Size: 335.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbdaffd3eb50f6880d4e27c2ba2a47193ba4e1959b4647e5e794b0872e981c5b`  
		Last Modified: Thu, 04 Aug 2022 00:59:38 GMT  
		Size: 53.8 MB (53784614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a74c1ad0f09fc99fb019bcbfebb1b57f4f7fcf7e968e6ece353a06d583cab8ed`  
		Last Modified: Thu, 04 Aug 2022 00:59:31 GMT  
		Size: 315.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad2b7db10f4eacccefc72231d395d9920b81dd4bba86be2a8994b8ee9161ec92`  
		Last Modified: Thu, 04 Aug 2022 00:59:38 GMT  
		Size: 44.1 MB (44115089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f6281129c7fb0746caa0023cec4db82b482c85d81752eaafcff70498537c82a`  
		Last Modified: Wed, 24 Aug 2022 03:31:04 GMT  
		Size: 5.4 KB (5375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49dcabdef3045b25265175bee4894568254c4b35b769d77a0afedc6fd7ec9a1d`  
		Last Modified: Wed, 24 Aug 2022 03:31:04 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0.30`

```console
$ docker pull mysql@sha256:3de4d9814b28e48f225e259cc3b2c77530296afcec20bae53e1c7a4892f2a98e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8.0.30` - linux; amd64

```console
$ docker pull mysql@sha256:930e762c3f185d55d96a65e0d6cb2f724ffc16a87270f85283ae099d75e92ad0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.5 MB (132502250 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c989cc040bcf09e776e701e0fb567045ee77ed8667daf1a506d898717011bfe5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 04 Aug 2022 00:36:37 GMT
ADD file:0a05a213ae66f556b2b320291ac58ec9f2f67554e29338a072f1347f22864a49 in / 
# Thu, 04 Aug 2022 00:36:37 GMT
CMD ["/bin/bash"]
# Thu, 04 Aug 2022 01:24:42 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Thu, 04 Aug 2022 01:24:43 GMT
ENV GOSU_VERSION=1.14
# Thu, 04 Aug 2022 01:24:46 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 04 Aug 2022 01:25:08 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Thu, 04 Aug 2022 01:25:10 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Thu, 04 Aug 2022 01:25:10 GMT
ENV MYSQL_MAJOR=8.0
# Thu, 04 Aug 2022 01:25:10 GMT
ENV MYSQL_VERSION=8.0.30-1.el8
# Thu, 04 Aug 2022 01:25:10 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Thu, 04 Aug 2022 01:25:38 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Thu, 04 Aug 2022 01:25:39 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Thu, 04 Aug 2022 01:25:39 GMT
ENV MYSQL_SHELL_VERSION=8.0.30-1.el8
# Thu, 04 Aug 2022 01:26:10 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Thu, 04 Aug 2022 01:26:11 GMT
VOLUME [/var/lib/mysql]
# Wed, 24 Aug 2022 00:36:48 GMT
COPY file:0362167b353388be7fb99432d9373f030ddd789bd27d57e183555c672530b303 in /usr/local/bin/ 
# Wed, 24 Aug 2022 00:36:48 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 24 Aug 2022 00:36:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 24 Aug 2022 00:36:49 GMT
EXPOSE 3306 33060
# Wed, 24 Aug 2022 00:36:49 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:32c1bf40aba1f372a057d3280b0b7cdacde9d8500a069004e6f243bc09cde806`  
		Last Modified: Thu, 04 Aug 2022 00:37:33 GMT  
		Size: 39.2 MB (39223952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ac22f3a638d1c75f850c6c7b189d746c1ec6c58ec618f9e4b928f045df1b79d`  
		Last Modified: Thu, 04 Aug 2022 01:26:53 GMT  
		Size: 890.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1e7273ed05ed3b0f6be1e9a202f93199d88428c9dff52d1edce8d965ad50f8e`  
		Last Modified: Thu, 04 Aug 2022 01:26:54 GMT  
		Size: 928.8 KB (928835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20be45a0c6abbfaf62bd02c40f3cff6bf4822711b339ebcd4e1b7d6b2764ca20`  
		Last Modified: Thu, 04 Aug 2022 01:26:52 GMT  
		Size: 4.6 MB (4581809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:410a229693ff98f0a019a180a655ad903a882367b72f78f0ac3c595c1434a65e`  
		Last Modified: Thu, 04 Aug 2022 01:26:51 GMT  
		Size: 2.6 KB (2628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ce71e3a9b8879afc4dce1dc74841ecbae7da28798b238c88f0322b7bdc82472`  
		Last Modified: Thu, 04 Aug 2022 01:26:51 GMT  
		Size: 335.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c93c823af05bbde448c0a889b94ef2d6279b9c595c9b1a1abcbd49f795f7631c`  
		Last Modified: Thu, 04 Aug 2022 01:26:56 GMT  
		Size: 47.7 MB (47726773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6752c4d09c7204097f7ecbf50885874b620e77263452bb581ed1f4d9681344d`  
		Last Modified: Thu, 04 Aug 2022 01:26:49 GMT  
		Size: 315.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7f2cfe3efcbd4b98bf44100e9f3fc095ca4a480fd75a0028bae61aedfb6298a`  
		Last Modified: Thu, 04 Aug 2022 01:26:57 GMT  
		Size: 40.0 MB (40031217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09e782dbb2c3f52fb09d97fee4689b382e3789e244c209fe81782420a19d1a2a`  
		Last Modified: Wed, 24 Aug 2022 00:37:25 GMT  
		Size: 5.4 KB (5375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01199f522543dd7f72aa6b05d1be8d67dc48483700d79db260348af7e69f2aaa`  
		Last Modified: Wed, 24 Aug 2022 00:37:24 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8.0.30` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:54b1f5e74608236fe20d5dcdf39124a81244dd4d043b0798929614c1bc1ec602
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.2 MB (141193701 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1b9c6058e7a1b8f805b067ba9d4775d392fcfda1cdd601396716864c8f59e14`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 04 Aug 2022 00:40:43 GMT
ADD file:a68d82fa032efe6adc2926f7e745508f0541bba3f906e2702d34252353100747 in / 
# Thu, 04 Aug 2022 00:40:44 GMT
CMD ["/bin/bash"]
# Thu, 04 Aug 2022 00:57:16 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Thu, 04 Aug 2022 00:57:17 GMT
ENV GOSU_VERSION=1.14
# Thu, 04 Aug 2022 00:57:21 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 04 Aug 2022 00:57:44 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Thu, 04 Aug 2022 00:57:46 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Thu, 04 Aug 2022 00:57:47 GMT
ENV MYSQL_MAJOR=8.0
# Thu, 04 Aug 2022 00:57:48 GMT
ENV MYSQL_VERSION=8.0.30-1.el8
# Thu, 04 Aug 2022 00:57:49 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Thu, 04 Aug 2022 00:58:17 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Thu, 04 Aug 2022 00:58:17 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Thu, 04 Aug 2022 00:58:18 GMT
ENV MYSQL_SHELL_VERSION=8.0.30-1.el8
# Thu, 04 Aug 2022 00:58:50 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Thu, 04 Aug 2022 00:58:51 GMT
VOLUME [/var/lib/mysql]
# Wed, 24 Aug 2022 03:30:34 GMT
COPY file:0362167b353388be7fb99432d9373f030ddd789bd27d57e183555c672530b303 in /usr/local/bin/ 
# Wed, 24 Aug 2022 03:30:35 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 24 Aug 2022 03:30:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 24 Aug 2022 03:30:37 GMT
EXPOSE 3306 33060
# Wed, 24 Aug 2022 03:30:38 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:ecf56004177eb6ca162c88de29e84bc4ba3d2e7efd3703df9ecae51b89003d52`  
		Last Modified: Thu, 04 Aug 2022 00:41:51 GMT  
		Size: 38.0 MB (38023046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1091d9f012e1e44cf00d872494ff008feb11a824aa940f5fccaadcf0f043e951`  
		Last Modified: Thu, 04 Aug 2022 00:59:35 GMT  
		Size: 888.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fabd9779d4678f8577c74505cc31bd42788a9ffa1eba563340b8ef29946b3e55`  
		Last Modified: Thu, 04 Aug 2022 00:59:36 GMT  
		Size: 857.2 KB (857152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6278448e2e194f0e2e8e7d2f29495296d594f7bd2e63d0306037e5b4f5125eb`  
		Last Modified: Thu, 04 Aug 2022 00:59:34 GMT  
		Size: 4.4 MB (4404159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6050832741b8d8e4dfba20e0d31c88f56b9b645c97752c9bbec708740c3e6e15`  
		Last Modified: Thu, 04 Aug 2022 00:59:33 GMT  
		Size: 2.6 KB (2607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0be9d1181fe5f7d6c39819a56c680e5e010a7b808b96eb00eabdeacd66ee6c1`  
		Last Modified: Thu, 04 Aug 2022 00:59:33 GMT  
		Size: 335.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbdaffd3eb50f6880d4e27c2ba2a47193ba4e1959b4647e5e794b0872e981c5b`  
		Last Modified: Thu, 04 Aug 2022 00:59:38 GMT  
		Size: 53.8 MB (53784614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a74c1ad0f09fc99fb019bcbfebb1b57f4f7fcf7e968e6ece353a06d583cab8ed`  
		Last Modified: Thu, 04 Aug 2022 00:59:31 GMT  
		Size: 315.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad2b7db10f4eacccefc72231d395d9920b81dd4bba86be2a8994b8ee9161ec92`  
		Last Modified: Thu, 04 Aug 2022 00:59:38 GMT  
		Size: 44.1 MB (44115089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f6281129c7fb0746caa0023cec4db82b482c85d81752eaafcff70498537c82a`  
		Last Modified: Wed, 24 Aug 2022 03:31:04 GMT  
		Size: 5.4 KB (5375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49dcabdef3045b25265175bee4894568254c4b35b769d77a0afedc6fd7ec9a1d`  
		Last Modified: Wed, 24 Aug 2022 03:31:04 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0.30-debian`

```console
$ docker pull mysql@sha256:1b9a6291084f62abdcba3d057e6932e5419910c469f506f627eb31756e1b4666
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:8.0.30-debian` - linux; amd64

```console
$ docker pull mysql@sha256:ae245d06921e615701b017b2f6ac7aedaaf4cdf351bf57302cab7bc732ef3766
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **157.9 MB (157850853 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:960207ea9ac0c08b0485963dd531c0fcb4409c980661579f474af0119032a90a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 23 Aug 2022 00:20:50 GMT
ADD file:7726efb0e0eb5003dbcf2967ec29364479eec8b41f2569ff189372153115b54b in / 
# Tue, 23 Aug 2022 00:20:51 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 03:38:21 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 23 Aug 2022 03:38:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 03:38:26 GMT
ENV GOSU_VERSION=1.14
# Tue, 23 Aug 2022 03:38:35 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 23 Aug 2022 03:38:36 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 23 Aug 2022 03:38:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 03:38:42 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Tue, 23 Aug 2022 03:38:42 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 23 Aug 2022 03:38:42 GMT
ENV MYSQL_VERSION=8.0.30-1debian11
# Tue, 23 Aug 2022 03:38:43 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ bullseye mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Tue, 23 Aug 2022 03:38:56 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 23 Aug 2022 03:38:57 GMT
VOLUME [/var/lib/mysql]
# Tue, 23 Aug 2022 03:38:57 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Wed, 24 Aug 2022 00:36:52 GMT
COPY file:0362167b353388be7fb99432d9373f030ddd789bd27d57e183555c672530b303 in /usr/local/bin/ 
# Wed, 24 Aug 2022 00:36:53 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 24 Aug 2022 00:36:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 24 Aug 2022 00:36:53 GMT
EXPOSE 3306 33060
# Wed, 24 Aug 2022 00:36:53 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:7a6db449b51b92eac5c81cdbd82917785343f1664b2be57b22337b0a40c5b29d`  
		Last Modified: Tue, 23 Aug 2022 00:24:59 GMT  
		Size: 31.4 MB (31381485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63b23008bc872644b3493308929a67cefe09bcc825a15028af9b65d2b86b8154`  
		Last Modified: Tue, 23 Aug 2022 03:40:21 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82fdf48499dbc8cadd345c9a461bee300ec7f328fd970ea456ad13582f974b22`  
		Last Modified: Tue, 23 Aug 2022 03:40:22 GMT  
		Size: 4.4 MB (4414801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c75d7f84228a2f19e49b9a70c960e1b9fe6eceb637a24727ed6ec6c574b584d`  
		Last Modified: Tue, 23 Aug 2022 03:40:19 GMT  
		Size: 1.4 MB (1418466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61089f488e727e34e9b1c515a769ea0f63e4178b9f1f8a4b697f8345cd6a2fab`  
		Last Modified: Tue, 23 Aug 2022 03:40:19 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c82b0badc95c597bc8fa0c39ee975457037cb54ecafb310b75368ebaf1ea1c8`  
		Last Modified: Tue, 23 Aug 2022 03:40:21 GMT  
		Size: 12.7 MB (12661891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:245253769f71d25434c6c23a35770f5a993727fa9396802f45d5c41bf69ef18f`  
		Last Modified: Tue, 23 Aug 2022 03:40:19 GMT  
		Size: 2.5 KB (2549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7459b3c285350cb2e864e202e4a6ce674fe99d2338698d8aba402dca9be2a3f`  
		Last Modified: Tue, 23 Aug 2022 03:40:16 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e669258b3f94cee1da8b0e384ee0e8461fcaadff509b2929f9c2b45e684d674`  
		Last Modified: Tue, 23 Aug 2022 03:40:33 GMT  
		Size: 108.0 MB (107963194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7db97a7c2c85d65c31c5ecfaf632608190d8bd998f012fa7e7888fb4b9bd562`  
		Last Modified: Tue, 23 Aug 2022 03:40:16 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d96137de95c38044d259df48352ed8c80df7702fb6ee065be7cddcc1b0b3dc9`  
		Last Modified: Wed, 24 Aug 2022 00:37:52 GMT  
		Size: 5.4 KB (5367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eaa7d534011271dfaee8ae54a5c425d1e7913d687e2e33c5e4cab48dd813bc6`  
		Last Modified: Wed, 24 Aug 2022 00:37:52 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0.30-oracle`

```console
$ docker pull mysql@sha256:3de4d9814b28e48f225e259cc3b2c77530296afcec20bae53e1c7a4892f2a98e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8.0.30-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:930e762c3f185d55d96a65e0d6cb2f724ffc16a87270f85283ae099d75e92ad0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.5 MB (132502250 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c989cc040bcf09e776e701e0fb567045ee77ed8667daf1a506d898717011bfe5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 04 Aug 2022 00:36:37 GMT
ADD file:0a05a213ae66f556b2b320291ac58ec9f2f67554e29338a072f1347f22864a49 in / 
# Thu, 04 Aug 2022 00:36:37 GMT
CMD ["/bin/bash"]
# Thu, 04 Aug 2022 01:24:42 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Thu, 04 Aug 2022 01:24:43 GMT
ENV GOSU_VERSION=1.14
# Thu, 04 Aug 2022 01:24:46 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 04 Aug 2022 01:25:08 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Thu, 04 Aug 2022 01:25:10 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Thu, 04 Aug 2022 01:25:10 GMT
ENV MYSQL_MAJOR=8.0
# Thu, 04 Aug 2022 01:25:10 GMT
ENV MYSQL_VERSION=8.0.30-1.el8
# Thu, 04 Aug 2022 01:25:10 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Thu, 04 Aug 2022 01:25:38 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Thu, 04 Aug 2022 01:25:39 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Thu, 04 Aug 2022 01:25:39 GMT
ENV MYSQL_SHELL_VERSION=8.0.30-1.el8
# Thu, 04 Aug 2022 01:26:10 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Thu, 04 Aug 2022 01:26:11 GMT
VOLUME [/var/lib/mysql]
# Wed, 24 Aug 2022 00:36:48 GMT
COPY file:0362167b353388be7fb99432d9373f030ddd789bd27d57e183555c672530b303 in /usr/local/bin/ 
# Wed, 24 Aug 2022 00:36:48 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 24 Aug 2022 00:36:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 24 Aug 2022 00:36:49 GMT
EXPOSE 3306 33060
# Wed, 24 Aug 2022 00:36:49 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:32c1bf40aba1f372a057d3280b0b7cdacde9d8500a069004e6f243bc09cde806`  
		Last Modified: Thu, 04 Aug 2022 00:37:33 GMT  
		Size: 39.2 MB (39223952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ac22f3a638d1c75f850c6c7b189d746c1ec6c58ec618f9e4b928f045df1b79d`  
		Last Modified: Thu, 04 Aug 2022 01:26:53 GMT  
		Size: 890.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1e7273ed05ed3b0f6be1e9a202f93199d88428c9dff52d1edce8d965ad50f8e`  
		Last Modified: Thu, 04 Aug 2022 01:26:54 GMT  
		Size: 928.8 KB (928835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20be45a0c6abbfaf62bd02c40f3cff6bf4822711b339ebcd4e1b7d6b2764ca20`  
		Last Modified: Thu, 04 Aug 2022 01:26:52 GMT  
		Size: 4.6 MB (4581809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:410a229693ff98f0a019a180a655ad903a882367b72f78f0ac3c595c1434a65e`  
		Last Modified: Thu, 04 Aug 2022 01:26:51 GMT  
		Size: 2.6 KB (2628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ce71e3a9b8879afc4dce1dc74841ecbae7da28798b238c88f0322b7bdc82472`  
		Last Modified: Thu, 04 Aug 2022 01:26:51 GMT  
		Size: 335.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c93c823af05bbde448c0a889b94ef2d6279b9c595c9b1a1abcbd49f795f7631c`  
		Last Modified: Thu, 04 Aug 2022 01:26:56 GMT  
		Size: 47.7 MB (47726773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6752c4d09c7204097f7ecbf50885874b620e77263452bb581ed1f4d9681344d`  
		Last Modified: Thu, 04 Aug 2022 01:26:49 GMT  
		Size: 315.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7f2cfe3efcbd4b98bf44100e9f3fc095ca4a480fd75a0028bae61aedfb6298a`  
		Last Modified: Thu, 04 Aug 2022 01:26:57 GMT  
		Size: 40.0 MB (40031217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09e782dbb2c3f52fb09d97fee4689b382e3789e244c209fe81782420a19d1a2a`  
		Last Modified: Wed, 24 Aug 2022 00:37:25 GMT  
		Size: 5.4 KB (5375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01199f522543dd7f72aa6b05d1be8d67dc48483700d79db260348af7e69f2aaa`  
		Last Modified: Wed, 24 Aug 2022 00:37:24 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8.0.30-oracle` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:54b1f5e74608236fe20d5dcdf39124a81244dd4d043b0798929614c1bc1ec602
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.2 MB (141193701 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1b9c6058e7a1b8f805b067ba9d4775d392fcfda1cdd601396716864c8f59e14`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 04 Aug 2022 00:40:43 GMT
ADD file:a68d82fa032efe6adc2926f7e745508f0541bba3f906e2702d34252353100747 in / 
# Thu, 04 Aug 2022 00:40:44 GMT
CMD ["/bin/bash"]
# Thu, 04 Aug 2022 00:57:16 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Thu, 04 Aug 2022 00:57:17 GMT
ENV GOSU_VERSION=1.14
# Thu, 04 Aug 2022 00:57:21 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 04 Aug 2022 00:57:44 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Thu, 04 Aug 2022 00:57:46 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Thu, 04 Aug 2022 00:57:47 GMT
ENV MYSQL_MAJOR=8.0
# Thu, 04 Aug 2022 00:57:48 GMT
ENV MYSQL_VERSION=8.0.30-1.el8
# Thu, 04 Aug 2022 00:57:49 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Thu, 04 Aug 2022 00:58:17 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Thu, 04 Aug 2022 00:58:17 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Thu, 04 Aug 2022 00:58:18 GMT
ENV MYSQL_SHELL_VERSION=8.0.30-1.el8
# Thu, 04 Aug 2022 00:58:50 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Thu, 04 Aug 2022 00:58:51 GMT
VOLUME [/var/lib/mysql]
# Wed, 24 Aug 2022 03:30:34 GMT
COPY file:0362167b353388be7fb99432d9373f030ddd789bd27d57e183555c672530b303 in /usr/local/bin/ 
# Wed, 24 Aug 2022 03:30:35 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 24 Aug 2022 03:30:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 24 Aug 2022 03:30:37 GMT
EXPOSE 3306 33060
# Wed, 24 Aug 2022 03:30:38 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:ecf56004177eb6ca162c88de29e84bc4ba3d2e7efd3703df9ecae51b89003d52`  
		Last Modified: Thu, 04 Aug 2022 00:41:51 GMT  
		Size: 38.0 MB (38023046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1091d9f012e1e44cf00d872494ff008feb11a824aa940f5fccaadcf0f043e951`  
		Last Modified: Thu, 04 Aug 2022 00:59:35 GMT  
		Size: 888.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fabd9779d4678f8577c74505cc31bd42788a9ffa1eba563340b8ef29946b3e55`  
		Last Modified: Thu, 04 Aug 2022 00:59:36 GMT  
		Size: 857.2 KB (857152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6278448e2e194f0e2e8e7d2f29495296d594f7bd2e63d0306037e5b4f5125eb`  
		Last Modified: Thu, 04 Aug 2022 00:59:34 GMT  
		Size: 4.4 MB (4404159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6050832741b8d8e4dfba20e0d31c88f56b9b645c97752c9bbec708740c3e6e15`  
		Last Modified: Thu, 04 Aug 2022 00:59:33 GMT  
		Size: 2.6 KB (2607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0be9d1181fe5f7d6c39819a56c680e5e010a7b808b96eb00eabdeacd66ee6c1`  
		Last Modified: Thu, 04 Aug 2022 00:59:33 GMT  
		Size: 335.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbdaffd3eb50f6880d4e27c2ba2a47193ba4e1959b4647e5e794b0872e981c5b`  
		Last Modified: Thu, 04 Aug 2022 00:59:38 GMT  
		Size: 53.8 MB (53784614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a74c1ad0f09fc99fb019bcbfebb1b57f4f7fcf7e968e6ece353a06d583cab8ed`  
		Last Modified: Thu, 04 Aug 2022 00:59:31 GMT  
		Size: 315.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad2b7db10f4eacccefc72231d395d9920b81dd4bba86be2a8994b8ee9161ec92`  
		Last Modified: Thu, 04 Aug 2022 00:59:38 GMT  
		Size: 44.1 MB (44115089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f6281129c7fb0746caa0023cec4db82b482c85d81752eaafcff70498537c82a`  
		Last Modified: Wed, 24 Aug 2022 03:31:04 GMT  
		Size: 5.4 KB (5375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49dcabdef3045b25265175bee4894568254c4b35b769d77a0afedc6fd7ec9a1d`  
		Last Modified: Wed, 24 Aug 2022 03:31:04 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:debian`

```console
$ docker pull mysql@sha256:1b9a6291084f62abdcba3d057e6932e5419910c469f506f627eb31756e1b4666
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:debian` - linux; amd64

```console
$ docker pull mysql@sha256:ae245d06921e615701b017b2f6ac7aedaaf4cdf351bf57302cab7bc732ef3766
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **157.9 MB (157850853 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:960207ea9ac0c08b0485963dd531c0fcb4409c980661579f474af0119032a90a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 23 Aug 2022 00:20:50 GMT
ADD file:7726efb0e0eb5003dbcf2967ec29364479eec8b41f2569ff189372153115b54b in / 
# Tue, 23 Aug 2022 00:20:51 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 03:38:21 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 23 Aug 2022 03:38:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 03:38:26 GMT
ENV GOSU_VERSION=1.14
# Tue, 23 Aug 2022 03:38:35 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 23 Aug 2022 03:38:36 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 23 Aug 2022 03:38:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 03:38:42 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Tue, 23 Aug 2022 03:38:42 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 23 Aug 2022 03:38:42 GMT
ENV MYSQL_VERSION=8.0.30-1debian11
# Tue, 23 Aug 2022 03:38:43 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ bullseye mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Tue, 23 Aug 2022 03:38:56 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Tue, 23 Aug 2022 03:38:57 GMT
VOLUME [/var/lib/mysql]
# Tue, 23 Aug 2022 03:38:57 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Wed, 24 Aug 2022 00:36:52 GMT
COPY file:0362167b353388be7fb99432d9373f030ddd789bd27d57e183555c672530b303 in /usr/local/bin/ 
# Wed, 24 Aug 2022 00:36:53 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 24 Aug 2022 00:36:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 24 Aug 2022 00:36:53 GMT
EXPOSE 3306 33060
# Wed, 24 Aug 2022 00:36:53 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:7a6db449b51b92eac5c81cdbd82917785343f1664b2be57b22337b0a40c5b29d`  
		Last Modified: Tue, 23 Aug 2022 00:24:59 GMT  
		Size: 31.4 MB (31381485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63b23008bc872644b3493308929a67cefe09bcc825a15028af9b65d2b86b8154`  
		Last Modified: Tue, 23 Aug 2022 03:40:21 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82fdf48499dbc8cadd345c9a461bee300ec7f328fd970ea456ad13582f974b22`  
		Last Modified: Tue, 23 Aug 2022 03:40:22 GMT  
		Size: 4.4 MB (4414801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c75d7f84228a2f19e49b9a70c960e1b9fe6eceb637a24727ed6ec6c574b584d`  
		Last Modified: Tue, 23 Aug 2022 03:40:19 GMT  
		Size: 1.4 MB (1418466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61089f488e727e34e9b1c515a769ea0f63e4178b9f1f8a4b697f8345cd6a2fab`  
		Last Modified: Tue, 23 Aug 2022 03:40:19 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c82b0badc95c597bc8fa0c39ee975457037cb54ecafb310b75368ebaf1ea1c8`  
		Last Modified: Tue, 23 Aug 2022 03:40:21 GMT  
		Size: 12.7 MB (12661891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:245253769f71d25434c6c23a35770f5a993727fa9396802f45d5c41bf69ef18f`  
		Last Modified: Tue, 23 Aug 2022 03:40:19 GMT  
		Size: 2.5 KB (2549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7459b3c285350cb2e864e202e4a6ce674fe99d2338698d8aba402dca9be2a3f`  
		Last Modified: Tue, 23 Aug 2022 03:40:16 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e669258b3f94cee1da8b0e384ee0e8461fcaadff509b2929f9c2b45e684d674`  
		Last Modified: Tue, 23 Aug 2022 03:40:33 GMT  
		Size: 108.0 MB (107963194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7db97a7c2c85d65c31c5ecfaf632608190d8bd998f012fa7e7888fb4b9bd562`  
		Last Modified: Tue, 23 Aug 2022 03:40:16 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d96137de95c38044d259df48352ed8c80df7702fb6ee065be7cddcc1b0b3dc9`  
		Last Modified: Wed, 24 Aug 2022 00:37:52 GMT  
		Size: 5.4 KB (5367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eaa7d534011271dfaee8ae54a5c425d1e7913d687e2e33c5e4cab48dd813bc6`  
		Last Modified: Wed, 24 Aug 2022 00:37:52 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:latest`

```console
$ docker pull mysql@sha256:3de4d9814b28e48f225e259cc3b2c77530296afcec20bae53e1c7a4892f2a98e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:latest` - linux; amd64

```console
$ docker pull mysql@sha256:930e762c3f185d55d96a65e0d6cb2f724ffc16a87270f85283ae099d75e92ad0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.5 MB (132502250 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c989cc040bcf09e776e701e0fb567045ee77ed8667daf1a506d898717011bfe5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 04 Aug 2022 00:36:37 GMT
ADD file:0a05a213ae66f556b2b320291ac58ec9f2f67554e29338a072f1347f22864a49 in / 
# Thu, 04 Aug 2022 00:36:37 GMT
CMD ["/bin/bash"]
# Thu, 04 Aug 2022 01:24:42 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Thu, 04 Aug 2022 01:24:43 GMT
ENV GOSU_VERSION=1.14
# Thu, 04 Aug 2022 01:24:46 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 04 Aug 2022 01:25:08 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Thu, 04 Aug 2022 01:25:10 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Thu, 04 Aug 2022 01:25:10 GMT
ENV MYSQL_MAJOR=8.0
# Thu, 04 Aug 2022 01:25:10 GMT
ENV MYSQL_VERSION=8.0.30-1.el8
# Thu, 04 Aug 2022 01:25:10 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Thu, 04 Aug 2022 01:25:38 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Thu, 04 Aug 2022 01:25:39 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Thu, 04 Aug 2022 01:25:39 GMT
ENV MYSQL_SHELL_VERSION=8.0.30-1.el8
# Thu, 04 Aug 2022 01:26:10 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Thu, 04 Aug 2022 01:26:11 GMT
VOLUME [/var/lib/mysql]
# Wed, 24 Aug 2022 00:36:48 GMT
COPY file:0362167b353388be7fb99432d9373f030ddd789bd27d57e183555c672530b303 in /usr/local/bin/ 
# Wed, 24 Aug 2022 00:36:48 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 24 Aug 2022 00:36:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 24 Aug 2022 00:36:49 GMT
EXPOSE 3306 33060
# Wed, 24 Aug 2022 00:36:49 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:32c1bf40aba1f372a057d3280b0b7cdacde9d8500a069004e6f243bc09cde806`  
		Last Modified: Thu, 04 Aug 2022 00:37:33 GMT  
		Size: 39.2 MB (39223952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ac22f3a638d1c75f850c6c7b189d746c1ec6c58ec618f9e4b928f045df1b79d`  
		Last Modified: Thu, 04 Aug 2022 01:26:53 GMT  
		Size: 890.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1e7273ed05ed3b0f6be1e9a202f93199d88428c9dff52d1edce8d965ad50f8e`  
		Last Modified: Thu, 04 Aug 2022 01:26:54 GMT  
		Size: 928.8 KB (928835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20be45a0c6abbfaf62bd02c40f3cff6bf4822711b339ebcd4e1b7d6b2764ca20`  
		Last Modified: Thu, 04 Aug 2022 01:26:52 GMT  
		Size: 4.6 MB (4581809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:410a229693ff98f0a019a180a655ad903a882367b72f78f0ac3c595c1434a65e`  
		Last Modified: Thu, 04 Aug 2022 01:26:51 GMT  
		Size: 2.6 KB (2628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ce71e3a9b8879afc4dce1dc74841ecbae7da28798b238c88f0322b7bdc82472`  
		Last Modified: Thu, 04 Aug 2022 01:26:51 GMT  
		Size: 335.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c93c823af05bbde448c0a889b94ef2d6279b9c595c9b1a1abcbd49f795f7631c`  
		Last Modified: Thu, 04 Aug 2022 01:26:56 GMT  
		Size: 47.7 MB (47726773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6752c4d09c7204097f7ecbf50885874b620e77263452bb581ed1f4d9681344d`  
		Last Modified: Thu, 04 Aug 2022 01:26:49 GMT  
		Size: 315.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7f2cfe3efcbd4b98bf44100e9f3fc095ca4a480fd75a0028bae61aedfb6298a`  
		Last Modified: Thu, 04 Aug 2022 01:26:57 GMT  
		Size: 40.0 MB (40031217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09e782dbb2c3f52fb09d97fee4689b382e3789e244c209fe81782420a19d1a2a`  
		Last Modified: Wed, 24 Aug 2022 00:37:25 GMT  
		Size: 5.4 KB (5375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01199f522543dd7f72aa6b05d1be8d67dc48483700d79db260348af7e69f2aaa`  
		Last Modified: Wed, 24 Aug 2022 00:37:24 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:latest` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:54b1f5e74608236fe20d5dcdf39124a81244dd4d043b0798929614c1bc1ec602
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.2 MB (141193701 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1b9c6058e7a1b8f805b067ba9d4775d392fcfda1cdd601396716864c8f59e14`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 04 Aug 2022 00:40:43 GMT
ADD file:a68d82fa032efe6adc2926f7e745508f0541bba3f906e2702d34252353100747 in / 
# Thu, 04 Aug 2022 00:40:44 GMT
CMD ["/bin/bash"]
# Thu, 04 Aug 2022 00:57:16 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Thu, 04 Aug 2022 00:57:17 GMT
ENV GOSU_VERSION=1.14
# Thu, 04 Aug 2022 00:57:21 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 04 Aug 2022 00:57:44 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Thu, 04 Aug 2022 00:57:46 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Thu, 04 Aug 2022 00:57:47 GMT
ENV MYSQL_MAJOR=8.0
# Thu, 04 Aug 2022 00:57:48 GMT
ENV MYSQL_VERSION=8.0.30-1.el8
# Thu, 04 Aug 2022 00:57:49 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Thu, 04 Aug 2022 00:58:17 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Thu, 04 Aug 2022 00:58:17 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Thu, 04 Aug 2022 00:58:18 GMT
ENV MYSQL_SHELL_VERSION=8.0.30-1.el8
# Thu, 04 Aug 2022 00:58:50 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Thu, 04 Aug 2022 00:58:51 GMT
VOLUME [/var/lib/mysql]
# Wed, 24 Aug 2022 03:30:34 GMT
COPY file:0362167b353388be7fb99432d9373f030ddd789bd27d57e183555c672530b303 in /usr/local/bin/ 
# Wed, 24 Aug 2022 03:30:35 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 24 Aug 2022 03:30:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 24 Aug 2022 03:30:37 GMT
EXPOSE 3306 33060
# Wed, 24 Aug 2022 03:30:38 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:ecf56004177eb6ca162c88de29e84bc4ba3d2e7efd3703df9ecae51b89003d52`  
		Last Modified: Thu, 04 Aug 2022 00:41:51 GMT  
		Size: 38.0 MB (38023046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1091d9f012e1e44cf00d872494ff008feb11a824aa940f5fccaadcf0f043e951`  
		Last Modified: Thu, 04 Aug 2022 00:59:35 GMT  
		Size: 888.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fabd9779d4678f8577c74505cc31bd42788a9ffa1eba563340b8ef29946b3e55`  
		Last Modified: Thu, 04 Aug 2022 00:59:36 GMT  
		Size: 857.2 KB (857152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6278448e2e194f0e2e8e7d2f29495296d594f7bd2e63d0306037e5b4f5125eb`  
		Last Modified: Thu, 04 Aug 2022 00:59:34 GMT  
		Size: 4.4 MB (4404159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6050832741b8d8e4dfba20e0d31c88f56b9b645c97752c9bbec708740c3e6e15`  
		Last Modified: Thu, 04 Aug 2022 00:59:33 GMT  
		Size: 2.6 KB (2607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0be9d1181fe5f7d6c39819a56c680e5e010a7b808b96eb00eabdeacd66ee6c1`  
		Last Modified: Thu, 04 Aug 2022 00:59:33 GMT  
		Size: 335.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbdaffd3eb50f6880d4e27c2ba2a47193ba4e1959b4647e5e794b0872e981c5b`  
		Last Modified: Thu, 04 Aug 2022 00:59:38 GMT  
		Size: 53.8 MB (53784614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a74c1ad0f09fc99fb019bcbfebb1b57f4f7fcf7e968e6ece353a06d583cab8ed`  
		Last Modified: Thu, 04 Aug 2022 00:59:31 GMT  
		Size: 315.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad2b7db10f4eacccefc72231d395d9920b81dd4bba86be2a8994b8ee9161ec92`  
		Last Modified: Thu, 04 Aug 2022 00:59:38 GMT  
		Size: 44.1 MB (44115089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f6281129c7fb0746caa0023cec4db82b482c85d81752eaafcff70498537c82a`  
		Last Modified: Wed, 24 Aug 2022 03:31:04 GMT  
		Size: 5.4 KB (5375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49dcabdef3045b25265175bee4894568254c4b35b769d77a0afedc6fd7ec9a1d`  
		Last Modified: Wed, 24 Aug 2022 03:31:04 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:oracle`

```console
$ docker pull mysql@sha256:3de4d9814b28e48f225e259cc3b2c77530296afcec20bae53e1c7a4892f2a98e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:oracle` - linux; amd64

```console
$ docker pull mysql@sha256:930e762c3f185d55d96a65e0d6cb2f724ffc16a87270f85283ae099d75e92ad0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.5 MB (132502250 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c989cc040bcf09e776e701e0fb567045ee77ed8667daf1a506d898717011bfe5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 04 Aug 2022 00:36:37 GMT
ADD file:0a05a213ae66f556b2b320291ac58ec9f2f67554e29338a072f1347f22864a49 in / 
# Thu, 04 Aug 2022 00:36:37 GMT
CMD ["/bin/bash"]
# Thu, 04 Aug 2022 01:24:42 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Thu, 04 Aug 2022 01:24:43 GMT
ENV GOSU_VERSION=1.14
# Thu, 04 Aug 2022 01:24:46 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 04 Aug 2022 01:25:08 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Thu, 04 Aug 2022 01:25:10 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Thu, 04 Aug 2022 01:25:10 GMT
ENV MYSQL_MAJOR=8.0
# Thu, 04 Aug 2022 01:25:10 GMT
ENV MYSQL_VERSION=8.0.30-1.el8
# Thu, 04 Aug 2022 01:25:10 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Thu, 04 Aug 2022 01:25:38 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Thu, 04 Aug 2022 01:25:39 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Thu, 04 Aug 2022 01:25:39 GMT
ENV MYSQL_SHELL_VERSION=8.0.30-1.el8
# Thu, 04 Aug 2022 01:26:10 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Thu, 04 Aug 2022 01:26:11 GMT
VOLUME [/var/lib/mysql]
# Wed, 24 Aug 2022 00:36:48 GMT
COPY file:0362167b353388be7fb99432d9373f030ddd789bd27d57e183555c672530b303 in /usr/local/bin/ 
# Wed, 24 Aug 2022 00:36:48 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 24 Aug 2022 00:36:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 24 Aug 2022 00:36:49 GMT
EXPOSE 3306 33060
# Wed, 24 Aug 2022 00:36:49 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:32c1bf40aba1f372a057d3280b0b7cdacde9d8500a069004e6f243bc09cde806`  
		Last Modified: Thu, 04 Aug 2022 00:37:33 GMT  
		Size: 39.2 MB (39223952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ac22f3a638d1c75f850c6c7b189d746c1ec6c58ec618f9e4b928f045df1b79d`  
		Last Modified: Thu, 04 Aug 2022 01:26:53 GMT  
		Size: 890.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1e7273ed05ed3b0f6be1e9a202f93199d88428c9dff52d1edce8d965ad50f8e`  
		Last Modified: Thu, 04 Aug 2022 01:26:54 GMT  
		Size: 928.8 KB (928835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20be45a0c6abbfaf62bd02c40f3cff6bf4822711b339ebcd4e1b7d6b2764ca20`  
		Last Modified: Thu, 04 Aug 2022 01:26:52 GMT  
		Size: 4.6 MB (4581809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:410a229693ff98f0a019a180a655ad903a882367b72f78f0ac3c595c1434a65e`  
		Last Modified: Thu, 04 Aug 2022 01:26:51 GMT  
		Size: 2.6 KB (2628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ce71e3a9b8879afc4dce1dc74841ecbae7da28798b238c88f0322b7bdc82472`  
		Last Modified: Thu, 04 Aug 2022 01:26:51 GMT  
		Size: 335.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c93c823af05bbde448c0a889b94ef2d6279b9c595c9b1a1abcbd49f795f7631c`  
		Last Modified: Thu, 04 Aug 2022 01:26:56 GMT  
		Size: 47.7 MB (47726773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6752c4d09c7204097f7ecbf50885874b620e77263452bb581ed1f4d9681344d`  
		Last Modified: Thu, 04 Aug 2022 01:26:49 GMT  
		Size: 315.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7f2cfe3efcbd4b98bf44100e9f3fc095ca4a480fd75a0028bae61aedfb6298a`  
		Last Modified: Thu, 04 Aug 2022 01:26:57 GMT  
		Size: 40.0 MB (40031217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09e782dbb2c3f52fb09d97fee4689b382e3789e244c209fe81782420a19d1a2a`  
		Last Modified: Wed, 24 Aug 2022 00:37:25 GMT  
		Size: 5.4 KB (5375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01199f522543dd7f72aa6b05d1be8d67dc48483700d79db260348af7e69f2aaa`  
		Last Modified: Wed, 24 Aug 2022 00:37:24 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:oracle` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:54b1f5e74608236fe20d5dcdf39124a81244dd4d043b0798929614c1bc1ec602
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.2 MB (141193701 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1b9c6058e7a1b8f805b067ba9d4775d392fcfda1cdd601396716864c8f59e14`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 04 Aug 2022 00:40:43 GMT
ADD file:a68d82fa032efe6adc2926f7e745508f0541bba3f906e2702d34252353100747 in / 
# Thu, 04 Aug 2022 00:40:44 GMT
CMD ["/bin/bash"]
# Thu, 04 Aug 2022 00:57:16 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Thu, 04 Aug 2022 00:57:17 GMT
ENV GOSU_VERSION=1.14
# Thu, 04 Aug 2022 00:57:21 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 04 Aug 2022 00:57:44 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Thu, 04 Aug 2022 00:57:46 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Thu, 04 Aug 2022 00:57:47 GMT
ENV MYSQL_MAJOR=8.0
# Thu, 04 Aug 2022 00:57:48 GMT
ENV MYSQL_VERSION=8.0.30-1.el8
# Thu, 04 Aug 2022 00:57:49 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Thu, 04 Aug 2022 00:58:17 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Thu, 04 Aug 2022 00:58:17 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Thu, 04 Aug 2022 00:58:18 GMT
ENV MYSQL_SHELL_VERSION=8.0.30-1.el8
# Thu, 04 Aug 2022 00:58:50 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Thu, 04 Aug 2022 00:58:51 GMT
VOLUME [/var/lib/mysql]
# Wed, 24 Aug 2022 03:30:34 GMT
COPY file:0362167b353388be7fb99432d9373f030ddd789bd27d57e183555c672530b303 in /usr/local/bin/ 
# Wed, 24 Aug 2022 03:30:35 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 24 Aug 2022 03:30:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 24 Aug 2022 03:30:37 GMT
EXPOSE 3306 33060
# Wed, 24 Aug 2022 03:30:38 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:ecf56004177eb6ca162c88de29e84bc4ba3d2e7efd3703df9ecae51b89003d52`  
		Last Modified: Thu, 04 Aug 2022 00:41:51 GMT  
		Size: 38.0 MB (38023046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1091d9f012e1e44cf00d872494ff008feb11a824aa940f5fccaadcf0f043e951`  
		Last Modified: Thu, 04 Aug 2022 00:59:35 GMT  
		Size: 888.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fabd9779d4678f8577c74505cc31bd42788a9ffa1eba563340b8ef29946b3e55`  
		Last Modified: Thu, 04 Aug 2022 00:59:36 GMT  
		Size: 857.2 KB (857152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6278448e2e194f0e2e8e7d2f29495296d594f7bd2e63d0306037e5b4f5125eb`  
		Last Modified: Thu, 04 Aug 2022 00:59:34 GMT  
		Size: 4.4 MB (4404159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6050832741b8d8e4dfba20e0d31c88f56b9b645c97752c9bbec708740c3e6e15`  
		Last Modified: Thu, 04 Aug 2022 00:59:33 GMT  
		Size: 2.6 KB (2607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0be9d1181fe5f7d6c39819a56c680e5e010a7b808b96eb00eabdeacd66ee6c1`  
		Last Modified: Thu, 04 Aug 2022 00:59:33 GMT  
		Size: 335.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbdaffd3eb50f6880d4e27c2ba2a47193ba4e1959b4647e5e794b0872e981c5b`  
		Last Modified: Thu, 04 Aug 2022 00:59:38 GMT  
		Size: 53.8 MB (53784614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a74c1ad0f09fc99fb019bcbfebb1b57f4f7fcf7e968e6ece353a06d583cab8ed`  
		Last Modified: Thu, 04 Aug 2022 00:59:31 GMT  
		Size: 315.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad2b7db10f4eacccefc72231d395d9920b81dd4bba86be2a8994b8ee9161ec92`  
		Last Modified: Thu, 04 Aug 2022 00:59:38 GMT  
		Size: 44.1 MB (44115089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f6281129c7fb0746caa0023cec4db82b482c85d81752eaafcff70498537c82a`  
		Last Modified: Wed, 24 Aug 2022 03:31:04 GMT  
		Size: 5.4 KB (5375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49dcabdef3045b25265175bee4894568254c4b35b769d77a0afedc6fd7ec9a1d`  
		Last Modified: Wed, 24 Aug 2022 03:31:04 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
