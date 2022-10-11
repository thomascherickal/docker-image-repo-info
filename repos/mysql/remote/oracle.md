## `mysql:oracle`

```console
$ docker pull mysql@sha256:f71a0cd78ceda34e3e1a9f3c1e3dd27b220a15142b53b9d3e73d12a4fcaea513
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:oracle` - linux; amd64

```console
$ docker pull mysql@sha256:f90d1aeb92a5c7b3a4178a3052d8bc27b1f52a811aacb27b619c10b778b9f281
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.9 MB (133890226 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbaea59d1b4194257138a6434ec0820a13097dd7e900135e78daf9759fe2407a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 07 Oct 2022 20:31:40 GMT
ADD file:40e1b0533d9ae91c868834395cbd4b74cf2a47965791be201c03ae764f9da2b0 in / 
# Fri, 07 Oct 2022 20:31:41 GMT
CMD ["/bin/bash"]
# Fri, 07 Oct 2022 21:05:33 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Fri, 07 Oct 2022 21:05:33 GMT
ENV GOSU_VERSION=1.14
# Fri, 07 Oct 2022 21:05:36 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 07 Oct 2022 21:05:58 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Fri, 07 Oct 2022 21:06:00 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Fri, 07 Oct 2022 21:06:00 GMT
ENV MYSQL_MAJOR=8.0
# Fri, 07 Oct 2022 21:06:00 GMT
ENV MYSQL_VERSION=8.0.30-1.el8
# Fri, 07 Oct 2022 21:06:00 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Fri, 07 Oct 2022 21:06:28 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Fri, 07 Oct 2022 21:06:29 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Fri, 07 Oct 2022 21:06:29 GMT
ENV MYSQL_SHELL_VERSION=8.0.30-1.el8
# Fri, 07 Oct 2022 21:07:04 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Fri, 07 Oct 2022 21:07:04 GMT
VOLUME [/var/lib/mysql]
# Fri, 07 Oct 2022 21:07:05 GMT
COPY file:5e84598933ec95c9918378d8dde5be8d5f80b0e1fc321a029f840f313201ebce in /usr/local/bin/ 
# Fri, 07 Oct 2022 21:07:05 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 07 Oct 2022 21:07:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Oct 2022 21:07:05 GMT
EXPOSE 3306 33060
# Fri, 07 Oct 2022 21:07:05 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:295ca23427284cb123fd4c132a1ecb521e7f787ac75dadec342f744a343efec4`  
		Last Modified: Fri, 07 Oct 2022 20:33:22 GMT  
		Size: 40.6 MB (40589568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79af4312a7e0fb060724a99077fbd6a3460284520318bbfe874d11e472aed010`  
		Last Modified: Fri, 07 Oct 2022 21:08:51 GMT  
		Size: 887.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48d3d73d17046a044f9f4a45aa0f74afa79387dc1eb634ef96eb39a947b3077d`  
		Last Modified: Fri, 07 Oct 2022 21:08:51 GMT  
		Size: 928.8 KB (928836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:521b8724b397717c0920f045a0dc9b778426bb5ed5ff17f2ecaece3b27914fe3`  
		Last Modified: Fri, 07 Oct 2022 21:08:49 GMT  
		Size: 4.6 MB (4606973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8cf360b4a14d6543edc2e7f35ce87406aa7b82c29e252f8ef911f39dcbc6de2`  
		Last Modified: Fri, 07 Oct 2022 21:08:48 GMT  
		Size: 2.6 KB (2631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0115482cc006f85365a790dc394ead0f59f922046bb77b3509e6f7989b32b2a5`  
		Last Modified: Fri, 07 Oct 2022 21:08:48 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a360b08917ea13f41e1d042db0163b46c0069b93a5e2995543ab10fa70541e16`  
		Last Modified: Fri, 07 Oct 2022 21:08:54 GMT  
		Size: 47.7 MB (47733932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12deeb3c132385712ac84f6ab3842432f96d231682957f254fdb8400156b3736`  
		Last Modified: Fri, 07 Oct 2022 21:08:46 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee1dc10db1e9a87dda49ac546d7263db2fd5e6163aa17228c7d60f464bf91098`  
		Last Modified: Fri, 07 Oct 2022 21:08:53 GMT  
		Size: 40.0 MB (40021240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64be404ad29c0faf50a4c5855fcbbb8491b2f8fd89ac4df11b3a0b26f990a4da`  
		Last Modified: Fri, 07 Oct 2022 21:08:46 GMT  
		Size: 5.4 KB (5388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1921fe8879a2ef55d203b4ad84ee572904a1afb7b195013a82bc3568b85624e2`  
		Last Modified: Fri, 07 Oct 2022 21:08:46 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:oracle` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:8490ebfe3bb013177c180f0768129dcbea914c964656fc7eb430ab615dd7c2fd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.6 MB (155558318 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a0f9faac565852cc07eb311168d3bab14bd4326790f07f5194e6243a9279efea`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 07 Oct 2022 20:51:45 GMT
ADD file:6eb7b065ffe8855d82638de19bd23fba329883c96f01d093e7bc6bdb5da836a3 in / 
# Fri, 07 Oct 2022 20:51:46 GMT
CMD ["/bin/bash"]
# Fri, 07 Oct 2022 21:09:40 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Fri, 07 Oct 2022 21:09:41 GMT
ENV GOSU_VERSION=1.14
# Fri, 07 Oct 2022 21:09:45 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 07 Oct 2022 21:10:14 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Fri, 07 Oct 2022 21:10:16 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Fri, 07 Oct 2022 21:10:17 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 11 Oct 2022 19:57:33 GMT
ENV MYSQL_VERSION=8.0.31-1.el8
# Tue, 11 Oct 2022 19:57:34 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Tue, 11 Oct 2022 19:58:03 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Tue, 11 Oct 2022 19:58:04 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Tue, 11 Oct 2022 19:58:05 GMT
ENV MYSQL_SHELL_VERSION=8.0.31-1.el8
# Tue, 11 Oct 2022 19:58:39 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Tue, 11 Oct 2022 19:58:40 GMT
VOLUME [/var/lib/mysql]
# Tue, 11 Oct 2022 19:58:41 GMT
COPY file:5e84598933ec95c9918378d8dde5be8d5f80b0e1fc321a029f840f313201ebce in /usr/local/bin/ 
# Tue, 11 Oct 2022 19:58:41 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 11 Oct 2022 19:58:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 11 Oct 2022 19:58:43 GMT
EXPOSE 3306 33060
# Tue, 11 Oct 2022 19:58:44 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:5d45c82139e084eb338a0a2346c4ec4c6d2bfa4acda9194cf6602728b4a3e89f`  
		Last Modified: Fri, 07 Oct 2022 20:53:34 GMT  
		Size: 39.4 MB (39409020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c544deffc3a52cba4e3a2ec48f677586760eb4717c161c4adebcb8ce20402a8`  
		Last Modified: Fri, 07 Oct 2022 21:12:14 GMT  
		Size: 888.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af07bf98dff8f0d9fa86a18b24151f9803947d9d622097b25bf3f5874b2bd6c9`  
		Last Modified: Fri, 07 Oct 2022 21:12:14 GMT  
		Size: 857.2 KB (857152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0554dfac498a04af357c6a46c1e81c7a38af77e0f18e416c035c3e64f7d9905e`  
		Last Modified: Fri, 07 Oct 2022 21:12:12 GMT  
		Size: 4.4 MB (4433409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f612237e783e94a541b8163f9f2a3d5d66b3b804fdddcd51e7b752f50f7ffaec`  
		Last Modified: Fri, 07 Oct 2022 21:12:11 GMT  
		Size: 2.6 KB (2610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7249cc35cb4b72d02bb0ec5f45d6742867a7ef9c71408f3a6c06cbc8a47ac885`  
		Last Modified: Tue, 11 Oct 2022 19:59:19 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41fea0f5462f60112533ea2946783960b74473253d3f26681e6289baa8e62e46`  
		Last Modified: Tue, 11 Oct 2022 19:59:25 GMT  
		Size: 55.4 MB (55421592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f227634493daa08c50c895e1a4ae3353b9c819de56b6bec0d72249b2c5868e9`  
		Last Modified: Tue, 11 Oct 2022 19:59:17 GMT  
		Size: 319.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:846b06f0fa9dbbb1c079065a179a74420ecb2e0d20963d3b077ff51c779cd27f`  
		Last Modified: Tue, 11 Oct 2022 19:59:27 GMT  
		Size: 55.4 MB (55427484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd488d76876a35a3de0441f1f7aa2c02774f1efef1451ba2e34122a2b8fb3222`  
		Last Modified: Tue, 11 Oct 2022 19:59:17 GMT  
		Size: 5.4 KB (5389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82bd893588df38744ddad3b6039f364344ad7bc8713e4dae5befe7696b3cfddd`  
		Last Modified: Tue, 11 Oct 2022 19:59:17 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
