## `mysql:latest`

```console
$ docker pull mysql@sha256:06314a7a220f6043436cfd72fd9c7f174fd58ef69fe4b788625fa53be4ab66aa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mysql:latest` - linux; amd64

```console
$ docker pull mysql@sha256:fe2a93f68a7ddef56a39cbc8b3faaf41ca6c910978255119941c1b71899aa6c6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **157.3 MB (157264983 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8fad08b3c84be3e9164f86153224ab616bf71ee2c79677154c2e5cd3179cccfe`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 21 Oct 2022 19:20:54 GMT
ADD file:66ffe38a497f15c1941fcc4c64fda875cf27856f2ade5128546c10590c5ca84a in / 
# Fri, 21 Oct 2022 19:20:54 GMT
CMD ["/bin/bash"]
# Fri, 21 Oct 2022 19:46:11 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Fri, 21 Oct 2022 19:46:11 GMT
ENV GOSU_VERSION=1.14
# Fri, 21 Oct 2022 19:46:14 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 21 Oct 2022 19:46:37 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Fri, 21 Oct 2022 19:46:38 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Fri, 21 Oct 2022 19:46:38 GMT
ENV MYSQL_MAJOR=8.0
# Fri, 21 Oct 2022 19:46:38 GMT
ENV MYSQL_VERSION=8.0.31-1.el8
# Fri, 21 Oct 2022 19:46:39 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Fri, 21 Oct 2022 19:47:08 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Fri, 21 Oct 2022 19:47:09 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Fri, 21 Oct 2022 19:47:09 GMT
ENV MYSQL_SHELL_VERSION=8.0.31-1.el8
# Fri, 21 Oct 2022 19:47:43 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Fri, 21 Oct 2022 19:47:44 GMT
VOLUME [/var/lib/mysql]
# Fri, 21 Oct 2022 19:47:44 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Fri, 21 Oct 2022 19:47:45 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 21 Oct 2022 19:47:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 21 Oct 2022 19:47:45 GMT
EXPOSE 3306 33060
# Fri, 21 Oct 2022 19:47:45 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:50cbc88660a5576a306374b5ee70e3e8aeb602409e05ffa41cd4680769ae0574`  
		Last Modified: Fri, 21 Oct 2022 19:22:39 GMT  
		Size: 40.6 MB (40588747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92ca853f7184003ce4a998ddf789288fb6bca33039a73cbd4ba03ba525f27bb7`  
		Last Modified: Fri, 21 Oct 2022 19:49:41 GMT  
		Size: 889.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a20476962308f364c624cd515a836f813023b7bff68e93ae6aeac715b0e8f21`  
		Last Modified: Fri, 21 Oct 2022 19:49:42 GMT  
		Size: 928.8 KB (928835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe3fea56f9fb03595109612dc70a638e205294bcdda1964e39dd3851ee949fff`  
		Last Modified: Fri, 21 Oct 2022 19:49:40 GMT  
		Size: 4.6 MB (4607033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b058249d3104921cd4d5c5885643a97a8be8f9a69124fc9beed35cf791a0813f`  
		Last Modified: Fri, 21 Oct 2022 19:49:39 GMT  
		Size: 2.6 KB (2629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d5014a20163fa346756c80c1114d1ea993e9478cdfb6c08da61684a56b3e2af`  
		Last Modified: Fri, 21 Oct 2022 19:49:39 GMT  
		Size: 337.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:906aa7388ee2006b8f4362b5e9e068081be6bfc44a8f3b2bcddd6921cf7d54c7`  
		Last Modified: Fri, 21 Oct 2022 19:49:46 GMT  
		Size: 56.0 MB (56046468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86b5e2150967eeafa4e4e92254de9f529ea591d2d4b32ac6bf879b2cdb510222`  
		Last Modified: Fri, 21 Oct 2022 19:49:37 GMT  
		Size: 315.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c6b15dcdf4eda4c5061aefe4f754f90946717295e7fa5ea7dbaccff2b4f368f`  
		Last Modified: Fri, 21 Oct 2022 19:49:48 GMT  
		Size: 55.1 MB (55084220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21de4337b977fd518044876a04543776db696d6bc40559290e2dc785f3fa1cd2`  
		Last Modified: Fri, 21 Oct 2022 19:49:37 GMT  
		Size: 5.4 KB (5389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35dab154f2aeb6b8b6a8282f9df9d12aea07b392a14b82d9f9d04003f9588863`  
		Last Modified: Fri, 21 Oct 2022 19:49:37 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mysql:latest` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:5dae1c4fb603384ad5f68d3a792e5cc1095c23740785261740f00d0739e097b3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.6 MB (155562941 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d7d53e5f7cab773dc36cea9ba5009d948dbffd06acceb29c4ffed2f75f4ad51f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Fri, 21 Oct 2022 19:41:03 GMT
ADD file:2ccafa0c5b388d404f1100108ad9a9cb06c3e4ca4543c4b0f2aadfd9c4b97e45 in / 
# Fri, 21 Oct 2022 19:41:03 GMT
CMD ["/bin/bash"]
# Fri, 21 Oct 2022 20:02:14 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql
# Fri, 21 Oct 2022 20:02:15 GMT
ENV GOSU_VERSION=1.14
# Fri, 21 Oct 2022 20:02:20 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 21 Oct 2022 20:02:42 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all
# Fri, 21 Oct 2022 20:02:43 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME"
# Fri, 21 Oct 2022 20:02:44 GMT
ENV MYSQL_MAJOR=8.0
# Fri, 21 Oct 2022 20:02:45 GMT
ENV MYSQL_VERSION=8.0.31-1.el8
# Fri, 21 Oct 2022 20:02:46 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo
# Fri, 21 Oct 2022 20:03:19 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version
# Fri, 21 Oct 2022 20:03:20 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo
# Fri, 21 Oct 2022 20:03:20 GMT
ENV MYSQL_SHELL_VERSION=8.0.31-1.el8
# Fri, 21 Oct 2022 20:03:52 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version
# Fri, 21 Oct 2022 20:03:53 GMT
VOLUME [/var/lib/mysql]
# Fri, 21 Oct 2022 20:03:55 GMT
COPY file:e9c22353a1133b89c5bca24ecacd348acd094e50e5e5c45375a997c6b1f07192 in /usr/local/bin/ 
# Fri, 21 Oct 2022 20:03:56 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 21 Oct 2022 20:03:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 21 Oct 2022 20:03:57 GMT
EXPOSE 3306 33060
# Fri, 21 Oct 2022 20:03:58 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:ba2bcb842ee086f4d448ac74f4e172e2568d56d24e6efae9b402c0e37f418943`  
		Last Modified: Fri, 21 Oct 2022 19:42:50 GMT  
		Size: 39.4 MB (39408151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08f573f3d8f30de658c99546dfd56922e80e9293938b142d28198865c4c4a9ac`  
		Last Modified: Fri, 21 Oct 2022 20:04:33 GMT  
		Size: 889.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4de9dcca6a477790d74ccaf1a44e93d82058c1abfe8acc7d9949cd166f40e03`  
		Last Modified: Fri, 21 Oct 2022 20:04:34 GMT  
		Size: 857.2 KB (857152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab3d1d1f0399c6049042613a98e9c464de870d057f8589f496ad644fca5baad8`  
		Last Modified: Fri, 21 Oct 2022 20:04:32 GMT  
		Size: 4.4 MB (4433279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:283bc354d9b803601a6cfc1b2c93b8497c0eca55ca6c4180663c547784192ce9`  
		Last Modified: Fri, 21 Oct 2022 20:04:31 GMT  
		Size: 2.6 KB (2607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ef2e77bf45616b4d382065d9adcf89ae082529714fb253e1672aed550a3d166`  
		Last Modified: Fri, 21 Oct 2022 20:04:31 GMT  
		Size: 333.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8d13a94caf14e2d057950a534f5c7bb6e3ea40449ac98341a77d3de764270b6`  
		Last Modified: Fri, 21 Oct 2022 20:04:37 GMT  
		Size: 55.4 MB (55421386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45c1f1629008ad09afd71e6e8ac0337985cf8bb01382d50dfcbad35efa1789cb`  
		Last Modified: Fri, 21 Oct 2022 20:04:29 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f892d0f3ede917e6800f61a5c88869e6897dd7a85dd6664d864f9a17b5757c64`  
		Last Modified: Fri, 21 Oct 2022 20:04:39 GMT  
		Size: 55.4 MB (55433315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:346b88d5e2639641c57de86ca6641db6b00fdb7908b52bbfce8d5c2809b78039`  
		Last Modified: Fri, 21 Oct 2022 20:04:29 GMT  
		Size: 5.4 KB (5392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:998f0dbf65c702dbec59a92b1a9238a7cdc44967a4d67908b9153a401781bf11`  
		Last Modified: Fri, 21 Oct 2022 20:04:29 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
