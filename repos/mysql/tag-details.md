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
$ docker pull mysql@sha256:4f9bfb0f7dd97739ceedb546b381534bb11e9b4abf013d6ad9ae6473fed66099
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 2
	-	linux; amd64
	-	unknown; unknown

### `mysql:5` - linux; amd64

```console
$ docker pull mysql@sha256:188121394576d05aedb5daf229403bf58d4ee16e04e81828e4d43b72bd227bc2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.2 MB (170176061 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b85be0b10d389e268b35d4c04075b95c295dd24d595e8c5261e43ab94c47de4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 27 Jul 2023 22:18:54 GMT
ADD file:2726e2d5d9aaf4024ea489d9049884aa06c0c95d6111037ba29987ba029ddc44 in / 
# Thu, 27 Jul 2023 22:18:54 GMT
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
	-	`sha256:9ad776bc39341b015fa96ec38b0ef30213514fedd245d657d3188d81b46d367c`  
		Last Modified: Thu, 12 Oct 2023 21:30:53 GMT  
		Size: 50.5 MB (50496653 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9e4eda42c982f018b636fece13fbfe13b3c485002a9e5b1b4742d4a9b2472344`  
		Last Modified: Thu, 12 Oct 2023 22:46:48 GMT  
		Size: 870.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:df6d882cf587c90f71772f078245206204ef6e06995073356c7a2e00d328d14c`  
		Last Modified: Thu, 12 Oct 2023 22:46:48 GMT  
		Size: 983.5 KB (983548 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6c804e92b324adecac8c3c0829f89949711442b1895d71c858360a18bfdd1043`  
		Last Modified: Thu, 12 Oct 2023 22:46:48 GMT  
		Size: 4.6 MB (4581890 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fd54ada0c48d0dec4f65e2e53d9924fca6888029f800b994c4ad5629e5503172`  
		Last Modified: Thu, 12 Oct 2023 22:46:49 GMT  
		Size: 3.1 KB (3077 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4ed8fb20ac8df2f75e04b1bb786677b8ed82131aa33d652f176b708e0e05a350`  
		Last Modified: Thu, 12 Oct 2023 22:46:49 GMT  
		Size: 333.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:eec2b1bc545491ca4135d1327d5d78299951efe05b6306e683d5d85f5d367ac3`  
		Last Modified: Thu, 12 Oct 2023 22:46:51 GMT  
		Size: 25.5 MB (25533109 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:41c3423057b75bfcdb2dcc8930c701bbcbebbe183f13ebd17316eee7657fa69f`  
		Last Modified: Thu, 12 Oct 2023 22:46:50 GMT  
		Size: 317.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:122b2c7b16c0784f4f6edf05f89df6cd3864f50838f30ba1c58a7c1e00515cd1`  
		Last Modified: Thu, 12 Oct 2023 22:46:56 GMT  
		Size: 88.6 MB (88570755 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0d30e03d70e3e18516a20a38b5f5160974f52706f98e372c560a51d22479788f`  
		Last Modified: Thu, 12 Oct 2023 22:46:51 GMT  
		Size: 5.4 KB (5387 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:71c43898e898ff024290d810c763e672209840a60f00ecd50cf138b16756c88d`  
		Last Modified: Thu, 12 Oct 2023 22:46:52 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:5` - unknown; unknown

```console
$ docker pull mysql@sha256:f6d617308dde54c4515d27dc7f6c3190da1a767bf4203eb03d6f0491cc6a0909
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.5 MB (14459686 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b102079ba75bd947c0eff2ef29718862d2a85b66bae829bc1cb0435887adb1f9`

```dockerfile
```

-	Layers:
	-	`sha256:0f321d3ef98514552b6fb61836bf1e7c253e5c213a5b39c963115490a11509ef`  
		Last Modified: Thu, 12 Oct 2023 22:46:49 GMT  
		Size: 14.4 MB (14423234 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:82e53b4ee50168adfbdb6db4e785a17926a698ce8595d58be1fce6cac977106b`  
		Last Modified: Thu, 12 Oct 2023 22:46:48 GMT  
		Size: 36.5 KB (36452 bytes)  
		MIME: application/vnd.in-toto+json

## `mysql:5-oracle`

```console
$ docker pull mysql@sha256:4f9bfb0f7dd97739ceedb546b381534bb11e9b4abf013d6ad9ae6473fed66099
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 2
	-	linux; amd64
	-	unknown; unknown

### `mysql:5-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:188121394576d05aedb5daf229403bf58d4ee16e04e81828e4d43b72bd227bc2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.2 MB (170176061 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b85be0b10d389e268b35d4c04075b95c295dd24d595e8c5261e43ab94c47de4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 27 Jul 2023 22:18:54 GMT
ADD file:2726e2d5d9aaf4024ea489d9049884aa06c0c95d6111037ba29987ba029ddc44 in / 
# Thu, 27 Jul 2023 22:18:54 GMT
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
	-	`sha256:9ad776bc39341b015fa96ec38b0ef30213514fedd245d657d3188d81b46d367c`  
		Last Modified: Thu, 12 Oct 2023 21:30:53 GMT  
		Size: 50.5 MB (50496653 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9e4eda42c982f018b636fece13fbfe13b3c485002a9e5b1b4742d4a9b2472344`  
		Last Modified: Thu, 12 Oct 2023 22:46:48 GMT  
		Size: 870.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:df6d882cf587c90f71772f078245206204ef6e06995073356c7a2e00d328d14c`  
		Last Modified: Thu, 12 Oct 2023 22:46:48 GMT  
		Size: 983.5 KB (983548 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6c804e92b324adecac8c3c0829f89949711442b1895d71c858360a18bfdd1043`  
		Last Modified: Thu, 12 Oct 2023 22:46:48 GMT  
		Size: 4.6 MB (4581890 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fd54ada0c48d0dec4f65e2e53d9924fca6888029f800b994c4ad5629e5503172`  
		Last Modified: Thu, 12 Oct 2023 22:46:49 GMT  
		Size: 3.1 KB (3077 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4ed8fb20ac8df2f75e04b1bb786677b8ed82131aa33d652f176b708e0e05a350`  
		Last Modified: Thu, 12 Oct 2023 22:46:49 GMT  
		Size: 333.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:eec2b1bc545491ca4135d1327d5d78299951efe05b6306e683d5d85f5d367ac3`  
		Last Modified: Thu, 12 Oct 2023 22:46:51 GMT  
		Size: 25.5 MB (25533109 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:41c3423057b75bfcdb2dcc8930c701bbcbebbe183f13ebd17316eee7657fa69f`  
		Last Modified: Thu, 12 Oct 2023 22:46:50 GMT  
		Size: 317.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:122b2c7b16c0784f4f6edf05f89df6cd3864f50838f30ba1c58a7c1e00515cd1`  
		Last Modified: Thu, 12 Oct 2023 22:46:56 GMT  
		Size: 88.6 MB (88570755 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0d30e03d70e3e18516a20a38b5f5160974f52706f98e372c560a51d22479788f`  
		Last Modified: Thu, 12 Oct 2023 22:46:51 GMT  
		Size: 5.4 KB (5387 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:71c43898e898ff024290d810c763e672209840a60f00ecd50cf138b16756c88d`  
		Last Modified: Thu, 12 Oct 2023 22:46:52 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:5-oracle` - unknown; unknown

```console
$ docker pull mysql@sha256:f6d617308dde54c4515d27dc7f6c3190da1a767bf4203eb03d6f0491cc6a0909
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.5 MB (14459686 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b102079ba75bd947c0eff2ef29718862d2a85b66bae829bc1cb0435887adb1f9`

```dockerfile
```

-	Layers:
	-	`sha256:0f321d3ef98514552b6fb61836bf1e7c253e5c213a5b39c963115490a11509ef`  
		Last Modified: Thu, 12 Oct 2023 22:46:49 GMT  
		Size: 14.4 MB (14423234 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:82e53b4ee50168adfbdb6db4e785a17926a698ce8595d58be1fce6cac977106b`  
		Last Modified: Thu, 12 Oct 2023 22:46:48 GMT  
		Size: 36.5 KB (36452 bytes)  
		MIME: application/vnd.in-toto+json

## `mysql:5.7`

```console
$ docker pull mysql@sha256:4f9bfb0f7dd97739ceedb546b381534bb11e9b4abf013d6ad9ae6473fed66099
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 2
	-	linux; amd64
	-	unknown; unknown

### `mysql:5.7` - linux; amd64

```console
$ docker pull mysql@sha256:188121394576d05aedb5daf229403bf58d4ee16e04e81828e4d43b72bd227bc2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.2 MB (170176061 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b85be0b10d389e268b35d4c04075b95c295dd24d595e8c5261e43ab94c47de4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 27 Jul 2023 22:18:54 GMT
ADD file:2726e2d5d9aaf4024ea489d9049884aa06c0c95d6111037ba29987ba029ddc44 in / 
# Thu, 27 Jul 2023 22:18:54 GMT
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
	-	`sha256:9ad776bc39341b015fa96ec38b0ef30213514fedd245d657d3188d81b46d367c`  
		Last Modified: Thu, 12 Oct 2023 21:30:53 GMT  
		Size: 50.5 MB (50496653 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9e4eda42c982f018b636fece13fbfe13b3c485002a9e5b1b4742d4a9b2472344`  
		Last Modified: Thu, 12 Oct 2023 22:46:48 GMT  
		Size: 870.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:df6d882cf587c90f71772f078245206204ef6e06995073356c7a2e00d328d14c`  
		Last Modified: Thu, 12 Oct 2023 22:46:48 GMT  
		Size: 983.5 KB (983548 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6c804e92b324adecac8c3c0829f89949711442b1895d71c858360a18bfdd1043`  
		Last Modified: Thu, 12 Oct 2023 22:46:48 GMT  
		Size: 4.6 MB (4581890 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fd54ada0c48d0dec4f65e2e53d9924fca6888029f800b994c4ad5629e5503172`  
		Last Modified: Thu, 12 Oct 2023 22:46:49 GMT  
		Size: 3.1 KB (3077 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4ed8fb20ac8df2f75e04b1bb786677b8ed82131aa33d652f176b708e0e05a350`  
		Last Modified: Thu, 12 Oct 2023 22:46:49 GMT  
		Size: 333.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:eec2b1bc545491ca4135d1327d5d78299951efe05b6306e683d5d85f5d367ac3`  
		Last Modified: Thu, 12 Oct 2023 22:46:51 GMT  
		Size: 25.5 MB (25533109 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:41c3423057b75bfcdb2dcc8930c701bbcbebbe183f13ebd17316eee7657fa69f`  
		Last Modified: Thu, 12 Oct 2023 22:46:50 GMT  
		Size: 317.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:122b2c7b16c0784f4f6edf05f89df6cd3864f50838f30ba1c58a7c1e00515cd1`  
		Last Modified: Thu, 12 Oct 2023 22:46:56 GMT  
		Size: 88.6 MB (88570755 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0d30e03d70e3e18516a20a38b5f5160974f52706f98e372c560a51d22479788f`  
		Last Modified: Thu, 12 Oct 2023 22:46:51 GMT  
		Size: 5.4 KB (5387 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:71c43898e898ff024290d810c763e672209840a60f00ecd50cf138b16756c88d`  
		Last Modified: Thu, 12 Oct 2023 22:46:52 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:5.7` - unknown; unknown

```console
$ docker pull mysql@sha256:f6d617308dde54c4515d27dc7f6c3190da1a767bf4203eb03d6f0491cc6a0909
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.5 MB (14459686 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b102079ba75bd947c0eff2ef29718862d2a85b66bae829bc1cb0435887adb1f9`

```dockerfile
```

-	Layers:
	-	`sha256:0f321d3ef98514552b6fb61836bf1e7c253e5c213a5b39c963115490a11509ef`  
		Last Modified: Thu, 12 Oct 2023 22:46:49 GMT  
		Size: 14.4 MB (14423234 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:82e53b4ee50168adfbdb6db4e785a17926a698ce8595d58be1fce6cac977106b`  
		Last Modified: Thu, 12 Oct 2023 22:46:48 GMT  
		Size: 36.5 KB (36452 bytes)  
		MIME: application/vnd.in-toto+json

## `mysql:5.7-oracle`

```console
$ docker pull mysql@sha256:4f9bfb0f7dd97739ceedb546b381534bb11e9b4abf013d6ad9ae6473fed66099
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 2
	-	linux; amd64
	-	unknown; unknown

### `mysql:5.7-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:188121394576d05aedb5daf229403bf58d4ee16e04e81828e4d43b72bd227bc2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.2 MB (170176061 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b85be0b10d389e268b35d4c04075b95c295dd24d595e8c5261e43ab94c47de4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 27 Jul 2023 22:18:54 GMT
ADD file:2726e2d5d9aaf4024ea489d9049884aa06c0c95d6111037ba29987ba029ddc44 in / 
# Thu, 27 Jul 2023 22:18:54 GMT
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
	-	`sha256:9ad776bc39341b015fa96ec38b0ef30213514fedd245d657d3188d81b46d367c`  
		Last Modified: Thu, 12 Oct 2023 21:30:53 GMT  
		Size: 50.5 MB (50496653 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9e4eda42c982f018b636fece13fbfe13b3c485002a9e5b1b4742d4a9b2472344`  
		Last Modified: Thu, 12 Oct 2023 22:46:48 GMT  
		Size: 870.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:df6d882cf587c90f71772f078245206204ef6e06995073356c7a2e00d328d14c`  
		Last Modified: Thu, 12 Oct 2023 22:46:48 GMT  
		Size: 983.5 KB (983548 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6c804e92b324adecac8c3c0829f89949711442b1895d71c858360a18bfdd1043`  
		Last Modified: Thu, 12 Oct 2023 22:46:48 GMT  
		Size: 4.6 MB (4581890 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fd54ada0c48d0dec4f65e2e53d9924fca6888029f800b994c4ad5629e5503172`  
		Last Modified: Thu, 12 Oct 2023 22:46:49 GMT  
		Size: 3.1 KB (3077 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4ed8fb20ac8df2f75e04b1bb786677b8ed82131aa33d652f176b708e0e05a350`  
		Last Modified: Thu, 12 Oct 2023 22:46:49 GMT  
		Size: 333.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:eec2b1bc545491ca4135d1327d5d78299951efe05b6306e683d5d85f5d367ac3`  
		Last Modified: Thu, 12 Oct 2023 22:46:51 GMT  
		Size: 25.5 MB (25533109 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:41c3423057b75bfcdb2dcc8930c701bbcbebbe183f13ebd17316eee7657fa69f`  
		Last Modified: Thu, 12 Oct 2023 22:46:50 GMT  
		Size: 317.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:122b2c7b16c0784f4f6edf05f89df6cd3864f50838f30ba1c58a7c1e00515cd1`  
		Last Modified: Thu, 12 Oct 2023 22:46:56 GMT  
		Size: 88.6 MB (88570755 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0d30e03d70e3e18516a20a38b5f5160974f52706f98e372c560a51d22479788f`  
		Last Modified: Thu, 12 Oct 2023 22:46:51 GMT  
		Size: 5.4 KB (5387 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:71c43898e898ff024290d810c763e672209840a60f00ecd50cf138b16756c88d`  
		Last Modified: Thu, 12 Oct 2023 22:46:52 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:5.7-oracle` - unknown; unknown

```console
$ docker pull mysql@sha256:f6d617308dde54c4515d27dc7f6c3190da1a767bf4203eb03d6f0491cc6a0909
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.5 MB (14459686 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b102079ba75bd947c0eff2ef29718862d2a85b66bae829bc1cb0435887adb1f9`

```dockerfile
```

-	Layers:
	-	`sha256:0f321d3ef98514552b6fb61836bf1e7c253e5c213a5b39c963115490a11509ef`  
		Last Modified: Thu, 12 Oct 2023 22:46:49 GMT  
		Size: 14.4 MB (14423234 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:82e53b4ee50168adfbdb6db4e785a17926a698ce8595d58be1fce6cac977106b`  
		Last Modified: Thu, 12 Oct 2023 22:46:48 GMT  
		Size: 36.5 KB (36452 bytes)  
		MIME: application/vnd.in-toto+json

## `mysql:5.7.43`

```console
$ docker pull mysql@sha256:4f9bfb0f7dd97739ceedb546b381534bb11e9b4abf013d6ad9ae6473fed66099
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 2
	-	linux; amd64
	-	unknown; unknown

### `mysql:5.7.43` - linux; amd64

```console
$ docker pull mysql@sha256:188121394576d05aedb5daf229403bf58d4ee16e04e81828e4d43b72bd227bc2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.2 MB (170176061 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b85be0b10d389e268b35d4c04075b95c295dd24d595e8c5261e43ab94c47de4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 27 Jul 2023 22:18:54 GMT
ADD file:2726e2d5d9aaf4024ea489d9049884aa06c0c95d6111037ba29987ba029ddc44 in / 
# Thu, 27 Jul 2023 22:18:54 GMT
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
	-	`sha256:9ad776bc39341b015fa96ec38b0ef30213514fedd245d657d3188d81b46d367c`  
		Last Modified: Thu, 12 Oct 2023 21:30:53 GMT  
		Size: 50.5 MB (50496653 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9e4eda42c982f018b636fece13fbfe13b3c485002a9e5b1b4742d4a9b2472344`  
		Last Modified: Thu, 12 Oct 2023 22:46:48 GMT  
		Size: 870.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:df6d882cf587c90f71772f078245206204ef6e06995073356c7a2e00d328d14c`  
		Last Modified: Thu, 12 Oct 2023 22:46:48 GMT  
		Size: 983.5 KB (983548 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6c804e92b324adecac8c3c0829f89949711442b1895d71c858360a18bfdd1043`  
		Last Modified: Thu, 12 Oct 2023 22:46:48 GMT  
		Size: 4.6 MB (4581890 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fd54ada0c48d0dec4f65e2e53d9924fca6888029f800b994c4ad5629e5503172`  
		Last Modified: Thu, 12 Oct 2023 22:46:49 GMT  
		Size: 3.1 KB (3077 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4ed8fb20ac8df2f75e04b1bb786677b8ed82131aa33d652f176b708e0e05a350`  
		Last Modified: Thu, 12 Oct 2023 22:46:49 GMT  
		Size: 333.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:eec2b1bc545491ca4135d1327d5d78299951efe05b6306e683d5d85f5d367ac3`  
		Last Modified: Thu, 12 Oct 2023 22:46:51 GMT  
		Size: 25.5 MB (25533109 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:41c3423057b75bfcdb2dcc8930c701bbcbebbe183f13ebd17316eee7657fa69f`  
		Last Modified: Thu, 12 Oct 2023 22:46:50 GMT  
		Size: 317.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:122b2c7b16c0784f4f6edf05f89df6cd3864f50838f30ba1c58a7c1e00515cd1`  
		Last Modified: Thu, 12 Oct 2023 22:46:56 GMT  
		Size: 88.6 MB (88570755 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0d30e03d70e3e18516a20a38b5f5160974f52706f98e372c560a51d22479788f`  
		Last Modified: Thu, 12 Oct 2023 22:46:51 GMT  
		Size: 5.4 KB (5387 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:71c43898e898ff024290d810c763e672209840a60f00ecd50cf138b16756c88d`  
		Last Modified: Thu, 12 Oct 2023 22:46:52 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:5.7.43` - unknown; unknown

```console
$ docker pull mysql@sha256:f6d617308dde54c4515d27dc7f6c3190da1a767bf4203eb03d6f0491cc6a0909
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.5 MB (14459686 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b102079ba75bd947c0eff2ef29718862d2a85b66bae829bc1cb0435887adb1f9`

```dockerfile
```

-	Layers:
	-	`sha256:0f321d3ef98514552b6fb61836bf1e7c253e5c213a5b39c963115490a11509ef`  
		Last Modified: Thu, 12 Oct 2023 22:46:49 GMT  
		Size: 14.4 MB (14423234 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:82e53b4ee50168adfbdb6db4e785a17926a698ce8595d58be1fce6cac977106b`  
		Last Modified: Thu, 12 Oct 2023 22:46:48 GMT  
		Size: 36.5 KB (36452 bytes)  
		MIME: application/vnd.in-toto+json

## `mysql:5.7.43-oracle`

```console
$ docker pull mysql@sha256:4f9bfb0f7dd97739ceedb546b381534bb11e9b4abf013d6ad9ae6473fed66099
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 2
	-	linux; amd64
	-	unknown; unknown

### `mysql:5.7.43-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:188121394576d05aedb5daf229403bf58d4ee16e04e81828e4d43b72bd227bc2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.2 MB (170176061 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b85be0b10d389e268b35d4c04075b95c295dd24d595e8c5261e43ab94c47de4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 27 Jul 2023 22:18:54 GMT
ADD file:2726e2d5d9aaf4024ea489d9049884aa06c0c95d6111037ba29987ba029ddc44 in / 
# Thu, 27 Jul 2023 22:18:54 GMT
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
	-	`sha256:9ad776bc39341b015fa96ec38b0ef30213514fedd245d657d3188d81b46d367c`  
		Last Modified: Thu, 12 Oct 2023 21:30:53 GMT  
		Size: 50.5 MB (50496653 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9e4eda42c982f018b636fece13fbfe13b3c485002a9e5b1b4742d4a9b2472344`  
		Last Modified: Thu, 12 Oct 2023 22:46:48 GMT  
		Size: 870.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:df6d882cf587c90f71772f078245206204ef6e06995073356c7a2e00d328d14c`  
		Last Modified: Thu, 12 Oct 2023 22:46:48 GMT  
		Size: 983.5 KB (983548 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6c804e92b324adecac8c3c0829f89949711442b1895d71c858360a18bfdd1043`  
		Last Modified: Thu, 12 Oct 2023 22:46:48 GMT  
		Size: 4.6 MB (4581890 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fd54ada0c48d0dec4f65e2e53d9924fca6888029f800b994c4ad5629e5503172`  
		Last Modified: Thu, 12 Oct 2023 22:46:49 GMT  
		Size: 3.1 KB (3077 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4ed8fb20ac8df2f75e04b1bb786677b8ed82131aa33d652f176b708e0e05a350`  
		Last Modified: Thu, 12 Oct 2023 22:46:49 GMT  
		Size: 333.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:eec2b1bc545491ca4135d1327d5d78299951efe05b6306e683d5d85f5d367ac3`  
		Last Modified: Thu, 12 Oct 2023 22:46:51 GMT  
		Size: 25.5 MB (25533109 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:41c3423057b75bfcdb2dcc8930c701bbcbebbe183f13ebd17316eee7657fa69f`  
		Last Modified: Thu, 12 Oct 2023 22:46:50 GMT  
		Size: 317.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:122b2c7b16c0784f4f6edf05f89df6cd3864f50838f30ba1c58a7c1e00515cd1`  
		Last Modified: Thu, 12 Oct 2023 22:46:56 GMT  
		Size: 88.6 MB (88570755 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0d30e03d70e3e18516a20a38b5f5160974f52706f98e372c560a51d22479788f`  
		Last Modified: Thu, 12 Oct 2023 22:46:51 GMT  
		Size: 5.4 KB (5387 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:71c43898e898ff024290d810c763e672209840a60f00ecd50cf138b16756c88d`  
		Last Modified: Thu, 12 Oct 2023 22:46:52 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:5.7.43-oracle` - unknown; unknown

```console
$ docker pull mysql@sha256:f6d617308dde54c4515d27dc7f6c3190da1a767bf4203eb03d6f0491cc6a0909
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.5 MB (14459686 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b102079ba75bd947c0eff2ef29718862d2a85b66bae829bc1cb0435887adb1f9`

```dockerfile
```

-	Layers:
	-	`sha256:0f321d3ef98514552b6fb61836bf1e7c253e5c213a5b39c963115490a11509ef`  
		Last Modified: Thu, 12 Oct 2023 22:46:49 GMT  
		Size: 14.4 MB (14423234 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:82e53b4ee50168adfbdb6db4e785a17926a698ce8595d58be1fce6cac977106b`  
		Last Modified: Thu, 12 Oct 2023 22:46:48 GMT  
		Size: 36.5 KB (36452 bytes)  
		MIME: application/vnd.in-toto+json

## `mysql:8`

```console
$ docker pull mysql@sha256:f61944ff3f2961363a4d22913b2ac581523273679d7e14dd26e8db8c9f571a7e
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `mysql:8` - linux; amd64

```console
$ docker pull mysql@sha256:c458b26f2f9f9fe086ed75d1f8db8e2dde371801403f2c7da9be4fb228a2944a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **166.1 MB (166123241 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae2502152260b33bfafb9c3e3a1811086317e0236abf83a59503cec0f8980573`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 27 Jul 2023 22:18:51 GMT
ADD file:0f45bdf93b14a2ab9389b71d23b6c7f6d2935c8016e3b6422814f8fc79bef986 in / 
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
	-	`sha256:8e0176adc18c476bdfcc701f01cda5acf49bc8e6d7fadac8072091a43fafbb25`  
		Last Modified: Fri, 20 Oct 2023 18:28:56 GMT  
		Size: 44.3 MB (44279620 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:14e977b0f4b2310e3eaed27abcab0fad4dae8f9bafa8f77c4ed5316fff629f2f`  
		Last Modified: Fri, 20 Oct 2023 19:04:04 GMT  
		Size: 885.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a7b58dd6f78b98d9ff6fbc049f2f7cb84174c74dd57cacbdb185f9b896bb2919`  
		Last Modified: Fri, 20 Oct 2023 19:04:05 GMT  
		Size: 982.8 KB (982806 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fba70cc872a5b5a727ef28a9ed8203ad526cb069dc21dcad1076bcf98286ffa5`  
		Last Modified: Fri, 20 Oct 2023 19:04:05 GMT  
		Size: 4.6 MB (4613864 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5db2cc6eab8f76e59babee0c88038ba1e7d20bbdca06ae1fc2480d89aee76343`  
		Last Modified: Fri, 20 Oct 2023 19:04:05 GMT  
		Size: 2.6 KB (2607 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:081f41f573ba759e534574da506eb0a6593adb408cf88d3f9c5c7665c8d0807f`  
		Last Modified: Fri, 20 Oct 2023 19:04:06 GMT  
		Size: 339.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:86bf2dc4ded9433a1f0b2155401a202843311dc129425e4a35f193dbdb4254f9`  
		Last Modified: Fri, 20 Oct 2023 19:04:11 GMT  
		Size: 58.8 MB (58754172 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:47f08b0e916e6e60dc941429579e860a2f1c4b6eeaedd5600bac7391f41c7733`  
		Last Modified: Fri, 20 Oct 2023 19:04:07 GMT  
		Size: 317.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:850e29ae8eeb4a7f347575c2fa8f159be328eacad69cc27f5376b7836b808a5f`  
		Last Modified: Fri, 20 Oct 2023 19:04:10 GMT  
		Size: 57.5 MB (57483245 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:13517fe0d921160b87a62dea36c2d361e7936b2fa5e8c4319001c6e472fbd166`  
		Last Modified: Fri, 20 Oct 2023 19:04:08 GMT  
		Size: 5.4 KB (5386 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:8` - unknown; unknown

```console
$ docker pull mysql@sha256:2faea6171999069839076bda0781b64056aab4ea0d102220851de5690d238082
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.2 MB (11247404 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:abc364c5064a4eca4aab69f869586ab10aacdf0add869b720111829105492cbc`

```dockerfile
```

-	Layers:
	-	`sha256:5900cd702aca9703a447153286a87bf27042d3f0cdcfbde3c19f960bf2053668`  
		Last Modified: Fri, 20 Oct 2023 19:04:05 GMT  
		Size: 11.2 MB (11213826 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:f3a630b6ecb72d9898f9adf3385edfa15b93e6184b045b18842358fd8c6ae3cf`  
		Last Modified: Fri, 20 Oct 2023 19:04:04 GMT  
		Size: 33.6 KB (33578 bytes)  
		MIME: application/vnd.in-toto+json

### `mysql:8` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:376751ad5724968a1dc5cb624852332955a0f82adf09c2d903023fc79c80a178
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.4 MB (170390818 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d858cb210e4b84459d06dc864905ffa5d12429467e45db806ade28932e5bd65d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 27 Jul 2023 22:18:51 GMT
ADD file:e189ba41c54c386435a3292026b75a1386976d3222102c16a725f58f594f284e in / 
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
	-	`sha256:e39ec8f010eb75816ae2c21b014f7fdecffb48374079b6f1bce017214e2a45cd`  
		Last Modified: Fri, 20 Oct 2023 18:40:29 GMT  
		Size: 43.7 MB (43672784 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e2b7fadc33ecff9fcb4c6067c675ad7d14bb8b71f383f243e558ae552cf8da05`  
		Last Modified: Fri, 20 Oct 2023 20:38:15 GMT  
		Size: 883.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9d193449aafd2e76aefe49f553ee2d007ed850656e18916b74c5d28057e6cfb7`  
		Last Modified: Fri, 20 Oct 2023 20:38:15 GMT  
		Size: 913.0 KB (912965 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6ea497c74b15661c8dcda90c65a4d6878277fb00ba8ce6c4b71bab676b372c34`  
		Last Modified: Fri, 20 Oct 2023 20:38:16 GMT  
		Size: 4.3 MB (4302158 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7778acbf55f327acde293ae0092a016ebf0324943d47aa131140a802397301d2`  
		Last Modified: Fri, 20 Oct 2023 20:38:16 GMT  
		Size: 2.6 KB (2607 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b65a5d7a2435a3664f7d77ed9e51646b62721b51396b27ff9d2853dd377ec76d`  
		Last Modified: Fri, 20 Oct 2023 20:38:16 GMT  
		Size: 339.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cef9fb0078a5e4eb83b7675f763bcf1e93ba403dd95139d00679313915b83831`  
		Last Modified: Fri, 20 Oct 2023 20:38:20 GMT  
		Size: 57.7 MB (57702031 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5b6dc73ec72424a05d131a7d8bbc28951e86bf53ebd4cd79a7d3777baacd5dd9`  
		Last Modified: Fri, 20 Oct 2023 20:38:18 GMT  
		Size: 317.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d992bb39e209c72e87bf31c42c6b1a34210084f585778ab64dd129de5e2c2672`  
		Last Modified: Fri, 20 Oct 2023 20:38:21 GMT  
		Size: 63.8 MB (63791340 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4431432b89a3ffd8f9dafe35d1a3c42ceb8caa0f23eda1f67b2e29eabf00412a`  
		Last Modified: Fri, 20 Oct 2023 20:38:18 GMT  
		Size: 5.4 KB (5394 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:8` - unknown; unknown

```console
$ docker pull mysql@sha256:287fd970d795844678660fc69a6c613789e5b61134e6b755b61afda3f925122e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.2 MB (11246015 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e28ecb6013e37bf1ec95d4ce0d35d11ddbc3d02006aae2aafed3d536dec4cea`

```dockerfile
```

-	Layers:
	-	`sha256:e386e5c32eff52a8f31e3168432997b2fc1924a764878f857a4039968d5b4355`  
		Last Modified: Fri, 20 Oct 2023 20:38:16 GMT  
		Size: 11.2 MB (11212414 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:93236631c96ce25fe9eb4000349de4979b3f67ab3c5fc4d22628d8bd9fb98ddf`  
		Last Modified: Fri, 20 Oct 2023 20:38:15 GMT  
		Size: 33.6 KB (33601 bytes)  
		MIME: application/vnd.in-toto+json

## `mysql:8-oracle`

```console
$ docker pull mysql@sha256:f61944ff3f2961363a4d22913b2ac581523273679d7e14dd26e8db8c9f571a7e
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `mysql:8-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:c458b26f2f9f9fe086ed75d1f8db8e2dde371801403f2c7da9be4fb228a2944a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **166.1 MB (166123241 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae2502152260b33bfafb9c3e3a1811086317e0236abf83a59503cec0f8980573`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 27 Jul 2023 22:18:51 GMT
ADD file:0f45bdf93b14a2ab9389b71d23b6c7f6d2935c8016e3b6422814f8fc79bef986 in / 
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
	-	`sha256:8e0176adc18c476bdfcc701f01cda5acf49bc8e6d7fadac8072091a43fafbb25`  
		Last Modified: Fri, 20 Oct 2023 18:28:56 GMT  
		Size: 44.3 MB (44279620 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:14e977b0f4b2310e3eaed27abcab0fad4dae8f9bafa8f77c4ed5316fff629f2f`  
		Last Modified: Fri, 20 Oct 2023 19:04:04 GMT  
		Size: 885.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a7b58dd6f78b98d9ff6fbc049f2f7cb84174c74dd57cacbdb185f9b896bb2919`  
		Last Modified: Fri, 20 Oct 2023 19:04:05 GMT  
		Size: 982.8 KB (982806 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fba70cc872a5b5a727ef28a9ed8203ad526cb069dc21dcad1076bcf98286ffa5`  
		Last Modified: Fri, 20 Oct 2023 19:04:05 GMT  
		Size: 4.6 MB (4613864 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5db2cc6eab8f76e59babee0c88038ba1e7d20bbdca06ae1fc2480d89aee76343`  
		Last Modified: Fri, 20 Oct 2023 19:04:05 GMT  
		Size: 2.6 KB (2607 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:081f41f573ba759e534574da506eb0a6593adb408cf88d3f9c5c7665c8d0807f`  
		Last Modified: Fri, 20 Oct 2023 19:04:06 GMT  
		Size: 339.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:86bf2dc4ded9433a1f0b2155401a202843311dc129425e4a35f193dbdb4254f9`  
		Last Modified: Fri, 20 Oct 2023 19:04:11 GMT  
		Size: 58.8 MB (58754172 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:47f08b0e916e6e60dc941429579e860a2f1c4b6eeaedd5600bac7391f41c7733`  
		Last Modified: Fri, 20 Oct 2023 19:04:07 GMT  
		Size: 317.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:850e29ae8eeb4a7f347575c2fa8f159be328eacad69cc27f5376b7836b808a5f`  
		Last Modified: Fri, 20 Oct 2023 19:04:10 GMT  
		Size: 57.5 MB (57483245 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:13517fe0d921160b87a62dea36c2d361e7936b2fa5e8c4319001c6e472fbd166`  
		Last Modified: Fri, 20 Oct 2023 19:04:08 GMT  
		Size: 5.4 KB (5386 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:8-oracle` - unknown; unknown

```console
$ docker pull mysql@sha256:2faea6171999069839076bda0781b64056aab4ea0d102220851de5690d238082
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.2 MB (11247404 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:abc364c5064a4eca4aab69f869586ab10aacdf0add869b720111829105492cbc`

```dockerfile
```

-	Layers:
	-	`sha256:5900cd702aca9703a447153286a87bf27042d3f0cdcfbde3c19f960bf2053668`  
		Last Modified: Fri, 20 Oct 2023 19:04:05 GMT  
		Size: 11.2 MB (11213826 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:f3a630b6ecb72d9898f9adf3385edfa15b93e6184b045b18842358fd8c6ae3cf`  
		Last Modified: Fri, 20 Oct 2023 19:04:04 GMT  
		Size: 33.6 KB (33578 bytes)  
		MIME: application/vnd.in-toto+json

### `mysql:8-oracle` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:376751ad5724968a1dc5cb624852332955a0f82adf09c2d903023fc79c80a178
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.4 MB (170390818 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d858cb210e4b84459d06dc864905ffa5d12429467e45db806ade28932e5bd65d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 27 Jul 2023 22:18:51 GMT
ADD file:e189ba41c54c386435a3292026b75a1386976d3222102c16a725f58f594f284e in / 
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
	-	`sha256:e39ec8f010eb75816ae2c21b014f7fdecffb48374079b6f1bce017214e2a45cd`  
		Last Modified: Fri, 20 Oct 2023 18:40:29 GMT  
		Size: 43.7 MB (43672784 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e2b7fadc33ecff9fcb4c6067c675ad7d14bb8b71f383f243e558ae552cf8da05`  
		Last Modified: Fri, 20 Oct 2023 20:38:15 GMT  
		Size: 883.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9d193449aafd2e76aefe49f553ee2d007ed850656e18916b74c5d28057e6cfb7`  
		Last Modified: Fri, 20 Oct 2023 20:38:15 GMT  
		Size: 913.0 KB (912965 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6ea497c74b15661c8dcda90c65a4d6878277fb00ba8ce6c4b71bab676b372c34`  
		Last Modified: Fri, 20 Oct 2023 20:38:16 GMT  
		Size: 4.3 MB (4302158 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7778acbf55f327acde293ae0092a016ebf0324943d47aa131140a802397301d2`  
		Last Modified: Fri, 20 Oct 2023 20:38:16 GMT  
		Size: 2.6 KB (2607 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b65a5d7a2435a3664f7d77ed9e51646b62721b51396b27ff9d2853dd377ec76d`  
		Last Modified: Fri, 20 Oct 2023 20:38:16 GMT  
		Size: 339.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cef9fb0078a5e4eb83b7675f763bcf1e93ba403dd95139d00679313915b83831`  
		Last Modified: Fri, 20 Oct 2023 20:38:20 GMT  
		Size: 57.7 MB (57702031 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5b6dc73ec72424a05d131a7d8bbc28951e86bf53ebd4cd79a7d3777baacd5dd9`  
		Last Modified: Fri, 20 Oct 2023 20:38:18 GMT  
		Size: 317.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d992bb39e209c72e87bf31c42c6b1a34210084f585778ab64dd129de5e2c2672`  
		Last Modified: Fri, 20 Oct 2023 20:38:21 GMT  
		Size: 63.8 MB (63791340 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4431432b89a3ffd8f9dafe35d1a3c42ceb8caa0f23eda1f67b2e29eabf00412a`  
		Last Modified: Fri, 20 Oct 2023 20:38:18 GMT  
		Size: 5.4 KB (5394 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:8-oracle` - unknown; unknown

```console
$ docker pull mysql@sha256:287fd970d795844678660fc69a6c613789e5b61134e6b755b61afda3f925122e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.2 MB (11246015 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e28ecb6013e37bf1ec95d4ce0d35d11ddbc3d02006aae2aafed3d536dec4cea`

```dockerfile
```

-	Layers:
	-	`sha256:e386e5c32eff52a8f31e3168432997b2fc1924a764878f857a4039968d5b4355`  
		Last Modified: Fri, 20 Oct 2023 20:38:16 GMT  
		Size: 11.2 MB (11212414 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:93236631c96ce25fe9eb4000349de4979b3f67ab3c5fc4d22628d8bd9fb98ddf`  
		Last Modified: Fri, 20 Oct 2023 20:38:15 GMT  
		Size: 33.6 KB (33601 bytes)  
		MIME: application/vnd.in-toto+json

## `mysql:8.0`

```console
$ docker pull mysql@sha256:59ae56ac42c6c09aebd9a7bb8d9f07a5fdf836f956e050946f85bbfa29d0a080
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `mysql:8.0` - linux; amd64

```console
$ docker pull mysql@sha256:8b8835a2c32cd7357a5d2ea4b49ad870ff519c8c1d4add362803feddf4a0a973
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **165.9 MB (165869861 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1d66a2a0aa16e23edc8d1c1e08be4a0ba8c239c9414a90b1d0cb4944ca4a194`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 20 Jul 2023 22:15:44 GMT
ADD file:0f45bdf93b14a2ab9389b71d23b6c7f6d2935c8016e3b6422814f8fc79bef986 in / 
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
	-	`sha256:8e0176adc18c476bdfcc701f01cda5acf49bc8e6d7fadac8072091a43fafbb25`  
		Last Modified: Fri, 20 Oct 2023 18:28:56 GMT  
		Size: 44.3 MB (44279620 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:de512b6f1736a825c3faf1f6e29b250af00fdb081c26d02f1276237265d272e2`  
		Last Modified: Fri, 20 Oct 2023 19:04:03 GMT  
		Size: 882.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fb3459be0c6886d8c2e23eb23a582006b68738b48bd52db4bd1303d9ae8286c6`  
		Last Modified: Fri, 20 Oct 2023 19:04:03 GMT  
		Size: 982.8 KB (982809 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:77379308b924f78d087b9cfded2b5333247182de433e11417ea7d81f2c574f27`  
		Last Modified: Fri, 20 Oct 2023 19:04:03 GMT  
		Size: 4.6 MB (4613882 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bfadef6257d17e2d887a0bfdf3948749ed43e98f99eff26251fc63f3e6b2cef3`  
		Last Modified: Fri, 20 Oct 2023 19:04:04 GMT  
		Size: 2.6 KB (2609 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5034ed0fbcb845f3118bc99cd00e20d01ef0c8ce7ad6ce378833004e55c90948`  
		Last Modified: Fri, 20 Oct 2023 19:04:05 GMT  
		Size: 333.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c0363a641ba973d0dc144b009898cb31c06a4c04dde2b2f59a553407e463abb6`  
		Last Modified: Fri, 20 Oct 2023 19:04:08 GMT  
		Size: 58.5 MB (58486052 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:49cafcd8a97548e00aba56544fe0d961c8de101a22f560158687c6ea874e2543`  
		Last Modified: Fri, 20 Oct 2023 19:04:05 GMT  
		Size: 318.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c2f92e2c3315cb55c51e20d5f9da7105d08e0c94a1ff8264a6b59dc3f19384c2`  
		Last Modified: Fri, 20 Oct 2023 19:04:11 GMT  
		Size: 57.5 MB (57497846 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a3f49bb45462ec43aa4975c1480f1a980dc0a0f9063d1dccb9a2371529de4d9d`  
		Last Modified: Fri, 20 Oct 2023 19:04:06 GMT  
		Size: 5.4 KB (5388 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7238affa01f6b755e3715d2269dc451392b079dc8c242ea2204a29d3f6d212ae`  
		Last Modified: Fri, 20 Oct 2023 19:04:08 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:8.0` - unknown; unknown

```console
$ docker pull mysql@sha256:9b23f72f8ec6a984af3064cbe759daecda0037c7227e116e98689f75e7729762
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.2 MB (11246228 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6905ab0de6eb417c6c062b8a3dbbcd3462314eb33b04baf8ecf1ea0fa9a7ec63`

```dockerfile
```

-	Layers:
	-	`sha256:b7b94af060c390356daf63f3b9b9424a11d553e7f628f0d900c26f670219f63f`  
		Last Modified: Fri, 20 Oct 2023 19:04:04 GMT  
		Size: 11.2 MB (11212034 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:0cefd81b6c7497a200591b31f91e0ed09959f3d14aa5685f673b86d9c5ff38c7`  
		Last Modified: Fri, 20 Oct 2023 19:04:03 GMT  
		Size: 34.2 KB (34194 bytes)  
		MIME: application/vnd.in-toto+json

### `mysql:8.0` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:3c362d5eed04f271a2ebad41f45fed5ed86e934da533a079bcbd2b3a4ff372e8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.1 MB (170132091 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93db1e4f7846804531842503e6855d382e5647732a309f62a46a736f649fd5cf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 20 Jul 2023 22:15:44 GMT
ADD file:e189ba41c54c386435a3292026b75a1386976d3222102c16a725f58f594f284e in / 
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
	-	`sha256:e39ec8f010eb75816ae2c21b014f7fdecffb48374079b6f1bce017214e2a45cd`  
		Last Modified: Fri, 20 Oct 2023 18:40:29 GMT  
		Size: 43.7 MB (43672784 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e2b7fadc33ecff9fcb4c6067c675ad7d14bb8b71f383f243e558ae552cf8da05`  
		Last Modified: Fri, 20 Oct 2023 20:38:15 GMT  
		Size: 883.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9d193449aafd2e76aefe49f553ee2d007ed850656e18916b74c5d28057e6cfb7`  
		Last Modified: Fri, 20 Oct 2023 20:38:15 GMT  
		Size: 913.0 KB (912965 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6ea497c74b15661c8dcda90c65a4d6878277fb00ba8ce6c4b71bab676b372c34`  
		Last Modified: Fri, 20 Oct 2023 20:38:16 GMT  
		Size: 4.3 MB (4302158 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7778acbf55f327acde293ae0092a016ebf0324943d47aa131140a802397301d2`  
		Last Modified: Fri, 20 Oct 2023 20:38:16 GMT  
		Size: 2.6 KB (2607 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fa2675fd414a6242f407f6b5a8bd013f30d2bad261deb6a6a440e1121da1857a`  
		Last Modified: Fri, 20 Oct 2023 20:40:01 GMT  
		Size: 332.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d24f782b47329ae0e2c2e08d37b0a47553fb07bd5dadb7ea7e91f570f559084a`  
		Last Modified: Fri, 20 Oct 2023 20:40:07 GMT  
		Size: 57.5 MB (57454168 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d72061df12b27dfb6b550389fdadb3bc290a2cf8f5baaa58828fe7efb543d359`  
		Last Modified: Fri, 20 Oct 2023 20:40:01 GMT  
		Size: 315.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:44c59a54226d295d690d41a35b4c9fa1bb3b8a106e062b6129ea176b19d17dac`  
		Last Modified: Fri, 20 Oct 2023 20:40:06 GMT  
		Size: 63.8 MB (63780363 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c8eba2a1704137c2b007bc0efdbb676a8b8b58a1b2b6e1deaa5422fd5a687b64`  
		Last Modified: Fri, 20 Oct 2023 20:40:03 GMT  
		Size: 5.4 KB (5394 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0c1c0cd211c9ba4d8a84ae33b95fcc805e19bd7f5c1b33cc5b4ae25d8b65eb95`  
		Last Modified: Fri, 20 Oct 2023 20:40:03 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:8.0` - unknown; unknown

```console
$ docker pull mysql@sha256:02b282dd539f9d295b046ade8c8e5fceaa55fae8ae5a1c06a7f73661febe933e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.2 MB (11244647 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5e7bd00c2deab1e38d8476e0d21ad22483ad150defe9046127684ce18187823`

```dockerfile
```

-	Layers:
	-	`sha256:6f2dda0ddc63496263d54aec6345f9c431c1010428062119568b0710affab9ca`  
		Last Modified: Fri, 20 Oct 2023 20:40:02 GMT  
		Size: 11.2 MB (11210610 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:d5f8fca198352f62646eb00da40475ee7c1fd82d42f01a54d8e4bd4cf257eb8d`  
		Last Modified: Fri, 20 Oct 2023 20:40:01 GMT  
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
$ docker pull mysql@sha256:59ae56ac42c6c09aebd9a7bb8d9f07a5fdf836f956e050946f85bbfa29d0a080
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `mysql:8.0-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:8b8835a2c32cd7357a5d2ea4b49ad870ff519c8c1d4add362803feddf4a0a973
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **165.9 MB (165869861 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1d66a2a0aa16e23edc8d1c1e08be4a0ba8c239c9414a90b1d0cb4944ca4a194`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 20 Jul 2023 22:15:44 GMT
ADD file:0f45bdf93b14a2ab9389b71d23b6c7f6d2935c8016e3b6422814f8fc79bef986 in / 
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
	-	`sha256:8e0176adc18c476bdfcc701f01cda5acf49bc8e6d7fadac8072091a43fafbb25`  
		Last Modified: Fri, 20 Oct 2023 18:28:56 GMT  
		Size: 44.3 MB (44279620 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:de512b6f1736a825c3faf1f6e29b250af00fdb081c26d02f1276237265d272e2`  
		Last Modified: Fri, 20 Oct 2023 19:04:03 GMT  
		Size: 882.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fb3459be0c6886d8c2e23eb23a582006b68738b48bd52db4bd1303d9ae8286c6`  
		Last Modified: Fri, 20 Oct 2023 19:04:03 GMT  
		Size: 982.8 KB (982809 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:77379308b924f78d087b9cfded2b5333247182de433e11417ea7d81f2c574f27`  
		Last Modified: Fri, 20 Oct 2023 19:04:03 GMT  
		Size: 4.6 MB (4613882 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bfadef6257d17e2d887a0bfdf3948749ed43e98f99eff26251fc63f3e6b2cef3`  
		Last Modified: Fri, 20 Oct 2023 19:04:04 GMT  
		Size: 2.6 KB (2609 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5034ed0fbcb845f3118bc99cd00e20d01ef0c8ce7ad6ce378833004e55c90948`  
		Last Modified: Fri, 20 Oct 2023 19:04:05 GMT  
		Size: 333.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c0363a641ba973d0dc144b009898cb31c06a4c04dde2b2f59a553407e463abb6`  
		Last Modified: Fri, 20 Oct 2023 19:04:08 GMT  
		Size: 58.5 MB (58486052 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:49cafcd8a97548e00aba56544fe0d961c8de101a22f560158687c6ea874e2543`  
		Last Modified: Fri, 20 Oct 2023 19:04:05 GMT  
		Size: 318.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c2f92e2c3315cb55c51e20d5f9da7105d08e0c94a1ff8264a6b59dc3f19384c2`  
		Last Modified: Fri, 20 Oct 2023 19:04:11 GMT  
		Size: 57.5 MB (57497846 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a3f49bb45462ec43aa4975c1480f1a980dc0a0f9063d1dccb9a2371529de4d9d`  
		Last Modified: Fri, 20 Oct 2023 19:04:06 GMT  
		Size: 5.4 KB (5388 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7238affa01f6b755e3715d2269dc451392b079dc8c242ea2204a29d3f6d212ae`  
		Last Modified: Fri, 20 Oct 2023 19:04:08 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:8.0-oracle` - unknown; unknown

```console
$ docker pull mysql@sha256:9b23f72f8ec6a984af3064cbe759daecda0037c7227e116e98689f75e7729762
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.2 MB (11246228 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6905ab0de6eb417c6c062b8a3dbbcd3462314eb33b04baf8ecf1ea0fa9a7ec63`

```dockerfile
```

-	Layers:
	-	`sha256:b7b94af060c390356daf63f3b9b9424a11d553e7f628f0d900c26f670219f63f`  
		Last Modified: Fri, 20 Oct 2023 19:04:04 GMT  
		Size: 11.2 MB (11212034 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:0cefd81b6c7497a200591b31f91e0ed09959f3d14aa5685f673b86d9c5ff38c7`  
		Last Modified: Fri, 20 Oct 2023 19:04:03 GMT  
		Size: 34.2 KB (34194 bytes)  
		MIME: application/vnd.in-toto+json

### `mysql:8.0-oracle` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:3c362d5eed04f271a2ebad41f45fed5ed86e934da533a079bcbd2b3a4ff372e8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.1 MB (170132091 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93db1e4f7846804531842503e6855d382e5647732a309f62a46a736f649fd5cf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 20 Jul 2023 22:15:44 GMT
ADD file:e189ba41c54c386435a3292026b75a1386976d3222102c16a725f58f594f284e in / 
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
	-	`sha256:e39ec8f010eb75816ae2c21b014f7fdecffb48374079b6f1bce017214e2a45cd`  
		Last Modified: Fri, 20 Oct 2023 18:40:29 GMT  
		Size: 43.7 MB (43672784 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e2b7fadc33ecff9fcb4c6067c675ad7d14bb8b71f383f243e558ae552cf8da05`  
		Last Modified: Fri, 20 Oct 2023 20:38:15 GMT  
		Size: 883.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9d193449aafd2e76aefe49f553ee2d007ed850656e18916b74c5d28057e6cfb7`  
		Last Modified: Fri, 20 Oct 2023 20:38:15 GMT  
		Size: 913.0 KB (912965 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6ea497c74b15661c8dcda90c65a4d6878277fb00ba8ce6c4b71bab676b372c34`  
		Last Modified: Fri, 20 Oct 2023 20:38:16 GMT  
		Size: 4.3 MB (4302158 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7778acbf55f327acde293ae0092a016ebf0324943d47aa131140a802397301d2`  
		Last Modified: Fri, 20 Oct 2023 20:38:16 GMT  
		Size: 2.6 KB (2607 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fa2675fd414a6242f407f6b5a8bd013f30d2bad261deb6a6a440e1121da1857a`  
		Last Modified: Fri, 20 Oct 2023 20:40:01 GMT  
		Size: 332.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d24f782b47329ae0e2c2e08d37b0a47553fb07bd5dadb7ea7e91f570f559084a`  
		Last Modified: Fri, 20 Oct 2023 20:40:07 GMT  
		Size: 57.5 MB (57454168 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d72061df12b27dfb6b550389fdadb3bc290a2cf8f5baaa58828fe7efb543d359`  
		Last Modified: Fri, 20 Oct 2023 20:40:01 GMT  
		Size: 315.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:44c59a54226d295d690d41a35b4c9fa1bb3b8a106e062b6129ea176b19d17dac`  
		Last Modified: Fri, 20 Oct 2023 20:40:06 GMT  
		Size: 63.8 MB (63780363 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c8eba2a1704137c2b007bc0efdbb676a8b8b58a1b2b6e1deaa5422fd5a687b64`  
		Last Modified: Fri, 20 Oct 2023 20:40:03 GMT  
		Size: 5.4 KB (5394 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0c1c0cd211c9ba4d8a84ae33b95fcc805e19bd7f5c1b33cc5b4ae25d8b65eb95`  
		Last Modified: Fri, 20 Oct 2023 20:40:03 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:8.0-oracle` - unknown; unknown

```console
$ docker pull mysql@sha256:02b282dd539f9d295b046ade8c8e5fceaa55fae8ae5a1c06a7f73661febe933e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.2 MB (11244647 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5e7bd00c2deab1e38d8476e0d21ad22483ad150defe9046127684ce18187823`

```dockerfile
```

-	Layers:
	-	`sha256:6f2dda0ddc63496263d54aec6345f9c431c1010428062119568b0710affab9ca`  
		Last Modified: Fri, 20 Oct 2023 20:40:02 GMT  
		Size: 11.2 MB (11210610 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:d5f8fca198352f62646eb00da40475ee7c1fd82d42f01a54d8e4bd4cf257eb8d`  
		Last Modified: Fri, 20 Oct 2023 20:40:01 GMT  
		Size: 34.0 KB (34037 bytes)  
		MIME: application/vnd.in-toto+json

## `mysql:8.0.34`

```console
$ docker pull mysql@sha256:59ae56ac42c6c09aebd9a7bb8d9f07a5fdf836f956e050946f85bbfa29d0a080
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `mysql:8.0.34` - linux; amd64

```console
$ docker pull mysql@sha256:8b8835a2c32cd7357a5d2ea4b49ad870ff519c8c1d4add362803feddf4a0a973
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **165.9 MB (165869861 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1d66a2a0aa16e23edc8d1c1e08be4a0ba8c239c9414a90b1d0cb4944ca4a194`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 20 Jul 2023 22:15:44 GMT
ADD file:0f45bdf93b14a2ab9389b71d23b6c7f6d2935c8016e3b6422814f8fc79bef986 in / 
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
	-	`sha256:8e0176adc18c476bdfcc701f01cda5acf49bc8e6d7fadac8072091a43fafbb25`  
		Last Modified: Fri, 20 Oct 2023 18:28:56 GMT  
		Size: 44.3 MB (44279620 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:de512b6f1736a825c3faf1f6e29b250af00fdb081c26d02f1276237265d272e2`  
		Last Modified: Fri, 20 Oct 2023 19:04:03 GMT  
		Size: 882.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fb3459be0c6886d8c2e23eb23a582006b68738b48bd52db4bd1303d9ae8286c6`  
		Last Modified: Fri, 20 Oct 2023 19:04:03 GMT  
		Size: 982.8 KB (982809 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:77379308b924f78d087b9cfded2b5333247182de433e11417ea7d81f2c574f27`  
		Last Modified: Fri, 20 Oct 2023 19:04:03 GMT  
		Size: 4.6 MB (4613882 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bfadef6257d17e2d887a0bfdf3948749ed43e98f99eff26251fc63f3e6b2cef3`  
		Last Modified: Fri, 20 Oct 2023 19:04:04 GMT  
		Size: 2.6 KB (2609 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5034ed0fbcb845f3118bc99cd00e20d01ef0c8ce7ad6ce378833004e55c90948`  
		Last Modified: Fri, 20 Oct 2023 19:04:05 GMT  
		Size: 333.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c0363a641ba973d0dc144b009898cb31c06a4c04dde2b2f59a553407e463abb6`  
		Last Modified: Fri, 20 Oct 2023 19:04:08 GMT  
		Size: 58.5 MB (58486052 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:49cafcd8a97548e00aba56544fe0d961c8de101a22f560158687c6ea874e2543`  
		Last Modified: Fri, 20 Oct 2023 19:04:05 GMT  
		Size: 318.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c2f92e2c3315cb55c51e20d5f9da7105d08e0c94a1ff8264a6b59dc3f19384c2`  
		Last Modified: Fri, 20 Oct 2023 19:04:11 GMT  
		Size: 57.5 MB (57497846 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a3f49bb45462ec43aa4975c1480f1a980dc0a0f9063d1dccb9a2371529de4d9d`  
		Last Modified: Fri, 20 Oct 2023 19:04:06 GMT  
		Size: 5.4 KB (5388 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7238affa01f6b755e3715d2269dc451392b079dc8c242ea2204a29d3f6d212ae`  
		Last Modified: Fri, 20 Oct 2023 19:04:08 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:8.0.34` - unknown; unknown

```console
$ docker pull mysql@sha256:9b23f72f8ec6a984af3064cbe759daecda0037c7227e116e98689f75e7729762
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.2 MB (11246228 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6905ab0de6eb417c6c062b8a3dbbcd3462314eb33b04baf8ecf1ea0fa9a7ec63`

```dockerfile
```

-	Layers:
	-	`sha256:b7b94af060c390356daf63f3b9b9424a11d553e7f628f0d900c26f670219f63f`  
		Last Modified: Fri, 20 Oct 2023 19:04:04 GMT  
		Size: 11.2 MB (11212034 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:0cefd81b6c7497a200591b31f91e0ed09959f3d14aa5685f673b86d9c5ff38c7`  
		Last Modified: Fri, 20 Oct 2023 19:04:03 GMT  
		Size: 34.2 KB (34194 bytes)  
		MIME: application/vnd.in-toto+json

### `mysql:8.0.34` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:3c362d5eed04f271a2ebad41f45fed5ed86e934da533a079bcbd2b3a4ff372e8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.1 MB (170132091 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93db1e4f7846804531842503e6855d382e5647732a309f62a46a736f649fd5cf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 20 Jul 2023 22:15:44 GMT
ADD file:e189ba41c54c386435a3292026b75a1386976d3222102c16a725f58f594f284e in / 
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
	-	`sha256:e39ec8f010eb75816ae2c21b014f7fdecffb48374079b6f1bce017214e2a45cd`  
		Last Modified: Fri, 20 Oct 2023 18:40:29 GMT  
		Size: 43.7 MB (43672784 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e2b7fadc33ecff9fcb4c6067c675ad7d14bb8b71f383f243e558ae552cf8da05`  
		Last Modified: Fri, 20 Oct 2023 20:38:15 GMT  
		Size: 883.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9d193449aafd2e76aefe49f553ee2d007ed850656e18916b74c5d28057e6cfb7`  
		Last Modified: Fri, 20 Oct 2023 20:38:15 GMT  
		Size: 913.0 KB (912965 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6ea497c74b15661c8dcda90c65a4d6878277fb00ba8ce6c4b71bab676b372c34`  
		Last Modified: Fri, 20 Oct 2023 20:38:16 GMT  
		Size: 4.3 MB (4302158 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7778acbf55f327acde293ae0092a016ebf0324943d47aa131140a802397301d2`  
		Last Modified: Fri, 20 Oct 2023 20:38:16 GMT  
		Size: 2.6 KB (2607 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fa2675fd414a6242f407f6b5a8bd013f30d2bad261deb6a6a440e1121da1857a`  
		Last Modified: Fri, 20 Oct 2023 20:40:01 GMT  
		Size: 332.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d24f782b47329ae0e2c2e08d37b0a47553fb07bd5dadb7ea7e91f570f559084a`  
		Last Modified: Fri, 20 Oct 2023 20:40:07 GMT  
		Size: 57.5 MB (57454168 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d72061df12b27dfb6b550389fdadb3bc290a2cf8f5baaa58828fe7efb543d359`  
		Last Modified: Fri, 20 Oct 2023 20:40:01 GMT  
		Size: 315.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:44c59a54226d295d690d41a35b4c9fa1bb3b8a106e062b6129ea176b19d17dac`  
		Last Modified: Fri, 20 Oct 2023 20:40:06 GMT  
		Size: 63.8 MB (63780363 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c8eba2a1704137c2b007bc0efdbb676a8b8b58a1b2b6e1deaa5422fd5a687b64`  
		Last Modified: Fri, 20 Oct 2023 20:40:03 GMT  
		Size: 5.4 KB (5394 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0c1c0cd211c9ba4d8a84ae33b95fcc805e19bd7f5c1b33cc5b4ae25d8b65eb95`  
		Last Modified: Fri, 20 Oct 2023 20:40:03 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:8.0.34` - unknown; unknown

```console
$ docker pull mysql@sha256:02b282dd539f9d295b046ade8c8e5fceaa55fae8ae5a1c06a7f73661febe933e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.2 MB (11244647 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5e7bd00c2deab1e38d8476e0d21ad22483ad150defe9046127684ce18187823`

```dockerfile
```

-	Layers:
	-	`sha256:6f2dda0ddc63496263d54aec6345f9c431c1010428062119568b0710affab9ca`  
		Last Modified: Fri, 20 Oct 2023 20:40:02 GMT  
		Size: 11.2 MB (11210610 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:d5f8fca198352f62646eb00da40475ee7c1fd82d42f01a54d8e4bd4cf257eb8d`  
		Last Modified: Fri, 20 Oct 2023 20:40:01 GMT  
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
$ docker pull mysql@sha256:59ae56ac42c6c09aebd9a7bb8d9f07a5fdf836f956e050946f85bbfa29d0a080
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `mysql:8.0.34-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:8b8835a2c32cd7357a5d2ea4b49ad870ff519c8c1d4add362803feddf4a0a973
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **165.9 MB (165869861 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1d66a2a0aa16e23edc8d1c1e08be4a0ba8c239c9414a90b1d0cb4944ca4a194`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 20 Jul 2023 22:15:44 GMT
ADD file:0f45bdf93b14a2ab9389b71d23b6c7f6d2935c8016e3b6422814f8fc79bef986 in / 
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
	-	`sha256:8e0176adc18c476bdfcc701f01cda5acf49bc8e6d7fadac8072091a43fafbb25`  
		Last Modified: Fri, 20 Oct 2023 18:28:56 GMT  
		Size: 44.3 MB (44279620 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:de512b6f1736a825c3faf1f6e29b250af00fdb081c26d02f1276237265d272e2`  
		Last Modified: Fri, 20 Oct 2023 19:04:03 GMT  
		Size: 882.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fb3459be0c6886d8c2e23eb23a582006b68738b48bd52db4bd1303d9ae8286c6`  
		Last Modified: Fri, 20 Oct 2023 19:04:03 GMT  
		Size: 982.8 KB (982809 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:77379308b924f78d087b9cfded2b5333247182de433e11417ea7d81f2c574f27`  
		Last Modified: Fri, 20 Oct 2023 19:04:03 GMT  
		Size: 4.6 MB (4613882 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bfadef6257d17e2d887a0bfdf3948749ed43e98f99eff26251fc63f3e6b2cef3`  
		Last Modified: Fri, 20 Oct 2023 19:04:04 GMT  
		Size: 2.6 KB (2609 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5034ed0fbcb845f3118bc99cd00e20d01ef0c8ce7ad6ce378833004e55c90948`  
		Last Modified: Fri, 20 Oct 2023 19:04:05 GMT  
		Size: 333.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c0363a641ba973d0dc144b009898cb31c06a4c04dde2b2f59a553407e463abb6`  
		Last Modified: Fri, 20 Oct 2023 19:04:08 GMT  
		Size: 58.5 MB (58486052 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:49cafcd8a97548e00aba56544fe0d961c8de101a22f560158687c6ea874e2543`  
		Last Modified: Fri, 20 Oct 2023 19:04:05 GMT  
		Size: 318.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c2f92e2c3315cb55c51e20d5f9da7105d08e0c94a1ff8264a6b59dc3f19384c2`  
		Last Modified: Fri, 20 Oct 2023 19:04:11 GMT  
		Size: 57.5 MB (57497846 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a3f49bb45462ec43aa4975c1480f1a980dc0a0f9063d1dccb9a2371529de4d9d`  
		Last Modified: Fri, 20 Oct 2023 19:04:06 GMT  
		Size: 5.4 KB (5388 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7238affa01f6b755e3715d2269dc451392b079dc8c242ea2204a29d3f6d212ae`  
		Last Modified: Fri, 20 Oct 2023 19:04:08 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:8.0.34-oracle` - unknown; unknown

```console
$ docker pull mysql@sha256:9b23f72f8ec6a984af3064cbe759daecda0037c7227e116e98689f75e7729762
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.2 MB (11246228 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6905ab0de6eb417c6c062b8a3dbbcd3462314eb33b04baf8ecf1ea0fa9a7ec63`

```dockerfile
```

-	Layers:
	-	`sha256:b7b94af060c390356daf63f3b9b9424a11d553e7f628f0d900c26f670219f63f`  
		Last Modified: Fri, 20 Oct 2023 19:04:04 GMT  
		Size: 11.2 MB (11212034 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:0cefd81b6c7497a200591b31f91e0ed09959f3d14aa5685f673b86d9c5ff38c7`  
		Last Modified: Fri, 20 Oct 2023 19:04:03 GMT  
		Size: 34.2 KB (34194 bytes)  
		MIME: application/vnd.in-toto+json

### `mysql:8.0.34-oracle` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:3c362d5eed04f271a2ebad41f45fed5ed86e934da533a079bcbd2b3a4ff372e8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.1 MB (170132091 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93db1e4f7846804531842503e6855d382e5647732a309f62a46a736f649fd5cf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 20 Jul 2023 22:15:44 GMT
ADD file:e189ba41c54c386435a3292026b75a1386976d3222102c16a725f58f594f284e in / 
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
	-	`sha256:e39ec8f010eb75816ae2c21b014f7fdecffb48374079b6f1bce017214e2a45cd`  
		Last Modified: Fri, 20 Oct 2023 18:40:29 GMT  
		Size: 43.7 MB (43672784 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e2b7fadc33ecff9fcb4c6067c675ad7d14bb8b71f383f243e558ae552cf8da05`  
		Last Modified: Fri, 20 Oct 2023 20:38:15 GMT  
		Size: 883.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9d193449aafd2e76aefe49f553ee2d007ed850656e18916b74c5d28057e6cfb7`  
		Last Modified: Fri, 20 Oct 2023 20:38:15 GMT  
		Size: 913.0 KB (912965 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6ea497c74b15661c8dcda90c65a4d6878277fb00ba8ce6c4b71bab676b372c34`  
		Last Modified: Fri, 20 Oct 2023 20:38:16 GMT  
		Size: 4.3 MB (4302158 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7778acbf55f327acde293ae0092a016ebf0324943d47aa131140a802397301d2`  
		Last Modified: Fri, 20 Oct 2023 20:38:16 GMT  
		Size: 2.6 KB (2607 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fa2675fd414a6242f407f6b5a8bd013f30d2bad261deb6a6a440e1121da1857a`  
		Last Modified: Fri, 20 Oct 2023 20:40:01 GMT  
		Size: 332.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d24f782b47329ae0e2c2e08d37b0a47553fb07bd5dadb7ea7e91f570f559084a`  
		Last Modified: Fri, 20 Oct 2023 20:40:07 GMT  
		Size: 57.5 MB (57454168 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d72061df12b27dfb6b550389fdadb3bc290a2cf8f5baaa58828fe7efb543d359`  
		Last Modified: Fri, 20 Oct 2023 20:40:01 GMT  
		Size: 315.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:44c59a54226d295d690d41a35b4c9fa1bb3b8a106e062b6129ea176b19d17dac`  
		Last Modified: Fri, 20 Oct 2023 20:40:06 GMT  
		Size: 63.8 MB (63780363 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c8eba2a1704137c2b007bc0efdbb676a8b8b58a1b2b6e1deaa5422fd5a687b64`  
		Last Modified: Fri, 20 Oct 2023 20:40:03 GMT  
		Size: 5.4 KB (5394 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0c1c0cd211c9ba4d8a84ae33b95fcc805e19bd7f5c1b33cc5b4ae25d8b65eb95`  
		Last Modified: Fri, 20 Oct 2023 20:40:03 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:8.0.34-oracle` - unknown; unknown

```console
$ docker pull mysql@sha256:02b282dd539f9d295b046ade8c8e5fceaa55fae8ae5a1c06a7f73661febe933e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.2 MB (11244647 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5e7bd00c2deab1e38d8476e0d21ad22483ad150defe9046127684ce18187823`

```dockerfile
```

-	Layers:
	-	`sha256:6f2dda0ddc63496263d54aec6345f9c431c1010428062119568b0710affab9ca`  
		Last Modified: Fri, 20 Oct 2023 20:40:02 GMT  
		Size: 11.2 MB (11210610 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:d5f8fca198352f62646eb00da40475ee7c1fd82d42f01a54d8e4bd4cf257eb8d`  
		Last Modified: Fri, 20 Oct 2023 20:40:01 GMT  
		Size: 34.0 KB (34037 bytes)  
		MIME: application/vnd.in-toto+json

## `mysql:8.1`

```console
$ docker pull mysql@sha256:f61944ff3f2961363a4d22913b2ac581523273679d7e14dd26e8db8c9f571a7e
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `mysql:8.1` - linux; amd64

```console
$ docker pull mysql@sha256:c458b26f2f9f9fe086ed75d1f8db8e2dde371801403f2c7da9be4fb228a2944a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **166.1 MB (166123241 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae2502152260b33bfafb9c3e3a1811086317e0236abf83a59503cec0f8980573`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 27 Jul 2023 22:18:51 GMT
ADD file:0f45bdf93b14a2ab9389b71d23b6c7f6d2935c8016e3b6422814f8fc79bef986 in / 
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
	-	`sha256:8e0176adc18c476bdfcc701f01cda5acf49bc8e6d7fadac8072091a43fafbb25`  
		Last Modified: Fri, 20 Oct 2023 18:28:56 GMT  
		Size: 44.3 MB (44279620 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:14e977b0f4b2310e3eaed27abcab0fad4dae8f9bafa8f77c4ed5316fff629f2f`  
		Last Modified: Fri, 20 Oct 2023 19:04:04 GMT  
		Size: 885.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a7b58dd6f78b98d9ff6fbc049f2f7cb84174c74dd57cacbdb185f9b896bb2919`  
		Last Modified: Fri, 20 Oct 2023 19:04:05 GMT  
		Size: 982.8 KB (982806 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fba70cc872a5b5a727ef28a9ed8203ad526cb069dc21dcad1076bcf98286ffa5`  
		Last Modified: Fri, 20 Oct 2023 19:04:05 GMT  
		Size: 4.6 MB (4613864 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5db2cc6eab8f76e59babee0c88038ba1e7d20bbdca06ae1fc2480d89aee76343`  
		Last Modified: Fri, 20 Oct 2023 19:04:05 GMT  
		Size: 2.6 KB (2607 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:081f41f573ba759e534574da506eb0a6593adb408cf88d3f9c5c7665c8d0807f`  
		Last Modified: Fri, 20 Oct 2023 19:04:06 GMT  
		Size: 339.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:86bf2dc4ded9433a1f0b2155401a202843311dc129425e4a35f193dbdb4254f9`  
		Last Modified: Fri, 20 Oct 2023 19:04:11 GMT  
		Size: 58.8 MB (58754172 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:47f08b0e916e6e60dc941429579e860a2f1c4b6eeaedd5600bac7391f41c7733`  
		Last Modified: Fri, 20 Oct 2023 19:04:07 GMT  
		Size: 317.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:850e29ae8eeb4a7f347575c2fa8f159be328eacad69cc27f5376b7836b808a5f`  
		Last Modified: Fri, 20 Oct 2023 19:04:10 GMT  
		Size: 57.5 MB (57483245 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:13517fe0d921160b87a62dea36c2d361e7936b2fa5e8c4319001c6e472fbd166`  
		Last Modified: Fri, 20 Oct 2023 19:04:08 GMT  
		Size: 5.4 KB (5386 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:8.1` - unknown; unknown

```console
$ docker pull mysql@sha256:2faea6171999069839076bda0781b64056aab4ea0d102220851de5690d238082
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.2 MB (11247404 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:abc364c5064a4eca4aab69f869586ab10aacdf0add869b720111829105492cbc`

```dockerfile
```

-	Layers:
	-	`sha256:5900cd702aca9703a447153286a87bf27042d3f0cdcfbde3c19f960bf2053668`  
		Last Modified: Fri, 20 Oct 2023 19:04:05 GMT  
		Size: 11.2 MB (11213826 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:f3a630b6ecb72d9898f9adf3385edfa15b93e6184b045b18842358fd8c6ae3cf`  
		Last Modified: Fri, 20 Oct 2023 19:04:04 GMT  
		Size: 33.6 KB (33578 bytes)  
		MIME: application/vnd.in-toto+json

### `mysql:8.1` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:376751ad5724968a1dc5cb624852332955a0f82adf09c2d903023fc79c80a178
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.4 MB (170390818 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d858cb210e4b84459d06dc864905ffa5d12429467e45db806ade28932e5bd65d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 27 Jul 2023 22:18:51 GMT
ADD file:e189ba41c54c386435a3292026b75a1386976d3222102c16a725f58f594f284e in / 
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
	-	`sha256:e39ec8f010eb75816ae2c21b014f7fdecffb48374079b6f1bce017214e2a45cd`  
		Last Modified: Fri, 20 Oct 2023 18:40:29 GMT  
		Size: 43.7 MB (43672784 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e2b7fadc33ecff9fcb4c6067c675ad7d14bb8b71f383f243e558ae552cf8da05`  
		Last Modified: Fri, 20 Oct 2023 20:38:15 GMT  
		Size: 883.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9d193449aafd2e76aefe49f553ee2d007ed850656e18916b74c5d28057e6cfb7`  
		Last Modified: Fri, 20 Oct 2023 20:38:15 GMT  
		Size: 913.0 KB (912965 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6ea497c74b15661c8dcda90c65a4d6878277fb00ba8ce6c4b71bab676b372c34`  
		Last Modified: Fri, 20 Oct 2023 20:38:16 GMT  
		Size: 4.3 MB (4302158 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7778acbf55f327acde293ae0092a016ebf0324943d47aa131140a802397301d2`  
		Last Modified: Fri, 20 Oct 2023 20:38:16 GMT  
		Size: 2.6 KB (2607 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b65a5d7a2435a3664f7d77ed9e51646b62721b51396b27ff9d2853dd377ec76d`  
		Last Modified: Fri, 20 Oct 2023 20:38:16 GMT  
		Size: 339.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cef9fb0078a5e4eb83b7675f763bcf1e93ba403dd95139d00679313915b83831`  
		Last Modified: Fri, 20 Oct 2023 20:38:20 GMT  
		Size: 57.7 MB (57702031 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5b6dc73ec72424a05d131a7d8bbc28951e86bf53ebd4cd79a7d3777baacd5dd9`  
		Last Modified: Fri, 20 Oct 2023 20:38:18 GMT  
		Size: 317.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d992bb39e209c72e87bf31c42c6b1a34210084f585778ab64dd129de5e2c2672`  
		Last Modified: Fri, 20 Oct 2023 20:38:21 GMT  
		Size: 63.8 MB (63791340 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4431432b89a3ffd8f9dafe35d1a3c42ceb8caa0f23eda1f67b2e29eabf00412a`  
		Last Modified: Fri, 20 Oct 2023 20:38:18 GMT  
		Size: 5.4 KB (5394 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:8.1` - unknown; unknown

```console
$ docker pull mysql@sha256:287fd970d795844678660fc69a6c613789e5b61134e6b755b61afda3f925122e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.2 MB (11246015 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e28ecb6013e37bf1ec95d4ce0d35d11ddbc3d02006aae2aafed3d536dec4cea`

```dockerfile
```

-	Layers:
	-	`sha256:e386e5c32eff52a8f31e3168432997b2fc1924a764878f857a4039968d5b4355`  
		Last Modified: Fri, 20 Oct 2023 20:38:16 GMT  
		Size: 11.2 MB (11212414 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:93236631c96ce25fe9eb4000349de4979b3f67ab3c5fc4d22628d8bd9fb98ddf`  
		Last Modified: Fri, 20 Oct 2023 20:38:15 GMT  
		Size: 33.6 KB (33601 bytes)  
		MIME: application/vnd.in-toto+json

## `mysql:8.1-oracle`

```console
$ docker pull mysql@sha256:f61944ff3f2961363a4d22913b2ac581523273679d7e14dd26e8db8c9f571a7e
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `mysql:8.1-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:c458b26f2f9f9fe086ed75d1f8db8e2dde371801403f2c7da9be4fb228a2944a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **166.1 MB (166123241 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae2502152260b33bfafb9c3e3a1811086317e0236abf83a59503cec0f8980573`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 27 Jul 2023 22:18:51 GMT
ADD file:0f45bdf93b14a2ab9389b71d23b6c7f6d2935c8016e3b6422814f8fc79bef986 in / 
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
	-	`sha256:8e0176adc18c476bdfcc701f01cda5acf49bc8e6d7fadac8072091a43fafbb25`  
		Last Modified: Fri, 20 Oct 2023 18:28:56 GMT  
		Size: 44.3 MB (44279620 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:14e977b0f4b2310e3eaed27abcab0fad4dae8f9bafa8f77c4ed5316fff629f2f`  
		Last Modified: Fri, 20 Oct 2023 19:04:04 GMT  
		Size: 885.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a7b58dd6f78b98d9ff6fbc049f2f7cb84174c74dd57cacbdb185f9b896bb2919`  
		Last Modified: Fri, 20 Oct 2023 19:04:05 GMT  
		Size: 982.8 KB (982806 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fba70cc872a5b5a727ef28a9ed8203ad526cb069dc21dcad1076bcf98286ffa5`  
		Last Modified: Fri, 20 Oct 2023 19:04:05 GMT  
		Size: 4.6 MB (4613864 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5db2cc6eab8f76e59babee0c88038ba1e7d20bbdca06ae1fc2480d89aee76343`  
		Last Modified: Fri, 20 Oct 2023 19:04:05 GMT  
		Size: 2.6 KB (2607 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:081f41f573ba759e534574da506eb0a6593adb408cf88d3f9c5c7665c8d0807f`  
		Last Modified: Fri, 20 Oct 2023 19:04:06 GMT  
		Size: 339.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:86bf2dc4ded9433a1f0b2155401a202843311dc129425e4a35f193dbdb4254f9`  
		Last Modified: Fri, 20 Oct 2023 19:04:11 GMT  
		Size: 58.8 MB (58754172 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:47f08b0e916e6e60dc941429579e860a2f1c4b6eeaedd5600bac7391f41c7733`  
		Last Modified: Fri, 20 Oct 2023 19:04:07 GMT  
		Size: 317.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:850e29ae8eeb4a7f347575c2fa8f159be328eacad69cc27f5376b7836b808a5f`  
		Last Modified: Fri, 20 Oct 2023 19:04:10 GMT  
		Size: 57.5 MB (57483245 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:13517fe0d921160b87a62dea36c2d361e7936b2fa5e8c4319001c6e472fbd166`  
		Last Modified: Fri, 20 Oct 2023 19:04:08 GMT  
		Size: 5.4 KB (5386 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:8.1-oracle` - unknown; unknown

```console
$ docker pull mysql@sha256:2faea6171999069839076bda0781b64056aab4ea0d102220851de5690d238082
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.2 MB (11247404 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:abc364c5064a4eca4aab69f869586ab10aacdf0add869b720111829105492cbc`

```dockerfile
```

-	Layers:
	-	`sha256:5900cd702aca9703a447153286a87bf27042d3f0cdcfbde3c19f960bf2053668`  
		Last Modified: Fri, 20 Oct 2023 19:04:05 GMT  
		Size: 11.2 MB (11213826 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:f3a630b6ecb72d9898f9adf3385edfa15b93e6184b045b18842358fd8c6ae3cf`  
		Last Modified: Fri, 20 Oct 2023 19:04:04 GMT  
		Size: 33.6 KB (33578 bytes)  
		MIME: application/vnd.in-toto+json

### `mysql:8.1-oracle` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:376751ad5724968a1dc5cb624852332955a0f82adf09c2d903023fc79c80a178
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.4 MB (170390818 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d858cb210e4b84459d06dc864905ffa5d12429467e45db806ade28932e5bd65d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 27 Jul 2023 22:18:51 GMT
ADD file:e189ba41c54c386435a3292026b75a1386976d3222102c16a725f58f594f284e in / 
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
	-	`sha256:e39ec8f010eb75816ae2c21b014f7fdecffb48374079b6f1bce017214e2a45cd`  
		Last Modified: Fri, 20 Oct 2023 18:40:29 GMT  
		Size: 43.7 MB (43672784 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e2b7fadc33ecff9fcb4c6067c675ad7d14bb8b71f383f243e558ae552cf8da05`  
		Last Modified: Fri, 20 Oct 2023 20:38:15 GMT  
		Size: 883.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9d193449aafd2e76aefe49f553ee2d007ed850656e18916b74c5d28057e6cfb7`  
		Last Modified: Fri, 20 Oct 2023 20:38:15 GMT  
		Size: 913.0 KB (912965 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6ea497c74b15661c8dcda90c65a4d6878277fb00ba8ce6c4b71bab676b372c34`  
		Last Modified: Fri, 20 Oct 2023 20:38:16 GMT  
		Size: 4.3 MB (4302158 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7778acbf55f327acde293ae0092a016ebf0324943d47aa131140a802397301d2`  
		Last Modified: Fri, 20 Oct 2023 20:38:16 GMT  
		Size: 2.6 KB (2607 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b65a5d7a2435a3664f7d77ed9e51646b62721b51396b27ff9d2853dd377ec76d`  
		Last Modified: Fri, 20 Oct 2023 20:38:16 GMT  
		Size: 339.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cef9fb0078a5e4eb83b7675f763bcf1e93ba403dd95139d00679313915b83831`  
		Last Modified: Fri, 20 Oct 2023 20:38:20 GMT  
		Size: 57.7 MB (57702031 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5b6dc73ec72424a05d131a7d8bbc28951e86bf53ebd4cd79a7d3777baacd5dd9`  
		Last Modified: Fri, 20 Oct 2023 20:38:18 GMT  
		Size: 317.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d992bb39e209c72e87bf31c42c6b1a34210084f585778ab64dd129de5e2c2672`  
		Last Modified: Fri, 20 Oct 2023 20:38:21 GMT  
		Size: 63.8 MB (63791340 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4431432b89a3ffd8f9dafe35d1a3c42ceb8caa0f23eda1f67b2e29eabf00412a`  
		Last Modified: Fri, 20 Oct 2023 20:38:18 GMT  
		Size: 5.4 KB (5394 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:8.1-oracle` - unknown; unknown

```console
$ docker pull mysql@sha256:287fd970d795844678660fc69a6c613789e5b61134e6b755b61afda3f925122e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.2 MB (11246015 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e28ecb6013e37bf1ec95d4ce0d35d11ddbc3d02006aae2aafed3d536dec4cea`

```dockerfile
```

-	Layers:
	-	`sha256:e386e5c32eff52a8f31e3168432997b2fc1924a764878f857a4039968d5b4355`  
		Last Modified: Fri, 20 Oct 2023 20:38:16 GMT  
		Size: 11.2 MB (11212414 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:93236631c96ce25fe9eb4000349de4979b3f67ab3c5fc4d22628d8bd9fb98ddf`  
		Last Modified: Fri, 20 Oct 2023 20:38:15 GMT  
		Size: 33.6 KB (33601 bytes)  
		MIME: application/vnd.in-toto+json

## `mysql:8.1.0`

```console
$ docker pull mysql@sha256:f61944ff3f2961363a4d22913b2ac581523273679d7e14dd26e8db8c9f571a7e
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `mysql:8.1.0` - linux; amd64

```console
$ docker pull mysql@sha256:c458b26f2f9f9fe086ed75d1f8db8e2dde371801403f2c7da9be4fb228a2944a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **166.1 MB (166123241 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae2502152260b33bfafb9c3e3a1811086317e0236abf83a59503cec0f8980573`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 27 Jul 2023 22:18:51 GMT
ADD file:0f45bdf93b14a2ab9389b71d23b6c7f6d2935c8016e3b6422814f8fc79bef986 in / 
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
	-	`sha256:8e0176adc18c476bdfcc701f01cda5acf49bc8e6d7fadac8072091a43fafbb25`  
		Last Modified: Fri, 20 Oct 2023 18:28:56 GMT  
		Size: 44.3 MB (44279620 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:14e977b0f4b2310e3eaed27abcab0fad4dae8f9bafa8f77c4ed5316fff629f2f`  
		Last Modified: Fri, 20 Oct 2023 19:04:04 GMT  
		Size: 885.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a7b58dd6f78b98d9ff6fbc049f2f7cb84174c74dd57cacbdb185f9b896bb2919`  
		Last Modified: Fri, 20 Oct 2023 19:04:05 GMT  
		Size: 982.8 KB (982806 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fba70cc872a5b5a727ef28a9ed8203ad526cb069dc21dcad1076bcf98286ffa5`  
		Last Modified: Fri, 20 Oct 2023 19:04:05 GMT  
		Size: 4.6 MB (4613864 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5db2cc6eab8f76e59babee0c88038ba1e7d20bbdca06ae1fc2480d89aee76343`  
		Last Modified: Fri, 20 Oct 2023 19:04:05 GMT  
		Size: 2.6 KB (2607 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:081f41f573ba759e534574da506eb0a6593adb408cf88d3f9c5c7665c8d0807f`  
		Last Modified: Fri, 20 Oct 2023 19:04:06 GMT  
		Size: 339.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:86bf2dc4ded9433a1f0b2155401a202843311dc129425e4a35f193dbdb4254f9`  
		Last Modified: Fri, 20 Oct 2023 19:04:11 GMT  
		Size: 58.8 MB (58754172 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:47f08b0e916e6e60dc941429579e860a2f1c4b6eeaedd5600bac7391f41c7733`  
		Last Modified: Fri, 20 Oct 2023 19:04:07 GMT  
		Size: 317.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:850e29ae8eeb4a7f347575c2fa8f159be328eacad69cc27f5376b7836b808a5f`  
		Last Modified: Fri, 20 Oct 2023 19:04:10 GMT  
		Size: 57.5 MB (57483245 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:13517fe0d921160b87a62dea36c2d361e7936b2fa5e8c4319001c6e472fbd166`  
		Last Modified: Fri, 20 Oct 2023 19:04:08 GMT  
		Size: 5.4 KB (5386 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:8.1.0` - unknown; unknown

```console
$ docker pull mysql@sha256:2faea6171999069839076bda0781b64056aab4ea0d102220851de5690d238082
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.2 MB (11247404 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:abc364c5064a4eca4aab69f869586ab10aacdf0add869b720111829105492cbc`

```dockerfile
```

-	Layers:
	-	`sha256:5900cd702aca9703a447153286a87bf27042d3f0cdcfbde3c19f960bf2053668`  
		Last Modified: Fri, 20 Oct 2023 19:04:05 GMT  
		Size: 11.2 MB (11213826 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:f3a630b6ecb72d9898f9adf3385edfa15b93e6184b045b18842358fd8c6ae3cf`  
		Last Modified: Fri, 20 Oct 2023 19:04:04 GMT  
		Size: 33.6 KB (33578 bytes)  
		MIME: application/vnd.in-toto+json

### `mysql:8.1.0` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:376751ad5724968a1dc5cb624852332955a0f82adf09c2d903023fc79c80a178
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.4 MB (170390818 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d858cb210e4b84459d06dc864905ffa5d12429467e45db806ade28932e5bd65d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 27 Jul 2023 22:18:51 GMT
ADD file:e189ba41c54c386435a3292026b75a1386976d3222102c16a725f58f594f284e in / 
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
	-	`sha256:e39ec8f010eb75816ae2c21b014f7fdecffb48374079b6f1bce017214e2a45cd`  
		Last Modified: Fri, 20 Oct 2023 18:40:29 GMT  
		Size: 43.7 MB (43672784 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e2b7fadc33ecff9fcb4c6067c675ad7d14bb8b71f383f243e558ae552cf8da05`  
		Last Modified: Fri, 20 Oct 2023 20:38:15 GMT  
		Size: 883.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9d193449aafd2e76aefe49f553ee2d007ed850656e18916b74c5d28057e6cfb7`  
		Last Modified: Fri, 20 Oct 2023 20:38:15 GMT  
		Size: 913.0 KB (912965 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6ea497c74b15661c8dcda90c65a4d6878277fb00ba8ce6c4b71bab676b372c34`  
		Last Modified: Fri, 20 Oct 2023 20:38:16 GMT  
		Size: 4.3 MB (4302158 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7778acbf55f327acde293ae0092a016ebf0324943d47aa131140a802397301d2`  
		Last Modified: Fri, 20 Oct 2023 20:38:16 GMT  
		Size: 2.6 KB (2607 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b65a5d7a2435a3664f7d77ed9e51646b62721b51396b27ff9d2853dd377ec76d`  
		Last Modified: Fri, 20 Oct 2023 20:38:16 GMT  
		Size: 339.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cef9fb0078a5e4eb83b7675f763bcf1e93ba403dd95139d00679313915b83831`  
		Last Modified: Fri, 20 Oct 2023 20:38:20 GMT  
		Size: 57.7 MB (57702031 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5b6dc73ec72424a05d131a7d8bbc28951e86bf53ebd4cd79a7d3777baacd5dd9`  
		Last Modified: Fri, 20 Oct 2023 20:38:18 GMT  
		Size: 317.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d992bb39e209c72e87bf31c42c6b1a34210084f585778ab64dd129de5e2c2672`  
		Last Modified: Fri, 20 Oct 2023 20:38:21 GMT  
		Size: 63.8 MB (63791340 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4431432b89a3ffd8f9dafe35d1a3c42ceb8caa0f23eda1f67b2e29eabf00412a`  
		Last Modified: Fri, 20 Oct 2023 20:38:18 GMT  
		Size: 5.4 KB (5394 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:8.1.0` - unknown; unknown

```console
$ docker pull mysql@sha256:287fd970d795844678660fc69a6c613789e5b61134e6b755b61afda3f925122e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.2 MB (11246015 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e28ecb6013e37bf1ec95d4ce0d35d11ddbc3d02006aae2aafed3d536dec4cea`

```dockerfile
```

-	Layers:
	-	`sha256:e386e5c32eff52a8f31e3168432997b2fc1924a764878f857a4039968d5b4355`  
		Last Modified: Fri, 20 Oct 2023 20:38:16 GMT  
		Size: 11.2 MB (11212414 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:93236631c96ce25fe9eb4000349de4979b3f67ab3c5fc4d22628d8bd9fb98ddf`  
		Last Modified: Fri, 20 Oct 2023 20:38:15 GMT  
		Size: 33.6 KB (33601 bytes)  
		MIME: application/vnd.in-toto+json

## `mysql:8.1.0-oracle`

```console
$ docker pull mysql@sha256:f61944ff3f2961363a4d22913b2ac581523273679d7e14dd26e8db8c9f571a7e
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `mysql:8.1.0-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:c458b26f2f9f9fe086ed75d1f8db8e2dde371801403f2c7da9be4fb228a2944a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **166.1 MB (166123241 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae2502152260b33bfafb9c3e3a1811086317e0236abf83a59503cec0f8980573`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 27 Jul 2023 22:18:51 GMT
ADD file:0f45bdf93b14a2ab9389b71d23b6c7f6d2935c8016e3b6422814f8fc79bef986 in / 
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
	-	`sha256:8e0176adc18c476bdfcc701f01cda5acf49bc8e6d7fadac8072091a43fafbb25`  
		Last Modified: Fri, 20 Oct 2023 18:28:56 GMT  
		Size: 44.3 MB (44279620 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:14e977b0f4b2310e3eaed27abcab0fad4dae8f9bafa8f77c4ed5316fff629f2f`  
		Last Modified: Fri, 20 Oct 2023 19:04:04 GMT  
		Size: 885.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a7b58dd6f78b98d9ff6fbc049f2f7cb84174c74dd57cacbdb185f9b896bb2919`  
		Last Modified: Fri, 20 Oct 2023 19:04:05 GMT  
		Size: 982.8 KB (982806 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fba70cc872a5b5a727ef28a9ed8203ad526cb069dc21dcad1076bcf98286ffa5`  
		Last Modified: Fri, 20 Oct 2023 19:04:05 GMT  
		Size: 4.6 MB (4613864 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5db2cc6eab8f76e59babee0c88038ba1e7d20bbdca06ae1fc2480d89aee76343`  
		Last Modified: Fri, 20 Oct 2023 19:04:05 GMT  
		Size: 2.6 KB (2607 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:081f41f573ba759e534574da506eb0a6593adb408cf88d3f9c5c7665c8d0807f`  
		Last Modified: Fri, 20 Oct 2023 19:04:06 GMT  
		Size: 339.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:86bf2dc4ded9433a1f0b2155401a202843311dc129425e4a35f193dbdb4254f9`  
		Last Modified: Fri, 20 Oct 2023 19:04:11 GMT  
		Size: 58.8 MB (58754172 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:47f08b0e916e6e60dc941429579e860a2f1c4b6eeaedd5600bac7391f41c7733`  
		Last Modified: Fri, 20 Oct 2023 19:04:07 GMT  
		Size: 317.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:850e29ae8eeb4a7f347575c2fa8f159be328eacad69cc27f5376b7836b808a5f`  
		Last Modified: Fri, 20 Oct 2023 19:04:10 GMT  
		Size: 57.5 MB (57483245 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:13517fe0d921160b87a62dea36c2d361e7936b2fa5e8c4319001c6e472fbd166`  
		Last Modified: Fri, 20 Oct 2023 19:04:08 GMT  
		Size: 5.4 KB (5386 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:8.1.0-oracle` - unknown; unknown

```console
$ docker pull mysql@sha256:2faea6171999069839076bda0781b64056aab4ea0d102220851de5690d238082
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.2 MB (11247404 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:abc364c5064a4eca4aab69f869586ab10aacdf0add869b720111829105492cbc`

```dockerfile
```

-	Layers:
	-	`sha256:5900cd702aca9703a447153286a87bf27042d3f0cdcfbde3c19f960bf2053668`  
		Last Modified: Fri, 20 Oct 2023 19:04:05 GMT  
		Size: 11.2 MB (11213826 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:f3a630b6ecb72d9898f9adf3385edfa15b93e6184b045b18842358fd8c6ae3cf`  
		Last Modified: Fri, 20 Oct 2023 19:04:04 GMT  
		Size: 33.6 KB (33578 bytes)  
		MIME: application/vnd.in-toto+json

### `mysql:8.1.0-oracle` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:376751ad5724968a1dc5cb624852332955a0f82adf09c2d903023fc79c80a178
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.4 MB (170390818 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d858cb210e4b84459d06dc864905ffa5d12429467e45db806ade28932e5bd65d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 27 Jul 2023 22:18:51 GMT
ADD file:e189ba41c54c386435a3292026b75a1386976d3222102c16a725f58f594f284e in / 
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
	-	`sha256:e39ec8f010eb75816ae2c21b014f7fdecffb48374079b6f1bce017214e2a45cd`  
		Last Modified: Fri, 20 Oct 2023 18:40:29 GMT  
		Size: 43.7 MB (43672784 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e2b7fadc33ecff9fcb4c6067c675ad7d14bb8b71f383f243e558ae552cf8da05`  
		Last Modified: Fri, 20 Oct 2023 20:38:15 GMT  
		Size: 883.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9d193449aafd2e76aefe49f553ee2d007ed850656e18916b74c5d28057e6cfb7`  
		Last Modified: Fri, 20 Oct 2023 20:38:15 GMT  
		Size: 913.0 KB (912965 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6ea497c74b15661c8dcda90c65a4d6878277fb00ba8ce6c4b71bab676b372c34`  
		Last Modified: Fri, 20 Oct 2023 20:38:16 GMT  
		Size: 4.3 MB (4302158 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7778acbf55f327acde293ae0092a016ebf0324943d47aa131140a802397301d2`  
		Last Modified: Fri, 20 Oct 2023 20:38:16 GMT  
		Size: 2.6 KB (2607 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b65a5d7a2435a3664f7d77ed9e51646b62721b51396b27ff9d2853dd377ec76d`  
		Last Modified: Fri, 20 Oct 2023 20:38:16 GMT  
		Size: 339.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cef9fb0078a5e4eb83b7675f763bcf1e93ba403dd95139d00679313915b83831`  
		Last Modified: Fri, 20 Oct 2023 20:38:20 GMT  
		Size: 57.7 MB (57702031 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5b6dc73ec72424a05d131a7d8bbc28951e86bf53ebd4cd79a7d3777baacd5dd9`  
		Last Modified: Fri, 20 Oct 2023 20:38:18 GMT  
		Size: 317.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d992bb39e209c72e87bf31c42c6b1a34210084f585778ab64dd129de5e2c2672`  
		Last Modified: Fri, 20 Oct 2023 20:38:21 GMT  
		Size: 63.8 MB (63791340 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4431432b89a3ffd8f9dafe35d1a3c42ceb8caa0f23eda1f67b2e29eabf00412a`  
		Last Modified: Fri, 20 Oct 2023 20:38:18 GMT  
		Size: 5.4 KB (5394 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:8.1.0-oracle` - unknown; unknown

```console
$ docker pull mysql@sha256:287fd970d795844678660fc69a6c613789e5b61134e6b755b61afda3f925122e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.2 MB (11246015 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e28ecb6013e37bf1ec95d4ce0d35d11ddbc3d02006aae2aafed3d536dec4cea`

```dockerfile
```

-	Layers:
	-	`sha256:e386e5c32eff52a8f31e3168432997b2fc1924a764878f857a4039968d5b4355`  
		Last Modified: Fri, 20 Oct 2023 20:38:16 GMT  
		Size: 11.2 MB (11212414 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:93236631c96ce25fe9eb4000349de4979b3f67ab3c5fc4d22628d8bd9fb98ddf`  
		Last Modified: Fri, 20 Oct 2023 20:38:15 GMT  
		Size: 33.6 KB (33601 bytes)  
		MIME: application/vnd.in-toto+json

## `mysql:innovation`

```console
$ docker pull mysql@sha256:f61944ff3f2961363a4d22913b2ac581523273679d7e14dd26e8db8c9f571a7e
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `mysql:innovation` - linux; amd64

```console
$ docker pull mysql@sha256:c458b26f2f9f9fe086ed75d1f8db8e2dde371801403f2c7da9be4fb228a2944a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **166.1 MB (166123241 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae2502152260b33bfafb9c3e3a1811086317e0236abf83a59503cec0f8980573`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 27 Jul 2023 22:18:51 GMT
ADD file:0f45bdf93b14a2ab9389b71d23b6c7f6d2935c8016e3b6422814f8fc79bef986 in / 
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
	-	`sha256:8e0176adc18c476bdfcc701f01cda5acf49bc8e6d7fadac8072091a43fafbb25`  
		Last Modified: Fri, 20 Oct 2023 18:28:56 GMT  
		Size: 44.3 MB (44279620 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:14e977b0f4b2310e3eaed27abcab0fad4dae8f9bafa8f77c4ed5316fff629f2f`  
		Last Modified: Fri, 20 Oct 2023 19:04:04 GMT  
		Size: 885.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a7b58dd6f78b98d9ff6fbc049f2f7cb84174c74dd57cacbdb185f9b896bb2919`  
		Last Modified: Fri, 20 Oct 2023 19:04:05 GMT  
		Size: 982.8 KB (982806 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fba70cc872a5b5a727ef28a9ed8203ad526cb069dc21dcad1076bcf98286ffa5`  
		Last Modified: Fri, 20 Oct 2023 19:04:05 GMT  
		Size: 4.6 MB (4613864 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5db2cc6eab8f76e59babee0c88038ba1e7d20bbdca06ae1fc2480d89aee76343`  
		Last Modified: Fri, 20 Oct 2023 19:04:05 GMT  
		Size: 2.6 KB (2607 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:081f41f573ba759e534574da506eb0a6593adb408cf88d3f9c5c7665c8d0807f`  
		Last Modified: Fri, 20 Oct 2023 19:04:06 GMT  
		Size: 339.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:86bf2dc4ded9433a1f0b2155401a202843311dc129425e4a35f193dbdb4254f9`  
		Last Modified: Fri, 20 Oct 2023 19:04:11 GMT  
		Size: 58.8 MB (58754172 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:47f08b0e916e6e60dc941429579e860a2f1c4b6eeaedd5600bac7391f41c7733`  
		Last Modified: Fri, 20 Oct 2023 19:04:07 GMT  
		Size: 317.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:850e29ae8eeb4a7f347575c2fa8f159be328eacad69cc27f5376b7836b808a5f`  
		Last Modified: Fri, 20 Oct 2023 19:04:10 GMT  
		Size: 57.5 MB (57483245 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:13517fe0d921160b87a62dea36c2d361e7936b2fa5e8c4319001c6e472fbd166`  
		Last Modified: Fri, 20 Oct 2023 19:04:08 GMT  
		Size: 5.4 KB (5386 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:innovation` - unknown; unknown

```console
$ docker pull mysql@sha256:2faea6171999069839076bda0781b64056aab4ea0d102220851de5690d238082
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.2 MB (11247404 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:abc364c5064a4eca4aab69f869586ab10aacdf0add869b720111829105492cbc`

```dockerfile
```

-	Layers:
	-	`sha256:5900cd702aca9703a447153286a87bf27042d3f0cdcfbde3c19f960bf2053668`  
		Last Modified: Fri, 20 Oct 2023 19:04:05 GMT  
		Size: 11.2 MB (11213826 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:f3a630b6ecb72d9898f9adf3385edfa15b93e6184b045b18842358fd8c6ae3cf`  
		Last Modified: Fri, 20 Oct 2023 19:04:04 GMT  
		Size: 33.6 KB (33578 bytes)  
		MIME: application/vnd.in-toto+json

### `mysql:innovation` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:376751ad5724968a1dc5cb624852332955a0f82adf09c2d903023fc79c80a178
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.4 MB (170390818 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d858cb210e4b84459d06dc864905ffa5d12429467e45db806ade28932e5bd65d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 27 Jul 2023 22:18:51 GMT
ADD file:e189ba41c54c386435a3292026b75a1386976d3222102c16a725f58f594f284e in / 
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
	-	`sha256:e39ec8f010eb75816ae2c21b014f7fdecffb48374079b6f1bce017214e2a45cd`  
		Last Modified: Fri, 20 Oct 2023 18:40:29 GMT  
		Size: 43.7 MB (43672784 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e2b7fadc33ecff9fcb4c6067c675ad7d14bb8b71f383f243e558ae552cf8da05`  
		Last Modified: Fri, 20 Oct 2023 20:38:15 GMT  
		Size: 883.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9d193449aafd2e76aefe49f553ee2d007ed850656e18916b74c5d28057e6cfb7`  
		Last Modified: Fri, 20 Oct 2023 20:38:15 GMT  
		Size: 913.0 KB (912965 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6ea497c74b15661c8dcda90c65a4d6878277fb00ba8ce6c4b71bab676b372c34`  
		Last Modified: Fri, 20 Oct 2023 20:38:16 GMT  
		Size: 4.3 MB (4302158 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7778acbf55f327acde293ae0092a016ebf0324943d47aa131140a802397301d2`  
		Last Modified: Fri, 20 Oct 2023 20:38:16 GMT  
		Size: 2.6 KB (2607 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b65a5d7a2435a3664f7d77ed9e51646b62721b51396b27ff9d2853dd377ec76d`  
		Last Modified: Fri, 20 Oct 2023 20:38:16 GMT  
		Size: 339.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cef9fb0078a5e4eb83b7675f763bcf1e93ba403dd95139d00679313915b83831`  
		Last Modified: Fri, 20 Oct 2023 20:38:20 GMT  
		Size: 57.7 MB (57702031 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5b6dc73ec72424a05d131a7d8bbc28951e86bf53ebd4cd79a7d3777baacd5dd9`  
		Last Modified: Fri, 20 Oct 2023 20:38:18 GMT  
		Size: 317.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d992bb39e209c72e87bf31c42c6b1a34210084f585778ab64dd129de5e2c2672`  
		Last Modified: Fri, 20 Oct 2023 20:38:21 GMT  
		Size: 63.8 MB (63791340 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4431432b89a3ffd8f9dafe35d1a3c42ceb8caa0f23eda1f67b2e29eabf00412a`  
		Last Modified: Fri, 20 Oct 2023 20:38:18 GMT  
		Size: 5.4 KB (5394 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:innovation` - unknown; unknown

```console
$ docker pull mysql@sha256:287fd970d795844678660fc69a6c613789e5b61134e6b755b61afda3f925122e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.2 MB (11246015 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e28ecb6013e37bf1ec95d4ce0d35d11ddbc3d02006aae2aafed3d536dec4cea`

```dockerfile
```

-	Layers:
	-	`sha256:e386e5c32eff52a8f31e3168432997b2fc1924a764878f857a4039968d5b4355`  
		Last Modified: Fri, 20 Oct 2023 20:38:16 GMT  
		Size: 11.2 MB (11212414 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:93236631c96ce25fe9eb4000349de4979b3f67ab3c5fc4d22628d8bd9fb98ddf`  
		Last Modified: Fri, 20 Oct 2023 20:38:15 GMT  
		Size: 33.6 KB (33601 bytes)  
		MIME: application/vnd.in-toto+json

## `mysql:innovation-oracle`

```console
$ docker pull mysql@sha256:f61944ff3f2961363a4d22913b2ac581523273679d7e14dd26e8db8c9f571a7e
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `mysql:innovation-oracle` - linux; amd64

```console
$ docker pull mysql@sha256:c458b26f2f9f9fe086ed75d1f8db8e2dde371801403f2c7da9be4fb228a2944a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **166.1 MB (166123241 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae2502152260b33bfafb9c3e3a1811086317e0236abf83a59503cec0f8980573`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 27 Jul 2023 22:18:51 GMT
ADD file:0f45bdf93b14a2ab9389b71d23b6c7f6d2935c8016e3b6422814f8fc79bef986 in / 
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
	-	`sha256:8e0176adc18c476bdfcc701f01cda5acf49bc8e6d7fadac8072091a43fafbb25`  
		Last Modified: Fri, 20 Oct 2023 18:28:56 GMT  
		Size: 44.3 MB (44279620 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:14e977b0f4b2310e3eaed27abcab0fad4dae8f9bafa8f77c4ed5316fff629f2f`  
		Last Modified: Fri, 20 Oct 2023 19:04:04 GMT  
		Size: 885.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a7b58dd6f78b98d9ff6fbc049f2f7cb84174c74dd57cacbdb185f9b896bb2919`  
		Last Modified: Fri, 20 Oct 2023 19:04:05 GMT  
		Size: 982.8 KB (982806 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fba70cc872a5b5a727ef28a9ed8203ad526cb069dc21dcad1076bcf98286ffa5`  
		Last Modified: Fri, 20 Oct 2023 19:04:05 GMT  
		Size: 4.6 MB (4613864 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5db2cc6eab8f76e59babee0c88038ba1e7d20bbdca06ae1fc2480d89aee76343`  
		Last Modified: Fri, 20 Oct 2023 19:04:05 GMT  
		Size: 2.6 KB (2607 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:081f41f573ba759e534574da506eb0a6593adb408cf88d3f9c5c7665c8d0807f`  
		Last Modified: Fri, 20 Oct 2023 19:04:06 GMT  
		Size: 339.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:86bf2dc4ded9433a1f0b2155401a202843311dc129425e4a35f193dbdb4254f9`  
		Last Modified: Fri, 20 Oct 2023 19:04:11 GMT  
		Size: 58.8 MB (58754172 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:47f08b0e916e6e60dc941429579e860a2f1c4b6eeaedd5600bac7391f41c7733`  
		Last Modified: Fri, 20 Oct 2023 19:04:07 GMT  
		Size: 317.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:850e29ae8eeb4a7f347575c2fa8f159be328eacad69cc27f5376b7836b808a5f`  
		Last Modified: Fri, 20 Oct 2023 19:04:10 GMT  
		Size: 57.5 MB (57483245 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:13517fe0d921160b87a62dea36c2d361e7936b2fa5e8c4319001c6e472fbd166`  
		Last Modified: Fri, 20 Oct 2023 19:04:08 GMT  
		Size: 5.4 KB (5386 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:innovation-oracle` - unknown; unknown

```console
$ docker pull mysql@sha256:2faea6171999069839076bda0781b64056aab4ea0d102220851de5690d238082
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.2 MB (11247404 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:abc364c5064a4eca4aab69f869586ab10aacdf0add869b720111829105492cbc`

```dockerfile
```

-	Layers:
	-	`sha256:5900cd702aca9703a447153286a87bf27042d3f0cdcfbde3c19f960bf2053668`  
		Last Modified: Fri, 20 Oct 2023 19:04:05 GMT  
		Size: 11.2 MB (11213826 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:f3a630b6ecb72d9898f9adf3385edfa15b93e6184b045b18842358fd8c6ae3cf`  
		Last Modified: Fri, 20 Oct 2023 19:04:04 GMT  
		Size: 33.6 KB (33578 bytes)  
		MIME: application/vnd.in-toto+json

### `mysql:innovation-oracle` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:376751ad5724968a1dc5cb624852332955a0f82adf09c2d903023fc79c80a178
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.4 MB (170390818 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d858cb210e4b84459d06dc864905ffa5d12429467e45db806ade28932e5bd65d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 27 Jul 2023 22:18:51 GMT
ADD file:e189ba41c54c386435a3292026b75a1386976d3222102c16a725f58f594f284e in / 
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
	-	`sha256:e39ec8f010eb75816ae2c21b014f7fdecffb48374079b6f1bce017214e2a45cd`  
		Last Modified: Fri, 20 Oct 2023 18:40:29 GMT  
		Size: 43.7 MB (43672784 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e2b7fadc33ecff9fcb4c6067c675ad7d14bb8b71f383f243e558ae552cf8da05`  
		Last Modified: Fri, 20 Oct 2023 20:38:15 GMT  
		Size: 883.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9d193449aafd2e76aefe49f553ee2d007ed850656e18916b74c5d28057e6cfb7`  
		Last Modified: Fri, 20 Oct 2023 20:38:15 GMT  
		Size: 913.0 KB (912965 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6ea497c74b15661c8dcda90c65a4d6878277fb00ba8ce6c4b71bab676b372c34`  
		Last Modified: Fri, 20 Oct 2023 20:38:16 GMT  
		Size: 4.3 MB (4302158 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7778acbf55f327acde293ae0092a016ebf0324943d47aa131140a802397301d2`  
		Last Modified: Fri, 20 Oct 2023 20:38:16 GMT  
		Size: 2.6 KB (2607 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b65a5d7a2435a3664f7d77ed9e51646b62721b51396b27ff9d2853dd377ec76d`  
		Last Modified: Fri, 20 Oct 2023 20:38:16 GMT  
		Size: 339.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cef9fb0078a5e4eb83b7675f763bcf1e93ba403dd95139d00679313915b83831`  
		Last Modified: Fri, 20 Oct 2023 20:38:20 GMT  
		Size: 57.7 MB (57702031 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5b6dc73ec72424a05d131a7d8bbc28951e86bf53ebd4cd79a7d3777baacd5dd9`  
		Last Modified: Fri, 20 Oct 2023 20:38:18 GMT  
		Size: 317.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d992bb39e209c72e87bf31c42c6b1a34210084f585778ab64dd129de5e2c2672`  
		Last Modified: Fri, 20 Oct 2023 20:38:21 GMT  
		Size: 63.8 MB (63791340 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4431432b89a3ffd8f9dafe35d1a3c42ceb8caa0f23eda1f67b2e29eabf00412a`  
		Last Modified: Fri, 20 Oct 2023 20:38:18 GMT  
		Size: 5.4 KB (5394 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:innovation-oracle` - unknown; unknown

```console
$ docker pull mysql@sha256:287fd970d795844678660fc69a6c613789e5b61134e6b755b61afda3f925122e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.2 MB (11246015 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e28ecb6013e37bf1ec95d4ce0d35d11ddbc3d02006aae2aafed3d536dec4cea`

```dockerfile
```

-	Layers:
	-	`sha256:e386e5c32eff52a8f31e3168432997b2fc1924a764878f857a4039968d5b4355`  
		Last Modified: Fri, 20 Oct 2023 20:38:16 GMT  
		Size: 11.2 MB (11212414 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:93236631c96ce25fe9eb4000349de4979b3f67ab3c5fc4d22628d8bd9fb98ddf`  
		Last Modified: Fri, 20 Oct 2023 20:38:15 GMT  
		Size: 33.6 KB (33601 bytes)  
		MIME: application/vnd.in-toto+json

## `mysql:latest`

```console
$ docker pull mysql@sha256:f61944ff3f2961363a4d22913b2ac581523273679d7e14dd26e8db8c9f571a7e
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `mysql:latest` - linux; amd64

```console
$ docker pull mysql@sha256:c458b26f2f9f9fe086ed75d1f8db8e2dde371801403f2c7da9be4fb228a2944a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **166.1 MB (166123241 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae2502152260b33bfafb9c3e3a1811086317e0236abf83a59503cec0f8980573`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 27 Jul 2023 22:18:51 GMT
ADD file:0f45bdf93b14a2ab9389b71d23b6c7f6d2935c8016e3b6422814f8fc79bef986 in / 
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
	-	`sha256:8e0176adc18c476bdfcc701f01cda5acf49bc8e6d7fadac8072091a43fafbb25`  
		Last Modified: Fri, 20 Oct 2023 18:28:56 GMT  
		Size: 44.3 MB (44279620 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:14e977b0f4b2310e3eaed27abcab0fad4dae8f9bafa8f77c4ed5316fff629f2f`  
		Last Modified: Fri, 20 Oct 2023 19:04:04 GMT  
		Size: 885.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a7b58dd6f78b98d9ff6fbc049f2f7cb84174c74dd57cacbdb185f9b896bb2919`  
		Last Modified: Fri, 20 Oct 2023 19:04:05 GMT  
		Size: 982.8 KB (982806 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fba70cc872a5b5a727ef28a9ed8203ad526cb069dc21dcad1076bcf98286ffa5`  
		Last Modified: Fri, 20 Oct 2023 19:04:05 GMT  
		Size: 4.6 MB (4613864 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5db2cc6eab8f76e59babee0c88038ba1e7d20bbdca06ae1fc2480d89aee76343`  
		Last Modified: Fri, 20 Oct 2023 19:04:05 GMT  
		Size: 2.6 KB (2607 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:081f41f573ba759e534574da506eb0a6593adb408cf88d3f9c5c7665c8d0807f`  
		Last Modified: Fri, 20 Oct 2023 19:04:06 GMT  
		Size: 339.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:86bf2dc4ded9433a1f0b2155401a202843311dc129425e4a35f193dbdb4254f9`  
		Last Modified: Fri, 20 Oct 2023 19:04:11 GMT  
		Size: 58.8 MB (58754172 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:47f08b0e916e6e60dc941429579e860a2f1c4b6eeaedd5600bac7391f41c7733`  
		Last Modified: Fri, 20 Oct 2023 19:04:07 GMT  
		Size: 317.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:850e29ae8eeb4a7f347575c2fa8f159be328eacad69cc27f5376b7836b808a5f`  
		Last Modified: Fri, 20 Oct 2023 19:04:10 GMT  
		Size: 57.5 MB (57483245 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:13517fe0d921160b87a62dea36c2d361e7936b2fa5e8c4319001c6e472fbd166`  
		Last Modified: Fri, 20 Oct 2023 19:04:08 GMT  
		Size: 5.4 KB (5386 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:latest` - unknown; unknown

```console
$ docker pull mysql@sha256:2faea6171999069839076bda0781b64056aab4ea0d102220851de5690d238082
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.2 MB (11247404 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:abc364c5064a4eca4aab69f869586ab10aacdf0add869b720111829105492cbc`

```dockerfile
```

-	Layers:
	-	`sha256:5900cd702aca9703a447153286a87bf27042d3f0cdcfbde3c19f960bf2053668`  
		Last Modified: Fri, 20 Oct 2023 19:04:05 GMT  
		Size: 11.2 MB (11213826 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:f3a630b6ecb72d9898f9adf3385edfa15b93e6184b045b18842358fd8c6ae3cf`  
		Last Modified: Fri, 20 Oct 2023 19:04:04 GMT  
		Size: 33.6 KB (33578 bytes)  
		MIME: application/vnd.in-toto+json

### `mysql:latest` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:376751ad5724968a1dc5cb624852332955a0f82adf09c2d903023fc79c80a178
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.4 MB (170390818 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d858cb210e4b84459d06dc864905ffa5d12429467e45db806ade28932e5bd65d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 27 Jul 2023 22:18:51 GMT
ADD file:e189ba41c54c386435a3292026b75a1386976d3222102c16a725f58f594f284e in / 
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
	-	`sha256:e39ec8f010eb75816ae2c21b014f7fdecffb48374079b6f1bce017214e2a45cd`  
		Last Modified: Fri, 20 Oct 2023 18:40:29 GMT  
		Size: 43.7 MB (43672784 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e2b7fadc33ecff9fcb4c6067c675ad7d14bb8b71f383f243e558ae552cf8da05`  
		Last Modified: Fri, 20 Oct 2023 20:38:15 GMT  
		Size: 883.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9d193449aafd2e76aefe49f553ee2d007ed850656e18916b74c5d28057e6cfb7`  
		Last Modified: Fri, 20 Oct 2023 20:38:15 GMT  
		Size: 913.0 KB (912965 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6ea497c74b15661c8dcda90c65a4d6878277fb00ba8ce6c4b71bab676b372c34`  
		Last Modified: Fri, 20 Oct 2023 20:38:16 GMT  
		Size: 4.3 MB (4302158 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7778acbf55f327acde293ae0092a016ebf0324943d47aa131140a802397301d2`  
		Last Modified: Fri, 20 Oct 2023 20:38:16 GMT  
		Size: 2.6 KB (2607 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b65a5d7a2435a3664f7d77ed9e51646b62721b51396b27ff9d2853dd377ec76d`  
		Last Modified: Fri, 20 Oct 2023 20:38:16 GMT  
		Size: 339.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cef9fb0078a5e4eb83b7675f763bcf1e93ba403dd95139d00679313915b83831`  
		Last Modified: Fri, 20 Oct 2023 20:38:20 GMT  
		Size: 57.7 MB (57702031 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5b6dc73ec72424a05d131a7d8bbc28951e86bf53ebd4cd79a7d3777baacd5dd9`  
		Last Modified: Fri, 20 Oct 2023 20:38:18 GMT  
		Size: 317.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d992bb39e209c72e87bf31c42c6b1a34210084f585778ab64dd129de5e2c2672`  
		Last Modified: Fri, 20 Oct 2023 20:38:21 GMT  
		Size: 63.8 MB (63791340 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4431432b89a3ffd8f9dafe35d1a3c42ceb8caa0f23eda1f67b2e29eabf00412a`  
		Last Modified: Fri, 20 Oct 2023 20:38:18 GMT  
		Size: 5.4 KB (5394 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:latest` - unknown; unknown

```console
$ docker pull mysql@sha256:287fd970d795844678660fc69a6c613789e5b61134e6b755b61afda3f925122e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.2 MB (11246015 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e28ecb6013e37bf1ec95d4ce0d35d11ddbc3d02006aae2aafed3d536dec4cea`

```dockerfile
```

-	Layers:
	-	`sha256:e386e5c32eff52a8f31e3168432997b2fc1924a764878f857a4039968d5b4355`  
		Last Modified: Fri, 20 Oct 2023 20:38:16 GMT  
		Size: 11.2 MB (11212414 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:93236631c96ce25fe9eb4000349de4979b3f67ab3c5fc4d22628d8bd9fb98ddf`  
		Last Modified: Fri, 20 Oct 2023 20:38:15 GMT  
		Size: 33.6 KB (33601 bytes)  
		MIME: application/vnd.in-toto+json

## `mysql:oracle`

```console
$ docker pull mysql@sha256:f61944ff3f2961363a4d22913b2ac581523273679d7e14dd26e8db8c9f571a7e
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `mysql:oracle` - linux; amd64

```console
$ docker pull mysql@sha256:c458b26f2f9f9fe086ed75d1f8db8e2dde371801403f2c7da9be4fb228a2944a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **166.1 MB (166123241 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae2502152260b33bfafb9c3e3a1811086317e0236abf83a59503cec0f8980573`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 27 Jul 2023 22:18:51 GMT
ADD file:0f45bdf93b14a2ab9389b71d23b6c7f6d2935c8016e3b6422814f8fc79bef986 in / 
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
	-	`sha256:8e0176adc18c476bdfcc701f01cda5acf49bc8e6d7fadac8072091a43fafbb25`  
		Last Modified: Fri, 20 Oct 2023 18:28:56 GMT  
		Size: 44.3 MB (44279620 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:14e977b0f4b2310e3eaed27abcab0fad4dae8f9bafa8f77c4ed5316fff629f2f`  
		Last Modified: Fri, 20 Oct 2023 19:04:04 GMT  
		Size: 885.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a7b58dd6f78b98d9ff6fbc049f2f7cb84174c74dd57cacbdb185f9b896bb2919`  
		Last Modified: Fri, 20 Oct 2023 19:04:05 GMT  
		Size: 982.8 KB (982806 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fba70cc872a5b5a727ef28a9ed8203ad526cb069dc21dcad1076bcf98286ffa5`  
		Last Modified: Fri, 20 Oct 2023 19:04:05 GMT  
		Size: 4.6 MB (4613864 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5db2cc6eab8f76e59babee0c88038ba1e7d20bbdca06ae1fc2480d89aee76343`  
		Last Modified: Fri, 20 Oct 2023 19:04:05 GMT  
		Size: 2.6 KB (2607 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:081f41f573ba759e534574da506eb0a6593adb408cf88d3f9c5c7665c8d0807f`  
		Last Modified: Fri, 20 Oct 2023 19:04:06 GMT  
		Size: 339.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:86bf2dc4ded9433a1f0b2155401a202843311dc129425e4a35f193dbdb4254f9`  
		Last Modified: Fri, 20 Oct 2023 19:04:11 GMT  
		Size: 58.8 MB (58754172 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:47f08b0e916e6e60dc941429579e860a2f1c4b6eeaedd5600bac7391f41c7733`  
		Last Modified: Fri, 20 Oct 2023 19:04:07 GMT  
		Size: 317.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:850e29ae8eeb4a7f347575c2fa8f159be328eacad69cc27f5376b7836b808a5f`  
		Last Modified: Fri, 20 Oct 2023 19:04:10 GMT  
		Size: 57.5 MB (57483245 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:13517fe0d921160b87a62dea36c2d361e7936b2fa5e8c4319001c6e472fbd166`  
		Last Modified: Fri, 20 Oct 2023 19:04:08 GMT  
		Size: 5.4 KB (5386 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:oracle` - unknown; unknown

```console
$ docker pull mysql@sha256:2faea6171999069839076bda0781b64056aab4ea0d102220851de5690d238082
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.2 MB (11247404 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:abc364c5064a4eca4aab69f869586ab10aacdf0add869b720111829105492cbc`

```dockerfile
```

-	Layers:
	-	`sha256:5900cd702aca9703a447153286a87bf27042d3f0cdcfbde3c19f960bf2053668`  
		Last Modified: Fri, 20 Oct 2023 19:04:05 GMT  
		Size: 11.2 MB (11213826 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:f3a630b6ecb72d9898f9adf3385edfa15b93e6184b045b18842358fd8c6ae3cf`  
		Last Modified: Fri, 20 Oct 2023 19:04:04 GMT  
		Size: 33.6 KB (33578 bytes)  
		MIME: application/vnd.in-toto+json

### `mysql:oracle` - linux; arm64 variant v8

```console
$ docker pull mysql@sha256:376751ad5724968a1dc5cb624852332955a0f82adf09c2d903023fc79c80a178
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.4 MB (170390818 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d858cb210e4b84459d06dc864905ffa5d12429467e45db806ade28932e5bd65d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mysqld"]`

```dockerfile
# Thu, 27 Jul 2023 22:18:51 GMT
ADD file:e189ba41c54c386435a3292026b75a1386976d3222102c16a725f58f594f284e in / 
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
	-	`sha256:e39ec8f010eb75816ae2c21b014f7fdecffb48374079b6f1bce017214e2a45cd`  
		Last Modified: Fri, 20 Oct 2023 18:40:29 GMT  
		Size: 43.7 MB (43672784 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e2b7fadc33ecff9fcb4c6067c675ad7d14bb8b71f383f243e558ae552cf8da05`  
		Last Modified: Fri, 20 Oct 2023 20:38:15 GMT  
		Size: 883.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9d193449aafd2e76aefe49f553ee2d007ed850656e18916b74c5d28057e6cfb7`  
		Last Modified: Fri, 20 Oct 2023 20:38:15 GMT  
		Size: 913.0 KB (912965 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6ea497c74b15661c8dcda90c65a4d6878277fb00ba8ce6c4b71bab676b372c34`  
		Last Modified: Fri, 20 Oct 2023 20:38:16 GMT  
		Size: 4.3 MB (4302158 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7778acbf55f327acde293ae0092a016ebf0324943d47aa131140a802397301d2`  
		Last Modified: Fri, 20 Oct 2023 20:38:16 GMT  
		Size: 2.6 KB (2607 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b65a5d7a2435a3664f7d77ed9e51646b62721b51396b27ff9d2853dd377ec76d`  
		Last Modified: Fri, 20 Oct 2023 20:38:16 GMT  
		Size: 339.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cef9fb0078a5e4eb83b7675f763bcf1e93ba403dd95139d00679313915b83831`  
		Last Modified: Fri, 20 Oct 2023 20:38:20 GMT  
		Size: 57.7 MB (57702031 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5b6dc73ec72424a05d131a7d8bbc28951e86bf53ebd4cd79a7d3777baacd5dd9`  
		Last Modified: Fri, 20 Oct 2023 20:38:18 GMT  
		Size: 317.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d992bb39e209c72e87bf31c42c6b1a34210084f585778ab64dd129de5e2c2672`  
		Last Modified: Fri, 20 Oct 2023 20:38:21 GMT  
		Size: 63.8 MB (63791340 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4431432b89a3ffd8f9dafe35d1a3c42ceb8caa0f23eda1f67b2e29eabf00412a`  
		Last Modified: Fri, 20 Oct 2023 20:38:18 GMT  
		Size: 5.4 KB (5394 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `mysql:oracle` - unknown; unknown

```console
$ docker pull mysql@sha256:287fd970d795844678660fc69a6c613789e5b61134e6b755b61afda3f925122e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.2 MB (11246015 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e28ecb6013e37bf1ec95d4ce0d35d11ddbc3d02006aae2aafed3d536dec4cea`

```dockerfile
```

-	Layers:
	-	`sha256:e386e5c32eff52a8f31e3168432997b2fc1924a764878f857a4039968d5b4355`  
		Last Modified: Fri, 20 Oct 2023 20:38:16 GMT  
		Size: 11.2 MB (11212414 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:93236631c96ce25fe9eb4000349de4979b3f67ab3c5fc4d22628d8bd9fb98ddf`  
		Last Modified: Fri, 20 Oct 2023 20:38:15 GMT  
		Size: 33.6 KB (33601 bytes)  
		MIME: application/vnd.in-toto+json
