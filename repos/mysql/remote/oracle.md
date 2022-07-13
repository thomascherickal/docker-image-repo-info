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
