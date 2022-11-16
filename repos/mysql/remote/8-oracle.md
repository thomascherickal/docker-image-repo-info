## `mysql:8-oracle`

```console
$ docker pull mysql@sha256:25aace9734db96ae09c24c6a2eeb6db4720c41d493de352eb76007eddf437fbe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:bd6a2996d80605c41b1ebd8f822894471695b1fd2427505ac518e650a14ef8c6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **157.2 MB (157232215 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a04bf34fdf036292486d39f731cffaf0bb56522c340fe4841b2c71cf89c9d62`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 04 Nov 2022 23:33:07 GMT
ADD file:00e6899b8d3eccf7f795d17f9316af6ae0f3955ef2204b61bd064f5173c18357 in / 
# Fri, 04 Nov 2022 23:33:07 GMT
CMD ["/bin/bash"]
# Sat, 05 Nov 2022 02:34:46 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Sat, 05 Nov 2022 02:34:46 GMT
ENV GOSU_VERSION=1.14
# Sat, 05 Nov 2022 02:34:50 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 05 Nov 2022 02:35:13 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Sat, 05 Nov 2022 02:35:14 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Sat, 05 Nov 2022 02:35:14 GMT
ENV MYSQL_MAJOR=8.0
# Sat, 05 Nov 2022 02:35:14 GMT
ENV MYSQL_VERSION=8.0.31-1.el8
# Sat, 05 Nov 2022 02:35:15 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Sat, 05 Nov 2022 02:35:44 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Sat, 05 Nov 2022 02:35:45 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Sat, 05 Nov 2022 02:35:45 GMT
ENV MYSQL_SHELL_VERSION=8.0.31-1.el8
# Sat, 05 Nov 2022 02:36:18 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Sat, 05 Nov 2022 02:36:19 GMT
VOLUME [/var/lib/mysql]
# Sat, 05 Nov 2022 02:36:19 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Sat, 05 Nov 2022 02:36:20 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Sat, 05 Nov 2022 02:36:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 05 Nov 2022 02:36:20 GMT
EXPOSE 3306 33060
# Sat, 05 Nov 2022 02:36:20 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:feec22b5b79860f47a87861bed3a29d5431a279cc239b44a2522a9ab5459d844`  
		Last Modified: Fri, 04 Nov 2022 23:34:48 GMT  
		Size: 40.6 MB (40580917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b33952322b1265ccfb1a2fa879b86ccb58a3c5f02567a902cac8d7d1e1fbcac`  
		Last Modified: Sat, 05 Nov 2022 02:38:17 GMT  
		Size: 888.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8632ee03bb1ca20bb263a7bab04dda4995925a4ed5e2a16fa83e174a53a840c3`  
		Last Modified: Sat, 05 Nov 2022 02:38:17 GMT  
		Size: 928.8 KB (928831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:636ccd115361ca8e84b27ef37d14d6119748b71900dade590ecd963afab4450c`  
		Last Modified: Sat, 05 Nov 2022 02:38:16 GMT  
		Size: 4.6 MB (4596992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b07c8fac8eead4f4a9e8284577eaf9ae5ca2c78a3cbecf1b9f0c7a4b78337665`  
		Last Modified: Sat, 05 Nov 2022 02:38:15 GMT  
		Size: 2.6 KB (2629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e44c54db9c140998b59508c389ead06ffbe863051125b2dd2b150db5d8f87010`  
		Last Modified: Sat, 05 Nov 2022 02:38:14 GMT  
		Size: 335.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf9c45749101c2502030b52b11f5cf1031d08ceabeab91283742467bdbe2dc62`  
		Last Modified: Sat, 05 Nov 2022 02:38:21 GMT  
		Size: 56.0 MB (56047607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f2fa3febc47da546527aae2d8de736b7562b0e8f5a37a63778aa86307af8d2d`  
		Last Modified: Sat, 05 Nov 2022 02:38:12 GMT  
		Size: 317.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44d5e1d3c311ae16390016bcf09a400cc9e67473f8ea5787abe0855f510e917b`  
		Last Modified: Sat, 05 Nov 2022 02:38:23 GMT  
		Size: 55.1 MB (55068188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb3db2c5d8ec681907739aa09873795aa7ffacfacfbd43d79f140331029f8517`  
		Last Modified: Sat, 05 Nov 2022 02:38:13 GMT  
		Size: 5.4 KB (5390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0ead729abd92d539d786eed0146f98fbfb8a970de2f0b082e9a0aa4ecc6d1fc`  
		Last Modified: Sat, 05 Nov 2022 02:38:12 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8-oracle` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:a0b6340a3f236d39451f2373c5d137bf64eb54233163c186ef1480e8844f0ffd
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **159.0 MB (159044836 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b61a400e8776905c7164e1adcf7c9457bfe43dca3db94b667a3e4dd8e7f02c1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 15 Nov 2022 23:40:44 GMT
ADD file:44569001378d2d59b2d169aba48a6b2b88529ca46fd5d85598eff7ca37ded076 in / 
# Tue, 15 Nov 2022 23:40:45 GMT
CMD ["/bin/bash"]
# Wed, 16 Nov 2022 01:33:23 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 16 Nov 2022 01:33:23 GMT
ENV GOSU_VERSION=1.14
# Wed, 16 Nov 2022 01:33:26 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 16 Nov 2022 01:33:47 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Wed, 16 Nov 2022 01:33:48 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 16 Nov 2022 01:33:48 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 16 Nov 2022 01:33:48 GMT
ENV MYSQL_VERSION=8.0.31-1.el8
# Wed, 16 Nov 2022 01:33:49 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 16 Nov 2022 01:34:14 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 16 Nov 2022 01:34:16 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 16 Nov 2022 01:34:16 GMT
ENV MYSQL_SHELL_VERSION=8.0.31-1.el8
# Wed, 16 Nov 2022 01:34:44 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Wed, 16 Nov 2022 01:34:46 GMT
VOLUME [/var/lib/mysql]
# Wed, 16 Nov 2022 01:34:46 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 16 Nov 2022 01:34:46 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 16 Nov 2022 01:34:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Nov 2022 01:34:46 GMT
EXPOSE 3306 33060
# Wed, 16 Nov 2022 01:34:46 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:01d65ebb4955ae24720eb5c24ff08081fed75975aea7b87c96ef7e58175901e0`  
		Last Modified: Tue, 15 Nov 2022 23:41:32 GMT  
		Size: 42.8 MB (42774711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d609fcc3c7fb5a4b262e7f8a002961e11802f03e441d9e8a2c1d0a03b606e1ee`  
		Last Modified: Wed, 16 Nov 2022 01:35:16 GMT  
		Size: 886.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52c09cdcd2da34e1fedf1e87c4cf449692e8fcd446a600a227ff7a3c678eba26`  
		Last Modified: Wed, 16 Nov 2022 01:35:16 GMT  
		Size: 857.2 KB (857169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a478ef641e124539c75eca120d506f59fc5058ce27559d948305ec930643717`  
		Last Modified: Wed, 16 Nov 2022 01:35:15 GMT  
		Size: 4.5 MB (4465955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f3956cc2f3fb1e3431a0db90666aa3e21c2015b9ddd6da49babc7bb389a09e8`  
		Last Modified: Wed, 16 Nov 2022 01:35:14 GMT  
		Size: 2.6 KB (2630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33c37cc7a1914f1576343f24a780bedcdea90a844ccd62488df65355b06468fd`  
		Last Modified: Wed, 16 Nov 2022 01:35:14 GMT  
		Size: 337.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f0cd074dc147bcc06f8561f3added6b2ea97772000b3628f2e03503691904e0`  
		Last Modified: Wed, 16 Nov 2022 01:35:18 GMT  
		Size: 55.5 MB (55457981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9186a35382189d0459f0ce2a8166b45cbf2be5599cfe5716bdbc5de71ee3d2b2`  
		Last Modified: Wed, 16 Nov 2022 01:35:12 GMT  
		Size: 318.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0443c4afe5f0f372b7558dc78484a7577e29c0d906b2e4324fbeb81d6bee853f`  
		Last Modified: Wed, 16 Nov 2022 01:35:20 GMT  
		Size: 55.5 MB (55479334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3dbcd809e720177fc48884b92fb5e724ada0908ef9449445df4847f40a9c3d2`  
		Last Modified: Wed, 16 Nov 2022 01:35:12 GMT  
		Size: 5.4 KB (5394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb36129f08c1e07dd8ad073c1fa8012fb05b03766001cbc228fbddc20edec95e`  
		Last Modified: Wed, 16 Nov 2022 01:35:12 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
