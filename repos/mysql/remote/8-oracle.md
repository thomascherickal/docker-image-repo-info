## `mysql:8-oracle`

```console
$ docker pull mysql@sha256:3de4d9814b28e48f225e259cc3b2c77530296afcec20bae53e1c7a4892f2a98e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:8-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:930e762c3f185d55d96a65e0d6cb2f724ffc16a87270f85283ae099d75e92ad0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.5 MB (132502250 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c989cc040bcf09e776e701e0fb567045ee77ed8667daf1a506d898717011bfe5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 04 Aug 2022 00:36:37 GMT
ADD file:0a05a213ae66f556b2b320291ac58ec9f2f67554e29338a072f1347f22864a49 in / 
# Thu, 04 Aug 2022 00:36:37 GMT
CMD ["/bin/bash"]
# Thu, 04 Aug 2022 01:24:42 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Thu, 04 Aug 2022 01:24:43 GMT
ENV GOSU_VERSION=1.14
# Thu, 04 Aug 2022 01:24:46 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 04 Aug 2022 01:25:08 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Thu, 04 Aug 2022 01:25:10 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Thu, 04 Aug 2022 01:25:10 GMT
ENV MYSQL_MAJOR=8.0
# Thu, 04 Aug 2022 01:25:10 GMT
ENV MYSQL_VERSION=8.0.30-1.el8
# Thu, 04 Aug 2022 01:25:10 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Thu, 04 Aug 2022 01:25:38 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Thu, 04 Aug 2022 01:25:39 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Thu, 04 Aug 2022 01:25:39 GMT
ENV MYSQL_SHELL_VERSION=8.0.30-1.el8
# Thu, 04 Aug 2022 01:26:10 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Thu, 04 Aug 2022 01:26:11 GMT
VOLUME [/var/lib/mysql]
# Wed, 24 Aug 2022 00:36:48 GMT
COPY file:0362167b353388be7fb99432d9373f030ddd789bd27d57e183555c672530b303 in /usr/local/bin/ 
# Wed, 24 Aug 2022 00:36:48 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 24 Aug 2022 00:36:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 24 Aug 2022 00:36:49 GMT
EXPOSE 3306 33060
# Wed, 24 Aug 2022 00:36:49 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:32c1bf40aba1f372a057d3280b0b7cdacde9d8500a069004e6f243bc09cde806`  
		Last Modified: Thu, 04 Aug 2022 00:37:33 GMT  
		Size: 39.2 MB (39223952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ac22f3a638d1c75f850c6c7b189d746c1ec6c58ec618f9e4b928f045df1b79d`  
		Last Modified: Thu, 04 Aug 2022 01:26:53 GMT  
		Size: 890.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1e7273ed05ed3b0f6be1e9a202f93199d88428c9dff52d1edce8d965ad50f8e`  
		Last Modified: Thu, 04 Aug 2022 01:26:54 GMT  
		Size: 928.8 KB (928835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20be45a0c6abbfaf62bd02c40f3cff6bf4822711b339ebcd4e1b7d6b2764ca20`  
		Last Modified: Thu, 04 Aug 2022 01:26:52 GMT  
		Size: 4.6 MB (4581809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:410a229693ff98f0a019a180a655ad903a882367b72f78f0ac3c595c1434a65e`  
		Last Modified: Thu, 04 Aug 2022 01:26:51 GMT  
		Size: 2.6 KB (2628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ce71e3a9b8879afc4dce1dc74841ecbae7da28798b238c88f0322b7bdc82472`  
		Last Modified: Thu, 04 Aug 2022 01:26:51 GMT  
		Size: 335.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c93c823af05bbde448c0a889b94ef2d6279b9c595c9b1a1abcbd49f795f7631c`  
		Last Modified: Thu, 04 Aug 2022 01:26:56 GMT  
		Size: 47.7 MB (47726773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6752c4d09c7204097f7ecbf50885874b620e77263452bb581ed1f4d9681344d`  
		Last Modified: Thu, 04 Aug 2022 01:26:49 GMT  
		Size: 315.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7f2cfe3efcbd4b98bf44100e9f3fc095ca4a480fd75a0028bae61aedfb6298a`  
		Last Modified: Thu, 04 Aug 2022 01:26:57 GMT  
		Size: 40.0 MB (40031217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09e782dbb2c3f52fb09d97fee4689b382e3789e244c209fe81782420a19d1a2a`  
		Last Modified: Wed, 24 Aug 2022 00:37:25 GMT  
		Size: 5.4 KB (5375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01199f522543dd7f72aa6b05d1be8d67dc48483700d79db260348af7e69f2aaa`  
		Last Modified: Wed, 24 Aug 2022 00:37:24 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:8-oracle` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:54b1f5e74608236fe20d5dcdf39124a81244dd4d043b0798929614c1bc1ec602
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.2 MB (141193701 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1b9c6058e7a1b8f805b067ba9d4775d392fcfda1cdd601396716864c8f59e14`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 04 Aug 2022 00:40:43 GMT
ADD file:a68d82fa032efe6adc2926f7e745508f0541bba3f906e2702d34252353100747 in / 
# Thu, 04 Aug 2022 00:40:44 GMT
CMD ["/bin/bash"]
# Thu, 04 Aug 2022 00:57:16 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Thu, 04 Aug 2022 00:57:17 GMT
ENV GOSU_VERSION=1.14
# Thu, 04 Aug 2022 00:57:21 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 04 Aug 2022 00:57:44 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Thu, 04 Aug 2022 00:57:46 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Thu, 04 Aug 2022 00:57:47 GMT
ENV MYSQL_MAJOR=8.0
# Thu, 04 Aug 2022 00:57:48 GMT
ENV MYSQL_VERSION=8.0.30-1.el8
# Thu, 04 Aug 2022 00:57:49 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Thu, 04 Aug 2022 00:58:17 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Thu, 04 Aug 2022 00:58:17 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Thu, 04 Aug 2022 00:58:18 GMT
ENV MYSQL_SHELL_VERSION=8.0.30-1.el8
# Thu, 04 Aug 2022 00:58:50 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Thu, 04 Aug 2022 00:58:51 GMT
VOLUME [/var/lib/mysql]
# Wed, 24 Aug 2022 03:30:34 GMT
COPY file:0362167b353388be7fb99432d9373f030ddd789bd27d57e183555c672530b303 in /usr/local/bin/ 
# Wed, 24 Aug 2022 03:30:35 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 24 Aug 2022 03:30:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 24 Aug 2022 03:30:37 GMT
EXPOSE 3306 33060
# Wed, 24 Aug 2022 03:30:38 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:ecf56004177eb6ca162c88de29e84bc4ba3d2e7efd3703df9ecae51b89003d52`  
		Last Modified: Thu, 04 Aug 2022 00:41:51 GMT  
		Size: 38.0 MB (38023046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1091d9f012e1e44cf00d872494ff008feb11a824aa940f5fccaadcf0f043e951`  
		Last Modified: Thu, 04 Aug 2022 00:59:35 GMT  
		Size: 888.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fabd9779d4678f8577c74505cc31bd42788a9ffa1eba563340b8ef29946b3e55`  
		Last Modified: Thu, 04 Aug 2022 00:59:36 GMT  
		Size: 857.2 KB (857152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6278448e2e194f0e2e8e7d2f29495296d594f7bd2e63d0306037e5b4f5125eb`  
		Last Modified: Thu, 04 Aug 2022 00:59:34 GMT  
		Size: 4.4 MB (4404159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6050832741b8d8e4dfba20e0d31c88f56b9b645c97752c9bbec708740c3e6e15`  
		Last Modified: Thu, 04 Aug 2022 00:59:33 GMT  
		Size: 2.6 KB (2607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0be9d1181fe5f7d6c39819a56c680e5e010a7b808b96eb00eabdeacd66ee6c1`  
		Last Modified: Thu, 04 Aug 2022 00:59:33 GMT  
		Size: 335.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbdaffd3eb50f6880d4e27c2ba2a47193ba4e1959b4647e5e794b0872e981c5b`  
		Last Modified: Thu, 04 Aug 2022 00:59:38 GMT  
		Size: 53.8 MB (53784614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a74c1ad0f09fc99fb019bcbfebb1b57f4f7fcf7e968e6ece353a06d583cab8ed`  
		Last Modified: Thu, 04 Aug 2022 00:59:31 GMT  
		Size: 315.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad2b7db10f4eacccefc72231d395d9920b81dd4bba86be2a8994b8ee9161ec92`  
		Last Modified: Thu, 04 Aug 2022 00:59:38 GMT  
		Size: 44.1 MB (44115089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f6281129c7fb0746caa0023cec4db82b482c85d81752eaafcff70498537c82a`  
		Last Modified: Wed, 24 Aug 2022 03:31:04 GMT  
		Size: 5.4 KB (5375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49dcabdef3045b25265175bee4894568254c4b35b769d77a0afedc6fd7ec9a1d`  
		Last Modified: Wed, 24 Aug 2022 03:31:04 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
