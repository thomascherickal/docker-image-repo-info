## `mysql:5-oracle`

```console
$ docker pull mysql@sha256:4b06f8a7ab8eed910846cff9aa0ec6cc1e6c0b9f678c62056ab6d06b0c3cc9fb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `mysql:5-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:c1300a3402d32add695f70747a29880143e6da74d5930cc24a17eb5d4a742d4c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.9 MB (126910143 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d976e8b0f43da244b5f9d79036af76fd70982d0d893d12c4644e4ed40788e391`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 19 May 2022 18:21:17 GMT
ADD file:60c2a17c0433d95caf7d6bac5520da02174f48bf0c50f6f369b00bf8f9774f82 in / 
# Thu, 19 May 2022 18:21:17 GMT
CMD ["/bin/bash"]
# Thu, 19 May 2022 18:47:44 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql; 		mkdir /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d
# Thu, 19 May 2022 18:47:44 GMT
ENV GOSU_VERSION=1.14
# Thu, 19 May 2022 18:47:47 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 19 May 2022 18:47:58 GMT
RUN set -eux; 	yum install -y 		gzip 		openssl 		xz 		zstd 	; 	yum clean all
# Thu, 19 May 2022 18:47:59 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Thu, 19 May 2022 18:47:59 GMT
ENV MYSQL_MAJOR=5.7
# Thu, 19 May 2022 18:47:59 GMT
ENV MYSQL_VERSION=5.7.38-1.el7
# Thu, 19 May 2022 18:47:59 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql5.7-server-minimal]'; 		echo 'name=MySQL 5.7 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-5.7-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Thu, 19 May 2022 18:48:13 GMT
RUN set -eux; 	yum install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	yum clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 		mysqld --version; 	mysql --version
# Thu, 19 May 2022 18:48:14 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Thu, 19 May 2022 18:48:14 GMT
ENV MYSQL_SHELL_VERSION=8.0.29-1.el7
# Thu, 19 May 2022 18:48:32 GMT
RUN set -eux; 	yum install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	yum clean all; 		mysqlsh --version
# Thu, 19 May 2022 18:48:33 GMT
VOLUME [/var/lib/mysql]
# Fri, 20 May 2022 19:40:47 GMT
COPY file:8245bb7ec0ba19a0b26df1f3a76eb35ff15083784071bf24358e434ce338e784 in /usr/local/bin/ 
# Fri, 20 May 2022 19:40:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 20 May 2022 19:40:47 GMT
EXPOSE 3306 33060
# Fri, 20 May 2022 19:40:47 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:f0182e2fe516824cf8f93b207b7c4b65d05c48db476f53312b17b5cd952bfcc3`  
		Last Modified: Thu, 19 May 2022 18:22:04 GMT  
		Size: 48.8 MB (48757934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bee5e90eb10a94a478f939d07381938536ef8d0e34f1ebf62e9ae46d9f9a1b98`  
		Last Modified: Thu, 19 May 2022 18:49:15 GMT  
		Size: 1.1 KB (1061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:918efb5a19fdff32ebbd33154bbbd84a4dbffd235322accd6ab8aa71ca2d3bbc`  
		Last Modified: Thu, 19 May 2022 18:49:13 GMT  
		Size: 930.2 KB (930229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62093a3d9873d04c95dac16a1f5351ec06126d2b0b2eee3d719a9054f192cd80`  
		Last Modified: Thu, 19 May 2022 18:49:13 GMT  
		Size: 3.8 MB (3760687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50893e22eb52afb36426bb228d1d140d9983f8f5738cd6a138af4732de54ddc0`  
		Last Modified: Thu, 19 May 2022 18:49:12 GMT  
		Size: 2.7 KB (2654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d5b859cc25c9ac85939eb1e97b5ee0adf65f53b10f4394372726142dda05cac`  
		Last Modified: Thu, 19 May 2022 18:49:10 GMT  
		Size: 335.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ea71ed17aba2bf2c4cccc50c9e2a525dd3073ef1ed8dee89553c7de243265a9`  
		Last Modified: Thu, 19 May 2022 18:49:14 GMT  
		Size: 25.5 MB (25476871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fde64eb02cf9d89a916ca0031cdef2c5f77a8437ca8726ff2445924977b24d36`  
		Last Modified: Thu, 19 May 2022 18:49:10 GMT  
		Size: 319.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6fd1907b83f9d8971dfeebcbacd4f9009fb58e15722673546f13ec17f617629`  
		Last Modified: Thu, 19 May 2022 18:49:19 GMT  
		Size: 48.0 MB (47974906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52fc05d0aca9919175c74f0e31a979ce350530c87f659b259d9b11b2b6101f10`  
		Last Modified: Fri, 20 May 2022 19:42:00 GMT  
		Size: 5.1 KB (5147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
