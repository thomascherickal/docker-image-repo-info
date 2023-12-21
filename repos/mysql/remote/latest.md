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
