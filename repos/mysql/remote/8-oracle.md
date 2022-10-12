## `mysql:8-oracle`

```console
$ docker pull mysql@sha256:147572c972192417add6f1cf65ea33edfd44086e461a3381601b53e1662f5d15
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:fb3d8639a938515aaac38acb13c4acc061366a20322c55bbedae9d127cd2f2b3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **157.3 MB (157265417 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40b83de8fb1a29d9b47d3ecbff86f67d22f8418f6e6ef5d349aaca2c2919074a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 12 Oct 2022 21:20:42 GMT
ADD file:ceac4c0bc6dd71b3868d5af15bdaab832a2f61b45c12116b2df42ef8cfbf9fa1 in / 
# Wed, 12 Oct 2022 21:20:42 GMT
CMD ["/bin/bash"]
# Wed, 12 Oct 2022 21:37:29 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 12 Oct 2022 21:37:29 GMT
ENV GOSU_VERSION=1.14
# Wed, 12 Oct 2022 21:37:33 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 12 Oct 2022 21:37:56 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Wed, 12 Oct 2022 21:37:57 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 12 Oct 2022 21:37:58 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 12 Oct 2022 21:37:58 GMT
ENV MYSQL_VERSION=8.0.31-1.el8
# Wed, 12 Oct 2022 21:37:58 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 12 Oct 2022 21:38:28 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 12 Oct 2022 21:38:29 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 12 Oct 2022 21:38:29 GMT
ENV MYSQL_SHELL_VERSION=8.0.31-1.el8
# Wed, 12 Oct 2022 21:39:03 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Wed, 12 Oct 2022 21:39:04 GMT
VOLUME [/var/lib/mysql]
# Wed, 12 Oct 2022 21:39:04 GMT
COPY file:5e84598933ec95c9918378d8dde5be8d5f80b0e1fc321a029f840f313201ebce in /usr/local/bin/ 
# Wed, 12 Oct 2022 21:39:04 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 12 Oct 2022 21:39:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 Oct 2022 21:39:05 GMT
EXPOSE 3306 33060
# Wed, 12 Oct 2022 21:39:05 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:5ed150ed0abef03007b46722de75bcb3e517f22532a46146fcec4fb1761d4347`  
		Last Modified: Wed, 12 Oct 2022 21:22:08 GMT  
		Size: 40.6 MB (40589408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fede58e17ac8f886aa620315c1c85d2979e38aa05aebf00aacba6d240a18620`  
		Last Modified: Wed, 12 Oct 2022 21:39:40 GMT  
		Size: 886.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:994a6ddd6efe5eef3b2be88576cfa2e823d47f0c7db10554360438631d0f786b`  
		Last Modified: Wed, 12 Oct 2022 21:39:41 GMT  
		Size: 928.8 KB (928832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:028bda79779b4b2f4b249922d92841289aeae64aea45154be16cd17cfe986fdd`  
		Last Modified: Wed, 12 Oct 2022 21:39:39 GMT  
		Size: 4.6 MB (4606927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:426fbe9e56a28ac107f62e7fb3b835c320ff0997c762490c853ae8242765da9f`  
		Last Modified: Wed, 12 Oct 2022 21:39:38 GMT  
		Size: 2.6 KB (2630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a00e58dd193f3585ff724fd8ba4f7c78d83cf33b851a186b925b36317542f34`  
		Last Modified: Wed, 12 Oct 2022 21:39:38 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a4f64494005d7365861de3808b1c39783259162154a12b6b6694e5303732c2b`  
		Last Modified: Wed, 12 Oct 2022 21:39:45 GMT  
		Size: 56.0 MB (56046404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fba8ab3534a7c32755a032486836b05d3d5a724ba6e7127ce259a0ea02fae975`  
		Last Modified: Wed, 12 Oct 2022 21:39:36 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2695938edf88c0409d640f6edcb00898d28478ed80505fd449f6c05c2b99ec3d`  
		Last Modified: Wed, 12 Oct 2022 21:39:46 GMT  
		Size: 55.1 MB (55084174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3754e2587bed8ece9b5713bcb14924d27691927399a3750fb6d8ebceb000d771`  
		Last Modified: Wed, 12 Oct 2022 21:39:36 GMT  
		Size: 5.4 KB (5385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b9f154543e74f792239c3ac5377c8deb20f3956a8e60db04486c4313c0979d7`  
		Last Modified: Wed, 12 Oct 2022 21:39:36 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8-oracle` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:4a90a0b47798672d3e19064171610cd055cb1d5b702dcf67d6c675c9cb61a96d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.6 MB (155564637 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:262f364f4f01337f2027e10c7ca2994dc28883afb24386100c89351126d76fe4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 12 Oct 2022 20:40:56 GMT
ADD file:049ff2e28998fde860d1a12f43ec245d10345a71953f67108180c23c237ce26e in / 
# Wed, 12 Oct 2022 20:40:56 GMT
CMD ["/bin/bash"]
# Wed, 12 Oct 2022 21:24:43 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Wed, 12 Oct 2022 21:24:43 GMT
ENV GOSU_VERSION=1.14
# Wed, 12 Oct 2022 21:24:47 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 12 Oct 2022 21:25:15 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Wed, 12 Oct 2022 21:25:17 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Wed, 12 Oct 2022 21:25:18 GMT
ENV MYSQL_MAJOR=8.0
# Wed, 12 Oct 2022 21:25:19 GMT
ENV MYSQL_VERSION=8.0.31-1.el8
# Wed, 12 Oct 2022 21:25:20 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Wed, 12 Oct 2022 21:25:52 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Wed, 12 Oct 2022 21:25:53 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Wed, 12 Oct 2022 21:25:54 GMT
ENV MYSQL_SHELL_VERSION=8.0.31-1.el8
# Wed, 12 Oct 2022 21:26:33 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Wed, 12 Oct 2022 21:26:34 GMT
VOLUME [/var/lib/mysql]
# Wed, 12 Oct 2022 21:26:36 GMT
COPY file:5e84598933ec95c9918378d8dde5be8d5f80b0e1fc321a029f840f313201ebce in /usr/local/bin/ 
# Wed, 12 Oct 2022 21:26:37 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 12 Oct 2022 21:26:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 Oct 2022 21:26:38 GMT
EXPOSE 3306 33060
# Wed, 12 Oct 2022 21:26:39 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:828689dcde4b0fe396ab27cf3a6d5f71ee01d48891421ec4381d74ed415be5d0`  
		Last Modified: Wed, 12 Oct 2022 20:42:33 GMT  
		Size: 39.4 MB (39409290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f061378e43d33dc614866c620ab52f8985729cda946779352b12f6a73d099d3`  
		Last Modified: Wed, 12 Oct 2022 21:27:19 GMT  
		Size: 888.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b1a79ec4c767ad1034121ce2905bb5a3326d01d2c3e24a384b55d34a923bcba`  
		Last Modified: Wed, 12 Oct 2022 21:27:19 GMT  
		Size: 857.1 KB (857150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29639854082a90b6e050d61546185cee56cbc0a0224e0a37222ab57bd00917d3`  
		Last Modified: Wed, 12 Oct 2022 21:27:18 GMT  
		Size: 4.4 MB (4433340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7be1d8abaf67b766b14bd7b5ee219ce3181b651617cede1fbef78809e83ae2f3`  
		Last Modified: Wed, 12 Oct 2022 21:27:17 GMT  
		Size: 2.6 KB (2607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:862924992b62147c16c1cad215c391bd43f107b291971074dda31445e6171439`  
		Last Modified: Wed, 12 Oct 2022 21:27:15 GMT  
		Size: 333.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d8afc4c260a8060504c3a8696a68694051c62b5dad9774d6b95cc57e9cc10c7`  
		Last Modified: Wed, 12 Oct 2022 21:27:21 GMT  
		Size: 55.4 MB (55421557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fb5afa1cf8a3c9f31ed89a4b56cdf88a1d9638c5cadbfc1d8e971265c90892b`  
		Last Modified: Wed, 12 Oct 2022 21:27:13 GMT  
		Size: 319.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:693834f1d9bae56fd201dd9a4d7b2eadf83d04d230f650f0c1948876324517e8`  
		Last Modified: Wed, 12 Oct 2022 21:27:23 GMT  
		Size: 55.4 MB (55433646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3411c71dcce2f58523c25058a0800a7e635b92e410e805a30120b936e51a2cb8`  
		Last Modified: Wed, 12 Oct 2022 21:27:16 GMT  
		Size: 5.4 KB (5386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:877257953583c21228d6fcef6578b5bdfe8729c7f6ee6b366bade14693a92fa5`  
		Last Modified: Wed, 12 Oct 2022 21:27:14 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
