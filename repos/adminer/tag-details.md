<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `adminer`

-	[`adminer:4`](#adminer4)
-	[`adminer:4-fastcgi`](#adminer4-fastcgi)
-	[`adminer:4-standalone`](#adminer4-standalone)
-	[`adminer:4.8.1`](#adminer481)
-	[`adminer:4.8.1-fastcgi`](#adminer481-fastcgi)
-	[`adminer:4.8.1-standalone`](#adminer481-standalone)
-	[`adminer:fastcgi`](#adminerfastcgi)
-	[`adminer:latest`](#adminerlatest)
-	[`adminer:standalone`](#adminerstandalone)

## `adminer:4`

```console
$ docker pull adminer@sha256:d4a361f0fdbc2f8a4732a62635e043e7a883e3785a54d54f5eb0d9ce3ad80204
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `adminer:4` - linux; amd64

```console
$ docker pull adminer@sha256:8991350a6cc5acd8a607828617ad1cbd062b38528e6889664e0030b43f45d5f8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.9 MB (95901310 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:471e5d2fb746396a521960c56f7eafb8490e52be8cb499d4c0e00904c673be4e`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Sat, 04 Feb 2023 06:51:26 GMT
ADD file:cc6a56676703ec7ab5db8f2f7bc18a3169c0816d38703845b6b77ae5342ab41c in / 
# Sat, 04 Feb 2023 06:51:27 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 14:02:55 GMT
STOPSIGNAL SIGINT
# Sat, 04 Feb 2023 14:03:16 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 14:03:17 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Sat, 04 Feb 2023 14:03:17 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Sat, 04 Feb 2023 14:03:17 GMT
WORKDIR /var/www/html
# Sat, 04 Feb 2023 14:03:18 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Sat, 04 Feb 2023 14:03:18 GMT
ENV ADMINER_VERSION=4.8.1
# Sat, 04 Feb 2023 14:03:18 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Sat, 04 Feb 2023 14:03:18 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Sat, 04 Feb 2023 14:03:30 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 04 Feb 2023 14:03:30 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Sat, 04 Feb 2023 14:03:30 GMT
ENTRYPOINT ["entrypoint.sh"]
# Sat, 04 Feb 2023 14:03:30 GMT
USER adminer
# Sat, 04 Feb 2023 14:03:30 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Sat, 04 Feb 2023 14:03:30 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:699c8a97647f5789e5850bcf1a3d5afe9730edb654e1ae0714d5bd198a67a3ed`  
		Last Modified: Sat, 04 Feb 2023 06:55:53 GMT  
		Size: 55.0 MB (55025312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:154fe4cd65e5c30dd59093bd2c5edeb1d7892246dcb092564c35adb2dcc3f87b`  
		Last Modified: Sat, 04 Feb 2023 14:04:12 GMT  
		Size: 39.5 MB (39486607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:567f91a0a4b1cd6524fda2a63dd1948bf5fc7c699b172c4e9cb5986c1e5eceb7`  
		Last Modified: Sat, 04 Feb 2023 14:04:04 GMT  
		Size: 386.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce84d71503c32a8a86b5d886948c5d7d8138945998b4c31f05bfe35af0dbcd4b`  
		Last Modified: Sat, 04 Feb 2023 14:04:04 GMT  
		Size: 1.9 KB (1875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a11b9280fafb872c844c5dbff2fc246006a97a59897561411ce2c0d3676897f3`  
		Last Modified: Sat, 04 Feb 2023 14:04:04 GMT  
		Size: 1.5 KB (1477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e15d0e23848f1f6f5daf25c58fdf76a136a6dec252c28c3c1332250ad8e81c6`  
		Last Modified: Sat, 04 Feb 2023 14:04:04 GMT  
		Size: 1.4 MB (1385162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c610542bc6221747547117c74d457e30e7fce1c9394a494b2ee945e89f6faf3a`  
		Last Modified: Sat, 04 Feb 2023 14:04:04 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4` - linux; arm variant v5

```console
$ docker pull adminer@sha256:f41d812a0a97b02f761e994e55331571cbd685a2bfdeef007e9c8d098f61a58e
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.2 MB (91188340 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:937bc7e7afadd352160727b3edded381d4f7131ad46c77906131729950141670`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Thu, 09 Feb 2023 02:00:16 GMT
ADD file:f5b31ee6dfb50a99818c1a4b3aba7c6ba1557b1547aa730e4230600017520691 in / 
# Thu, 09 Feb 2023 02:00:17 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 02:24:11 GMT
STOPSIGNAL SIGINT
# Thu, 09 Feb 2023 02:25:10 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 02:25:11 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Thu, 09 Feb 2023 02:25:12 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 09 Feb 2023 02:25:12 GMT
WORKDIR /var/www/html
# Thu, 09 Feb 2023 02:25:13 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 09 Feb 2023 02:25:13 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 09 Feb 2023 02:25:13 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 09 Feb 2023 02:25:13 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 09 Feb 2023 02:25:29 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 09 Feb 2023 02:25:29 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 09 Feb 2023 02:25:29 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 09 Feb 2023 02:25:29 GMT
USER adminer
# Thu, 09 Feb 2023 02:25:29 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Thu, 09 Feb 2023 02:25:29 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:f316396b5265978a8de9d493acdc7cda735a1fae190efbd5359650183ab7271f`  
		Last Modified: Thu, 09 Feb 2023 02:05:10 GMT  
		Size: 52.6 MB (52551796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0815a961482b87ff7ddc14fbf492d26b081ca226c383b265a39b9d900705a745`  
		Last Modified: Thu, 09 Feb 2023 02:26:40 GMT  
		Size: 37.2 MB (37247283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:907d5f9eb045277cd9fb22287b0e14b7fcd0ddcf52829c1e884706cae455c579`  
		Last Modified: Thu, 09 Feb 2023 02:26:30 GMT  
		Size: 393.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8109ea45000a26ce9c558139872c68cc18839c5d9d58b6362bad0e61335be87`  
		Last Modified: Thu, 09 Feb 2023 02:26:30 GMT  
		Size: 1.8 KB (1840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de171f42adf643e4c74d58974916e2f121db8d111d838e580c9b53bed7875d54`  
		Last Modified: Thu, 09 Feb 2023 02:26:30 GMT  
		Size: 1.5 KB (1478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d391953776d5d50c308770e750f4b1df9f2041dcec59d1ea998f85fb7e012962`  
		Last Modified: Thu, 09 Feb 2023 02:26:30 GMT  
		Size: 1.4 MB (1385055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a563edb132e3a3c8e9654277a5136351be9d1d1582967ba0ada9e4772683912`  
		Last Modified: Thu, 09 Feb 2023 02:26:30 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4` - linux; arm variant v7

```console
$ docker pull adminer@sha256:9d12f8ae49e2b1ccac684b16522c130d56646a6c56fdcead2d1dbd5be32b71ea
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.8 MB (87762862 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe294facea4e18353cea22666d19efa67a350c0803293d20d943e0c6e97467b0`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Sat, 04 Feb 2023 09:59:19 GMT
ADD file:239b5255d05e0742f381f82fb7cd586fcc6d9a427263238a2be3372c494ae933 in / 
# Sat, 04 Feb 2023 09:59:20 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 10:43:54 GMT
STOPSIGNAL SIGINT
# Sat, 04 Feb 2023 10:44:19 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 10:44:20 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Sat, 04 Feb 2023 10:44:20 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Sat, 04 Feb 2023 10:44:20 GMT
WORKDIR /var/www/html
# Sat, 04 Feb 2023 10:44:20 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Sat, 04 Feb 2023 10:44:20 GMT
ENV ADMINER_VERSION=4.8.1
# Sat, 04 Feb 2023 10:44:21 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Sat, 04 Feb 2023 10:44:21 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Sat, 04 Feb 2023 10:44:33 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 04 Feb 2023 10:44:33 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Sat, 04 Feb 2023 10:44:33 GMT
ENTRYPOINT ["entrypoint.sh"]
# Sat, 04 Feb 2023 10:44:33 GMT
USER adminer
# Sat, 04 Feb 2023 10:44:34 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Sat, 04 Feb 2023 10:44:34 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:7a21a86b3957d8c99250334cfb78c55af4f8c9277f2f1d4abd53d0362f96323d`  
		Last Modified: Sat, 04 Feb 2023 10:05:53 GMT  
		Size: 50.2 MB (50190828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f647e4e293fd395af7ac8037948dbe3388c6cb6db3064a00c9f7b5ae32ba1bd1`  
		Last Modified: Sat, 04 Feb 2023 10:45:41 GMT  
		Size: 36.2 MB (36182796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc9bd65829db2cfa0c5e7daf2f0a09bc126930cc6f916496844b3e8adeb9d8ed`  
		Last Modified: Sat, 04 Feb 2023 10:45:31 GMT  
		Size: 394.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ca053278ba99e9e29b58a59e0d4e18b6a12ae83036d127f90aeed075f61139c`  
		Last Modified: Sat, 04 Feb 2023 10:45:31 GMT  
		Size: 1.8 KB (1835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:212108f5743ed386440da376a9d15e10b2349f1a1573187b747a06ea2d32abc6`  
		Last Modified: Sat, 04 Feb 2023 10:45:31 GMT  
		Size: 1.5 KB (1477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9c4b14fe58151d7c0bc6589d5264310b8afa5674ec2f3a675e5c524a8eb12df`  
		Last Modified: Sat, 04 Feb 2023 10:45:32 GMT  
		Size: 1.4 MB (1385040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5305f0630fde46637c4b273861b8dc1fd8735642c1290f7d39e3f62c58452f35`  
		Last Modified: Sat, 04 Feb 2023 10:45:31 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4` - linux; arm64 variant v8

```console
$ docker pull adminer@sha256:4f5db61ed6cff7c4d001092c5ce6d5eb7501a356739d77657c28f6b813d428c2
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.3 MB (94313416 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f55903b78a43635b55478abb38f63cd77f3e0ec223947f72aee5c6872a07ffd1`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Sat, 04 Feb 2023 06:17:26 GMT
ADD file:c5a7c65d67685092faa3456c1a772550aa6d06ac07e1f98a95d39c31e304dbf8 in / 
# Sat, 04 Feb 2023 06:17:27 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 06:40:07 GMT
STOPSIGNAL SIGINT
# Sat, 04 Feb 2023 06:40:27 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 06:40:28 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Sat, 04 Feb 2023 06:40:29 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Sat, 04 Feb 2023 06:40:29 GMT
WORKDIR /var/www/html
# Sat, 04 Feb 2023 06:40:29 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Sat, 04 Feb 2023 06:40:29 GMT
ENV ADMINER_VERSION=4.8.1
# Sat, 04 Feb 2023 06:40:29 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Sat, 04 Feb 2023 06:40:29 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Sat, 04 Feb 2023 06:40:39 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 04 Feb 2023 06:40:39 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Sat, 04 Feb 2023 06:40:39 GMT
ENTRYPOINT ["entrypoint.sh"]
# Sat, 04 Feb 2023 06:40:40 GMT
USER adminer
# Sat, 04 Feb 2023 06:40:40 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Sat, 04 Feb 2023 06:40:40 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:fac7262b6510529638951e16807cf1758f42c892ed924e334c27bb8bbcf7d7c2`  
		Last Modified: Sat, 04 Feb 2023 06:21:01 GMT  
		Size: 53.7 MB (53681927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a3c4993b9ed6a78b02081f8b79138654baa646295eb90d0f09eb178f86f610b`  
		Last Modified: Sat, 04 Feb 2023 06:41:19 GMT  
		Size: 39.2 MB (39242179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77346147b34a65302ad6ba550d6ab4659b2d986cd2c2e57248651460e8a3e589`  
		Last Modified: Sat, 04 Feb 2023 06:41:12 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56563dd7963c36713d65f09a5387503374566d7296c2bfa4422bf2d3ceb3bbeb`  
		Last Modified: Sat, 04 Feb 2023 06:41:12 GMT  
		Size: 1.9 KB (1879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fa2e6ff1278f9c9246cfedeee571a41de27494a6f3d518f136dbb8a225d7d33`  
		Last Modified: Sat, 04 Feb 2023 06:41:12 GMT  
		Size: 1.5 KB (1481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f24f727f464d597cc5ae7abb0b697c3807940cf0cca55089c3cbc553eee16523`  
		Last Modified: Sat, 04 Feb 2023 06:41:12 GMT  
		Size: 1.4 MB (1385069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:717c6895aefe53599660cfa578fea33535395f3479fdaecb0f2db55b2fa1165a`  
		Last Modified: Sat, 04 Feb 2023 06:41:12 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4` - linux; 386

```console
$ docker pull adminer@sha256:9aeaa40748b7ce615a50ef6b58624bde25df408d8e05367d32f939a9ebac3a1d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.0 MB (96953374 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0059247fefe0e30e3270aaad4163ba4bfc56aa80f66364c27054b4f9bd7ef47`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Sat, 04 Feb 2023 07:49:07 GMT
ADD file:d610d24eb19fe7e275924d58b6dad6b9f3dce21359a4ef81d04298e94382f102 in / 
# Sat, 04 Feb 2023 07:49:07 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 08:14:35 GMT
STOPSIGNAL SIGINT
# Sat, 04 Feb 2023 08:14:57 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 08:14:58 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Sat, 04 Feb 2023 08:14:59 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Sat, 04 Feb 2023 08:14:59 GMT
WORKDIR /var/www/html
# Sat, 04 Feb 2023 08:15:01 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Sat, 04 Feb 2023 08:15:01 GMT
ENV ADMINER_VERSION=4.8.1
# Sat, 04 Feb 2023 08:15:02 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Sat, 04 Feb 2023 08:15:03 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Sat, 04 Feb 2023 08:15:16 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 04 Feb 2023 08:15:17 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Sat, 04 Feb 2023 08:15:17 GMT
ENTRYPOINT ["entrypoint.sh"]
# Sat, 04 Feb 2023 08:15:18 GMT
USER adminer
# Sat, 04 Feb 2023 08:15:19 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Sat, 04 Feb 2023 08:15:20 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:082bfbf393a7a28cd82d531b1903cc5d788ac6af1b972045ad1d0deeff1aa6ab`  
		Last Modified: Sat, 04 Feb 2023 07:54:34 GMT  
		Size: 56.0 MB (56005478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb56dd30a9439c969b4e4698f93d1d6904887b24d016964a7c0857e306cbf507`  
		Last Modified: Sat, 04 Feb 2023 08:16:26 GMT  
		Size: 39.6 MB (39558401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0895a9cfae4403af4769bb7fc2334726c0db5a6929982d11aca84a6fd3b4247`  
		Last Modified: Sat, 04 Feb 2023 08:16:17 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b8ed21414ac18410d2cd7538e45767fefbf32a8719524c47f79dbb6481c58a9`  
		Last Modified: Sat, 04 Feb 2023 08:16:17 GMT  
		Size: 1.7 KB (1718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba129a165b264b065c4c64c28d541b80a301b07360486eeaaa32fffd058c8614`  
		Last Modified: Sat, 04 Feb 2023 08:16:17 GMT  
		Size: 1.5 KB (1479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d33029a943fe1a9b73a9717bc4636749407077422d7374aa4dddc3a99a9f97a7`  
		Last Modified: Sat, 04 Feb 2023 08:16:17 GMT  
		Size: 1.4 MB (1385416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:036ba73b7268a6aed37bd51a00d8c5ffd4f4a71eb03b0aa0e8ed0a6c0123bc82`  
		Last Modified: Sat, 04 Feb 2023 08:16:17 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4` - linux; mips64le

```console
$ docker pull adminer@sha256:0566934f328c80510fdb62adfc866aeb360712e6df9b0a27474a0ad53c6148a4
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.6 MB (92610528 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fcc732f3bac92ee347514fc3ed0501efa9c7a348b4e0c1d588c77787ddf8dbe4`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Thu, 09 Feb 2023 02:44:36 GMT
ADD file:0cc085dc00beb990e7bfcdd8b37dceccb8f6d62d7c5ce2d7e736cdf4d52ab799 in / 
# Thu, 09 Feb 2023 02:44:41 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 06:13:03 GMT
STOPSIGNAL SIGINT
# Thu, 09 Feb 2023 06:14:56 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 06:15:02 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Thu, 09 Feb 2023 06:15:09 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 09 Feb 2023 06:15:12 GMT
WORKDIR /var/www/html
# Thu, 09 Feb 2023 06:15:15 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 09 Feb 2023 06:15:18 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 09 Feb 2023 06:15:22 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 09 Feb 2023 06:15:25 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 09 Feb 2023 06:16:14 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 09 Feb 2023 06:16:17 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 09 Feb 2023 06:16:20 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 09 Feb 2023 06:16:23 GMT
USER adminer
# Thu, 09 Feb 2023 06:16:26 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Thu, 09 Feb 2023 06:16:30 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:11a4758105e306ed24134ddf12f4d813426845c37a0ab14cb71de94c2858f09c`  
		Last Modified: Thu, 09 Feb 2023 02:53:05 GMT  
		Size: 53.3 MB (53266784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7daca01da5691398087a3bfc7f953540cff885f22074e0129fda0d5e578a7a64`  
		Last Modified: Thu, 09 Feb 2023 06:19:06 GMT  
		Size: 38.0 MB (37953476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53cfc05716a9d1f679b734de3bff7a1b9714f5eb4b5040d6e143defb24f4975b`  
		Last Modified: Thu, 09 Feb 2023 06:18:37 GMT  
		Size: 395.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66588c07e295fc98922360681aab4fd6a5c85ca29e0d60b27a06b53038e89c06`  
		Last Modified: Thu, 09 Feb 2023 06:18:37 GMT  
		Size: 1.7 KB (1729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6920b4dc4d4b5e73a928683693ea3ec779eb5c2100896fcc49acbb46ca85198a`  
		Last Modified: Thu, 09 Feb 2023 06:18:37 GMT  
		Size: 1.5 KB (1479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a2bb1759b592851efa52aa0ae0243e97ddaee48fec421bde7daeb618542cca8`  
		Last Modified: Thu, 09 Feb 2023 06:18:38 GMT  
		Size: 1.4 MB (1386172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1a36c2a9b981a0b8491e075725805da77790fd3eb7a7b71f664ef3c369a2e14`  
		Last Modified: Thu, 09 Feb 2023 06:18:37 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4` - linux; ppc64le

```console
$ docker pull adminer@sha256:47a4ade05e65fa4596b6163d81cd7a4fa77513df4972a34167a78b55224b98d7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.2 MB (101226739 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d968381d4dcfc992e9ec7607ed161acc52925d93157eed9ed50bbc08830df809`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Sat, 04 Feb 2023 12:25:27 GMT
ADD file:724a2ac3b6190353442c93dce0ad4b3ab5c60144fc8204131767af6760e11980 in / 
# Sat, 04 Feb 2023 12:25:30 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 17:52:28 GMT
STOPSIGNAL SIGINT
# Sat, 04 Feb 2023 17:53:25 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 17:53:28 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Sat, 04 Feb 2023 17:53:31 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Sat, 04 Feb 2023 17:53:31 GMT
WORKDIR /var/www/html
# Sat, 04 Feb 2023 17:53:32 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Sat, 04 Feb 2023 17:53:32 GMT
ENV ADMINER_VERSION=4.8.1
# Sat, 04 Feb 2023 17:53:32 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Sat, 04 Feb 2023 17:53:33 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Sat, 04 Feb 2023 17:54:00 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 04 Feb 2023 17:54:00 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Sat, 04 Feb 2023 17:54:00 GMT
ENTRYPOINT ["entrypoint.sh"]
# Sat, 04 Feb 2023 17:54:01 GMT
USER adminer
# Sat, 04 Feb 2023 17:54:01 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Sat, 04 Feb 2023 17:54:02 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:c14c296a64e0f557b40f88759a913c28d0b28c646e5ec0cf0ceb49457156a792`  
		Last Modified: Sat, 04 Feb 2023 12:31:37 GMT  
		Size: 58.9 MB (58897064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2874c2bcc11a32eb3e38ad44035b5962c96846742a4307ba2c420da009e81ea7`  
		Last Modified: Sat, 04 Feb 2023 17:55:24 GMT  
		Size: 40.9 MB (40940112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dff9f9467cf09d7f5c242cfb1cacef36591219699095992b5738c1a88620f1d1`  
		Last Modified: Sat, 04 Feb 2023 17:55:09 GMT  
		Size: 394.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5c16d0da50d675218fc2a7373e45781eb595f8a795b902bcadf6be87ec0c887`  
		Last Modified: Sat, 04 Feb 2023 17:55:09 GMT  
		Size: 1.9 KB (1879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20dcb0d7c1b30e96ea63a399103c52c4292e83ce4579f47057d8dfe4d78b0aef`  
		Last Modified: Sat, 04 Feb 2023 17:55:09 GMT  
		Size: 1.5 KB (1478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3f8d644f4416950947c0acf3f7511db8085e591667b824d91224cec02554543`  
		Last Modified: Sat, 04 Feb 2023 17:55:09 GMT  
		Size: 1.4 MB (1385321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02759dcc9c00093b87b4c7129217d0bb02701ea0aa1e86f4d8f0eaf7a56723ab`  
		Last Modified: Sat, 04 Feb 2023 17:55:09 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4` - linux; s390x

```console
$ docker pull adminer@sha256:2719e0584d03780419167688eaba32d1ee3527400ff69f7f2cdd3db286a68aa8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.7 MB (93688213 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e9613c6a60d2d28ec14e33ed1f2f4b998316d21902a342ceca374a3b98116f1`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Thu, 09 Feb 2023 02:41:26 GMT
ADD file:952595f2a554945ef740fa7b1fbc617a9ce3e1c3b90ddf1e7c0ac6018e6a98f9 in / 
# Thu, 09 Feb 2023 02:41:30 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 07:18:54 GMT
STOPSIGNAL SIGINT
# Thu, 09 Feb 2023 07:20:03 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 07:20:13 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Thu, 09 Feb 2023 07:20:15 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 09 Feb 2023 07:20:16 GMT
WORKDIR /var/www/html
# Thu, 09 Feb 2023 07:20:17 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 09 Feb 2023 07:20:18 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 09 Feb 2023 07:20:19 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 09 Feb 2023 07:20:20 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 09 Feb 2023 07:20:29 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 09 Feb 2023 07:20:29 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 09 Feb 2023 07:20:29 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 09 Feb 2023 07:20:30 GMT
USER adminer
# Thu, 09 Feb 2023 07:20:30 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Thu, 09 Feb 2023 07:20:30 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:83809ebda0c421fc95029bc6775e0a0c1eba6916a58b115dcb6a14885dae2028`  
		Last Modified: Thu, 09 Feb 2023 02:45:46 GMT  
		Size: 53.3 MB (53278896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7e31cf57a38a02fa2d3f8ff53add4d422bd4ff62ec4b24e0831c6725cee4b77`  
		Last Modified: Thu, 09 Feb 2023 07:21:24 GMT  
		Size: 39.0 MB (39019658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0633cef61215983b712e699a77b2f0a05ae8e463a4b6c07ffa63d79c6d451f3`  
		Last Modified: Thu, 09 Feb 2023 07:21:18 GMT  
		Size: 394.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:827d0eb471d78ca9b876122dfaeddf3edb023c66c6efa92c4ec68f85e999114d`  
		Last Modified: Thu, 09 Feb 2023 07:21:18 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e6233ba1bdaa0fba57704d8dc153af1171478f4f644bcd1672d9a4fd9712ccb`  
		Last Modified: Thu, 09 Feb 2023 07:21:18 GMT  
		Size: 1.5 KB (1483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5eb9aee6c3e13c08694db2a9db11c9563576952794921b2cfa054236137c34ba`  
		Last Modified: Thu, 09 Feb 2023 07:21:18 GMT  
		Size: 1.4 MB (1385406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c778394cc4cf1727666c9cc60aec4329d57cae6761ed5d514b755368d165048`  
		Last Modified: Thu, 09 Feb 2023 07:21:18 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `adminer:4-fastcgi`

```console
$ docker pull adminer@sha256:7085d390109c63834cf471af0ddb9f6285d0002d0d2ee12424f8b50088fc9db2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `adminer:4-fastcgi` - linux; amd64

```console
$ docker pull adminer@sha256:a487a7e8be03bc50ec36d32b800c2a2a32ed6a5c238faca2dd38021b93b52991
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.9 MB (95904051 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64f86f40f9d98336b024a973361cd24981a21d3aba73369f77965c23e25186cf`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Sat, 04 Feb 2023 06:51:26 GMT
ADD file:cc6a56676703ec7ab5db8f2f7bc18a3169c0816d38703845b6b77ae5342ab41c in / 
# Sat, 04 Feb 2023 06:51:27 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 14:02:55 GMT
STOPSIGNAL SIGINT
# Sat, 04 Feb 2023 14:03:16 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 14:03:17 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Sat, 04 Feb 2023 14:03:36 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Sat, 04 Feb 2023 14:03:37 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Sat, 04 Feb 2023 14:03:37 GMT
WORKDIR /var/www/html
# Sat, 04 Feb 2023 14:03:37 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Sat, 04 Feb 2023 14:03:37 GMT
ENV ADMINER_VERSION=4.8.1
# Sat, 04 Feb 2023 14:03:37 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Sat, 04 Feb 2023 14:03:37 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Sat, 04 Feb 2023 14:03:48 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 04 Feb 2023 14:03:48 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Sat, 04 Feb 2023 14:03:49 GMT
ENTRYPOINT ["entrypoint.sh"]
# Sat, 04 Feb 2023 14:03:49 GMT
USER adminer
# Sat, 04 Feb 2023 14:03:49 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:699c8a97647f5789e5850bcf1a3d5afe9730edb654e1ae0714d5bd198a67a3ed`  
		Last Modified: Sat, 04 Feb 2023 06:55:53 GMT  
		Size: 55.0 MB (55025312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:154fe4cd65e5c30dd59093bd2c5edeb1d7892246dcb092564c35adb2dcc3f87b`  
		Last Modified: Sat, 04 Feb 2023 14:04:12 GMT  
		Size: 39.5 MB (39486607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:567f91a0a4b1cd6524fda2a63dd1948bf5fc7c699b172c4e9cb5986c1e5eceb7`  
		Last Modified: Sat, 04 Feb 2023 14:04:04 GMT  
		Size: 386.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43e065a08a3a44ef53db81a6b0ab94330ab02fd8a0d5c02758e2a9ccba2db806`  
		Last Modified: Sat, 04 Feb 2023 14:04:31 GMT  
		Size: 2.7 KB (2707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0154f5a2a5df6dc3e259a0da06081c740b1cc6974b3c6d2a763c82f68342132e`  
		Last Modified: Sat, 04 Feb 2023 14:04:31 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4af9bb043e0acb2d1b281a5d3f020e2437196040d7a09afda443537a7e3f3c40`  
		Last Modified: Sat, 04 Feb 2023 14:04:31 GMT  
		Size: 1.5 KB (1477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc585851cc1446d5ca0866b33d000cee9fcdac28a4c9d92bd803915ff149b87a`  
		Last Modified: Sat, 04 Feb 2023 14:04:31 GMT  
		Size: 1.4 MB (1385188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:345df3ed0a37be7be2ffe6d6abae3125fbfeb1a8624a4942368abf7585f2657a`  
		Last Modified: Sat, 04 Feb 2023 14:04:31 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-fastcgi` - linux; arm variant v5

```console
$ docker pull adminer@sha256:326ae96ad868945cc6ce21ae1125608876936e0a60b14764f309118e60ef3f11
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.2 MB (91191039 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12511271c61962718849cd85d462dfe90b30f31ec29c7600b97a3d1da83e8b1d`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Thu, 09 Feb 2023 02:00:16 GMT
ADD file:f5b31ee6dfb50a99818c1a4b3aba7c6ba1557b1547aa730e4230600017520691 in / 
# Thu, 09 Feb 2023 02:00:17 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 02:24:11 GMT
STOPSIGNAL SIGINT
# Thu, 09 Feb 2023 02:25:10 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 02:25:11 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Thu, 09 Feb 2023 02:25:39 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Thu, 09 Feb 2023 02:25:39 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 09 Feb 2023 02:25:40 GMT
WORKDIR /var/www/html
# Thu, 09 Feb 2023 02:25:40 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 09 Feb 2023 02:25:40 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 09 Feb 2023 02:25:40 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 09 Feb 2023 02:25:40 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 09 Feb 2023 02:25:56 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 09 Feb 2023 02:25:57 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 09 Feb 2023 02:25:57 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 09 Feb 2023 02:25:57 GMT
USER adminer
# Thu, 09 Feb 2023 02:25:57 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:f316396b5265978a8de9d493acdc7cda735a1fae190efbd5359650183ab7271f`  
		Last Modified: Thu, 09 Feb 2023 02:05:10 GMT  
		Size: 52.6 MB (52551796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0815a961482b87ff7ddc14fbf492d26b081ca226c383b265a39b9d900705a745`  
		Last Modified: Thu, 09 Feb 2023 02:26:40 GMT  
		Size: 37.2 MB (37247283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:907d5f9eb045277cd9fb22287b0e14b7fcd0ddcf52829c1e884706cae455c579`  
		Last Modified: Thu, 09 Feb 2023 02:26:30 GMT  
		Size: 393.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a3fe13d432c7dc589c9f54a560146f1249dfb75cf8f7169dfce8ac53c037021`  
		Last Modified: Thu, 09 Feb 2023 02:27:04 GMT  
		Size: 2.7 KB (2711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c23eca33f0e2498aefa42e88bcc0e47b715bdd1aae38f94434fb4ea6bdc0795e`  
		Last Modified: Thu, 09 Feb 2023 02:27:04 GMT  
		Size: 1.8 KB (1840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05f6bb9d806bbc982ab481b1906091f08c8ada35a23423c887544b3f135ac66f`  
		Last Modified: Thu, 09 Feb 2023 02:27:04 GMT  
		Size: 1.5 KB (1480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1c811cb2797199efbeb3147f223e01f6c28cee6d87b39a36fe8eb5347b987cd`  
		Last Modified: Thu, 09 Feb 2023 02:27:05 GMT  
		Size: 1.4 MB (1385045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6475dd585587079dec552c0910151d39ef0972f2f7ac63073ae5b67064c15ba3`  
		Last Modified: Thu, 09 Feb 2023 02:27:04 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-fastcgi` - linux; arm variant v7

```console
$ docker pull adminer@sha256:1745d08452780cad59501ee3c384e5cae58ab9f36b395347e4470f47f02f24ed
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.8 MB (87765580 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:004424ead9c2af6485083598520693d3cdc5f59da6283b4ccfc7424319280fc3`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Sat, 04 Feb 2023 09:59:19 GMT
ADD file:239b5255d05e0742f381f82fb7cd586fcc6d9a427263238a2be3372c494ae933 in / 
# Sat, 04 Feb 2023 09:59:20 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 10:43:54 GMT
STOPSIGNAL SIGINT
# Sat, 04 Feb 2023 10:44:19 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 10:44:20 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Sat, 04 Feb 2023 10:44:47 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Sat, 04 Feb 2023 10:44:47 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Sat, 04 Feb 2023 10:44:47 GMT
WORKDIR /var/www/html
# Sat, 04 Feb 2023 10:44:48 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Sat, 04 Feb 2023 10:44:48 GMT
ENV ADMINER_VERSION=4.8.1
# Sat, 04 Feb 2023 10:44:48 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Sat, 04 Feb 2023 10:44:48 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Sat, 04 Feb 2023 10:45:00 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 04 Feb 2023 10:45:00 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Sat, 04 Feb 2023 10:45:00 GMT
ENTRYPOINT ["entrypoint.sh"]
# Sat, 04 Feb 2023 10:45:01 GMT
USER adminer
# Sat, 04 Feb 2023 10:45:01 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:7a21a86b3957d8c99250334cfb78c55af4f8c9277f2f1d4abd53d0362f96323d`  
		Last Modified: Sat, 04 Feb 2023 10:05:53 GMT  
		Size: 50.2 MB (50190828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f647e4e293fd395af7ac8037948dbe3388c6cb6db3064a00c9f7b5ae32ba1bd1`  
		Last Modified: Sat, 04 Feb 2023 10:45:41 GMT  
		Size: 36.2 MB (36182796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc9bd65829db2cfa0c5e7daf2f0a09bc126930cc6f916496844b3e8adeb9d8ed`  
		Last Modified: Sat, 04 Feb 2023 10:45:31 GMT  
		Size: 394.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcec0a137102a4df6e8f3bae77f95cb2d0288be8d86aa062191a0994da6a09a1`  
		Last Modified: Sat, 04 Feb 2023 10:46:04 GMT  
		Size: 2.7 KB (2710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9366bc96b1ef426445bd576c64c5638c631fd82aeb0453f3871a82d91ecd0df1`  
		Last Modified: Sat, 04 Feb 2023 10:46:04 GMT  
		Size: 1.8 KB (1836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:459144f5a86bfff13a40970a73b497f8392eccdd9238e210b72ed37ace1dd2c8`  
		Last Modified: Sat, 04 Feb 2023 10:46:04 GMT  
		Size: 1.5 KB (1481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3a153a1f8dd4081e72343761ee75a8397e7809582b6a8d42a491dbc499b8719`  
		Last Modified: Sat, 04 Feb 2023 10:46:05 GMT  
		Size: 1.4 MB (1385045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc9fe3e24aab98148380a5d410c285619711932dcdcbe7cca25ee0aae77b4cb3`  
		Last Modified: Sat, 04 Feb 2023 10:46:04 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-fastcgi` - linux; arm64 variant v8

```console
$ docker pull adminer@sha256:14e5c9e9653cd354401e9d672d76e6462430024848ee435c02d0ff4332126317
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.3 MB (94316110 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0fa0825c1e857cf1eab6178105270bd008b049eb53696b1d94ed671c6284c846`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Sat, 04 Feb 2023 06:17:26 GMT
ADD file:c5a7c65d67685092faa3456c1a772550aa6d06ac07e1f98a95d39c31e304dbf8 in / 
# Sat, 04 Feb 2023 06:17:27 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 06:40:07 GMT
STOPSIGNAL SIGINT
# Sat, 04 Feb 2023 06:40:27 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 06:40:28 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Sat, 04 Feb 2023 06:40:47 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Sat, 04 Feb 2023 06:40:48 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Sat, 04 Feb 2023 06:40:48 GMT
WORKDIR /var/www/html
# Sat, 04 Feb 2023 06:40:48 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Sat, 04 Feb 2023 06:40:48 GMT
ENV ADMINER_VERSION=4.8.1
# Sat, 04 Feb 2023 06:40:48 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Sat, 04 Feb 2023 06:40:48 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Sat, 04 Feb 2023 06:40:57 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 04 Feb 2023 06:40:57 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Sat, 04 Feb 2023 06:40:58 GMT
ENTRYPOINT ["entrypoint.sh"]
# Sat, 04 Feb 2023 06:40:58 GMT
USER adminer
# Sat, 04 Feb 2023 06:40:58 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:fac7262b6510529638951e16807cf1758f42c892ed924e334c27bb8bbcf7d7c2`  
		Last Modified: Sat, 04 Feb 2023 06:21:01 GMT  
		Size: 53.7 MB (53681927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a3c4993b9ed6a78b02081f8b79138654baa646295eb90d0f09eb178f86f610b`  
		Last Modified: Sat, 04 Feb 2023 06:41:19 GMT  
		Size: 39.2 MB (39242179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77346147b34a65302ad6ba550d6ab4659b2d986cd2c2e57248651460e8a3e589`  
		Last Modified: Sat, 04 Feb 2023 06:41:12 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d66723d85a15a95d2bc016413f1fb69ae885d83e587a97d2043d370cf67e2db1`  
		Last Modified: Sat, 04 Feb 2023 06:41:36 GMT  
		Size: 2.7 KB (2707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7d226beb0ae597acd7e2647b0f4d4fc5227c69df6dff1165b4fe514cfad8130`  
		Last Modified: Sat, 04 Feb 2023 06:41:36 GMT  
		Size: 1.9 KB (1878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:def3ff5795d638c86eb1ce6b33aa5b7ac1991a913a5795be71a67c8f0bc1eab6`  
		Last Modified: Sat, 04 Feb 2023 06:41:36 GMT  
		Size: 1.5 KB (1476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:277a8bd87f658c231dabf9f7c494772cd03abace79d86737b913b73e89ee7bac`  
		Last Modified: Sat, 04 Feb 2023 06:41:37 GMT  
		Size: 1.4 MB (1385063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e95c557117dcc88c76c221f757a0f3404ad012a7726a260eadd4aba9b4e3341`  
		Last Modified: Sat, 04 Feb 2023 06:41:37 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-fastcgi` - linux; 386

```console
$ docker pull adminer@sha256:b0a3d3e0b21c7f00206ed8268c4dd0c6f085e410f729fb795bb885f8cac1098f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.0 MB (96956091 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9fa3646b337edc6af84c9cd6a950e859eaf4183842f124b5742da2f3495e257`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Sat, 04 Feb 2023 07:49:07 GMT
ADD file:d610d24eb19fe7e275924d58b6dad6b9f3dce21359a4ef81d04298e94382f102 in / 
# Sat, 04 Feb 2023 07:49:07 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 08:14:35 GMT
STOPSIGNAL SIGINT
# Sat, 04 Feb 2023 08:14:57 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 08:14:58 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Sat, 04 Feb 2023 08:15:27 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Sat, 04 Feb 2023 08:15:28 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Sat, 04 Feb 2023 08:15:29 GMT
WORKDIR /var/www/html
# Sat, 04 Feb 2023 08:15:31 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Sat, 04 Feb 2023 08:15:31 GMT
ENV ADMINER_VERSION=4.8.1
# Sat, 04 Feb 2023 08:15:32 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Sat, 04 Feb 2023 08:15:33 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Sat, 04 Feb 2023 08:15:45 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 04 Feb 2023 08:15:47 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Sat, 04 Feb 2023 08:15:47 GMT
ENTRYPOINT ["entrypoint.sh"]
# Sat, 04 Feb 2023 08:15:48 GMT
USER adminer
# Sat, 04 Feb 2023 08:15:49 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:082bfbf393a7a28cd82d531b1903cc5d788ac6af1b972045ad1d0deeff1aa6ab`  
		Last Modified: Sat, 04 Feb 2023 07:54:34 GMT  
		Size: 56.0 MB (56005478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb56dd30a9439c969b4e4698f93d1d6904887b24d016964a7c0857e306cbf507`  
		Last Modified: Sat, 04 Feb 2023 08:16:26 GMT  
		Size: 39.6 MB (39558401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0895a9cfae4403af4769bb7fc2334726c0db5a6929982d11aca84a6fd3b4247`  
		Last Modified: Sat, 04 Feb 2023 08:16:17 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fb386372d050d61199d8b69f8eba0503204b1435c14765dcc7391690f40e104`  
		Last Modified: Sat, 04 Feb 2023 08:16:47 GMT  
		Size: 2.7 KB (2709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92775617fc6814142b985df263b604974edc157e129229cd23234c9ea1e661e6`  
		Last Modified: Sat, 04 Feb 2023 08:16:47 GMT  
		Size: 1.7 KB (1714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f95cd3c9ca70db181013ee630ed1999515d90622129ffa1cffcb8610f0f456f7`  
		Last Modified: Sat, 04 Feb 2023 08:16:48 GMT  
		Size: 1.5 KB (1480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fe214dd6c4ba9b73bd44278fa41542b21e1144c6ff3ac53e197896801e87d48`  
		Last Modified: Sat, 04 Feb 2023 08:16:48 GMT  
		Size: 1.4 MB (1385428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:469bbb9c9519bc4c9fbd635879319fa1b6f74e4a9f271572fb23cbc31bcd739c`  
		Last Modified: Sat, 04 Feb 2023 08:16:47 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-fastcgi` - linux; mips64le

```console
$ docker pull adminer@sha256:d49eaa95df7a4b3b648e490d31d318b52533773169fecbc5a057d0012ea43a55
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.6 MB (92613258 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5cbd3305cd6fd59e4170383251a3e22ee9ca9c66bae9ba0b1914c9ffae1b23f6`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Thu, 09 Feb 2023 02:44:36 GMT
ADD file:0cc085dc00beb990e7bfcdd8b37dceccb8f6d62d7c5ce2d7e736cdf4d52ab799 in / 
# Thu, 09 Feb 2023 02:44:41 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 06:13:03 GMT
STOPSIGNAL SIGINT
# Thu, 09 Feb 2023 06:14:56 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 06:15:02 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Thu, 09 Feb 2023 06:16:50 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Thu, 09 Feb 2023 06:16:56 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 09 Feb 2023 06:16:59 GMT
WORKDIR /var/www/html
# Thu, 09 Feb 2023 06:17:02 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 09 Feb 2023 06:17:05 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 09 Feb 2023 06:17:08 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 09 Feb 2023 06:17:11 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 09 Feb 2023 06:17:59 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 09 Feb 2023 06:18:02 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 09 Feb 2023 06:18:05 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 09 Feb 2023 06:18:09 GMT
USER adminer
# Thu, 09 Feb 2023 06:18:12 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:11a4758105e306ed24134ddf12f4d813426845c37a0ab14cb71de94c2858f09c`  
		Last Modified: Thu, 09 Feb 2023 02:53:05 GMT  
		Size: 53.3 MB (53266784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7daca01da5691398087a3bfc7f953540cff885f22074e0129fda0d5e578a7a64`  
		Last Modified: Thu, 09 Feb 2023 06:19:06 GMT  
		Size: 38.0 MB (37953476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53cfc05716a9d1f679b734de3bff7a1b9714f5eb4b5040d6e143defb24f4975b`  
		Last Modified: Thu, 09 Feb 2023 06:18:37 GMT  
		Size: 395.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6df2d2de23d5a64cae787901af3f38fcaf86ab721824c7226d9bb8586ddba9fa`  
		Last Modified: Thu, 09 Feb 2023 06:19:25 GMT  
		Size: 2.7 KB (2714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f7734475a7c59ac576ed3322ac3274c2a727bb9a6c660381c515c9bf8ded7c0`  
		Last Modified: Thu, 09 Feb 2023 06:19:25 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b439c2c16da41627079e7dc7e3e2618e41b7ac3019f33d234ac6a50e1271e8c`  
		Last Modified: Thu, 09 Feb 2023 06:19:25 GMT  
		Size: 1.5 KB (1481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de57b503c9c79ca9d98a1575e8b2a2fec4f4f34a8184502f8a1697d783873671`  
		Last Modified: Thu, 09 Feb 2023 06:19:26 GMT  
		Size: 1.4 MB (1386183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27aac5c4950f7dd7352e76a2718d3c9d2974ba7ea1b383509d9a235534ccf422`  
		Last Modified: Thu, 09 Feb 2023 06:19:25 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-fastcgi` - linux; ppc64le

```console
$ docker pull adminer@sha256:4cbfd32fc3e0995849078137f63ac73353137c150f2af36869c97efcfd354baf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.2 MB (101229475 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6003343fd4014a739aa486639e78adf252f5a00a89aada720a7d97a43b19b920`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Sat, 04 Feb 2023 12:25:27 GMT
ADD file:724a2ac3b6190353442c93dce0ad4b3ab5c60144fc8204131767af6760e11980 in / 
# Sat, 04 Feb 2023 12:25:30 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 17:52:28 GMT
STOPSIGNAL SIGINT
# Sat, 04 Feb 2023 17:53:25 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 17:53:28 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Sat, 04 Feb 2023 17:54:10 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Sat, 04 Feb 2023 17:54:12 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Sat, 04 Feb 2023 17:54:12 GMT
WORKDIR /var/www/html
# Sat, 04 Feb 2023 17:54:13 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Sat, 04 Feb 2023 17:54:13 GMT
ENV ADMINER_VERSION=4.8.1
# Sat, 04 Feb 2023 17:54:14 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Sat, 04 Feb 2023 17:54:14 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Sat, 04 Feb 2023 17:54:37 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 04 Feb 2023 17:54:38 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Sat, 04 Feb 2023 17:54:38 GMT
ENTRYPOINT ["entrypoint.sh"]
# Sat, 04 Feb 2023 17:54:39 GMT
USER adminer
# Sat, 04 Feb 2023 17:54:39 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:c14c296a64e0f557b40f88759a913c28d0b28c646e5ec0cf0ceb49457156a792`  
		Last Modified: Sat, 04 Feb 2023 12:31:37 GMT  
		Size: 58.9 MB (58897064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2874c2bcc11a32eb3e38ad44035b5962c96846742a4307ba2c420da009e81ea7`  
		Last Modified: Sat, 04 Feb 2023 17:55:24 GMT  
		Size: 40.9 MB (40940112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dff9f9467cf09d7f5c242cfb1cacef36591219699095992b5738c1a88620f1d1`  
		Last Modified: Sat, 04 Feb 2023 17:55:09 GMT  
		Size: 394.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:268a861c77efb05e4765d3315e40b2b4a6eacb3bb56a931f6c7e4ac1b5d7a265`  
		Last Modified: Sat, 04 Feb 2023 17:55:49 GMT  
		Size: 2.7 KB (2713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d71f60a34a72995c8870893c023406f4337b9a7f557f7bd26fcd612bee6cce28`  
		Last Modified: Sat, 04 Feb 2023 17:55:49 GMT  
		Size: 1.9 KB (1875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d8ca4564d1e76d1b90184e8ab33c27849b4edd5735ea578f8c79dd312d99bfe`  
		Last Modified: Sat, 04 Feb 2023 17:55:49 GMT  
		Size: 1.5 KB (1479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f53ee83c5e9a3c93576c0b61fabdb84f2dbcb11a7a34d0f80a557d128e40db47`  
		Last Modified: Sat, 04 Feb 2023 17:55:50 GMT  
		Size: 1.4 MB (1385349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75395692fa85a6f6cd605c59de5987ad5629d3f4557722b950098cf11ff887ef`  
		Last Modified: Sat, 04 Feb 2023 17:55:49 GMT  
		Size: 489.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-fastcgi` - linux; s390x

```console
$ docker pull adminer@sha256:18930d5a14bb6b0eed4846e2b4a90aa9c731d4bde1eaf1abd60b51fe04453482
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.7 MB (93690838 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70050059db8c471d2394648f649f412ef6339c12ef4d0eeda7baa78c8bda768d`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Thu, 09 Feb 2023 02:41:26 GMT
ADD file:952595f2a554945ef740fa7b1fbc617a9ce3e1c3b90ddf1e7c0ac6018e6a98f9 in / 
# Thu, 09 Feb 2023 02:41:30 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 07:18:54 GMT
STOPSIGNAL SIGINT
# Thu, 09 Feb 2023 07:20:03 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 07:20:13 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Thu, 09 Feb 2023 07:20:43 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Thu, 09 Feb 2023 07:20:43 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 09 Feb 2023 07:20:43 GMT
WORKDIR /var/www/html
# Thu, 09 Feb 2023 07:20:44 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 09 Feb 2023 07:20:44 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 09 Feb 2023 07:20:44 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 09 Feb 2023 07:20:44 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 09 Feb 2023 07:20:52 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 09 Feb 2023 07:20:52 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 09 Feb 2023 07:20:52 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 09 Feb 2023 07:20:52 GMT
USER adminer
# Thu, 09 Feb 2023 07:20:52 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:83809ebda0c421fc95029bc6775e0a0c1eba6916a58b115dcb6a14885dae2028`  
		Last Modified: Thu, 09 Feb 2023 02:45:46 GMT  
		Size: 53.3 MB (53278896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7e31cf57a38a02fa2d3f8ff53add4d422bd4ff62ec4b24e0831c6725cee4b77`  
		Last Modified: Thu, 09 Feb 2023 07:21:24 GMT  
		Size: 39.0 MB (39019658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0633cef61215983b712e699a77b2f0a05ae8e463a4b6c07ffa63d79c6d451f3`  
		Last Modified: Thu, 09 Feb 2023 07:21:18 GMT  
		Size: 394.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c646918dad5e786008b8b31bc7f8cac9feb3521e1d4fbf6ba3c37c97bca49c6`  
		Last Modified: Thu, 09 Feb 2023 07:21:40 GMT  
		Size: 2.7 KB (2713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7c07b11a4865d90a2153a6c3e2e55161be6e83d2506f65db1ea5772aebd7219`  
		Last Modified: Thu, 09 Feb 2023 07:21:40 GMT  
		Size: 1.9 KB (1883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e13620c00e8614858376f34b19455eec2ec9325ff8082ea4407d7d72c6a4d268`  
		Last Modified: Thu, 09 Feb 2023 07:21:40 GMT  
		Size: 1.5 KB (1480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8900c81dcea2d296a964de4c28bca524bf07456b72f0cf57f0f50936cb7cf920`  
		Last Modified: Thu, 09 Feb 2023 07:21:40 GMT  
		Size: 1.4 MB (1385322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6632f7644ccabb5e6050f96cc7957a22e0bf86f0e5eff036f2a33254d3b34db`  
		Last Modified: Thu, 09 Feb 2023 07:21:40 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `adminer:4-standalone`

```console
$ docker pull adminer@sha256:d4a361f0fdbc2f8a4732a62635e043e7a883e3785a54d54f5eb0d9ce3ad80204
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `adminer:4-standalone` - linux; amd64

```console
$ docker pull adminer@sha256:8991350a6cc5acd8a607828617ad1cbd062b38528e6889664e0030b43f45d5f8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.9 MB (95901310 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:471e5d2fb746396a521960c56f7eafb8490e52be8cb499d4c0e00904c673be4e`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Sat, 04 Feb 2023 06:51:26 GMT
ADD file:cc6a56676703ec7ab5db8f2f7bc18a3169c0816d38703845b6b77ae5342ab41c in / 
# Sat, 04 Feb 2023 06:51:27 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 14:02:55 GMT
STOPSIGNAL SIGINT
# Sat, 04 Feb 2023 14:03:16 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 14:03:17 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Sat, 04 Feb 2023 14:03:17 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Sat, 04 Feb 2023 14:03:17 GMT
WORKDIR /var/www/html
# Sat, 04 Feb 2023 14:03:18 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Sat, 04 Feb 2023 14:03:18 GMT
ENV ADMINER_VERSION=4.8.1
# Sat, 04 Feb 2023 14:03:18 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Sat, 04 Feb 2023 14:03:18 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Sat, 04 Feb 2023 14:03:30 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 04 Feb 2023 14:03:30 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Sat, 04 Feb 2023 14:03:30 GMT
ENTRYPOINT ["entrypoint.sh"]
# Sat, 04 Feb 2023 14:03:30 GMT
USER adminer
# Sat, 04 Feb 2023 14:03:30 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Sat, 04 Feb 2023 14:03:30 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:699c8a97647f5789e5850bcf1a3d5afe9730edb654e1ae0714d5bd198a67a3ed`  
		Last Modified: Sat, 04 Feb 2023 06:55:53 GMT  
		Size: 55.0 MB (55025312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:154fe4cd65e5c30dd59093bd2c5edeb1d7892246dcb092564c35adb2dcc3f87b`  
		Last Modified: Sat, 04 Feb 2023 14:04:12 GMT  
		Size: 39.5 MB (39486607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:567f91a0a4b1cd6524fda2a63dd1948bf5fc7c699b172c4e9cb5986c1e5eceb7`  
		Last Modified: Sat, 04 Feb 2023 14:04:04 GMT  
		Size: 386.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce84d71503c32a8a86b5d886948c5d7d8138945998b4c31f05bfe35af0dbcd4b`  
		Last Modified: Sat, 04 Feb 2023 14:04:04 GMT  
		Size: 1.9 KB (1875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a11b9280fafb872c844c5dbff2fc246006a97a59897561411ce2c0d3676897f3`  
		Last Modified: Sat, 04 Feb 2023 14:04:04 GMT  
		Size: 1.5 KB (1477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e15d0e23848f1f6f5daf25c58fdf76a136a6dec252c28c3c1332250ad8e81c6`  
		Last Modified: Sat, 04 Feb 2023 14:04:04 GMT  
		Size: 1.4 MB (1385162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c610542bc6221747547117c74d457e30e7fce1c9394a494b2ee945e89f6faf3a`  
		Last Modified: Sat, 04 Feb 2023 14:04:04 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-standalone` - linux; arm variant v5

```console
$ docker pull adminer@sha256:f41d812a0a97b02f761e994e55331571cbd685a2bfdeef007e9c8d098f61a58e
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.2 MB (91188340 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:937bc7e7afadd352160727b3edded381d4f7131ad46c77906131729950141670`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Thu, 09 Feb 2023 02:00:16 GMT
ADD file:f5b31ee6dfb50a99818c1a4b3aba7c6ba1557b1547aa730e4230600017520691 in / 
# Thu, 09 Feb 2023 02:00:17 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 02:24:11 GMT
STOPSIGNAL SIGINT
# Thu, 09 Feb 2023 02:25:10 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 02:25:11 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Thu, 09 Feb 2023 02:25:12 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 09 Feb 2023 02:25:12 GMT
WORKDIR /var/www/html
# Thu, 09 Feb 2023 02:25:13 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 09 Feb 2023 02:25:13 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 09 Feb 2023 02:25:13 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 09 Feb 2023 02:25:13 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 09 Feb 2023 02:25:29 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 09 Feb 2023 02:25:29 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 09 Feb 2023 02:25:29 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 09 Feb 2023 02:25:29 GMT
USER adminer
# Thu, 09 Feb 2023 02:25:29 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Thu, 09 Feb 2023 02:25:29 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:f316396b5265978a8de9d493acdc7cda735a1fae190efbd5359650183ab7271f`  
		Last Modified: Thu, 09 Feb 2023 02:05:10 GMT  
		Size: 52.6 MB (52551796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0815a961482b87ff7ddc14fbf492d26b081ca226c383b265a39b9d900705a745`  
		Last Modified: Thu, 09 Feb 2023 02:26:40 GMT  
		Size: 37.2 MB (37247283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:907d5f9eb045277cd9fb22287b0e14b7fcd0ddcf52829c1e884706cae455c579`  
		Last Modified: Thu, 09 Feb 2023 02:26:30 GMT  
		Size: 393.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8109ea45000a26ce9c558139872c68cc18839c5d9d58b6362bad0e61335be87`  
		Last Modified: Thu, 09 Feb 2023 02:26:30 GMT  
		Size: 1.8 KB (1840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de171f42adf643e4c74d58974916e2f121db8d111d838e580c9b53bed7875d54`  
		Last Modified: Thu, 09 Feb 2023 02:26:30 GMT  
		Size: 1.5 KB (1478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d391953776d5d50c308770e750f4b1df9f2041dcec59d1ea998f85fb7e012962`  
		Last Modified: Thu, 09 Feb 2023 02:26:30 GMT  
		Size: 1.4 MB (1385055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a563edb132e3a3c8e9654277a5136351be9d1d1582967ba0ada9e4772683912`  
		Last Modified: Thu, 09 Feb 2023 02:26:30 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-standalone` - linux; arm variant v7

```console
$ docker pull adminer@sha256:9d12f8ae49e2b1ccac684b16522c130d56646a6c56fdcead2d1dbd5be32b71ea
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.8 MB (87762862 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe294facea4e18353cea22666d19efa67a350c0803293d20d943e0c6e97467b0`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Sat, 04 Feb 2023 09:59:19 GMT
ADD file:239b5255d05e0742f381f82fb7cd586fcc6d9a427263238a2be3372c494ae933 in / 
# Sat, 04 Feb 2023 09:59:20 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 10:43:54 GMT
STOPSIGNAL SIGINT
# Sat, 04 Feb 2023 10:44:19 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 10:44:20 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Sat, 04 Feb 2023 10:44:20 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Sat, 04 Feb 2023 10:44:20 GMT
WORKDIR /var/www/html
# Sat, 04 Feb 2023 10:44:20 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Sat, 04 Feb 2023 10:44:20 GMT
ENV ADMINER_VERSION=4.8.1
# Sat, 04 Feb 2023 10:44:21 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Sat, 04 Feb 2023 10:44:21 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Sat, 04 Feb 2023 10:44:33 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 04 Feb 2023 10:44:33 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Sat, 04 Feb 2023 10:44:33 GMT
ENTRYPOINT ["entrypoint.sh"]
# Sat, 04 Feb 2023 10:44:33 GMT
USER adminer
# Sat, 04 Feb 2023 10:44:34 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Sat, 04 Feb 2023 10:44:34 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:7a21a86b3957d8c99250334cfb78c55af4f8c9277f2f1d4abd53d0362f96323d`  
		Last Modified: Sat, 04 Feb 2023 10:05:53 GMT  
		Size: 50.2 MB (50190828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f647e4e293fd395af7ac8037948dbe3388c6cb6db3064a00c9f7b5ae32ba1bd1`  
		Last Modified: Sat, 04 Feb 2023 10:45:41 GMT  
		Size: 36.2 MB (36182796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc9bd65829db2cfa0c5e7daf2f0a09bc126930cc6f916496844b3e8adeb9d8ed`  
		Last Modified: Sat, 04 Feb 2023 10:45:31 GMT  
		Size: 394.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ca053278ba99e9e29b58a59e0d4e18b6a12ae83036d127f90aeed075f61139c`  
		Last Modified: Sat, 04 Feb 2023 10:45:31 GMT  
		Size: 1.8 KB (1835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:212108f5743ed386440da376a9d15e10b2349f1a1573187b747a06ea2d32abc6`  
		Last Modified: Sat, 04 Feb 2023 10:45:31 GMT  
		Size: 1.5 KB (1477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9c4b14fe58151d7c0bc6589d5264310b8afa5674ec2f3a675e5c524a8eb12df`  
		Last Modified: Sat, 04 Feb 2023 10:45:32 GMT  
		Size: 1.4 MB (1385040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5305f0630fde46637c4b273861b8dc1fd8735642c1290f7d39e3f62c58452f35`  
		Last Modified: Sat, 04 Feb 2023 10:45:31 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-standalone` - linux; arm64 variant v8

```console
$ docker pull adminer@sha256:4f5db61ed6cff7c4d001092c5ce6d5eb7501a356739d77657c28f6b813d428c2
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.3 MB (94313416 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f55903b78a43635b55478abb38f63cd77f3e0ec223947f72aee5c6872a07ffd1`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Sat, 04 Feb 2023 06:17:26 GMT
ADD file:c5a7c65d67685092faa3456c1a772550aa6d06ac07e1f98a95d39c31e304dbf8 in / 
# Sat, 04 Feb 2023 06:17:27 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 06:40:07 GMT
STOPSIGNAL SIGINT
# Sat, 04 Feb 2023 06:40:27 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 06:40:28 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Sat, 04 Feb 2023 06:40:29 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Sat, 04 Feb 2023 06:40:29 GMT
WORKDIR /var/www/html
# Sat, 04 Feb 2023 06:40:29 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Sat, 04 Feb 2023 06:40:29 GMT
ENV ADMINER_VERSION=4.8.1
# Sat, 04 Feb 2023 06:40:29 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Sat, 04 Feb 2023 06:40:29 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Sat, 04 Feb 2023 06:40:39 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 04 Feb 2023 06:40:39 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Sat, 04 Feb 2023 06:40:39 GMT
ENTRYPOINT ["entrypoint.sh"]
# Sat, 04 Feb 2023 06:40:40 GMT
USER adminer
# Sat, 04 Feb 2023 06:40:40 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Sat, 04 Feb 2023 06:40:40 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:fac7262b6510529638951e16807cf1758f42c892ed924e334c27bb8bbcf7d7c2`  
		Last Modified: Sat, 04 Feb 2023 06:21:01 GMT  
		Size: 53.7 MB (53681927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a3c4993b9ed6a78b02081f8b79138654baa646295eb90d0f09eb178f86f610b`  
		Last Modified: Sat, 04 Feb 2023 06:41:19 GMT  
		Size: 39.2 MB (39242179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77346147b34a65302ad6ba550d6ab4659b2d986cd2c2e57248651460e8a3e589`  
		Last Modified: Sat, 04 Feb 2023 06:41:12 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56563dd7963c36713d65f09a5387503374566d7296c2bfa4422bf2d3ceb3bbeb`  
		Last Modified: Sat, 04 Feb 2023 06:41:12 GMT  
		Size: 1.9 KB (1879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fa2e6ff1278f9c9246cfedeee571a41de27494a6f3d518f136dbb8a225d7d33`  
		Last Modified: Sat, 04 Feb 2023 06:41:12 GMT  
		Size: 1.5 KB (1481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f24f727f464d597cc5ae7abb0b697c3807940cf0cca55089c3cbc553eee16523`  
		Last Modified: Sat, 04 Feb 2023 06:41:12 GMT  
		Size: 1.4 MB (1385069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:717c6895aefe53599660cfa578fea33535395f3479fdaecb0f2db55b2fa1165a`  
		Last Modified: Sat, 04 Feb 2023 06:41:12 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-standalone` - linux; 386

```console
$ docker pull adminer@sha256:9aeaa40748b7ce615a50ef6b58624bde25df408d8e05367d32f939a9ebac3a1d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.0 MB (96953374 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0059247fefe0e30e3270aaad4163ba4bfc56aa80f66364c27054b4f9bd7ef47`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Sat, 04 Feb 2023 07:49:07 GMT
ADD file:d610d24eb19fe7e275924d58b6dad6b9f3dce21359a4ef81d04298e94382f102 in / 
# Sat, 04 Feb 2023 07:49:07 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 08:14:35 GMT
STOPSIGNAL SIGINT
# Sat, 04 Feb 2023 08:14:57 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 08:14:58 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Sat, 04 Feb 2023 08:14:59 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Sat, 04 Feb 2023 08:14:59 GMT
WORKDIR /var/www/html
# Sat, 04 Feb 2023 08:15:01 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Sat, 04 Feb 2023 08:15:01 GMT
ENV ADMINER_VERSION=4.8.1
# Sat, 04 Feb 2023 08:15:02 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Sat, 04 Feb 2023 08:15:03 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Sat, 04 Feb 2023 08:15:16 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 04 Feb 2023 08:15:17 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Sat, 04 Feb 2023 08:15:17 GMT
ENTRYPOINT ["entrypoint.sh"]
# Sat, 04 Feb 2023 08:15:18 GMT
USER adminer
# Sat, 04 Feb 2023 08:15:19 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Sat, 04 Feb 2023 08:15:20 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:082bfbf393a7a28cd82d531b1903cc5d788ac6af1b972045ad1d0deeff1aa6ab`  
		Last Modified: Sat, 04 Feb 2023 07:54:34 GMT  
		Size: 56.0 MB (56005478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb56dd30a9439c969b4e4698f93d1d6904887b24d016964a7c0857e306cbf507`  
		Last Modified: Sat, 04 Feb 2023 08:16:26 GMT  
		Size: 39.6 MB (39558401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0895a9cfae4403af4769bb7fc2334726c0db5a6929982d11aca84a6fd3b4247`  
		Last Modified: Sat, 04 Feb 2023 08:16:17 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b8ed21414ac18410d2cd7538e45767fefbf32a8719524c47f79dbb6481c58a9`  
		Last Modified: Sat, 04 Feb 2023 08:16:17 GMT  
		Size: 1.7 KB (1718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba129a165b264b065c4c64c28d541b80a301b07360486eeaaa32fffd058c8614`  
		Last Modified: Sat, 04 Feb 2023 08:16:17 GMT  
		Size: 1.5 KB (1479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d33029a943fe1a9b73a9717bc4636749407077422d7374aa4dddc3a99a9f97a7`  
		Last Modified: Sat, 04 Feb 2023 08:16:17 GMT  
		Size: 1.4 MB (1385416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:036ba73b7268a6aed37bd51a00d8c5ffd4f4a71eb03b0aa0e8ed0a6c0123bc82`  
		Last Modified: Sat, 04 Feb 2023 08:16:17 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-standalone` - linux; mips64le

```console
$ docker pull adminer@sha256:0566934f328c80510fdb62adfc866aeb360712e6df9b0a27474a0ad53c6148a4
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.6 MB (92610528 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fcc732f3bac92ee347514fc3ed0501efa9c7a348b4e0c1d588c77787ddf8dbe4`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Thu, 09 Feb 2023 02:44:36 GMT
ADD file:0cc085dc00beb990e7bfcdd8b37dceccb8f6d62d7c5ce2d7e736cdf4d52ab799 in / 
# Thu, 09 Feb 2023 02:44:41 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 06:13:03 GMT
STOPSIGNAL SIGINT
# Thu, 09 Feb 2023 06:14:56 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 06:15:02 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Thu, 09 Feb 2023 06:15:09 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 09 Feb 2023 06:15:12 GMT
WORKDIR /var/www/html
# Thu, 09 Feb 2023 06:15:15 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 09 Feb 2023 06:15:18 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 09 Feb 2023 06:15:22 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 09 Feb 2023 06:15:25 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 09 Feb 2023 06:16:14 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 09 Feb 2023 06:16:17 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 09 Feb 2023 06:16:20 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 09 Feb 2023 06:16:23 GMT
USER adminer
# Thu, 09 Feb 2023 06:16:26 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Thu, 09 Feb 2023 06:16:30 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:11a4758105e306ed24134ddf12f4d813426845c37a0ab14cb71de94c2858f09c`  
		Last Modified: Thu, 09 Feb 2023 02:53:05 GMT  
		Size: 53.3 MB (53266784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7daca01da5691398087a3bfc7f953540cff885f22074e0129fda0d5e578a7a64`  
		Last Modified: Thu, 09 Feb 2023 06:19:06 GMT  
		Size: 38.0 MB (37953476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53cfc05716a9d1f679b734de3bff7a1b9714f5eb4b5040d6e143defb24f4975b`  
		Last Modified: Thu, 09 Feb 2023 06:18:37 GMT  
		Size: 395.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66588c07e295fc98922360681aab4fd6a5c85ca29e0d60b27a06b53038e89c06`  
		Last Modified: Thu, 09 Feb 2023 06:18:37 GMT  
		Size: 1.7 KB (1729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6920b4dc4d4b5e73a928683693ea3ec779eb5c2100896fcc49acbb46ca85198a`  
		Last Modified: Thu, 09 Feb 2023 06:18:37 GMT  
		Size: 1.5 KB (1479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a2bb1759b592851efa52aa0ae0243e97ddaee48fec421bde7daeb618542cca8`  
		Last Modified: Thu, 09 Feb 2023 06:18:38 GMT  
		Size: 1.4 MB (1386172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1a36c2a9b981a0b8491e075725805da77790fd3eb7a7b71f664ef3c369a2e14`  
		Last Modified: Thu, 09 Feb 2023 06:18:37 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-standalone` - linux; ppc64le

```console
$ docker pull adminer@sha256:47a4ade05e65fa4596b6163d81cd7a4fa77513df4972a34167a78b55224b98d7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.2 MB (101226739 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d968381d4dcfc992e9ec7607ed161acc52925d93157eed9ed50bbc08830df809`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Sat, 04 Feb 2023 12:25:27 GMT
ADD file:724a2ac3b6190353442c93dce0ad4b3ab5c60144fc8204131767af6760e11980 in / 
# Sat, 04 Feb 2023 12:25:30 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 17:52:28 GMT
STOPSIGNAL SIGINT
# Sat, 04 Feb 2023 17:53:25 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 17:53:28 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Sat, 04 Feb 2023 17:53:31 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Sat, 04 Feb 2023 17:53:31 GMT
WORKDIR /var/www/html
# Sat, 04 Feb 2023 17:53:32 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Sat, 04 Feb 2023 17:53:32 GMT
ENV ADMINER_VERSION=4.8.1
# Sat, 04 Feb 2023 17:53:32 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Sat, 04 Feb 2023 17:53:33 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Sat, 04 Feb 2023 17:54:00 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 04 Feb 2023 17:54:00 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Sat, 04 Feb 2023 17:54:00 GMT
ENTRYPOINT ["entrypoint.sh"]
# Sat, 04 Feb 2023 17:54:01 GMT
USER adminer
# Sat, 04 Feb 2023 17:54:01 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Sat, 04 Feb 2023 17:54:02 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:c14c296a64e0f557b40f88759a913c28d0b28c646e5ec0cf0ceb49457156a792`  
		Last Modified: Sat, 04 Feb 2023 12:31:37 GMT  
		Size: 58.9 MB (58897064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2874c2bcc11a32eb3e38ad44035b5962c96846742a4307ba2c420da009e81ea7`  
		Last Modified: Sat, 04 Feb 2023 17:55:24 GMT  
		Size: 40.9 MB (40940112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dff9f9467cf09d7f5c242cfb1cacef36591219699095992b5738c1a88620f1d1`  
		Last Modified: Sat, 04 Feb 2023 17:55:09 GMT  
		Size: 394.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5c16d0da50d675218fc2a7373e45781eb595f8a795b902bcadf6be87ec0c887`  
		Last Modified: Sat, 04 Feb 2023 17:55:09 GMT  
		Size: 1.9 KB (1879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20dcb0d7c1b30e96ea63a399103c52c4292e83ce4579f47057d8dfe4d78b0aef`  
		Last Modified: Sat, 04 Feb 2023 17:55:09 GMT  
		Size: 1.5 KB (1478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3f8d644f4416950947c0acf3f7511db8085e591667b824d91224cec02554543`  
		Last Modified: Sat, 04 Feb 2023 17:55:09 GMT  
		Size: 1.4 MB (1385321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02759dcc9c00093b87b4c7129217d0bb02701ea0aa1e86f4d8f0eaf7a56723ab`  
		Last Modified: Sat, 04 Feb 2023 17:55:09 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-standalone` - linux; s390x

```console
$ docker pull adminer@sha256:2719e0584d03780419167688eaba32d1ee3527400ff69f7f2cdd3db286a68aa8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.7 MB (93688213 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e9613c6a60d2d28ec14e33ed1f2f4b998316d21902a342ceca374a3b98116f1`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Thu, 09 Feb 2023 02:41:26 GMT
ADD file:952595f2a554945ef740fa7b1fbc617a9ce3e1c3b90ddf1e7c0ac6018e6a98f9 in / 
# Thu, 09 Feb 2023 02:41:30 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 07:18:54 GMT
STOPSIGNAL SIGINT
# Thu, 09 Feb 2023 07:20:03 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 07:20:13 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Thu, 09 Feb 2023 07:20:15 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 09 Feb 2023 07:20:16 GMT
WORKDIR /var/www/html
# Thu, 09 Feb 2023 07:20:17 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 09 Feb 2023 07:20:18 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 09 Feb 2023 07:20:19 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 09 Feb 2023 07:20:20 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 09 Feb 2023 07:20:29 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 09 Feb 2023 07:20:29 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 09 Feb 2023 07:20:29 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 09 Feb 2023 07:20:30 GMT
USER adminer
# Thu, 09 Feb 2023 07:20:30 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Thu, 09 Feb 2023 07:20:30 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:83809ebda0c421fc95029bc6775e0a0c1eba6916a58b115dcb6a14885dae2028`  
		Last Modified: Thu, 09 Feb 2023 02:45:46 GMT  
		Size: 53.3 MB (53278896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7e31cf57a38a02fa2d3f8ff53add4d422bd4ff62ec4b24e0831c6725cee4b77`  
		Last Modified: Thu, 09 Feb 2023 07:21:24 GMT  
		Size: 39.0 MB (39019658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0633cef61215983b712e699a77b2f0a05ae8e463a4b6c07ffa63d79c6d451f3`  
		Last Modified: Thu, 09 Feb 2023 07:21:18 GMT  
		Size: 394.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:827d0eb471d78ca9b876122dfaeddf3edb023c66c6efa92c4ec68f85e999114d`  
		Last Modified: Thu, 09 Feb 2023 07:21:18 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e6233ba1bdaa0fba57704d8dc153af1171478f4f644bcd1672d9a4fd9712ccb`  
		Last Modified: Thu, 09 Feb 2023 07:21:18 GMT  
		Size: 1.5 KB (1483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5eb9aee6c3e13c08694db2a9db11c9563576952794921b2cfa054236137c34ba`  
		Last Modified: Thu, 09 Feb 2023 07:21:18 GMT  
		Size: 1.4 MB (1385406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c778394cc4cf1727666c9cc60aec4329d57cae6761ed5d514b755368d165048`  
		Last Modified: Thu, 09 Feb 2023 07:21:18 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `adminer:4.8.1`

```console
$ docker pull adminer@sha256:d4a361f0fdbc2f8a4732a62635e043e7a883e3785a54d54f5eb0d9ce3ad80204
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `adminer:4.8.1` - linux; amd64

```console
$ docker pull adminer@sha256:8991350a6cc5acd8a607828617ad1cbd062b38528e6889664e0030b43f45d5f8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.9 MB (95901310 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:471e5d2fb746396a521960c56f7eafb8490e52be8cb499d4c0e00904c673be4e`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Sat, 04 Feb 2023 06:51:26 GMT
ADD file:cc6a56676703ec7ab5db8f2f7bc18a3169c0816d38703845b6b77ae5342ab41c in / 
# Sat, 04 Feb 2023 06:51:27 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 14:02:55 GMT
STOPSIGNAL SIGINT
# Sat, 04 Feb 2023 14:03:16 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 14:03:17 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Sat, 04 Feb 2023 14:03:17 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Sat, 04 Feb 2023 14:03:17 GMT
WORKDIR /var/www/html
# Sat, 04 Feb 2023 14:03:18 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Sat, 04 Feb 2023 14:03:18 GMT
ENV ADMINER_VERSION=4.8.1
# Sat, 04 Feb 2023 14:03:18 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Sat, 04 Feb 2023 14:03:18 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Sat, 04 Feb 2023 14:03:30 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 04 Feb 2023 14:03:30 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Sat, 04 Feb 2023 14:03:30 GMT
ENTRYPOINT ["entrypoint.sh"]
# Sat, 04 Feb 2023 14:03:30 GMT
USER adminer
# Sat, 04 Feb 2023 14:03:30 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Sat, 04 Feb 2023 14:03:30 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:699c8a97647f5789e5850bcf1a3d5afe9730edb654e1ae0714d5bd198a67a3ed`  
		Last Modified: Sat, 04 Feb 2023 06:55:53 GMT  
		Size: 55.0 MB (55025312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:154fe4cd65e5c30dd59093bd2c5edeb1d7892246dcb092564c35adb2dcc3f87b`  
		Last Modified: Sat, 04 Feb 2023 14:04:12 GMT  
		Size: 39.5 MB (39486607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:567f91a0a4b1cd6524fda2a63dd1948bf5fc7c699b172c4e9cb5986c1e5eceb7`  
		Last Modified: Sat, 04 Feb 2023 14:04:04 GMT  
		Size: 386.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce84d71503c32a8a86b5d886948c5d7d8138945998b4c31f05bfe35af0dbcd4b`  
		Last Modified: Sat, 04 Feb 2023 14:04:04 GMT  
		Size: 1.9 KB (1875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a11b9280fafb872c844c5dbff2fc246006a97a59897561411ce2c0d3676897f3`  
		Last Modified: Sat, 04 Feb 2023 14:04:04 GMT  
		Size: 1.5 KB (1477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e15d0e23848f1f6f5daf25c58fdf76a136a6dec252c28c3c1332250ad8e81c6`  
		Last Modified: Sat, 04 Feb 2023 14:04:04 GMT  
		Size: 1.4 MB (1385162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c610542bc6221747547117c74d457e30e7fce1c9394a494b2ee945e89f6faf3a`  
		Last Modified: Sat, 04 Feb 2023 14:04:04 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1` - linux; arm variant v5

```console
$ docker pull adminer@sha256:f41d812a0a97b02f761e994e55331571cbd685a2bfdeef007e9c8d098f61a58e
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.2 MB (91188340 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:937bc7e7afadd352160727b3edded381d4f7131ad46c77906131729950141670`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Thu, 09 Feb 2023 02:00:16 GMT
ADD file:f5b31ee6dfb50a99818c1a4b3aba7c6ba1557b1547aa730e4230600017520691 in / 
# Thu, 09 Feb 2023 02:00:17 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 02:24:11 GMT
STOPSIGNAL SIGINT
# Thu, 09 Feb 2023 02:25:10 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 02:25:11 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Thu, 09 Feb 2023 02:25:12 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 09 Feb 2023 02:25:12 GMT
WORKDIR /var/www/html
# Thu, 09 Feb 2023 02:25:13 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 09 Feb 2023 02:25:13 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 09 Feb 2023 02:25:13 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 09 Feb 2023 02:25:13 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 09 Feb 2023 02:25:29 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 09 Feb 2023 02:25:29 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 09 Feb 2023 02:25:29 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 09 Feb 2023 02:25:29 GMT
USER adminer
# Thu, 09 Feb 2023 02:25:29 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Thu, 09 Feb 2023 02:25:29 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:f316396b5265978a8de9d493acdc7cda735a1fae190efbd5359650183ab7271f`  
		Last Modified: Thu, 09 Feb 2023 02:05:10 GMT  
		Size: 52.6 MB (52551796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0815a961482b87ff7ddc14fbf492d26b081ca226c383b265a39b9d900705a745`  
		Last Modified: Thu, 09 Feb 2023 02:26:40 GMT  
		Size: 37.2 MB (37247283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:907d5f9eb045277cd9fb22287b0e14b7fcd0ddcf52829c1e884706cae455c579`  
		Last Modified: Thu, 09 Feb 2023 02:26:30 GMT  
		Size: 393.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8109ea45000a26ce9c558139872c68cc18839c5d9d58b6362bad0e61335be87`  
		Last Modified: Thu, 09 Feb 2023 02:26:30 GMT  
		Size: 1.8 KB (1840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de171f42adf643e4c74d58974916e2f121db8d111d838e580c9b53bed7875d54`  
		Last Modified: Thu, 09 Feb 2023 02:26:30 GMT  
		Size: 1.5 KB (1478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d391953776d5d50c308770e750f4b1df9f2041dcec59d1ea998f85fb7e012962`  
		Last Modified: Thu, 09 Feb 2023 02:26:30 GMT  
		Size: 1.4 MB (1385055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a563edb132e3a3c8e9654277a5136351be9d1d1582967ba0ada9e4772683912`  
		Last Modified: Thu, 09 Feb 2023 02:26:30 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1` - linux; arm variant v7

```console
$ docker pull adminer@sha256:9d12f8ae49e2b1ccac684b16522c130d56646a6c56fdcead2d1dbd5be32b71ea
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.8 MB (87762862 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe294facea4e18353cea22666d19efa67a350c0803293d20d943e0c6e97467b0`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Sat, 04 Feb 2023 09:59:19 GMT
ADD file:239b5255d05e0742f381f82fb7cd586fcc6d9a427263238a2be3372c494ae933 in / 
# Sat, 04 Feb 2023 09:59:20 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 10:43:54 GMT
STOPSIGNAL SIGINT
# Sat, 04 Feb 2023 10:44:19 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 10:44:20 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Sat, 04 Feb 2023 10:44:20 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Sat, 04 Feb 2023 10:44:20 GMT
WORKDIR /var/www/html
# Sat, 04 Feb 2023 10:44:20 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Sat, 04 Feb 2023 10:44:20 GMT
ENV ADMINER_VERSION=4.8.1
# Sat, 04 Feb 2023 10:44:21 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Sat, 04 Feb 2023 10:44:21 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Sat, 04 Feb 2023 10:44:33 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 04 Feb 2023 10:44:33 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Sat, 04 Feb 2023 10:44:33 GMT
ENTRYPOINT ["entrypoint.sh"]
# Sat, 04 Feb 2023 10:44:33 GMT
USER adminer
# Sat, 04 Feb 2023 10:44:34 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Sat, 04 Feb 2023 10:44:34 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:7a21a86b3957d8c99250334cfb78c55af4f8c9277f2f1d4abd53d0362f96323d`  
		Last Modified: Sat, 04 Feb 2023 10:05:53 GMT  
		Size: 50.2 MB (50190828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f647e4e293fd395af7ac8037948dbe3388c6cb6db3064a00c9f7b5ae32ba1bd1`  
		Last Modified: Sat, 04 Feb 2023 10:45:41 GMT  
		Size: 36.2 MB (36182796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc9bd65829db2cfa0c5e7daf2f0a09bc126930cc6f916496844b3e8adeb9d8ed`  
		Last Modified: Sat, 04 Feb 2023 10:45:31 GMT  
		Size: 394.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ca053278ba99e9e29b58a59e0d4e18b6a12ae83036d127f90aeed075f61139c`  
		Last Modified: Sat, 04 Feb 2023 10:45:31 GMT  
		Size: 1.8 KB (1835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:212108f5743ed386440da376a9d15e10b2349f1a1573187b747a06ea2d32abc6`  
		Last Modified: Sat, 04 Feb 2023 10:45:31 GMT  
		Size: 1.5 KB (1477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9c4b14fe58151d7c0bc6589d5264310b8afa5674ec2f3a675e5c524a8eb12df`  
		Last Modified: Sat, 04 Feb 2023 10:45:32 GMT  
		Size: 1.4 MB (1385040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5305f0630fde46637c4b273861b8dc1fd8735642c1290f7d39e3f62c58452f35`  
		Last Modified: Sat, 04 Feb 2023 10:45:31 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1` - linux; arm64 variant v8

```console
$ docker pull adminer@sha256:4f5db61ed6cff7c4d001092c5ce6d5eb7501a356739d77657c28f6b813d428c2
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.3 MB (94313416 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f55903b78a43635b55478abb38f63cd77f3e0ec223947f72aee5c6872a07ffd1`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Sat, 04 Feb 2023 06:17:26 GMT
ADD file:c5a7c65d67685092faa3456c1a772550aa6d06ac07e1f98a95d39c31e304dbf8 in / 
# Sat, 04 Feb 2023 06:17:27 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 06:40:07 GMT
STOPSIGNAL SIGINT
# Sat, 04 Feb 2023 06:40:27 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 06:40:28 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Sat, 04 Feb 2023 06:40:29 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Sat, 04 Feb 2023 06:40:29 GMT
WORKDIR /var/www/html
# Sat, 04 Feb 2023 06:40:29 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Sat, 04 Feb 2023 06:40:29 GMT
ENV ADMINER_VERSION=4.8.1
# Sat, 04 Feb 2023 06:40:29 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Sat, 04 Feb 2023 06:40:29 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Sat, 04 Feb 2023 06:40:39 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 04 Feb 2023 06:40:39 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Sat, 04 Feb 2023 06:40:39 GMT
ENTRYPOINT ["entrypoint.sh"]
# Sat, 04 Feb 2023 06:40:40 GMT
USER adminer
# Sat, 04 Feb 2023 06:40:40 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Sat, 04 Feb 2023 06:40:40 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:fac7262b6510529638951e16807cf1758f42c892ed924e334c27bb8bbcf7d7c2`  
		Last Modified: Sat, 04 Feb 2023 06:21:01 GMT  
		Size: 53.7 MB (53681927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a3c4993b9ed6a78b02081f8b79138654baa646295eb90d0f09eb178f86f610b`  
		Last Modified: Sat, 04 Feb 2023 06:41:19 GMT  
		Size: 39.2 MB (39242179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77346147b34a65302ad6ba550d6ab4659b2d986cd2c2e57248651460e8a3e589`  
		Last Modified: Sat, 04 Feb 2023 06:41:12 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56563dd7963c36713d65f09a5387503374566d7296c2bfa4422bf2d3ceb3bbeb`  
		Last Modified: Sat, 04 Feb 2023 06:41:12 GMT  
		Size: 1.9 KB (1879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fa2e6ff1278f9c9246cfedeee571a41de27494a6f3d518f136dbb8a225d7d33`  
		Last Modified: Sat, 04 Feb 2023 06:41:12 GMT  
		Size: 1.5 KB (1481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f24f727f464d597cc5ae7abb0b697c3807940cf0cca55089c3cbc553eee16523`  
		Last Modified: Sat, 04 Feb 2023 06:41:12 GMT  
		Size: 1.4 MB (1385069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:717c6895aefe53599660cfa578fea33535395f3479fdaecb0f2db55b2fa1165a`  
		Last Modified: Sat, 04 Feb 2023 06:41:12 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1` - linux; 386

```console
$ docker pull adminer@sha256:9aeaa40748b7ce615a50ef6b58624bde25df408d8e05367d32f939a9ebac3a1d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.0 MB (96953374 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0059247fefe0e30e3270aaad4163ba4bfc56aa80f66364c27054b4f9bd7ef47`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Sat, 04 Feb 2023 07:49:07 GMT
ADD file:d610d24eb19fe7e275924d58b6dad6b9f3dce21359a4ef81d04298e94382f102 in / 
# Sat, 04 Feb 2023 07:49:07 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 08:14:35 GMT
STOPSIGNAL SIGINT
# Sat, 04 Feb 2023 08:14:57 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 08:14:58 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Sat, 04 Feb 2023 08:14:59 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Sat, 04 Feb 2023 08:14:59 GMT
WORKDIR /var/www/html
# Sat, 04 Feb 2023 08:15:01 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Sat, 04 Feb 2023 08:15:01 GMT
ENV ADMINER_VERSION=4.8.1
# Sat, 04 Feb 2023 08:15:02 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Sat, 04 Feb 2023 08:15:03 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Sat, 04 Feb 2023 08:15:16 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 04 Feb 2023 08:15:17 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Sat, 04 Feb 2023 08:15:17 GMT
ENTRYPOINT ["entrypoint.sh"]
# Sat, 04 Feb 2023 08:15:18 GMT
USER adminer
# Sat, 04 Feb 2023 08:15:19 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Sat, 04 Feb 2023 08:15:20 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:082bfbf393a7a28cd82d531b1903cc5d788ac6af1b972045ad1d0deeff1aa6ab`  
		Last Modified: Sat, 04 Feb 2023 07:54:34 GMT  
		Size: 56.0 MB (56005478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb56dd30a9439c969b4e4698f93d1d6904887b24d016964a7c0857e306cbf507`  
		Last Modified: Sat, 04 Feb 2023 08:16:26 GMT  
		Size: 39.6 MB (39558401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0895a9cfae4403af4769bb7fc2334726c0db5a6929982d11aca84a6fd3b4247`  
		Last Modified: Sat, 04 Feb 2023 08:16:17 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b8ed21414ac18410d2cd7538e45767fefbf32a8719524c47f79dbb6481c58a9`  
		Last Modified: Sat, 04 Feb 2023 08:16:17 GMT  
		Size: 1.7 KB (1718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba129a165b264b065c4c64c28d541b80a301b07360486eeaaa32fffd058c8614`  
		Last Modified: Sat, 04 Feb 2023 08:16:17 GMT  
		Size: 1.5 KB (1479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d33029a943fe1a9b73a9717bc4636749407077422d7374aa4dddc3a99a9f97a7`  
		Last Modified: Sat, 04 Feb 2023 08:16:17 GMT  
		Size: 1.4 MB (1385416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:036ba73b7268a6aed37bd51a00d8c5ffd4f4a71eb03b0aa0e8ed0a6c0123bc82`  
		Last Modified: Sat, 04 Feb 2023 08:16:17 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1` - linux; mips64le

```console
$ docker pull adminer@sha256:0566934f328c80510fdb62adfc866aeb360712e6df9b0a27474a0ad53c6148a4
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.6 MB (92610528 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fcc732f3bac92ee347514fc3ed0501efa9c7a348b4e0c1d588c77787ddf8dbe4`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Thu, 09 Feb 2023 02:44:36 GMT
ADD file:0cc085dc00beb990e7bfcdd8b37dceccb8f6d62d7c5ce2d7e736cdf4d52ab799 in / 
# Thu, 09 Feb 2023 02:44:41 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 06:13:03 GMT
STOPSIGNAL SIGINT
# Thu, 09 Feb 2023 06:14:56 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 06:15:02 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Thu, 09 Feb 2023 06:15:09 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 09 Feb 2023 06:15:12 GMT
WORKDIR /var/www/html
# Thu, 09 Feb 2023 06:15:15 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 09 Feb 2023 06:15:18 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 09 Feb 2023 06:15:22 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 09 Feb 2023 06:15:25 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 09 Feb 2023 06:16:14 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 09 Feb 2023 06:16:17 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 09 Feb 2023 06:16:20 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 09 Feb 2023 06:16:23 GMT
USER adminer
# Thu, 09 Feb 2023 06:16:26 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Thu, 09 Feb 2023 06:16:30 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:11a4758105e306ed24134ddf12f4d813426845c37a0ab14cb71de94c2858f09c`  
		Last Modified: Thu, 09 Feb 2023 02:53:05 GMT  
		Size: 53.3 MB (53266784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7daca01da5691398087a3bfc7f953540cff885f22074e0129fda0d5e578a7a64`  
		Last Modified: Thu, 09 Feb 2023 06:19:06 GMT  
		Size: 38.0 MB (37953476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53cfc05716a9d1f679b734de3bff7a1b9714f5eb4b5040d6e143defb24f4975b`  
		Last Modified: Thu, 09 Feb 2023 06:18:37 GMT  
		Size: 395.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66588c07e295fc98922360681aab4fd6a5c85ca29e0d60b27a06b53038e89c06`  
		Last Modified: Thu, 09 Feb 2023 06:18:37 GMT  
		Size: 1.7 KB (1729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6920b4dc4d4b5e73a928683693ea3ec779eb5c2100896fcc49acbb46ca85198a`  
		Last Modified: Thu, 09 Feb 2023 06:18:37 GMT  
		Size: 1.5 KB (1479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a2bb1759b592851efa52aa0ae0243e97ddaee48fec421bde7daeb618542cca8`  
		Last Modified: Thu, 09 Feb 2023 06:18:38 GMT  
		Size: 1.4 MB (1386172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1a36c2a9b981a0b8491e075725805da77790fd3eb7a7b71f664ef3c369a2e14`  
		Last Modified: Thu, 09 Feb 2023 06:18:37 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1` - linux; ppc64le

```console
$ docker pull adminer@sha256:47a4ade05e65fa4596b6163d81cd7a4fa77513df4972a34167a78b55224b98d7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.2 MB (101226739 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d968381d4dcfc992e9ec7607ed161acc52925d93157eed9ed50bbc08830df809`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Sat, 04 Feb 2023 12:25:27 GMT
ADD file:724a2ac3b6190353442c93dce0ad4b3ab5c60144fc8204131767af6760e11980 in / 
# Sat, 04 Feb 2023 12:25:30 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 17:52:28 GMT
STOPSIGNAL SIGINT
# Sat, 04 Feb 2023 17:53:25 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 17:53:28 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Sat, 04 Feb 2023 17:53:31 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Sat, 04 Feb 2023 17:53:31 GMT
WORKDIR /var/www/html
# Sat, 04 Feb 2023 17:53:32 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Sat, 04 Feb 2023 17:53:32 GMT
ENV ADMINER_VERSION=4.8.1
# Sat, 04 Feb 2023 17:53:32 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Sat, 04 Feb 2023 17:53:33 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Sat, 04 Feb 2023 17:54:00 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 04 Feb 2023 17:54:00 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Sat, 04 Feb 2023 17:54:00 GMT
ENTRYPOINT ["entrypoint.sh"]
# Sat, 04 Feb 2023 17:54:01 GMT
USER adminer
# Sat, 04 Feb 2023 17:54:01 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Sat, 04 Feb 2023 17:54:02 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:c14c296a64e0f557b40f88759a913c28d0b28c646e5ec0cf0ceb49457156a792`  
		Last Modified: Sat, 04 Feb 2023 12:31:37 GMT  
		Size: 58.9 MB (58897064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2874c2bcc11a32eb3e38ad44035b5962c96846742a4307ba2c420da009e81ea7`  
		Last Modified: Sat, 04 Feb 2023 17:55:24 GMT  
		Size: 40.9 MB (40940112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dff9f9467cf09d7f5c242cfb1cacef36591219699095992b5738c1a88620f1d1`  
		Last Modified: Sat, 04 Feb 2023 17:55:09 GMT  
		Size: 394.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5c16d0da50d675218fc2a7373e45781eb595f8a795b902bcadf6be87ec0c887`  
		Last Modified: Sat, 04 Feb 2023 17:55:09 GMT  
		Size: 1.9 KB (1879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20dcb0d7c1b30e96ea63a399103c52c4292e83ce4579f47057d8dfe4d78b0aef`  
		Last Modified: Sat, 04 Feb 2023 17:55:09 GMT  
		Size: 1.5 KB (1478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3f8d644f4416950947c0acf3f7511db8085e591667b824d91224cec02554543`  
		Last Modified: Sat, 04 Feb 2023 17:55:09 GMT  
		Size: 1.4 MB (1385321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02759dcc9c00093b87b4c7129217d0bb02701ea0aa1e86f4d8f0eaf7a56723ab`  
		Last Modified: Sat, 04 Feb 2023 17:55:09 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1` - linux; s390x

```console
$ docker pull adminer@sha256:2719e0584d03780419167688eaba32d1ee3527400ff69f7f2cdd3db286a68aa8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.7 MB (93688213 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e9613c6a60d2d28ec14e33ed1f2f4b998316d21902a342ceca374a3b98116f1`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Thu, 09 Feb 2023 02:41:26 GMT
ADD file:952595f2a554945ef740fa7b1fbc617a9ce3e1c3b90ddf1e7c0ac6018e6a98f9 in / 
# Thu, 09 Feb 2023 02:41:30 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 07:18:54 GMT
STOPSIGNAL SIGINT
# Thu, 09 Feb 2023 07:20:03 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 07:20:13 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Thu, 09 Feb 2023 07:20:15 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 09 Feb 2023 07:20:16 GMT
WORKDIR /var/www/html
# Thu, 09 Feb 2023 07:20:17 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 09 Feb 2023 07:20:18 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 09 Feb 2023 07:20:19 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 09 Feb 2023 07:20:20 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 09 Feb 2023 07:20:29 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 09 Feb 2023 07:20:29 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 09 Feb 2023 07:20:29 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 09 Feb 2023 07:20:30 GMT
USER adminer
# Thu, 09 Feb 2023 07:20:30 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Thu, 09 Feb 2023 07:20:30 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:83809ebda0c421fc95029bc6775e0a0c1eba6916a58b115dcb6a14885dae2028`  
		Last Modified: Thu, 09 Feb 2023 02:45:46 GMT  
		Size: 53.3 MB (53278896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7e31cf57a38a02fa2d3f8ff53add4d422bd4ff62ec4b24e0831c6725cee4b77`  
		Last Modified: Thu, 09 Feb 2023 07:21:24 GMT  
		Size: 39.0 MB (39019658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0633cef61215983b712e699a77b2f0a05ae8e463a4b6c07ffa63d79c6d451f3`  
		Last Modified: Thu, 09 Feb 2023 07:21:18 GMT  
		Size: 394.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:827d0eb471d78ca9b876122dfaeddf3edb023c66c6efa92c4ec68f85e999114d`  
		Last Modified: Thu, 09 Feb 2023 07:21:18 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e6233ba1bdaa0fba57704d8dc153af1171478f4f644bcd1672d9a4fd9712ccb`  
		Last Modified: Thu, 09 Feb 2023 07:21:18 GMT  
		Size: 1.5 KB (1483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5eb9aee6c3e13c08694db2a9db11c9563576952794921b2cfa054236137c34ba`  
		Last Modified: Thu, 09 Feb 2023 07:21:18 GMT  
		Size: 1.4 MB (1385406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c778394cc4cf1727666c9cc60aec4329d57cae6761ed5d514b755368d165048`  
		Last Modified: Thu, 09 Feb 2023 07:21:18 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `adminer:4.8.1-fastcgi`

```console
$ docker pull adminer@sha256:7085d390109c63834cf471af0ddb9f6285d0002d0d2ee12424f8b50088fc9db2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `adminer:4.8.1-fastcgi` - linux; amd64

```console
$ docker pull adminer@sha256:a487a7e8be03bc50ec36d32b800c2a2a32ed6a5c238faca2dd38021b93b52991
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.9 MB (95904051 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64f86f40f9d98336b024a973361cd24981a21d3aba73369f77965c23e25186cf`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Sat, 04 Feb 2023 06:51:26 GMT
ADD file:cc6a56676703ec7ab5db8f2f7bc18a3169c0816d38703845b6b77ae5342ab41c in / 
# Sat, 04 Feb 2023 06:51:27 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 14:02:55 GMT
STOPSIGNAL SIGINT
# Sat, 04 Feb 2023 14:03:16 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 14:03:17 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Sat, 04 Feb 2023 14:03:36 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Sat, 04 Feb 2023 14:03:37 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Sat, 04 Feb 2023 14:03:37 GMT
WORKDIR /var/www/html
# Sat, 04 Feb 2023 14:03:37 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Sat, 04 Feb 2023 14:03:37 GMT
ENV ADMINER_VERSION=4.8.1
# Sat, 04 Feb 2023 14:03:37 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Sat, 04 Feb 2023 14:03:37 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Sat, 04 Feb 2023 14:03:48 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 04 Feb 2023 14:03:48 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Sat, 04 Feb 2023 14:03:49 GMT
ENTRYPOINT ["entrypoint.sh"]
# Sat, 04 Feb 2023 14:03:49 GMT
USER adminer
# Sat, 04 Feb 2023 14:03:49 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:699c8a97647f5789e5850bcf1a3d5afe9730edb654e1ae0714d5bd198a67a3ed`  
		Last Modified: Sat, 04 Feb 2023 06:55:53 GMT  
		Size: 55.0 MB (55025312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:154fe4cd65e5c30dd59093bd2c5edeb1d7892246dcb092564c35adb2dcc3f87b`  
		Last Modified: Sat, 04 Feb 2023 14:04:12 GMT  
		Size: 39.5 MB (39486607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:567f91a0a4b1cd6524fda2a63dd1948bf5fc7c699b172c4e9cb5986c1e5eceb7`  
		Last Modified: Sat, 04 Feb 2023 14:04:04 GMT  
		Size: 386.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43e065a08a3a44ef53db81a6b0ab94330ab02fd8a0d5c02758e2a9ccba2db806`  
		Last Modified: Sat, 04 Feb 2023 14:04:31 GMT  
		Size: 2.7 KB (2707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0154f5a2a5df6dc3e259a0da06081c740b1cc6974b3c6d2a763c82f68342132e`  
		Last Modified: Sat, 04 Feb 2023 14:04:31 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4af9bb043e0acb2d1b281a5d3f020e2437196040d7a09afda443537a7e3f3c40`  
		Last Modified: Sat, 04 Feb 2023 14:04:31 GMT  
		Size: 1.5 KB (1477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc585851cc1446d5ca0866b33d000cee9fcdac28a4c9d92bd803915ff149b87a`  
		Last Modified: Sat, 04 Feb 2023 14:04:31 GMT  
		Size: 1.4 MB (1385188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:345df3ed0a37be7be2ffe6d6abae3125fbfeb1a8624a4942368abf7585f2657a`  
		Last Modified: Sat, 04 Feb 2023 14:04:31 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1-fastcgi` - linux; arm variant v5

```console
$ docker pull adminer@sha256:326ae96ad868945cc6ce21ae1125608876936e0a60b14764f309118e60ef3f11
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.2 MB (91191039 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12511271c61962718849cd85d462dfe90b30f31ec29c7600b97a3d1da83e8b1d`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Thu, 09 Feb 2023 02:00:16 GMT
ADD file:f5b31ee6dfb50a99818c1a4b3aba7c6ba1557b1547aa730e4230600017520691 in / 
# Thu, 09 Feb 2023 02:00:17 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 02:24:11 GMT
STOPSIGNAL SIGINT
# Thu, 09 Feb 2023 02:25:10 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 02:25:11 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Thu, 09 Feb 2023 02:25:39 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Thu, 09 Feb 2023 02:25:39 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 09 Feb 2023 02:25:40 GMT
WORKDIR /var/www/html
# Thu, 09 Feb 2023 02:25:40 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 09 Feb 2023 02:25:40 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 09 Feb 2023 02:25:40 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 09 Feb 2023 02:25:40 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 09 Feb 2023 02:25:56 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 09 Feb 2023 02:25:57 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 09 Feb 2023 02:25:57 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 09 Feb 2023 02:25:57 GMT
USER adminer
# Thu, 09 Feb 2023 02:25:57 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:f316396b5265978a8de9d493acdc7cda735a1fae190efbd5359650183ab7271f`  
		Last Modified: Thu, 09 Feb 2023 02:05:10 GMT  
		Size: 52.6 MB (52551796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0815a961482b87ff7ddc14fbf492d26b081ca226c383b265a39b9d900705a745`  
		Last Modified: Thu, 09 Feb 2023 02:26:40 GMT  
		Size: 37.2 MB (37247283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:907d5f9eb045277cd9fb22287b0e14b7fcd0ddcf52829c1e884706cae455c579`  
		Last Modified: Thu, 09 Feb 2023 02:26:30 GMT  
		Size: 393.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a3fe13d432c7dc589c9f54a560146f1249dfb75cf8f7169dfce8ac53c037021`  
		Last Modified: Thu, 09 Feb 2023 02:27:04 GMT  
		Size: 2.7 KB (2711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c23eca33f0e2498aefa42e88bcc0e47b715bdd1aae38f94434fb4ea6bdc0795e`  
		Last Modified: Thu, 09 Feb 2023 02:27:04 GMT  
		Size: 1.8 KB (1840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05f6bb9d806bbc982ab481b1906091f08c8ada35a23423c887544b3f135ac66f`  
		Last Modified: Thu, 09 Feb 2023 02:27:04 GMT  
		Size: 1.5 KB (1480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1c811cb2797199efbeb3147f223e01f6c28cee6d87b39a36fe8eb5347b987cd`  
		Last Modified: Thu, 09 Feb 2023 02:27:05 GMT  
		Size: 1.4 MB (1385045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6475dd585587079dec552c0910151d39ef0972f2f7ac63073ae5b67064c15ba3`  
		Last Modified: Thu, 09 Feb 2023 02:27:04 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1-fastcgi` - linux; arm variant v7

```console
$ docker pull adminer@sha256:1745d08452780cad59501ee3c384e5cae58ab9f36b395347e4470f47f02f24ed
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.8 MB (87765580 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:004424ead9c2af6485083598520693d3cdc5f59da6283b4ccfc7424319280fc3`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Sat, 04 Feb 2023 09:59:19 GMT
ADD file:239b5255d05e0742f381f82fb7cd586fcc6d9a427263238a2be3372c494ae933 in / 
# Sat, 04 Feb 2023 09:59:20 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 10:43:54 GMT
STOPSIGNAL SIGINT
# Sat, 04 Feb 2023 10:44:19 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 10:44:20 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Sat, 04 Feb 2023 10:44:47 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Sat, 04 Feb 2023 10:44:47 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Sat, 04 Feb 2023 10:44:47 GMT
WORKDIR /var/www/html
# Sat, 04 Feb 2023 10:44:48 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Sat, 04 Feb 2023 10:44:48 GMT
ENV ADMINER_VERSION=4.8.1
# Sat, 04 Feb 2023 10:44:48 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Sat, 04 Feb 2023 10:44:48 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Sat, 04 Feb 2023 10:45:00 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 04 Feb 2023 10:45:00 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Sat, 04 Feb 2023 10:45:00 GMT
ENTRYPOINT ["entrypoint.sh"]
# Sat, 04 Feb 2023 10:45:01 GMT
USER adminer
# Sat, 04 Feb 2023 10:45:01 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:7a21a86b3957d8c99250334cfb78c55af4f8c9277f2f1d4abd53d0362f96323d`  
		Last Modified: Sat, 04 Feb 2023 10:05:53 GMT  
		Size: 50.2 MB (50190828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f647e4e293fd395af7ac8037948dbe3388c6cb6db3064a00c9f7b5ae32ba1bd1`  
		Last Modified: Sat, 04 Feb 2023 10:45:41 GMT  
		Size: 36.2 MB (36182796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc9bd65829db2cfa0c5e7daf2f0a09bc126930cc6f916496844b3e8adeb9d8ed`  
		Last Modified: Sat, 04 Feb 2023 10:45:31 GMT  
		Size: 394.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcec0a137102a4df6e8f3bae77f95cb2d0288be8d86aa062191a0994da6a09a1`  
		Last Modified: Sat, 04 Feb 2023 10:46:04 GMT  
		Size: 2.7 KB (2710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9366bc96b1ef426445bd576c64c5638c631fd82aeb0453f3871a82d91ecd0df1`  
		Last Modified: Sat, 04 Feb 2023 10:46:04 GMT  
		Size: 1.8 KB (1836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:459144f5a86bfff13a40970a73b497f8392eccdd9238e210b72ed37ace1dd2c8`  
		Last Modified: Sat, 04 Feb 2023 10:46:04 GMT  
		Size: 1.5 KB (1481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3a153a1f8dd4081e72343761ee75a8397e7809582b6a8d42a491dbc499b8719`  
		Last Modified: Sat, 04 Feb 2023 10:46:05 GMT  
		Size: 1.4 MB (1385045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc9fe3e24aab98148380a5d410c285619711932dcdcbe7cca25ee0aae77b4cb3`  
		Last Modified: Sat, 04 Feb 2023 10:46:04 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1-fastcgi` - linux; arm64 variant v8

```console
$ docker pull adminer@sha256:14e5c9e9653cd354401e9d672d76e6462430024848ee435c02d0ff4332126317
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.3 MB (94316110 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0fa0825c1e857cf1eab6178105270bd008b049eb53696b1d94ed671c6284c846`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Sat, 04 Feb 2023 06:17:26 GMT
ADD file:c5a7c65d67685092faa3456c1a772550aa6d06ac07e1f98a95d39c31e304dbf8 in / 
# Sat, 04 Feb 2023 06:17:27 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 06:40:07 GMT
STOPSIGNAL SIGINT
# Sat, 04 Feb 2023 06:40:27 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 06:40:28 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Sat, 04 Feb 2023 06:40:47 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Sat, 04 Feb 2023 06:40:48 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Sat, 04 Feb 2023 06:40:48 GMT
WORKDIR /var/www/html
# Sat, 04 Feb 2023 06:40:48 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Sat, 04 Feb 2023 06:40:48 GMT
ENV ADMINER_VERSION=4.8.1
# Sat, 04 Feb 2023 06:40:48 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Sat, 04 Feb 2023 06:40:48 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Sat, 04 Feb 2023 06:40:57 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 04 Feb 2023 06:40:57 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Sat, 04 Feb 2023 06:40:58 GMT
ENTRYPOINT ["entrypoint.sh"]
# Sat, 04 Feb 2023 06:40:58 GMT
USER adminer
# Sat, 04 Feb 2023 06:40:58 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:fac7262b6510529638951e16807cf1758f42c892ed924e334c27bb8bbcf7d7c2`  
		Last Modified: Sat, 04 Feb 2023 06:21:01 GMT  
		Size: 53.7 MB (53681927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a3c4993b9ed6a78b02081f8b79138654baa646295eb90d0f09eb178f86f610b`  
		Last Modified: Sat, 04 Feb 2023 06:41:19 GMT  
		Size: 39.2 MB (39242179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77346147b34a65302ad6ba550d6ab4659b2d986cd2c2e57248651460e8a3e589`  
		Last Modified: Sat, 04 Feb 2023 06:41:12 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d66723d85a15a95d2bc016413f1fb69ae885d83e587a97d2043d370cf67e2db1`  
		Last Modified: Sat, 04 Feb 2023 06:41:36 GMT  
		Size: 2.7 KB (2707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7d226beb0ae597acd7e2647b0f4d4fc5227c69df6dff1165b4fe514cfad8130`  
		Last Modified: Sat, 04 Feb 2023 06:41:36 GMT  
		Size: 1.9 KB (1878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:def3ff5795d638c86eb1ce6b33aa5b7ac1991a913a5795be71a67c8f0bc1eab6`  
		Last Modified: Sat, 04 Feb 2023 06:41:36 GMT  
		Size: 1.5 KB (1476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:277a8bd87f658c231dabf9f7c494772cd03abace79d86737b913b73e89ee7bac`  
		Last Modified: Sat, 04 Feb 2023 06:41:37 GMT  
		Size: 1.4 MB (1385063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e95c557117dcc88c76c221f757a0f3404ad012a7726a260eadd4aba9b4e3341`  
		Last Modified: Sat, 04 Feb 2023 06:41:37 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1-fastcgi` - linux; 386

```console
$ docker pull adminer@sha256:b0a3d3e0b21c7f00206ed8268c4dd0c6f085e410f729fb795bb885f8cac1098f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.0 MB (96956091 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9fa3646b337edc6af84c9cd6a950e859eaf4183842f124b5742da2f3495e257`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Sat, 04 Feb 2023 07:49:07 GMT
ADD file:d610d24eb19fe7e275924d58b6dad6b9f3dce21359a4ef81d04298e94382f102 in / 
# Sat, 04 Feb 2023 07:49:07 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 08:14:35 GMT
STOPSIGNAL SIGINT
# Sat, 04 Feb 2023 08:14:57 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 08:14:58 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Sat, 04 Feb 2023 08:15:27 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Sat, 04 Feb 2023 08:15:28 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Sat, 04 Feb 2023 08:15:29 GMT
WORKDIR /var/www/html
# Sat, 04 Feb 2023 08:15:31 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Sat, 04 Feb 2023 08:15:31 GMT
ENV ADMINER_VERSION=4.8.1
# Sat, 04 Feb 2023 08:15:32 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Sat, 04 Feb 2023 08:15:33 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Sat, 04 Feb 2023 08:15:45 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 04 Feb 2023 08:15:47 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Sat, 04 Feb 2023 08:15:47 GMT
ENTRYPOINT ["entrypoint.sh"]
# Sat, 04 Feb 2023 08:15:48 GMT
USER adminer
# Sat, 04 Feb 2023 08:15:49 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:082bfbf393a7a28cd82d531b1903cc5d788ac6af1b972045ad1d0deeff1aa6ab`  
		Last Modified: Sat, 04 Feb 2023 07:54:34 GMT  
		Size: 56.0 MB (56005478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb56dd30a9439c969b4e4698f93d1d6904887b24d016964a7c0857e306cbf507`  
		Last Modified: Sat, 04 Feb 2023 08:16:26 GMT  
		Size: 39.6 MB (39558401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0895a9cfae4403af4769bb7fc2334726c0db5a6929982d11aca84a6fd3b4247`  
		Last Modified: Sat, 04 Feb 2023 08:16:17 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fb386372d050d61199d8b69f8eba0503204b1435c14765dcc7391690f40e104`  
		Last Modified: Sat, 04 Feb 2023 08:16:47 GMT  
		Size: 2.7 KB (2709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92775617fc6814142b985df263b604974edc157e129229cd23234c9ea1e661e6`  
		Last Modified: Sat, 04 Feb 2023 08:16:47 GMT  
		Size: 1.7 KB (1714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f95cd3c9ca70db181013ee630ed1999515d90622129ffa1cffcb8610f0f456f7`  
		Last Modified: Sat, 04 Feb 2023 08:16:48 GMT  
		Size: 1.5 KB (1480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fe214dd6c4ba9b73bd44278fa41542b21e1144c6ff3ac53e197896801e87d48`  
		Last Modified: Sat, 04 Feb 2023 08:16:48 GMT  
		Size: 1.4 MB (1385428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:469bbb9c9519bc4c9fbd635879319fa1b6f74e4a9f271572fb23cbc31bcd739c`  
		Last Modified: Sat, 04 Feb 2023 08:16:47 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1-fastcgi` - linux; mips64le

```console
$ docker pull adminer@sha256:d49eaa95df7a4b3b648e490d31d318b52533773169fecbc5a057d0012ea43a55
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.6 MB (92613258 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5cbd3305cd6fd59e4170383251a3e22ee9ca9c66bae9ba0b1914c9ffae1b23f6`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Thu, 09 Feb 2023 02:44:36 GMT
ADD file:0cc085dc00beb990e7bfcdd8b37dceccb8f6d62d7c5ce2d7e736cdf4d52ab799 in / 
# Thu, 09 Feb 2023 02:44:41 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 06:13:03 GMT
STOPSIGNAL SIGINT
# Thu, 09 Feb 2023 06:14:56 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 06:15:02 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Thu, 09 Feb 2023 06:16:50 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Thu, 09 Feb 2023 06:16:56 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 09 Feb 2023 06:16:59 GMT
WORKDIR /var/www/html
# Thu, 09 Feb 2023 06:17:02 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 09 Feb 2023 06:17:05 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 09 Feb 2023 06:17:08 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 09 Feb 2023 06:17:11 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 09 Feb 2023 06:17:59 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 09 Feb 2023 06:18:02 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 09 Feb 2023 06:18:05 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 09 Feb 2023 06:18:09 GMT
USER adminer
# Thu, 09 Feb 2023 06:18:12 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:11a4758105e306ed24134ddf12f4d813426845c37a0ab14cb71de94c2858f09c`  
		Last Modified: Thu, 09 Feb 2023 02:53:05 GMT  
		Size: 53.3 MB (53266784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7daca01da5691398087a3bfc7f953540cff885f22074e0129fda0d5e578a7a64`  
		Last Modified: Thu, 09 Feb 2023 06:19:06 GMT  
		Size: 38.0 MB (37953476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53cfc05716a9d1f679b734de3bff7a1b9714f5eb4b5040d6e143defb24f4975b`  
		Last Modified: Thu, 09 Feb 2023 06:18:37 GMT  
		Size: 395.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6df2d2de23d5a64cae787901af3f38fcaf86ab721824c7226d9bb8586ddba9fa`  
		Last Modified: Thu, 09 Feb 2023 06:19:25 GMT  
		Size: 2.7 KB (2714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f7734475a7c59ac576ed3322ac3274c2a727bb9a6c660381c515c9bf8ded7c0`  
		Last Modified: Thu, 09 Feb 2023 06:19:25 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b439c2c16da41627079e7dc7e3e2618e41b7ac3019f33d234ac6a50e1271e8c`  
		Last Modified: Thu, 09 Feb 2023 06:19:25 GMT  
		Size: 1.5 KB (1481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de57b503c9c79ca9d98a1575e8b2a2fec4f4f34a8184502f8a1697d783873671`  
		Last Modified: Thu, 09 Feb 2023 06:19:26 GMT  
		Size: 1.4 MB (1386183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27aac5c4950f7dd7352e76a2718d3c9d2974ba7ea1b383509d9a235534ccf422`  
		Last Modified: Thu, 09 Feb 2023 06:19:25 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1-fastcgi` - linux; ppc64le

```console
$ docker pull adminer@sha256:4cbfd32fc3e0995849078137f63ac73353137c150f2af36869c97efcfd354baf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.2 MB (101229475 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6003343fd4014a739aa486639e78adf252f5a00a89aada720a7d97a43b19b920`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Sat, 04 Feb 2023 12:25:27 GMT
ADD file:724a2ac3b6190353442c93dce0ad4b3ab5c60144fc8204131767af6760e11980 in / 
# Sat, 04 Feb 2023 12:25:30 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 17:52:28 GMT
STOPSIGNAL SIGINT
# Sat, 04 Feb 2023 17:53:25 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 17:53:28 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Sat, 04 Feb 2023 17:54:10 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Sat, 04 Feb 2023 17:54:12 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Sat, 04 Feb 2023 17:54:12 GMT
WORKDIR /var/www/html
# Sat, 04 Feb 2023 17:54:13 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Sat, 04 Feb 2023 17:54:13 GMT
ENV ADMINER_VERSION=4.8.1
# Sat, 04 Feb 2023 17:54:14 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Sat, 04 Feb 2023 17:54:14 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Sat, 04 Feb 2023 17:54:37 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 04 Feb 2023 17:54:38 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Sat, 04 Feb 2023 17:54:38 GMT
ENTRYPOINT ["entrypoint.sh"]
# Sat, 04 Feb 2023 17:54:39 GMT
USER adminer
# Sat, 04 Feb 2023 17:54:39 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:c14c296a64e0f557b40f88759a913c28d0b28c646e5ec0cf0ceb49457156a792`  
		Last Modified: Sat, 04 Feb 2023 12:31:37 GMT  
		Size: 58.9 MB (58897064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2874c2bcc11a32eb3e38ad44035b5962c96846742a4307ba2c420da009e81ea7`  
		Last Modified: Sat, 04 Feb 2023 17:55:24 GMT  
		Size: 40.9 MB (40940112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dff9f9467cf09d7f5c242cfb1cacef36591219699095992b5738c1a88620f1d1`  
		Last Modified: Sat, 04 Feb 2023 17:55:09 GMT  
		Size: 394.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:268a861c77efb05e4765d3315e40b2b4a6eacb3bb56a931f6c7e4ac1b5d7a265`  
		Last Modified: Sat, 04 Feb 2023 17:55:49 GMT  
		Size: 2.7 KB (2713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d71f60a34a72995c8870893c023406f4337b9a7f557f7bd26fcd612bee6cce28`  
		Last Modified: Sat, 04 Feb 2023 17:55:49 GMT  
		Size: 1.9 KB (1875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d8ca4564d1e76d1b90184e8ab33c27849b4edd5735ea578f8c79dd312d99bfe`  
		Last Modified: Sat, 04 Feb 2023 17:55:49 GMT  
		Size: 1.5 KB (1479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f53ee83c5e9a3c93576c0b61fabdb84f2dbcb11a7a34d0f80a557d128e40db47`  
		Last Modified: Sat, 04 Feb 2023 17:55:50 GMT  
		Size: 1.4 MB (1385349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75395692fa85a6f6cd605c59de5987ad5629d3f4557722b950098cf11ff887ef`  
		Last Modified: Sat, 04 Feb 2023 17:55:49 GMT  
		Size: 489.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1-fastcgi` - linux; s390x

```console
$ docker pull adminer@sha256:18930d5a14bb6b0eed4846e2b4a90aa9c731d4bde1eaf1abd60b51fe04453482
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.7 MB (93690838 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70050059db8c471d2394648f649f412ef6339c12ef4d0eeda7baa78c8bda768d`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Thu, 09 Feb 2023 02:41:26 GMT
ADD file:952595f2a554945ef740fa7b1fbc617a9ce3e1c3b90ddf1e7c0ac6018e6a98f9 in / 
# Thu, 09 Feb 2023 02:41:30 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 07:18:54 GMT
STOPSIGNAL SIGINT
# Thu, 09 Feb 2023 07:20:03 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 07:20:13 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Thu, 09 Feb 2023 07:20:43 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Thu, 09 Feb 2023 07:20:43 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 09 Feb 2023 07:20:43 GMT
WORKDIR /var/www/html
# Thu, 09 Feb 2023 07:20:44 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 09 Feb 2023 07:20:44 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 09 Feb 2023 07:20:44 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 09 Feb 2023 07:20:44 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 09 Feb 2023 07:20:52 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 09 Feb 2023 07:20:52 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 09 Feb 2023 07:20:52 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 09 Feb 2023 07:20:52 GMT
USER adminer
# Thu, 09 Feb 2023 07:20:52 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:83809ebda0c421fc95029bc6775e0a0c1eba6916a58b115dcb6a14885dae2028`  
		Last Modified: Thu, 09 Feb 2023 02:45:46 GMT  
		Size: 53.3 MB (53278896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7e31cf57a38a02fa2d3f8ff53add4d422bd4ff62ec4b24e0831c6725cee4b77`  
		Last Modified: Thu, 09 Feb 2023 07:21:24 GMT  
		Size: 39.0 MB (39019658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0633cef61215983b712e699a77b2f0a05ae8e463a4b6c07ffa63d79c6d451f3`  
		Last Modified: Thu, 09 Feb 2023 07:21:18 GMT  
		Size: 394.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c646918dad5e786008b8b31bc7f8cac9feb3521e1d4fbf6ba3c37c97bca49c6`  
		Last Modified: Thu, 09 Feb 2023 07:21:40 GMT  
		Size: 2.7 KB (2713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7c07b11a4865d90a2153a6c3e2e55161be6e83d2506f65db1ea5772aebd7219`  
		Last Modified: Thu, 09 Feb 2023 07:21:40 GMT  
		Size: 1.9 KB (1883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e13620c00e8614858376f34b19455eec2ec9325ff8082ea4407d7d72c6a4d268`  
		Last Modified: Thu, 09 Feb 2023 07:21:40 GMT  
		Size: 1.5 KB (1480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8900c81dcea2d296a964de4c28bca524bf07456b72f0cf57f0f50936cb7cf920`  
		Last Modified: Thu, 09 Feb 2023 07:21:40 GMT  
		Size: 1.4 MB (1385322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6632f7644ccabb5e6050f96cc7957a22e0bf86f0e5eff036f2a33254d3b34db`  
		Last Modified: Thu, 09 Feb 2023 07:21:40 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `adminer:4.8.1-standalone`

```console
$ docker pull adminer@sha256:d4a361f0fdbc2f8a4732a62635e043e7a883e3785a54d54f5eb0d9ce3ad80204
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `adminer:4.8.1-standalone` - linux; amd64

```console
$ docker pull adminer@sha256:8991350a6cc5acd8a607828617ad1cbd062b38528e6889664e0030b43f45d5f8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.9 MB (95901310 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:471e5d2fb746396a521960c56f7eafb8490e52be8cb499d4c0e00904c673be4e`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Sat, 04 Feb 2023 06:51:26 GMT
ADD file:cc6a56676703ec7ab5db8f2f7bc18a3169c0816d38703845b6b77ae5342ab41c in / 
# Sat, 04 Feb 2023 06:51:27 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 14:02:55 GMT
STOPSIGNAL SIGINT
# Sat, 04 Feb 2023 14:03:16 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 14:03:17 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Sat, 04 Feb 2023 14:03:17 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Sat, 04 Feb 2023 14:03:17 GMT
WORKDIR /var/www/html
# Sat, 04 Feb 2023 14:03:18 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Sat, 04 Feb 2023 14:03:18 GMT
ENV ADMINER_VERSION=4.8.1
# Sat, 04 Feb 2023 14:03:18 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Sat, 04 Feb 2023 14:03:18 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Sat, 04 Feb 2023 14:03:30 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 04 Feb 2023 14:03:30 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Sat, 04 Feb 2023 14:03:30 GMT
ENTRYPOINT ["entrypoint.sh"]
# Sat, 04 Feb 2023 14:03:30 GMT
USER adminer
# Sat, 04 Feb 2023 14:03:30 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Sat, 04 Feb 2023 14:03:30 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:699c8a97647f5789e5850bcf1a3d5afe9730edb654e1ae0714d5bd198a67a3ed`  
		Last Modified: Sat, 04 Feb 2023 06:55:53 GMT  
		Size: 55.0 MB (55025312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:154fe4cd65e5c30dd59093bd2c5edeb1d7892246dcb092564c35adb2dcc3f87b`  
		Last Modified: Sat, 04 Feb 2023 14:04:12 GMT  
		Size: 39.5 MB (39486607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:567f91a0a4b1cd6524fda2a63dd1948bf5fc7c699b172c4e9cb5986c1e5eceb7`  
		Last Modified: Sat, 04 Feb 2023 14:04:04 GMT  
		Size: 386.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce84d71503c32a8a86b5d886948c5d7d8138945998b4c31f05bfe35af0dbcd4b`  
		Last Modified: Sat, 04 Feb 2023 14:04:04 GMT  
		Size: 1.9 KB (1875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a11b9280fafb872c844c5dbff2fc246006a97a59897561411ce2c0d3676897f3`  
		Last Modified: Sat, 04 Feb 2023 14:04:04 GMT  
		Size: 1.5 KB (1477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e15d0e23848f1f6f5daf25c58fdf76a136a6dec252c28c3c1332250ad8e81c6`  
		Last Modified: Sat, 04 Feb 2023 14:04:04 GMT  
		Size: 1.4 MB (1385162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c610542bc6221747547117c74d457e30e7fce1c9394a494b2ee945e89f6faf3a`  
		Last Modified: Sat, 04 Feb 2023 14:04:04 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1-standalone` - linux; arm variant v5

```console
$ docker pull adminer@sha256:f41d812a0a97b02f761e994e55331571cbd685a2bfdeef007e9c8d098f61a58e
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.2 MB (91188340 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:937bc7e7afadd352160727b3edded381d4f7131ad46c77906131729950141670`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Thu, 09 Feb 2023 02:00:16 GMT
ADD file:f5b31ee6dfb50a99818c1a4b3aba7c6ba1557b1547aa730e4230600017520691 in / 
# Thu, 09 Feb 2023 02:00:17 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 02:24:11 GMT
STOPSIGNAL SIGINT
# Thu, 09 Feb 2023 02:25:10 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 02:25:11 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Thu, 09 Feb 2023 02:25:12 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 09 Feb 2023 02:25:12 GMT
WORKDIR /var/www/html
# Thu, 09 Feb 2023 02:25:13 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 09 Feb 2023 02:25:13 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 09 Feb 2023 02:25:13 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 09 Feb 2023 02:25:13 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 09 Feb 2023 02:25:29 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 09 Feb 2023 02:25:29 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 09 Feb 2023 02:25:29 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 09 Feb 2023 02:25:29 GMT
USER adminer
# Thu, 09 Feb 2023 02:25:29 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Thu, 09 Feb 2023 02:25:29 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:f316396b5265978a8de9d493acdc7cda735a1fae190efbd5359650183ab7271f`  
		Last Modified: Thu, 09 Feb 2023 02:05:10 GMT  
		Size: 52.6 MB (52551796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0815a961482b87ff7ddc14fbf492d26b081ca226c383b265a39b9d900705a745`  
		Last Modified: Thu, 09 Feb 2023 02:26:40 GMT  
		Size: 37.2 MB (37247283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:907d5f9eb045277cd9fb22287b0e14b7fcd0ddcf52829c1e884706cae455c579`  
		Last Modified: Thu, 09 Feb 2023 02:26:30 GMT  
		Size: 393.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8109ea45000a26ce9c558139872c68cc18839c5d9d58b6362bad0e61335be87`  
		Last Modified: Thu, 09 Feb 2023 02:26:30 GMT  
		Size: 1.8 KB (1840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de171f42adf643e4c74d58974916e2f121db8d111d838e580c9b53bed7875d54`  
		Last Modified: Thu, 09 Feb 2023 02:26:30 GMT  
		Size: 1.5 KB (1478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d391953776d5d50c308770e750f4b1df9f2041dcec59d1ea998f85fb7e012962`  
		Last Modified: Thu, 09 Feb 2023 02:26:30 GMT  
		Size: 1.4 MB (1385055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a563edb132e3a3c8e9654277a5136351be9d1d1582967ba0ada9e4772683912`  
		Last Modified: Thu, 09 Feb 2023 02:26:30 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1-standalone` - linux; arm variant v7

```console
$ docker pull adminer@sha256:9d12f8ae49e2b1ccac684b16522c130d56646a6c56fdcead2d1dbd5be32b71ea
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.8 MB (87762862 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe294facea4e18353cea22666d19efa67a350c0803293d20d943e0c6e97467b0`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Sat, 04 Feb 2023 09:59:19 GMT
ADD file:239b5255d05e0742f381f82fb7cd586fcc6d9a427263238a2be3372c494ae933 in / 
# Sat, 04 Feb 2023 09:59:20 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 10:43:54 GMT
STOPSIGNAL SIGINT
# Sat, 04 Feb 2023 10:44:19 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 10:44:20 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Sat, 04 Feb 2023 10:44:20 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Sat, 04 Feb 2023 10:44:20 GMT
WORKDIR /var/www/html
# Sat, 04 Feb 2023 10:44:20 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Sat, 04 Feb 2023 10:44:20 GMT
ENV ADMINER_VERSION=4.8.1
# Sat, 04 Feb 2023 10:44:21 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Sat, 04 Feb 2023 10:44:21 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Sat, 04 Feb 2023 10:44:33 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 04 Feb 2023 10:44:33 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Sat, 04 Feb 2023 10:44:33 GMT
ENTRYPOINT ["entrypoint.sh"]
# Sat, 04 Feb 2023 10:44:33 GMT
USER adminer
# Sat, 04 Feb 2023 10:44:34 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Sat, 04 Feb 2023 10:44:34 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:7a21a86b3957d8c99250334cfb78c55af4f8c9277f2f1d4abd53d0362f96323d`  
		Last Modified: Sat, 04 Feb 2023 10:05:53 GMT  
		Size: 50.2 MB (50190828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f647e4e293fd395af7ac8037948dbe3388c6cb6db3064a00c9f7b5ae32ba1bd1`  
		Last Modified: Sat, 04 Feb 2023 10:45:41 GMT  
		Size: 36.2 MB (36182796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc9bd65829db2cfa0c5e7daf2f0a09bc126930cc6f916496844b3e8adeb9d8ed`  
		Last Modified: Sat, 04 Feb 2023 10:45:31 GMT  
		Size: 394.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ca053278ba99e9e29b58a59e0d4e18b6a12ae83036d127f90aeed075f61139c`  
		Last Modified: Sat, 04 Feb 2023 10:45:31 GMT  
		Size: 1.8 KB (1835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:212108f5743ed386440da376a9d15e10b2349f1a1573187b747a06ea2d32abc6`  
		Last Modified: Sat, 04 Feb 2023 10:45:31 GMT  
		Size: 1.5 KB (1477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9c4b14fe58151d7c0bc6589d5264310b8afa5674ec2f3a675e5c524a8eb12df`  
		Last Modified: Sat, 04 Feb 2023 10:45:32 GMT  
		Size: 1.4 MB (1385040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5305f0630fde46637c4b273861b8dc1fd8735642c1290f7d39e3f62c58452f35`  
		Last Modified: Sat, 04 Feb 2023 10:45:31 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1-standalone` - linux; arm64 variant v8

```console
$ docker pull adminer@sha256:4f5db61ed6cff7c4d001092c5ce6d5eb7501a356739d77657c28f6b813d428c2
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.3 MB (94313416 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f55903b78a43635b55478abb38f63cd77f3e0ec223947f72aee5c6872a07ffd1`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Sat, 04 Feb 2023 06:17:26 GMT
ADD file:c5a7c65d67685092faa3456c1a772550aa6d06ac07e1f98a95d39c31e304dbf8 in / 
# Sat, 04 Feb 2023 06:17:27 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 06:40:07 GMT
STOPSIGNAL SIGINT
# Sat, 04 Feb 2023 06:40:27 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 06:40:28 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Sat, 04 Feb 2023 06:40:29 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Sat, 04 Feb 2023 06:40:29 GMT
WORKDIR /var/www/html
# Sat, 04 Feb 2023 06:40:29 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Sat, 04 Feb 2023 06:40:29 GMT
ENV ADMINER_VERSION=4.8.1
# Sat, 04 Feb 2023 06:40:29 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Sat, 04 Feb 2023 06:40:29 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Sat, 04 Feb 2023 06:40:39 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 04 Feb 2023 06:40:39 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Sat, 04 Feb 2023 06:40:39 GMT
ENTRYPOINT ["entrypoint.sh"]
# Sat, 04 Feb 2023 06:40:40 GMT
USER adminer
# Sat, 04 Feb 2023 06:40:40 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Sat, 04 Feb 2023 06:40:40 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:fac7262b6510529638951e16807cf1758f42c892ed924e334c27bb8bbcf7d7c2`  
		Last Modified: Sat, 04 Feb 2023 06:21:01 GMT  
		Size: 53.7 MB (53681927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a3c4993b9ed6a78b02081f8b79138654baa646295eb90d0f09eb178f86f610b`  
		Last Modified: Sat, 04 Feb 2023 06:41:19 GMT  
		Size: 39.2 MB (39242179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77346147b34a65302ad6ba550d6ab4659b2d986cd2c2e57248651460e8a3e589`  
		Last Modified: Sat, 04 Feb 2023 06:41:12 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56563dd7963c36713d65f09a5387503374566d7296c2bfa4422bf2d3ceb3bbeb`  
		Last Modified: Sat, 04 Feb 2023 06:41:12 GMT  
		Size: 1.9 KB (1879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fa2e6ff1278f9c9246cfedeee571a41de27494a6f3d518f136dbb8a225d7d33`  
		Last Modified: Sat, 04 Feb 2023 06:41:12 GMT  
		Size: 1.5 KB (1481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f24f727f464d597cc5ae7abb0b697c3807940cf0cca55089c3cbc553eee16523`  
		Last Modified: Sat, 04 Feb 2023 06:41:12 GMT  
		Size: 1.4 MB (1385069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:717c6895aefe53599660cfa578fea33535395f3479fdaecb0f2db55b2fa1165a`  
		Last Modified: Sat, 04 Feb 2023 06:41:12 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1-standalone` - linux; 386

```console
$ docker pull adminer@sha256:9aeaa40748b7ce615a50ef6b58624bde25df408d8e05367d32f939a9ebac3a1d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.0 MB (96953374 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0059247fefe0e30e3270aaad4163ba4bfc56aa80f66364c27054b4f9bd7ef47`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Sat, 04 Feb 2023 07:49:07 GMT
ADD file:d610d24eb19fe7e275924d58b6dad6b9f3dce21359a4ef81d04298e94382f102 in / 
# Sat, 04 Feb 2023 07:49:07 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 08:14:35 GMT
STOPSIGNAL SIGINT
# Sat, 04 Feb 2023 08:14:57 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 08:14:58 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Sat, 04 Feb 2023 08:14:59 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Sat, 04 Feb 2023 08:14:59 GMT
WORKDIR /var/www/html
# Sat, 04 Feb 2023 08:15:01 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Sat, 04 Feb 2023 08:15:01 GMT
ENV ADMINER_VERSION=4.8.1
# Sat, 04 Feb 2023 08:15:02 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Sat, 04 Feb 2023 08:15:03 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Sat, 04 Feb 2023 08:15:16 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 04 Feb 2023 08:15:17 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Sat, 04 Feb 2023 08:15:17 GMT
ENTRYPOINT ["entrypoint.sh"]
# Sat, 04 Feb 2023 08:15:18 GMT
USER adminer
# Sat, 04 Feb 2023 08:15:19 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Sat, 04 Feb 2023 08:15:20 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:082bfbf393a7a28cd82d531b1903cc5d788ac6af1b972045ad1d0deeff1aa6ab`  
		Last Modified: Sat, 04 Feb 2023 07:54:34 GMT  
		Size: 56.0 MB (56005478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb56dd30a9439c969b4e4698f93d1d6904887b24d016964a7c0857e306cbf507`  
		Last Modified: Sat, 04 Feb 2023 08:16:26 GMT  
		Size: 39.6 MB (39558401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0895a9cfae4403af4769bb7fc2334726c0db5a6929982d11aca84a6fd3b4247`  
		Last Modified: Sat, 04 Feb 2023 08:16:17 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b8ed21414ac18410d2cd7538e45767fefbf32a8719524c47f79dbb6481c58a9`  
		Last Modified: Sat, 04 Feb 2023 08:16:17 GMT  
		Size: 1.7 KB (1718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba129a165b264b065c4c64c28d541b80a301b07360486eeaaa32fffd058c8614`  
		Last Modified: Sat, 04 Feb 2023 08:16:17 GMT  
		Size: 1.5 KB (1479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d33029a943fe1a9b73a9717bc4636749407077422d7374aa4dddc3a99a9f97a7`  
		Last Modified: Sat, 04 Feb 2023 08:16:17 GMT  
		Size: 1.4 MB (1385416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:036ba73b7268a6aed37bd51a00d8c5ffd4f4a71eb03b0aa0e8ed0a6c0123bc82`  
		Last Modified: Sat, 04 Feb 2023 08:16:17 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1-standalone` - linux; mips64le

```console
$ docker pull adminer@sha256:0566934f328c80510fdb62adfc866aeb360712e6df9b0a27474a0ad53c6148a4
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.6 MB (92610528 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fcc732f3bac92ee347514fc3ed0501efa9c7a348b4e0c1d588c77787ddf8dbe4`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Thu, 09 Feb 2023 02:44:36 GMT
ADD file:0cc085dc00beb990e7bfcdd8b37dceccb8f6d62d7c5ce2d7e736cdf4d52ab799 in / 
# Thu, 09 Feb 2023 02:44:41 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 06:13:03 GMT
STOPSIGNAL SIGINT
# Thu, 09 Feb 2023 06:14:56 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 06:15:02 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Thu, 09 Feb 2023 06:15:09 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 09 Feb 2023 06:15:12 GMT
WORKDIR /var/www/html
# Thu, 09 Feb 2023 06:15:15 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 09 Feb 2023 06:15:18 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 09 Feb 2023 06:15:22 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 09 Feb 2023 06:15:25 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 09 Feb 2023 06:16:14 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 09 Feb 2023 06:16:17 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 09 Feb 2023 06:16:20 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 09 Feb 2023 06:16:23 GMT
USER adminer
# Thu, 09 Feb 2023 06:16:26 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Thu, 09 Feb 2023 06:16:30 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:11a4758105e306ed24134ddf12f4d813426845c37a0ab14cb71de94c2858f09c`  
		Last Modified: Thu, 09 Feb 2023 02:53:05 GMT  
		Size: 53.3 MB (53266784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7daca01da5691398087a3bfc7f953540cff885f22074e0129fda0d5e578a7a64`  
		Last Modified: Thu, 09 Feb 2023 06:19:06 GMT  
		Size: 38.0 MB (37953476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53cfc05716a9d1f679b734de3bff7a1b9714f5eb4b5040d6e143defb24f4975b`  
		Last Modified: Thu, 09 Feb 2023 06:18:37 GMT  
		Size: 395.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66588c07e295fc98922360681aab4fd6a5c85ca29e0d60b27a06b53038e89c06`  
		Last Modified: Thu, 09 Feb 2023 06:18:37 GMT  
		Size: 1.7 KB (1729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6920b4dc4d4b5e73a928683693ea3ec779eb5c2100896fcc49acbb46ca85198a`  
		Last Modified: Thu, 09 Feb 2023 06:18:37 GMT  
		Size: 1.5 KB (1479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a2bb1759b592851efa52aa0ae0243e97ddaee48fec421bde7daeb618542cca8`  
		Last Modified: Thu, 09 Feb 2023 06:18:38 GMT  
		Size: 1.4 MB (1386172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1a36c2a9b981a0b8491e075725805da77790fd3eb7a7b71f664ef3c369a2e14`  
		Last Modified: Thu, 09 Feb 2023 06:18:37 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1-standalone` - linux; ppc64le

```console
$ docker pull adminer@sha256:47a4ade05e65fa4596b6163d81cd7a4fa77513df4972a34167a78b55224b98d7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.2 MB (101226739 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d968381d4dcfc992e9ec7607ed161acc52925d93157eed9ed50bbc08830df809`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Sat, 04 Feb 2023 12:25:27 GMT
ADD file:724a2ac3b6190353442c93dce0ad4b3ab5c60144fc8204131767af6760e11980 in / 
# Sat, 04 Feb 2023 12:25:30 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 17:52:28 GMT
STOPSIGNAL SIGINT
# Sat, 04 Feb 2023 17:53:25 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 17:53:28 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Sat, 04 Feb 2023 17:53:31 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Sat, 04 Feb 2023 17:53:31 GMT
WORKDIR /var/www/html
# Sat, 04 Feb 2023 17:53:32 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Sat, 04 Feb 2023 17:53:32 GMT
ENV ADMINER_VERSION=4.8.1
# Sat, 04 Feb 2023 17:53:32 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Sat, 04 Feb 2023 17:53:33 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Sat, 04 Feb 2023 17:54:00 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 04 Feb 2023 17:54:00 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Sat, 04 Feb 2023 17:54:00 GMT
ENTRYPOINT ["entrypoint.sh"]
# Sat, 04 Feb 2023 17:54:01 GMT
USER adminer
# Sat, 04 Feb 2023 17:54:01 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Sat, 04 Feb 2023 17:54:02 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:c14c296a64e0f557b40f88759a913c28d0b28c646e5ec0cf0ceb49457156a792`  
		Last Modified: Sat, 04 Feb 2023 12:31:37 GMT  
		Size: 58.9 MB (58897064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2874c2bcc11a32eb3e38ad44035b5962c96846742a4307ba2c420da009e81ea7`  
		Last Modified: Sat, 04 Feb 2023 17:55:24 GMT  
		Size: 40.9 MB (40940112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dff9f9467cf09d7f5c242cfb1cacef36591219699095992b5738c1a88620f1d1`  
		Last Modified: Sat, 04 Feb 2023 17:55:09 GMT  
		Size: 394.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5c16d0da50d675218fc2a7373e45781eb595f8a795b902bcadf6be87ec0c887`  
		Last Modified: Sat, 04 Feb 2023 17:55:09 GMT  
		Size: 1.9 KB (1879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20dcb0d7c1b30e96ea63a399103c52c4292e83ce4579f47057d8dfe4d78b0aef`  
		Last Modified: Sat, 04 Feb 2023 17:55:09 GMT  
		Size: 1.5 KB (1478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3f8d644f4416950947c0acf3f7511db8085e591667b824d91224cec02554543`  
		Last Modified: Sat, 04 Feb 2023 17:55:09 GMT  
		Size: 1.4 MB (1385321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02759dcc9c00093b87b4c7129217d0bb02701ea0aa1e86f4d8f0eaf7a56723ab`  
		Last Modified: Sat, 04 Feb 2023 17:55:09 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1-standalone` - linux; s390x

```console
$ docker pull adminer@sha256:2719e0584d03780419167688eaba32d1ee3527400ff69f7f2cdd3db286a68aa8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.7 MB (93688213 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e9613c6a60d2d28ec14e33ed1f2f4b998316d21902a342ceca374a3b98116f1`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Thu, 09 Feb 2023 02:41:26 GMT
ADD file:952595f2a554945ef740fa7b1fbc617a9ce3e1c3b90ddf1e7c0ac6018e6a98f9 in / 
# Thu, 09 Feb 2023 02:41:30 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 07:18:54 GMT
STOPSIGNAL SIGINT
# Thu, 09 Feb 2023 07:20:03 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 07:20:13 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Thu, 09 Feb 2023 07:20:15 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 09 Feb 2023 07:20:16 GMT
WORKDIR /var/www/html
# Thu, 09 Feb 2023 07:20:17 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 09 Feb 2023 07:20:18 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 09 Feb 2023 07:20:19 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 09 Feb 2023 07:20:20 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 09 Feb 2023 07:20:29 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 09 Feb 2023 07:20:29 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 09 Feb 2023 07:20:29 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 09 Feb 2023 07:20:30 GMT
USER adminer
# Thu, 09 Feb 2023 07:20:30 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Thu, 09 Feb 2023 07:20:30 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:83809ebda0c421fc95029bc6775e0a0c1eba6916a58b115dcb6a14885dae2028`  
		Last Modified: Thu, 09 Feb 2023 02:45:46 GMT  
		Size: 53.3 MB (53278896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7e31cf57a38a02fa2d3f8ff53add4d422bd4ff62ec4b24e0831c6725cee4b77`  
		Last Modified: Thu, 09 Feb 2023 07:21:24 GMT  
		Size: 39.0 MB (39019658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0633cef61215983b712e699a77b2f0a05ae8e463a4b6c07ffa63d79c6d451f3`  
		Last Modified: Thu, 09 Feb 2023 07:21:18 GMT  
		Size: 394.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:827d0eb471d78ca9b876122dfaeddf3edb023c66c6efa92c4ec68f85e999114d`  
		Last Modified: Thu, 09 Feb 2023 07:21:18 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e6233ba1bdaa0fba57704d8dc153af1171478f4f644bcd1672d9a4fd9712ccb`  
		Last Modified: Thu, 09 Feb 2023 07:21:18 GMT  
		Size: 1.5 KB (1483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5eb9aee6c3e13c08694db2a9db11c9563576952794921b2cfa054236137c34ba`  
		Last Modified: Thu, 09 Feb 2023 07:21:18 GMT  
		Size: 1.4 MB (1385406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c778394cc4cf1727666c9cc60aec4329d57cae6761ed5d514b755368d165048`  
		Last Modified: Thu, 09 Feb 2023 07:21:18 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `adminer:fastcgi`

```console
$ docker pull adminer@sha256:7085d390109c63834cf471af0ddb9f6285d0002d0d2ee12424f8b50088fc9db2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `adminer:fastcgi` - linux; amd64

```console
$ docker pull adminer@sha256:a487a7e8be03bc50ec36d32b800c2a2a32ed6a5c238faca2dd38021b93b52991
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.9 MB (95904051 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64f86f40f9d98336b024a973361cd24981a21d3aba73369f77965c23e25186cf`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Sat, 04 Feb 2023 06:51:26 GMT
ADD file:cc6a56676703ec7ab5db8f2f7bc18a3169c0816d38703845b6b77ae5342ab41c in / 
# Sat, 04 Feb 2023 06:51:27 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 14:02:55 GMT
STOPSIGNAL SIGINT
# Sat, 04 Feb 2023 14:03:16 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 14:03:17 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Sat, 04 Feb 2023 14:03:36 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Sat, 04 Feb 2023 14:03:37 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Sat, 04 Feb 2023 14:03:37 GMT
WORKDIR /var/www/html
# Sat, 04 Feb 2023 14:03:37 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Sat, 04 Feb 2023 14:03:37 GMT
ENV ADMINER_VERSION=4.8.1
# Sat, 04 Feb 2023 14:03:37 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Sat, 04 Feb 2023 14:03:37 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Sat, 04 Feb 2023 14:03:48 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 04 Feb 2023 14:03:48 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Sat, 04 Feb 2023 14:03:49 GMT
ENTRYPOINT ["entrypoint.sh"]
# Sat, 04 Feb 2023 14:03:49 GMT
USER adminer
# Sat, 04 Feb 2023 14:03:49 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:699c8a97647f5789e5850bcf1a3d5afe9730edb654e1ae0714d5bd198a67a3ed`  
		Last Modified: Sat, 04 Feb 2023 06:55:53 GMT  
		Size: 55.0 MB (55025312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:154fe4cd65e5c30dd59093bd2c5edeb1d7892246dcb092564c35adb2dcc3f87b`  
		Last Modified: Sat, 04 Feb 2023 14:04:12 GMT  
		Size: 39.5 MB (39486607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:567f91a0a4b1cd6524fda2a63dd1948bf5fc7c699b172c4e9cb5986c1e5eceb7`  
		Last Modified: Sat, 04 Feb 2023 14:04:04 GMT  
		Size: 386.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43e065a08a3a44ef53db81a6b0ab94330ab02fd8a0d5c02758e2a9ccba2db806`  
		Last Modified: Sat, 04 Feb 2023 14:04:31 GMT  
		Size: 2.7 KB (2707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0154f5a2a5df6dc3e259a0da06081c740b1cc6974b3c6d2a763c82f68342132e`  
		Last Modified: Sat, 04 Feb 2023 14:04:31 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4af9bb043e0acb2d1b281a5d3f020e2437196040d7a09afda443537a7e3f3c40`  
		Last Modified: Sat, 04 Feb 2023 14:04:31 GMT  
		Size: 1.5 KB (1477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc585851cc1446d5ca0866b33d000cee9fcdac28a4c9d92bd803915ff149b87a`  
		Last Modified: Sat, 04 Feb 2023 14:04:31 GMT  
		Size: 1.4 MB (1385188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:345df3ed0a37be7be2ffe6d6abae3125fbfeb1a8624a4942368abf7585f2657a`  
		Last Modified: Sat, 04 Feb 2023 14:04:31 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:fastcgi` - linux; arm variant v5

```console
$ docker pull adminer@sha256:326ae96ad868945cc6ce21ae1125608876936e0a60b14764f309118e60ef3f11
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.2 MB (91191039 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12511271c61962718849cd85d462dfe90b30f31ec29c7600b97a3d1da83e8b1d`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Thu, 09 Feb 2023 02:00:16 GMT
ADD file:f5b31ee6dfb50a99818c1a4b3aba7c6ba1557b1547aa730e4230600017520691 in / 
# Thu, 09 Feb 2023 02:00:17 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 02:24:11 GMT
STOPSIGNAL SIGINT
# Thu, 09 Feb 2023 02:25:10 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 02:25:11 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Thu, 09 Feb 2023 02:25:39 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Thu, 09 Feb 2023 02:25:39 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 09 Feb 2023 02:25:40 GMT
WORKDIR /var/www/html
# Thu, 09 Feb 2023 02:25:40 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 09 Feb 2023 02:25:40 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 09 Feb 2023 02:25:40 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 09 Feb 2023 02:25:40 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 09 Feb 2023 02:25:56 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 09 Feb 2023 02:25:57 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 09 Feb 2023 02:25:57 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 09 Feb 2023 02:25:57 GMT
USER adminer
# Thu, 09 Feb 2023 02:25:57 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:f316396b5265978a8de9d493acdc7cda735a1fae190efbd5359650183ab7271f`  
		Last Modified: Thu, 09 Feb 2023 02:05:10 GMT  
		Size: 52.6 MB (52551796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0815a961482b87ff7ddc14fbf492d26b081ca226c383b265a39b9d900705a745`  
		Last Modified: Thu, 09 Feb 2023 02:26:40 GMT  
		Size: 37.2 MB (37247283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:907d5f9eb045277cd9fb22287b0e14b7fcd0ddcf52829c1e884706cae455c579`  
		Last Modified: Thu, 09 Feb 2023 02:26:30 GMT  
		Size: 393.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a3fe13d432c7dc589c9f54a560146f1249dfb75cf8f7169dfce8ac53c037021`  
		Last Modified: Thu, 09 Feb 2023 02:27:04 GMT  
		Size: 2.7 KB (2711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c23eca33f0e2498aefa42e88bcc0e47b715bdd1aae38f94434fb4ea6bdc0795e`  
		Last Modified: Thu, 09 Feb 2023 02:27:04 GMT  
		Size: 1.8 KB (1840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05f6bb9d806bbc982ab481b1906091f08c8ada35a23423c887544b3f135ac66f`  
		Last Modified: Thu, 09 Feb 2023 02:27:04 GMT  
		Size: 1.5 KB (1480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1c811cb2797199efbeb3147f223e01f6c28cee6d87b39a36fe8eb5347b987cd`  
		Last Modified: Thu, 09 Feb 2023 02:27:05 GMT  
		Size: 1.4 MB (1385045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6475dd585587079dec552c0910151d39ef0972f2f7ac63073ae5b67064c15ba3`  
		Last Modified: Thu, 09 Feb 2023 02:27:04 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:fastcgi` - linux; arm variant v7

```console
$ docker pull adminer@sha256:1745d08452780cad59501ee3c384e5cae58ab9f36b395347e4470f47f02f24ed
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.8 MB (87765580 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:004424ead9c2af6485083598520693d3cdc5f59da6283b4ccfc7424319280fc3`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Sat, 04 Feb 2023 09:59:19 GMT
ADD file:239b5255d05e0742f381f82fb7cd586fcc6d9a427263238a2be3372c494ae933 in / 
# Sat, 04 Feb 2023 09:59:20 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 10:43:54 GMT
STOPSIGNAL SIGINT
# Sat, 04 Feb 2023 10:44:19 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 10:44:20 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Sat, 04 Feb 2023 10:44:47 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Sat, 04 Feb 2023 10:44:47 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Sat, 04 Feb 2023 10:44:47 GMT
WORKDIR /var/www/html
# Sat, 04 Feb 2023 10:44:48 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Sat, 04 Feb 2023 10:44:48 GMT
ENV ADMINER_VERSION=4.8.1
# Sat, 04 Feb 2023 10:44:48 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Sat, 04 Feb 2023 10:44:48 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Sat, 04 Feb 2023 10:45:00 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 04 Feb 2023 10:45:00 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Sat, 04 Feb 2023 10:45:00 GMT
ENTRYPOINT ["entrypoint.sh"]
# Sat, 04 Feb 2023 10:45:01 GMT
USER adminer
# Sat, 04 Feb 2023 10:45:01 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:7a21a86b3957d8c99250334cfb78c55af4f8c9277f2f1d4abd53d0362f96323d`  
		Last Modified: Sat, 04 Feb 2023 10:05:53 GMT  
		Size: 50.2 MB (50190828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f647e4e293fd395af7ac8037948dbe3388c6cb6db3064a00c9f7b5ae32ba1bd1`  
		Last Modified: Sat, 04 Feb 2023 10:45:41 GMT  
		Size: 36.2 MB (36182796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc9bd65829db2cfa0c5e7daf2f0a09bc126930cc6f916496844b3e8adeb9d8ed`  
		Last Modified: Sat, 04 Feb 2023 10:45:31 GMT  
		Size: 394.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcec0a137102a4df6e8f3bae77f95cb2d0288be8d86aa062191a0994da6a09a1`  
		Last Modified: Sat, 04 Feb 2023 10:46:04 GMT  
		Size: 2.7 KB (2710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9366bc96b1ef426445bd576c64c5638c631fd82aeb0453f3871a82d91ecd0df1`  
		Last Modified: Sat, 04 Feb 2023 10:46:04 GMT  
		Size: 1.8 KB (1836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:459144f5a86bfff13a40970a73b497f8392eccdd9238e210b72ed37ace1dd2c8`  
		Last Modified: Sat, 04 Feb 2023 10:46:04 GMT  
		Size: 1.5 KB (1481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3a153a1f8dd4081e72343761ee75a8397e7809582b6a8d42a491dbc499b8719`  
		Last Modified: Sat, 04 Feb 2023 10:46:05 GMT  
		Size: 1.4 MB (1385045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc9fe3e24aab98148380a5d410c285619711932dcdcbe7cca25ee0aae77b4cb3`  
		Last Modified: Sat, 04 Feb 2023 10:46:04 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:fastcgi` - linux; arm64 variant v8

```console
$ docker pull adminer@sha256:14e5c9e9653cd354401e9d672d76e6462430024848ee435c02d0ff4332126317
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.3 MB (94316110 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0fa0825c1e857cf1eab6178105270bd008b049eb53696b1d94ed671c6284c846`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Sat, 04 Feb 2023 06:17:26 GMT
ADD file:c5a7c65d67685092faa3456c1a772550aa6d06ac07e1f98a95d39c31e304dbf8 in / 
# Sat, 04 Feb 2023 06:17:27 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 06:40:07 GMT
STOPSIGNAL SIGINT
# Sat, 04 Feb 2023 06:40:27 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 06:40:28 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Sat, 04 Feb 2023 06:40:47 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Sat, 04 Feb 2023 06:40:48 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Sat, 04 Feb 2023 06:40:48 GMT
WORKDIR /var/www/html
# Sat, 04 Feb 2023 06:40:48 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Sat, 04 Feb 2023 06:40:48 GMT
ENV ADMINER_VERSION=4.8.1
# Sat, 04 Feb 2023 06:40:48 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Sat, 04 Feb 2023 06:40:48 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Sat, 04 Feb 2023 06:40:57 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 04 Feb 2023 06:40:57 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Sat, 04 Feb 2023 06:40:58 GMT
ENTRYPOINT ["entrypoint.sh"]
# Sat, 04 Feb 2023 06:40:58 GMT
USER adminer
# Sat, 04 Feb 2023 06:40:58 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:fac7262b6510529638951e16807cf1758f42c892ed924e334c27bb8bbcf7d7c2`  
		Last Modified: Sat, 04 Feb 2023 06:21:01 GMT  
		Size: 53.7 MB (53681927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a3c4993b9ed6a78b02081f8b79138654baa646295eb90d0f09eb178f86f610b`  
		Last Modified: Sat, 04 Feb 2023 06:41:19 GMT  
		Size: 39.2 MB (39242179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77346147b34a65302ad6ba550d6ab4659b2d986cd2c2e57248651460e8a3e589`  
		Last Modified: Sat, 04 Feb 2023 06:41:12 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d66723d85a15a95d2bc016413f1fb69ae885d83e587a97d2043d370cf67e2db1`  
		Last Modified: Sat, 04 Feb 2023 06:41:36 GMT  
		Size: 2.7 KB (2707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7d226beb0ae597acd7e2647b0f4d4fc5227c69df6dff1165b4fe514cfad8130`  
		Last Modified: Sat, 04 Feb 2023 06:41:36 GMT  
		Size: 1.9 KB (1878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:def3ff5795d638c86eb1ce6b33aa5b7ac1991a913a5795be71a67c8f0bc1eab6`  
		Last Modified: Sat, 04 Feb 2023 06:41:36 GMT  
		Size: 1.5 KB (1476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:277a8bd87f658c231dabf9f7c494772cd03abace79d86737b913b73e89ee7bac`  
		Last Modified: Sat, 04 Feb 2023 06:41:37 GMT  
		Size: 1.4 MB (1385063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e95c557117dcc88c76c221f757a0f3404ad012a7726a260eadd4aba9b4e3341`  
		Last Modified: Sat, 04 Feb 2023 06:41:37 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:fastcgi` - linux; 386

```console
$ docker pull adminer@sha256:b0a3d3e0b21c7f00206ed8268c4dd0c6f085e410f729fb795bb885f8cac1098f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.0 MB (96956091 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9fa3646b337edc6af84c9cd6a950e859eaf4183842f124b5742da2f3495e257`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Sat, 04 Feb 2023 07:49:07 GMT
ADD file:d610d24eb19fe7e275924d58b6dad6b9f3dce21359a4ef81d04298e94382f102 in / 
# Sat, 04 Feb 2023 07:49:07 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 08:14:35 GMT
STOPSIGNAL SIGINT
# Sat, 04 Feb 2023 08:14:57 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 08:14:58 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Sat, 04 Feb 2023 08:15:27 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Sat, 04 Feb 2023 08:15:28 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Sat, 04 Feb 2023 08:15:29 GMT
WORKDIR /var/www/html
# Sat, 04 Feb 2023 08:15:31 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Sat, 04 Feb 2023 08:15:31 GMT
ENV ADMINER_VERSION=4.8.1
# Sat, 04 Feb 2023 08:15:32 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Sat, 04 Feb 2023 08:15:33 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Sat, 04 Feb 2023 08:15:45 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 04 Feb 2023 08:15:47 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Sat, 04 Feb 2023 08:15:47 GMT
ENTRYPOINT ["entrypoint.sh"]
# Sat, 04 Feb 2023 08:15:48 GMT
USER adminer
# Sat, 04 Feb 2023 08:15:49 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:082bfbf393a7a28cd82d531b1903cc5d788ac6af1b972045ad1d0deeff1aa6ab`  
		Last Modified: Sat, 04 Feb 2023 07:54:34 GMT  
		Size: 56.0 MB (56005478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb56dd30a9439c969b4e4698f93d1d6904887b24d016964a7c0857e306cbf507`  
		Last Modified: Sat, 04 Feb 2023 08:16:26 GMT  
		Size: 39.6 MB (39558401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0895a9cfae4403af4769bb7fc2334726c0db5a6929982d11aca84a6fd3b4247`  
		Last Modified: Sat, 04 Feb 2023 08:16:17 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fb386372d050d61199d8b69f8eba0503204b1435c14765dcc7391690f40e104`  
		Last Modified: Sat, 04 Feb 2023 08:16:47 GMT  
		Size: 2.7 KB (2709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92775617fc6814142b985df263b604974edc157e129229cd23234c9ea1e661e6`  
		Last Modified: Sat, 04 Feb 2023 08:16:47 GMT  
		Size: 1.7 KB (1714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f95cd3c9ca70db181013ee630ed1999515d90622129ffa1cffcb8610f0f456f7`  
		Last Modified: Sat, 04 Feb 2023 08:16:48 GMT  
		Size: 1.5 KB (1480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fe214dd6c4ba9b73bd44278fa41542b21e1144c6ff3ac53e197896801e87d48`  
		Last Modified: Sat, 04 Feb 2023 08:16:48 GMT  
		Size: 1.4 MB (1385428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:469bbb9c9519bc4c9fbd635879319fa1b6f74e4a9f271572fb23cbc31bcd739c`  
		Last Modified: Sat, 04 Feb 2023 08:16:47 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:fastcgi` - linux; mips64le

```console
$ docker pull adminer@sha256:d49eaa95df7a4b3b648e490d31d318b52533773169fecbc5a057d0012ea43a55
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.6 MB (92613258 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5cbd3305cd6fd59e4170383251a3e22ee9ca9c66bae9ba0b1914c9ffae1b23f6`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Thu, 09 Feb 2023 02:44:36 GMT
ADD file:0cc085dc00beb990e7bfcdd8b37dceccb8f6d62d7c5ce2d7e736cdf4d52ab799 in / 
# Thu, 09 Feb 2023 02:44:41 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 06:13:03 GMT
STOPSIGNAL SIGINT
# Thu, 09 Feb 2023 06:14:56 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 06:15:02 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Thu, 09 Feb 2023 06:16:50 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Thu, 09 Feb 2023 06:16:56 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 09 Feb 2023 06:16:59 GMT
WORKDIR /var/www/html
# Thu, 09 Feb 2023 06:17:02 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 09 Feb 2023 06:17:05 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 09 Feb 2023 06:17:08 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 09 Feb 2023 06:17:11 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 09 Feb 2023 06:17:59 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 09 Feb 2023 06:18:02 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 09 Feb 2023 06:18:05 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 09 Feb 2023 06:18:09 GMT
USER adminer
# Thu, 09 Feb 2023 06:18:12 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:11a4758105e306ed24134ddf12f4d813426845c37a0ab14cb71de94c2858f09c`  
		Last Modified: Thu, 09 Feb 2023 02:53:05 GMT  
		Size: 53.3 MB (53266784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7daca01da5691398087a3bfc7f953540cff885f22074e0129fda0d5e578a7a64`  
		Last Modified: Thu, 09 Feb 2023 06:19:06 GMT  
		Size: 38.0 MB (37953476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53cfc05716a9d1f679b734de3bff7a1b9714f5eb4b5040d6e143defb24f4975b`  
		Last Modified: Thu, 09 Feb 2023 06:18:37 GMT  
		Size: 395.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6df2d2de23d5a64cae787901af3f38fcaf86ab721824c7226d9bb8586ddba9fa`  
		Last Modified: Thu, 09 Feb 2023 06:19:25 GMT  
		Size: 2.7 KB (2714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f7734475a7c59ac576ed3322ac3274c2a727bb9a6c660381c515c9bf8ded7c0`  
		Last Modified: Thu, 09 Feb 2023 06:19:25 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b439c2c16da41627079e7dc7e3e2618e41b7ac3019f33d234ac6a50e1271e8c`  
		Last Modified: Thu, 09 Feb 2023 06:19:25 GMT  
		Size: 1.5 KB (1481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de57b503c9c79ca9d98a1575e8b2a2fec4f4f34a8184502f8a1697d783873671`  
		Last Modified: Thu, 09 Feb 2023 06:19:26 GMT  
		Size: 1.4 MB (1386183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27aac5c4950f7dd7352e76a2718d3c9d2974ba7ea1b383509d9a235534ccf422`  
		Last Modified: Thu, 09 Feb 2023 06:19:25 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:fastcgi` - linux; ppc64le

```console
$ docker pull adminer@sha256:4cbfd32fc3e0995849078137f63ac73353137c150f2af36869c97efcfd354baf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.2 MB (101229475 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6003343fd4014a739aa486639e78adf252f5a00a89aada720a7d97a43b19b920`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Sat, 04 Feb 2023 12:25:27 GMT
ADD file:724a2ac3b6190353442c93dce0ad4b3ab5c60144fc8204131767af6760e11980 in / 
# Sat, 04 Feb 2023 12:25:30 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 17:52:28 GMT
STOPSIGNAL SIGINT
# Sat, 04 Feb 2023 17:53:25 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 17:53:28 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Sat, 04 Feb 2023 17:54:10 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Sat, 04 Feb 2023 17:54:12 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Sat, 04 Feb 2023 17:54:12 GMT
WORKDIR /var/www/html
# Sat, 04 Feb 2023 17:54:13 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Sat, 04 Feb 2023 17:54:13 GMT
ENV ADMINER_VERSION=4.8.1
# Sat, 04 Feb 2023 17:54:14 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Sat, 04 Feb 2023 17:54:14 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Sat, 04 Feb 2023 17:54:37 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 04 Feb 2023 17:54:38 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Sat, 04 Feb 2023 17:54:38 GMT
ENTRYPOINT ["entrypoint.sh"]
# Sat, 04 Feb 2023 17:54:39 GMT
USER adminer
# Sat, 04 Feb 2023 17:54:39 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:c14c296a64e0f557b40f88759a913c28d0b28c646e5ec0cf0ceb49457156a792`  
		Last Modified: Sat, 04 Feb 2023 12:31:37 GMT  
		Size: 58.9 MB (58897064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2874c2bcc11a32eb3e38ad44035b5962c96846742a4307ba2c420da009e81ea7`  
		Last Modified: Sat, 04 Feb 2023 17:55:24 GMT  
		Size: 40.9 MB (40940112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dff9f9467cf09d7f5c242cfb1cacef36591219699095992b5738c1a88620f1d1`  
		Last Modified: Sat, 04 Feb 2023 17:55:09 GMT  
		Size: 394.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:268a861c77efb05e4765d3315e40b2b4a6eacb3bb56a931f6c7e4ac1b5d7a265`  
		Last Modified: Sat, 04 Feb 2023 17:55:49 GMT  
		Size: 2.7 KB (2713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d71f60a34a72995c8870893c023406f4337b9a7f557f7bd26fcd612bee6cce28`  
		Last Modified: Sat, 04 Feb 2023 17:55:49 GMT  
		Size: 1.9 KB (1875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d8ca4564d1e76d1b90184e8ab33c27849b4edd5735ea578f8c79dd312d99bfe`  
		Last Modified: Sat, 04 Feb 2023 17:55:49 GMT  
		Size: 1.5 KB (1479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f53ee83c5e9a3c93576c0b61fabdb84f2dbcb11a7a34d0f80a557d128e40db47`  
		Last Modified: Sat, 04 Feb 2023 17:55:50 GMT  
		Size: 1.4 MB (1385349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75395692fa85a6f6cd605c59de5987ad5629d3f4557722b950098cf11ff887ef`  
		Last Modified: Sat, 04 Feb 2023 17:55:49 GMT  
		Size: 489.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:fastcgi` - linux; s390x

```console
$ docker pull adminer@sha256:18930d5a14bb6b0eed4846e2b4a90aa9c731d4bde1eaf1abd60b51fe04453482
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.7 MB (93690838 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70050059db8c471d2394648f649f412ef6339c12ef4d0eeda7baa78c8bda768d`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Thu, 09 Feb 2023 02:41:26 GMT
ADD file:952595f2a554945ef740fa7b1fbc617a9ce3e1c3b90ddf1e7c0ac6018e6a98f9 in / 
# Thu, 09 Feb 2023 02:41:30 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 07:18:54 GMT
STOPSIGNAL SIGINT
# Thu, 09 Feb 2023 07:20:03 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 07:20:13 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Thu, 09 Feb 2023 07:20:43 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Thu, 09 Feb 2023 07:20:43 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 09 Feb 2023 07:20:43 GMT
WORKDIR /var/www/html
# Thu, 09 Feb 2023 07:20:44 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 09 Feb 2023 07:20:44 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 09 Feb 2023 07:20:44 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 09 Feb 2023 07:20:44 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 09 Feb 2023 07:20:52 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 09 Feb 2023 07:20:52 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 09 Feb 2023 07:20:52 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 09 Feb 2023 07:20:52 GMT
USER adminer
# Thu, 09 Feb 2023 07:20:52 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:83809ebda0c421fc95029bc6775e0a0c1eba6916a58b115dcb6a14885dae2028`  
		Last Modified: Thu, 09 Feb 2023 02:45:46 GMT  
		Size: 53.3 MB (53278896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7e31cf57a38a02fa2d3f8ff53add4d422bd4ff62ec4b24e0831c6725cee4b77`  
		Last Modified: Thu, 09 Feb 2023 07:21:24 GMT  
		Size: 39.0 MB (39019658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0633cef61215983b712e699a77b2f0a05ae8e463a4b6c07ffa63d79c6d451f3`  
		Last Modified: Thu, 09 Feb 2023 07:21:18 GMT  
		Size: 394.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c646918dad5e786008b8b31bc7f8cac9feb3521e1d4fbf6ba3c37c97bca49c6`  
		Last Modified: Thu, 09 Feb 2023 07:21:40 GMT  
		Size: 2.7 KB (2713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7c07b11a4865d90a2153a6c3e2e55161be6e83d2506f65db1ea5772aebd7219`  
		Last Modified: Thu, 09 Feb 2023 07:21:40 GMT  
		Size: 1.9 KB (1883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e13620c00e8614858376f34b19455eec2ec9325ff8082ea4407d7d72c6a4d268`  
		Last Modified: Thu, 09 Feb 2023 07:21:40 GMT  
		Size: 1.5 KB (1480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8900c81dcea2d296a964de4c28bca524bf07456b72f0cf57f0f50936cb7cf920`  
		Last Modified: Thu, 09 Feb 2023 07:21:40 GMT  
		Size: 1.4 MB (1385322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6632f7644ccabb5e6050f96cc7957a22e0bf86f0e5eff036f2a33254d3b34db`  
		Last Modified: Thu, 09 Feb 2023 07:21:40 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `adminer:latest`

```console
$ docker pull adminer@sha256:d4a361f0fdbc2f8a4732a62635e043e7a883e3785a54d54f5eb0d9ce3ad80204
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `adminer:latest` - linux; amd64

```console
$ docker pull adminer@sha256:8991350a6cc5acd8a607828617ad1cbd062b38528e6889664e0030b43f45d5f8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.9 MB (95901310 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:471e5d2fb746396a521960c56f7eafb8490e52be8cb499d4c0e00904c673be4e`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Sat, 04 Feb 2023 06:51:26 GMT
ADD file:cc6a56676703ec7ab5db8f2f7bc18a3169c0816d38703845b6b77ae5342ab41c in / 
# Sat, 04 Feb 2023 06:51:27 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 14:02:55 GMT
STOPSIGNAL SIGINT
# Sat, 04 Feb 2023 14:03:16 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 14:03:17 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Sat, 04 Feb 2023 14:03:17 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Sat, 04 Feb 2023 14:03:17 GMT
WORKDIR /var/www/html
# Sat, 04 Feb 2023 14:03:18 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Sat, 04 Feb 2023 14:03:18 GMT
ENV ADMINER_VERSION=4.8.1
# Sat, 04 Feb 2023 14:03:18 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Sat, 04 Feb 2023 14:03:18 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Sat, 04 Feb 2023 14:03:30 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 04 Feb 2023 14:03:30 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Sat, 04 Feb 2023 14:03:30 GMT
ENTRYPOINT ["entrypoint.sh"]
# Sat, 04 Feb 2023 14:03:30 GMT
USER adminer
# Sat, 04 Feb 2023 14:03:30 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Sat, 04 Feb 2023 14:03:30 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:699c8a97647f5789e5850bcf1a3d5afe9730edb654e1ae0714d5bd198a67a3ed`  
		Last Modified: Sat, 04 Feb 2023 06:55:53 GMT  
		Size: 55.0 MB (55025312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:154fe4cd65e5c30dd59093bd2c5edeb1d7892246dcb092564c35adb2dcc3f87b`  
		Last Modified: Sat, 04 Feb 2023 14:04:12 GMT  
		Size: 39.5 MB (39486607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:567f91a0a4b1cd6524fda2a63dd1948bf5fc7c699b172c4e9cb5986c1e5eceb7`  
		Last Modified: Sat, 04 Feb 2023 14:04:04 GMT  
		Size: 386.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce84d71503c32a8a86b5d886948c5d7d8138945998b4c31f05bfe35af0dbcd4b`  
		Last Modified: Sat, 04 Feb 2023 14:04:04 GMT  
		Size: 1.9 KB (1875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a11b9280fafb872c844c5dbff2fc246006a97a59897561411ce2c0d3676897f3`  
		Last Modified: Sat, 04 Feb 2023 14:04:04 GMT  
		Size: 1.5 KB (1477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e15d0e23848f1f6f5daf25c58fdf76a136a6dec252c28c3c1332250ad8e81c6`  
		Last Modified: Sat, 04 Feb 2023 14:04:04 GMT  
		Size: 1.4 MB (1385162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c610542bc6221747547117c74d457e30e7fce1c9394a494b2ee945e89f6faf3a`  
		Last Modified: Sat, 04 Feb 2023 14:04:04 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:latest` - linux; arm variant v5

```console
$ docker pull adminer@sha256:f41d812a0a97b02f761e994e55331571cbd685a2bfdeef007e9c8d098f61a58e
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.2 MB (91188340 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:937bc7e7afadd352160727b3edded381d4f7131ad46c77906131729950141670`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Thu, 09 Feb 2023 02:00:16 GMT
ADD file:f5b31ee6dfb50a99818c1a4b3aba7c6ba1557b1547aa730e4230600017520691 in / 
# Thu, 09 Feb 2023 02:00:17 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 02:24:11 GMT
STOPSIGNAL SIGINT
# Thu, 09 Feb 2023 02:25:10 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 02:25:11 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Thu, 09 Feb 2023 02:25:12 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 09 Feb 2023 02:25:12 GMT
WORKDIR /var/www/html
# Thu, 09 Feb 2023 02:25:13 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 09 Feb 2023 02:25:13 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 09 Feb 2023 02:25:13 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 09 Feb 2023 02:25:13 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 09 Feb 2023 02:25:29 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 09 Feb 2023 02:25:29 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 09 Feb 2023 02:25:29 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 09 Feb 2023 02:25:29 GMT
USER adminer
# Thu, 09 Feb 2023 02:25:29 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Thu, 09 Feb 2023 02:25:29 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:f316396b5265978a8de9d493acdc7cda735a1fae190efbd5359650183ab7271f`  
		Last Modified: Thu, 09 Feb 2023 02:05:10 GMT  
		Size: 52.6 MB (52551796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0815a961482b87ff7ddc14fbf492d26b081ca226c383b265a39b9d900705a745`  
		Last Modified: Thu, 09 Feb 2023 02:26:40 GMT  
		Size: 37.2 MB (37247283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:907d5f9eb045277cd9fb22287b0e14b7fcd0ddcf52829c1e884706cae455c579`  
		Last Modified: Thu, 09 Feb 2023 02:26:30 GMT  
		Size: 393.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8109ea45000a26ce9c558139872c68cc18839c5d9d58b6362bad0e61335be87`  
		Last Modified: Thu, 09 Feb 2023 02:26:30 GMT  
		Size: 1.8 KB (1840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de171f42adf643e4c74d58974916e2f121db8d111d838e580c9b53bed7875d54`  
		Last Modified: Thu, 09 Feb 2023 02:26:30 GMT  
		Size: 1.5 KB (1478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d391953776d5d50c308770e750f4b1df9f2041dcec59d1ea998f85fb7e012962`  
		Last Modified: Thu, 09 Feb 2023 02:26:30 GMT  
		Size: 1.4 MB (1385055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a563edb132e3a3c8e9654277a5136351be9d1d1582967ba0ada9e4772683912`  
		Last Modified: Thu, 09 Feb 2023 02:26:30 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:latest` - linux; arm variant v7

```console
$ docker pull adminer@sha256:9d12f8ae49e2b1ccac684b16522c130d56646a6c56fdcead2d1dbd5be32b71ea
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.8 MB (87762862 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe294facea4e18353cea22666d19efa67a350c0803293d20d943e0c6e97467b0`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Sat, 04 Feb 2023 09:59:19 GMT
ADD file:239b5255d05e0742f381f82fb7cd586fcc6d9a427263238a2be3372c494ae933 in / 
# Sat, 04 Feb 2023 09:59:20 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 10:43:54 GMT
STOPSIGNAL SIGINT
# Sat, 04 Feb 2023 10:44:19 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 10:44:20 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Sat, 04 Feb 2023 10:44:20 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Sat, 04 Feb 2023 10:44:20 GMT
WORKDIR /var/www/html
# Sat, 04 Feb 2023 10:44:20 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Sat, 04 Feb 2023 10:44:20 GMT
ENV ADMINER_VERSION=4.8.1
# Sat, 04 Feb 2023 10:44:21 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Sat, 04 Feb 2023 10:44:21 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Sat, 04 Feb 2023 10:44:33 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 04 Feb 2023 10:44:33 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Sat, 04 Feb 2023 10:44:33 GMT
ENTRYPOINT ["entrypoint.sh"]
# Sat, 04 Feb 2023 10:44:33 GMT
USER adminer
# Sat, 04 Feb 2023 10:44:34 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Sat, 04 Feb 2023 10:44:34 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:7a21a86b3957d8c99250334cfb78c55af4f8c9277f2f1d4abd53d0362f96323d`  
		Last Modified: Sat, 04 Feb 2023 10:05:53 GMT  
		Size: 50.2 MB (50190828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f647e4e293fd395af7ac8037948dbe3388c6cb6db3064a00c9f7b5ae32ba1bd1`  
		Last Modified: Sat, 04 Feb 2023 10:45:41 GMT  
		Size: 36.2 MB (36182796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc9bd65829db2cfa0c5e7daf2f0a09bc126930cc6f916496844b3e8adeb9d8ed`  
		Last Modified: Sat, 04 Feb 2023 10:45:31 GMT  
		Size: 394.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ca053278ba99e9e29b58a59e0d4e18b6a12ae83036d127f90aeed075f61139c`  
		Last Modified: Sat, 04 Feb 2023 10:45:31 GMT  
		Size: 1.8 KB (1835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:212108f5743ed386440da376a9d15e10b2349f1a1573187b747a06ea2d32abc6`  
		Last Modified: Sat, 04 Feb 2023 10:45:31 GMT  
		Size: 1.5 KB (1477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9c4b14fe58151d7c0bc6589d5264310b8afa5674ec2f3a675e5c524a8eb12df`  
		Last Modified: Sat, 04 Feb 2023 10:45:32 GMT  
		Size: 1.4 MB (1385040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5305f0630fde46637c4b273861b8dc1fd8735642c1290f7d39e3f62c58452f35`  
		Last Modified: Sat, 04 Feb 2023 10:45:31 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:latest` - linux; arm64 variant v8

```console
$ docker pull adminer@sha256:4f5db61ed6cff7c4d001092c5ce6d5eb7501a356739d77657c28f6b813d428c2
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.3 MB (94313416 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f55903b78a43635b55478abb38f63cd77f3e0ec223947f72aee5c6872a07ffd1`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Sat, 04 Feb 2023 06:17:26 GMT
ADD file:c5a7c65d67685092faa3456c1a772550aa6d06ac07e1f98a95d39c31e304dbf8 in / 
# Sat, 04 Feb 2023 06:17:27 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 06:40:07 GMT
STOPSIGNAL SIGINT
# Sat, 04 Feb 2023 06:40:27 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 06:40:28 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Sat, 04 Feb 2023 06:40:29 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Sat, 04 Feb 2023 06:40:29 GMT
WORKDIR /var/www/html
# Sat, 04 Feb 2023 06:40:29 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Sat, 04 Feb 2023 06:40:29 GMT
ENV ADMINER_VERSION=4.8.1
# Sat, 04 Feb 2023 06:40:29 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Sat, 04 Feb 2023 06:40:29 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Sat, 04 Feb 2023 06:40:39 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 04 Feb 2023 06:40:39 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Sat, 04 Feb 2023 06:40:39 GMT
ENTRYPOINT ["entrypoint.sh"]
# Sat, 04 Feb 2023 06:40:40 GMT
USER adminer
# Sat, 04 Feb 2023 06:40:40 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Sat, 04 Feb 2023 06:40:40 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:fac7262b6510529638951e16807cf1758f42c892ed924e334c27bb8bbcf7d7c2`  
		Last Modified: Sat, 04 Feb 2023 06:21:01 GMT  
		Size: 53.7 MB (53681927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a3c4993b9ed6a78b02081f8b79138654baa646295eb90d0f09eb178f86f610b`  
		Last Modified: Sat, 04 Feb 2023 06:41:19 GMT  
		Size: 39.2 MB (39242179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77346147b34a65302ad6ba550d6ab4659b2d986cd2c2e57248651460e8a3e589`  
		Last Modified: Sat, 04 Feb 2023 06:41:12 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56563dd7963c36713d65f09a5387503374566d7296c2bfa4422bf2d3ceb3bbeb`  
		Last Modified: Sat, 04 Feb 2023 06:41:12 GMT  
		Size: 1.9 KB (1879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fa2e6ff1278f9c9246cfedeee571a41de27494a6f3d518f136dbb8a225d7d33`  
		Last Modified: Sat, 04 Feb 2023 06:41:12 GMT  
		Size: 1.5 KB (1481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f24f727f464d597cc5ae7abb0b697c3807940cf0cca55089c3cbc553eee16523`  
		Last Modified: Sat, 04 Feb 2023 06:41:12 GMT  
		Size: 1.4 MB (1385069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:717c6895aefe53599660cfa578fea33535395f3479fdaecb0f2db55b2fa1165a`  
		Last Modified: Sat, 04 Feb 2023 06:41:12 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:latest` - linux; 386

```console
$ docker pull adminer@sha256:9aeaa40748b7ce615a50ef6b58624bde25df408d8e05367d32f939a9ebac3a1d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.0 MB (96953374 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0059247fefe0e30e3270aaad4163ba4bfc56aa80f66364c27054b4f9bd7ef47`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Sat, 04 Feb 2023 07:49:07 GMT
ADD file:d610d24eb19fe7e275924d58b6dad6b9f3dce21359a4ef81d04298e94382f102 in / 
# Sat, 04 Feb 2023 07:49:07 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 08:14:35 GMT
STOPSIGNAL SIGINT
# Sat, 04 Feb 2023 08:14:57 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 08:14:58 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Sat, 04 Feb 2023 08:14:59 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Sat, 04 Feb 2023 08:14:59 GMT
WORKDIR /var/www/html
# Sat, 04 Feb 2023 08:15:01 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Sat, 04 Feb 2023 08:15:01 GMT
ENV ADMINER_VERSION=4.8.1
# Sat, 04 Feb 2023 08:15:02 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Sat, 04 Feb 2023 08:15:03 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Sat, 04 Feb 2023 08:15:16 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 04 Feb 2023 08:15:17 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Sat, 04 Feb 2023 08:15:17 GMT
ENTRYPOINT ["entrypoint.sh"]
# Sat, 04 Feb 2023 08:15:18 GMT
USER adminer
# Sat, 04 Feb 2023 08:15:19 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Sat, 04 Feb 2023 08:15:20 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:082bfbf393a7a28cd82d531b1903cc5d788ac6af1b972045ad1d0deeff1aa6ab`  
		Last Modified: Sat, 04 Feb 2023 07:54:34 GMT  
		Size: 56.0 MB (56005478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb56dd30a9439c969b4e4698f93d1d6904887b24d016964a7c0857e306cbf507`  
		Last Modified: Sat, 04 Feb 2023 08:16:26 GMT  
		Size: 39.6 MB (39558401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0895a9cfae4403af4769bb7fc2334726c0db5a6929982d11aca84a6fd3b4247`  
		Last Modified: Sat, 04 Feb 2023 08:16:17 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b8ed21414ac18410d2cd7538e45767fefbf32a8719524c47f79dbb6481c58a9`  
		Last Modified: Sat, 04 Feb 2023 08:16:17 GMT  
		Size: 1.7 KB (1718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba129a165b264b065c4c64c28d541b80a301b07360486eeaaa32fffd058c8614`  
		Last Modified: Sat, 04 Feb 2023 08:16:17 GMT  
		Size: 1.5 KB (1479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d33029a943fe1a9b73a9717bc4636749407077422d7374aa4dddc3a99a9f97a7`  
		Last Modified: Sat, 04 Feb 2023 08:16:17 GMT  
		Size: 1.4 MB (1385416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:036ba73b7268a6aed37bd51a00d8c5ffd4f4a71eb03b0aa0e8ed0a6c0123bc82`  
		Last Modified: Sat, 04 Feb 2023 08:16:17 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:latest` - linux; mips64le

```console
$ docker pull adminer@sha256:0566934f328c80510fdb62adfc866aeb360712e6df9b0a27474a0ad53c6148a4
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.6 MB (92610528 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fcc732f3bac92ee347514fc3ed0501efa9c7a348b4e0c1d588c77787ddf8dbe4`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Thu, 09 Feb 2023 02:44:36 GMT
ADD file:0cc085dc00beb990e7bfcdd8b37dceccb8f6d62d7c5ce2d7e736cdf4d52ab799 in / 
# Thu, 09 Feb 2023 02:44:41 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 06:13:03 GMT
STOPSIGNAL SIGINT
# Thu, 09 Feb 2023 06:14:56 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 06:15:02 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Thu, 09 Feb 2023 06:15:09 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 09 Feb 2023 06:15:12 GMT
WORKDIR /var/www/html
# Thu, 09 Feb 2023 06:15:15 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 09 Feb 2023 06:15:18 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 09 Feb 2023 06:15:22 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 09 Feb 2023 06:15:25 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 09 Feb 2023 06:16:14 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 09 Feb 2023 06:16:17 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 09 Feb 2023 06:16:20 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 09 Feb 2023 06:16:23 GMT
USER adminer
# Thu, 09 Feb 2023 06:16:26 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Thu, 09 Feb 2023 06:16:30 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:11a4758105e306ed24134ddf12f4d813426845c37a0ab14cb71de94c2858f09c`  
		Last Modified: Thu, 09 Feb 2023 02:53:05 GMT  
		Size: 53.3 MB (53266784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7daca01da5691398087a3bfc7f953540cff885f22074e0129fda0d5e578a7a64`  
		Last Modified: Thu, 09 Feb 2023 06:19:06 GMT  
		Size: 38.0 MB (37953476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53cfc05716a9d1f679b734de3bff7a1b9714f5eb4b5040d6e143defb24f4975b`  
		Last Modified: Thu, 09 Feb 2023 06:18:37 GMT  
		Size: 395.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66588c07e295fc98922360681aab4fd6a5c85ca29e0d60b27a06b53038e89c06`  
		Last Modified: Thu, 09 Feb 2023 06:18:37 GMT  
		Size: 1.7 KB (1729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6920b4dc4d4b5e73a928683693ea3ec779eb5c2100896fcc49acbb46ca85198a`  
		Last Modified: Thu, 09 Feb 2023 06:18:37 GMT  
		Size: 1.5 KB (1479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a2bb1759b592851efa52aa0ae0243e97ddaee48fec421bde7daeb618542cca8`  
		Last Modified: Thu, 09 Feb 2023 06:18:38 GMT  
		Size: 1.4 MB (1386172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1a36c2a9b981a0b8491e075725805da77790fd3eb7a7b71f664ef3c369a2e14`  
		Last Modified: Thu, 09 Feb 2023 06:18:37 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:latest` - linux; ppc64le

```console
$ docker pull adminer@sha256:47a4ade05e65fa4596b6163d81cd7a4fa77513df4972a34167a78b55224b98d7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.2 MB (101226739 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d968381d4dcfc992e9ec7607ed161acc52925d93157eed9ed50bbc08830df809`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Sat, 04 Feb 2023 12:25:27 GMT
ADD file:724a2ac3b6190353442c93dce0ad4b3ab5c60144fc8204131767af6760e11980 in / 
# Sat, 04 Feb 2023 12:25:30 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 17:52:28 GMT
STOPSIGNAL SIGINT
# Sat, 04 Feb 2023 17:53:25 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 17:53:28 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Sat, 04 Feb 2023 17:53:31 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Sat, 04 Feb 2023 17:53:31 GMT
WORKDIR /var/www/html
# Sat, 04 Feb 2023 17:53:32 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Sat, 04 Feb 2023 17:53:32 GMT
ENV ADMINER_VERSION=4.8.1
# Sat, 04 Feb 2023 17:53:32 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Sat, 04 Feb 2023 17:53:33 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Sat, 04 Feb 2023 17:54:00 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 04 Feb 2023 17:54:00 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Sat, 04 Feb 2023 17:54:00 GMT
ENTRYPOINT ["entrypoint.sh"]
# Sat, 04 Feb 2023 17:54:01 GMT
USER adminer
# Sat, 04 Feb 2023 17:54:01 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Sat, 04 Feb 2023 17:54:02 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:c14c296a64e0f557b40f88759a913c28d0b28c646e5ec0cf0ceb49457156a792`  
		Last Modified: Sat, 04 Feb 2023 12:31:37 GMT  
		Size: 58.9 MB (58897064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2874c2bcc11a32eb3e38ad44035b5962c96846742a4307ba2c420da009e81ea7`  
		Last Modified: Sat, 04 Feb 2023 17:55:24 GMT  
		Size: 40.9 MB (40940112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dff9f9467cf09d7f5c242cfb1cacef36591219699095992b5738c1a88620f1d1`  
		Last Modified: Sat, 04 Feb 2023 17:55:09 GMT  
		Size: 394.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5c16d0da50d675218fc2a7373e45781eb595f8a795b902bcadf6be87ec0c887`  
		Last Modified: Sat, 04 Feb 2023 17:55:09 GMT  
		Size: 1.9 KB (1879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20dcb0d7c1b30e96ea63a399103c52c4292e83ce4579f47057d8dfe4d78b0aef`  
		Last Modified: Sat, 04 Feb 2023 17:55:09 GMT  
		Size: 1.5 KB (1478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3f8d644f4416950947c0acf3f7511db8085e591667b824d91224cec02554543`  
		Last Modified: Sat, 04 Feb 2023 17:55:09 GMT  
		Size: 1.4 MB (1385321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02759dcc9c00093b87b4c7129217d0bb02701ea0aa1e86f4d8f0eaf7a56723ab`  
		Last Modified: Sat, 04 Feb 2023 17:55:09 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:latest` - linux; s390x

```console
$ docker pull adminer@sha256:2719e0584d03780419167688eaba32d1ee3527400ff69f7f2cdd3db286a68aa8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.7 MB (93688213 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e9613c6a60d2d28ec14e33ed1f2f4b998316d21902a342ceca374a3b98116f1`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Thu, 09 Feb 2023 02:41:26 GMT
ADD file:952595f2a554945ef740fa7b1fbc617a9ce3e1c3b90ddf1e7c0ac6018e6a98f9 in / 
# Thu, 09 Feb 2023 02:41:30 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 07:18:54 GMT
STOPSIGNAL SIGINT
# Thu, 09 Feb 2023 07:20:03 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 07:20:13 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Thu, 09 Feb 2023 07:20:15 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 09 Feb 2023 07:20:16 GMT
WORKDIR /var/www/html
# Thu, 09 Feb 2023 07:20:17 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 09 Feb 2023 07:20:18 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 09 Feb 2023 07:20:19 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 09 Feb 2023 07:20:20 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 09 Feb 2023 07:20:29 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 09 Feb 2023 07:20:29 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 09 Feb 2023 07:20:29 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 09 Feb 2023 07:20:30 GMT
USER adminer
# Thu, 09 Feb 2023 07:20:30 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Thu, 09 Feb 2023 07:20:30 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:83809ebda0c421fc95029bc6775e0a0c1eba6916a58b115dcb6a14885dae2028`  
		Last Modified: Thu, 09 Feb 2023 02:45:46 GMT  
		Size: 53.3 MB (53278896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7e31cf57a38a02fa2d3f8ff53add4d422bd4ff62ec4b24e0831c6725cee4b77`  
		Last Modified: Thu, 09 Feb 2023 07:21:24 GMT  
		Size: 39.0 MB (39019658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0633cef61215983b712e699a77b2f0a05ae8e463a4b6c07ffa63d79c6d451f3`  
		Last Modified: Thu, 09 Feb 2023 07:21:18 GMT  
		Size: 394.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:827d0eb471d78ca9b876122dfaeddf3edb023c66c6efa92c4ec68f85e999114d`  
		Last Modified: Thu, 09 Feb 2023 07:21:18 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e6233ba1bdaa0fba57704d8dc153af1171478f4f644bcd1672d9a4fd9712ccb`  
		Last Modified: Thu, 09 Feb 2023 07:21:18 GMT  
		Size: 1.5 KB (1483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5eb9aee6c3e13c08694db2a9db11c9563576952794921b2cfa054236137c34ba`  
		Last Modified: Thu, 09 Feb 2023 07:21:18 GMT  
		Size: 1.4 MB (1385406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c778394cc4cf1727666c9cc60aec4329d57cae6761ed5d514b755368d165048`  
		Last Modified: Thu, 09 Feb 2023 07:21:18 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `adminer:standalone`

```console
$ docker pull adminer@sha256:d4a361f0fdbc2f8a4732a62635e043e7a883e3785a54d54f5eb0d9ce3ad80204
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `adminer:standalone` - linux; amd64

```console
$ docker pull adminer@sha256:8991350a6cc5acd8a607828617ad1cbd062b38528e6889664e0030b43f45d5f8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.9 MB (95901310 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:471e5d2fb746396a521960c56f7eafb8490e52be8cb499d4c0e00904c673be4e`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Sat, 04 Feb 2023 06:51:26 GMT
ADD file:cc6a56676703ec7ab5db8f2f7bc18a3169c0816d38703845b6b77ae5342ab41c in / 
# Sat, 04 Feb 2023 06:51:27 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 14:02:55 GMT
STOPSIGNAL SIGINT
# Sat, 04 Feb 2023 14:03:16 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 14:03:17 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Sat, 04 Feb 2023 14:03:17 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Sat, 04 Feb 2023 14:03:17 GMT
WORKDIR /var/www/html
# Sat, 04 Feb 2023 14:03:18 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Sat, 04 Feb 2023 14:03:18 GMT
ENV ADMINER_VERSION=4.8.1
# Sat, 04 Feb 2023 14:03:18 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Sat, 04 Feb 2023 14:03:18 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Sat, 04 Feb 2023 14:03:30 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 04 Feb 2023 14:03:30 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Sat, 04 Feb 2023 14:03:30 GMT
ENTRYPOINT ["entrypoint.sh"]
# Sat, 04 Feb 2023 14:03:30 GMT
USER adminer
# Sat, 04 Feb 2023 14:03:30 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Sat, 04 Feb 2023 14:03:30 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:699c8a97647f5789e5850bcf1a3d5afe9730edb654e1ae0714d5bd198a67a3ed`  
		Last Modified: Sat, 04 Feb 2023 06:55:53 GMT  
		Size: 55.0 MB (55025312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:154fe4cd65e5c30dd59093bd2c5edeb1d7892246dcb092564c35adb2dcc3f87b`  
		Last Modified: Sat, 04 Feb 2023 14:04:12 GMT  
		Size: 39.5 MB (39486607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:567f91a0a4b1cd6524fda2a63dd1948bf5fc7c699b172c4e9cb5986c1e5eceb7`  
		Last Modified: Sat, 04 Feb 2023 14:04:04 GMT  
		Size: 386.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce84d71503c32a8a86b5d886948c5d7d8138945998b4c31f05bfe35af0dbcd4b`  
		Last Modified: Sat, 04 Feb 2023 14:04:04 GMT  
		Size: 1.9 KB (1875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a11b9280fafb872c844c5dbff2fc246006a97a59897561411ce2c0d3676897f3`  
		Last Modified: Sat, 04 Feb 2023 14:04:04 GMT  
		Size: 1.5 KB (1477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e15d0e23848f1f6f5daf25c58fdf76a136a6dec252c28c3c1332250ad8e81c6`  
		Last Modified: Sat, 04 Feb 2023 14:04:04 GMT  
		Size: 1.4 MB (1385162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c610542bc6221747547117c74d457e30e7fce1c9394a494b2ee945e89f6faf3a`  
		Last Modified: Sat, 04 Feb 2023 14:04:04 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:standalone` - linux; arm variant v5

```console
$ docker pull adminer@sha256:f41d812a0a97b02f761e994e55331571cbd685a2bfdeef007e9c8d098f61a58e
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.2 MB (91188340 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:937bc7e7afadd352160727b3edded381d4f7131ad46c77906131729950141670`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Thu, 09 Feb 2023 02:00:16 GMT
ADD file:f5b31ee6dfb50a99818c1a4b3aba7c6ba1557b1547aa730e4230600017520691 in / 
# Thu, 09 Feb 2023 02:00:17 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 02:24:11 GMT
STOPSIGNAL SIGINT
# Thu, 09 Feb 2023 02:25:10 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 02:25:11 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Thu, 09 Feb 2023 02:25:12 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 09 Feb 2023 02:25:12 GMT
WORKDIR /var/www/html
# Thu, 09 Feb 2023 02:25:13 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 09 Feb 2023 02:25:13 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 09 Feb 2023 02:25:13 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 09 Feb 2023 02:25:13 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 09 Feb 2023 02:25:29 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 09 Feb 2023 02:25:29 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 09 Feb 2023 02:25:29 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 09 Feb 2023 02:25:29 GMT
USER adminer
# Thu, 09 Feb 2023 02:25:29 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Thu, 09 Feb 2023 02:25:29 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:f316396b5265978a8de9d493acdc7cda735a1fae190efbd5359650183ab7271f`  
		Last Modified: Thu, 09 Feb 2023 02:05:10 GMT  
		Size: 52.6 MB (52551796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0815a961482b87ff7ddc14fbf492d26b081ca226c383b265a39b9d900705a745`  
		Last Modified: Thu, 09 Feb 2023 02:26:40 GMT  
		Size: 37.2 MB (37247283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:907d5f9eb045277cd9fb22287b0e14b7fcd0ddcf52829c1e884706cae455c579`  
		Last Modified: Thu, 09 Feb 2023 02:26:30 GMT  
		Size: 393.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8109ea45000a26ce9c558139872c68cc18839c5d9d58b6362bad0e61335be87`  
		Last Modified: Thu, 09 Feb 2023 02:26:30 GMT  
		Size: 1.8 KB (1840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de171f42adf643e4c74d58974916e2f121db8d111d838e580c9b53bed7875d54`  
		Last Modified: Thu, 09 Feb 2023 02:26:30 GMT  
		Size: 1.5 KB (1478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d391953776d5d50c308770e750f4b1df9f2041dcec59d1ea998f85fb7e012962`  
		Last Modified: Thu, 09 Feb 2023 02:26:30 GMT  
		Size: 1.4 MB (1385055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a563edb132e3a3c8e9654277a5136351be9d1d1582967ba0ada9e4772683912`  
		Last Modified: Thu, 09 Feb 2023 02:26:30 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:standalone` - linux; arm variant v7

```console
$ docker pull adminer@sha256:9d12f8ae49e2b1ccac684b16522c130d56646a6c56fdcead2d1dbd5be32b71ea
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.8 MB (87762862 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe294facea4e18353cea22666d19efa67a350c0803293d20d943e0c6e97467b0`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Sat, 04 Feb 2023 09:59:19 GMT
ADD file:239b5255d05e0742f381f82fb7cd586fcc6d9a427263238a2be3372c494ae933 in / 
# Sat, 04 Feb 2023 09:59:20 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 10:43:54 GMT
STOPSIGNAL SIGINT
# Sat, 04 Feb 2023 10:44:19 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 10:44:20 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Sat, 04 Feb 2023 10:44:20 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Sat, 04 Feb 2023 10:44:20 GMT
WORKDIR /var/www/html
# Sat, 04 Feb 2023 10:44:20 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Sat, 04 Feb 2023 10:44:20 GMT
ENV ADMINER_VERSION=4.8.1
# Sat, 04 Feb 2023 10:44:21 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Sat, 04 Feb 2023 10:44:21 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Sat, 04 Feb 2023 10:44:33 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 04 Feb 2023 10:44:33 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Sat, 04 Feb 2023 10:44:33 GMT
ENTRYPOINT ["entrypoint.sh"]
# Sat, 04 Feb 2023 10:44:33 GMT
USER adminer
# Sat, 04 Feb 2023 10:44:34 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Sat, 04 Feb 2023 10:44:34 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:7a21a86b3957d8c99250334cfb78c55af4f8c9277f2f1d4abd53d0362f96323d`  
		Last Modified: Sat, 04 Feb 2023 10:05:53 GMT  
		Size: 50.2 MB (50190828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f647e4e293fd395af7ac8037948dbe3388c6cb6db3064a00c9f7b5ae32ba1bd1`  
		Last Modified: Sat, 04 Feb 2023 10:45:41 GMT  
		Size: 36.2 MB (36182796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc9bd65829db2cfa0c5e7daf2f0a09bc126930cc6f916496844b3e8adeb9d8ed`  
		Last Modified: Sat, 04 Feb 2023 10:45:31 GMT  
		Size: 394.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ca053278ba99e9e29b58a59e0d4e18b6a12ae83036d127f90aeed075f61139c`  
		Last Modified: Sat, 04 Feb 2023 10:45:31 GMT  
		Size: 1.8 KB (1835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:212108f5743ed386440da376a9d15e10b2349f1a1573187b747a06ea2d32abc6`  
		Last Modified: Sat, 04 Feb 2023 10:45:31 GMT  
		Size: 1.5 KB (1477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9c4b14fe58151d7c0bc6589d5264310b8afa5674ec2f3a675e5c524a8eb12df`  
		Last Modified: Sat, 04 Feb 2023 10:45:32 GMT  
		Size: 1.4 MB (1385040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5305f0630fde46637c4b273861b8dc1fd8735642c1290f7d39e3f62c58452f35`  
		Last Modified: Sat, 04 Feb 2023 10:45:31 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:standalone` - linux; arm64 variant v8

```console
$ docker pull adminer@sha256:4f5db61ed6cff7c4d001092c5ce6d5eb7501a356739d77657c28f6b813d428c2
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.3 MB (94313416 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f55903b78a43635b55478abb38f63cd77f3e0ec223947f72aee5c6872a07ffd1`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Sat, 04 Feb 2023 06:17:26 GMT
ADD file:c5a7c65d67685092faa3456c1a772550aa6d06ac07e1f98a95d39c31e304dbf8 in / 
# Sat, 04 Feb 2023 06:17:27 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 06:40:07 GMT
STOPSIGNAL SIGINT
# Sat, 04 Feb 2023 06:40:27 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 06:40:28 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Sat, 04 Feb 2023 06:40:29 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Sat, 04 Feb 2023 06:40:29 GMT
WORKDIR /var/www/html
# Sat, 04 Feb 2023 06:40:29 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Sat, 04 Feb 2023 06:40:29 GMT
ENV ADMINER_VERSION=4.8.1
# Sat, 04 Feb 2023 06:40:29 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Sat, 04 Feb 2023 06:40:29 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Sat, 04 Feb 2023 06:40:39 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 04 Feb 2023 06:40:39 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Sat, 04 Feb 2023 06:40:39 GMT
ENTRYPOINT ["entrypoint.sh"]
# Sat, 04 Feb 2023 06:40:40 GMT
USER adminer
# Sat, 04 Feb 2023 06:40:40 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Sat, 04 Feb 2023 06:40:40 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:fac7262b6510529638951e16807cf1758f42c892ed924e334c27bb8bbcf7d7c2`  
		Last Modified: Sat, 04 Feb 2023 06:21:01 GMT  
		Size: 53.7 MB (53681927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a3c4993b9ed6a78b02081f8b79138654baa646295eb90d0f09eb178f86f610b`  
		Last Modified: Sat, 04 Feb 2023 06:41:19 GMT  
		Size: 39.2 MB (39242179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77346147b34a65302ad6ba550d6ab4659b2d986cd2c2e57248651460e8a3e589`  
		Last Modified: Sat, 04 Feb 2023 06:41:12 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56563dd7963c36713d65f09a5387503374566d7296c2bfa4422bf2d3ceb3bbeb`  
		Last Modified: Sat, 04 Feb 2023 06:41:12 GMT  
		Size: 1.9 KB (1879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fa2e6ff1278f9c9246cfedeee571a41de27494a6f3d518f136dbb8a225d7d33`  
		Last Modified: Sat, 04 Feb 2023 06:41:12 GMT  
		Size: 1.5 KB (1481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f24f727f464d597cc5ae7abb0b697c3807940cf0cca55089c3cbc553eee16523`  
		Last Modified: Sat, 04 Feb 2023 06:41:12 GMT  
		Size: 1.4 MB (1385069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:717c6895aefe53599660cfa578fea33535395f3479fdaecb0f2db55b2fa1165a`  
		Last Modified: Sat, 04 Feb 2023 06:41:12 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:standalone` - linux; 386

```console
$ docker pull adminer@sha256:9aeaa40748b7ce615a50ef6b58624bde25df408d8e05367d32f939a9ebac3a1d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.0 MB (96953374 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0059247fefe0e30e3270aaad4163ba4bfc56aa80f66364c27054b4f9bd7ef47`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Sat, 04 Feb 2023 07:49:07 GMT
ADD file:d610d24eb19fe7e275924d58b6dad6b9f3dce21359a4ef81d04298e94382f102 in / 
# Sat, 04 Feb 2023 07:49:07 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 08:14:35 GMT
STOPSIGNAL SIGINT
# Sat, 04 Feb 2023 08:14:57 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 08:14:58 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Sat, 04 Feb 2023 08:14:59 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Sat, 04 Feb 2023 08:14:59 GMT
WORKDIR /var/www/html
# Sat, 04 Feb 2023 08:15:01 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Sat, 04 Feb 2023 08:15:01 GMT
ENV ADMINER_VERSION=4.8.1
# Sat, 04 Feb 2023 08:15:02 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Sat, 04 Feb 2023 08:15:03 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Sat, 04 Feb 2023 08:15:16 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 04 Feb 2023 08:15:17 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Sat, 04 Feb 2023 08:15:17 GMT
ENTRYPOINT ["entrypoint.sh"]
# Sat, 04 Feb 2023 08:15:18 GMT
USER adminer
# Sat, 04 Feb 2023 08:15:19 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Sat, 04 Feb 2023 08:15:20 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:082bfbf393a7a28cd82d531b1903cc5d788ac6af1b972045ad1d0deeff1aa6ab`  
		Last Modified: Sat, 04 Feb 2023 07:54:34 GMT  
		Size: 56.0 MB (56005478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb56dd30a9439c969b4e4698f93d1d6904887b24d016964a7c0857e306cbf507`  
		Last Modified: Sat, 04 Feb 2023 08:16:26 GMT  
		Size: 39.6 MB (39558401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0895a9cfae4403af4769bb7fc2334726c0db5a6929982d11aca84a6fd3b4247`  
		Last Modified: Sat, 04 Feb 2023 08:16:17 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b8ed21414ac18410d2cd7538e45767fefbf32a8719524c47f79dbb6481c58a9`  
		Last Modified: Sat, 04 Feb 2023 08:16:17 GMT  
		Size: 1.7 KB (1718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba129a165b264b065c4c64c28d541b80a301b07360486eeaaa32fffd058c8614`  
		Last Modified: Sat, 04 Feb 2023 08:16:17 GMT  
		Size: 1.5 KB (1479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d33029a943fe1a9b73a9717bc4636749407077422d7374aa4dddc3a99a9f97a7`  
		Last Modified: Sat, 04 Feb 2023 08:16:17 GMT  
		Size: 1.4 MB (1385416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:036ba73b7268a6aed37bd51a00d8c5ffd4f4a71eb03b0aa0e8ed0a6c0123bc82`  
		Last Modified: Sat, 04 Feb 2023 08:16:17 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:standalone` - linux; mips64le

```console
$ docker pull adminer@sha256:0566934f328c80510fdb62adfc866aeb360712e6df9b0a27474a0ad53c6148a4
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.6 MB (92610528 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fcc732f3bac92ee347514fc3ed0501efa9c7a348b4e0c1d588c77787ddf8dbe4`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Thu, 09 Feb 2023 02:44:36 GMT
ADD file:0cc085dc00beb990e7bfcdd8b37dceccb8f6d62d7c5ce2d7e736cdf4d52ab799 in / 
# Thu, 09 Feb 2023 02:44:41 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 06:13:03 GMT
STOPSIGNAL SIGINT
# Thu, 09 Feb 2023 06:14:56 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 06:15:02 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Thu, 09 Feb 2023 06:15:09 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 09 Feb 2023 06:15:12 GMT
WORKDIR /var/www/html
# Thu, 09 Feb 2023 06:15:15 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 09 Feb 2023 06:15:18 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 09 Feb 2023 06:15:22 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 09 Feb 2023 06:15:25 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 09 Feb 2023 06:16:14 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 09 Feb 2023 06:16:17 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 09 Feb 2023 06:16:20 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 09 Feb 2023 06:16:23 GMT
USER adminer
# Thu, 09 Feb 2023 06:16:26 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Thu, 09 Feb 2023 06:16:30 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:11a4758105e306ed24134ddf12f4d813426845c37a0ab14cb71de94c2858f09c`  
		Last Modified: Thu, 09 Feb 2023 02:53:05 GMT  
		Size: 53.3 MB (53266784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7daca01da5691398087a3bfc7f953540cff885f22074e0129fda0d5e578a7a64`  
		Last Modified: Thu, 09 Feb 2023 06:19:06 GMT  
		Size: 38.0 MB (37953476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53cfc05716a9d1f679b734de3bff7a1b9714f5eb4b5040d6e143defb24f4975b`  
		Last Modified: Thu, 09 Feb 2023 06:18:37 GMT  
		Size: 395.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66588c07e295fc98922360681aab4fd6a5c85ca29e0d60b27a06b53038e89c06`  
		Last Modified: Thu, 09 Feb 2023 06:18:37 GMT  
		Size: 1.7 KB (1729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6920b4dc4d4b5e73a928683693ea3ec779eb5c2100896fcc49acbb46ca85198a`  
		Last Modified: Thu, 09 Feb 2023 06:18:37 GMT  
		Size: 1.5 KB (1479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a2bb1759b592851efa52aa0ae0243e97ddaee48fec421bde7daeb618542cca8`  
		Last Modified: Thu, 09 Feb 2023 06:18:38 GMT  
		Size: 1.4 MB (1386172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1a36c2a9b981a0b8491e075725805da77790fd3eb7a7b71f664ef3c369a2e14`  
		Last Modified: Thu, 09 Feb 2023 06:18:37 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:standalone` - linux; ppc64le

```console
$ docker pull adminer@sha256:47a4ade05e65fa4596b6163d81cd7a4fa77513df4972a34167a78b55224b98d7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.2 MB (101226739 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d968381d4dcfc992e9ec7607ed161acc52925d93157eed9ed50bbc08830df809`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Sat, 04 Feb 2023 12:25:27 GMT
ADD file:724a2ac3b6190353442c93dce0ad4b3ab5c60144fc8204131767af6760e11980 in / 
# Sat, 04 Feb 2023 12:25:30 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 17:52:28 GMT
STOPSIGNAL SIGINT
# Sat, 04 Feb 2023 17:53:25 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 17:53:28 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Sat, 04 Feb 2023 17:53:31 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Sat, 04 Feb 2023 17:53:31 GMT
WORKDIR /var/www/html
# Sat, 04 Feb 2023 17:53:32 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Sat, 04 Feb 2023 17:53:32 GMT
ENV ADMINER_VERSION=4.8.1
# Sat, 04 Feb 2023 17:53:32 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Sat, 04 Feb 2023 17:53:33 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Sat, 04 Feb 2023 17:54:00 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 04 Feb 2023 17:54:00 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Sat, 04 Feb 2023 17:54:00 GMT
ENTRYPOINT ["entrypoint.sh"]
# Sat, 04 Feb 2023 17:54:01 GMT
USER adminer
# Sat, 04 Feb 2023 17:54:01 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Sat, 04 Feb 2023 17:54:02 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:c14c296a64e0f557b40f88759a913c28d0b28c646e5ec0cf0ceb49457156a792`  
		Last Modified: Sat, 04 Feb 2023 12:31:37 GMT  
		Size: 58.9 MB (58897064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2874c2bcc11a32eb3e38ad44035b5962c96846742a4307ba2c420da009e81ea7`  
		Last Modified: Sat, 04 Feb 2023 17:55:24 GMT  
		Size: 40.9 MB (40940112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dff9f9467cf09d7f5c242cfb1cacef36591219699095992b5738c1a88620f1d1`  
		Last Modified: Sat, 04 Feb 2023 17:55:09 GMT  
		Size: 394.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5c16d0da50d675218fc2a7373e45781eb595f8a795b902bcadf6be87ec0c887`  
		Last Modified: Sat, 04 Feb 2023 17:55:09 GMT  
		Size: 1.9 KB (1879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20dcb0d7c1b30e96ea63a399103c52c4292e83ce4579f47057d8dfe4d78b0aef`  
		Last Modified: Sat, 04 Feb 2023 17:55:09 GMT  
		Size: 1.5 KB (1478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3f8d644f4416950947c0acf3f7511db8085e591667b824d91224cec02554543`  
		Last Modified: Sat, 04 Feb 2023 17:55:09 GMT  
		Size: 1.4 MB (1385321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02759dcc9c00093b87b4c7129217d0bb02701ea0aa1e86f4d8f0eaf7a56723ab`  
		Last Modified: Sat, 04 Feb 2023 17:55:09 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:standalone` - linux; s390x

```console
$ docker pull adminer@sha256:2719e0584d03780419167688eaba32d1ee3527400ff69f7f2cdd3db286a68aa8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.7 MB (93688213 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e9613c6a60d2d28ec14e33ed1f2f4b998316d21902a342ceca374a3b98116f1`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Thu, 09 Feb 2023 02:41:26 GMT
ADD file:952595f2a554945ef740fa7b1fbc617a9ce3e1c3b90ddf1e7c0ac6018e6a98f9 in / 
# Thu, 09 Feb 2023 02:41:30 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 07:18:54 GMT
STOPSIGNAL SIGINT
# Thu, 09 Feb 2023 07:20:03 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 07:20:13 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Thu, 09 Feb 2023 07:20:15 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 09 Feb 2023 07:20:16 GMT
WORKDIR /var/www/html
# Thu, 09 Feb 2023 07:20:17 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 09 Feb 2023 07:20:18 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 09 Feb 2023 07:20:19 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 09 Feb 2023 07:20:20 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 09 Feb 2023 07:20:29 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 09 Feb 2023 07:20:29 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 09 Feb 2023 07:20:29 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 09 Feb 2023 07:20:30 GMT
USER adminer
# Thu, 09 Feb 2023 07:20:30 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Thu, 09 Feb 2023 07:20:30 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:83809ebda0c421fc95029bc6775e0a0c1eba6916a58b115dcb6a14885dae2028`  
		Last Modified: Thu, 09 Feb 2023 02:45:46 GMT  
		Size: 53.3 MB (53278896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7e31cf57a38a02fa2d3f8ff53add4d422bd4ff62ec4b24e0831c6725cee4b77`  
		Last Modified: Thu, 09 Feb 2023 07:21:24 GMT  
		Size: 39.0 MB (39019658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0633cef61215983b712e699a77b2f0a05ae8e463a4b6c07ffa63d79c6d451f3`  
		Last Modified: Thu, 09 Feb 2023 07:21:18 GMT  
		Size: 394.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:827d0eb471d78ca9b876122dfaeddf3edb023c66c6efa92c4ec68f85e999114d`  
		Last Modified: Thu, 09 Feb 2023 07:21:18 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e6233ba1bdaa0fba57704d8dc153af1171478f4f644bcd1672d9a4fd9712ccb`  
		Last Modified: Thu, 09 Feb 2023 07:21:18 GMT  
		Size: 1.5 KB (1483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5eb9aee6c3e13c08694db2a9db11c9563576952794921b2cfa054236137c34ba`  
		Last Modified: Thu, 09 Feb 2023 07:21:18 GMT  
		Size: 1.4 MB (1385406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c778394cc4cf1727666c9cc60aec4329d57cae6761ed5d514b755368d165048`  
		Last Modified: Thu, 09 Feb 2023 07:21:18 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
