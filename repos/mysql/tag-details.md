<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `mysql`

-	[`mysql:5`](#mysql5)
-	[`mysql:5-oracle`](#mysql5-oracle)
-	[`mysql:5.7`](#mysql57)
-	[`mysql:5.7-oracle`](#mysql57-oracle)
-	[`mysql:5.7.43`](#mysql5743)
-	[`mysql:5.7.43-oracle`](#mysql5743-oracle)
-	[`mysql:8`](#mysql8)
-	[`mysql:8-oracle`](#mysql8-oracle)
-	[`mysql:8.0`](#mysql80)
-	[`mysql:8.0-debian`](#mysql80-debian)
-	[`mysql:8.0-oracle`](#mysql80-oracle)
-	[`mysql:8.0.34`](#mysql8034)
-	[`mysql:8.0.34-debian`](#mysql8034-debian)
-	[`mysql:8.0.34-oracle`](#mysql8034-oracle)
-	[`mysql:8.1`](#mysql81)
-	[`mysql:8.1-oracle`](#mysql81-oracle)
-	[`mysql:8.1.0`](#mysql810)
-	[`mysql:8.1.0-oracle`](#mysql810-oracle)
-	[`mysql:innovation`](#mysqlinnovation)
-	[`mysql:innovation-oracle`](#mysqlinnovation-oracle)
-	[`mysql:latest`](#mysqllatest)
-	[`mysql:oracle`](#mysqloracle)

## `mysql:5`

```console
$ docker pull mysql@sha256:2eabad08824e3120dbec9096c276e3956e1922636c06fbb383ae9ea9c499bf43
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5` - linux; amd64

```console
$ docker pull mysql@sha256:8e044d43c8d38550dc1c935a0797f76adfa55024dd075f30161602395f99f0ca
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.2 MB (170232038 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d7b085374dbc1ca6ee83a18b488b9da0425749c87051e8bd8287dc2a2c775ecb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 14 Jun 2023 07:21:40 GMT
ADD file:733a37449d62d6e9f530185b9244e06cd8ff0ee896632576ae644437d0a1f852 in / 
# Wed, 14 Jun 2023 07:21:40 GMT
CMD ["/bin/bash"]
# Wed, 14 Jun 2023 09:53:50 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 14 Jun 2023 09:53:50 GMT
ENV GOSU_VERSION=1.16
# Wed, 14 Jun 2023 09:53:53 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 14 Jun 2023 09:54:11 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False oracle-epel-release-el7; 	yum install -y --setopt=skip_missing_names_on_install=False 		bzip2 		gzip 		openssl 		xz 		zstd 	; 	yum clean all
# Wed, 14 Jun 2023 09:54:12 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 14 Jun 2023 09:54:12 GMT
ENV MYSQL_MAJOR=5.7
# Wed, 14 Jun 2023 09:54:12 GMT
ENV MYSQL_VERSION=5.7.42-1.el7
# Wed, 14 Jun 2023 09:54:13 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql5.7-server-minimal]'; 		echo 'name=MySQL 5.7 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-5.7-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 14 Jun 2023 09:54:31 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-community-server-minimal-$MYSQL_VERSION"; 	yum clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	{ echo '!includedir /etc/mysql/mysql.conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/mysql.conf.d; 		find /etc/my.cnf /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/'; 		mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 14 Jun 2023 09:54:31 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Tue, 25 Jul 2023 01:39:21 GMT
ENV MYSQL_SHELL_VERSION=8.0.34-1.el7
# Tue, 25 Jul 2023 01:40:06 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-shell-$MYSQL_SHELL_VERSION"; 	yum clean all; 		mysqlsh --version
# Tue, 25 Jul 2023 01:40:07 GMT
VOLUME [/var/lib/mysql]
# Tue, 25 Jul 2023 01:40:07 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Tue, 25 Jul 2023 01:40:08 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 25 Jul 2023 01:40:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 25 Jul 2023 01:40:08 GMT
EXPOSE 3306 33060
# Tue, 25 Jul 2023 01:40:08 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:70e9ff4420fbc58483e68c13199a06c24b14013b2548998a7e367f59ca5157bc`  
		Last Modified: Wed, 14 Jun 2023 07:22:30 GMT  
		Size: 50.5 MB (50484765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ca4383b183f283dc0ac1a0351f5cb31f75dbd244bee8dc0988af4a50f2c59df`  
		Last Modified: Wed, 14 Jun 2023 09:55:49 GMT  
		Size: 872.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e282e7651b1612ff17f6246e0847dad6996add940329721a4756a1879f15a23`  
		Last Modified: Wed, 14 Jun 2023 09:55:49 GMT  
		Size: 983.7 KB (983711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ffa0e0ca7078cd2e1abcaa6847bc545576fd23586b4ae3ccc90b31637f27b1f`  
		Last Modified: Wed, 14 Jun 2023 09:55:48 GMT  
		Size: 4.6 MB (4601387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eb790cf638212f7a95cd187ed8515ff749c06d616bab23ee7ff4f87969533c7`  
		Last Modified: Wed, 14 Jun 2023 09:55:47 GMT  
		Size: 2.7 KB (2658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b7ffc37d8e9c1691a3e04e9fcdf2409484ca22e3b8a1b81e30c0b0ad85551df`  
		Last Modified: Wed, 14 Jun 2023 09:55:47 GMT  
		Size: 336.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4393c12228b9628c8d3a8c421e92080b206ee9445951e9119fce64d61a7fd143`  
		Last Modified: Wed, 14 Jun 2023 09:55:49 GMT  
		Size: 25.5 MB (25534088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:389d2c130d520b0e7953b08faa0ad308866e0cb139cd341ddc16501aac8cc3a7`  
		Last Modified: Wed, 14 Jun 2023 09:55:45 GMT  
		Size: 315.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed0e2667409210fd996b0c9d1f8b7beccfde55fb2333ab740933f16a68ea173c`  
		Last Modified: Tue, 25 Jul 2023 01:41:46 GMT  
		Size: 88.6 MB (88618392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8c72f236cd0004bebf358545db81bde2373557f98f40505c51874541f0ab662`  
		Last Modified: Tue, 25 Jul 2023 01:41:32 GMT  
		Size: 5.4 KB (5393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a9cda718bb791d96ab90baddec90d24fc434b63fe73f41658c096b7823c0c3e`  
		Last Modified: Tue, 25 Jul 2023 01:41:32 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5-oracle`

```console
$ docker pull mysql@sha256:2eabad08824e3120dbec9096c276e3956e1922636c06fbb383ae9ea9c499bf43
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:8e044d43c8d38550dc1c935a0797f76adfa55024dd075f30161602395f99f0ca
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.2 MB (170232038 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d7b085374dbc1ca6ee83a18b488b9da0425749c87051e8bd8287dc2a2c775ecb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 14 Jun 2023 07:21:40 GMT
ADD file:733a37449d62d6e9f530185b9244e06cd8ff0ee896632576ae644437d0a1f852 in / 
# Wed, 14 Jun 2023 07:21:40 GMT
CMD ["/bin/bash"]
# Wed, 14 Jun 2023 09:53:50 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 14 Jun 2023 09:53:50 GMT
ENV GOSU_VERSION=1.16
# Wed, 14 Jun 2023 09:53:53 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 14 Jun 2023 09:54:11 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False oracle-epel-release-el7; 	yum install -y --setopt=skip_missing_names_on_install=False 		bzip2 		gzip 		openssl 		xz 		zstd 	; 	yum clean all
# Wed, 14 Jun 2023 09:54:12 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 14 Jun 2023 09:54:12 GMT
ENV MYSQL_MAJOR=5.7
# Wed, 14 Jun 2023 09:54:12 GMT
ENV MYSQL_VERSION=5.7.42-1.el7
# Wed, 14 Jun 2023 09:54:13 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql5.7-server-minimal]'; 		echo 'name=MySQL 5.7 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-5.7-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 14 Jun 2023 09:54:31 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-community-server-minimal-$MYSQL_VERSION"; 	yum clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	{ echo '!includedir /etc/mysql/mysql.conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/mysql.conf.d; 		find /etc/my.cnf /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/'; 		mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 14 Jun 2023 09:54:31 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Tue, 25 Jul 2023 01:39:21 GMT
ENV MYSQL_SHELL_VERSION=8.0.34-1.el7
# Tue, 25 Jul 2023 01:40:06 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-shell-$MYSQL_SHELL_VERSION"; 	yum clean all; 		mysqlsh --version
# Tue, 25 Jul 2023 01:40:07 GMT
VOLUME [/var/lib/mysql]
# Tue, 25 Jul 2023 01:40:07 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Tue, 25 Jul 2023 01:40:08 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 25 Jul 2023 01:40:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 25 Jul 2023 01:40:08 GMT
EXPOSE 3306 33060
# Tue, 25 Jul 2023 01:40:08 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:70e9ff4420fbc58483e68c13199a06c24b14013b2548998a7e367f59ca5157bc`  
		Last Modified: Wed, 14 Jun 2023 07:22:30 GMT  
		Size: 50.5 MB (50484765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ca4383b183f283dc0ac1a0351f5cb31f75dbd244bee8dc0988af4a50f2c59df`  
		Last Modified: Wed, 14 Jun 2023 09:55:49 GMT  
		Size: 872.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e282e7651b1612ff17f6246e0847dad6996add940329721a4756a1879f15a23`  
		Last Modified: Wed, 14 Jun 2023 09:55:49 GMT  
		Size: 983.7 KB (983711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ffa0e0ca7078cd2e1abcaa6847bc545576fd23586b4ae3ccc90b31637f27b1f`  
		Last Modified: Wed, 14 Jun 2023 09:55:48 GMT  
		Size: 4.6 MB (4601387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eb790cf638212f7a95cd187ed8515ff749c06d616bab23ee7ff4f87969533c7`  
		Last Modified: Wed, 14 Jun 2023 09:55:47 GMT  
		Size: 2.7 KB (2658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b7ffc37d8e9c1691a3e04e9fcdf2409484ca22e3b8a1b81e30c0b0ad85551df`  
		Last Modified: Wed, 14 Jun 2023 09:55:47 GMT  
		Size: 336.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4393c12228b9628c8d3a8c421e92080b206ee9445951e9119fce64d61a7fd143`  
		Last Modified: Wed, 14 Jun 2023 09:55:49 GMT  
		Size: 25.5 MB (25534088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:389d2c130d520b0e7953b08faa0ad308866e0cb139cd341ddc16501aac8cc3a7`  
		Last Modified: Wed, 14 Jun 2023 09:55:45 GMT  
		Size: 315.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed0e2667409210fd996b0c9d1f8b7beccfde55fb2333ab740933f16a68ea173c`  
		Last Modified: Tue, 25 Jul 2023 01:41:46 GMT  
		Size: 88.6 MB (88618392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8c72f236cd0004bebf358545db81bde2373557f98f40505c51874541f0ab662`  
		Last Modified: Tue, 25 Jul 2023 01:41:32 GMT  
		Size: 5.4 KB (5393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a9cda718bb791d96ab90baddec90d24fc434b63fe73f41658c096b7823c0c3e`  
		Last Modified: Tue, 25 Jul 2023 01:41:32 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7`

```console
$ docker pull mysql@sha256:2eabad08824e3120dbec9096c276e3956e1922636c06fbb383ae9ea9c499bf43
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7` - linux; amd64

```console
$ docker pull mysql@sha256:8e044d43c8d38550dc1c935a0797f76adfa55024dd075f30161602395f99f0ca
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.2 MB (170232038 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d7b085374dbc1ca6ee83a18b488b9da0425749c87051e8bd8287dc2a2c775ecb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 14 Jun 2023 07:21:40 GMT
ADD file:733a37449d62d6e9f530185b9244e06cd8ff0ee896632576ae644437d0a1f852 in / 
# Wed, 14 Jun 2023 07:21:40 GMT
CMD ["/bin/bash"]
# Wed, 14 Jun 2023 09:53:50 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 14 Jun 2023 09:53:50 GMT
ENV GOSU_VERSION=1.16
# Wed, 14 Jun 2023 09:53:53 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 14 Jun 2023 09:54:11 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False oracle-epel-release-el7; 	yum install -y --setopt=skip_missing_names_on_install=False 		bzip2 		gzip 		openssl 		xz 		zstd 	; 	yum clean all
# Wed, 14 Jun 2023 09:54:12 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 14 Jun 2023 09:54:12 GMT
ENV MYSQL_MAJOR=5.7
# Wed, 14 Jun 2023 09:54:12 GMT
ENV MYSQL_VERSION=5.7.42-1.el7
# Wed, 14 Jun 2023 09:54:13 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql5.7-server-minimal]'; 		echo 'name=MySQL 5.7 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-5.7-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 14 Jun 2023 09:54:31 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-community-server-minimal-$MYSQL_VERSION"; 	yum clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	{ echo '!includedir /etc/mysql/mysql.conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/mysql.conf.d; 		find /etc/my.cnf /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/'; 		mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 14 Jun 2023 09:54:31 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Tue, 25 Jul 2023 01:39:21 GMT
ENV MYSQL_SHELL_VERSION=8.0.34-1.el7
# Tue, 25 Jul 2023 01:40:06 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-shell-$MYSQL_SHELL_VERSION"; 	yum clean all; 		mysqlsh --version
# Tue, 25 Jul 2023 01:40:07 GMT
VOLUME [/var/lib/mysql]
# Tue, 25 Jul 2023 01:40:07 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Tue, 25 Jul 2023 01:40:08 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 25 Jul 2023 01:40:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 25 Jul 2023 01:40:08 GMT
EXPOSE 3306 33060
# Tue, 25 Jul 2023 01:40:08 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:70e9ff4420fbc58483e68c13199a06c24b14013b2548998a7e367f59ca5157bc`  
		Last Modified: Wed, 14 Jun 2023 07:22:30 GMT  
		Size: 50.5 MB (50484765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ca4383b183f283dc0ac1a0351f5cb31f75dbd244bee8dc0988af4a50f2c59df`  
		Last Modified: Wed, 14 Jun 2023 09:55:49 GMT  
		Size: 872.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e282e7651b1612ff17f6246e0847dad6996add940329721a4756a1879f15a23`  
		Last Modified: Wed, 14 Jun 2023 09:55:49 GMT  
		Size: 983.7 KB (983711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ffa0e0ca7078cd2e1abcaa6847bc545576fd23586b4ae3ccc90b31637f27b1f`  
		Last Modified: Wed, 14 Jun 2023 09:55:48 GMT  
		Size: 4.6 MB (4601387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eb790cf638212f7a95cd187ed8515ff749c06d616bab23ee7ff4f87969533c7`  
		Last Modified: Wed, 14 Jun 2023 09:55:47 GMT  
		Size: 2.7 KB (2658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b7ffc37d8e9c1691a3e04e9fcdf2409484ca22e3b8a1b81e30c0b0ad85551df`  
		Last Modified: Wed, 14 Jun 2023 09:55:47 GMT  
		Size: 336.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4393c12228b9628c8d3a8c421e92080b206ee9445951e9119fce64d61a7fd143`  
		Last Modified: Wed, 14 Jun 2023 09:55:49 GMT  
		Size: 25.5 MB (25534088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:389d2c130d520b0e7953b08faa0ad308866e0cb139cd341ddc16501aac8cc3a7`  
		Last Modified: Wed, 14 Jun 2023 09:55:45 GMT  
		Size: 315.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed0e2667409210fd996b0c9d1f8b7beccfde55fb2333ab740933f16a68ea173c`  
		Last Modified: Tue, 25 Jul 2023 01:41:46 GMT  
		Size: 88.6 MB (88618392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8c72f236cd0004bebf358545db81bde2373557f98f40505c51874541f0ab662`  
		Last Modified: Tue, 25 Jul 2023 01:41:32 GMT  
		Size: 5.4 KB (5393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a9cda718bb791d96ab90baddec90d24fc434b63fe73f41658c096b7823c0c3e`  
		Last Modified: Tue, 25 Jul 2023 01:41:32 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7-oracle`

```console
$ docker pull mysql@sha256:2eabad08824e3120dbec9096c276e3956e1922636c06fbb383ae9ea9c499bf43
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:8e044d43c8d38550dc1c935a0797f76adfa55024dd075f30161602395f99f0ca
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.2 MB (170232038 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d7b085374dbc1ca6ee83a18b488b9da0425749c87051e8bd8287dc2a2c775ecb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 14 Jun 2023 07:21:40 GMT
ADD file:733a37449d62d6e9f530185b9244e06cd8ff0ee896632576ae644437d0a1f852 in / 
# Wed, 14 Jun 2023 07:21:40 GMT
CMD ["/bin/bash"]
# Wed, 14 Jun 2023 09:53:50 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 14 Jun 2023 09:53:50 GMT
ENV GOSU_VERSION=1.16
# Wed, 14 Jun 2023 09:53:53 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 14 Jun 2023 09:54:11 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False oracle-epel-release-el7; 	yum install -y --setopt=skip_missing_names_on_install=False 		bzip2 		gzip 		openssl 		xz 		zstd 	; 	yum clean all
# Wed, 14 Jun 2023 09:54:12 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 14 Jun 2023 09:54:12 GMT
ENV MYSQL_MAJOR=5.7
# Wed, 14 Jun 2023 09:54:12 GMT
ENV MYSQL_VERSION=5.7.42-1.el7
# Wed, 14 Jun 2023 09:54:13 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql5.7-server-minimal]'; 		echo 'name=MySQL 5.7 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-5.7-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 14 Jun 2023 09:54:31 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-community-server-minimal-$MYSQL_VERSION"; 	yum clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	{ echo '!includedir /etc/mysql/mysql.conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/mysql.conf.d; 		find /etc/my.cnf /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/'; 		mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 14 Jun 2023 09:54:31 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Tue, 25 Jul 2023 01:39:21 GMT
ENV MYSQL_SHELL_VERSION=8.0.34-1.el7
# Tue, 25 Jul 2023 01:40:06 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-shell-$MYSQL_SHELL_VERSION"; 	yum clean all; 		mysqlsh --version
# Tue, 25 Jul 2023 01:40:07 GMT
VOLUME [/var/lib/mysql]
# Tue, 25 Jul 2023 01:40:07 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Tue, 25 Jul 2023 01:40:08 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 25 Jul 2023 01:40:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 25 Jul 2023 01:40:08 GMT
EXPOSE 3306 33060
# Tue, 25 Jul 2023 01:40:08 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:70e9ff4420fbc58483e68c13199a06c24b14013b2548998a7e367f59ca5157bc`  
		Last Modified: Wed, 14 Jun 2023 07:22:30 GMT  
		Size: 50.5 MB (50484765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ca4383b183f283dc0ac1a0351f5cb31f75dbd244bee8dc0988af4a50f2c59df`  
		Last Modified: Wed, 14 Jun 2023 09:55:49 GMT  
		Size: 872.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e282e7651b1612ff17f6246e0847dad6996add940329721a4756a1879f15a23`  
		Last Modified: Wed, 14 Jun 2023 09:55:49 GMT  
		Size: 983.7 KB (983711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ffa0e0ca7078cd2e1abcaa6847bc545576fd23586b4ae3ccc90b31637f27b1f`  
		Last Modified: Wed, 14 Jun 2023 09:55:48 GMT  
		Size: 4.6 MB (4601387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eb790cf638212f7a95cd187ed8515ff749c06d616bab23ee7ff4f87969533c7`  
		Last Modified: Wed, 14 Jun 2023 09:55:47 GMT  
		Size: 2.7 KB (2658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b7ffc37d8e9c1691a3e04e9fcdf2409484ca22e3b8a1b81e30c0b0ad85551df`  
		Last Modified: Wed, 14 Jun 2023 09:55:47 GMT  
		Size: 336.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4393c12228b9628c8d3a8c421e92080b206ee9445951e9119fce64d61a7fd143`  
		Last Modified: Wed, 14 Jun 2023 09:55:49 GMT  
		Size: 25.5 MB (25534088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:389d2c130d520b0e7953b08faa0ad308866e0cb139cd341ddc16501aac8cc3a7`  
		Last Modified: Wed, 14 Jun 2023 09:55:45 GMT  
		Size: 315.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed0e2667409210fd996b0c9d1f8b7beccfde55fb2333ab740933f16a68ea173c`  
		Last Modified: Tue, 25 Jul 2023 01:41:46 GMT  
		Size: 88.6 MB (88618392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8c72f236cd0004bebf358545db81bde2373557f98f40505c51874541f0ab662`  
		Last Modified: Tue, 25 Jul 2023 01:41:32 GMT  
		Size: 5.4 KB (5393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a9cda718bb791d96ab90baddec90d24fc434b63fe73f41658c096b7823c0c3e`  
		Last Modified: Tue, 25 Jul 2023 01:41:32 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7.43`

**does not exist** (yet?)

## `mysql:5.7.43-oracle`

**does not exist** (yet?)

## `mysql:8`

```console
$ docker pull mysql@sha256:51c4dc55d3abf4517a5a652794d1f0adb2f2ed1d1bedc847d6132d91cdb2ebbf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8` - linux; amd64

```console
$ docker pull mysql@sha256:1da5cf22e7177925fa4d2a707936ca4ade59ba10b40b23550b0ffc12f8340600
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **166.5 MB (166515599 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c5ae0d3388cc6f2c72e73c8b1b9a7ba29347d9d7117d426b5cd83c3b71fe2b9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 22 Jul 2023 01:20:32 GMT
ADD file:6d43f7bf7c8d8c056e6fcc566ccfa2c1e42be1ef095f94d6780d0ca7d9a02e6e in / 
# Sat, 22 Jul 2023 01:20:32 GMT
CMD ["/bin/bash"]
# Sat, 22 Jul 2023 01:37:28 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Sat, 22 Jul 2023 01:37:28 GMT
ENV GOSU_VERSION=1.16
# Sat, 22 Jul 2023 01:37:31 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 22 Jul 2023 01:37:58 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Sat, 22 Jul 2023 01:37:59 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Sat, 22 Jul 2023 01:37:59 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 25 Jul 2023 01:37:33 GMT
ENV MYSQL_VERSION=8.0.34-1.el8
# Tue, 25 Jul 2023 01:37:34 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Tue, 25 Jul 2023 01:38:08 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Tue, 25 Jul 2023 01:38:09 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Tue, 25 Jul 2023 01:38:09 GMT
ENV MYSQL_SHELL_VERSION=8.0.34-1.el8
# Tue, 25 Jul 2023 01:38:47 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Tue, 25 Jul 2023 01:38:48 GMT
VOLUME [/var/lib/mysql]
# Tue, 25 Jul 2023 01:38:48 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Tue, 25 Jul 2023 01:38:49 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 25 Jul 2023 01:38:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 25 Jul 2023 01:38:49 GMT
EXPOSE 3306 33060
# Tue, 25 Jul 2023 01:38:49 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:49bb46380f8cb3491e82d000b27a6eb26b2490291da814ce3363bbf2c8baeb1a`  
		Last Modified: Sat, 22 Jul 2023 01:21:47 GMT  
		Size: 44.9 MB (44915006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aab3066bbf8fc576b01df1b0391e5a72a7ff72b1c0c5d09a7bab3db2a51d4744`  
		Last Modified: Sat, 22 Jul 2023 01:39:42 GMT  
		Size: 884.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6eef8c26cf9c633276ffd191110525157aa8811962fce9164a8a79814d497bd`  
		Last Modified: Sat, 22 Jul 2023 01:39:42 GMT  
		Size: 982.8 KB (982822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e908b1dcba2267120afc44b8f24aba3cdf060da1257257196b07f34edd7e959`  
		Last Modified: Sat, 22 Jul 2023 01:39:41 GMT  
		Size: 4.6 MB (4611560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:480c3912a2fde8647ba9e97d569e907841498684daa29bd86ba58710923b927d`  
		Last Modified: Sat, 22 Jul 2023 01:39:40 GMT  
		Size: 2.6 KB (2629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:264c20cd444959db4b636f22bb6179f597e3cce76a719c4b89883c5c3d32b6b8`  
		Last Modified: Tue, 25 Jul 2023 01:40:29 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7afa4443f21ca6852bc9df1ea4ee418cb2de2e110b97dcff63469fc800c3498`  
		Last Modified: Tue, 25 Jul 2023 01:40:35 GMT  
		Size: 58.5 MB (58493543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d32c26cb271e9bac9fd739bf78492fc8f831792aeb0d657ee2dc79304598bc21`  
		Last Modified: Tue, 25 Jul 2023 01:40:27 GMT  
		Size: 317.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1f84a2204cb8c481eeee7c56cd79502c7eb68dad75dbc0620dcd264a33e8bf3`  
		Last Modified: Tue, 25 Jul 2023 01:40:37 GMT  
		Size: 57.5 MB (57502986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a41fcc5b5085e66b65b1416c884e349f58d5f498431dde90f81c5df20f56d97`  
		Last Modified: Tue, 25 Jul 2023 01:40:27 GMT  
		Size: 5.4 KB (5392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b8402026abb7d3c430c0873c480f604e969fd6d8aef70552f5445c81bcc84fa`  
		Last Modified: Tue, 25 Jul 2023 01:40:27 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:c589deae89d660f907875ca7ac419f0704fc20f6d3825329b585ee2402b35101
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.1 MB (170071542 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2031a058d3ba2b2446da5464f0a29aea1008799bef06f24fd67bbc6743e53788`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 22 Jul 2023 01:03:33 GMT
ADD file:49b1f7f2b2558f78918f26b488622ad08fa607583d0a45f4f116773e2c13cf96 in / 
# Sat, 22 Jul 2023 01:03:34 GMT
CMD ["/bin/bash"]
# Sat, 22 Jul 2023 01:20:07 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Sat, 22 Jul 2023 01:20:07 GMT
ENV GOSU_VERSION=1.16
# Sat, 22 Jul 2023 01:20:11 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 22 Jul 2023 01:20:36 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Sat, 22 Jul 2023 01:20:37 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Sat, 22 Jul 2023 01:20:37 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 25 Jul 2023 01:42:38 GMT
ENV MYSQL_VERSION=8.0.34-1.el8
# Tue, 25 Jul 2023 01:42:39 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Tue, 25 Jul 2023 01:43:09 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Tue, 25 Jul 2023 01:43:10 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Tue, 25 Jul 2023 01:43:11 GMT
ENV MYSQL_SHELL_VERSION=8.0.34-1.el8
# Tue, 25 Jul 2023 01:43:45 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Tue, 25 Jul 2023 01:43:47 GMT
VOLUME [/var/lib/mysql]
# Tue, 25 Jul 2023 01:43:47 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Tue, 25 Jul 2023 01:43:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 25 Jul 2023 01:43:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 25 Jul 2023 01:43:47 GMT
EXPOSE 3306 33060
# Tue, 25 Jul 2023 01:43:47 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:1817bc1e6309503caf2242a5c83a4a6e9ebfdfb378d39bc92607690883a98c66`  
		Last Modified: Sat, 22 Jul 2023 01:04:31 GMT  
		Size: 43.6 MB (43623755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:740bd54462bcaa8cf5795022cb1daf5bf3b565d088fa1589e0e310225f2420d2`  
		Last Modified: Sat, 22 Jul 2023 01:22:13 GMT  
		Size: 886.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7e5ed4e69b309907018566aa973118702a7ad4f73cb732e4fb36fea862eaa26`  
		Last Modified: Sat, 22 Jul 2023 01:22:13 GMT  
		Size: 913.0 KB (912994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fdf88d7bbb7fa583fd2dfb4b80fa9ae42f0e8f228e3c15bdcf873dfadcaa445`  
		Last Modified: Sat, 22 Jul 2023 01:22:12 GMT  
		Size: 4.3 MB (4294535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1a5f85609500a34b3d4c06362e79700456581cfaf64335c617b36a10635033b`  
		Last Modified: Sat, 22 Jul 2023 01:22:11 GMT  
		Size: 2.6 KB (2631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d2014e71aa1dbbbd5d97f00faf0554b15d6660c42309369628b916d76b2cb14`  
		Last Modified: Tue, 25 Jul 2023 01:44:21 GMT  
		Size: 337.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a65eef3628981996acbf5281bc80aff6f958a7a95b309aa45c4c48103d895795`  
		Last Modified: Tue, 25 Jul 2023 01:44:25 GMT  
		Size: 57.5 MB (57465006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1086465c0f610a7ac25f9d953a2aae549cd70023e40ef1126dc6e92e31a1c842`  
		Last Modified: Tue, 25 Jul 2023 01:44:19 GMT  
		Size: 317.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d718a732c3abee1163a53974bcfdf72f17454a49c9d8998fba92c60851f175b`  
		Last Modified: Tue, 25 Jul 2023 01:44:27 GMT  
		Size: 63.8 MB (63765566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c724fd4b412f48fecb147fd4d9d377059bcfb971c79ffde2d6fd43bbdb0d1384`  
		Last Modified: Tue, 25 Jul 2023 01:44:19 GMT  
		Size: 5.4 KB (5394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74fcbdd515b315a3e4eadc554a90a0b48392758d0686ee5c0bbdc6f9e7af7e76`  
		Last Modified: Tue, 25 Jul 2023 01:44:19 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8-oracle`

```console
$ docker pull mysql@sha256:51c4dc55d3abf4517a5a652794d1f0adb2f2ed1d1bedc847d6132d91cdb2ebbf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:1da5cf22e7177925fa4d2a707936ca4ade59ba10b40b23550b0ffc12f8340600
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **166.5 MB (166515599 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c5ae0d3388cc6f2c72e73c8b1b9a7ba29347d9d7117d426b5cd83c3b71fe2b9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 22 Jul 2023 01:20:32 GMT
ADD file:6d43f7bf7c8d8c056e6fcc566ccfa2c1e42be1ef095f94d6780d0ca7d9a02e6e in / 
# Sat, 22 Jul 2023 01:20:32 GMT
CMD ["/bin/bash"]
# Sat, 22 Jul 2023 01:37:28 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Sat, 22 Jul 2023 01:37:28 GMT
ENV GOSU_VERSION=1.16
# Sat, 22 Jul 2023 01:37:31 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 22 Jul 2023 01:37:58 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Sat, 22 Jul 2023 01:37:59 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Sat, 22 Jul 2023 01:37:59 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 25 Jul 2023 01:37:33 GMT
ENV MYSQL_VERSION=8.0.34-1.el8
# Tue, 25 Jul 2023 01:37:34 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Tue, 25 Jul 2023 01:38:08 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Tue, 25 Jul 2023 01:38:09 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Tue, 25 Jul 2023 01:38:09 GMT
ENV MYSQL_SHELL_VERSION=8.0.34-1.el8
# Tue, 25 Jul 2023 01:38:47 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Tue, 25 Jul 2023 01:38:48 GMT
VOLUME [/var/lib/mysql]
# Tue, 25 Jul 2023 01:38:48 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Tue, 25 Jul 2023 01:38:49 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 25 Jul 2023 01:38:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 25 Jul 2023 01:38:49 GMT
EXPOSE 3306 33060
# Tue, 25 Jul 2023 01:38:49 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:49bb46380f8cb3491e82d000b27a6eb26b2490291da814ce3363bbf2c8baeb1a`  
		Last Modified: Sat, 22 Jul 2023 01:21:47 GMT  
		Size: 44.9 MB (44915006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aab3066bbf8fc576b01df1b0391e5a72a7ff72b1c0c5d09a7bab3db2a51d4744`  
		Last Modified: Sat, 22 Jul 2023 01:39:42 GMT  
		Size: 884.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6eef8c26cf9c633276ffd191110525157aa8811962fce9164a8a79814d497bd`  
		Last Modified: Sat, 22 Jul 2023 01:39:42 GMT  
		Size: 982.8 KB (982822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e908b1dcba2267120afc44b8f24aba3cdf060da1257257196b07f34edd7e959`  
		Last Modified: Sat, 22 Jul 2023 01:39:41 GMT  
		Size: 4.6 MB (4611560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:480c3912a2fde8647ba9e97d569e907841498684daa29bd86ba58710923b927d`  
		Last Modified: Sat, 22 Jul 2023 01:39:40 GMT  
		Size: 2.6 KB (2629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:264c20cd444959db4b636f22bb6179f597e3cce76a719c4b89883c5c3d32b6b8`  
		Last Modified: Tue, 25 Jul 2023 01:40:29 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7afa4443f21ca6852bc9df1ea4ee418cb2de2e110b97dcff63469fc800c3498`  
		Last Modified: Tue, 25 Jul 2023 01:40:35 GMT  
		Size: 58.5 MB (58493543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d32c26cb271e9bac9fd739bf78492fc8f831792aeb0d657ee2dc79304598bc21`  
		Last Modified: Tue, 25 Jul 2023 01:40:27 GMT  
		Size: 317.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1f84a2204cb8c481eeee7c56cd79502c7eb68dad75dbc0620dcd264a33e8bf3`  
		Last Modified: Tue, 25 Jul 2023 01:40:37 GMT  
		Size: 57.5 MB (57502986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a41fcc5b5085e66b65b1416c884e349f58d5f498431dde90f81c5df20f56d97`  
		Last Modified: Tue, 25 Jul 2023 01:40:27 GMT  
		Size: 5.4 KB (5392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b8402026abb7d3c430c0873c480f604e969fd6d8aef70552f5445c81bcc84fa`  
		Last Modified: Tue, 25 Jul 2023 01:40:27 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8-oracle` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:c589deae89d660f907875ca7ac419f0704fc20f6d3825329b585ee2402b35101
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.1 MB (170071542 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2031a058d3ba2b2446da5464f0a29aea1008799bef06f24fd67bbc6743e53788`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 22 Jul 2023 01:03:33 GMT
ADD file:49b1f7f2b2558f78918f26b488622ad08fa607583d0a45f4f116773e2c13cf96 in / 
# Sat, 22 Jul 2023 01:03:34 GMT
CMD ["/bin/bash"]
# Sat, 22 Jul 2023 01:20:07 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Sat, 22 Jul 2023 01:20:07 GMT
ENV GOSU_VERSION=1.16
# Sat, 22 Jul 2023 01:20:11 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 22 Jul 2023 01:20:36 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Sat, 22 Jul 2023 01:20:37 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Sat, 22 Jul 2023 01:20:37 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 25 Jul 2023 01:42:38 GMT
ENV MYSQL_VERSION=8.0.34-1.el8
# Tue, 25 Jul 2023 01:42:39 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Tue, 25 Jul 2023 01:43:09 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Tue, 25 Jul 2023 01:43:10 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Tue, 25 Jul 2023 01:43:11 GMT
ENV MYSQL_SHELL_VERSION=8.0.34-1.el8
# Tue, 25 Jul 2023 01:43:45 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Tue, 25 Jul 2023 01:43:47 GMT
VOLUME [/var/lib/mysql]
# Tue, 25 Jul 2023 01:43:47 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Tue, 25 Jul 2023 01:43:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 25 Jul 2023 01:43:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 25 Jul 2023 01:43:47 GMT
EXPOSE 3306 33060
# Tue, 25 Jul 2023 01:43:47 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:1817bc1e6309503caf2242a5c83a4a6e9ebfdfb378d39bc92607690883a98c66`  
		Last Modified: Sat, 22 Jul 2023 01:04:31 GMT  
		Size: 43.6 MB (43623755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:740bd54462bcaa8cf5795022cb1daf5bf3b565d088fa1589e0e310225f2420d2`  
		Last Modified: Sat, 22 Jul 2023 01:22:13 GMT  
		Size: 886.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7e5ed4e69b309907018566aa973118702a7ad4f73cb732e4fb36fea862eaa26`  
		Last Modified: Sat, 22 Jul 2023 01:22:13 GMT  
		Size: 913.0 KB (912994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fdf88d7bbb7fa583fd2dfb4b80fa9ae42f0e8f228e3c15bdcf873dfadcaa445`  
		Last Modified: Sat, 22 Jul 2023 01:22:12 GMT  
		Size: 4.3 MB (4294535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1a5f85609500a34b3d4c06362e79700456581cfaf64335c617b36a10635033b`  
		Last Modified: Sat, 22 Jul 2023 01:22:11 GMT  
		Size: 2.6 KB (2631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d2014e71aa1dbbbd5d97f00faf0554b15d6660c42309369628b916d76b2cb14`  
		Last Modified: Tue, 25 Jul 2023 01:44:21 GMT  
		Size: 337.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a65eef3628981996acbf5281bc80aff6f958a7a95b309aa45c4c48103d895795`  
		Last Modified: Tue, 25 Jul 2023 01:44:25 GMT  
		Size: 57.5 MB (57465006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1086465c0f610a7ac25f9d953a2aae549cd70023e40ef1126dc6e92e31a1c842`  
		Last Modified: Tue, 25 Jul 2023 01:44:19 GMT  
		Size: 317.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d718a732c3abee1163a53974bcfdf72f17454a49c9d8998fba92c60851f175b`  
		Last Modified: Tue, 25 Jul 2023 01:44:27 GMT  
		Size: 63.8 MB (63765566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c724fd4b412f48fecb147fd4d9d377059bcfb971c79ffde2d6fd43bbdb0d1384`  
		Last Modified: Tue, 25 Jul 2023 01:44:19 GMT  
		Size: 5.4 KB (5394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74fcbdd515b315a3e4eadc554a90a0b48392758d0686ee5c0bbdc6f9e7af7e76`  
		Last Modified: Tue, 25 Jul 2023 01:44:19 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0`

```console
$ docker pull mysql@sha256:51c4dc55d3abf4517a5a652794d1f0adb2f2ed1d1bedc847d6132d91cdb2ebbf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8.0` - linux; amd64

```console
$ docker pull mysql@sha256:1da5cf22e7177925fa4d2a707936ca4ade59ba10b40b23550b0ffc12f8340600
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **166.5 MB (166515599 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c5ae0d3388cc6f2c72e73c8b1b9a7ba29347d9d7117d426b5cd83c3b71fe2b9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 22 Jul 2023 01:20:32 GMT
ADD file:6d43f7bf7c8d8c056e6fcc566ccfa2c1e42be1ef095f94d6780d0ca7d9a02e6e in / 
# Sat, 22 Jul 2023 01:20:32 GMT
CMD ["/bin/bash"]
# Sat, 22 Jul 2023 01:37:28 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Sat, 22 Jul 2023 01:37:28 GMT
ENV GOSU_VERSION=1.16
# Sat, 22 Jul 2023 01:37:31 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 22 Jul 2023 01:37:58 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Sat, 22 Jul 2023 01:37:59 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Sat, 22 Jul 2023 01:37:59 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 25 Jul 2023 01:37:33 GMT
ENV MYSQL_VERSION=8.0.34-1.el8
# Tue, 25 Jul 2023 01:37:34 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Tue, 25 Jul 2023 01:38:08 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Tue, 25 Jul 2023 01:38:09 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Tue, 25 Jul 2023 01:38:09 GMT
ENV MYSQL_SHELL_VERSION=8.0.34-1.el8
# Tue, 25 Jul 2023 01:38:47 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Tue, 25 Jul 2023 01:38:48 GMT
VOLUME [/var/lib/mysql]
# Tue, 25 Jul 2023 01:38:48 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Tue, 25 Jul 2023 01:38:49 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 25 Jul 2023 01:38:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 25 Jul 2023 01:38:49 GMT
EXPOSE 3306 33060
# Tue, 25 Jul 2023 01:38:49 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:49bb46380f8cb3491e82d000b27a6eb26b2490291da814ce3363bbf2c8baeb1a`  
		Last Modified: Sat, 22 Jul 2023 01:21:47 GMT  
		Size: 44.9 MB (44915006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aab3066bbf8fc576b01df1b0391e5a72a7ff72b1c0c5d09a7bab3db2a51d4744`  
		Last Modified: Sat, 22 Jul 2023 01:39:42 GMT  
		Size: 884.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6eef8c26cf9c633276ffd191110525157aa8811962fce9164a8a79814d497bd`  
		Last Modified: Sat, 22 Jul 2023 01:39:42 GMT  
		Size: 982.8 KB (982822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e908b1dcba2267120afc44b8f24aba3cdf060da1257257196b07f34edd7e959`  
		Last Modified: Sat, 22 Jul 2023 01:39:41 GMT  
		Size: 4.6 MB (4611560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:480c3912a2fde8647ba9e97d569e907841498684daa29bd86ba58710923b927d`  
		Last Modified: Sat, 22 Jul 2023 01:39:40 GMT  
		Size: 2.6 KB (2629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:264c20cd444959db4b636f22bb6179f597e3cce76a719c4b89883c5c3d32b6b8`  
		Last Modified: Tue, 25 Jul 2023 01:40:29 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7afa4443f21ca6852bc9df1ea4ee418cb2de2e110b97dcff63469fc800c3498`  
		Last Modified: Tue, 25 Jul 2023 01:40:35 GMT  
		Size: 58.5 MB (58493543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d32c26cb271e9bac9fd739bf78492fc8f831792aeb0d657ee2dc79304598bc21`  
		Last Modified: Tue, 25 Jul 2023 01:40:27 GMT  
		Size: 317.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1f84a2204cb8c481eeee7c56cd79502c7eb68dad75dbc0620dcd264a33e8bf3`  
		Last Modified: Tue, 25 Jul 2023 01:40:37 GMT  
		Size: 57.5 MB (57502986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a41fcc5b5085e66b65b1416c884e349f58d5f498431dde90f81c5df20f56d97`  
		Last Modified: Tue, 25 Jul 2023 01:40:27 GMT  
		Size: 5.4 KB (5392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b8402026abb7d3c430c0873c480f604e969fd6d8aef70552f5445c81bcc84fa`  
		Last Modified: Tue, 25 Jul 2023 01:40:27 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8.0` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:c589deae89d660f907875ca7ac419f0704fc20f6d3825329b585ee2402b35101
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.1 MB (170071542 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2031a058d3ba2b2446da5464f0a29aea1008799bef06f24fd67bbc6743e53788`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 22 Jul 2023 01:03:33 GMT
ADD file:49b1f7f2b2558f78918f26b488622ad08fa607583d0a45f4f116773e2c13cf96 in / 
# Sat, 22 Jul 2023 01:03:34 GMT
CMD ["/bin/bash"]
# Sat, 22 Jul 2023 01:20:07 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Sat, 22 Jul 2023 01:20:07 GMT
ENV GOSU_VERSION=1.16
# Sat, 22 Jul 2023 01:20:11 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 22 Jul 2023 01:20:36 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Sat, 22 Jul 2023 01:20:37 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Sat, 22 Jul 2023 01:20:37 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 25 Jul 2023 01:42:38 GMT
ENV MYSQL_VERSION=8.0.34-1.el8
# Tue, 25 Jul 2023 01:42:39 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Tue, 25 Jul 2023 01:43:09 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Tue, 25 Jul 2023 01:43:10 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Tue, 25 Jul 2023 01:43:11 GMT
ENV MYSQL_SHELL_VERSION=8.0.34-1.el8
# Tue, 25 Jul 2023 01:43:45 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Tue, 25 Jul 2023 01:43:47 GMT
VOLUME [/var/lib/mysql]
# Tue, 25 Jul 2023 01:43:47 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Tue, 25 Jul 2023 01:43:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 25 Jul 2023 01:43:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 25 Jul 2023 01:43:47 GMT
EXPOSE 3306 33060
# Tue, 25 Jul 2023 01:43:47 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:1817bc1e6309503caf2242a5c83a4a6e9ebfdfb378d39bc92607690883a98c66`  
		Last Modified: Sat, 22 Jul 2023 01:04:31 GMT  
		Size: 43.6 MB (43623755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:740bd54462bcaa8cf5795022cb1daf5bf3b565d088fa1589e0e310225f2420d2`  
		Last Modified: Sat, 22 Jul 2023 01:22:13 GMT  
		Size: 886.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7e5ed4e69b309907018566aa973118702a7ad4f73cb732e4fb36fea862eaa26`  
		Last Modified: Sat, 22 Jul 2023 01:22:13 GMT  
		Size: 913.0 KB (912994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fdf88d7bbb7fa583fd2dfb4b80fa9ae42f0e8f228e3c15bdcf873dfadcaa445`  
		Last Modified: Sat, 22 Jul 2023 01:22:12 GMT  
		Size: 4.3 MB (4294535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1a5f85609500a34b3d4c06362e79700456581cfaf64335c617b36a10635033b`  
		Last Modified: Sat, 22 Jul 2023 01:22:11 GMT  
		Size: 2.6 KB (2631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d2014e71aa1dbbbd5d97f00faf0554b15d6660c42309369628b916d76b2cb14`  
		Last Modified: Tue, 25 Jul 2023 01:44:21 GMT  
		Size: 337.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a65eef3628981996acbf5281bc80aff6f958a7a95b309aa45c4c48103d895795`  
		Last Modified: Tue, 25 Jul 2023 01:44:25 GMT  
		Size: 57.5 MB (57465006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1086465c0f610a7ac25f9d953a2aae549cd70023e40ef1126dc6e92e31a1c842`  
		Last Modified: Tue, 25 Jul 2023 01:44:19 GMT  
		Size: 317.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d718a732c3abee1163a53974bcfdf72f17454a49c9d8998fba92c60851f175b`  
		Last Modified: Tue, 25 Jul 2023 01:44:27 GMT  
		Size: 63.8 MB (63765566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c724fd4b412f48fecb147fd4d9d377059bcfb971c79ffde2d6fd43bbdb0d1384`  
		Last Modified: Tue, 25 Jul 2023 01:44:19 GMT  
		Size: 5.4 KB (5394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74fcbdd515b315a3e4eadc554a90a0b48392758d0686ee5c0bbdc6f9e7af7e76`  
		Last Modified: Tue, 25 Jul 2023 01:44:19 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0-debian`

```console
$ docker pull mysql@sha256:49f4fcb0087318aa1c222c7e8ceacbb541cdc457c6307d45e6ee4313f4902e33
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:8.0-debian` - linux; amd64

```console
$ docker pull mysql@sha256:26db38c917a651edd01fc69bb56b8e068397a1ca4dfef9739cecc61f3111e6b4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **179.5 MB (179509315 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:992367f7e447afa8958f0b52f60a32bf01362731ac144922e319c26d5bade895`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 27 Jul 2023 23:25:07 GMT
ADD file:3d726bf0abbc08d6dda026cc406cdfb529deb60071641d164de28fcd62d1c1c0 in / 
# Thu, 27 Jul 2023 23:25:07 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 04:00:21 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 28 Jul 2023 04:00:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg && rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 04:00:26 GMT
ENV GOSU_VERSION=1.16
# Fri, 28 Jul 2023 04:00:35 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 28 Jul 2023 04:00:35 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 28 Jul 2023 04:00:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 04:00:41 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Fri, 28 Jul 2023 04:00:41 GMT
ENV MYSQL_MAJOR=8.0
# Fri, 28 Jul 2023 04:00:41 GMT
ENV MYSQL_VERSION=8.0.34-1debian11
# Fri, 28 Jul 2023 04:00:42 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ bullseye mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Fri, 28 Jul 2023 04:00:56 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Fri, 28 Jul 2023 04:00:57 GMT
VOLUME [/var/lib/mysql]
# Fri, 28 Jul 2023 04:00:57 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Fri, 28 Jul 2023 04:00:57 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Fri, 28 Jul 2023 04:00:57 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 28 Jul 2023 04:00:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 28 Jul 2023 04:00:58 GMT
EXPOSE 3306 33060
# Fri, 28 Jul 2023 04:00:58 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:1d5252f66ea9b661aceca1027b3d7ca259a50608261a25b51148119ecf086932`  
		Last Modified: Thu, 27 Jul 2023 23:30:08 GMT  
		Size: 31.4 MB (31417602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b034716887fd3351d90a2dadd53aa4984cd39f8397149d2fde665822cbdfb285`  
		Last Modified: Fri, 28 Jul 2023 04:02:17 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:882448c7d618dde8cedcebbf5843a1abdc3f8840035073f44ac0be1c75a88222`  
		Last Modified: Fri, 28 Jul 2023 04:02:17 GMT  
		Size: 4.4 MB (4415051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c14ac4640b87d832c2419b4c3968a4718ab31ef1cec549b8415be42ebb792611`  
		Last Modified: Fri, 28 Jul 2023 04:02:15 GMT  
		Size: 1.5 MB (1471510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d2978613e401218d6fd28693e6d47c7110dd5d4bd2f750ee1d37fc4f8428fd9`  
		Last Modified: Fri, 28 Jul 2023 04:02:15 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c33d24cb8c756b450de2635eb9fba6c9647da56ab1945e6c2b4e3926725ac3de`  
		Last Modified: Fri, 28 Jul 2023 04:02:17 GMT  
		Size: 12.7 MB (12662071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52fa14fc88fc63d64bb0d429a08bdaaae8f80694ad373b7c85e566d535fc88e5`  
		Last Modified: Fri, 28 Jul 2023 04:02:14 GMT  
		Size: 2.5 KB (2549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42deb22ec16d8d602e97596083fd18c35167815a0af24879dfd937d052bf72be`  
		Last Modified: Fri, 28 Jul 2023 04:02:13 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3d31d600a65d21a8dcd2963f131d5a412a1b257f8b7ede1896a939929cc24e6`  
		Last Modified: Fri, 28 Jul 2023 04:02:30 GMT  
		Size: 129.5 MB (129532040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0b9f5aba00d7eab19f55c9f54637f274c1275e6a8f33508b24dc332c4334e07`  
		Last Modified: Fri, 28 Jul 2023 04:02:13 GMT  
		Size: 843.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98222a66de151bb3ad1b199d0398af90a4552e2515f3bd52663e7df2c56b72a7`  
		Last Modified: Fri, 28 Jul 2023 04:02:12 GMT  
		Size: 5.4 KB (5391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ff8f0c3c67bc36e46203bc2fb68ed8023121c5f4b607ddd8d8ff48c01384452`  
		Last Modified: Fri, 28 Jul 2023 04:02:13 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0-oracle`

```console
$ docker pull mysql@sha256:51c4dc55d3abf4517a5a652794d1f0adb2f2ed1d1bedc847d6132d91cdb2ebbf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8.0-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:1da5cf22e7177925fa4d2a707936ca4ade59ba10b40b23550b0ffc12f8340600
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **166.5 MB (166515599 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c5ae0d3388cc6f2c72e73c8b1b9a7ba29347d9d7117d426b5cd83c3b71fe2b9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 22 Jul 2023 01:20:32 GMT
ADD file:6d43f7bf7c8d8c056e6fcc566ccfa2c1e42be1ef095f94d6780d0ca7d9a02e6e in / 
# Sat, 22 Jul 2023 01:20:32 GMT
CMD ["/bin/bash"]
# Sat, 22 Jul 2023 01:37:28 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Sat, 22 Jul 2023 01:37:28 GMT
ENV GOSU_VERSION=1.16
# Sat, 22 Jul 2023 01:37:31 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 22 Jul 2023 01:37:58 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Sat, 22 Jul 2023 01:37:59 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Sat, 22 Jul 2023 01:37:59 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 25 Jul 2023 01:37:33 GMT
ENV MYSQL_VERSION=8.0.34-1.el8
# Tue, 25 Jul 2023 01:37:34 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Tue, 25 Jul 2023 01:38:08 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Tue, 25 Jul 2023 01:38:09 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Tue, 25 Jul 2023 01:38:09 GMT
ENV MYSQL_SHELL_VERSION=8.0.34-1.el8
# Tue, 25 Jul 2023 01:38:47 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Tue, 25 Jul 2023 01:38:48 GMT
VOLUME [/var/lib/mysql]
# Tue, 25 Jul 2023 01:38:48 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Tue, 25 Jul 2023 01:38:49 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 25 Jul 2023 01:38:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 25 Jul 2023 01:38:49 GMT
EXPOSE 3306 33060
# Tue, 25 Jul 2023 01:38:49 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:49bb46380f8cb3491e82d000b27a6eb26b2490291da814ce3363bbf2c8baeb1a`  
		Last Modified: Sat, 22 Jul 2023 01:21:47 GMT  
		Size: 44.9 MB (44915006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aab3066bbf8fc576b01df1b0391e5a72a7ff72b1c0c5d09a7bab3db2a51d4744`  
		Last Modified: Sat, 22 Jul 2023 01:39:42 GMT  
		Size: 884.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6eef8c26cf9c633276ffd191110525157aa8811962fce9164a8a79814d497bd`  
		Last Modified: Sat, 22 Jul 2023 01:39:42 GMT  
		Size: 982.8 KB (982822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e908b1dcba2267120afc44b8f24aba3cdf060da1257257196b07f34edd7e959`  
		Last Modified: Sat, 22 Jul 2023 01:39:41 GMT  
		Size: 4.6 MB (4611560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:480c3912a2fde8647ba9e97d569e907841498684daa29bd86ba58710923b927d`  
		Last Modified: Sat, 22 Jul 2023 01:39:40 GMT  
		Size: 2.6 KB (2629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:264c20cd444959db4b636f22bb6179f597e3cce76a719c4b89883c5c3d32b6b8`  
		Last Modified: Tue, 25 Jul 2023 01:40:29 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7afa4443f21ca6852bc9df1ea4ee418cb2de2e110b97dcff63469fc800c3498`  
		Last Modified: Tue, 25 Jul 2023 01:40:35 GMT  
		Size: 58.5 MB (58493543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d32c26cb271e9bac9fd739bf78492fc8f831792aeb0d657ee2dc79304598bc21`  
		Last Modified: Tue, 25 Jul 2023 01:40:27 GMT  
		Size: 317.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1f84a2204cb8c481eeee7c56cd79502c7eb68dad75dbc0620dcd264a33e8bf3`  
		Last Modified: Tue, 25 Jul 2023 01:40:37 GMT  
		Size: 57.5 MB (57502986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a41fcc5b5085e66b65b1416c884e349f58d5f498431dde90f81c5df20f56d97`  
		Last Modified: Tue, 25 Jul 2023 01:40:27 GMT  
		Size: 5.4 KB (5392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b8402026abb7d3c430c0873c480f604e969fd6d8aef70552f5445c81bcc84fa`  
		Last Modified: Tue, 25 Jul 2023 01:40:27 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8.0-oracle` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:c589deae89d660f907875ca7ac419f0704fc20f6d3825329b585ee2402b35101
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.1 MB (170071542 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2031a058d3ba2b2446da5464f0a29aea1008799bef06f24fd67bbc6743e53788`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 22 Jul 2023 01:03:33 GMT
ADD file:49b1f7f2b2558f78918f26b488622ad08fa607583d0a45f4f116773e2c13cf96 in / 
# Sat, 22 Jul 2023 01:03:34 GMT
CMD ["/bin/bash"]
# Sat, 22 Jul 2023 01:20:07 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Sat, 22 Jul 2023 01:20:07 GMT
ENV GOSU_VERSION=1.16
# Sat, 22 Jul 2023 01:20:11 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 22 Jul 2023 01:20:36 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Sat, 22 Jul 2023 01:20:37 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Sat, 22 Jul 2023 01:20:37 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 25 Jul 2023 01:42:38 GMT
ENV MYSQL_VERSION=8.0.34-1.el8
# Tue, 25 Jul 2023 01:42:39 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Tue, 25 Jul 2023 01:43:09 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Tue, 25 Jul 2023 01:43:10 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Tue, 25 Jul 2023 01:43:11 GMT
ENV MYSQL_SHELL_VERSION=8.0.34-1.el8
# Tue, 25 Jul 2023 01:43:45 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Tue, 25 Jul 2023 01:43:47 GMT
VOLUME [/var/lib/mysql]
# Tue, 25 Jul 2023 01:43:47 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Tue, 25 Jul 2023 01:43:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 25 Jul 2023 01:43:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 25 Jul 2023 01:43:47 GMT
EXPOSE 3306 33060
# Tue, 25 Jul 2023 01:43:47 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:1817bc1e6309503caf2242a5c83a4a6e9ebfdfb378d39bc92607690883a98c66`  
		Last Modified: Sat, 22 Jul 2023 01:04:31 GMT  
		Size: 43.6 MB (43623755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:740bd54462bcaa8cf5795022cb1daf5bf3b565d088fa1589e0e310225f2420d2`  
		Last Modified: Sat, 22 Jul 2023 01:22:13 GMT  
		Size: 886.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7e5ed4e69b309907018566aa973118702a7ad4f73cb732e4fb36fea862eaa26`  
		Last Modified: Sat, 22 Jul 2023 01:22:13 GMT  
		Size: 913.0 KB (912994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fdf88d7bbb7fa583fd2dfb4b80fa9ae42f0e8f228e3c15bdcf873dfadcaa445`  
		Last Modified: Sat, 22 Jul 2023 01:22:12 GMT  
		Size: 4.3 MB (4294535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1a5f85609500a34b3d4c06362e79700456581cfaf64335c617b36a10635033b`  
		Last Modified: Sat, 22 Jul 2023 01:22:11 GMT  
		Size: 2.6 KB (2631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d2014e71aa1dbbbd5d97f00faf0554b15d6660c42309369628b916d76b2cb14`  
		Last Modified: Tue, 25 Jul 2023 01:44:21 GMT  
		Size: 337.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a65eef3628981996acbf5281bc80aff6f958a7a95b309aa45c4c48103d895795`  
		Last Modified: Tue, 25 Jul 2023 01:44:25 GMT  
		Size: 57.5 MB (57465006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1086465c0f610a7ac25f9d953a2aae549cd70023e40ef1126dc6e92e31a1c842`  
		Last Modified: Tue, 25 Jul 2023 01:44:19 GMT  
		Size: 317.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d718a732c3abee1163a53974bcfdf72f17454a49c9d8998fba92c60851f175b`  
		Last Modified: Tue, 25 Jul 2023 01:44:27 GMT  
		Size: 63.8 MB (63765566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c724fd4b412f48fecb147fd4d9d377059bcfb971c79ffde2d6fd43bbdb0d1384`  
		Last Modified: Tue, 25 Jul 2023 01:44:19 GMT  
		Size: 5.4 KB (5394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74fcbdd515b315a3e4eadc554a90a0b48392758d0686ee5c0bbdc6f9e7af7e76`  
		Last Modified: Tue, 25 Jul 2023 01:44:19 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0.34`

```console
$ docker pull mysql@sha256:51c4dc55d3abf4517a5a652794d1f0adb2f2ed1d1bedc847d6132d91cdb2ebbf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8.0.34` - linux; amd64

```console
$ docker pull mysql@sha256:1da5cf22e7177925fa4d2a707936ca4ade59ba10b40b23550b0ffc12f8340600
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **166.5 MB (166515599 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c5ae0d3388cc6f2c72e73c8b1b9a7ba29347d9d7117d426b5cd83c3b71fe2b9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 22 Jul 2023 01:20:32 GMT
ADD file:6d43f7bf7c8d8c056e6fcc566ccfa2c1e42be1ef095f94d6780d0ca7d9a02e6e in / 
# Sat, 22 Jul 2023 01:20:32 GMT
CMD ["/bin/bash"]
# Sat, 22 Jul 2023 01:37:28 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Sat, 22 Jul 2023 01:37:28 GMT
ENV GOSU_VERSION=1.16
# Sat, 22 Jul 2023 01:37:31 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 22 Jul 2023 01:37:58 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Sat, 22 Jul 2023 01:37:59 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Sat, 22 Jul 2023 01:37:59 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 25 Jul 2023 01:37:33 GMT
ENV MYSQL_VERSION=8.0.34-1.el8
# Tue, 25 Jul 2023 01:37:34 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Tue, 25 Jul 2023 01:38:08 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Tue, 25 Jul 2023 01:38:09 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Tue, 25 Jul 2023 01:38:09 GMT
ENV MYSQL_SHELL_VERSION=8.0.34-1.el8
# Tue, 25 Jul 2023 01:38:47 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Tue, 25 Jul 2023 01:38:48 GMT
VOLUME [/var/lib/mysql]
# Tue, 25 Jul 2023 01:38:48 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Tue, 25 Jul 2023 01:38:49 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 25 Jul 2023 01:38:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 25 Jul 2023 01:38:49 GMT
EXPOSE 3306 33060
# Tue, 25 Jul 2023 01:38:49 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:49bb46380f8cb3491e82d000b27a6eb26b2490291da814ce3363bbf2c8baeb1a`  
		Last Modified: Sat, 22 Jul 2023 01:21:47 GMT  
		Size: 44.9 MB (44915006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aab3066bbf8fc576b01df1b0391e5a72a7ff72b1c0c5d09a7bab3db2a51d4744`  
		Last Modified: Sat, 22 Jul 2023 01:39:42 GMT  
		Size: 884.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6eef8c26cf9c633276ffd191110525157aa8811962fce9164a8a79814d497bd`  
		Last Modified: Sat, 22 Jul 2023 01:39:42 GMT  
		Size: 982.8 KB (982822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e908b1dcba2267120afc44b8f24aba3cdf060da1257257196b07f34edd7e959`  
		Last Modified: Sat, 22 Jul 2023 01:39:41 GMT  
		Size: 4.6 MB (4611560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:480c3912a2fde8647ba9e97d569e907841498684daa29bd86ba58710923b927d`  
		Last Modified: Sat, 22 Jul 2023 01:39:40 GMT  
		Size: 2.6 KB (2629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:264c20cd444959db4b636f22bb6179f597e3cce76a719c4b89883c5c3d32b6b8`  
		Last Modified: Tue, 25 Jul 2023 01:40:29 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7afa4443f21ca6852bc9df1ea4ee418cb2de2e110b97dcff63469fc800c3498`  
		Last Modified: Tue, 25 Jul 2023 01:40:35 GMT  
		Size: 58.5 MB (58493543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d32c26cb271e9bac9fd739bf78492fc8f831792aeb0d657ee2dc79304598bc21`  
		Last Modified: Tue, 25 Jul 2023 01:40:27 GMT  
		Size: 317.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1f84a2204cb8c481eeee7c56cd79502c7eb68dad75dbc0620dcd264a33e8bf3`  
		Last Modified: Tue, 25 Jul 2023 01:40:37 GMT  
		Size: 57.5 MB (57502986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a41fcc5b5085e66b65b1416c884e349f58d5f498431dde90f81c5df20f56d97`  
		Last Modified: Tue, 25 Jul 2023 01:40:27 GMT  
		Size: 5.4 KB (5392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b8402026abb7d3c430c0873c480f604e969fd6d8aef70552f5445c81bcc84fa`  
		Last Modified: Tue, 25 Jul 2023 01:40:27 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8.0.34` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:c589deae89d660f907875ca7ac419f0704fc20f6d3825329b585ee2402b35101
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.1 MB (170071542 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2031a058d3ba2b2446da5464f0a29aea1008799bef06f24fd67bbc6743e53788`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 22 Jul 2023 01:03:33 GMT
ADD file:49b1f7f2b2558f78918f26b488622ad08fa607583d0a45f4f116773e2c13cf96 in / 
# Sat, 22 Jul 2023 01:03:34 GMT
CMD ["/bin/bash"]
# Sat, 22 Jul 2023 01:20:07 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Sat, 22 Jul 2023 01:20:07 GMT
ENV GOSU_VERSION=1.16
# Sat, 22 Jul 2023 01:20:11 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 22 Jul 2023 01:20:36 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Sat, 22 Jul 2023 01:20:37 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Sat, 22 Jul 2023 01:20:37 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 25 Jul 2023 01:42:38 GMT
ENV MYSQL_VERSION=8.0.34-1.el8
# Tue, 25 Jul 2023 01:42:39 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Tue, 25 Jul 2023 01:43:09 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Tue, 25 Jul 2023 01:43:10 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Tue, 25 Jul 2023 01:43:11 GMT
ENV MYSQL_SHELL_VERSION=8.0.34-1.el8
# Tue, 25 Jul 2023 01:43:45 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Tue, 25 Jul 2023 01:43:47 GMT
VOLUME [/var/lib/mysql]
# Tue, 25 Jul 2023 01:43:47 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Tue, 25 Jul 2023 01:43:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 25 Jul 2023 01:43:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 25 Jul 2023 01:43:47 GMT
EXPOSE 3306 33060
# Tue, 25 Jul 2023 01:43:47 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:1817bc1e6309503caf2242a5c83a4a6e9ebfdfb378d39bc92607690883a98c66`  
		Last Modified: Sat, 22 Jul 2023 01:04:31 GMT  
		Size: 43.6 MB (43623755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:740bd54462bcaa8cf5795022cb1daf5bf3b565d088fa1589e0e310225f2420d2`  
		Last Modified: Sat, 22 Jul 2023 01:22:13 GMT  
		Size: 886.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7e5ed4e69b309907018566aa973118702a7ad4f73cb732e4fb36fea862eaa26`  
		Last Modified: Sat, 22 Jul 2023 01:22:13 GMT  
		Size: 913.0 KB (912994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fdf88d7bbb7fa583fd2dfb4b80fa9ae42f0e8f228e3c15bdcf873dfadcaa445`  
		Last Modified: Sat, 22 Jul 2023 01:22:12 GMT  
		Size: 4.3 MB (4294535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1a5f85609500a34b3d4c06362e79700456581cfaf64335c617b36a10635033b`  
		Last Modified: Sat, 22 Jul 2023 01:22:11 GMT  
		Size: 2.6 KB (2631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d2014e71aa1dbbbd5d97f00faf0554b15d6660c42309369628b916d76b2cb14`  
		Last Modified: Tue, 25 Jul 2023 01:44:21 GMT  
		Size: 337.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a65eef3628981996acbf5281bc80aff6f958a7a95b309aa45c4c48103d895795`  
		Last Modified: Tue, 25 Jul 2023 01:44:25 GMT  
		Size: 57.5 MB (57465006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1086465c0f610a7ac25f9d953a2aae549cd70023e40ef1126dc6e92e31a1c842`  
		Last Modified: Tue, 25 Jul 2023 01:44:19 GMT  
		Size: 317.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d718a732c3abee1163a53974bcfdf72f17454a49c9d8998fba92c60851f175b`  
		Last Modified: Tue, 25 Jul 2023 01:44:27 GMT  
		Size: 63.8 MB (63765566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c724fd4b412f48fecb147fd4d9d377059bcfb971c79ffde2d6fd43bbdb0d1384`  
		Last Modified: Tue, 25 Jul 2023 01:44:19 GMT  
		Size: 5.4 KB (5394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74fcbdd515b315a3e4eadc554a90a0b48392758d0686ee5c0bbdc6f9e7af7e76`  
		Last Modified: Tue, 25 Jul 2023 01:44:19 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0.34-debian`

```console
$ docker pull mysql@sha256:49f4fcb0087318aa1c222c7e8ceacbb541cdc457c6307d45e6ee4313f4902e33
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:8.0.34-debian` - linux; amd64

```console
$ docker pull mysql@sha256:26db38c917a651edd01fc69bb56b8e068397a1ca4dfef9739cecc61f3111e6b4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **179.5 MB (179509315 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:992367f7e447afa8958f0b52f60a32bf01362731ac144922e319c26d5bade895`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 27 Jul 2023 23:25:07 GMT
ADD file:3d726bf0abbc08d6dda026cc406cdfb529deb60071641d164de28fcd62d1c1c0 in / 
# Thu, 27 Jul 2023 23:25:07 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 04:00:21 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Fri, 28 Jul 2023 04:00:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg && rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 04:00:26 GMT
ENV GOSU_VERSION=1.16
# Fri, 28 Jul 2023 04:00:35 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 28 Jul 2023 04:00:35 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 28 Jul 2023 04:00:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 04:00:41 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Fri, 28 Jul 2023 04:00:41 GMT
ENV MYSQL_MAJOR=8.0
# Fri, 28 Jul 2023 04:00:41 GMT
ENV MYSQL_VERSION=8.0.34-1debian11
# Fri, 28 Jul 2023 04:00:42 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ bullseye mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Fri, 28 Jul 2023 04:00:56 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Fri, 28 Jul 2023 04:00:57 GMT
VOLUME [/var/lib/mysql]
# Fri, 28 Jul 2023 04:00:57 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Fri, 28 Jul 2023 04:00:57 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Fri, 28 Jul 2023 04:00:57 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 28 Jul 2023 04:00:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 28 Jul 2023 04:00:58 GMT
EXPOSE 3306 33060
# Fri, 28 Jul 2023 04:00:58 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:1d5252f66ea9b661aceca1027b3d7ca259a50608261a25b51148119ecf086932`  
		Last Modified: Thu, 27 Jul 2023 23:30:08 GMT  
		Size: 31.4 MB (31417602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b034716887fd3351d90a2dadd53aa4984cd39f8397149d2fde665822cbdfb285`  
		Last Modified: Fri, 28 Jul 2023 04:02:17 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:882448c7d618dde8cedcebbf5843a1abdc3f8840035073f44ac0be1c75a88222`  
		Last Modified: Fri, 28 Jul 2023 04:02:17 GMT  
		Size: 4.4 MB (4415051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c14ac4640b87d832c2419b4c3968a4718ab31ef1cec549b8415be42ebb792611`  
		Last Modified: Fri, 28 Jul 2023 04:02:15 GMT  
		Size: 1.5 MB (1471510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d2978613e401218d6fd28693e6d47c7110dd5d4bd2f750ee1d37fc4f8428fd9`  
		Last Modified: Fri, 28 Jul 2023 04:02:15 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c33d24cb8c756b450de2635eb9fba6c9647da56ab1945e6c2b4e3926725ac3de`  
		Last Modified: Fri, 28 Jul 2023 04:02:17 GMT  
		Size: 12.7 MB (12662071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52fa14fc88fc63d64bb0d429a08bdaaae8f80694ad373b7c85e566d535fc88e5`  
		Last Modified: Fri, 28 Jul 2023 04:02:14 GMT  
		Size: 2.5 KB (2549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42deb22ec16d8d602e97596083fd18c35167815a0af24879dfd937d052bf72be`  
		Last Modified: Fri, 28 Jul 2023 04:02:13 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3d31d600a65d21a8dcd2963f131d5a412a1b257f8b7ede1896a939929cc24e6`  
		Last Modified: Fri, 28 Jul 2023 04:02:30 GMT  
		Size: 129.5 MB (129532040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0b9f5aba00d7eab19f55c9f54637f274c1275e6a8f33508b24dc332c4334e07`  
		Last Modified: Fri, 28 Jul 2023 04:02:13 GMT  
		Size: 843.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98222a66de151bb3ad1b199d0398af90a4552e2515f3bd52663e7df2c56b72a7`  
		Last Modified: Fri, 28 Jul 2023 04:02:12 GMT  
		Size: 5.4 KB (5391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ff8f0c3c67bc36e46203bc2fb68ed8023121c5f4b607ddd8d8ff48c01384452`  
		Last Modified: Fri, 28 Jul 2023 04:02:13 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0.34-oracle`

```console
$ docker pull mysql@sha256:51c4dc55d3abf4517a5a652794d1f0adb2f2ed1d1bedc847d6132d91cdb2ebbf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8.0.34-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:1da5cf22e7177925fa4d2a707936ca4ade59ba10b40b23550b0ffc12f8340600
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **166.5 MB (166515599 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c5ae0d3388cc6f2c72e73c8b1b9a7ba29347d9d7117d426b5cd83c3b71fe2b9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 22 Jul 2023 01:20:32 GMT
ADD file:6d43f7bf7c8d8c056e6fcc566ccfa2c1e42be1ef095f94d6780d0ca7d9a02e6e in / 
# Sat, 22 Jul 2023 01:20:32 GMT
CMD ["/bin/bash"]
# Sat, 22 Jul 2023 01:37:28 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Sat, 22 Jul 2023 01:37:28 GMT
ENV GOSU_VERSION=1.16
# Sat, 22 Jul 2023 01:37:31 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 22 Jul 2023 01:37:58 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Sat, 22 Jul 2023 01:37:59 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Sat, 22 Jul 2023 01:37:59 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 25 Jul 2023 01:37:33 GMT
ENV MYSQL_VERSION=8.0.34-1.el8
# Tue, 25 Jul 2023 01:37:34 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Tue, 25 Jul 2023 01:38:08 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Tue, 25 Jul 2023 01:38:09 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Tue, 25 Jul 2023 01:38:09 GMT
ENV MYSQL_SHELL_VERSION=8.0.34-1.el8
# Tue, 25 Jul 2023 01:38:47 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Tue, 25 Jul 2023 01:38:48 GMT
VOLUME [/var/lib/mysql]
# Tue, 25 Jul 2023 01:38:48 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Tue, 25 Jul 2023 01:38:49 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 25 Jul 2023 01:38:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 25 Jul 2023 01:38:49 GMT
EXPOSE 3306 33060
# Tue, 25 Jul 2023 01:38:49 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:49bb46380f8cb3491e82d000b27a6eb26b2490291da814ce3363bbf2c8baeb1a`  
		Last Modified: Sat, 22 Jul 2023 01:21:47 GMT  
		Size: 44.9 MB (44915006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aab3066bbf8fc576b01df1b0391e5a72a7ff72b1c0c5d09a7bab3db2a51d4744`  
		Last Modified: Sat, 22 Jul 2023 01:39:42 GMT  
		Size: 884.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6eef8c26cf9c633276ffd191110525157aa8811962fce9164a8a79814d497bd`  
		Last Modified: Sat, 22 Jul 2023 01:39:42 GMT  
		Size: 982.8 KB (982822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e908b1dcba2267120afc44b8f24aba3cdf060da1257257196b07f34edd7e959`  
		Last Modified: Sat, 22 Jul 2023 01:39:41 GMT  
		Size: 4.6 MB (4611560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:480c3912a2fde8647ba9e97d569e907841498684daa29bd86ba58710923b927d`  
		Last Modified: Sat, 22 Jul 2023 01:39:40 GMT  
		Size: 2.6 KB (2629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:264c20cd444959db4b636f22bb6179f597e3cce76a719c4b89883c5c3d32b6b8`  
		Last Modified: Tue, 25 Jul 2023 01:40:29 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7afa4443f21ca6852bc9df1ea4ee418cb2de2e110b97dcff63469fc800c3498`  
		Last Modified: Tue, 25 Jul 2023 01:40:35 GMT  
		Size: 58.5 MB (58493543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d32c26cb271e9bac9fd739bf78492fc8f831792aeb0d657ee2dc79304598bc21`  
		Last Modified: Tue, 25 Jul 2023 01:40:27 GMT  
		Size: 317.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1f84a2204cb8c481eeee7c56cd79502c7eb68dad75dbc0620dcd264a33e8bf3`  
		Last Modified: Tue, 25 Jul 2023 01:40:37 GMT  
		Size: 57.5 MB (57502986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a41fcc5b5085e66b65b1416c884e349f58d5f498431dde90f81c5df20f56d97`  
		Last Modified: Tue, 25 Jul 2023 01:40:27 GMT  
		Size: 5.4 KB (5392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b8402026abb7d3c430c0873c480f604e969fd6d8aef70552f5445c81bcc84fa`  
		Last Modified: Tue, 25 Jul 2023 01:40:27 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8.0.34-oracle` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:c589deae89d660f907875ca7ac419f0704fc20f6d3825329b585ee2402b35101
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.1 MB (170071542 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2031a058d3ba2b2446da5464f0a29aea1008799bef06f24fd67bbc6743e53788`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 22 Jul 2023 01:03:33 GMT
ADD file:49b1f7f2b2558f78918f26b488622ad08fa607583d0a45f4f116773e2c13cf96 in / 
# Sat, 22 Jul 2023 01:03:34 GMT
CMD ["/bin/bash"]
# Sat, 22 Jul 2023 01:20:07 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Sat, 22 Jul 2023 01:20:07 GMT
ENV GOSU_VERSION=1.16
# Sat, 22 Jul 2023 01:20:11 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 22 Jul 2023 01:20:36 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Sat, 22 Jul 2023 01:20:37 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Sat, 22 Jul 2023 01:20:37 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 25 Jul 2023 01:42:38 GMT
ENV MYSQL_VERSION=8.0.34-1.el8
# Tue, 25 Jul 2023 01:42:39 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Tue, 25 Jul 2023 01:43:09 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Tue, 25 Jul 2023 01:43:10 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Tue, 25 Jul 2023 01:43:11 GMT
ENV MYSQL_SHELL_VERSION=8.0.34-1.el8
# Tue, 25 Jul 2023 01:43:45 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Tue, 25 Jul 2023 01:43:47 GMT
VOLUME [/var/lib/mysql]
# Tue, 25 Jul 2023 01:43:47 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Tue, 25 Jul 2023 01:43:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 25 Jul 2023 01:43:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 25 Jul 2023 01:43:47 GMT
EXPOSE 3306 33060
# Tue, 25 Jul 2023 01:43:47 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:1817bc1e6309503caf2242a5c83a4a6e9ebfdfb378d39bc92607690883a98c66`  
		Last Modified: Sat, 22 Jul 2023 01:04:31 GMT  
		Size: 43.6 MB (43623755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:740bd54462bcaa8cf5795022cb1daf5bf3b565d088fa1589e0e310225f2420d2`  
		Last Modified: Sat, 22 Jul 2023 01:22:13 GMT  
		Size: 886.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7e5ed4e69b309907018566aa973118702a7ad4f73cb732e4fb36fea862eaa26`  
		Last Modified: Sat, 22 Jul 2023 01:22:13 GMT  
		Size: 913.0 KB (912994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fdf88d7bbb7fa583fd2dfb4b80fa9ae42f0e8f228e3c15bdcf873dfadcaa445`  
		Last Modified: Sat, 22 Jul 2023 01:22:12 GMT  
		Size: 4.3 MB (4294535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1a5f85609500a34b3d4c06362e79700456581cfaf64335c617b36a10635033b`  
		Last Modified: Sat, 22 Jul 2023 01:22:11 GMT  
		Size: 2.6 KB (2631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d2014e71aa1dbbbd5d97f00faf0554b15d6660c42309369628b916d76b2cb14`  
		Last Modified: Tue, 25 Jul 2023 01:44:21 GMT  
		Size: 337.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a65eef3628981996acbf5281bc80aff6f958a7a95b309aa45c4c48103d895795`  
		Last Modified: Tue, 25 Jul 2023 01:44:25 GMT  
		Size: 57.5 MB (57465006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1086465c0f610a7ac25f9d953a2aae549cd70023e40ef1126dc6e92e31a1c842`  
		Last Modified: Tue, 25 Jul 2023 01:44:19 GMT  
		Size: 317.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d718a732c3abee1163a53974bcfdf72f17454a49c9d8998fba92c60851f175b`  
		Last Modified: Tue, 25 Jul 2023 01:44:27 GMT  
		Size: 63.8 MB (63765566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c724fd4b412f48fecb147fd4d9d377059bcfb971c79ffde2d6fd43bbdb0d1384`  
		Last Modified: Tue, 25 Jul 2023 01:44:19 GMT  
		Size: 5.4 KB (5394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74fcbdd515b315a3e4eadc554a90a0b48392758d0686ee5c0bbdc6f9e7af7e76`  
		Last Modified: Tue, 25 Jul 2023 01:44:19 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.1`

**does not exist** (yet?)

## `mysql:8.1-oracle`

**does not exist** (yet?)

## `mysql:8.1.0`

**does not exist** (yet?)

## `mysql:8.1.0-oracle`

**does not exist** (yet?)

## `mysql:innovation`

**does not exist** (yet?)

## `mysql:innovation-oracle`

**does not exist** (yet?)

## `mysql:latest`

```console
$ docker pull mysql@sha256:51c4dc55d3abf4517a5a652794d1f0adb2f2ed1d1bedc847d6132d91cdb2ebbf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:latest` - linux; amd64

```console
$ docker pull mysql@sha256:1da5cf22e7177925fa4d2a707936ca4ade59ba10b40b23550b0ffc12f8340600
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **166.5 MB (166515599 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c5ae0d3388cc6f2c72e73c8b1b9a7ba29347d9d7117d426b5cd83c3b71fe2b9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 22 Jul 2023 01:20:32 GMT
ADD file:6d43f7bf7c8d8c056e6fcc566ccfa2c1e42be1ef095f94d6780d0ca7d9a02e6e in / 
# Sat, 22 Jul 2023 01:20:32 GMT
CMD ["/bin/bash"]
# Sat, 22 Jul 2023 01:37:28 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Sat, 22 Jul 2023 01:37:28 GMT
ENV GOSU_VERSION=1.16
# Sat, 22 Jul 2023 01:37:31 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 22 Jul 2023 01:37:58 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Sat, 22 Jul 2023 01:37:59 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Sat, 22 Jul 2023 01:37:59 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 25 Jul 2023 01:37:33 GMT
ENV MYSQL_VERSION=8.0.34-1.el8
# Tue, 25 Jul 2023 01:37:34 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Tue, 25 Jul 2023 01:38:08 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Tue, 25 Jul 2023 01:38:09 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Tue, 25 Jul 2023 01:38:09 GMT
ENV MYSQL_SHELL_VERSION=8.0.34-1.el8
# Tue, 25 Jul 2023 01:38:47 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Tue, 25 Jul 2023 01:38:48 GMT
VOLUME [/var/lib/mysql]
# Tue, 25 Jul 2023 01:38:48 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Tue, 25 Jul 2023 01:38:49 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 25 Jul 2023 01:38:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 25 Jul 2023 01:38:49 GMT
EXPOSE 3306 33060
# Tue, 25 Jul 2023 01:38:49 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:49bb46380f8cb3491e82d000b27a6eb26b2490291da814ce3363bbf2c8baeb1a`  
		Last Modified: Sat, 22 Jul 2023 01:21:47 GMT  
		Size: 44.9 MB (44915006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aab3066bbf8fc576b01df1b0391e5a72a7ff72b1c0c5d09a7bab3db2a51d4744`  
		Last Modified: Sat, 22 Jul 2023 01:39:42 GMT  
		Size: 884.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6eef8c26cf9c633276ffd191110525157aa8811962fce9164a8a79814d497bd`  
		Last Modified: Sat, 22 Jul 2023 01:39:42 GMT  
		Size: 982.8 KB (982822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e908b1dcba2267120afc44b8f24aba3cdf060da1257257196b07f34edd7e959`  
		Last Modified: Sat, 22 Jul 2023 01:39:41 GMT  
		Size: 4.6 MB (4611560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:480c3912a2fde8647ba9e97d569e907841498684daa29bd86ba58710923b927d`  
		Last Modified: Sat, 22 Jul 2023 01:39:40 GMT  
		Size: 2.6 KB (2629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:264c20cd444959db4b636f22bb6179f597e3cce76a719c4b89883c5c3d32b6b8`  
		Last Modified: Tue, 25 Jul 2023 01:40:29 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7afa4443f21ca6852bc9df1ea4ee418cb2de2e110b97dcff63469fc800c3498`  
		Last Modified: Tue, 25 Jul 2023 01:40:35 GMT  
		Size: 58.5 MB (58493543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d32c26cb271e9bac9fd739bf78492fc8f831792aeb0d657ee2dc79304598bc21`  
		Last Modified: Tue, 25 Jul 2023 01:40:27 GMT  
		Size: 317.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1f84a2204cb8c481eeee7c56cd79502c7eb68dad75dbc0620dcd264a33e8bf3`  
		Last Modified: Tue, 25 Jul 2023 01:40:37 GMT  
		Size: 57.5 MB (57502986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a41fcc5b5085e66b65b1416c884e349f58d5f498431dde90f81c5df20f56d97`  
		Last Modified: Tue, 25 Jul 2023 01:40:27 GMT  
		Size: 5.4 KB (5392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b8402026abb7d3c430c0873c480f604e969fd6d8aef70552f5445c81bcc84fa`  
		Last Modified: Tue, 25 Jul 2023 01:40:27 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:latest` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:c589deae89d660f907875ca7ac419f0704fc20f6d3825329b585ee2402b35101
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.1 MB (170071542 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2031a058d3ba2b2446da5464f0a29aea1008799bef06f24fd67bbc6743e53788`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 22 Jul 2023 01:03:33 GMT
ADD file:49b1f7f2b2558f78918f26b488622ad08fa607583d0a45f4f116773e2c13cf96 in / 
# Sat, 22 Jul 2023 01:03:34 GMT
CMD ["/bin/bash"]
# Sat, 22 Jul 2023 01:20:07 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Sat, 22 Jul 2023 01:20:07 GMT
ENV GOSU_VERSION=1.16
# Sat, 22 Jul 2023 01:20:11 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 22 Jul 2023 01:20:36 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Sat, 22 Jul 2023 01:20:37 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Sat, 22 Jul 2023 01:20:37 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 25 Jul 2023 01:42:38 GMT
ENV MYSQL_VERSION=8.0.34-1.el8
# Tue, 25 Jul 2023 01:42:39 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Tue, 25 Jul 2023 01:43:09 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Tue, 25 Jul 2023 01:43:10 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Tue, 25 Jul 2023 01:43:11 GMT
ENV MYSQL_SHELL_VERSION=8.0.34-1.el8
# Tue, 25 Jul 2023 01:43:45 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Tue, 25 Jul 2023 01:43:47 GMT
VOLUME [/var/lib/mysql]
# Tue, 25 Jul 2023 01:43:47 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Tue, 25 Jul 2023 01:43:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 25 Jul 2023 01:43:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 25 Jul 2023 01:43:47 GMT
EXPOSE 3306 33060
# Tue, 25 Jul 2023 01:43:47 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:1817bc1e6309503caf2242a5c83a4a6e9ebfdfb378d39bc92607690883a98c66`  
		Last Modified: Sat, 22 Jul 2023 01:04:31 GMT  
		Size: 43.6 MB (43623755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:740bd54462bcaa8cf5795022cb1daf5bf3b565d088fa1589e0e310225f2420d2`  
		Last Modified: Sat, 22 Jul 2023 01:22:13 GMT  
		Size: 886.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7e5ed4e69b309907018566aa973118702a7ad4f73cb732e4fb36fea862eaa26`  
		Last Modified: Sat, 22 Jul 2023 01:22:13 GMT  
		Size: 913.0 KB (912994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fdf88d7bbb7fa583fd2dfb4b80fa9ae42f0e8f228e3c15bdcf873dfadcaa445`  
		Last Modified: Sat, 22 Jul 2023 01:22:12 GMT  
		Size: 4.3 MB (4294535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1a5f85609500a34b3d4c06362e79700456581cfaf64335c617b36a10635033b`  
		Last Modified: Sat, 22 Jul 2023 01:22:11 GMT  
		Size: 2.6 KB (2631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d2014e71aa1dbbbd5d97f00faf0554b15d6660c42309369628b916d76b2cb14`  
		Last Modified: Tue, 25 Jul 2023 01:44:21 GMT  
		Size: 337.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a65eef3628981996acbf5281bc80aff6f958a7a95b309aa45c4c48103d895795`  
		Last Modified: Tue, 25 Jul 2023 01:44:25 GMT  
		Size: 57.5 MB (57465006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1086465c0f610a7ac25f9d953a2aae549cd70023e40ef1126dc6e92e31a1c842`  
		Last Modified: Tue, 25 Jul 2023 01:44:19 GMT  
		Size: 317.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d718a732c3abee1163a53974bcfdf72f17454a49c9d8998fba92c60851f175b`  
		Last Modified: Tue, 25 Jul 2023 01:44:27 GMT  
		Size: 63.8 MB (63765566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c724fd4b412f48fecb147fd4d9d377059bcfb971c79ffde2d6fd43bbdb0d1384`  
		Last Modified: Tue, 25 Jul 2023 01:44:19 GMT  
		Size: 5.4 KB (5394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74fcbdd515b315a3e4eadc554a90a0b48392758d0686ee5c0bbdc6f9e7af7e76`  
		Last Modified: Tue, 25 Jul 2023 01:44:19 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:oracle`

```console
$ docker pull mysql@sha256:51c4dc55d3abf4517a5a652794d1f0adb2f2ed1d1bedc847d6132d91cdb2ebbf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:oracle` - linux; amd64

```console
$ docker pull mysql@sha256:1da5cf22e7177925fa4d2a707936ca4ade59ba10b40b23550b0ffc12f8340600
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **166.5 MB (166515599 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c5ae0d3388cc6f2c72e73c8b1b9a7ba29347d9d7117d426b5cd83c3b71fe2b9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 22 Jul 2023 01:20:32 GMT
ADD file:6d43f7bf7c8d8c056e6fcc566ccfa2c1e42be1ef095f94d6780d0ca7d9a02e6e in / 
# Sat, 22 Jul 2023 01:20:32 GMT
CMD ["/bin/bash"]
# Sat, 22 Jul 2023 01:37:28 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Sat, 22 Jul 2023 01:37:28 GMT
ENV GOSU_VERSION=1.16
# Sat, 22 Jul 2023 01:37:31 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 22 Jul 2023 01:37:58 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Sat, 22 Jul 2023 01:37:59 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Sat, 22 Jul 2023 01:37:59 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 25 Jul 2023 01:37:33 GMT
ENV MYSQL_VERSION=8.0.34-1.el8
# Tue, 25 Jul 2023 01:37:34 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Tue, 25 Jul 2023 01:38:08 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Tue, 25 Jul 2023 01:38:09 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Tue, 25 Jul 2023 01:38:09 GMT
ENV MYSQL_SHELL_VERSION=8.0.34-1.el8
# Tue, 25 Jul 2023 01:38:47 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Tue, 25 Jul 2023 01:38:48 GMT
VOLUME [/var/lib/mysql]
# Tue, 25 Jul 2023 01:38:48 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Tue, 25 Jul 2023 01:38:49 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 25 Jul 2023 01:38:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 25 Jul 2023 01:38:49 GMT
EXPOSE 3306 33060
# Tue, 25 Jul 2023 01:38:49 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:49bb46380f8cb3491e82d000b27a6eb26b2490291da814ce3363bbf2c8baeb1a`  
		Last Modified: Sat, 22 Jul 2023 01:21:47 GMT  
		Size: 44.9 MB (44915006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aab3066bbf8fc576b01df1b0391e5a72a7ff72b1c0c5d09a7bab3db2a51d4744`  
		Last Modified: Sat, 22 Jul 2023 01:39:42 GMT  
		Size: 884.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6eef8c26cf9c633276ffd191110525157aa8811962fce9164a8a79814d497bd`  
		Last Modified: Sat, 22 Jul 2023 01:39:42 GMT  
		Size: 982.8 KB (982822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e908b1dcba2267120afc44b8f24aba3cdf060da1257257196b07f34edd7e959`  
		Last Modified: Sat, 22 Jul 2023 01:39:41 GMT  
		Size: 4.6 MB (4611560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:480c3912a2fde8647ba9e97d569e907841498684daa29bd86ba58710923b927d`  
		Last Modified: Sat, 22 Jul 2023 01:39:40 GMT  
		Size: 2.6 KB (2629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:264c20cd444959db4b636f22bb6179f597e3cce76a719c4b89883c5c3d32b6b8`  
		Last Modified: Tue, 25 Jul 2023 01:40:29 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7afa4443f21ca6852bc9df1ea4ee418cb2de2e110b97dcff63469fc800c3498`  
		Last Modified: Tue, 25 Jul 2023 01:40:35 GMT  
		Size: 58.5 MB (58493543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d32c26cb271e9bac9fd739bf78492fc8f831792aeb0d657ee2dc79304598bc21`  
		Last Modified: Tue, 25 Jul 2023 01:40:27 GMT  
		Size: 317.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1f84a2204cb8c481eeee7c56cd79502c7eb68dad75dbc0620dcd264a33e8bf3`  
		Last Modified: Tue, 25 Jul 2023 01:40:37 GMT  
		Size: 57.5 MB (57502986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a41fcc5b5085e66b65b1416c884e349f58d5f498431dde90f81c5df20f56d97`  
		Last Modified: Tue, 25 Jul 2023 01:40:27 GMT  
		Size: 5.4 KB (5392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b8402026abb7d3c430c0873c480f604e969fd6d8aef70552f5445c81bcc84fa`  
		Last Modified: Tue, 25 Jul 2023 01:40:27 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:oracle` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:c589deae89d660f907875ca7ac419f0704fc20f6d3825329b585ee2402b35101
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.1 MB (170071542 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2031a058d3ba2b2446da5464f0a29aea1008799bef06f24fd67bbc6743e53788`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Sat, 22 Jul 2023 01:03:33 GMT
ADD file:49b1f7f2b2558f78918f26b488622ad08fa607583d0a45f4f116773e2c13cf96 in / 
# Sat, 22 Jul 2023 01:03:34 GMT
CMD ["/bin/bash"]
# Sat, 22 Jul 2023 01:20:07 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Sat, 22 Jul 2023 01:20:07 GMT
ENV GOSU_VERSION=1.16
# Sat, 22 Jul 2023 01:20:11 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 22 Jul 2023 01:20:36 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Sat, 22 Jul 2023 01:20:37 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Sat, 22 Jul 2023 01:20:37 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 25 Jul 2023 01:42:38 GMT
ENV MYSQL_VERSION=8.0.34-1.el8
# Tue, 25 Jul 2023 01:42:39 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Tue, 25 Jul 2023 01:43:09 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Tue, 25 Jul 2023 01:43:10 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Tue, 25 Jul 2023 01:43:11 GMT
ENV MYSQL_SHELL_VERSION=8.0.34-1.el8
# Tue, 25 Jul 2023 01:43:45 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Tue, 25 Jul 2023 01:43:47 GMT
VOLUME [/var/lib/mysql]
# Tue, 25 Jul 2023 01:43:47 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Tue, 25 Jul 2023 01:43:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 25 Jul 2023 01:43:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 25 Jul 2023 01:43:47 GMT
EXPOSE 3306 33060
# Tue, 25 Jul 2023 01:43:47 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:1817bc1e6309503caf2242a5c83a4a6e9ebfdfb378d39bc92607690883a98c66`  
		Last Modified: Sat, 22 Jul 2023 01:04:31 GMT  
		Size: 43.6 MB (43623755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:740bd54462bcaa8cf5795022cb1daf5bf3b565d088fa1589e0e310225f2420d2`  
		Last Modified: Sat, 22 Jul 2023 01:22:13 GMT  
		Size: 886.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7e5ed4e69b309907018566aa973118702a7ad4f73cb732e4fb36fea862eaa26`  
		Last Modified: Sat, 22 Jul 2023 01:22:13 GMT  
		Size: 913.0 KB (912994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fdf88d7bbb7fa583fd2dfb4b80fa9ae42f0e8f228e3c15bdcf873dfadcaa445`  
		Last Modified: Sat, 22 Jul 2023 01:22:12 GMT  
		Size: 4.3 MB (4294535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1a5f85609500a34b3d4c06362e79700456581cfaf64335c617b36a10635033b`  
		Last Modified: Sat, 22 Jul 2023 01:22:11 GMT  
		Size: 2.6 KB (2631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d2014e71aa1dbbbd5d97f00faf0554b15d6660c42309369628b916d76b2cb14`  
		Last Modified: Tue, 25 Jul 2023 01:44:21 GMT  
		Size: 337.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a65eef3628981996acbf5281bc80aff6f958a7a95b309aa45c4c48103d895795`  
		Last Modified: Tue, 25 Jul 2023 01:44:25 GMT  
		Size: 57.5 MB (57465006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1086465c0f610a7ac25f9d953a2aae549cd70023e40ef1126dc6e92e31a1c842`  
		Last Modified: Tue, 25 Jul 2023 01:44:19 GMT  
		Size: 317.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d718a732c3abee1163a53974bcfdf72f17454a49c9d8998fba92c60851f175b`  
		Last Modified: Tue, 25 Jul 2023 01:44:27 GMT  
		Size: 63.8 MB (63765566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c724fd4b412f48fecb147fd4d9d377059bcfb971c79ffde2d6fd43bbdb0d1384`  
		Last Modified: Tue, 25 Jul 2023 01:44:19 GMT  
		Size: 5.4 KB (5394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74fcbdd515b315a3e4eadc554a90a0b48392758d0686ee5c0bbdc6f9e7af7e76`  
		Last Modified: Tue, 25 Jul 2023 01:44:19 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
