## `mysql:8-oracle`

```console
$ docker pull mysql@sha256:5aeabca77ff42a3e47dec06f38546a7bcfce2f851ff967355201bf36fc072682
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:7393ba5c8671f58923b3798cf4bf1be4143830bd7d42f656befa3eade6d862b4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.1 MB (133138390 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:396873955d6abc41308a7d35c3a1d23c775d7f13231a126848c73ce736f388e5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 24 Mar 2022 01:39:10 GMT
ADD file:c0f0a367bc612431ac9286b506fef5505e0b5f3969515486d8052ec381524261 in / 
# Thu, 24 Mar 2022 01:39:10 GMT
CMD ["/bin/bash"]
# Thu, 24 Mar 2022 02:12:04 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql; 		mkdir /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d
# Thu, 24 Mar 2022 02:12:04 GMT
ENV GOSU_VERSION=1.14
# Thu, 24 Mar 2022 02:12:07 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 24 Mar 2022 02:12:26 GMT
RUN set -eux; 	microdnf install -y 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Thu, 24 Mar 2022 02:12:27 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Thu, 24 Mar 2022 02:12:27 GMT
ENV MYSQL_MAJOR=8.0
# Thu, 24 Mar 2022 02:12:27 GMT
ENV MYSQL_VERSION=8.0.28-1.el8
# Thu, 24 Mar 2022 02:12:28 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Thu, 24 Mar 2022 02:12:53 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 		mysqld --version; 	mysql --version
# Thu, 24 Mar 2022 02:12:53 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Thu, 24 Mar 2022 02:12:53 GMT
ENV MYSQL_SHELL_VERSION=8.0.28-1.el8
# Thu, 24 Mar 2022 02:13:23 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Thu, 24 Mar 2022 02:13:24 GMT
VOLUME [/var/lib/mysql]
# Thu, 24 Mar 2022 02:13:24 GMT
COPY file:e9a583a365264f0f565259ffd0f19e5199ef4351d098f75af32f633c0d6cbe73 in /usr/local/bin/ 
# Thu, 24 Mar 2022 02:13:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 24 Mar 2022 02:13:24 GMT
EXPOSE 3306 33060
# Thu, 24 Mar 2022 02:13:24 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:a9d3d14d30b79ab021a558da3520be505bd2c5ab0f4c85aa07a3ed43524cea2f`  
		Last Modified: Thu, 24 Mar 2022 01:40:02 GMT  
		Size: 42.1 MB (42111482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51c34c1c3d334fb2ab9c8d9c0195c46a22a08dc4d53f5cd8260dfa8c9130527c`  
		Last Modified: Thu, 24 Mar 2022 02:13:59 GMT  
		Size: 1.1 KB (1081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6edd8203272bf73c540c0edcdca1c2668dba76d53fed2a0ab5e67da19b7afe8c`  
		Last Modified: Thu, 24 Mar 2022 02:13:58 GMT  
		Size: 928.8 KB (928836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e4579ce2fbc2e8b1f50e6db4baccf038f1339415e4e4f205b6525ac976c896d`  
		Last Modified: Thu, 24 Mar 2022 02:13:58 GMT  
		Size: 4.5 MB (4546975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29fbf1e34da756947373b1c081a452ca1bd648aee10625d68f255dfaa626c016`  
		Last Modified: Thu, 24 Mar 2022 02:13:57 GMT  
		Size: 2.6 KB (2628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44e1e95a4b5094db5db1154008980c898c0715849fbc8c4a5fc3dbed6073c2ef`  
		Last Modified: Thu, 24 Mar 2022 02:13:55 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0074abeebc046de5186ef3d222c170beb09629607dd93bfce85be128a9a07633`  
		Last Modified: Thu, 24 Mar 2022 02:14:03 GMT  
		Size: 47.3 MB (47267258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c727cb58a0450cb56a6d163e0b5418430e30f7c276592763809016e6f7e04f3e`  
		Last Modified: Thu, 24 Mar 2022 02:13:55 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91fb1a877d961ee9a8d5ee2171e6167ca917f03075cda3e6d49e11ce5bc06cba`  
		Last Modified: Thu, 24 Mar 2022 02:14:02 GMT  
		Size: 38.3 MB (38274331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:386346d38ca10d69f485b26793e5ba51e680934d8528ca250b7829a645a7d371`  
		Last Modified: Thu, 24 Mar 2022 02:13:55 GMT  
		Size: 5.1 KB (5145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8-oracle` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:e9b456391b4bb798292b6a959f0d3a992911fc1f9c21cb1bee563096d9015f6f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.2 MB (141172027 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13b353a72fcab60e6c13412fdafe5840a37e7dad38f5c36f7374eff8b8321151`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 18 Mar 2022 00:35:35 GMT
ADD file:b16af05882bd38ac02b1f1cba2cc7e80bfbe467ce57f3cf35f1f5a551cee90fa in / 
# Fri, 18 Mar 2022 00:35:36 GMT
CMD ["/bin/bash"]
# Sat, 19 Mar 2022 14:48:31 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql; 		mkdir /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d
# Sat, 19 Mar 2022 14:48:32 GMT
ENV GOSU_VERSION=1.14
# Sat, 19 Mar 2022 14:48:35 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 19 Mar 2022 14:49:02 GMT
RUN set -eux; 	microdnf install -y 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Sat, 19 Mar 2022 14:49:46 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Sat, 19 Mar 2022 14:49:47 GMT
ENV MYSQL_MAJOR=8.0
# Sat, 19 Mar 2022 14:49:48 GMT
ENV MYSQL_VERSION=8.0.28-1.el8
# Sat, 19 Mar 2022 14:49:49 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Sat, 19 Mar 2022 14:50:16 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 		mysqld --version; 	mysql --version
# Sat, 19 Mar 2022 14:50:16 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Sat, 19 Mar 2022 14:50:17 GMT
ENV MYSQL_SHELL_VERSION=8.0.28-1.el8
# Sat, 19 Mar 2022 14:50:46 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Sat, 19 Mar 2022 14:50:46 GMT
VOLUME [/var/lib/mysql]
# Sat, 19 Mar 2022 14:50:48 GMT
COPY file:e9a583a365264f0f565259ffd0f19e5199ef4351d098f75af32f633c0d6cbe73 in /usr/local/bin/ 
# Sat, 19 Mar 2022 14:50:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 19 Mar 2022 14:50:49 GMT
EXPOSE 3306 33060
# Sat, 19 Mar 2022 14:50:50 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:2f8e506fd7c6683f24250871efec36e3fe21cc71090a2f5c59dccdcdfeed2311`  
		Last Modified: Fri, 18 Mar 2022 00:36:38 GMT  
		Size: 42.0 MB (42017883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d2e303329ed7fcb9aeb4e6a5e5e8ff70c5ecaca6b4004efe7c5538f98ae073e`  
		Last Modified: Sat, 19 Mar 2022 14:51:14 GMT  
		Size: 1.0 KB (1014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e43a54926eb5a7901c559b6766eb23666ade02e931708faf2888edadac9e1851`  
		Last Modified: Sat, 19 Mar 2022 14:51:13 GMT  
		Size: 857.2 KB (857152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0039e24d8493013955f1061869d44fbdb472434d801986ac8140f0b1846bf4a`  
		Last Modified: Sat, 19 Mar 2022 14:51:12 GMT  
		Size: 4.4 MB (4376516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50d112a79f85ef077e50966e6ff296393952c4e854cabca838a2ae8ea52346dd`  
		Last Modified: Sat, 19 Mar 2022 14:51:12 GMT  
		Size: 2.6 KB (2610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a816874cae3d0e7af62a465c20b10528a92dedfae97f28912f66a1e05d2eb35`  
		Last Modified: Sat, 19 Mar 2022 14:51:10 GMT  
		Size: 336.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87cf3e7c1e5610eed17336f2c459440bddfc67726e3c7fb87fafa6d6b69621d5`  
		Last Modified: Sat, 19 Mar 2022 14:51:17 GMT  
		Size: 53.4 MB (53429849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebd2d8bfe6537a1ff984d2f0af8a1ca0efeb31774cec4a12f966f708d51cb479`  
		Last Modified: Sat, 19 Mar 2022 14:51:10 GMT  
		Size: 315.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:380e2f8b0a3606c651c20ab98460614d53fb50d4b9a9f7b33eff69eebc508ab1`  
		Last Modified: Sat, 19 Mar 2022 14:51:17 GMT  
		Size: 40.5 MB (40481210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b9d4712db09dae7f88b55a0497883dc40d43f805f6a22a8c289b92a5a6a5398`  
		Last Modified: Sat, 19 Mar 2022 14:51:10 GMT  
		Size: 5.1 KB (5142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
