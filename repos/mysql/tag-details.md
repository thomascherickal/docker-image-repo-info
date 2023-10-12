<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `mysql`

-	[`mysql:5`](#mysql5)
-	[`mysql:5-oracle`](#mysql5-oracle)
-	[`mysql:5.7`](#mysql57)
-	[`mysql:5.7-oracle`](#mysql57-oracle)
-	[`mysql:5.7.43`](#mysql5743)
-	[`mysql:5.7.43-oracle`](#mysql5743-oracle)
-	[`mysql:8`](#mysql8)
-	[`mysql:8-oracle`](#mysql8-oracle)
-	[`mysql:8.0`](#mysql80)
-	[`mysql:8.0-debian`](#mysql80-debian)
-	[`mysql:8.0-oracle`](#mysql80-oracle)
-	[`mysql:8.0.34`](#mysql8034)
-	[`mysql:8.0.34-debian`](#mysql8034-debian)
-	[`mysql:8.0.34-oracle`](#mysql8034-oracle)
-	[`mysql:8.1`](#mysql81)
-	[`mysql:8.1-oracle`](#mysql81-oracle)
-	[`mysql:8.1.0`](#mysql810)
-	[`mysql:8.1.0-oracle`](#mysql810-oracle)
-	[`mysql:innovation`](#mysqlinnovation)
-	[`mysql:innovation-oracle`](#mysqlinnovation-oracle)
-	[`mysql:latest`](#mysqllatest)
-	[`mysql:oracle`](#mysqloracle)

## `mysql:5`

```console
$ docker pull mysql@sha256:a06310bb26d02a6118ae7fa825c172a0bf594e178c72230fc31674f348033270
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 2
	-	linux; amd64
	-	unknown; unknown

### `mysql:5` - linux; amd64

```console
$ docker pull mysql@sha256:e857469c4d22da38abe1f1b60a0e0bf7b0a5812f6bea1e247e375aa1701db925
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.2 MB (170195017 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5b7ceed4074932a04ea553af3124bb03b249affe14899e2cd746d1a63e12ecc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 14 Jun 2023 07:21:40 GMT
ADD file:733a37449d62d6e9f530185b9244e06cd8ff0ee896632576ae644437d0a1f852 in / 
# Wed, 14 Jun 2023 07:21:40 GMT
CMD ["/bin/bash"]
# Thu, 27 Jul 2023 22:18:54 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql # buildkit
# Thu, 27 Jul 2023 22:18:54 GMT
ENV GOSU_VERSION=1.16
# Thu, 27 Jul 2023 22:18:54 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Thu, 27 Jul 2023 22:18:54 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False oracle-epel-release-el7; 	yum install -y --setopt=skip_missing_names_on_install=False 		bzip2 		gzip 		openssl 		xz 		zstd 	; 	yum clean all # buildkit
# Thu, 27 Jul 2023 22:18:54 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME" # buildkit
# Thu, 27 Jul 2023 22:18:54 GMT
ENV MYSQL_MAJOR=5.7
# Thu, 27 Jul 2023 22:18:54 GMT
ENV MYSQL_VERSION=5.7.43-1.el7
# Thu, 27 Jul 2023 22:18:54 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql5.7-server-minimal]'; 		echo 'name=MySQL 5.7 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-5.7-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo # buildkit
# Thu, 27 Jul 2023 22:18:54 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-community-server-minimal-$MYSQL_VERSION"; 	yum clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	{ echo '!includedir /etc/mysql/mysql.conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/mysql.conf.d; 		find /etc/my.cnf /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/'; 		mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version # buildkit
# Thu, 27 Jul 2023 22:18:54 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo # buildkit
# Thu, 27 Jul 2023 22:18:54 GMT
ENV MYSQL_SHELL_VERSION=8.0.34-1.el7
# Thu, 27 Jul 2023 22:18:54 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-shell-$MYSQL_SHELL_VERSION"; 	yum clean all; 		mysqlsh --version # buildkit
# Thu, 27 Jul 2023 22:18:54 GMT
VOLUME [/var/lib/mysql]
# Thu, 27 Jul 2023 22:18:54 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 27 Jul 2023 22:18:54 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Thu, 27 Jul 2023 22:18:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 27 Jul 2023 22:18:54 GMT
EXPOSE map[3306/tcp:{} 33060/tcp:{}]
# Thu, 27 Jul 2023 22:18:54 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:70e9ff4420fbc58483e68c13199a06c24b14013b2548998a7e367f59ca5157bc`  
		Last Modified: Wed, 14 Jun 2023 07:22:30 GMT  
		Size: 50.5 MB (50484765 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:dc7fe6a7bf6360f616c9d90938e6370f30e346f78e5c861453b298ef679c2e6d`  
		Last Modified: Wed, 04 Oct 2023 22:59:56 GMT  
		Size: 870.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6c47791d5b2f2042d85f90d1b9ac09db0b1cd2aa51bf8a87be26af81f2e8b638`  
		Last Modified: Wed, 04 Oct 2023 22:59:56 GMT  
		Size: 983.6 KB (983557 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8aa08ad32885279e23f7369e78fe3c38dfac42110e56bf2a9b4bea2fe0bd81f0`  
		Last Modified: Wed, 04 Oct 2023 22:59:57 GMT  
		Size: 4.6 MB (4591549 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a74a35dfed64215cd12c2139cbc725717afaf002570e093deddfaaf78812cb92`  
		Last Modified: Wed, 04 Oct 2023 22:59:57 GMT  
		Size: 3.1 KB (3077 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:03a960f04fcecc8e8e28a23672e240468cbe5ce234dd740cd9e02beb0e652b45`  
		Last Modified: Wed, 04 Oct 2023 22:59:57 GMT  
		Size: 331.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:966afd0d388e93a8c5697781fb903de54f037f6b5a9e750631eedc3543cab86b`  
		Last Modified: Wed, 04 Oct 2023 23:00:00 GMT  
		Size: 25.5 MB (25532723 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d7b1625fdc9dd77266a8757af28b6ac427d1cd70b68133849ce1796670fc04a6`  
		Last Modified: Wed, 04 Oct 2023 22:59:58 GMT  
		Size: 317.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3428031e976c74095cb2ec2f383513266c921ed65200791ac495aa46e6513086`  
		Last Modified: Wed, 04 Oct 2023 23:00:03 GMT  
		Size: 88.6 MB (88592316 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:232612f35735a37afa48607ee6f57662675a3401595bbcfd99d3dd8efec502f8`  
		Last Modified: Wed, 04 Oct 2023 22:59:59 GMT  
		Size: 5.4 KB (5390 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:da583abbf6d06462fbfae531ee0cef96525e1b17baf36c9c217cb652c63a5f71`  
		Last Modified: Wed, 04 Oct 2023 23:00:00 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:5` - unknown; unknown

```console
$ docker pull mysql@sha256:08ece30b6fe1a922f173bd9bd28adaa01d77d070cf1293d9653668ef2e84e9f5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.5 MB (14459430 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19cf498d4a12fec4569f57d4f93dc34304e307b8748211a3b4dbac08c6d0760d`

```dockerfile
```

-	Layers:
	-	`sha256:4010fb6f8cd55b2d9050987eb8cb50842e8a63876073d6f558e059aaf51f6a28`  
		Last Modified: Wed, 04 Oct 2023 22:59:57 GMT  
		Size: 14.4 MB (14422978 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:9861c670f5c58916f944bffb660bde5d1803c908bc60e07d263d2937b13ab2f6`  
		Last Modified: Wed, 04 Oct 2023 22:59:56 GMT  
		Size: 36.5 KB (36452 bytes)  
		MIME: application/vnd.in-toto+json

## `mysql:5-oracle`

```console
$ docker pull mysql@sha256:a06310bb26d02a6118ae7fa825c172a0bf594e178c72230fc31674f348033270
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 2
	-	linux; amd64
	-	unknown; unknown

### `mysql:5-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:e857469c4d22da38abe1f1b60a0e0bf7b0a5812f6bea1e247e375aa1701db925
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.2 MB (170195017 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5b7ceed4074932a04ea553af3124bb03b249affe14899e2cd746d1a63e12ecc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 14 Jun 2023 07:21:40 GMT
ADD file:733a37449d62d6e9f530185b9244e06cd8ff0ee896632576ae644437d0a1f852 in / 
# Wed, 14 Jun 2023 07:21:40 GMT
CMD ["/bin/bash"]
# Thu, 27 Jul 2023 22:18:54 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql # buildkit
# Thu, 27 Jul 2023 22:18:54 GMT
ENV GOSU_VERSION=1.16
# Thu, 27 Jul 2023 22:18:54 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Thu, 27 Jul 2023 22:18:54 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False oracle-epel-release-el7; 	yum install -y --setopt=skip_missing_names_on_install=False 		bzip2 		gzip 		openssl 		xz 		zstd 	; 	yum clean all # buildkit
# Thu, 27 Jul 2023 22:18:54 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME" # buildkit
# Thu, 27 Jul 2023 22:18:54 GMT
ENV MYSQL_MAJOR=5.7
# Thu, 27 Jul 2023 22:18:54 GMT
ENV MYSQL_VERSION=5.7.43-1.el7
# Thu, 27 Jul 2023 22:18:54 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql5.7-server-minimal]'; 		echo 'name=MySQL 5.7 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-5.7-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo # buildkit
# Thu, 27 Jul 2023 22:18:54 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-community-server-minimal-$MYSQL_VERSION"; 	yum clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	{ echo '!includedir /etc/mysql/mysql.conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/mysql.conf.d; 		find /etc/my.cnf /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/'; 		mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version # buildkit
# Thu, 27 Jul 2023 22:18:54 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo # buildkit
# Thu, 27 Jul 2023 22:18:54 GMT
ENV MYSQL_SHELL_VERSION=8.0.34-1.el7
# Thu, 27 Jul 2023 22:18:54 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-shell-$MYSQL_SHELL_VERSION"; 	yum clean all; 		mysqlsh --version # buildkit
# Thu, 27 Jul 2023 22:18:54 GMT
VOLUME [/var/lib/mysql]
# Thu, 27 Jul 2023 22:18:54 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 27 Jul 2023 22:18:54 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Thu, 27 Jul 2023 22:18:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 27 Jul 2023 22:18:54 GMT
EXPOSE map[3306/tcp:{} 33060/tcp:{}]
# Thu, 27 Jul 2023 22:18:54 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:70e9ff4420fbc58483e68c13199a06c24b14013b2548998a7e367f59ca5157bc`  
		Last Modified: Wed, 14 Jun 2023 07:22:30 GMT  
		Size: 50.5 MB (50484765 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:dc7fe6a7bf6360f616c9d90938e6370f30e346f78e5c861453b298ef679c2e6d`  
		Last Modified: Wed, 04 Oct 2023 22:59:56 GMT  
		Size: 870.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6c47791d5b2f2042d85f90d1b9ac09db0b1cd2aa51bf8a87be26af81f2e8b638`  
		Last Modified: Wed, 04 Oct 2023 22:59:56 GMT  
		Size: 983.6 KB (983557 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8aa08ad32885279e23f7369e78fe3c38dfac42110e56bf2a9b4bea2fe0bd81f0`  
		Last Modified: Wed, 04 Oct 2023 22:59:57 GMT  
		Size: 4.6 MB (4591549 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a74a35dfed64215cd12c2139cbc725717afaf002570e093deddfaaf78812cb92`  
		Last Modified: Wed, 04 Oct 2023 22:59:57 GMT  
		Size: 3.1 KB (3077 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:03a960f04fcecc8e8e28a23672e240468cbe5ce234dd740cd9e02beb0e652b45`  
		Last Modified: Wed, 04 Oct 2023 22:59:57 GMT  
		Size: 331.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:966afd0d388e93a8c5697781fb903de54f037f6b5a9e750631eedc3543cab86b`  
		Last Modified: Wed, 04 Oct 2023 23:00:00 GMT  
		Size: 25.5 MB (25532723 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d7b1625fdc9dd77266a8757af28b6ac427d1cd70b68133849ce1796670fc04a6`  
		Last Modified: Wed, 04 Oct 2023 22:59:58 GMT  
		Size: 317.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3428031e976c74095cb2ec2f383513266c921ed65200791ac495aa46e6513086`  
		Last Modified: Wed, 04 Oct 2023 23:00:03 GMT  
		Size: 88.6 MB (88592316 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:232612f35735a37afa48607ee6f57662675a3401595bbcfd99d3dd8efec502f8`  
		Last Modified: Wed, 04 Oct 2023 22:59:59 GMT  
		Size: 5.4 KB (5390 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:da583abbf6d06462fbfae531ee0cef96525e1b17baf36c9c217cb652c63a5f71`  
		Last Modified: Wed, 04 Oct 2023 23:00:00 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:5-oracle` - unknown; unknown

```console
$ docker pull mysql@sha256:08ece30b6fe1a922f173bd9bd28adaa01d77d070cf1293d9653668ef2e84e9f5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.5 MB (14459430 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19cf498d4a12fec4569f57d4f93dc34304e307b8748211a3b4dbac08c6d0760d`

```dockerfile
```

-	Layers:
	-	`sha256:4010fb6f8cd55b2d9050987eb8cb50842e8a63876073d6f558e059aaf51f6a28`  
		Last Modified: Wed, 04 Oct 2023 22:59:57 GMT  
		Size: 14.4 MB (14422978 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:9861c670f5c58916f944bffb660bde5d1803c908bc60e07d263d2937b13ab2f6`  
		Last Modified: Wed, 04 Oct 2023 22:59:56 GMT  
		Size: 36.5 KB (36452 bytes)  
		MIME: application/vnd.in-toto+json

## `mysql:5.7`

```console
$ docker pull mysql@sha256:a06310bb26d02a6118ae7fa825c172a0bf594e178c72230fc31674f348033270
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 2
	-	linux; amd64
	-	unknown; unknown

### `mysql:5.7` - linux; amd64

```console
$ docker pull mysql@sha256:e857469c4d22da38abe1f1b60a0e0bf7b0a5812f6bea1e247e375aa1701db925
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.2 MB (170195017 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5b7ceed4074932a04ea553af3124bb03b249affe14899e2cd746d1a63e12ecc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 14 Jun 2023 07:21:40 GMT
ADD file:733a37449d62d6e9f530185b9244e06cd8ff0ee896632576ae644437d0a1f852 in / 
# Wed, 14 Jun 2023 07:21:40 GMT
CMD ["/bin/bash"]
# Thu, 27 Jul 2023 22:18:54 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql # buildkit
# Thu, 27 Jul 2023 22:18:54 GMT
ENV GOSU_VERSION=1.16
# Thu, 27 Jul 2023 22:18:54 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Thu, 27 Jul 2023 22:18:54 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False oracle-epel-release-el7; 	yum install -y --setopt=skip_missing_names_on_install=False 		bzip2 		gzip 		openssl 		xz 		zstd 	; 	yum clean all # buildkit
# Thu, 27 Jul 2023 22:18:54 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME" # buildkit
# Thu, 27 Jul 2023 22:18:54 GMT
ENV MYSQL_MAJOR=5.7
# Thu, 27 Jul 2023 22:18:54 GMT
ENV MYSQL_VERSION=5.7.43-1.el7
# Thu, 27 Jul 2023 22:18:54 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql5.7-server-minimal]'; 		echo 'name=MySQL 5.7 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-5.7-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo # buildkit
# Thu, 27 Jul 2023 22:18:54 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-community-server-minimal-$MYSQL_VERSION"; 	yum clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	{ echo '!includedir /etc/mysql/mysql.conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/mysql.conf.d; 		find /etc/my.cnf /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/'; 		mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version # buildkit
# Thu, 27 Jul 2023 22:18:54 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo # buildkit
# Thu, 27 Jul 2023 22:18:54 GMT
ENV MYSQL_SHELL_VERSION=8.0.34-1.el7
# Thu, 27 Jul 2023 22:18:54 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-shell-$MYSQL_SHELL_VERSION"; 	yum clean all; 		mysqlsh --version # buildkit
# Thu, 27 Jul 2023 22:18:54 GMT
VOLUME [/var/lib/mysql]
# Thu, 27 Jul 2023 22:18:54 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 27 Jul 2023 22:18:54 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Thu, 27 Jul 2023 22:18:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 27 Jul 2023 22:18:54 GMT
EXPOSE map[3306/tcp:{} 33060/tcp:{}]
# Thu, 27 Jul 2023 22:18:54 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:70e9ff4420fbc58483e68c13199a06c24b14013b2548998a7e367f59ca5157bc`  
		Last Modified: Wed, 14 Jun 2023 07:22:30 GMT  
		Size: 50.5 MB (50484765 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:dc7fe6a7bf6360f616c9d90938e6370f30e346f78e5c861453b298ef679c2e6d`  
		Last Modified: Wed, 04 Oct 2023 22:59:56 GMT  
		Size: 870.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6c47791d5b2f2042d85f90d1b9ac09db0b1cd2aa51bf8a87be26af81f2e8b638`  
		Last Modified: Wed, 04 Oct 2023 22:59:56 GMT  
		Size: 983.6 KB (983557 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8aa08ad32885279e23f7369e78fe3c38dfac42110e56bf2a9b4bea2fe0bd81f0`  
		Last Modified: Wed, 04 Oct 2023 22:59:57 GMT  
		Size: 4.6 MB (4591549 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a74a35dfed64215cd12c2139cbc725717afaf002570e093deddfaaf78812cb92`  
		Last Modified: Wed, 04 Oct 2023 22:59:57 GMT  
		Size: 3.1 KB (3077 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:03a960f04fcecc8e8e28a23672e240468cbe5ce234dd740cd9e02beb0e652b45`  
		Last Modified: Wed, 04 Oct 2023 22:59:57 GMT  
		Size: 331.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:966afd0d388e93a8c5697781fb903de54f037f6b5a9e750631eedc3543cab86b`  
		Last Modified: Wed, 04 Oct 2023 23:00:00 GMT  
		Size: 25.5 MB (25532723 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d7b1625fdc9dd77266a8757af28b6ac427d1cd70b68133849ce1796670fc04a6`  
		Last Modified: Wed, 04 Oct 2023 22:59:58 GMT  
		Size: 317.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3428031e976c74095cb2ec2f383513266c921ed65200791ac495aa46e6513086`  
		Last Modified: Wed, 04 Oct 2023 23:00:03 GMT  
		Size: 88.6 MB (88592316 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:232612f35735a37afa48607ee6f57662675a3401595bbcfd99d3dd8efec502f8`  
		Last Modified: Wed, 04 Oct 2023 22:59:59 GMT  
		Size: 5.4 KB (5390 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:da583abbf6d06462fbfae531ee0cef96525e1b17baf36c9c217cb652c63a5f71`  
		Last Modified: Wed, 04 Oct 2023 23:00:00 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:5.7` - unknown; unknown

```console
$ docker pull mysql@sha256:08ece30b6fe1a922f173bd9bd28adaa01d77d070cf1293d9653668ef2e84e9f5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.5 MB (14459430 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19cf498d4a12fec4569f57d4f93dc34304e307b8748211a3b4dbac08c6d0760d`

```dockerfile
```

-	Layers:
	-	`sha256:4010fb6f8cd55b2d9050987eb8cb50842e8a63876073d6f558e059aaf51f6a28`  
		Last Modified: Wed, 04 Oct 2023 22:59:57 GMT  
		Size: 14.4 MB (14422978 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:9861c670f5c58916f944bffb660bde5d1803c908bc60e07d263d2937b13ab2f6`  
		Last Modified: Wed, 04 Oct 2023 22:59:56 GMT  
		Size: 36.5 KB (36452 bytes)  
		MIME: application/vnd.in-toto+json

## `mysql:5.7-oracle`

```console
$ docker pull mysql@sha256:a06310bb26d02a6118ae7fa825c172a0bf594e178c72230fc31674f348033270
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 2
	-	linux; amd64
	-	unknown; unknown

### `mysql:5.7-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:e857469c4d22da38abe1f1b60a0e0bf7b0a5812f6bea1e247e375aa1701db925
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.2 MB (170195017 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5b7ceed4074932a04ea553af3124bb03b249affe14899e2cd746d1a63e12ecc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 14 Jun 2023 07:21:40 GMT
ADD file:733a37449d62d6e9f530185b9244e06cd8ff0ee896632576ae644437d0a1f852 in / 
# Wed, 14 Jun 2023 07:21:40 GMT
CMD ["/bin/bash"]
# Thu, 27 Jul 2023 22:18:54 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql # buildkit
# Thu, 27 Jul 2023 22:18:54 GMT
ENV GOSU_VERSION=1.16
# Thu, 27 Jul 2023 22:18:54 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Thu, 27 Jul 2023 22:18:54 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False oracle-epel-release-el7; 	yum install -y --setopt=skip_missing_names_on_install=False 		bzip2 		gzip 		openssl 		xz 		zstd 	; 	yum clean all # buildkit
# Thu, 27 Jul 2023 22:18:54 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME" # buildkit
# Thu, 27 Jul 2023 22:18:54 GMT
ENV MYSQL_MAJOR=5.7
# Thu, 27 Jul 2023 22:18:54 GMT
ENV MYSQL_VERSION=5.7.43-1.el7
# Thu, 27 Jul 2023 22:18:54 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql5.7-server-minimal]'; 		echo 'name=MySQL 5.7 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-5.7-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo # buildkit
# Thu, 27 Jul 2023 22:18:54 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-community-server-minimal-$MYSQL_VERSION"; 	yum clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	{ echo '!includedir /etc/mysql/mysql.conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/mysql.conf.d; 		find /etc/my.cnf /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/'; 		mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version # buildkit
# Thu, 27 Jul 2023 22:18:54 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo # buildkit
# Thu, 27 Jul 2023 22:18:54 GMT
ENV MYSQL_SHELL_VERSION=8.0.34-1.el7
# Thu, 27 Jul 2023 22:18:54 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-shell-$MYSQL_SHELL_VERSION"; 	yum clean all; 		mysqlsh --version # buildkit
# Thu, 27 Jul 2023 22:18:54 GMT
VOLUME [/var/lib/mysql]
# Thu, 27 Jul 2023 22:18:54 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 27 Jul 2023 22:18:54 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Thu, 27 Jul 2023 22:18:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 27 Jul 2023 22:18:54 GMT
EXPOSE map[3306/tcp:{} 33060/tcp:{}]
# Thu, 27 Jul 2023 22:18:54 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:70e9ff4420fbc58483e68c13199a06c24b14013b2548998a7e367f59ca5157bc`  
		Last Modified: Wed, 14 Jun 2023 07:22:30 GMT  
		Size: 50.5 MB (50484765 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:dc7fe6a7bf6360f616c9d90938e6370f30e346f78e5c861453b298ef679c2e6d`  
		Last Modified: Wed, 04 Oct 2023 22:59:56 GMT  
		Size: 870.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6c47791d5b2f2042d85f90d1b9ac09db0b1cd2aa51bf8a87be26af81f2e8b638`  
		Last Modified: Wed, 04 Oct 2023 22:59:56 GMT  
		Size: 983.6 KB (983557 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8aa08ad32885279e23f7369e78fe3c38dfac42110e56bf2a9b4bea2fe0bd81f0`  
		Last Modified: Wed, 04 Oct 2023 22:59:57 GMT  
		Size: 4.6 MB (4591549 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a74a35dfed64215cd12c2139cbc725717afaf002570e093deddfaaf78812cb92`  
		Last Modified: Wed, 04 Oct 2023 22:59:57 GMT  
		Size: 3.1 KB (3077 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:03a960f04fcecc8e8e28a23672e240468cbe5ce234dd740cd9e02beb0e652b45`  
		Last Modified: Wed, 04 Oct 2023 22:59:57 GMT  
		Size: 331.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:966afd0d388e93a8c5697781fb903de54f037f6b5a9e750631eedc3543cab86b`  
		Last Modified: Wed, 04 Oct 2023 23:00:00 GMT  
		Size: 25.5 MB (25532723 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d7b1625fdc9dd77266a8757af28b6ac427d1cd70b68133849ce1796670fc04a6`  
		Last Modified: Wed, 04 Oct 2023 22:59:58 GMT  
		Size: 317.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3428031e976c74095cb2ec2f383513266c921ed65200791ac495aa46e6513086`  
		Last Modified: Wed, 04 Oct 2023 23:00:03 GMT  
		Size: 88.6 MB (88592316 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:232612f35735a37afa48607ee6f57662675a3401595bbcfd99d3dd8efec502f8`  
		Last Modified: Wed, 04 Oct 2023 22:59:59 GMT  
		Size: 5.4 KB (5390 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:da583abbf6d06462fbfae531ee0cef96525e1b17baf36c9c217cb652c63a5f71`  
		Last Modified: Wed, 04 Oct 2023 23:00:00 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:5.7-oracle` - unknown; unknown

```console
$ docker pull mysql@sha256:08ece30b6fe1a922f173bd9bd28adaa01d77d070cf1293d9653668ef2e84e9f5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.5 MB (14459430 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19cf498d4a12fec4569f57d4f93dc34304e307b8748211a3b4dbac08c6d0760d`

```dockerfile
```

-	Layers:
	-	`sha256:4010fb6f8cd55b2d9050987eb8cb50842e8a63876073d6f558e059aaf51f6a28`  
		Last Modified: Wed, 04 Oct 2023 22:59:57 GMT  
		Size: 14.4 MB (14422978 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:9861c670f5c58916f944bffb660bde5d1803c908bc60e07d263d2937b13ab2f6`  
		Last Modified: Wed, 04 Oct 2023 22:59:56 GMT  
		Size: 36.5 KB (36452 bytes)  
		MIME: application/vnd.in-toto+json

## `mysql:5.7.43`

```console
$ docker pull mysql@sha256:a06310bb26d02a6118ae7fa825c172a0bf594e178c72230fc31674f348033270
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 2
	-	linux; amd64
	-	unknown; unknown

### `mysql:5.7.43` - linux; amd64

```console
$ docker pull mysql@sha256:e857469c4d22da38abe1f1b60a0e0bf7b0a5812f6bea1e247e375aa1701db925
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.2 MB (170195017 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5b7ceed4074932a04ea553af3124bb03b249affe14899e2cd746d1a63e12ecc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 14 Jun 2023 07:21:40 GMT
ADD file:733a37449d62d6e9f530185b9244e06cd8ff0ee896632576ae644437d0a1f852 in / 
# Wed, 14 Jun 2023 07:21:40 GMT
CMD ["/bin/bash"]
# Thu, 27 Jul 2023 22:18:54 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql # buildkit
# Thu, 27 Jul 2023 22:18:54 GMT
ENV GOSU_VERSION=1.16
# Thu, 27 Jul 2023 22:18:54 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Thu, 27 Jul 2023 22:18:54 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False oracle-epel-release-el7; 	yum install -y --setopt=skip_missing_names_on_install=False 		bzip2 		gzip 		openssl 		xz 		zstd 	; 	yum clean all # buildkit
# Thu, 27 Jul 2023 22:18:54 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME" # buildkit
# Thu, 27 Jul 2023 22:18:54 GMT
ENV MYSQL_MAJOR=5.7
# Thu, 27 Jul 2023 22:18:54 GMT
ENV MYSQL_VERSION=5.7.43-1.el7
# Thu, 27 Jul 2023 22:18:54 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql5.7-server-minimal]'; 		echo 'name=MySQL 5.7 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-5.7-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo # buildkit
# Thu, 27 Jul 2023 22:18:54 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-community-server-minimal-$MYSQL_VERSION"; 	yum clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	{ echo '!includedir /etc/mysql/mysql.conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/mysql.conf.d; 		find /etc/my.cnf /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/'; 		mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version # buildkit
# Thu, 27 Jul 2023 22:18:54 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo # buildkit
# Thu, 27 Jul 2023 22:18:54 GMT
ENV MYSQL_SHELL_VERSION=8.0.34-1.el7
# Thu, 27 Jul 2023 22:18:54 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-shell-$MYSQL_SHELL_VERSION"; 	yum clean all; 		mysqlsh --version # buildkit
# Thu, 27 Jul 2023 22:18:54 GMT
VOLUME [/var/lib/mysql]
# Thu, 27 Jul 2023 22:18:54 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 27 Jul 2023 22:18:54 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Thu, 27 Jul 2023 22:18:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 27 Jul 2023 22:18:54 GMT
EXPOSE map[3306/tcp:{} 33060/tcp:{}]
# Thu, 27 Jul 2023 22:18:54 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:70e9ff4420fbc58483e68c13199a06c24b14013b2548998a7e367f59ca5157bc`  
		Last Modified: Wed, 14 Jun 2023 07:22:30 GMT  
		Size: 50.5 MB (50484765 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:dc7fe6a7bf6360f616c9d90938e6370f30e346f78e5c861453b298ef679c2e6d`  
		Last Modified: Wed, 04 Oct 2023 22:59:56 GMT  
		Size: 870.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6c47791d5b2f2042d85f90d1b9ac09db0b1cd2aa51bf8a87be26af81f2e8b638`  
		Last Modified: Wed, 04 Oct 2023 22:59:56 GMT  
		Size: 983.6 KB (983557 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8aa08ad32885279e23f7369e78fe3c38dfac42110e56bf2a9b4bea2fe0bd81f0`  
		Last Modified: Wed, 04 Oct 2023 22:59:57 GMT  
		Size: 4.6 MB (4591549 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a74a35dfed64215cd12c2139cbc725717afaf002570e093deddfaaf78812cb92`  
		Last Modified: Wed, 04 Oct 2023 22:59:57 GMT  
		Size: 3.1 KB (3077 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:03a960f04fcecc8e8e28a23672e240468cbe5ce234dd740cd9e02beb0e652b45`  
		Last Modified: Wed, 04 Oct 2023 22:59:57 GMT  
		Size: 331.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:966afd0d388e93a8c5697781fb903de54f037f6b5a9e750631eedc3543cab86b`  
		Last Modified: Wed, 04 Oct 2023 23:00:00 GMT  
		Size: 25.5 MB (25532723 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d7b1625fdc9dd77266a8757af28b6ac427d1cd70b68133849ce1796670fc04a6`  
		Last Modified: Wed, 04 Oct 2023 22:59:58 GMT  
		Size: 317.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3428031e976c74095cb2ec2f383513266c921ed65200791ac495aa46e6513086`  
		Last Modified: Wed, 04 Oct 2023 23:00:03 GMT  
		Size: 88.6 MB (88592316 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:232612f35735a37afa48607ee6f57662675a3401595bbcfd99d3dd8efec502f8`  
		Last Modified: Wed, 04 Oct 2023 22:59:59 GMT  
		Size: 5.4 KB (5390 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:da583abbf6d06462fbfae531ee0cef96525e1b17baf36c9c217cb652c63a5f71`  
		Last Modified: Wed, 04 Oct 2023 23:00:00 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:5.7.43` - unknown; unknown

```console
$ docker pull mysql@sha256:08ece30b6fe1a922f173bd9bd28adaa01d77d070cf1293d9653668ef2e84e9f5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.5 MB (14459430 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19cf498d4a12fec4569f57d4f93dc34304e307b8748211a3b4dbac08c6d0760d`

```dockerfile
```

-	Layers:
	-	`sha256:4010fb6f8cd55b2d9050987eb8cb50842e8a63876073d6f558e059aaf51f6a28`  
		Last Modified: Wed, 04 Oct 2023 22:59:57 GMT  
		Size: 14.4 MB (14422978 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:9861c670f5c58916f944bffb660bde5d1803c908bc60e07d263d2937b13ab2f6`  
		Last Modified: Wed, 04 Oct 2023 22:59:56 GMT  
		Size: 36.5 KB (36452 bytes)  
		MIME: application/vnd.in-toto+json

## `mysql:5.7.43-oracle`

```console
$ docker pull mysql@sha256:a06310bb26d02a6118ae7fa825c172a0bf594e178c72230fc31674f348033270
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 2
	-	linux; amd64
	-	unknown; unknown

### `mysql:5.7.43-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:e857469c4d22da38abe1f1b60a0e0bf7b0a5812f6bea1e247e375aa1701db925
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.2 MB (170195017 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5b7ceed4074932a04ea553af3124bb03b249affe14899e2cd746d1a63e12ecc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Wed, 14 Jun 2023 07:21:40 GMT
ADD file:733a37449d62d6e9f530185b9244e06cd8ff0ee896632576ae644437d0a1f852 in / 
# Wed, 14 Jun 2023 07:21:40 GMT
CMD ["/bin/bash"]
# Thu, 27 Jul 2023 22:18:54 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql # buildkit
# Thu, 27 Jul 2023 22:18:54 GMT
ENV GOSU_VERSION=1.16
# Thu, 27 Jul 2023 22:18:54 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Thu, 27 Jul 2023 22:18:54 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False oracle-epel-release-el7; 	yum install -y --setopt=skip_missing_names_on_install=False 		bzip2 		gzip 		openssl 		xz 		zstd 	; 	yum clean all # buildkit
# Thu, 27 Jul 2023 22:18:54 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME" # buildkit
# Thu, 27 Jul 2023 22:18:54 GMT
ENV MYSQL_MAJOR=5.7
# Thu, 27 Jul 2023 22:18:54 GMT
ENV MYSQL_VERSION=5.7.43-1.el7
# Thu, 27 Jul 2023 22:18:54 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql5.7-server-minimal]'; 		echo 'name=MySQL 5.7 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-5.7-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo # buildkit
# Thu, 27 Jul 2023 22:18:54 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-community-server-minimal-$MYSQL_VERSION"; 	yum clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	{ echo '!includedir /etc/mysql/mysql.conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/mysql.conf.d; 		find /etc/my.cnf /etc/mysql/ -name '*.cnf' -print0 		| xargs -0 grep -lZE '^(bind-address|log)' 		| xargs -rt -0 sed -Ei 's/^(bind-address|log)/#&/'; 		mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version # buildkit
# Thu, 27 Jul 2023 22:18:54 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo # buildkit
# Thu, 27 Jul 2023 22:18:54 GMT
ENV MYSQL_SHELL_VERSION=8.0.34-1.el7
# Thu, 27 Jul 2023 22:18:54 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False "mysql-shell-$MYSQL_SHELL_VERSION"; 	yum clean all; 		mysqlsh --version # buildkit
# Thu, 27 Jul 2023 22:18:54 GMT
VOLUME [/var/lib/mysql]
# Thu, 27 Jul 2023 22:18:54 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 27 Jul 2023 22:18:54 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Thu, 27 Jul 2023 22:18:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 27 Jul 2023 22:18:54 GMT
EXPOSE map[3306/tcp:{} 33060/tcp:{}]
# Thu, 27 Jul 2023 22:18:54 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:70e9ff4420fbc58483e68c13199a06c24b14013b2548998a7e367f59ca5157bc`  
		Last Modified: Wed, 14 Jun 2023 07:22:30 GMT  
		Size: 50.5 MB (50484765 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:dc7fe6a7bf6360f616c9d90938e6370f30e346f78e5c861453b298ef679c2e6d`  
		Last Modified: Wed, 04 Oct 2023 22:59:56 GMT  
		Size: 870.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6c47791d5b2f2042d85f90d1b9ac09db0b1cd2aa51bf8a87be26af81f2e8b638`  
		Last Modified: Wed, 04 Oct 2023 22:59:56 GMT  
		Size: 983.6 KB (983557 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8aa08ad32885279e23f7369e78fe3c38dfac42110e56bf2a9b4bea2fe0bd81f0`  
		Last Modified: Wed, 04 Oct 2023 22:59:57 GMT  
		Size: 4.6 MB (4591549 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a74a35dfed64215cd12c2139cbc725717afaf002570e093deddfaaf78812cb92`  
		Last Modified: Wed, 04 Oct 2023 22:59:57 GMT  
		Size: 3.1 KB (3077 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:03a960f04fcecc8e8e28a23672e240468cbe5ce234dd740cd9e02beb0e652b45`  
		Last Modified: Wed, 04 Oct 2023 22:59:57 GMT  
		Size: 331.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:966afd0d388e93a8c5697781fb903de54f037f6b5a9e750631eedc3543cab86b`  
		Last Modified: Wed, 04 Oct 2023 23:00:00 GMT  
		Size: 25.5 MB (25532723 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d7b1625fdc9dd77266a8757af28b6ac427d1cd70b68133849ce1796670fc04a6`  
		Last Modified: Wed, 04 Oct 2023 22:59:58 GMT  
		Size: 317.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3428031e976c74095cb2ec2f383513266c921ed65200791ac495aa46e6513086`  
		Last Modified: Wed, 04 Oct 2023 23:00:03 GMT  
		Size: 88.6 MB (88592316 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:232612f35735a37afa48607ee6f57662675a3401595bbcfd99d3dd8efec502f8`  
		Last Modified: Wed, 04 Oct 2023 22:59:59 GMT  
		Size: 5.4 KB (5390 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:da583abbf6d06462fbfae531ee0cef96525e1b17baf36c9c217cb652c63a5f71`  
		Last Modified: Wed, 04 Oct 2023 23:00:00 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:5.7.43-oracle` - unknown; unknown

```console
$ docker pull mysql@sha256:08ece30b6fe1a922f173bd9bd28adaa01d77d070cf1293d9653668ef2e84e9f5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.5 MB (14459430 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19cf498d4a12fec4569f57d4f93dc34304e307b8748211a3b4dbac08c6d0760d`

```dockerfile
```

-	Layers:
	-	`sha256:4010fb6f8cd55b2d9050987eb8cb50842e8a63876073d6f558e059aaf51f6a28`  
		Last Modified: Wed, 04 Oct 2023 22:59:57 GMT  
		Size: 14.4 MB (14422978 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:9861c670f5c58916f944bffb660bde5d1803c908bc60e07d263d2937b13ab2f6`  
		Last Modified: Wed, 04 Oct 2023 22:59:56 GMT  
		Size: 36.5 KB (36452 bytes)  
		MIME: application/vnd.in-toto+json

## `mysql:8`

```console
$ docker pull mysql@sha256:9592f7dad3d285b9d2f89b1e9a586dbed983deb72ec190ba7d6af12120781d2e
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `mysql:8` - linux; amd64

```console
$ docker pull mysql@sha256:5253d1662109ba7776430522fd73bd37f1c5775235eec63883fb8294d22757bc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **166.9 MB (166863356 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c138801544a941ed9d1171794e3361533109aa7e22f2ea4e1ba85bccc84f6842`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 27 Jul 2023 22:18:51 GMT
ADD file:909c07f3bad92a80d3917d583769a01bf62c2cbf3dd24f450fb303b1db92a83e in / 
# Thu, 27 Jul 2023 22:18:51 GMT
CMD ["/bin/bash"]
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
ENV GOSU_VERSION=1.16
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME" # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
ENV MYSQL_MAJOR=innovation
# Thu, 27 Jul 2023 22:18:51 GMT
ENV MYSQL_VERSION=8.1.0-1.el8
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysqlinnovation-server-minimal]'; 		echo 'name=MySQL innovation Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-innovation-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
ENV MYSQL_SHELL_VERSION=8.0.34-1.el8
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
VOLUME [/var/lib/mysql]
# Thu, 27 Jul 2023 22:18:51 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 27 Jul 2023 22:18:51 GMT
EXPOSE map[3306/tcp:{} 33060/tcp:{}]
# Thu, 27 Jul 2023 22:18:51 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:5262579e8e45cb87fdc8fb6182d30da3c9e4f1036e02223508f287899ea434c0`  
		Last Modified: Thu, 21 Sep 2023 23:25:18 GMT  
		Size: 45.0 MB (44959147 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bfcc921068b5eaba8d310a26395ee4139cd54b21ec96369a39830e24cfe84477`  
		Last Modified: Wed, 04 Oct 2023 23:00:11 GMT  
		Size: 885.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:072a02315ab18d41372cf2e57b066a8ecf9954ab8d94cb5244ca20efe63df7ab`  
		Last Modified: Wed, 04 Oct 2023 23:00:11 GMT  
		Size: 982.8 KB (982808 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:711d47be56b4655b6deec62a811cddf52424477672f5930441ae8701ab012c95`  
		Last Modified: Wed, 04 Oct 2023 23:00:12 GMT  
		Size: 4.6 MB (4616305 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:755e67622a77c61bb6eb442164103b5395e7db380add9d61a2acb3425df65fa0`  
		Last Modified: Wed, 04 Oct 2023 23:00:12 GMT  
		Size: 2.6 KB (2608 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0080a11112d165a07d366db3a1ebd57709f066f4b13f10b57ec21e19d3d67d26`  
		Last Modified: Wed, 04 Oct 2023 23:00:12 GMT  
		Size: 340.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:adc45022a9ad6beda852b49f14ae18ff04ea052eb0f9391c31a29ecdffaa1ef1`  
		Last Modified: Wed, 04 Oct 2023 23:00:17 GMT  
		Size: 58.8 MB (58771345 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:67d8146998603ea2ed92b77bccbb35623a5eb39c6b047d15af930cec9ef79a9d`  
		Last Modified: Wed, 04 Oct 2023 23:00:13 GMT  
		Size: 316.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f431d85cf61e18099acd66976a43fb86be0ca84549a3853b4e2eaeb48557acb8`  
		Last Modified: Wed, 04 Oct 2023 23:00:16 GMT  
		Size: 57.5 MB (57524213 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4bbba6dd5ce26ba0b294a1cc506c8a57566efbaaf3701fe8eb752b54c4bd64c5`  
		Last Modified: Wed, 04 Oct 2023 23:00:14 GMT  
		Size: 5.4 KB (5389 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:8` - unknown; unknown

```console
$ docker pull mysql@sha256:3907151ff6c8a3d9a987e42f5af74ec79742398d67673c9e6f3baf067cbff3ab
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.1 MB (13141082 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3992e42cff0b10e86e3648547df8a978c66d19322dd629faa7cdacd2432028c9`

```dockerfile
```

-	Layers:
	-	`sha256:06d7ee16ec055f718e85ab70b205f9a40ac64f1f4bd3665bfd625ceffdce177c`  
		Last Modified: Wed, 04 Oct 2023 23:00:12 GMT  
		Size: 13.1 MB (13107503 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:81f9eeabc6e68920db4c4c28565e7cdbb580ecb31d9205d49fb827e33e860dd3`  
		Last Modified: Wed, 04 Oct 2023 23:00:11 GMT  
		Size: 33.6 KB (33579 bytes)  
		MIME: application/vnd.in-toto+json

### `mysql:8` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:8cacf9ef3db6f3e040c4ecde7f897706401d1f8330ca96862744e8b0d5781454
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.4 MB (170371412 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d30a00232fdc87bddbd635dad0486bf2278d705c76af20ec01f0814d0481064f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 27 Jul 2023 22:18:51 GMT
ADD file:b51d9ae1b78eb07ac424bfa71c45180e09ea3a5ed18fbfbcf881fb540bf83e9a in / 
# Thu, 27 Jul 2023 22:18:51 GMT
CMD ["/bin/bash"]
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
ENV GOSU_VERSION=1.16
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME" # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
ENV MYSQL_MAJOR=innovation
# Thu, 27 Jul 2023 22:18:51 GMT
ENV MYSQL_VERSION=8.1.0-1.el8
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysqlinnovation-server-minimal]'; 		echo 'name=MySQL innovation Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-innovation-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
ENV MYSQL_SHELL_VERSION=8.0.34-1.el8
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
VOLUME [/var/lib/mysql]
# Thu, 27 Jul 2023 22:18:51 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 27 Jul 2023 22:18:51 GMT
EXPOSE map[3306/tcp:{} 33060/tcp:{}]
# Thu, 27 Jul 2023 22:18:51 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:89ec84aa94fe6a62fb4e9f51aced09dea3cc4d7979c9f0ebd6b5bd4fd729e04e`  
		Last Modified: Thu, 12 Oct 2023 11:01:48 GMT  
		Size: 43.7 MB (43669807 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2047d0a85fcf9107bca7c22f98448ccf140ceed34e3b161beeb4904344032ab7`  
		Last Modified: Thu, 12 Oct 2023 20:57:52 GMT  
		Size: 884.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a981666a88bb712c4283e2a0a14f7ab9b27ff60bfc893fba647a0dbfaa93f6d0`  
		Last Modified: Thu, 12 Oct 2023 20:57:52 GMT  
		Size: 913.0 KB (912965 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7aa9dbd754432215cdd312410444c1c3859b4196dc771c13eba5a56682bef8dc`  
		Last Modified: Thu, 12 Oct 2023 20:57:52 GMT  
		Size: 4.3 MB (4303472 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b8ed90386e32a0124cf2dbca9de0ca31cd5f666b339a7e9a63dae44ed117e587`  
		Last Modified: Thu, 12 Oct 2023 20:57:53 GMT  
		Size: 2.6 KB (2609 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0b36981941b7e06e20d54a95dc6d483b22da2cb1e1fe68e9a77bcbcd2f55696c`  
		Last Modified: Thu, 12 Oct 2023 20:57:53 GMT  
		Size: 341.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ca996c23fc53d3fd7658d98952a4d481ae66e74585e2b72c55f961bf54455736`  
		Last Modified: Thu, 12 Oct 2023 20:57:57 GMT  
		Size: 57.7 MB (57701851 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:15050e9043e65433ddefd92b793734e91755006d5f756c6a9259998e9ccf916a`  
		Last Modified: Thu, 12 Oct 2023 20:57:54 GMT  
		Size: 316.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3ecfc97ced27490a7dd8db645fba5623698b5a933cb2359aedacf99e2dd74d54`  
		Last Modified: Thu, 12 Oct 2023 20:57:58 GMT  
		Size: 63.8 MB (63773775 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e435e3bf4d77af270e3b5245b5aa6234fcd3bb791ed57db4641d7ef99b33bf18`  
		Last Modified: Thu, 12 Oct 2023 20:57:55 GMT  
		Size: 5.4 KB (5392 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:8` - unknown; unknown

```console
$ docker pull mysql@sha256:33f7834b9a596feb3b7660924e45d3886bc1908da500f449c853ace58e7ef70d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.1 MB (13140098 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31013d6e714b5c7d6108fc3965658f4e7d97b6c8aa096f02b8230c4e1ebf99ae`

```dockerfile
```

-	Layers:
	-	`sha256:564dbabf3309a798678bcee0a9ac7f451cacb91050175a2e98f9313a605ae7cd`  
		Last Modified: Thu, 12 Oct 2023 20:57:54 GMT  
		Size: 13.1 MB (13106498 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:18613fc7c61e609bc95ef7402649a9c574fb26d032c9df3aa4e7b3f9b86b70e4`  
		Last Modified: Thu, 12 Oct 2023 20:57:52 GMT  
		Size: 33.6 KB (33600 bytes)  
		MIME: application/vnd.in-toto+json

## `mysql:8-oracle`

```console
$ docker pull mysql@sha256:9592f7dad3d285b9d2f89b1e9a586dbed983deb72ec190ba7d6af12120781d2e
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `mysql:8-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:5253d1662109ba7776430522fd73bd37f1c5775235eec63883fb8294d22757bc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **166.9 MB (166863356 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c138801544a941ed9d1171794e3361533109aa7e22f2ea4e1ba85bccc84f6842`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 27 Jul 2023 22:18:51 GMT
ADD file:909c07f3bad92a80d3917d583769a01bf62c2cbf3dd24f450fb303b1db92a83e in / 
# Thu, 27 Jul 2023 22:18:51 GMT
CMD ["/bin/bash"]
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
ENV GOSU_VERSION=1.16
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME" # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
ENV MYSQL_MAJOR=innovation
# Thu, 27 Jul 2023 22:18:51 GMT
ENV MYSQL_VERSION=8.1.0-1.el8
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysqlinnovation-server-minimal]'; 		echo 'name=MySQL innovation Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-innovation-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
ENV MYSQL_SHELL_VERSION=8.0.34-1.el8
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
VOLUME [/var/lib/mysql]
# Thu, 27 Jul 2023 22:18:51 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 27 Jul 2023 22:18:51 GMT
EXPOSE map[3306/tcp:{} 33060/tcp:{}]
# Thu, 27 Jul 2023 22:18:51 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:5262579e8e45cb87fdc8fb6182d30da3c9e4f1036e02223508f287899ea434c0`  
		Last Modified: Thu, 21 Sep 2023 23:25:18 GMT  
		Size: 45.0 MB (44959147 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bfcc921068b5eaba8d310a26395ee4139cd54b21ec96369a39830e24cfe84477`  
		Last Modified: Wed, 04 Oct 2023 23:00:11 GMT  
		Size: 885.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:072a02315ab18d41372cf2e57b066a8ecf9954ab8d94cb5244ca20efe63df7ab`  
		Last Modified: Wed, 04 Oct 2023 23:00:11 GMT  
		Size: 982.8 KB (982808 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:711d47be56b4655b6deec62a811cddf52424477672f5930441ae8701ab012c95`  
		Last Modified: Wed, 04 Oct 2023 23:00:12 GMT  
		Size: 4.6 MB (4616305 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:755e67622a77c61bb6eb442164103b5395e7db380add9d61a2acb3425df65fa0`  
		Last Modified: Wed, 04 Oct 2023 23:00:12 GMT  
		Size: 2.6 KB (2608 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0080a11112d165a07d366db3a1ebd57709f066f4b13f10b57ec21e19d3d67d26`  
		Last Modified: Wed, 04 Oct 2023 23:00:12 GMT  
		Size: 340.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:adc45022a9ad6beda852b49f14ae18ff04ea052eb0f9391c31a29ecdffaa1ef1`  
		Last Modified: Wed, 04 Oct 2023 23:00:17 GMT  
		Size: 58.8 MB (58771345 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:67d8146998603ea2ed92b77bccbb35623a5eb39c6b047d15af930cec9ef79a9d`  
		Last Modified: Wed, 04 Oct 2023 23:00:13 GMT  
		Size: 316.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f431d85cf61e18099acd66976a43fb86be0ca84549a3853b4e2eaeb48557acb8`  
		Last Modified: Wed, 04 Oct 2023 23:00:16 GMT  
		Size: 57.5 MB (57524213 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4bbba6dd5ce26ba0b294a1cc506c8a57566efbaaf3701fe8eb752b54c4bd64c5`  
		Last Modified: Wed, 04 Oct 2023 23:00:14 GMT  
		Size: 5.4 KB (5389 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:8-oracle` - unknown; unknown

```console
$ docker pull mysql@sha256:3907151ff6c8a3d9a987e42f5af74ec79742398d67673c9e6f3baf067cbff3ab
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.1 MB (13141082 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3992e42cff0b10e86e3648547df8a978c66d19322dd629faa7cdacd2432028c9`

```dockerfile
```

-	Layers:
	-	`sha256:06d7ee16ec055f718e85ab70b205f9a40ac64f1f4bd3665bfd625ceffdce177c`  
		Last Modified: Wed, 04 Oct 2023 23:00:12 GMT  
		Size: 13.1 MB (13107503 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:81f9eeabc6e68920db4c4c28565e7cdbb580ecb31d9205d49fb827e33e860dd3`  
		Last Modified: Wed, 04 Oct 2023 23:00:11 GMT  
		Size: 33.6 KB (33579 bytes)  
		MIME: application/vnd.in-toto+json

### `mysql:8-oracle` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:8cacf9ef3db6f3e040c4ecde7f897706401d1f8330ca96862744e8b0d5781454
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.4 MB (170371412 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d30a00232fdc87bddbd635dad0486bf2278d705c76af20ec01f0814d0481064f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 27 Jul 2023 22:18:51 GMT
ADD file:b51d9ae1b78eb07ac424bfa71c45180e09ea3a5ed18fbfbcf881fb540bf83e9a in / 
# Thu, 27 Jul 2023 22:18:51 GMT
CMD ["/bin/bash"]
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
ENV GOSU_VERSION=1.16
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME" # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
ENV MYSQL_MAJOR=innovation
# Thu, 27 Jul 2023 22:18:51 GMT
ENV MYSQL_VERSION=8.1.0-1.el8
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysqlinnovation-server-minimal]'; 		echo 'name=MySQL innovation Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-innovation-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
ENV MYSQL_SHELL_VERSION=8.0.34-1.el8
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
VOLUME [/var/lib/mysql]
# Thu, 27 Jul 2023 22:18:51 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 27 Jul 2023 22:18:51 GMT
EXPOSE map[3306/tcp:{} 33060/tcp:{}]
# Thu, 27 Jul 2023 22:18:51 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:89ec84aa94fe6a62fb4e9f51aced09dea3cc4d7979c9f0ebd6b5bd4fd729e04e`  
		Last Modified: Thu, 12 Oct 2023 11:01:48 GMT  
		Size: 43.7 MB (43669807 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2047d0a85fcf9107bca7c22f98448ccf140ceed34e3b161beeb4904344032ab7`  
		Last Modified: Thu, 12 Oct 2023 20:57:52 GMT  
		Size: 884.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a981666a88bb712c4283e2a0a14f7ab9b27ff60bfc893fba647a0dbfaa93f6d0`  
		Last Modified: Thu, 12 Oct 2023 20:57:52 GMT  
		Size: 913.0 KB (912965 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7aa9dbd754432215cdd312410444c1c3859b4196dc771c13eba5a56682bef8dc`  
		Last Modified: Thu, 12 Oct 2023 20:57:52 GMT  
		Size: 4.3 MB (4303472 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b8ed90386e32a0124cf2dbca9de0ca31cd5f666b339a7e9a63dae44ed117e587`  
		Last Modified: Thu, 12 Oct 2023 20:57:53 GMT  
		Size: 2.6 KB (2609 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0b36981941b7e06e20d54a95dc6d483b22da2cb1e1fe68e9a77bcbcd2f55696c`  
		Last Modified: Thu, 12 Oct 2023 20:57:53 GMT  
		Size: 341.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ca996c23fc53d3fd7658d98952a4d481ae66e74585e2b72c55f961bf54455736`  
		Last Modified: Thu, 12 Oct 2023 20:57:57 GMT  
		Size: 57.7 MB (57701851 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:15050e9043e65433ddefd92b793734e91755006d5f756c6a9259998e9ccf916a`  
		Last Modified: Thu, 12 Oct 2023 20:57:54 GMT  
		Size: 316.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3ecfc97ced27490a7dd8db645fba5623698b5a933cb2359aedacf99e2dd74d54`  
		Last Modified: Thu, 12 Oct 2023 20:57:58 GMT  
		Size: 63.8 MB (63773775 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e435e3bf4d77af270e3b5245b5aa6234fcd3bb791ed57db4641d7ef99b33bf18`  
		Last Modified: Thu, 12 Oct 2023 20:57:55 GMT  
		Size: 5.4 KB (5392 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:8-oracle` - unknown; unknown

```console
$ docker pull mysql@sha256:33f7834b9a596feb3b7660924e45d3886bc1908da500f449c853ace58e7ef70d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.1 MB (13140098 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31013d6e714b5c7d6108fc3965658f4e7d97b6c8aa096f02b8230c4e1ebf99ae`

```dockerfile
```

-	Layers:
	-	`sha256:564dbabf3309a798678bcee0a9ac7f451cacb91050175a2e98f9313a605ae7cd`  
		Last Modified: Thu, 12 Oct 2023 20:57:54 GMT  
		Size: 13.1 MB (13106498 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:18613fc7c61e609bc95ef7402649a9c574fb26d032c9df3aa4e7b3f9b86b70e4`  
		Last Modified: Thu, 12 Oct 2023 20:57:52 GMT  
		Size: 33.6 KB (33600 bytes)  
		MIME: application/vnd.in-toto+json

## `mysql:8.0`

```console
$ docker pull mysql@sha256:d69594a49f14c02df7eee5b265509e1fb131b1e9e1e54bee932c93051c010576
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `mysql:8.0` - linux; amd64

```console
$ docker pull mysql@sha256:0813cfe2d80467f39323b14c13ddbd25d57f56b051f4f1434e10a741f26fce05
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **166.6 MB (166593320 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82ebbd05b8a93f1c4a97ea6d89f3bd577a2e2330ad815a8dc967a383b83e7a36`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 20 Jul 2023 22:15:44 GMT
ADD file:909c07f3bad92a80d3917d583769a01bf62c2cbf3dd24f450fb303b1db92a83e in / 
# Thu, 20 Jul 2023 22:15:44 GMT
CMD ["/bin/bash"]
# Thu, 20 Jul 2023 22:15:44 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql # buildkit
# Thu, 20 Jul 2023 22:15:44 GMT
ENV GOSU_VERSION=1.16
# Thu, 20 Jul 2023 22:15:44 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Thu, 20 Jul 2023 22:15:44 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all # buildkit
# Thu, 20 Jul 2023 22:15:44 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME" # buildkit
# Thu, 20 Jul 2023 22:15:44 GMT
ENV MYSQL_MAJOR=8.0
# Thu, 20 Jul 2023 22:15:44 GMT
ENV MYSQL_VERSION=8.0.34-1.el8
# Thu, 20 Jul 2023 22:15:44 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo # buildkit
# Thu, 20 Jul 2023 22:15:44 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version # buildkit
# Thu, 20 Jul 2023 22:15:44 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo # buildkit
# Thu, 20 Jul 2023 22:15:44 GMT
ENV MYSQL_SHELL_VERSION=8.0.34-1.el8
# Thu, 20 Jul 2023 22:15:44 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version # buildkit
# Thu, 20 Jul 2023 22:15:44 GMT
VOLUME [/var/lib/mysql]
# Thu, 20 Jul 2023 22:15:44 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 20 Jul 2023 22:15:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Thu, 20 Jul 2023 22:15:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 20 Jul 2023 22:15:44 GMT
EXPOSE map[3306/tcp:{} 33060/tcp:{}]
# Thu, 20 Jul 2023 22:15:44 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:5262579e8e45cb87fdc8fb6182d30da3c9e4f1036e02223508f287899ea434c0`  
		Last Modified: Thu, 21 Sep 2023 23:25:18 GMT  
		Size: 45.0 MB (44959147 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c6f87bacd0dd48614ce31c95a5a76f58b1e17d8ceb0646a7cf0335d90baab73a`  
		Last Modified: Wed, 04 Oct 2023 23:00:27 GMT  
		Size: 885.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:581ee7db3e6539c1487c7299b747b063264033fde750dc1e1b36fb6c91a6d464`  
		Last Modified: Wed, 04 Oct 2023 23:00:27 GMT  
		Size: 982.8 KB (982804 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6d5c555a4100d6aeb3f92f990c72e9d32ffe30a355514a7ea5837c9a25192469`  
		Last Modified: Wed, 04 Oct 2023 23:00:28 GMT  
		Size: 4.6 MB (4616288 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:51f4afa7a279674cb5f4caa704105e4075b72efe0433c19776b2add99b59db66`  
		Last Modified: Wed, 04 Oct 2023 23:00:27 GMT  
		Size: 2.6 KB (2609 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d9e414f0b7c63dca45882245d6db287a6389f7f6efa747d3b305d86061754531`  
		Last Modified: Wed, 04 Oct 2023 23:00:28 GMT  
		Size: 332.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:aab3a444c469d72844d9607f27c890e4cb85d6751258bbbd81d5b054994159cf`  
		Last Modified: Wed, 04 Oct 2023 23:00:32 GMT  
		Size: 58.5 MB (58504954 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:aab51168fe3adf75d6483923d31c0774e50df598dc12d918655721b79b506d53`  
		Last Modified: Wed, 04 Oct 2023 23:00:29 GMT  
		Size: 315.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2a63757e7c9cf1e09fdc5c53f2de48cfd45a36e7a461907a3a63a6ebb85d3b4b`  
		Last Modified: Wed, 04 Oct 2023 23:00:32 GMT  
		Size: 57.5 MB (57520476 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:830e4b0cc0bc97158e46ff390f7d92c8967d38898bd4db483486d43ef76eeaba`  
		Last Modified: Wed, 04 Oct 2023 23:00:29 GMT  
		Size: 5.4 KB (5389 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cc0cd1f61ed72c4ad76bb8f7e6cf5156a5c602aea6d3157120a075eb86aa197d`  
		Last Modified: Wed, 04 Oct 2023 23:00:30 GMT  
		Size: 121.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:8.0` - unknown; unknown

```console
$ docker pull mysql@sha256:e6ae739fba80627190a3c51e20d0accb8d7d869dd591dfe1d5583a2aea571999
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.1 MB (13140061 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e22c57b768cdd0e2d048d4fcce33a660a75af3a4d046066bbef5cb5742116ff9`

```dockerfile
```

-	Layers:
	-	`sha256:64288b670e6f8145940a7536a8228eb4756812dda4a5395e645186c59582d34b`  
		Last Modified: Wed, 04 Oct 2023 23:00:28 GMT  
		Size: 13.1 MB (13105867 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:bbb01f0ecc5a33972b0e55c7f1cca10087cd381068ee443a51f25cefa45e36ee`  
		Last Modified: Wed, 04 Oct 2023 23:00:27 GMT  
		Size: 34.2 KB (34194 bytes)  
		MIME: application/vnd.in-toto+json

### `mysql:8.0` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:cea62ed306c9e2a96a3d8672381cdff326fd90123d284ef4852153c0a877835b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.1 MB (170129736 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01c3aea4e3deeec5a6139350e9c1bc1f108fbfdbeb136054e77ef4669e4ae1f7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 20 Jul 2023 22:15:44 GMT
ADD file:b51d9ae1b78eb07ac424bfa71c45180e09ea3a5ed18fbfbcf881fb540bf83e9a in / 
# Thu, 20 Jul 2023 22:15:44 GMT
CMD ["/bin/bash"]
# Thu, 20 Jul 2023 22:15:44 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql # buildkit
# Thu, 20 Jul 2023 22:15:44 GMT
ENV GOSU_VERSION=1.16
# Thu, 20 Jul 2023 22:15:44 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Thu, 20 Jul 2023 22:15:44 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all # buildkit
# Thu, 20 Jul 2023 22:15:44 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME" # buildkit
# Thu, 20 Jul 2023 22:15:44 GMT
ENV MYSQL_MAJOR=8.0
# Thu, 20 Jul 2023 22:15:44 GMT
ENV MYSQL_VERSION=8.0.34-1.el8
# Thu, 20 Jul 2023 22:15:44 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo # buildkit
# Thu, 20 Jul 2023 22:15:44 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version # buildkit
# Thu, 20 Jul 2023 22:15:44 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo # buildkit
# Thu, 20 Jul 2023 22:15:44 GMT
ENV MYSQL_SHELL_VERSION=8.0.34-1.el8
# Thu, 20 Jul 2023 22:15:44 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version # buildkit
# Thu, 20 Jul 2023 22:15:44 GMT
VOLUME [/var/lib/mysql]
# Thu, 20 Jul 2023 22:15:44 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 20 Jul 2023 22:15:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Thu, 20 Jul 2023 22:15:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 20 Jul 2023 22:15:44 GMT
EXPOSE map[3306/tcp:{} 33060/tcp:{}]
# Thu, 20 Jul 2023 22:15:44 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:89ec84aa94fe6a62fb4e9f51aced09dea3cc4d7979c9f0ebd6b5bd4fd729e04e`  
		Last Modified: Thu, 12 Oct 2023 11:01:48 GMT  
		Size: 43.7 MB (43669807 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2047d0a85fcf9107bca7c22f98448ccf140ceed34e3b161beeb4904344032ab7`  
		Last Modified: Thu, 12 Oct 2023 20:57:52 GMT  
		Size: 884.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a981666a88bb712c4283e2a0a14f7ab9b27ff60bfc893fba647a0dbfaa93f6d0`  
		Last Modified: Thu, 12 Oct 2023 20:57:52 GMT  
		Size: 913.0 KB (912965 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7aa9dbd754432215cdd312410444c1c3859b4196dc771c13eba5a56682bef8dc`  
		Last Modified: Thu, 12 Oct 2023 20:57:52 GMT  
		Size: 4.3 MB (4303472 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b8ed90386e32a0124cf2dbca9de0ca31cd5f666b339a7e9a63dae44ed117e587`  
		Last Modified: Thu, 12 Oct 2023 20:57:53 GMT  
		Size: 2.6 KB (2609 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:acf89d2c4916c1368bf3a4c6fb20a4441ec8cd4a3d57bdb015e9277b17286a03`  
		Last Modified: Thu, 12 Oct 2023 20:59:37 GMT  
		Size: 334.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:79120d0882796ce1ccdabc2e93d363faa3227c0773f4dccdad561aab2814f783`  
		Last Modified: Thu, 12 Oct 2023 20:59:41 GMT  
		Size: 57.5 MB (57461596 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c2d0fac447c9eae2f0323e6dedbe3131b2f651c46d5c52ee869f8d2e028a6c0e`  
		Last Modified: Thu, 12 Oct 2023 20:59:37 GMT  
		Size: 316.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6095297ac0a99514ffaa4f43e03709f12a64bce3301266c6324beabac8608835`  
		Last Modified: Thu, 12 Oct 2023 20:59:42 GMT  
		Size: 63.8 MB (63772242 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e274f5c921d7f5b78607112364fe96697bb43f6d9af8e38152c9d06b8cb0c9c9`  
		Last Modified: Thu, 12 Oct 2023 20:59:38 GMT  
		Size: 5.4 KB (5391 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:969873ad404751d35993621a462d3350aeb15f63238fc5930bd78d177d52db66`  
		Last Modified: Thu, 12 Oct 2023 20:59:39 GMT  
		Size: 120.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:8.0` - unknown; unknown

```console
$ docker pull mysql@sha256:3bc988bea23d6f5fd6693b7be9a8da8ace0346c8150ebe4bb0ea4e75cea797cb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.1 MB (13138887 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:857f42418489e182abc8b171c9c5048be74e446e9448248ec9e30443bdfb6aa9`

```dockerfile
```

-	Layers:
	-	`sha256:243dd07e28b64dcf4c34487ff9d905b095c9774305c321224a45370ccdeea70b`  
		Last Modified: Thu, 12 Oct 2023 20:59:39 GMT  
		Size: 13.1 MB (13104850 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:36467b2da21cc688d8b4728c2e497669d084b9212de6b061103a4c13b82a64d5`  
		Last Modified: Thu, 12 Oct 2023 20:59:37 GMT  
		Size: 34.0 KB (34037 bytes)  
		MIME: application/vnd.in-toto+json

## `mysql:8.0-debian`

```console
$ docker pull mysql@sha256:2a31847951cdf92d6901ef58b4c5a9fbe75b47823d9ade1f7a4652ede7a88e2d
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 2
	-	linux; amd64
	-	unknown; unknown

### `mysql:8.0-debian` - linux; amd64

```console
$ docker pull mysql@sha256:e10fb73841ef30dcdb02e0759035f7730e5303cdc455268de219407d3fb4b846
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **179.1 MB (179083456 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc21a4e132a7e63c4a4eca71b3e75fbc7e965aef2b157a60a9c322e41e592795`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 20 Jul 2023 22:15:44 GMT
ADD file:cb13581b8e7a9de4396639e5ca2f3817763435c0563232f85e3d899f6388a1b3 in / 
# Thu, 20 Jul 2023 22:15:44 GMT
CMD ["bash"]
# Thu, 20 Jul 2023 22:15:44 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql # buildkit
# Thu, 20 Jul 2023 22:15:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg && rm -rf /var/lib/apt/lists/* # buildkit
# Thu, 20 Jul 2023 22:15:44 GMT
ENV GOSU_VERSION=1.16
# Thu, 20 Jul 2023 22:15:44 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Thu, 20 Jul 2023 22:15:44 GMT
RUN mkdir /docker-entrypoint-initdb.d # buildkit
# Thu, 20 Jul 2023 22:15:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Thu, 20 Jul 2023 22:15:44 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" # buildkit
# Thu, 20 Jul 2023 22:15:44 GMT
ENV MYSQL_MAJOR=8.0
# Thu, 20 Jul 2023 22:15:44 GMT
ENV MYSQL_VERSION=8.0.34-1debian11
# Thu, 20 Jul 2023 22:15:44 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ bullseye mysql-8.0' > /etc/apt/sources.list.d/mysql.list # buildkit
# Thu, 20 Jul 2023 22:15:44 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql # buildkit
# Thu, 20 Jul 2023 22:15:44 GMT
VOLUME [/var/lib/mysql]
# Thu, 20 Jul 2023 22:15:44 GMT
COPY config/ /etc/mysql/ # buildkit
# Thu, 20 Jul 2023 22:15:44 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 20 Jul 2023 22:15:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Thu, 20 Jul 2023 22:15:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 20 Jul 2023 22:15:44 GMT
EXPOSE map[3306/tcp:{} 33060/tcp:{}]
# Thu, 20 Jul 2023 22:15:44 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:e67fdae3559346105027c63e7fb032bba57e62b1fe9f2da23e6fdfb56384e00b`  
		Last Modified: Wed, 11 Oct 2023 18:40:17 GMT  
		Size: 31.4 MB (31417862 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cf330228e741604571f4caab61f2cc172717b89147d1238d45d057fb46edb697`  
		Last Modified: Wed, 11 Oct 2023 20:03:39 GMT  
		Size: 1.6 KB (1646 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bafbe13d22f4d4ef6ed406ac05b335dc1371424f95a2beafc66051e6cb3974bf`  
		Last Modified: Wed, 11 Oct 2023 20:03:40 GMT  
		Size: 4.2 MB (4207542 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d8dcfd9f33b298cff0fc2ee7fd95dbd76a738414a4269d51121ef718fbcbf87b`  
		Last Modified: Wed, 11 Oct 2023 20:03:39 GMT  
		Size: 1.5 MB (1472483 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:21ae14d9c3e441351e1ec5b465e6bf617e393bc4a0ad072589600a2b8ae73b37`  
		Last Modified: Wed, 11 Oct 2023 20:03:39 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1086d8d2521ba8f681003c1bb0594f31379d599a291c6646085f007fe8f395a1`  
		Last Modified: Wed, 11 Oct 2023 20:03:41 GMT  
		Size: 12.5 MB (12455173 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:16afe97457504eb7005a224c7c679006bb937483986e5365633519004752f789`  
		Last Modified: Wed, 11 Oct 2023 20:03:40 GMT  
		Size: 2.5 KB (2497 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8169ee2bdb0a81c638c5dfb7aeef3c7c5b17755771f95a889cfe4c29b26e4966`  
		Last Modified: Wed, 11 Oct 2023 20:03:41 GMT  
		Size: 248.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8fdc0f64b1cbafeb07f2c175c0486123720ed151cdd007b251816564e4381d23`  
		Last Modified: Wed, 11 Oct 2023 20:03:47 GMT  
		Size: 129.5 MB (129519547 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3994da0db6238691c6a2208c2da4b3dafb961db6ca184feedab3435104154f4d`  
		Last Modified: Wed, 11 Oct 2023 20:03:41 GMT  
		Size: 837.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ae385311e5ed3100ff6111e185211d9a5749c784bd675d0ba713898acb9dafd8`  
		Last Modified: Wed, 11 Oct 2023 20:03:42 GMT  
		Size: 5.4 KB (5383 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e2ceafee559334b9217ef6cde4d657abe3fb79466a7ef1b5e6f911d185b689f6`  
		Last Modified: Wed, 11 Oct 2023 20:03:42 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:8.0-debian` - unknown; unknown

```console
$ docker pull mysql@sha256:2831145c9d8abb4571f51bd89b331516c37b2b0421ec56d2647082e631ce3d7c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.5 MB (3484026 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95857c88929774216f8e99858617023ea09d821927280ca85a5fbfdc8a6a609a`

```dockerfile
```

-	Layers:
	-	`sha256:d6cded17556303c4d1affc0cc57b7ae8b5fdce8a01462b0b5bf4608e0e7a413d`  
		Last Modified: Wed, 11 Oct 2023 20:03:39 GMT  
		Size: 3.5 MB (3450737 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:29553eed5402c121dca04ea081b05fbfc44820c10ddb43cc09308bc0051fd6c1`  
		Last Modified: Wed, 11 Oct 2023 20:03:39 GMT  
		Size: 33.3 KB (33289 bytes)  
		MIME: application/vnd.in-toto+json

## `mysql:8.0-oracle`

```console
$ docker pull mysql@sha256:d69594a49f14c02df7eee5b265509e1fb131b1e9e1e54bee932c93051c010576
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `mysql:8.0-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:0813cfe2d80467f39323b14c13ddbd25d57f56b051f4f1434e10a741f26fce05
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **166.6 MB (166593320 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82ebbd05b8a93f1c4a97ea6d89f3bd577a2e2330ad815a8dc967a383b83e7a36`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 20 Jul 2023 22:15:44 GMT
ADD file:909c07f3bad92a80d3917d583769a01bf62c2cbf3dd24f450fb303b1db92a83e in / 
# Thu, 20 Jul 2023 22:15:44 GMT
CMD ["/bin/bash"]
# Thu, 20 Jul 2023 22:15:44 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql # buildkit
# Thu, 20 Jul 2023 22:15:44 GMT
ENV GOSU_VERSION=1.16
# Thu, 20 Jul 2023 22:15:44 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Thu, 20 Jul 2023 22:15:44 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all # buildkit
# Thu, 20 Jul 2023 22:15:44 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME" # buildkit
# Thu, 20 Jul 2023 22:15:44 GMT
ENV MYSQL_MAJOR=8.0
# Thu, 20 Jul 2023 22:15:44 GMT
ENV MYSQL_VERSION=8.0.34-1.el8
# Thu, 20 Jul 2023 22:15:44 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo # buildkit
# Thu, 20 Jul 2023 22:15:44 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version # buildkit
# Thu, 20 Jul 2023 22:15:44 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo # buildkit
# Thu, 20 Jul 2023 22:15:44 GMT
ENV MYSQL_SHELL_VERSION=8.0.34-1.el8
# Thu, 20 Jul 2023 22:15:44 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version # buildkit
# Thu, 20 Jul 2023 22:15:44 GMT
VOLUME [/var/lib/mysql]
# Thu, 20 Jul 2023 22:15:44 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 20 Jul 2023 22:15:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Thu, 20 Jul 2023 22:15:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 20 Jul 2023 22:15:44 GMT
EXPOSE map[3306/tcp:{} 33060/tcp:{}]
# Thu, 20 Jul 2023 22:15:44 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:5262579e8e45cb87fdc8fb6182d30da3c9e4f1036e02223508f287899ea434c0`  
		Last Modified: Thu, 21 Sep 2023 23:25:18 GMT  
		Size: 45.0 MB (44959147 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c6f87bacd0dd48614ce31c95a5a76f58b1e17d8ceb0646a7cf0335d90baab73a`  
		Last Modified: Wed, 04 Oct 2023 23:00:27 GMT  
		Size: 885.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:581ee7db3e6539c1487c7299b747b063264033fde750dc1e1b36fb6c91a6d464`  
		Last Modified: Wed, 04 Oct 2023 23:00:27 GMT  
		Size: 982.8 KB (982804 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6d5c555a4100d6aeb3f92f990c72e9d32ffe30a355514a7ea5837c9a25192469`  
		Last Modified: Wed, 04 Oct 2023 23:00:28 GMT  
		Size: 4.6 MB (4616288 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:51f4afa7a279674cb5f4caa704105e4075b72efe0433c19776b2add99b59db66`  
		Last Modified: Wed, 04 Oct 2023 23:00:27 GMT  
		Size: 2.6 KB (2609 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d9e414f0b7c63dca45882245d6db287a6389f7f6efa747d3b305d86061754531`  
		Last Modified: Wed, 04 Oct 2023 23:00:28 GMT  
		Size: 332.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:aab3a444c469d72844d9607f27c890e4cb85d6751258bbbd81d5b054994159cf`  
		Last Modified: Wed, 04 Oct 2023 23:00:32 GMT  
		Size: 58.5 MB (58504954 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:aab51168fe3adf75d6483923d31c0774e50df598dc12d918655721b79b506d53`  
		Last Modified: Wed, 04 Oct 2023 23:00:29 GMT  
		Size: 315.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2a63757e7c9cf1e09fdc5c53f2de48cfd45a36e7a461907a3a63a6ebb85d3b4b`  
		Last Modified: Wed, 04 Oct 2023 23:00:32 GMT  
		Size: 57.5 MB (57520476 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:830e4b0cc0bc97158e46ff390f7d92c8967d38898bd4db483486d43ef76eeaba`  
		Last Modified: Wed, 04 Oct 2023 23:00:29 GMT  
		Size: 5.4 KB (5389 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cc0cd1f61ed72c4ad76bb8f7e6cf5156a5c602aea6d3157120a075eb86aa197d`  
		Last Modified: Wed, 04 Oct 2023 23:00:30 GMT  
		Size: 121.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:8.0-oracle` - unknown; unknown

```console
$ docker pull mysql@sha256:e6ae739fba80627190a3c51e20d0accb8d7d869dd591dfe1d5583a2aea571999
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.1 MB (13140061 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e22c57b768cdd0e2d048d4fcce33a660a75af3a4d046066bbef5cb5742116ff9`

```dockerfile
```

-	Layers:
	-	`sha256:64288b670e6f8145940a7536a8228eb4756812dda4a5395e645186c59582d34b`  
		Last Modified: Wed, 04 Oct 2023 23:00:28 GMT  
		Size: 13.1 MB (13105867 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:bbb01f0ecc5a33972b0e55c7f1cca10087cd381068ee443a51f25cefa45e36ee`  
		Last Modified: Wed, 04 Oct 2023 23:00:27 GMT  
		Size: 34.2 KB (34194 bytes)  
		MIME: application/vnd.in-toto+json

### `mysql:8.0-oracle` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:cea62ed306c9e2a96a3d8672381cdff326fd90123d284ef4852153c0a877835b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.1 MB (170129736 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01c3aea4e3deeec5a6139350e9c1bc1f108fbfdbeb136054e77ef4669e4ae1f7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 20 Jul 2023 22:15:44 GMT
ADD file:b51d9ae1b78eb07ac424bfa71c45180e09ea3a5ed18fbfbcf881fb540bf83e9a in / 
# Thu, 20 Jul 2023 22:15:44 GMT
CMD ["/bin/bash"]
# Thu, 20 Jul 2023 22:15:44 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql # buildkit
# Thu, 20 Jul 2023 22:15:44 GMT
ENV GOSU_VERSION=1.16
# Thu, 20 Jul 2023 22:15:44 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Thu, 20 Jul 2023 22:15:44 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all # buildkit
# Thu, 20 Jul 2023 22:15:44 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME" # buildkit
# Thu, 20 Jul 2023 22:15:44 GMT
ENV MYSQL_MAJOR=8.0
# Thu, 20 Jul 2023 22:15:44 GMT
ENV MYSQL_VERSION=8.0.34-1.el8
# Thu, 20 Jul 2023 22:15:44 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo # buildkit
# Thu, 20 Jul 2023 22:15:44 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version # buildkit
# Thu, 20 Jul 2023 22:15:44 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo # buildkit
# Thu, 20 Jul 2023 22:15:44 GMT
ENV MYSQL_SHELL_VERSION=8.0.34-1.el8
# Thu, 20 Jul 2023 22:15:44 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version # buildkit
# Thu, 20 Jul 2023 22:15:44 GMT
VOLUME [/var/lib/mysql]
# Thu, 20 Jul 2023 22:15:44 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 20 Jul 2023 22:15:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Thu, 20 Jul 2023 22:15:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 20 Jul 2023 22:15:44 GMT
EXPOSE map[3306/tcp:{} 33060/tcp:{}]
# Thu, 20 Jul 2023 22:15:44 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:89ec84aa94fe6a62fb4e9f51aced09dea3cc4d7979c9f0ebd6b5bd4fd729e04e`  
		Last Modified: Thu, 12 Oct 2023 11:01:48 GMT  
		Size: 43.7 MB (43669807 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2047d0a85fcf9107bca7c22f98448ccf140ceed34e3b161beeb4904344032ab7`  
		Last Modified: Thu, 12 Oct 2023 20:57:52 GMT  
		Size: 884.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a981666a88bb712c4283e2a0a14f7ab9b27ff60bfc893fba647a0dbfaa93f6d0`  
		Last Modified: Thu, 12 Oct 2023 20:57:52 GMT  
		Size: 913.0 KB (912965 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7aa9dbd754432215cdd312410444c1c3859b4196dc771c13eba5a56682bef8dc`  
		Last Modified: Thu, 12 Oct 2023 20:57:52 GMT  
		Size: 4.3 MB (4303472 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b8ed90386e32a0124cf2dbca9de0ca31cd5f666b339a7e9a63dae44ed117e587`  
		Last Modified: Thu, 12 Oct 2023 20:57:53 GMT  
		Size: 2.6 KB (2609 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:acf89d2c4916c1368bf3a4c6fb20a4441ec8cd4a3d57bdb015e9277b17286a03`  
		Last Modified: Thu, 12 Oct 2023 20:59:37 GMT  
		Size: 334.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:79120d0882796ce1ccdabc2e93d363faa3227c0773f4dccdad561aab2814f783`  
		Last Modified: Thu, 12 Oct 2023 20:59:41 GMT  
		Size: 57.5 MB (57461596 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c2d0fac447c9eae2f0323e6dedbe3131b2f651c46d5c52ee869f8d2e028a6c0e`  
		Last Modified: Thu, 12 Oct 2023 20:59:37 GMT  
		Size: 316.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6095297ac0a99514ffaa4f43e03709f12a64bce3301266c6324beabac8608835`  
		Last Modified: Thu, 12 Oct 2023 20:59:42 GMT  
		Size: 63.8 MB (63772242 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e274f5c921d7f5b78607112364fe96697bb43f6d9af8e38152c9d06b8cb0c9c9`  
		Last Modified: Thu, 12 Oct 2023 20:59:38 GMT  
		Size: 5.4 KB (5391 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:969873ad404751d35993621a462d3350aeb15f63238fc5930bd78d177d52db66`  
		Last Modified: Thu, 12 Oct 2023 20:59:39 GMT  
		Size: 120.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:8.0-oracle` - unknown; unknown

```console
$ docker pull mysql@sha256:3bc988bea23d6f5fd6693b7be9a8da8ace0346c8150ebe4bb0ea4e75cea797cb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.1 MB (13138887 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:857f42418489e182abc8b171c9c5048be74e446e9448248ec9e30443bdfb6aa9`

```dockerfile
```

-	Layers:
	-	`sha256:243dd07e28b64dcf4c34487ff9d905b095c9774305c321224a45370ccdeea70b`  
		Last Modified: Thu, 12 Oct 2023 20:59:39 GMT  
		Size: 13.1 MB (13104850 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:36467b2da21cc688d8b4728c2e497669d084b9212de6b061103a4c13b82a64d5`  
		Last Modified: Thu, 12 Oct 2023 20:59:37 GMT  
		Size: 34.0 KB (34037 bytes)  
		MIME: application/vnd.in-toto+json

## `mysql:8.0.34`

```console
$ docker pull mysql@sha256:d69594a49f14c02df7eee5b265509e1fb131b1e9e1e54bee932c93051c010576
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `mysql:8.0.34` - linux; amd64

```console
$ docker pull mysql@sha256:0813cfe2d80467f39323b14c13ddbd25d57f56b051f4f1434e10a741f26fce05
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **166.6 MB (166593320 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82ebbd05b8a93f1c4a97ea6d89f3bd577a2e2330ad815a8dc967a383b83e7a36`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 20 Jul 2023 22:15:44 GMT
ADD file:909c07f3bad92a80d3917d583769a01bf62c2cbf3dd24f450fb303b1db92a83e in / 
# Thu, 20 Jul 2023 22:15:44 GMT
CMD ["/bin/bash"]
# Thu, 20 Jul 2023 22:15:44 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql # buildkit
# Thu, 20 Jul 2023 22:15:44 GMT
ENV GOSU_VERSION=1.16
# Thu, 20 Jul 2023 22:15:44 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Thu, 20 Jul 2023 22:15:44 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all # buildkit
# Thu, 20 Jul 2023 22:15:44 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME" # buildkit
# Thu, 20 Jul 2023 22:15:44 GMT
ENV MYSQL_MAJOR=8.0
# Thu, 20 Jul 2023 22:15:44 GMT
ENV MYSQL_VERSION=8.0.34-1.el8
# Thu, 20 Jul 2023 22:15:44 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo # buildkit
# Thu, 20 Jul 2023 22:15:44 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version # buildkit
# Thu, 20 Jul 2023 22:15:44 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo # buildkit
# Thu, 20 Jul 2023 22:15:44 GMT
ENV MYSQL_SHELL_VERSION=8.0.34-1.el8
# Thu, 20 Jul 2023 22:15:44 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version # buildkit
# Thu, 20 Jul 2023 22:15:44 GMT
VOLUME [/var/lib/mysql]
# Thu, 20 Jul 2023 22:15:44 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 20 Jul 2023 22:15:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Thu, 20 Jul 2023 22:15:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 20 Jul 2023 22:15:44 GMT
EXPOSE map[3306/tcp:{} 33060/tcp:{}]
# Thu, 20 Jul 2023 22:15:44 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:5262579e8e45cb87fdc8fb6182d30da3c9e4f1036e02223508f287899ea434c0`  
		Last Modified: Thu, 21 Sep 2023 23:25:18 GMT  
		Size: 45.0 MB (44959147 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c6f87bacd0dd48614ce31c95a5a76f58b1e17d8ceb0646a7cf0335d90baab73a`  
		Last Modified: Wed, 04 Oct 2023 23:00:27 GMT  
		Size: 885.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:581ee7db3e6539c1487c7299b747b063264033fde750dc1e1b36fb6c91a6d464`  
		Last Modified: Wed, 04 Oct 2023 23:00:27 GMT  
		Size: 982.8 KB (982804 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6d5c555a4100d6aeb3f92f990c72e9d32ffe30a355514a7ea5837c9a25192469`  
		Last Modified: Wed, 04 Oct 2023 23:00:28 GMT  
		Size: 4.6 MB (4616288 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:51f4afa7a279674cb5f4caa704105e4075b72efe0433c19776b2add99b59db66`  
		Last Modified: Wed, 04 Oct 2023 23:00:27 GMT  
		Size: 2.6 KB (2609 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d9e414f0b7c63dca45882245d6db287a6389f7f6efa747d3b305d86061754531`  
		Last Modified: Wed, 04 Oct 2023 23:00:28 GMT  
		Size: 332.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:aab3a444c469d72844d9607f27c890e4cb85d6751258bbbd81d5b054994159cf`  
		Last Modified: Wed, 04 Oct 2023 23:00:32 GMT  
		Size: 58.5 MB (58504954 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:aab51168fe3adf75d6483923d31c0774e50df598dc12d918655721b79b506d53`  
		Last Modified: Wed, 04 Oct 2023 23:00:29 GMT  
		Size: 315.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2a63757e7c9cf1e09fdc5c53f2de48cfd45a36e7a461907a3a63a6ebb85d3b4b`  
		Last Modified: Wed, 04 Oct 2023 23:00:32 GMT  
		Size: 57.5 MB (57520476 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:830e4b0cc0bc97158e46ff390f7d92c8967d38898bd4db483486d43ef76eeaba`  
		Last Modified: Wed, 04 Oct 2023 23:00:29 GMT  
		Size: 5.4 KB (5389 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cc0cd1f61ed72c4ad76bb8f7e6cf5156a5c602aea6d3157120a075eb86aa197d`  
		Last Modified: Wed, 04 Oct 2023 23:00:30 GMT  
		Size: 121.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:8.0.34` - unknown; unknown

```console
$ docker pull mysql@sha256:e6ae739fba80627190a3c51e20d0accb8d7d869dd591dfe1d5583a2aea571999
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.1 MB (13140061 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e22c57b768cdd0e2d048d4fcce33a660a75af3a4d046066bbef5cb5742116ff9`

```dockerfile
```

-	Layers:
	-	`sha256:64288b670e6f8145940a7536a8228eb4756812dda4a5395e645186c59582d34b`  
		Last Modified: Wed, 04 Oct 2023 23:00:28 GMT  
		Size: 13.1 MB (13105867 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:bbb01f0ecc5a33972b0e55c7f1cca10087cd381068ee443a51f25cefa45e36ee`  
		Last Modified: Wed, 04 Oct 2023 23:00:27 GMT  
		Size: 34.2 KB (34194 bytes)  
		MIME: application/vnd.in-toto+json

### `mysql:8.0.34` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:cea62ed306c9e2a96a3d8672381cdff326fd90123d284ef4852153c0a877835b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.1 MB (170129736 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01c3aea4e3deeec5a6139350e9c1bc1f108fbfdbeb136054e77ef4669e4ae1f7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 20 Jul 2023 22:15:44 GMT
ADD file:b51d9ae1b78eb07ac424bfa71c45180e09ea3a5ed18fbfbcf881fb540bf83e9a in / 
# Thu, 20 Jul 2023 22:15:44 GMT
CMD ["/bin/bash"]
# Thu, 20 Jul 2023 22:15:44 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql # buildkit
# Thu, 20 Jul 2023 22:15:44 GMT
ENV GOSU_VERSION=1.16
# Thu, 20 Jul 2023 22:15:44 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Thu, 20 Jul 2023 22:15:44 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all # buildkit
# Thu, 20 Jul 2023 22:15:44 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME" # buildkit
# Thu, 20 Jul 2023 22:15:44 GMT
ENV MYSQL_MAJOR=8.0
# Thu, 20 Jul 2023 22:15:44 GMT
ENV MYSQL_VERSION=8.0.34-1.el8
# Thu, 20 Jul 2023 22:15:44 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo # buildkit
# Thu, 20 Jul 2023 22:15:44 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version # buildkit
# Thu, 20 Jul 2023 22:15:44 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo # buildkit
# Thu, 20 Jul 2023 22:15:44 GMT
ENV MYSQL_SHELL_VERSION=8.0.34-1.el8
# Thu, 20 Jul 2023 22:15:44 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version # buildkit
# Thu, 20 Jul 2023 22:15:44 GMT
VOLUME [/var/lib/mysql]
# Thu, 20 Jul 2023 22:15:44 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 20 Jul 2023 22:15:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Thu, 20 Jul 2023 22:15:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 20 Jul 2023 22:15:44 GMT
EXPOSE map[3306/tcp:{} 33060/tcp:{}]
# Thu, 20 Jul 2023 22:15:44 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:89ec84aa94fe6a62fb4e9f51aced09dea3cc4d7979c9f0ebd6b5bd4fd729e04e`  
		Last Modified: Thu, 12 Oct 2023 11:01:48 GMT  
		Size: 43.7 MB (43669807 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2047d0a85fcf9107bca7c22f98448ccf140ceed34e3b161beeb4904344032ab7`  
		Last Modified: Thu, 12 Oct 2023 20:57:52 GMT  
		Size: 884.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a981666a88bb712c4283e2a0a14f7ab9b27ff60bfc893fba647a0dbfaa93f6d0`  
		Last Modified: Thu, 12 Oct 2023 20:57:52 GMT  
		Size: 913.0 KB (912965 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7aa9dbd754432215cdd312410444c1c3859b4196dc771c13eba5a56682bef8dc`  
		Last Modified: Thu, 12 Oct 2023 20:57:52 GMT  
		Size: 4.3 MB (4303472 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b8ed90386e32a0124cf2dbca9de0ca31cd5f666b339a7e9a63dae44ed117e587`  
		Last Modified: Thu, 12 Oct 2023 20:57:53 GMT  
		Size: 2.6 KB (2609 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:acf89d2c4916c1368bf3a4c6fb20a4441ec8cd4a3d57bdb015e9277b17286a03`  
		Last Modified: Thu, 12 Oct 2023 20:59:37 GMT  
		Size: 334.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:79120d0882796ce1ccdabc2e93d363faa3227c0773f4dccdad561aab2814f783`  
		Last Modified: Thu, 12 Oct 2023 20:59:41 GMT  
		Size: 57.5 MB (57461596 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c2d0fac447c9eae2f0323e6dedbe3131b2f651c46d5c52ee869f8d2e028a6c0e`  
		Last Modified: Thu, 12 Oct 2023 20:59:37 GMT  
		Size: 316.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6095297ac0a99514ffaa4f43e03709f12a64bce3301266c6324beabac8608835`  
		Last Modified: Thu, 12 Oct 2023 20:59:42 GMT  
		Size: 63.8 MB (63772242 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e274f5c921d7f5b78607112364fe96697bb43f6d9af8e38152c9d06b8cb0c9c9`  
		Last Modified: Thu, 12 Oct 2023 20:59:38 GMT  
		Size: 5.4 KB (5391 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:969873ad404751d35993621a462d3350aeb15f63238fc5930bd78d177d52db66`  
		Last Modified: Thu, 12 Oct 2023 20:59:39 GMT  
		Size: 120.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:8.0.34` - unknown; unknown

```console
$ docker pull mysql@sha256:3bc988bea23d6f5fd6693b7be9a8da8ace0346c8150ebe4bb0ea4e75cea797cb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.1 MB (13138887 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:857f42418489e182abc8b171c9c5048be74e446e9448248ec9e30443bdfb6aa9`

```dockerfile
```

-	Layers:
	-	`sha256:243dd07e28b64dcf4c34487ff9d905b095c9774305c321224a45370ccdeea70b`  
		Last Modified: Thu, 12 Oct 2023 20:59:39 GMT  
		Size: 13.1 MB (13104850 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:36467b2da21cc688d8b4728c2e497669d084b9212de6b061103a4c13b82a64d5`  
		Last Modified: Thu, 12 Oct 2023 20:59:37 GMT  
		Size: 34.0 KB (34037 bytes)  
		MIME: application/vnd.in-toto+json

## `mysql:8.0.34-debian`

```console
$ docker pull mysql@sha256:2a31847951cdf92d6901ef58b4c5a9fbe75b47823d9ade1f7a4652ede7a88e2d
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 2
	-	linux; amd64
	-	unknown; unknown

### `mysql:8.0.34-debian` - linux; amd64

```console
$ docker pull mysql@sha256:e10fb73841ef30dcdb02e0759035f7730e5303cdc455268de219407d3fb4b846
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **179.1 MB (179083456 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc21a4e132a7e63c4a4eca71b3e75fbc7e965aef2b157a60a9c322e41e592795`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 20 Jul 2023 22:15:44 GMT
ADD file:cb13581b8e7a9de4396639e5ca2f3817763435c0563232f85e3d899f6388a1b3 in / 
# Thu, 20 Jul 2023 22:15:44 GMT
CMD ["bash"]
# Thu, 20 Jul 2023 22:15:44 GMT
RUN groupadd -r mysql && useradd -r -g mysql mysql # buildkit
# Thu, 20 Jul 2023 22:15:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends gnupg && rm -rf /var/lib/apt/lists/* # buildkit
# Thu, 20 Jul 2023 22:15:44 GMT
ENV GOSU_VERSION=1.16
# Thu, 20 Jul 2023 22:15:44 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Thu, 20 Jul 2023 22:15:44 GMT
RUN mkdir /docker-entrypoint-initdb.d # buildkit
# Thu, 20 Jul 2023 22:15:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		openssl 		perl 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Thu, 20 Jul 2023 22:15:44 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$key" > /etc/apt/keyrings/mysql.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" # buildkit
# Thu, 20 Jul 2023 22:15:44 GMT
ENV MYSQL_MAJOR=8.0
# Thu, 20 Jul 2023 22:15:44 GMT
ENV MYSQL_VERSION=8.0.34-1debian11
# Thu, 20 Jul 2023 22:15:44 GMT
RUN echo 'deb [ signed-by=/etc/apt/keyrings/mysql.gpg ] http://repo.mysql.com/apt/debian/ bullseye mysql-8.0' > /etc/apt/sources.list.d/mysql.list # buildkit
# Thu, 20 Jul 2023 22:15:44 GMT
RUN { 		echo mysql-community-server mysql-community-server/data-dir select ''; 		echo mysql-community-server mysql-community-server/root-pass password ''; 		echo mysql-community-server mysql-community-server/re-root-pass password ''; 		echo mysql-community-server mysql-community-server/remove-test-db select false; 	} | debconf-set-selections 	&& apt-get update 	&& apt-get install -y 		mysql-community-client="${MYSQL_VERSION}" 		mysql-community-server-core="${MYSQL_VERSION}" 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mysql && mkdir -p /var/lib/mysql /var/run/mysqld 	&& chown -R mysql:mysql /var/lib/mysql /var/run/mysqld 	&& chmod 1777 /var/run/mysqld /var/lib/mysql # buildkit
# Thu, 20 Jul 2023 22:15:44 GMT
VOLUME [/var/lib/mysql]
# Thu, 20 Jul 2023 22:15:44 GMT
COPY config/ /etc/mysql/ # buildkit
# Thu, 20 Jul 2023 22:15:44 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 20 Jul 2023 22:15:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Thu, 20 Jul 2023 22:15:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 20 Jul 2023 22:15:44 GMT
EXPOSE map[3306/tcp:{} 33060/tcp:{}]
# Thu, 20 Jul 2023 22:15:44 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:e67fdae3559346105027c63e7fb032bba57e62b1fe9f2da23e6fdfb56384e00b`  
		Last Modified: Wed, 11 Oct 2023 18:40:17 GMT  
		Size: 31.4 MB (31417862 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cf330228e741604571f4caab61f2cc172717b89147d1238d45d057fb46edb697`  
		Last Modified: Wed, 11 Oct 2023 20:03:39 GMT  
		Size: 1.6 KB (1646 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bafbe13d22f4d4ef6ed406ac05b335dc1371424f95a2beafc66051e6cb3974bf`  
		Last Modified: Wed, 11 Oct 2023 20:03:40 GMT  
		Size: 4.2 MB (4207542 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d8dcfd9f33b298cff0fc2ee7fd95dbd76a738414a4269d51121ef718fbcbf87b`  
		Last Modified: Wed, 11 Oct 2023 20:03:39 GMT  
		Size: 1.5 MB (1472483 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:21ae14d9c3e441351e1ec5b465e6bf617e393bc4a0ad072589600a2b8ae73b37`  
		Last Modified: Wed, 11 Oct 2023 20:03:39 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1086d8d2521ba8f681003c1bb0594f31379d599a291c6646085f007fe8f395a1`  
		Last Modified: Wed, 11 Oct 2023 20:03:41 GMT  
		Size: 12.5 MB (12455173 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:16afe97457504eb7005a224c7c679006bb937483986e5365633519004752f789`  
		Last Modified: Wed, 11 Oct 2023 20:03:40 GMT  
		Size: 2.5 KB (2497 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8169ee2bdb0a81c638c5dfb7aeef3c7c5b17755771f95a889cfe4c29b26e4966`  
		Last Modified: Wed, 11 Oct 2023 20:03:41 GMT  
		Size: 248.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8fdc0f64b1cbafeb07f2c175c0486123720ed151cdd007b251816564e4381d23`  
		Last Modified: Wed, 11 Oct 2023 20:03:47 GMT  
		Size: 129.5 MB (129519547 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3994da0db6238691c6a2208c2da4b3dafb961db6ca184feedab3435104154f4d`  
		Last Modified: Wed, 11 Oct 2023 20:03:41 GMT  
		Size: 837.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ae385311e5ed3100ff6111e185211d9a5749c784bd675d0ba713898acb9dafd8`  
		Last Modified: Wed, 11 Oct 2023 20:03:42 GMT  
		Size: 5.4 KB (5383 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e2ceafee559334b9217ef6cde4d657abe3fb79466a7ef1b5e6f911d185b689f6`  
		Last Modified: Wed, 11 Oct 2023 20:03:42 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:8.0.34-debian` - unknown; unknown

```console
$ docker pull mysql@sha256:2831145c9d8abb4571f51bd89b331516c37b2b0421ec56d2647082e631ce3d7c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.5 MB (3484026 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95857c88929774216f8e99858617023ea09d821927280ca85a5fbfdc8a6a609a`

```dockerfile
```

-	Layers:
	-	`sha256:d6cded17556303c4d1affc0cc57b7ae8b5fdce8a01462b0b5bf4608e0e7a413d`  
		Last Modified: Wed, 11 Oct 2023 20:03:39 GMT  
		Size: 3.5 MB (3450737 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:29553eed5402c121dca04ea081b05fbfc44820c10ddb43cc09308bc0051fd6c1`  
		Last Modified: Wed, 11 Oct 2023 20:03:39 GMT  
		Size: 33.3 KB (33289 bytes)  
		MIME: application/vnd.in-toto+json

## `mysql:8.0.34-oracle`

```console
$ docker pull mysql@sha256:d69594a49f14c02df7eee5b265509e1fb131b1e9e1e54bee932c93051c010576
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `mysql:8.0.34-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:0813cfe2d80467f39323b14c13ddbd25d57f56b051f4f1434e10a741f26fce05
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **166.6 MB (166593320 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82ebbd05b8a93f1c4a97ea6d89f3bd577a2e2330ad815a8dc967a383b83e7a36`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 20 Jul 2023 22:15:44 GMT
ADD file:909c07f3bad92a80d3917d583769a01bf62c2cbf3dd24f450fb303b1db92a83e in / 
# Thu, 20 Jul 2023 22:15:44 GMT
CMD ["/bin/bash"]
# Thu, 20 Jul 2023 22:15:44 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql # buildkit
# Thu, 20 Jul 2023 22:15:44 GMT
ENV GOSU_VERSION=1.16
# Thu, 20 Jul 2023 22:15:44 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Thu, 20 Jul 2023 22:15:44 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all # buildkit
# Thu, 20 Jul 2023 22:15:44 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME" # buildkit
# Thu, 20 Jul 2023 22:15:44 GMT
ENV MYSQL_MAJOR=8.0
# Thu, 20 Jul 2023 22:15:44 GMT
ENV MYSQL_VERSION=8.0.34-1.el8
# Thu, 20 Jul 2023 22:15:44 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo # buildkit
# Thu, 20 Jul 2023 22:15:44 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version # buildkit
# Thu, 20 Jul 2023 22:15:44 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo # buildkit
# Thu, 20 Jul 2023 22:15:44 GMT
ENV MYSQL_SHELL_VERSION=8.0.34-1.el8
# Thu, 20 Jul 2023 22:15:44 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version # buildkit
# Thu, 20 Jul 2023 22:15:44 GMT
VOLUME [/var/lib/mysql]
# Thu, 20 Jul 2023 22:15:44 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 20 Jul 2023 22:15:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Thu, 20 Jul 2023 22:15:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 20 Jul 2023 22:15:44 GMT
EXPOSE map[3306/tcp:{} 33060/tcp:{}]
# Thu, 20 Jul 2023 22:15:44 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:5262579e8e45cb87fdc8fb6182d30da3c9e4f1036e02223508f287899ea434c0`  
		Last Modified: Thu, 21 Sep 2023 23:25:18 GMT  
		Size: 45.0 MB (44959147 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c6f87bacd0dd48614ce31c95a5a76f58b1e17d8ceb0646a7cf0335d90baab73a`  
		Last Modified: Wed, 04 Oct 2023 23:00:27 GMT  
		Size: 885.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:581ee7db3e6539c1487c7299b747b063264033fde750dc1e1b36fb6c91a6d464`  
		Last Modified: Wed, 04 Oct 2023 23:00:27 GMT  
		Size: 982.8 KB (982804 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6d5c555a4100d6aeb3f92f990c72e9d32ffe30a355514a7ea5837c9a25192469`  
		Last Modified: Wed, 04 Oct 2023 23:00:28 GMT  
		Size: 4.6 MB (4616288 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:51f4afa7a279674cb5f4caa704105e4075b72efe0433c19776b2add99b59db66`  
		Last Modified: Wed, 04 Oct 2023 23:00:27 GMT  
		Size: 2.6 KB (2609 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d9e414f0b7c63dca45882245d6db287a6389f7f6efa747d3b305d86061754531`  
		Last Modified: Wed, 04 Oct 2023 23:00:28 GMT  
		Size: 332.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:aab3a444c469d72844d9607f27c890e4cb85d6751258bbbd81d5b054994159cf`  
		Last Modified: Wed, 04 Oct 2023 23:00:32 GMT  
		Size: 58.5 MB (58504954 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:aab51168fe3adf75d6483923d31c0774e50df598dc12d918655721b79b506d53`  
		Last Modified: Wed, 04 Oct 2023 23:00:29 GMT  
		Size: 315.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2a63757e7c9cf1e09fdc5c53f2de48cfd45a36e7a461907a3a63a6ebb85d3b4b`  
		Last Modified: Wed, 04 Oct 2023 23:00:32 GMT  
		Size: 57.5 MB (57520476 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:830e4b0cc0bc97158e46ff390f7d92c8967d38898bd4db483486d43ef76eeaba`  
		Last Modified: Wed, 04 Oct 2023 23:00:29 GMT  
		Size: 5.4 KB (5389 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cc0cd1f61ed72c4ad76bb8f7e6cf5156a5c602aea6d3157120a075eb86aa197d`  
		Last Modified: Wed, 04 Oct 2023 23:00:30 GMT  
		Size: 121.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:8.0.34-oracle` - unknown; unknown

```console
$ docker pull mysql@sha256:e6ae739fba80627190a3c51e20d0accb8d7d869dd591dfe1d5583a2aea571999
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.1 MB (13140061 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e22c57b768cdd0e2d048d4fcce33a660a75af3a4d046066bbef5cb5742116ff9`

```dockerfile
```

-	Layers:
	-	`sha256:64288b670e6f8145940a7536a8228eb4756812dda4a5395e645186c59582d34b`  
		Last Modified: Wed, 04 Oct 2023 23:00:28 GMT  
		Size: 13.1 MB (13105867 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:bbb01f0ecc5a33972b0e55c7f1cca10087cd381068ee443a51f25cefa45e36ee`  
		Last Modified: Wed, 04 Oct 2023 23:00:27 GMT  
		Size: 34.2 KB (34194 bytes)  
		MIME: application/vnd.in-toto+json

### `mysql:8.0.34-oracle` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:cea62ed306c9e2a96a3d8672381cdff326fd90123d284ef4852153c0a877835b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.1 MB (170129736 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01c3aea4e3deeec5a6139350e9c1bc1f108fbfdbeb136054e77ef4669e4ae1f7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 20 Jul 2023 22:15:44 GMT
ADD file:b51d9ae1b78eb07ac424bfa71c45180e09ea3a5ed18fbfbcf881fb540bf83e9a in / 
# Thu, 20 Jul 2023 22:15:44 GMT
CMD ["/bin/bash"]
# Thu, 20 Jul 2023 22:15:44 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql # buildkit
# Thu, 20 Jul 2023 22:15:44 GMT
ENV GOSU_VERSION=1.16
# Thu, 20 Jul 2023 22:15:44 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Thu, 20 Jul 2023 22:15:44 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all # buildkit
# Thu, 20 Jul 2023 22:15:44 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME" # buildkit
# Thu, 20 Jul 2023 22:15:44 GMT
ENV MYSQL_MAJOR=8.0
# Thu, 20 Jul 2023 22:15:44 GMT
ENV MYSQL_VERSION=8.0.34-1.el8
# Thu, 20 Jul 2023 22:15:44 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql8.0-server-minimal]'; 		echo 'name=MySQL 8.0 Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-8.0-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo # buildkit
# Thu, 20 Jul 2023 22:15:44 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version # buildkit
# Thu, 20 Jul 2023 22:15:44 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo # buildkit
# Thu, 20 Jul 2023 22:15:44 GMT
ENV MYSQL_SHELL_VERSION=8.0.34-1.el8
# Thu, 20 Jul 2023 22:15:44 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version # buildkit
# Thu, 20 Jul 2023 22:15:44 GMT
VOLUME [/var/lib/mysql]
# Thu, 20 Jul 2023 22:15:44 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 20 Jul 2023 22:15:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Thu, 20 Jul 2023 22:15:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 20 Jul 2023 22:15:44 GMT
EXPOSE map[3306/tcp:{} 33060/tcp:{}]
# Thu, 20 Jul 2023 22:15:44 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:89ec84aa94fe6a62fb4e9f51aced09dea3cc4d7979c9f0ebd6b5bd4fd729e04e`  
		Last Modified: Thu, 12 Oct 2023 11:01:48 GMT  
		Size: 43.7 MB (43669807 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2047d0a85fcf9107bca7c22f98448ccf140ceed34e3b161beeb4904344032ab7`  
		Last Modified: Thu, 12 Oct 2023 20:57:52 GMT  
		Size: 884.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a981666a88bb712c4283e2a0a14f7ab9b27ff60bfc893fba647a0dbfaa93f6d0`  
		Last Modified: Thu, 12 Oct 2023 20:57:52 GMT  
		Size: 913.0 KB (912965 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7aa9dbd754432215cdd312410444c1c3859b4196dc771c13eba5a56682bef8dc`  
		Last Modified: Thu, 12 Oct 2023 20:57:52 GMT  
		Size: 4.3 MB (4303472 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b8ed90386e32a0124cf2dbca9de0ca31cd5f666b339a7e9a63dae44ed117e587`  
		Last Modified: Thu, 12 Oct 2023 20:57:53 GMT  
		Size: 2.6 KB (2609 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:acf89d2c4916c1368bf3a4c6fb20a4441ec8cd4a3d57bdb015e9277b17286a03`  
		Last Modified: Thu, 12 Oct 2023 20:59:37 GMT  
		Size: 334.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:79120d0882796ce1ccdabc2e93d363faa3227c0773f4dccdad561aab2814f783`  
		Last Modified: Thu, 12 Oct 2023 20:59:41 GMT  
		Size: 57.5 MB (57461596 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c2d0fac447c9eae2f0323e6dedbe3131b2f651c46d5c52ee869f8d2e028a6c0e`  
		Last Modified: Thu, 12 Oct 2023 20:59:37 GMT  
		Size: 316.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6095297ac0a99514ffaa4f43e03709f12a64bce3301266c6324beabac8608835`  
		Last Modified: Thu, 12 Oct 2023 20:59:42 GMT  
		Size: 63.8 MB (63772242 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e274f5c921d7f5b78607112364fe96697bb43f6d9af8e38152c9d06b8cb0c9c9`  
		Last Modified: Thu, 12 Oct 2023 20:59:38 GMT  
		Size: 5.4 KB (5391 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:969873ad404751d35993621a462d3350aeb15f63238fc5930bd78d177d52db66`  
		Last Modified: Thu, 12 Oct 2023 20:59:39 GMT  
		Size: 120.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:8.0.34-oracle` - unknown; unknown

```console
$ docker pull mysql@sha256:3bc988bea23d6f5fd6693b7be9a8da8ace0346c8150ebe4bb0ea4e75cea797cb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.1 MB (13138887 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:857f42418489e182abc8b171c9c5048be74e446e9448248ec9e30443bdfb6aa9`

```dockerfile
```

-	Layers:
	-	`sha256:243dd07e28b64dcf4c34487ff9d905b095c9774305c321224a45370ccdeea70b`  
		Last Modified: Thu, 12 Oct 2023 20:59:39 GMT  
		Size: 13.1 MB (13104850 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:36467b2da21cc688d8b4728c2e497669d084b9212de6b061103a4c13b82a64d5`  
		Last Modified: Thu, 12 Oct 2023 20:59:37 GMT  
		Size: 34.0 KB (34037 bytes)  
		MIME: application/vnd.in-toto+json

## `mysql:8.1`

```console
$ docker pull mysql@sha256:9592f7dad3d285b9d2f89b1e9a586dbed983deb72ec190ba7d6af12120781d2e
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `mysql:8.1` - linux; amd64

```console
$ docker pull mysql@sha256:5253d1662109ba7776430522fd73bd37f1c5775235eec63883fb8294d22757bc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **166.9 MB (166863356 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c138801544a941ed9d1171794e3361533109aa7e22f2ea4e1ba85bccc84f6842`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 27 Jul 2023 22:18:51 GMT
ADD file:909c07f3bad92a80d3917d583769a01bf62c2cbf3dd24f450fb303b1db92a83e in / 
# Thu, 27 Jul 2023 22:18:51 GMT
CMD ["/bin/bash"]
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
ENV GOSU_VERSION=1.16
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME" # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
ENV MYSQL_MAJOR=innovation
# Thu, 27 Jul 2023 22:18:51 GMT
ENV MYSQL_VERSION=8.1.0-1.el8
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysqlinnovation-server-minimal]'; 		echo 'name=MySQL innovation Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-innovation-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
ENV MYSQL_SHELL_VERSION=8.0.34-1.el8
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
VOLUME [/var/lib/mysql]
# Thu, 27 Jul 2023 22:18:51 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 27 Jul 2023 22:18:51 GMT
EXPOSE map[3306/tcp:{} 33060/tcp:{}]
# Thu, 27 Jul 2023 22:18:51 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:5262579e8e45cb87fdc8fb6182d30da3c9e4f1036e02223508f287899ea434c0`  
		Last Modified: Thu, 21 Sep 2023 23:25:18 GMT  
		Size: 45.0 MB (44959147 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bfcc921068b5eaba8d310a26395ee4139cd54b21ec96369a39830e24cfe84477`  
		Last Modified: Wed, 04 Oct 2023 23:00:11 GMT  
		Size: 885.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:072a02315ab18d41372cf2e57b066a8ecf9954ab8d94cb5244ca20efe63df7ab`  
		Last Modified: Wed, 04 Oct 2023 23:00:11 GMT  
		Size: 982.8 KB (982808 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:711d47be56b4655b6deec62a811cddf52424477672f5930441ae8701ab012c95`  
		Last Modified: Wed, 04 Oct 2023 23:00:12 GMT  
		Size: 4.6 MB (4616305 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:755e67622a77c61bb6eb442164103b5395e7db380add9d61a2acb3425df65fa0`  
		Last Modified: Wed, 04 Oct 2023 23:00:12 GMT  
		Size: 2.6 KB (2608 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0080a11112d165a07d366db3a1ebd57709f066f4b13f10b57ec21e19d3d67d26`  
		Last Modified: Wed, 04 Oct 2023 23:00:12 GMT  
		Size: 340.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:adc45022a9ad6beda852b49f14ae18ff04ea052eb0f9391c31a29ecdffaa1ef1`  
		Last Modified: Wed, 04 Oct 2023 23:00:17 GMT  
		Size: 58.8 MB (58771345 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:67d8146998603ea2ed92b77bccbb35623a5eb39c6b047d15af930cec9ef79a9d`  
		Last Modified: Wed, 04 Oct 2023 23:00:13 GMT  
		Size: 316.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f431d85cf61e18099acd66976a43fb86be0ca84549a3853b4e2eaeb48557acb8`  
		Last Modified: Wed, 04 Oct 2023 23:00:16 GMT  
		Size: 57.5 MB (57524213 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4bbba6dd5ce26ba0b294a1cc506c8a57566efbaaf3701fe8eb752b54c4bd64c5`  
		Last Modified: Wed, 04 Oct 2023 23:00:14 GMT  
		Size: 5.4 KB (5389 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:8.1` - unknown; unknown

```console
$ docker pull mysql@sha256:3907151ff6c8a3d9a987e42f5af74ec79742398d67673c9e6f3baf067cbff3ab
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.1 MB (13141082 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3992e42cff0b10e86e3648547df8a978c66d19322dd629faa7cdacd2432028c9`

```dockerfile
```

-	Layers:
	-	`sha256:06d7ee16ec055f718e85ab70b205f9a40ac64f1f4bd3665bfd625ceffdce177c`  
		Last Modified: Wed, 04 Oct 2023 23:00:12 GMT  
		Size: 13.1 MB (13107503 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:81f9eeabc6e68920db4c4c28565e7cdbb580ecb31d9205d49fb827e33e860dd3`  
		Last Modified: Wed, 04 Oct 2023 23:00:11 GMT  
		Size: 33.6 KB (33579 bytes)  
		MIME: application/vnd.in-toto+json

### `mysql:8.1` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:8cacf9ef3db6f3e040c4ecde7f897706401d1f8330ca96862744e8b0d5781454
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.4 MB (170371412 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d30a00232fdc87bddbd635dad0486bf2278d705c76af20ec01f0814d0481064f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 27 Jul 2023 22:18:51 GMT
ADD file:b51d9ae1b78eb07ac424bfa71c45180e09ea3a5ed18fbfbcf881fb540bf83e9a in / 
# Thu, 27 Jul 2023 22:18:51 GMT
CMD ["/bin/bash"]
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
ENV GOSU_VERSION=1.16
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME" # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
ENV MYSQL_MAJOR=innovation
# Thu, 27 Jul 2023 22:18:51 GMT
ENV MYSQL_VERSION=8.1.0-1.el8
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysqlinnovation-server-minimal]'; 		echo 'name=MySQL innovation Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-innovation-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
ENV MYSQL_SHELL_VERSION=8.0.34-1.el8
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
VOLUME [/var/lib/mysql]
# Thu, 27 Jul 2023 22:18:51 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 27 Jul 2023 22:18:51 GMT
EXPOSE map[3306/tcp:{} 33060/tcp:{}]
# Thu, 27 Jul 2023 22:18:51 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:89ec84aa94fe6a62fb4e9f51aced09dea3cc4d7979c9f0ebd6b5bd4fd729e04e`  
		Last Modified: Thu, 12 Oct 2023 11:01:48 GMT  
		Size: 43.7 MB (43669807 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2047d0a85fcf9107bca7c22f98448ccf140ceed34e3b161beeb4904344032ab7`  
		Last Modified: Thu, 12 Oct 2023 20:57:52 GMT  
		Size: 884.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a981666a88bb712c4283e2a0a14f7ab9b27ff60bfc893fba647a0dbfaa93f6d0`  
		Last Modified: Thu, 12 Oct 2023 20:57:52 GMT  
		Size: 913.0 KB (912965 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7aa9dbd754432215cdd312410444c1c3859b4196dc771c13eba5a56682bef8dc`  
		Last Modified: Thu, 12 Oct 2023 20:57:52 GMT  
		Size: 4.3 MB (4303472 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b8ed90386e32a0124cf2dbca9de0ca31cd5f666b339a7e9a63dae44ed117e587`  
		Last Modified: Thu, 12 Oct 2023 20:57:53 GMT  
		Size: 2.6 KB (2609 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0b36981941b7e06e20d54a95dc6d483b22da2cb1e1fe68e9a77bcbcd2f55696c`  
		Last Modified: Thu, 12 Oct 2023 20:57:53 GMT  
		Size: 341.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ca996c23fc53d3fd7658d98952a4d481ae66e74585e2b72c55f961bf54455736`  
		Last Modified: Thu, 12 Oct 2023 20:57:57 GMT  
		Size: 57.7 MB (57701851 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:15050e9043e65433ddefd92b793734e91755006d5f756c6a9259998e9ccf916a`  
		Last Modified: Thu, 12 Oct 2023 20:57:54 GMT  
		Size: 316.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3ecfc97ced27490a7dd8db645fba5623698b5a933cb2359aedacf99e2dd74d54`  
		Last Modified: Thu, 12 Oct 2023 20:57:58 GMT  
		Size: 63.8 MB (63773775 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e435e3bf4d77af270e3b5245b5aa6234fcd3bb791ed57db4641d7ef99b33bf18`  
		Last Modified: Thu, 12 Oct 2023 20:57:55 GMT  
		Size: 5.4 KB (5392 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:8.1` - unknown; unknown

```console
$ docker pull mysql@sha256:33f7834b9a596feb3b7660924e45d3886bc1908da500f449c853ace58e7ef70d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.1 MB (13140098 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31013d6e714b5c7d6108fc3965658f4e7d97b6c8aa096f02b8230c4e1ebf99ae`

```dockerfile
```

-	Layers:
	-	`sha256:564dbabf3309a798678bcee0a9ac7f451cacb91050175a2e98f9313a605ae7cd`  
		Last Modified: Thu, 12 Oct 2023 20:57:54 GMT  
		Size: 13.1 MB (13106498 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:18613fc7c61e609bc95ef7402649a9c574fb26d032c9df3aa4e7b3f9b86b70e4`  
		Last Modified: Thu, 12 Oct 2023 20:57:52 GMT  
		Size: 33.6 KB (33600 bytes)  
		MIME: application/vnd.in-toto+json

## `mysql:8.1-oracle`

```console
$ docker pull mysql@sha256:9592f7dad3d285b9d2f89b1e9a586dbed983deb72ec190ba7d6af12120781d2e
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `mysql:8.1-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:5253d1662109ba7776430522fd73bd37f1c5775235eec63883fb8294d22757bc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **166.9 MB (166863356 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c138801544a941ed9d1171794e3361533109aa7e22f2ea4e1ba85bccc84f6842`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 27 Jul 2023 22:18:51 GMT
ADD file:909c07f3bad92a80d3917d583769a01bf62c2cbf3dd24f450fb303b1db92a83e in / 
# Thu, 27 Jul 2023 22:18:51 GMT
CMD ["/bin/bash"]
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
ENV GOSU_VERSION=1.16
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME" # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
ENV MYSQL_MAJOR=innovation
# Thu, 27 Jul 2023 22:18:51 GMT
ENV MYSQL_VERSION=8.1.0-1.el8
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysqlinnovation-server-minimal]'; 		echo 'name=MySQL innovation Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-innovation-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
ENV MYSQL_SHELL_VERSION=8.0.34-1.el8
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
VOLUME [/var/lib/mysql]
# Thu, 27 Jul 2023 22:18:51 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 27 Jul 2023 22:18:51 GMT
EXPOSE map[3306/tcp:{} 33060/tcp:{}]
# Thu, 27 Jul 2023 22:18:51 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:5262579e8e45cb87fdc8fb6182d30da3c9e4f1036e02223508f287899ea434c0`  
		Last Modified: Thu, 21 Sep 2023 23:25:18 GMT  
		Size: 45.0 MB (44959147 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bfcc921068b5eaba8d310a26395ee4139cd54b21ec96369a39830e24cfe84477`  
		Last Modified: Wed, 04 Oct 2023 23:00:11 GMT  
		Size: 885.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:072a02315ab18d41372cf2e57b066a8ecf9954ab8d94cb5244ca20efe63df7ab`  
		Last Modified: Wed, 04 Oct 2023 23:00:11 GMT  
		Size: 982.8 KB (982808 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:711d47be56b4655b6deec62a811cddf52424477672f5930441ae8701ab012c95`  
		Last Modified: Wed, 04 Oct 2023 23:00:12 GMT  
		Size: 4.6 MB (4616305 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:755e67622a77c61bb6eb442164103b5395e7db380add9d61a2acb3425df65fa0`  
		Last Modified: Wed, 04 Oct 2023 23:00:12 GMT  
		Size: 2.6 KB (2608 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0080a11112d165a07d366db3a1ebd57709f066f4b13f10b57ec21e19d3d67d26`  
		Last Modified: Wed, 04 Oct 2023 23:00:12 GMT  
		Size: 340.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:adc45022a9ad6beda852b49f14ae18ff04ea052eb0f9391c31a29ecdffaa1ef1`  
		Last Modified: Wed, 04 Oct 2023 23:00:17 GMT  
		Size: 58.8 MB (58771345 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:67d8146998603ea2ed92b77bccbb35623a5eb39c6b047d15af930cec9ef79a9d`  
		Last Modified: Wed, 04 Oct 2023 23:00:13 GMT  
		Size: 316.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f431d85cf61e18099acd66976a43fb86be0ca84549a3853b4e2eaeb48557acb8`  
		Last Modified: Wed, 04 Oct 2023 23:00:16 GMT  
		Size: 57.5 MB (57524213 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4bbba6dd5ce26ba0b294a1cc506c8a57566efbaaf3701fe8eb752b54c4bd64c5`  
		Last Modified: Wed, 04 Oct 2023 23:00:14 GMT  
		Size: 5.4 KB (5389 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:8.1-oracle` - unknown; unknown

```console
$ docker pull mysql@sha256:3907151ff6c8a3d9a987e42f5af74ec79742398d67673c9e6f3baf067cbff3ab
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.1 MB (13141082 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3992e42cff0b10e86e3648547df8a978c66d19322dd629faa7cdacd2432028c9`

```dockerfile
```

-	Layers:
	-	`sha256:06d7ee16ec055f718e85ab70b205f9a40ac64f1f4bd3665bfd625ceffdce177c`  
		Last Modified: Wed, 04 Oct 2023 23:00:12 GMT  
		Size: 13.1 MB (13107503 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:81f9eeabc6e68920db4c4c28565e7cdbb580ecb31d9205d49fb827e33e860dd3`  
		Last Modified: Wed, 04 Oct 2023 23:00:11 GMT  
		Size: 33.6 KB (33579 bytes)  
		MIME: application/vnd.in-toto+json

### `mysql:8.1-oracle` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:8cacf9ef3db6f3e040c4ecde7f897706401d1f8330ca96862744e8b0d5781454
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.4 MB (170371412 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d30a00232fdc87bddbd635dad0486bf2278d705c76af20ec01f0814d0481064f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 27 Jul 2023 22:18:51 GMT
ADD file:b51d9ae1b78eb07ac424bfa71c45180e09ea3a5ed18fbfbcf881fb540bf83e9a in / 
# Thu, 27 Jul 2023 22:18:51 GMT
CMD ["/bin/bash"]
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
ENV GOSU_VERSION=1.16
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME" # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
ENV MYSQL_MAJOR=innovation
# Thu, 27 Jul 2023 22:18:51 GMT
ENV MYSQL_VERSION=8.1.0-1.el8
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysqlinnovation-server-minimal]'; 		echo 'name=MySQL innovation Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-innovation-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
ENV MYSQL_SHELL_VERSION=8.0.34-1.el8
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
VOLUME [/var/lib/mysql]
# Thu, 27 Jul 2023 22:18:51 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 27 Jul 2023 22:18:51 GMT
EXPOSE map[3306/tcp:{} 33060/tcp:{}]
# Thu, 27 Jul 2023 22:18:51 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:89ec84aa94fe6a62fb4e9f51aced09dea3cc4d7979c9f0ebd6b5bd4fd729e04e`  
		Last Modified: Thu, 12 Oct 2023 11:01:48 GMT  
		Size: 43.7 MB (43669807 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2047d0a85fcf9107bca7c22f98448ccf140ceed34e3b161beeb4904344032ab7`  
		Last Modified: Thu, 12 Oct 2023 20:57:52 GMT  
		Size: 884.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a981666a88bb712c4283e2a0a14f7ab9b27ff60bfc893fba647a0dbfaa93f6d0`  
		Last Modified: Thu, 12 Oct 2023 20:57:52 GMT  
		Size: 913.0 KB (912965 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7aa9dbd754432215cdd312410444c1c3859b4196dc771c13eba5a56682bef8dc`  
		Last Modified: Thu, 12 Oct 2023 20:57:52 GMT  
		Size: 4.3 MB (4303472 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b8ed90386e32a0124cf2dbca9de0ca31cd5f666b339a7e9a63dae44ed117e587`  
		Last Modified: Thu, 12 Oct 2023 20:57:53 GMT  
		Size: 2.6 KB (2609 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0b36981941b7e06e20d54a95dc6d483b22da2cb1e1fe68e9a77bcbcd2f55696c`  
		Last Modified: Thu, 12 Oct 2023 20:57:53 GMT  
		Size: 341.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ca996c23fc53d3fd7658d98952a4d481ae66e74585e2b72c55f961bf54455736`  
		Last Modified: Thu, 12 Oct 2023 20:57:57 GMT  
		Size: 57.7 MB (57701851 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:15050e9043e65433ddefd92b793734e91755006d5f756c6a9259998e9ccf916a`  
		Last Modified: Thu, 12 Oct 2023 20:57:54 GMT  
		Size: 316.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3ecfc97ced27490a7dd8db645fba5623698b5a933cb2359aedacf99e2dd74d54`  
		Last Modified: Thu, 12 Oct 2023 20:57:58 GMT  
		Size: 63.8 MB (63773775 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e435e3bf4d77af270e3b5245b5aa6234fcd3bb791ed57db4641d7ef99b33bf18`  
		Last Modified: Thu, 12 Oct 2023 20:57:55 GMT  
		Size: 5.4 KB (5392 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:8.1-oracle` - unknown; unknown

```console
$ docker pull mysql@sha256:33f7834b9a596feb3b7660924e45d3886bc1908da500f449c853ace58e7ef70d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.1 MB (13140098 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31013d6e714b5c7d6108fc3965658f4e7d97b6c8aa096f02b8230c4e1ebf99ae`

```dockerfile
```

-	Layers:
	-	`sha256:564dbabf3309a798678bcee0a9ac7f451cacb91050175a2e98f9313a605ae7cd`  
		Last Modified: Thu, 12 Oct 2023 20:57:54 GMT  
		Size: 13.1 MB (13106498 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:18613fc7c61e609bc95ef7402649a9c574fb26d032c9df3aa4e7b3f9b86b70e4`  
		Last Modified: Thu, 12 Oct 2023 20:57:52 GMT  
		Size: 33.6 KB (33600 bytes)  
		MIME: application/vnd.in-toto+json

## `mysql:8.1.0`

```console
$ docker pull mysql@sha256:9592f7dad3d285b9d2f89b1e9a586dbed983deb72ec190ba7d6af12120781d2e
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `mysql:8.1.0` - linux; amd64

```console
$ docker pull mysql@sha256:5253d1662109ba7776430522fd73bd37f1c5775235eec63883fb8294d22757bc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **166.9 MB (166863356 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c138801544a941ed9d1171794e3361533109aa7e22f2ea4e1ba85bccc84f6842`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 27 Jul 2023 22:18:51 GMT
ADD file:909c07f3bad92a80d3917d583769a01bf62c2cbf3dd24f450fb303b1db92a83e in / 
# Thu, 27 Jul 2023 22:18:51 GMT
CMD ["/bin/bash"]
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
ENV GOSU_VERSION=1.16
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME" # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
ENV MYSQL_MAJOR=innovation
# Thu, 27 Jul 2023 22:18:51 GMT
ENV MYSQL_VERSION=8.1.0-1.el8
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysqlinnovation-server-minimal]'; 		echo 'name=MySQL innovation Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-innovation-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
ENV MYSQL_SHELL_VERSION=8.0.34-1.el8
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
VOLUME [/var/lib/mysql]
# Thu, 27 Jul 2023 22:18:51 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 27 Jul 2023 22:18:51 GMT
EXPOSE map[3306/tcp:{} 33060/tcp:{}]
# Thu, 27 Jul 2023 22:18:51 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:5262579e8e45cb87fdc8fb6182d30da3c9e4f1036e02223508f287899ea434c0`  
		Last Modified: Thu, 21 Sep 2023 23:25:18 GMT  
		Size: 45.0 MB (44959147 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bfcc921068b5eaba8d310a26395ee4139cd54b21ec96369a39830e24cfe84477`  
		Last Modified: Wed, 04 Oct 2023 23:00:11 GMT  
		Size: 885.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:072a02315ab18d41372cf2e57b066a8ecf9954ab8d94cb5244ca20efe63df7ab`  
		Last Modified: Wed, 04 Oct 2023 23:00:11 GMT  
		Size: 982.8 KB (982808 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:711d47be56b4655b6deec62a811cddf52424477672f5930441ae8701ab012c95`  
		Last Modified: Wed, 04 Oct 2023 23:00:12 GMT  
		Size: 4.6 MB (4616305 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:755e67622a77c61bb6eb442164103b5395e7db380add9d61a2acb3425df65fa0`  
		Last Modified: Wed, 04 Oct 2023 23:00:12 GMT  
		Size: 2.6 KB (2608 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0080a11112d165a07d366db3a1ebd57709f066f4b13f10b57ec21e19d3d67d26`  
		Last Modified: Wed, 04 Oct 2023 23:00:12 GMT  
		Size: 340.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:adc45022a9ad6beda852b49f14ae18ff04ea052eb0f9391c31a29ecdffaa1ef1`  
		Last Modified: Wed, 04 Oct 2023 23:00:17 GMT  
		Size: 58.8 MB (58771345 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:67d8146998603ea2ed92b77bccbb35623a5eb39c6b047d15af930cec9ef79a9d`  
		Last Modified: Wed, 04 Oct 2023 23:00:13 GMT  
		Size: 316.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f431d85cf61e18099acd66976a43fb86be0ca84549a3853b4e2eaeb48557acb8`  
		Last Modified: Wed, 04 Oct 2023 23:00:16 GMT  
		Size: 57.5 MB (57524213 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4bbba6dd5ce26ba0b294a1cc506c8a57566efbaaf3701fe8eb752b54c4bd64c5`  
		Last Modified: Wed, 04 Oct 2023 23:00:14 GMT  
		Size: 5.4 KB (5389 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:8.1.0` - unknown; unknown

```console
$ docker pull mysql@sha256:3907151ff6c8a3d9a987e42f5af74ec79742398d67673c9e6f3baf067cbff3ab
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.1 MB (13141082 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3992e42cff0b10e86e3648547df8a978c66d19322dd629faa7cdacd2432028c9`

```dockerfile
```

-	Layers:
	-	`sha256:06d7ee16ec055f718e85ab70b205f9a40ac64f1f4bd3665bfd625ceffdce177c`  
		Last Modified: Wed, 04 Oct 2023 23:00:12 GMT  
		Size: 13.1 MB (13107503 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:81f9eeabc6e68920db4c4c28565e7cdbb580ecb31d9205d49fb827e33e860dd3`  
		Last Modified: Wed, 04 Oct 2023 23:00:11 GMT  
		Size: 33.6 KB (33579 bytes)  
		MIME: application/vnd.in-toto+json

### `mysql:8.1.0` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:8cacf9ef3db6f3e040c4ecde7f897706401d1f8330ca96862744e8b0d5781454
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.4 MB (170371412 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d30a00232fdc87bddbd635dad0486bf2278d705c76af20ec01f0814d0481064f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 27 Jul 2023 22:18:51 GMT
ADD file:b51d9ae1b78eb07ac424bfa71c45180e09ea3a5ed18fbfbcf881fb540bf83e9a in / 
# Thu, 27 Jul 2023 22:18:51 GMT
CMD ["/bin/bash"]
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
ENV GOSU_VERSION=1.16
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME" # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
ENV MYSQL_MAJOR=innovation
# Thu, 27 Jul 2023 22:18:51 GMT
ENV MYSQL_VERSION=8.1.0-1.el8
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysqlinnovation-server-minimal]'; 		echo 'name=MySQL innovation Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-innovation-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
ENV MYSQL_SHELL_VERSION=8.0.34-1.el8
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
VOLUME [/var/lib/mysql]
# Thu, 27 Jul 2023 22:18:51 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 27 Jul 2023 22:18:51 GMT
EXPOSE map[3306/tcp:{} 33060/tcp:{}]
# Thu, 27 Jul 2023 22:18:51 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:89ec84aa94fe6a62fb4e9f51aced09dea3cc4d7979c9f0ebd6b5bd4fd729e04e`  
		Last Modified: Thu, 12 Oct 2023 11:01:48 GMT  
		Size: 43.7 MB (43669807 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2047d0a85fcf9107bca7c22f98448ccf140ceed34e3b161beeb4904344032ab7`  
		Last Modified: Thu, 12 Oct 2023 20:57:52 GMT  
		Size: 884.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a981666a88bb712c4283e2a0a14f7ab9b27ff60bfc893fba647a0dbfaa93f6d0`  
		Last Modified: Thu, 12 Oct 2023 20:57:52 GMT  
		Size: 913.0 KB (912965 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7aa9dbd754432215cdd312410444c1c3859b4196dc771c13eba5a56682bef8dc`  
		Last Modified: Thu, 12 Oct 2023 20:57:52 GMT  
		Size: 4.3 MB (4303472 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b8ed90386e32a0124cf2dbca9de0ca31cd5f666b339a7e9a63dae44ed117e587`  
		Last Modified: Thu, 12 Oct 2023 20:57:53 GMT  
		Size: 2.6 KB (2609 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0b36981941b7e06e20d54a95dc6d483b22da2cb1e1fe68e9a77bcbcd2f55696c`  
		Last Modified: Thu, 12 Oct 2023 20:57:53 GMT  
		Size: 341.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ca996c23fc53d3fd7658d98952a4d481ae66e74585e2b72c55f961bf54455736`  
		Last Modified: Thu, 12 Oct 2023 20:57:57 GMT  
		Size: 57.7 MB (57701851 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:15050e9043e65433ddefd92b793734e91755006d5f756c6a9259998e9ccf916a`  
		Last Modified: Thu, 12 Oct 2023 20:57:54 GMT  
		Size: 316.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3ecfc97ced27490a7dd8db645fba5623698b5a933cb2359aedacf99e2dd74d54`  
		Last Modified: Thu, 12 Oct 2023 20:57:58 GMT  
		Size: 63.8 MB (63773775 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e435e3bf4d77af270e3b5245b5aa6234fcd3bb791ed57db4641d7ef99b33bf18`  
		Last Modified: Thu, 12 Oct 2023 20:57:55 GMT  
		Size: 5.4 KB (5392 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:8.1.0` - unknown; unknown

```console
$ docker pull mysql@sha256:33f7834b9a596feb3b7660924e45d3886bc1908da500f449c853ace58e7ef70d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.1 MB (13140098 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31013d6e714b5c7d6108fc3965658f4e7d97b6c8aa096f02b8230c4e1ebf99ae`

```dockerfile
```

-	Layers:
	-	`sha256:564dbabf3309a798678bcee0a9ac7f451cacb91050175a2e98f9313a605ae7cd`  
		Last Modified: Thu, 12 Oct 2023 20:57:54 GMT  
		Size: 13.1 MB (13106498 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:18613fc7c61e609bc95ef7402649a9c574fb26d032c9df3aa4e7b3f9b86b70e4`  
		Last Modified: Thu, 12 Oct 2023 20:57:52 GMT  
		Size: 33.6 KB (33600 bytes)  
		MIME: application/vnd.in-toto+json

## `mysql:8.1.0-oracle`

```console
$ docker pull mysql@sha256:9592f7dad3d285b9d2f89b1e9a586dbed983deb72ec190ba7d6af12120781d2e
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `mysql:8.1.0-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:5253d1662109ba7776430522fd73bd37f1c5775235eec63883fb8294d22757bc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **166.9 MB (166863356 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c138801544a941ed9d1171794e3361533109aa7e22f2ea4e1ba85bccc84f6842`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 27 Jul 2023 22:18:51 GMT
ADD file:909c07f3bad92a80d3917d583769a01bf62c2cbf3dd24f450fb303b1db92a83e in / 
# Thu, 27 Jul 2023 22:18:51 GMT
CMD ["/bin/bash"]
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
ENV GOSU_VERSION=1.16
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME" # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
ENV MYSQL_MAJOR=innovation
# Thu, 27 Jul 2023 22:18:51 GMT
ENV MYSQL_VERSION=8.1.0-1.el8
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysqlinnovation-server-minimal]'; 		echo 'name=MySQL innovation Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-innovation-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
ENV MYSQL_SHELL_VERSION=8.0.34-1.el8
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
VOLUME [/var/lib/mysql]
# Thu, 27 Jul 2023 22:18:51 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 27 Jul 2023 22:18:51 GMT
EXPOSE map[3306/tcp:{} 33060/tcp:{}]
# Thu, 27 Jul 2023 22:18:51 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:5262579e8e45cb87fdc8fb6182d30da3c9e4f1036e02223508f287899ea434c0`  
		Last Modified: Thu, 21 Sep 2023 23:25:18 GMT  
		Size: 45.0 MB (44959147 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bfcc921068b5eaba8d310a26395ee4139cd54b21ec96369a39830e24cfe84477`  
		Last Modified: Wed, 04 Oct 2023 23:00:11 GMT  
		Size: 885.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:072a02315ab18d41372cf2e57b066a8ecf9954ab8d94cb5244ca20efe63df7ab`  
		Last Modified: Wed, 04 Oct 2023 23:00:11 GMT  
		Size: 982.8 KB (982808 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:711d47be56b4655b6deec62a811cddf52424477672f5930441ae8701ab012c95`  
		Last Modified: Wed, 04 Oct 2023 23:00:12 GMT  
		Size: 4.6 MB (4616305 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:755e67622a77c61bb6eb442164103b5395e7db380add9d61a2acb3425df65fa0`  
		Last Modified: Wed, 04 Oct 2023 23:00:12 GMT  
		Size: 2.6 KB (2608 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0080a11112d165a07d366db3a1ebd57709f066f4b13f10b57ec21e19d3d67d26`  
		Last Modified: Wed, 04 Oct 2023 23:00:12 GMT  
		Size: 340.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:adc45022a9ad6beda852b49f14ae18ff04ea052eb0f9391c31a29ecdffaa1ef1`  
		Last Modified: Wed, 04 Oct 2023 23:00:17 GMT  
		Size: 58.8 MB (58771345 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:67d8146998603ea2ed92b77bccbb35623a5eb39c6b047d15af930cec9ef79a9d`  
		Last Modified: Wed, 04 Oct 2023 23:00:13 GMT  
		Size: 316.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f431d85cf61e18099acd66976a43fb86be0ca84549a3853b4e2eaeb48557acb8`  
		Last Modified: Wed, 04 Oct 2023 23:00:16 GMT  
		Size: 57.5 MB (57524213 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4bbba6dd5ce26ba0b294a1cc506c8a57566efbaaf3701fe8eb752b54c4bd64c5`  
		Last Modified: Wed, 04 Oct 2023 23:00:14 GMT  
		Size: 5.4 KB (5389 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:8.1.0-oracle` - unknown; unknown

```console
$ docker pull mysql@sha256:3907151ff6c8a3d9a987e42f5af74ec79742398d67673c9e6f3baf067cbff3ab
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.1 MB (13141082 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3992e42cff0b10e86e3648547df8a978c66d19322dd629faa7cdacd2432028c9`

```dockerfile
```

-	Layers:
	-	`sha256:06d7ee16ec055f718e85ab70b205f9a40ac64f1f4bd3665bfd625ceffdce177c`  
		Last Modified: Wed, 04 Oct 2023 23:00:12 GMT  
		Size: 13.1 MB (13107503 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:81f9eeabc6e68920db4c4c28565e7cdbb580ecb31d9205d49fb827e33e860dd3`  
		Last Modified: Wed, 04 Oct 2023 23:00:11 GMT  
		Size: 33.6 KB (33579 bytes)  
		MIME: application/vnd.in-toto+json

### `mysql:8.1.0-oracle` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:8cacf9ef3db6f3e040c4ecde7f897706401d1f8330ca96862744e8b0d5781454
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.4 MB (170371412 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d30a00232fdc87bddbd635dad0486bf2278d705c76af20ec01f0814d0481064f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 27 Jul 2023 22:18:51 GMT
ADD file:b51d9ae1b78eb07ac424bfa71c45180e09ea3a5ed18fbfbcf881fb540bf83e9a in / 
# Thu, 27 Jul 2023 22:18:51 GMT
CMD ["/bin/bash"]
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
ENV GOSU_VERSION=1.16
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME" # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
ENV MYSQL_MAJOR=innovation
# Thu, 27 Jul 2023 22:18:51 GMT
ENV MYSQL_VERSION=8.1.0-1.el8
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysqlinnovation-server-minimal]'; 		echo 'name=MySQL innovation Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-innovation-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
ENV MYSQL_SHELL_VERSION=8.0.34-1.el8
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
VOLUME [/var/lib/mysql]
# Thu, 27 Jul 2023 22:18:51 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 27 Jul 2023 22:18:51 GMT
EXPOSE map[3306/tcp:{} 33060/tcp:{}]
# Thu, 27 Jul 2023 22:18:51 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:89ec84aa94fe6a62fb4e9f51aced09dea3cc4d7979c9f0ebd6b5bd4fd729e04e`  
		Last Modified: Thu, 12 Oct 2023 11:01:48 GMT  
		Size: 43.7 MB (43669807 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2047d0a85fcf9107bca7c22f98448ccf140ceed34e3b161beeb4904344032ab7`  
		Last Modified: Thu, 12 Oct 2023 20:57:52 GMT  
		Size: 884.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a981666a88bb712c4283e2a0a14f7ab9b27ff60bfc893fba647a0dbfaa93f6d0`  
		Last Modified: Thu, 12 Oct 2023 20:57:52 GMT  
		Size: 913.0 KB (912965 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7aa9dbd754432215cdd312410444c1c3859b4196dc771c13eba5a56682bef8dc`  
		Last Modified: Thu, 12 Oct 2023 20:57:52 GMT  
		Size: 4.3 MB (4303472 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b8ed90386e32a0124cf2dbca9de0ca31cd5f666b339a7e9a63dae44ed117e587`  
		Last Modified: Thu, 12 Oct 2023 20:57:53 GMT  
		Size: 2.6 KB (2609 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0b36981941b7e06e20d54a95dc6d483b22da2cb1e1fe68e9a77bcbcd2f55696c`  
		Last Modified: Thu, 12 Oct 2023 20:57:53 GMT  
		Size: 341.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ca996c23fc53d3fd7658d98952a4d481ae66e74585e2b72c55f961bf54455736`  
		Last Modified: Thu, 12 Oct 2023 20:57:57 GMT  
		Size: 57.7 MB (57701851 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:15050e9043e65433ddefd92b793734e91755006d5f756c6a9259998e9ccf916a`  
		Last Modified: Thu, 12 Oct 2023 20:57:54 GMT  
		Size: 316.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3ecfc97ced27490a7dd8db645fba5623698b5a933cb2359aedacf99e2dd74d54`  
		Last Modified: Thu, 12 Oct 2023 20:57:58 GMT  
		Size: 63.8 MB (63773775 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e435e3bf4d77af270e3b5245b5aa6234fcd3bb791ed57db4641d7ef99b33bf18`  
		Last Modified: Thu, 12 Oct 2023 20:57:55 GMT  
		Size: 5.4 KB (5392 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:8.1.0-oracle` - unknown; unknown

```console
$ docker pull mysql@sha256:33f7834b9a596feb3b7660924e45d3886bc1908da500f449c853ace58e7ef70d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.1 MB (13140098 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31013d6e714b5c7d6108fc3965658f4e7d97b6c8aa096f02b8230c4e1ebf99ae`

```dockerfile
```

-	Layers:
	-	`sha256:564dbabf3309a798678bcee0a9ac7f451cacb91050175a2e98f9313a605ae7cd`  
		Last Modified: Thu, 12 Oct 2023 20:57:54 GMT  
		Size: 13.1 MB (13106498 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:18613fc7c61e609bc95ef7402649a9c574fb26d032c9df3aa4e7b3f9b86b70e4`  
		Last Modified: Thu, 12 Oct 2023 20:57:52 GMT  
		Size: 33.6 KB (33600 bytes)  
		MIME: application/vnd.in-toto+json

## `mysql:innovation`

```console
$ docker pull mysql@sha256:9592f7dad3d285b9d2f89b1e9a586dbed983deb72ec190ba7d6af12120781d2e
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `mysql:innovation` - linux; amd64

```console
$ docker pull mysql@sha256:5253d1662109ba7776430522fd73bd37f1c5775235eec63883fb8294d22757bc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **166.9 MB (166863356 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c138801544a941ed9d1171794e3361533109aa7e22f2ea4e1ba85bccc84f6842`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 27 Jul 2023 22:18:51 GMT
ADD file:909c07f3bad92a80d3917d583769a01bf62c2cbf3dd24f450fb303b1db92a83e in / 
# Thu, 27 Jul 2023 22:18:51 GMT
CMD ["/bin/bash"]
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
ENV GOSU_VERSION=1.16
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME" # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
ENV MYSQL_MAJOR=innovation
# Thu, 27 Jul 2023 22:18:51 GMT
ENV MYSQL_VERSION=8.1.0-1.el8
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysqlinnovation-server-minimal]'; 		echo 'name=MySQL innovation Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-innovation-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
ENV MYSQL_SHELL_VERSION=8.0.34-1.el8
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
VOLUME [/var/lib/mysql]
# Thu, 27 Jul 2023 22:18:51 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 27 Jul 2023 22:18:51 GMT
EXPOSE map[3306/tcp:{} 33060/tcp:{}]
# Thu, 27 Jul 2023 22:18:51 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:5262579e8e45cb87fdc8fb6182d30da3c9e4f1036e02223508f287899ea434c0`  
		Last Modified: Thu, 21 Sep 2023 23:25:18 GMT  
		Size: 45.0 MB (44959147 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bfcc921068b5eaba8d310a26395ee4139cd54b21ec96369a39830e24cfe84477`  
		Last Modified: Wed, 04 Oct 2023 23:00:11 GMT  
		Size: 885.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:072a02315ab18d41372cf2e57b066a8ecf9954ab8d94cb5244ca20efe63df7ab`  
		Last Modified: Wed, 04 Oct 2023 23:00:11 GMT  
		Size: 982.8 KB (982808 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:711d47be56b4655b6deec62a811cddf52424477672f5930441ae8701ab012c95`  
		Last Modified: Wed, 04 Oct 2023 23:00:12 GMT  
		Size: 4.6 MB (4616305 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:755e67622a77c61bb6eb442164103b5395e7db380add9d61a2acb3425df65fa0`  
		Last Modified: Wed, 04 Oct 2023 23:00:12 GMT  
		Size: 2.6 KB (2608 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0080a11112d165a07d366db3a1ebd57709f066f4b13f10b57ec21e19d3d67d26`  
		Last Modified: Wed, 04 Oct 2023 23:00:12 GMT  
		Size: 340.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:adc45022a9ad6beda852b49f14ae18ff04ea052eb0f9391c31a29ecdffaa1ef1`  
		Last Modified: Wed, 04 Oct 2023 23:00:17 GMT  
		Size: 58.8 MB (58771345 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:67d8146998603ea2ed92b77bccbb35623a5eb39c6b047d15af930cec9ef79a9d`  
		Last Modified: Wed, 04 Oct 2023 23:00:13 GMT  
		Size: 316.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f431d85cf61e18099acd66976a43fb86be0ca84549a3853b4e2eaeb48557acb8`  
		Last Modified: Wed, 04 Oct 2023 23:00:16 GMT  
		Size: 57.5 MB (57524213 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4bbba6dd5ce26ba0b294a1cc506c8a57566efbaaf3701fe8eb752b54c4bd64c5`  
		Last Modified: Wed, 04 Oct 2023 23:00:14 GMT  
		Size: 5.4 KB (5389 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:innovation` - unknown; unknown

```console
$ docker pull mysql@sha256:3907151ff6c8a3d9a987e42f5af74ec79742398d67673c9e6f3baf067cbff3ab
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.1 MB (13141082 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3992e42cff0b10e86e3648547df8a978c66d19322dd629faa7cdacd2432028c9`

```dockerfile
```

-	Layers:
	-	`sha256:06d7ee16ec055f718e85ab70b205f9a40ac64f1f4bd3665bfd625ceffdce177c`  
		Last Modified: Wed, 04 Oct 2023 23:00:12 GMT  
		Size: 13.1 MB (13107503 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:81f9eeabc6e68920db4c4c28565e7cdbb580ecb31d9205d49fb827e33e860dd3`  
		Last Modified: Wed, 04 Oct 2023 23:00:11 GMT  
		Size: 33.6 KB (33579 bytes)  
		MIME: application/vnd.in-toto+json

### `mysql:innovation` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:8cacf9ef3db6f3e040c4ecde7f897706401d1f8330ca96862744e8b0d5781454
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.4 MB (170371412 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d30a00232fdc87bddbd635dad0486bf2278d705c76af20ec01f0814d0481064f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 27 Jul 2023 22:18:51 GMT
ADD file:b51d9ae1b78eb07ac424bfa71c45180e09ea3a5ed18fbfbcf881fb540bf83e9a in / 
# Thu, 27 Jul 2023 22:18:51 GMT
CMD ["/bin/bash"]
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
ENV GOSU_VERSION=1.16
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME" # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
ENV MYSQL_MAJOR=innovation
# Thu, 27 Jul 2023 22:18:51 GMT
ENV MYSQL_VERSION=8.1.0-1.el8
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysqlinnovation-server-minimal]'; 		echo 'name=MySQL innovation Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-innovation-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
ENV MYSQL_SHELL_VERSION=8.0.34-1.el8
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
VOLUME [/var/lib/mysql]
# Thu, 27 Jul 2023 22:18:51 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 27 Jul 2023 22:18:51 GMT
EXPOSE map[3306/tcp:{} 33060/tcp:{}]
# Thu, 27 Jul 2023 22:18:51 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:89ec84aa94fe6a62fb4e9f51aced09dea3cc4d7979c9f0ebd6b5bd4fd729e04e`  
		Last Modified: Thu, 12 Oct 2023 11:01:48 GMT  
		Size: 43.7 MB (43669807 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2047d0a85fcf9107bca7c22f98448ccf140ceed34e3b161beeb4904344032ab7`  
		Last Modified: Thu, 12 Oct 2023 20:57:52 GMT  
		Size: 884.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a981666a88bb712c4283e2a0a14f7ab9b27ff60bfc893fba647a0dbfaa93f6d0`  
		Last Modified: Thu, 12 Oct 2023 20:57:52 GMT  
		Size: 913.0 KB (912965 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7aa9dbd754432215cdd312410444c1c3859b4196dc771c13eba5a56682bef8dc`  
		Last Modified: Thu, 12 Oct 2023 20:57:52 GMT  
		Size: 4.3 MB (4303472 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b8ed90386e32a0124cf2dbca9de0ca31cd5f666b339a7e9a63dae44ed117e587`  
		Last Modified: Thu, 12 Oct 2023 20:57:53 GMT  
		Size: 2.6 KB (2609 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0b36981941b7e06e20d54a95dc6d483b22da2cb1e1fe68e9a77bcbcd2f55696c`  
		Last Modified: Thu, 12 Oct 2023 20:57:53 GMT  
		Size: 341.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ca996c23fc53d3fd7658d98952a4d481ae66e74585e2b72c55f961bf54455736`  
		Last Modified: Thu, 12 Oct 2023 20:57:57 GMT  
		Size: 57.7 MB (57701851 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:15050e9043e65433ddefd92b793734e91755006d5f756c6a9259998e9ccf916a`  
		Last Modified: Thu, 12 Oct 2023 20:57:54 GMT  
		Size: 316.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3ecfc97ced27490a7dd8db645fba5623698b5a933cb2359aedacf99e2dd74d54`  
		Last Modified: Thu, 12 Oct 2023 20:57:58 GMT  
		Size: 63.8 MB (63773775 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e435e3bf4d77af270e3b5245b5aa6234fcd3bb791ed57db4641d7ef99b33bf18`  
		Last Modified: Thu, 12 Oct 2023 20:57:55 GMT  
		Size: 5.4 KB (5392 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:innovation` - unknown; unknown

```console
$ docker pull mysql@sha256:33f7834b9a596feb3b7660924e45d3886bc1908da500f449c853ace58e7ef70d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.1 MB (13140098 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31013d6e714b5c7d6108fc3965658f4e7d97b6c8aa096f02b8230c4e1ebf99ae`

```dockerfile
```

-	Layers:
	-	`sha256:564dbabf3309a798678bcee0a9ac7f451cacb91050175a2e98f9313a605ae7cd`  
		Last Modified: Thu, 12 Oct 2023 20:57:54 GMT  
		Size: 13.1 MB (13106498 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:18613fc7c61e609bc95ef7402649a9c574fb26d032c9df3aa4e7b3f9b86b70e4`  
		Last Modified: Thu, 12 Oct 2023 20:57:52 GMT  
		Size: 33.6 KB (33600 bytes)  
		MIME: application/vnd.in-toto+json

## `mysql:innovation-oracle`

```console
$ docker pull mysql@sha256:9592f7dad3d285b9d2f89b1e9a586dbed983deb72ec190ba7d6af12120781d2e
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `mysql:innovation-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:5253d1662109ba7776430522fd73bd37f1c5775235eec63883fb8294d22757bc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **166.9 MB (166863356 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c138801544a941ed9d1171794e3361533109aa7e22f2ea4e1ba85bccc84f6842`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 27 Jul 2023 22:18:51 GMT
ADD file:909c07f3bad92a80d3917d583769a01bf62c2cbf3dd24f450fb303b1db92a83e in / 
# Thu, 27 Jul 2023 22:18:51 GMT
CMD ["/bin/bash"]
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
ENV GOSU_VERSION=1.16
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME" # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
ENV MYSQL_MAJOR=innovation
# Thu, 27 Jul 2023 22:18:51 GMT
ENV MYSQL_VERSION=8.1.0-1.el8
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysqlinnovation-server-minimal]'; 		echo 'name=MySQL innovation Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-innovation-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
ENV MYSQL_SHELL_VERSION=8.0.34-1.el8
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
VOLUME [/var/lib/mysql]
# Thu, 27 Jul 2023 22:18:51 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 27 Jul 2023 22:18:51 GMT
EXPOSE map[3306/tcp:{} 33060/tcp:{}]
# Thu, 27 Jul 2023 22:18:51 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:5262579e8e45cb87fdc8fb6182d30da3c9e4f1036e02223508f287899ea434c0`  
		Last Modified: Thu, 21 Sep 2023 23:25:18 GMT  
		Size: 45.0 MB (44959147 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bfcc921068b5eaba8d310a26395ee4139cd54b21ec96369a39830e24cfe84477`  
		Last Modified: Wed, 04 Oct 2023 23:00:11 GMT  
		Size: 885.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:072a02315ab18d41372cf2e57b066a8ecf9954ab8d94cb5244ca20efe63df7ab`  
		Last Modified: Wed, 04 Oct 2023 23:00:11 GMT  
		Size: 982.8 KB (982808 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:711d47be56b4655b6deec62a811cddf52424477672f5930441ae8701ab012c95`  
		Last Modified: Wed, 04 Oct 2023 23:00:12 GMT  
		Size: 4.6 MB (4616305 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:755e67622a77c61bb6eb442164103b5395e7db380add9d61a2acb3425df65fa0`  
		Last Modified: Wed, 04 Oct 2023 23:00:12 GMT  
		Size: 2.6 KB (2608 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0080a11112d165a07d366db3a1ebd57709f066f4b13f10b57ec21e19d3d67d26`  
		Last Modified: Wed, 04 Oct 2023 23:00:12 GMT  
		Size: 340.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:adc45022a9ad6beda852b49f14ae18ff04ea052eb0f9391c31a29ecdffaa1ef1`  
		Last Modified: Wed, 04 Oct 2023 23:00:17 GMT  
		Size: 58.8 MB (58771345 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:67d8146998603ea2ed92b77bccbb35623a5eb39c6b047d15af930cec9ef79a9d`  
		Last Modified: Wed, 04 Oct 2023 23:00:13 GMT  
		Size: 316.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f431d85cf61e18099acd66976a43fb86be0ca84549a3853b4e2eaeb48557acb8`  
		Last Modified: Wed, 04 Oct 2023 23:00:16 GMT  
		Size: 57.5 MB (57524213 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4bbba6dd5ce26ba0b294a1cc506c8a57566efbaaf3701fe8eb752b54c4bd64c5`  
		Last Modified: Wed, 04 Oct 2023 23:00:14 GMT  
		Size: 5.4 KB (5389 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:innovation-oracle` - unknown; unknown

```console
$ docker pull mysql@sha256:3907151ff6c8a3d9a987e42f5af74ec79742398d67673c9e6f3baf067cbff3ab
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.1 MB (13141082 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3992e42cff0b10e86e3648547df8a978c66d19322dd629faa7cdacd2432028c9`

```dockerfile
```

-	Layers:
	-	`sha256:06d7ee16ec055f718e85ab70b205f9a40ac64f1f4bd3665bfd625ceffdce177c`  
		Last Modified: Wed, 04 Oct 2023 23:00:12 GMT  
		Size: 13.1 MB (13107503 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:81f9eeabc6e68920db4c4c28565e7cdbb580ecb31d9205d49fb827e33e860dd3`  
		Last Modified: Wed, 04 Oct 2023 23:00:11 GMT  
		Size: 33.6 KB (33579 bytes)  
		MIME: application/vnd.in-toto+json

### `mysql:innovation-oracle` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:8cacf9ef3db6f3e040c4ecde7f897706401d1f8330ca96862744e8b0d5781454
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.4 MB (170371412 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d30a00232fdc87bddbd635dad0486bf2278d705c76af20ec01f0814d0481064f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 27 Jul 2023 22:18:51 GMT
ADD file:b51d9ae1b78eb07ac424bfa71c45180e09ea3a5ed18fbfbcf881fb540bf83e9a in / 
# Thu, 27 Jul 2023 22:18:51 GMT
CMD ["/bin/bash"]
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
ENV GOSU_VERSION=1.16
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME" # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
ENV MYSQL_MAJOR=innovation
# Thu, 27 Jul 2023 22:18:51 GMT
ENV MYSQL_VERSION=8.1.0-1.el8
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysqlinnovation-server-minimal]'; 		echo 'name=MySQL innovation Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-innovation-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
ENV MYSQL_SHELL_VERSION=8.0.34-1.el8
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
VOLUME [/var/lib/mysql]
# Thu, 27 Jul 2023 22:18:51 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 27 Jul 2023 22:18:51 GMT
EXPOSE map[3306/tcp:{} 33060/tcp:{}]
# Thu, 27 Jul 2023 22:18:51 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:89ec84aa94fe6a62fb4e9f51aced09dea3cc4d7979c9f0ebd6b5bd4fd729e04e`  
		Last Modified: Thu, 12 Oct 2023 11:01:48 GMT  
		Size: 43.7 MB (43669807 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2047d0a85fcf9107bca7c22f98448ccf140ceed34e3b161beeb4904344032ab7`  
		Last Modified: Thu, 12 Oct 2023 20:57:52 GMT  
		Size: 884.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a981666a88bb712c4283e2a0a14f7ab9b27ff60bfc893fba647a0dbfaa93f6d0`  
		Last Modified: Thu, 12 Oct 2023 20:57:52 GMT  
		Size: 913.0 KB (912965 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7aa9dbd754432215cdd312410444c1c3859b4196dc771c13eba5a56682bef8dc`  
		Last Modified: Thu, 12 Oct 2023 20:57:52 GMT  
		Size: 4.3 MB (4303472 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b8ed90386e32a0124cf2dbca9de0ca31cd5f666b339a7e9a63dae44ed117e587`  
		Last Modified: Thu, 12 Oct 2023 20:57:53 GMT  
		Size: 2.6 KB (2609 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0b36981941b7e06e20d54a95dc6d483b22da2cb1e1fe68e9a77bcbcd2f55696c`  
		Last Modified: Thu, 12 Oct 2023 20:57:53 GMT  
		Size: 341.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ca996c23fc53d3fd7658d98952a4d481ae66e74585e2b72c55f961bf54455736`  
		Last Modified: Thu, 12 Oct 2023 20:57:57 GMT  
		Size: 57.7 MB (57701851 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:15050e9043e65433ddefd92b793734e91755006d5f756c6a9259998e9ccf916a`  
		Last Modified: Thu, 12 Oct 2023 20:57:54 GMT  
		Size: 316.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3ecfc97ced27490a7dd8db645fba5623698b5a933cb2359aedacf99e2dd74d54`  
		Last Modified: Thu, 12 Oct 2023 20:57:58 GMT  
		Size: 63.8 MB (63773775 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e435e3bf4d77af270e3b5245b5aa6234fcd3bb791ed57db4641d7ef99b33bf18`  
		Last Modified: Thu, 12 Oct 2023 20:57:55 GMT  
		Size: 5.4 KB (5392 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:innovation-oracle` - unknown; unknown

```console
$ docker pull mysql@sha256:33f7834b9a596feb3b7660924e45d3886bc1908da500f449c853ace58e7ef70d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.1 MB (13140098 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31013d6e714b5c7d6108fc3965658f4e7d97b6c8aa096f02b8230c4e1ebf99ae`

```dockerfile
```

-	Layers:
	-	`sha256:564dbabf3309a798678bcee0a9ac7f451cacb91050175a2e98f9313a605ae7cd`  
		Last Modified: Thu, 12 Oct 2023 20:57:54 GMT  
		Size: 13.1 MB (13106498 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:18613fc7c61e609bc95ef7402649a9c574fb26d032c9df3aa4e7b3f9b86b70e4`  
		Last Modified: Thu, 12 Oct 2023 20:57:52 GMT  
		Size: 33.6 KB (33600 bytes)  
		MIME: application/vnd.in-toto+json

## `mysql:latest`

```console
$ docker pull mysql@sha256:9592f7dad3d285b9d2f89b1e9a586dbed983deb72ec190ba7d6af12120781d2e
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `mysql:latest` - linux; amd64

```console
$ docker pull mysql@sha256:5253d1662109ba7776430522fd73bd37f1c5775235eec63883fb8294d22757bc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **166.9 MB (166863356 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c138801544a941ed9d1171794e3361533109aa7e22f2ea4e1ba85bccc84f6842`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 27 Jul 2023 22:18:51 GMT
ADD file:909c07f3bad92a80d3917d583769a01bf62c2cbf3dd24f450fb303b1db92a83e in / 
# Thu, 27 Jul 2023 22:18:51 GMT
CMD ["/bin/bash"]
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
ENV GOSU_VERSION=1.16
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME" # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
ENV MYSQL_MAJOR=innovation
# Thu, 27 Jul 2023 22:18:51 GMT
ENV MYSQL_VERSION=8.1.0-1.el8
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysqlinnovation-server-minimal]'; 		echo 'name=MySQL innovation Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-innovation-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
ENV MYSQL_SHELL_VERSION=8.0.34-1.el8
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
VOLUME [/var/lib/mysql]
# Thu, 27 Jul 2023 22:18:51 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 27 Jul 2023 22:18:51 GMT
EXPOSE map[3306/tcp:{} 33060/tcp:{}]
# Thu, 27 Jul 2023 22:18:51 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:5262579e8e45cb87fdc8fb6182d30da3c9e4f1036e02223508f287899ea434c0`  
		Last Modified: Thu, 21 Sep 2023 23:25:18 GMT  
		Size: 45.0 MB (44959147 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bfcc921068b5eaba8d310a26395ee4139cd54b21ec96369a39830e24cfe84477`  
		Last Modified: Wed, 04 Oct 2023 23:00:11 GMT  
		Size: 885.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:072a02315ab18d41372cf2e57b066a8ecf9954ab8d94cb5244ca20efe63df7ab`  
		Last Modified: Wed, 04 Oct 2023 23:00:11 GMT  
		Size: 982.8 KB (982808 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:711d47be56b4655b6deec62a811cddf52424477672f5930441ae8701ab012c95`  
		Last Modified: Wed, 04 Oct 2023 23:00:12 GMT  
		Size: 4.6 MB (4616305 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:755e67622a77c61bb6eb442164103b5395e7db380add9d61a2acb3425df65fa0`  
		Last Modified: Wed, 04 Oct 2023 23:00:12 GMT  
		Size: 2.6 KB (2608 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0080a11112d165a07d366db3a1ebd57709f066f4b13f10b57ec21e19d3d67d26`  
		Last Modified: Wed, 04 Oct 2023 23:00:12 GMT  
		Size: 340.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:adc45022a9ad6beda852b49f14ae18ff04ea052eb0f9391c31a29ecdffaa1ef1`  
		Last Modified: Wed, 04 Oct 2023 23:00:17 GMT  
		Size: 58.8 MB (58771345 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:67d8146998603ea2ed92b77bccbb35623a5eb39c6b047d15af930cec9ef79a9d`  
		Last Modified: Wed, 04 Oct 2023 23:00:13 GMT  
		Size: 316.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f431d85cf61e18099acd66976a43fb86be0ca84549a3853b4e2eaeb48557acb8`  
		Last Modified: Wed, 04 Oct 2023 23:00:16 GMT  
		Size: 57.5 MB (57524213 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4bbba6dd5ce26ba0b294a1cc506c8a57566efbaaf3701fe8eb752b54c4bd64c5`  
		Last Modified: Wed, 04 Oct 2023 23:00:14 GMT  
		Size: 5.4 KB (5389 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:latest` - unknown; unknown

```console
$ docker pull mysql@sha256:3907151ff6c8a3d9a987e42f5af74ec79742398d67673c9e6f3baf067cbff3ab
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.1 MB (13141082 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3992e42cff0b10e86e3648547df8a978c66d19322dd629faa7cdacd2432028c9`

```dockerfile
```

-	Layers:
	-	`sha256:06d7ee16ec055f718e85ab70b205f9a40ac64f1f4bd3665bfd625ceffdce177c`  
		Last Modified: Wed, 04 Oct 2023 23:00:12 GMT  
		Size: 13.1 MB (13107503 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:81f9eeabc6e68920db4c4c28565e7cdbb580ecb31d9205d49fb827e33e860dd3`  
		Last Modified: Wed, 04 Oct 2023 23:00:11 GMT  
		Size: 33.6 KB (33579 bytes)  
		MIME: application/vnd.in-toto+json

### `mysql:latest` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:8cacf9ef3db6f3e040c4ecde7f897706401d1f8330ca96862744e8b0d5781454
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.4 MB (170371412 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d30a00232fdc87bddbd635dad0486bf2278d705c76af20ec01f0814d0481064f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 27 Jul 2023 22:18:51 GMT
ADD file:b51d9ae1b78eb07ac424bfa71c45180e09ea3a5ed18fbfbcf881fb540bf83e9a in / 
# Thu, 27 Jul 2023 22:18:51 GMT
CMD ["/bin/bash"]
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
ENV GOSU_VERSION=1.16
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME" # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
ENV MYSQL_MAJOR=innovation
# Thu, 27 Jul 2023 22:18:51 GMT
ENV MYSQL_VERSION=8.1.0-1.el8
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysqlinnovation-server-minimal]'; 		echo 'name=MySQL innovation Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-innovation-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
ENV MYSQL_SHELL_VERSION=8.0.34-1.el8
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
VOLUME [/var/lib/mysql]
# Thu, 27 Jul 2023 22:18:51 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 27 Jul 2023 22:18:51 GMT
EXPOSE map[3306/tcp:{} 33060/tcp:{}]
# Thu, 27 Jul 2023 22:18:51 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:89ec84aa94fe6a62fb4e9f51aced09dea3cc4d7979c9f0ebd6b5bd4fd729e04e`  
		Last Modified: Thu, 12 Oct 2023 11:01:48 GMT  
		Size: 43.7 MB (43669807 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2047d0a85fcf9107bca7c22f98448ccf140ceed34e3b161beeb4904344032ab7`  
		Last Modified: Thu, 12 Oct 2023 20:57:52 GMT  
		Size: 884.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a981666a88bb712c4283e2a0a14f7ab9b27ff60bfc893fba647a0dbfaa93f6d0`  
		Last Modified: Thu, 12 Oct 2023 20:57:52 GMT  
		Size: 913.0 KB (912965 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7aa9dbd754432215cdd312410444c1c3859b4196dc771c13eba5a56682bef8dc`  
		Last Modified: Thu, 12 Oct 2023 20:57:52 GMT  
		Size: 4.3 MB (4303472 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b8ed90386e32a0124cf2dbca9de0ca31cd5f666b339a7e9a63dae44ed117e587`  
		Last Modified: Thu, 12 Oct 2023 20:57:53 GMT  
		Size: 2.6 KB (2609 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0b36981941b7e06e20d54a95dc6d483b22da2cb1e1fe68e9a77bcbcd2f55696c`  
		Last Modified: Thu, 12 Oct 2023 20:57:53 GMT  
		Size: 341.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ca996c23fc53d3fd7658d98952a4d481ae66e74585e2b72c55f961bf54455736`  
		Last Modified: Thu, 12 Oct 2023 20:57:57 GMT  
		Size: 57.7 MB (57701851 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:15050e9043e65433ddefd92b793734e91755006d5f756c6a9259998e9ccf916a`  
		Last Modified: Thu, 12 Oct 2023 20:57:54 GMT  
		Size: 316.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3ecfc97ced27490a7dd8db645fba5623698b5a933cb2359aedacf99e2dd74d54`  
		Last Modified: Thu, 12 Oct 2023 20:57:58 GMT  
		Size: 63.8 MB (63773775 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e435e3bf4d77af270e3b5245b5aa6234fcd3bb791ed57db4641d7ef99b33bf18`  
		Last Modified: Thu, 12 Oct 2023 20:57:55 GMT  
		Size: 5.4 KB (5392 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:latest` - unknown; unknown

```console
$ docker pull mysql@sha256:33f7834b9a596feb3b7660924e45d3886bc1908da500f449c853ace58e7ef70d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.1 MB (13140098 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31013d6e714b5c7d6108fc3965658f4e7d97b6c8aa096f02b8230c4e1ebf99ae`

```dockerfile
```

-	Layers:
	-	`sha256:564dbabf3309a798678bcee0a9ac7f451cacb91050175a2e98f9313a605ae7cd`  
		Last Modified: Thu, 12 Oct 2023 20:57:54 GMT  
		Size: 13.1 MB (13106498 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:18613fc7c61e609bc95ef7402649a9c574fb26d032c9df3aa4e7b3f9b86b70e4`  
		Last Modified: Thu, 12 Oct 2023 20:57:52 GMT  
		Size: 33.6 KB (33600 bytes)  
		MIME: application/vnd.in-toto+json

## `mysql:oracle`

```console
$ docker pull mysql@sha256:9592f7dad3d285b9d2f89b1e9a586dbed983deb72ec190ba7d6af12120781d2e
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `mysql:oracle` - linux; amd64

```console
$ docker pull mysql@sha256:5253d1662109ba7776430522fd73bd37f1c5775235eec63883fb8294d22757bc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **166.9 MB (166863356 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c138801544a941ed9d1171794e3361533109aa7e22f2ea4e1ba85bccc84f6842`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 27 Jul 2023 22:18:51 GMT
ADD file:909c07f3bad92a80d3917d583769a01bf62c2cbf3dd24f450fb303b1db92a83e in / 
# Thu, 27 Jul 2023 22:18:51 GMT
CMD ["/bin/bash"]
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
ENV GOSU_VERSION=1.16
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME" # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
ENV MYSQL_MAJOR=innovation
# Thu, 27 Jul 2023 22:18:51 GMT
ENV MYSQL_VERSION=8.1.0-1.el8
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysqlinnovation-server-minimal]'; 		echo 'name=MySQL innovation Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-innovation-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
ENV MYSQL_SHELL_VERSION=8.0.34-1.el8
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
VOLUME [/var/lib/mysql]
# Thu, 27 Jul 2023 22:18:51 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 27 Jul 2023 22:18:51 GMT
EXPOSE map[3306/tcp:{} 33060/tcp:{}]
# Thu, 27 Jul 2023 22:18:51 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:5262579e8e45cb87fdc8fb6182d30da3c9e4f1036e02223508f287899ea434c0`  
		Last Modified: Thu, 21 Sep 2023 23:25:18 GMT  
		Size: 45.0 MB (44959147 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bfcc921068b5eaba8d310a26395ee4139cd54b21ec96369a39830e24cfe84477`  
		Last Modified: Wed, 04 Oct 2023 23:00:11 GMT  
		Size: 885.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:072a02315ab18d41372cf2e57b066a8ecf9954ab8d94cb5244ca20efe63df7ab`  
		Last Modified: Wed, 04 Oct 2023 23:00:11 GMT  
		Size: 982.8 KB (982808 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:711d47be56b4655b6deec62a811cddf52424477672f5930441ae8701ab012c95`  
		Last Modified: Wed, 04 Oct 2023 23:00:12 GMT  
		Size: 4.6 MB (4616305 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:755e67622a77c61bb6eb442164103b5395e7db380add9d61a2acb3425df65fa0`  
		Last Modified: Wed, 04 Oct 2023 23:00:12 GMT  
		Size: 2.6 KB (2608 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0080a11112d165a07d366db3a1ebd57709f066f4b13f10b57ec21e19d3d67d26`  
		Last Modified: Wed, 04 Oct 2023 23:00:12 GMT  
		Size: 340.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:adc45022a9ad6beda852b49f14ae18ff04ea052eb0f9391c31a29ecdffaa1ef1`  
		Last Modified: Wed, 04 Oct 2023 23:00:17 GMT  
		Size: 58.8 MB (58771345 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:67d8146998603ea2ed92b77bccbb35623a5eb39c6b047d15af930cec9ef79a9d`  
		Last Modified: Wed, 04 Oct 2023 23:00:13 GMT  
		Size: 316.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f431d85cf61e18099acd66976a43fb86be0ca84549a3853b4e2eaeb48557acb8`  
		Last Modified: Wed, 04 Oct 2023 23:00:16 GMT  
		Size: 57.5 MB (57524213 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4bbba6dd5ce26ba0b294a1cc506c8a57566efbaaf3701fe8eb752b54c4bd64c5`  
		Last Modified: Wed, 04 Oct 2023 23:00:14 GMT  
		Size: 5.4 KB (5389 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:oracle` - unknown; unknown

```console
$ docker pull mysql@sha256:3907151ff6c8a3d9a987e42f5af74ec79742398d67673c9e6f3baf067cbff3ab
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.1 MB (13141082 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3992e42cff0b10e86e3648547df8a978c66d19322dd629faa7cdacd2432028c9`

```dockerfile
```

-	Layers:
	-	`sha256:06d7ee16ec055f718e85ab70b205f9a40ac64f1f4bd3665bfd625ceffdce177c`  
		Last Modified: Wed, 04 Oct 2023 23:00:12 GMT  
		Size: 13.1 MB (13107503 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:81f9eeabc6e68920db4c4c28565e7cdbb580ecb31d9205d49fb827e33e860dd3`  
		Last Modified: Wed, 04 Oct 2023 23:00:11 GMT  
		Size: 33.6 KB (33579 bytes)  
		MIME: application/vnd.in-toto+json

### `mysql:oracle` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:8cacf9ef3db6f3e040c4ecde7f897706401d1f8330ca96862744e8b0d5781454
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.4 MB (170371412 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d30a00232fdc87bddbd635dad0486bf2278d705c76af20ec01f0814d0481064f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 27 Jul 2023 22:18:51 GMT
ADD file:b51d9ae1b78eb07ac424bfa71c45180e09ea3a5ed18fbfbcf881fb540bf83e9a in / 
# Thu, 27 Jul 2023 22:18:51 GMT
CMD ["/bin/bash"]
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	groupadd --system --gid 999 mysql; 	useradd --system --uid 999 --gid 999 --home-dir /var/lib/mysql --no-create-home mysql # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
ENV GOSU_VERSION=1.16
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	arch="$(uname -m)"; 	case "$arch" in 		aarch64) gosuArch='arm64' ;; 		x86_64) gosuArch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 	curl -fL -o /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch.asc"; 	curl -fL -o /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$gosuArch"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	microdnf install -y 		bzip2 		gzip 		openssl 		xz 		zstd 		findutils 	; 	microdnf clean all # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	key='859BE8D7C586F538430B19C2467B942D3A79BD29'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql; 	rm -rf "$GNUPGHOME" # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
ENV MYSQL_MAJOR=innovation
# Thu, 27 Jul 2023 22:18:51 GMT
ENV MYSQL_VERSION=8.1.0-1.el8
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysqlinnovation-server-minimal]'; 		echo 'name=MySQL innovation Server Minimal'; 		echo 'enabled=1'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-innovation-community/docker/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-minimal.repo # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	microdnf install -y "mysql-community-server-minimal-$MYSQL_VERSION"; 	microdnf clean all; 	grep -F 'socket=/var/lib/mysql/mysql.sock' /etc/my.cnf; 	sed -i 's!^socket=.*!socket=/var/run/mysqld/mysqld.sock!' /etc/my.cnf; 	grep -F 'socket=/var/run/mysqld/mysqld.sock' /etc/my.cnf; 	{ echo '[client]'; echo 'socket=/var/run/mysqld/mysqld.sock'; } >> /etc/my.cnf; 		! grep -F '!includedir' /etc/my.cnf; 	{ echo; echo '!includedir /etc/mysql/conf.d/'; } >> /etc/my.cnf; 	mkdir -p /etc/mysql/conf.d; 	mkdir -p /var/lib/mysql /var/run/mysqld; 	chown mysql:mysql /var/lib/mysql /var/run/mysqld; 	chmod 1777 /var/lib/mysql /var/run/mysqld; 		mkdir /docker-entrypoint-initdb.d; 		mysqld --version; 	mysql --version # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eu; 	. /etc/os-release; 	{ 		echo '[mysql-tools-community]'; 		echo 'name=MySQL Tools Community'; 		echo "baseurl=https://repo.mysql.com/yum/mysql-tools-community/el/${VERSION_ID%%[.-]*}/\$basearch/"; 		echo 'enabled=1'; 		echo 'gpgcheck=1'; 		echo 'gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql'; 		echo 'module_hotfixes=true'; 	} | tee /etc/yum.repos.d/mysql-community-tools.repo # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
ENV MYSQL_SHELL_VERSION=8.0.34-1.el8
# Thu, 27 Jul 2023 22:18:51 GMT
RUN set -eux; 	microdnf install -y "mysql-shell-$MYSQL_SHELL_VERSION"; 	microdnf clean all; 		mysqlsh --version # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
VOLUME [/var/lib/mysql]
# Thu, 27 Jul 2023 22:18:51 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 27 Jul 2023 22:18:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 27 Jul 2023 22:18:51 GMT
EXPOSE map[3306/tcp:{} 33060/tcp:{}]
# Thu, 27 Jul 2023 22:18:51 GMT
CMD ["mysqld"]
```

-	Layers:
	-	`sha256:89ec84aa94fe6a62fb4e9f51aced09dea3cc4d7979c9f0ebd6b5bd4fd729e04e`  
		Last Modified: Thu, 12 Oct 2023 11:01:48 GMT  
		Size: 43.7 MB (43669807 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2047d0a85fcf9107bca7c22f98448ccf140ceed34e3b161beeb4904344032ab7`  
		Last Modified: Thu, 12 Oct 2023 20:57:52 GMT  
		Size: 884.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a981666a88bb712c4283e2a0a14f7ab9b27ff60bfc893fba647a0dbfaa93f6d0`  
		Last Modified: Thu, 12 Oct 2023 20:57:52 GMT  
		Size: 913.0 KB (912965 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7aa9dbd754432215cdd312410444c1c3859b4196dc771c13eba5a56682bef8dc`  
		Last Modified: Thu, 12 Oct 2023 20:57:52 GMT  
		Size: 4.3 MB (4303472 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b8ed90386e32a0124cf2dbca9de0ca31cd5f666b339a7e9a63dae44ed117e587`  
		Last Modified: Thu, 12 Oct 2023 20:57:53 GMT  
		Size: 2.6 KB (2609 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0b36981941b7e06e20d54a95dc6d483b22da2cb1e1fe68e9a77bcbcd2f55696c`  
		Last Modified: Thu, 12 Oct 2023 20:57:53 GMT  
		Size: 341.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ca996c23fc53d3fd7658d98952a4d481ae66e74585e2b72c55f961bf54455736`  
		Last Modified: Thu, 12 Oct 2023 20:57:57 GMT  
		Size: 57.7 MB (57701851 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:15050e9043e65433ddefd92b793734e91755006d5f756c6a9259998e9ccf916a`  
		Last Modified: Thu, 12 Oct 2023 20:57:54 GMT  
		Size: 316.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3ecfc97ced27490a7dd8db645fba5623698b5a933cb2359aedacf99e2dd74d54`  
		Last Modified: Thu, 12 Oct 2023 20:57:58 GMT  
		Size: 63.8 MB (63773775 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e435e3bf4d77af270e3b5245b5aa6234fcd3bb791ed57db4641d7ef99b33bf18`  
		Last Modified: Thu, 12 Oct 2023 20:57:55 GMT  
		Size: 5.4 KB (5392 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:oracle` - unknown; unknown

```console
$ docker pull mysql@sha256:33f7834b9a596feb3b7660924e45d3886bc1908da500f449c853ace58e7ef70d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.1 MB (13140098 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31013d6e714b5c7d6108fc3965658f4e7d97b6c8aa096f02b8230c4e1ebf99ae`

```dockerfile
```

-	Layers:
	-	`sha256:564dbabf3309a798678bcee0a9ac7f451cacb91050175a2e98f9313a605ae7cd`  
		Last Modified: Thu, 12 Oct 2023 20:57:54 GMT  
		Size: 13.1 MB (13106498 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:18613fc7c61e609bc95ef7402649a9c574fb26d032c9df3aa4e7b3f9b86b70e4`  
		Last Modified: Thu, 12 Oct 2023 20:57:52 GMT  
		Size: 33.6 KB (33600 bytes)  
		MIME: application/vnd.in-toto+json
