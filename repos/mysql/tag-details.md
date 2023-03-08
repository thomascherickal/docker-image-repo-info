<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `mysql`

-	[`mysql:5`](#mysql5)
-	[`mysql:5-debian`](#mysql5-debian)
-	[`mysql:5-oracle`](#mysql5-oracle)
-	[`mysql:5.7`](#mysql57)
-	[`mysql:5.7-debian`](#mysql57-debian)
-	[`mysql:5.7-oracle`](#mysql57-oracle)
-	[`mysql:5.7.41`](#mysql5741)
-	[`mysql:5.7.41-debian`](#mysql5741-debian)
-	[`mysql:5.7.41-oracle`](#mysql5741-oracle)
-	[`mysql:8`](#mysql8)
-	[`mysql:8-debian`](#mysql8-debian)
-	[`mysql:8-oracle`](#mysql8-oracle)
-	[`mysql:8.0`](#mysql80)
-	[`mysql:8.0-debian`](#mysql80-debian)
-	[`mysql:8.0-oracle`](#mysql80-oracle)
-	[`mysql:8.0.32`](#mysql8032)
-	[`mysql:8.0.32-debian`](#mysql8032-debian)
-	[`mysql:8.0.32-oracle`](#mysql8032-oracle)
-	[`mysql:debian`](#mysqldebian)
-	[`mysql:latest`](#mysqllatest)
-	[`mysql:oracle`](#mysqloracle)

## `mysql:5`

```console
$ docker pull mysql@sha256:9202fc6bc8fa63615e6bfc0049fc660f712d164220c5c54d86519870c305ea48
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5` - linux; amd64

```console
$ docker pull mysql@sha256:c5d8092d5424881f6fb831fefd502de90495c2b62c87d0be67f7b66748906252
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.0 MB (130008096 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0018a8d838923d94318aa8dd3195510226b31540901a6f4c643aacec69f7ab62`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 08 Mar 2023 20:22:54 GMT
ADD file:e205deb729daf99a168c27d3f97cd2b69e736fc9d4bee9ea220ec86921574a0f in / 
# Wed, 08 Mar 2023 20:22:55 GMT
CMD ["/bin/bash"]
# Wed, 08 Mar 2023 20:42:01 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 08 Mar 2023 20:42:02 GMT
ENV GOSU_VERSION=1.16
# Wed, 08 Mar 2023 20:42:04 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 08 Mar 2023 20:42:22 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False oracle-epel-release-el7; 	yum install -y --setopt=skip_missing_names_on_install=False 		bzip2 		gzip 		openssl 		xz 		zstd 	; 	yum clean all
# Wed, 08 Mar 2023 20:42:23 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 08 Mar 2023 20:42:23 GMT
ENV MYSQL_MAJOR=5.7
# Wed, 08 Mar 2023 20:42:23 GMT
ENV MYSQL_VERSION=5.7.41-1.el7
# Wed, 08 Mar 2023 20:42:23 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql5.7-server-minimal]'; 		echo 'name=MySQL 5.7 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-5.7-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 08 Mar 2023 20:42:42 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-community-server-minimal-$MYSQL_VERSION"; 	yum clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	{ echo '!includedir /etc/mysql/mysql.conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/mysql.conf.d; 		find /etc/my.cnf /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/'; 		mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 08 Mar 2023 20:42:43 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 08 Mar 2023 20:42:43 GMT
ENV MYSQL_SHELL_VERSION=8.0.32-1.el7
# Wed, 08 Mar 2023 20:43:07 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-shell-$MYSQL_SHELL_VERSION"; 	yum clean all; 		mysqlsh --version
# Wed, 08 Mar 2023 20:43:08 GMT
VOLUME [/var/lib/mysql]
# Wed, 08 Mar 2023 20:43:08 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 08 Mar 2023 20:43:08 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 08 Mar 2023 20:43:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 08 Mar 2023 20:43:09 GMT
EXPOSE 3306 33060
# Wed, 08 Mar 2023 20:43:09 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:7b659169cb9226d08443358aa4e8147f3144614ac33f7a41217b0cf62a4d3326`  
		Last Modified: Wed, 08 Mar 2023 20:24:41 GMT  
		Size: 50.5 MB (50467964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e47c3f06a3f5705076a7154d7f81aa0bb1433377185e05fa520105f17af2f370`  
		Last Modified: Wed, 08 Mar 2023 20:44:24 GMT  
		Size: 871.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0656a27f56e8064f2d45e3264e37ae491064cf57f2469f9703ffd780771b496`  
		Last Modified: Wed, 08 Mar 2023 20:44:24 GMT  
		Size: 983.7 KB (983707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9f33f34ef42570bb8d9a791d31a6653685baecc2464a6ae65f57d19d2954b5d`  
		Last Modified: Wed, 08 Mar 2023 20:44:23 GMT  
		Size: 4.6 MB (4585631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fc5cbaf8704473ad86bf905f4416c09c189ca133bd57418884189b501f3bbd8`  
		Last Modified: Wed, 08 Mar 2023 20:44:22 GMT  
		Size: 2.7 KB (2654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fb8407bef93fd1fc829cfd13269442f272898b097cfda975b92617eb101bbf8`  
		Last Modified: Wed, 08 Mar 2023 20:44:22 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8be4a2d031b5252b75e271b780be63c907f72b1b15280c13bdbcfe8a4cd653e`  
		Last Modified: Wed, 08 Mar 2023 20:44:24 GMT  
		Size: 25.5 MB (25521558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6cb2bff25e38b09537aa3d38f370061b28bc812ff4ffff86b4b1a435f544173`  
		Last Modified: Wed, 08 Mar 2023 20:44:20 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:056cc4a5c89ae053998222fcd94d51e5c6b3eec297d15e9b7d60b182269b76b8`  
		Last Modified: Wed, 08 Mar 2023 20:44:30 GMT  
		Size: 48.4 MB (48439547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8428969731444b79af296589ae42c54ebcba5e34cb2c12d6cb4e1a5e95f918db`  
		Last Modified: Wed, 08 Mar 2023 20:44:20 GMT  
		Size: 5.4 KB (5393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e55b6e95b292d6e888669bbd77813b1bd08cab1d6b78d1dfe959b959062135ac`  
		Last Modified: Wed, 08 Mar 2023 20:44:20 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5-debian`

```console
$ docker pull mysql@sha256:36002a394b549b6d293d7f76de854e69399f0c093e6b1f16baefdafe5ea21ffa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5-debian` - linux; amd64

```console
$ docker pull mysql@sha256:ef2398ea6c295c668cf3e969c28ae7088845b07beb07b96792698c3f80c69c8f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **162.7 MB (162694168 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20e50dddd01b351b398beff0bb34172b2edcb046f290ff29ea946b92f7c60cfd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 01 Mar 2023 04:10:22 GMT
ADD file:2254e48bf53907be7a0b1744bc4fcd7805a627672793cf5f86a01ac751a1b24d in / 
# Wed, 01 Mar 2023 04:10:22 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 08:17:40 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 01 Mar 2023 08:17:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 08:17:48 GMT
ENV GOSU_VERSION=1.16
# Wed, 01 Mar 2023 08:17:56 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 01 Mar 2023 08:17:57 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 01 Mar 2023 08:18:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 08:18:04 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Wed, 01 Mar 2023 08:18:04 GMT
ENV MYSQL_MAJOR=5.7
# Wed, 01 Mar 2023 08:18:04 GMT
ENV MYSQL_VERSION=5.7.41-1debian10
# Wed, 01 Mar 2023 08:18:05 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-5.7' > /etc/apt/sources.list.d/mysql.list
# Wed, 01 Mar 2023 08:18:23 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-server="${MYSQL_VERSION}" 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Wed, 01 Mar 2023 08:18:24 GMT
VOLUME [/var/lib/mysql]
# Wed, 01 Mar 2023 08:18:24 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 01 Mar 2023 08:18:25 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 01 Mar 2023 08:18:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Mar 2023 08:18:25 GMT
EXPOSE 3306 33060
# Wed, 01 Mar 2023 08:18:25 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:8fd419aca81cfd3987d61550e700546537628562693bc01acc9f85468f483706`  
		Last Modified: Wed, 01 Mar 2023 04:15:04 GMT  
		Size: 27.1 MB (27139882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d19bdbefd94aa10eb97a97f00a8597a423524a8ee1ac0481ee949550aab103d4`  
		Last Modified: Wed, 01 Mar 2023 08:19:28 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:925e2a505f95d645bf606d89d712e36892cf107ac2734f53a99d73d957828dbd`  
		Last Modified: Wed, 01 Mar 2023 08:19:28 GMT  
		Size: 4.2 MB (4182352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:615b524b079671c0807d23d7b6165c051d3e057cf337dc79c4692eff7f2a1754`  
		Last Modified: Wed, 01 Mar 2023 08:19:27 GMT  
		Size: 1.4 MB (1441782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23269a497e1054aa28f4f235d816862f2a9cff683f19dc248bb57d0c9bdbc544`  
		Last Modified: Wed, 01 Mar 2023 08:19:27 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:034fd6f00cfd596d0fc2e2a26ac97b0a306501ee99bff82b16a26dcf1e06b21b`  
		Last Modified: Wed, 01 Mar 2023 08:19:29 GMT  
		Size: 14.1 MB (14087009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a1c4f6ce4b763cc7098b8bb50e2063925a87b37b938873fb8721773fdc77891`  
		Last Modified: Wed, 01 Mar 2023 08:19:25 GMT  
		Size: 2.5 KB (2548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a74551e5bdd8aa6103cb0145f16fd744127eb8e2076d188e3bdae8e304ffb0b`  
		Last Modified: Wed, 01 Mar 2023 08:19:25 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5a3a8bb0579b93926aafefcf6a0f480e7eef4bdd55faebd8c23c3dc84748743`  
		Last Modified: Wed, 01 Mar 2023 08:19:39 GMT  
		Size: 115.8 MB (115832956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cfbfd35c59124cb5b9f9562b11ab90a3f11e8634febc4bf66e0d75231f98c5b`  
		Last Modified: Wed, 01 Mar 2023 08:19:25 GMT  
		Size: 5.4 KB (5388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a9277a314e7f20aba5d30ad70cfb9c6fc26283bc49c06199e1285d04a31b4cb`  
		Last Modified: Wed, 01 Mar 2023 08:19:25 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5-oracle`

```console
$ docker pull mysql@sha256:9202fc6bc8fa63615e6bfc0049fc660f712d164220c5c54d86519870c305ea48
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:c5d8092d5424881f6fb831fefd502de90495c2b62c87d0be67f7b66748906252
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.0 MB (130008096 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0018a8d838923d94318aa8dd3195510226b31540901a6f4c643aacec69f7ab62`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 08 Mar 2023 20:22:54 GMT
ADD file:e205deb729daf99a168c27d3f97cd2b69e736fc9d4bee9ea220ec86921574a0f in / 
# Wed, 08 Mar 2023 20:22:55 GMT
CMD ["/bin/bash"]
# Wed, 08 Mar 2023 20:42:01 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 08 Mar 2023 20:42:02 GMT
ENV GOSU_VERSION=1.16
# Wed, 08 Mar 2023 20:42:04 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 08 Mar 2023 20:42:22 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False oracle-epel-release-el7; 	yum install -y --setopt=skip_missing_names_on_install=False 		bzip2 		gzip 		openssl 		xz 		zstd 	; 	yum clean all
# Wed, 08 Mar 2023 20:42:23 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 08 Mar 2023 20:42:23 GMT
ENV MYSQL_MAJOR=5.7
# Wed, 08 Mar 2023 20:42:23 GMT
ENV MYSQL_VERSION=5.7.41-1.el7
# Wed, 08 Mar 2023 20:42:23 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql5.7-server-minimal]'; 		echo 'name=MySQL 5.7 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-5.7-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 08 Mar 2023 20:42:42 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-community-server-minimal-$MYSQL_VERSION"; 	yum clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	{ echo '!includedir /etc/mysql/mysql.conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/mysql.conf.d; 		find /etc/my.cnf /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/'; 		mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 08 Mar 2023 20:42:43 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 08 Mar 2023 20:42:43 GMT
ENV MYSQL_SHELL_VERSION=8.0.32-1.el7
# Wed, 08 Mar 2023 20:43:07 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-shell-$MYSQL_SHELL_VERSION"; 	yum clean all; 		mysqlsh --version
# Wed, 08 Mar 2023 20:43:08 GMT
VOLUME [/var/lib/mysql]
# Wed, 08 Mar 2023 20:43:08 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 08 Mar 2023 20:43:08 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 08 Mar 2023 20:43:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 08 Mar 2023 20:43:09 GMT
EXPOSE 3306 33060
# Wed, 08 Mar 2023 20:43:09 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:7b659169cb9226d08443358aa4e8147f3144614ac33f7a41217b0cf62a4d3326`  
		Last Modified: Wed, 08 Mar 2023 20:24:41 GMT  
		Size: 50.5 MB (50467964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e47c3f06a3f5705076a7154d7f81aa0bb1433377185e05fa520105f17af2f370`  
		Last Modified: Wed, 08 Mar 2023 20:44:24 GMT  
		Size: 871.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0656a27f56e8064f2d45e3264e37ae491064cf57f2469f9703ffd780771b496`  
		Last Modified: Wed, 08 Mar 2023 20:44:24 GMT  
		Size: 983.7 KB (983707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9f33f34ef42570bb8d9a791d31a6653685baecc2464a6ae65f57d19d2954b5d`  
		Last Modified: Wed, 08 Mar 2023 20:44:23 GMT  
		Size: 4.6 MB (4585631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fc5cbaf8704473ad86bf905f4416c09c189ca133bd57418884189b501f3bbd8`  
		Last Modified: Wed, 08 Mar 2023 20:44:22 GMT  
		Size: 2.7 KB (2654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fb8407bef93fd1fc829cfd13269442f272898b097cfda975b92617eb101bbf8`  
		Last Modified: Wed, 08 Mar 2023 20:44:22 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8be4a2d031b5252b75e271b780be63c907f72b1b15280c13bdbcfe8a4cd653e`  
		Last Modified: Wed, 08 Mar 2023 20:44:24 GMT  
		Size: 25.5 MB (25521558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6cb2bff25e38b09537aa3d38f370061b28bc812ff4ffff86b4b1a435f544173`  
		Last Modified: Wed, 08 Mar 2023 20:44:20 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:056cc4a5c89ae053998222fcd94d51e5c6b3eec297d15e9b7d60b182269b76b8`  
		Last Modified: Wed, 08 Mar 2023 20:44:30 GMT  
		Size: 48.4 MB (48439547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8428969731444b79af296589ae42c54ebcba5e34cb2c12d6cb4e1a5e95f918db`  
		Last Modified: Wed, 08 Mar 2023 20:44:20 GMT  
		Size: 5.4 KB (5393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e55b6e95b292d6e888669bbd77813b1bd08cab1d6b78d1dfe959b959062135ac`  
		Last Modified: Wed, 08 Mar 2023 20:44:20 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7`

```console
$ docker pull mysql@sha256:9202fc6bc8fa63615e6bfc0049fc660f712d164220c5c54d86519870c305ea48
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7` - linux; amd64

```console
$ docker pull mysql@sha256:c5d8092d5424881f6fb831fefd502de90495c2b62c87d0be67f7b66748906252
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.0 MB (130008096 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0018a8d838923d94318aa8dd3195510226b31540901a6f4c643aacec69f7ab62`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 08 Mar 2023 20:22:54 GMT
ADD file:e205deb729daf99a168c27d3f97cd2b69e736fc9d4bee9ea220ec86921574a0f in / 
# Wed, 08 Mar 2023 20:22:55 GMT
CMD ["/bin/bash"]
# Wed, 08 Mar 2023 20:42:01 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 08 Mar 2023 20:42:02 GMT
ENV GOSU_VERSION=1.16
# Wed, 08 Mar 2023 20:42:04 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 08 Mar 2023 20:42:22 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False oracle-epel-release-el7; 	yum install -y --setopt=skip_missing_names_on_install=False 		bzip2 		gzip 		openssl 		xz 		zstd 	; 	yum clean all
# Wed, 08 Mar 2023 20:42:23 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 08 Mar 2023 20:42:23 GMT
ENV MYSQL_MAJOR=5.7
# Wed, 08 Mar 2023 20:42:23 GMT
ENV MYSQL_VERSION=5.7.41-1.el7
# Wed, 08 Mar 2023 20:42:23 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql5.7-server-minimal]'; 		echo 'name=MySQL 5.7 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-5.7-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 08 Mar 2023 20:42:42 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-community-server-minimal-$MYSQL_VERSION"; 	yum clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	{ echo '!includedir /etc/mysql/mysql.conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/mysql.conf.d; 		find /etc/my.cnf /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/'; 		mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 08 Mar 2023 20:42:43 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 08 Mar 2023 20:42:43 GMT
ENV MYSQL_SHELL_VERSION=8.0.32-1.el7
# Wed, 08 Mar 2023 20:43:07 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-shell-$MYSQL_SHELL_VERSION"; 	yum clean all; 		mysqlsh --version
# Wed, 08 Mar 2023 20:43:08 GMT
VOLUME [/var/lib/mysql]
# Wed, 08 Mar 2023 20:43:08 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 08 Mar 2023 20:43:08 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 08 Mar 2023 20:43:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 08 Mar 2023 20:43:09 GMT
EXPOSE 3306 33060
# Wed, 08 Mar 2023 20:43:09 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:7b659169cb9226d08443358aa4e8147f3144614ac33f7a41217b0cf62a4d3326`  
		Last Modified: Wed, 08 Mar 2023 20:24:41 GMT  
		Size: 50.5 MB (50467964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e47c3f06a3f5705076a7154d7f81aa0bb1433377185e05fa520105f17af2f370`  
		Last Modified: Wed, 08 Mar 2023 20:44:24 GMT  
		Size: 871.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0656a27f56e8064f2d45e3264e37ae491064cf57f2469f9703ffd780771b496`  
		Last Modified: Wed, 08 Mar 2023 20:44:24 GMT  
		Size: 983.7 KB (983707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9f33f34ef42570bb8d9a791d31a6653685baecc2464a6ae65f57d19d2954b5d`  
		Last Modified: Wed, 08 Mar 2023 20:44:23 GMT  
		Size: 4.6 MB (4585631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fc5cbaf8704473ad86bf905f4416c09c189ca133bd57418884189b501f3bbd8`  
		Last Modified: Wed, 08 Mar 2023 20:44:22 GMT  
		Size: 2.7 KB (2654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fb8407bef93fd1fc829cfd13269442f272898b097cfda975b92617eb101bbf8`  
		Last Modified: Wed, 08 Mar 2023 20:44:22 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8be4a2d031b5252b75e271b780be63c907f72b1b15280c13bdbcfe8a4cd653e`  
		Last Modified: Wed, 08 Mar 2023 20:44:24 GMT  
		Size: 25.5 MB (25521558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6cb2bff25e38b09537aa3d38f370061b28bc812ff4ffff86b4b1a435f544173`  
		Last Modified: Wed, 08 Mar 2023 20:44:20 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:056cc4a5c89ae053998222fcd94d51e5c6b3eec297d15e9b7d60b182269b76b8`  
		Last Modified: Wed, 08 Mar 2023 20:44:30 GMT  
		Size: 48.4 MB (48439547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8428969731444b79af296589ae42c54ebcba5e34cb2c12d6cb4e1a5e95f918db`  
		Last Modified: Wed, 08 Mar 2023 20:44:20 GMT  
		Size: 5.4 KB (5393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e55b6e95b292d6e888669bbd77813b1bd08cab1d6b78d1dfe959b959062135ac`  
		Last Modified: Wed, 08 Mar 2023 20:44:20 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7-debian`

```console
$ docker pull mysql@sha256:36002a394b549b6d293d7f76de854e69399f0c093e6b1f16baefdafe5ea21ffa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7-debian` - linux; amd64

```console
$ docker pull mysql@sha256:ef2398ea6c295c668cf3e969c28ae7088845b07beb07b96792698c3f80c69c8f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **162.7 MB (162694168 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20e50dddd01b351b398beff0bb34172b2edcb046f290ff29ea946b92f7c60cfd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 01 Mar 2023 04:10:22 GMT
ADD file:2254e48bf53907be7a0b1744bc4fcd7805a627672793cf5f86a01ac751a1b24d in / 
# Wed, 01 Mar 2023 04:10:22 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 08:17:40 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 01 Mar 2023 08:17:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 08:17:48 GMT
ENV GOSU_VERSION=1.16
# Wed, 01 Mar 2023 08:17:56 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 01 Mar 2023 08:17:57 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 01 Mar 2023 08:18:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 08:18:04 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Wed, 01 Mar 2023 08:18:04 GMT
ENV MYSQL_MAJOR=5.7
# Wed, 01 Mar 2023 08:18:04 GMT
ENV MYSQL_VERSION=5.7.41-1debian10
# Wed, 01 Mar 2023 08:18:05 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-5.7' > /etc/apt/sources.list.d/mysql.list
# Wed, 01 Mar 2023 08:18:23 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-server="${MYSQL_VERSION}" 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Wed, 01 Mar 2023 08:18:24 GMT
VOLUME [/var/lib/mysql]
# Wed, 01 Mar 2023 08:18:24 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 01 Mar 2023 08:18:25 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 01 Mar 2023 08:18:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Mar 2023 08:18:25 GMT
EXPOSE 3306 33060
# Wed, 01 Mar 2023 08:18:25 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:8fd419aca81cfd3987d61550e700546537628562693bc01acc9f85468f483706`  
		Last Modified: Wed, 01 Mar 2023 04:15:04 GMT  
		Size: 27.1 MB (27139882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d19bdbefd94aa10eb97a97f00a8597a423524a8ee1ac0481ee949550aab103d4`  
		Last Modified: Wed, 01 Mar 2023 08:19:28 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:925e2a505f95d645bf606d89d712e36892cf107ac2734f53a99d73d957828dbd`  
		Last Modified: Wed, 01 Mar 2023 08:19:28 GMT  
		Size: 4.2 MB (4182352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:615b524b079671c0807d23d7b6165c051d3e057cf337dc79c4692eff7f2a1754`  
		Last Modified: Wed, 01 Mar 2023 08:19:27 GMT  
		Size: 1.4 MB (1441782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23269a497e1054aa28f4f235d816862f2a9cff683f19dc248bb57d0c9bdbc544`  
		Last Modified: Wed, 01 Mar 2023 08:19:27 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:034fd6f00cfd596d0fc2e2a26ac97b0a306501ee99bff82b16a26dcf1e06b21b`  
		Last Modified: Wed, 01 Mar 2023 08:19:29 GMT  
		Size: 14.1 MB (14087009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a1c4f6ce4b763cc7098b8bb50e2063925a87b37b938873fb8721773fdc77891`  
		Last Modified: Wed, 01 Mar 2023 08:19:25 GMT  
		Size: 2.5 KB (2548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a74551e5bdd8aa6103cb0145f16fd744127eb8e2076d188e3bdae8e304ffb0b`  
		Last Modified: Wed, 01 Mar 2023 08:19:25 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5a3a8bb0579b93926aafefcf6a0f480e7eef4bdd55faebd8c23c3dc84748743`  
		Last Modified: Wed, 01 Mar 2023 08:19:39 GMT  
		Size: 115.8 MB (115832956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cfbfd35c59124cb5b9f9562b11ab90a3f11e8634febc4bf66e0d75231f98c5b`  
		Last Modified: Wed, 01 Mar 2023 08:19:25 GMT  
		Size: 5.4 KB (5388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a9277a314e7f20aba5d30ad70cfb9c6fc26283bc49c06199e1285d04a31b4cb`  
		Last Modified: Wed, 01 Mar 2023 08:19:25 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7-oracle`

```console
$ docker pull mysql@sha256:9202fc6bc8fa63615e6bfc0049fc660f712d164220c5c54d86519870c305ea48
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:c5d8092d5424881f6fb831fefd502de90495c2b62c87d0be67f7b66748906252
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.0 MB (130008096 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0018a8d838923d94318aa8dd3195510226b31540901a6f4c643aacec69f7ab62`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 08 Mar 2023 20:22:54 GMT
ADD file:e205deb729daf99a168c27d3f97cd2b69e736fc9d4bee9ea220ec86921574a0f in / 
# Wed, 08 Mar 2023 20:22:55 GMT
CMD ["/bin/bash"]
# Wed, 08 Mar 2023 20:42:01 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 08 Mar 2023 20:42:02 GMT
ENV GOSU_VERSION=1.16
# Wed, 08 Mar 2023 20:42:04 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 08 Mar 2023 20:42:22 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False oracle-epel-release-el7; 	yum install -y --setopt=skip_missing_names_on_install=False 		bzip2 		gzip 		openssl 		xz 		zstd 	; 	yum clean all
# Wed, 08 Mar 2023 20:42:23 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 08 Mar 2023 20:42:23 GMT
ENV MYSQL_MAJOR=5.7
# Wed, 08 Mar 2023 20:42:23 GMT
ENV MYSQL_VERSION=5.7.41-1.el7
# Wed, 08 Mar 2023 20:42:23 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql5.7-server-minimal]'; 		echo 'name=MySQL 5.7 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-5.7-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 08 Mar 2023 20:42:42 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-community-server-minimal-$MYSQL_VERSION"; 	yum clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	{ echo '!includedir /etc/mysql/mysql.conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/mysql.conf.d; 		find /etc/my.cnf /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/'; 		mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 08 Mar 2023 20:42:43 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 08 Mar 2023 20:42:43 GMT
ENV MYSQL_SHELL_VERSION=8.0.32-1.el7
# Wed, 08 Mar 2023 20:43:07 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-shell-$MYSQL_SHELL_VERSION"; 	yum clean all; 		mysqlsh --version
# Wed, 08 Mar 2023 20:43:08 GMT
VOLUME [/var/lib/mysql]
# Wed, 08 Mar 2023 20:43:08 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 08 Mar 2023 20:43:08 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 08 Mar 2023 20:43:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 08 Mar 2023 20:43:09 GMT
EXPOSE 3306 33060
# Wed, 08 Mar 2023 20:43:09 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:7b659169cb9226d08443358aa4e8147f3144614ac33f7a41217b0cf62a4d3326`  
		Last Modified: Wed, 08 Mar 2023 20:24:41 GMT  
		Size: 50.5 MB (50467964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e47c3f06a3f5705076a7154d7f81aa0bb1433377185e05fa520105f17af2f370`  
		Last Modified: Wed, 08 Mar 2023 20:44:24 GMT  
		Size: 871.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0656a27f56e8064f2d45e3264e37ae491064cf57f2469f9703ffd780771b496`  
		Last Modified: Wed, 08 Mar 2023 20:44:24 GMT  
		Size: 983.7 KB (983707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9f33f34ef42570bb8d9a791d31a6653685baecc2464a6ae65f57d19d2954b5d`  
		Last Modified: Wed, 08 Mar 2023 20:44:23 GMT  
		Size: 4.6 MB (4585631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fc5cbaf8704473ad86bf905f4416c09c189ca133bd57418884189b501f3bbd8`  
		Last Modified: Wed, 08 Mar 2023 20:44:22 GMT  
		Size: 2.7 KB (2654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fb8407bef93fd1fc829cfd13269442f272898b097cfda975b92617eb101bbf8`  
		Last Modified: Wed, 08 Mar 2023 20:44:22 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8be4a2d031b5252b75e271b780be63c907f72b1b15280c13bdbcfe8a4cd653e`  
		Last Modified: Wed, 08 Mar 2023 20:44:24 GMT  
		Size: 25.5 MB (25521558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6cb2bff25e38b09537aa3d38f370061b28bc812ff4ffff86b4b1a435f544173`  
		Last Modified: Wed, 08 Mar 2023 20:44:20 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:056cc4a5c89ae053998222fcd94d51e5c6b3eec297d15e9b7d60b182269b76b8`  
		Last Modified: Wed, 08 Mar 2023 20:44:30 GMT  
		Size: 48.4 MB (48439547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8428969731444b79af296589ae42c54ebcba5e34cb2c12d6cb4e1a5e95f918db`  
		Last Modified: Wed, 08 Mar 2023 20:44:20 GMT  
		Size: 5.4 KB (5393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e55b6e95b292d6e888669bbd77813b1bd08cab1d6b78d1dfe959b959062135ac`  
		Last Modified: Wed, 08 Mar 2023 20:44:20 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7.41`

```console
$ docker pull mysql@sha256:9202fc6bc8fa63615e6bfc0049fc660f712d164220c5c54d86519870c305ea48
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7.41` - linux; amd64

```console
$ docker pull mysql@sha256:c5d8092d5424881f6fb831fefd502de90495c2b62c87d0be67f7b66748906252
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.0 MB (130008096 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0018a8d838923d94318aa8dd3195510226b31540901a6f4c643aacec69f7ab62`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 08 Mar 2023 20:22:54 GMT
ADD file:e205deb729daf99a168c27d3f97cd2b69e736fc9d4bee9ea220ec86921574a0f in / 
# Wed, 08 Mar 2023 20:22:55 GMT
CMD ["/bin/bash"]
# Wed, 08 Mar 2023 20:42:01 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 08 Mar 2023 20:42:02 GMT
ENV GOSU_VERSION=1.16
# Wed, 08 Mar 2023 20:42:04 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 08 Mar 2023 20:42:22 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False oracle-epel-release-el7; 	yum install -y --setopt=skip_missing_names_on_install=False 		bzip2 		gzip 		openssl 		xz 		zstd 	; 	yum clean all
# Wed, 08 Mar 2023 20:42:23 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 08 Mar 2023 20:42:23 GMT
ENV MYSQL_MAJOR=5.7
# Wed, 08 Mar 2023 20:42:23 GMT
ENV MYSQL_VERSION=5.7.41-1.el7
# Wed, 08 Mar 2023 20:42:23 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql5.7-server-minimal]'; 		echo 'name=MySQL 5.7 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-5.7-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 08 Mar 2023 20:42:42 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-community-server-minimal-$MYSQL_VERSION"; 	yum clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	{ echo '!includedir /etc/mysql/mysql.conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/mysql.conf.d; 		find /etc/my.cnf /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/'; 		mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 08 Mar 2023 20:42:43 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 08 Mar 2023 20:42:43 GMT
ENV MYSQL_SHELL_VERSION=8.0.32-1.el7
# Wed, 08 Mar 2023 20:43:07 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-shell-$MYSQL_SHELL_VERSION"; 	yum clean all; 		mysqlsh --version
# Wed, 08 Mar 2023 20:43:08 GMT
VOLUME [/var/lib/mysql]
# Wed, 08 Mar 2023 20:43:08 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 08 Mar 2023 20:43:08 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 08 Mar 2023 20:43:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 08 Mar 2023 20:43:09 GMT
EXPOSE 3306 33060
# Wed, 08 Mar 2023 20:43:09 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:7b659169cb9226d08443358aa4e8147f3144614ac33f7a41217b0cf62a4d3326`  
		Last Modified: Wed, 08 Mar 2023 20:24:41 GMT  
		Size: 50.5 MB (50467964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e47c3f06a3f5705076a7154d7f81aa0bb1433377185e05fa520105f17af2f370`  
		Last Modified: Wed, 08 Mar 2023 20:44:24 GMT  
		Size: 871.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0656a27f56e8064f2d45e3264e37ae491064cf57f2469f9703ffd780771b496`  
		Last Modified: Wed, 08 Mar 2023 20:44:24 GMT  
		Size: 983.7 KB (983707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9f33f34ef42570bb8d9a791d31a6653685baecc2464a6ae65f57d19d2954b5d`  
		Last Modified: Wed, 08 Mar 2023 20:44:23 GMT  
		Size: 4.6 MB (4585631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fc5cbaf8704473ad86bf905f4416c09c189ca133bd57418884189b501f3bbd8`  
		Last Modified: Wed, 08 Mar 2023 20:44:22 GMT  
		Size: 2.7 KB (2654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fb8407bef93fd1fc829cfd13269442f272898b097cfda975b92617eb101bbf8`  
		Last Modified: Wed, 08 Mar 2023 20:44:22 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8be4a2d031b5252b75e271b780be63c907f72b1b15280c13bdbcfe8a4cd653e`  
		Last Modified: Wed, 08 Mar 2023 20:44:24 GMT  
		Size: 25.5 MB (25521558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6cb2bff25e38b09537aa3d38f370061b28bc812ff4ffff86b4b1a435f544173`  
		Last Modified: Wed, 08 Mar 2023 20:44:20 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:056cc4a5c89ae053998222fcd94d51e5c6b3eec297d15e9b7d60b182269b76b8`  
		Last Modified: Wed, 08 Mar 2023 20:44:30 GMT  
		Size: 48.4 MB (48439547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8428969731444b79af296589ae42c54ebcba5e34cb2c12d6cb4e1a5e95f918db`  
		Last Modified: Wed, 08 Mar 2023 20:44:20 GMT  
		Size: 5.4 KB (5393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e55b6e95b292d6e888669bbd77813b1bd08cab1d6b78d1dfe959b959062135ac`  
		Last Modified: Wed, 08 Mar 2023 20:44:20 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7.41-debian`

```console
$ docker pull mysql@sha256:36002a394b549b6d293d7f76de854e69399f0c093e6b1f16baefdafe5ea21ffa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7.41-debian` - linux; amd64

```console
$ docker pull mysql@sha256:ef2398ea6c295c668cf3e969c28ae7088845b07beb07b96792698c3f80c69c8f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **162.7 MB (162694168 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20e50dddd01b351b398beff0bb34172b2edcb046f290ff29ea946b92f7c60cfd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 01 Mar 2023 04:10:22 GMT
ADD file:2254e48bf53907be7a0b1744bc4fcd7805a627672793cf5f86a01ac751a1b24d in / 
# Wed, 01 Mar 2023 04:10:22 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 08:17:40 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 01 Mar 2023 08:17:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 08:17:48 GMT
ENV GOSU_VERSION=1.16
# Wed, 01 Mar 2023 08:17:56 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 01 Mar 2023 08:17:57 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 01 Mar 2023 08:18:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 08:18:04 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Wed, 01 Mar 2023 08:18:04 GMT
ENV MYSQL_MAJOR=5.7
# Wed, 01 Mar 2023 08:18:04 GMT
ENV MYSQL_VERSION=5.7.41-1debian10
# Wed, 01 Mar 2023 08:18:05 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-5.7' > /etc/apt/sources.list.d/mysql.list
# Wed, 01 Mar 2023 08:18:23 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-server="${MYSQL_VERSION}" 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Wed, 01 Mar 2023 08:18:24 GMT
VOLUME [/var/lib/mysql]
# Wed, 01 Mar 2023 08:18:24 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 01 Mar 2023 08:18:25 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 01 Mar 2023 08:18:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Mar 2023 08:18:25 GMT
EXPOSE 3306 33060
# Wed, 01 Mar 2023 08:18:25 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:8fd419aca81cfd3987d61550e700546537628562693bc01acc9f85468f483706`  
		Last Modified: Wed, 01 Mar 2023 04:15:04 GMT  
		Size: 27.1 MB (27139882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d19bdbefd94aa10eb97a97f00a8597a423524a8ee1ac0481ee949550aab103d4`  
		Last Modified: Wed, 01 Mar 2023 08:19:28 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:925e2a505f95d645bf606d89d712e36892cf107ac2734f53a99d73d957828dbd`  
		Last Modified: Wed, 01 Mar 2023 08:19:28 GMT  
		Size: 4.2 MB (4182352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:615b524b079671c0807d23d7b6165c051d3e057cf337dc79c4692eff7f2a1754`  
		Last Modified: Wed, 01 Mar 2023 08:19:27 GMT  
		Size: 1.4 MB (1441782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23269a497e1054aa28f4f235d816862f2a9cff683f19dc248bb57d0c9bdbc544`  
		Last Modified: Wed, 01 Mar 2023 08:19:27 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:034fd6f00cfd596d0fc2e2a26ac97b0a306501ee99bff82b16a26dcf1e06b21b`  
		Last Modified: Wed, 01 Mar 2023 08:19:29 GMT  
		Size: 14.1 MB (14087009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a1c4f6ce4b763cc7098b8bb50e2063925a87b37b938873fb8721773fdc77891`  
		Last Modified: Wed, 01 Mar 2023 08:19:25 GMT  
		Size: 2.5 KB (2548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a74551e5bdd8aa6103cb0145f16fd744127eb8e2076d188e3bdae8e304ffb0b`  
		Last Modified: Wed, 01 Mar 2023 08:19:25 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5a3a8bb0579b93926aafefcf6a0f480e7eef4bdd55faebd8c23c3dc84748743`  
		Last Modified: Wed, 01 Mar 2023 08:19:39 GMT  
		Size: 115.8 MB (115832956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cfbfd35c59124cb5b9f9562b11ab90a3f11e8634febc4bf66e0d75231f98c5b`  
		Last Modified: Wed, 01 Mar 2023 08:19:25 GMT  
		Size: 5.4 KB (5388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a9277a314e7f20aba5d30ad70cfb9c6fc26283bc49c06199e1285d04a31b4cb`  
		Last Modified: Wed, 01 Mar 2023 08:19:25 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7.41-oracle`

```console
$ docker pull mysql@sha256:9202fc6bc8fa63615e6bfc0049fc660f712d164220c5c54d86519870c305ea48
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7.41-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:c5d8092d5424881f6fb831fefd502de90495c2b62c87d0be67f7b66748906252
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.0 MB (130008096 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0018a8d838923d94318aa8dd3195510226b31540901a6f4c643aacec69f7ab62`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 08 Mar 2023 20:22:54 GMT
ADD file:e205deb729daf99a168c27d3f97cd2b69e736fc9d4bee9ea220ec86921574a0f in / 
# Wed, 08 Mar 2023 20:22:55 GMT
CMD ["/bin/bash"]
# Wed, 08 Mar 2023 20:42:01 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 08 Mar 2023 20:42:02 GMT
ENV GOSU_VERSION=1.16
# Wed, 08 Mar 2023 20:42:04 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 08 Mar 2023 20:42:22 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False oracle-epel-release-el7; 	yum install -y --setopt=skip_missing_names_on_install=False 		bzip2 		gzip 		openssl 		xz 		zstd 	; 	yum clean all
# Wed, 08 Mar 2023 20:42:23 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 08 Mar 2023 20:42:23 GMT
ENV MYSQL_MAJOR=5.7
# Wed, 08 Mar 2023 20:42:23 GMT
ENV MYSQL_VERSION=5.7.41-1.el7
# Wed, 08 Mar 2023 20:42:23 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql5.7-server-minimal]'; 		echo 'name=MySQL 5.7 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-5.7-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 08 Mar 2023 20:42:42 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-community-server-minimal-$MYSQL_VERSION"; 	yum clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	{ echo '!includedir /etc/mysql/mysql.conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/mysql.conf.d; 		find /etc/my.cnf /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/'; 		mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 08 Mar 2023 20:42:43 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 08 Mar 2023 20:42:43 GMT
ENV MYSQL_SHELL_VERSION=8.0.32-1.el7
# Wed, 08 Mar 2023 20:43:07 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-shell-$MYSQL_SHELL_VERSION"; 	yum clean all; 		mysqlsh --version
# Wed, 08 Mar 2023 20:43:08 GMT
VOLUME [/var/lib/mysql]
# Wed, 08 Mar 2023 20:43:08 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 08 Mar 2023 20:43:08 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 08 Mar 2023 20:43:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 08 Mar 2023 20:43:09 GMT
EXPOSE 3306 33060
# Wed, 08 Mar 2023 20:43:09 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:7b659169cb9226d08443358aa4e8147f3144614ac33f7a41217b0cf62a4d3326`  
		Last Modified: Wed, 08 Mar 2023 20:24:41 GMT  
		Size: 50.5 MB (50467964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e47c3f06a3f5705076a7154d7f81aa0bb1433377185e05fa520105f17af2f370`  
		Last Modified: Wed, 08 Mar 2023 20:44:24 GMT  
		Size: 871.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0656a27f56e8064f2d45e3264e37ae491064cf57f2469f9703ffd780771b496`  
		Last Modified: Wed, 08 Mar 2023 20:44:24 GMT  
		Size: 983.7 KB (983707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9f33f34ef42570bb8d9a791d31a6653685baecc2464a6ae65f57d19d2954b5d`  
		Last Modified: Wed, 08 Mar 2023 20:44:23 GMT  
		Size: 4.6 MB (4585631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fc5cbaf8704473ad86bf905f4416c09c189ca133bd57418884189b501f3bbd8`  
		Last Modified: Wed, 08 Mar 2023 20:44:22 GMT  
		Size: 2.7 KB (2654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fb8407bef93fd1fc829cfd13269442f272898b097cfda975b92617eb101bbf8`  
		Last Modified: Wed, 08 Mar 2023 20:44:22 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8be4a2d031b5252b75e271b780be63c907f72b1b15280c13bdbcfe8a4cd653e`  
		Last Modified: Wed, 08 Mar 2023 20:44:24 GMT  
		Size: 25.5 MB (25521558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6cb2bff25e38b09537aa3d38f370061b28bc812ff4ffff86b4b1a435f544173`  
		Last Modified: Wed, 08 Mar 2023 20:44:20 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:056cc4a5c89ae053998222fcd94d51e5c6b3eec297d15e9b7d60b182269b76b8`  
		Last Modified: Wed, 08 Mar 2023 20:44:30 GMT  
		Size: 48.4 MB (48439547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8428969731444b79af296589ae42c54ebcba5e34cb2c12d6cb4e1a5e95f918db`  
		Last Modified: Wed, 08 Mar 2023 20:44:20 GMT  
		Size: 5.4 KB (5393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e55b6e95b292d6e888669bbd77813b1bd08cab1d6b78d1dfe959b959062135ac`  
		Last Modified: Wed, 08 Mar 2023 20:44:20 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8`

```console
$ docker pull mysql@sha256:2596158f73606ba571e1af29a9c32bec5dc021a2495e4a70d194a9b49664f4d9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8` - linux; amd64

```console
$ docker pull mysql@sha256:79866c649987750de41276796f7b29a54be80834dd2bc20e435dc9554a33945f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.6 MB (156597480 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4073e6a6f54214da05256022b9a86e2f3f480703d1fc457a7085107c854e5ce3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 08 Mar 2023 20:22:31 GMT
ADD file:eca2b657866c594c67fc9041ad2a4a309e62fc8338add46c3917517649f748b2 in / 
# Wed, 08 Mar 2023 20:22:32 GMT
CMD ["/bin/bash"]
# Wed, 08 Mar 2023 20:40:06 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 08 Mar 2023 20:40:06 GMT
ENV GOSU_VERSION=1.16
# Wed, 08 Mar 2023 20:40:10 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 08 Mar 2023 20:40:35 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Wed, 08 Mar 2023 20:40:36 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 08 Mar 2023 20:40:36 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 08 Mar 2023 20:40:36 GMT
ENV MYSQL_VERSION=8.0.32-1.el8
# Wed, 08 Mar 2023 20:40:37 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 08 Mar 2023 20:41:09 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 08 Mar 2023 20:41:10 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 08 Mar 2023 20:41:10 GMT
ENV MYSQL_SHELL_VERSION=8.0.32-1.el8
# Wed, 08 Mar 2023 20:41:46 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Wed, 08 Mar 2023 20:41:47 GMT
VOLUME [/var/lib/mysql]
# Wed, 08 Mar 2023 20:41:47 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 08 Mar 2023 20:41:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 08 Mar 2023 20:41:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 08 Mar 2023 20:41:48 GMT
EXPOSE 3306 33060
# Wed, 08 Mar 2023 20:41:48 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:767a87c583278931a33db59dc8586fdcfa03c53a801cce573f0e861c31ec4c89`  
		Last Modified: Wed, 08 Mar 2023 20:24:06 GMT  
		Size: 44.6 MB (44557814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbd6d17e71a0fa12983f197a9f8c76b09ba416527debf78c14ac504317aec0f9`  
		Last Modified: Wed, 08 Mar 2023 20:43:49 GMT  
		Size: 887.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b17ad003fbc8375915bdad1cb4569356ce65dd16d5456337326e085572bb7ba`  
		Last Modified: Wed, 08 Mar 2023 20:43:49 GMT  
		Size: 982.8 KB (982819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:410b54c19b6bfa2624cb49d3ea768c0a46dc4719b1aa0a9f54f28024246f7c72`  
		Last Modified: Wed, 08 Mar 2023 20:43:48 GMT  
		Size: 4.6 MB (4624011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6192cec941545dc76c7a164680b55bb3ffe8271191bb2fc09d1bb18a64df4d3`  
		Last Modified: Wed, 08 Mar 2023 20:43:47 GMT  
		Size: 2.6 KB (2631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7be351756ff4dda5f0a2744d5bbd15c4133d6fe4aca456ce732fe4d870ebb06`  
		Last Modified: Wed, 08 Mar 2023 20:43:47 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae2d1ab519ee3bd717c6c2012e651f9511d04720f77724af8399f8d19c78c8a2`  
		Last Modified: Wed, 08 Mar 2023 20:43:53 GMT  
		Size: 56.2 MB (56233013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:119cfaa7dea024112488b45621d53ecf602293f6bdbcc3796090251911979f47`  
		Last Modified: Wed, 08 Mar 2023 20:43:45 GMT  
		Size: 317.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7176b3cc6ba140af2b8354ea0889eff5ccf7d9dadc9110d3b8d0f69c126c29d8`  
		Last Modified: Wed, 08 Mar 2023 20:43:55 GMT  
		Size: 50.2 MB (50190140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eb39e909e2beef35e5c3ea7d67c45c519eb06c9685846dd37f514ef68d18149`  
		Last Modified: Wed, 08 Mar 2023 20:43:45 GMT  
		Size: 5.4 KB (5393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e935886e1025cc7de30d6afcf9e7612a0dae12d42294969399544173a3bbfde3`  
		Last Modified: Wed, 08 Mar 2023 20:43:45 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:d1887ec2b0018304daad8cdc1506d718ed0f04bed93ac87372355c12bba6bc08
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.4 MB (155433895 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7c54c29e20dccc1aefb936c8eba8bb8b98b87a4921102aba87fde2df5810af9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 08 Mar 2023 21:02:19 GMT
ADD file:18f4bd510f88f32e538884e4e633449c2c8dbf8a5f88b6b6b165ab05872d9507 in / 
# Wed, 08 Mar 2023 21:02:19 GMT
CMD ["/bin/bash"]
# Wed, 08 Mar 2023 21:25:35 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 08 Mar 2023 21:25:35 GMT
ENV GOSU_VERSION=1.16
# Wed, 08 Mar 2023 21:25:39 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 08 Mar 2023 21:26:01 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Wed, 08 Mar 2023 21:26:03 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 08 Mar 2023 21:26:03 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 08 Mar 2023 21:26:03 GMT
ENV MYSQL_VERSION=8.0.32-1.el8
# Wed, 08 Mar 2023 21:26:03 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 08 Mar 2023 21:26:29 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 08 Mar 2023 21:26:31 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 08 Mar 2023 21:26:31 GMT
ENV MYSQL_SHELL_VERSION=8.0.32-1.el8
# Wed, 08 Mar 2023 21:27:03 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Wed, 08 Mar 2023 21:27:05 GMT
VOLUME [/var/lib/mysql]
# Wed, 08 Mar 2023 21:27:05 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 08 Mar 2023 21:27:05 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 08 Mar 2023 21:27:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 08 Mar 2023 21:27:05 GMT
EXPOSE 3306 33060
# Wed, 08 Mar 2023 21:27:06 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:8ff0c9d62930fe3f55e00ba3be2db6be3643b07da9804d1c9b83b0d3181f0df5`  
		Last Modified: Wed, 08 Mar 2023 21:03:40 GMT  
		Size: 43.5 MB (43456139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c7ab176cd9d87a44c6b82369dab38d2a8a8f75036009413cc37399ed49b38e9`  
		Last Modified: Wed, 08 Mar 2023 21:27:28 GMT  
		Size: 886.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f6283edca869f9d898e92d4e5720e7ed8d16433dc7263b4a351b5c67199082c`  
		Last Modified: Wed, 08 Mar 2023 21:27:28 GMT  
		Size: 913.0 KB (912997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74489f3832cb81c43de395aa7a1345a5e233361ad8e2e460e3e9cf80f124329f`  
		Last Modified: Wed, 08 Mar 2023 21:27:26 GMT  
		Size: 4.5 MB (4456734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68fdb433cd6ed223c0ca86d0aca93e05f0df1a03588b2e63dbcdd7f836f6e785`  
		Last Modified: Wed, 08 Mar 2023 21:27:26 GMT  
		Size: 2.6 KB (2629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed704471ee1020a0a1808d0d8117ddeeea6154e24d50690959921a413029a880`  
		Last Modified: Wed, 08 Mar 2023 21:27:26 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8017dfacae02bc956ca22b2e23db59dc69f2e3a2948d497e3cb0a9429ba5342e`  
		Last Modified: Wed, 08 Mar 2023 21:27:30 GMT  
		Size: 55.6 MB (55615967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c01cb78ffdd6ef9f062f5d2a80e243e249de2447fd68e17c17b7a2938ed5cff`  
		Last Modified: Wed, 08 Mar 2023 21:27:24 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa238b7fd3ad0bf546c26574e4edcd1761584f55d8b338a7b0330399baae3e49`  
		Last Modified: Wed, 08 Mar 2023 21:27:31 GMT  
		Size: 51.0 MB (50982384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a86d0b8c1ccc4f969ad0e7b9fa57a409e360db176437a087a5fd9406b081691`  
		Last Modified: Wed, 08 Mar 2023 21:27:24 GMT  
		Size: 5.4 KB (5388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:326b54668f8b18657ed13771324644998d14801db082e346aad6c8dd67aecb51`  
		Last Modified: Wed, 08 Mar 2023 21:27:24 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8-debian`

```console
$ docker pull mysql@sha256:c26ffcfefadf3698514de6e8e8b3566cd0da5b8a9ee3543ea0eb44bc5faab6dc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:8-debian` - linux; amd64

```console
$ docker pull mysql@sha256:2f7872dbcb701e16397e23e368148ee9411027cd4baf5905d0622ccccc35092e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **177.8 MB (177766717 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f88e52842dfbc5faff99e03317eb17892293cd424cd745e74ec04408ba255207`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 01 Mar 2023 04:09:58 GMT
ADD file:493a5b0c8d2d63a1343258b3f9aa5fcd59a93f44fe26ad9e56b094c3a08fd3be in / 
# Wed, 01 Mar 2023 04:09:59 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 08:16:50 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 01 Mar 2023 08:16:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 08:16:56 GMT
ENV GOSU_VERSION=1.16
# Wed, 01 Mar 2023 08:17:04 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 01 Mar 2023 08:17:05 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 01 Mar 2023 08:17:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 08:17:11 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Wed, 01 Mar 2023 08:17:12 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 01 Mar 2023 08:17:12 GMT
ENV MYSQL_VERSION=8.0.32-1debian11
# Wed, 01 Mar 2023 08:17:12 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ bullseye mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Wed, 01 Mar 2023 08:17:27 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Wed, 01 Mar 2023 08:17:28 GMT
VOLUME [/var/lib/mysql]
# Wed, 01 Mar 2023 08:17:28 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Wed, 01 Mar 2023 08:17:28 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 01 Mar 2023 08:17:29 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 01 Mar 2023 08:17:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Mar 2023 08:17:29 GMT
EXPOSE 3306 33060
# Wed, 01 Mar 2023 08:17:29 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:3f9582a2cbe7197f39185419c0ced2c986389f8fc6aa805e1f5c090eea6511e0`  
		Last Modified: Wed, 01 Mar 2023 04:14:23 GMT  
		Size: 31.4 MB (31411403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:760f99c7c3059a32499d51cb02152df032fc466298a3e2b7e600029b9b91f4ea`  
		Last Modified: Wed, 01 Mar 2023 08:18:54 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d20338c318a65cc44a3e0a1a60cb9c690d286ff757ea0b3a976bf24748a0316`  
		Last Modified: Wed, 01 Mar 2023 08:18:54 GMT  
		Size: 4.4 MB (4414965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e92be7428ec909fce6a3b308505a95430380d7b319e454a1eb04c11f33522f7`  
		Last Modified: Wed, 01 Mar 2023 08:18:52 GMT  
		Size: 1.5 MB (1471440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1c491527f8245e4dc5378618790c15c6885747848d85b17bcb6dce84ad2ff88`  
		Last Modified: Wed, 01 Mar 2023 08:18:51 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8aab5d3f904fbf665f9b72bfad9092bce3e58555608293d61f421931eaf99f80`  
		Last Modified: Wed, 01 Mar 2023 08:18:54 GMT  
		Size: 12.7 MB (12661962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0764a75d4948f4bc90025d5a92b44e3ff0372e8798b456860ee310dd9bb3e52f`  
		Last Modified: Wed, 01 Mar 2023 08:18:51 GMT  
		Size: 2.5 KB (2549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abceaa621503b0635e2b0e9740dfe37f20b0c42d1d17615caebdc44f5f05949f`  
		Last Modified: Wed, 01 Mar 2023 08:18:50 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09a8f23f9143940d284a3ff2c1767c607db5bfe4652eb720a811f902a4188707`  
		Last Modified: Wed, 01 Mar 2023 08:19:09 GMT  
		Size: 127.8 MB (127795909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfad9bee7b38020e4c875fff67ed05f30ab2e771c0db576fe03213199b20dec0`  
		Last Modified: Wed, 01 Mar 2023 08:18:50 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fdbfd558513023768b43219f0840d9f390b92f42e0249e9051a7dd596965f7b`  
		Last Modified: Wed, 01 Mar 2023 08:18:50 GMT  
		Size: 5.4 KB (5389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d6b54fce3b52f5381a599e59836f8faf08f2c8077888bdc30eb2b217a96dbbe`  
		Last Modified: Wed, 01 Mar 2023 08:18:50 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8-oracle`

```console
$ docker pull mysql@sha256:2596158f73606ba571e1af29a9c32bec5dc021a2495e4a70d194a9b49664f4d9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:79866c649987750de41276796f7b29a54be80834dd2bc20e435dc9554a33945f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.6 MB (156597480 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4073e6a6f54214da05256022b9a86e2f3f480703d1fc457a7085107c854e5ce3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 08 Mar 2023 20:22:31 GMT
ADD file:eca2b657866c594c67fc9041ad2a4a309e62fc8338add46c3917517649f748b2 in / 
# Wed, 08 Mar 2023 20:22:32 GMT
CMD ["/bin/bash"]
# Wed, 08 Mar 2023 20:40:06 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 08 Mar 2023 20:40:06 GMT
ENV GOSU_VERSION=1.16
# Wed, 08 Mar 2023 20:40:10 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 08 Mar 2023 20:40:35 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Wed, 08 Mar 2023 20:40:36 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 08 Mar 2023 20:40:36 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 08 Mar 2023 20:40:36 GMT
ENV MYSQL_VERSION=8.0.32-1.el8
# Wed, 08 Mar 2023 20:40:37 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 08 Mar 2023 20:41:09 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 08 Mar 2023 20:41:10 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 08 Mar 2023 20:41:10 GMT
ENV MYSQL_SHELL_VERSION=8.0.32-1.el8
# Wed, 08 Mar 2023 20:41:46 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Wed, 08 Mar 2023 20:41:47 GMT
VOLUME [/var/lib/mysql]
# Wed, 08 Mar 2023 20:41:47 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 08 Mar 2023 20:41:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 08 Mar 2023 20:41:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 08 Mar 2023 20:41:48 GMT
EXPOSE 3306 33060
# Wed, 08 Mar 2023 20:41:48 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:767a87c583278931a33db59dc8586fdcfa03c53a801cce573f0e861c31ec4c89`  
		Last Modified: Wed, 08 Mar 2023 20:24:06 GMT  
		Size: 44.6 MB (44557814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbd6d17e71a0fa12983f197a9f8c76b09ba416527debf78c14ac504317aec0f9`  
		Last Modified: Wed, 08 Mar 2023 20:43:49 GMT  
		Size: 887.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b17ad003fbc8375915bdad1cb4569356ce65dd16d5456337326e085572bb7ba`  
		Last Modified: Wed, 08 Mar 2023 20:43:49 GMT  
		Size: 982.8 KB (982819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:410b54c19b6bfa2624cb49d3ea768c0a46dc4719b1aa0a9f54f28024246f7c72`  
		Last Modified: Wed, 08 Mar 2023 20:43:48 GMT  
		Size: 4.6 MB (4624011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6192cec941545dc76c7a164680b55bb3ffe8271191bb2fc09d1bb18a64df4d3`  
		Last Modified: Wed, 08 Mar 2023 20:43:47 GMT  
		Size: 2.6 KB (2631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7be351756ff4dda5f0a2744d5bbd15c4133d6fe4aca456ce732fe4d870ebb06`  
		Last Modified: Wed, 08 Mar 2023 20:43:47 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae2d1ab519ee3bd717c6c2012e651f9511d04720f77724af8399f8d19c78c8a2`  
		Last Modified: Wed, 08 Mar 2023 20:43:53 GMT  
		Size: 56.2 MB (56233013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:119cfaa7dea024112488b45621d53ecf602293f6bdbcc3796090251911979f47`  
		Last Modified: Wed, 08 Mar 2023 20:43:45 GMT  
		Size: 317.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7176b3cc6ba140af2b8354ea0889eff5ccf7d9dadc9110d3b8d0f69c126c29d8`  
		Last Modified: Wed, 08 Mar 2023 20:43:55 GMT  
		Size: 50.2 MB (50190140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eb39e909e2beef35e5c3ea7d67c45c519eb06c9685846dd37f514ef68d18149`  
		Last Modified: Wed, 08 Mar 2023 20:43:45 GMT  
		Size: 5.4 KB (5393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e935886e1025cc7de30d6afcf9e7612a0dae12d42294969399544173a3bbfde3`  
		Last Modified: Wed, 08 Mar 2023 20:43:45 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8-oracle` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:d1887ec2b0018304daad8cdc1506d718ed0f04bed93ac87372355c12bba6bc08
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.4 MB (155433895 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7c54c29e20dccc1aefb936c8eba8bb8b98b87a4921102aba87fde2df5810af9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 08 Mar 2023 21:02:19 GMT
ADD file:18f4bd510f88f32e538884e4e633449c2c8dbf8a5f88b6b6b165ab05872d9507 in / 
# Wed, 08 Mar 2023 21:02:19 GMT
CMD ["/bin/bash"]
# Wed, 08 Mar 2023 21:25:35 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 08 Mar 2023 21:25:35 GMT
ENV GOSU_VERSION=1.16
# Wed, 08 Mar 2023 21:25:39 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 08 Mar 2023 21:26:01 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Wed, 08 Mar 2023 21:26:03 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 08 Mar 2023 21:26:03 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 08 Mar 2023 21:26:03 GMT
ENV MYSQL_VERSION=8.0.32-1.el8
# Wed, 08 Mar 2023 21:26:03 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 08 Mar 2023 21:26:29 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 08 Mar 2023 21:26:31 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 08 Mar 2023 21:26:31 GMT
ENV MYSQL_SHELL_VERSION=8.0.32-1.el8
# Wed, 08 Mar 2023 21:27:03 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Wed, 08 Mar 2023 21:27:05 GMT
VOLUME [/var/lib/mysql]
# Wed, 08 Mar 2023 21:27:05 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 08 Mar 2023 21:27:05 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 08 Mar 2023 21:27:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 08 Mar 2023 21:27:05 GMT
EXPOSE 3306 33060
# Wed, 08 Mar 2023 21:27:06 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:8ff0c9d62930fe3f55e00ba3be2db6be3643b07da9804d1c9b83b0d3181f0df5`  
		Last Modified: Wed, 08 Mar 2023 21:03:40 GMT  
		Size: 43.5 MB (43456139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c7ab176cd9d87a44c6b82369dab38d2a8a8f75036009413cc37399ed49b38e9`  
		Last Modified: Wed, 08 Mar 2023 21:27:28 GMT  
		Size: 886.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f6283edca869f9d898e92d4e5720e7ed8d16433dc7263b4a351b5c67199082c`  
		Last Modified: Wed, 08 Mar 2023 21:27:28 GMT  
		Size: 913.0 KB (912997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74489f3832cb81c43de395aa7a1345a5e233361ad8e2e460e3e9cf80f124329f`  
		Last Modified: Wed, 08 Mar 2023 21:27:26 GMT  
		Size: 4.5 MB (4456734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68fdb433cd6ed223c0ca86d0aca93e05f0df1a03588b2e63dbcdd7f836f6e785`  
		Last Modified: Wed, 08 Mar 2023 21:27:26 GMT  
		Size: 2.6 KB (2629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed704471ee1020a0a1808d0d8117ddeeea6154e24d50690959921a413029a880`  
		Last Modified: Wed, 08 Mar 2023 21:27:26 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8017dfacae02bc956ca22b2e23db59dc69f2e3a2948d497e3cb0a9429ba5342e`  
		Last Modified: Wed, 08 Mar 2023 21:27:30 GMT  
		Size: 55.6 MB (55615967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c01cb78ffdd6ef9f062f5d2a80e243e249de2447fd68e17c17b7a2938ed5cff`  
		Last Modified: Wed, 08 Mar 2023 21:27:24 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa238b7fd3ad0bf546c26574e4edcd1761584f55d8b338a7b0330399baae3e49`  
		Last Modified: Wed, 08 Mar 2023 21:27:31 GMT  
		Size: 51.0 MB (50982384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a86d0b8c1ccc4f969ad0e7b9fa57a409e360db176437a087a5fd9406b081691`  
		Last Modified: Wed, 08 Mar 2023 21:27:24 GMT  
		Size: 5.4 KB (5388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:326b54668f8b18657ed13771324644998d14801db082e346aad6c8dd67aecb51`  
		Last Modified: Wed, 08 Mar 2023 21:27:24 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0`

```console
$ docker pull mysql@sha256:2596158f73606ba571e1af29a9c32bec5dc021a2495e4a70d194a9b49664f4d9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8.0` - linux; amd64

```console
$ docker pull mysql@sha256:79866c649987750de41276796f7b29a54be80834dd2bc20e435dc9554a33945f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.6 MB (156597480 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4073e6a6f54214da05256022b9a86e2f3f480703d1fc457a7085107c854e5ce3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 08 Mar 2023 20:22:31 GMT
ADD file:eca2b657866c594c67fc9041ad2a4a309e62fc8338add46c3917517649f748b2 in / 
# Wed, 08 Mar 2023 20:22:32 GMT
CMD ["/bin/bash"]
# Wed, 08 Mar 2023 20:40:06 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 08 Mar 2023 20:40:06 GMT
ENV GOSU_VERSION=1.16
# Wed, 08 Mar 2023 20:40:10 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 08 Mar 2023 20:40:35 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Wed, 08 Mar 2023 20:40:36 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 08 Mar 2023 20:40:36 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 08 Mar 2023 20:40:36 GMT
ENV MYSQL_VERSION=8.0.32-1.el8
# Wed, 08 Mar 2023 20:40:37 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 08 Mar 2023 20:41:09 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 08 Mar 2023 20:41:10 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 08 Mar 2023 20:41:10 GMT
ENV MYSQL_SHELL_VERSION=8.0.32-1.el8
# Wed, 08 Mar 2023 20:41:46 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Wed, 08 Mar 2023 20:41:47 GMT
VOLUME [/var/lib/mysql]
# Wed, 08 Mar 2023 20:41:47 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 08 Mar 2023 20:41:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 08 Mar 2023 20:41:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 08 Mar 2023 20:41:48 GMT
EXPOSE 3306 33060
# Wed, 08 Mar 2023 20:41:48 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:767a87c583278931a33db59dc8586fdcfa03c53a801cce573f0e861c31ec4c89`  
		Last Modified: Wed, 08 Mar 2023 20:24:06 GMT  
		Size: 44.6 MB (44557814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbd6d17e71a0fa12983f197a9f8c76b09ba416527debf78c14ac504317aec0f9`  
		Last Modified: Wed, 08 Mar 2023 20:43:49 GMT  
		Size: 887.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b17ad003fbc8375915bdad1cb4569356ce65dd16d5456337326e085572bb7ba`  
		Last Modified: Wed, 08 Mar 2023 20:43:49 GMT  
		Size: 982.8 KB (982819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:410b54c19b6bfa2624cb49d3ea768c0a46dc4719b1aa0a9f54f28024246f7c72`  
		Last Modified: Wed, 08 Mar 2023 20:43:48 GMT  
		Size: 4.6 MB (4624011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6192cec941545dc76c7a164680b55bb3ffe8271191bb2fc09d1bb18a64df4d3`  
		Last Modified: Wed, 08 Mar 2023 20:43:47 GMT  
		Size: 2.6 KB (2631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7be351756ff4dda5f0a2744d5bbd15c4133d6fe4aca456ce732fe4d870ebb06`  
		Last Modified: Wed, 08 Mar 2023 20:43:47 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae2d1ab519ee3bd717c6c2012e651f9511d04720f77724af8399f8d19c78c8a2`  
		Last Modified: Wed, 08 Mar 2023 20:43:53 GMT  
		Size: 56.2 MB (56233013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:119cfaa7dea024112488b45621d53ecf602293f6bdbcc3796090251911979f47`  
		Last Modified: Wed, 08 Mar 2023 20:43:45 GMT  
		Size: 317.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7176b3cc6ba140af2b8354ea0889eff5ccf7d9dadc9110d3b8d0f69c126c29d8`  
		Last Modified: Wed, 08 Mar 2023 20:43:55 GMT  
		Size: 50.2 MB (50190140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eb39e909e2beef35e5c3ea7d67c45c519eb06c9685846dd37f514ef68d18149`  
		Last Modified: Wed, 08 Mar 2023 20:43:45 GMT  
		Size: 5.4 KB (5393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e935886e1025cc7de30d6afcf9e7612a0dae12d42294969399544173a3bbfde3`  
		Last Modified: Wed, 08 Mar 2023 20:43:45 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8.0` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:d1887ec2b0018304daad8cdc1506d718ed0f04bed93ac87372355c12bba6bc08
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.4 MB (155433895 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7c54c29e20dccc1aefb936c8eba8bb8b98b87a4921102aba87fde2df5810af9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 08 Mar 2023 21:02:19 GMT
ADD file:18f4bd510f88f32e538884e4e633449c2c8dbf8a5f88b6b6b165ab05872d9507 in / 
# Wed, 08 Mar 2023 21:02:19 GMT
CMD ["/bin/bash"]
# Wed, 08 Mar 2023 21:25:35 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 08 Mar 2023 21:25:35 GMT
ENV GOSU_VERSION=1.16
# Wed, 08 Mar 2023 21:25:39 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 08 Mar 2023 21:26:01 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Wed, 08 Mar 2023 21:26:03 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 08 Mar 2023 21:26:03 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 08 Mar 2023 21:26:03 GMT
ENV MYSQL_VERSION=8.0.32-1.el8
# Wed, 08 Mar 2023 21:26:03 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 08 Mar 2023 21:26:29 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 08 Mar 2023 21:26:31 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 08 Mar 2023 21:26:31 GMT
ENV MYSQL_SHELL_VERSION=8.0.32-1.el8
# Wed, 08 Mar 2023 21:27:03 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Wed, 08 Mar 2023 21:27:05 GMT
VOLUME [/var/lib/mysql]
# Wed, 08 Mar 2023 21:27:05 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 08 Mar 2023 21:27:05 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 08 Mar 2023 21:27:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 08 Mar 2023 21:27:05 GMT
EXPOSE 3306 33060
# Wed, 08 Mar 2023 21:27:06 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:8ff0c9d62930fe3f55e00ba3be2db6be3643b07da9804d1c9b83b0d3181f0df5`  
		Last Modified: Wed, 08 Mar 2023 21:03:40 GMT  
		Size: 43.5 MB (43456139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c7ab176cd9d87a44c6b82369dab38d2a8a8f75036009413cc37399ed49b38e9`  
		Last Modified: Wed, 08 Mar 2023 21:27:28 GMT  
		Size: 886.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f6283edca869f9d898e92d4e5720e7ed8d16433dc7263b4a351b5c67199082c`  
		Last Modified: Wed, 08 Mar 2023 21:27:28 GMT  
		Size: 913.0 KB (912997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74489f3832cb81c43de395aa7a1345a5e233361ad8e2e460e3e9cf80f124329f`  
		Last Modified: Wed, 08 Mar 2023 21:27:26 GMT  
		Size: 4.5 MB (4456734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68fdb433cd6ed223c0ca86d0aca93e05f0df1a03588b2e63dbcdd7f836f6e785`  
		Last Modified: Wed, 08 Mar 2023 21:27:26 GMT  
		Size: 2.6 KB (2629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed704471ee1020a0a1808d0d8117ddeeea6154e24d50690959921a413029a880`  
		Last Modified: Wed, 08 Mar 2023 21:27:26 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8017dfacae02bc956ca22b2e23db59dc69f2e3a2948d497e3cb0a9429ba5342e`  
		Last Modified: Wed, 08 Mar 2023 21:27:30 GMT  
		Size: 55.6 MB (55615967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c01cb78ffdd6ef9f062f5d2a80e243e249de2447fd68e17c17b7a2938ed5cff`  
		Last Modified: Wed, 08 Mar 2023 21:27:24 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa238b7fd3ad0bf546c26574e4edcd1761584f55d8b338a7b0330399baae3e49`  
		Last Modified: Wed, 08 Mar 2023 21:27:31 GMT  
		Size: 51.0 MB (50982384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a86d0b8c1ccc4f969ad0e7b9fa57a409e360db176437a087a5fd9406b081691`  
		Last Modified: Wed, 08 Mar 2023 21:27:24 GMT  
		Size: 5.4 KB (5388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:326b54668f8b18657ed13771324644998d14801db082e346aad6c8dd67aecb51`  
		Last Modified: Wed, 08 Mar 2023 21:27:24 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0-debian`

```console
$ docker pull mysql@sha256:c26ffcfefadf3698514de6e8e8b3566cd0da5b8a9ee3543ea0eb44bc5faab6dc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:8.0-debian` - linux; amd64

```console
$ docker pull mysql@sha256:2f7872dbcb701e16397e23e368148ee9411027cd4baf5905d0622ccccc35092e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **177.8 MB (177766717 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f88e52842dfbc5faff99e03317eb17892293cd424cd745e74ec04408ba255207`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 01 Mar 2023 04:09:58 GMT
ADD file:493a5b0c8d2d63a1343258b3f9aa5fcd59a93f44fe26ad9e56b094c3a08fd3be in / 
# Wed, 01 Mar 2023 04:09:59 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 08:16:50 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 01 Mar 2023 08:16:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 08:16:56 GMT
ENV GOSU_VERSION=1.16
# Wed, 01 Mar 2023 08:17:04 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 01 Mar 2023 08:17:05 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 01 Mar 2023 08:17:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 08:17:11 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Wed, 01 Mar 2023 08:17:12 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 01 Mar 2023 08:17:12 GMT
ENV MYSQL_VERSION=8.0.32-1debian11
# Wed, 01 Mar 2023 08:17:12 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ bullseye mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Wed, 01 Mar 2023 08:17:27 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Wed, 01 Mar 2023 08:17:28 GMT
VOLUME [/var/lib/mysql]
# Wed, 01 Mar 2023 08:17:28 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Wed, 01 Mar 2023 08:17:28 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 01 Mar 2023 08:17:29 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 01 Mar 2023 08:17:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Mar 2023 08:17:29 GMT
EXPOSE 3306 33060
# Wed, 01 Mar 2023 08:17:29 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:3f9582a2cbe7197f39185419c0ced2c986389f8fc6aa805e1f5c090eea6511e0`  
		Last Modified: Wed, 01 Mar 2023 04:14:23 GMT  
		Size: 31.4 MB (31411403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:760f99c7c3059a32499d51cb02152df032fc466298a3e2b7e600029b9b91f4ea`  
		Last Modified: Wed, 01 Mar 2023 08:18:54 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d20338c318a65cc44a3e0a1a60cb9c690d286ff757ea0b3a976bf24748a0316`  
		Last Modified: Wed, 01 Mar 2023 08:18:54 GMT  
		Size: 4.4 MB (4414965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e92be7428ec909fce6a3b308505a95430380d7b319e454a1eb04c11f33522f7`  
		Last Modified: Wed, 01 Mar 2023 08:18:52 GMT  
		Size: 1.5 MB (1471440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1c491527f8245e4dc5378618790c15c6885747848d85b17bcb6dce84ad2ff88`  
		Last Modified: Wed, 01 Mar 2023 08:18:51 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8aab5d3f904fbf665f9b72bfad9092bce3e58555608293d61f421931eaf99f80`  
		Last Modified: Wed, 01 Mar 2023 08:18:54 GMT  
		Size: 12.7 MB (12661962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0764a75d4948f4bc90025d5a92b44e3ff0372e8798b456860ee310dd9bb3e52f`  
		Last Modified: Wed, 01 Mar 2023 08:18:51 GMT  
		Size: 2.5 KB (2549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abceaa621503b0635e2b0e9740dfe37f20b0c42d1d17615caebdc44f5f05949f`  
		Last Modified: Wed, 01 Mar 2023 08:18:50 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09a8f23f9143940d284a3ff2c1767c607db5bfe4652eb720a811f902a4188707`  
		Last Modified: Wed, 01 Mar 2023 08:19:09 GMT  
		Size: 127.8 MB (127795909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfad9bee7b38020e4c875fff67ed05f30ab2e771c0db576fe03213199b20dec0`  
		Last Modified: Wed, 01 Mar 2023 08:18:50 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fdbfd558513023768b43219f0840d9f390b92f42e0249e9051a7dd596965f7b`  
		Last Modified: Wed, 01 Mar 2023 08:18:50 GMT  
		Size: 5.4 KB (5389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d6b54fce3b52f5381a599e59836f8faf08f2c8077888bdc30eb2b217a96dbbe`  
		Last Modified: Wed, 01 Mar 2023 08:18:50 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0-oracle`

```console
$ docker pull mysql@sha256:2596158f73606ba571e1af29a9c32bec5dc021a2495e4a70d194a9b49664f4d9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8.0-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:79866c649987750de41276796f7b29a54be80834dd2bc20e435dc9554a33945f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.6 MB (156597480 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4073e6a6f54214da05256022b9a86e2f3f480703d1fc457a7085107c854e5ce3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 08 Mar 2023 20:22:31 GMT
ADD file:eca2b657866c594c67fc9041ad2a4a309e62fc8338add46c3917517649f748b2 in / 
# Wed, 08 Mar 2023 20:22:32 GMT
CMD ["/bin/bash"]
# Wed, 08 Mar 2023 20:40:06 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 08 Mar 2023 20:40:06 GMT
ENV GOSU_VERSION=1.16
# Wed, 08 Mar 2023 20:40:10 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 08 Mar 2023 20:40:35 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Wed, 08 Mar 2023 20:40:36 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 08 Mar 2023 20:40:36 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 08 Mar 2023 20:40:36 GMT
ENV MYSQL_VERSION=8.0.32-1.el8
# Wed, 08 Mar 2023 20:40:37 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 08 Mar 2023 20:41:09 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 08 Mar 2023 20:41:10 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 08 Mar 2023 20:41:10 GMT
ENV MYSQL_SHELL_VERSION=8.0.32-1.el8
# Wed, 08 Mar 2023 20:41:46 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Wed, 08 Mar 2023 20:41:47 GMT
VOLUME [/var/lib/mysql]
# Wed, 08 Mar 2023 20:41:47 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 08 Mar 2023 20:41:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 08 Mar 2023 20:41:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 08 Mar 2023 20:41:48 GMT
EXPOSE 3306 33060
# Wed, 08 Mar 2023 20:41:48 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:767a87c583278931a33db59dc8586fdcfa03c53a801cce573f0e861c31ec4c89`  
		Last Modified: Wed, 08 Mar 2023 20:24:06 GMT  
		Size: 44.6 MB (44557814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbd6d17e71a0fa12983f197a9f8c76b09ba416527debf78c14ac504317aec0f9`  
		Last Modified: Wed, 08 Mar 2023 20:43:49 GMT  
		Size: 887.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b17ad003fbc8375915bdad1cb4569356ce65dd16d5456337326e085572bb7ba`  
		Last Modified: Wed, 08 Mar 2023 20:43:49 GMT  
		Size: 982.8 KB (982819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:410b54c19b6bfa2624cb49d3ea768c0a46dc4719b1aa0a9f54f28024246f7c72`  
		Last Modified: Wed, 08 Mar 2023 20:43:48 GMT  
		Size: 4.6 MB (4624011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6192cec941545dc76c7a164680b55bb3ffe8271191bb2fc09d1bb18a64df4d3`  
		Last Modified: Wed, 08 Mar 2023 20:43:47 GMT  
		Size: 2.6 KB (2631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7be351756ff4dda5f0a2744d5bbd15c4133d6fe4aca456ce732fe4d870ebb06`  
		Last Modified: Wed, 08 Mar 2023 20:43:47 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae2d1ab519ee3bd717c6c2012e651f9511d04720f77724af8399f8d19c78c8a2`  
		Last Modified: Wed, 08 Mar 2023 20:43:53 GMT  
		Size: 56.2 MB (56233013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:119cfaa7dea024112488b45621d53ecf602293f6bdbcc3796090251911979f47`  
		Last Modified: Wed, 08 Mar 2023 20:43:45 GMT  
		Size: 317.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7176b3cc6ba140af2b8354ea0889eff5ccf7d9dadc9110d3b8d0f69c126c29d8`  
		Last Modified: Wed, 08 Mar 2023 20:43:55 GMT  
		Size: 50.2 MB (50190140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eb39e909e2beef35e5c3ea7d67c45c519eb06c9685846dd37f514ef68d18149`  
		Last Modified: Wed, 08 Mar 2023 20:43:45 GMT  
		Size: 5.4 KB (5393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e935886e1025cc7de30d6afcf9e7612a0dae12d42294969399544173a3bbfde3`  
		Last Modified: Wed, 08 Mar 2023 20:43:45 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8.0-oracle` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:d1887ec2b0018304daad8cdc1506d718ed0f04bed93ac87372355c12bba6bc08
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.4 MB (155433895 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7c54c29e20dccc1aefb936c8eba8bb8b98b87a4921102aba87fde2df5810af9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 08 Mar 2023 21:02:19 GMT
ADD file:18f4bd510f88f32e538884e4e633449c2c8dbf8a5f88b6b6b165ab05872d9507 in / 
# Wed, 08 Mar 2023 21:02:19 GMT
CMD ["/bin/bash"]
# Wed, 08 Mar 2023 21:25:35 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 08 Mar 2023 21:25:35 GMT
ENV GOSU_VERSION=1.16
# Wed, 08 Mar 2023 21:25:39 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 08 Mar 2023 21:26:01 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Wed, 08 Mar 2023 21:26:03 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 08 Mar 2023 21:26:03 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 08 Mar 2023 21:26:03 GMT
ENV MYSQL_VERSION=8.0.32-1.el8
# Wed, 08 Mar 2023 21:26:03 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 08 Mar 2023 21:26:29 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 08 Mar 2023 21:26:31 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 08 Mar 2023 21:26:31 GMT
ENV MYSQL_SHELL_VERSION=8.0.32-1.el8
# Wed, 08 Mar 2023 21:27:03 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Wed, 08 Mar 2023 21:27:05 GMT
VOLUME [/var/lib/mysql]
# Wed, 08 Mar 2023 21:27:05 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 08 Mar 2023 21:27:05 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 08 Mar 2023 21:27:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 08 Mar 2023 21:27:05 GMT
EXPOSE 3306 33060
# Wed, 08 Mar 2023 21:27:06 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:8ff0c9d62930fe3f55e00ba3be2db6be3643b07da9804d1c9b83b0d3181f0df5`  
		Last Modified: Wed, 08 Mar 2023 21:03:40 GMT  
		Size: 43.5 MB (43456139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c7ab176cd9d87a44c6b82369dab38d2a8a8f75036009413cc37399ed49b38e9`  
		Last Modified: Wed, 08 Mar 2023 21:27:28 GMT  
		Size: 886.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f6283edca869f9d898e92d4e5720e7ed8d16433dc7263b4a351b5c67199082c`  
		Last Modified: Wed, 08 Mar 2023 21:27:28 GMT  
		Size: 913.0 KB (912997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74489f3832cb81c43de395aa7a1345a5e233361ad8e2e460e3e9cf80f124329f`  
		Last Modified: Wed, 08 Mar 2023 21:27:26 GMT  
		Size: 4.5 MB (4456734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68fdb433cd6ed223c0ca86d0aca93e05f0df1a03588b2e63dbcdd7f836f6e785`  
		Last Modified: Wed, 08 Mar 2023 21:27:26 GMT  
		Size: 2.6 KB (2629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed704471ee1020a0a1808d0d8117ddeeea6154e24d50690959921a413029a880`  
		Last Modified: Wed, 08 Mar 2023 21:27:26 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8017dfacae02bc956ca22b2e23db59dc69f2e3a2948d497e3cb0a9429ba5342e`  
		Last Modified: Wed, 08 Mar 2023 21:27:30 GMT  
		Size: 55.6 MB (55615967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c01cb78ffdd6ef9f062f5d2a80e243e249de2447fd68e17c17b7a2938ed5cff`  
		Last Modified: Wed, 08 Mar 2023 21:27:24 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa238b7fd3ad0bf546c26574e4edcd1761584f55d8b338a7b0330399baae3e49`  
		Last Modified: Wed, 08 Mar 2023 21:27:31 GMT  
		Size: 51.0 MB (50982384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a86d0b8c1ccc4f969ad0e7b9fa57a409e360db176437a087a5fd9406b081691`  
		Last Modified: Wed, 08 Mar 2023 21:27:24 GMT  
		Size: 5.4 KB (5388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:326b54668f8b18657ed13771324644998d14801db082e346aad6c8dd67aecb51`  
		Last Modified: Wed, 08 Mar 2023 21:27:24 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0.32`

```console
$ docker pull mysql@sha256:2596158f73606ba571e1af29a9c32bec5dc021a2495e4a70d194a9b49664f4d9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8.0.32` - linux; amd64

```console
$ docker pull mysql@sha256:79866c649987750de41276796f7b29a54be80834dd2bc20e435dc9554a33945f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.6 MB (156597480 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4073e6a6f54214da05256022b9a86e2f3f480703d1fc457a7085107c854e5ce3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 08 Mar 2023 20:22:31 GMT
ADD file:eca2b657866c594c67fc9041ad2a4a309e62fc8338add46c3917517649f748b2 in / 
# Wed, 08 Mar 2023 20:22:32 GMT
CMD ["/bin/bash"]
# Wed, 08 Mar 2023 20:40:06 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 08 Mar 2023 20:40:06 GMT
ENV GOSU_VERSION=1.16
# Wed, 08 Mar 2023 20:40:10 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 08 Mar 2023 20:40:35 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Wed, 08 Mar 2023 20:40:36 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 08 Mar 2023 20:40:36 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 08 Mar 2023 20:40:36 GMT
ENV MYSQL_VERSION=8.0.32-1.el8
# Wed, 08 Mar 2023 20:40:37 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 08 Mar 2023 20:41:09 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 08 Mar 2023 20:41:10 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 08 Mar 2023 20:41:10 GMT
ENV MYSQL_SHELL_VERSION=8.0.32-1.el8
# Wed, 08 Mar 2023 20:41:46 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Wed, 08 Mar 2023 20:41:47 GMT
VOLUME [/var/lib/mysql]
# Wed, 08 Mar 2023 20:41:47 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 08 Mar 2023 20:41:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 08 Mar 2023 20:41:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 08 Mar 2023 20:41:48 GMT
EXPOSE 3306 33060
# Wed, 08 Mar 2023 20:41:48 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:767a87c583278931a33db59dc8586fdcfa03c53a801cce573f0e861c31ec4c89`  
		Last Modified: Wed, 08 Mar 2023 20:24:06 GMT  
		Size: 44.6 MB (44557814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbd6d17e71a0fa12983f197a9f8c76b09ba416527debf78c14ac504317aec0f9`  
		Last Modified: Wed, 08 Mar 2023 20:43:49 GMT  
		Size: 887.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b17ad003fbc8375915bdad1cb4569356ce65dd16d5456337326e085572bb7ba`  
		Last Modified: Wed, 08 Mar 2023 20:43:49 GMT  
		Size: 982.8 KB (982819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:410b54c19b6bfa2624cb49d3ea768c0a46dc4719b1aa0a9f54f28024246f7c72`  
		Last Modified: Wed, 08 Mar 2023 20:43:48 GMT  
		Size: 4.6 MB (4624011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6192cec941545dc76c7a164680b55bb3ffe8271191bb2fc09d1bb18a64df4d3`  
		Last Modified: Wed, 08 Mar 2023 20:43:47 GMT  
		Size: 2.6 KB (2631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7be351756ff4dda5f0a2744d5bbd15c4133d6fe4aca456ce732fe4d870ebb06`  
		Last Modified: Wed, 08 Mar 2023 20:43:47 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae2d1ab519ee3bd717c6c2012e651f9511d04720f77724af8399f8d19c78c8a2`  
		Last Modified: Wed, 08 Mar 2023 20:43:53 GMT  
		Size: 56.2 MB (56233013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:119cfaa7dea024112488b45621d53ecf602293f6bdbcc3796090251911979f47`  
		Last Modified: Wed, 08 Mar 2023 20:43:45 GMT  
		Size: 317.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7176b3cc6ba140af2b8354ea0889eff5ccf7d9dadc9110d3b8d0f69c126c29d8`  
		Last Modified: Wed, 08 Mar 2023 20:43:55 GMT  
		Size: 50.2 MB (50190140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eb39e909e2beef35e5c3ea7d67c45c519eb06c9685846dd37f514ef68d18149`  
		Last Modified: Wed, 08 Mar 2023 20:43:45 GMT  
		Size: 5.4 KB (5393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e935886e1025cc7de30d6afcf9e7612a0dae12d42294969399544173a3bbfde3`  
		Last Modified: Wed, 08 Mar 2023 20:43:45 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8.0.32` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:d1887ec2b0018304daad8cdc1506d718ed0f04bed93ac87372355c12bba6bc08
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.4 MB (155433895 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7c54c29e20dccc1aefb936c8eba8bb8b98b87a4921102aba87fde2df5810af9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 08 Mar 2023 21:02:19 GMT
ADD file:18f4bd510f88f32e538884e4e633449c2c8dbf8a5f88b6b6b165ab05872d9507 in / 
# Wed, 08 Mar 2023 21:02:19 GMT
CMD ["/bin/bash"]
# Wed, 08 Mar 2023 21:25:35 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 08 Mar 2023 21:25:35 GMT
ENV GOSU_VERSION=1.16
# Wed, 08 Mar 2023 21:25:39 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 08 Mar 2023 21:26:01 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Wed, 08 Mar 2023 21:26:03 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 08 Mar 2023 21:26:03 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 08 Mar 2023 21:26:03 GMT
ENV MYSQL_VERSION=8.0.32-1.el8
# Wed, 08 Mar 2023 21:26:03 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 08 Mar 2023 21:26:29 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 08 Mar 2023 21:26:31 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 08 Mar 2023 21:26:31 GMT
ENV MYSQL_SHELL_VERSION=8.0.32-1.el8
# Wed, 08 Mar 2023 21:27:03 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Wed, 08 Mar 2023 21:27:05 GMT
VOLUME [/var/lib/mysql]
# Wed, 08 Mar 2023 21:27:05 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 08 Mar 2023 21:27:05 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 08 Mar 2023 21:27:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 08 Mar 2023 21:27:05 GMT
EXPOSE 3306 33060
# Wed, 08 Mar 2023 21:27:06 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:8ff0c9d62930fe3f55e00ba3be2db6be3643b07da9804d1c9b83b0d3181f0df5`  
		Last Modified: Wed, 08 Mar 2023 21:03:40 GMT  
		Size: 43.5 MB (43456139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c7ab176cd9d87a44c6b82369dab38d2a8a8f75036009413cc37399ed49b38e9`  
		Last Modified: Wed, 08 Mar 2023 21:27:28 GMT  
		Size: 886.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f6283edca869f9d898e92d4e5720e7ed8d16433dc7263b4a351b5c67199082c`  
		Last Modified: Wed, 08 Mar 2023 21:27:28 GMT  
		Size: 913.0 KB (912997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74489f3832cb81c43de395aa7a1345a5e233361ad8e2e460e3e9cf80f124329f`  
		Last Modified: Wed, 08 Mar 2023 21:27:26 GMT  
		Size: 4.5 MB (4456734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68fdb433cd6ed223c0ca86d0aca93e05f0df1a03588b2e63dbcdd7f836f6e785`  
		Last Modified: Wed, 08 Mar 2023 21:27:26 GMT  
		Size: 2.6 KB (2629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed704471ee1020a0a1808d0d8117ddeeea6154e24d50690959921a413029a880`  
		Last Modified: Wed, 08 Mar 2023 21:27:26 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8017dfacae02bc956ca22b2e23db59dc69f2e3a2948d497e3cb0a9429ba5342e`  
		Last Modified: Wed, 08 Mar 2023 21:27:30 GMT  
		Size: 55.6 MB (55615967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c01cb78ffdd6ef9f062f5d2a80e243e249de2447fd68e17c17b7a2938ed5cff`  
		Last Modified: Wed, 08 Mar 2023 21:27:24 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa238b7fd3ad0bf546c26574e4edcd1761584f55d8b338a7b0330399baae3e49`  
		Last Modified: Wed, 08 Mar 2023 21:27:31 GMT  
		Size: 51.0 MB (50982384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a86d0b8c1ccc4f969ad0e7b9fa57a409e360db176437a087a5fd9406b081691`  
		Last Modified: Wed, 08 Mar 2023 21:27:24 GMT  
		Size: 5.4 KB (5388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:326b54668f8b18657ed13771324644998d14801db082e346aad6c8dd67aecb51`  
		Last Modified: Wed, 08 Mar 2023 21:27:24 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0.32-debian`

```console
$ docker pull mysql@sha256:c26ffcfefadf3698514de6e8e8b3566cd0da5b8a9ee3543ea0eb44bc5faab6dc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:8.0.32-debian` - linux; amd64

```console
$ docker pull mysql@sha256:2f7872dbcb701e16397e23e368148ee9411027cd4baf5905d0622ccccc35092e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **177.8 MB (177766717 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f88e52842dfbc5faff99e03317eb17892293cd424cd745e74ec04408ba255207`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 01 Mar 2023 04:09:58 GMT
ADD file:493a5b0c8d2d63a1343258b3f9aa5fcd59a93f44fe26ad9e56b094c3a08fd3be in / 
# Wed, 01 Mar 2023 04:09:59 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 08:16:50 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 01 Mar 2023 08:16:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 08:16:56 GMT
ENV GOSU_VERSION=1.16
# Wed, 01 Mar 2023 08:17:04 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 01 Mar 2023 08:17:05 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 01 Mar 2023 08:17:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 08:17:11 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Wed, 01 Mar 2023 08:17:12 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 01 Mar 2023 08:17:12 GMT
ENV MYSQL_VERSION=8.0.32-1debian11
# Wed, 01 Mar 2023 08:17:12 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ bullseye mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Wed, 01 Mar 2023 08:17:27 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Wed, 01 Mar 2023 08:17:28 GMT
VOLUME [/var/lib/mysql]
# Wed, 01 Mar 2023 08:17:28 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Wed, 01 Mar 2023 08:17:28 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 01 Mar 2023 08:17:29 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 01 Mar 2023 08:17:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Mar 2023 08:17:29 GMT
EXPOSE 3306 33060
# Wed, 01 Mar 2023 08:17:29 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:3f9582a2cbe7197f39185419c0ced2c986389f8fc6aa805e1f5c090eea6511e0`  
		Last Modified: Wed, 01 Mar 2023 04:14:23 GMT  
		Size: 31.4 MB (31411403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:760f99c7c3059a32499d51cb02152df032fc466298a3e2b7e600029b9b91f4ea`  
		Last Modified: Wed, 01 Mar 2023 08:18:54 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d20338c318a65cc44a3e0a1a60cb9c690d286ff757ea0b3a976bf24748a0316`  
		Last Modified: Wed, 01 Mar 2023 08:18:54 GMT  
		Size: 4.4 MB (4414965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e92be7428ec909fce6a3b308505a95430380d7b319e454a1eb04c11f33522f7`  
		Last Modified: Wed, 01 Mar 2023 08:18:52 GMT  
		Size: 1.5 MB (1471440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1c491527f8245e4dc5378618790c15c6885747848d85b17bcb6dce84ad2ff88`  
		Last Modified: Wed, 01 Mar 2023 08:18:51 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8aab5d3f904fbf665f9b72bfad9092bce3e58555608293d61f421931eaf99f80`  
		Last Modified: Wed, 01 Mar 2023 08:18:54 GMT  
		Size: 12.7 MB (12661962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0764a75d4948f4bc90025d5a92b44e3ff0372e8798b456860ee310dd9bb3e52f`  
		Last Modified: Wed, 01 Mar 2023 08:18:51 GMT  
		Size: 2.5 KB (2549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abceaa621503b0635e2b0e9740dfe37f20b0c42d1d17615caebdc44f5f05949f`  
		Last Modified: Wed, 01 Mar 2023 08:18:50 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09a8f23f9143940d284a3ff2c1767c607db5bfe4652eb720a811f902a4188707`  
		Last Modified: Wed, 01 Mar 2023 08:19:09 GMT  
		Size: 127.8 MB (127795909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfad9bee7b38020e4c875fff67ed05f30ab2e771c0db576fe03213199b20dec0`  
		Last Modified: Wed, 01 Mar 2023 08:18:50 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fdbfd558513023768b43219f0840d9f390b92f42e0249e9051a7dd596965f7b`  
		Last Modified: Wed, 01 Mar 2023 08:18:50 GMT  
		Size: 5.4 KB (5389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d6b54fce3b52f5381a599e59836f8faf08f2c8077888bdc30eb2b217a96dbbe`  
		Last Modified: Wed, 01 Mar 2023 08:18:50 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0.32-oracle`

```console
$ docker pull mysql@sha256:2596158f73606ba571e1af29a9c32bec5dc021a2495e4a70d194a9b49664f4d9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8.0.32-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:79866c649987750de41276796f7b29a54be80834dd2bc20e435dc9554a33945f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.6 MB (156597480 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4073e6a6f54214da05256022b9a86e2f3f480703d1fc457a7085107c854e5ce3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 08 Mar 2023 20:22:31 GMT
ADD file:eca2b657866c594c67fc9041ad2a4a309e62fc8338add46c3917517649f748b2 in / 
# Wed, 08 Mar 2023 20:22:32 GMT
CMD ["/bin/bash"]
# Wed, 08 Mar 2023 20:40:06 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 08 Mar 2023 20:40:06 GMT
ENV GOSU_VERSION=1.16
# Wed, 08 Mar 2023 20:40:10 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 08 Mar 2023 20:40:35 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Wed, 08 Mar 2023 20:40:36 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 08 Mar 2023 20:40:36 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 08 Mar 2023 20:40:36 GMT
ENV MYSQL_VERSION=8.0.32-1.el8
# Wed, 08 Mar 2023 20:40:37 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 08 Mar 2023 20:41:09 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 08 Mar 2023 20:41:10 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 08 Mar 2023 20:41:10 GMT
ENV MYSQL_SHELL_VERSION=8.0.32-1.el8
# Wed, 08 Mar 2023 20:41:46 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Wed, 08 Mar 2023 20:41:47 GMT
VOLUME [/var/lib/mysql]
# Wed, 08 Mar 2023 20:41:47 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 08 Mar 2023 20:41:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 08 Mar 2023 20:41:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 08 Mar 2023 20:41:48 GMT
EXPOSE 3306 33060
# Wed, 08 Mar 2023 20:41:48 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:767a87c583278931a33db59dc8586fdcfa03c53a801cce573f0e861c31ec4c89`  
		Last Modified: Wed, 08 Mar 2023 20:24:06 GMT  
		Size: 44.6 MB (44557814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbd6d17e71a0fa12983f197a9f8c76b09ba416527debf78c14ac504317aec0f9`  
		Last Modified: Wed, 08 Mar 2023 20:43:49 GMT  
		Size: 887.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b17ad003fbc8375915bdad1cb4569356ce65dd16d5456337326e085572bb7ba`  
		Last Modified: Wed, 08 Mar 2023 20:43:49 GMT  
		Size: 982.8 KB (982819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:410b54c19b6bfa2624cb49d3ea768c0a46dc4719b1aa0a9f54f28024246f7c72`  
		Last Modified: Wed, 08 Mar 2023 20:43:48 GMT  
		Size: 4.6 MB (4624011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6192cec941545dc76c7a164680b55bb3ffe8271191bb2fc09d1bb18a64df4d3`  
		Last Modified: Wed, 08 Mar 2023 20:43:47 GMT  
		Size: 2.6 KB (2631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7be351756ff4dda5f0a2744d5bbd15c4133d6fe4aca456ce732fe4d870ebb06`  
		Last Modified: Wed, 08 Mar 2023 20:43:47 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae2d1ab519ee3bd717c6c2012e651f9511d04720f77724af8399f8d19c78c8a2`  
		Last Modified: Wed, 08 Mar 2023 20:43:53 GMT  
		Size: 56.2 MB (56233013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:119cfaa7dea024112488b45621d53ecf602293f6bdbcc3796090251911979f47`  
		Last Modified: Wed, 08 Mar 2023 20:43:45 GMT  
		Size: 317.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7176b3cc6ba140af2b8354ea0889eff5ccf7d9dadc9110d3b8d0f69c126c29d8`  
		Last Modified: Wed, 08 Mar 2023 20:43:55 GMT  
		Size: 50.2 MB (50190140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eb39e909e2beef35e5c3ea7d67c45c519eb06c9685846dd37f514ef68d18149`  
		Last Modified: Wed, 08 Mar 2023 20:43:45 GMT  
		Size: 5.4 KB (5393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e935886e1025cc7de30d6afcf9e7612a0dae12d42294969399544173a3bbfde3`  
		Last Modified: Wed, 08 Mar 2023 20:43:45 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8.0.32-oracle` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:d1887ec2b0018304daad8cdc1506d718ed0f04bed93ac87372355c12bba6bc08
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.4 MB (155433895 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7c54c29e20dccc1aefb936c8eba8bb8b98b87a4921102aba87fde2df5810af9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 08 Mar 2023 21:02:19 GMT
ADD file:18f4bd510f88f32e538884e4e633449c2c8dbf8a5f88b6b6b165ab05872d9507 in / 
# Wed, 08 Mar 2023 21:02:19 GMT
CMD ["/bin/bash"]
# Wed, 08 Mar 2023 21:25:35 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 08 Mar 2023 21:25:35 GMT
ENV GOSU_VERSION=1.16
# Wed, 08 Mar 2023 21:25:39 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 08 Mar 2023 21:26:01 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Wed, 08 Mar 2023 21:26:03 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 08 Mar 2023 21:26:03 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 08 Mar 2023 21:26:03 GMT
ENV MYSQL_VERSION=8.0.32-1.el8
# Wed, 08 Mar 2023 21:26:03 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 08 Mar 2023 21:26:29 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 08 Mar 2023 21:26:31 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 08 Mar 2023 21:26:31 GMT
ENV MYSQL_SHELL_VERSION=8.0.32-1.el8
# Wed, 08 Mar 2023 21:27:03 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Wed, 08 Mar 2023 21:27:05 GMT
VOLUME [/var/lib/mysql]
# Wed, 08 Mar 2023 21:27:05 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 08 Mar 2023 21:27:05 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 08 Mar 2023 21:27:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 08 Mar 2023 21:27:05 GMT
EXPOSE 3306 33060
# Wed, 08 Mar 2023 21:27:06 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:8ff0c9d62930fe3f55e00ba3be2db6be3643b07da9804d1c9b83b0d3181f0df5`  
		Last Modified: Wed, 08 Mar 2023 21:03:40 GMT  
		Size: 43.5 MB (43456139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c7ab176cd9d87a44c6b82369dab38d2a8a8f75036009413cc37399ed49b38e9`  
		Last Modified: Wed, 08 Mar 2023 21:27:28 GMT  
		Size: 886.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f6283edca869f9d898e92d4e5720e7ed8d16433dc7263b4a351b5c67199082c`  
		Last Modified: Wed, 08 Mar 2023 21:27:28 GMT  
		Size: 913.0 KB (912997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74489f3832cb81c43de395aa7a1345a5e233361ad8e2e460e3e9cf80f124329f`  
		Last Modified: Wed, 08 Mar 2023 21:27:26 GMT  
		Size: 4.5 MB (4456734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68fdb433cd6ed223c0ca86d0aca93e05f0df1a03588b2e63dbcdd7f836f6e785`  
		Last Modified: Wed, 08 Mar 2023 21:27:26 GMT  
		Size: 2.6 KB (2629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed704471ee1020a0a1808d0d8117ddeeea6154e24d50690959921a413029a880`  
		Last Modified: Wed, 08 Mar 2023 21:27:26 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8017dfacae02bc956ca22b2e23db59dc69f2e3a2948d497e3cb0a9429ba5342e`  
		Last Modified: Wed, 08 Mar 2023 21:27:30 GMT  
		Size: 55.6 MB (55615967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c01cb78ffdd6ef9f062f5d2a80e243e249de2447fd68e17c17b7a2938ed5cff`  
		Last Modified: Wed, 08 Mar 2023 21:27:24 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa238b7fd3ad0bf546c26574e4edcd1761584f55d8b338a7b0330399baae3e49`  
		Last Modified: Wed, 08 Mar 2023 21:27:31 GMT  
		Size: 51.0 MB (50982384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a86d0b8c1ccc4f969ad0e7b9fa57a409e360db176437a087a5fd9406b081691`  
		Last Modified: Wed, 08 Mar 2023 21:27:24 GMT  
		Size: 5.4 KB (5388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:326b54668f8b18657ed13771324644998d14801db082e346aad6c8dd67aecb51`  
		Last Modified: Wed, 08 Mar 2023 21:27:24 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:debian`

```console
$ docker pull mysql@sha256:c26ffcfefadf3698514de6e8e8b3566cd0da5b8a9ee3543ea0eb44bc5faab6dc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:debian` - linux; amd64

```console
$ docker pull mysql@sha256:2f7872dbcb701e16397e23e368148ee9411027cd4baf5905d0622ccccc35092e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **177.8 MB (177766717 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f88e52842dfbc5faff99e03317eb17892293cd424cd745e74ec04408ba255207`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 01 Mar 2023 04:09:58 GMT
ADD file:493a5b0c8d2d63a1343258b3f9aa5fcd59a93f44fe26ad9e56b094c3a08fd3be in / 
# Wed, 01 Mar 2023 04:09:59 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 08:16:50 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 01 Mar 2023 08:16:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 08:16:56 GMT
ENV GOSU_VERSION=1.16
# Wed, 01 Mar 2023 08:17:04 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 01 Mar 2023 08:17:05 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 01 Mar 2023 08:17:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 08:17:11 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Wed, 01 Mar 2023 08:17:12 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 01 Mar 2023 08:17:12 GMT
ENV MYSQL_VERSION=8.0.32-1debian11
# Wed, 01 Mar 2023 08:17:12 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ bullseye mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Wed, 01 Mar 2023 08:17:27 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Wed, 01 Mar 2023 08:17:28 GMT
VOLUME [/var/lib/mysql]
# Wed, 01 Mar 2023 08:17:28 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Wed, 01 Mar 2023 08:17:28 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 01 Mar 2023 08:17:29 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 01 Mar 2023 08:17:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Mar 2023 08:17:29 GMT
EXPOSE 3306 33060
# Wed, 01 Mar 2023 08:17:29 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:3f9582a2cbe7197f39185419c0ced2c986389f8fc6aa805e1f5c090eea6511e0`  
		Last Modified: Wed, 01 Mar 2023 04:14:23 GMT  
		Size: 31.4 MB (31411403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:760f99c7c3059a32499d51cb02152df032fc466298a3e2b7e600029b9b91f4ea`  
		Last Modified: Wed, 01 Mar 2023 08:18:54 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d20338c318a65cc44a3e0a1a60cb9c690d286ff757ea0b3a976bf24748a0316`  
		Last Modified: Wed, 01 Mar 2023 08:18:54 GMT  
		Size: 4.4 MB (4414965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e92be7428ec909fce6a3b308505a95430380d7b319e454a1eb04c11f33522f7`  
		Last Modified: Wed, 01 Mar 2023 08:18:52 GMT  
		Size: 1.5 MB (1471440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1c491527f8245e4dc5378618790c15c6885747848d85b17bcb6dce84ad2ff88`  
		Last Modified: Wed, 01 Mar 2023 08:18:51 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8aab5d3f904fbf665f9b72bfad9092bce3e58555608293d61f421931eaf99f80`  
		Last Modified: Wed, 01 Mar 2023 08:18:54 GMT  
		Size: 12.7 MB (12661962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0764a75d4948f4bc90025d5a92b44e3ff0372e8798b456860ee310dd9bb3e52f`  
		Last Modified: Wed, 01 Mar 2023 08:18:51 GMT  
		Size: 2.5 KB (2549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abceaa621503b0635e2b0e9740dfe37f20b0c42d1d17615caebdc44f5f05949f`  
		Last Modified: Wed, 01 Mar 2023 08:18:50 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09a8f23f9143940d284a3ff2c1767c607db5bfe4652eb720a811f902a4188707`  
		Last Modified: Wed, 01 Mar 2023 08:19:09 GMT  
		Size: 127.8 MB (127795909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfad9bee7b38020e4c875fff67ed05f30ab2e771c0db576fe03213199b20dec0`  
		Last Modified: Wed, 01 Mar 2023 08:18:50 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fdbfd558513023768b43219f0840d9f390b92f42e0249e9051a7dd596965f7b`  
		Last Modified: Wed, 01 Mar 2023 08:18:50 GMT  
		Size: 5.4 KB (5389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d6b54fce3b52f5381a599e59836f8faf08f2c8077888bdc30eb2b217a96dbbe`  
		Last Modified: Wed, 01 Mar 2023 08:18:50 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:latest`

```console
$ docker pull mysql@sha256:2596158f73606ba571e1af29a9c32bec5dc021a2495e4a70d194a9b49664f4d9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:latest` - linux; amd64

```console
$ docker pull mysql@sha256:79866c649987750de41276796f7b29a54be80834dd2bc20e435dc9554a33945f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.6 MB (156597480 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4073e6a6f54214da05256022b9a86e2f3f480703d1fc457a7085107c854e5ce3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 08 Mar 2023 20:22:31 GMT
ADD file:eca2b657866c594c67fc9041ad2a4a309e62fc8338add46c3917517649f748b2 in / 
# Wed, 08 Mar 2023 20:22:32 GMT
CMD ["/bin/bash"]
# Wed, 08 Mar 2023 20:40:06 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 08 Mar 2023 20:40:06 GMT
ENV GOSU_VERSION=1.16
# Wed, 08 Mar 2023 20:40:10 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 08 Mar 2023 20:40:35 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Wed, 08 Mar 2023 20:40:36 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 08 Mar 2023 20:40:36 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 08 Mar 2023 20:40:36 GMT
ENV MYSQL_VERSION=8.0.32-1.el8
# Wed, 08 Mar 2023 20:40:37 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 08 Mar 2023 20:41:09 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 08 Mar 2023 20:41:10 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 08 Mar 2023 20:41:10 GMT
ENV MYSQL_SHELL_VERSION=8.0.32-1.el8
# Wed, 08 Mar 2023 20:41:46 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Wed, 08 Mar 2023 20:41:47 GMT
VOLUME [/var/lib/mysql]
# Wed, 08 Mar 2023 20:41:47 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 08 Mar 2023 20:41:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 08 Mar 2023 20:41:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 08 Mar 2023 20:41:48 GMT
EXPOSE 3306 33060
# Wed, 08 Mar 2023 20:41:48 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:767a87c583278931a33db59dc8586fdcfa03c53a801cce573f0e861c31ec4c89`  
		Last Modified: Wed, 08 Mar 2023 20:24:06 GMT  
		Size: 44.6 MB (44557814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbd6d17e71a0fa12983f197a9f8c76b09ba416527debf78c14ac504317aec0f9`  
		Last Modified: Wed, 08 Mar 2023 20:43:49 GMT  
		Size: 887.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b17ad003fbc8375915bdad1cb4569356ce65dd16d5456337326e085572bb7ba`  
		Last Modified: Wed, 08 Mar 2023 20:43:49 GMT  
		Size: 982.8 KB (982819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:410b54c19b6bfa2624cb49d3ea768c0a46dc4719b1aa0a9f54f28024246f7c72`  
		Last Modified: Wed, 08 Mar 2023 20:43:48 GMT  
		Size: 4.6 MB (4624011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6192cec941545dc76c7a164680b55bb3ffe8271191bb2fc09d1bb18a64df4d3`  
		Last Modified: Wed, 08 Mar 2023 20:43:47 GMT  
		Size: 2.6 KB (2631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7be351756ff4dda5f0a2744d5bbd15c4133d6fe4aca456ce732fe4d870ebb06`  
		Last Modified: Wed, 08 Mar 2023 20:43:47 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae2d1ab519ee3bd717c6c2012e651f9511d04720f77724af8399f8d19c78c8a2`  
		Last Modified: Wed, 08 Mar 2023 20:43:53 GMT  
		Size: 56.2 MB (56233013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:119cfaa7dea024112488b45621d53ecf602293f6bdbcc3796090251911979f47`  
		Last Modified: Wed, 08 Mar 2023 20:43:45 GMT  
		Size: 317.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7176b3cc6ba140af2b8354ea0889eff5ccf7d9dadc9110d3b8d0f69c126c29d8`  
		Last Modified: Wed, 08 Mar 2023 20:43:55 GMT  
		Size: 50.2 MB (50190140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eb39e909e2beef35e5c3ea7d67c45c519eb06c9685846dd37f514ef68d18149`  
		Last Modified: Wed, 08 Mar 2023 20:43:45 GMT  
		Size: 5.4 KB (5393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e935886e1025cc7de30d6afcf9e7612a0dae12d42294969399544173a3bbfde3`  
		Last Modified: Wed, 08 Mar 2023 20:43:45 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:latest` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:d1887ec2b0018304daad8cdc1506d718ed0f04bed93ac87372355c12bba6bc08
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.4 MB (155433895 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7c54c29e20dccc1aefb936c8eba8bb8b98b87a4921102aba87fde2df5810af9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 08 Mar 2023 21:02:19 GMT
ADD file:18f4bd510f88f32e538884e4e633449c2c8dbf8a5f88b6b6b165ab05872d9507 in / 
# Wed, 08 Mar 2023 21:02:19 GMT
CMD ["/bin/bash"]
# Wed, 08 Mar 2023 21:25:35 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 08 Mar 2023 21:25:35 GMT
ENV GOSU_VERSION=1.16
# Wed, 08 Mar 2023 21:25:39 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 08 Mar 2023 21:26:01 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Wed, 08 Mar 2023 21:26:03 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 08 Mar 2023 21:26:03 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 08 Mar 2023 21:26:03 GMT
ENV MYSQL_VERSION=8.0.32-1.el8
# Wed, 08 Mar 2023 21:26:03 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 08 Mar 2023 21:26:29 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 08 Mar 2023 21:26:31 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 08 Mar 2023 21:26:31 GMT
ENV MYSQL_SHELL_VERSION=8.0.32-1.el8
# Wed, 08 Mar 2023 21:27:03 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Wed, 08 Mar 2023 21:27:05 GMT
VOLUME [/var/lib/mysql]
# Wed, 08 Mar 2023 21:27:05 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 08 Mar 2023 21:27:05 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 08 Mar 2023 21:27:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 08 Mar 2023 21:27:05 GMT
EXPOSE 3306 33060
# Wed, 08 Mar 2023 21:27:06 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:8ff0c9d62930fe3f55e00ba3be2db6be3643b07da9804d1c9b83b0d3181f0df5`  
		Last Modified: Wed, 08 Mar 2023 21:03:40 GMT  
		Size: 43.5 MB (43456139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c7ab176cd9d87a44c6b82369dab38d2a8a8f75036009413cc37399ed49b38e9`  
		Last Modified: Wed, 08 Mar 2023 21:27:28 GMT  
		Size: 886.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f6283edca869f9d898e92d4e5720e7ed8d16433dc7263b4a351b5c67199082c`  
		Last Modified: Wed, 08 Mar 2023 21:27:28 GMT  
		Size: 913.0 KB (912997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74489f3832cb81c43de395aa7a1345a5e233361ad8e2e460e3e9cf80f124329f`  
		Last Modified: Wed, 08 Mar 2023 21:27:26 GMT  
		Size: 4.5 MB (4456734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68fdb433cd6ed223c0ca86d0aca93e05f0df1a03588b2e63dbcdd7f836f6e785`  
		Last Modified: Wed, 08 Mar 2023 21:27:26 GMT  
		Size: 2.6 KB (2629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed704471ee1020a0a1808d0d8117ddeeea6154e24d50690959921a413029a880`  
		Last Modified: Wed, 08 Mar 2023 21:27:26 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8017dfacae02bc956ca22b2e23db59dc69f2e3a2948d497e3cb0a9429ba5342e`  
		Last Modified: Wed, 08 Mar 2023 21:27:30 GMT  
		Size: 55.6 MB (55615967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c01cb78ffdd6ef9f062f5d2a80e243e249de2447fd68e17c17b7a2938ed5cff`  
		Last Modified: Wed, 08 Mar 2023 21:27:24 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa238b7fd3ad0bf546c26574e4edcd1761584f55d8b338a7b0330399baae3e49`  
		Last Modified: Wed, 08 Mar 2023 21:27:31 GMT  
		Size: 51.0 MB (50982384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a86d0b8c1ccc4f969ad0e7b9fa57a409e360db176437a087a5fd9406b081691`  
		Last Modified: Wed, 08 Mar 2023 21:27:24 GMT  
		Size: 5.4 KB (5388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:326b54668f8b18657ed13771324644998d14801db082e346aad6c8dd67aecb51`  
		Last Modified: Wed, 08 Mar 2023 21:27:24 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:oracle`

```console
$ docker pull mysql@sha256:2596158f73606ba571e1af29a9c32bec5dc021a2495e4a70d194a9b49664f4d9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:oracle` - linux; amd64

```console
$ docker pull mysql@sha256:79866c649987750de41276796f7b29a54be80834dd2bc20e435dc9554a33945f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.6 MB (156597480 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4073e6a6f54214da05256022b9a86e2f3f480703d1fc457a7085107c854e5ce3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 08 Mar 2023 20:22:31 GMT
ADD file:eca2b657866c594c67fc9041ad2a4a309e62fc8338add46c3917517649f748b2 in / 
# Wed, 08 Mar 2023 20:22:32 GMT
CMD ["/bin/bash"]
# Wed, 08 Mar 2023 20:40:06 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 08 Mar 2023 20:40:06 GMT
ENV GOSU_VERSION=1.16
# Wed, 08 Mar 2023 20:40:10 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 08 Mar 2023 20:40:35 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Wed, 08 Mar 2023 20:40:36 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 08 Mar 2023 20:40:36 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 08 Mar 2023 20:40:36 GMT
ENV MYSQL_VERSION=8.0.32-1.el8
# Wed, 08 Mar 2023 20:40:37 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 08 Mar 2023 20:41:09 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 08 Mar 2023 20:41:10 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 08 Mar 2023 20:41:10 GMT
ENV MYSQL_SHELL_VERSION=8.0.32-1.el8
# Wed, 08 Mar 2023 20:41:46 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Wed, 08 Mar 2023 20:41:47 GMT
VOLUME [/var/lib/mysql]
# Wed, 08 Mar 2023 20:41:47 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 08 Mar 2023 20:41:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 08 Mar 2023 20:41:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 08 Mar 2023 20:41:48 GMT
EXPOSE 3306 33060
# Wed, 08 Mar 2023 20:41:48 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:767a87c583278931a33db59dc8586fdcfa03c53a801cce573f0e861c31ec4c89`  
		Last Modified: Wed, 08 Mar 2023 20:24:06 GMT  
		Size: 44.6 MB (44557814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbd6d17e71a0fa12983f197a9f8c76b09ba416527debf78c14ac504317aec0f9`  
		Last Modified: Wed, 08 Mar 2023 20:43:49 GMT  
		Size: 887.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b17ad003fbc8375915bdad1cb4569356ce65dd16d5456337326e085572bb7ba`  
		Last Modified: Wed, 08 Mar 2023 20:43:49 GMT  
		Size: 982.8 KB (982819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:410b54c19b6bfa2624cb49d3ea768c0a46dc4719b1aa0a9f54f28024246f7c72`  
		Last Modified: Wed, 08 Mar 2023 20:43:48 GMT  
		Size: 4.6 MB (4624011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6192cec941545dc76c7a164680b55bb3ffe8271191bb2fc09d1bb18a64df4d3`  
		Last Modified: Wed, 08 Mar 2023 20:43:47 GMT  
		Size: 2.6 KB (2631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7be351756ff4dda5f0a2744d5bbd15c4133d6fe4aca456ce732fe4d870ebb06`  
		Last Modified: Wed, 08 Mar 2023 20:43:47 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae2d1ab519ee3bd717c6c2012e651f9511d04720f77724af8399f8d19c78c8a2`  
		Last Modified: Wed, 08 Mar 2023 20:43:53 GMT  
		Size: 56.2 MB (56233013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:119cfaa7dea024112488b45621d53ecf602293f6bdbcc3796090251911979f47`  
		Last Modified: Wed, 08 Mar 2023 20:43:45 GMT  
		Size: 317.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7176b3cc6ba140af2b8354ea0889eff5ccf7d9dadc9110d3b8d0f69c126c29d8`  
		Last Modified: Wed, 08 Mar 2023 20:43:55 GMT  
		Size: 50.2 MB (50190140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eb39e909e2beef35e5c3ea7d67c45c519eb06c9685846dd37f514ef68d18149`  
		Last Modified: Wed, 08 Mar 2023 20:43:45 GMT  
		Size: 5.4 KB (5393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e935886e1025cc7de30d6afcf9e7612a0dae12d42294969399544173a3bbfde3`  
		Last Modified: Wed, 08 Mar 2023 20:43:45 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:oracle` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:d1887ec2b0018304daad8cdc1506d718ed0f04bed93ac87372355c12bba6bc08
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.4 MB (155433895 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7c54c29e20dccc1aefb936c8eba8bb8b98b87a4921102aba87fde2df5810af9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 08 Mar 2023 21:02:19 GMT
ADD file:18f4bd510f88f32e538884e4e633449c2c8dbf8a5f88b6b6b165ab05872d9507 in / 
# Wed, 08 Mar 2023 21:02:19 GMT
CMD ["/bin/bash"]
# Wed, 08 Mar 2023 21:25:35 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 08 Mar 2023 21:25:35 GMT
ENV GOSU_VERSION=1.16
# Wed, 08 Mar 2023 21:25:39 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 08 Mar 2023 21:26:01 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Wed, 08 Mar 2023 21:26:03 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 08 Mar 2023 21:26:03 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 08 Mar 2023 21:26:03 GMT
ENV MYSQL_VERSION=8.0.32-1.el8
# Wed, 08 Mar 2023 21:26:03 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 08 Mar 2023 21:26:29 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 08 Mar 2023 21:26:31 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 08 Mar 2023 21:26:31 GMT
ENV MYSQL_SHELL_VERSION=8.0.32-1.el8
# Wed, 08 Mar 2023 21:27:03 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Wed, 08 Mar 2023 21:27:05 GMT
VOLUME [/var/lib/mysql]
# Wed, 08 Mar 2023 21:27:05 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 08 Mar 2023 21:27:05 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 08 Mar 2023 21:27:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 08 Mar 2023 21:27:05 GMT
EXPOSE 3306 33060
# Wed, 08 Mar 2023 21:27:06 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:8ff0c9d62930fe3f55e00ba3be2db6be3643b07da9804d1c9b83b0d3181f0df5`  
		Last Modified: Wed, 08 Mar 2023 21:03:40 GMT  
		Size: 43.5 MB (43456139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c7ab176cd9d87a44c6b82369dab38d2a8a8f75036009413cc37399ed49b38e9`  
		Last Modified: Wed, 08 Mar 2023 21:27:28 GMT  
		Size: 886.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f6283edca869f9d898e92d4e5720e7ed8d16433dc7263b4a351b5c67199082c`  
		Last Modified: Wed, 08 Mar 2023 21:27:28 GMT  
		Size: 913.0 KB (912997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74489f3832cb81c43de395aa7a1345a5e233361ad8e2e460e3e9cf80f124329f`  
		Last Modified: Wed, 08 Mar 2023 21:27:26 GMT  
		Size: 4.5 MB (4456734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68fdb433cd6ed223c0ca86d0aca93e05f0df1a03588b2e63dbcdd7f836f6e785`  
		Last Modified: Wed, 08 Mar 2023 21:27:26 GMT  
		Size: 2.6 KB (2629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed704471ee1020a0a1808d0d8117ddeeea6154e24d50690959921a413029a880`  
		Last Modified: Wed, 08 Mar 2023 21:27:26 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8017dfacae02bc956ca22b2e23db59dc69f2e3a2948d497e3cb0a9429ba5342e`  
		Last Modified: Wed, 08 Mar 2023 21:27:30 GMT  
		Size: 55.6 MB (55615967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c01cb78ffdd6ef9f062f5d2a80e243e249de2447fd68e17c17b7a2938ed5cff`  
		Last Modified: Wed, 08 Mar 2023 21:27:24 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa238b7fd3ad0bf546c26574e4edcd1761584f55d8b338a7b0330399baae3e49`  
		Last Modified: Wed, 08 Mar 2023 21:27:31 GMT  
		Size: 51.0 MB (50982384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a86d0b8c1ccc4f969ad0e7b9fa57a409e360db176437a087a5fd9406b081691`  
		Last Modified: Wed, 08 Mar 2023 21:27:24 GMT  
		Size: 5.4 KB (5388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:326b54668f8b18657ed13771324644998d14801db082e346aad6c8dd67aecb51`  
		Last Modified: Wed, 08 Mar 2023 21:27:24 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
