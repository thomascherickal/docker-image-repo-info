## `mysql:8-oracle`

```console
$ docker pull mysql@sha256:15f069202c46cf861ce429423ae3f8dfa6423306fbf399eaef36094ce30dd75c
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
$ docker pull mysql@sha256:7d0a45fa34f810414c187b8e414828be93e8590ce89f91df5bd705d3d5b15b55
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.4 MB (169393383 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1732fe3340d5c0968312658c137eaa840f53c3bb83b5f962a67e3bdd784724b7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 15 Jun 2023 23:40:30 GMT
ADD file:37cef5fcd08f57d005adb8f14f69ecc78a9c669280f45f7d81b1c899489e93ba in / 
# Thu, 15 Jun 2023 23:40:31 GMT
CMD ["/bin/bash"]
# Thu, 15 Jun 2023 23:57:04 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Thu, 15 Jun 2023 23:57:04 GMT
ENV GOSU_VERSION=1.16
# Thu, 15 Jun 2023 23:57:07 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 15 Jun 2023 23:57:32 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Thu, 15 Jun 2023 23:57:34 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Thu, 15 Jun 2023 23:57:34 GMT
ENV MYSQL_MAJOR=8.0
# Thu, 15 Jun 2023 23:57:34 GMT
ENV MYSQL_VERSION=8.0.33-1.el8
# Thu, 15 Jun 2023 23:57:34 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Thu, 15 Jun 2023 23:58:02 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Thu, 15 Jun 2023 23:58:03 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Thu, 15 Jun 2023 23:58:03 GMT
ENV MYSQL_SHELL_VERSION=8.0.33-1.el8
# Thu, 15 Jun 2023 23:58:35 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Thu, 15 Jun 2023 23:58:36 GMT
VOLUME [/var/lib/mysql]
# Thu, 15 Jun 2023 23:58:36 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Thu, 15 Jun 2023 23:58:37 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 15 Jun 2023 23:58:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Jun 2023 23:58:37 GMT
EXPOSE 3306 33060
# Thu, 15 Jun 2023 23:58:37 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:029ab4a5f8e75aadbbba1505624cf10a4c35a0fd897cc85b9e7536785b8ba37c`  
		Last Modified: Thu, 15 Jun 2023 23:41:45 GMT  
		Size: 43.6 MB (43601336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:379e18ca6956bdccee2f520f4ccc7284781f399b535905304436bc35591490d2`  
		Last Modified: Thu, 15 Jun 2023 23:58:52 GMT  
		Size: 884.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:311296d6436fbeadfd03e0ae0355dcc5f5c1c98558f1614c769c7bdcff3b027e`  
		Last Modified: Thu, 15 Jun 2023 23:58:53 GMT  
		Size: 913.0 KB (912993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54e90a5b94ab12d36935e1a1a25334fe6fbd1f53268e896bdc55ad3d53af1825`  
		Last Modified: Thu, 15 Jun 2023 23:58:51 GMT  
		Size: 4.3 MB (4294980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db50017c9a15b71f9511f7f1f5a9711477d408a11c8264e41c89cb0e9a43b26`  
		Last Modified: Thu, 15 Jun 2023 23:58:50 GMT  
		Size: 2.6 KB (2629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:161c1da0ab84372390263bf0c351228b372f7a644e62a4119cbcf24f5d80db52`  
		Last Modified: Thu, 15 Jun 2023 23:58:50 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3edd797f390f0eaaee4fd70be5ab6000ec7a107da17615e56e136a36fd68c975`  
		Last Modified: Thu, 15 Jun 2023 23:58:55 GMT  
		Size: 57.7 MB (57684788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a4467fea2ad904bac6b4971ed2d25a804a158d13f73d3ac1462ba7d4727e0c6`  
		Last Modified: Thu, 15 Jun 2023 23:58:49 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ce24500a1de2c8409b9bb7a667cb5d30255c8c5208d4600de7e94f55e145a51`  
		Last Modified: Thu, 15 Jun 2023 23:58:56 GMT  
		Size: 62.9 MB (62889613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:083135b3ad0925a8ae1c9176583bdd752145ba88e670b100f38f85d422424b0c`  
		Last Modified: Thu, 15 Jun 2023 23:58:48 GMT  
		Size: 5.4 KB (5389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:250e3c290ce1494cfc96725e6ca52a984ded53b6b11965df8973a305bfcfe31c`  
		Last Modified: Thu, 15 Jun 2023 23:58:49 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
