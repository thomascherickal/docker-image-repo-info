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
