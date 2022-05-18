## `mysql:oracle`

```console
$ docker pull mysql@sha256:2befebef0265220c2d6caed2599cd4fe6497c90408fc9f9925684ae26e92d769
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:oracle` - linux; amd64

```console
$ docker pull mysql@sha256:8141c03377ac2ad7853c98833d620015590d76caa5c17d1d7599ef26baf44da4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.6 MB (131645641 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28bb00bfe52a2aae96a7ab476f324e2c37fab25dd52dd86ff436331e067b4696`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 17 May 2022 22:41:42 GMT
ADD file:bbaf69bdffd0f506e447fbc52dca450a8966d950b8fa9aebd3a1bd5bd98f8b28 in / 
# Tue, 17 May 2022 22:41:42 GMT
CMD ["/bin/bash"]
# Tue, 17 May 2022 23:10:18 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql; 		mkdir /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d
# Tue, 17 May 2022 23:10:18 GMT
ENV GOSU_VERSION=1.14
# Tue, 17 May 2022 23:10:22 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 17 May 2022 23:10:42 GMT
RUN set -eux; 	microdnf install -y 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Tue, 17 May 2022 23:10:43 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Tue, 17 May 2022 23:10:43 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 17 May 2022 23:10:43 GMT
ENV MYSQL_VERSION=8.0.29-1.el8
# Tue, 17 May 2022 23:10:44 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Tue, 17 May 2022 23:11:10 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 		mysqld --version; 	mysql --version
# Tue, 17 May 2022 23:11:11 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Tue, 17 May 2022 23:11:11 GMT
ENV MYSQL_SHELL_VERSION=8.0.29-1.el8
# Tue, 17 May 2022 23:11:40 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Tue, 17 May 2022 23:11:40 GMT
VOLUME [/var/lib/mysql]
# Tue, 17 May 2022 23:11:40 GMT
COPY file:e9a583a365264f0f565259ffd0f19e5199ef4351d098f75af32f633c0d6cbe73 in /usr/local/bin/ 
# Tue, 17 May 2022 23:11:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 17 May 2022 23:11:41 GMT
EXPOSE 3306 33060
# Tue, 17 May 2022 23:11:41 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:90a00d516db16c568d3da8e0a7a5a78fa6fef5a39f3d688f831d254b77791565`  
		Last Modified: Tue, 17 May 2022 22:42:38 GMT  
		Size: 39.2 MB (39220501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec380701a2aab4173cf5a055f74c99227ae7c4fddf87803362ac984b3cbfa8ef`  
		Last Modified: Tue, 17 May 2022 23:12:28 GMT  
		Size: 1.1 KB (1080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c639d40d7782dd181799bc0e030b8269850fa3ad5bb3bbdeb511ea1c782e33c6`  
		Last Modified: Tue, 17 May 2022 23:12:26 GMT  
		Size: 928.8 KB (928834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ba2e5b74a30bdb2c55f39992bb2ae64d81e0b737541ad217123841bd41bda53`  
		Last Modified: Tue, 17 May 2022 23:12:26 GMT  
		Size: 4.5 MB (4536235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bce381d3796288927fc508cdc11bdca5a6c3d0dca64c13c2fc51035851ab296`  
		Last Modified: Tue, 17 May 2022 23:12:25 GMT  
		Size: 2.6 KB (2630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5e5b79d5c8e16d050f0a02cf0d1214f77e2a4e272b88299488b054d7c95f711`  
		Last Modified: Tue, 17 May 2022 23:12:23 GMT  
		Size: 337.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:858b3b51a1f97d5a72794a4cde78e9130b00620b922db41c2bc3ac79a55e8f58`  
		Last Modified: Tue, 17 May 2022 23:12:30 GMT  
		Size: 47.2 MB (47242274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2171f9f10a16c77335db5f61043051469c24c5080d9f80f87d5778f96b2bbc1c`  
		Last Modified: Tue, 17 May 2022 23:12:23 GMT  
		Size: 317.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f0fa78a73ac6ced6b681d9255b9345f3f8ab04aec0f08aa1fa0533dc37f055e`  
		Last Modified: Tue, 17 May 2022 23:12:31 GMT  
		Size: 39.7 MB (39708291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c240edbdbe67409f4ac9e83c9fc86c0cebf506ad3ebfd9d1ccdd29baa7a9e889`  
		Last Modified: Tue, 17 May 2022 23:12:23 GMT  
		Size: 5.1 KB (5142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:oracle` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:32019f5c8959fb725787a9873aeee9c28c8a4a054413e89263f37aa2007901c1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.6 MB (138552501 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e001f62601a11aea9a86873c2edf17d733c7a26cbd6d4ea0e05e0a73e9140e6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 17 May 2022 22:52:38 GMT
ADD file:263fe8ce0663428b324fa2909814084a77bf17118d772058d41546b804a4b968 in / 
# Tue, 17 May 2022 22:52:39 GMT
CMD ["/bin/bash"]
# Tue, 17 May 2022 23:09:01 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql; 		mkdir /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d
# Tue, 17 May 2022 23:09:02 GMT
ENV GOSU_VERSION=1.14
# Tue, 17 May 2022 23:09:05 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 17 May 2022 23:09:26 GMT
RUN set -eux; 	microdnf install -y 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Tue, 17 May 2022 23:09:28 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Tue, 17 May 2022 23:09:29 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 17 May 2022 23:09:30 GMT
ENV MYSQL_VERSION=8.0.29-1.el8
# Tue, 17 May 2022 23:09:31 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Tue, 17 May 2022 23:09:55 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 		mysqld --version; 	mysql --version
# Tue, 17 May 2022 23:09:55 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Tue, 17 May 2022 23:09:56 GMT
ENV MYSQL_SHELL_VERSION=8.0.29-1.el8
# Tue, 17 May 2022 23:10:23 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Tue, 17 May 2022 23:10:24 GMT
VOLUME [/var/lib/mysql]
# Tue, 17 May 2022 23:10:26 GMT
COPY file:e9a583a365264f0f565259ffd0f19e5199ef4351d098f75af32f633c0d6cbe73 in /usr/local/bin/ 
# Tue, 17 May 2022 23:10:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 17 May 2022 23:10:27 GMT
EXPOSE 3306 33060
# Tue, 17 May 2022 23:10:28 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:0dbddf5847a3e154a061766ddebe6a3cae471c97cabb3be2871f6d91f265d137`  
		Last Modified: Tue, 17 May 2022 22:53:43 GMT  
		Size: 38.0 MB (38012703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db29b0b5a771d422a5f85337ad705ae13b90861da7c4ae8a2d3020b42d0d4892`  
		Last Modified: Tue, 17 May 2022 23:10:58 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3855c850e40abd0de4601587237af854d07522e10e3bb9ee0e8c66b40ae49911`  
		Last Modified: Tue, 17 May 2022 23:10:56 GMT  
		Size: 857.2 KB (857152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a57b88152cf6fe699baa66b60fd8c2f07daef18b1931fae4dfc7c92d5d48ae5`  
		Last Modified: Tue, 17 May 2022 23:10:56 GMT  
		Size: 4.3 MB (4342967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ac9375febdd7998b9cc129e95d554b5b9d024f9ecf3053d3e7156a31279923f`  
		Last Modified: Tue, 17 May 2022 23:10:55 GMT  
		Size: 2.6 KB (2609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a199a4e720f0e82bafd1852cdf3a57870a449bcb60c197daf349869c4d332bb3`  
		Last Modified: Tue, 17 May 2022 23:10:53 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aebac76248d98ab600a56814d6569f0e4f4799aceb8bc8d8999f1b88938873e6`  
		Last Modified: Tue, 17 May 2022 23:11:00 GMT  
		Size: 53.3 MB (53299522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1b6eb52402d98a9e93f419ca2bc248862a3b2b7e0c0fc6800cadd1622dc46e9`  
		Last Modified: Tue, 17 May 2022 23:10:53 GMT  
		Size: 317.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ef5d943dd79edceeeeb858d6e3e80aa85a14a1f402e70156d2fd61d6e5f60a4`  
		Last Modified: Tue, 17 May 2022 23:11:01 GMT  
		Size: 42.0 MB (42030739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cd2e0c049de23bde6eb2d74d0ccebd69780e107d88608b72e6e229ea7c8bdf3`  
		Last Modified: Tue, 17 May 2022 23:10:53 GMT  
		Size: 5.1 KB (5142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
