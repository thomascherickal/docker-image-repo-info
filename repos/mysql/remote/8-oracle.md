## `mysql:8-oracle`

```console
$ docker pull mysql@sha256:dd29f448c221a5ccd8d7545394772af6fe02925935e45a1c1e803ca1c08274f5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:29ea1f451c3aad88df5a24288f76442286dc7fa6874d96a022e93a8a7efda880
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **165.7 MB (165650520 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91b53e2624b431e562ed9076a9a506c5e78387f2cb4dad5968fd51ade839baa1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 16 Jun 2023 00:20:42 GMT
ADD file:9f649031a04a4d0b24cc167d52bbd5ae3415fd808304c971291e35e75109822a in / 
# Fri, 16 Jun 2023 00:20:43 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 00:37:33 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Fri, 16 Jun 2023 00:37:33 GMT
ENV GOSU_VERSION=1.16
# Fri, 16 Jun 2023 00:37:36 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 16 Jun 2023 00:38:03 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Fri, 16 Jun 2023 00:38:04 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Fri, 16 Jun 2023 00:38:04 GMT
ENV MYSQL_MAJOR=8.0
# Fri, 16 Jun 2023 00:38:04 GMT
ENV MYSQL_VERSION=8.0.33-1.el8
# Fri, 16 Jun 2023 00:38:04 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Fri, 16 Jun 2023 00:38:37 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Fri, 16 Jun 2023 00:38:38 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Fri, 16 Jun 2023 00:38:38 GMT
ENV MYSQL_SHELL_VERSION=8.0.33-1.el8
# Fri, 16 Jun 2023 00:39:15 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Fri, 16 Jun 2023 00:39:16 GMT
VOLUME [/var/lib/mysql]
# Fri, 16 Jun 2023 00:39:16 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Fri, 16 Jun 2023 00:39:16 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 16 Jun 2023 00:39:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 00:39:16 GMT
EXPOSE 3306 33060
# Fri, 16 Jun 2023 00:39:17 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:46ef68baacb785b3cf2f2826bfce791acb5264bed0fdf301623ac0c3c57f4daf`  
		Last Modified: Fri, 16 Jun 2023 00:22:14 GMT  
		Size: 44.9 MB (44871780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94c1114b2e9c0ba99041080c16f9cd2cc0b58f3ba47400cbeded060ae9aa2a58`  
		Last Modified: Fri, 16 Jun 2023 00:39:47 GMT  
		Size: 886.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff05e3f388023fb59f887c07497c9d09720f06e7c9c0641c8650c91219d992ef`  
		Last Modified: Fri, 16 Jun 2023 00:39:47 GMT  
		Size: 982.8 KB (982821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41cc3fcd99122af19a3586bbd08f963df55c278e637c28789868871e57ac52be`  
		Last Modified: Fri, 16 Jun 2023 00:39:46 GMT  
		Size: 4.6 MB (4612914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07bbc8bdf52a1396cf678cea6022e4ddd772594aa67be88ee5d2526dca4f8119`  
		Last Modified: Fri, 16 Jun 2023 00:39:45 GMT  
		Size: 2.6 KB (2629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d88f83726a9409e62c9e5bdbe16cfe138ef4815a0e60012438c6df0e3170102`  
		Last Modified: Fri, 16 Jun 2023 00:39:45 GMT  
		Size: 335.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf5c7d5d33f72689fd134bf4550db3753da17ad9ac56aa5bd15f7b9a1bb7453c`  
		Last Modified: Fri, 16 Jun 2023 00:39:52 GMT  
		Size: 58.6 MB (58602433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9db3175a2a660e9718faf64d43427ec34dd44af39a81c68c2a231bf10f6ae1c9`  
		Last Modified: Fri, 16 Jun 2023 00:39:43 GMT  
		Size: 319.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feaedeb27fa9b58368158724d925fe3ceda7fc4db137e4c56a6fb9f25a24e5d2`  
		Last Modified: Fri, 16 Jun 2023 00:39:53 GMT  
		Size: 56.6 MB (56570890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf91e7784414e9912ef38afc2c6771177cd73be84a212ba7fe23799f66e9699f`  
		Last Modified: Fri, 16 Jun 2023 00:39:43 GMT  
		Size: 5.4 KB (5392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1770db1c329de5a86e8685058094ee739297578f72fbfb376991078c288c59f`  
		Last Modified: Fri, 16 Jun 2023 00:39:43 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8-oracle` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:1d42cf001a7bd8cb99fcc41ff98730b69094317cd3f78f9e9990c289e193da7e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.4 MB (169420967 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:772571a08c67835aed7436d84973e885cc439b6cdd4dd1cc661a907d8acd3591`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Tue, 04 Jul 2023 00:52:20 GMT
ADD file:1313260ee8b32fa94bcf06c44034cd7e4f9baf44c7df9e74facfe21323b37292 in / 
# Tue, 04 Jul 2023 00:52:21 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 01:28:04 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Tue, 04 Jul 2023 01:28:04 GMT
ENV GOSU_VERSION=1.16
# Tue, 04 Jul 2023 01:28:07 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 04 Jul 2023 01:28:31 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Tue, 04 Jul 2023 01:28:33 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Tue, 04 Jul 2023 01:28:33 GMT
ENV MYSQL_MAJOR=8.0
# Tue, 04 Jul 2023 01:28:33 GMT
ENV MYSQL_VERSION=8.0.33-1.el8
# Tue, 04 Jul 2023 01:28:33 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Tue, 04 Jul 2023 01:29:02 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Tue, 04 Jul 2023 01:29:04 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Tue, 04 Jul 2023 01:29:04 GMT
ENV MYSQL_SHELL_VERSION=8.0.33-1.el8
# Tue, 04 Jul 2023 01:29:38 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Tue, 04 Jul 2023 01:29:40 GMT
VOLUME [/var/lib/mysql]
# Tue, 04 Jul 2023 01:29:40 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Tue, 04 Jul 2023 01:29:40 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 04 Jul 2023 01:29:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 01:29:41 GMT
EXPOSE 3306 33060
# Tue, 04 Jul 2023 01:29:41 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:29e800056b7e3d5007df41c0ad55416bb45d5863affcf39316c5755e71b20a30`  
		Last Modified: Tue, 04 Jul 2023 00:53:16 GMT  
		Size: 43.6 MB (43595268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69da292eb326146b0c10267953b72d6fcd767e284c36c30d51473fbcb67ca5a2`  
		Last Modified: Tue, 04 Jul 2023 01:30:08 GMT  
		Size: 885.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8850ef02dd581452d67b8bb9f54cd949b21fb95ff57bde8fadec5902bd385695`  
		Last Modified: Tue, 04 Jul 2023 01:30:08 GMT  
		Size: 913.0 KB (913006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86a76caa9e2025c7ecf56e460c12252a1216f8ac7773a0c7b289628b6c53760d`  
		Last Modified: Tue, 04 Jul 2023 01:30:07 GMT  
		Size: 4.3 MB (4298277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:881324b108321b7769c7d33bb4b0d2ae626a06ae82441448e5d3c1c5e0eebf77`  
		Last Modified: Tue, 04 Jul 2023 01:30:06 GMT  
		Size: 2.6 KB (2631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f5d1a8fa489bd8a99aeade310f01d71c431979332edfd44d3f2f02c7fa531fb`  
		Last Modified: Tue, 04 Jul 2023 01:30:06 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5efbe9eacf59876277173d2d29ad4fbe9be9678e82ea7308ef0f816b862a0653`  
		Last Modified: Tue, 04 Jul 2023 01:30:09 GMT  
		Size: 57.7 MB (57696479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80db22f26c0faf0e95ac6454baa4179c1c6481a688d8473246a212c1cfe9ee24`  
		Last Modified: Tue, 04 Jul 2023 01:30:04 GMT  
		Size: 320.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5595b935c31c94590c65a3bd92f06b5f4e56874b04b4d8c351cd03327c4c7dc`  
		Last Modified: Tue, 04 Jul 2023 01:30:12 GMT  
		Size: 62.9 MB (62908250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c391d4efe15967c07ecfcbb07109613e9d801d994a094624dc6881fec27f5eb7`  
		Last Modified: Tue, 04 Jul 2023 01:30:04 GMT  
		Size: 5.4 KB (5396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5527cf2eb5f0f72a2582baa44f61182d16ea054b51bff962ef6760480e17ba9`  
		Last Modified: Tue, 04 Jul 2023 01:30:04 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
