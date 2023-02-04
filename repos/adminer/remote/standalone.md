## `adminer:standalone`

```console
$ docker pull adminer@sha256:19e0ba9e8b43fde46ca276e795c181d7cd07f3edc0fe88cc1e1880b02be0399e
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
$ docker pull adminer@sha256:7c1fa4cba8de32f8dcd0490b2a2422c631b19bb487e99b086994b5c05a3e5304
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.2 MB (91166086 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e49dc547f30520e8cc02bd7952804ffcd3083edcff85583be202968d662f1d30`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Sat, 04 Feb 2023 02:46:21 GMT
ADD file:1c80f7ec931ef9c6fa80892f75b88f6b3aebe7abe65f4a13b9371eb98475ca96 in / 
# Sat, 04 Feb 2023 02:46:23 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 03:10:13 GMT
STOPSIGNAL SIGINT
# Sat, 04 Feb 2023 03:10:42 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 03:10:43 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Sat, 04 Feb 2023 03:10:43 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Sat, 04 Feb 2023 03:10:44 GMT
WORKDIR /var/www/html
# Sat, 04 Feb 2023 03:10:44 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Sat, 04 Feb 2023 03:10:44 GMT
ENV ADMINER_VERSION=4.8.1
# Sat, 04 Feb 2023 03:10:44 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Sat, 04 Feb 2023 03:10:44 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Sat, 04 Feb 2023 03:10:59 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 04 Feb 2023 03:10:59 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Sat, 04 Feb 2023 03:10:59 GMT
ENTRYPOINT ["entrypoint.sh"]
# Sat, 04 Feb 2023 03:10:59 GMT
USER adminer
# Sat, 04 Feb 2023 03:10:59 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Sat, 04 Feb 2023 03:10:59 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:193207e81b928808ec6f645dfaf0b61e74f80f891a3bad16651e923e85334c17`  
		Last Modified: Sat, 04 Feb 2023 02:51:10 GMT  
		Size: 52.5 MB (52530008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bf1e080dcd3cfdef2852c2a62475d65a3be37771728b0f57be08714f0c60e36`  
		Last Modified: Sat, 04 Feb 2023 03:12:03 GMT  
		Size: 37.2 MB (37246915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4bb45667a6f38868757806bcd165542a734a196db03d91aabbef270ef54210e`  
		Last Modified: Sat, 04 Feb 2023 03:11:53 GMT  
		Size: 395.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7e27c4ea0322a359fdb6aeb5d6c9336b31e2ab266d453f594e2372614b70c8f`  
		Last Modified: Sat, 04 Feb 2023 03:11:53 GMT  
		Size: 1.8 KB (1835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca440ca86e683467380dce0cca920c799bbfe61964be1764d3259310da89b340`  
		Last Modified: Sat, 04 Feb 2023 03:11:53 GMT  
		Size: 1.5 KB (1479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70cef54c0996b2fbcc45896c5b316b1d4d1a0ebaadc7402e4e46fd30bdca6400`  
		Last Modified: Sat, 04 Feb 2023 03:11:54 GMT  
		Size: 1.4 MB (1384960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e498ef275098488f6b8d48d742a015b32577dcd1ac762f40ceb3b035fb4316c`  
		Last Modified: Sat, 04 Feb 2023 03:11:53 GMT  
		Size: 494.0 B  
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
$ docker pull adminer@sha256:5bce7eb38b57d0c072096fc13fc21c2e5fb6fc9f9e2958c94330171da1493cc0
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.6 MB (92588549 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5aefc9be870e13f4af4e99c037900c1d7c798aac6e5076305e0b6099f6143fd3`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Sat, 04 Feb 2023 06:19:34 GMT
ADD file:6ce59568f971e1c72981ffb01f3c6b67b20b5b055edec122273990ec1c36f042 in / 
# Sat, 04 Feb 2023 06:19:40 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 18:20:42 GMT
STOPSIGNAL SIGINT
# Sat, 04 Feb 2023 18:22:40 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 18:22:47 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Sat, 04 Feb 2023 18:22:53 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Sat, 04 Feb 2023 18:22:57 GMT
WORKDIR /var/www/html
# Sat, 04 Feb 2023 18:23:00 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Sat, 04 Feb 2023 18:23:03 GMT
ENV ADMINER_VERSION=4.8.1
# Sat, 04 Feb 2023 18:23:07 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Sat, 04 Feb 2023 18:23:10 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Sat, 04 Feb 2023 18:24:03 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 04 Feb 2023 18:24:06 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Sat, 04 Feb 2023 18:24:09 GMT
ENTRYPOINT ["entrypoint.sh"]
# Sat, 04 Feb 2023 18:24:13 GMT
USER adminer
# Sat, 04 Feb 2023 18:24:16 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Sat, 04 Feb 2023 18:24:20 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:c1dc6b83fd5771c0e7c97ea21324a2c2a31849a9f2b37f7f4cf80645847ed538`  
		Last Modified: Sat, 04 Feb 2023 06:27:44 GMT  
		Size: 53.2 MB (53245135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92ab32f110ef640b2fbbb65789abec072a1b0380c0af8fb6441b36b0ca3994e3`  
		Last Modified: Sat, 04 Feb 2023 18:26:58 GMT  
		Size: 38.0 MB (37953128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d44568332bd32162444311aef1d12398133a3f670149554f2124cd9c8b780394`  
		Last Modified: Sat, 04 Feb 2023 18:26:30 GMT  
		Size: 398.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:044a96bad01b6418f1c9ac5e5ac32867b6c818ffe6d15b737b4336779c5a078d`  
		Last Modified: Sat, 04 Feb 2023 18:26:30 GMT  
		Size: 1.7 KB (1729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a365d2b5bcf2c09212100c4042cea12f3c3b2139054d5756506bdd8a86d8ad5e`  
		Last Modified: Sat, 04 Feb 2023 18:26:30 GMT  
		Size: 1.5 KB (1481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb68bdb53cd88698a7c919dff7276cbaef8187845a6979db5203926edcf13b7c`  
		Last Modified: Sat, 04 Feb 2023 18:26:31 GMT  
		Size: 1.4 MB (1386184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b7167ff0b3b1a61d81feec13bb17836d08cde6d3186e96a53d475c1e8df2d4d`  
		Last Modified: Sat, 04 Feb 2023 18:26:30 GMT  
		Size: 494.0 B  
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
$ docker pull adminer@sha256:c3f405ec472179d37cbb59a97aae02ce8c3664e1ce4f253a6c7389b060a19d5f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.7 MB (93667223 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12806fc9688bbfeea1fa8cae1265eac7672deb67de2eaf2c8a710cc21756c6e1`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Sat, 04 Feb 2023 04:05:57 GMT
ADD file:57d389473a23d7f4ecc41746379cb0b904a0ed555b55b4cae8e0ebbb2fdb063b in / 
# Sat, 04 Feb 2023 04:06:00 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 04:28:05 GMT
STOPSIGNAL SIGINT
# Sat, 04 Feb 2023 04:28:27 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 04:28:29 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Sat, 04 Feb 2023 04:28:30 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Sat, 04 Feb 2023 04:28:30 GMT
WORKDIR /var/www/html
# Sat, 04 Feb 2023 04:28:30 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Sat, 04 Feb 2023 04:28:30 GMT
ENV ADMINER_VERSION=4.8.1
# Sat, 04 Feb 2023 04:28:31 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Sat, 04 Feb 2023 04:28:31 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Sat, 04 Feb 2023 04:28:39 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 04 Feb 2023 04:28:39 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Sat, 04 Feb 2023 04:28:40 GMT
ENTRYPOINT ["entrypoint.sh"]
# Sat, 04 Feb 2023 04:28:40 GMT
USER adminer
# Sat, 04 Feb 2023 04:28:40 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Sat, 04 Feb 2023 04:28:40 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:20679e968bacc458d63e0ab992076c085ca41e6c4c6d2a152130c347a7604493`  
		Last Modified: Sat, 04 Feb 2023 04:10:08 GMT  
		Size: 53.3 MB (53258422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0b3cd564086af4d6785d439bcbd880b22b876f7203406b8c89a2a1ea92b6175`  
		Last Modified: Sat, 04 Feb 2023 04:29:28 GMT  
		Size: 39.0 MB (39019368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:331aa0615ad09c32e532edacfd3b679e9803f68103e992b7ba35c6a11735634d`  
		Last Modified: Sat, 04 Feb 2023 04:29:22 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e30624611f807e5e1ebce2fb2c63f0f51a585a417d59e47b6976254425d49ac`  
		Last Modified: Sat, 04 Feb 2023 04:29:22 GMT  
		Size: 1.9 KB (1879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0b896b54b83150710468b71246e462f41af780297c4244290a154600a7ef2e3`  
		Last Modified: Sat, 04 Feb 2023 04:29:22 GMT  
		Size: 1.5 KB (1477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5be63f66c0e34a26ea76521a7355373ee9f89088f867afe1beaa51634fe65949`  
		Last Modified: Sat, 04 Feb 2023 04:29:22 GMT  
		Size: 1.4 MB (1385196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:649e2be8d8568f532bdec719c417f06eaf4f6dea7a60a251d691fe718b97b5f4`  
		Last Modified: Sat, 04 Feb 2023 04:29:22 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
