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
$ docker pull mysql@sha256:44056c45e214c26c37b6f244534c6fb5f8a40eacbc28e870a2652b19d7a8a814
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
$ docker pull mysql@sha256:2b94677c88791084b0deb390e1966c74f5b6b439c70437587d0ba25f0df52df0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.4 MB (170366065 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54fea0bc79f9c00cc1eb77f4ce9314d116b731d441f86972c6ffeef5987a0429`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 27 Jul 2023 22:18:51 GMT
ADD file:c630310324edbc0dd09d0912b8e7074d17ac71b1be8a14af9663872c081c4632 in / 
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
	-	`sha256:286c1c922769d7608c32cf62931e95d7d169a0306164d24ce7d7a8a065959315`  
		Last Modified: Thu, 21 Sep 2023 23:41:39 GMT  
		Size: 43.7 MB (43657726 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cb7c97478965081773cf774f51b68ba7bc4ddeb1a1c4911ac6dd52e3939a9b02`  
		Last Modified: Wed, 04 Oct 2023 23:56:04 GMT  
		Size: 885.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4056102542df153013330c711c65a022891653dcb4f6b7b8584d32d1cc6ebf65`  
		Last Modified: Wed, 04 Oct 2023 23:56:04 GMT  
		Size: 913.0 KB (912965 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2cfd45c39ba383ddf8f928620c4623faab5bbed0c180b48b176c0361d441a358`  
		Last Modified: Wed, 04 Oct 2023 23:56:04 GMT  
		Size: 4.3 MB (4300663 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:770637688c59082858f7a4a8f12a627c10790774fad0c720ad868e871efcce47`  
		Last Modified: Wed, 04 Oct 2023 23:56:05 GMT  
		Size: 2.6 KB (2608 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5e04d4eff28a3ef1fd9d6816f12752bb2798413e20d7e54f9ac982ce912ea77b`  
		Last Modified: Wed, 04 Oct 2023 23:56:05 GMT  
		Size: 338.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6efba642676b7f08b17d6c5b657eebe1461166225dd8fd60013ceab2901c4e51`  
		Last Modified: Wed, 04 Oct 2023 23:56:08 GMT  
		Size: 57.7 MB (57708457 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6e706e7799d0736ff1b4df27c3a6703dcbb92134231f84f4fbcf841a201a8968`  
		Last Modified: Wed, 04 Oct 2023 23:56:06 GMT  
		Size: 316.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:94ede8436e0c5c1ba426163ae22d2e78a4449c1f90423be382adc88ef5e7f7df`  
		Last Modified: Wed, 04 Oct 2023 23:56:09 GMT  
		Size: 63.8 MB (63776717 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0433c6008f7b23b7308d19214b170ec2a1320794fad4f14e3089c9e932c73520`  
		Last Modified: Wed, 04 Oct 2023 23:56:07 GMT  
		Size: 5.4 KB (5390 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:8` - unknown; unknown

```console
$ docker pull mysql@sha256:0798fb11106cd915317ee2e883428e8c0509b66ba50c330bc08d98b71a2a4a93
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.1 MB (13139770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:50972c5093bb54a90971a3f64892fb3376c16d66dab33ee483a98b6b83f98382`

```dockerfile
```

-	Layers:
	-	`sha256:0952fb4b6cad899f5e32f2f4c030e7016feffbf1eaa3ee34e5bffc73c7e23b91`  
		Last Modified: Wed, 04 Oct 2023 23:56:05 GMT  
		Size: 13.1 MB (13106170 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:f9ff6e0e61f3655ad5ff5e9c2ebcd98ddbd7fcd1fd289af381f54c15137e50be`  
		Last Modified: Wed, 04 Oct 2023 23:56:03 GMT  
		Size: 33.6 KB (33600 bytes)  
		MIME: application/vnd.in-toto+json

## `mysql:8-oracle`

```console
$ docker pull mysql@sha256:44056c45e214c26c37b6f244534c6fb5f8a40eacbc28e870a2652b19d7a8a814
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
$ docker pull mysql@sha256:2b94677c88791084b0deb390e1966c74f5b6b439c70437587d0ba25f0df52df0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.4 MB (170366065 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54fea0bc79f9c00cc1eb77f4ce9314d116b731d441f86972c6ffeef5987a0429`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 27 Jul 2023 22:18:51 GMT
ADD file:c630310324edbc0dd09d0912b8e7074d17ac71b1be8a14af9663872c081c4632 in / 
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
	-	`sha256:286c1c922769d7608c32cf62931e95d7d169a0306164d24ce7d7a8a065959315`  
		Last Modified: Thu, 21 Sep 2023 23:41:39 GMT  
		Size: 43.7 MB (43657726 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cb7c97478965081773cf774f51b68ba7bc4ddeb1a1c4911ac6dd52e3939a9b02`  
		Last Modified: Wed, 04 Oct 2023 23:56:04 GMT  
		Size: 885.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4056102542df153013330c711c65a022891653dcb4f6b7b8584d32d1cc6ebf65`  
		Last Modified: Wed, 04 Oct 2023 23:56:04 GMT  
		Size: 913.0 KB (912965 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2cfd45c39ba383ddf8f928620c4623faab5bbed0c180b48b176c0361d441a358`  
		Last Modified: Wed, 04 Oct 2023 23:56:04 GMT  
		Size: 4.3 MB (4300663 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:770637688c59082858f7a4a8f12a627c10790774fad0c720ad868e871efcce47`  
		Last Modified: Wed, 04 Oct 2023 23:56:05 GMT  
		Size: 2.6 KB (2608 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5e04d4eff28a3ef1fd9d6816f12752bb2798413e20d7e54f9ac982ce912ea77b`  
		Last Modified: Wed, 04 Oct 2023 23:56:05 GMT  
		Size: 338.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6efba642676b7f08b17d6c5b657eebe1461166225dd8fd60013ceab2901c4e51`  
		Last Modified: Wed, 04 Oct 2023 23:56:08 GMT  
		Size: 57.7 MB (57708457 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6e706e7799d0736ff1b4df27c3a6703dcbb92134231f84f4fbcf841a201a8968`  
		Last Modified: Wed, 04 Oct 2023 23:56:06 GMT  
		Size: 316.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:94ede8436e0c5c1ba426163ae22d2e78a4449c1f90423be382adc88ef5e7f7df`  
		Last Modified: Wed, 04 Oct 2023 23:56:09 GMT  
		Size: 63.8 MB (63776717 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0433c6008f7b23b7308d19214b170ec2a1320794fad4f14e3089c9e932c73520`  
		Last Modified: Wed, 04 Oct 2023 23:56:07 GMT  
		Size: 5.4 KB (5390 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:8-oracle` - unknown; unknown

```console
$ docker pull mysql@sha256:0798fb11106cd915317ee2e883428e8c0509b66ba50c330bc08d98b71a2a4a93
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.1 MB (13139770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:50972c5093bb54a90971a3f64892fb3376c16d66dab33ee483a98b6b83f98382`

```dockerfile
```

-	Layers:
	-	`sha256:0952fb4b6cad899f5e32f2f4c030e7016feffbf1eaa3ee34e5bffc73c7e23b91`  
		Last Modified: Wed, 04 Oct 2023 23:56:05 GMT  
		Size: 13.1 MB (13106170 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:f9ff6e0e61f3655ad5ff5e9c2ebcd98ddbd7fcd1fd289af381f54c15137e50be`  
		Last Modified: Wed, 04 Oct 2023 23:56:03 GMT  
		Size: 33.6 KB (33600 bytes)  
		MIME: application/vnd.in-toto+json

## `mysql:8.0`

```console
$ docker pull mysql@sha256:4753043f21f0297253b35a5809a0ec3f12597e8dbeeb709647307edc943ea7b1
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
$ docker pull mysql@sha256:b53d710ff4601fe53cf3b32369d56b070b7c0b0c4e0a3dac1dae977fac910b8c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.1 MB (170123425 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:00398590b51593720288c6333fe5ece2b6ea5d82149cba4d162fe7bb36458af9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 20 Jul 2023 22:15:44 GMT
ADD file:c630310324edbc0dd09d0912b8e7074d17ac71b1be8a14af9663872c081c4632 in / 
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
	-	`sha256:286c1c922769d7608c32cf62931e95d7d169a0306164d24ce7d7a8a065959315`  
		Last Modified: Thu, 21 Sep 2023 23:41:39 GMT  
		Size: 43.7 MB (43657726 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cb7c97478965081773cf774f51b68ba7bc4ddeb1a1c4911ac6dd52e3939a9b02`  
		Last Modified: Wed, 04 Oct 2023 23:56:04 GMT  
		Size: 885.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4056102542df153013330c711c65a022891653dcb4f6b7b8584d32d1cc6ebf65`  
		Last Modified: Wed, 04 Oct 2023 23:56:04 GMT  
		Size: 913.0 KB (912965 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2cfd45c39ba383ddf8f928620c4623faab5bbed0c180b48b176c0361d441a358`  
		Last Modified: Wed, 04 Oct 2023 23:56:04 GMT  
		Size: 4.3 MB (4300663 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:770637688c59082858f7a4a8f12a627c10790774fad0c720ad868e871efcce47`  
		Last Modified: Wed, 04 Oct 2023 23:56:05 GMT  
		Size: 2.6 KB (2608 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5a861e3d21480520a0263e8face32e49eb171b1613c16872dd768feb0aec2dbb`  
		Last Modified: Wed, 04 Oct 2023 23:58:59 GMT  
		Size: 331.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:195966b431b79cbe375890a7fe72071a917f22b90896e83dbaccd6717df1e445`  
		Last Modified: Wed, 04 Oct 2023 23:59:02 GMT  
		Size: 57.5 MB (57468863 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1b74cd64690d65d2b9d2af078aa671c8182378925e536ed12ddf218e2a561dbe`  
		Last Modified: Wed, 04 Oct 2023 23:58:59 GMT  
		Size: 316.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f200597d6a3533057e94877128f83f74b9e0cdb43d888b8cc08c6f1f17c353e6`  
		Last Modified: Wed, 04 Oct 2023 23:59:02 GMT  
		Size: 63.8 MB (63773557 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:99e4f7fe1d225064a21070d34a38998652a381a335f11f51864952422d831826`  
		Last Modified: Wed, 04 Oct 2023 23:59:00 GMT  
		Size: 5.4 KB (5390 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ec757deb4f034459686537b7107257cd1189e0c830d34ccb8203c6cc41305127`  
		Last Modified: Wed, 04 Oct 2023 23:59:00 GMT  
		Size: 121.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:8.0` - unknown; unknown

```console
$ docker pull mysql@sha256:72d316095c41a3f3c8c3d8df68e03a8ad784f92ec5c59b7d75b20a5d9e0c63e6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.1 MB (13138559 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:578f58724d84493691ee921343f6a337e31581cd00d321b36d29ec2422cd55d2`

```dockerfile
```

-	Layers:
	-	`sha256:ebc5f7d11ffbecb1a549677b243de2438b4ce50411711113f89bec8bf827ba8e`  
		Last Modified: Wed, 04 Oct 2023 23:58:59 GMT  
		Size: 13.1 MB (13104522 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:d4fde13c45b031bac7275b8309a106f8e7bd0a6952e1d812bc04bd6fb8e9bb8f`  
		Last Modified: Wed, 04 Oct 2023 23:58:58 GMT  
		Size: 34.0 KB (34037 bytes)  
		MIME: application/vnd.in-toto+json

## `mysql:8.0-debian`

```console
$ docker pull mysql@sha256:4fffc17d0b3f56a35289dc13d8a8b70d7aef753cdee8b2b156f3d3e58dd00eff
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 2
	-	linux; amd64
	-	unknown; unknown

### `mysql:8.0-debian` - linux; amd64

```console
$ docker pull mysql@sha256:23a7246ec961512baa2c92d2ffb67a19bd720df718c2f54a92d4e977d2be87f0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **179.1 MB (179080557 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4678275e0fe7dcd40b0bf147b20a53d8c8c5690dabf89e0452869ab9066c9caf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 20 Jul 2023 22:15:44 GMT
ADD file:7eb149bcaba1d7dcab06b3f9a0615ca459e9cb28459a0864f92b0037f270ba66 in / 
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
	-	`sha256:7dbc1adf280e1aa588c033eaa746aa6db327ee16be705740f81741f5e6945c86`  
		Last Modified: Wed, 20 Sep 2023 05:01:05 GMT  
		Size: 31.4 MB (31417711 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:29abb1ea03b088ca196333ed77499b0cb4406fa4bf54f7d51eb6ac44a01dc968`  
		Last Modified: Wed, 04 Oct 2023 22:59:00 GMT  
		Size: 1.6 KB (1649 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:36a8d9666cf362bf7d76f6dcf231172b7dc898985a86902c56f243c172efb38b`  
		Last Modified: Wed, 04 Oct 2023 22:59:01 GMT  
		Size: 4.2 MB (4207513 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:dcdc474cb88fc82c8f19747f45e6f3ebe8f2fcc9d83a3eab3500ba6d5e33c3ec`  
		Last Modified: Wed, 04 Oct 2023 22:59:01 GMT  
		Size: 1.5 MB (1471159 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3b033a776030ad4fbdc7cd154072f789ba0d066add90db24edd81c7bcab7d7af`  
		Last Modified: Wed, 04 Oct 2023 22:59:01 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:15723812afb933a58cbd9b9e17e819de68633a8f4c420a7d6a13fbf77e66779d`  
		Last Modified: Wed, 04 Oct 2023 22:59:02 GMT  
		Size: 12.5 MB (12454575 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0ae5ce1000e4ff6042dcb42233625387829666dbfa96d8f6d83ca91bce33519d`  
		Last Modified: Wed, 04 Oct 2023 22:59:01 GMT  
		Size: 2.5 KB (2496 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:193105897b5f0e0f748a55b9c0195e995d780259c69d2f344645520c231c5e84`  
		Last Modified: Wed, 04 Oct 2023 22:59:02 GMT  
		Size: 247.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4a6e741f8760493234908704a3ff106515857de5f513f92d21f923b3c8eab8a9`  
		Last Modified: Wed, 04 Oct 2023 22:59:09 GMT  
		Size: 129.5 MB (129518741 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4d391c4a885e9f6b83e6dc4811d2ac1540e915697cd93155e19e2081bc49289f`  
		Last Modified: Wed, 04 Oct 2023 22:59:02 GMT  
		Size: 840.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d9430eb4818aa63b7c5154be4258f0485caf6d98755c37e069e3008698274dbc`  
		Last Modified: Wed, 04 Oct 2023 22:59:03 GMT  
		Size: 5.4 KB (5389 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e2cd902f2db56164c80a7bb4b7e836a560fb549780dada2e5e2a6126c0905abe`  
		Last Modified: Wed, 04 Oct 2023 22:59:04 GMT  
		Size: 121.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:8.0-debian` - unknown; unknown

```console
$ docker pull mysql@sha256:08ee30921fc4cf06d224872221086d9385f1755aa95768fbd9fd2fb339be3875
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.5 MB (3483922 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e68d4b443ea251a2e68c1400e12b6e5d73b54a0eaae654630c8d14329f57643`

```dockerfile
```

-	Layers:
	-	`sha256:2a324618e23500501709233e59b878570e2d825ab59b68653b05fc31985920d0`  
		Last Modified: Wed, 04 Oct 2023 22:59:01 GMT  
		Size: 3.5 MB (3450633 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:9e5c9c55b5e3796287a31393a38865475b3edfbac4bce507f102cdae3e37d8c3`  
		Last Modified: Wed, 04 Oct 2023 22:59:01 GMT  
		Size: 33.3 KB (33289 bytes)  
		MIME: application/vnd.in-toto+json

## `mysql:8.0-oracle`

```console
$ docker pull mysql@sha256:4753043f21f0297253b35a5809a0ec3f12597e8dbeeb709647307edc943ea7b1
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
$ docker pull mysql@sha256:b53d710ff4601fe53cf3b32369d56b070b7c0b0c4e0a3dac1dae977fac910b8c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.1 MB (170123425 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:00398590b51593720288c6333fe5ece2b6ea5d82149cba4d162fe7bb36458af9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 20 Jul 2023 22:15:44 GMT
ADD file:c630310324edbc0dd09d0912b8e7074d17ac71b1be8a14af9663872c081c4632 in / 
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
	-	`sha256:286c1c922769d7608c32cf62931e95d7d169a0306164d24ce7d7a8a065959315`  
		Last Modified: Thu, 21 Sep 2023 23:41:39 GMT  
		Size: 43.7 MB (43657726 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cb7c97478965081773cf774f51b68ba7bc4ddeb1a1c4911ac6dd52e3939a9b02`  
		Last Modified: Wed, 04 Oct 2023 23:56:04 GMT  
		Size: 885.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4056102542df153013330c711c65a022891653dcb4f6b7b8584d32d1cc6ebf65`  
		Last Modified: Wed, 04 Oct 2023 23:56:04 GMT  
		Size: 913.0 KB (912965 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2cfd45c39ba383ddf8f928620c4623faab5bbed0c180b48b176c0361d441a358`  
		Last Modified: Wed, 04 Oct 2023 23:56:04 GMT  
		Size: 4.3 MB (4300663 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:770637688c59082858f7a4a8f12a627c10790774fad0c720ad868e871efcce47`  
		Last Modified: Wed, 04 Oct 2023 23:56:05 GMT  
		Size: 2.6 KB (2608 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5a861e3d21480520a0263e8face32e49eb171b1613c16872dd768feb0aec2dbb`  
		Last Modified: Wed, 04 Oct 2023 23:58:59 GMT  
		Size: 331.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:195966b431b79cbe375890a7fe72071a917f22b90896e83dbaccd6717df1e445`  
		Last Modified: Wed, 04 Oct 2023 23:59:02 GMT  
		Size: 57.5 MB (57468863 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1b74cd64690d65d2b9d2af078aa671c8182378925e536ed12ddf218e2a561dbe`  
		Last Modified: Wed, 04 Oct 2023 23:58:59 GMT  
		Size: 316.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f200597d6a3533057e94877128f83f74b9e0cdb43d888b8cc08c6f1f17c353e6`  
		Last Modified: Wed, 04 Oct 2023 23:59:02 GMT  
		Size: 63.8 MB (63773557 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:99e4f7fe1d225064a21070d34a38998652a381a335f11f51864952422d831826`  
		Last Modified: Wed, 04 Oct 2023 23:59:00 GMT  
		Size: 5.4 KB (5390 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ec757deb4f034459686537b7107257cd1189e0c830d34ccb8203c6cc41305127`  
		Last Modified: Wed, 04 Oct 2023 23:59:00 GMT  
		Size: 121.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:8.0-oracle` - unknown; unknown

```console
$ docker pull mysql@sha256:72d316095c41a3f3c8c3d8df68e03a8ad784f92ec5c59b7d75b20a5d9e0c63e6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.1 MB (13138559 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:578f58724d84493691ee921343f6a337e31581cd00d321b36d29ec2422cd55d2`

```dockerfile
```

-	Layers:
	-	`sha256:ebc5f7d11ffbecb1a549677b243de2438b4ce50411711113f89bec8bf827ba8e`  
		Last Modified: Wed, 04 Oct 2023 23:58:59 GMT  
		Size: 13.1 MB (13104522 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:d4fde13c45b031bac7275b8309a106f8e7bd0a6952e1d812bc04bd6fb8e9bb8f`  
		Last Modified: Wed, 04 Oct 2023 23:58:58 GMT  
		Size: 34.0 KB (34037 bytes)  
		MIME: application/vnd.in-toto+json

## `mysql:8.0.34`

```console
$ docker pull mysql@sha256:4753043f21f0297253b35a5809a0ec3f12597e8dbeeb709647307edc943ea7b1
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
$ docker pull mysql@sha256:b53d710ff4601fe53cf3b32369d56b070b7c0b0c4e0a3dac1dae977fac910b8c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.1 MB (170123425 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:00398590b51593720288c6333fe5ece2b6ea5d82149cba4d162fe7bb36458af9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 20 Jul 2023 22:15:44 GMT
ADD file:c630310324edbc0dd09d0912b8e7074d17ac71b1be8a14af9663872c081c4632 in / 
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
	-	`sha256:286c1c922769d7608c32cf62931e95d7d169a0306164d24ce7d7a8a065959315`  
		Last Modified: Thu, 21 Sep 2023 23:41:39 GMT  
		Size: 43.7 MB (43657726 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cb7c97478965081773cf774f51b68ba7bc4ddeb1a1c4911ac6dd52e3939a9b02`  
		Last Modified: Wed, 04 Oct 2023 23:56:04 GMT  
		Size: 885.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4056102542df153013330c711c65a022891653dcb4f6b7b8584d32d1cc6ebf65`  
		Last Modified: Wed, 04 Oct 2023 23:56:04 GMT  
		Size: 913.0 KB (912965 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2cfd45c39ba383ddf8f928620c4623faab5bbed0c180b48b176c0361d441a358`  
		Last Modified: Wed, 04 Oct 2023 23:56:04 GMT  
		Size: 4.3 MB (4300663 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:770637688c59082858f7a4a8f12a627c10790774fad0c720ad868e871efcce47`  
		Last Modified: Wed, 04 Oct 2023 23:56:05 GMT  
		Size: 2.6 KB (2608 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5a861e3d21480520a0263e8face32e49eb171b1613c16872dd768feb0aec2dbb`  
		Last Modified: Wed, 04 Oct 2023 23:58:59 GMT  
		Size: 331.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:195966b431b79cbe375890a7fe72071a917f22b90896e83dbaccd6717df1e445`  
		Last Modified: Wed, 04 Oct 2023 23:59:02 GMT  
		Size: 57.5 MB (57468863 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1b74cd64690d65d2b9d2af078aa671c8182378925e536ed12ddf218e2a561dbe`  
		Last Modified: Wed, 04 Oct 2023 23:58:59 GMT  
		Size: 316.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f200597d6a3533057e94877128f83f74b9e0cdb43d888b8cc08c6f1f17c353e6`  
		Last Modified: Wed, 04 Oct 2023 23:59:02 GMT  
		Size: 63.8 MB (63773557 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:99e4f7fe1d225064a21070d34a38998652a381a335f11f51864952422d831826`  
		Last Modified: Wed, 04 Oct 2023 23:59:00 GMT  
		Size: 5.4 KB (5390 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ec757deb4f034459686537b7107257cd1189e0c830d34ccb8203c6cc41305127`  
		Last Modified: Wed, 04 Oct 2023 23:59:00 GMT  
		Size: 121.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:8.0.34` - unknown; unknown

```console
$ docker pull mysql@sha256:72d316095c41a3f3c8c3d8df68e03a8ad784f92ec5c59b7d75b20a5d9e0c63e6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.1 MB (13138559 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:578f58724d84493691ee921343f6a337e31581cd00d321b36d29ec2422cd55d2`

```dockerfile
```

-	Layers:
	-	`sha256:ebc5f7d11ffbecb1a549677b243de2438b4ce50411711113f89bec8bf827ba8e`  
		Last Modified: Wed, 04 Oct 2023 23:58:59 GMT  
		Size: 13.1 MB (13104522 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:d4fde13c45b031bac7275b8309a106f8e7bd0a6952e1d812bc04bd6fb8e9bb8f`  
		Last Modified: Wed, 04 Oct 2023 23:58:58 GMT  
		Size: 34.0 KB (34037 bytes)  
		MIME: application/vnd.in-toto+json

## `mysql:8.0.34-debian`

```console
$ docker pull mysql@sha256:4fffc17d0b3f56a35289dc13d8a8b70d7aef753cdee8b2b156f3d3e58dd00eff
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 2
	-	linux; amd64
	-	unknown; unknown

### `mysql:8.0.34-debian` - linux; amd64

```console
$ docker pull mysql@sha256:23a7246ec961512baa2c92d2ffb67a19bd720df718c2f54a92d4e977d2be87f0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **179.1 MB (179080557 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4678275e0fe7dcd40b0bf147b20a53d8c8c5690dabf89e0452869ab9066c9caf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 20 Jul 2023 22:15:44 GMT
ADD file:7eb149bcaba1d7dcab06b3f9a0615ca459e9cb28459a0864f92b0037f270ba66 in / 
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
	-	`sha256:7dbc1adf280e1aa588c033eaa746aa6db327ee16be705740f81741f5e6945c86`  
		Last Modified: Wed, 20 Sep 2023 05:01:05 GMT  
		Size: 31.4 MB (31417711 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:29abb1ea03b088ca196333ed77499b0cb4406fa4bf54f7d51eb6ac44a01dc968`  
		Last Modified: Wed, 04 Oct 2023 22:59:00 GMT  
		Size: 1.6 KB (1649 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:36a8d9666cf362bf7d76f6dcf231172b7dc898985a86902c56f243c172efb38b`  
		Last Modified: Wed, 04 Oct 2023 22:59:01 GMT  
		Size: 4.2 MB (4207513 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:dcdc474cb88fc82c8f19747f45e6f3ebe8f2fcc9d83a3eab3500ba6d5e33c3ec`  
		Last Modified: Wed, 04 Oct 2023 22:59:01 GMT  
		Size: 1.5 MB (1471159 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3b033a776030ad4fbdc7cd154072f789ba0d066add90db24edd81c7bcab7d7af`  
		Last Modified: Wed, 04 Oct 2023 22:59:01 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:15723812afb933a58cbd9b9e17e819de68633a8f4c420a7d6a13fbf77e66779d`  
		Last Modified: Wed, 04 Oct 2023 22:59:02 GMT  
		Size: 12.5 MB (12454575 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0ae5ce1000e4ff6042dcb42233625387829666dbfa96d8f6d83ca91bce33519d`  
		Last Modified: Wed, 04 Oct 2023 22:59:01 GMT  
		Size: 2.5 KB (2496 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:193105897b5f0e0f748a55b9c0195e995d780259c69d2f344645520c231c5e84`  
		Last Modified: Wed, 04 Oct 2023 22:59:02 GMT  
		Size: 247.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4a6e741f8760493234908704a3ff106515857de5f513f92d21f923b3c8eab8a9`  
		Last Modified: Wed, 04 Oct 2023 22:59:09 GMT  
		Size: 129.5 MB (129518741 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4d391c4a885e9f6b83e6dc4811d2ac1540e915697cd93155e19e2081bc49289f`  
		Last Modified: Wed, 04 Oct 2023 22:59:02 GMT  
		Size: 840.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d9430eb4818aa63b7c5154be4258f0485caf6d98755c37e069e3008698274dbc`  
		Last Modified: Wed, 04 Oct 2023 22:59:03 GMT  
		Size: 5.4 KB (5389 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e2cd902f2db56164c80a7bb4b7e836a560fb549780dada2e5e2a6126c0905abe`  
		Last Modified: Wed, 04 Oct 2023 22:59:04 GMT  
		Size: 121.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:8.0.34-debian` - unknown; unknown

```console
$ docker pull mysql@sha256:08ee30921fc4cf06d224872221086d9385f1755aa95768fbd9fd2fb339be3875
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.5 MB (3483922 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e68d4b443ea251a2e68c1400e12b6e5d73b54a0eaae654630c8d14329f57643`

```dockerfile
```

-	Layers:
	-	`sha256:2a324618e23500501709233e59b878570e2d825ab59b68653b05fc31985920d0`  
		Last Modified: Wed, 04 Oct 2023 22:59:01 GMT  
		Size: 3.5 MB (3450633 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:9e5c9c55b5e3796287a31393a38865475b3edfbac4bce507f102cdae3e37d8c3`  
		Last Modified: Wed, 04 Oct 2023 22:59:01 GMT  
		Size: 33.3 KB (33289 bytes)  
		MIME: application/vnd.in-toto+json

## `mysql:8.0.34-oracle`

```console
$ docker pull mysql@sha256:4753043f21f0297253b35a5809a0ec3f12597e8dbeeb709647307edc943ea7b1
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
$ docker pull mysql@sha256:b53d710ff4601fe53cf3b32369d56b070b7c0b0c4e0a3dac1dae977fac910b8c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.1 MB (170123425 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:00398590b51593720288c6333fe5ece2b6ea5d82149cba4d162fe7bb36458af9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 20 Jul 2023 22:15:44 GMT
ADD file:c630310324edbc0dd09d0912b8e7074d17ac71b1be8a14af9663872c081c4632 in / 
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
	-	`sha256:286c1c922769d7608c32cf62931e95d7d169a0306164d24ce7d7a8a065959315`  
		Last Modified: Thu, 21 Sep 2023 23:41:39 GMT  
		Size: 43.7 MB (43657726 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cb7c97478965081773cf774f51b68ba7bc4ddeb1a1c4911ac6dd52e3939a9b02`  
		Last Modified: Wed, 04 Oct 2023 23:56:04 GMT  
		Size: 885.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4056102542df153013330c711c65a022891653dcb4f6b7b8584d32d1cc6ebf65`  
		Last Modified: Wed, 04 Oct 2023 23:56:04 GMT  
		Size: 913.0 KB (912965 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2cfd45c39ba383ddf8f928620c4623faab5bbed0c180b48b176c0361d441a358`  
		Last Modified: Wed, 04 Oct 2023 23:56:04 GMT  
		Size: 4.3 MB (4300663 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:770637688c59082858f7a4a8f12a627c10790774fad0c720ad868e871efcce47`  
		Last Modified: Wed, 04 Oct 2023 23:56:05 GMT  
		Size: 2.6 KB (2608 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5a861e3d21480520a0263e8face32e49eb171b1613c16872dd768feb0aec2dbb`  
		Last Modified: Wed, 04 Oct 2023 23:58:59 GMT  
		Size: 331.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:195966b431b79cbe375890a7fe72071a917f22b90896e83dbaccd6717df1e445`  
		Last Modified: Wed, 04 Oct 2023 23:59:02 GMT  
		Size: 57.5 MB (57468863 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1b74cd64690d65d2b9d2af078aa671c8182378925e536ed12ddf218e2a561dbe`  
		Last Modified: Wed, 04 Oct 2023 23:58:59 GMT  
		Size: 316.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f200597d6a3533057e94877128f83f74b9e0cdb43d888b8cc08c6f1f17c353e6`  
		Last Modified: Wed, 04 Oct 2023 23:59:02 GMT  
		Size: 63.8 MB (63773557 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:99e4f7fe1d225064a21070d34a38998652a381a335f11f51864952422d831826`  
		Last Modified: Wed, 04 Oct 2023 23:59:00 GMT  
		Size: 5.4 KB (5390 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ec757deb4f034459686537b7107257cd1189e0c830d34ccb8203c6cc41305127`  
		Last Modified: Wed, 04 Oct 2023 23:59:00 GMT  
		Size: 121.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:8.0.34-oracle` - unknown; unknown

```console
$ docker pull mysql@sha256:72d316095c41a3f3c8c3d8df68e03a8ad784f92ec5c59b7d75b20a5d9e0c63e6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.1 MB (13138559 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:578f58724d84493691ee921343f6a337e31581cd00d321b36d29ec2422cd55d2`

```dockerfile
```

-	Layers:
	-	`sha256:ebc5f7d11ffbecb1a549677b243de2438b4ce50411711113f89bec8bf827ba8e`  
		Last Modified: Wed, 04 Oct 2023 23:58:59 GMT  
		Size: 13.1 MB (13104522 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:d4fde13c45b031bac7275b8309a106f8e7bd0a6952e1d812bc04bd6fb8e9bb8f`  
		Last Modified: Wed, 04 Oct 2023 23:58:58 GMT  
		Size: 34.0 KB (34037 bytes)  
		MIME: application/vnd.in-toto+json

## `mysql:8.1`

```console
$ docker pull mysql@sha256:44056c45e214c26c37b6f244534c6fb5f8a40eacbc28e870a2652b19d7a8a814
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
$ docker pull mysql@sha256:2b94677c88791084b0deb390e1966c74f5b6b439c70437587d0ba25f0df52df0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.4 MB (170366065 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54fea0bc79f9c00cc1eb77f4ce9314d116b731d441f86972c6ffeef5987a0429`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 27 Jul 2023 22:18:51 GMT
ADD file:c630310324edbc0dd09d0912b8e7074d17ac71b1be8a14af9663872c081c4632 in / 
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
	-	`sha256:286c1c922769d7608c32cf62931e95d7d169a0306164d24ce7d7a8a065959315`  
		Last Modified: Thu, 21 Sep 2023 23:41:39 GMT  
		Size: 43.7 MB (43657726 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cb7c97478965081773cf774f51b68ba7bc4ddeb1a1c4911ac6dd52e3939a9b02`  
		Last Modified: Wed, 04 Oct 2023 23:56:04 GMT  
		Size: 885.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4056102542df153013330c711c65a022891653dcb4f6b7b8584d32d1cc6ebf65`  
		Last Modified: Wed, 04 Oct 2023 23:56:04 GMT  
		Size: 913.0 KB (912965 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2cfd45c39ba383ddf8f928620c4623faab5bbed0c180b48b176c0361d441a358`  
		Last Modified: Wed, 04 Oct 2023 23:56:04 GMT  
		Size: 4.3 MB (4300663 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:770637688c59082858f7a4a8f12a627c10790774fad0c720ad868e871efcce47`  
		Last Modified: Wed, 04 Oct 2023 23:56:05 GMT  
		Size: 2.6 KB (2608 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5e04d4eff28a3ef1fd9d6816f12752bb2798413e20d7e54f9ac982ce912ea77b`  
		Last Modified: Wed, 04 Oct 2023 23:56:05 GMT  
		Size: 338.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6efba642676b7f08b17d6c5b657eebe1461166225dd8fd60013ceab2901c4e51`  
		Last Modified: Wed, 04 Oct 2023 23:56:08 GMT  
		Size: 57.7 MB (57708457 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6e706e7799d0736ff1b4df27c3a6703dcbb92134231f84f4fbcf841a201a8968`  
		Last Modified: Wed, 04 Oct 2023 23:56:06 GMT  
		Size: 316.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:94ede8436e0c5c1ba426163ae22d2e78a4449c1f90423be382adc88ef5e7f7df`  
		Last Modified: Wed, 04 Oct 2023 23:56:09 GMT  
		Size: 63.8 MB (63776717 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0433c6008f7b23b7308d19214b170ec2a1320794fad4f14e3089c9e932c73520`  
		Last Modified: Wed, 04 Oct 2023 23:56:07 GMT  
		Size: 5.4 KB (5390 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:8.1` - unknown; unknown

```console
$ docker pull mysql@sha256:0798fb11106cd915317ee2e883428e8c0509b66ba50c330bc08d98b71a2a4a93
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.1 MB (13139770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:50972c5093bb54a90971a3f64892fb3376c16d66dab33ee483a98b6b83f98382`

```dockerfile
```

-	Layers:
	-	`sha256:0952fb4b6cad899f5e32f2f4c030e7016feffbf1eaa3ee34e5bffc73c7e23b91`  
		Last Modified: Wed, 04 Oct 2023 23:56:05 GMT  
		Size: 13.1 MB (13106170 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:f9ff6e0e61f3655ad5ff5e9c2ebcd98ddbd7fcd1fd289af381f54c15137e50be`  
		Last Modified: Wed, 04 Oct 2023 23:56:03 GMT  
		Size: 33.6 KB (33600 bytes)  
		MIME: application/vnd.in-toto+json

## `mysql:8.1-oracle`

```console
$ docker pull mysql@sha256:44056c45e214c26c37b6f244534c6fb5f8a40eacbc28e870a2652b19d7a8a814
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
$ docker pull mysql@sha256:2b94677c88791084b0deb390e1966c74f5b6b439c70437587d0ba25f0df52df0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.4 MB (170366065 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54fea0bc79f9c00cc1eb77f4ce9314d116b731d441f86972c6ffeef5987a0429`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 27 Jul 2023 22:18:51 GMT
ADD file:c630310324edbc0dd09d0912b8e7074d17ac71b1be8a14af9663872c081c4632 in / 
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
	-	`sha256:286c1c922769d7608c32cf62931e95d7d169a0306164d24ce7d7a8a065959315`  
		Last Modified: Thu, 21 Sep 2023 23:41:39 GMT  
		Size: 43.7 MB (43657726 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cb7c97478965081773cf774f51b68ba7bc4ddeb1a1c4911ac6dd52e3939a9b02`  
		Last Modified: Wed, 04 Oct 2023 23:56:04 GMT  
		Size: 885.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4056102542df153013330c711c65a022891653dcb4f6b7b8584d32d1cc6ebf65`  
		Last Modified: Wed, 04 Oct 2023 23:56:04 GMT  
		Size: 913.0 KB (912965 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2cfd45c39ba383ddf8f928620c4623faab5bbed0c180b48b176c0361d441a358`  
		Last Modified: Wed, 04 Oct 2023 23:56:04 GMT  
		Size: 4.3 MB (4300663 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:770637688c59082858f7a4a8f12a627c10790774fad0c720ad868e871efcce47`  
		Last Modified: Wed, 04 Oct 2023 23:56:05 GMT  
		Size: 2.6 KB (2608 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5e04d4eff28a3ef1fd9d6816f12752bb2798413e20d7e54f9ac982ce912ea77b`  
		Last Modified: Wed, 04 Oct 2023 23:56:05 GMT  
		Size: 338.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6efba642676b7f08b17d6c5b657eebe1461166225dd8fd60013ceab2901c4e51`  
		Last Modified: Wed, 04 Oct 2023 23:56:08 GMT  
		Size: 57.7 MB (57708457 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6e706e7799d0736ff1b4df27c3a6703dcbb92134231f84f4fbcf841a201a8968`  
		Last Modified: Wed, 04 Oct 2023 23:56:06 GMT  
		Size: 316.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:94ede8436e0c5c1ba426163ae22d2e78a4449c1f90423be382adc88ef5e7f7df`  
		Last Modified: Wed, 04 Oct 2023 23:56:09 GMT  
		Size: 63.8 MB (63776717 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0433c6008f7b23b7308d19214b170ec2a1320794fad4f14e3089c9e932c73520`  
		Last Modified: Wed, 04 Oct 2023 23:56:07 GMT  
		Size: 5.4 KB (5390 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:8.1-oracle` - unknown; unknown

```console
$ docker pull mysql@sha256:0798fb11106cd915317ee2e883428e8c0509b66ba50c330bc08d98b71a2a4a93
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.1 MB (13139770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:50972c5093bb54a90971a3f64892fb3376c16d66dab33ee483a98b6b83f98382`

```dockerfile
```

-	Layers:
	-	`sha256:0952fb4b6cad899f5e32f2f4c030e7016feffbf1eaa3ee34e5bffc73c7e23b91`  
		Last Modified: Wed, 04 Oct 2023 23:56:05 GMT  
		Size: 13.1 MB (13106170 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:f9ff6e0e61f3655ad5ff5e9c2ebcd98ddbd7fcd1fd289af381f54c15137e50be`  
		Last Modified: Wed, 04 Oct 2023 23:56:03 GMT  
		Size: 33.6 KB (33600 bytes)  
		MIME: application/vnd.in-toto+json

## `mysql:8.1.0`

```console
$ docker pull mysql@sha256:44056c45e214c26c37b6f244534c6fb5f8a40eacbc28e870a2652b19d7a8a814
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
$ docker pull mysql@sha256:2b94677c88791084b0deb390e1966c74f5b6b439c70437587d0ba25f0df52df0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.4 MB (170366065 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54fea0bc79f9c00cc1eb77f4ce9314d116b731d441f86972c6ffeef5987a0429`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 27 Jul 2023 22:18:51 GMT
ADD file:c630310324edbc0dd09d0912b8e7074d17ac71b1be8a14af9663872c081c4632 in / 
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
	-	`sha256:286c1c922769d7608c32cf62931e95d7d169a0306164d24ce7d7a8a065959315`  
		Last Modified: Thu, 21 Sep 2023 23:41:39 GMT  
		Size: 43.7 MB (43657726 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cb7c97478965081773cf774f51b68ba7bc4ddeb1a1c4911ac6dd52e3939a9b02`  
		Last Modified: Wed, 04 Oct 2023 23:56:04 GMT  
		Size: 885.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4056102542df153013330c711c65a022891653dcb4f6b7b8584d32d1cc6ebf65`  
		Last Modified: Wed, 04 Oct 2023 23:56:04 GMT  
		Size: 913.0 KB (912965 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2cfd45c39ba383ddf8f928620c4623faab5bbed0c180b48b176c0361d441a358`  
		Last Modified: Wed, 04 Oct 2023 23:56:04 GMT  
		Size: 4.3 MB (4300663 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:770637688c59082858f7a4a8f12a627c10790774fad0c720ad868e871efcce47`  
		Last Modified: Wed, 04 Oct 2023 23:56:05 GMT  
		Size: 2.6 KB (2608 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5e04d4eff28a3ef1fd9d6816f12752bb2798413e20d7e54f9ac982ce912ea77b`  
		Last Modified: Wed, 04 Oct 2023 23:56:05 GMT  
		Size: 338.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6efba642676b7f08b17d6c5b657eebe1461166225dd8fd60013ceab2901c4e51`  
		Last Modified: Wed, 04 Oct 2023 23:56:08 GMT  
		Size: 57.7 MB (57708457 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6e706e7799d0736ff1b4df27c3a6703dcbb92134231f84f4fbcf841a201a8968`  
		Last Modified: Wed, 04 Oct 2023 23:56:06 GMT  
		Size: 316.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:94ede8436e0c5c1ba426163ae22d2e78a4449c1f90423be382adc88ef5e7f7df`  
		Last Modified: Wed, 04 Oct 2023 23:56:09 GMT  
		Size: 63.8 MB (63776717 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0433c6008f7b23b7308d19214b170ec2a1320794fad4f14e3089c9e932c73520`  
		Last Modified: Wed, 04 Oct 2023 23:56:07 GMT  
		Size: 5.4 KB (5390 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:8.1.0` - unknown; unknown

```console
$ docker pull mysql@sha256:0798fb11106cd915317ee2e883428e8c0509b66ba50c330bc08d98b71a2a4a93
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.1 MB (13139770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:50972c5093bb54a90971a3f64892fb3376c16d66dab33ee483a98b6b83f98382`

```dockerfile
```

-	Layers:
	-	`sha256:0952fb4b6cad899f5e32f2f4c030e7016feffbf1eaa3ee34e5bffc73c7e23b91`  
		Last Modified: Wed, 04 Oct 2023 23:56:05 GMT  
		Size: 13.1 MB (13106170 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:f9ff6e0e61f3655ad5ff5e9c2ebcd98ddbd7fcd1fd289af381f54c15137e50be`  
		Last Modified: Wed, 04 Oct 2023 23:56:03 GMT  
		Size: 33.6 KB (33600 bytes)  
		MIME: application/vnd.in-toto+json

## `mysql:8.1.0-oracle`

```console
$ docker pull mysql@sha256:44056c45e214c26c37b6f244534c6fb5f8a40eacbc28e870a2652b19d7a8a814
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
$ docker pull mysql@sha256:2b94677c88791084b0deb390e1966c74f5b6b439c70437587d0ba25f0df52df0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.4 MB (170366065 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54fea0bc79f9c00cc1eb77f4ce9314d116b731d441f86972c6ffeef5987a0429`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 27 Jul 2023 22:18:51 GMT
ADD file:c630310324edbc0dd09d0912b8e7074d17ac71b1be8a14af9663872c081c4632 in / 
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
	-	`sha256:286c1c922769d7608c32cf62931e95d7d169a0306164d24ce7d7a8a065959315`  
		Last Modified: Thu, 21 Sep 2023 23:41:39 GMT  
		Size: 43.7 MB (43657726 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cb7c97478965081773cf774f51b68ba7bc4ddeb1a1c4911ac6dd52e3939a9b02`  
		Last Modified: Wed, 04 Oct 2023 23:56:04 GMT  
		Size: 885.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4056102542df153013330c711c65a022891653dcb4f6b7b8584d32d1cc6ebf65`  
		Last Modified: Wed, 04 Oct 2023 23:56:04 GMT  
		Size: 913.0 KB (912965 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2cfd45c39ba383ddf8f928620c4623faab5bbed0c180b48b176c0361d441a358`  
		Last Modified: Wed, 04 Oct 2023 23:56:04 GMT  
		Size: 4.3 MB (4300663 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:770637688c59082858f7a4a8f12a627c10790774fad0c720ad868e871efcce47`  
		Last Modified: Wed, 04 Oct 2023 23:56:05 GMT  
		Size: 2.6 KB (2608 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5e04d4eff28a3ef1fd9d6816f12752bb2798413e20d7e54f9ac982ce912ea77b`  
		Last Modified: Wed, 04 Oct 2023 23:56:05 GMT  
		Size: 338.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6efba642676b7f08b17d6c5b657eebe1461166225dd8fd60013ceab2901c4e51`  
		Last Modified: Wed, 04 Oct 2023 23:56:08 GMT  
		Size: 57.7 MB (57708457 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6e706e7799d0736ff1b4df27c3a6703dcbb92134231f84f4fbcf841a201a8968`  
		Last Modified: Wed, 04 Oct 2023 23:56:06 GMT  
		Size: 316.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:94ede8436e0c5c1ba426163ae22d2e78a4449c1f90423be382adc88ef5e7f7df`  
		Last Modified: Wed, 04 Oct 2023 23:56:09 GMT  
		Size: 63.8 MB (63776717 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0433c6008f7b23b7308d19214b170ec2a1320794fad4f14e3089c9e932c73520`  
		Last Modified: Wed, 04 Oct 2023 23:56:07 GMT  
		Size: 5.4 KB (5390 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:8.1.0-oracle` - unknown; unknown

```console
$ docker pull mysql@sha256:0798fb11106cd915317ee2e883428e8c0509b66ba50c330bc08d98b71a2a4a93
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.1 MB (13139770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:50972c5093bb54a90971a3f64892fb3376c16d66dab33ee483a98b6b83f98382`

```dockerfile
```

-	Layers:
	-	`sha256:0952fb4b6cad899f5e32f2f4c030e7016feffbf1eaa3ee34e5bffc73c7e23b91`  
		Last Modified: Wed, 04 Oct 2023 23:56:05 GMT  
		Size: 13.1 MB (13106170 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:f9ff6e0e61f3655ad5ff5e9c2ebcd98ddbd7fcd1fd289af381f54c15137e50be`  
		Last Modified: Wed, 04 Oct 2023 23:56:03 GMT  
		Size: 33.6 KB (33600 bytes)  
		MIME: application/vnd.in-toto+json

## `mysql:innovation`

```console
$ docker pull mysql@sha256:44056c45e214c26c37b6f244534c6fb5f8a40eacbc28e870a2652b19d7a8a814
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
$ docker pull mysql@sha256:2b94677c88791084b0deb390e1966c74f5b6b439c70437587d0ba25f0df52df0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.4 MB (170366065 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54fea0bc79f9c00cc1eb77f4ce9314d116b731d441f86972c6ffeef5987a0429`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 27 Jul 2023 22:18:51 GMT
ADD file:c630310324edbc0dd09d0912b8e7074d17ac71b1be8a14af9663872c081c4632 in / 
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
	-	`sha256:286c1c922769d7608c32cf62931e95d7d169a0306164d24ce7d7a8a065959315`  
		Last Modified: Thu, 21 Sep 2023 23:41:39 GMT  
		Size: 43.7 MB (43657726 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cb7c97478965081773cf774f51b68ba7bc4ddeb1a1c4911ac6dd52e3939a9b02`  
		Last Modified: Wed, 04 Oct 2023 23:56:04 GMT  
		Size: 885.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4056102542df153013330c711c65a022891653dcb4f6b7b8584d32d1cc6ebf65`  
		Last Modified: Wed, 04 Oct 2023 23:56:04 GMT  
		Size: 913.0 KB (912965 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2cfd45c39ba383ddf8f928620c4623faab5bbed0c180b48b176c0361d441a358`  
		Last Modified: Wed, 04 Oct 2023 23:56:04 GMT  
		Size: 4.3 MB (4300663 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:770637688c59082858f7a4a8f12a627c10790774fad0c720ad868e871efcce47`  
		Last Modified: Wed, 04 Oct 2023 23:56:05 GMT  
		Size: 2.6 KB (2608 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5e04d4eff28a3ef1fd9d6816f12752bb2798413e20d7e54f9ac982ce912ea77b`  
		Last Modified: Wed, 04 Oct 2023 23:56:05 GMT  
		Size: 338.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6efba642676b7f08b17d6c5b657eebe1461166225dd8fd60013ceab2901c4e51`  
		Last Modified: Wed, 04 Oct 2023 23:56:08 GMT  
		Size: 57.7 MB (57708457 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6e706e7799d0736ff1b4df27c3a6703dcbb92134231f84f4fbcf841a201a8968`  
		Last Modified: Wed, 04 Oct 2023 23:56:06 GMT  
		Size: 316.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:94ede8436e0c5c1ba426163ae22d2e78a4449c1f90423be382adc88ef5e7f7df`  
		Last Modified: Wed, 04 Oct 2023 23:56:09 GMT  
		Size: 63.8 MB (63776717 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0433c6008f7b23b7308d19214b170ec2a1320794fad4f14e3089c9e932c73520`  
		Last Modified: Wed, 04 Oct 2023 23:56:07 GMT  
		Size: 5.4 KB (5390 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:innovation` - unknown; unknown

```console
$ docker pull mysql@sha256:0798fb11106cd915317ee2e883428e8c0509b66ba50c330bc08d98b71a2a4a93
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.1 MB (13139770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:50972c5093bb54a90971a3f64892fb3376c16d66dab33ee483a98b6b83f98382`

```dockerfile
```

-	Layers:
	-	`sha256:0952fb4b6cad899f5e32f2f4c030e7016feffbf1eaa3ee34e5bffc73c7e23b91`  
		Last Modified: Wed, 04 Oct 2023 23:56:05 GMT  
		Size: 13.1 MB (13106170 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:f9ff6e0e61f3655ad5ff5e9c2ebcd98ddbd7fcd1fd289af381f54c15137e50be`  
		Last Modified: Wed, 04 Oct 2023 23:56:03 GMT  
		Size: 33.6 KB (33600 bytes)  
		MIME: application/vnd.in-toto+json

## `mysql:innovation-oracle`

```console
$ docker pull mysql@sha256:44056c45e214c26c37b6f244534c6fb5f8a40eacbc28e870a2652b19d7a8a814
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
$ docker pull mysql@sha256:2b94677c88791084b0deb390e1966c74f5b6b439c70437587d0ba25f0df52df0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.4 MB (170366065 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54fea0bc79f9c00cc1eb77f4ce9314d116b731d441f86972c6ffeef5987a0429`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 27 Jul 2023 22:18:51 GMT
ADD file:c630310324edbc0dd09d0912b8e7074d17ac71b1be8a14af9663872c081c4632 in / 
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
	-	`sha256:286c1c922769d7608c32cf62931e95d7d169a0306164d24ce7d7a8a065959315`  
		Last Modified: Thu, 21 Sep 2023 23:41:39 GMT  
		Size: 43.7 MB (43657726 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cb7c97478965081773cf774f51b68ba7bc4ddeb1a1c4911ac6dd52e3939a9b02`  
		Last Modified: Wed, 04 Oct 2023 23:56:04 GMT  
		Size: 885.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4056102542df153013330c711c65a022891653dcb4f6b7b8584d32d1cc6ebf65`  
		Last Modified: Wed, 04 Oct 2023 23:56:04 GMT  
		Size: 913.0 KB (912965 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2cfd45c39ba383ddf8f928620c4623faab5bbed0c180b48b176c0361d441a358`  
		Last Modified: Wed, 04 Oct 2023 23:56:04 GMT  
		Size: 4.3 MB (4300663 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:770637688c59082858f7a4a8f12a627c10790774fad0c720ad868e871efcce47`  
		Last Modified: Wed, 04 Oct 2023 23:56:05 GMT  
		Size: 2.6 KB (2608 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5e04d4eff28a3ef1fd9d6816f12752bb2798413e20d7e54f9ac982ce912ea77b`  
		Last Modified: Wed, 04 Oct 2023 23:56:05 GMT  
		Size: 338.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6efba642676b7f08b17d6c5b657eebe1461166225dd8fd60013ceab2901c4e51`  
		Last Modified: Wed, 04 Oct 2023 23:56:08 GMT  
		Size: 57.7 MB (57708457 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6e706e7799d0736ff1b4df27c3a6703dcbb92134231f84f4fbcf841a201a8968`  
		Last Modified: Wed, 04 Oct 2023 23:56:06 GMT  
		Size: 316.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:94ede8436e0c5c1ba426163ae22d2e78a4449c1f90423be382adc88ef5e7f7df`  
		Last Modified: Wed, 04 Oct 2023 23:56:09 GMT  
		Size: 63.8 MB (63776717 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0433c6008f7b23b7308d19214b170ec2a1320794fad4f14e3089c9e932c73520`  
		Last Modified: Wed, 04 Oct 2023 23:56:07 GMT  
		Size: 5.4 KB (5390 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:innovation-oracle` - unknown; unknown

```console
$ docker pull mysql@sha256:0798fb11106cd915317ee2e883428e8c0509b66ba50c330bc08d98b71a2a4a93
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.1 MB (13139770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:50972c5093bb54a90971a3f64892fb3376c16d66dab33ee483a98b6b83f98382`

```dockerfile
```

-	Layers:
	-	`sha256:0952fb4b6cad899f5e32f2f4c030e7016feffbf1eaa3ee34e5bffc73c7e23b91`  
		Last Modified: Wed, 04 Oct 2023 23:56:05 GMT  
		Size: 13.1 MB (13106170 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:f9ff6e0e61f3655ad5ff5e9c2ebcd98ddbd7fcd1fd289af381f54c15137e50be`  
		Last Modified: Wed, 04 Oct 2023 23:56:03 GMT  
		Size: 33.6 KB (33600 bytes)  
		MIME: application/vnd.in-toto+json

## `mysql:latest`

```console
$ docker pull mysql@sha256:44056c45e214c26c37b6f244534c6fb5f8a40eacbc28e870a2652b19d7a8a814
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
$ docker pull mysql@sha256:2b94677c88791084b0deb390e1966c74f5b6b439c70437587d0ba25f0df52df0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.4 MB (170366065 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54fea0bc79f9c00cc1eb77f4ce9314d116b731d441f86972c6ffeef5987a0429`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 27 Jul 2023 22:18:51 GMT
ADD file:c630310324edbc0dd09d0912b8e7074d17ac71b1be8a14af9663872c081c4632 in / 
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
	-	`sha256:286c1c922769d7608c32cf62931e95d7d169a0306164d24ce7d7a8a065959315`  
		Last Modified: Thu, 21 Sep 2023 23:41:39 GMT  
		Size: 43.7 MB (43657726 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cb7c97478965081773cf774f51b68ba7bc4ddeb1a1c4911ac6dd52e3939a9b02`  
		Last Modified: Wed, 04 Oct 2023 23:56:04 GMT  
		Size: 885.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4056102542df153013330c711c65a022891653dcb4f6b7b8584d32d1cc6ebf65`  
		Last Modified: Wed, 04 Oct 2023 23:56:04 GMT  
		Size: 913.0 KB (912965 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2cfd45c39ba383ddf8f928620c4623faab5bbed0c180b48b176c0361d441a358`  
		Last Modified: Wed, 04 Oct 2023 23:56:04 GMT  
		Size: 4.3 MB (4300663 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:770637688c59082858f7a4a8f12a627c10790774fad0c720ad868e871efcce47`  
		Last Modified: Wed, 04 Oct 2023 23:56:05 GMT  
		Size: 2.6 KB (2608 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5e04d4eff28a3ef1fd9d6816f12752bb2798413e20d7e54f9ac982ce912ea77b`  
		Last Modified: Wed, 04 Oct 2023 23:56:05 GMT  
		Size: 338.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6efba642676b7f08b17d6c5b657eebe1461166225dd8fd60013ceab2901c4e51`  
		Last Modified: Wed, 04 Oct 2023 23:56:08 GMT  
		Size: 57.7 MB (57708457 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6e706e7799d0736ff1b4df27c3a6703dcbb92134231f84f4fbcf841a201a8968`  
		Last Modified: Wed, 04 Oct 2023 23:56:06 GMT  
		Size: 316.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:94ede8436e0c5c1ba426163ae22d2e78a4449c1f90423be382adc88ef5e7f7df`  
		Last Modified: Wed, 04 Oct 2023 23:56:09 GMT  
		Size: 63.8 MB (63776717 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0433c6008f7b23b7308d19214b170ec2a1320794fad4f14e3089c9e932c73520`  
		Last Modified: Wed, 04 Oct 2023 23:56:07 GMT  
		Size: 5.4 KB (5390 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:latest` - unknown; unknown

```console
$ docker pull mysql@sha256:0798fb11106cd915317ee2e883428e8c0509b66ba50c330bc08d98b71a2a4a93
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.1 MB (13139770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:50972c5093bb54a90971a3f64892fb3376c16d66dab33ee483a98b6b83f98382`

```dockerfile
```

-	Layers:
	-	`sha256:0952fb4b6cad899f5e32f2f4c030e7016feffbf1eaa3ee34e5bffc73c7e23b91`  
		Last Modified: Wed, 04 Oct 2023 23:56:05 GMT  
		Size: 13.1 MB (13106170 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:f9ff6e0e61f3655ad5ff5e9c2ebcd98ddbd7fcd1fd289af381f54c15137e50be`  
		Last Modified: Wed, 04 Oct 2023 23:56:03 GMT  
		Size: 33.6 KB (33600 bytes)  
		MIME: application/vnd.in-toto+json

## `mysql:oracle`

```console
$ docker pull mysql@sha256:44056c45e214c26c37b6f244534c6fb5f8a40eacbc28e870a2652b19d7a8a814
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
$ docker pull mysql@sha256:2b94677c88791084b0deb390e1966c74f5b6b439c70437587d0ba25f0df52df0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.4 MB (170366065 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54fea0bc79f9c00cc1eb77f4ce9314d116b731d441f86972c6ffeef5987a0429`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 27 Jul 2023 22:18:51 GMT
ADD file:c630310324edbc0dd09d0912b8e7074d17ac71b1be8a14af9663872c081c4632 in / 
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
	-	`sha256:286c1c922769d7608c32cf62931e95d7d169a0306164d24ce7d7a8a065959315`  
		Last Modified: Thu, 21 Sep 2023 23:41:39 GMT  
		Size: 43.7 MB (43657726 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cb7c97478965081773cf774f51b68ba7bc4ddeb1a1c4911ac6dd52e3939a9b02`  
		Last Modified: Wed, 04 Oct 2023 23:56:04 GMT  
		Size: 885.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4056102542df153013330c711c65a022891653dcb4f6b7b8584d32d1cc6ebf65`  
		Last Modified: Wed, 04 Oct 2023 23:56:04 GMT  
		Size: 913.0 KB (912965 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2cfd45c39ba383ddf8f928620c4623faab5bbed0c180b48b176c0361d441a358`  
		Last Modified: Wed, 04 Oct 2023 23:56:04 GMT  
		Size: 4.3 MB (4300663 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:770637688c59082858f7a4a8f12a627c10790774fad0c720ad868e871efcce47`  
		Last Modified: Wed, 04 Oct 2023 23:56:05 GMT  
		Size: 2.6 KB (2608 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5e04d4eff28a3ef1fd9d6816f12752bb2798413e20d7e54f9ac982ce912ea77b`  
		Last Modified: Wed, 04 Oct 2023 23:56:05 GMT  
		Size: 338.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6efba642676b7f08b17d6c5b657eebe1461166225dd8fd60013ceab2901c4e51`  
		Last Modified: Wed, 04 Oct 2023 23:56:08 GMT  
		Size: 57.7 MB (57708457 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6e706e7799d0736ff1b4df27c3a6703dcbb92134231f84f4fbcf841a201a8968`  
		Last Modified: Wed, 04 Oct 2023 23:56:06 GMT  
		Size: 316.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:94ede8436e0c5c1ba426163ae22d2e78a4449c1f90423be382adc88ef5e7f7df`  
		Last Modified: Wed, 04 Oct 2023 23:56:09 GMT  
		Size: 63.8 MB (63776717 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0433c6008f7b23b7308d19214b170ec2a1320794fad4f14e3089c9e932c73520`  
		Last Modified: Wed, 04 Oct 2023 23:56:07 GMT  
		Size: 5.4 KB (5390 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:oracle` - unknown; unknown

```console
$ docker pull mysql@sha256:0798fb11106cd915317ee2e883428e8c0509b66ba50c330bc08d98b71a2a4a93
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.1 MB (13139770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:50972c5093bb54a90971a3f64892fb3376c16d66dab33ee483a98b6b83f98382`

```dockerfile
```

-	Layers:
	-	`sha256:0952fb4b6cad899f5e32f2f4c030e7016feffbf1eaa3ee34e5bffc73c7e23b91`  
		Last Modified: Wed, 04 Oct 2023 23:56:05 GMT  
		Size: 13.1 MB (13106170 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:f9ff6e0e61f3655ad5ff5e9c2ebcd98ddbd7fcd1fd289af381f54c15137e50be`  
		Last Modified: Wed, 04 Oct 2023 23:56:03 GMT  
		Size: 33.6 KB (33600 bytes)  
		MIME: application/vnd.in-toto+json
