## `mysql:5-oracle`

```console
$ docker pull mysql@sha256:c67e9e97879305e0c7a4934372f35bdb7d79d4a0914d7304d0ee6836be0127a8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:3030fdb1154e62ed44c2e2dbbc7dee2643ee27fb6dd201b06b19a87682498e8b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.9 MB (126873058 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f19b3d18c4a01f69bdb995e46233fcdcc66c1ef84bc8d28396e981c020e395ee`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 16 Jun 2022 01:20:22 GMT
ADD file:5e615d6d49ec50cba937fa86f5fb7d6a4a7e680b2b4f5b659e879b95304c0417 in / 
# Thu, 16 Jun 2022 01:20:22 GMT
CMD ["/bin/bash"]
# Thu, 16 Jun 2022 01:38:41 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql; 		mkdir /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d
# Thu, 16 Jun 2022 01:38:41 GMT
ENV GOSU_VERSION=1.14
# Thu, 16 Jun 2022 01:38:45 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 16 Jun 2022 01:38:55 GMT
RUN set -eux; 	yum install -y 		gzip 		openssl 		xz 		zstd 	; 	yum clean all
# Thu, 16 Jun 2022 01:38:56 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Thu, 16 Jun 2022 01:38:56 GMT
ENV MYSQL_MAJOR=5.7
# Thu, 16 Jun 2022 01:38:56 GMT
ENV MYSQL_VERSION=5.7.38-1.el7
# Thu, 16 Jun 2022 01:38:57 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql5.7-server-minimal]'; 		echo 'name=MySQL 5.7 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-5.7-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Thu, 16 Jun 2022 01:39:11 GMT
RUN set -eux; 	yum install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	yum clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 		mysqld --version; 	mysql --version
# Thu, 16 Jun 2022 01:39:11 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Thu, 16 Jun 2022 01:39:12 GMT
ENV MYSQL_SHELL_VERSION=8.0.29-1.el7
# Thu, 16 Jun 2022 01:39:29 GMT
RUN set -eux; 	yum install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	yum clean all; 		mysqlsh --version
# Thu, 16 Jun 2022 01:39:30 GMT
VOLUME [/var/lib/mysql]
# Thu, 16 Jun 2022 01:39:30 GMT
COPY file:d27cf504fa76fb5a4038020a01eaaf52723b17b751566119de311adacb043752 in /usr/local/bin/ 
# Thu, 16 Jun 2022 01:39:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 16 Jun 2022 01:39:31 GMT
EXPOSE 3306 33060
# Thu, 16 Jun 2022 01:39:31 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:63183c9b4598e16c4cef95f706d50ff6c928de41f391cd513495b27eaa27bf89`  
		Last Modified: Thu, 16 Jun 2022 01:21:08 GMT  
		Size: 48.8 MB (48757931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:921fb508f1d1aecc5558b119c43c60ca99e2803d417ea98b5a55f94975ac5440`  
		Last Modified: Thu, 16 Jun 2022 01:40:10 GMT  
		Size: 1.1 KB (1059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c722a284ecb6bbcc3803b2a9fb3df9e58ebd491e421507db7c73d8f4255cf0f4`  
		Last Modified: Thu, 16 Jun 2022 01:40:09 GMT  
		Size: 930.2 KB (930225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e1ea46ae00991c24638c08d268652beb0ce5b878c83d34964f12345618c8941`  
		Last Modified: Thu, 16 Jun 2022 01:40:11 GMT  
		Size: 3.8 MB (3750823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e15dccdcd437d9fe54d225731d32bb52246dc75794a5d49e7f12010322dd06c1`  
		Last Modified: Thu, 16 Jun 2022 01:40:08 GMT  
		Size: 2.7 KB (2659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1050fbf8b84448d369e5743034ffd13580e9313a7e5092eace10220aa687f9b`  
		Last Modified: Thu, 16 Jun 2022 01:40:06 GMT  
		Size: 332.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:848d1501cd8fc9f77a4e51a2e6dc077dcc0e468191ffaf2f433a4ffb4f7f63c1`  
		Last Modified: Thu, 16 Jun 2022 01:40:10 GMT  
		Size: 25.5 MB (25466694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98f50b8fa8c9ba100ca41212bdb8cb892fa707fb9395959c967bcc9355b3ddea`  
		Last Modified: Thu, 16 Jun 2022 01:40:06 GMT  
		Size: 317.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb8b3d4a8dbcebd64c0cd3dcde292b97e52335441dac4d3c0e8e010d1197578b`  
		Last Modified: Thu, 16 Jun 2022 01:40:15 GMT  
		Size: 48.0 MB (47957859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4284667ffa5966a13950eda5dee3eb23bc10e60d2dee427c9e7c18c789099568`  
		Last Modified: Thu, 16 Jun 2022 01:40:06 GMT  
		Size: 5.2 KB (5159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
