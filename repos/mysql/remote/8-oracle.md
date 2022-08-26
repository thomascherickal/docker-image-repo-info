## `mysql:8-oracle`

```console
$ docker pull mysql@sha256:9323fe0e2893e2a8acff14f866616d8a519653069dbec411e7d6bf0f83b22dcc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:6964c211b5fadfc3b6a84986cbd3c78418b091c2fd44074f58d9c15d9b0f5f52
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.8 MB (132816933 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70325c69f1fe76e7f4e62e62fb5ef4e76acb45935075cec7b4cb42a928fef78a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 26 Aug 2022 21:25:57 GMT
ADD file:923c2af16ef366fe4e85b8ba8979b8a31da0cdbc606c08148463849bf66c395b in / 
# Fri, 26 Aug 2022 21:25:57 GMT
CMD ["/bin/bash"]
# Fri, 26 Aug 2022 21:55:56 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Fri, 26 Aug 2022 21:55:56 GMT
ENV GOSU_VERSION=1.14
# Fri, 26 Aug 2022 21:56:00 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 26 Aug 2022 21:56:22 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Fri, 26 Aug 2022 21:56:23 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Fri, 26 Aug 2022 21:56:23 GMT
ENV MYSQL_MAJOR=8.0
# Fri, 26 Aug 2022 21:56:24 GMT
ENV MYSQL_VERSION=8.0.30-1.el8
# Fri, 26 Aug 2022 21:56:24 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Fri, 26 Aug 2022 21:56:53 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Fri, 26 Aug 2022 21:56:54 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Fri, 26 Aug 2022 21:56:54 GMT
ENV MYSQL_SHELL_VERSION=8.0.30-1.el8
# Fri, 26 Aug 2022 21:57:24 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Fri, 26 Aug 2022 21:57:25 GMT
VOLUME [/var/lib/mysql]
# Fri, 26 Aug 2022 21:57:25 GMT
COPY file:5e84598933ec95c9918378d8dde5be8d5f80b0e1fc321a029f840f313201ebce in /usr/local/bin/ 
# Fri, 26 Aug 2022 21:57:25 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 26 Aug 2022 21:57:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Aug 2022 21:57:26 GMT
EXPOSE 3306 33060
# Fri, 26 Aug 2022 21:57:26 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:ee4ca39e1b6ea333d785f1cbc6b64b874a4f16f1200dad9e17d2015c925d1d57`  
		Last Modified: Fri, 26 Aug 2022 21:27:39 GMT  
		Size: 39.5 MB (39520501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55731ee5cc27ced42a0ea701da6c01ea54436624a61249e930ac796f0d539a25`  
		Last Modified: Fri, 26 Aug 2022 21:58:10 GMT  
		Size: 886.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3fd4ba8837dcaaf863ffc3ef194a0811c9a25271e9a6f8f97791f35311eb150`  
		Last Modified: Fri, 26 Aug 2022 21:58:10 GMT  
		Size: 928.8 KB (928832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfdb35add3bdb652fb29883c67fc10bd46a3fb0be64298abc066a4a06bb37115`  
		Last Modified: Fri, 26 Aug 2022 21:58:09 GMT  
		Size: 4.6 MB (4613200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb34f3e592a8dea4241df25f68119b066f2c978dfeb6af0e57b637bebf3b1a4e`  
		Last Modified: Fri, 26 Aug 2022 21:58:08 GMT  
		Size: 2.6 KB (2630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:961390a73dd279bcd61e333bc0319200dfb88add6a01deb2159d608df495cc39`  
		Last Modified: Fri, 26 Aug 2022 21:58:08 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:338d4f22364bc14c90f342e4cb8a945b9e0caf236cfec0b19cff3d702d7e01b2`  
		Last Modified: Fri, 26 Aug 2022 21:58:13 GMT  
		Size: 47.7 MB (47741816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:633ee7c9891570f248e85d04fe735e5574693fbb615ee5c36dd743c96df097fa`  
		Last Modified: Fri, 26 Aug 2022 21:58:06 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:961374a411ee16c47884f4887ba1ffce8e0bc51523a59ff121734a06ac8ca3a7`  
		Last Modified: Fri, 26 Aug 2022 21:58:13 GMT  
		Size: 40.0 MB (40002910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da93a12a127a0237fe8c07cb62f9228af9f799d0ef27e4825bf31914c52b276a`  
		Last Modified: Fri, 26 Aug 2022 21:58:06 GMT  
		Size: 5.4 KB (5388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6931149ad6ae8c447dce56977bfe1173a2197f264f3ccdee1e2bff7700a48ced`  
		Last Modified: Fri, 26 Aug 2022 21:58:06 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8-oracle` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:3867cc00238a77b6b083528b1f166aca1b583105e0512b2ed6f60f59058cf69d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.5 MB (141486259 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab84ad4f2f97f044d80f4bf012945d4c8d6042048b73271a47d93a3c08a1bbcc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 24 Aug 2022 19:54:55 GMT
ADD file:2016956ebf5b305d0029ca641d3175f879fb9c5f35f801b5c52927afeb8f8422 in / 
# Wed, 24 Aug 2022 19:54:56 GMT
CMD ["/bin/bash"]
# Wed, 24 Aug 2022 23:27:10 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 24 Aug 2022 23:27:11 GMT
ENV GOSU_VERSION=1.14
# Wed, 24 Aug 2022 23:27:15 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 24 Aug 2022 23:27:42 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Wed, 24 Aug 2022 23:27:44 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 24 Aug 2022 23:27:45 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 24 Aug 2022 23:27:46 GMT
ENV MYSQL_VERSION=8.0.30-1.el8
# Wed, 24 Aug 2022 23:27:47 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 24 Aug 2022 23:28:15 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 24 Aug 2022 23:28:16 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 24 Aug 2022 23:28:17 GMT
ENV MYSQL_SHELL_VERSION=8.0.30-1.el8
# Wed, 24 Aug 2022 23:28:50 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Wed, 24 Aug 2022 23:28:50 GMT
VOLUME [/var/lib/mysql]
# Wed, 24 Aug 2022 23:28:52 GMT
COPY file:5e84598933ec95c9918378d8dde5be8d5f80b0e1fc321a029f840f313201ebce in /usr/local/bin/ 
# Wed, 24 Aug 2022 23:28:52 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 24 Aug 2022 23:28:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 24 Aug 2022 23:28:54 GMT
EXPOSE 3306 33060
# Wed, 24 Aug 2022 23:28:55 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:4fad3655bea38b31843315fea6a076b3b13bee189d1b3d017cf9beb5feb39909`  
		Last Modified: Wed, 24 Aug 2022 19:56:49 GMT  
		Size: 38.3 MB (38320858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1489aec86f05309535ae29b2e7285f7ddba0b211836da72348539af0dd2d2379`  
		Last Modified: Wed, 24 Aug 2022 23:29:27 GMT  
		Size: 889.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e77d836384670fd3478d4cb657d41d327855d5dcc673df62f3927ed1efecfa4`  
		Last Modified: Wed, 24 Aug 2022 23:29:28 GMT  
		Size: 857.1 KB (857150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17790976537f48772d0403d40aaf852af07261cbf3d6110070668dbc8f25431f`  
		Last Modified: Wed, 24 Aug 2022 23:29:26 GMT  
		Size: 4.4 MB (4414507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33612199b4969498bbdcbddd62b16347eb14a67a2efbd1b181906fc74b5a2fb8`  
		Last Modified: Wed, 24 Aug 2022 23:29:25 GMT  
		Size: 2.6 KB (2608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b30b18c17cd9cfb053d6e6ae6ad6429a164076460b894f02f3b545e95383ebb0`  
		Last Modified: Wed, 24 Aug 2022 23:29:25 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17e4ac18a5976c9357cf9f1b4323b5b0a2986f2fb9b1a36e68c37c34593eaa94`  
		Last Modified: Wed, 24 Aug 2022 23:29:31 GMT  
		Size: 53.8 MB (53807224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78373903781864bd12a3e2f169bc0652de0c80da8c0a6e7c157ded33af01af6f`  
		Last Modified: Wed, 24 Aug 2022 23:29:23 GMT  
		Size: 319.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd1c3e38760bbc319c418e9108aa8822c95df8890183ffd9942644203ec93d16`  
		Last Modified: Wed, 24 Aug 2022 23:29:31 GMT  
		Size: 44.1 MB (44076861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d81f0e370f2f6604fa2568bec195f4d1bcdfe0862b75f1344dd40cd74fe9c30`  
		Last Modified: Wed, 24 Aug 2022 23:29:23 GMT  
		Size: 5.4 KB (5388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0deb86930a31d65f5259ad22853029d7ee86a1a80041881096b387cdb9ec7bec`  
		Last Modified: Wed, 24 Aug 2022 23:29:23 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
