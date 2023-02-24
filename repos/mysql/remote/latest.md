## `mysql:latest`

```console
$ docker pull mysql@sha256:d8dc78532e9eb3759344bf89e6e7236a34132ab79150607eb08cc746989aa047
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:latest` - linux; amd64

```console
$ docker pull mysql@sha256:61c1efe1cff61a37c399d556feb489fcb81caedd871e65c018bcbdce8fe208b2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.6 MB (156589242 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f06b49211c09ddf194684fbc6c02be56773227927b1e937b489ec414a04b3f7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 24 Feb 2023 00:20:27 GMT
ADD file:9c8b13ccecebc19a9105d94b9b8060d87741d158a6de27ec96b14028de164443 in / 
# Fri, 24 Feb 2023 00:20:28 GMT
CMD ["/bin/bash"]
# Fri, 24 Feb 2023 00:36:40 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Fri, 24 Feb 2023 00:36:40 GMT
ENV GOSU_VERSION=1.16
# Fri, 24 Feb 2023 00:36:44 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 24 Feb 2023 00:37:08 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Fri, 24 Feb 2023 00:37:09 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Fri, 24 Feb 2023 00:37:09 GMT
ENV MYSQL_MAJOR=8.0
# Fri, 24 Feb 2023 00:37:09 GMT
ENV MYSQL_VERSION=8.0.32-1.el8
# Fri, 24 Feb 2023 00:37:10 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Fri, 24 Feb 2023 00:37:41 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Fri, 24 Feb 2023 00:37:42 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Fri, 24 Feb 2023 00:37:42 GMT
ENV MYSQL_SHELL_VERSION=8.0.32-1.el8
# Fri, 24 Feb 2023 00:38:17 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Fri, 24 Feb 2023 00:38:18 GMT
VOLUME [/var/lib/mysql]
# Fri, 24 Feb 2023 00:38:18 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Fri, 24 Feb 2023 00:38:18 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 24 Feb 2023 00:38:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Feb 2023 00:38:19 GMT
EXPOSE 3306 33060
# Fri, 24 Feb 2023 00:38:19 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:b4ddc423e0463a3d58b6c40ac1d97a950af62e9db703bb4c9d55afad67394149`  
		Last Modified: Fri, 24 Feb 2023 00:21:21 GMT  
		Size: 44.6 MB (44556861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b338d8e4ffd1e3235cdf4f4841d12ff13f2ccfee682aa612f3e8343e0141643b`  
		Last Modified: Fri, 24 Feb 2023 00:39:01 GMT  
		Size: 887.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2b1b06949abd179cb95c929cfe27a0aa8dd32d9e637d4ac6290709afdc06fd1`  
		Last Modified: Fri, 24 Feb 2023 00:39:02 GMT  
		Size: 982.8 KB (982820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daf393284da93334f96f25a5a63d00463c76a29f6b592d5031bff423600852a8`  
		Last Modified: Fri, 24 Feb 2023 00:39:00 GMT  
		Size: 4.6 MB (4624682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cb8337ae65dd496946fa6e84c3c790c208027898c40770628be8e6a62b88691`  
		Last Modified: Fri, 24 Feb 2023 00:38:59 GMT  
		Size: 2.6 KB (2630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6c2cc79221c2e6e69f72154874705f1ac0688c27184675d3d24542a097e341a`  
		Last Modified: Fri, 24 Feb 2023 00:38:59 GMT  
		Size: 338.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cec461351e0bb3a3059f3d1b2f8bae8515faad0837a6ff51f58640b2c242a84`  
		Last Modified: Fri, 24 Feb 2023 00:39:06 GMT  
		Size: 56.2 MB (56225153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab6bf0cba08ee281cf9ec2fbff52f9eab5914bb191f9252c6b14862d14927c55`  
		Last Modified: Fri, 24 Feb 2023 00:38:58 GMT  
		Size: 319.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8df43cafbd11a1eb8765efb82093fa3102f483935899c72ca0e9bc8288b45638`  
		Last Modified: Fri, 24 Feb 2023 00:39:07 GMT  
		Size: 50.2 MB (50190038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6d0aac53df5f1f304941701900d4de2fe96866208cee0b2c7ebbaa4c705f7d4`  
		Last Modified: Fri, 24 Feb 2023 00:38:57 GMT  
		Size: 5.4 KB (5393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b24148c7c251a7e5faad9490b84ef37663e0c8d24c507751423c51c10e50821b`  
		Last Modified: Fri, 24 Feb 2023 00:38:57 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:latest` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:dad4eee297ae4453beddfdf5921c001a26cb14be2bb1748f25e18747fcb3ba7c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.4 MB (155439967 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad405c51acf652c5191416adf3309de93f77ff0c9217d85f2f809d5f5d9a26a4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 23 Feb 2023 23:40:03 GMT
ADD file:b9db410ba951fb740a34187417442b96a27a7fd918b16023c16cb1b0777b292f in / 
# Thu, 23 Feb 2023 23:40:04 GMT
CMD ["/bin/bash"]
# Thu, 23 Feb 2023 23:56:02 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Thu, 23 Feb 2023 23:56:02 GMT
ENV GOSU_VERSION=1.16
# Thu, 23 Feb 2023 23:56:06 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Feb 2023 23:56:28 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Thu, 23 Feb 2023 23:56:29 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Thu, 23 Feb 2023 23:56:29 GMT
ENV MYSQL_MAJOR=8.0
# Thu, 23 Feb 2023 23:56:29 GMT
ENV MYSQL_VERSION=8.0.32-1.el8
# Thu, 23 Feb 2023 23:56:30 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Thu, 23 Feb 2023 23:56:55 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Thu, 23 Feb 2023 23:56:57 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Thu, 23 Feb 2023 23:56:57 GMT
ENV MYSQL_SHELL_VERSION=8.0.32-1.el8
# Thu, 23 Feb 2023 23:57:30 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Thu, 23 Feb 2023 23:57:31 GMT
VOLUME [/var/lib/mysql]
# Thu, 23 Feb 2023 23:57:31 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Thu, 23 Feb 2023 23:57:31 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 23 Feb 2023 23:57:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Feb 2023 23:57:32 GMT
EXPOSE 3306 33060
# Thu, 23 Feb 2023 23:57:32 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:fdf42ad2544e3a5379ea5e0050457e87df46409adba81dba4686a3efc595ccd2`  
		Last Modified: Thu, 23 Feb 2023 23:40:48 GMT  
		Size: 43.5 MB (43461050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:923b645414f5105d2c3a1bf6b146916472842b362b5f10bb6276a3329b18e443`  
		Last Modified: Thu, 23 Feb 2023 23:57:54 GMT  
		Size: 885.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83902a79075e521165e1deaaae38fd0ff216b20ee1badaec8507e1931eca4589`  
		Last Modified: Thu, 23 Feb 2023 23:57:54 GMT  
		Size: 913.0 KB (912996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfb14f86bde28a9538763e04f7868abf6a284d5b6c6491aa445e673b5f426772`  
		Last Modified: Thu, 23 Feb 2023 23:57:53 GMT  
		Size: 4.5 MB (4458520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec26d0e9a62d3ed49503175473e68bf7a8981d8c29557484af67dbd66cc9ef8f`  
		Last Modified: Thu, 23 Feb 2023 23:57:52 GMT  
		Size: 2.6 KB (2628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bde93ebd7c103f7655aeb5c229c0520c090531b0d93883e8e848e0ebac934f9`  
		Last Modified: Thu, 23 Feb 2023 23:57:52 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:877e8353012d100c2909f8f797f2839371b6c28902bce5410a076e1002107115`  
		Last Modified: Thu, 23 Feb 2023 23:57:56 GMT  
		Size: 55.6 MB (55614337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6a5fc068f835de1d7d6f2cb8083e162b6298a7982d44174491883cae67a0d77`  
		Last Modified: Thu, 23 Feb 2023 23:57:50 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6952f0e6afaa3499993b2e8d0744477f9d209076bd8b0538f96623c63589d472`  
		Last Modified: Thu, 23 Feb 2023 23:57:58 GMT  
		Size: 51.0 MB (50983391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e00194a8d15bb2de6954768582c366c22f5feee22a650e3713ea84a2a20f6d7`  
		Last Modified: Thu, 23 Feb 2023 23:57:51 GMT  
		Size: 5.4 KB (5389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6c604291c18fb6ce2f96e3c790a98517cb937ac104d09c251da307fc172a6a1`  
		Last Modified: Thu, 23 Feb 2023 23:57:50 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
