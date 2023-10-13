## `mariadb:jammy`

```console
$ docker pull mariadb@sha256:1094f2fcf0273e48ccfa1feb78dfc306631605f769008568be0c964e0c53b47b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `mariadb:jammy` - linux; amd64

```console
$ docker pull mariadb@sha256:e51c275914b2da5e8e8e0ed9eaecf1e4d5142b5e570f231224320001cf5c86cf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.3 MB (123281094 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f35870862d64d0e29598fba1d7f75cfefeb3f891cb22b3e2d4459c903e666554`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Thu, 05 Oct 2023 07:33:30 GMT
ARG RELEASE
# Thu, 05 Oct 2023 07:33:30 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 05 Oct 2023 07:33:30 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 05 Oct 2023 07:33:30 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 05 Oct 2023 07:33:32 GMT
ADD file:63d5ab3ef0aab308c0e71cb67292c5467f60deafa9b0418cbb220affcd078444 in / 
# Thu, 05 Oct 2023 07:33:32 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 09:41:34 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 13 Oct 2023 09:41:34 GMT
ENV GOSU_VERSION=1.14
# Fri, 13 Oct 2023 09:41:35 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 13 Oct 2023 09:41:53 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 13 Oct 2023 09:41:53 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 13 Oct 2023 09:41:54 GMT
ENV LANG=C.UTF-8
# Fri, 13 Oct 2023 09:41:54 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=11.1.2 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Fri, 13 Oct 2023 09:41:54 GMT
ARG MARIADB_VERSION=1:11.1.2+maria~ubu2204
# Fri, 13 Oct 2023 09:41:54 GMT
ENV MARIADB_VERSION=1:11.1.2+maria~ubu2204
# Fri, 13 Oct 2023 09:41:54 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-11.1.2/repo/ubuntu/ jammy main main/debug
# Fri, 13 Oct 2023 09:41:54 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.1.2/repo/ubuntu/ jammy main main/debug
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 13 Oct 2023 09:42:14 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.1.2/repo/ubuntu/ jammy main main/debug
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	mkdir -p /var/lib/mysql/mysql ; touch /var/lib/mysql/mysql/user.frm ; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql /etc/mysql/mariadb.conf.d/50-mariadb_safe.cnf; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Fri, 13 Oct 2023 09:42:15 GMT
VOLUME [/var/lib/mysql]
# Fri, 13 Oct 2023 09:42:15 GMT
COPY file:1980cab2a8b7fba7431710370aad263c40d659a4885e66510adf2002b57ddf4c in /usr/local/bin/healthcheck.sh 
# Fri, 13 Oct 2023 09:42:15 GMT
COPY file:41cd6c305128c82d238b47cc775ecf2262c7b95806428fa87026c43a3d858b56 in /usr/local/bin/ 
# Fri, 13 Oct 2023 09:42:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 13 Oct 2023 09:42:16 GMT
EXPOSE 3306
# Fri, 13 Oct 2023 09:42:16 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:43f89b94cd7df92a2f7e565b8fb1b7f502eff2cd225508cbd7ea2d36a9a3a601`  
		Last Modified: Thu, 05 Oct 2023 08:42:10 GMT  
		Size: 30.4 MB (30439111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfb413a01c7e51062c729f32b69c3b714877109c5af99249b5719195f5b47bde`  
		Last Modified: Fri, 13 Oct 2023 09:46:50 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d3f76b535d32df1e1b6d9991225a8d848a904dd369845b276143676d1f92d5e`  
		Last Modified: Fri, 13 Oct 2023 09:46:51 GMT  
		Size: 5.6 MB (5592621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7efd05ec01e5adc411f4cb915b9b08dc51606371b92e1f3b1a245dc4c5065cd`  
		Last Modified: Fri, 13 Oct 2023 09:46:48 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe2ff83c75dfda686e360e676c7b54eacd2ee02e8c05ce20bf4f2564e0cb80de`  
		Last Modified: Fri, 13 Oct 2023 09:46:48 GMT  
		Size: 332.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50ee0c078c9359ce827ce831452a58adbed812ec39bbaabdd3b05c6dfceff4c9`  
		Last Modified: Fri, 13 Oct 2023 09:47:00 GMT  
		Size: 87.2 MB (87235999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6975e72928bb27788719355cb8a8be77770490f10d36b34ba2c2f0a162e6f3de`  
		Last Modified: Fri, 13 Oct 2023 09:46:48 GMT  
		Size: 3.6 KB (3565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:561d1b426cbdc3b5787fcb4bff535a1361085d373e726eb975c673dd88d840c4`  
		Last Modified: Fri, 13 Oct 2023 09:46:48 GMT  
		Size: 7.6 KB (7569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:jammy` - linux; arm64 variant v8

```console
$ docker pull mariadb@sha256:25284a245c96dcbdf7a21a2fdd2b43dc2969b7d6114a40d8eadfb0245bdbff61
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.8 MB (117772793 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ffb1e17cd845f23ca803c00de3742e860ab9599d0fc52db8f30cb4d5e517a7ca`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Thu, 05 Oct 2023 07:32:20 GMT
ARG RELEASE
# Thu, 05 Oct 2023 07:32:21 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 05 Oct 2023 07:32:21 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 05 Oct 2023 07:32:21 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 05 Oct 2023 07:32:22 GMT
ADD file:f8594e26831508c318e42c8dfd9942041031087b8de1bf3fec11fd75b8b30fd4 in / 
# Thu, 05 Oct 2023 07:32:22 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 05:14:05 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 13 Oct 2023 05:14:05 GMT
ENV GOSU_VERSION=1.14
# Fri, 13 Oct 2023 05:14:05 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 13 Oct 2023 05:14:20 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 13 Oct 2023 05:14:21 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 13 Oct 2023 05:14:21 GMT
ENV LANG=C.UTF-8
# Fri, 13 Oct 2023 05:14:21 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=11.1.2 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Fri, 13 Oct 2023 05:14:21 GMT
ARG MARIADB_VERSION=1:11.1.2+maria~ubu2204
# Fri, 13 Oct 2023 05:14:21 GMT
ENV MARIADB_VERSION=1:11.1.2+maria~ubu2204
# Fri, 13 Oct 2023 05:14:21 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-11.1.2/repo/ubuntu/ jammy main main/debug
# Fri, 13 Oct 2023 05:14:22 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.1.2/repo/ubuntu/ jammy main main/debug
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 13 Oct 2023 05:14:43 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.1.2/repo/ubuntu/ jammy main main/debug
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	mkdir -p /var/lib/mysql/mysql ; touch /var/lib/mysql/mysql/user.frm ; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql /etc/mysql/mariadb.conf.d/50-mariadb_safe.cnf; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Fri, 13 Oct 2023 05:14:44 GMT
VOLUME [/var/lib/mysql]
# Fri, 13 Oct 2023 05:14:44 GMT
COPY file:1980cab2a8b7fba7431710370aad263c40d659a4885e66510adf2002b57ddf4c in /usr/local/bin/healthcheck.sh 
# Fri, 13 Oct 2023 05:14:44 GMT
COPY file:41cd6c305128c82d238b47cc775ecf2262c7b95806428fa87026c43a3d858b56 in /usr/local/bin/ 
# Fri, 13 Oct 2023 05:14:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 13 Oct 2023 05:14:44 GMT
EXPOSE 3306
# Fri, 13 Oct 2023 05:14:44 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:895d322e8e5957c04af3ab7b3431f2a562182d34167c6e159e02044150a66967`  
		Last Modified: Thu, 05 Oct 2023 08:57:30 GMT  
		Size: 28.4 MB (28391939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a51395918e98ab58b9872a4e3d0acb20194883f9e0b19a487c8719b50273668`  
		Last Modified: Fri, 13 Oct 2023 05:18:40 GMT  
		Size: 1.8 KB (1753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e9dc8b7a0af9ee9ad9e96d8cfcdbd553b7fd618bf4c714d7321f99e6df83091`  
		Last Modified: Fri, 13 Oct 2023 05:18:41 GMT  
		Size: 5.4 MB (5406605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae4c0a6d779e95ad9d374b8d1840c37c6c76984adb591108f05f2666b62a721c`  
		Last Modified: Fri, 13 Oct 2023 05:18:38 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4abfa2f57d4562f0b600e21f949c0d22f3e399826d7aa2f633170a6b3dd26ad3`  
		Last Modified: Fri, 13 Oct 2023 05:18:38 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:705550d68fde860171fab35c85b820d3a1eb4b476a43190979a28fb84bb419ea`  
		Last Modified: Fri, 13 Oct 2023 05:18:48 GMT  
		Size: 84.0 MB (83960894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec9df31fc22c4070be6615b62c4435790ed33dc1444a6144e71c4e7b29af8b01`  
		Last Modified: Fri, 13 Oct 2023 05:18:38 GMT  
		Size: 3.6 KB (3561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16773732efee950139647602f4d75c6027e51869a55269d6bd290ee189054f7e`  
		Last Modified: Fri, 13 Oct 2023 05:18:38 GMT  
		Size: 7.6 KB (7564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:jammy` - linux; ppc64le

```console
$ docker pull mariadb@sha256:c180356c6adce55e32012187009100e2e89ad4f316613124be258dacfa06aa9e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.6 MB (131636744 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b4f82d9a9a38c8ddc592c0953c705c4813e444f5754692a679368bdbcbb28c3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Thu, 05 Oct 2023 07:34:18 GMT
ARG RELEASE
# Thu, 05 Oct 2023 07:34:19 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 05 Oct 2023 07:34:19 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 05 Oct 2023 07:34:19 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 05 Oct 2023 07:34:22 GMT
ADD file:595ff761b2778bdc6bb59cbe8ce51c4a247e0f279ccd59a17b5be6cdeac0b4d2 in / 
# Thu, 05 Oct 2023 07:34:22 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 05:51:50 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 13 Oct 2023 05:51:51 GMT
ENV GOSU_VERSION=1.14
# Fri, 13 Oct 2023 05:51:52 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Fri, 13 Oct 2023 05:52:53 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 13 Oct 2023 05:52:55 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 13 Oct 2023 05:52:56 GMT
ENV LANG=C.UTF-8
# Fri, 13 Oct 2023 05:52:57 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=11.1.2 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Fri, 13 Oct 2023 05:52:58 GMT
ARG MARIADB_VERSION=1:11.1.2+maria~ubu2204
# Fri, 13 Oct 2023 05:52:59 GMT
ENV MARIADB_VERSION=1:11.1.2+maria~ubu2204
# Fri, 13 Oct 2023 05:53:02 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-11.1.2/repo/ubuntu/ jammy main main/debug
# Fri, 13 Oct 2023 05:53:07 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.1.2/repo/ubuntu/ jammy main main/debug
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Fri, 13 Oct 2023 05:55:02 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.1.2/repo/ubuntu/ jammy main main/debug
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	mkdir -p /var/lib/mysql/mysql ; touch /var/lib/mysql/mysql/user.frm ; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql /etc/mysql/mariadb.conf.d/50-mariadb_safe.cnf; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Fri, 13 Oct 2023 05:55:16 GMT
VOLUME [/var/lib/mysql]
# Fri, 13 Oct 2023 05:55:16 GMT
COPY file:1980cab2a8b7fba7431710370aad263c40d659a4885e66510adf2002b57ddf4c in /usr/local/bin/healthcheck.sh 
# Fri, 13 Oct 2023 05:55:17 GMT
COPY file:41cd6c305128c82d238b47cc775ecf2262c7b95806428fa87026c43a3d858b56 in /usr/local/bin/ 
# Fri, 13 Oct 2023 05:55:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 13 Oct 2023 05:55:19 GMT
EXPOSE 3306
# Fri, 13 Oct 2023 05:55:24 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:589c4cce1daa100afadbdbeda96025d02f85c117e0e60b70801af41b4e618668`  
		Last Modified: Fri, 13 Oct 2023 06:13:20 GMT  
		Size: 35.7 MB (35682793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5d05729d5870810fd32a20e53e5037ba79b46c20d6d9c38a2e8f68d254cd92f`  
		Last Modified: Fri, 13 Oct 2023 06:13:14 GMT  
		Size: 1.8 KB (1750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3bac9baac0aaa4bceb71d69ae160ff94fa53f97355bc41df349dfb19c47d677`  
		Last Modified: Fri, 13 Oct 2023 06:13:15 GMT  
		Size: 6.0 MB (6018289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed5e7d9fb45ffcf8e04c3e2cdb4f8ace9398f584596be8d3e0d1966fedd5d098`  
		Last Modified: Fri, 13 Oct 2023 06:13:12 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf581ebaeda1d9b107b00e16408de1c804c8bbcf3267d0a7c5d75cc99d80a109`  
		Last Modified: Fri, 13 Oct 2023 06:13:12 GMT  
		Size: 335.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a544ba3546e326904c8176059279a0aed099483cb47c91a9b25392f90d15f2c0`  
		Last Modified: Fri, 13 Oct 2023 06:13:27 GMT  
		Size: 89.9 MB (89922293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d42823d9e05383a744d26ecf73175b99f317c0838f5b477137b7d5125741196`  
		Last Modified: Fri, 13 Oct 2023 06:13:12 GMT  
		Size: 3.6 KB (3566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:377ea8ae4d1493c631d788a65225cb436e9232a5edab6b88fe658c407d161f77`  
		Last Modified: Fri, 13 Oct 2023 06:13:12 GMT  
		Size: 7.6 KB (7569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mariadb:jammy` - linux; s390x

```console
$ docker pull mariadb@sha256:30976184383065a3f89342d1b9af609ca171c938377016f576b7d2ef55d2262a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.8 MB (121768610 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad9fe009147a6a4bbcd3486d41074329423463f58cab97d101e0245ec6a13ef0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mariadbd"]`

```dockerfile
# Mon, 25 Sep 2023 10:17:26 GMT
ARG RELEASE
# Mon, 25 Sep 2023 10:17:26 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 25 Sep 2023 10:17:26 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 25 Sep 2023 10:17:26 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 25 Sep 2023 10:17:28 GMT
ADD file:78683f2464233172a7cd0d6adc4c7d9fb3ef05fa67ca22e6fbaca0325496a536 in / 
# Mon, 25 Sep 2023 10:17:28 GMT
CMD ["/bin/bash"]
# Tue, 03 Oct 2023 09:31:03 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Tue, 03 Oct 2023 09:31:03 GMT
ENV GOSU_VERSION=1.14
# Tue, 03 Oct 2023 09:31:03 GMT
ARG GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
# Tue, 03 Oct 2023 09:31:31 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN set -eux; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends 		ca-certificates 		gpg 		gpgv 		libjemalloc2 		pwgen 		tzdata 		xz-utils 		zstd ; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get install -y --no-install-recommends 		dirmngr 		gpg-agent 		wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -q -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -q -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	GNUPGHOME="$(mktemp -d)"; 	export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$GPG_KEYS" > /etc/apt/trusted.gpg.d/mariadb.gpg; 	if command -v gpgconf >/dev/null; then 		gpgconf --kill all; 	fi; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] ||	apt-mark manual $savedAptMark >/dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 03 Oct 2023 09:31:33 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 03 Oct 2023 09:31:33 GMT
ENV LANG=C.UTF-8
# Tue, 03 Oct 2023 09:31:33 GMT
LABEL org.opencontainers.image.authors=MariaDB Community org.opencontainers.image.title=MariaDB Database org.opencontainers.image.description=MariaDB Database for relational SQL org.opencontainers.image.documentation=https://hub.docker.com/_/mariadb/ org.opencontainers.image.base.name=docker.io/library/ubuntu:jammy org.opencontainers.image.licenses=GPL-2.0 org.opencontainers.image.source=https://github.com/MariaDB/mariadb-docker org.opencontainers.image.vendor=MariaDB Community org.opencontainers.image.version=11.1.2 org.opencontainers.image.url=https://github.com/MariaDB/mariadb-docker
# Tue, 03 Oct 2023 09:31:33 GMT
ARG MARIADB_VERSION=1:11.1.2+maria~ubu2204
# Tue, 03 Oct 2023 09:31:33 GMT
ENV MARIADB_VERSION=1:11.1.2+maria~ubu2204
# Tue, 03 Oct 2023 09:31:33 GMT
ARG REPOSITORY=http://archive.mariadb.org/mariadb-11.1.2/repo/ubuntu/ jammy main main/debug
# Tue, 03 Oct 2023 09:31:34 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.1.2/repo/ubuntu/ jammy main main/debug
RUN set -e;	echo "deb ${REPOSITORY}" > /etc/apt/sources.list.d/mariadb.list; 	{ 		echo 'Package: *'; 		echo 'Pin: release o=MariaDB'; 		echo 'Pin-Priority: 999'; 	} > /etc/apt/preferences.d/mariadb
# Tue, 03 Oct 2023 09:31:54 GMT
# ARGS: GPG_KEYS=177F4010FE56CA3336300305F1656F24C74CD1D8 REPOSITORY=http://archive.mariadb.org/mariadb-11.1.2/repo/ubuntu/ jammy main main/debug
RUN set -ex; 	{ 		echo "mariadb-server" mysql-server/root_password password 'unused'; 		echo "mariadb-server" mysql-server/root_password_again password 'unused'; 	} | debconf-set-selections; 	apt-get update; 	mkdir -p /var/lib/mysql/mysql ; touch /var/lib/mysql/mysql/user.frm ; 	apt-get install -y --no-install-recommends mariadb-server="$MARIADB_VERSION" mariadb-backup socat 	; 	rm -rf /var/lib/apt/lists/*; 	rm -rf /var/lib/mysql /etc/mysql/mariadb.conf.d/50-mariadb_safe.cnf; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown -R mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 777 /var/run/mysqld; 	find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log|user\s)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log|user\s)/#&/'; 	printf "[mariadb]\nhost-cache-size=0\nskip-name-resolve\n" > /etc/mysql/mariadb.conf.d/05-skipcache.cnf; 	if [ -L /etc/mysql/my.cnf ]; then 		sed -i -e '/includedir/ {N;s/\(.*\)\n\(.*\)/\n\2\n\1/}' /etc/mysql/mariadb.cnf; 	fi
# Tue, 03 Oct 2023 09:32:01 GMT
VOLUME [/var/lib/mysql]
# Tue, 03 Oct 2023 09:32:01 GMT
COPY file:1980cab2a8b7fba7431710370aad263c40d659a4885e66510adf2002b57ddf4c in /usr/local/bin/healthcheck.sh 
# Tue, 03 Oct 2023 09:32:01 GMT
COPY file:41cd6c305128c82d238b47cc775ecf2262c7b95806428fa87026c43a3d858b56 in /usr/local/bin/ 
# Tue, 03 Oct 2023 09:32:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 03 Oct 2023 09:32:01 GMT
EXPOSE 3306
# Tue, 03 Oct 2023 09:32:02 GMT
CMD ["mariadbd"]
```

-	Layers:
	-	`sha256:b6ba488997f9924c9473e547d56b3d4ae74495b1092ca3c613243185ee5d5151`  
		Last Modified: Tue, 03 Oct 2023 08:59:45 GMT  
		Size: 28.7 MB (28651983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8a584e32b3d82668c369c5ead9479789c0845cd03c048d06c629e06948c8c3a`  
		Last Modified: Tue, 03 Oct 2023 09:35:30 GMT  
		Size: 1.8 KB (1754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0259261f1fd94fd4f6b9fb280550d7cabf1025368c9c1d64ba1aaedd74d11ce3`  
		Last Modified: Tue, 03 Oct 2023 09:35:31 GMT  
		Size: 5.5 MB (5470761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e1e565b9ed21ee9724953ed0119d5ff978afdbf3700a11b406683478aba40aa`  
		Last Modified: Tue, 03 Oct 2023 09:35:28 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e52e9b934cc5a53bd0897e1c7a47862bfed6c7eea4ea975eb4a36f7c32d4104`  
		Last Modified: Tue, 03 Oct 2023 09:35:29 GMT  
		Size: 332.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a244d46f8cc1f8f6b66916e2a8219b3b2c347c1052d7e0018f63cbc033b6003`  
		Last Modified: Tue, 03 Oct 2023 09:35:41 GMT  
		Size: 87.6 MB (87632500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ae5d9b5686c7062600f0fa723d0d306b51661d86d37938fde6b16fc516e799a`  
		Last Modified: Tue, 03 Oct 2023 09:35:28 GMT  
		Size: 3.6 KB (3565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:045ff0dd4c6e6dfd21e1cd14ea28a1547171daee59694687a9e858ac75053cef`  
		Last Modified: Tue, 03 Oct 2023 09:35:28 GMT  
		Size: 7.6 KB (7566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
