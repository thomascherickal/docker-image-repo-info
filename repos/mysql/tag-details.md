<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `mysql`

-	[`mysql:5`](#mysql5)
-	[`mysql:5-debian`](#mysql5-debian)
-	[`mysql:5-oracle`](#mysql5-oracle)
-	[`mysql:5.7`](#mysql57)
-	[`mysql:5.7-debian`](#mysql57-debian)
-	[`mysql:5.7-oracle`](#mysql57-oracle)
-	[`mysql:5.7.40`](#mysql5740)
-	[`mysql:5.7.40-debian`](#mysql5740-debian)
-	[`mysql:5.7.40-oracle`](#mysql5740-oracle)
-	[`mysql:8`](#mysql8)
-	[`mysql:8-debian`](#mysql8-debian)
-	[`mysql:8-oracle`](#mysql8-oracle)
-	[`mysql:8.0`](#mysql80)
-	[`mysql:8.0-debian`](#mysql80-debian)
-	[`mysql:8.0-oracle`](#mysql80-oracle)
-	[`mysql:8.0.31`](#mysql8031)
-	[`mysql:8.0.31-debian`](#mysql8031-debian)
-	[`mysql:8.0.31-oracle`](#mysql8031-oracle)
-	[`mysql:debian`](#mysqldebian)
-	[`mysql:latest`](#mysqllatest)
-	[`mysql:oracle`](#mysqloracle)

## `mysql:5`

```console
$ docker pull mysql@sha256:6306f106a056e24b3a2582a59a4c84cd199907f826eff27df36406f227cd9a7d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5` - linux; amd64

```console
$ docker pull mysql@sha256:bd0fb5a175fc225ce9c2c4357c0f532bda1413e0b8555a157770f92daa5a89e0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.3 MB (144279475 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d410f4167eea912908b2f9bcc24eff870cb3c131dfb755088b79a4188bfeb40f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 07 Dec 2022 01:51:56 GMT
ADD file:3853624d773c4bf6fc1464ca06bd07366109fab78072fcab59075073a5da6525 in / 
# Wed, 07 Dec 2022 01:51:56 GMT
CMD ["/bin/bash"]
# Wed, 07 Dec 2022 02:23:50 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 07 Dec 2022 02:23:50 GMT
ENV GOSU_VERSION=1.14
# Wed, 07 Dec 2022 02:23:52 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 07 Dec 2022 02:24:09 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False oracle-epel-release-el7; 	yum install -y --setopt=skip_missing_names_on_install=False 		bzip2 		gzip 		openssl 		xz 		zstd 	; 	yum clean all
# Wed, 07 Dec 2022 02:24:10 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 07 Dec 2022 02:24:10 GMT
ENV MYSQL_MAJOR=5.7
# Wed, 07 Dec 2022 02:24:10 GMT
ENV MYSQL_VERSION=5.7.40-1.el7
# Wed, 07 Dec 2022 02:24:11 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql5.7-server-minimal]'; 		echo 'name=MySQL 5.7 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-5.7-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 07 Dec 2022 02:24:29 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-community-server-minimal-$MYSQL_VERSION"; 	yum clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	{ echo '!includedir /etc/mysql/mysql.conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/mysql.conf.d; 		find /etc/my.cnf /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/'; 		mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 07 Dec 2022 02:24:30 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 07 Dec 2022 02:24:30 GMT
ENV MYSQL_SHELL_VERSION=8.0.31-1.el7
# Wed, 07 Dec 2022 02:24:53 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-shell-$MYSQL_SHELL_VERSION"; 	yum clean all; 		mysqlsh --version
# Wed, 07 Dec 2022 02:24:54 GMT
VOLUME [/var/lib/mysql]
# Wed, 07 Dec 2022 02:24:54 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 07 Dec 2022 02:24:55 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 07 Dec 2022 02:24:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 07 Dec 2022 02:24:55 GMT
EXPOSE 3306 33060
# Wed, 07 Dec 2022 02:24:55 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:d26998a7c52d2b84e7927f97651d1d703a805c8e4d3f658a03138721f5a5dd44`  
		Last Modified: Wed, 07 Dec 2022 01:53:46 GMT  
		Size: 49.8 MB (49818482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a9d8a3567e30df99576e0a4dbca773af581230fee203891610e6ccbdaa823d2`  
		Last Modified: Wed, 07 Dec 2022 02:26:00 GMT  
		Size: 871.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfee1f0f349e08af59ed77c7d56ede70f0c5739daa2477ef54a4ee457f5e3e47`  
		Last Modified: Wed, 07 Dec 2022 02:26:01 GMT  
		Size: 930.2 KB (930227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71ff8dfb9b12b027c35d779fe4f06a9b3d0d26efed52153324cfa2f409423b0d`  
		Last Modified: Wed, 07 Dec 2022 02:25:59 GMT  
		Size: 4.5 MB (4539026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf56cbebc916d35659623816867a456610961f77db6d9753e738c5564651dfa0`  
		Last Modified: Wed, 07 Dec 2022 02:25:58 GMT  
		Size: 2.7 KB (2658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e747e5e37d77f3d8331753fc4c4eb0b0e5af8648ee5b2eec8fa274ebdddb475`  
		Last Modified: Wed, 07 Dec 2022 02:25:58 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:711a06e512dab8bc033e74a32300e408fc4d5ab67e6db0f84942d3ddadb7376d`  
		Last Modified: Wed, 07 Dec 2022 02:26:01 GMT  
		Size: 25.5 MB (25532079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3288d68e4e9e0f5e70378db2d166bf205b73ca677bdf72384be72fa529264ed1`  
		Last Modified: Wed, 07 Dec 2022 02:25:57 GMT  
		Size: 315.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49271f2d6d157b6b14c6d6c165b3b29b8d29aef70edd653702832a48bcecf382`  
		Last Modified: Wed, 07 Dec 2022 02:26:08 GMT  
		Size: 63.4 MB (63449972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f782f6cac69ce870188610aef114b2852e9f69f2b849a4df90c0209bf8dc1717`  
		Last Modified: Wed, 07 Dec 2022 02:25:57 GMT  
		Size: 5.4 KB (5386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:701dea355691c2e0ccc548aa219fc1dd83ba44ff81843802aef25e77e813454d`  
		Last Modified: Wed, 07 Dec 2022 02:25:57 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5-debian`

```console
$ docker pull mysql@sha256:c134741fc67355f1f57939624ff3e117bc0a2b0e6566fca60f85bce847a04ace
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5-debian` - linux; amd64

```console
$ docker pull mysql@sha256:c7f71d444e2a3434aede4594672722dd2e2f4e886882f5133cb2b7ee23d0e5a7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **162.6 MB (162596962 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94165850af50f5fc2c2cdf49a5c0d6e71d1408c3817eae97a681ae86b15fab19`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 21 Dec 2022 01:20:52 GMT
ADD file:660e0093a3da49e4ca41260d09d585754ccb1eff8974c4b0dd4456b76ddbbc9a in / 
# Wed, 21 Dec 2022 01:20:52 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 11:32:39 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 21 Dec 2022 11:32:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 11:32:45 GMT
ENV GOSU_VERSION=1.14
# Wed, 21 Dec 2022 11:32:54 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 21 Dec 2022 11:32:54 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 21 Dec 2022 11:33:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 11:33:02 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Wed, 21 Dec 2022 11:33:02 GMT
ENV MYSQL_MAJOR=5.7
# Wed, 21 Dec 2022 11:33:02 GMT
ENV MYSQL_VERSION=5.7.40-1debian10
# Wed, 21 Dec 2022 11:33:03 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-5.7' > /etc/apt/sources.list.d/mysql.list
# Wed, 21 Dec 2022 11:33:22 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-server="${MYSQL_VERSION}" 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Wed, 21 Dec 2022 11:33:23 GMT
VOLUME [/var/lib/mysql]
# Wed, 21 Dec 2022 11:33:23 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 21 Dec 2022 11:33:23 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 21 Dec 2022 11:33:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Dec 2022 11:33:24 GMT
EXPOSE 3306 33060
# Wed, 21 Dec 2022 11:33:24 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:b52ebda398ed2c4602ea06056f78d45a59474ee4e2a020967251ba082424e7e2`  
		Last Modified: Wed, 21 Dec 2022 01:25:17 GMT  
		Size: 27.1 MB (27140331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ce9a79d5155fd4711289385da53044c809d4e3c678327ca6d45fb6a9f4cf987`  
		Last Modified: Wed, 21 Dec 2022 11:34:31 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e261668310f535cff440b65def4e46639ea51e56eb7e29f3dcd0d2bc789dc16`  
		Last Modified: Wed, 21 Dec 2022 11:34:30 GMT  
		Size: 4.2 MB (4182322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3123e9b617f90c63e401b61f20202da262ba291624f9cf582382b6606266d4f`  
		Last Modified: Wed, 21 Dec 2022 11:34:30 GMT  
		Size: 1.4 MB (1388870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f0c53d4059e024752565a418a176ee322c7975e3573daac8543596533034c0d`  
		Last Modified: Wed, 21 Dec 2022 11:34:29 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a769258f8c5aae1218e004f37090ebf203889beee192d48cef2bc63238e41bdb`  
		Last Modified: Wed, 21 Dec 2022 11:34:32 GMT  
		Size: 14.1 MB (14089454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6478aa5af16e1946961ac5a640d2dd50637ef7f6f5a19546baf2add23b9f0930`  
		Last Modified: Wed, 21 Dec 2022 11:34:27 GMT  
		Size: 2.5 KB (2545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86a4405a4c9e0921b9c4f114716117465cab4932d55dd832a73ef363f18e4f75`  
		Last Modified: Wed, 21 Dec 2022 11:34:27 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eae9863c382483c9a8a0bc99c315132f7b91a2abdd9c8e6c4854e15a5f8770b2`  
		Last Modified: Wed, 21 Dec 2022 11:34:43 GMT  
		Size: 115.8 MB (115785799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a741ea6ad10a9767f461430b7c34fbe4cd65ce41bcd26837e7a0a32d5144aae4`  
		Last Modified: Wed, 21 Dec 2022 11:34:27 GMT  
		Size: 5.4 KB (5389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62548f9fac91770f96cdf945c008bf822f27efacd5d895c9643be71f8555485a`  
		Last Modified: Wed, 21 Dec 2022 11:34:27 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5-oracle`

```console
$ docker pull mysql@sha256:6306f106a056e24b3a2582a59a4c84cd199907f826eff27df36406f227cd9a7d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:bd0fb5a175fc225ce9c2c4357c0f532bda1413e0b8555a157770f92daa5a89e0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.3 MB (144279475 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d410f4167eea912908b2f9bcc24eff870cb3c131dfb755088b79a4188bfeb40f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 07 Dec 2022 01:51:56 GMT
ADD file:3853624d773c4bf6fc1464ca06bd07366109fab78072fcab59075073a5da6525 in / 
# Wed, 07 Dec 2022 01:51:56 GMT
CMD ["/bin/bash"]
# Wed, 07 Dec 2022 02:23:50 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 07 Dec 2022 02:23:50 GMT
ENV GOSU_VERSION=1.14
# Wed, 07 Dec 2022 02:23:52 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 07 Dec 2022 02:24:09 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False oracle-epel-release-el7; 	yum install -y --setopt=skip_missing_names_on_install=False 		bzip2 		gzip 		openssl 		xz 		zstd 	; 	yum clean all
# Wed, 07 Dec 2022 02:24:10 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 07 Dec 2022 02:24:10 GMT
ENV MYSQL_MAJOR=5.7
# Wed, 07 Dec 2022 02:24:10 GMT
ENV MYSQL_VERSION=5.7.40-1.el7
# Wed, 07 Dec 2022 02:24:11 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql5.7-server-minimal]'; 		echo 'name=MySQL 5.7 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-5.7-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 07 Dec 2022 02:24:29 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-community-server-minimal-$MYSQL_VERSION"; 	yum clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	{ echo '!includedir /etc/mysql/mysql.conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/mysql.conf.d; 		find /etc/my.cnf /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/'; 		mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 07 Dec 2022 02:24:30 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 07 Dec 2022 02:24:30 GMT
ENV MYSQL_SHELL_VERSION=8.0.31-1.el7
# Wed, 07 Dec 2022 02:24:53 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-shell-$MYSQL_SHELL_VERSION"; 	yum clean all; 		mysqlsh --version
# Wed, 07 Dec 2022 02:24:54 GMT
VOLUME [/var/lib/mysql]
# Wed, 07 Dec 2022 02:24:54 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 07 Dec 2022 02:24:55 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 07 Dec 2022 02:24:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 07 Dec 2022 02:24:55 GMT
EXPOSE 3306 33060
# Wed, 07 Dec 2022 02:24:55 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:d26998a7c52d2b84e7927f97651d1d703a805c8e4d3f658a03138721f5a5dd44`  
		Last Modified: Wed, 07 Dec 2022 01:53:46 GMT  
		Size: 49.8 MB (49818482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a9d8a3567e30df99576e0a4dbca773af581230fee203891610e6ccbdaa823d2`  
		Last Modified: Wed, 07 Dec 2022 02:26:00 GMT  
		Size: 871.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfee1f0f349e08af59ed77c7d56ede70f0c5739daa2477ef54a4ee457f5e3e47`  
		Last Modified: Wed, 07 Dec 2022 02:26:01 GMT  
		Size: 930.2 KB (930227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71ff8dfb9b12b027c35d779fe4f06a9b3d0d26efed52153324cfa2f409423b0d`  
		Last Modified: Wed, 07 Dec 2022 02:25:59 GMT  
		Size: 4.5 MB (4539026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf56cbebc916d35659623816867a456610961f77db6d9753e738c5564651dfa0`  
		Last Modified: Wed, 07 Dec 2022 02:25:58 GMT  
		Size: 2.7 KB (2658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e747e5e37d77f3d8331753fc4c4eb0b0e5af8648ee5b2eec8fa274ebdddb475`  
		Last Modified: Wed, 07 Dec 2022 02:25:58 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:711a06e512dab8bc033e74a32300e408fc4d5ab67e6db0f84942d3ddadb7376d`  
		Last Modified: Wed, 07 Dec 2022 02:26:01 GMT  
		Size: 25.5 MB (25532079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3288d68e4e9e0f5e70378db2d166bf205b73ca677bdf72384be72fa529264ed1`  
		Last Modified: Wed, 07 Dec 2022 02:25:57 GMT  
		Size: 315.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49271f2d6d157b6b14c6d6c165b3b29b8d29aef70edd653702832a48bcecf382`  
		Last Modified: Wed, 07 Dec 2022 02:26:08 GMT  
		Size: 63.4 MB (63449972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f782f6cac69ce870188610aef114b2852e9f69f2b849a4df90c0209bf8dc1717`  
		Last Modified: Wed, 07 Dec 2022 02:25:57 GMT  
		Size: 5.4 KB (5386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:701dea355691c2e0ccc548aa219fc1dd83ba44ff81843802aef25e77e813454d`  
		Last Modified: Wed, 07 Dec 2022 02:25:57 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7`

```console
$ docker pull mysql@sha256:6306f106a056e24b3a2582a59a4c84cd199907f826eff27df36406f227cd9a7d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7` - linux; amd64

```console
$ docker pull mysql@sha256:bd0fb5a175fc225ce9c2c4357c0f532bda1413e0b8555a157770f92daa5a89e0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.3 MB (144279475 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d410f4167eea912908b2f9bcc24eff870cb3c131dfb755088b79a4188bfeb40f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 07 Dec 2022 01:51:56 GMT
ADD file:3853624d773c4bf6fc1464ca06bd07366109fab78072fcab59075073a5da6525 in / 
# Wed, 07 Dec 2022 01:51:56 GMT
CMD ["/bin/bash"]
# Wed, 07 Dec 2022 02:23:50 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 07 Dec 2022 02:23:50 GMT
ENV GOSU_VERSION=1.14
# Wed, 07 Dec 2022 02:23:52 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 07 Dec 2022 02:24:09 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False oracle-epel-release-el7; 	yum install -y --setopt=skip_missing_names_on_install=False 		bzip2 		gzip 		openssl 		xz 		zstd 	; 	yum clean all
# Wed, 07 Dec 2022 02:24:10 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 07 Dec 2022 02:24:10 GMT
ENV MYSQL_MAJOR=5.7
# Wed, 07 Dec 2022 02:24:10 GMT
ENV MYSQL_VERSION=5.7.40-1.el7
# Wed, 07 Dec 2022 02:24:11 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql5.7-server-minimal]'; 		echo 'name=MySQL 5.7 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-5.7-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 07 Dec 2022 02:24:29 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-community-server-minimal-$MYSQL_VERSION"; 	yum clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	{ echo '!includedir /etc/mysql/mysql.conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/mysql.conf.d; 		find /etc/my.cnf /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/'; 		mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 07 Dec 2022 02:24:30 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 07 Dec 2022 02:24:30 GMT
ENV MYSQL_SHELL_VERSION=8.0.31-1.el7
# Wed, 07 Dec 2022 02:24:53 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-shell-$MYSQL_SHELL_VERSION"; 	yum clean all; 		mysqlsh --version
# Wed, 07 Dec 2022 02:24:54 GMT
VOLUME [/var/lib/mysql]
# Wed, 07 Dec 2022 02:24:54 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 07 Dec 2022 02:24:55 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 07 Dec 2022 02:24:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 07 Dec 2022 02:24:55 GMT
EXPOSE 3306 33060
# Wed, 07 Dec 2022 02:24:55 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:d26998a7c52d2b84e7927f97651d1d703a805c8e4d3f658a03138721f5a5dd44`  
		Last Modified: Wed, 07 Dec 2022 01:53:46 GMT  
		Size: 49.8 MB (49818482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a9d8a3567e30df99576e0a4dbca773af581230fee203891610e6ccbdaa823d2`  
		Last Modified: Wed, 07 Dec 2022 02:26:00 GMT  
		Size: 871.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfee1f0f349e08af59ed77c7d56ede70f0c5739daa2477ef54a4ee457f5e3e47`  
		Last Modified: Wed, 07 Dec 2022 02:26:01 GMT  
		Size: 930.2 KB (930227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71ff8dfb9b12b027c35d779fe4f06a9b3d0d26efed52153324cfa2f409423b0d`  
		Last Modified: Wed, 07 Dec 2022 02:25:59 GMT  
		Size: 4.5 MB (4539026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf56cbebc916d35659623816867a456610961f77db6d9753e738c5564651dfa0`  
		Last Modified: Wed, 07 Dec 2022 02:25:58 GMT  
		Size: 2.7 KB (2658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e747e5e37d77f3d8331753fc4c4eb0b0e5af8648ee5b2eec8fa274ebdddb475`  
		Last Modified: Wed, 07 Dec 2022 02:25:58 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:711a06e512dab8bc033e74a32300e408fc4d5ab67e6db0f84942d3ddadb7376d`  
		Last Modified: Wed, 07 Dec 2022 02:26:01 GMT  
		Size: 25.5 MB (25532079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3288d68e4e9e0f5e70378db2d166bf205b73ca677bdf72384be72fa529264ed1`  
		Last Modified: Wed, 07 Dec 2022 02:25:57 GMT  
		Size: 315.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49271f2d6d157b6b14c6d6c165b3b29b8d29aef70edd653702832a48bcecf382`  
		Last Modified: Wed, 07 Dec 2022 02:26:08 GMT  
		Size: 63.4 MB (63449972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f782f6cac69ce870188610aef114b2852e9f69f2b849a4df90c0209bf8dc1717`  
		Last Modified: Wed, 07 Dec 2022 02:25:57 GMT  
		Size: 5.4 KB (5386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:701dea355691c2e0ccc548aa219fc1dd83ba44ff81843802aef25e77e813454d`  
		Last Modified: Wed, 07 Dec 2022 02:25:57 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7-debian`

```console
$ docker pull mysql@sha256:c134741fc67355f1f57939624ff3e117bc0a2b0e6566fca60f85bce847a04ace
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7-debian` - linux; amd64

```console
$ docker pull mysql@sha256:c7f71d444e2a3434aede4594672722dd2e2f4e886882f5133cb2b7ee23d0e5a7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **162.6 MB (162596962 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94165850af50f5fc2c2cdf49a5c0d6e71d1408c3817eae97a681ae86b15fab19`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 21 Dec 2022 01:20:52 GMT
ADD file:660e0093a3da49e4ca41260d09d585754ccb1eff8974c4b0dd4456b76ddbbc9a in / 
# Wed, 21 Dec 2022 01:20:52 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 11:32:39 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 21 Dec 2022 11:32:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 11:32:45 GMT
ENV GOSU_VERSION=1.14
# Wed, 21 Dec 2022 11:32:54 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 21 Dec 2022 11:32:54 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 21 Dec 2022 11:33:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 11:33:02 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Wed, 21 Dec 2022 11:33:02 GMT
ENV MYSQL_MAJOR=5.7
# Wed, 21 Dec 2022 11:33:02 GMT
ENV MYSQL_VERSION=5.7.40-1debian10
# Wed, 21 Dec 2022 11:33:03 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-5.7' > /etc/apt/sources.list.d/mysql.list
# Wed, 21 Dec 2022 11:33:22 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-server="${MYSQL_VERSION}" 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Wed, 21 Dec 2022 11:33:23 GMT
VOLUME [/var/lib/mysql]
# Wed, 21 Dec 2022 11:33:23 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 21 Dec 2022 11:33:23 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 21 Dec 2022 11:33:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Dec 2022 11:33:24 GMT
EXPOSE 3306 33060
# Wed, 21 Dec 2022 11:33:24 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:b52ebda398ed2c4602ea06056f78d45a59474ee4e2a020967251ba082424e7e2`  
		Last Modified: Wed, 21 Dec 2022 01:25:17 GMT  
		Size: 27.1 MB (27140331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ce9a79d5155fd4711289385da53044c809d4e3c678327ca6d45fb6a9f4cf987`  
		Last Modified: Wed, 21 Dec 2022 11:34:31 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e261668310f535cff440b65def4e46639ea51e56eb7e29f3dcd0d2bc789dc16`  
		Last Modified: Wed, 21 Dec 2022 11:34:30 GMT  
		Size: 4.2 MB (4182322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3123e9b617f90c63e401b61f20202da262ba291624f9cf582382b6606266d4f`  
		Last Modified: Wed, 21 Dec 2022 11:34:30 GMT  
		Size: 1.4 MB (1388870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f0c53d4059e024752565a418a176ee322c7975e3573daac8543596533034c0d`  
		Last Modified: Wed, 21 Dec 2022 11:34:29 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a769258f8c5aae1218e004f37090ebf203889beee192d48cef2bc63238e41bdb`  
		Last Modified: Wed, 21 Dec 2022 11:34:32 GMT  
		Size: 14.1 MB (14089454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6478aa5af16e1946961ac5a640d2dd50637ef7f6f5a19546baf2add23b9f0930`  
		Last Modified: Wed, 21 Dec 2022 11:34:27 GMT  
		Size: 2.5 KB (2545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86a4405a4c9e0921b9c4f114716117465cab4932d55dd832a73ef363f18e4f75`  
		Last Modified: Wed, 21 Dec 2022 11:34:27 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eae9863c382483c9a8a0bc99c315132f7b91a2abdd9c8e6c4854e15a5f8770b2`  
		Last Modified: Wed, 21 Dec 2022 11:34:43 GMT  
		Size: 115.8 MB (115785799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a741ea6ad10a9767f461430b7c34fbe4cd65ce41bcd26837e7a0a32d5144aae4`  
		Last Modified: Wed, 21 Dec 2022 11:34:27 GMT  
		Size: 5.4 KB (5389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62548f9fac91770f96cdf945c008bf822f27efacd5d895c9643be71f8555485a`  
		Last Modified: Wed, 21 Dec 2022 11:34:27 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7-oracle`

```console
$ docker pull mysql@sha256:6306f106a056e24b3a2582a59a4c84cd199907f826eff27df36406f227cd9a7d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:bd0fb5a175fc225ce9c2c4357c0f532bda1413e0b8555a157770f92daa5a89e0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.3 MB (144279475 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d410f4167eea912908b2f9bcc24eff870cb3c131dfb755088b79a4188bfeb40f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 07 Dec 2022 01:51:56 GMT
ADD file:3853624d773c4bf6fc1464ca06bd07366109fab78072fcab59075073a5da6525 in / 
# Wed, 07 Dec 2022 01:51:56 GMT
CMD ["/bin/bash"]
# Wed, 07 Dec 2022 02:23:50 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 07 Dec 2022 02:23:50 GMT
ENV GOSU_VERSION=1.14
# Wed, 07 Dec 2022 02:23:52 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 07 Dec 2022 02:24:09 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False oracle-epel-release-el7; 	yum install -y --setopt=skip_missing_names_on_install=False 		bzip2 		gzip 		openssl 		xz 		zstd 	; 	yum clean all
# Wed, 07 Dec 2022 02:24:10 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 07 Dec 2022 02:24:10 GMT
ENV MYSQL_MAJOR=5.7
# Wed, 07 Dec 2022 02:24:10 GMT
ENV MYSQL_VERSION=5.7.40-1.el7
# Wed, 07 Dec 2022 02:24:11 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql5.7-server-minimal]'; 		echo 'name=MySQL 5.7 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-5.7-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 07 Dec 2022 02:24:29 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-community-server-minimal-$MYSQL_VERSION"; 	yum clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	{ echo '!includedir /etc/mysql/mysql.conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/mysql.conf.d; 		find /etc/my.cnf /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/'; 		mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 07 Dec 2022 02:24:30 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 07 Dec 2022 02:24:30 GMT
ENV MYSQL_SHELL_VERSION=8.0.31-1.el7
# Wed, 07 Dec 2022 02:24:53 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-shell-$MYSQL_SHELL_VERSION"; 	yum clean all; 		mysqlsh --version
# Wed, 07 Dec 2022 02:24:54 GMT
VOLUME [/var/lib/mysql]
# Wed, 07 Dec 2022 02:24:54 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 07 Dec 2022 02:24:55 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 07 Dec 2022 02:24:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 07 Dec 2022 02:24:55 GMT
EXPOSE 3306 33060
# Wed, 07 Dec 2022 02:24:55 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:d26998a7c52d2b84e7927f97651d1d703a805c8e4d3f658a03138721f5a5dd44`  
		Last Modified: Wed, 07 Dec 2022 01:53:46 GMT  
		Size: 49.8 MB (49818482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a9d8a3567e30df99576e0a4dbca773af581230fee203891610e6ccbdaa823d2`  
		Last Modified: Wed, 07 Dec 2022 02:26:00 GMT  
		Size: 871.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfee1f0f349e08af59ed77c7d56ede70f0c5739daa2477ef54a4ee457f5e3e47`  
		Last Modified: Wed, 07 Dec 2022 02:26:01 GMT  
		Size: 930.2 KB (930227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71ff8dfb9b12b027c35d779fe4f06a9b3d0d26efed52153324cfa2f409423b0d`  
		Last Modified: Wed, 07 Dec 2022 02:25:59 GMT  
		Size: 4.5 MB (4539026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf56cbebc916d35659623816867a456610961f77db6d9753e738c5564651dfa0`  
		Last Modified: Wed, 07 Dec 2022 02:25:58 GMT  
		Size: 2.7 KB (2658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e747e5e37d77f3d8331753fc4c4eb0b0e5af8648ee5b2eec8fa274ebdddb475`  
		Last Modified: Wed, 07 Dec 2022 02:25:58 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:711a06e512dab8bc033e74a32300e408fc4d5ab67e6db0f84942d3ddadb7376d`  
		Last Modified: Wed, 07 Dec 2022 02:26:01 GMT  
		Size: 25.5 MB (25532079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3288d68e4e9e0f5e70378db2d166bf205b73ca677bdf72384be72fa529264ed1`  
		Last Modified: Wed, 07 Dec 2022 02:25:57 GMT  
		Size: 315.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49271f2d6d157b6b14c6d6c165b3b29b8d29aef70edd653702832a48bcecf382`  
		Last Modified: Wed, 07 Dec 2022 02:26:08 GMT  
		Size: 63.4 MB (63449972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f782f6cac69ce870188610aef114b2852e9f69f2b849a4df90c0209bf8dc1717`  
		Last Modified: Wed, 07 Dec 2022 02:25:57 GMT  
		Size: 5.4 KB (5386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:701dea355691c2e0ccc548aa219fc1dd83ba44ff81843802aef25e77e813454d`  
		Last Modified: Wed, 07 Dec 2022 02:25:57 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7.40`

```console
$ docker pull mysql@sha256:6306f106a056e24b3a2582a59a4c84cd199907f826eff27df36406f227cd9a7d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7.40` - linux; amd64

```console
$ docker pull mysql@sha256:bd0fb5a175fc225ce9c2c4357c0f532bda1413e0b8555a157770f92daa5a89e0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.3 MB (144279475 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d410f4167eea912908b2f9bcc24eff870cb3c131dfb755088b79a4188bfeb40f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 07 Dec 2022 01:51:56 GMT
ADD file:3853624d773c4bf6fc1464ca06bd07366109fab78072fcab59075073a5da6525 in / 
# Wed, 07 Dec 2022 01:51:56 GMT
CMD ["/bin/bash"]
# Wed, 07 Dec 2022 02:23:50 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 07 Dec 2022 02:23:50 GMT
ENV GOSU_VERSION=1.14
# Wed, 07 Dec 2022 02:23:52 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 07 Dec 2022 02:24:09 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False oracle-epel-release-el7; 	yum install -y --setopt=skip_missing_names_on_install=False 		bzip2 		gzip 		openssl 		xz 		zstd 	; 	yum clean all
# Wed, 07 Dec 2022 02:24:10 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 07 Dec 2022 02:24:10 GMT
ENV MYSQL_MAJOR=5.7
# Wed, 07 Dec 2022 02:24:10 GMT
ENV MYSQL_VERSION=5.7.40-1.el7
# Wed, 07 Dec 2022 02:24:11 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql5.7-server-minimal]'; 		echo 'name=MySQL 5.7 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-5.7-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 07 Dec 2022 02:24:29 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-community-server-minimal-$MYSQL_VERSION"; 	yum clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	{ echo '!includedir /etc/mysql/mysql.conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/mysql.conf.d; 		find /etc/my.cnf /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/'; 		mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 07 Dec 2022 02:24:30 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 07 Dec 2022 02:24:30 GMT
ENV MYSQL_SHELL_VERSION=8.0.31-1.el7
# Wed, 07 Dec 2022 02:24:53 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-shell-$MYSQL_SHELL_VERSION"; 	yum clean all; 		mysqlsh --version
# Wed, 07 Dec 2022 02:24:54 GMT
VOLUME [/var/lib/mysql]
# Wed, 07 Dec 2022 02:24:54 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 07 Dec 2022 02:24:55 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 07 Dec 2022 02:24:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 07 Dec 2022 02:24:55 GMT
EXPOSE 3306 33060
# Wed, 07 Dec 2022 02:24:55 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:d26998a7c52d2b84e7927f97651d1d703a805c8e4d3f658a03138721f5a5dd44`  
		Last Modified: Wed, 07 Dec 2022 01:53:46 GMT  
		Size: 49.8 MB (49818482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a9d8a3567e30df99576e0a4dbca773af581230fee203891610e6ccbdaa823d2`  
		Last Modified: Wed, 07 Dec 2022 02:26:00 GMT  
		Size: 871.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfee1f0f349e08af59ed77c7d56ede70f0c5739daa2477ef54a4ee457f5e3e47`  
		Last Modified: Wed, 07 Dec 2022 02:26:01 GMT  
		Size: 930.2 KB (930227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71ff8dfb9b12b027c35d779fe4f06a9b3d0d26efed52153324cfa2f409423b0d`  
		Last Modified: Wed, 07 Dec 2022 02:25:59 GMT  
		Size: 4.5 MB (4539026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf56cbebc916d35659623816867a456610961f77db6d9753e738c5564651dfa0`  
		Last Modified: Wed, 07 Dec 2022 02:25:58 GMT  
		Size: 2.7 KB (2658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e747e5e37d77f3d8331753fc4c4eb0b0e5af8648ee5b2eec8fa274ebdddb475`  
		Last Modified: Wed, 07 Dec 2022 02:25:58 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:711a06e512dab8bc033e74a32300e408fc4d5ab67e6db0f84942d3ddadb7376d`  
		Last Modified: Wed, 07 Dec 2022 02:26:01 GMT  
		Size: 25.5 MB (25532079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3288d68e4e9e0f5e70378db2d166bf205b73ca677bdf72384be72fa529264ed1`  
		Last Modified: Wed, 07 Dec 2022 02:25:57 GMT  
		Size: 315.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49271f2d6d157b6b14c6d6c165b3b29b8d29aef70edd653702832a48bcecf382`  
		Last Modified: Wed, 07 Dec 2022 02:26:08 GMT  
		Size: 63.4 MB (63449972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f782f6cac69ce870188610aef114b2852e9f69f2b849a4df90c0209bf8dc1717`  
		Last Modified: Wed, 07 Dec 2022 02:25:57 GMT  
		Size: 5.4 KB (5386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:701dea355691c2e0ccc548aa219fc1dd83ba44ff81843802aef25e77e813454d`  
		Last Modified: Wed, 07 Dec 2022 02:25:57 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7.40-debian`

```console
$ docker pull mysql@sha256:c134741fc67355f1f57939624ff3e117bc0a2b0e6566fca60f85bce847a04ace
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7.40-debian` - linux; amd64

```console
$ docker pull mysql@sha256:c7f71d444e2a3434aede4594672722dd2e2f4e886882f5133cb2b7ee23d0e5a7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **162.6 MB (162596962 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94165850af50f5fc2c2cdf49a5c0d6e71d1408c3817eae97a681ae86b15fab19`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 21 Dec 2022 01:20:52 GMT
ADD file:660e0093a3da49e4ca41260d09d585754ccb1eff8974c4b0dd4456b76ddbbc9a in / 
# Wed, 21 Dec 2022 01:20:52 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 11:32:39 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 21 Dec 2022 11:32:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 11:32:45 GMT
ENV GOSU_VERSION=1.14
# Wed, 21 Dec 2022 11:32:54 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 21 Dec 2022 11:32:54 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 21 Dec 2022 11:33:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 11:33:02 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Wed, 21 Dec 2022 11:33:02 GMT
ENV MYSQL_MAJOR=5.7
# Wed, 21 Dec 2022 11:33:02 GMT
ENV MYSQL_VERSION=5.7.40-1debian10
# Wed, 21 Dec 2022 11:33:03 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ buster mysql-5.7' > /etc/apt/sources.list.d/mysql.list
# Wed, 21 Dec 2022 11:33:22 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-server="${MYSQL_VERSION}" 	&& find /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/' 	&& echo '[mysqld]\nskip-host-cache\nskip-name-resolve' > /etc/mysql/conf.d/docker.cnf 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Wed, 21 Dec 2022 11:33:23 GMT
VOLUME [/var/lib/mysql]
# Wed, 21 Dec 2022 11:33:23 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 21 Dec 2022 11:33:23 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 21 Dec 2022 11:33:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Dec 2022 11:33:24 GMT
EXPOSE 3306 33060
# Wed, 21 Dec 2022 11:33:24 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:b52ebda398ed2c4602ea06056f78d45a59474ee4e2a020967251ba082424e7e2`  
		Last Modified: Wed, 21 Dec 2022 01:25:17 GMT  
		Size: 27.1 MB (27140331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ce9a79d5155fd4711289385da53044c809d4e3c678327ca6d45fb6a9f4cf987`  
		Last Modified: Wed, 21 Dec 2022 11:34:31 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e261668310f535cff440b65def4e46639ea51e56eb7e29f3dcd0d2bc789dc16`  
		Last Modified: Wed, 21 Dec 2022 11:34:30 GMT  
		Size: 4.2 MB (4182322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3123e9b617f90c63e401b61f20202da262ba291624f9cf582382b6606266d4f`  
		Last Modified: Wed, 21 Dec 2022 11:34:30 GMT  
		Size: 1.4 MB (1388870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f0c53d4059e024752565a418a176ee322c7975e3573daac8543596533034c0d`  
		Last Modified: Wed, 21 Dec 2022 11:34:29 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a769258f8c5aae1218e004f37090ebf203889beee192d48cef2bc63238e41bdb`  
		Last Modified: Wed, 21 Dec 2022 11:34:32 GMT  
		Size: 14.1 MB (14089454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6478aa5af16e1946961ac5a640d2dd50637ef7f6f5a19546baf2add23b9f0930`  
		Last Modified: Wed, 21 Dec 2022 11:34:27 GMT  
		Size: 2.5 KB (2545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86a4405a4c9e0921b9c4f114716117465cab4932d55dd832a73ef363f18e4f75`  
		Last Modified: Wed, 21 Dec 2022 11:34:27 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eae9863c382483c9a8a0bc99c315132f7b91a2abdd9c8e6c4854e15a5f8770b2`  
		Last Modified: Wed, 21 Dec 2022 11:34:43 GMT  
		Size: 115.8 MB (115785799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a741ea6ad10a9767f461430b7c34fbe4cd65ce41bcd26837e7a0a32d5144aae4`  
		Last Modified: Wed, 21 Dec 2022 11:34:27 GMT  
		Size: 5.4 KB (5389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62548f9fac91770f96cdf945c008bf822f27efacd5d895c9643be71f8555485a`  
		Last Modified: Wed, 21 Dec 2022 11:34:27 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:5.7.40-oracle`

```console
$ docker pull mysql@sha256:6306f106a056e24b3a2582a59a4c84cd199907f826eff27df36406f227cd9a7d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5.7.40-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:bd0fb5a175fc225ce9c2c4357c0f532bda1413e0b8555a157770f92daa5a89e0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.3 MB (144279475 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d410f4167eea912908b2f9bcc24eff870cb3c131dfb755088b79a4188bfeb40f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 07 Dec 2022 01:51:56 GMT
ADD file:3853624d773c4bf6fc1464ca06bd07366109fab78072fcab59075073a5da6525 in / 
# Wed, 07 Dec 2022 01:51:56 GMT
CMD ["/bin/bash"]
# Wed, 07 Dec 2022 02:23:50 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 07 Dec 2022 02:23:50 GMT
ENV GOSU_VERSION=1.14
# Wed, 07 Dec 2022 02:23:52 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 07 Dec 2022 02:24:09 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False oracle-epel-release-el7; 	yum install -y --setopt=skip_missing_names_on_install=False 		bzip2 		gzip 		openssl 		xz 		zstd 	; 	yum clean all
# Wed, 07 Dec 2022 02:24:10 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 07 Dec 2022 02:24:10 GMT
ENV MYSQL_MAJOR=5.7
# Wed, 07 Dec 2022 02:24:10 GMT
ENV MYSQL_VERSION=5.7.40-1.el7
# Wed, 07 Dec 2022 02:24:11 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql5.7-server-minimal]'; 		echo 'name=MySQL 5.7 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-5.7-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 07 Dec 2022 02:24:29 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-community-server-minimal-$MYSQL_VERSION"; 	yum clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	{ echo '!includedir /etc/mysql/mysql.conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/mysql.conf.d; 		find /etc/my.cnf /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/'; 		mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 07 Dec 2022 02:24:30 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 07 Dec 2022 02:24:30 GMT
ENV MYSQL_SHELL_VERSION=8.0.31-1.el7
# Wed, 07 Dec 2022 02:24:53 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-shell-$MYSQL_SHELL_VERSION"; 	yum clean all; 		mysqlsh --version
# Wed, 07 Dec 2022 02:24:54 GMT
VOLUME [/var/lib/mysql]
# Wed, 07 Dec 2022 02:24:54 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 07 Dec 2022 02:24:55 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 07 Dec 2022 02:24:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 07 Dec 2022 02:24:55 GMT
EXPOSE 3306 33060
# Wed, 07 Dec 2022 02:24:55 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:d26998a7c52d2b84e7927f97651d1d703a805c8e4d3f658a03138721f5a5dd44`  
		Last Modified: Wed, 07 Dec 2022 01:53:46 GMT  
		Size: 49.8 MB (49818482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a9d8a3567e30df99576e0a4dbca773af581230fee203891610e6ccbdaa823d2`  
		Last Modified: Wed, 07 Dec 2022 02:26:00 GMT  
		Size: 871.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfee1f0f349e08af59ed77c7d56ede70f0c5739daa2477ef54a4ee457f5e3e47`  
		Last Modified: Wed, 07 Dec 2022 02:26:01 GMT  
		Size: 930.2 KB (930227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71ff8dfb9b12b027c35d779fe4f06a9b3d0d26efed52153324cfa2f409423b0d`  
		Last Modified: Wed, 07 Dec 2022 02:25:59 GMT  
		Size: 4.5 MB (4539026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf56cbebc916d35659623816867a456610961f77db6d9753e738c5564651dfa0`  
		Last Modified: Wed, 07 Dec 2022 02:25:58 GMT  
		Size: 2.7 KB (2658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e747e5e37d77f3d8331753fc4c4eb0b0e5af8648ee5b2eec8fa274ebdddb475`  
		Last Modified: Wed, 07 Dec 2022 02:25:58 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:711a06e512dab8bc033e74a32300e408fc4d5ab67e6db0f84942d3ddadb7376d`  
		Last Modified: Wed, 07 Dec 2022 02:26:01 GMT  
		Size: 25.5 MB (25532079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3288d68e4e9e0f5e70378db2d166bf205b73ca677bdf72384be72fa529264ed1`  
		Last Modified: Wed, 07 Dec 2022 02:25:57 GMT  
		Size: 315.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49271f2d6d157b6b14c6d6c165b3b29b8d29aef70edd653702832a48bcecf382`  
		Last Modified: Wed, 07 Dec 2022 02:26:08 GMT  
		Size: 63.4 MB (63449972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f782f6cac69ce870188610aef114b2852e9f69f2b849a4df90c0209bf8dc1717`  
		Last Modified: Wed, 07 Dec 2022 02:25:57 GMT  
		Size: 5.4 KB (5386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:701dea355691c2e0ccc548aa219fc1dd83ba44ff81843802aef25e77e813454d`  
		Last Modified: Wed, 07 Dec 2022 02:25:57 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8`

```console
$ docker pull mysql@sha256:3d7ae561cf6095f6aca8eb7830e1d14734227b1fb4748092f2be2cfbccf7d614
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8` - linux; amd64

```console
$ docker pull mysql@sha256:cfddf275c8b1ae1583c0f6afb4899d4dbe14111a6462699559a1f4dc8f4d5f6e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **160.6 MB (160585430 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7484689f290f1defe06b65befc54cb6ad91a667cf0af59a265ffe76c46bd0478`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 07 Dec 2022 01:51:27 GMT
ADD file:04d9ae26c2acac414b69a784563f765d531aeaf941ea0341025b4544f9ade244 in / 
# Wed, 07 Dec 2022 01:51:27 GMT
CMD ["/bin/bash"]
# Wed, 07 Dec 2022 02:21:54 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 07 Dec 2022 02:21:55 GMT
ENV GOSU_VERSION=1.14
# Wed, 07 Dec 2022 02:21:58 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 07 Dec 2022 02:22:21 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Wed, 07 Dec 2022 02:22:22 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 07 Dec 2022 02:22:23 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 07 Dec 2022 02:22:23 GMT
ENV MYSQL_VERSION=8.0.31-1.el8
# Wed, 07 Dec 2022 02:22:23 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 07 Dec 2022 02:22:53 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 07 Dec 2022 02:22:54 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 07 Dec 2022 02:22:54 GMT
ENV MYSQL_SHELL_VERSION=8.0.31-1.el8
# Wed, 07 Dec 2022 02:23:29 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Wed, 07 Dec 2022 02:23:30 GMT
VOLUME [/var/lib/mysql]
# Wed, 07 Dec 2022 02:23:30 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 07 Dec 2022 02:23:31 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 07 Dec 2022 02:23:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 07 Dec 2022 02:23:31 GMT
EXPOSE 3306 33060
# Wed, 07 Dec 2022 02:23:31 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:0ed027b72ddc5d1a749fc58b7c26610167393b08ae71ef6625496508903f70a2`  
		Last Modified: Wed, 07 Dec 2022 01:53:11 GMT  
		Size: 43.9 MB (43868738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0296159747f12f208fbf9721970ca290348698ac443cf98311477b6e44f18acc`  
		Last Modified: Wed, 07 Dec 2022 02:25:25 GMT  
		Size: 886.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d2f9b664bd354b5b8823bbdda42cf0813f2d8d3b5693f952c0a8516af84a826`  
		Last Modified: Wed, 07 Dec 2022 02:25:25 GMT  
		Size: 928.8 KB (928835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df6519f81c2689152b478834162cfe2f21ef37c472108a3e3a03a6ac0f5cbdd9`  
		Last Modified: Wed, 07 Dec 2022 02:25:24 GMT  
		Size: 4.6 MB (4608004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36bb5e56d458a7652c87ab8c3909c0ad098feaa81e73649bb37704701ca3ee6d`  
		Last Modified: Wed, 07 Dec 2022 02:25:23 GMT  
		Size: 2.6 KB (2630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:054e8fde88d0e345bf3d5a7bb06dd62c56cc5b26713a0a27223e54f849a28d2c`  
		Last Modified: Wed, 07 Dec 2022 02:25:23 GMT  
		Size: 332.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2b494c50c7f5297000bd4e8bd09e9dbf84d44ffc5eb3e5028701db6a6749117`  
		Last Modified: Wed, 07 Dec 2022 02:25:30 GMT  
		Size: 56.1 MB (56063632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:132bc0d471b8b86912c8fff2877e1b2fcab03fdcbefa81630f33cb60ba5455c7`  
		Last Modified: Wed, 07 Dec 2022 02:25:21 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:135ec7033a05d2a5153f07e0b7983246a867df3c29a0fafc5ae47c90c35a1bf4`  
		Last Modified: Wed, 07 Dec 2022 02:25:31 GMT  
		Size: 55.1 MB (55106545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5961f02724723ffcd87c7e08efc9beb635496e32e530de0976755bf24843153b`  
		Last Modified: Wed, 07 Dec 2022 02:25:21 GMT  
		Size: 5.4 KB (5391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75b5f7a3d3a49109ed3673860a5c5ed0f3f070b099b59dfc9b1c45761ca1aaca`  
		Last Modified: Wed, 07 Dec 2022 02:25:21 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:abd7d1e4a42b96a58c702db2633df611d201789b07c01749dac1aff97b83ba8f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **159.0 MB (159024595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b6f3978ca2905ae9bc14cfe86ae2f004f8c36561b722a06f64b73001b1898a5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 07 Dec 2022 02:10:44 GMT
ADD file:6fdd782c2779edf7149126e79dcb46ebde32975107cdd5d129cce0860e797cde in / 
# Wed, 07 Dec 2022 02:10:44 GMT
CMD ["/bin/bash"]
# Wed, 07 Dec 2022 02:50:18 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 07 Dec 2022 02:50:18 GMT
ENV GOSU_VERSION=1.14
# Wed, 07 Dec 2022 02:50:22 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 07 Dec 2022 02:50:43 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Wed, 07 Dec 2022 02:50:44 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 07 Dec 2022 02:50:44 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 07 Dec 2022 02:50:44 GMT
ENV MYSQL_VERSION=8.0.31-1.el8
# Wed, 07 Dec 2022 02:50:44 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 07 Dec 2022 02:51:09 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 07 Dec 2022 02:51:10 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 07 Dec 2022 02:51:10 GMT
ENV MYSQL_SHELL_VERSION=8.0.31-1.el8
# Wed, 07 Dec 2022 02:51:38 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Wed, 07 Dec 2022 02:51:39 GMT
VOLUME [/var/lib/mysql]
# Wed, 07 Dec 2022 02:51:39 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 07 Dec 2022 02:51:40 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 07 Dec 2022 02:51:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 07 Dec 2022 02:51:40 GMT
EXPOSE 3306 33060
# Wed, 07 Dec 2022 02:51:40 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:12a06ca91af857ea3cb02aedc5c643c5f06865868ae5c386c8ea664be60ead7e`  
		Last Modified: Wed, 07 Dec 2022 02:12:09 GMT  
		Size: 42.8 MB (42772059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fec1cb1944f64443d61a29e94cddba36d0cb8a09c80e0247375445bc62b842e`  
		Last Modified: Wed, 07 Dec 2022 02:52:10 GMT  
		Size: 887.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aede38c79379349fd3e9d191f92be36e68adc230840ae21c015f166b96e2067a`  
		Last Modified: Wed, 07 Dec 2022 02:52:10 GMT  
		Size: 857.2 KB (857168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51b980849561d1ed6bffe5deb621498e150f4f0f148af7a2654dd90ed42d7bfb`  
		Last Modified: Wed, 07 Dec 2022 02:52:09 GMT  
		Size: 4.5 MB (4464908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f503d79ed4bc3c439b28068291b1260757ab2de86163c8954962d88ff917e22a`  
		Last Modified: Wed, 07 Dec 2022 02:52:08 GMT  
		Size: 2.6 KB (2624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fb44db361f7e1027fb0010e8a3447c6e9337f6685ab4901f57030d01f730f74`  
		Last Modified: Wed, 07 Dec 2022 02:52:08 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:943b6dcee7dec15078e15da5cf8750748ae482bd7f5f206ecee44f5627229836`  
		Last Modified: Wed, 07 Dec 2022 02:52:13 GMT  
		Size: 55.4 MB (55444877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:911277c1fe4b4a08873f70cde5b84e7b38fd3d1c31c9c884baff83bd23886c96`  
		Last Modified: Wed, 07 Dec 2022 02:52:06 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a477017d045777c9cc1150499a65250c49ffd0669c2fa9fa8b64fb9e73cd353c`  
		Last Modified: Wed, 07 Dec 2022 02:52:14 GMT  
		Size: 55.5 MB (55475909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84b5061403a5151af9ccac6299ba1e8037c8f7a049dcc22e8808fd0095566e88`  
		Last Modified: Wed, 07 Dec 2022 02:52:06 GMT  
		Size: 5.4 KB (5392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ff27d035d66da6c178b69b95ddb8d8e913e206938df13d13dc0de764684b8c5`  
		Last Modified: Wed, 07 Dec 2022 02:52:06 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8-debian`

```console
$ docker pull mysql@sha256:e0a793ddd093df31139fc695ed889fdd3ec910c76ddf3186683efe2d67a2ba96
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:8-debian` - linux; amd64

```console
$ docker pull mysql@sha256:ac248facf748e93a1022552d4f15311ef8bd8be7ba841305a1b404ed59196de6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **177.5 MB (177548446 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3b748431f76159ff04ec985c63bf42dae5206be3aee4e1d244182b297299354`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 21 Dec 2022 01:20:32 GMT
ADD file:73e68ae6852c9afbb2989dc9c5b7c6668843f454b1bdcfb48658bfbc6c4af69e in / 
# Wed, 21 Dec 2022 01:20:33 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 11:31:49 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 21 Dec 2022 11:31:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 11:31:55 GMT
ENV GOSU_VERSION=1.14
# Wed, 21 Dec 2022 11:32:03 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 21 Dec 2022 11:32:04 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 21 Dec 2022 11:32:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 11:32:10 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Wed, 21 Dec 2022 11:32:10 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 21 Dec 2022 11:32:11 GMT
ENV MYSQL_VERSION=8.0.31-1debian11
# Wed, 21 Dec 2022 11:32:11 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ bullseye mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Wed, 21 Dec 2022 11:32:26 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Wed, 21 Dec 2022 11:32:27 GMT
VOLUME [/var/lib/mysql]
# Wed, 21 Dec 2022 11:32:27 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Wed, 21 Dec 2022 11:32:27 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 21 Dec 2022 11:32:28 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 21 Dec 2022 11:32:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Dec 2022 11:32:28 GMT
EXPOSE 3306 33060
# Wed, 21 Dec 2022 11:32:28 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:3f4ca61aafcd4fc07267a105067db35c0f0ac630e1970f3cd0c7bf552780e985`  
		Last Modified: Wed, 21 Dec 2022 01:24:36 GMT  
		Size: 31.4 MB (31396943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c71b14b90321c4c925c97bde825eb21b3c97f7f6b9f73ad028c29bf93347ee2`  
		Last Modified: Wed, 21 Dec 2022 11:33:54 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b20239cd5b3eb4255955404db9ddf231a20a91b74c52e8ae82513e70d75e84a`  
		Last Modified: Wed, 21 Dec 2022 11:33:55 GMT  
		Size: 4.4 MB (4414844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69a92a8be7b81fc7d582c733edcb95ffe26bd8ff252e05167b70b896561c550a`  
		Last Modified: Wed, 21 Dec 2022 11:33:53 GMT  
		Size: 1.4 MB (1418501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed87af8210d03be6cf68e7ddc53ca53f0b7cb5d2526d8b350a6499f0b09d7b7f`  
		Last Modified: Wed, 21 Dec 2022 11:33:52 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89326f0fbca735cd9db355568c579a062d4e4f1a151dee777fca6739679c8559`  
		Last Modified: Wed, 21 Dec 2022 11:33:55 GMT  
		Size: 12.7 MB (12662005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2d532ea748ea86b00b0defbd158232a20f45862f4693dd6967e7ed4f379c57f`  
		Last Modified: Wed, 21 Dec 2022 11:33:52 GMT  
		Size: 2.5 KB (2545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46e4e09af7ec7aa3580ada1847200f65da4879d557475f2f356c43d6f2200669`  
		Last Modified: Wed, 21 Dec 2022 11:33:51 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d62f3c764f6b95a24939111413263a1dd1e0ffcf895cb6757b4aff64a412340`  
		Last Modified: Wed, 21 Dec 2022 11:34:10 GMT  
		Size: 127.6 MB (127645114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edad28c75e273ba1d4fade07eba864f0ad81767b605529a4918c6d6aa8b4a2ba`  
		Last Modified: Wed, 21 Dec 2022 11:33:51 GMT  
		Size: 846.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a2005ac0b2c3804a85b1ef7cfc06d078e2ecce524d07697c9f58f811367b26e`  
		Last Modified: Wed, 21 Dec 2022 11:33:51 GMT  
		Size: 5.4 KB (5391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ff97e27ba8e3f53c701cbd1841c5e91dfe25863598c0d09302e83871f2b344e`  
		Last Modified: Wed, 21 Dec 2022 11:33:51 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8-oracle`

```console
$ docker pull mysql@sha256:3d7ae561cf6095f6aca8eb7830e1d14734227b1fb4748092f2be2cfbccf7d614
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:cfddf275c8b1ae1583c0f6afb4899d4dbe14111a6462699559a1f4dc8f4d5f6e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **160.6 MB (160585430 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7484689f290f1defe06b65befc54cb6ad91a667cf0af59a265ffe76c46bd0478`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 07 Dec 2022 01:51:27 GMT
ADD file:04d9ae26c2acac414b69a784563f765d531aeaf941ea0341025b4544f9ade244 in / 
# Wed, 07 Dec 2022 01:51:27 GMT
CMD ["/bin/bash"]
# Wed, 07 Dec 2022 02:21:54 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 07 Dec 2022 02:21:55 GMT
ENV GOSU_VERSION=1.14
# Wed, 07 Dec 2022 02:21:58 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 07 Dec 2022 02:22:21 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Wed, 07 Dec 2022 02:22:22 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 07 Dec 2022 02:22:23 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 07 Dec 2022 02:22:23 GMT
ENV MYSQL_VERSION=8.0.31-1.el8
# Wed, 07 Dec 2022 02:22:23 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 07 Dec 2022 02:22:53 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 07 Dec 2022 02:22:54 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 07 Dec 2022 02:22:54 GMT
ENV MYSQL_SHELL_VERSION=8.0.31-1.el8
# Wed, 07 Dec 2022 02:23:29 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Wed, 07 Dec 2022 02:23:30 GMT
VOLUME [/var/lib/mysql]
# Wed, 07 Dec 2022 02:23:30 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 07 Dec 2022 02:23:31 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 07 Dec 2022 02:23:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 07 Dec 2022 02:23:31 GMT
EXPOSE 3306 33060
# Wed, 07 Dec 2022 02:23:31 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:0ed027b72ddc5d1a749fc58b7c26610167393b08ae71ef6625496508903f70a2`  
		Last Modified: Wed, 07 Dec 2022 01:53:11 GMT  
		Size: 43.9 MB (43868738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0296159747f12f208fbf9721970ca290348698ac443cf98311477b6e44f18acc`  
		Last Modified: Wed, 07 Dec 2022 02:25:25 GMT  
		Size: 886.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d2f9b664bd354b5b8823bbdda42cf0813f2d8d3b5693f952c0a8516af84a826`  
		Last Modified: Wed, 07 Dec 2022 02:25:25 GMT  
		Size: 928.8 KB (928835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df6519f81c2689152b478834162cfe2f21ef37c472108a3e3a03a6ac0f5cbdd9`  
		Last Modified: Wed, 07 Dec 2022 02:25:24 GMT  
		Size: 4.6 MB (4608004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36bb5e56d458a7652c87ab8c3909c0ad098feaa81e73649bb37704701ca3ee6d`  
		Last Modified: Wed, 07 Dec 2022 02:25:23 GMT  
		Size: 2.6 KB (2630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:054e8fde88d0e345bf3d5a7bb06dd62c56cc5b26713a0a27223e54f849a28d2c`  
		Last Modified: Wed, 07 Dec 2022 02:25:23 GMT  
		Size: 332.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2b494c50c7f5297000bd4e8bd09e9dbf84d44ffc5eb3e5028701db6a6749117`  
		Last Modified: Wed, 07 Dec 2022 02:25:30 GMT  
		Size: 56.1 MB (56063632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:132bc0d471b8b86912c8fff2877e1b2fcab03fdcbefa81630f33cb60ba5455c7`  
		Last Modified: Wed, 07 Dec 2022 02:25:21 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:135ec7033a05d2a5153f07e0b7983246a867df3c29a0fafc5ae47c90c35a1bf4`  
		Last Modified: Wed, 07 Dec 2022 02:25:31 GMT  
		Size: 55.1 MB (55106545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5961f02724723ffcd87c7e08efc9beb635496e32e530de0976755bf24843153b`  
		Last Modified: Wed, 07 Dec 2022 02:25:21 GMT  
		Size: 5.4 KB (5391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75b5f7a3d3a49109ed3673860a5c5ed0f3f070b099b59dfc9b1c45761ca1aaca`  
		Last Modified: Wed, 07 Dec 2022 02:25:21 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8-oracle` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:abd7d1e4a42b96a58c702db2633df611d201789b07c01749dac1aff97b83ba8f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **159.0 MB (159024595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b6f3978ca2905ae9bc14cfe86ae2f004f8c36561b722a06f64b73001b1898a5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 07 Dec 2022 02:10:44 GMT
ADD file:6fdd782c2779edf7149126e79dcb46ebde32975107cdd5d129cce0860e797cde in / 
# Wed, 07 Dec 2022 02:10:44 GMT
CMD ["/bin/bash"]
# Wed, 07 Dec 2022 02:50:18 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 07 Dec 2022 02:50:18 GMT
ENV GOSU_VERSION=1.14
# Wed, 07 Dec 2022 02:50:22 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 07 Dec 2022 02:50:43 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Wed, 07 Dec 2022 02:50:44 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 07 Dec 2022 02:50:44 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 07 Dec 2022 02:50:44 GMT
ENV MYSQL_VERSION=8.0.31-1.el8
# Wed, 07 Dec 2022 02:50:44 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 07 Dec 2022 02:51:09 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 07 Dec 2022 02:51:10 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 07 Dec 2022 02:51:10 GMT
ENV MYSQL_SHELL_VERSION=8.0.31-1.el8
# Wed, 07 Dec 2022 02:51:38 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Wed, 07 Dec 2022 02:51:39 GMT
VOLUME [/var/lib/mysql]
# Wed, 07 Dec 2022 02:51:39 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 07 Dec 2022 02:51:40 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 07 Dec 2022 02:51:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 07 Dec 2022 02:51:40 GMT
EXPOSE 3306 33060
# Wed, 07 Dec 2022 02:51:40 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:12a06ca91af857ea3cb02aedc5c643c5f06865868ae5c386c8ea664be60ead7e`  
		Last Modified: Wed, 07 Dec 2022 02:12:09 GMT  
		Size: 42.8 MB (42772059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fec1cb1944f64443d61a29e94cddba36d0cb8a09c80e0247375445bc62b842e`  
		Last Modified: Wed, 07 Dec 2022 02:52:10 GMT  
		Size: 887.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aede38c79379349fd3e9d191f92be36e68adc230840ae21c015f166b96e2067a`  
		Last Modified: Wed, 07 Dec 2022 02:52:10 GMT  
		Size: 857.2 KB (857168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51b980849561d1ed6bffe5deb621498e150f4f0f148af7a2654dd90ed42d7bfb`  
		Last Modified: Wed, 07 Dec 2022 02:52:09 GMT  
		Size: 4.5 MB (4464908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f503d79ed4bc3c439b28068291b1260757ab2de86163c8954962d88ff917e22a`  
		Last Modified: Wed, 07 Dec 2022 02:52:08 GMT  
		Size: 2.6 KB (2624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fb44db361f7e1027fb0010e8a3447c6e9337f6685ab4901f57030d01f730f74`  
		Last Modified: Wed, 07 Dec 2022 02:52:08 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:943b6dcee7dec15078e15da5cf8750748ae482bd7f5f206ecee44f5627229836`  
		Last Modified: Wed, 07 Dec 2022 02:52:13 GMT  
		Size: 55.4 MB (55444877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:911277c1fe4b4a08873f70cde5b84e7b38fd3d1c31c9c884baff83bd23886c96`  
		Last Modified: Wed, 07 Dec 2022 02:52:06 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a477017d045777c9cc1150499a65250c49ffd0669c2fa9fa8b64fb9e73cd353c`  
		Last Modified: Wed, 07 Dec 2022 02:52:14 GMT  
		Size: 55.5 MB (55475909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84b5061403a5151af9ccac6299ba1e8037c8f7a049dcc22e8808fd0095566e88`  
		Last Modified: Wed, 07 Dec 2022 02:52:06 GMT  
		Size: 5.4 KB (5392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ff27d035d66da6c178b69b95ddb8d8e913e206938df13d13dc0de764684b8c5`  
		Last Modified: Wed, 07 Dec 2022 02:52:06 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0`

```console
$ docker pull mysql@sha256:3d7ae561cf6095f6aca8eb7830e1d14734227b1fb4748092f2be2cfbccf7d614
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8.0` - linux; amd64

```console
$ docker pull mysql@sha256:cfddf275c8b1ae1583c0f6afb4899d4dbe14111a6462699559a1f4dc8f4d5f6e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **160.6 MB (160585430 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7484689f290f1defe06b65befc54cb6ad91a667cf0af59a265ffe76c46bd0478`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 07 Dec 2022 01:51:27 GMT
ADD file:04d9ae26c2acac414b69a784563f765d531aeaf941ea0341025b4544f9ade244 in / 
# Wed, 07 Dec 2022 01:51:27 GMT
CMD ["/bin/bash"]
# Wed, 07 Dec 2022 02:21:54 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 07 Dec 2022 02:21:55 GMT
ENV GOSU_VERSION=1.14
# Wed, 07 Dec 2022 02:21:58 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 07 Dec 2022 02:22:21 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Wed, 07 Dec 2022 02:22:22 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 07 Dec 2022 02:22:23 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 07 Dec 2022 02:22:23 GMT
ENV MYSQL_VERSION=8.0.31-1.el8
# Wed, 07 Dec 2022 02:22:23 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 07 Dec 2022 02:22:53 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 07 Dec 2022 02:22:54 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 07 Dec 2022 02:22:54 GMT
ENV MYSQL_SHELL_VERSION=8.0.31-1.el8
# Wed, 07 Dec 2022 02:23:29 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Wed, 07 Dec 2022 02:23:30 GMT
VOLUME [/var/lib/mysql]
# Wed, 07 Dec 2022 02:23:30 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 07 Dec 2022 02:23:31 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 07 Dec 2022 02:23:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 07 Dec 2022 02:23:31 GMT
EXPOSE 3306 33060
# Wed, 07 Dec 2022 02:23:31 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:0ed027b72ddc5d1a749fc58b7c26610167393b08ae71ef6625496508903f70a2`  
		Last Modified: Wed, 07 Dec 2022 01:53:11 GMT  
		Size: 43.9 MB (43868738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0296159747f12f208fbf9721970ca290348698ac443cf98311477b6e44f18acc`  
		Last Modified: Wed, 07 Dec 2022 02:25:25 GMT  
		Size: 886.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d2f9b664bd354b5b8823bbdda42cf0813f2d8d3b5693f952c0a8516af84a826`  
		Last Modified: Wed, 07 Dec 2022 02:25:25 GMT  
		Size: 928.8 KB (928835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df6519f81c2689152b478834162cfe2f21ef37c472108a3e3a03a6ac0f5cbdd9`  
		Last Modified: Wed, 07 Dec 2022 02:25:24 GMT  
		Size: 4.6 MB (4608004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36bb5e56d458a7652c87ab8c3909c0ad098feaa81e73649bb37704701ca3ee6d`  
		Last Modified: Wed, 07 Dec 2022 02:25:23 GMT  
		Size: 2.6 KB (2630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:054e8fde88d0e345bf3d5a7bb06dd62c56cc5b26713a0a27223e54f849a28d2c`  
		Last Modified: Wed, 07 Dec 2022 02:25:23 GMT  
		Size: 332.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2b494c50c7f5297000bd4e8bd09e9dbf84d44ffc5eb3e5028701db6a6749117`  
		Last Modified: Wed, 07 Dec 2022 02:25:30 GMT  
		Size: 56.1 MB (56063632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:132bc0d471b8b86912c8fff2877e1b2fcab03fdcbefa81630f33cb60ba5455c7`  
		Last Modified: Wed, 07 Dec 2022 02:25:21 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:135ec7033a05d2a5153f07e0b7983246a867df3c29a0fafc5ae47c90c35a1bf4`  
		Last Modified: Wed, 07 Dec 2022 02:25:31 GMT  
		Size: 55.1 MB (55106545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5961f02724723ffcd87c7e08efc9beb635496e32e530de0976755bf24843153b`  
		Last Modified: Wed, 07 Dec 2022 02:25:21 GMT  
		Size: 5.4 KB (5391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75b5f7a3d3a49109ed3673860a5c5ed0f3f070b099b59dfc9b1c45761ca1aaca`  
		Last Modified: Wed, 07 Dec 2022 02:25:21 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8.0` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:abd7d1e4a42b96a58c702db2633df611d201789b07c01749dac1aff97b83ba8f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **159.0 MB (159024595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b6f3978ca2905ae9bc14cfe86ae2f004f8c36561b722a06f64b73001b1898a5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 07 Dec 2022 02:10:44 GMT
ADD file:6fdd782c2779edf7149126e79dcb46ebde32975107cdd5d129cce0860e797cde in / 
# Wed, 07 Dec 2022 02:10:44 GMT
CMD ["/bin/bash"]
# Wed, 07 Dec 2022 02:50:18 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 07 Dec 2022 02:50:18 GMT
ENV GOSU_VERSION=1.14
# Wed, 07 Dec 2022 02:50:22 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 07 Dec 2022 02:50:43 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Wed, 07 Dec 2022 02:50:44 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 07 Dec 2022 02:50:44 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 07 Dec 2022 02:50:44 GMT
ENV MYSQL_VERSION=8.0.31-1.el8
# Wed, 07 Dec 2022 02:50:44 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 07 Dec 2022 02:51:09 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 07 Dec 2022 02:51:10 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 07 Dec 2022 02:51:10 GMT
ENV MYSQL_SHELL_VERSION=8.0.31-1.el8
# Wed, 07 Dec 2022 02:51:38 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Wed, 07 Dec 2022 02:51:39 GMT
VOLUME [/var/lib/mysql]
# Wed, 07 Dec 2022 02:51:39 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 07 Dec 2022 02:51:40 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 07 Dec 2022 02:51:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 07 Dec 2022 02:51:40 GMT
EXPOSE 3306 33060
# Wed, 07 Dec 2022 02:51:40 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:12a06ca91af857ea3cb02aedc5c643c5f06865868ae5c386c8ea664be60ead7e`  
		Last Modified: Wed, 07 Dec 2022 02:12:09 GMT  
		Size: 42.8 MB (42772059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fec1cb1944f64443d61a29e94cddba36d0cb8a09c80e0247375445bc62b842e`  
		Last Modified: Wed, 07 Dec 2022 02:52:10 GMT  
		Size: 887.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aede38c79379349fd3e9d191f92be36e68adc230840ae21c015f166b96e2067a`  
		Last Modified: Wed, 07 Dec 2022 02:52:10 GMT  
		Size: 857.2 KB (857168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51b980849561d1ed6bffe5deb621498e150f4f0f148af7a2654dd90ed42d7bfb`  
		Last Modified: Wed, 07 Dec 2022 02:52:09 GMT  
		Size: 4.5 MB (4464908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f503d79ed4bc3c439b28068291b1260757ab2de86163c8954962d88ff917e22a`  
		Last Modified: Wed, 07 Dec 2022 02:52:08 GMT  
		Size: 2.6 KB (2624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fb44db361f7e1027fb0010e8a3447c6e9337f6685ab4901f57030d01f730f74`  
		Last Modified: Wed, 07 Dec 2022 02:52:08 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:943b6dcee7dec15078e15da5cf8750748ae482bd7f5f206ecee44f5627229836`  
		Last Modified: Wed, 07 Dec 2022 02:52:13 GMT  
		Size: 55.4 MB (55444877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:911277c1fe4b4a08873f70cde5b84e7b38fd3d1c31c9c884baff83bd23886c96`  
		Last Modified: Wed, 07 Dec 2022 02:52:06 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a477017d045777c9cc1150499a65250c49ffd0669c2fa9fa8b64fb9e73cd353c`  
		Last Modified: Wed, 07 Dec 2022 02:52:14 GMT  
		Size: 55.5 MB (55475909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84b5061403a5151af9ccac6299ba1e8037c8f7a049dcc22e8808fd0095566e88`  
		Last Modified: Wed, 07 Dec 2022 02:52:06 GMT  
		Size: 5.4 KB (5392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ff27d035d66da6c178b69b95ddb8d8e913e206938df13d13dc0de764684b8c5`  
		Last Modified: Wed, 07 Dec 2022 02:52:06 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0-debian`

```console
$ docker pull mysql@sha256:e0a793ddd093df31139fc695ed889fdd3ec910c76ddf3186683efe2d67a2ba96
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:8.0-debian` - linux; amd64

```console
$ docker pull mysql@sha256:ac248facf748e93a1022552d4f15311ef8bd8be7ba841305a1b404ed59196de6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **177.5 MB (177548446 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3b748431f76159ff04ec985c63bf42dae5206be3aee4e1d244182b297299354`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 21 Dec 2022 01:20:32 GMT
ADD file:73e68ae6852c9afbb2989dc9c5b7c6668843f454b1bdcfb48658bfbc6c4af69e in / 
# Wed, 21 Dec 2022 01:20:33 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 11:31:49 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 21 Dec 2022 11:31:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 11:31:55 GMT
ENV GOSU_VERSION=1.14
# Wed, 21 Dec 2022 11:32:03 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 21 Dec 2022 11:32:04 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 21 Dec 2022 11:32:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 11:32:10 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Wed, 21 Dec 2022 11:32:10 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 21 Dec 2022 11:32:11 GMT
ENV MYSQL_VERSION=8.0.31-1debian11
# Wed, 21 Dec 2022 11:32:11 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ bullseye mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Wed, 21 Dec 2022 11:32:26 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Wed, 21 Dec 2022 11:32:27 GMT
VOLUME [/var/lib/mysql]
# Wed, 21 Dec 2022 11:32:27 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Wed, 21 Dec 2022 11:32:27 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 21 Dec 2022 11:32:28 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 21 Dec 2022 11:32:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Dec 2022 11:32:28 GMT
EXPOSE 3306 33060
# Wed, 21 Dec 2022 11:32:28 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:3f4ca61aafcd4fc07267a105067db35c0f0ac630e1970f3cd0c7bf552780e985`  
		Last Modified: Wed, 21 Dec 2022 01:24:36 GMT  
		Size: 31.4 MB (31396943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c71b14b90321c4c925c97bde825eb21b3c97f7f6b9f73ad028c29bf93347ee2`  
		Last Modified: Wed, 21 Dec 2022 11:33:54 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b20239cd5b3eb4255955404db9ddf231a20a91b74c52e8ae82513e70d75e84a`  
		Last Modified: Wed, 21 Dec 2022 11:33:55 GMT  
		Size: 4.4 MB (4414844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69a92a8be7b81fc7d582c733edcb95ffe26bd8ff252e05167b70b896561c550a`  
		Last Modified: Wed, 21 Dec 2022 11:33:53 GMT  
		Size: 1.4 MB (1418501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed87af8210d03be6cf68e7ddc53ca53f0b7cb5d2526d8b350a6499f0b09d7b7f`  
		Last Modified: Wed, 21 Dec 2022 11:33:52 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89326f0fbca735cd9db355568c579a062d4e4f1a151dee777fca6739679c8559`  
		Last Modified: Wed, 21 Dec 2022 11:33:55 GMT  
		Size: 12.7 MB (12662005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2d532ea748ea86b00b0defbd158232a20f45862f4693dd6967e7ed4f379c57f`  
		Last Modified: Wed, 21 Dec 2022 11:33:52 GMT  
		Size: 2.5 KB (2545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46e4e09af7ec7aa3580ada1847200f65da4879d557475f2f356c43d6f2200669`  
		Last Modified: Wed, 21 Dec 2022 11:33:51 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d62f3c764f6b95a24939111413263a1dd1e0ffcf895cb6757b4aff64a412340`  
		Last Modified: Wed, 21 Dec 2022 11:34:10 GMT  
		Size: 127.6 MB (127645114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edad28c75e273ba1d4fade07eba864f0ad81767b605529a4918c6d6aa8b4a2ba`  
		Last Modified: Wed, 21 Dec 2022 11:33:51 GMT  
		Size: 846.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a2005ac0b2c3804a85b1ef7cfc06d078e2ecce524d07697c9f58f811367b26e`  
		Last Modified: Wed, 21 Dec 2022 11:33:51 GMT  
		Size: 5.4 KB (5391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ff97e27ba8e3f53c701cbd1841c5e91dfe25863598c0d09302e83871f2b344e`  
		Last Modified: Wed, 21 Dec 2022 11:33:51 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0-oracle`

```console
$ docker pull mysql@sha256:3d7ae561cf6095f6aca8eb7830e1d14734227b1fb4748092f2be2cfbccf7d614
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8.0-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:cfddf275c8b1ae1583c0f6afb4899d4dbe14111a6462699559a1f4dc8f4d5f6e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **160.6 MB (160585430 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7484689f290f1defe06b65befc54cb6ad91a667cf0af59a265ffe76c46bd0478`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 07 Dec 2022 01:51:27 GMT
ADD file:04d9ae26c2acac414b69a784563f765d531aeaf941ea0341025b4544f9ade244 in / 
# Wed, 07 Dec 2022 01:51:27 GMT
CMD ["/bin/bash"]
# Wed, 07 Dec 2022 02:21:54 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 07 Dec 2022 02:21:55 GMT
ENV GOSU_VERSION=1.14
# Wed, 07 Dec 2022 02:21:58 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 07 Dec 2022 02:22:21 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Wed, 07 Dec 2022 02:22:22 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 07 Dec 2022 02:22:23 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 07 Dec 2022 02:22:23 GMT
ENV MYSQL_VERSION=8.0.31-1.el8
# Wed, 07 Dec 2022 02:22:23 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 07 Dec 2022 02:22:53 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 07 Dec 2022 02:22:54 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 07 Dec 2022 02:22:54 GMT
ENV MYSQL_SHELL_VERSION=8.0.31-1.el8
# Wed, 07 Dec 2022 02:23:29 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Wed, 07 Dec 2022 02:23:30 GMT
VOLUME [/var/lib/mysql]
# Wed, 07 Dec 2022 02:23:30 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 07 Dec 2022 02:23:31 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 07 Dec 2022 02:23:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 07 Dec 2022 02:23:31 GMT
EXPOSE 3306 33060
# Wed, 07 Dec 2022 02:23:31 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:0ed027b72ddc5d1a749fc58b7c26610167393b08ae71ef6625496508903f70a2`  
		Last Modified: Wed, 07 Dec 2022 01:53:11 GMT  
		Size: 43.9 MB (43868738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0296159747f12f208fbf9721970ca290348698ac443cf98311477b6e44f18acc`  
		Last Modified: Wed, 07 Dec 2022 02:25:25 GMT  
		Size: 886.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d2f9b664bd354b5b8823bbdda42cf0813f2d8d3b5693f952c0a8516af84a826`  
		Last Modified: Wed, 07 Dec 2022 02:25:25 GMT  
		Size: 928.8 KB (928835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df6519f81c2689152b478834162cfe2f21ef37c472108a3e3a03a6ac0f5cbdd9`  
		Last Modified: Wed, 07 Dec 2022 02:25:24 GMT  
		Size: 4.6 MB (4608004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36bb5e56d458a7652c87ab8c3909c0ad098feaa81e73649bb37704701ca3ee6d`  
		Last Modified: Wed, 07 Dec 2022 02:25:23 GMT  
		Size: 2.6 KB (2630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:054e8fde88d0e345bf3d5a7bb06dd62c56cc5b26713a0a27223e54f849a28d2c`  
		Last Modified: Wed, 07 Dec 2022 02:25:23 GMT  
		Size: 332.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2b494c50c7f5297000bd4e8bd09e9dbf84d44ffc5eb3e5028701db6a6749117`  
		Last Modified: Wed, 07 Dec 2022 02:25:30 GMT  
		Size: 56.1 MB (56063632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:132bc0d471b8b86912c8fff2877e1b2fcab03fdcbefa81630f33cb60ba5455c7`  
		Last Modified: Wed, 07 Dec 2022 02:25:21 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:135ec7033a05d2a5153f07e0b7983246a867df3c29a0fafc5ae47c90c35a1bf4`  
		Last Modified: Wed, 07 Dec 2022 02:25:31 GMT  
		Size: 55.1 MB (55106545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5961f02724723ffcd87c7e08efc9beb635496e32e530de0976755bf24843153b`  
		Last Modified: Wed, 07 Dec 2022 02:25:21 GMT  
		Size: 5.4 KB (5391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75b5f7a3d3a49109ed3673860a5c5ed0f3f070b099b59dfc9b1c45761ca1aaca`  
		Last Modified: Wed, 07 Dec 2022 02:25:21 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8.0-oracle` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:abd7d1e4a42b96a58c702db2633df611d201789b07c01749dac1aff97b83ba8f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **159.0 MB (159024595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b6f3978ca2905ae9bc14cfe86ae2f004f8c36561b722a06f64b73001b1898a5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 07 Dec 2022 02:10:44 GMT
ADD file:6fdd782c2779edf7149126e79dcb46ebde32975107cdd5d129cce0860e797cde in / 
# Wed, 07 Dec 2022 02:10:44 GMT
CMD ["/bin/bash"]
# Wed, 07 Dec 2022 02:50:18 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 07 Dec 2022 02:50:18 GMT
ENV GOSU_VERSION=1.14
# Wed, 07 Dec 2022 02:50:22 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 07 Dec 2022 02:50:43 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Wed, 07 Dec 2022 02:50:44 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 07 Dec 2022 02:50:44 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 07 Dec 2022 02:50:44 GMT
ENV MYSQL_VERSION=8.0.31-1.el8
# Wed, 07 Dec 2022 02:50:44 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 07 Dec 2022 02:51:09 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 07 Dec 2022 02:51:10 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 07 Dec 2022 02:51:10 GMT
ENV MYSQL_SHELL_VERSION=8.0.31-1.el8
# Wed, 07 Dec 2022 02:51:38 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Wed, 07 Dec 2022 02:51:39 GMT
VOLUME [/var/lib/mysql]
# Wed, 07 Dec 2022 02:51:39 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 07 Dec 2022 02:51:40 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 07 Dec 2022 02:51:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 07 Dec 2022 02:51:40 GMT
EXPOSE 3306 33060
# Wed, 07 Dec 2022 02:51:40 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:12a06ca91af857ea3cb02aedc5c643c5f06865868ae5c386c8ea664be60ead7e`  
		Last Modified: Wed, 07 Dec 2022 02:12:09 GMT  
		Size: 42.8 MB (42772059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fec1cb1944f64443d61a29e94cddba36d0cb8a09c80e0247375445bc62b842e`  
		Last Modified: Wed, 07 Dec 2022 02:52:10 GMT  
		Size: 887.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aede38c79379349fd3e9d191f92be36e68adc230840ae21c015f166b96e2067a`  
		Last Modified: Wed, 07 Dec 2022 02:52:10 GMT  
		Size: 857.2 KB (857168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51b980849561d1ed6bffe5deb621498e150f4f0f148af7a2654dd90ed42d7bfb`  
		Last Modified: Wed, 07 Dec 2022 02:52:09 GMT  
		Size: 4.5 MB (4464908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f503d79ed4bc3c439b28068291b1260757ab2de86163c8954962d88ff917e22a`  
		Last Modified: Wed, 07 Dec 2022 02:52:08 GMT  
		Size: 2.6 KB (2624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fb44db361f7e1027fb0010e8a3447c6e9337f6685ab4901f57030d01f730f74`  
		Last Modified: Wed, 07 Dec 2022 02:52:08 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:943b6dcee7dec15078e15da5cf8750748ae482bd7f5f206ecee44f5627229836`  
		Last Modified: Wed, 07 Dec 2022 02:52:13 GMT  
		Size: 55.4 MB (55444877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:911277c1fe4b4a08873f70cde5b84e7b38fd3d1c31c9c884baff83bd23886c96`  
		Last Modified: Wed, 07 Dec 2022 02:52:06 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a477017d045777c9cc1150499a65250c49ffd0669c2fa9fa8b64fb9e73cd353c`  
		Last Modified: Wed, 07 Dec 2022 02:52:14 GMT  
		Size: 55.5 MB (55475909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84b5061403a5151af9ccac6299ba1e8037c8f7a049dcc22e8808fd0095566e88`  
		Last Modified: Wed, 07 Dec 2022 02:52:06 GMT  
		Size: 5.4 KB (5392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ff27d035d66da6c178b69b95ddb8d8e913e206938df13d13dc0de764684b8c5`  
		Last Modified: Wed, 07 Dec 2022 02:52:06 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0.31`

```console
$ docker pull mysql@sha256:3d7ae561cf6095f6aca8eb7830e1d14734227b1fb4748092f2be2cfbccf7d614
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8.0.31` - linux; amd64

```console
$ docker pull mysql@sha256:cfddf275c8b1ae1583c0f6afb4899d4dbe14111a6462699559a1f4dc8f4d5f6e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **160.6 MB (160585430 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7484689f290f1defe06b65befc54cb6ad91a667cf0af59a265ffe76c46bd0478`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 07 Dec 2022 01:51:27 GMT
ADD file:04d9ae26c2acac414b69a784563f765d531aeaf941ea0341025b4544f9ade244 in / 
# Wed, 07 Dec 2022 01:51:27 GMT
CMD ["/bin/bash"]
# Wed, 07 Dec 2022 02:21:54 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 07 Dec 2022 02:21:55 GMT
ENV GOSU_VERSION=1.14
# Wed, 07 Dec 2022 02:21:58 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 07 Dec 2022 02:22:21 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Wed, 07 Dec 2022 02:22:22 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 07 Dec 2022 02:22:23 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 07 Dec 2022 02:22:23 GMT
ENV MYSQL_VERSION=8.0.31-1.el8
# Wed, 07 Dec 2022 02:22:23 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 07 Dec 2022 02:22:53 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 07 Dec 2022 02:22:54 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 07 Dec 2022 02:22:54 GMT
ENV MYSQL_SHELL_VERSION=8.0.31-1.el8
# Wed, 07 Dec 2022 02:23:29 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Wed, 07 Dec 2022 02:23:30 GMT
VOLUME [/var/lib/mysql]
# Wed, 07 Dec 2022 02:23:30 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 07 Dec 2022 02:23:31 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 07 Dec 2022 02:23:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 07 Dec 2022 02:23:31 GMT
EXPOSE 3306 33060
# Wed, 07 Dec 2022 02:23:31 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:0ed027b72ddc5d1a749fc58b7c26610167393b08ae71ef6625496508903f70a2`  
		Last Modified: Wed, 07 Dec 2022 01:53:11 GMT  
		Size: 43.9 MB (43868738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0296159747f12f208fbf9721970ca290348698ac443cf98311477b6e44f18acc`  
		Last Modified: Wed, 07 Dec 2022 02:25:25 GMT  
		Size: 886.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d2f9b664bd354b5b8823bbdda42cf0813f2d8d3b5693f952c0a8516af84a826`  
		Last Modified: Wed, 07 Dec 2022 02:25:25 GMT  
		Size: 928.8 KB (928835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df6519f81c2689152b478834162cfe2f21ef37c472108a3e3a03a6ac0f5cbdd9`  
		Last Modified: Wed, 07 Dec 2022 02:25:24 GMT  
		Size: 4.6 MB (4608004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36bb5e56d458a7652c87ab8c3909c0ad098feaa81e73649bb37704701ca3ee6d`  
		Last Modified: Wed, 07 Dec 2022 02:25:23 GMT  
		Size: 2.6 KB (2630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:054e8fde88d0e345bf3d5a7bb06dd62c56cc5b26713a0a27223e54f849a28d2c`  
		Last Modified: Wed, 07 Dec 2022 02:25:23 GMT  
		Size: 332.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2b494c50c7f5297000bd4e8bd09e9dbf84d44ffc5eb3e5028701db6a6749117`  
		Last Modified: Wed, 07 Dec 2022 02:25:30 GMT  
		Size: 56.1 MB (56063632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:132bc0d471b8b86912c8fff2877e1b2fcab03fdcbefa81630f33cb60ba5455c7`  
		Last Modified: Wed, 07 Dec 2022 02:25:21 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:135ec7033a05d2a5153f07e0b7983246a867df3c29a0fafc5ae47c90c35a1bf4`  
		Last Modified: Wed, 07 Dec 2022 02:25:31 GMT  
		Size: 55.1 MB (55106545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5961f02724723ffcd87c7e08efc9beb635496e32e530de0976755bf24843153b`  
		Last Modified: Wed, 07 Dec 2022 02:25:21 GMT  
		Size: 5.4 KB (5391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75b5f7a3d3a49109ed3673860a5c5ed0f3f070b099b59dfc9b1c45761ca1aaca`  
		Last Modified: Wed, 07 Dec 2022 02:25:21 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8.0.31` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:abd7d1e4a42b96a58c702db2633df611d201789b07c01749dac1aff97b83ba8f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **159.0 MB (159024595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b6f3978ca2905ae9bc14cfe86ae2f004f8c36561b722a06f64b73001b1898a5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 07 Dec 2022 02:10:44 GMT
ADD file:6fdd782c2779edf7149126e79dcb46ebde32975107cdd5d129cce0860e797cde in / 
# Wed, 07 Dec 2022 02:10:44 GMT
CMD ["/bin/bash"]
# Wed, 07 Dec 2022 02:50:18 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 07 Dec 2022 02:50:18 GMT
ENV GOSU_VERSION=1.14
# Wed, 07 Dec 2022 02:50:22 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 07 Dec 2022 02:50:43 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Wed, 07 Dec 2022 02:50:44 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 07 Dec 2022 02:50:44 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 07 Dec 2022 02:50:44 GMT
ENV MYSQL_VERSION=8.0.31-1.el8
# Wed, 07 Dec 2022 02:50:44 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 07 Dec 2022 02:51:09 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 07 Dec 2022 02:51:10 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 07 Dec 2022 02:51:10 GMT
ENV MYSQL_SHELL_VERSION=8.0.31-1.el8
# Wed, 07 Dec 2022 02:51:38 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Wed, 07 Dec 2022 02:51:39 GMT
VOLUME [/var/lib/mysql]
# Wed, 07 Dec 2022 02:51:39 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 07 Dec 2022 02:51:40 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 07 Dec 2022 02:51:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 07 Dec 2022 02:51:40 GMT
EXPOSE 3306 33060
# Wed, 07 Dec 2022 02:51:40 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:12a06ca91af857ea3cb02aedc5c643c5f06865868ae5c386c8ea664be60ead7e`  
		Last Modified: Wed, 07 Dec 2022 02:12:09 GMT  
		Size: 42.8 MB (42772059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fec1cb1944f64443d61a29e94cddba36d0cb8a09c80e0247375445bc62b842e`  
		Last Modified: Wed, 07 Dec 2022 02:52:10 GMT  
		Size: 887.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aede38c79379349fd3e9d191f92be36e68adc230840ae21c015f166b96e2067a`  
		Last Modified: Wed, 07 Dec 2022 02:52:10 GMT  
		Size: 857.2 KB (857168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51b980849561d1ed6bffe5deb621498e150f4f0f148af7a2654dd90ed42d7bfb`  
		Last Modified: Wed, 07 Dec 2022 02:52:09 GMT  
		Size: 4.5 MB (4464908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f503d79ed4bc3c439b28068291b1260757ab2de86163c8954962d88ff917e22a`  
		Last Modified: Wed, 07 Dec 2022 02:52:08 GMT  
		Size: 2.6 KB (2624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fb44db361f7e1027fb0010e8a3447c6e9337f6685ab4901f57030d01f730f74`  
		Last Modified: Wed, 07 Dec 2022 02:52:08 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:943b6dcee7dec15078e15da5cf8750748ae482bd7f5f206ecee44f5627229836`  
		Last Modified: Wed, 07 Dec 2022 02:52:13 GMT  
		Size: 55.4 MB (55444877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:911277c1fe4b4a08873f70cde5b84e7b38fd3d1c31c9c884baff83bd23886c96`  
		Last Modified: Wed, 07 Dec 2022 02:52:06 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a477017d045777c9cc1150499a65250c49ffd0669c2fa9fa8b64fb9e73cd353c`  
		Last Modified: Wed, 07 Dec 2022 02:52:14 GMT  
		Size: 55.5 MB (55475909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84b5061403a5151af9ccac6299ba1e8037c8f7a049dcc22e8808fd0095566e88`  
		Last Modified: Wed, 07 Dec 2022 02:52:06 GMT  
		Size: 5.4 KB (5392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ff27d035d66da6c178b69b95ddb8d8e913e206938df13d13dc0de764684b8c5`  
		Last Modified: Wed, 07 Dec 2022 02:52:06 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0.31-debian`

```console
$ docker pull mysql@sha256:e0a793ddd093df31139fc695ed889fdd3ec910c76ddf3186683efe2d67a2ba96
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:8.0.31-debian` - linux; amd64

```console
$ docker pull mysql@sha256:ac248facf748e93a1022552d4f15311ef8bd8be7ba841305a1b404ed59196de6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **177.5 MB (177548446 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3b748431f76159ff04ec985c63bf42dae5206be3aee4e1d244182b297299354`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 21 Dec 2022 01:20:32 GMT
ADD file:73e68ae6852c9afbb2989dc9c5b7c6668843f454b1bdcfb48658bfbc6c4af69e in / 
# Wed, 21 Dec 2022 01:20:33 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 11:31:49 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 21 Dec 2022 11:31:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 11:31:55 GMT
ENV GOSU_VERSION=1.14
# Wed, 21 Dec 2022 11:32:03 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 21 Dec 2022 11:32:04 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 21 Dec 2022 11:32:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 11:32:10 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Wed, 21 Dec 2022 11:32:10 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 21 Dec 2022 11:32:11 GMT
ENV MYSQL_VERSION=8.0.31-1debian11
# Wed, 21 Dec 2022 11:32:11 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ bullseye mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Wed, 21 Dec 2022 11:32:26 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Wed, 21 Dec 2022 11:32:27 GMT
VOLUME [/var/lib/mysql]
# Wed, 21 Dec 2022 11:32:27 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Wed, 21 Dec 2022 11:32:27 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 21 Dec 2022 11:32:28 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 21 Dec 2022 11:32:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Dec 2022 11:32:28 GMT
EXPOSE 3306 33060
# Wed, 21 Dec 2022 11:32:28 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:3f4ca61aafcd4fc07267a105067db35c0f0ac630e1970f3cd0c7bf552780e985`  
		Last Modified: Wed, 21 Dec 2022 01:24:36 GMT  
		Size: 31.4 MB (31396943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c71b14b90321c4c925c97bde825eb21b3c97f7f6b9f73ad028c29bf93347ee2`  
		Last Modified: Wed, 21 Dec 2022 11:33:54 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b20239cd5b3eb4255955404db9ddf231a20a91b74c52e8ae82513e70d75e84a`  
		Last Modified: Wed, 21 Dec 2022 11:33:55 GMT  
		Size: 4.4 MB (4414844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69a92a8be7b81fc7d582c733edcb95ffe26bd8ff252e05167b70b896561c550a`  
		Last Modified: Wed, 21 Dec 2022 11:33:53 GMT  
		Size: 1.4 MB (1418501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed87af8210d03be6cf68e7ddc53ca53f0b7cb5d2526d8b350a6499f0b09d7b7f`  
		Last Modified: Wed, 21 Dec 2022 11:33:52 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89326f0fbca735cd9db355568c579a062d4e4f1a151dee777fca6739679c8559`  
		Last Modified: Wed, 21 Dec 2022 11:33:55 GMT  
		Size: 12.7 MB (12662005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2d532ea748ea86b00b0defbd158232a20f45862f4693dd6967e7ed4f379c57f`  
		Last Modified: Wed, 21 Dec 2022 11:33:52 GMT  
		Size: 2.5 KB (2545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46e4e09af7ec7aa3580ada1847200f65da4879d557475f2f356c43d6f2200669`  
		Last Modified: Wed, 21 Dec 2022 11:33:51 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d62f3c764f6b95a24939111413263a1dd1e0ffcf895cb6757b4aff64a412340`  
		Last Modified: Wed, 21 Dec 2022 11:34:10 GMT  
		Size: 127.6 MB (127645114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edad28c75e273ba1d4fade07eba864f0ad81767b605529a4918c6d6aa8b4a2ba`  
		Last Modified: Wed, 21 Dec 2022 11:33:51 GMT  
		Size: 846.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a2005ac0b2c3804a85b1ef7cfc06d078e2ecce524d07697c9f58f811367b26e`  
		Last Modified: Wed, 21 Dec 2022 11:33:51 GMT  
		Size: 5.4 KB (5391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ff97e27ba8e3f53c701cbd1841c5e91dfe25863598c0d09302e83871f2b344e`  
		Last Modified: Wed, 21 Dec 2022 11:33:51 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:8.0.31-oracle`

```console
$ docker pull mysql@sha256:3d7ae561cf6095f6aca8eb7830e1d14734227b1fb4748092f2be2cfbccf7d614
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8.0.31-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:cfddf275c8b1ae1583c0f6afb4899d4dbe14111a6462699559a1f4dc8f4d5f6e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **160.6 MB (160585430 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7484689f290f1defe06b65befc54cb6ad91a667cf0af59a265ffe76c46bd0478`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 07 Dec 2022 01:51:27 GMT
ADD file:04d9ae26c2acac414b69a784563f765d531aeaf941ea0341025b4544f9ade244 in / 
# Wed, 07 Dec 2022 01:51:27 GMT
CMD ["/bin/bash"]
# Wed, 07 Dec 2022 02:21:54 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 07 Dec 2022 02:21:55 GMT
ENV GOSU_VERSION=1.14
# Wed, 07 Dec 2022 02:21:58 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 07 Dec 2022 02:22:21 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Wed, 07 Dec 2022 02:22:22 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 07 Dec 2022 02:22:23 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 07 Dec 2022 02:22:23 GMT
ENV MYSQL_VERSION=8.0.31-1.el8
# Wed, 07 Dec 2022 02:22:23 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 07 Dec 2022 02:22:53 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 07 Dec 2022 02:22:54 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 07 Dec 2022 02:22:54 GMT
ENV MYSQL_SHELL_VERSION=8.0.31-1.el8
# Wed, 07 Dec 2022 02:23:29 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Wed, 07 Dec 2022 02:23:30 GMT
VOLUME [/var/lib/mysql]
# Wed, 07 Dec 2022 02:23:30 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 07 Dec 2022 02:23:31 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 07 Dec 2022 02:23:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 07 Dec 2022 02:23:31 GMT
EXPOSE 3306 33060
# Wed, 07 Dec 2022 02:23:31 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:0ed027b72ddc5d1a749fc58b7c26610167393b08ae71ef6625496508903f70a2`  
		Last Modified: Wed, 07 Dec 2022 01:53:11 GMT  
		Size: 43.9 MB (43868738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0296159747f12f208fbf9721970ca290348698ac443cf98311477b6e44f18acc`  
		Last Modified: Wed, 07 Dec 2022 02:25:25 GMT  
		Size: 886.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d2f9b664bd354b5b8823bbdda42cf0813f2d8d3b5693f952c0a8516af84a826`  
		Last Modified: Wed, 07 Dec 2022 02:25:25 GMT  
		Size: 928.8 KB (928835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df6519f81c2689152b478834162cfe2f21ef37c472108a3e3a03a6ac0f5cbdd9`  
		Last Modified: Wed, 07 Dec 2022 02:25:24 GMT  
		Size: 4.6 MB (4608004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36bb5e56d458a7652c87ab8c3909c0ad098feaa81e73649bb37704701ca3ee6d`  
		Last Modified: Wed, 07 Dec 2022 02:25:23 GMT  
		Size: 2.6 KB (2630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:054e8fde88d0e345bf3d5a7bb06dd62c56cc5b26713a0a27223e54f849a28d2c`  
		Last Modified: Wed, 07 Dec 2022 02:25:23 GMT  
		Size: 332.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2b494c50c7f5297000bd4e8bd09e9dbf84d44ffc5eb3e5028701db6a6749117`  
		Last Modified: Wed, 07 Dec 2022 02:25:30 GMT  
		Size: 56.1 MB (56063632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:132bc0d471b8b86912c8fff2877e1b2fcab03fdcbefa81630f33cb60ba5455c7`  
		Last Modified: Wed, 07 Dec 2022 02:25:21 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:135ec7033a05d2a5153f07e0b7983246a867df3c29a0fafc5ae47c90c35a1bf4`  
		Last Modified: Wed, 07 Dec 2022 02:25:31 GMT  
		Size: 55.1 MB (55106545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5961f02724723ffcd87c7e08efc9beb635496e32e530de0976755bf24843153b`  
		Last Modified: Wed, 07 Dec 2022 02:25:21 GMT  
		Size: 5.4 KB (5391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75b5f7a3d3a49109ed3673860a5c5ed0f3f070b099b59dfc9b1c45761ca1aaca`  
		Last Modified: Wed, 07 Dec 2022 02:25:21 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8.0.31-oracle` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:abd7d1e4a42b96a58c702db2633df611d201789b07c01749dac1aff97b83ba8f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **159.0 MB (159024595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b6f3978ca2905ae9bc14cfe86ae2f004f8c36561b722a06f64b73001b1898a5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 07 Dec 2022 02:10:44 GMT
ADD file:6fdd782c2779edf7149126e79dcb46ebde32975107cdd5d129cce0860e797cde in / 
# Wed, 07 Dec 2022 02:10:44 GMT
CMD ["/bin/bash"]
# Wed, 07 Dec 2022 02:50:18 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 07 Dec 2022 02:50:18 GMT
ENV GOSU_VERSION=1.14
# Wed, 07 Dec 2022 02:50:22 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 07 Dec 2022 02:50:43 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Wed, 07 Dec 2022 02:50:44 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 07 Dec 2022 02:50:44 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 07 Dec 2022 02:50:44 GMT
ENV MYSQL_VERSION=8.0.31-1.el8
# Wed, 07 Dec 2022 02:50:44 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 07 Dec 2022 02:51:09 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 07 Dec 2022 02:51:10 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 07 Dec 2022 02:51:10 GMT
ENV MYSQL_SHELL_VERSION=8.0.31-1.el8
# Wed, 07 Dec 2022 02:51:38 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Wed, 07 Dec 2022 02:51:39 GMT
VOLUME [/var/lib/mysql]
# Wed, 07 Dec 2022 02:51:39 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 07 Dec 2022 02:51:40 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 07 Dec 2022 02:51:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 07 Dec 2022 02:51:40 GMT
EXPOSE 3306 33060
# Wed, 07 Dec 2022 02:51:40 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:12a06ca91af857ea3cb02aedc5c643c5f06865868ae5c386c8ea664be60ead7e`  
		Last Modified: Wed, 07 Dec 2022 02:12:09 GMT  
		Size: 42.8 MB (42772059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fec1cb1944f64443d61a29e94cddba36d0cb8a09c80e0247375445bc62b842e`  
		Last Modified: Wed, 07 Dec 2022 02:52:10 GMT  
		Size: 887.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aede38c79379349fd3e9d191f92be36e68adc230840ae21c015f166b96e2067a`  
		Last Modified: Wed, 07 Dec 2022 02:52:10 GMT  
		Size: 857.2 KB (857168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51b980849561d1ed6bffe5deb621498e150f4f0f148af7a2654dd90ed42d7bfb`  
		Last Modified: Wed, 07 Dec 2022 02:52:09 GMT  
		Size: 4.5 MB (4464908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f503d79ed4bc3c439b28068291b1260757ab2de86163c8954962d88ff917e22a`  
		Last Modified: Wed, 07 Dec 2022 02:52:08 GMT  
		Size: 2.6 KB (2624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fb44db361f7e1027fb0010e8a3447c6e9337f6685ab4901f57030d01f730f74`  
		Last Modified: Wed, 07 Dec 2022 02:52:08 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:943b6dcee7dec15078e15da5cf8750748ae482bd7f5f206ecee44f5627229836`  
		Last Modified: Wed, 07 Dec 2022 02:52:13 GMT  
		Size: 55.4 MB (55444877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:911277c1fe4b4a08873f70cde5b84e7b38fd3d1c31c9c884baff83bd23886c96`  
		Last Modified: Wed, 07 Dec 2022 02:52:06 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a477017d045777c9cc1150499a65250c49ffd0669c2fa9fa8b64fb9e73cd353c`  
		Last Modified: Wed, 07 Dec 2022 02:52:14 GMT  
		Size: 55.5 MB (55475909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84b5061403a5151af9ccac6299ba1e8037c8f7a049dcc22e8808fd0095566e88`  
		Last Modified: Wed, 07 Dec 2022 02:52:06 GMT  
		Size: 5.4 KB (5392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ff27d035d66da6c178b69b95ddb8d8e913e206938df13d13dc0de764684b8c5`  
		Last Modified: Wed, 07 Dec 2022 02:52:06 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:debian`

```console
$ docker pull mysql@sha256:e0a793ddd093df31139fc695ed889fdd3ec910c76ddf3186683efe2d67a2ba96
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:debian` - linux; amd64

```console
$ docker pull mysql@sha256:ac248facf748e93a1022552d4f15311ef8bd8be7ba841305a1b404ed59196de6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **177.5 MB (177548446 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3b748431f76159ff04ec985c63bf42dae5206be3aee4e1d244182b297299354`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 21 Dec 2022 01:20:32 GMT
ADD file:73e68ae6852c9afbb2989dc9c5b7c6668843f454b1bdcfb48658bfbc6c4af69e in / 
# Wed, 21 Dec 2022 01:20:33 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 11:31:49 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql
# Wed, 21 Dec 2022 11:31:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg dirmngr && rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 11:31:55 GMT
ENV GOSU_VERSION=1.14
# Wed, 21 Dec 2022 11:32:03 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 21 Dec 2022 11:32:04 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 21 Dec 2022 11:32:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 11:32:10 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Wed, 21 Dec 2022 11:32:10 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 21 Dec 2022 11:32:11 GMT
ENV MYSQL_VERSION=8.0.31-1debian11
# Wed, 21 Dec 2022 11:32:11 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ bullseye mysql-8.0' > /etc/apt/sources.list.d/mysql.list
# Wed, 21 Dec 2022 11:32:26 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql
# Wed, 21 Dec 2022 11:32:27 GMT
VOLUME [/var/lib/mysql]
# Wed, 21 Dec 2022 11:32:27 GMT
COPY dir:2e040acc386ebd23b8571951a51e6cb93647df091bc26159b8c757ef82b3fcda in /etc/mysql/ 
# Wed, 21 Dec 2022 11:32:27 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 21 Dec 2022 11:32:28 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 21 Dec 2022 11:32:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Dec 2022 11:32:28 GMT
EXPOSE 3306 33060
# Wed, 21 Dec 2022 11:32:28 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:3f4ca61aafcd4fc07267a105067db35c0f0ac630e1970f3cd0c7bf552780e985`  
		Last Modified: Wed, 21 Dec 2022 01:24:36 GMT  
		Size: 31.4 MB (31396943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c71b14b90321c4c925c97bde825eb21b3c97f7f6b9f73ad028c29bf93347ee2`  
		Last Modified: Wed, 21 Dec 2022 11:33:54 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b20239cd5b3eb4255955404db9ddf231a20a91b74c52e8ae82513e70d75e84a`  
		Last Modified: Wed, 21 Dec 2022 11:33:55 GMT  
		Size: 4.4 MB (4414844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69a92a8be7b81fc7d582c733edcb95ffe26bd8ff252e05167b70b896561c550a`  
		Last Modified: Wed, 21 Dec 2022 11:33:53 GMT  
		Size: 1.4 MB (1418501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed87af8210d03be6cf68e7ddc53ca53f0b7cb5d2526d8b350a6499f0b09d7b7f`  
		Last Modified: Wed, 21 Dec 2022 11:33:52 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89326f0fbca735cd9db355568c579a062d4e4f1a151dee777fca6739679c8559`  
		Last Modified: Wed, 21 Dec 2022 11:33:55 GMT  
		Size: 12.7 MB (12662005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2d532ea748ea86b00b0defbd158232a20f45862f4693dd6967e7ed4f379c57f`  
		Last Modified: Wed, 21 Dec 2022 11:33:52 GMT  
		Size: 2.5 KB (2545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46e4e09af7ec7aa3580ada1847200f65da4879d557475f2f356c43d6f2200669`  
		Last Modified: Wed, 21 Dec 2022 11:33:51 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d62f3c764f6b95a24939111413263a1dd1e0ffcf895cb6757b4aff64a412340`  
		Last Modified: Wed, 21 Dec 2022 11:34:10 GMT  
		Size: 127.6 MB (127645114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edad28c75e273ba1d4fade07eba864f0ad81767b605529a4918c6d6aa8b4a2ba`  
		Last Modified: Wed, 21 Dec 2022 11:33:51 GMT  
		Size: 846.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a2005ac0b2c3804a85b1ef7cfc06d078e2ecce524d07697c9f58f811367b26e`  
		Last Modified: Wed, 21 Dec 2022 11:33:51 GMT  
		Size: 5.4 KB (5391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ff97e27ba8e3f53c701cbd1841c5e91dfe25863598c0d09302e83871f2b344e`  
		Last Modified: Wed, 21 Dec 2022 11:33:51 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:latest`

```console
$ docker pull mysql@sha256:3d7ae561cf6095f6aca8eb7830e1d14734227b1fb4748092f2be2cfbccf7d614
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:latest` - linux; amd64

```console
$ docker pull mysql@sha256:cfddf275c8b1ae1583c0f6afb4899d4dbe14111a6462699559a1f4dc8f4d5f6e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **160.6 MB (160585430 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7484689f290f1defe06b65befc54cb6ad91a667cf0af59a265ffe76c46bd0478`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 07 Dec 2022 01:51:27 GMT
ADD file:04d9ae26c2acac414b69a784563f765d531aeaf941ea0341025b4544f9ade244 in / 
# Wed, 07 Dec 2022 01:51:27 GMT
CMD ["/bin/bash"]
# Wed, 07 Dec 2022 02:21:54 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 07 Dec 2022 02:21:55 GMT
ENV GOSU_VERSION=1.14
# Wed, 07 Dec 2022 02:21:58 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 07 Dec 2022 02:22:21 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Wed, 07 Dec 2022 02:22:22 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 07 Dec 2022 02:22:23 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 07 Dec 2022 02:22:23 GMT
ENV MYSQL_VERSION=8.0.31-1.el8
# Wed, 07 Dec 2022 02:22:23 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 07 Dec 2022 02:22:53 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 07 Dec 2022 02:22:54 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 07 Dec 2022 02:22:54 GMT
ENV MYSQL_SHELL_VERSION=8.0.31-1.el8
# Wed, 07 Dec 2022 02:23:29 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Wed, 07 Dec 2022 02:23:30 GMT
VOLUME [/var/lib/mysql]
# Wed, 07 Dec 2022 02:23:30 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 07 Dec 2022 02:23:31 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 07 Dec 2022 02:23:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 07 Dec 2022 02:23:31 GMT
EXPOSE 3306 33060
# Wed, 07 Dec 2022 02:23:31 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:0ed027b72ddc5d1a749fc58b7c26610167393b08ae71ef6625496508903f70a2`  
		Last Modified: Wed, 07 Dec 2022 01:53:11 GMT  
		Size: 43.9 MB (43868738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0296159747f12f208fbf9721970ca290348698ac443cf98311477b6e44f18acc`  
		Last Modified: Wed, 07 Dec 2022 02:25:25 GMT  
		Size: 886.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d2f9b664bd354b5b8823bbdda42cf0813f2d8d3b5693f952c0a8516af84a826`  
		Last Modified: Wed, 07 Dec 2022 02:25:25 GMT  
		Size: 928.8 KB (928835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df6519f81c2689152b478834162cfe2f21ef37c472108a3e3a03a6ac0f5cbdd9`  
		Last Modified: Wed, 07 Dec 2022 02:25:24 GMT  
		Size: 4.6 MB (4608004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36bb5e56d458a7652c87ab8c3909c0ad098feaa81e73649bb37704701ca3ee6d`  
		Last Modified: Wed, 07 Dec 2022 02:25:23 GMT  
		Size: 2.6 KB (2630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:054e8fde88d0e345bf3d5a7bb06dd62c56cc5b26713a0a27223e54f849a28d2c`  
		Last Modified: Wed, 07 Dec 2022 02:25:23 GMT  
		Size: 332.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2b494c50c7f5297000bd4e8bd09e9dbf84d44ffc5eb3e5028701db6a6749117`  
		Last Modified: Wed, 07 Dec 2022 02:25:30 GMT  
		Size: 56.1 MB (56063632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:132bc0d471b8b86912c8fff2877e1b2fcab03fdcbefa81630f33cb60ba5455c7`  
		Last Modified: Wed, 07 Dec 2022 02:25:21 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:135ec7033a05d2a5153f07e0b7983246a867df3c29a0fafc5ae47c90c35a1bf4`  
		Last Modified: Wed, 07 Dec 2022 02:25:31 GMT  
		Size: 55.1 MB (55106545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5961f02724723ffcd87c7e08efc9beb635496e32e530de0976755bf24843153b`  
		Last Modified: Wed, 07 Dec 2022 02:25:21 GMT  
		Size: 5.4 KB (5391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75b5f7a3d3a49109ed3673860a5c5ed0f3f070b099b59dfc9b1c45761ca1aaca`  
		Last Modified: Wed, 07 Dec 2022 02:25:21 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:latest` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:abd7d1e4a42b96a58c702db2633df611d201789b07c01749dac1aff97b83ba8f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **159.0 MB (159024595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b6f3978ca2905ae9bc14cfe86ae2f004f8c36561b722a06f64b73001b1898a5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 07 Dec 2022 02:10:44 GMT
ADD file:6fdd782c2779edf7149126e79dcb46ebde32975107cdd5d129cce0860e797cde in / 
# Wed, 07 Dec 2022 02:10:44 GMT
CMD ["/bin/bash"]
# Wed, 07 Dec 2022 02:50:18 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 07 Dec 2022 02:50:18 GMT
ENV GOSU_VERSION=1.14
# Wed, 07 Dec 2022 02:50:22 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 07 Dec 2022 02:50:43 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Wed, 07 Dec 2022 02:50:44 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 07 Dec 2022 02:50:44 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 07 Dec 2022 02:50:44 GMT
ENV MYSQL_VERSION=8.0.31-1.el8
# Wed, 07 Dec 2022 02:50:44 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 07 Dec 2022 02:51:09 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 07 Dec 2022 02:51:10 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 07 Dec 2022 02:51:10 GMT
ENV MYSQL_SHELL_VERSION=8.0.31-1.el8
# Wed, 07 Dec 2022 02:51:38 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Wed, 07 Dec 2022 02:51:39 GMT
VOLUME [/var/lib/mysql]
# Wed, 07 Dec 2022 02:51:39 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 07 Dec 2022 02:51:40 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 07 Dec 2022 02:51:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 07 Dec 2022 02:51:40 GMT
EXPOSE 3306 33060
# Wed, 07 Dec 2022 02:51:40 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:12a06ca91af857ea3cb02aedc5c643c5f06865868ae5c386c8ea664be60ead7e`  
		Last Modified: Wed, 07 Dec 2022 02:12:09 GMT  
		Size: 42.8 MB (42772059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fec1cb1944f64443d61a29e94cddba36d0cb8a09c80e0247375445bc62b842e`  
		Last Modified: Wed, 07 Dec 2022 02:52:10 GMT  
		Size: 887.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aede38c79379349fd3e9d191f92be36e68adc230840ae21c015f166b96e2067a`  
		Last Modified: Wed, 07 Dec 2022 02:52:10 GMT  
		Size: 857.2 KB (857168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51b980849561d1ed6bffe5deb621498e150f4f0f148af7a2654dd90ed42d7bfb`  
		Last Modified: Wed, 07 Dec 2022 02:52:09 GMT  
		Size: 4.5 MB (4464908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f503d79ed4bc3c439b28068291b1260757ab2de86163c8954962d88ff917e22a`  
		Last Modified: Wed, 07 Dec 2022 02:52:08 GMT  
		Size: 2.6 KB (2624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fb44db361f7e1027fb0010e8a3447c6e9337f6685ab4901f57030d01f730f74`  
		Last Modified: Wed, 07 Dec 2022 02:52:08 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:943b6dcee7dec15078e15da5cf8750748ae482bd7f5f206ecee44f5627229836`  
		Last Modified: Wed, 07 Dec 2022 02:52:13 GMT  
		Size: 55.4 MB (55444877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:911277c1fe4b4a08873f70cde5b84e7b38fd3d1c31c9c884baff83bd23886c96`  
		Last Modified: Wed, 07 Dec 2022 02:52:06 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a477017d045777c9cc1150499a65250c49ffd0669c2fa9fa8b64fb9e73cd353c`  
		Last Modified: Wed, 07 Dec 2022 02:52:14 GMT  
		Size: 55.5 MB (55475909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84b5061403a5151af9ccac6299ba1e8037c8f7a049dcc22e8808fd0095566e88`  
		Last Modified: Wed, 07 Dec 2022 02:52:06 GMT  
		Size: 5.4 KB (5392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ff27d035d66da6c178b69b95ddb8d8e913e206938df13d13dc0de764684b8c5`  
		Last Modified: Wed, 07 Dec 2022 02:52:06 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mysql:oracle`

```console
$ docker pull mysql@sha256:3d7ae561cf6095f6aca8eb7830e1d14734227b1fb4748092f2be2cfbccf7d614
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:oracle` - linux; amd64

```console
$ docker pull mysql@sha256:cfddf275c8b1ae1583c0f6afb4899d4dbe14111a6462699559a1f4dc8f4d5f6e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **160.6 MB (160585430 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7484689f290f1defe06b65befc54cb6ad91a667cf0af59a265ffe76c46bd0478`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 07 Dec 2022 01:51:27 GMT
ADD file:04d9ae26c2acac414b69a784563f765d531aeaf941ea0341025b4544f9ade244 in / 
# Wed, 07 Dec 2022 01:51:27 GMT
CMD ["/bin/bash"]
# Wed, 07 Dec 2022 02:21:54 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 07 Dec 2022 02:21:55 GMT
ENV GOSU_VERSION=1.14
# Wed, 07 Dec 2022 02:21:58 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 07 Dec 2022 02:22:21 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Wed, 07 Dec 2022 02:22:22 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 07 Dec 2022 02:22:23 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 07 Dec 2022 02:22:23 GMT
ENV MYSQL_VERSION=8.0.31-1.el8
# Wed, 07 Dec 2022 02:22:23 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 07 Dec 2022 02:22:53 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 07 Dec 2022 02:22:54 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 07 Dec 2022 02:22:54 GMT
ENV MYSQL_SHELL_VERSION=8.0.31-1.el8
# Wed, 07 Dec 2022 02:23:29 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Wed, 07 Dec 2022 02:23:30 GMT
VOLUME [/var/lib/mysql]
# Wed, 07 Dec 2022 02:23:30 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 07 Dec 2022 02:23:31 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 07 Dec 2022 02:23:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 07 Dec 2022 02:23:31 GMT
EXPOSE 3306 33060
# Wed, 07 Dec 2022 02:23:31 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:0ed027b72ddc5d1a749fc58b7c26610167393b08ae71ef6625496508903f70a2`  
		Last Modified: Wed, 07 Dec 2022 01:53:11 GMT  
		Size: 43.9 MB (43868738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0296159747f12f208fbf9721970ca290348698ac443cf98311477b6e44f18acc`  
		Last Modified: Wed, 07 Dec 2022 02:25:25 GMT  
		Size: 886.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d2f9b664bd354b5b8823bbdda42cf0813f2d8d3b5693f952c0a8516af84a826`  
		Last Modified: Wed, 07 Dec 2022 02:25:25 GMT  
		Size: 928.8 KB (928835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df6519f81c2689152b478834162cfe2f21ef37c472108a3e3a03a6ac0f5cbdd9`  
		Last Modified: Wed, 07 Dec 2022 02:25:24 GMT  
		Size: 4.6 MB (4608004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36bb5e56d458a7652c87ab8c3909c0ad098feaa81e73649bb37704701ca3ee6d`  
		Last Modified: Wed, 07 Dec 2022 02:25:23 GMT  
		Size: 2.6 KB (2630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:054e8fde88d0e345bf3d5a7bb06dd62c56cc5b26713a0a27223e54f849a28d2c`  
		Last Modified: Wed, 07 Dec 2022 02:25:23 GMT  
		Size: 332.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2b494c50c7f5297000bd4e8bd09e9dbf84d44ffc5eb3e5028701db6a6749117`  
		Last Modified: Wed, 07 Dec 2022 02:25:30 GMT  
		Size: 56.1 MB (56063632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:132bc0d471b8b86912c8fff2877e1b2fcab03fdcbefa81630f33cb60ba5455c7`  
		Last Modified: Wed, 07 Dec 2022 02:25:21 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:135ec7033a05d2a5153f07e0b7983246a867df3c29a0fafc5ae47c90c35a1bf4`  
		Last Modified: Wed, 07 Dec 2022 02:25:31 GMT  
		Size: 55.1 MB (55106545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5961f02724723ffcd87c7e08efc9beb635496e32e530de0976755bf24843153b`  
		Last Modified: Wed, 07 Dec 2022 02:25:21 GMT  
		Size: 5.4 KB (5391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75b5f7a3d3a49109ed3673860a5c5ed0f3f070b099b59dfc9b1c45761ca1aaca`  
		Last Modified: Wed, 07 Dec 2022 02:25:21 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:oracle` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:abd7d1e4a42b96a58c702db2633df611d201789b07c01749dac1aff97b83ba8f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **159.0 MB (159024595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b6f3978ca2905ae9bc14cfe86ae2f004f8c36561b722a06f64b73001b1898a5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 07 Dec 2022 02:10:44 GMT
ADD file:6fdd782c2779edf7149126e79dcb46ebde32975107cdd5d129cce0860e797cde in / 
# Wed, 07 Dec 2022 02:10:44 GMT
CMD ["/bin/bash"]
# Wed, 07 Dec 2022 02:50:18 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 07 Dec 2022 02:50:18 GMT
ENV GOSU_VERSION=1.14
# Wed, 07 Dec 2022 02:50:22 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 07 Dec 2022 02:50:43 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Wed, 07 Dec 2022 02:50:44 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 07 Dec 2022 02:50:44 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 07 Dec 2022 02:50:44 GMT
ENV MYSQL_VERSION=8.0.31-1.el8
# Wed, 07 Dec 2022 02:50:44 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 07 Dec 2022 02:51:09 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 07 Dec 2022 02:51:10 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 07 Dec 2022 02:51:10 GMT
ENV MYSQL_SHELL_VERSION=8.0.31-1.el8
# Wed, 07 Dec 2022 02:51:38 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Wed, 07 Dec 2022 02:51:39 GMT
VOLUME [/var/lib/mysql]
# Wed, 07 Dec 2022 02:51:39 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Wed, 07 Dec 2022 02:51:40 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 07 Dec 2022 02:51:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 07 Dec 2022 02:51:40 GMT
EXPOSE 3306 33060
# Wed, 07 Dec 2022 02:51:40 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:12a06ca91af857ea3cb02aedc5c643c5f06865868ae5c386c8ea664be60ead7e`  
		Last Modified: Wed, 07 Dec 2022 02:12:09 GMT  
		Size: 42.8 MB (42772059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fec1cb1944f64443d61a29e94cddba36d0cb8a09c80e0247375445bc62b842e`  
		Last Modified: Wed, 07 Dec 2022 02:52:10 GMT  
		Size: 887.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aede38c79379349fd3e9d191f92be36e68adc230840ae21c015f166b96e2067a`  
		Last Modified: Wed, 07 Dec 2022 02:52:10 GMT  
		Size: 857.2 KB (857168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51b980849561d1ed6bffe5deb621498e150f4f0f148af7a2654dd90ed42d7bfb`  
		Last Modified: Wed, 07 Dec 2022 02:52:09 GMT  
		Size: 4.5 MB (4464908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f503d79ed4bc3c439b28068291b1260757ab2de86163c8954962d88ff917e22a`  
		Last Modified: Wed, 07 Dec 2022 02:52:08 GMT  
		Size: 2.6 KB (2624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fb44db361f7e1027fb0010e8a3447c6e9337f6685ab4901f57030d01f730f74`  
		Last Modified: Wed, 07 Dec 2022 02:52:08 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:943b6dcee7dec15078e15da5cf8750748ae482bd7f5f206ecee44f5627229836`  
		Last Modified: Wed, 07 Dec 2022 02:52:13 GMT  
		Size: 55.4 MB (55444877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:911277c1fe4b4a08873f70cde5b84e7b38fd3d1c31c9c884baff83bd23886c96`  
		Last Modified: Wed, 07 Dec 2022 02:52:06 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a477017d045777c9cc1150499a65250c49ffd0669c2fa9fa8b64fb9e73cd353c`  
		Last Modified: Wed, 07 Dec 2022 02:52:14 GMT  
		Size: 55.5 MB (55475909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84b5061403a5151af9ccac6299ba1e8037c8f7a049dcc22e8808fd0095566e88`  
		Last Modified: Wed, 07 Dec 2022 02:52:06 GMT  
		Size: 5.4 KB (5392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ff27d035d66da6c178b69b95ddb8d8e913e206938df13d13dc0de764684b8c5`  
		Last Modified: Wed, 07 Dec 2022 02:52:06 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
