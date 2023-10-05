## `mysql:innovation-oracle`

```console
$ docker pull mysql@sha256:44056c45e214c26c37b6f244534c6fb5f8a40eacbc28e870a2652b19d7a8a814
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `mysql:innovation-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:5253d1662109ba7776430522fd73bd37f1c5775235eec63883fb8294d22757bc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **166.9 MB (166863356 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c138801544a941ed9d1171794e3361533109aa7e22f2ea4e1ba85bccc84f6842`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 27 Jul 2023 22:18:51 GMT
ADD file:909c07f3bad92a80d3917d583769a01bf62c2cbf3dd24f450fb303b1db92a83e in / 
# Thu, 27 Jul 2023 22:18:51 GMT
CMD ["/bin/bash"]
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
ENV GOSU_VERSION=1.16
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME" # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
ENV MYSQL_MAJOR=innovation
# Thu, 27 Jul 2023 22:18:51 GMT
ENV MYSQL_VERSION=8.1.0-1.el8
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysqlinnovation-server-minimal]'; 		echo 'name=MySQL innovation Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-innovation-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
ENV MYSQL_SHELL_VERSION=8.0.34-1.el8
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
VOLUME [/var/lib/mysql]
# Thu, 27 Jul 2023 22:18:51 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 27 Jul 2023 22:18:51 GMT
EXPOSE map[3306/tcp:{} 33060/tcp:{}]
# Thu, 27 Jul 2023 22:18:51 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:5262579e8e45cb87fdc8fb6182d30da3c9e4f1036e02223508f287899ea434c0`  
		Last Modified: Thu, 21 Sep 2023 23:25:18 GMT  
		Size: 45.0 MB (44959147 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bfcc921068b5eaba8d310a26395ee4139cd54b21ec96369a39830e24cfe84477`  
		Last Modified: Wed, 04 Oct 2023 23:00:11 GMT  
		Size: 885.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:072a02315ab18d41372cf2e57b066a8ecf9954ab8d94cb5244ca20efe63df7ab`  
		Last Modified: Wed, 04 Oct 2023 23:00:11 GMT  
		Size: 982.8 KB (982808 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:711d47be56b4655b6deec62a811cddf52424477672f5930441ae8701ab012c95`  
		Last Modified: Wed, 04 Oct 2023 23:00:12 GMT  
		Size: 4.6 MB (4616305 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:755e67622a77c61bb6eb442164103b5395e7db380add9d61a2acb3425df65fa0`  
		Last Modified: Wed, 04 Oct 2023 23:00:12 GMT  
		Size: 2.6 KB (2608 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0080a11112d165a07d366db3a1ebd57709f066f4b13f10b57ec21e19d3d67d26`  
		Last Modified: Wed, 04 Oct 2023 23:00:12 GMT  
		Size: 340.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:adc45022a9ad6beda852b49f14ae18ff04ea052eb0f9391c31a29ecdffaa1ef1`  
		Last Modified: Wed, 04 Oct 2023 23:00:17 GMT  
		Size: 58.8 MB (58771345 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:67d8146998603ea2ed92b77bccbb35623a5eb39c6b047d15af930cec9ef79a9d`  
		Last Modified: Wed, 04 Oct 2023 23:00:13 GMT  
		Size: 316.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f431d85cf61e18099acd66976a43fb86be0ca84549a3853b4e2eaeb48557acb8`  
		Last Modified: Wed, 04 Oct 2023 23:00:16 GMT  
		Size: 57.5 MB (57524213 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4bbba6dd5ce26ba0b294a1cc506c8a57566efbaaf3701fe8eb752b54c4bd64c5`  
		Last Modified: Wed, 04 Oct 2023 23:00:14 GMT  
		Size: 5.4 KB (5389 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:innovation-oracle` - unknown; unknown

```console
$ docker pull mysql@sha256:3907151ff6c8a3d9a987e42f5af74ec79742398d67673c9e6f3baf067cbff3ab
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.1 MB (13141082 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3992e42cff0b10e86e3648547df8a978c66d19322dd629faa7cdacd2432028c9`

```dockerfile
```

-	Layers:
	-	`sha256:06d7ee16ec055f718e85ab70b205f9a40ac64f1f4bd3665bfd625ceffdce177c`  
		Last Modified: Wed, 04 Oct 2023 23:00:12 GMT  
		Size: 13.1 MB (13107503 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:81f9eeabc6e68920db4c4c28565e7cdbb580ecb31d9205d49fb827e33e860dd3`  
		Last Modified: Wed, 04 Oct 2023 23:00:11 GMT  
		Size: 33.6 KB (33579 bytes)  
		MIME: application/vnd.in-toto+json

### `mysql:innovation-oracle` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:2b94677c88791084b0deb390e1966c74f5b6b439c70437587d0ba25f0df52df0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.4 MB (170366065 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54fea0bc79f9c00cc1eb77f4ce9314d116b731d441f86972c6ffeef5987a0429`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 27 Jul 2023 22:18:51 GMT
ADD file:c630310324edbc0dd09d0912b8e7074d17ac71b1be8a14af9663872c081c4632 in / 
# Thu, 27 Jul 2023 22:18:51 GMT
CMD ["/bin/bash"]
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
ENV GOSU_VERSION=1.16
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME" # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
ENV MYSQL_MAJOR=innovation
# Thu, 27 Jul 2023 22:18:51 GMT
ENV MYSQL_VERSION=8.1.0-1.el8
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysqlinnovation-server-minimal]'; 		echo 'name=MySQL innovation Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-innovation-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
ENV MYSQL_SHELL_VERSION=8.0.34-1.el8
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
VOLUME [/var/lib/mysql]
# Thu, 27 Jul 2023 22:18:51 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 27 Jul 2023 22:18:51 GMT
EXPOSE map[3306/tcp:{} 33060/tcp:{}]
# Thu, 27 Jul 2023 22:18:51 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:286c1c922769d7608c32cf62931e95d7d169a0306164d24ce7d7a8a065959315`  
		Last Modified: Thu, 21 Sep 2023 23:41:39 GMT  
		Size: 43.7 MB (43657726 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cb7c97478965081773cf774f51b68ba7bc4ddeb1a1c4911ac6dd52e3939a9b02`  
		Last Modified: Wed, 04 Oct 2023 23:56:04 GMT  
		Size: 885.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4056102542df153013330c711c65a022891653dcb4f6b7b8584d32d1cc6ebf65`  
		Last Modified: Wed, 04 Oct 2023 23:56:04 GMT  
		Size: 913.0 KB (912965 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2cfd45c39ba383ddf8f928620c4623faab5bbed0c180b48b176c0361d441a358`  
		Last Modified: Wed, 04 Oct 2023 23:56:04 GMT  
		Size: 4.3 MB (4300663 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:770637688c59082858f7a4a8f12a627c10790774fad0c720ad868e871efcce47`  
		Last Modified: Wed, 04 Oct 2023 23:56:05 GMT  
		Size: 2.6 KB (2608 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5e04d4eff28a3ef1fd9d6816f12752bb2798413e20d7e54f9ac982ce912ea77b`  
		Last Modified: Wed, 04 Oct 2023 23:56:05 GMT  
		Size: 338.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6efba642676b7f08b17d6c5b657eebe1461166225dd8fd60013ceab2901c4e51`  
		Last Modified: Wed, 04 Oct 2023 23:56:08 GMT  
		Size: 57.7 MB (57708457 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6e706e7799d0736ff1b4df27c3a6703dcbb92134231f84f4fbcf841a201a8968`  
		Last Modified: Wed, 04 Oct 2023 23:56:06 GMT  
		Size: 316.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:94ede8436e0c5c1ba426163ae22d2e78a4449c1f90423be382adc88ef5e7f7df`  
		Last Modified: Wed, 04 Oct 2023 23:56:09 GMT  
		Size: 63.8 MB (63776717 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0433c6008f7b23b7308d19214b170ec2a1320794fad4f14e3089c9e932c73520`  
		Last Modified: Wed, 04 Oct 2023 23:56:07 GMT  
		Size: 5.4 KB (5390 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:innovation-oracle` - unknown; unknown

```console
$ docker pull mysql@sha256:0798fb11106cd915317ee2e883428e8c0509b66ba50c330bc08d98b71a2a4a93
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.1 MB (13139770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:50972c5093bb54a90971a3f64892fb3376c16d66dab33ee483a98b6b83f98382`

```dockerfile
```

-	Layers:
	-	`sha256:0952fb4b6cad899f5e32f2f4c030e7016feffbf1eaa3ee34e5bffc73c7e23b91`  
		Last Modified: Wed, 04 Oct 2023 23:56:05 GMT  
		Size: 13.1 MB (13106170 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:f9ff6e0e61f3655ad5ff5e9c2ebcd98ddbd7fcd1fd289af381f54c15137e50be`  
		Last Modified: Wed, 04 Oct 2023 23:56:03 GMT  
		Size: 33.6 KB (33600 bytes)  
		MIME: application/vnd.in-toto+json
