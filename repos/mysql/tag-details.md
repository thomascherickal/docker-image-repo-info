<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `mysql`

-	[`mysql:8`](#mysql8)
-	[`mysql:8-oracle`](#mysql8-oracle)
-	[`mysql:8-oraclelinux8`](#mysql8-oraclelinux8)
-	[`mysql:8.0`](#mysql80)
-	[`mysql:8.0-bullseye`](#mysql80-bullseye)
-	[`mysql:8.0-debian`](#mysql80-debian)
-	[`mysql:8.0-oracle`](#mysql80-oracle)
-	[`mysql:8.0-oraclelinux8`](#mysql80-oraclelinux8)
-	[`mysql:8.0.35`](#mysql8035)
-	[`mysql:8.0.35-bullseye`](#mysql8035-bullseye)
-	[`mysql:8.0.35-debian`](#mysql8035-debian)
-	[`mysql:8.0.35-oracle`](#mysql8035-oracle)
-	[`mysql:8.0.35-oraclelinux8`](#mysql8035-oraclelinux8)
-	[`mysql:8.2`](#mysql82)
-	[`mysql:8.2-oracle`](#mysql82-oracle)
-	[`mysql:8.2-oraclelinux8`](#mysql82-oraclelinux8)
-	[`mysql:8.2.0`](#mysql820)
-	[`mysql:8.2.0-oracle`](#mysql820-oracle)
-	[`mysql:8.2.0-oraclelinux8`](#mysql820-oraclelinux8)
-	[`mysql:innovation`](#mysqlinnovation)
-	[`mysql:innovation-oracle`](#mysqlinnovation-oracle)
-	[`mysql:innovation-oraclelinux8`](#mysqlinnovation-oraclelinux8)
-	[`mysql:latest`](#mysqllatest)
-	[`mysql:oracle`](#mysqloracle)
-	[`mysql:oraclelinux8`](#mysqloraclelinux8)

## `mysql:8`

```console
$ docker pull mysql@sha256:2d82ba6960cdf254de13f57d7265570c0675bc8bae1051e4a9806cff863006c9
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `mysql:8` - linux; amd64

```console
$ docker pull mysql@sha256:28a16e31b140d750048cd5fadcaed22ac08d0eeb18567f79f822aee1f237b43c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **181.6 MB (181572393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73246731c4b01c19b8713c6408c6c5d898ac04f75f2a4ce998930f12091542f2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 18 Dec 2023 23:06:09 GMT
ADD file:da89b67e484bc45f357250a868fd78e28086b13e4315635d19648e5d43812e89 in / 
# Mon, 18 Dec 2023 23:06:09 GMT
CMD ["/bin/bash"]
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV GOSU_VERSION=1.16
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME" # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_MAJOR=innovation
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_VERSION=8.2.0-1.el8
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eu; 	{ 		echo '[mysqlinnovation-server-minimal]'; 		echo 'name=MySQL innovation Server Minimal'; 		echo 'enabled=1'; 		echo 'baseurl=https://repo.mysql.com/yum/mysql-innovation-community/docker/el/8/$basearch/'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eu; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo 'baseurl=https://repo.mysql.com/yum/mysql-tools-innovation-community/el/8/$basearch/'; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_SHELL_VERSION=8.2.1-1.el8
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
VOLUME [/var/lib/mysql]
# Mon, 18 Dec 2023 23:06:09 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 18 Dec 2023 23:06:09 GMT
EXPOSE map[3306/tcp:{} 33060/tcp:{}]
# Mon, 18 Dec 2023 23:06:09 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:bce031bc522d421fb188ef82a530f85c5477bb87cdeacdb911ea86f3f7cd3b66`  
		Last Modified: Wed, 20 Dec 2023 22:42:00 GMT  
		Size: 51.3 MB (51323468 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cf7e9f463619cbda1168fb597e71ce50b4ecd4546ad74050f5b5c67a152ca249`  
		Last Modified: Thu, 21 Dec 2023 00:41:48 GMT  
		Size: 883.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:105f403783c74e137d330ef98facdded2cab753187765ed8c453bb7b061a0002`  
		Last Modified: Thu, 21 Dec 2023 00:41:48 GMT  
		Size: 982.8 KB (982809 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:878e53a613d8011ad3d6207863d1555fe571430d3c6f7659d1eb0fd7f28ba7de`  
		Last Modified: Thu, 21 Dec 2023 00:41:48 GMT  
		Size: 4.6 MB (4594819 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2a362044e79fb6669726216e996a0a9fa018ba304d75ac30c9378a93160182de`  
		Last Modified: Thu, 21 Dec 2023 00:41:48 GMT  
		Size: 2.6 KB (2608 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6e4df4f73cfe883156b974e5269c673e52de0e1a56d610f2974793cd52d8b043`  
		Last Modified: Thu, 21 Dec 2023 00:41:49 GMT  
		Size: 340.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:69263d6347550e51a3b3f972d5aee303fd3c8c6d75376aad0b4cdcd4cb3f83be`  
		Last Modified: Thu, 21 Dec 2023 00:41:49 GMT  
		Size: 62.6 MB (62574253 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fe5e855492024c60c48d8eb006c94b71d6622f6d5c741cfa611e571a88a67d37`  
		Last Modified: Thu, 21 Dec 2023 00:41:49 GMT  
		Size: 325.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5c02229ce6f164ee6c47c91ddaa42db249b197b8b28dc6814a4df879a4f96a3e`  
		Last Modified: Thu, 21 Dec 2023 00:41:50 GMT  
		Size: 62.1 MB (62087711 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7320aa32bf42c0642bc86e30dac0b10335258a24b6ba374e173918ba8d9f9f63`  
		Last Modified: Thu, 21 Dec 2023 00:41:49 GMT  
		Size: 5.2 KB (5177 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:8` - unknown; unknown

```console
$ docker pull mysql@sha256:483bf8eb111365bf322a25443d3f96ae0d80829c60f00fb329d8a0de0f21c6e7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.6 MB (11608021 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:501f9b1df36151d7e7ebba69fac20d69995d956d3851313ac3b4fdf9fa4e9ad3`

```dockerfile
```

-	Layers:
	-	`sha256:8de9290b82bb48a07e68ea96148c288ffa09729055d5c506b7690cf42f948baf`  
		Last Modified: Thu, 21 Dec 2023 00:41:48 GMT  
		Size: 11.6 MB (11573114 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:0b8a63c307592189c7a4ea188ee3b5e76eba99edc475a34c635157d5e893e536`  
		Last Modified: Thu, 21 Dec 2023 00:41:48 GMT  
		Size: 34.9 KB (34907 bytes)  
		MIME: application/vnd.in-toto+json

### `mysql:8` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:86f5987d89514a0ec8043202ba341717c6d2f726749924ef7f220839ac576cf8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **185.3 MB (185275916 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e963a4c2b1a0d8774a4b6138a86d2bcca8b8f5cec58fbfabf7ae4ae021159e0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 06 Dec 2023 19:42:27 GMT
ADD file:f5ee75151bd25b33e72aa4c0560815f35f6e662876bf3733a02e5cb970227358 in / 
# Wed, 06 Dec 2023 19:42:27 GMT
CMD ["/bin/bash"]
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV GOSU_VERSION=1.16
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME" # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_MAJOR=innovation
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_VERSION=8.2.0-1.el8
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eu; 	{ 		echo '[mysqlinnovation-server-minimal]'; 		echo 'name=MySQL innovation Server Minimal'; 		echo 'enabled=1'; 		echo 'baseurl=https://repo.mysql.com/yum/mysql-innovation-community/docker/el/8/$basearch/'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eu; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo 'baseurl=https://repo.mysql.com/yum/mysql-tools-innovation-community/el/8/$basearch/'; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_SHELL_VERSION=8.2.1-1.el8
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
VOLUME [/var/lib/mysql]
# Mon, 18 Dec 2023 23:06:09 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 18 Dec 2023 23:06:09 GMT
EXPOSE map[3306/tcp:{} 33060/tcp:{}]
# Mon, 18 Dec 2023 23:06:09 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:edfaa6c9daada52a737333e0818f3d697d745aab3f3351e773218a524ebc9e53`  
		Last Modified: Wed, 06 Dec 2023 19:43:23 GMT  
		Size: 50.1 MB (50072545 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:19c686b91aca61da8058a44e9f6aa06cbb27aa65cf2db0768377bcc6899dc0c2`  
		Last Modified: Thu, 14 Dec 2023 20:15:05 GMT  
		Size: 885.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8c39062282e36f6169d219352cb19810ac7506e408e89b4ef33c400903a6ecc1`  
		Last Modified: Thu, 14 Dec 2023 20:15:05 GMT  
		Size: 913.0 KB (912965 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:73452dd561ff872804f5a63faab7552647c80c8a399e834fe154707a48613b20`  
		Last Modified: Thu, 14 Dec 2023 20:15:05 GMT  
		Size: 4.3 MB (4300794 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0ba54e261f50c32496de78ff38c42eb03cb97850ddbeb3c96f4fe34ea1cb23bc`  
		Last Modified: Thu, 14 Dec 2023 20:15:05 GMT  
		Size: 2.6 KB (2609 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b22c0fd6cce4772b17fe2500d6ce97e3a35076112226cc23269afa1542f7b51d`  
		Last Modified: Thu, 14 Dec 2023 20:15:06 GMT  
		Size: 340.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:eaffd91cbb1278d374c5b91f8a3e87239e73b0113a1fa5835faf13bcb05948dc`  
		Last Modified: Thu, 14 Dec 2023 20:15:09 GMT  
		Size: 61.6 MB (61602995 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3ec60922d8e9eefbce5167faf6f2296ddec22dcafc9a84f5db6f94e92e032089`  
		Last Modified: Thu, 14 Dec 2023 20:15:07 GMT  
		Size: 325.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:942dbd5bb0a98d45556f650aa3174e3e4a5fcf822e5e7a67529ae622bb02b14a`  
		Last Modified: Thu, 14 Dec 2023 20:15:09 GMT  
		Size: 68.4 MB (68377279 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bc7ea546f5793dcfecf365aefc956d7999a086211dc195cbb5d73d09df397fe2`  
		Last Modified: Tue, 19 Dec 2023 21:07:09 GMT  
		Size: 5.2 KB (5179 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:8` - unknown; unknown

```console
$ docker pull mysql@sha256:9b1966fea33a8f487098b70ebc30c23b2700a8731bcff2bd124779ba2f8cf2be
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.6 MB (11606464 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:557704055f52c52ae3fcc218fa7168216870eca8326c1b1e89d434ad3ec00204`

```dockerfile
```

-	Layers:
	-	`sha256:0b211226c249aefed58e7da4b41bb3219beb5345fe5ed4e65c65ab47e378292b`  
		Last Modified: Tue, 19 Dec 2023 21:07:09 GMT  
		Size: 11.6 MB (11571692 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:097024790a6d6019cd411ce0478476fbfebc733402110550a33d6009f3aca07d`  
		Last Modified: Tue, 19 Dec 2023 21:07:09 GMT  
		Size: 34.8 KB (34772 bytes)  
		MIME: application/vnd.in-toto+json

## `mysql:8-oracle`

```console
$ docker pull mysql@sha256:2d82ba6960cdf254de13f57d7265570c0675bc8bae1051e4a9806cff863006c9
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `mysql:8-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:28a16e31b140d750048cd5fadcaed22ac08d0eeb18567f79f822aee1f237b43c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **181.6 MB (181572393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73246731c4b01c19b8713c6408c6c5d898ac04f75f2a4ce998930f12091542f2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 18 Dec 2023 23:06:09 GMT
ADD file:da89b67e484bc45f357250a868fd78e28086b13e4315635d19648e5d43812e89 in / 
# Mon, 18 Dec 2023 23:06:09 GMT
CMD ["/bin/bash"]
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV GOSU_VERSION=1.16
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME" # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_MAJOR=innovation
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_VERSION=8.2.0-1.el8
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eu; 	{ 		echo '[mysqlinnovation-server-minimal]'; 		echo 'name=MySQL innovation Server Minimal'; 		echo 'enabled=1'; 		echo 'baseurl=https://repo.mysql.com/yum/mysql-innovation-community/docker/el/8/$basearch/'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eu; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo 'baseurl=https://repo.mysql.com/yum/mysql-tools-innovation-community/el/8/$basearch/'; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_SHELL_VERSION=8.2.1-1.el8
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
VOLUME [/var/lib/mysql]
# Mon, 18 Dec 2023 23:06:09 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 18 Dec 2023 23:06:09 GMT
EXPOSE map[3306/tcp:{} 33060/tcp:{}]
# Mon, 18 Dec 2023 23:06:09 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:bce031bc522d421fb188ef82a530f85c5477bb87cdeacdb911ea86f3f7cd3b66`  
		Last Modified: Wed, 20 Dec 2023 22:42:00 GMT  
		Size: 51.3 MB (51323468 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cf7e9f463619cbda1168fb597e71ce50b4ecd4546ad74050f5b5c67a152ca249`  
		Last Modified: Thu, 21 Dec 2023 00:41:48 GMT  
		Size: 883.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:105f403783c74e137d330ef98facdded2cab753187765ed8c453bb7b061a0002`  
		Last Modified: Thu, 21 Dec 2023 00:41:48 GMT  
		Size: 982.8 KB (982809 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:878e53a613d8011ad3d6207863d1555fe571430d3c6f7659d1eb0fd7f28ba7de`  
		Last Modified: Thu, 21 Dec 2023 00:41:48 GMT  
		Size: 4.6 MB (4594819 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2a362044e79fb6669726216e996a0a9fa018ba304d75ac30c9378a93160182de`  
		Last Modified: Thu, 21 Dec 2023 00:41:48 GMT  
		Size: 2.6 KB (2608 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6e4df4f73cfe883156b974e5269c673e52de0e1a56d610f2974793cd52d8b043`  
		Last Modified: Thu, 21 Dec 2023 00:41:49 GMT  
		Size: 340.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:69263d6347550e51a3b3f972d5aee303fd3c8c6d75376aad0b4cdcd4cb3f83be`  
		Last Modified: Thu, 21 Dec 2023 00:41:49 GMT  
		Size: 62.6 MB (62574253 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fe5e855492024c60c48d8eb006c94b71d6622f6d5c741cfa611e571a88a67d37`  
		Last Modified: Thu, 21 Dec 2023 00:41:49 GMT  
		Size: 325.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5c02229ce6f164ee6c47c91ddaa42db249b197b8b28dc6814a4df879a4f96a3e`  
		Last Modified: Thu, 21 Dec 2023 00:41:50 GMT  
		Size: 62.1 MB (62087711 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7320aa32bf42c0642bc86e30dac0b10335258a24b6ba374e173918ba8d9f9f63`  
		Last Modified: Thu, 21 Dec 2023 00:41:49 GMT  
		Size: 5.2 KB (5177 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:8-oracle` - unknown; unknown

```console
$ docker pull mysql@sha256:483bf8eb111365bf322a25443d3f96ae0d80829c60f00fb329d8a0de0f21c6e7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.6 MB (11608021 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:501f9b1df36151d7e7ebba69fac20d69995d956d3851313ac3b4fdf9fa4e9ad3`

```dockerfile
```

-	Layers:
	-	`sha256:8de9290b82bb48a07e68ea96148c288ffa09729055d5c506b7690cf42f948baf`  
		Last Modified: Thu, 21 Dec 2023 00:41:48 GMT  
		Size: 11.6 MB (11573114 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:0b8a63c307592189c7a4ea188ee3b5e76eba99edc475a34c635157d5e893e536`  
		Last Modified: Thu, 21 Dec 2023 00:41:48 GMT  
		Size: 34.9 KB (34907 bytes)  
		MIME: application/vnd.in-toto+json

### `mysql:8-oracle` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:86f5987d89514a0ec8043202ba341717c6d2f726749924ef7f220839ac576cf8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **185.3 MB (185275916 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e963a4c2b1a0d8774a4b6138a86d2bcca8b8f5cec58fbfabf7ae4ae021159e0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 06 Dec 2023 19:42:27 GMT
ADD file:f5ee75151bd25b33e72aa4c0560815f35f6e662876bf3733a02e5cb970227358 in / 
# Wed, 06 Dec 2023 19:42:27 GMT
CMD ["/bin/bash"]
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV GOSU_VERSION=1.16
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME" # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_MAJOR=innovation
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_VERSION=8.2.0-1.el8
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eu; 	{ 		echo '[mysqlinnovation-server-minimal]'; 		echo 'name=MySQL innovation Server Minimal'; 		echo 'enabled=1'; 		echo 'baseurl=https://repo.mysql.com/yum/mysql-innovation-community/docker/el/8/$basearch/'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eu; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo 'baseurl=https://repo.mysql.com/yum/mysql-tools-innovation-community/el/8/$basearch/'; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_SHELL_VERSION=8.2.1-1.el8
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
VOLUME [/var/lib/mysql]
# Mon, 18 Dec 2023 23:06:09 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 18 Dec 2023 23:06:09 GMT
EXPOSE map[3306/tcp:{} 33060/tcp:{}]
# Mon, 18 Dec 2023 23:06:09 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:edfaa6c9daada52a737333e0818f3d697d745aab3f3351e773218a524ebc9e53`  
		Last Modified: Wed, 06 Dec 2023 19:43:23 GMT  
		Size: 50.1 MB (50072545 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:19c686b91aca61da8058a44e9f6aa06cbb27aa65cf2db0768377bcc6899dc0c2`  
		Last Modified: Thu, 14 Dec 2023 20:15:05 GMT  
		Size: 885.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8c39062282e36f6169d219352cb19810ac7506e408e89b4ef33c400903a6ecc1`  
		Last Modified: Thu, 14 Dec 2023 20:15:05 GMT  
		Size: 913.0 KB (912965 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:73452dd561ff872804f5a63faab7552647c80c8a399e834fe154707a48613b20`  
		Last Modified: Thu, 14 Dec 2023 20:15:05 GMT  
		Size: 4.3 MB (4300794 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0ba54e261f50c32496de78ff38c42eb03cb97850ddbeb3c96f4fe34ea1cb23bc`  
		Last Modified: Thu, 14 Dec 2023 20:15:05 GMT  
		Size: 2.6 KB (2609 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b22c0fd6cce4772b17fe2500d6ce97e3a35076112226cc23269afa1542f7b51d`  
		Last Modified: Thu, 14 Dec 2023 20:15:06 GMT  
		Size: 340.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:eaffd91cbb1278d374c5b91f8a3e87239e73b0113a1fa5835faf13bcb05948dc`  
		Last Modified: Thu, 14 Dec 2023 20:15:09 GMT  
		Size: 61.6 MB (61602995 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3ec60922d8e9eefbce5167faf6f2296ddec22dcafc9a84f5db6f94e92e032089`  
		Last Modified: Thu, 14 Dec 2023 20:15:07 GMT  
		Size: 325.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:942dbd5bb0a98d45556f650aa3174e3e4a5fcf822e5e7a67529ae622bb02b14a`  
		Last Modified: Thu, 14 Dec 2023 20:15:09 GMT  
		Size: 68.4 MB (68377279 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bc7ea546f5793dcfecf365aefc956d7999a086211dc195cbb5d73d09df397fe2`  
		Last Modified: Tue, 19 Dec 2023 21:07:09 GMT  
		Size: 5.2 KB (5179 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:8-oracle` - unknown; unknown

```console
$ docker pull mysql@sha256:9b1966fea33a8f487098b70ebc30c23b2700a8731bcff2bd124779ba2f8cf2be
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.6 MB (11606464 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:557704055f52c52ae3fcc218fa7168216870eca8326c1b1e89d434ad3ec00204`

```dockerfile
```

-	Layers:
	-	`sha256:0b211226c249aefed58e7da4b41bb3219beb5345fe5ed4e65c65ab47e378292b`  
		Last Modified: Tue, 19 Dec 2023 21:07:09 GMT  
		Size: 11.6 MB (11571692 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:097024790a6d6019cd411ce0478476fbfebc733402110550a33d6009f3aca07d`  
		Last Modified: Tue, 19 Dec 2023 21:07:09 GMT  
		Size: 34.8 KB (34772 bytes)  
		MIME: application/vnd.in-toto+json

## `mysql:8-oraclelinux8`

```console
$ docker pull mysql@sha256:2d82ba6960cdf254de13f57d7265570c0675bc8bae1051e4a9806cff863006c9
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `mysql:8-oraclelinux8` - linux; amd64

```console
$ docker pull mysql@sha256:28a16e31b140d750048cd5fadcaed22ac08d0eeb18567f79f822aee1f237b43c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **181.6 MB (181572393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73246731c4b01c19b8713c6408c6c5d898ac04f75f2a4ce998930f12091542f2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 18 Dec 2023 23:06:09 GMT
ADD file:da89b67e484bc45f357250a868fd78e28086b13e4315635d19648e5d43812e89 in / 
# Mon, 18 Dec 2023 23:06:09 GMT
CMD ["/bin/bash"]
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV GOSU_VERSION=1.16
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME" # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_MAJOR=innovation
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_VERSION=8.2.0-1.el8
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eu; 	{ 		echo '[mysqlinnovation-server-minimal]'; 		echo 'name=MySQL innovation Server Minimal'; 		echo 'enabled=1'; 		echo 'baseurl=https://repo.mysql.com/yum/mysql-innovation-community/docker/el/8/$basearch/'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eu; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo 'baseurl=https://repo.mysql.com/yum/mysql-tools-innovation-community/el/8/$basearch/'; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_SHELL_VERSION=8.2.1-1.el8
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
VOLUME [/var/lib/mysql]
# Mon, 18 Dec 2023 23:06:09 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 18 Dec 2023 23:06:09 GMT
EXPOSE map[3306/tcp:{} 33060/tcp:{}]
# Mon, 18 Dec 2023 23:06:09 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:bce031bc522d421fb188ef82a530f85c5477bb87cdeacdb911ea86f3f7cd3b66`  
		Last Modified: Wed, 20 Dec 2023 22:42:00 GMT  
		Size: 51.3 MB (51323468 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cf7e9f463619cbda1168fb597e71ce50b4ecd4546ad74050f5b5c67a152ca249`  
		Last Modified: Thu, 21 Dec 2023 00:41:48 GMT  
		Size: 883.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:105f403783c74e137d330ef98facdded2cab753187765ed8c453bb7b061a0002`  
		Last Modified: Thu, 21 Dec 2023 00:41:48 GMT  
		Size: 982.8 KB (982809 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:878e53a613d8011ad3d6207863d1555fe571430d3c6f7659d1eb0fd7f28ba7de`  
		Last Modified: Thu, 21 Dec 2023 00:41:48 GMT  
		Size: 4.6 MB (4594819 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2a362044e79fb6669726216e996a0a9fa018ba304d75ac30c9378a93160182de`  
		Last Modified: Thu, 21 Dec 2023 00:41:48 GMT  
		Size: 2.6 KB (2608 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6e4df4f73cfe883156b974e5269c673e52de0e1a56d610f2974793cd52d8b043`  
		Last Modified: Thu, 21 Dec 2023 00:41:49 GMT  
		Size: 340.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:69263d6347550e51a3b3f972d5aee303fd3c8c6d75376aad0b4cdcd4cb3f83be`  
		Last Modified: Thu, 21 Dec 2023 00:41:49 GMT  
		Size: 62.6 MB (62574253 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fe5e855492024c60c48d8eb006c94b71d6622f6d5c741cfa611e571a88a67d37`  
		Last Modified: Thu, 21 Dec 2023 00:41:49 GMT  
		Size: 325.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5c02229ce6f164ee6c47c91ddaa42db249b197b8b28dc6814a4df879a4f96a3e`  
		Last Modified: Thu, 21 Dec 2023 00:41:50 GMT  
		Size: 62.1 MB (62087711 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7320aa32bf42c0642bc86e30dac0b10335258a24b6ba374e173918ba8d9f9f63`  
		Last Modified: Thu, 21 Dec 2023 00:41:49 GMT  
		Size: 5.2 KB (5177 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:8-oraclelinux8` - unknown; unknown

```console
$ docker pull mysql@sha256:483bf8eb111365bf322a25443d3f96ae0d80829c60f00fb329d8a0de0f21c6e7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.6 MB (11608021 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:501f9b1df36151d7e7ebba69fac20d69995d956d3851313ac3b4fdf9fa4e9ad3`

```dockerfile
```

-	Layers:
	-	`sha256:8de9290b82bb48a07e68ea96148c288ffa09729055d5c506b7690cf42f948baf`  
		Last Modified: Thu, 21 Dec 2023 00:41:48 GMT  
		Size: 11.6 MB (11573114 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:0b8a63c307592189c7a4ea188ee3b5e76eba99edc475a34c635157d5e893e536`  
		Last Modified: Thu, 21 Dec 2023 00:41:48 GMT  
		Size: 34.9 KB (34907 bytes)  
		MIME: application/vnd.in-toto+json

### `mysql:8-oraclelinux8` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:86f5987d89514a0ec8043202ba341717c6d2f726749924ef7f220839ac576cf8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **185.3 MB (185275916 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e963a4c2b1a0d8774a4b6138a86d2bcca8b8f5cec58fbfabf7ae4ae021159e0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 06 Dec 2023 19:42:27 GMT
ADD file:f5ee75151bd25b33e72aa4c0560815f35f6e662876bf3733a02e5cb970227358 in / 
# Wed, 06 Dec 2023 19:42:27 GMT
CMD ["/bin/bash"]
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV GOSU_VERSION=1.16
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME" # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_MAJOR=innovation
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_VERSION=8.2.0-1.el8
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eu; 	{ 		echo '[mysqlinnovation-server-minimal]'; 		echo 'name=MySQL innovation Server Minimal'; 		echo 'enabled=1'; 		echo 'baseurl=https://repo.mysql.com/yum/mysql-innovation-community/docker/el/8/$basearch/'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eu; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo 'baseurl=https://repo.mysql.com/yum/mysql-tools-innovation-community/el/8/$basearch/'; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_SHELL_VERSION=8.2.1-1.el8
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
VOLUME [/var/lib/mysql]
# Mon, 18 Dec 2023 23:06:09 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 18 Dec 2023 23:06:09 GMT
EXPOSE map[3306/tcp:{} 33060/tcp:{}]
# Mon, 18 Dec 2023 23:06:09 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:edfaa6c9daada52a737333e0818f3d697d745aab3f3351e773218a524ebc9e53`  
		Last Modified: Wed, 06 Dec 2023 19:43:23 GMT  
		Size: 50.1 MB (50072545 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:19c686b91aca61da8058a44e9f6aa06cbb27aa65cf2db0768377bcc6899dc0c2`  
		Last Modified: Thu, 14 Dec 2023 20:15:05 GMT  
		Size: 885.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8c39062282e36f6169d219352cb19810ac7506e408e89b4ef33c400903a6ecc1`  
		Last Modified: Thu, 14 Dec 2023 20:15:05 GMT  
		Size: 913.0 KB (912965 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:73452dd561ff872804f5a63faab7552647c80c8a399e834fe154707a48613b20`  
		Last Modified: Thu, 14 Dec 2023 20:15:05 GMT  
		Size: 4.3 MB (4300794 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0ba54e261f50c32496de78ff38c42eb03cb97850ddbeb3c96f4fe34ea1cb23bc`  
		Last Modified: Thu, 14 Dec 2023 20:15:05 GMT  
		Size: 2.6 KB (2609 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b22c0fd6cce4772b17fe2500d6ce97e3a35076112226cc23269afa1542f7b51d`  
		Last Modified: Thu, 14 Dec 2023 20:15:06 GMT  
		Size: 340.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:eaffd91cbb1278d374c5b91f8a3e87239e73b0113a1fa5835faf13bcb05948dc`  
		Last Modified: Thu, 14 Dec 2023 20:15:09 GMT  
		Size: 61.6 MB (61602995 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3ec60922d8e9eefbce5167faf6f2296ddec22dcafc9a84f5db6f94e92e032089`  
		Last Modified: Thu, 14 Dec 2023 20:15:07 GMT  
		Size: 325.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:942dbd5bb0a98d45556f650aa3174e3e4a5fcf822e5e7a67529ae622bb02b14a`  
		Last Modified: Thu, 14 Dec 2023 20:15:09 GMT  
		Size: 68.4 MB (68377279 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bc7ea546f5793dcfecf365aefc956d7999a086211dc195cbb5d73d09df397fe2`  
		Last Modified: Tue, 19 Dec 2023 21:07:09 GMT  
		Size: 5.2 KB (5179 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:8-oraclelinux8` - unknown; unknown

```console
$ docker pull mysql@sha256:9b1966fea33a8f487098b70ebc30c23b2700a8731bcff2bd124779ba2f8cf2be
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.6 MB (11606464 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:557704055f52c52ae3fcc218fa7168216870eca8326c1b1e89d434ad3ec00204`

```dockerfile
```

-	Layers:
	-	`sha256:0b211226c249aefed58e7da4b41bb3219beb5345fe5ed4e65c65ab47e378292b`  
		Last Modified: Tue, 19 Dec 2023 21:07:09 GMT  
		Size: 11.6 MB (11571692 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:097024790a6d6019cd411ce0478476fbfebc733402110550a33d6009f3aca07d`  
		Last Modified: Tue, 19 Dec 2023 21:07:09 GMT  
		Size: 34.8 KB (34772 bytes)  
		MIME: application/vnd.in-toto+json

## `mysql:8.0`

```console
$ docker pull mysql@sha256:c80ef5968b6baf12e9ba95412d4725971207228e5274518db92e26d0e169372b
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `mysql:8.0` - linux; amd64

```console
$ docker pull mysql@sha256:3a0b76a2ee46a23fc8e0c5e2d38d016a8466bbc774c933d719ae0b5308982dba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **173.7 MB (173728874 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba048db12589d011b77ab3ea33b7010d0b549214c8baa5fd885e4af84887928f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 18 Dec 2023 23:06:09 GMT
ADD file:da89b67e484bc45f357250a868fd78e28086b13e4315635d19648e5d43812e89 in / 
# Mon, 18 Dec 2023 23:06:09 GMT
CMD ["/bin/bash"]
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV GOSU_VERSION=1.16
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME" # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_MAJOR=8.0
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_VERSION=8.0.35-1.el8
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eu; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo 'baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/8/$basearch/'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eu; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo 'baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/8/$basearch/'; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_SHELL_VERSION=8.0.35-1.el8
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
VOLUME [/var/lib/mysql]
# Mon, 18 Dec 2023 23:06:09 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 18 Dec 2023 23:06:09 GMT
EXPOSE map[3306/tcp:{} 33060/tcp:{}]
# Mon, 18 Dec 2023 23:06:09 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:bce031bc522d421fb188ef82a530f85c5477bb87cdeacdb911ea86f3f7cd3b66`  
		Last Modified: Wed, 20 Dec 2023 22:42:00 GMT  
		Size: 51.3 MB (51323468 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9d95fc125cf8067473c7c0aeb06cc55f45268807b23568fbc3f14cab35d285cf`  
		Last Modified: Thu, 21 Dec 2023 00:42:07 GMT  
		Size: 890.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:22412d6d690fcd08a40e3808538b28c8ff614ca7d4292b97f91862c7d90f8279`  
		Last Modified: Thu, 21 Dec 2023 00:42:07 GMT  
		Size: 982.8 KB (982808 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:79d453aad0ebfa3f5472ee10df0b3e529d95ea63518574c69ceb52f5cf22d4c4`  
		Last Modified: Thu, 21 Dec 2023 00:42:07 GMT  
		Size: 4.6 MB (4594897 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1b6cca7a391de90190ab3ccfd94b95a59a48c0622005d5a5f5f364ac0c4c02e0`  
		Last Modified: Thu, 21 Dec 2023 00:42:07 GMT  
		Size: 2.6 KB (2604 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f9e7ae94329772a89c4c8e768d2f2209b96d4573ecf54dd50a679ddcaab6ec64`  
		Last Modified: Thu, 21 Dec 2023 00:42:08 GMT  
		Size: 332.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:af3e28b094a2e946679cb3f91d09922e2ae80bc117e6c3dc52016468e77ff1c9`  
		Last Modified: Thu, 21 Dec 2023 00:42:09 GMT  
		Size: 58.5 MB (58505933 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:db237bdcf1c0c61bb338e11bec6ba80c30afae0097636229de54a52fc9b2b41f`  
		Last Modified: Thu, 21 Dec 2023 00:42:08 GMT  
		Size: 315.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4b3c3f5cb4f4c88a98466d248ca0027a0abbd6d6301f0d166bd925eb58cf5ebd`  
		Last Modified: Thu, 21 Dec 2023 00:42:09 GMT  
		Size: 58.3 MB (58312328 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:394dbd7e05eb13c1f4b395b558b1c40b708996f1c5eb5dead40242895ce31121`  
		Last Modified: Thu, 21 Dec 2023 00:42:09 GMT  
		Size: 5.2 KB (5178 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:18a167e598b07c1067ec74fb4f63dd9a06c3baa1b6923afe66cfb4911c76632f`  
		Last Modified: Thu, 21 Dec 2023 00:42:09 GMT  
		Size: 121.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:8.0` - unknown; unknown

```console
$ docker pull mysql@sha256:e947f8eb99f01f51bb4a1a0506f0a5e23e03b48e78c68fb4931232b92bc96154
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.6 MB (11602599 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c396d9ca70fb4db2a43ca8d5ce6ab8de931e72363589fd41c168185836c0988b`

```dockerfile
```

-	Layers:
	-	`sha256:e5579f8c4a1d658618ca9a6429cc1f69801c829936675aed2b3837bd7b03ba46`  
		Last Modified: Thu, 21 Dec 2023 00:42:07 GMT  
		Size: 11.6 MB (11568051 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:c65568400f27660daae64a470173a41ed0af8ec67a24a230eae4e6ff1d0a53d8`  
		Last Modified: Thu, 21 Dec 2023 00:42:07 GMT  
		Size: 34.5 KB (34548 bytes)  
		MIME: application/vnd.in-toto+json

### `mysql:8.0` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:1fd4aa0943c8abc8bc478aea910779854c9f5375ba776a0413afe127006436e4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **177.4 MB (177445080 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9fdb9342cc99594cd3a8428facc5dcf87588c74f2c9991e75055c8ed8bb457db`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 06 Dec 2023 19:42:27 GMT
ADD file:f5ee75151bd25b33e72aa4c0560815f35f6e662876bf3733a02e5cb970227358 in / 
# Wed, 06 Dec 2023 19:42:27 GMT
CMD ["/bin/bash"]
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV GOSU_VERSION=1.16
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME" # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_MAJOR=8.0
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_VERSION=8.0.35-1.el8
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eu; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo 'baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/8/$basearch/'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eu; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo 'baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/8/$basearch/'; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_SHELL_VERSION=8.0.35-1.el8
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
VOLUME [/var/lib/mysql]
# Mon, 18 Dec 2023 23:06:09 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 18 Dec 2023 23:06:09 GMT
EXPOSE map[3306/tcp:{} 33060/tcp:{}]
# Mon, 18 Dec 2023 23:06:09 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:edfaa6c9daada52a737333e0818f3d697d745aab3f3351e773218a524ebc9e53`  
		Last Modified: Wed, 06 Dec 2023 19:43:23 GMT  
		Size: 50.1 MB (50072545 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:19c686b91aca61da8058a44e9f6aa06cbb27aa65cf2db0768377bcc6899dc0c2`  
		Last Modified: Thu, 14 Dec 2023 20:15:05 GMT  
		Size: 885.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8c39062282e36f6169d219352cb19810ac7506e408e89b4ef33c400903a6ecc1`  
		Last Modified: Thu, 14 Dec 2023 20:15:05 GMT  
		Size: 913.0 KB (912965 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:73452dd561ff872804f5a63faab7552647c80c8a399e834fe154707a48613b20`  
		Last Modified: Thu, 14 Dec 2023 20:15:05 GMT  
		Size: 4.3 MB (4300794 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0ba54e261f50c32496de78ff38c42eb03cb97850ddbeb3c96f4fe34ea1cb23bc`  
		Last Modified: Thu, 14 Dec 2023 20:15:05 GMT  
		Size: 2.6 KB (2609 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f8a2d4a8cba602b5e3cd65d5e0557988bcbd78b091afb3f6ae0d15864790987f`  
		Last Modified: Thu, 14 Dec 2023 20:16:54 GMT  
		Size: 332.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e6ba09d9fb3dfd35ff7ebbb6eb20bd59a35b737aec5e0e2f2c42eb50dda9d1e1`  
		Last Modified: Thu, 14 Dec 2023 20:16:56 GMT  
		Size: 57.6 MB (57573677 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3039dd1391bc16761b31a730472044ed80f3817b431f9de14e0b2b9e5949a66e`  
		Last Modified: Thu, 14 Dec 2023 20:16:54 GMT  
		Size: 316.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ad4d0901f4a72dd35f6f7f609dbcc9e9d4cc321ed55cad8b778a73cd0e8b4132`  
		Last Modified: Thu, 14 Dec 2023 20:16:56 GMT  
		Size: 64.6 MB (64575659 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e07375f3b7d754961d4d4dab48979ab0ff5a27d70949da753b98f86e075f16ba`  
		Last Modified: Tue, 19 Dec 2023 22:04:07 GMT  
		Size: 5.2 KB (5178 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6e4d42b5ded666fd53f1cfa7026d0fcdf1222cebf111756700d3ea573e069a99`  
		Last Modified: Tue, 19 Dec 2023 22:04:07 GMT  
		Size: 120.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:8.0` - unknown; unknown

```console
$ docker pull mysql@sha256:cb0dde16b43ff62c5e9a8293635a3e506404e3942f91170a5624de10dbcc3c6b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.6 MB (11601006 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b517449c77273c30cf2ea6ee95149207a40bdcc2657a73ee0bdcf8cb8d32f8ff`

```dockerfile
```

-	Layers:
	-	`sha256:7540cc15c09e88ca43d3a437e9e95e9e0763f75f5f13a14201e79ad422ea1aeb`  
		Last Modified: Tue, 19 Dec 2023 22:04:07 GMT  
		Size: 11.6 MB (11566611 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:4947d50d277de5c30205c9c1354c1d66254980e8e4bf4796a6abaeda465c1125`  
		Last Modified: Tue, 19 Dec 2023 22:04:06 GMT  
		Size: 34.4 KB (34395 bytes)  
		MIME: application/vnd.in-toto+json

## `mysql:8.0-bullseye`

```console
$ docker pull mysql@sha256:79da18642ae62b3c728a3bd4de3ce0fbf71f0e3a2101331b99fa0c048656a361
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 2
	-	linux; amd64
	-	unknown; unknown

### `mysql:8.0-bullseye` - linux; amd64

```console
$ docker pull mysql@sha256:c69b5add61fd1cad3b6090513022eb7d62cb7820f41afa3844604b5de39275d9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **179.1 MB (179126303 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9316e617b776de06ac3b3a8705adb5d2af933639d5394d7620643981e38236c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 18 Dec 2023 23:06:09 GMT
ADD file:bb44d67b03db8efaeb0c4171474f441d14ff35f328f13add32b289fca062fa2f in / 
# Mon, 18 Dec 2023 23:06:09 GMT
CMD ["bash"]
# Mon, 18 Dec 2023 23:06:09 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg && rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV GOSU_VERSION=1.16
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN mkdir /docker-entrypoint-initdb.d # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	key='BCA4 3417 C3B4 85DD 128E C6D4 B7B3 B788 A8D3 785C'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_MAJOR=8.0
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_VERSION=8.0.35-1debian11
# Mon, 18 Dec 2023 23:06:09 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ bullseye mysql-8.0' > /etc/apt/sources.list.d/mysql.list # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
VOLUME [/var/lib/mysql]
# Mon, 18 Dec 2023 23:06:09 GMT
COPY config/ /etc/mysql/ # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 18 Dec 2023 23:06:09 GMT
EXPOSE map[3306/tcp:{} 33060/tcp:{}]
# Mon, 18 Dec 2023 23:06:09 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:b5a0d5c14ba9ece1eecd5137c468d9a123372b0af2ed2c8c4446137730c90e5b`  
		Last Modified: Tue, 19 Dec 2023 01:25:40 GMT  
		Size: 31.4 MB (31417873 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:da5817b65ce4cfccfbd1cab936288cc2c9f576106fd0ab111cddb3f49604b511`  
		Last Modified: Tue, 19 Dec 2023 03:48:09 GMT  
		Size: 1.6 KB (1648 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:22e837abaef2fbc36a2e530f662337e34b8657c6c7a8c5fa8985bd2da8558e88`  
		Last Modified: Tue, 19 Dec 2023 03:48:09 GMT  
		Size: 4.2 MB (4207553 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:20780fd9cbff99edbacd139c37874ca887f245bfcb551a864ae2d16d2796e66d`  
		Last Modified: Tue, 19 Dec 2023 03:48:10 GMT  
		Size: 1.5 MB (1472512 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:79fdc95bdfcd9c8e64e72e935d8cf5ead3f36df49822e4855a109cd7f02ad1da`  
		Last Modified: Tue, 19 Dec 2023 03:48:09 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6363b252c0190906b09055d3b005632c4e935437229d10bd1fde49edc0f09552`  
		Last Modified: Tue, 19 Dec 2023 03:48:10 GMT  
		Size: 12.5 MB (12455047 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:53763e330a11bdf71cdb59546001958be08d795253de155d76d3de7ca5cd0414`  
		Last Modified: Tue, 19 Dec 2023 03:48:10 GMT  
		Size: 2.5 KB (2497 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0f86f27fd6e32a832a7f07fca219bbf972cb94ac5eaeaf863956a7b6eed62325`  
		Last Modified: Tue, 19 Dec 2023 03:48:10 GMT  
		Size: 248.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f366e63462a4138b04a5404fb55d39d8319c2d32fb72a72aa0dfaaad7138c84d`  
		Last Modified: Tue, 19 Dec 2023 03:48:13 GMT  
		Size: 129.6 MB (129562666 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:253e0e751437680411c5e8fb4fcc53b9f8550407de309acfed0c90eefcc6e118`  
		Last Modified: Tue, 19 Dec 2023 03:48:11 GMT  
		Size: 843.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:36545369253738d314a9c0f1c27e796624b955d8421c3e76c206199838d60067`  
		Last Modified: Tue, 19 Dec 2023 03:48:11 GMT  
		Size: 5.2 KB (5178 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9c0d0816114713ba3afb8894fe438b4b455b71f36a17be963b18cde665d20dd2`  
		Last Modified: Tue, 19 Dec 2023 03:48:11 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:8.0-bullseye` - unknown; unknown

```console
$ docker pull mysql@sha256:c62f70ff2e4bb366308fe3fd509d1dd64808e2cd97872b409e7eafb90478bb17
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.6 MB (3587245 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b9696d74f06fc27194d39f6f22be3bbda0f9ca68d4399239252d6aa0ab2414fb`

```dockerfile
```

-	Layers:
	-	`sha256:01d50b5cf5a872322fba73f7e117e4f0a2d6e1ee97cbd1a7af58c52025cf8abe`  
		Last Modified: Tue, 19 Dec 2023 03:48:09 GMT  
		Size: 3.6 MB (3552993 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:eee7cfb8f5ef7f6fa00dcfa001913c382d4d8dca42cf15cb520f93802bdeea4b`  
		Last Modified: Tue, 19 Dec 2023 03:48:09 GMT  
		Size: 34.3 KB (34252 bytes)  
		MIME: application/vnd.in-toto+json

## `mysql:8.0-debian`

```console
$ docker pull mysql@sha256:79da18642ae62b3c728a3bd4de3ce0fbf71f0e3a2101331b99fa0c048656a361
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 2
	-	linux; amd64
	-	unknown; unknown

### `mysql:8.0-debian` - linux; amd64

```console
$ docker pull mysql@sha256:c69b5add61fd1cad3b6090513022eb7d62cb7820f41afa3844604b5de39275d9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **179.1 MB (179126303 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9316e617b776de06ac3b3a8705adb5d2af933639d5394d7620643981e38236c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 18 Dec 2023 23:06:09 GMT
ADD file:bb44d67b03db8efaeb0c4171474f441d14ff35f328f13add32b289fca062fa2f in / 
# Mon, 18 Dec 2023 23:06:09 GMT
CMD ["bash"]
# Mon, 18 Dec 2023 23:06:09 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg && rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV GOSU_VERSION=1.16
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN mkdir /docker-entrypoint-initdb.d # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	key='BCA4 3417 C3B4 85DD 128E C6D4 B7B3 B788 A8D3 785C'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_MAJOR=8.0
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_VERSION=8.0.35-1debian11
# Mon, 18 Dec 2023 23:06:09 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ bullseye mysql-8.0' > /etc/apt/sources.list.d/mysql.list # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
VOLUME [/var/lib/mysql]
# Mon, 18 Dec 2023 23:06:09 GMT
COPY config/ /etc/mysql/ # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 18 Dec 2023 23:06:09 GMT
EXPOSE map[3306/tcp:{} 33060/tcp:{}]
# Mon, 18 Dec 2023 23:06:09 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:b5a0d5c14ba9ece1eecd5137c468d9a123372b0af2ed2c8c4446137730c90e5b`  
		Last Modified: Tue, 19 Dec 2023 01:25:40 GMT  
		Size: 31.4 MB (31417873 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:da5817b65ce4cfccfbd1cab936288cc2c9f576106fd0ab111cddb3f49604b511`  
		Last Modified: Tue, 19 Dec 2023 03:48:09 GMT  
		Size: 1.6 KB (1648 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:22e837abaef2fbc36a2e530f662337e34b8657c6c7a8c5fa8985bd2da8558e88`  
		Last Modified: Tue, 19 Dec 2023 03:48:09 GMT  
		Size: 4.2 MB (4207553 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:20780fd9cbff99edbacd139c37874ca887f245bfcb551a864ae2d16d2796e66d`  
		Last Modified: Tue, 19 Dec 2023 03:48:10 GMT  
		Size: 1.5 MB (1472512 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:79fdc95bdfcd9c8e64e72e935d8cf5ead3f36df49822e4855a109cd7f02ad1da`  
		Last Modified: Tue, 19 Dec 2023 03:48:09 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6363b252c0190906b09055d3b005632c4e935437229d10bd1fde49edc0f09552`  
		Last Modified: Tue, 19 Dec 2023 03:48:10 GMT  
		Size: 12.5 MB (12455047 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:53763e330a11bdf71cdb59546001958be08d795253de155d76d3de7ca5cd0414`  
		Last Modified: Tue, 19 Dec 2023 03:48:10 GMT  
		Size: 2.5 KB (2497 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0f86f27fd6e32a832a7f07fca219bbf972cb94ac5eaeaf863956a7b6eed62325`  
		Last Modified: Tue, 19 Dec 2023 03:48:10 GMT  
		Size: 248.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f366e63462a4138b04a5404fb55d39d8319c2d32fb72a72aa0dfaaad7138c84d`  
		Last Modified: Tue, 19 Dec 2023 03:48:13 GMT  
		Size: 129.6 MB (129562666 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:253e0e751437680411c5e8fb4fcc53b9f8550407de309acfed0c90eefcc6e118`  
		Last Modified: Tue, 19 Dec 2023 03:48:11 GMT  
		Size: 843.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:36545369253738d314a9c0f1c27e796624b955d8421c3e76c206199838d60067`  
		Last Modified: Tue, 19 Dec 2023 03:48:11 GMT  
		Size: 5.2 KB (5178 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9c0d0816114713ba3afb8894fe438b4b455b71f36a17be963b18cde665d20dd2`  
		Last Modified: Tue, 19 Dec 2023 03:48:11 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:8.0-debian` - unknown; unknown

```console
$ docker pull mysql@sha256:c62f70ff2e4bb366308fe3fd509d1dd64808e2cd97872b409e7eafb90478bb17
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.6 MB (3587245 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b9696d74f06fc27194d39f6f22be3bbda0f9ca68d4399239252d6aa0ab2414fb`

```dockerfile
```

-	Layers:
	-	`sha256:01d50b5cf5a872322fba73f7e117e4f0a2d6e1ee97cbd1a7af58c52025cf8abe`  
		Last Modified: Tue, 19 Dec 2023 03:48:09 GMT  
		Size: 3.6 MB (3552993 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:eee7cfb8f5ef7f6fa00dcfa001913c382d4d8dca42cf15cb520f93802bdeea4b`  
		Last Modified: Tue, 19 Dec 2023 03:48:09 GMT  
		Size: 34.3 KB (34252 bytes)  
		MIME: application/vnd.in-toto+json

## `mysql:8.0-oracle`

```console
$ docker pull mysql@sha256:c80ef5968b6baf12e9ba95412d4725971207228e5274518db92e26d0e169372b
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `mysql:8.0-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:3a0b76a2ee46a23fc8e0c5e2d38d016a8466bbc774c933d719ae0b5308982dba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **173.7 MB (173728874 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba048db12589d011b77ab3ea33b7010d0b549214c8baa5fd885e4af84887928f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 18 Dec 2023 23:06:09 GMT
ADD file:da89b67e484bc45f357250a868fd78e28086b13e4315635d19648e5d43812e89 in / 
# Mon, 18 Dec 2023 23:06:09 GMT
CMD ["/bin/bash"]
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV GOSU_VERSION=1.16
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME" # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_MAJOR=8.0
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_VERSION=8.0.35-1.el8
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eu; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo 'baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/8/$basearch/'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eu; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo 'baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/8/$basearch/'; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_SHELL_VERSION=8.0.35-1.el8
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
VOLUME [/var/lib/mysql]
# Mon, 18 Dec 2023 23:06:09 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 18 Dec 2023 23:06:09 GMT
EXPOSE map[3306/tcp:{} 33060/tcp:{}]
# Mon, 18 Dec 2023 23:06:09 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:bce031bc522d421fb188ef82a530f85c5477bb87cdeacdb911ea86f3f7cd3b66`  
		Last Modified: Wed, 20 Dec 2023 22:42:00 GMT  
		Size: 51.3 MB (51323468 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9d95fc125cf8067473c7c0aeb06cc55f45268807b23568fbc3f14cab35d285cf`  
		Last Modified: Thu, 21 Dec 2023 00:42:07 GMT  
		Size: 890.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:22412d6d690fcd08a40e3808538b28c8ff614ca7d4292b97f91862c7d90f8279`  
		Last Modified: Thu, 21 Dec 2023 00:42:07 GMT  
		Size: 982.8 KB (982808 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:79d453aad0ebfa3f5472ee10df0b3e529d95ea63518574c69ceb52f5cf22d4c4`  
		Last Modified: Thu, 21 Dec 2023 00:42:07 GMT  
		Size: 4.6 MB (4594897 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1b6cca7a391de90190ab3ccfd94b95a59a48c0622005d5a5f5f364ac0c4c02e0`  
		Last Modified: Thu, 21 Dec 2023 00:42:07 GMT  
		Size: 2.6 KB (2604 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f9e7ae94329772a89c4c8e768d2f2209b96d4573ecf54dd50a679ddcaab6ec64`  
		Last Modified: Thu, 21 Dec 2023 00:42:08 GMT  
		Size: 332.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:af3e28b094a2e946679cb3f91d09922e2ae80bc117e6c3dc52016468e77ff1c9`  
		Last Modified: Thu, 21 Dec 2023 00:42:09 GMT  
		Size: 58.5 MB (58505933 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:db237bdcf1c0c61bb338e11bec6ba80c30afae0097636229de54a52fc9b2b41f`  
		Last Modified: Thu, 21 Dec 2023 00:42:08 GMT  
		Size: 315.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4b3c3f5cb4f4c88a98466d248ca0027a0abbd6d6301f0d166bd925eb58cf5ebd`  
		Last Modified: Thu, 21 Dec 2023 00:42:09 GMT  
		Size: 58.3 MB (58312328 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:394dbd7e05eb13c1f4b395b558b1c40b708996f1c5eb5dead40242895ce31121`  
		Last Modified: Thu, 21 Dec 2023 00:42:09 GMT  
		Size: 5.2 KB (5178 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:18a167e598b07c1067ec74fb4f63dd9a06c3baa1b6923afe66cfb4911c76632f`  
		Last Modified: Thu, 21 Dec 2023 00:42:09 GMT  
		Size: 121.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:8.0-oracle` - unknown; unknown

```console
$ docker pull mysql@sha256:e947f8eb99f01f51bb4a1a0506f0a5e23e03b48e78c68fb4931232b92bc96154
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.6 MB (11602599 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c396d9ca70fb4db2a43ca8d5ce6ab8de931e72363589fd41c168185836c0988b`

```dockerfile
```

-	Layers:
	-	`sha256:e5579f8c4a1d658618ca9a6429cc1f69801c829936675aed2b3837bd7b03ba46`  
		Last Modified: Thu, 21 Dec 2023 00:42:07 GMT  
		Size: 11.6 MB (11568051 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:c65568400f27660daae64a470173a41ed0af8ec67a24a230eae4e6ff1d0a53d8`  
		Last Modified: Thu, 21 Dec 2023 00:42:07 GMT  
		Size: 34.5 KB (34548 bytes)  
		MIME: application/vnd.in-toto+json

### `mysql:8.0-oracle` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:1fd4aa0943c8abc8bc478aea910779854c9f5375ba776a0413afe127006436e4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **177.4 MB (177445080 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9fdb9342cc99594cd3a8428facc5dcf87588c74f2c9991e75055c8ed8bb457db`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 06 Dec 2023 19:42:27 GMT
ADD file:f5ee75151bd25b33e72aa4c0560815f35f6e662876bf3733a02e5cb970227358 in / 
# Wed, 06 Dec 2023 19:42:27 GMT
CMD ["/bin/bash"]
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV GOSU_VERSION=1.16
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME" # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_MAJOR=8.0
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_VERSION=8.0.35-1.el8
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eu; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo 'baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/8/$basearch/'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eu; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo 'baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/8/$basearch/'; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_SHELL_VERSION=8.0.35-1.el8
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
VOLUME [/var/lib/mysql]
# Mon, 18 Dec 2023 23:06:09 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 18 Dec 2023 23:06:09 GMT
EXPOSE map[3306/tcp:{} 33060/tcp:{}]
# Mon, 18 Dec 2023 23:06:09 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:edfaa6c9daada52a737333e0818f3d697d745aab3f3351e773218a524ebc9e53`  
		Last Modified: Wed, 06 Dec 2023 19:43:23 GMT  
		Size: 50.1 MB (50072545 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:19c686b91aca61da8058a44e9f6aa06cbb27aa65cf2db0768377bcc6899dc0c2`  
		Last Modified: Thu, 14 Dec 2023 20:15:05 GMT  
		Size: 885.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8c39062282e36f6169d219352cb19810ac7506e408e89b4ef33c400903a6ecc1`  
		Last Modified: Thu, 14 Dec 2023 20:15:05 GMT  
		Size: 913.0 KB (912965 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:73452dd561ff872804f5a63faab7552647c80c8a399e834fe154707a48613b20`  
		Last Modified: Thu, 14 Dec 2023 20:15:05 GMT  
		Size: 4.3 MB (4300794 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0ba54e261f50c32496de78ff38c42eb03cb97850ddbeb3c96f4fe34ea1cb23bc`  
		Last Modified: Thu, 14 Dec 2023 20:15:05 GMT  
		Size: 2.6 KB (2609 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f8a2d4a8cba602b5e3cd65d5e0557988bcbd78b091afb3f6ae0d15864790987f`  
		Last Modified: Thu, 14 Dec 2023 20:16:54 GMT  
		Size: 332.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e6ba09d9fb3dfd35ff7ebbb6eb20bd59a35b737aec5e0e2f2c42eb50dda9d1e1`  
		Last Modified: Thu, 14 Dec 2023 20:16:56 GMT  
		Size: 57.6 MB (57573677 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3039dd1391bc16761b31a730472044ed80f3817b431f9de14e0b2b9e5949a66e`  
		Last Modified: Thu, 14 Dec 2023 20:16:54 GMT  
		Size: 316.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ad4d0901f4a72dd35f6f7f609dbcc9e9d4cc321ed55cad8b778a73cd0e8b4132`  
		Last Modified: Thu, 14 Dec 2023 20:16:56 GMT  
		Size: 64.6 MB (64575659 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e07375f3b7d754961d4d4dab48979ab0ff5a27d70949da753b98f86e075f16ba`  
		Last Modified: Tue, 19 Dec 2023 22:04:07 GMT  
		Size: 5.2 KB (5178 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6e4d42b5ded666fd53f1cfa7026d0fcdf1222cebf111756700d3ea573e069a99`  
		Last Modified: Tue, 19 Dec 2023 22:04:07 GMT  
		Size: 120.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:8.0-oracle` - unknown; unknown

```console
$ docker pull mysql@sha256:cb0dde16b43ff62c5e9a8293635a3e506404e3942f91170a5624de10dbcc3c6b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.6 MB (11601006 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b517449c77273c30cf2ea6ee95149207a40bdcc2657a73ee0bdcf8cb8d32f8ff`

```dockerfile
```

-	Layers:
	-	`sha256:7540cc15c09e88ca43d3a437e9e95e9e0763f75f5f13a14201e79ad422ea1aeb`  
		Last Modified: Tue, 19 Dec 2023 22:04:07 GMT  
		Size: 11.6 MB (11566611 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:4947d50d277de5c30205c9c1354c1d66254980e8e4bf4796a6abaeda465c1125`  
		Last Modified: Tue, 19 Dec 2023 22:04:06 GMT  
		Size: 34.4 KB (34395 bytes)  
		MIME: application/vnd.in-toto+json

## `mysql:8.0-oraclelinux8`

```console
$ docker pull mysql@sha256:c80ef5968b6baf12e9ba95412d4725971207228e5274518db92e26d0e169372b
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `mysql:8.0-oraclelinux8` - linux; amd64

```console
$ docker pull mysql@sha256:3a0b76a2ee46a23fc8e0c5e2d38d016a8466bbc774c933d719ae0b5308982dba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **173.7 MB (173728874 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba048db12589d011b77ab3ea33b7010d0b549214c8baa5fd885e4af84887928f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 18 Dec 2023 23:06:09 GMT
ADD file:da89b67e484bc45f357250a868fd78e28086b13e4315635d19648e5d43812e89 in / 
# Mon, 18 Dec 2023 23:06:09 GMT
CMD ["/bin/bash"]
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV GOSU_VERSION=1.16
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME" # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_MAJOR=8.0
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_VERSION=8.0.35-1.el8
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eu; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo 'baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/8/$basearch/'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eu; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo 'baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/8/$basearch/'; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_SHELL_VERSION=8.0.35-1.el8
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
VOLUME [/var/lib/mysql]
# Mon, 18 Dec 2023 23:06:09 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 18 Dec 2023 23:06:09 GMT
EXPOSE map[3306/tcp:{} 33060/tcp:{}]
# Mon, 18 Dec 2023 23:06:09 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:bce031bc522d421fb188ef82a530f85c5477bb87cdeacdb911ea86f3f7cd3b66`  
		Last Modified: Wed, 20 Dec 2023 22:42:00 GMT  
		Size: 51.3 MB (51323468 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9d95fc125cf8067473c7c0aeb06cc55f45268807b23568fbc3f14cab35d285cf`  
		Last Modified: Thu, 21 Dec 2023 00:42:07 GMT  
		Size: 890.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:22412d6d690fcd08a40e3808538b28c8ff614ca7d4292b97f91862c7d90f8279`  
		Last Modified: Thu, 21 Dec 2023 00:42:07 GMT  
		Size: 982.8 KB (982808 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:79d453aad0ebfa3f5472ee10df0b3e529d95ea63518574c69ceb52f5cf22d4c4`  
		Last Modified: Thu, 21 Dec 2023 00:42:07 GMT  
		Size: 4.6 MB (4594897 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1b6cca7a391de90190ab3ccfd94b95a59a48c0622005d5a5f5f364ac0c4c02e0`  
		Last Modified: Thu, 21 Dec 2023 00:42:07 GMT  
		Size: 2.6 KB (2604 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f9e7ae94329772a89c4c8e768d2f2209b96d4573ecf54dd50a679ddcaab6ec64`  
		Last Modified: Thu, 21 Dec 2023 00:42:08 GMT  
		Size: 332.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:af3e28b094a2e946679cb3f91d09922e2ae80bc117e6c3dc52016468e77ff1c9`  
		Last Modified: Thu, 21 Dec 2023 00:42:09 GMT  
		Size: 58.5 MB (58505933 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:db237bdcf1c0c61bb338e11bec6ba80c30afae0097636229de54a52fc9b2b41f`  
		Last Modified: Thu, 21 Dec 2023 00:42:08 GMT  
		Size: 315.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4b3c3f5cb4f4c88a98466d248ca0027a0abbd6d6301f0d166bd925eb58cf5ebd`  
		Last Modified: Thu, 21 Dec 2023 00:42:09 GMT  
		Size: 58.3 MB (58312328 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:394dbd7e05eb13c1f4b395b558b1c40b708996f1c5eb5dead40242895ce31121`  
		Last Modified: Thu, 21 Dec 2023 00:42:09 GMT  
		Size: 5.2 KB (5178 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:18a167e598b07c1067ec74fb4f63dd9a06c3baa1b6923afe66cfb4911c76632f`  
		Last Modified: Thu, 21 Dec 2023 00:42:09 GMT  
		Size: 121.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:8.0-oraclelinux8` - unknown; unknown

```console
$ docker pull mysql@sha256:e947f8eb99f01f51bb4a1a0506f0a5e23e03b48e78c68fb4931232b92bc96154
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.6 MB (11602599 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c396d9ca70fb4db2a43ca8d5ce6ab8de931e72363589fd41c168185836c0988b`

```dockerfile
```

-	Layers:
	-	`sha256:e5579f8c4a1d658618ca9a6429cc1f69801c829936675aed2b3837bd7b03ba46`  
		Last Modified: Thu, 21 Dec 2023 00:42:07 GMT  
		Size: 11.6 MB (11568051 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:c65568400f27660daae64a470173a41ed0af8ec67a24a230eae4e6ff1d0a53d8`  
		Last Modified: Thu, 21 Dec 2023 00:42:07 GMT  
		Size: 34.5 KB (34548 bytes)  
		MIME: application/vnd.in-toto+json

### `mysql:8.0-oraclelinux8` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:1fd4aa0943c8abc8bc478aea910779854c9f5375ba776a0413afe127006436e4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **177.4 MB (177445080 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9fdb9342cc99594cd3a8428facc5dcf87588c74f2c9991e75055c8ed8bb457db`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 06 Dec 2023 19:42:27 GMT
ADD file:f5ee75151bd25b33e72aa4c0560815f35f6e662876bf3733a02e5cb970227358 in / 
# Wed, 06 Dec 2023 19:42:27 GMT
CMD ["/bin/bash"]
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV GOSU_VERSION=1.16
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME" # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_MAJOR=8.0
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_VERSION=8.0.35-1.el8
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eu; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo 'baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/8/$basearch/'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eu; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo 'baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/8/$basearch/'; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_SHELL_VERSION=8.0.35-1.el8
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
VOLUME [/var/lib/mysql]
# Mon, 18 Dec 2023 23:06:09 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 18 Dec 2023 23:06:09 GMT
EXPOSE map[3306/tcp:{} 33060/tcp:{}]
# Mon, 18 Dec 2023 23:06:09 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:edfaa6c9daada52a737333e0818f3d697d745aab3f3351e773218a524ebc9e53`  
		Last Modified: Wed, 06 Dec 2023 19:43:23 GMT  
		Size: 50.1 MB (50072545 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:19c686b91aca61da8058a44e9f6aa06cbb27aa65cf2db0768377bcc6899dc0c2`  
		Last Modified: Thu, 14 Dec 2023 20:15:05 GMT  
		Size: 885.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8c39062282e36f6169d219352cb19810ac7506e408e89b4ef33c400903a6ecc1`  
		Last Modified: Thu, 14 Dec 2023 20:15:05 GMT  
		Size: 913.0 KB (912965 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:73452dd561ff872804f5a63faab7552647c80c8a399e834fe154707a48613b20`  
		Last Modified: Thu, 14 Dec 2023 20:15:05 GMT  
		Size: 4.3 MB (4300794 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0ba54e261f50c32496de78ff38c42eb03cb97850ddbeb3c96f4fe34ea1cb23bc`  
		Last Modified: Thu, 14 Dec 2023 20:15:05 GMT  
		Size: 2.6 KB (2609 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f8a2d4a8cba602b5e3cd65d5e0557988bcbd78b091afb3f6ae0d15864790987f`  
		Last Modified: Thu, 14 Dec 2023 20:16:54 GMT  
		Size: 332.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e6ba09d9fb3dfd35ff7ebbb6eb20bd59a35b737aec5e0e2f2c42eb50dda9d1e1`  
		Last Modified: Thu, 14 Dec 2023 20:16:56 GMT  
		Size: 57.6 MB (57573677 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3039dd1391bc16761b31a730472044ed80f3817b431f9de14e0b2b9e5949a66e`  
		Last Modified: Thu, 14 Dec 2023 20:16:54 GMT  
		Size: 316.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ad4d0901f4a72dd35f6f7f609dbcc9e9d4cc321ed55cad8b778a73cd0e8b4132`  
		Last Modified: Thu, 14 Dec 2023 20:16:56 GMT  
		Size: 64.6 MB (64575659 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e07375f3b7d754961d4d4dab48979ab0ff5a27d70949da753b98f86e075f16ba`  
		Last Modified: Tue, 19 Dec 2023 22:04:07 GMT  
		Size: 5.2 KB (5178 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6e4d42b5ded666fd53f1cfa7026d0fcdf1222cebf111756700d3ea573e069a99`  
		Last Modified: Tue, 19 Dec 2023 22:04:07 GMT  
		Size: 120.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:8.0-oraclelinux8` - unknown; unknown

```console
$ docker pull mysql@sha256:cb0dde16b43ff62c5e9a8293635a3e506404e3942f91170a5624de10dbcc3c6b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.6 MB (11601006 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b517449c77273c30cf2ea6ee95149207a40bdcc2657a73ee0bdcf8cb8d32f8ff`

```dockerfile
```

-	Layers:
	-	`sha256:7540cc15c09e88ca43d3a437e9e95e9e0763f75f5f13a14201e79ad422ea1aeb`  
		Last Modified: Tue, 19 Dec 2023 22:04:07 GMT  
		Size: 11.6 MB (11566611 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:4947d50d277de5c30205c9c1354c1d66254980e8e4bf4796a6abaeda465c1125`  
		Last Modified: Tue, 19 Dec 2023 22:04:06 GMT  
		Size: 34.4 KB (34395 bytes)  
		MIME: application/vnd.in-toto+json

## `mysql:8.0.35`

```console
$ docker pull mysql@sha256:c80ef5968b6baf12e9ba95412d4725971207228e5274518db92e26d0e169372b
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `mysql:8.0.35` - linux; amd64

```console
$ docker pull mysql@sha256:3a0b76a2ee46a23fc8e0c5e2d38d016a8466bbc774c933d719ae0b5308982dba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **173.7 MB (173728874 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba048db12589d011b77ab3ea33b7010d0b549214c8baa5fd885e4af84887928f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 18 Dec 2023 23:06:09 GMT
ADD file:da89b67e484bc45f357250a868fd78e28086b13e4315635d19648e5d43812e89 in / 
# Mon, 18 Dec 2023 23:06:09 GMT
CMD ["/bin/bash"]
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV GOSU_VERSION=1.16
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME" # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_MAJOR=8.0
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_VERSION=8.0.35-1.el8
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eu; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo 'baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/8/$basearch/'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eu; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo 'baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/8/$basearch/'; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_SHELL_VERSION=8.0.35-1.el8
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
VOLUME [/var/lib/mysql]
# Mon, 18 Dec 2023 23:06:09 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 18 Dec 2023 23:06:09 GMT
EXPOSE map[3306/tcp:{} 33060/tcp:{}]
# Mon, 18 Dec 2023 23:06:09 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:bce031bc522d421fb188ef82a530f85c5477bb87cdeacdb911ea86f3f7cd3b66`  
		Last Modified: Wed, 20 Dec 2023 22:42:00 GMT  
		Size: 51.3 MB (51323468 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9d95fc125cf8067473c7c0aeb06cc55f45268807b23568fbc3f14cab35d285cf`  
		Last Modified: Thu, 21 Dec 2023 00:42:07 GMT  
		Size: 890.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:22412d6d690fcd08a40e3808538b28c8ff614ca7d4292b97f91862c7d90f8279`  
		Last Modified: Thu, 21 Dec 2023 00:42:07 GMT  
		Size: 982.8 KB (982808 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:79d453aad0ebfa3f5472ee10df0b3e529d95ea63518574c69ceb52f5cf22d4c4`  
		Last Modified: Thu, 21 Dec 2023 00:42:07 GMT  
		Size: 4.6 MB (4594897 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1b6cca7a391de90190ab3ccfd94b95a59a48c0622005d5a5f5f364ac0c4c02e0`  
		Last Modified: Thu, 21 Dec 2023 00:42:07 GMT  
		Size: 2.6 KB (2604 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f9e7ae94329772a89c4c8e768d2f2209b96d4573ecf54dd50a679ddcaab6ec64`  
		Last Modified: Thu, 21 Dec 2023 00:42:08 GMT  
		Size: 332.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:af3e28b094a2e946679cb3f91d09922e2ae80bc117e6c3dc52016468e77ff1c9`  
		Last Modified: Thu, 21 Dec 2023 00:42:09 GMT  
		Size: 58.5 MB (58505933 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:db237bdcf1c0c61bb338e11bec6ba80c30afae0097636229de54a52fc9b2b41f`  
		Last Modified: Thu, 21 Dec 2023 00:42:08 GMT  
		Size: 315.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4b3c3f5cb4f4c88a98466d248ca0027a0abbd6d6301f0d166bd925eb58cf5ebd`  
		Last Modified: Thu, 21 Dec 2023 00:42:09 GMT  
		Size: 58.3 MB (58312328 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:394dbd7e05eb13c1f4b395b558b1c40b708996f1c5eb5dead40242895ce31121`  
		Last Modified: Thu, 21 Dec 2023 00:42:09 GMT  
		Size: 5.2 KB (5178 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:18a167e598b07c1067ec74fb4f63dd9a06c3baa1b6923afe66cfb4911c76632f`  
		Last Modified: Thu, 21 Dec 2023 00:42:09 GMT  
		Size: 121.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:8.0.35` - unknown; unknown

```console
$ docker pull mysql@sha256:e947f8eb99f01f51bb4a1a0506f0a5e23e03b48e78c68fb4931232b92bc96154
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.6 MB (11602599 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c396d9ca70fb4db2a43ca8d5ce6ab8de931e72363589fd41c168185836c0988b`

```dockerfile
```

-	Layers:
	-	`sha256:e5579f8c4a1d658618ca9a6429cc1f69801c829936675aed2b3837bd7b03ba46`  
		Last Modified: Thu, 21 Dec 2023 00:42:07 GMT  
		Size: 11.6 MB (11568051 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:c65568400f27660daae64a470173a41ed0af8ec67a24a230eae4e6ff1d0a53d8`  
		Last Modified: Thu, 21 Dec 2023 00:42:07 GMT  
		Size: 34.5 KB (34548 bytes)  
		MIME: application/vnd.in-toto+json

### `mysql:8.0.35` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:1fd4aa0943c8abc8bc478aea910779854c9f5375ba776a0413afe127006436e4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **177.4 MB (177445080 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9fdb9342cc99594cd3a8428facc5dcf87588c74f2c9991e75055c8ed8bb457db`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 06 Dec 2023 19:42:27 GMT
ADD file:f5ee75151bd25b33e72aa4c0560815f35f6e662876bf3733a02e5cb970227358 in / 
# Wed, 06 Dec 2023 19:42:27 GMT
CMD ["/bin/bash"]
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV GOSU_VERSION=1.16
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME" # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_MAJOR=8.0
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_VERSION=8.0.35-1.el8
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eu; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo 'baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/8/$basearch/'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eu; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo 'baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/8/$basearch/'; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_SHELL_VERSION=8.0.35-1.el8
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
VOLUME [/var/lib/mysql]
# Mon, 18 Dec 2023 23:06:09 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 18 Dec 2023 23:06:09 GMT
EXPOSE map[3306/tcp:{} 33060/tcp:{}]
# Mon, 18 Dec 2023 23:06:09 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:edfaa6c9daada52a737333e0818f3d697d745aab3f3351e773218a524ebc9e53`  
		Last Modified: Wed, 06 Dec 2023 19:43:23 GMT  
		Size: 50.1 MB (50072545 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:19c686b91aca61da8058a44e9f6aa06cbb27aa65cf2db0768377bcc6899dc0c2`  
		Last Modified: Thu, 14 Dec 2023 20:15:05 GMT  
		Size: 885.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8c39062282e36f6169d219352cb19810ac7506e408e89b4ef33c400903a6ecc1`  
		Last Modified: Thu, 14 Dec 2023 20:15:05 GMT  
		Size: 913.0 KB (912965 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:73452dd561ff872804f5a63faab7552647c80c8a399e834fe154707a48613b20`  
		Last Modified: Thu, 14 Dec 2023 20:15:05 GMT  
		Size: 4.3 MB (4300794 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0ba54e261f50c32496de78ff38c42eb03cb97850ddbeb3c96f4fe34ea1cb23bc`  
		Last Modified: Thu, 14 Dec 2023 20:15:05 GMT  
		Size: 2.6 KB (2609 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f8a2d4a8cba602b5e3cd65d5e0557988bcbd78b091afb3f6ae0d15864790987f`  
		Last Modified: Thu, 14 Dec 2023 20:16:54 GMT  
		Size: 332.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e6ba09d9fb3dfd35ff7ebbb6eb20bd59a35b737aec5e0e2f2c42eb50dda9d1e1`  
		Last Modified: Thu, 14 Dec 2023 20:16:56 GMT  
		Size: 57.6 MB (57573677 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3039dd1391bc16761b31a730472044ed80f3817b431f9de14e0b2b9e5949a66e`  
		Last Modified: Thu, 14 Dec 2023 20:16:54 GMT  
		Size: 316.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ad4d0901f4a72dd35f6f7f609dbcc9e9d4cc321ed55cad8b778a73cd0e8b4132`  
		Last Modified: Thu, 14 Dec 2023 20:16:56 GMT  
		Size: 64.6 MB (64575659 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e07375f3b7d754961d4d4dab48979ab0ff5a27d70949da753b98f86e075f16ba`  
		Last Modified: Tue, 19 Dec 2023 22:04:07 GMT  
		Size: 5.2 KB (5178 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6e4d42b5ded666fd53f1cfa7026d0fcdf1222cebf111756700d3ea573e069a99`  
		Last Modified: Tue, 19 Dec 2023 22:04:07 GMT  
		Size: 120.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:8.0.35` - unknown; unknown

```console
$ docker pull mysql@sha256:cb0dde16b43ff62c5e9a8293635a3e506404e3942f91170a5624de10dbcc3c6b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.6 MB (11601006 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b517449c77273c30cf2ea6ee95149207a40bdcc2657a73ee0bdcf8cb8d32f8ff`

```dockerfile
```

-	Layers:
	-	`sha256:7540cc15c09e88ca43d3a437e9e95e9e0763f75f5f13a14201e79ad422ea1aeb`  
		Last Modified: Tue, 19 Dec 2023 22:04:07 GMT  
		Size: 11.6 MB (11566611 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:4947d50d277de5c30205c9c1354c1d66254980e8e4bf4796a6abaeda465c1125`  
		Last Modified: Tue, 19 Dec 2023 22:04:06 GMT  
		Size: 34.4 KB (34395 bytes)  
		MIME: application/vnd.in-toto+json

## `mysql:8.0.35-bullseye`

```console
$ docker pull mysql@sha256:79da18642ae62b3c728a3bd4de3ce0fbf71f0e3a2101331b99fa0c048656a361
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 2
	-	linux; amd64
	-	unknown; unknown

### `mysql:8.0.35-bullseye` - linux; amd64

```console
$ docker pull mysql@sha256:c69b5add61fd1cad3b6090513022eb7d62cb7820f41afa3844604b5de39275d9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **179.1 MB (179126303 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9316e617b776de06ac3b3a8705adb5d2af933639d5394d7620643981e38236c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 18 Dec 2023 23:06:09 GMT
ADD file:bb44d67b03db8efaeb0c4171474f441d14ff35f328f13add32b289fca062fa2f in / 
# Mon, 18 Dec 2023 23:06:09 GMT
CMD ["bash"]
# Mon, 18 Dec 2023 23:06:09 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg && rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV GOSU_VERSION=1.16
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN mkdir /docker-entrypoint-initdb.d # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	key='BCA4 3417 C3B4 85DD 128E C6D4 B7B3 B788 A8D3 785C'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_MAJOR=8.0
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_VERSION=8.0.35-1debian11
# Mon, 18 Dec 2023 23:06:09 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ bullseye mysql-8.0' > /etc/apt/sources.list.d/mysql.list # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
VOLUME [/var/lib/mysql]
# Mon, 18 Dec 2023 23:06:09 GMT
COPY config/ /etc/mysql/ # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 18 Dec 2023 23:06:09 GMT
EXPOSE map[3306/tcp:{} 33060/tcp:{}]
# Mon, 18 Dec 2023 23:06:09 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:b5a0d5c14ba9ece1eecd5137c468d9a123372b0af2ed2c8c4446137730c90e5b`  
		Last Modified: Tue, 19 Dec 2023 01:25:40 GMT  
		Size: 31.4 MB (31417873 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:da5817b65ce4cfccfbd1cab936288cc2c9f576106fd0ab111cddb3f49604b511`  
		Last Modified: Tue, 19 Dec 2023 03:48:09 GMT  
		Size: 1.6 KB (1648 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:22e837abaef2fbc36a2e530f662337e34b8657c6c7a8c5fa8985bd2da8558e88`  
		Last Modified: Tue, 19 Dec 2023 03:48:09 GMT  
		Size: 4.2 MB (4207553 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:20780fd9cbff99edbacd139c37874ca887f245bfcb551a864ae2d16d2796e66d`  
		Last Modified: Tue, 19 Dec 2023 03:48:10 GMT  
		Size: 1.5 MB (1472512 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:79fdc95bdfcd9c8e64e72e935d8cf5ead3f36df49822e4855a109cd7f02ad1da`  
		Last Modified: Tue, 19 Dec 2023 03:48:09 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6363b252c0190906b09055d3b005632c4e935437229d10bd1fde49edc0f09552`  
		Last Modified: Tue, 19 Dec 2023 03:48:10 GMT  
		Size: 12.5 MB (12455047 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:53763e330a11bdf71cdb59546001958be08d795253de155d76d3de7ca5cd0414`  
		Last Modified: Tue, 19 Dec 2023 03:48:10 GMT  
		Size: 2.5 KB (2497 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0f86f27fd6e32a832a7f07fca219bbf972cb94ac5eaeaf863956a7b6eed62325`  
		Last Modified: Tue, 19 Dec 2023 03:48:10 GMT  
		Size: 248.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f366e63462a4138b04a5404fb55d39d8319c2d32fb72a72aa0dfaaad7138c84d`  
		Last Modified: Tue, 19 Dec 2023 03:48:13 GMT  
		Size: 129.6 MB (129562666 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:253e0e751437680411c5e8fb4fcc53b9f8550407de309acfed0c90eefcc6e118`  
		Last Modified: Tue, 19 Dec 2023 03:48:11 GMT  
		Size: 843.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:36545369253738d314a9c0f1c27e796624b955d8421c3e76c206199838d60067`  
		Last Modified: Tue, 19 Dec 2023 03:48:11 GMT  
		Size: 5.2 KB (5178 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9c0d0816114713ba3afb8894fe438b4b455b71f36a17be963b18cde665d20dd2`  
		Last Modified: Tue, 19 Dec 2023 03:48:11 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:8.0.35-bullseye` - unknown; unknown

```console
$ docker pull mysql@sha256:c62f70ff2e4bb366308fe3fd509d1dd64808e2cd97872b409e7eafb90478bb17
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.6 MB (3587245 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b9696d74f06fc27194d39f6f22be3bbda0f9ca68d4399239252d6aa0ab2414fb`

```dockerfile
```

-	Layers:
	-	`sha256:01d50b5cf5a872322fba73f7e117e4f0a2d6e1ee97cbd1a7af58c52025cf8abe`  
		Last Modified: Tue, 19 Dec 2023 03:48:09 GMT  
		Size: 3.6 MB (3552993 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:eee7cfb8f5ef7f6fa00dcfa001913c382d4d8dca42cf15cb520f93802bdeea4b`  
		Last Modified: Tue, 19 Dec 2023 03:48:09 GMT  
		Size: 34.3 KB (34252 bytes)  
		MIME: application/vnd.in-toto+json

## `mysql:8.0.35-debian`

```console
$ docker pull mysql@sha256:79da18642ae62b3c728a3bd4de3ce0fbf71f0e3a2101331b99fa0c048656a361
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 2
	-	linux; amd64
	-	unknown; unknown

### `mysql:8.0.35-debian` - linux; amd64

```console
$ docker pull mysql@sha256:c69b5add61fd1cad3b6090513022eb7d62cb7820f41afa3844604b5de39275d9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **179.1 MB (179126303 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9316e617b776de06ac3b3a8705adb5d2af933639d5394d7620643981e38236c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 18 Dec 2023 23:06:09 GMT
ADD file:bb44d67b03db8efaeb0c4171474f441d14ff35f328f13add32b289fca062fa2f in / 
# Mon, 18 Dec 2023 23:06:09 GMT
CMD ["bash"]
# Mon, 18 Dec 2023 23:06:09 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg && rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV GOSU_VERSION=1.16
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN mkdir /docker-entrypoint-initdb.d # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	key='BCA4 3417 C3B4 85DD 128E C6D4 B7B3 B788 A8D3 785C'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_MAJOR=8.0
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_VERSION=8.0.35-1debian11
# Mon, 18 Dec 2023 23:06:09 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ bullseye mysql-8.0' > /etc/apt/sources.list.d/mysql.list # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
VOLUME [/var/lib/mysql]
# Mon, 18 Dec 2023 23:06:09 GMT
COPY config/ /etc/mysql/ # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 18 Dec 2023 23:06:09 GMT
EXPOSE map[3306/tcp:{} 33060/tcp:{}]
# Mon, 18 Dec 2023 23:06:09 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:b5a0d5c14ba9ece1eecd5137c468d9a123372b0af2ed2c8c4446137730c90e5b`  
		Last Modified: Tue, 19 Dec 2023 01:25:40 GMT  
		Size: 31.4 MB (31417873 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:da5817b65ce4cfccfbd1cab936288cc2c9f576106fd0ab111cddb3f49604b511`  
		Last Modified: Tue, 19 Dec 2023 03:48:09 GMT  
		Size: 1.6 KB (1648 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:22e837abaef2fbc36a2e530f662337e34b8657c6c7a8c5fa8985bd2da8558e88`  
		Last Modified: Tue, 19 Dec 2023 03:48:09 GMT  
		Size: 4.2 MB (4207553 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:20780fd9cbff99edbacd139c37874ca887f245bfcb551a864ae2d16d2796e66d`  
		Last Modified: Tue, 19 Dec 2023 03:48:10 GMT  
		Size: 1.5 MB (1472512 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:79fdc95bdfcd9c8e64e72e935d8cf5ead3f36df49822e4855a109cd7f02ad1da`  
		Last Modified: Tue, 19 Dec 2023 03:48:09 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6363b252c0190906b09055d3b005632c4e935437229d10bd1fde49edc0f09552`  
		Last Modified: Tue, 19 Dec 2023 03:48:10 GMT  
		Size: 12.5 MB (12455047 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:53763e330a11bdf71cdb59546001958be08d795253de155d76d3de7ca5cd0414`  
		Last Modified: Tue, 19 Dec 2023 03:48:10 GMT  
		Size: 2.5 KB (2497 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0f86f27fd6e32a832a7f07fca219bbf972cb94ac5eaeaf863956a7b6eed62325`  
		Last Modified: Tue, 19 Dec 2023 03:48:10 GMT  
		Size: 248.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f366e63462a4138b04a5404fb55d39d8319c2d32fb72a72aa0dfaaad7138c84d`  
		Last Modified: Tue, 19 Dec 2023 03:48:13 GMT  
		Size: 129.6 MB (129562666 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:253e0e751437680411c5e8fb4fcc53b9f8550407de309acfed0c90eefcc6e118`  
		Last Modified: Tue, 19 Dec 2023 03:48:11 GMT  
		Size: 843.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:36545369253738d314a9c0f1c27e796624b955d8421c3e76c206199838d60067`  
		Last Modified: Tue, 19 Dec 2023 03:48:11 GMT  
		Size: 5.2 KB (5178 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9c0d0816114713ba3afb8894fe438b4b455b71f36a17be963b18cde665d20dd2`  
		Last Modified: Tue, 19 Dec 2023 03:48:11 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:8.0.35-debian` - unknown; unknown

```console
$ docker pull mysql@sha256:c62f70ff2e4bb366308fe3fd509d1dd64808e2cd97872b409e7eafb90478bb17
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.6 MB (3587245 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b9696d74f06fc27194d39f6f22be3bbda0f9ca68d4399239252d6aa0ab2414fb`

```dockerfile
```

-	Layers:
	-	`sha256:01d50b5cf5a872322fba73f7e117e4f0a2d6e1ee97cbd1a7af58c52025cf8abe`  
		Last Modified: Tue, 19 Dec 2023 03:48:09 GMT  
		Size: 3.6 MB (3552993 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:eee7cfb8f5ef7f6fa00dcfa001913c382d4d8dca42cf15cb520f93802bdeea4b`  
		Last Modified: Tue, 19 Dec 2023 03:48:09 GMT  
		Size: 34.3 KB (34252 bytes)  
		MIME: application/vnd.in-toto+json

## `mysql:8.0.35-oracle`

```console
$ docker pull mysql@sha256:c80ef5968b6baf12e9ba95412d4725971207228e5274518db92e26d0e169372b
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `mysql:8.0.35-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:3a0b76a2ee46a23fc8e0c5e2d38d016a8466bbc774c933d719ae0b5308982dba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **173.7 MB (173728874 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba048db12589d011b77ab3ea33b7010d0b549214c8baa5fd885e4af84887928f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 18 Dec 2023 23:06:09 GMT
ADD file:da89b67e484bc45f357250a868fd78e28086b13e4315635d19648e5d43812e89 in / 
# Mon, 18 Dec 2023 23:06:09 GMT
CMD ["/bin/bash"]
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV GOSU_VERSION=1.16
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME" # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_MAJOR=8.0
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_VERSION=8.0.35-1.el8
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eu; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo 'baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/8/$basearch/'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eu; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo 'baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/8/$basearch/'; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_SHELL_VERSION=8.0.35-1.el8
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
VOLUME [/var/lib/mysql]
# Mon, 18 Dec 2023 23:06:09 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 18 Dec 2023 23:06:09 GMT
EXPOSE map[3306/tcp:{} 33060/tcp:{}]
# Mon, 18 Dec 2023 23:06:09 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:bce031bc522d421fb188ef82a530f85c5477bb87cdeacdb911ea86f3f7cd3b66`  
		Last Modified: Wed, 20 Dec 2023 22:42:00 GMT  
		Size: 51.3 MB (51323468 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9d95fc125cf8067473c7c0aeb06cc55f45268807b23568fbc3f14cab35d285cf`  
		Last Modified: Thu, 21 Dec 2023 00:42:07 GMT  
		Size: 890.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:22412d6d690fcd08a40e3808538b28c8ff614ca7d4292b97f91862c7d90f8279`  
		Last Modified: Thu, 21 Dec 2023 00:42:07 GMT  
		Size: 982.8 KB (982808 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:79d453aad0ebfa3f5472ee10df0b3e529d95ea63518574c69ceb52f5cf22d4c4`  
		Last Modified: Thu, 21 Dec 2023 00:42:07 GMT  
		Size: 4.6 MB (4594897 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1b6cca7a391de90190ab3ccfd94b95a59a48c0622005d5a5f5f364ac0c4c02e0`  
		Last Modified: Thu, 21 Dec 2023 00:42:07 GMT  
		Size: 2.6 KB (2604 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f9e7ae94329772a89c4c8e768d2f2209b96d4573ecf54dd50a679ddcaab6ec64`  
		Last Modified: Thu, 21 Dec 2023 00:42:08 GMT  
		Size: 332.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:af3e28b094a2e946679cb3f91d09922e2ae80bc117e6c3dc52016468e77ff1c9`  
		Last Modified: Thu, 21 Dec 2023 00:42:09 GMT  
		Size: 58.5 MB (58505933 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:db237bdcf1c0c61bb338e11bec6ba80c30afae0097636229de54a52fc9b2b41f`  
		Last Modified: Thu, 21 Dec 2023 00:42:08 GMT  
		Size: 315.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4b3c3f5cb4f4c88a98466d248ca0027a0abbd6d6301f0d166bd925eb58cf5ebd`  
		Last Modified: Thu, 21 Dec 2023 00:42:09 GMT  
		Size: 58.3 MB (58312328 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:394dbd7e05eb13c1f4b395b558b1c40b708996f1c5eb5dead40242895ce31121`  
		Last Modified: Thu, 21 Dec 2023 00:42:09 GMT  
		Size: 5.2 KB (5178 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:18a167e598b07c1067ec74fb4f63dd9a06c3baa1b6923afe66cfb4911c76632f`  
		Last Modified: Thu, 21 Dec 2023 00:42:09 GMT  
		Size: 121.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:8.0.35-oracle` - unknown; unknown

```console
$ docker pull mysql@sha256:e947f8eb99f01f51bb4a1a0506f0a5e23e03b48e78c68fb4931232b92bc96154
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.6 MB (11602599 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c396d9ca70fb4db2a43ca8d5ce6ab8de931e72363589fd41c168185836c0988b`

```dockerfile
```

-	Layers:
	-	`sha256:e5579f8c4a1d658618ca9a6429cc1f69801c829936675aed2b3837bd7b03ba46`  
		Last Modified: Thu, 21 Dec 2023 00:42:07 GMT  
		Size: 11.6 MB (11568051 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:c65568400f27660daae64a470173a41ed0af8ec67a24a230eae4e6ff1d0a53d8`  
		Last Modified: Thu, 21 Dec 2023 00:42:07 GMT  
		Size: 34.5 KB (34548 bytes)  
		MIME: application/vnd.in-toto+json

### `mysql:8.0.35-oracle` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:1fd4aa0943c8abc8bc478aea910779854c9f5375ba776a0413afe127006436e4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **177.4 MB (177445080 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9fdb9342cc99594cd3a8428facc5dcf87588c74f2c9991e75055c8ed8bb457db`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 06 Dec 2023 19:42:27 GMT
ADD file:f5ee75151bd25b33e72aa4c0560815f35f6e662876bf3733a02e5cb970227358 in / 
# Wed, 06 Dec 2023 19:42:27 GMT
CMD ["/bin/bash"]
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV GOSU_VERSION=1.16
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME" # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_MAJOR=8.0
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_VERSION=8.0.35-1.el8
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eu; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo 'baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/8/$basearch/'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eu; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo 'baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/8/$basearch/'; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_SHELL_VERSION=8.0.35-1.el8
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
VOLUME [/var/lib/mysql]
# Mon, 18 Dec 2023 23:06:09 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 18 Dec 2023 23:06:09 GMT
EXPOSE map[3306/tcp:{} 33060/tcp:{}]
# Mon, 18 Dec 2023 23:06:09 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:edfaa6c9daada52a737333e0818f3d697d745aab3f3351e773218a524ebc9e53`  
		Last Modified: Wed, 06 Dec 2023 19:43:23 GMT  
		Size: 50.1 MB (50072545 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:19c686b91aca61da8058a44e9f6aa06cbb27aa65cf2db0768377bcc6899dc0c2`  
		Last Modified: Thu, 14 Dec 2023 20:15:05 GMT  
		Size: 885.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8c39062282e36f6169d219352cb19810ac7506e408e89b4ef33c400903a6ecc1`  
		Last Modified: Thu, 14 Dec 2023 20:15:05 GMT  
		Size: 913.0 KB (912965 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:73452dd561ff872804f5a63faab7552647c80c8a399e834fe154707a48613b20`  
		Last Modified: Thu, 14 Dec 2023 20:15:05 GMT  
		Size: 4.3 MB (4300794 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0ba54e261f50c32496de78ff38c42eb03cb97850ddbeb3c96f4fe34ea1cb23bc`  
		Last Modified: Thu, 14 Dec 2023 20:15:05 GMT  
		Size: 2.6 KB (2609 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f8a2d4a8cba602b5e3cd65d5e0557988bcbd78b091afb3f6ae0d15864790987f`  
		Last Modified: Thu, 14 Dec 2023 20:16:54 GMT  
		Size: 332.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e6ba09d9fb3dfd35ff7ebbb6eb20bd59a35b737aec5e0e2f2c42eb50dda9d1e1`  
		Last Modified: Thu, 14 Dec 2023 20:16:56 GMT  
		Size: 57.6 MB (57573677 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3039dd1391bc16761b31a730472044ed80f3817b431f9de14e0b2b9e5949a66e`  
		Last Modified: Thu, 14 Dec 2023 20:16:54 GMT  
		Size: 316.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ad4d0901f4a72dd35f6f7f609dbcc9e9d4cc321ed55cad8b778a73cd0e8b4132`  
		Last Modified: Thu, 14 Dec 2023 20:16:56 GMT  
		Size: 64.6 MB (64575659 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e07375f3b7d754961d4d4dab48979ab0ff5a27d70949da753b98f86e075f16ba`  
		Last Modified: Tue, 19 Dec 2023 22:04:07 GMT  
		Size: 5.2 KB (5178 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6e4d42b5ded666fd53f1cfa7026d0fcdf1222cebf111756700d3ea573e069a99`  
		Last Modified: Tue, 19 Dec 2023 22:04:07 GMT  
		Size: 120.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:8.0.35-oracle` - unknown; unknown

```console
$ docker pull mysql@sha256:cb0dde16b43ff62c5e9a8293635a3e506404e3942f91170a5624de10dbcc3c6b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.6 MB (11601006 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b517449c77273c30cf2ea6ee95149207a40bdcc2657a73ee0bdcf8cb8d32f8ff`

```dockerfile
```

-	Layers:
	-	`sha256:7540cc15c09e88ca43d3a437e9e95e9e0763f75f5f13a14201e79ad422ea1aeb`  
		Last Modified: Tue, 19 Dec 2023 22:04:07 GMT  
		Size: 11.6 MB (11566611 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:4947d50d277de5c30205c9c1354c1d66254980e8e4bf4796a6abaeda465c1125`  
		Last Modified: Tue, 19 Dec 2023 22:04:06 GMT  
		Size: 34.4 KB (34395 bytes)  
		MIME: application/vnd.in-toto+json

## `mysql:8.0.35-oraclelinux8`

```console
$ docker pull mysql@sha256:c80ef5968b6baf12e9ba95412d4725971207228e5274518db92e26d0e169372b
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `mysql:8.0.35-oraclelinux8` - linux; amd64

```console
$ docker pull mysql@sha256:3a0b76a2ee46a23fc8e0c5e2d38d016a8466bbc774c933d719ae0b5308982dba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **173.7 MB (173728874 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba048db12589d011b77ab3ea33b7010d0b549214c8baa5fd885e4af84887928f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 18 Dec 2023 23:06:09 GMT
ADD file:da89b67e484bc45f357250a868fd78e28086b13e4315635d19648e5d43812e89 in / 
# Mon, 18 Dec 2023 23:06:09 GMT
CMD ["/bin/bash"]
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV GOSU_VERSION=1.16
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME" # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_MAJOR=8.0
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_VERSION=8.0.35-1.el8
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eu; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo 'baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/8/$basearch/'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eu; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo 'baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/8/$basearch/'; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_SHELL_VERSION=8.0.35-1.el8
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
VOLUME [/var/lib/mysql]
# Mon, 18 Dec 2023 23:06:09 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 18 Dec 2023 23:06:09 GMT
EXPOSE map[3306/tcp:{} 33060/tcp:{}]
# Mon, 18 Dec 2023 23:06:09 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:bce031bc522d421fb188ef82a530f85c5477bb87cdeacdb911ea86f3f7cd3b66`  
		Last Modified: Wed, 20 Dec 2023 22:42:00 GMT  
		Size: 51.3 MB (51323468 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9d95fc125cf8067473c7c0aeb06cc55f45268807b23568fbc3f14cab35d285cf`  
		Last Modified: Thu, 21 Dec 2023 00:42:07 GMT  
		Size: 890.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:22412d6d690fcd08a40e3808538b28c8ff614ca7d4292b97f91862c7d90f8279`  
		Last Modified: Thu, 21 Dec 2023 00:42:07 GMT  
		Size: 982.8 KB (982808 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:79d453aad0ebfa3f5472ee10df0b3e529d95ea63518574c69ceb52f5cf22d4c4`  
		Last Modified: Thu, 21 Dec 2023 00:42:07 GMT  
		Size: 4.6 MB (4594897 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1b6cca7a391de90190ab3ccfd94b95a59a48c0622005d5a5f5f364ac0c4c02e0`  
		Last Modified: Thu, 21 Dec 2023 00:42:07 GMT  
		Size: 2.6 KB (2604 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f9e7ae94329772a89c4c8e768d2f2209b96d4573ecf54dd50a679ddcaab6ec64`  
		Last Modified: Thu, 21 Dec 2023 00:42:08 GMT  
		Size: 332.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:af3e28b094a2e946679cb3f91d09922e2ae80bc117e6c3dc52016468e77ff1c9`  
		Last Modified: Thu, 21 Dec 2023 00:42:09 GMT  
		Size: 58.5 MB (58505933 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:db237bdcf1c0c61bb338e11bec6ba80c30afae0097636229de54a52fc9b2b41f`  
		Last Modified: Thu, 21 Dec 2023 00:42:08 GMT  
		Size: 315.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4b3c3f5cb4f4c88a98466d248ca0027a0abbd6d6301f0d166bd925eb58cf5ebd`  
		Last Modified: Thu, 21 Dec 2023 00:42:09 GMT  
		Size: 58.3 MB (58312328 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:394dbd7e05eb13c1f4b395b558b1c40b708996f1c5eb5dead40242895ce31121`  
		Last Modified: Thu, 21 Dec 2023 00:42:09 GMT  
		Size: 5.2 KB (5178 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:18a167e598b07c1067ec74fb4f63dd9a06c3baa1b6923afe66cfb4911c76632f`  
		Last Modified: Thu, 21 Dec 2023 00:42:09 GMT  
		Size: 121.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:8.0.35-oraclelinux8` - unknown; unknown

```console
$ docker pull mysql@sha256:e947f8eb99f01f51bb4a1a0506f0a5e23e03b48e78c68fb4931232b92bc96154
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.6 MB (11602599 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c396d9ca70fb4db2a43ca8d5ce6ab8de931e72363589fd41c168185836c0988b`

```dockerfile
```

-	Layers:
	-	`sha256:e5579f8c4a1d658618ca9a6429cc1f69801c829936675aed2b3837bd7b03ba46`  
		Last Modified: Thu, 21 Dec 2023 00:42:07 GMT  
		Size: 11.6 MB (11568051 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:c65568400f27660daae64a470173a41ed0af8ec67a24a230eae4e6ff1d0a53d8`  
		Last Modified: Thu, 21 Dec 2023 00:42:07 GMT  
		Size: 34.5 KB (34548 bytes)  
		MIME: application/vnd.in-toto+json

### `mysql:8.0.35-oraclelinux8` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:1fd4aa0943c8abc8bc478aea910779854c9f5375ba776a0413afe127006436e4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **177.4 MB (177445080 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9fdb9342cc99594cd3a8428facc5dcf87588c74f2c9991e75055c8ed8bb457db`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 06 Dec 2023 19:42:27 GMT
ADD file:f5ee75151bd25b33e72aa4c0560815f35f6e662876bf3733a02e5cb970227358 in / 
# Wed, 06 Dec 2023 19:42:27 GMT
CMD ["/bin/bash"]
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV GOSU_VERSION=1.16
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME" # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_MAJOR=8.0
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_VERSION=8.0.35-1.el8
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eu; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo 'baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/8/$basearch/'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eu; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo 'baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/8/$basearch/'; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_SHELL_VERSION=8.0.35-1.el8
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
VOLUME [/var/lib/mysql]
# Mon, 18 Dec 2023 23:06:09 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 18 Dec 2023 23:06:09 GMT
EXPOSE map[3306/tcp:{} 33060/tcp:{}]
# Mon, 18 Dec 2023 23:06:09 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:edfaa6c9daada52a737333e0818f3d697d745aab3f3351e773218a524ebc9e53`  
		Last Modified: Wed, 06 Dec 2023 19:43:23 GMT  
		Size: 50.1 MB (50072545 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:19c686b91aca61da8058a44e9f6aa06cbb27aa65cf2db0768377bcc6899dc0c2`  
		Last Modified: Thu, 14 Dec 2023 20:15:05 GMT  
		Size: 885.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8c39062282e36f6169d219352cb19810ac7506e408e89b4ef33c400903a6ecc1`  
		Last Modified: Thu, 14 Dec 2023 20:15:05 GMT  
		Size: 913.0 KB (912965 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:73452dd561ff872804f5a63faab7552647c80c8a399e834fe154707a48613b20`  
		Last Modified: Thu, 14 Dec 2023 20:15:05 GMT  
		Size: 4.3 MB (4300794 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0ba54e261f50c32496de78ff38c42eb03cb97850ddbeb3c96f4fe34ea1cb23bc`  
		Last Modified: Thu, 14 Dec 2023 20:15:05 GMT  
		Size: 2.6 KB (2609 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f8a2d4a8cba602b5e3cd65d5e0557988bcbd78b091afb3f6ae0d15864790987f`  
		Last Modified: Thu, 14 Dec 2023 20:16:54 GMT  
		Size: 332.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e6ba09d9fb3dfd35ff7ebbb6eb20bd59a35b737aec5e0e2f2c42eb50dda9d1e1`  
		Last Modified: Thu, 14 Dec 2023 20:16:56 GMT  
		Size: 57.6 MB (57573677 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3039dd1391bc16761b31a730472044ed80f3817b431f9de14e0b2b9e5949a66e`  
		Last Modified: Thu, 14 Dec 2023 20:16:54 GMT  
		Size: 316.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ad4d0901f4a72dd35f6f7f609dbcc9e9d4cc321ed55cad8b778a73cd0e8b4132`  
		Last Modified: Thu, 14 Dec 2023 20:16:56 GMT  
		Size: 64.6 MB (64575659 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e07375f3b7d754961d4d4dab48979ab0ff5a27d70949da753b98f86e075f16ba`  
		Last Modified: Tue, 19 Dec 2023 22:04:07 GMT  
		Size: 5.2 KB (5178 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6e4d42b5ded666fd53f1cfa7026d0fcdf1222cebf111756700d3ea573e069a99`  
		Last Modified: Tue, 19 Dec 2023 22:04:07 GMT  
		Size: 120.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:8.0.35-oraclelinux8` - unknown; unknown

```console
$ docker pull mysql@sha256:cb0dde16b43ff62c5e9a8293635a3e506404e3942f91170a5624de10dbcc3c6b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.6 MB (11601006 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b517449c77273c30cf2ea6ee95149207a40bdcc2657a73ee0bdcf8cb8d32f8ff`

```dockerfile
```

-	Layers:
	-	`sha256:7540cc15c09e88ca43d3a437e9e95e9e0763f75f5f13a14201e79ad422ea1aeb`  
		Last Modified: Tue, 19 Dec 2023 22:04:07 GMT  
		Size: 11.6 MB (11566611 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:4947d50d277de5c30205c9c1354c1d66254980e8e4bf4796a6abaeda465c1125`  
		Last Modified: Tue, 19 Dec 2023 22:04:06 GMT  
		Size: 34.4 KB (34395 bytes)  
		MIME: application/vnd.in-toto+json

## `mysql:8.2`

```console
$ docker pull mysql@sha256:2d82ba6960cdf254de13f57d7265570c0675bc8bae1051e4a9806cff863006c9
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `mysql:8.2` - linux; amd64

```console
$ docker pull mysql@sha256:28a16e31b140d750048cd5fadcaed22ac08d0eeb18567f79f822aee1f237b43c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **181.6 MB (181572393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73246731c4b01c19b8713c6408c6c5d898ac04f75f2a4ce998930f12091542f2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 18 Dec 2023 23:06:09 GMT
ADD file:da89b67e484bc45f357250a868fd78e28086b13e4315635d19648e5d43812e89 in / 
# Mon, 18 Dec 2023 23:06:09 GMT
CMD ["/bin/bash"]
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV GOSU_VERSION=1.16
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME" # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_MAJOR=innovation
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_VERSION=8.2.0-1.el8
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eu; 	{ 		echo '[mysqlinnovation-server-minimal]'; 		echo 'name=MySQL innovation Server Minimal'; 		echo 'enabled=1'; 		echo 'baseurl=https://repo.mysql.com/yum/mysql-innovation-community/docker/el/8/$basearch/'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eu; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo 'baseurl=https://repo.mysql.com/yum/mysql-tools-innovation-community/el/8/$basearch/'; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_SHELL_VERSION=8.2.1-1.el8
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
VOLUME [/var/lib/mysql]
# Mon, 18 Dec 2023 23:06:09 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 18 Dec 2023 23:06:09 GMT
EXPOSE map[3306/tcp:{} 33060/tcp:{}]
# Mon, 18 Dec 2023 23:06:09 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:bce031bc522d421fb188ef82a530f85c5477bb87cdeacdb911ea86f3f7cd3b66`  
		Last Modified: Wed, 20 Dec 2023 22:42:00 GMT  
		Size: 51.3 MB (51323468 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cf7e9f463619cbda1168fb597e71ce50b4ecd4546ad74050f5b5c67a152ca249`  
		Last Modified: Thu, 21 Dec 2023 00:41:48 GMT  
		Size: 883.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:105f403783c74e137d330ef98facdded2cab753187765ed8c453bb7b061a0002`  
		Last Modified: Thu, 21 Dec 2023 00:41:48 GMT  
		Size: 982.8 KB (982809 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:878e53a613d8011ad3d6207863d1555fe571430d3c6f7659d1eb0fd7f28ba7de`  
		Last Modified: Thu, 21 Dec 2023 00:41:48 GMT  
		Size: 4.6 MB (4594819 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2a362044e79fb6669726216e996a0a9fa018ba304d75ac30c9378a93160182de`  
		Last Modified: Thu, 21 Dec 2023 00:41:48 GMT  
		Size: 2.6 KB (2608 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6e4df4f73cfe883156b974e5269c673e52de0e1a56d610f2974793cd52d8b043`  
		Last Modified: Thu, 21 Dec 2023 00:41:49 GMT  
		Size: 340.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:69263d6347550e51a3b3f972d5aee303fd3c8c6d75376aad0b4cdcd4cb3f83be`  
		Last Modified: Thu, 21 Dec 2023 00:41:49 GMT  
		Size: 62.6 MB (62574253 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fe5e855492024c60c48d8eb006c94b71d6622f6d5c741cfa611e571a88a67d37`  
		Last Modified: Thu, 21 Dec 2023 00:41:49 GMT  
		Size: 325.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5c02229ce6f164ee6c47c91ddaa42db249b197b8b28dc6814a4df879a4f96a3e`  
		Last Modified: Thu, 21 Dec 2023 00:41:50 GMT  
		Size: 62.1 MB (62087711 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7320aa32bf42c0642bc86e30dac0b10335258a24b6ba374e173918ba8d9f9f63`  
		Last Modified: Thu, 21 Dec 2023 00:41:49 GMT  
		Size: 5.2 KB (5177 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:8.2` - unknown; unknown

```console
$ docker pull mysql@sha256:483bf8eb111365bf322a25443d3f96ae0d80829c60f00fb329d8a0de0f21c6e7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.6 MB (11608021 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:501f9b1df36151d7e7ebba69fac20d69995d956d3851313ac3b4fdf9fa4e9ad3`

```dockerfile
```

-	Layers:
	-	`sha256:8de9290b82bb48a07e68ea96148c288ffa09729055d5c506b7690cf42f948baf`  
		Last Modified: Thu, 21 Dec 2023 00:41:48 GMT  
		Size: 11.6 MB (11573114 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:0b8a63c307592189c7a4ea188ee3b5e76eba99edc475a34c635157d5e893e536`  
		Last Modified: Thu, 21 Dec 2023 00:41:48 GMT  
		Size: 34.9 KB (34907 bytes)  
		MIME: application/vnd.in-toto+json

### `mysql:8.2` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:86f5987d89514a0ec8043202ba341717c6d2f726749924ef7f220839ac576cf8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **185.3 MB (185275916 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e963a4c2b1a0d8774a4b6138a86d2bcca8b8f5cec58fbfabf7ae4ae021159e0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 06 Dec 2023 19:42:27 GMT
ADD file:f5ee75151bd25b33e72aa4c0560815f35f6e662876bf3733a02e5cb970227358 in / 
# Wed, 06 Dec 2023 19:42:27 GMT
CMD ["/bin/bash"]
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV GOSU_VERSION=1.16
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME" # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_MAJOR=innovation
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_VERSION=8.2.0-1.el8
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eu; 	{ 		echo '[mysqlinnovation-server-minimal]'; 		echo 'name=MySQL innovation Server Minimal'; 		echo 'enabled=1'; 		echo 'baseurl=https://repo.mysql.com/yum/mysql-innovation-community/docker/el/8/$basearch/'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eu; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo 'baseurl=https://repo.mysql.com/yum/mysql-tools-innovation-community/el/8/$basearch/'; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_SHELL_VERSION=8.2.1-1.el8
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
VOLUME [/var/lib/mysql]
# Mon, 18 Dec 2023 23:06:09 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 18 Dec 2023 23:06:09 GMT
EXPOSE map[3306/tcp:{} 33060/tcp:{}]
# Mon, 18 Dec 2023 23:06:09 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:edfaa6c9daada52a737333e0818f3d697d745aab3f3351e773218a524ebc9e53`  
		Last Modified: Wed, 06 Dec 2023 19:43:23 GMT  
		Size: 50.1 MB (50072545 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:19c686b91aca61da8058a44e9f6aa06cbb27aa65cf2db0768377bcc6899dc0c2`  
		Last Modified: Thu, 14 Dec 2023 20:15:05 GMT  
		Size: 885.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8c39062282e36f6169d219352cb19810ac7506e408e89b4ef33c400903a6ecc1`  
		Last Modified: Thu, 14 Dec 2023 20:15:05 GMT  
		Size: 913.0 KB (912965 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:73452dd561ff872804f5a63faab7552647c80c8a399e834fe154707a48613b20`  
		Last Modified: Thu, 14 Dec 2023 20:15:05 GMT  
		Size: 4.3 MB (4300794 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0ba54e261f50c32496de78ff38c42eb03cb97850ddbeb3c96f4fe34ea1cb23bc`  
		Last Modified: Thu, 14 Dec 2023 20:15:05 GMT  
		Size: 2.6 KB (2609 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b22c0fd6cce4772b17fe2500d6ce97e3a35076112226cc23269afa1542f7b51d`  
		Last Modified: Thu, 14 Dec 2023 20:15:06 GMT  
		Size: 340.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:eaffd91cbb1278d374c5b91f8a3e87239e73b0113a1fa5835faf13bcb05948dc`  
		Last Modified: Thu, 14 Dec 2023 20:15:09 GMT  
		Size: 61.6 MB (61602995 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3ec60922d8e9eefbce5167faf6f2296ddec22dcafc9a84f5db6f94e92e032089`  
		Last Modified: Thu, 14 Dec 2023 20:15:07 GMT  
		Size: 325.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:942dbd5bb0a98d45556f650aa3174e3e4a5fcf822e5e7a67529ae622bb02b14a`  
		Last Modified: Thu, 14 Dec 2023 20:15:09 GMT  
		Size: 68.4 MB (68377279 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bc7ea546f5793dcfecf365aefc956d7999a086211dc195cbb5d73d09df397fe2`  
		Last Modified: Tue, 19 Dec 2023 21:07:09 GMT  
		Size: 5.2 KB (5179 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:8.2` - unknown; unknown

```console
$ docker pull mysql@sha256:9b1966fea33a8f487098b70ebc30c23b2700a8731bcff2bd124779ba2f8cf2be
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.6 MB (11606464 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:557704055f52c52ae3fcc218fa7168216870eca8326c1b1e89d434ad3ec00204`

```dockerfile
```

-	Layers:
	-	`sha256:0b211226c249aefed58e7da4b41bb3219beb5345fe5ed4e65c65ab47e378292b`  
		Last Modified: Tue, 19 Dec 2023 21:07:09 GMT  
		Size: 11.6 MB (11571692 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:097024790a6d6019cd411ce0478476fbfebc733402110550a33d6009f3aca07d`  
		Last Modified: Tue, 19 Dec 2023 21:07:09 GMT  
		Size: 34.8 KB (34772 bytes)  
		MIME: application/vnd.in-toto+json

## `mysql:8.2-oracle`

```console
$ docker pull mysql@sha256:2d82ba6960cdf254de13f57d7265570c0675bc8bae1051e4a9806cff863006c9
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `mysql:8.2-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:28a16e31b140d750048cd5fadcaed22ac08d0eeb18567f79f822aee1f237b43c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **181.6 MB (181572393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73246731c4b01c19b8713c6408c6c5d898ac04f75f2a4ce998930f12091542f2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 18 Dec 2023 23:06:09 GMT
ADD file:da89b67e484bc45f357250a868fd78e28086b13e4315635d19648e5d43812e89 in / 
# Mon, 18 Dec 2023 23:06:09 GMT
CMD ["/bin/bash"]
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV GOSU_VERSION=1.16
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME" # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_MAJOR=innovation
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_VERSION=8.2.0-1.el8
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eu; 	{ 		echo '[mysqlinnovation-server-minimal]'; 		echo 'name=MySQL innovation Server Minimal'; 		echo 'enabled=1'; 		echo 'baseurl=https://repo.mysql.com/yum/mysql-innovation-community/docker/el/8/$basearch/'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eu; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo 'baseurl=https://repo.mysql.com/yum/mysql-tools-innovation-community/el/8/$basearch/'; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_SHELL_VERSION=8.2.1-1.el8
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
VOLUME [/var/lib/mysql]
# Mon, 18 Dec 2023 23:06:09 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 18 Dec 2023 23:06:09 GMT
EXPOSE map[3306/tcp:{} 33060/tcp:{}]
# Mon, 18 Dec 2023 23:06:09 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:bce031bc522d421fb188ef82a530f85c5477bb87cdeacdb911ea86f3f7cd3b66`  
		Last Modified: Wed, 20 Dec 2023 22:42:00 GMT  
		Size: 51.3 MB (51323468 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cf7e9f463619cbda1168fb597e71ce50b4ecd4546ad74050f5b5c67a152ca249`  
		Last Modified: Thu, 21 Dec 2023 00:41:48 GMT  
		Size: 883.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:105f403783c74e137d330ef98facdded2cab753187765ed8c453bb7b061a0002`  
		Last Modified: Thu, 21 Dec 2023 00:41:48 GMT  
		Size: 982.8 KB (982809 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:878e53a613d8011ad3d6207863d1555fe571430d3c6f7659d1eb0fd7f28ba7de`  
		Last Modified: Thu, 21 Dec 2023 00:41:48 GMT  
		Size: 4.6 MB (4594819 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2a362044e79fb6669726216e996a0a9fa018ba304d75ac30c9378a93160182de`  
		Last Modified: Thu, 21 Dec 2023 00:41:48 GMT  
		Size: 2.6 KB (2608 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6e4df4f73cfe883156b974e5269c673e52de0e1a56d610f2974793cd52d8b043`  
		Last Modified: Thu, 21 Dec 2023 00:41:49 GMT  
		Size: 340.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:69263d6347550e51a3b3f972d5aee303fd3c8c6d75376aad0b4cdcd4cb3f83be`  
		Last Modified: Thu, 21 Dec 2023 00:41:49 GMT  
		Size: 62.6 MB (62574253 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fe5e855492024c60c48d8eb006c94b71d6622f6d5c741cfa611e571a88a67d37`  
		Last Modified: Thu, 21 Dec 2023 00:41:49 GMT  
		Size: 325.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5c02229ce6f164ee6c47c91ddaa42db249b197b8b28dc6814a4df879a4f96a3e`  
		Last Modified: Thu, 21 Dec 2023 00:41:50 GMT  
		Size: 62.1 MB (62087711 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7320aa32bf42c0642bc86e30dac0b10335258a24b6ba374e173918ba8d9f9f63`  
		Last Modified: Thu, 21 Dec 2023 00:41:49 GMT  
		Size: 5.2 KB (5177 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:8.2-oracle` - unknown; unknown

```console
$ docker pull mysql@sha256:483bf8eb111365bf322a25443d3f96ae0d80829c60f00fb329d8a0de0f21c6e7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.6 MB (11608021 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:501f9b1df36151d7e7ebba69fac20d69995d956d3851313ac3b4fdf9fa4e9ad3`

```dockerfile
```

-	Layers:
	-	`sha256:8de9290b82bb48a07e68ea96148c288ffa09729055d5c506b7690cf42f948baf`  
		Last Modified: Thu, 21 Dec 2023 00:41:48 GMT  
		Size: 11.6 MB (11573114 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:0b8a63c307592189c7a4ea188ee3b5e76eba99edc475a34c635157d5e893e536`  
		Last Modified: Thu, 21 Dec 2023 00:41:48 GMT  
		Size: 34.9 KB (34907 bytes)  
		MIME: application/vnd.in-toto+json

### `mysql:8.2-oracle` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:86f5987d89514a0ec8043202ba341717c6d2f726749924ef7f220839ac576cf8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **185.3 MB (185275916 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e963a4c2b1a0d8774a4b6138a86d2bcca8b8f5cec58fbfabf7ae4ae021159e0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 06 Dec 2023 19:42:27 GMT
ADD file:f5ee75151bd25b33e72aa4c0560815f35f6e662876bf3733a02e5cb970227358 in / 
# Wed, 06 Dec 2023 19:42:27 GMT
CMD ["/bin/bash"]
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV GOSU_VERSION=1.16
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME" # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_MAJOR=innovation
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_VERSION=8.2.0-1.el8
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eu; 	{ 		echo '[mysqlinnovation-server-minimal]'; 		echo 'name=MySQL innovation Server Minimal'; 		echo 'enabled=1'; 		echo 'baseurl=https://repo.mysql.com/yum/mysql-innovation-community/docker/el/8/$basearch/'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eu; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo 'baseurl=https://repo.mysql.com/yum/mysql-tools-innovation-community/el/8/$basearch/'; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_SHELL_VERSION=8.2.1-1.el8
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
VOLUME [/var/lib/mysql]
# Mon, 18 Dec 2023 23:06:09 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 18 Dec 2023 23:06:09 GMT
EXPOSE map[3306/tcp:{} 33060/tcp:{}]
# Mon, 18 Dec 2023 23:06:09 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:edfaa6c9daada52a737333e0818f3d697d745aab3f3351e773218a524ebc9e53`  
		Last Modified: Wed, 06 Dec 2023 19:43:23 GMT  
		Size: 50.1 MB (50072545 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:19c686b91aca61da8058a44e9f6aa06cbb27aa65cf2db0768377bcc6899dc0c2`  
		Last Modified: Thu, 14 Dec 2023 20:15:05 GMT  
		Size: 885.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8c39062282e36f6169d219352cb19810ac7506e408e89b4ef33c400903a6ecc1`  
		Last Modified: Thu, 14 Dec 2023 20:15:05 GMT  
		Size: 913.0 KB (912965 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:73452dd561ff872804f5a63faab7552647c80c8a399e834fe154707a48613b20`  
		Last Modified: Thu, 14 Dec 2023 20:15:05 GMT  
		Size: 4.3 MB (4300794 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0ba54e261f50c32496de78ff38c42eb03cb97850ddbeb3c96f4fe34ea1cb23bc`  
		Last Modified: Thu, 14 Dec 2023 20:15:05 GMT  
		Size: 2.6 KB (2609 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b22c0fd6cce4772b17fe2500d6ce97e3a35076112226cc23269afa1542f7b51d`  
		Last Modified: Thu, 14 Dec 2023 20:15:06 GMT  
		Size: 340.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:eaffd91cbb1278d374c5b91f8a3e87239e73b0113a1fa5835faf13bcb05948dc`  
		Last Modified: Thu, 14 Dec 2023 20:15:09 GMT  
		Size: 61.6 MB (61602995 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3ec60922d8e9eefbce5167faf6f2296ddec22dcafc9a84f5db6f94e92e032089`  
		Last Modified: Thu, 14 Dec 2023 20:15:07 GMT  
		Size: 325.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:942dbd5bb0a98d45556f650aa3174e3e4a5fcf822e5e7a67529ae622bb02b14a`  
		Last Modified: Thu, 14 Dec 2023 20:15:09 GMT  
		Size: 68.4 MB (68377279 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bc7ea546f5793dcfecf365aefc956d7999a086211dc195cbb5d73d09df397fe2`  
		Last Modified: Tue, 19 Dec 2023 21:07:09 GMT  
		Size: 5.2 KB (5179 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:8.2-oracle` - unknown; unknown

```console
$ docker pull mysql@sha256:9b1966fea33a8f487098b70ebc30c23b2700a8731bcff2bd124779ba2f8cf2be
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.6 MB (11606464 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:557704055f52c52ae3fcc218fa7168216870eca8326c1b1e89d434ad3ec00204`

```dockerfile
```

-	Layers:
	-	`sha256:0b211226c249aefed58e7da4b41bb3219beb5345fe5ed4e65c65ab47e378292b`  
		Last Modified: Tue, 19 Dec 2023 21:07:09 GMT  
		Size: 11.6 MB (11571692 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:097024790a6d6019cd411ce0478476fbfebc733402110550a33d6009f3aca07d`  
		Last Modified: Tue, 19 Dec 2023 21:07:09 GMT  
		Size: 34.8 KB (34772 bytes)  
		MIME: application/vnd.in-toto+json

## `mysql:8.2-oraclelinux8`

```console
$ docker pull mysql@sha256:2d82ba6960cdf254de13f57d7265570c0675bc8bae1051e4a9806cff863006c9
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `mysql:8.2-oraclelinux8` - linux; amd64

```console
$ docker pull mysql@sha256:28a16e31b140d750048cd5fadcaed22ac08d0eeb18567f79f822aee1f237b43c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **181.6 MB (181572393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73246731c4b01c19b8713c6408c6c5d898ac04f75f2a4ce998930f12091542f2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 18 Dec 2023 23:06:09 GMT
ADD file:da89b67e484bc45f357250a868fd78e28086b13e4315635d19648e5d43812e89 in / 
# Mon, 18 Dec 2023 23:06:09 GMT
CMD ["/bin/bash"]
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV GOSU_VERSION=1.16
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME" # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_MAJOR=innovation
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_VERSION=8.2.0-1.el8
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eu; 	{ 		echo '[mysqlinnovation-server-minimal]'; 		echo 'name=MySQL innovation Server Minimal'; 		echo 'enabled=1'; 		echo 'baseurl=https://repo.mysql.com/yum/mysql-innovation-community/docker/el/8/$basearch/'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eu; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo 'baseurl=https://repo.mysql.com/yum/mysql-tools-innovation-community/el/8/$basearch/'; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_SHELL_VERSION=8.2.1-1.el8
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
VOLUME [/var/lib/mysql]
# Mon, 18 Dec 2023 23:06:09 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 18 Dec 2023 23:06:09 GMT
EXPOSE map[3306/tcp:{} 33060/tcp:{}]
# Mon, 18 Dec 2023 23:06:09 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:bce031bc522d421fb188ef82a530f85c5477bb87cdeacdb911ea86f3f7cd3b66`  
		Last Modified: Wed, 20 Dec 2023 22:42:00 GMT  
		Size: 51.3 MB (51323468 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cf7e9f463619cbda1168fb597e71ce50b4ecd4546ad74050f5b5c67a152ca249`  
		Last Modified: Thu, 21 Dec 2023 00:41:48 GMT  
		Size: 883.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:105f403783c74e137d330ef98facdded2cab753187765ed8c453bb7b061a0002`  
		Last Modified: Thu, 21 Dec 2023 00:41:48 GMT  
		Size: 982.8 KB (982809 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:878e53a613d8011ad3d6207863d1555fe571430d3c6f7659d1eb0fd7f28ba7de`  
		Last Modified: Thu, 21 Dec 2023 00:41:48 GMT  
		Size: 4.6 MB (4594819 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2a362044e79fb6669726216e996a0a9fa018ba304d75ac30c9378a93160182de`  
		Last Modified: Thu, 21 Dec 2023 00:41:48 GMT  
		Size: 2.6 KB (2608 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6e4df4f73cfe883156b974e5269c673e52de0e1a56d610f2974793cd52d8b043`  
		Last Modified: Thu, 21 Dec 2023 00:41:49 GMT  
		Size: 340.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:69263d6347550e51a3b3f972d5aee303fd3c8c6d75376aad0b4cdcd4cb3f83be`  
		Last Modified: Thu, 21 Dec 2023 00:41:49 GMT  
		Size: 62.6 MB (62574253 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fe5e855492024c60c48d8eb006c94b71d6622f6d5c741cfa611e571a88a67d37`  
		Last Modified: Thu, 21 Dec 2023 00:41:49 GMT  
		Size: 325.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5c02229ce6f164ee6c47c91ddaa42db249b197b8b28dc6814a4df879a4f96a3e`  
		Last Modified: Thu, 21 Dec 2023 00:41:50 GMT  
		Size: 62.1 MB (62087711 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7320aa32bf42c0642bc86e30dac0b10335258a24b6ba374e173918ba8d9f9f63`  
		Last Modified: Thu, 21 Dec 2023 00:41:49 GMT  
		Size: 5.2 KB (5177 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:8.2-oraclelinux8` - unknown; unknown

```console
$ docker pull mysql@sha256:483bf8eb111365bf322a25443d3f96ae0d80829c60f00fb329d8a0de0f21c6e7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.6 MB (11608021 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:501f9b1df36151d7e7ebba69fac20d69995d956d3851313ac3b4fdf9fa4e9ad3`

```dockerfile
```

-	Layers:
	-	`sha256:8de9290b82bb48a07e68ea96148c288ffa09729055d5c506b7690cf42f948baf`  
		Last Modified: Thu, 21 Dec 2023 00:41:48 GMT  
		Size: 11.6 MB (11573114 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:0b8a63c307592189c7a4ea188ee3b5e76eba99edc475a34c635157d5e893e536`  
		Last Modified: Thu, 21 Dec 2023 00:41:48 GMT  
		Size: 34.9 KB (34907 bytes)  
		MIME: application/vnd.in-toto+json

### `mysql:8.2-oraclelinux8` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:86f5987d89514a0ec8043202ba341717c6d2f726749924ef7f220839ac576cf8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **185.3 MB (185275916 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e963a4c2b1a0d8774a4b6138a86d2bcca8b8f5cec58fbfabf7ae4ae021159e0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 06 Dec 2023 19:42:27 GMT
ADD file:f5ee75151bd25b33e72aa4c0560815f35f6e662876bf3733a02e5cb970227358 in / 
# Wed, 06 Dec 2023 19:42:27 GMT
CMD ["/bin/bash"]
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV GOSU_VERSION=1.16
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME" # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_MAJOR=innovation
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_VERSION=8.2.0-1.el8
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eu; 	{ 		echo '[mysqlinnovation-server-minimal]'; 		echo 'name=MySQL innovation Server Minimal'; 		echo 'enabled=1'; 		echo 'baseurl=https://repo.mysql.com/yum/mysql-innovation-community/docker/el/8/$basearch/'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eu; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo 'baseurl=https://repo.mysql.com/yum/mysql-tools-innovation-community/el/8/$basearch/'; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_SHELL_VERSION=8.2.1-1.el8
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
VOLUME [/var/lib/mysql]
# Mon, 18 Dec 2023 23:06:09 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 18 Dec 2023 23:06:09 GMT
EXPOSE map[3306/tcp:{} 33060/tcp:{}]
# Mon, 18 Dec 2023 23:06:09 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:edfaa6c9daada52a737333e0818f3d697d745aab3f3351e773218a524ebc9e53`  
		Last Modified: Wed, 06 Dec 2023 19:43:23 GMT  
		Size: 50.1 MB (50072545 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:19c686b91aca61da8058a44e9f6aa06cbb27aa65cf2db0768377bcc6899dc0c2`  
		Last Modified: Thu, 14 Dec 2023 20:15:05 GMT  
		Size: 885.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8c39062282e36f6169d219352cb19810ac7506e408e89b4ef33c400903a6ecc1`  
		Last Modified: Thu, 14 Dec 2023 20:15:05 GMT  
		Size: 913.0 KB (912965 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:73452dd561ff872804f5a63faab7552647c80c8a399e834fe154707a48613b20`  
		Last Modified: Thu, 14 Dec 2023 20:15:05 GMT  
		Size: 4.3 MB (4300794 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0ba54e261f50c32496de78ff38c42eb03cb97850ddbeb3c96f4fe34ea1cb23bc`  
		Last Modified: Thu, 14 Dec 2023 20:15:05 GMT  
		Size: 2.6 KB (2609 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b22c0fd6cce4772b17fe2500d6ce97e3a35076112226cc23269afa1542f7b51d`  
		Last Modified: Thu, 14 Dec 2023 20:15:06 GMT  
		Size: 340.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:eaffd91cbb1278d374c5b91f8a3e87239e73b0113a1fa5835faf13bcb05948dc`  
		Last Modified: Thu, 14 Dec 2023 20:15:09 GMT  
		Size: 61.6 MB (61602995 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3ec60922d8e9eefbce5167faf6f2296ddec22dcafc9a84f5db6f94e92e032089`  
		Last Modified: Thu, 14 Dec 2023 20:15:07 GMT  
		Size: 325.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:942dbd5bb0a98d45556f650aa3174e3e4a5fcf822e5e7a67529ae622bb02b14a`  
		Last Modified: Thu, 14 Dec 2023 20:15:09 GMT  
		Size: 68.4 MB (68377279 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bc7ea546f5793dcfecf365aefc956d7999a086211dc195cbb5d73d09df397fe2`  
		Last Modified: Tue, 19 Dec 2023 21:07:09 GMT  
		Size: 5.2 KB (5179 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:8.2-oraclelinux8` - unknown; unknown

```console
$ docker pull mysql@sha256:9b1966fea33a8f487098b70ebc30c23b2700a8731bcff2bd124779ba2f8cf2be
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.6 MB (11606464 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:557704055f52c52ae3fcc218fa7168216870eca8326c1b1e89d434ad3ec00204`

```dockerfile
```

-	Layers:
	-	`sha256:0b211226c249aefed58e7da4b41bb3219beb5345fe5ed4e65c65ab47e378292b`  
		Last Modified: Tue, 19 Dec 2023 21:07:09 GMT  
		Size: 11.6 MB (11571692 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:097024790a6d6019cd411ce0478476fbfebc733402110550a33d6009f3aca07d`  
		Last Modified: Tue, 19 Dec 2023 21:07:09 GMT  
		Size: 34.8 KB (34772 bytes)  
		MIME: application/vnd.in-toto+json

## `mysql:8.2.0`

```console
$ docker pull mysql@sha256:2d82ba6960cdf254de13f57d7265570c0675bc8bae1051e4a9806cff863006c9
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `mysql:8.2.0` - linux; amd64

```console
$ docker pull mysql@sha256:28a16e31b140d750048cd5fadcaed22ac08d0eeb18567f79f822aee1f237b43c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **181.6 MB (181572393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73246731c4b01c19b8713c6408c6c5d898ac04f75f2a4ce998930f12091542f2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 18 Dec 2023 23:06:09 GMT
ADD file:da89b67e484bc45f357250a868fd78e28086b13e4315635d19648e5d43812e89 in / 
# Mon, 18 Dec 2023 23:06:09 GMT
CMD ["/bin/bash"]
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV GOSU_VERSION=1.16
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME" # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_MAJOR=innovation
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_VERSION=8.2.0-1.el8
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eu; 	{ 		echo '[mysqlinnovation-server-minimal]'; 		echo 'name=MySQL innovation Server Minimal'; 		echo 'enabled=1'; 		echo 'baseurl=https://repo.mysql.com/yum/mysql-innovation-community/docker/el/8/$basearch/'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eu; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo 'baseurl=https://repo.mysql.com/yum/mysql-tools-innovation-community/el/8/$basearch/'; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_SHELL_VERSION=8.2.1-1.el8
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
VOLUME [/var/lib/mysql]
# Mon, 18 Dec 2023 23:06:09 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 18 Dec 2023 23:06:09 GMT
EXPOSE map[3306/tcp:{} 33060/tcp:{}]
# Mon, 18 Dec 2023 23:06:09 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:bce031bc522d421fb188ef82a530f85c5477bb87cdeacdb911ea86f3f7cd3b66`  
		Last Modified: Wed, 20 Dec 2023 22:42:00 GMT  
		Size: 51.3 MB (51323468 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cf7e9f463619cbda1168fb597e71ce50b4ecd4546ad74050f5b5c67a152ca249`  
		Last Modified: Thu, 21 Dec 2023 00:41:48 GMT  
		Size: 883.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:105f403783c74e137d330ef98facdded2cab753187765ed8c453bb7b061a0002`  
		Last Modified: Thu, 21 Dec 2023 00:41:48 GMT  
		Size: 982.8 KB (982809 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:878e53a613d8011ad3d6207863d1555fe571430d3c6f7659d1eb0fd7f28ba7de`  
		Last Modified: Thu, 21 Dec 2023 00:41:48 GMT  
		Size: 4.6 MB (4594819 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2a362044e79fb6669726216e996a0a9fa018ba304d75ac30c9378a93160182de`  
		Last Modified: Thu, 21 Dec 2023 00:41:48 GMT  
		Size: 2.6 KB (2608 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6e4df4f73cfe883156b974e5269c673e52de0e1a56d610f2974793cd52d8b043`  
		Last Modified: Thu, 21 Dec 2023 00:41:49 GMT  
		Size: 340.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:69263d6347550e51a3b3f972d5aee303fd3c8c6d75376aad0b4cdcd4cb3f83be`  
		Last Modified: Thu, 21 Dec 2023 00:41:49 GMT  
		Size: 62.6 MB (62574253 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fe5e855492024c60c48d8eb006c94b71d6622f6d5c741cfa611e571a88a67d37`  
		Last Modified: Thu, 21 Dec 2023 00:41:49 GMT  
		Size: 325.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5c02229ce6f164ee6c47c91ddaa42db249b197b8b28dc6814a4df879a4f96a3e`  
		Last Modified: Thu, 21 Dec 2023 00:41:50 GMT  
		Size: 62.1 MB (62087711 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7320aa32bf42c0642bc86e30dac0b10335258a24b6ba374e173918ba8d9f9f63`  
		Last Modified: Thu, 21 Dec 2023 00:41:49 GMT  
		Size: 5.2 KB (5177 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:8.2.0` - unknown; unknown

```console
$ docker pull mysql@sha256:483bf8eb111365bf322a25443d3f96ae0d80829c60f00fb329d8a0de0f21c6e7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.6 MB (11608021 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:501f9b1df36151d7e7ebba69fac20d69995d956d3851313ac3b4fdf9fa4e9ad3`

```dockerfile
```

-	Layers:
	-	`sha256:8de9290b82bb48a07e68ea96148c288ffa09729055d5c506b7690cf42f948baf`  
		Last Modified: Thu, 21 Dec 2023 00:41:48 GMT  
		Size: 11.6 MB (11573114 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:0b8a63c307592189c7a4ea188ee3b5e76eba99edc475a34c635157d5e893e536`  
		Last Modified: Thu, 21 Dec 2023 00:41:48 GMT  
		Size: 34.9 KB (34907 bytes)  
		MIME: application/vnd.in-toto+json

### `mysql:8.2.0` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:86f5987d89514a0ec8043202ba341717c6d2f726749924ef7f220839ac576cf8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **185.3 MB (185275916 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e963a4c2b1a0d8774a4b6138a86d2bcca8b8f5cec58fbfabf7ae4ae021159e0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 06 Dec 2023 19:42:27 GMT
ADD file:f5ee75151bd25b33e72aa4c0560815f35f6e662876bf3733a02e5cb970227358 in / 
# Wed, 06 Dec 2023 19:42:27 GMT
CMD ["/bin/bash"]
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV GOSU_VERSION=1.16
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME" # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_MAJOR=innovation
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_VERSION=8.2.0-1.el8
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eu; 	{ 		echo '[mysqlinnovation-server-minimal]'; 		echo 'name=MySQL innovation Server Minimal'; 		echo 'enabled=1'; 		echo 'baseurl=https://repo.mysql.com/yum/mysql-innovation-community/docker/el/8/$basearch/'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eu; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo 'baseurl=https://repo.mysql.com/yum/mysql-tools-innovation-community/el/8/$basearch/'; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_SHELL_VERSION=8.2.1-1.el8
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
VOLUME [/var/lib/mysql]
# Mon, 18 Dec 2023 23:06:09 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 18 Dec 2023 23:06:09 GMT
EXPOSE map[3306/tcp:{} 33060/tcp:{}]
# Mon, 18 Dec 2023 23:06:09 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:edfaa6c9daada52a737333e0818f3d697d745aab3f3351e773218a524ebc9e53`  
		Last Modified: Wed, 06 Dec 2023 19:43:23 GMT  
		Size: 50.1 MB (50072545 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:19c686b91aca61da8058a44e9f6aa06cbb27aa65cf2db0768377bcc6899dc0c2`  
		Last Modified: Thu, 14 Dec 2023 20:15:05 GMT  
		Size: 885.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8c39062282e36f6169d219352cb19810ac7506e408e89b4ef33c400903a6ecc1`  
		Last Modified: Thu, 14 Dec 2023 20:15:05 GMT  
		Size: 913.0 KB (912965 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:73452dd561ff872804f5a63faab7552647c80c8a399e834fe154707a48613b20`  
		Last Modified: Thu, 14 Dec 2023 20:15:05 GMT  
		Size: 4.3 MB (4300794 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0ba54e261f50c32496de78ff38c42eb03cb97850ddbeb3c96f4fe34ea1cb23bc`  
		Last Modified: Thu, 14 Dec 2023 20:15:05 GMT  
		Size: 2.6 KB (2609 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b22c0fd6cce4772b17fe2500d6ce97e3a35076112226cc23269afa1542f7b51d`  
		Last Modified: Thu, 14 Dec 2023 20:15:06 GMT  
		Size: 340.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:eaffd91cbb1278d374c5b91f8a3e87239e73b0113a1fa5835faf13bcb05948dc`  
		Last Modified: Thu, 14 Dec 2023 20:15:09 GMT  
		Size: 61.6 MB (61602995 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3ec60922d8e9eefbce5167faf6f2296ddec22dcafc9a84f5db6f94e92e032089`  
		Last Modified: Thu, 14 Dec 2023 20:15:07 GMT  
		Size: 325.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:942dbd5bb0a98d45556f650aa3174e3e4a5fcf822e5e7a67529ae622bb02b14a`  
		Last Modified: Thu, 14 Dec 2023 20:15:09 GMT  
		Size: 68.4 MB (68377279 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bc7ea546f5793dcfecf365aefc956d7999a086211dc195cbb5d73d09df397fe2`  
		Last Modified: Tue, 19 Dec 2023 21:07:09 GMT  
		Size: 5.2 KB (5179 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:8.2.0` - unknown; unknown

```console
$ docker pull mysql@sha256:9b1966fea33a8f487098b70ebc30c23b2700a8731bcff2bd124779ba2f8cf2be
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.6 MB (11606464 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:557704055f52c52ae3fcc218fa7168216870eca8326c1b1e89d434ad3ec00204`

```dockerfile
```

-	Layers:
	-	`sha256:0b211226c249aefed58e7da4b41bb3219beb5345fe5ed4e65c65ab47e378292b`  
		Last Modified: Tue, 19 Dec 2023 21:07:09 GMT  
		Size: 11.6 MB (11571692 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:097024790a6d6019cd411ce0478476fbfebc733402110550a33d6009f3aca07d`  
		Last Modified: Tue, 19 Dec 2023 21:07:09 GMT  
		Size: 34.8 KB (34772 bytes)  
		MIME: application/vnd.in-toto+json

## `mysql:8.2.0-oracle`

```console
$ docker pull mysql@sha256:2d82ba6960cdf254de13f57d7265570c0675bc8bae1051e4a9806cff863006c9
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `mysql:8.2.0-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:28a16e31b140d750048cd5fadcaed22ac08d0eeb18567f79f822aee1f237b43c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **181.6 MB (181572393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73246731c4b01c19b8713c6408c6c5d898ac04f75f2a4ce998930f12091542f2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 18 Dec 2023 23:06:09 GMT
ADD file:da89b67e484bc45f357250a868fd78e28086b13e4315635d19648e5d43812e89 in / 
# Mon, 18 Dec 2023 23:06:09 GMT
CMD ["/bin/bash"]
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV GOSU_VERSION=1.16
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME" # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_MAJOR=innovation
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_VERSION=8.2.0-1.el8
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eu; 	{ 		echo '[mysqlinnovation-server-minimal]'; 		echo 'name=MySQL innovation Server Minimal'; 		echo 'enabled=1'; 		echo 'baseurl=https://repo.mysql.com/yum/mysql-innovation-community/docker/el/8/$basearch/'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eu; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo 'baseurl=https://repo.mysql.com/yum/mysql-tools-innovation-community/el/8/$basearch/'; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_SHELL_VERSION=8.2.1-1.el8
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
VOLUME [/var/lib/mysql]
# Mon, 18 Dec 2023 23:06:09 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 18 Dec 2023 23:06:09 GMT
EXPOSE map[3306/tcp:{} 33060/tcp:{}]
# Mon, 18 Dec 2023 23:06:09 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:bce031bc522d421fb188ef82a530f85c5477bb87cdeacdb911ea86f3f7cd3b66`  
		Last Modified: Wed, 20 Dec 2023 22:42:00 GMT  
		Size: 51.3 MB (51323468 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cf7e9f463619cbda1168fb597e71ce50b4ecd4546ad74050f5b5c67a152ca249`  
		Last Modified: Thu, 21 Dec 2023 00:41:48 GMT  
		Size: 883.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:105f403783c74e137d330ef98facdded2cab753187765ed8c453bb7b061a0002`  
		Last Modified: Thu, 21 Dec 2023 00:41:48 GMT  
		Size: 982.8 KB (982809 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:878e53a613d8011ad3d6207863d1555fe571430d3c6f7659d1eb0fd7f28ba7de`  
		Last Modified: Thu, 21 Dec 2023 00:41:48 GMT  
		Size: 4.6 MB (4594819 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2a362044e79fb6669726216e996a0a9fa018ba304d75ac30c9378a93160182de`  
		Last Modified: Thu, 21 Dec 2023 00:41:48 GMT  
		Size: 2.6 KB (2608 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6e4df4f73cfe883156b974e5269c673e52de0e1a56d610f2974793cd52d8b043`  
		Last Modified: Thu, 21 Dec 2023 00:41:49 GMT  
		Size: 340.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:69263d6347550e51a3b3f972d5aee303fd3c8c6d75376aad0b4cdcd4cb3f83be`  
		Last Modified: Thu, 21 Dec 2023 00:41:49 GMT  
		Size: 62.6 MB (62574253 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fe5e855492024c60c48d8eb006c94b71d6622f6d5c741cfa611e571a88a67d37`  
		Last Modified: Thu, 21 Dec 2023 00:41:49 GMT  
		Size: 325.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5c02229ce6f164ee6c47c91ddaa42db249b197b8b28dc6814a4df879a4f96a3e`  
		Last Modified: Thu, 21 Dec 2023 00:41:50 GMT  
		Size: 62.1 MB (62087711 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7320aa32bf42c0642bc86e30dac0b10335258a24b6ba374e173918ba8d9f9f63`  
		Last Modified: Thu, 21 Dec 2023 00:41:49 GMT  
		Size: 5.2 KB (5177 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:8.2.0-oracle` - unknown; unknown

```console
$ docker pull mysql@sha256:483bf8eb111365bf322a25443d3f96ae0d80829c60f00fb329d8a0de0f21c6e7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.6 MB (11608021 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:501f9b1df36151d7e7ebba69fac20d69995d956d3851313ac3b4fdf9fa4e9ad3`

```dockerfile
```

-	Layers:
	-	`sha256:8de9290b82bb48a07e68ea96148c288ffa09729055d5c506b7690cf42f948baf`  
		Last Modified: Thu, 21 Dec 2023 00:41:48 GMT  
		Size: 11.6 MB (11573114 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:0b8a63c307592189c7a4ea188ee3b5e76eba99edc475a34c635157d5e893e536`  
		Last Modified: Thu, 21 Dec 2023 00:41:48 GMT  
		Size: 34.9 KB (34907 bytes)  
		MIME: application/vnd.in-toto+json

### `mysql:8.2.0-oracle` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:86f5987d89514a0ec8043202ba341717c6d2f726749924ef7f220839ac576cf8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **185.3 MB (185275916 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e963a4c2b1a0d8774a4b6138a86d2bcca8b8f5cec58fbfabf7ae4ae021159e0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 06 Dec 2023 19:42:27 GMT
ADD file:f5ee75151bd25b33e72aa4c0560815f35f6e662876bf3733a02e5cb970227358 in / 
# Wed, 06 Dec 2023 19:42:27 GMT
CMD ["/bin/bash"]
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV GOSU_VERSION=1.16
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME" # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_MAJOR=innovation
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_VERSION=8.2.0-1.el8
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eu; 	{ 		echo '[mysqlinnovation-server-minimal]'; 		echo 'name=MySQL innovation Server Minimal'; 		echo 'enabled=1'; 		echo 'baseurl=https://repo.mysql.com/yum/mysql-innovation-community/docker/el/8/$basearch/'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eu; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo 'baseurl=https://repo.mysql.com/yum/mysql-tools-innovation-community/el/8/$basearch/'; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_SHELL_VERSION=8.2.1-1.el8
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
VOLUME [/var/lib/mysql]
# Mon, 18 Dec 2023 23:06:09 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 18 Dec 2023 23:06:09 GMT
EXPOSE map[3306/tcp:{} 33060/tcp:{}]
# Mon, 18 Dec 2023 23:06:09 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:edfaa6c9daada52a737333e0818f3d697d745aab3f3351e773218a524ebc9e53`  
		Last Modified: Wed, 06 Dec 2023 19:43:23 GMT  
		Size: 50.1 MB (50072545 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:19c686b91aca61da8058a44e9f6aa06cbb27aa65cf2db0768377bcc6899dc0c2`  
		Last Modified: Thu, 14 Dec 2023 20:15:05 GMT  
		Size: 885.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8c39062282e36f6169d219352cb19810ac7506e408e89b4ef33c400903a6ecc1`  
		Last Modified: Thu, 14 Dec 2023 20:15:05 GMT  
		Size: 913.0 KB (912965 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:73452dd561ff872804f5a63faab7552647c80c8a399e834fe154707a48613b20`  
		Last Modified: Thu, 14 Dec 2023 20:15:05 GMT  
		Size: 4.3 MB (4300794 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0ba54e261f50c32496de78ff38c42eb03cb97850ddbeb3c96f4fe34ea1cb23bc`  
		Last Modified: Thu, 14 Dec 2023 20:15:05 GMT  
		Size: 2.6 KB (2609 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b22c0fd6cce4772b17fe2500d6ce97e3a35076112226cc23269afa1542f7b51d`  
		Last Modified: Thu, 14 Dec 2023 20:15:06 GMT  
		Size: 340.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:eaffd91cbb1278d374c5b91f8a3e87239e73b0113a1fa5835faf13bcb05948dc`  
		Last Modified: Thu, 14 Dec 2023 20:15:09 GMT  
		Size: 61.6 MB (61602995 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3ec60922d8e9eefbce5167faf6f2296ddec22dcafc9a84f5db6f94e92e032089`  
		Last Modified: Thu, 14 Dec 2023 20:15:07 GMT  
		Size: 325.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:942dbd5bb0a98d45556f650aa3174e3e4a5fcf822e5e7a67529ae622bb02b14a`  
		Last Modified: Thu, 14 Dec 2023 20:15:09 GMT  
		Size: 68.4 MB (68377279 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bc7ea546f5793dcfecf365aefc956d7999a086211dc195cbb5d73d09df397fe2`  
		Last Modified: Tue, 19 Dec 2023 21:07:09 GMT  
		Size: 5.2 KB (5179 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:8.2.0-oracle` - unknown; unknown

```console
$ docker pull mysql@sha256:9b1966fea33a8f487098b70ebc30c23b2700a8731bcff2bd124779ba2f8cf2be
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.6 MB (11606464 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:557704055f52c52ae3fcc218fa7168216870eca8326c1b1e89d434ad3ec00204`

```dockerfile
```

-	Layers:
	-	`sha256:0b211226c249aefed58e7da4b41bb3219beb5345fe5ed4e65c65ab47e378292b`  
		Last Modified: Tue, 19 Dec 2023 21:07:09 GMT  
		Size: 11.6 MB (11571692 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:097024790a6d6019cd411ce0478476fbfebc733402110550a33d6009f3aca07d`  
		Last Modified: Tue, 19 Dec 2023 21:07:09 GMT  
		Size: 34.8 KB (34772 bytes)  
		MIME: application/vnd.in-toto+json

## `mysql:8.2.0-oraclelinux8`

```console
$ docker pull mysql@sha256:2d82ba6960cdf254de13f57d7265570c0675bc8bae1051e4a9806cff863006c9
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `mysql:8.2.0-oraclelinux8` - linux; amd64

```console
$ docker pull mysql@sha256:28a16e31b140d750048cd5fadcaed22ac08d0eeb18567f79f822aee1f237b43c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **181.6 MB (181572393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73246731c4b01c19b8713c6408c6c5d898ac04f75f2a4ce998930f12091542f2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 18 Dec 2023 23:06:09 GMT
ADD file:da89b67e484bc45f357250a868fd78e28086b13e4315635d19648e5d43812e89 in / 
# Mon, 18 Dec 2023 23:06:09 GMT
CMD ["/bin/bash"]
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV GOSU_VERSION=1.16
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME" # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_MAJOR=innovation
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_VERSION=8.2.0-1.el8
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eu; 	{ 		echo '[mysqlinnovation-server-minimal]'; 		echo 'name=MySQL innovation Server Minimal'; 		echo 'enabled=1'; 		echo 'baseurl=https://repo.mysql.com/yum/mysql-innovation-community/docker/el/8/$basearch/'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eu; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo 'baseurl=https://repo.mysql.com/yum/mysql-tools-innovation-community/el/8/$basearch/'; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_SHELL_VERSION=8.2.1-1.el8
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
VOLUME [/var/lib/mysql]
# Mon, 18 Dec 2023 23:06:09 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 18 Dec 2023 23:06:09 GMT
EXPOSE map[3306/tcp:{} 33060/tcp:{}]
# Mon, 18 Dec 2023 23:06:09 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:bce031bc522d421fb188ef82a530f85c5477bb87cdeacdb911ea86f3f7cd3b66`  
		Last Modified: Wed, 20 Dec 2023 22:42:00 GMT  
		Size: 51.3 MB (51323468 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cf7e9f463619cbda1168fb597e71ce50b4ecd4546ad74050f5b5c67a152ca249`  
		Last Modified: Thu, 21 Dec 2023 00:41:48 GMT  
		Size: 883.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:105f403783c74e137d330ef98facdded2cab753187765ed8c453bb7b061a0002`  
		Last Modified: Thu, 21 Dec 2023 00:41:48 GMT  
		Size: 982.8 KB (982809 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:878e53a613d8011ad3d6207863d1555fe571430d3c6f7659d1eb0fd7f28ba7de`  
		Last Modified: Thu, 21 Dec 2023 00:41:48 GMT  
		Size: 4.6 MB (4594819 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2a362044e79fb6669726216e996a0a9fa018ba304d75ac30c9378a93160182de`  
		Last Modified: Thu, 21 Dec 2023 00:41:48 GMT  
		Size: 2.6 KB (2608 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6e4df4f73cfe883156b974e5269c673e52de0e1a56d610f2974793cd52d8b043`  
		Last Modified: Thu, 21 Dec 2023 00:41:49 GMT  
		Size: 340.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:69263d6347550e51a3b3f972d5aee303fd3c8c6d75376aad0b4cdcd4cb3f83be`  
		Last Modified: Thu, 21 Dec 2023 00:41:49 GMT  
		Size: 62.6 MB (62574253 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fe5e855492024c60c48d8eb006c94b71d6622f6d5c741cfa611e571a88a67d37`  
		Last Modified: Thu, 21 Dec 2023 00:41:49 GMT  
		Size: 325.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5c02229ce6f164ee6c47c91ddaa42db249b197b8b28dc6814a4df879a4f96a3e`  
		Last Modified: Thu, 21 Dec 2023 00:41:50 GMT  
		Size: 62.1 MB (62087711 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7320aa32bf42c0642bc86e30dac0b10335258a24b6ba374e173918ba8d9f9f63`  
		Last Modified: Thu, 21 Dec 2023 00:41:49 GMT  
		Size: 5.2 KB (5177 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:8.2.0-oraclelinux8` - unknown; unknown

```console
$ docker pull mysql@sha256:483bf8eb111365bf322a25443d3f96ae0d80829c60f00fb329d8a0de0f21c6e7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.6 MB (11608021 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:501f9b1df36151d7e7ebba69fac20d69995d956d3851313ac3b4fdf9fa4e9ad3`

```dockerfile
```

-	Layers:
	-	`sha256:8de9290b82bb48a07e68ea96148c288ffa09729055d5c506b7690cf42f948baf`  
		Last Modified: Thu, 21 Dec 2023 00:41:48 GMT  
		Size: 11.6 MB (11573114 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:0b8a63c307592189c7a4ea188ee3b5e76eba99edc475a34c635157d5e893e536`  
		Last Modified: Thu, 21 Dec 2023 00:41:48 GMT  
		Size: 34.9 KB (34907 bytes)  
		MIME: application/vnd.in-toto+json

### `mysql:8.2.0-oraclelinux8` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:86f5987d89514a0ec8043202ba341717c6d2f726749924ef7f220839ac576cf8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **185.3 MB (185275916 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e963a4c2b1a0d8774a4b6138a86d2bcca8b8f5cec58fbfabf7ae4ae021159e0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 06 Dec 2023 19:42:27 GMT
ADD file:f5ee75151bd25b33e72aa4c0560815f35f6e662876bf3733a02e5cb970227358 in / 
# Wed, 06 Dec 2023 19:42:27 GMT
CMD ["/bin/bash"]
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV GOSU_VERSION=1.16
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME" # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_MAJOR=innovation
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_VERSION=8.2.0-1.el8
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eu; 	{ 		echo '[mysqlinnovation-server-minimal]'; 		echo 'name=MySQL innovation Server Minimal'; 		echo 'enabled=1'; 		echo 'baseurl=https://repo.mysql.com/yum/mysql-innovation-community/docker/el/8/$basearch/'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eu; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo 'baseurl=https://repo.mysql.com/yum/mysql-tools-innovation-community/el/8/$basearch/'; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_SHELL_VERSION=8.2.1-1.el8
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
VOLUME [/var/lib/mysql]
# Mon, 18 Dec 2023 23:06:09 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 18 Dec 2023 23:06:09 GMT
EXPOSE map[3306/tcp:{} 33060/tcp:{}]
# Mon, 18 Dec 2023 23:06:09 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:edfaa6c9daada52a737333e0818f3d697d745aab3f3351e773218a524ebc9e53`  
		Last Modified: Wed, 06 Dec 2023 19:43:23 GMT  
		Size: 50.1 MB (50072545 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:19c686b91aca61da8058a44e9f6aa06cbb27aa65cf2db0768377bcc6899dc0c2`  
		Last Modified: Thu, 14 Dec 2023 20:15:05 GMT  
		Size: 885.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8c39062282e36f6169d219352cb19810ac7506e408e89b4ef33c400903a6ecc1`  
		Last Modified: Thu, 14 Dec 2023 20:15:05 GMT  
		Size: 913.0 KB (912965 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:73452dd561ff872804f5a63faab7552647c80c8a399e834fe154707a48613b20`  
		Last Modified: Thu, 14 Dec 2023 20:15:05 GMT  
		Size: 4.3 MB (4300794 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0ba54e261f50c32496de78ff38c42eb03cb97850ddbeb3c96f4fe34ea1cb23bc`  
		Last Modified: Thu, 14 Dec 2023 20:15:05 GMT  
		Size: 2.6 KB (2609 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b22c0fd6cce4772b17fe2500d6ce97e3a35076112226cc23269afa1542f7b51d`  
		Last Modified: Thu, 14 Dec 2023 20:15:06 GMT  
		Size: 340.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:eaffd91cbb1278d374c5b91f8a3e87239e73b0113a1fa5835faf13bcb05948dc`  
		Last Modified: Thu, 14 Dec 2023 20:15:09 GMT  
		Size: 61.6 MB (61602995 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3ec60922d8e9eefbce5167faf6f2296ddec22dcafc9a84f5db6f94e92e032089`  
		Last Modified: Thu, 14 Dec 2023 20:15:07 GMT  
		Size: 325.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:942dbd5bb0a98d45556f650aa3174e3e4a5fcf822e5e7a67529ae622bb02b14a`  
		Last Modified: Thu, 14 Dec 2023 20:15:09 GMT  
		Size: 68.4 MB (68377279 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bc7ea546f5793dcfecf365aefc956d7999a086211dc195cbb5d73d09df397fe2`  
		Last Modified: Tue, 19 Dec 2023 21:07:09 GMT  
		Size: 5.2 KB (5179 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:8.2.0-oraclelinux8` - unknown; unknown

```console
$ docker pull mysql@sha256:9b1966fea33a8f487098b70ebc30c23b2700a8731bcff2bd124779ba2f8cf2be
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.6 MB (11606464 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:557704055f52c52ae3fcc218fa7168216870eca8326c1b1e89d434ad3ec00204`

```dockerfile
```

-	Layers:
	-	`sha256:0b211226c249aefed58e7da4b41bb3219beb5345fe5ed4e65c65ab47e378292b`  
		Last Modified: Tue, 19 Dec 2023 21:07:09 GMT  
		Size: 11.6 MB (11571692 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:097024790a6d6019cd411ce0478476fbfebc733402110550a33d6009f3aca07d`  
		Last Modified: Tue, 19 Dec 2023 21:07:09 GMT  
		Size: 34.8 KB (34772 bytes)  
		MIME: application/vnd.in-toto+json

## `mysql:innovation`

```console
$ docker pull mysql@sha256:2d82ba6960cdf254de13f57d7265570c0675bc8bae1051e4a9806cff863006c9
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `mysql:innovation` - linux; amd64

```console
$ docker pull mysql@sha256:28a16e31b140d750048cd5fadcaed22ac08d0eeb18567f79f822aee1f237b43c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **181.6 MB (181572393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73246731c4b01c19b8713c6408c6c5d898ac04f75f2a4ce998930f12091542f2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 18 Dec 2023 23:06:09 GMT
ADD file:da89b67e484bc45f357250a868fd78e28086b13e4315635d19648e5d43812e89 in / 
# Mon, 18 Dec 2023 23:06:09 GMT
CMD ["/bin/bash"]
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV GOSU_VERSION=1.16
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME" # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_MAJOR=innovation
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_VERSION=8.2.0-1.el8
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eu; 	{ 		echo '[mysqlinnovation-server-minimal]'; 		echo 'name=MySQL innovation Server Minimal'; 		echo 'enabled=1'; 		echo 'baseurl=https://repo.mysql.com/yum/mysql-innovation-community/docker/el/8/$basearch/'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eu; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo 'baseurl=https://repo.mysql.com/yum/mysql-tools-innovation-community/el/8/$basearch/'; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_SHELL_VERSION=8.2.1-1.el8
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
VOLUME [/var/lib/mysql]
# Mon, 18 Dec 2023 23:06:09 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 18 Dec 2023 23:06:09 GMT
EXPOSE map[3306/tcp:{} 33060/tcp:{}]
# Mon, 18 Dec 2023 23:06:09 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:bce031bc522d421fb188ef82a530f85c5477bb87cdeacdb911ea86f3f7cd3b66`  
		Last Modified: Wed, 20 Dec 2023 22:42:00 GMT  
		Size: 51.3 MB (51323468 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cf7e9f463619cbda1168fb597e71ce50b4ecd4546ad74050f5b5c67a152ca249`  
		Last Modified: Thu, 21 Dec 2023 00:41:48 GMT  
		Size: 883.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:105f403783c74e137d330ef98facdded2cab753187765ed8c453bb7b061a0002`  
		Last Modified: Thu, 21 Dec 2023 00:41:48 GMT  
		Size: 982.8 KB (982809 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:878e53a613d8011ad3d6207863d1555fe571430d3c6f7659d1eb0fd7f28ba7de`  
		Last Modified: Thu, 21 Dec 2023 00:41:48 GMT  
		Size: 4.6 MB (4594819 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2a362044e79fb6669726216e996a0a9fa018ba304d75ac30c9378a93160182de`  
		Last Modified: Thu, 21 Dec 2023 00:41:48 GMT  
		Size: 2.6 KB (2608 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6e4df4f73cfe883156b974e5269c673e52de0e1a56d610f2974793cd52d8b043`  
		Last Modified: Thu, 21 Dec 2023 00:41:49 GMT  
		Size: 340.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:69263d6347550e51a3b3f972d5aee303fd3c8c6d75376aad0b4cdcd4cb3f83be`  
		Last Modified: Thu, 21 Dec 2023 00:41:49 GMT  
		Size: 62.6 MB (62574253 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fe5e855492024c60c48d8eb006c94b71d6622f6d5c741cfa611e571a88a67d37`  
		Last Modified: Thu, 21 Dec 2023 00:41:49 GMT  
		Size: 325.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5c02229ce6f164ee6c47c91ddaa42db249b197b8b28dc6814a4df879a4f96a3e`  
		Last Modified: Thu, 21 Dec 2023 00:41:50 GMT  
		Size: 62.1 MB (62087711 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7320aa32bf42c0642bc86e30dac0b10335258a24b6ba374e173918ba8d9f9f63`  
		Last Modified: Thu, 21 Dec 2023 00:41:49 GMT  
		Size: 5.2 KB (5177 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:innovation` - unknown; unknown

```console
$ docker pull mysql@sha256:483bf8eb111365bf322a25443d3f96ae0d80829c60f00fb329d8a0de0f21c6e7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.6 MB (11608021 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:501f9b1df36151d7e7ebba69fac20d69995d956d3851313ac3b4fdf9fa4e9ad3`

```dockerfile
```

-	Layers:
	-	`sha256:8de9290b82bb48a07e68ea96148c288ffa09729055d5c506b7690cf42f948baf`  
		Last Modified: Thu, 21 Dec 2023 00:41:48 GMT  
		Size: 11.6 MB (11573114 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:0b8a63c307592189c7a4ea188ee3b5e76eba99edc475a34c635157d5e893e536`  
		Last Modified: Thu, 21 Dec 2023 00:41:48 GMT  
		Size: 34.9 KB (34907 bytes)  
		MIME: application/vnd.in-toto+json

### `mysql:innovation` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:86f5987d89514a0ec8043202ba341717c6d2f726749924ef7f220839ac576cf8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **185.3 MB (185275916 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e963a4c2b1a0d8774a4b6138a86d2bcca8b8f5cec58fbfabf7ae4ae021159e0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 06 Dec 2023 19:42:27 GMT
ADD file:f5ee75151bd25b33e72aa4c0560815f35f6e662876bf3733a02e5cb970227358 in / 
# Wed, 06 Dec 2023 19:42:27 GMT
CMD ["/bin/bash"]
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV GOSU_VERSION=1.16
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME" # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_MAJOR=innovation
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_VERSION=8.2.0-1.el8
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eu; 	{ 		echo '[mysqlinnovation-server-minimal]'; 		echo 'name=MySQL innovation Server Minimal'; 		echo 'enabled=1'; 		echo 'baseurl=https://repo.mysql.com/yum/mysql-innovation-community/docker/el/8/$basearch/'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eu; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo 'baseurl=https://repo.mysql.com/yum/mysql-tools-innovation-community/el/8/$basearch/'; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_SHELL_VERSION=8.2.1-1.el8
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
VOLUME [/var/lib/mysql]
# Mon, 18 Dec 2023 23:06:09 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 18 Dec 2023 23:06:09 GMT
EXPOSE map[3306/tcp:{} 33060/tcp:{}]
# Mon, 18 Dec 2023 23:06:09 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:edfaa6c9daada52a737333e0818f3d697d745aab3f3351e773218a524ebc9e53`  
		Last Modified: Wed, 06 Dec 2023 19:43:23 GMT  
		Size: 50.1 MB (50072545 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:19c686b91aca61da8058a44e9f6aa06cbb27aa65cf2db0768377bcc6899dc0c2`  
		Last Modified: Thu, 14 Dec 2023 20:15:05 GMT  
		Size: 885.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8c39062282e36f6169d219352cb19810ac7506e408e89b4ef33c400903a6ecc1`  
		Last Modified: Thu, 14 Dec 2023 20:15:05 GMT  
		Size: 913.0 KB (912965 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:73452dd561ff872804f5a63faab7552647c80c8a399e834fe154707a48613b20`  
		Last Modified: Thu, 14 Dec 2023 20:15:05 GMT  
		Size: 4.3 MB (4300794 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0ba54e261f50c32496de78ff38c42eb03cb97850ddbeb3c96f4fe34ea1cb23bc`  
		Last Modified: Thu, 14 Dec 2023 20:15:05 GMT  
		Size: 2.6 KB (2609 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b22c0fd6cce4772b17fe2500d6ce97e3a35076112226cc23269afa1542f7b51d`  
		Last Modified: Thu, 14 Dec 2023 20:15:06 GMT  
		Size: 340.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:eaffd91cbb1278d374c5b91f8a3e87239e73b0113a1fa5835faf13bcb05948dc`  
		Last Modified: Thu, 14 Dec 2023 20:15:09 GMT  
		Size: 61.6 MB (61602995 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3ec60922d8e9eefbce5167faf6f2296ddec22dcafc9a84f5db6f94e92e032089`  
		Last Modified: Thu, 14 Dec 2023 20:15:07 GMT  
		Size: 325.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:942dbd5bb0a98d45556f650aa3174e3e4a5fcf822e5e7a67529ae622bb02b14a`  
		Last Modified: Thu, 14 Dec 2023 20:15:09 GMT  
		Size: 68.4 MB (68377279 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bc7ea546f5793dcfecf365aefc956d7999a086211dc195cbb5d73d09df397fe2`  
		Last Modified: Tue, 19 Dec 2023 21:07:09 GMT  
		Size: 5.2 KB (5179 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:innovation` - unknown; unknown

```console
$ docker pull mysql@sha256:9b1966fea33a8f487098b70ebc30c23b2700a8731bcff2bd124779ba2f8cf2be
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.6 MB (11606464 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:557704055f52c52ae3fcc218fa7168216870eca8326c1b1e89d434ad3ec00204`

```dockerfile
```

-	Layers:
	-	`sha256:0b211226c249aefed58e7da4b41bb3219beb5345fe5ed4e65c65ab47e378292b`  
		Last Modified: Tue, 19 Dec 2023 21:07:09 GMT  
		Size: 11.6 MB (11571692 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:097024790a6d6019cd411ce0478476fbfebc733402110550a33d6009f3aca07d`  
		Last Modified: Tue, 19 Dec 2023 21:07:09 GMT  
		Size: 34.8 KB (34772 bytes)  
		MIME: application/vnd.in-toto+json

## `mysql:innovation-oracle`

```console
$ docker pull mysql@sha256:2d82ba6960cdf254de13f57d7265570c0675bc8bae1051e4a9806cff863006c9
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `mysql:innovation-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:28a16e31b140d750048cd5fadcaed22ac08d0eeb18567f79f822aee1f237b43c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **181.6 MB (181572393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73246731c4b01c19b8713c6408c6c5d898ac04f75f2a4ce998930f12091542f2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 18 Dec 2023 23:06:09 GMT
ADD file:da89b67e484bc45f357250a868fd78e28086b13e4315635d19648e5d43812e89 in / 
# Mon, 18 Dec 2023 23:06:09 GMT
CMD ["/bin/bash"]
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV GOSU_VERSION=1.16
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME" # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_MAJOR=innovation
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_VERSION=8.2.0-1.el8
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eu; 	{ 		echo '[mysqlinnovation-server-minimal]'; 		echo 'name=MySQL innovation Server Minimal'; 		echo 'enabled=1'; 		echo 'baseurl=https://repo.mysql.com/yum/mysql-innovation-community/docker/el/8/$basearch/'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eu; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo 'baseurl=https://repo.mysql.com/yum/mysql-tools-innovation-community/el/8/$basearch/'; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_SHELL_VERSION=8.2.1-1.el8
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
VOLUME [/var/lib/mysql]
# Mon, 18 Dec 2023 23:06:09 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 18 Dec 2023 23:06:09 GMT
EXPOSE map[3306/tcp:{} 33060/tcp:{}]
# Mon, 18 Dec 2023 23:06:09 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:bce031bc522d421fb188ef82a530f85c5477bb87cdeacdb911ea86f3f7cd3b66`  
		Last Modified: Wed, 20 Dec 2023 22:42:00 GMT  
		Size: 51.3 MB (51323468 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cf7e9f463619cbda1168fb597e71ce50b4ecd4546ad74050f5b5c67a152ca249`  
		Last Modified: Thu, 21 Dec 2023 00:41:48 GMT  
		Size: 883.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:105f403783c74e137d330ef98facdded2cab753187765ed8c453bb7b061a0002`  
		Last Modified: Thu, 21 Dec 2023 00:41:48 GMT  
		Size: 982.8 KB (982809 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:878e53a613d8011ad3d6207863d1555fe571430d3c6f7659d1eb0fd7f28ba7de`  
		Last Modified: Thu, 21 Dec 2023 00:41:48 GMT  
		Size: 4.6 MB (4594819 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2a362044e79fb6669726216e996a0a9fa018ba304d75ac30c9378a93160182de`  
		Last Modified: Thu, 21 Dec 2023 00:41:48 GMT  
		Size: 2.6 KB (2608 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6e4df4f73cfe883156b974e5269c673e52de0e1a56d610f2974793cd52d8b043`  
		Last Modified: Thu, 21 Dec 2023 00:41:49 GMT  
		Size: 340.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:69263d6347550e51a3b3f972d5aee303fd3c8c6d75376aad0b4cdcd4cb3f83be`  
		Last Modified: Thu, 21 Dec 2023 00:41:49 GMT  
		Size: 62.6 MB (62574253 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fe5e855492024c60c48d8eb006c94b71d6622f6d5c741cfa611e571a88a67d37`  
		Last Modified: Thu, 21 Dec 2023 00:41:49 GMT  
		Size: 325.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5c02229ce6f164ee6c47c91ddaa42db249b197b8b28dc6814a4df879a4f96a3e`  
		Last Modified: Thu, 21 Dec 2023 00:41:50 GMT  
		Size: 62.1 MB (62087711 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7320aa32bf42c0642bc86e30dac0b10335258a24b6ba374e173918ba8d9f9f63`  
		Last Modified: Thu, 21 Dec 2023 00:41:49 GMT  
		Size: 5.2 KB (5177 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:innovation-oracle` - unknown; unknown

```console
$ docker pull mysql@sha256:483bf8eb111365bf322a25443d3f96ae0d80829c60f00fb329d8a0de0f21c6e7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.6 MB (11608021 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:501f9b1df36151d7e7ebba69fac20d69995d956d3851313ac3b4fdf9fa4e9ad3`

```dockerfile
```

-	Layers:
	-	`sha256:8de9290b82bb48a07e68ea96148c288ffa09729055d5c506b7690cf42f948baf`  
		Last Modified: Thu, 21 Dec 2023 00:41:48 GMT  
		Size: 11.6 MB (11573114 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:0b8a63c307592189c7a4ea188ee3b5e76eba99edc475a34c635157d5e893e536`  
		Last Modified: Thu, 21 Dec 2023 00:41:48 GMT  
		Size: 34.9 KB (34907 bytes)  
		MIME: application/vnd.in-toto+json

### `mysql:innovation-oracle` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:86f5987d89514a0ec8043202ba341717c6d2f726749924ef7f220839ac576cf8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **185.3 MB (185275916 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e963a4c2b1a0d8774a4b6138a86d2bcca8b8f5cec58fbfabf7ae4ae021159e0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 06 Dec 2023 19:42:27 GMT
ADD file:f5ee75151bd25b33e72aa4c0560815f35f6e662876bf3733a02e5cb970227358 in / 
# Wed, 06 Dec 2023 19:42:27 GMT
CMD ["/bin/bash"]
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV GOSU_VERSION=1.16
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME" # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_MAJOR=innovation
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_VERSION=8.2.0-1.el8
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eu; 	{ 		echo '[mysqlinnovation-server-minimal]'; 		echo 'name=MySQL innovation Server Minimal'; 		echo 'enabled=1'; 		echo 'baseurl=https://repo.mysql.com/yum/mysql-innovation-community/docker/el/8/$basearch/'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eu; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo 'baseurl=https://repo.mysql.com/yum/mysql-tools-innovation-community/el/8/$basearch/'; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_SHELL_VERSION=8.2.1-1.el8
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
VOLUME [/var/lib/mysql]
# Mon, 18 Dec 2023 23:06:09 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 18 Dec 2023 23:06:09 GMT
EXPOSE map[3306/tcp:{} 33060/tcp:{}]
# Mon, 18 Dec 2023 23:06:09 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:edfaa6c9daada52a737333e0818f3d697d745aab3f3351e773218a524ebc9e53`  
		Last Modified: Wed, 06 Dec 2023 19:43:23 GMT  
		Size: 50.1 MB (50072545 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:19c686b91aca61da8058a44e9f6aa06cbb27aa65cf2db0768377bcc6899dc0c2`  
		Last Modified: Thu, 14 Dec 2023 20:15:05 GMT  
		Size: 885.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8c39062282e36f6169d219352cb19810ac7506e408e89b4ef33c400903a6ecc1`  
		Last Modified: Thu, 14 Dec 2023 20:15:05 GMT  
		Size: 913.0 KB (912965 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:73452dd561ff872804f5a63faab7552647c80c8a399e834fe154707a48613b20`  
		Last Modified: Thu, 14 Dec 2023 20:15:05 GMT  
		Size: 4.3 MB (4300794 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0ba54e261f50c32496de78ff38c42eb03cb97850ddbeb3c96f4fe34ea1cb23bc`  
		Last Modified: Thu, 14 Dec 2023 20:15:05 GMT  
		Size: 2.6 KB (2609 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b22c0fd6cce4772b17fe2500d6ce97e3a35076112226cc23269afa1542f7b51d`  
		Last Modified: Thu, 14 Dec 2023 20:15:06 GMT  
		Size: 340.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:eaffd91cbb1278d374c5b91f8a3e87239e73b0113a1fa5835faf13bcb05948dc`  
		Last Modified: Thu, 14 Dec 2023 20:15:09 GMT  
		Size: 61.6 MB (61602995 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3ec60922d8e9eefbce5167faf6f2296ddec22dcafc9a84f5db6f94e92e032089`  
		Last Modified: Thu, 14 Dec 2023 20:15:07 GMT  
		Size: 325.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:942dbd5bb0a98d45556f650aa3174e3e4a5fcf822e5e7a67529ae622bb02b14a`  
		Last Modified: Thu, 14 Dec 2023 20:15:09 GMT  
		Size: 68.4 MB (68377279 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bc7ea546f5793dcfecf365aefc956d7999a086211dc195cbb5d73d09df397fe2`  
		Last Modified: Tue, 19 Dec 2023 21:07:09 GMT  
		Size: 5.2 KB (5179 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:innovation-oracle` - unknown; unknown

```console
$ docker pull mysql@sha256:9b1966fea33a8f487098b70ebc30c23b2700a8731bcff2bd124779ba2f8cf2be
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.6 MB (11606464 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:557704055f52c52ae3fcc218fa7168216870eca8326c1b1e89d434ad3ec00204`

```dockerfile
```

-	Layers:
	-	`sha256:0b211226c249aefed58e7da4b41bb3219beb5345fe5ed4e65c65ab47e378292b`  
		Last Modified: Tue, 19 Dec 2023 21:07:09 GMT  
		Size: 11.6 MB (11571692 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:097024790a6d6019cd411ce0478476fbfebc733402110550a33d6009f3aca07d`  
		Last Modified: Tue, 19 Dec 2023 21:07:09 GMT  
		Size: 34.8 KB (34772 bytes)  
		MIME: application/vnd.in-toto+json

## `mysql:innovation-oraclelinux8`

```console
$ docker pull mysql@sha256:2d82ba6960cdf254de13f57d7265570c0675bc8bae1051e4a9806cff863006c9
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `mysql:innovation-oraclelinux8` - linux; amd64

```console
$ docker pull mysql@sha256:28a16e31b140d750048cd5fadcaed22ac08d0eeb18567f79f822aee1f237b43c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **181.6 MB (181572393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73246731c4b01c19b8713c6408c6c5d898ac04f75f2a4ce998930f12091542f2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 18 Dec 2023 23:06:09 GMT
ADD file:da89b67e484bc45f357250a868fd78e28086b13e4315635d19648e5d43812e89 in / 
# Mon, 18 Dec 2023 23:06:09 GMT
CMD ["/bin/bash"]
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV GOSU_VERSION=1.16
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME" # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_MAJOR=innovation
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_VERSION=8.2.0-1.el8
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eu; 	{ 		echo '[mysqlinnovation-server-minimal]'; 		echo 'name=MySQL innovation Server Minimal'; 		echo 'enabled=1'; 		echo 'baseurl=https://repo.mysql.com/yum/mysql-innovation-community/docker/el/8/$basearch/'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eu; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo 'baseurl=https://repo.mysql.com/yum/mysql-tools-innovation-community/el/8/$basearch/'; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_SHELL_VERSION=8.2.1-1.el8
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
VOLUME [/var/lib/mysql]
# Mon, 18 Dec 2023 23:06:09 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 18 Dec 2023 23:06:09 GMT
EXPOSE map[3306/tcp:{} 33060/tcp:{}]
# Mon, 18 Dec 2023 23:06:09 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:bce031bc522d421fb188ef82a530f85c5477bb87cdeacdb911ea86f3f7cd3b66`  
		Last Modified: Wed, 20 Dec 2023 22:42:00 GMT  
		Size: 51.3 MB (51323468 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cf7e9f463619cbda1168fb597e71ce50b4ecd4546ad74050f5b5c67a152ca249`  
		Last Modified: Thu, 21 Dec 2023 00:41:48 GMT  
		Size: 883.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:105f403783c74e137d330ef98facdded2cab753187765ed8c453bb7b061a0002`  
		Last Modified: Thu, 21 Dec 2023 00:41:48 GMT  
		Size: 982.8 KB (982809 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:878e53a613d8011ad3d6207863d1555fe571430d3c6f7659d1eb0fd7f28ba7de`  
		Last Modified: Thu, 21 Dec 2023 00:41:48 GMT  
		Size: 4.6 MB (4594819 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2a362044e79fb6669726216e996a0a9fa018ba304d75ac30c9378a93160182de`  
		Last Modified: Thu, 21 Dec 2023 00:41:48 GMT  
		Size: 2.6 KB (2608 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6e4df4f73cfe883156b974e5269c673e52de0e1a56d610f2974793cd52d8b043`  
		Last Modified: Thu, 21 Dec 2023 00:41:49 GMT  
		Size: 340.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:69263d6347550e51a3b3f972d5aee303fd3c8c6d75376aad0b4cdcd4cb3f83be`  
		Last Modified: Thu, 21 Dec 2023 00:41:49 GMT  
		Size: 62.6 MB (62574253 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fe5e855492024c60c48d8eb006c94b71d6622f6d5c741cfa611e571a88a67d37`  
		Last Modified: Thu, 21 Dec 2023 00:41:49 GMT  
		Size: 325.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5c02229ce6f164ee6c47c91ddaa42db249b197b8b28dc6814a4df879a4f96a3e`  
		Last Modified: Thu, 21 Dec 2023 00:41:50 GMT  
		Size: 62.1 MB (62087711 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7320aa32bf42c0642bc86e30dac0b10335258a24b6ba374e173918ba8d9f9f63`  
		Last Modified: Thu, 21 Dec 2023 00:41:49 GMT  
		Size: 5.2 KB (5177 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:innovation-oraclelinux8` - unknown; unknown

```console
$ docker pull mysql@sha256:483bf8eb111365bf322a25443d3f96ae0d80829c60f00fb329d8a0de0f21c6e7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.6 MB (11608021 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:501f9b1df36151d7e7ebba69fac20d69995d956d3851313ac3b4fdf9fa4e9ad3`

```dockerfile
```

-	Layers:
	-	`sha256:8de9290b82bb48a07e68ea96148c288ffa09729055d5c506b7690cf42f948baf`  
		Last Modified: Thu, 21 Dec 2023 00:41:48 GMT  
		Size: 11.6 MB (11573114 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:0b8a63c307592189c7a4ea188ee3b5e76eba99edc475a34c635157d5e893e536`  
		Last Modified: Thu, 21 Dec 2023 00:41:48 GMT  
		Size: 34.9 KB (34907 bytes)  
		MIME: application/vnd.in-toto+json

### `mysql:innovation-oraclelinux8` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:86f5987d89514a0ec8043202ba341717c6d2f726749924ef7f220839ac576cf8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **185.3 MB (185275916 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e963a4c2b1a0d8774a4b6138a86d2bcca8b8f5cec58fbfabf7ae4ae021159e0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 06 Dec 2023 19:42:27 GMT
ADD file:f5ee75151bd25b33e72aa4c0560815f35f6e662876bf3733a02e5cb970227358 in / 
# Wed, 06 Dec 2023 19:42:27 GMT
CMD ["/bin/bash"]
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV GOSU_VERSION=1.16
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME" # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_MAJOR=innovation
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_VERSION=8.2.0-1.el8
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eu; 	{ 		echo '[mysqlinnovation-server-minimal]'; 		echo 'name=MySQL innovation Server Minimal'; 		echo 'enabled=1'; 		echo 'baseurl=https://repo.mysql.com/yum/mysql-innovation-community/docker/el/8/$basearch/'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eu; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo 'baseurl=https://repo.mysql.com/yum/mysql-tools-innovation-community/el/8/$basearch/'; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_SHELL_VERSION=8.2.1-1.el8
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
VOLUME [/var/lib/mysql]
# Mon, 18 Dec 2023 23:06:09 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 18 Dec 2023 23:06:09 GMT
EXPOSE map[3306/tcp:{} 33060/tcp:{}]
# Mon, 18 Dec 2023 23:06:09 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:edfaa6c9daada52a737333e0818f3d697d745aab3f3351e773218a524ebc9e53`  
		Last Modified: Wed, 06 Dec 2023 19:43:23 GMT  
		Size: 50.1 MB (50072545 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:19c686b91aca61da8058a44e9f6aa06cbb27aa65cf2db0768377bcc6899dc0c2`  
		Last Modified: Thu, 14 Dec 2023 20:15:05 GMT  
		Size: 885.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8c39062282e36f6169d219352cb19810ac7506e408e89b4ef33c400903a6ecc1`  
		Last Modified: Thu, 14 Dec 2023 20:15:05 GMT  
		Size: 913.0 KB (912965 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:73452dd561ff872804f5a63faab7552647c80c8a399e834fe154707a48613b20`  
		Last Modified: Thu, 14 Dec 2023 20:15:05 GMT  
		Size: 4.3 MB (4300794 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0ba54e261f50c32496de78ff38c42eb03cb97850ddbeb3c96f4fe34ea1cb23bc`  
		Last Modified: Thu, 14 Dec 2023 20:15:05 GMT  
		Size: 2.6 KB (2609 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b22c0fd6cce4772b17fe2500d6ce97e3a35076112226cc23269afa1542f7b51d`  
		Last Modified: Thu, 14 Dec 2023 20:15:06 GMT  
		Size: 340.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:eaffd91cbb1278d374c5b91f8a3e87239e73b0113a1fa5835faf13bcb05948dc`  
		Last Modified: Thu, 14 Dec 2023 20:15:09 GMT  
		Size: 61.6 MB (61602995 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3ec60922d8e9eefbce5167faf6f2296ddec22dcafc9a84f5db6f94e92e032089`  
		Last Modified: Thu, 14 Dec 2023 20:15:07 GMT  
		Size: 325.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:942dbd5bb0a98d45556f650aa3174e3e4a5fcf822e5e7a67529ae622bb02b14a`  
		Last Modified: Thu, 14 Dec 2023 20:15:09 GMT  
		Size: 68.4 MB (68377279 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bc7ea546f5793dcfecf365aefc956d7999a086211dc195cbb5d73d09df397fe2`  
		Last Modified: Tue, 19 Dec 2023 21:07:09 GMT  
		Size: 5.2 KB (5179 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:innovation-oraclelinux8` - unknown; unknown

```console
$ docker pull mysql@sha256:9b1966fea33a8f487098b70ebc30c23b2700a8731bcff2bd124779ba2f8cf2be
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.6 MB (11606464 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:557704055f52c52ae3fcc218fa7168216870eca8326c1b1e89d434ad3ec00204`

```dockerfile
```

-	Layers:
	-	`sha256:0b211226c249aefed58e7da4b41bb3219beb5345fe5ed4e65c65ab47e378292b`  
		Last Modified: Tue, 19 Dec 2023 21:07:09 GMT  
		Size: 11.6 MB (11571692 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:097024790a6d6019cd411ce0478476fbfebc733402110550a33d6009f3aca07d`  
		Last Modified: Tue, 19 Dec 2023 21:07:09 GMT  
		Size: 34.8 KB (34772 bytes)  
		MIME: application/vnd.in-toto+json

## `mysql:latest`

```console
$ docker pull mysql@sha256:2d82ba6960cdf254de13f57d7265570c0675bc8bae1051e4a9806cff863006c9
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `mysql:latest` - linux; amd64

```console
$ docker pull mysql@sha256:28a16e31b140d750048cd5fadcaed22ac08d0eeb18567f79f822aee1f237b43c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **181.6 MB (181572393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73246731c4b01c19b8713c6408c6c5d898ac04f75f2a4ce998930f12091542f2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 18 Dec 2023 23:06:09 GMT
ADD file:da89b67e484bc45f357250a868fd78e28086b13e4315635d19648e5d43812e89 in / 
# Mon, 18 Dec 2023 23:06:09 GMT
CMD ["/bin/bash"]
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV GOSU_VERSION=1.16
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME" # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_MAJOR=innovation
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_VERSION=8.2.0-1.el8
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eu; 	{ 		echo '[mysqlinnovation-server-minimal]'; 		echo 'name=MySQL innovation Server Minimal'; 		echo 'enabled=1'; 		echo 'baseurl=https://repo.mysql.com/yum/mysql-innovation-community/docker/el/8/$basearch/'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eu; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo 'baseurl=https://repo.mysql.com/yum/mysql-tools-innovation-community/el/8/$basearch/'; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_SHELL_VERSION=8.2.1-1.el8
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
VOLUME [/var/lib/mysql]
# Mon, 18 Dec 2023 23:06:09 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 18 Dec 2023 23:06:09 GMT
EXPOSE map[3306/tcp:{} 33060/tcp:{}]
# Mon, 18 Dec 2023 23:06:09 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:bce031bc522d421fb188ef82a530f85c5477bb87cdeacdb911ea86f3f7cd3b66`  
		Last Modified: Wed, 20 Dec 2023 22:42:00 GMT  
		Size: 51.3 MB (51323468 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cf7e9f463619cbda1168fb597e71ce50b4ecd4546ad74050f5b5c67a152ca249`  
		Last Modified: Thu, 21 Dec 2023 00:41:48 GMT  
		Size: 883.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:105f403783c74e137d330ef98facdded2cab753187765ed8c453bb7b061a0002`  
		Last Modified: Thu, 21 Dec 2023 00:41:48 GMT  
		Size: 982.8 KB (982809 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:878e53a613d8011ad3d6207863d1555fe571430d3c6f7659d1eb0fd7f28ba7de`  
		Last Modified: Thu, 21 Dec 2023 00:41:48 GMT  
		Size: 4.6 MB (4594819 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2a362044e79fb6669726216e996a0a9fa018ba304d75ac30c9378a93160182de`  
		Last Modified: Thu, 21 Dec 2023 00:41:48 GMT  
		Size: 2.6 KB (2608 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6e4df4f73cfe883156b974e5269c673e52de0e1a56d610f2974793cd52d8b043`  
		Last Modified: Thu, 21 Dec 2023 00:41:49 GMT  
		Size: 340.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:69263d6347550e51a3b3f972d5aee303fd3c8c6d75376aad0b4cdcd4cb3f83be`  
		Last Modified: Thu, 21 Dec 2023 00:41:49 GMT  
		Size: 62.6 MB (62574253 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fe5e855492024c60c48d8eb006c94b71d6622f6d5c741cfa611e571a88a67d37`  
		Last Modified: Thu, 21 Dec 2023 00:41:49 GMT  
		Size: 325.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5c02229ce6f164ee6c47c91ddaa42db249b197b8b28dc6814a4df879a4f96a3e`  
		Last Modified: Thu, 21 Dec 2023 00:41:50 GMT  
		Size: 62.1 MB (62087711 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7320aa32bf42c0642bc86e30dac0b10335258a24b6ba374e173918ba8d9f9f63`  
		Last Modified: Thu, 21 Dec 2023 00:41:49 GMT  
		Size: 5.2 KB (5177 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:latest` - unknown; unknown

```console
$ docker pull mysql@sha256:483bf8eb111365bf322a25443d3f96ae0d80829c60f00fb329d8a0de0f21c6e7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.6 MB (11608021 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:501f9b1df36151d7e7ebba69fac20d69995d956d3851313ac3b4fdf9fa4e9ad3`

```dockerfile
```

-	Layers:
	-	`sha256:8de9290b82bb48a07e68ea96148c288ffa09729055d5c506b7690cf42f948baf`  
		Last Modified: Thu, 21 Dec 2023 00:41:48 GMT  
		Size: 11.6 MB (11573114 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:0b8a63c307592189c7a4ea188ee3b5e76eba99edc475a34c635157d5e893e536`  
		Last Modified: Thu, 21 Dec 2023 00:41:48 GMT  
		Size: 34.9 KB (34907 bytes)  
		MIME: application/vnd.in-toto+json

### `mysql:latest` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:86f5987d89514a0ec8043202ba341717c6d2f726749924ef7f220839ac576cf8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **185.3 MB (185275916 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e963a4c2b1a0d8774a4b6138a86d2bcca8b8f5cec58fbfabf7ae4ae021159e0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 06 Dec 2023 19:42:27 GMT
ADD file:f5ee75151bd25b33e72aa4c0560815f35f6e662876bf3733a02e5cb970227358 in / 
# Wed, 06 Dec 2023 19:42:27 GMT
CMD ["/bin/bash"]
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV GOSU_VERSION=1.16
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME" # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_MAJOR=innovation
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_VERSION=8.2.0-1.el8
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eu; 	{ 		echo '[mysqlinnovation-server-minimal]'; 		echo 'name=MySQL innovation Server Minimal'; 		echo 'enabled=1'; 		echo 'baseurl=https://repo.mysql.com/yum/mysql-innovation-community/docker/el/8/$basearch/'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eu; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo 'baseurl=https://repo.mysql.com/yum/mysql-tools-innovation-community/el/8/$basearch/'; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_SHELL_VERSION=8.2.1-1.el8
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
VOLUME [/var/lib/mysql]
# Mon, 18 Dec 2023 23:06:09 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 18 Dec 2023 23:06:09 GMT
EXPOSE map[3306/tcp:{} 33060/tcp:{}]
# Mon, 18 Dec 2023 23:06:09 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:edfaa6c9daada52a737333e0818f3d697d745aab3f3351e773218a524ebc9e53`  
		Last Modified: Wed, 06 Dec 2023 19:43:23 GMT  
		Size: 50.1 MB (50072545 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:19c686b91aca61da8058a44e9f6aa06cbb27aa65cf2db0768377bcc6899dc0c2`  
		Last Modified: Thu, 14 Dec 2023 20:15:05 GMT  
		Size: 885.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8c39062282e36f6169d219352cb19810ac7506e408e89b4ef33c400903a6ecc1`  
		Last Modified: Thu, 14 Dec 2023 20:15:05 GMT  
		Size: 913.0 KB (912965 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:73452dd561ff872804f5a63faab7552647c80c8a399e834fe154707a48613b20`  
		Last Modified: Thu, 14 Dec 2023 20:15:05 GMT  
		Size: 4.3 MB (4300794 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0ba54e261f50c32496de78ff38c42eb03cb97850ddbeb3c96f4fe34ea1cb23bc`  
		Last Modified: Thu, 14 Dec 2023 20:15:05 GMT  
		Size: 2.6 KB (2609 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b22c0fd6cce4772b17fe2500d6ce97e3a35076112226cc23269afa1542f7b51d`  
		Last Modified: Thu, 14 Dec 2023 20:15:06 GMT  
		Size: 340.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:eaffd91cbb1278d374c5b91f8a3e87239e73b0113a1fa5835faf13bcb05948dc`  
		Last Modified: Thu, 14 Dec 2023 20:15:09 GMT  
		Size: 61.6 MB (61602995 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3ec60922d8e9eefbce5167faf6f2296ddec22dcafc9a84f5db6f94e92e032089`  
		Last Modified: Thu, 14 Dec 2023 20:15:07 GMT  
		Size: 325.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:942dbd5bb0a98d45556f650aa3174e3e4a5fcf822e5e7a67529ae622bb02b14a`  
		Last Modified: Thu, 14 Dec 2023 20:15:09 GMT  
		Size: 68.4 MB (68377279 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bc7ea546f5793dcfecf365aefc956d7999a086211dc195cbb5d73d09df397fe2`  
		Last Modified: Tue, 19 Dec 2023 21:07:09 GMT  
		Size: 5.2 KB (5179 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:latest` - unknown; unknown

```console
$ docker pull mysql@sha256:9b1966fea33a8f487098b70ebc30c23b2700a8731bcff2bd124779ba2f8cf2be
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.6 MB (11606464 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:557704055f52c52ae3fcc218fa7168216870eca8326c1b1e89d434ad3ec00204`

```dockerfile
```

-	Layers:
	-	`sha256:0b211226c249aefed58e7da4b41bb3219beb5345fe5ed4e65c65ab47e378292b`  
		Last Modified: Tue, 19 Dec 2023 21:07:09 GMT  
		Size: 11.6 MB (11571692 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:097024790a6d6019cd411ce0478476fbfebc733402110550a33d6009f3aca07d`  
		Last Modified: Tue, 19 Dec 2023 21:07:09 GMT  
		Size: 34.8 KB (34772 bytes)  
		MIME: application/vnd.in-toto+json

## `mysql:oracle`

```console
$ docker pull mysql@sha256:2d82ba6960cdf254de13f57d7265570c0675bc8bae1051e4a9806cff863006c9
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `mysql:oracle` - linux; amd64

```console
$ docker pull mysql@sha256:28a16e31b140d750048cd5fadcaed22ac08d0eeb18567f79f822aee1f237b43c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **181.6 MB (181572393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73246731c4b01c19b8713c6408c6c5d898ac04f75f2a4ce998930f12091542f2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 18 Dec 2023 23:06:09 GMT
ADD file:da89b67e484bc45f357250a868fd78e28086b13e4315635d19648e5d43812e89 in / 
# Mon, 18 Dec 2023 23:06:09 GMT
CMD ["/bin/bash"]
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV GOSU_VERSION=1.16
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME" # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_MAJOR=innovation
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_VERSION=8.2.0-1.el8
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eu; 	{ 		echo '[mysqlinnovation-server-minimal]'; 		echo 'name=MySQL innovation Server Minimal'; 		echo 'enabled=1'; 		echo 'baseurl=https://repo.mysql.com/yum/mysql-innovation-community/docker/el/8/$basearch/'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eu; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo 'baseurl=https://repo.mysql.com/yum/mysql-tools-innovation-community/el/8/$basearch/'; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_SHELL_VERSION=8.2.1-1.el8
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
VOLUME [/var/lib/mysql]
# Mon, 18 Dec 2023 23:06:09 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 18 Dec 2023 23:06:09 GMT
EXPOSE map[3306/tcp:{} 33060/tcp:{}]
# Mon, 18 Dec 2023 23:06:09 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:bce031bc522d421fb188ef82a530f85c5477bb87cdeacdb911ea86f3f7cd3b66`  
		Last Modified: Wed, 20 Dec 2023 22:42:00 GMT  
		Size: 51.3 MB (51323468 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cf7e9f463619cbda1168fb597e71ce50b4ecd4546ad74050f5b5c67a152ca249`  
		Last Modified: Thu, 21 Dec 2023 00:41:48 GMT  
		Size: 883.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:105f403783c74e137d330ef98facdded2cab753187765ed8c453bb7b061a0002`  
		Last Modified: Thu, 21 Dec 2023 00:41:48 GMT  
		Size: 982.8 KB (982809 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:878e53a613d8011ad3d6207863d1555fe571430d3c6f7659d1eb0fd7f28ba7de`  
		Last Modified: Thu, 21 Dec 2023 00:41:48 GMT  
		Size: 4.6 MB (4594819 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2a362044e79fb6669726216e996a0a9fa018ba304d75ac30c9378a93160182de`  
		Last Modified: Thu, 21 Dec 2023 00:41:48 GMT  
		Size: 2.6 KB (2608 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6e4df4f73cfe883156b974e5269c673e52de0e1a56d610f2974793cd52d8b043`  
		Last Modified: Thu, 21 Dec 2023 00:41:49 GMT  
		Size: 340.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:69263d6347550e51a3b3f972d5aee303fd3c8c6d75376aad0b4cdcd4cb3f83be`  
		Last Modified: Thu, 21 Dec 2023 00:41:49 GMT  
		Size: 62.6 MB (62574253 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fe5e855492024c60c48d8eb006c94b71d6622f6d5c741cfa611e571a88a67d37`  
		Last Modified: Thu, 21 Dec 2023 00:41:49 GMT  
		Size: 325.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5c02229ce6f164ee6c47c91ddaa42db249b197b8b28dc6814a4df879a4f96a3e`  
		Last Modified: Thu, 21 Dec 2023 00:41:50 GMT  
		Size: 62.1 MB (62087711 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7320aa32bf42c0642bc86e30dac0b10335258a24b6ba374e173918ba8d9f9f63`  
		Last Modified: Thu, 21 Dec 2023 00:41:49 GMT  
		Size: 5.2 KB (5177 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:oracle` - unknown; unknown

```console
$ docker pull mysql@sha256:483bf8eb111365bf322a25443d3f96ae0d80829c60f00fb329d8a0de0f21c6e7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.6 MB (11608021 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:501f9b1df36151d7e7ebba69fac20d69995d956d3851313ac3b4fdf9fa4e9ad3`

```dockerfile
```

-	Layers:
	-	`sha256:8de9290b82bb48a07e68ea96148c288ffa09729055d5c506b7690cf42f948baf`  
		Last Modified: Thu, 21 Dec 2023 00:41:48 GMT  
		Size: 11.6 MB (11573114 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:0b8a63c307592189c7a4ea188ee3b5e76eba99edc475a34c635157d5e893e536`  
		Last Modified: Thu, 21 Dec 2023 00:41:48 GMT  
		Size: 34.9 KB (34907 bytes)  
		MIME: application/vnd.in-toto+json

### `mysql:oracle` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:86f5987d89514a0ec8043202ba341717c6d2f726749924ef7f220839ac576cf8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **185.3 MB (185275916 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e963a4c2b1a0d8774a4b6138a86d2bcca8b8f5cec58fbfabf7ae4ae021159e0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 06 Dec 2023 19:42:27 GMT
ADD file:f5ee75151bd25b33e72aa4c0560815f35f6e662876bf3733a02e5cb970227358 in / 
# Wed, 06 Dec 2023 19:42:27 GMT
CMD ["/bin/bash"]
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV GOSU_VERSION=1.16
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME" # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_MAJOR=innovation
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_VERSION=8.2.0-1.el8
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eu; 	{ 		echo '[mysqlinnovation-server-minimal]'; 		echo 'name=MySQL innovation Server Minimal'; 		echo 'enabled=1'; 		echo 'baseurl=https://repo.mysql.com/yum/mysql-innovation-community/docker/el/8/$basearch/'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eu; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo 'baseurl=https://repo.mysql.com/yum/mysql-tools-innovation-community/el/8/$basearch/'; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_SHELL_VERSION=8.2.1-1.el8
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
VOLUME [/var/lib/mysql]
# Mon, 18 Dec 2023 23:06:09 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 18 Dec 2023 23:06:09 GMT
EXPOSE map[3306/tcp:{} 33060/tcp:{}]
# Mon, 18 Dec 2023 23:06:09 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:edfaa6c9daada52a737333e0818f3d697d745aab3f3351e773218a524ebc9e53`  
		Last Modified: Wed, 06 Dec 2023 19:43:23 GMT  
		Size: 50.1 MB (50072545 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:19c686b91aca61da8058a44e9f6aa06cbb27aa65cf2db0768377bcc6899dc0c2`  
		Last Modified: Thu, 14 Dec 2023 20:15:05 GMT  
		Size: 885.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8c39062282e36f6169d219352cb19810ac7506e408e89b4ef33c400903a6ecc1`  
		Last Modified: Thu, 14 Dec 2023 20:15:05 GMT  
		Size: 913.0 KB (912965 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:73452dd561ff872804f5a63faab7552647c80c8a399e834fe154707a48613b20`  
		Last Modified: Thu, 14 Dec 2023 20:15:05 GMT  
		Size: 4.3 MB (4300794 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0ba54e261f50c32496de78ff38c42eb03cb97850ddbeb3c96f4fe34ea1cb23bc`  
		Last Modified: Thu, 14 Dec 2023 20:15:05 GMT  
		Size: 2.6 KB (2609 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b22c0fd6cce4772b17fe2500d6ce97e3a35076112226cc23269afa1542f7b51d`  
		Last Modified: Thu, 14 Dec 2023 20:15:06 GMT  
		Size: 340.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:eaffd91cbb1278d374c5b91f8a3e87239e73b0113a1fa5835faf13bcb05948dc`  
		Last Modified: Thu, 14 Dec 2023 20:15:09 GMT  
		Size: 61.6 MB (61602995 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3ec60922d8e9eefbce5167faf6f2296ddec22dcafc9a84f5db6f94e92e032089`  
		Last Modified: Thu, 14 Dec 2023 20:15:07 GMT  
		Size: 325.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:942dbd5bb0a98d45556f650aa3174e3e4a5fcf822e5e7a67529ae622bb02b14a`  
		Last Modified: Thu, 14 Dec 2023 20:15:09 GMT  
		Size: 68.4 MB (68377279 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bc7ea546f5793dcfecf365aefc956d7999a086211dc195cbb5d73d09df397fe2`  
		Last Modified: Tue, 19 Dec 2023 21:07:09 GMT  
		Size: 5.2 KB (5179 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:oracle` - unknown; unknown

```console
$ docker pull mysql@sha256:9b1966fea33a8f487098b70ebc30c23b2700a8731bcff2bd124779ba2f8cf2be
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.6 MB (11606464 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:557704055f52c52ae3fcc218fa7168216870eca8326c1b1e89d434ad3ec00204`

```dockerfile
```

-	Layers:
	-	`sha256:0b211226c249aefed58e7da4b41bb3219beb5345fe5ed4e65c65ab47e378292b`  
		Last Modified: Tue, 19 Dec 2023 21:07:09 GMT  
		Size: 11.6 MB (11571692 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:097024790a6d6019cd411ce0478476fbfebc733402110550a33d6009f3aca07d`  
		Last Modified: Tue, 19 Dec 2023 21:07:09 GMT  
		Size: 34.8 KB (34772 bytes)  
		MIME: application/vnd.in-toto+json

## `mysql:oraclelinux8`

```console
$ docker pull mysql@sha256:2d82ba6960cdf254de13f57d7265570c0675bc8bae1051e4a9806cff863006c9
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `mysql:oraclelinux8` - linux; amd64

```console
$ docker pull mysql@sha256:28a16e31b140d750048cd5fadcaed22ac08d0eeb18567f79f822aee1f237b43c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **181.6 MB (181572393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73246731c4b01c19b8713c6408c6c5d898ac04f75f2a4ce998930f12091542f2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Mon, 18 Dec 2023 23:06:09 GMT
ADD file:da89b67e484bc45f357250a868fd78e28086b13e4315635d19648e5d43812e89 in / 
# Mon, 18 Dec 2023 23:06:09 GMT
CMD ["/bin/bash"]
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV GOSU_VERSION=1.16
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME" # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_MAJOR=innovation
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_VERSION=8.2.0-1.el8
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eu; 	{ 		echo '[mysqlinnovation-server-minimal]'; 		echo 'name=MySQL innovation Server Minimal'; 		echo 'enabled=1'; 		echo 'baseurl=https://repo.mysql.com/yum/mysql-innovation-community/docker/el/8/$basearch/'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eu; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo 'baseurl=https://repo.mysql.com/yum/mysql-tools-innovation-community/el/8/$basearch/'; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_SHELL_VERSION=8.2.1-1.el8
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
VOLUME [/var/lib/mysql]
# Mon, 18 Dec 2023 23:06:09 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 18 Dec 2023 23:06:09 GMT
EXPOSE map[3306/tcp:{} 33060/tcp:{}]
# Mon, 18 Dec 2023 23:06:09 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:bce031bc522d421fb188ef82a530f85c5477bb87cdeacdb911ea86f3f7cd3b66`  
		Last Modified: Wed, 20 Dec 2023 22:42:00 GMT  
		Size: 51.3 MB (51323468 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cf7e9f463619cbda1168fb597e71ce50b4ecd4546ad74050f5b5c67a152ca249`  
		Last Modified: Thu, 21 Dec 2023 00:41:48 GMT  
		Size: 883.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:105f403783c74e137d330ef98facdded2cab753187765ed8c453bb7b061a0002`  
		Last Modified: Thu, 21 Dec 2023 00:41:48 GMT  
		Size: 982.8 KB (982809 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:878e53a613d8011ad3d6207863d1555fe571430d3c6f7659d1eb0fd7f28ba7de`  
		Last Modified: Thu, 21 Dec 2023 00:41:48 GMT  
		Size: 4.6 MB (4594819 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2a362044e79fb6669726216e996a0a9fa018ba304d75ac30c9378a93160182de`  
		Last Modified: Thu, 21 Dec 2023 00:41:48 GMT  
		Size: 2.6 KB (2608 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6e4df4f73cfe883156b974e5269c673e52de0e1a56d610f2974793cd52d8b043`  
		Last Modified: Thu, 21 Dec 2023 00:41:49 GMT  
		Size: 340.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:69263d6347550e51a3b3f972d5aee303fd3c8c6d75376aad0b4cdcd4cb3f83be`  
		Last Modified: Thu, 21 Dec 2023 00:41:49 GMT  
		Size: 62.6 MB (62574253 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fe5e855492024c60c48d8eb006c94b71d6622f6d5c741cfa611e571a88a67d37`  
		Last Modified: Thu, 21 Dec 2023 00:41:49 GMT  
		Size: 325.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5c02229ce6f164ee6c47c91ddaa42db249b197b8b28dc6814a4df879a4f96a3e`  
		Last Modified: Thu, 21 Dec 2023 00:41:50 GMT  
		Size: 62.1 MB (62087711 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7320aa32bf42c0642bc86e30dac0b10335258a24b6ba374e173918ba8d9f9f63`  
		Last Modified: Thu, 21 Dec 2023 00:41:49 GMT  
		Size: 5.2 KB (5177 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:oraclelinux8` - unknown; unknown

```console
$ docker pull mysql@sha256:483bf8eb111365bf322a25443d3f96ae0d80829c60f00fb329d8a0de0f21c6e7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.6 MB (11608021 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:501f9b1df36151d7e7ebba69fac20d69995d956d3851313ac3b4fdf9fa4e9ad3`

```dockerfile
```

-	Layers:
	-	`sha256:8de9290b82bb48a07e68ea96148c288ffa09729055d5c506b7690cf42f948baf`  
		Last Modified: Thu, 21 Dec 2023 00:41:48 GMT  
		Size: 11.6 MB (11573114 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:0b8a63c307592189c7a4ea188ee3b5e76eba99edc475a34c635157d5e893e536`  
		Last Modified: Thu, 21 Dec 2023 00:41:48 GMT  
		Size: 34.9 KB (34907 bytes)  
		MIME: application/vnd.in-toto+json

### `mysql:oraclelinux8` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:86f5987d89514a0ec8043202ba341717c6d2f726749924ef7f220839ac576cf8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **185.3 MB (185275916 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e963a4c2b1a0d8774a4b6138a86d2bcca8b8f5cec58fbfabf7ae4ae021159e0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 06 Dec 2023 19:42:27 GMT
ADD file:f5ee75151bd25b33e72aa4c0560815f35f6e662876bf3733a02e5cb970227358 in / 
# Wed, 06 Dec 2023 19:42:27 GMT
CMD ["/bin/bash"]
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV GOSU_VERSION=1.16
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME" # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_MAJOR=innovation
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_VERSION=8.2.0-1.el8
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eu; 	{ 		echo '[mysqlinnovation-server-minimal]'; 		echo 'name=MySQL innovation Server Minimal'; 		echo 'enabled=1'; 		echo 'baseurl=https://repo.mysql.com/yum/mysql-innovation-community/docker/el/8/$basearch/'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eu; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo 'baseurl=https://repo.mysql.com/yum/mysql-tools-innovation-community/el/8/$basearch/'; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENV MYSQL_SHELL_VERSION=8.2.1-1.el8
# Mon, 18 Dec 2023 23:06:09 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
VOLUME [/var/lib/mysql]
# Mon, 18 Dec 2023 23:06:09 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 18 Dec 2023 23:06:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 18 Dec 2023 23:06:09 GMT
EXPOSE map[3306/tcp:{} 33060/tcp:{}]
# Mon, 18 Dec 2023 23:06:09 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:edfaa6c9daada52a737333e0818f3d697d745aab3f3351e773218a524ebc9e53`  
		Last Modified: Wed, 06 Dec 2023 19:43:23 GMT  
		Size: 50.1 MB (50072545 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:19c686b91aca61da8058a44e9f6aa06cbb27aa65cf2db0768377bcc6899dc0c2`  
		Last Modified: Thu, 14 Dec 2023 20:15:05 GMT  
		Size: 885.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8c39062282e36f6169d219352cb19810ac7506e408e89b4ef33c400903a6ecc1`  
		Last Modified: Thu, 14 Dec 2023 20:15:05 GMT  
		Size: 913.0 KB (912965 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:73452dd561ff872804f5a63faab7552647c80c8a399e834fe154707a48613b20`  
		Last Modified: Thu, 14 Dec 2023 20:15:05 GMT  
		Size: 4.3 MB (4300794 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0ba54e261f50c32496de78ff38c42eb03cb97850ddbeb3c96f4fe34ea1cb23bc`  
		Last Modified: Thu, 14 Dec 2023 20:15:05 GMT  
		Size: 2.6 KB (2609 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b22c0fd6cce4772b17fe2500d6ce97e3a35076112226cc23269afa1542f7b51d`  
		Last Modified: Thu, 14 Dec 2023 20:15:06 GMT  
		Size: 340.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:eaffd91cbb1278d374c5b91f8a3e87239e73b0113a1fa5835faf13bcb05948dc`  
		Last Modified: Thu, 14 Dec 2023 20:15:09 GMT  
		Size: 61.6 MB (61602995 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3ec60922d8e9eefbce5167faf6f2296ddec22dcafc9a84f5db6f94e92e032089`  
		Last Modified: Thu, 14 Dec 2023 20:15:07 GMT  
		Size: 325.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:942dbd5bb0a98d45556f650aa3174e3e4a5fcf822e5e7a67529ae622bb02b14a`  
		Last Modified: Thu, 14 Dec 2023 20:15:09 GMT  
		Size: 68.4 MB (68377279 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bc7ea546f5793dcfecf365aefc956d7999a086211dc195cbb5d73d09df397fe2`  
		Last Modified: Tue, 19 Dec 2023 21:07:09 GMT  
		Size: 5.2 KB (5179 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:oraclelinux8` - unknown; unknown

```console
$ docker pull mysql@sha256:9b1966fea33a8f487098b70ebc30c23b2700a8731bcff2bd124779ba2f8cf2be
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.6 MB (11606464 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:557704055f52c52ae3fcc218fa7168216870eca8326c1b1e89d434ad3ec00204`

```dockerfile
```

-	Layers:
	-	`sha256:0b211226c249aefed58e7da4b41bb3219beb5345fe5ed4e65c65ab47e378292b`  
		Last Modified: Tue, 19 Dec 2023 21:07:09 GMT  
		Size: 11.6 MB (11571692 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:097024790a6d6019cd411ce0478476fbfebc733402110550a33d6009f3aca07d`  
		Last Modified: Tue, 19 Dec 2023 21:07:09 GMT  
		Size: 34.8 KB (34772 bytes)  
		MIME: application/vnd.in-toto+json
