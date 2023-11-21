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
$ docker pull adminer@sha256:0ce7583815dabdd9f560ee0afed630ecb33df6756f4b66c85c197011559a0248
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
$ docker pull adminer@sha256:78d95e4c7a6cfb584a500e0e8ca7db956ab9ff1cd4b3239306b330c2637ecfa2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.9 MB (95942047 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7554c8e10d81e451e656e73d613de4f9c885b91255f46a2fdc03ccf275a1d449`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:46 GMT
ADD file:71543995e4d314b0c86da5ddf8e0cb74649767d30b3e5b6261360de354f0567b in / 
# Tue, 21 Nov 2023 05:21:46 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 09:49:06 GMT
STOPSIGNAL SIGINT
# Tue, 21 Nov 2023 09:49:25 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 09:49:26 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 21 Nov 2023 09:49:27 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 21 Nov 2023 09:49:27 GMT
WORKDIR /var/www/html
# Tue, 21 Nov 2023 09:49:27 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 21 Nov 2023 09:49:27 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 21 Nov 2023 09:49:27 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 21 Nov 2023 09:49:27 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 21 Nov 2023 09:49:39 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Nov 2023 09:49:39 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 21 Nov 2023 09:49:39 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 21 Nov 2023 09:49:39 GMT
USER adminer
# Tue, 21 Nov 2023 09:49:39 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Tue, 21 Nov 2023 09:49:39 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:d1da99c2f14827498c4a9bb3623ae909b44564bdabad1802f064169069df81fb`  
		Last Modified: Tue, 21 Nov 2023 05:26:17 GMT  
		Size: 55.1 MB (55057903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d7c776bdbb7e1224dedbc306fec7eb6e3842bd895a396927c36fa7f434312a3`  
		Last Modified: Tue, 21 Nov 2023 09:50:18 GMT  
		Size: 39.5 MB (39493553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:987d0f042e915521e94497a8e40892d4ec0532bd7641920df5ace1000310d793`  
		Last Modified: Tue, 21 Nov 2023 09:50:10 GMT  
		Size: 389.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb163dc8650b5fde5c72f76b8937b3c38d3dd4c7a2922d7b6f95a0890070c4d9`  
		Last Modified: Tue, 21 Nov 2023 09:50:10 GMT  
		Size: 1.9 KB (1878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98b256c86f3d5b1eab91122ae075d7b3b15d1185ebe1cc10a8b4d2fb6f2bdf5f`  
		Last Modified: Tue, 21 Nov 2023 09:50:10 GMT  
		Size: 1.5 KB (1480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7952b9a84b1867112d08313ef023ee4917d7bbd0f91f4d8ae3ce1b17376d345e`  
		Last Modified: Tue, 21 Nov 2023 09:50:11 GMT  
		Size: 1.4 MB (1386353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77cf83a8d79b963388e7d18d6836ac44d7832d08fa39ab46ba57f0c92e48e1f2`  
		Last Modified: Tue, 21 Nov 2023 09:50:10 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4` - linux; arm variant v5

```console
$ docker pull adminer@sha256:f6bb8e720054e43d3bc65a163e9fc4146ce4c215db05216f56be5cbac7428eb7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.2 MB (91205860 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9bd45b72f483757bdbd0f31b96e08578a127cc80966526aa0a9a897f5012203`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Tue, 21 Nov 2023 05:01:00 GMT
ADD file:a5c8bd4b0873bd9ad0402143df41b5fd89c50bd24bb071b7d010919e189d88f9 in / 
# Tue, 21 Nov 2023 05:01:00 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 05:46:09 GMT
STOPSIGNAL SIGINT
# Tue, 21 Nov 2023 05:46:38 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 05:46:39 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 21 Nov 2023 05:46:40 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 21 Nov 2023 05:46:40 GMT
WORKDIR /var/www/html
# Tue, 21 Nov 2023 05:46:40 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 21 Nov 2023 05:46:40 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 21 Nov 2023 05:46:40 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 21 Nov 2023 05:46:40 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 21 Nov 2023 05:46:55 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Nov 2023 05:46:55 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 21 Nov 2023 05:46:55 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 21 Nov 2023 05:46:55 GMT
USER adminer
# Tue, 21 Nov 2023 05:46:55 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Tue, 21 Nov 2023 05:46:55 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:7378d71ea16926a061a2edbf0eb3dd13563fcb3ba9cf139c25e8334b36db1adf`  
		Last Modified: Tue, 21 Nov 2023 05:04:15 GMT  
		Size: 52.6 MB (52562921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cde673c33e7bfa6c04aeb9e184923984b648ae971715981d598aca5162e3c911`  
		Last Modified: Tue, 21 Nov 2023 05:47:34 GMT  
		Size: 37.3 MB (37252430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4fee5ad01a4adcbc52d632521a683e83dd44bb905a3048fc20faaa96d58f747`  
		Last Modified: Tue, 21 Nov 2023 05:47:25 GMT  
		Size: 386.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:062df034c3a9a14a736fb1733f5f91b8c5cad9974f6b67df85f488a45026f47c`  
		Last Modified: Tue, 21 Nov 2023 05:47:24 GMT  
		Size: 1.9 KB (1869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:610f64ab71d9f5c7abad4551870c223a9b95603025384ef1e7a85f624f0b0467`  
		Last Modified: Tue, 21 Nov 2023 05:47:24 GMT  
		Size: 1.5 KB (1481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59cca3ff7ed68079f673662534d292a264aa5c1d7d4358251d8e25f21faa9f94`  
		Last Modified: Tue, 21 Nov 2023 05:47:25 GMT  
		Size: 1.4 MB (1386281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:753ad2913e083c1b5cb5b06853944934450629b0451d408743ddffc1f4c0a843`  
		Last Modified: Tue, 21 Nov 2023 05:47:24 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4` - linux; arm variant v7

```console
$ docker pull adminer@sha256:6faef276799d02bdd9abf0ba022b692fd46f8144584adcfa771a76d225131045
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.8 MB (87796870 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9bb280f29bbaaa440662c6cbd26fabd7313fb299195b0ff2ca0cc22cff61f1ab`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Tue, 21 Nov 2023 03:57:54 GMT
ADD file:ed8d88d0476fad37879d872d61d05a8cffff35609566f080f78bb882d1bae26b in / 
# Tue, 21 Nov 2023 03:57:54 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 06:58:56 GMT
STOPSIGNAL SIGINT
# Tue, 21 Nov 2023 06:59:20 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 06:59:21 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 21 Nov 2023 06:59:21 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 21 Nov 2023 06:59:21 GMT
WORKDIR /var/www/html
# Tue, 21 Nov 2023 06:59:21 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 21 Nov 2023 06:59:21 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 21 Nov 2023 06:59:21 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 21 Nov 2023 06:59:22 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 21 Nov 2023 06:59:37 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Nov 2023 06:59:37 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 21 Nov 2023 06:59:37 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 21 Nov 2023 06:59:37 GMT
USER adminer
# Tue, 21 Nov 2023 06:59:37 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Tue, 21 Nov 2023 06:59:37 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:1dac19092a737e476f9b096fe28463512ae21c4f596dd2f8b84d62530416dffe`  
		Last Modified: Tue, 21 Nov 2023 04:02:11 GMT  
		Size: 50.2 MB (50215653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2f8153e5d67bc5a0049a12eb2430f50747238b7d4023cacdfc5dad9cdbd244a`  
		Last Modified: Tue, 21 Nov 2023 07:00:24 GMT  
		Size: 36.2 MB (36190640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ea62b864a160dff0b693d9397a8b84a1bc65e8e381b223294a8ac5ac8c68b8a`  
		Last Modified: Tue, 21 Nov 2023 07:00:15 GMT  
		Size: 393.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e2dd6fa8973e47e4cce58445b7207793f22b2371aa58678dc17d4172eac0b32`  
		Last Modified: Tue, 21 Nov 2023 07:00:15 GMT  
		Size: 1.9 KB (1871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4d33015217bf866b0d2c44cd29bf71617469b2e87e38eb15795aa3a293c83fa`  
		Last Modified: Tue, 21 Nov 2023 07:00:16 GMT  
		Size: 1.5 KB (1478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24ee8e39b9683ef6aa34033169655e5585db29d9557c0e1eb9aa117e1c771047`  
		Last Modified: Tue, 21 Nov 2023 07:00:16 GMT  
		Size: 1.4 MB (1386341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c14859802a2676aa6a511bbd06ce80a759e38e94927cd4d4b60dd202568ef5b`  
		Last Modified: Tue, 21 Nov 2023 07:00:15 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4` - linux; arm64 variant v8

```console
$ docker pull adminer@sha256:e5fda74f5900f3c7ef8f74bda0392b45089f33f56374326bb331d8db26eb8b41
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.3 MB (94346130 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ccf82dd602ee08aa22718c108fcbcedbebb819a09c86b9f0fe8f2c1737bd08a7`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:13 GMT
ADD file:614987b9855939825ad2383e7bacbf14ea208d74906982bba3a67126702c8371 in / 
# Tue, 21 Nov 2023 06:27:13 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 10:22:26 GMT
STOPSIGNAL SIGINT
# Tue, 21 Nov 2023 10:22:43 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 10:22:44 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 21 Nov 2023 10:22:44 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 21 Nov 2023 10:22:44 GMT
WORKDIR /var/www/html
# Tue, 21 Nov 2023 10:22:44 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 21 Nov 2023 10:22:44 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 21 Nov 2023 10:22:45 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 21 Nov 2023 10:22:45 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 21 Nov 2023 10:22:54 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Nov 2023 10:22:54 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 21 Nov 2023 10:22:54 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 21 Nov 2023 10:22:54 GMT
USER adminer
# Tue, 21 Nov 2023 10:22:55 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Tue, 21 Nov 2023 10:22:55 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:bbf382c14c7b19b81c612f639e09e6a7b04eccd4481d0abac48b8ace9faae3b3`  
		Last Modified: Tue, 21 Nov 2023 06:30:47 GMT  
		Size: 53.7 MB (53707872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aa045892ab5d3693eb19355bad15725aa10139ceb2bfc2cb6141778f671e8e4`  
		Last Modified: Tue, 21 Nov 2023 10:23:29 GMT  
		Size: 39.2 MB (39247701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d77bfaecae2cacef431f4d68d17c26be0ab2300b5dfee893959aaae0c6427677`  
		Last Modified: Tue, 21 Nov 2023 10:23:21 GMT  
		Size: 386.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1364c7eb4b90daedaca80aff830c09309115f174a295c35ba7885c60557fa1e`  
		Last Modified: Tue, 21 Nov 2023 10:23:21 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:080b929d6ed912f11ed340726920967a938d3632641f4f86e15a30fc7b255888`  
		Last Modified: Tue, 21 Nov 2023 10:23:21 GMT  
		Size: 1.5 KB (1477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:633cfed53ab70b9e08d21a78973fc2a318d49c9cc54f3100604c9b91dd533c82`  
		Last Modified: Tue, 21 Nov 2023 10:23:22 GMT  
		Size: 1.4 MB (1386322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc610b080dd3b327bfe4b6ca8da59bc3a5555a295aff6c4f18d172f070b4e1ab`  
		Last Modified: Tue, 21 Nov 2023 10:23:21 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4` - linux; 386

```console
$ docker pull adminer@sha256:173f2532a535a7780bffa43d6385797ba5335ab89832cb016cbb54cb0ab60fb2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.0 MB (96998974 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85b8488ee11e55b40364ca362184cc13095a7b83f1c1e65e524862cc27000db2`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Tue, 21 Nov 2023 04:40:03 GMT
ADD file:54170328827ccc52692c964f0c45a65ed6efdf39897f2c226672fdf526f3c412 in / 
# Tue, 21 Nov 2023 04:40:04 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 15:41:51 GMT
STOPSIGNAL SIGINT
# Tue, 21 Nov 2023 15:42:20 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 15:42:21 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 21 Nov 2023 15:42:22 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 21 Nov 2023 15:42:22 GMT
WORKDIR /var/www/html
# Tue, 21 Nov 2023 15:42:22 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 21 Nov 2023 15:42:22 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 21 Nov 2023 15:42:22 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 21 Nov 2023 15:42:22 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 21 Nov 2023 15:42:37 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Nov 2023 15:42:37 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 21 Nov 2023 15:42:37 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 21 Nov 2023 15:42:37 GMT
USER adminer
# Tue, 21 Nov 2023 15:42:37 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Tue, 21 Nov 2023 15:42:37 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:e33c1468a29e45636d4d9529b663048f7e8aa83ff428eb0681253bd4200e23ec`  
		Last Modified: Tue, 21 Nov 2023 04:44:57 GMT  
		Size: 56.0 MB (56046301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8137e600c481ac4ed29cae88512a113a2eadcc1d26e72628216670ef4f61ba30`  
		Last Modified: Tue, 21 Nov 2023 15:43:16 GMT  
		Size: 39.6 MB (39562172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e42a8870a081f3a4ab284980034bebec6585740c88e4c40ae98b2e1fa9955f5`  
		Last Modified: Tue, 21 Nov 2023 15:43:05 GMT  
		Size: 392.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48c728479be5016dacc84b6c0c244f327eff896df6a326af2826d6ad4c5387b6`  
		Last Modified: Tue, 21 Nov 2023 15:43:05 GMT  
		Size: 1.9 KB (1870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1000dcb7b3ee07a4d8a46142cda4b99b13051577e48599f89d62c8fd8c7e61a8`  
		Last Modified: Tue, 21 Nov 2023 15:43:05 GMT  
		Size: 1.5 KB (1482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d8473e68cd9a1e0940ff9bb80857e7d32bfde252766cc39fc1c3566222b0c1c`  
		Last Modified: Tue, 21 Nov 2023 15:43:06 GMT  
		Size: 1.4 MB (1386265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d7609e79a7e8443050102286e60b2022e9f3447043db395cabb7e2ad151b1e0`  
		Last Modified: Tue, 21 Nov 2023 15:43:05 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4` - linux; mips64le

```console
$ docker pull adminer@sha256:84b1c19875f37b42946db21b87c80b8f8d9d9c7392eff0a7a065cf6d5fe769b2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.6 MB (92634921 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6454361a51d8f0d5781cd1854359c6b0812cc29466f516dd6386754b3583699`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Tue, 21 Nov 2023 04:10:25 GMT
ADD file:dbfc3d226166089c4db0c154fdcea8049b8758c6812f1c397dec1444985e8557 in / 
# Tue, 21 Nov 2023 04:10:31 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 12:14:44 GMT
STOPSIGNAL SIGINT
# Tue, 21 Nov 2023 12:16:43 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 12:16:50 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 21 Nov 2023 12:16:57 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 21 Nov 2023 12:17:00 GMT
WORKDIR /var/www/html
# Tue, 21 Nov 2023 12:17:04 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 21 Nov 2023 12:17:07 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 21 Nov 2023 12:17:10 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 21 Nov 2023 12:17:14 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 21 Nov 2023 12:18:08 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Nov 2023 12:18:11 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 21 Nov 2023 12:18:14 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 21 Nov 2023 12:18:17 GMT
USER adminer
# Tue, 21 Nov 2023 12:18:21 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Tue, 21 Nov 2023 12:18:24 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:ca31218601e95f4aafae0dcadda7600aeb04db374e1e829d5c123f8033ba3472`  
		Last Modified: Tue, 21 Nov 2023 04:21:21 GMT  
		Size: 53.3 MB (53289162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d172a1ce4463b8a1bb14b88d9f7c98a7f06f260dfc2849e77f3d41be6d17db9`  
		Last Modified: Tue, 21 Nov 2023 12:21:00 GMT  
		Size: 38.0 MB (37954467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbd3b039fbc0efa77466cfb045c80c120d45355cf2db0dd6533eeb1cee6296e1`  
		Last Modified: Tue, 21 Nov 2023 12:20:33 GMT  
		Size: 394.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bac97c667ed055993103f32b019a430a853a94eef6bf75086fda9949a9fd1d8`  
		Last Modified: Tue, 21 Nov 2023 12:20:34 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66eec20186701717a98146a63c5c8f88304d44243fe6f6505edf4d1135672446`  
		Last Modified: Tue, 21 Nov 2023 12:20:34 GMT  
		Size: 1.5 KB (1483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a56ddb348b2b13a6cac73829460bdcce2971790b6be59ac9da70b739453488b8`  
		Last Modified: Tue, 21 Nov 2023 12:20:34 GMT  
		Size: 1.4 MB (1387192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f922348b25af66b56cdd7a4863a9a120057afa01489fc9058cf7e975b198d05`  
		Last Modified: Tue, 21 Nov 2023 12:20:34 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4` - linux; ppc64le

```console
$ docker pull adminer@sha256:3b96a3711e0e719557e514cb8870567e67ab545a7fe18b4feeca4e0e4c85d678
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.3 MB (101265448 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0c151160d019f74dfe13959cf16722a5172a0023a5f747201c90b752e001545`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Tue, 21 Nov 2023 04:24:26 GMT
ADD file:c21c2b6cb3f9bdf6cc3641e9ebf810a461174480c6cd1c25515cf9fce4aa2143 in / 
# Tue, 21 Nov 2023 04:24:30 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 06:49:59 GMT
STOPSIGNAL SIGINT
# Tue, 21 Nov 2023 06:50:40 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 06:50:42 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 21 Nov 2023 06:50:44 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 21 Nov 2023 06:50:44 GMT
WORKDIR /var/www/html
# Tue, 21 Nov 2023 06:50:44 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 21 Nov 2023 06:50:44 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 21 Nov 2023 06:50:45 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 21 Nov 2023 06:50:45 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 21 Nov 2023 06:51:03 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Nov 2023 06:51:03 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 21 Nov 2023 06:51:03 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 21 Nov 2023 06:51:03 GMT
USER adminer
# Tue, 21 Nov 2023 06:51:04 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Tue, 21 Nov 2023 06:51:04 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:23ebe74b854f8f6e2671f4c8cc147a6925fb7d929ce5898f7ca2af9781bf7d38`  
		Last Modified: Tue, 21 Nov 2023 04:29:21 GMT  
		Size: 58.9 MB (58929678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa255108512a37e57b2fdf827a0fdb4e3783a0649fb80ecdd431d4921dd6761c`  
		Last Modified: Tue, 21 Nov 2023 06:51:51 GMT  
		Size: 40.9 MB (40945122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5862ce535fc870ad9665c04e9816effde44c5f4469bc852265ba0bfe11ad7001`  
		Last Modified: Tue, 21 Nov 2023 06:51:41 GMT  
		Size: 391.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7204feb32d0a6fe6dd0348f7a8c2845b90b631ba893c08c48a724057c8a5e3d1`  
		Last Modified: Tue, 21 Nov 2023 06:51:41 GMT  
		Size: 1.9 KB (1879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb06eb196e5a191ad6e9d6d43052c2fd0f833100bf197c73f3f9c8df967003d1`  
		Last Modified: Tue, 21 Nov 2023 06:51:41 GMT  
		Size: 1.5 KB (1482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76df205e8013dede04db80018bebbabea233e0186671f2fd251fa440acde39ef`  
		Last Modified: Tue, 21 Nov 2023 06:51:41 GMT  
		Size: 1.4 MB (1386403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7099dfc32b7ad37a3cfe50e8aad19c609d5e9daf0535dd5cd0f853de87d0de8f`  
		Last Modified: Tue, 21 Nov 2023 06:51:41 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4` - linux; s390x

```console
$ docker pull adminer@sha256:0832c83b0a0b564f962bc8f2f82974852bda2c876629b26a32e31e5b99e8fbc0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.7 MB (93709271 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72ed9e5473cf095c9f6c3263d8ff775ee9a240aa6597b921ebd51ec24f8978c1`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Tue, 21 Nov 2023 05:04:52 GMT
ADD file:b0a8fd50925b3555a0c10177e65551cae288917f9bad8fb4728ec83cc0765afe in / 
# Tue, 21 Nov 2023 05:05:01 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 06:04:07 GMT
STOPSIGNAL SIGINT
# Tue, 21 Nov 2023 06:04:29 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 06:04:35 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 21 Nov 2023 06:04:35 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 21 Nov 2023 06:04:36 GMT
WORKDIR /var/www/html
# Tue, 21 Nov 2023 06:04:36 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 21 Nov 2023 06:04:36 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 21 Nov 2023 06:04:36 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 21 Nov 2023 06:04:36 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 21 Nov 2023 06:04:45 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Nov 2023 06:04:46 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 21 Nov 2023 06:04:46 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 21 Nov 2023 06:04:46 GMT
USER adminer
# Tue, 21 Nov 2023 06:04:46 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Tue, 21 Nov 2023 06:04:47 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:9488c1539560318cb45b39150f91e365b928c0a246788663f5c72d185864bd3e`  
		Last Modified: Tue, 21 Nov 2023 05:10:34 GMT  
		Size: 53.3 MB (53296396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09efec12dc42685e3fe1693d18bc42d61971044de30a99ee3f044d942e93a470`  
		Last Modified: Tue, 21 Nov 2023 06:05:38 GMT  
		Size: 39.0 MB (39022251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d211af034ddf5d1e81df73b8d237d1c15d165b5443c533eedbeecc5659d4d4b`  
		Last Modified: Tue, 21 Nov 2023 06:05:31 GMT  
		Size: 393.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd2e9fc8bb5d1ec8686111ad3e20155b1ac539fc01b742c2318311374c9c3d29`  
		Last Modified: Tue, 21 Nov 2023 06:05:31 GMT  
		Size: 1.9 KB (1877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2acddcee94070eff9faaeaa170066fa650714281ae6b3094fc1d49c010f3902`  
		Last Modified: Tue, 21 Nov 2023 06:05:31 GMT  
		Size: 1.5 KB (1480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21ffbd0e004b4f2f9f75bdc6731ed7d644c91ee50221377d2ff00e82aa1f99b9`  
		Last Modified: Tue, 21 Nov 2023 06:05:31 GMT  
		Size: 1.4 MB (1386383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44baab47b2128777f4b94d45e4a91e7bd440dcb23e61b28ec31c8ac469b3cf40`  
		Last Modified: Tue, 21 Nov 2023 06:05:31 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `adminer:4-fastcgi`

```console
$ docker pull adminer@sha256:daa291dff0f15be3ba5d0a8cfdcf137d8dd0b1f9304d132c686a4e95dcd489dd
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
$ docker pull adminer@sha256:8440f4060b767baf10aa0a817bae4ebe1d2991721279fdc2656503639463bd7b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.9 MB (95944774 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e93286ecedd0f7ab872f2a51eafc625c321f348ed0da94d7f8364be85227c44`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:46 GMT
ADD file:71543995e4d314b0c86da5ddf8e0cb74649767d30b3e5b6261360de354f0567b in / 
# Tue, 21 Nov 2023 05:21:46 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 09:49:06 GMT
STOPSIGNAL SIGINT
# Tue, 21 Nov 2023 09:49:25 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 09:49:26 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 21 Nov 2023 09:49:47 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Tue, 21 Nov 2023 09:49:47 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 21 Nov 2023 09:49:48 GMT
WORKDIR /var/www/html
# Tue, 21 Nov 2023 09:49:48 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 21 Nov 2023 09:49:48 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 21 Nov 2023 09:49:48 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 21 Nov 2023 09:49:48 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 21 Nov 2023 09:49:59 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Nov 2023 09:49:59 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 21 Nov 2023 09:49:59 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 21 Nov 2023 09:49:59 GMT
USER adminer
# Tue, 21 Nov 2023 09:49:59 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:d1da99c2f14827498c4a9bb3623ae909b44564bdabad1802f064169069df81fb`  
		Last Modified: Tue, 21 Nov 2023 05:26:17 GMT  
		Size: 55.1 MB (55057903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d7c776bdbb7e1224dedbc306fec7eb6e3842bd895a396927c36fa7f434312a3`  
		Last Modified: Tue, 21 Nov 2023 09:50:18 GMT  
		Size: 39.5 MB (39493553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:987d0f042e915521e94497a8e40892d4ec0532bd7641920df5ace1000310d793`  
		Last Modified: Tue, 21 Nov 2023 09:50:10 GMT  
		Size: 389.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38f43fc128ac2c6808d4b9a8087484f11d8cd4105abf9cd319353086c9b3b1d6`  
		Last Modified: Tue, 21 Nov 2023 09:50:34 GMT  
		Size: 2.7 KB (2714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96fdd5fed3b41dde57c97813fce8fc18ab9b07901345f868f32d346cfc74eb01`  
		Last Modified: Tue, 21 Nov 2023 09:50:34 GMT  
		Size: 1.9 KB (1878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3322f8293171857aeafd5fe96548028722034a3151f51dc695cc3cbef006e6a8`  
		Last Modified: Tue, 21 Nov 2023 09:50:34 GMT  
		Size: 1.5 KB (1480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2653b5cb64efa6e1c82031fa6e50d69957ca93e7f1660cc5e97344e601703f8e`  
		Last Modified: Tue, 21 Nov 2023 09:50:34 GMT  
		Size: 1.4 MB (1386365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5038798e96f08d106fc18e6a12538f783f08af440d0957a26c321901ebbad4b`  
		Last Modified: Tue, 21 Nov 2023 09:50:34 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-fastcgi` - linux; arm variant v5

```console
$ docker pull adminer@sha256:b8f1ebac81289510963e10734e0ac78c24878a69d7aebbb9a3a29789c26dbfac
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.2 MB (91208572 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f60ec0b531cc5d09c3980c35d88d86cc1f9b8542ad54fcf7ff77d98ac3dea22`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Tue, 21 Nov 2023 05:01:00 GMT
ADD file:a5c8bd4b0873bd9ad0402143df41b5fd89c50bd24bb071b7d010919e189d88f9 in / 
# Tue, 21 Nov 2023 05:01:00 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 05:46:09 GMT
STOPSIGNAL SIGINT
# Tue, 21 Nov 2023 05:46:38 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 05:46:39 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 21 Nov 2023 05:46:58 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Tue, 21 Nov 2023 05:46:58 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 21 Nov 2023 05:46:58 GMT
WORKDIR /var/www/html
# Tue, 21 Nov 2023 05:46:58 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 21 Nov 2023 05:46:58 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 21 Nov 2023 05:46:58 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 21 Nov 2023 05:46:59 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 21 Nov 2023 05:47:15 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Nov 2023 05:47:15 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 21 Nov 2023 05:47:15 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 21 Nov 2023 05:47:15 GMT
USER adminer
# Tue, 21 Nov 2023 05:47:15 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:7378d71ea16926a061a2edbf0eb3dd13563fcb3ba9cf139c25e8334b36db1adf`  
		Last Modified: Tue, 21 Nov 2023 05:04:15 GMT  
		Size: 52.6 MB (52562921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cde673c33e7bfa6c04aeb9e184923984b648ae971715981d598aca5162e3c911`  
		Last Modified: Tue, 21 Nov 2023 05:47:34 GMT  
		Size: 37.3 MB (37252430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4fee5ad01a4adcbc52d632521a683e83dd44bb905a3048fc20faaa96d58f747`  
		Last Modified: Tue, 21 Nov 2023 05:47:25 GMT  
		Size: 386.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5f71f261b85a2e069d758daa1be7f3e53672fa4b8902826510a9159db451264`  
		Last Modified: Tue, 21 Nov 2023 05:47:51 GMT  
		Size: 2.7 KB (2705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d67d58698593646eb7ab4b717360bf37ab36a671802cb216b3262ce695ef1e5`  
		Last Modified: Tue, 21 Nov 2023 05:47:51 GMT  
		Size: 1.9 KB (1870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d309e407d77f27b1a5409e0ce83c664cb9f080a3168176e8114376d8721a153e`  
		Last Modified: Tue, 21 Nov 2023 05:47:51 GMT  
		Size: 1.5 KB (1477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ee0aa3b9dd1374206375afa28a3b15aa7e6b58abf1b669705b9a86f43e0be79`  
		Last Modified: Tue, 21 Nov 2023 05:47:51 GMT  
		Size: 1.4 MB (1386292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74eeb313bede5967e1e4dd1a8bef17eda92f71136ff55d6ed522d984a8712436`  
		Last Modified: Tue, 21 Nov 2023 05:47:51 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-fastcgi` - linux; arm variant v7

```console
$ docker pull adminer@sha256:1674e094629be082c484d9c7c974fa715e706fbf661bafc68bad546bed9ffe00
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.8 MB (87799571 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c995386759ce4cef4ffbcffb5be8163c9813d2a8220561e9a841f14fb07e0bd`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Tue, 21 Nov 2023 03:57:54 GMT
ADD file:ed8d88d0476fad37879d872d61d05a8cffff35609566f080f78bb882d1bae26b in / 
# Tue, 21 Nov 2023 03:57:54 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 06:58:56 GMT
STOPSIGNAL SIGINT
# Tue, 21 Nov 2023 06:59:20 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 06:59:21 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 21 Nov 2023 06:59:45 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Tue, 21 Nov 2023 06:59:46 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 21 Nov 2023 06:59:46 GMT
WORKDIR /var/www/html
# Tue, 21 Nov 2023 06:59:46 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 21 Nov 2023 06:59:46 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 21 Nov 2023 06:59:47 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 21 Nov 2023 06:59:47 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 21 Nov 2023 07:00:00 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Nov 2023 07:00:01 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 21 Nov 2023 07:00:01 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 21 Nov 2023 07:00:01 GMT
USER adminer
# Tue, 21 Nov 2023 07:00:01 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:1dac19092a737e476f9b096fe28463512ae21c4f596dd2f8b84d62530416dffe`  
		Last Modified: Tue, 21 Nov 2023 04:02:11 GMT  
		Size: 50.2 MB (50215653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2f8153e5d67bc5a0049a12eb2430f50747238b7d4023cacdfc5dad9cdbd244a`  
		Last Modified: Tue, 21 Nov 2023 07:00:24 GMT  
		Size: 36.2 MB (36190640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ea62b864a160dff0b693d9397a8b84a1bc65e8e381b223294a8ac5ac8c68b8a`  
		Last Modified: Tue, 21 Nov 2023 07:00:15 GMT  
		Size: 393.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e77dfeac49a3de3540eb4b5ade85851c08d2523b73c838b14a68fe81a3ec17a1`  
		Last Modified: Tue, 21 Nov 2023 07:00:40 GMT  
		Size: 2.7 KB (2715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e25f712f1f600f798ffd1261db13ef564f0af09c7c65533ed8ed59ec3b26552`  
		Last Modified: Tue, 21 Nov 2023 07:00:40 GMT  
		Size: 1.9 KB (1871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81cdb234e089dedc46386bbac8970166dab2d606288d8c1d426d4b4e617dc9dc`  
		Last Modified: Tue, 21 Nov 2023 07:00:41 GMT  
		Size: 1.5 KB (1476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fea6f1b6b2d8c666838e4a7ca42f2fbcfe498fc2a0eea88d569639836fa56140`  
		Last Modified: Tue, 21 Nov 2023 07:00:41 GMT  
		Size: 1.4 MB (1386332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fd0838894de2a37bd6487e6cf8b3c35ea2ee2e2793979871db8f810c871abd4`  
		Last Modified: Tue, 21 Nov 2023 07:00:41 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-fastcgi` - linux; arm64 variant v8

```console
$ docker pull adminer@sha256:84a893178255bde14cc03ffe152122623fe05eb3839e5f5bae856fb7da83814b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.3 MB (94348838 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b1d17ed2083c8a28275848906f461bdfdb42e15994ac21d9a62087dc6d034d2`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:13 GMT
ADD file:614987b9855939825ad2383e7bacbf14ea208d74906982bba3a67126702c8371 in / 
# Tue, 21 Nov 2023 06:27:13 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 10:22:26 GMT
STOPSIGNAL SIGINT
# Tue, 21 Nov 2023 10:22:43 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 10:22:44 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 21 Nov 2023 10:23:00 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Tue, 21 Nov 2023 10:23:00 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 21 Nov 2023 10:23:00 GMT
WORKDIR /var/www/html
# Tue, 21 Nov 2023 10:23:00 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 21 Nov 2023 10:23:00 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 21 Nov 2023 10:23:00 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 21 Nov 2023 10:23:01 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 21 Nov 2023 10:23:10 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Nov 2023 10:23:11 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 21 Nov 2023 10:23:11 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 21 Nov 2023 10:23:11 GMT
USER adminer
# Tue, 21 Nov 2023 10:23:11 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:bbf382c14c7b19b81c612f639e09e6a7b04eccd4481d0abac48b8ace9faae3b3`  
		Last Modified: Tue, 21 Nov 2023 06:30:47 GMT  
		Size: 53.7 MB (53707872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aa045892ab5d3693eb19355bad15725aa10139ceb2bfc2cb6141778f671e8e4`  
		Last Modified: Tue, 21 Nov 2023 10:23:29 GMT  
		Size: 39.2 MB (39247701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d77bfaecae2cacef431f4d68d17c26be0ab2300b5dfee893959aaae0c6427677`  
		Last Modified: Tue, 21 Nov 2023 10:23:21 GMT  
		Size: 386.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0caf62f5f6228f681c738a20ff40e768d645f553295e9a804e07c9983f280b5`  
		Last Modified: Tue, 21 Nov 2023 10:23:46 GMT  
		Size: 2.7 KB (2705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2df7041a632dc747d7c856a4b14a181da3e49fb1fb8e613f35a8b25404cb7269`  
		Last Modified: Tue, 21 Nov 2023 10:23:46 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c1e97ecf3d9ca77aee6de698d163482237c5a78acbe0e5ff1e47768d6e3fcb6`  
		Last Modified: Tue, 21 Nov 2023 10:23:46 GMT  
		Size: 1.5 KB (1477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce1ef470c48dc65a0917a06d12f3b23a206308eedf67bb228f570870947eb345`  
		Last Modified: Tue, 21 Nov 2023 10:23:47 GMT  
		Size: 1.4 MB (1386324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9363d2b46e93f744f02df5f1ad6d68e5d6ec8debff805842925426c2c0853d95`  
		Last Modified: Tue, 21 Nov 2023 10:23:46 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-fastcgi` - linux; 386

```console
$ docker pull adminer@sha256:063600a67051477eb2d252722e908e12954e92aa2f1103c08bc6ec0c98c81900
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.0 MB (97001696 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9faffd6534bfd19c55ba87d0ea06c0dec17f32f96aaf19d3d273080350957b57`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Tue, 21 Nov 2023 04:40:03 GMT
ADD file:54170328827ccc52692c964f0c45a65ed6efdf39897f2c226672fdf526f3c412 in / 
# Tue, 21 Nov 2023 04:40:04 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 15:41:51 GMT
STOPSIGNAL SIGINT
# Tue, 21 Nov 2023 15:42:20 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 15:42:21 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 21 Nov 2023 15:42:40 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Tue, 21 Nov 2023 15:42:40 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 21 Nov 2023 15:42:41 GMT
WORKDIR /var/www/html
# Tue, 21 Nov 2023 15:42:41 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 21 Nov 2023 15:42:41 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 21 Nov 2023 15:42:41 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 21 Nov 2023 15:42:41 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 21 Nov 2023 15:42:56 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Nov 2023 15:42:56 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 21 Nov 2023 15:42:56 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 21 Nov 2023 15:42:56 GMT
USER adminer
# Tue, 21 Nov 2023 15:42:56 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:e33c1468a29e45636d4d9529b663048f7e8aa83ff428eb0681253bd4200e23ec`  
		Last Modified: Tue, 21 Nov 2023 04:44:57 GMT  
		Size: 56.0 MB (56046301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8137e600c481ac4ed29cae88512a113a2eadcc1d26e72628216670ef4f61ba30`  
		Last Modified: Tue, 21 Nov 2023 15:43:16 GMT  
		Size: 39.6 MB (39562172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e42a8870a081f3a4ab284980034bebec6585740c88e4c40ae98b2e1fa9955f5`  
		Last Modified: Tue, 21 Nov 2023 15:43:05 GMT  
		Size: 392.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ea29f8bfe081038362130d161f4fce7184b04e8b23e4e6eb76012853b52eb29`  
		Last Modified: Tue, 21 Nov 2023 15:43:34 GMT  
		Size: 2.7 KB (2711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c61c47ded185575a69531bea47b571461b9b5a7dbe771c12d9a5351c2274616`  
		Last Modified: Tue, 21 Nov 2023 15:43:34 GMT  
		Size: 1.9 KB (1867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce13699c4877d6078a5c0d0891b3ab176e81a19c03c25322e69a1da82443611a`  
		Last Modified: Tue, 21 Nov 2023 15:43:34 GMT  
		Size: 1.5 KB (1480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:467cdaa3b936c126690238f64a0f87f1ea5c53e47ad6b7a300a08e68304b4c5e`  
		Last Modified: Tue, 21 Nov 2023 15:43:34 GMT  
		Size: 1.4 MB (1386283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08c8258bd975965d721bb178e601818437b2ec83ecf04991a03e7ac42e8262f1`  
		Last Modified: Tue, 21 Nov 2023 15:43:34 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-fastcgi` - linux; mips64le

```console
$ docker pull adminer@sha256:a764c136226771f05874d428d466ab7617443109af05761f5a301d774d3d78ef
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.6 MB (92637624 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6dcb8d7570466b2e24f152459f05444501a2db6bec81dd770f36a922da335bf3`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Tue, 21 Nov 2023 04:10:25 GMT
ADD file:dbfc3d226166089c4db0c154fdcea8049b8758c6812f1c397dec1444985e8557 in / 
# Tue, 21 Nov 2023 04:10:31 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 12:14:44 GMT
STOPSIGNAL SIGINT
# Tue, 21 Nov 2023 12:16:43 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 12:16:50 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 21 Nov 2023 12:18:45 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Tue, 21 Nov 2023 12:18:52 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 21 Nov 2023 12:18:55 GMT
WORKDIR /var/www/html
# Tue, 21 Nov 2023 12:18:59 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 21 Nov 2023 12:19:02 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 21 Nov 2023 12:19:05 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 21 Nov 2023 12:19:09 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 21 Nov 2023 12:20:00 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Nov 2023 12:20:03 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 21 Nov 2023 12:20:06 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 21 Nov 2023 12:20:10 GMT
USER adminer
# Tue, 21 Nov 2023 12:20:13 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:ca31218601e95f4aafae0dcadda7600aeb04db374e1e829d5c123f8033ba3472`  
		Last Modified: Tue, 21 Nov 2023 04:21:21 GMT  
		Size: 53.3 MB (53289162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d172a1ce4463b8a1bb14b88d9f7c98a7f06f260dfc2849e77f3d41be6d17db9`  
		Last Modified: Tue, 21 Nov 2023 12:21:00 GMT  
		Size: 38.0 MB (37954467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbd3b039fbc0efa77466cfb045c80c120d45355cf2db0dd6533eeb1cee6296e1`  
		Last Modified: Tue, 21 Nov 2023 12:20:33 GMT  
		Size: 394.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:873ce81c2a5a659c6ba90c59b5fdd1a3c215439a655c8efe1b62a042ba6dc956`  
		Last Modified: Tue, 21 Nov 2023 12:21:19 GMT  
		Size: 2.7 KB (2714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:046c3c9cda84191a448b5676717eb2efd43aa616bd1a7936fd1ffa7333fe414d`  
		Last Modified: Tue, 21 Nov 2023 12:21:19 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d5fb1a0ccda92972577970b93a35e31e87aca9efdf320fe33d64fbb50e5f5be`  
		Last Modified: Tue, 21 Nov 2023 12:21:19 GMT  
		Size: 1.5 KB (1479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16f226ce3836498318ee4d4f1573efc49e08a2a6cdfd7403a3089f66f24194f3`  
		Last Modified: Tue, 21 Nov 2023 12:21:20 GMT  
		Size: 1.4 MB (1387178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc2ef37541c711003007d218f46c929098bfda475d45d9ced2d3700246c0d143`  
		Last Modified: Tue, 21 Nov 2023 12:21:19 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-fastcgi` - linux; ppc64le

```console
$ docker pull adminer@sha256:988a50cb007ef650a43dfb195f4730d2268d36b717db2cdbc731914c725ee8df
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.3 MB (101268149 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f2e2a636068dd83fb84a9bcecd6a718528598da747489d7573b02bdfa6f20140`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Tue, 21 Nov 2023 04:24:26 GMT
ADD file:c21c2b6cb3f9bdf6cc3641e9ebf810a461174480c6cd1c25515cf9fce4aa2143 in / 
# Tue, 21 Nov 2023 04:24:30 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 06:49:59 GMT
STOPSIGNAL SIGINT
# Tue, 21 Nov 2023 06:50:40 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 06:50:42 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 21 Nov 2023 06:51:10 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Tue, 21 Nov 2023 06:51:11 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 21 Nov 2023 06:51:11 GMT
WORKDIR /var/www/html
# Tue, 21 Nov 2023 06:51:12 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 21 Nov 2023 06:51:12 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 21 Nov 2023 06:51:12 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 21 Nov 2023 06:51:13 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 21 Nov 2023 06:51:30 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Nov 2023 06:51:30 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 21 Nov 2023 06:51:30 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 21 Nov 2023 06:51:31 GMT
USER adminer
# Tue, 21 Nov 2023 06:51:31 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:23ebe74b854f8f6e2671f4c8cc147a6925fb7d929ce5898f7ca2af9781bf7d38`  
		Last Modified: Tue, 21 Nov 2023 04:29:21 GMT  
		Size: 58.9 MB (58929678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa255108512a37e57b2fdf827a0fdb4e3783a0649fb80ecdd431d4921dd6761c`  
		Last Modified: Tue, 21 Nov 2023 06:51:51 GMT  
		Size: 40.9 MB (40945122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5862ce535fc870ad9665c04e9816effde44c5f4469bc852265ba0bfe11ad7001`  
		Last Modified: Tue, 21 Nov 2023 06:51:41 GMT  
		Size: 391.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eb07c0427e1d513dc1c2e122ef9b33a7ce04c7f6e7ac25eb3cdc16b7c4f3dd0`  
		Last Modified: Tue, 21 Nov 2023 06:52:10 GMT  
		Size: 2.7 KB (2709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e1a3baf382e8ecd698319193729a0416bcdcbe069383e956a41029751483ab8`  
		Last Modified: Tue, 21 Nov 2023 06:52:10 GMT  
		Size: 1.9 KB (1878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd36769ccabc572d519d259cd2369096462f35a823d2817c593ce165f30f690b`  
		Last Modified: Tue, 21 Nov 2023 06:52:10 GMT  
		Size: 1.5 KB (1480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e35256cd8ee36eeca9a95cc2fc4ad45b213f5025c0d7211c00f76beae6c7a0bd`  
		Last Modified: Tue, 21 Nov 2023 06:52:11 GMT  
		Size: 1.4 MB (1386400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:417adc53867ad9b9d99a43bc9736c1285bc9af029e2938bd516928b92cad7093`  
		Last Modified: Tue, 21 Nov 2023 06:52:10 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-fastcgi` - linux; s390x

```console
$ docker pull adminer@sha256:8920ecc20283083c9296766b19c975eabf1764eecadbcd7b97ed7bb11e30921e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.7 MB (93711989 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33df00454cb56b58abb106b0161ca460cdce0f5d1f8162177becb869dde24b99`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Tue, 21 Nov 2023 05:04:52 GMT
ADD file:b0a8fd50925b3555a0c10177e65551cae288917f9bad8fb4728ec83cc0765afe in / 
# Tue, 21 Nov 2023 05:05:01 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 06:04:07 GMT
STOPSIGNAL SIGINT
# Tue, 21 Nov 2023 06:04:29 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 06:04:35 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 21 Nov 2023 06:05:00 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Tue, 21 Nov 2023 06:05:00 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 21 Nov 2023 06:05:00 GMT
WORKDIR /var/www/html
# Tue, 21 Nov 2023 06:05:01 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 21 Nov 2023 06:05:01 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 21 Nov 2023 06:05:01 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 21 Nov 2023 06:05:01 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 21 Nov 2023 06:05:11 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Nov 2023 06:05:11 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 21 Nov 2023 06:05:11 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 21 Nov 2023 06:05:12 GMT
USER adminer
# Tue, 21 Nov 2023 06:05:12 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:9488c1539560318cb45b39150f91e365b928c0a246788663f5c72d185864bd3e`  
		Last Modified: Tue, 21 Nov 2023 05:10:34 GMT  
		Size: 53.3 MB (53296396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09efec12dc42685e3fe1693d18bc42d61971044de30a99ee3f044d942e93a470`  
		Last Modified: Tue, 21 Nov 2023 06:05:38 GMT  
		Size: 39.0 MB (39022251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d211af034ddf5d1e81df73b8d237d1c15d165b5443c533eedbeecc5659d4d4b`  
		Last Modified: Tue, 21 Nov 2023 06:05:31 GMT  
		Size: 393.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32f1b2d24e5fca07170540193831c2b4e39ddb10d4fc7736e631b2aa11ed601a`  
		Last Modified: Tue, 21 Nov 2023 06:05:48 GMT  
		Size: 2.7 KB (2711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6439585d05cece3d9af2be5ecb1d12bf8e78e1a23a419fb2f49451ede72e90ba`  
		Last Modified: Tue, 21 Nov 2023 06:05:48 GMT  
		Size: 1.9 KB (1879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aea2cdf22e5a5de0f7b5cc6c97c9c03a8fe82113a1d7d5153a55592fdf09568`  
		Last Modified: Tue, 21 Nov 2023 06:05:48 GMT  
		Size: 1.5 KB (1479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:922a0d106738cf725844ac8a3a5ef1352d0048149982aee61fe3d0f67bb8a041`  
		Last Modified: Tue, 21 Nov 2023 06:05:48 GMT  
		Size: 1.4 MB (1386389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:791aaf97ba65859a96b769218ea3ab780b809cc6bcacb784b88c24756e99ef6b`  
		Last Modified: Tue, 21 Nov 2023 06:05:48 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `adminer:4-standalone`

```console
$ docker pull adminer@sha256:0ce7583815dabdd9f560ee0afed630ecb33df6756f4b66c85c197011559a0248
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
$ docker pull adminer@sha256:78d95e4c7a6cfb584a500e0e8ca7db956ab9ff1cd4b3239306b330c2637ecfa2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.9 MB (95942047 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7554c8e10d81e451e656e73d613de4f9c885b91255f46a2fdc03ccf275a1d449`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:46 GMT
ADD file:71543995e4d314b0c86da5ddf8e0cb74649767d30b3e5b6261360de354f0567b in / 
# Tue, 21 Nov 2023 05:21:46 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 09:49:06 GMT
STOPSIGNAL SIGINT
# Tue, 21 Nov 2023 09:49:25 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 09:49:26 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 21 Nov 2023 09:49:27 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 21 Nov 2023 09:49:27 GMT
WORKDIR /var/www/html
# Tue, 21 Nov 2023 09:49:27 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 21 Nov 2023 09:49:27 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 21 Nov 2023 09:49:27 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 21 Nov 2023 09:49:27 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 21 Nov 2023 09:49:39 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Nov 2023 09:49:39 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 21 Nov 2023 09:49:39 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 21 Nov 2023 09:49:39 GMT
USER adminer
# Tue, 21 Nov 2023 09:49:39 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Tue, 21 Nov 2023 09:49:39 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:d1da99c2f14827498c4a9bb3623ae909b44564bdabad1802f064169069df81fb`  
		Last Modified: Tue, 21 Nov 2023 05:26:17 GMT  
		Size: 55.1 MB (55057903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d7c776bdbb7e1224dedbc306fec7eb6e3842bd895a396927c36fa7f434312a3`  
		Last Modified: Tue, 21 Nov 2023 09:50:18 GMT  
		Size: 39.5 MB (39493553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:987d0f042e915521e94497a8e40892d4ec0532bd7641920df5ace1000310d793`  
		Last Modified: Tue, 21 Nov 2023 09:50:10 GMT  
		Size: 389.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb163dc8650b5fde5c72f76b8937b3c38d3dd4c7a2922d7b6f95a0890070c4d9`  
		Last Modified: Tue, 21 Nov 2023 09:50:10 GMT  
		Size: 1.9 KB (1878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98b256c86f3d5b1eab91122ae075d7b3b15d1185ebe1cc10a8b4d2fb6f2bdf5f`  
		Last Modified: Tue, 21 Nov 2023 09:50:10 GMT  
		Size: 1.5 KB (1480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7952b9a84b1867112d08313ef023ee4917d7bbd0f91f4d8ae3ce1b17376d345e`  
		Last Modified: Tue, 21 Nov 2023 09:50:11 GMT  
		Size: 1.4 MB (1386353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77cf83a8d79b963388e7d18d6836ac44d7832d08fa39ab46ba57f0c92e48e1f2`  
		Last Modified: Tue, 21 Nov 2023 09:50:10 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-standalone` - linux; arm variant v5

```console
$ docker pull adminer@sha256:f6bb8e720054e43d3bc65a163e9fc4146ce4c215db05216f56be5cbac7428eb7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.2 MB (91205860 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9bd45b72f483757bdbd0f31b96e08578a127cc80966526aa0a9a897f5012203`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Tue, 21 Nov 2023 05:01:00 GMT
ADD file:a5c8bd4b0873bd9ad0402143df41b5fd89c50bd24bb071b7d010919e189d88f9 in / 
# Tue, 21 Nov 2023 05:01:00 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 05:46:09 GMT
STOPSIGNAL SIGINT
# Tue, 21 Nov 2023 05:46:38 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 05:46:39 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 21 Nov 2023 05:46:40 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 21 Nov 2023 05:46:40 GMT
WORKDIR /var/www/html
# Tue, 21 Nov 2023 05:46:40 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 21 Nov 2023 05:46:40 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 21 Nov 2023 05:46:40 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 21 Nov 2023 05:46:40 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 21 Nov 2023 05:46:55 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Nov 2023 05:46:55 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 21 Nov 2023 05:46:55 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 21 Nov 2023 05:46:55 GMT
USER adminer
# Tue, 21 Nov 2023 05:46:55 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Tue, 21 Nov 2023 05:46:55 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:7378d71ea16926a061a2edbf0eb3dd13563fcb3ba9cf139c25e8334b36db1adf`  
		Last Modified: Tue, 21 Nov 2023 05:04:15 GMT  
		Size: 52.6 MB (52562921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cde673c33e7bfa6c04aeb9e184923984b648ae971715981d598aca5162e3c911`  
		Last Modified: Tue, 21 Nov 2023 05:47:34 GMT  
		Size: 37.3 MB (37252430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4fee5ad01a4adcbc52d632521a683e83dd44bb905a3048fc20faaa96d58f747`  
		Last Modified: Tue, 21 Nov 2023 05:47:25 GMT  
		Size: 386.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:062df034c3a9a14a736fb1733f5f91b8c5cad9974f6b67df85f488a45026f47c`  
		Last Modified: Tue, 21 Nov 2023 05:47:24 GMT  
		Size: 1.9 KB (1869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:610f64ab71d9f5c7abad4551870c223a9b95603025384ef1e7a85f624f0b0467`  
		Last Modified: Tue, 21 Nov 2023 05:47:24 GMT  
		Size: 1.5 KB (1481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59cca3ff7ed68079f673662534d292a264aa5c1d7d4358251d8e25f21faa9f94`  
		Last Modified: Tue, 21 Nov 2023 05:47:25 GMT  
		Size: 1.4 MB (1386281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:753ad2913e083c1b5cb5b06853944934450629b0451d408743ddffc1f4c0a843`  
		Last Modified: Tue, 21 Nov 2023 05:47:24 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-standalone` - linux; arm variant v7

```console
$ docker pull adminer@sha256:6faef276799d02bdd9abf0ba022b692fd46f8144584adcfa771a76d225131045
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.8 MB (87796870 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9bb280f29bbaaa440662c6cbd26fabd7313fb299195b0ff2ca0cc22cff61f1ab`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Tue, 21 Nov 2023 03:57:54 GMT
ADD file:ed8d88d0476fad37879d872d61d05a8cffff35609566f080f78bb882d1bae26b in / 
# Tue, 21 Nov 2023 03:57:54 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 06:58:56 GMT
STOPSIGNAL SIGINT
# Tue, 21 Nov 2023 06:59:20 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 06:59:21 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 21 Nov 2023 06:59:21 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 21 Nov 2023 06:59:21 GMT
WORKDIR /var/www/html
# Tue, 21 Nov 2023 06:59:21 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 21 Nov 2023 06:59:21 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 21 Nov 2023 06:59:21 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 21 Nov 2023 06:59:22 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 21 Nov 2023 06:59:37 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Nov 2023 06:59:37 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 21 Nov 2023 06:59:37 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 21 Nov 2023 06:59:37 GMT
USER adminer
# Tue, 21 Nov 2023 06:59:37 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Tue, 21 Nov 2023 06:59:37 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:1dac19092a737e476f9b096fe28463512ae21c4f596dd2f8b84d62530416dffe`  
		Last Modified: Tue, 21 Nov 2023 04:02:11 GMT  
		Size: 50.2 MB (50215653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2f8153e5d67bc5a0049a12eb2430f50747238b7d4023cacdfc5dad9cdbd244a`  
		Last Modified: Tue, 21 Nov 2023 07:00:24 GMT  
		Size: 36.2 MB (36190640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ea62b864a160dff0b693d9397a8b84a1bc65e8e381b223294a8ac5ac8c68b8a`  
		Last Modified: Tue, 21 Nov 2023 07:00:15 GMT  
		Size: 393.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e2dd6fa8973e47e4cce58445b7207793f22b2371aa58678dc17d4172eac0b32`  
		Last Modified: Tue, 21 Nov 2023 07:00:15 GMT  
		Size: 1.9 KB (1871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4d33015217bf866b0d2c44cd29bf71617469b2e87e38eb15795aa3a293c83fa`  
		Last Modified: Tue, 21 Nov 2023 07:00:16 GMT  
		Size: 1.5 KB (1478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24ee8e39b9683ef6aa34033169655e5585db29d9557c0e1eb9aa117e1c771047`  
		Last Modified: Tue, 21 Nov 2023 07:00:16 GMT  
		Size: 1.4 MB (1386341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c14859802a2676aa6a511bbd06ce80a759e38e94927cd4d4b60dd202568ef5b`  
		Last Modified: Tue, 21 Nov 2023 07:00:15 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-standalone` - linux; arm64 variant v8

```console
$ docker pull adminer@sha256:e5fda74f5900f3c7ef8f74bda0392b45089f33f56374326bb331d8db26eb8b41
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.3 MB (94346130 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ccf82dd602ee08aa22718c108fcbcedbebb819a09c86b9f0fe8f2c1737bd08a7`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:13 GMT
ADD file:614987b9855939825ad2383e7bacbf14ea208d74906982bba3a67126702c8371 in / 
# Tue, 21 Nov 2023 06:27:13 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 10:22:26 GMT
STOPSIGNAL SIGINT
# Tue, 21 Nov 2023 10:22:43 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 10:22:44 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 21 Nov 2023 10:22:44 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 21 Nov 2023 10:22:44 GMT
WORKDIR /var/www/html
# Tue, 21 Nov 2023 10:22:44 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 21 Nov 2023 10:22:44 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 21 Nov 2023 10:22:45 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 21 Nov 2023 10:22:45 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 21 Nov 2023 10:22:54 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Nov 2023 10:22:54 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 21 Nov 2023 10:22:54 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 21 Nov 2023 10:22:54 GMT
USER adminer
# Tue, 21 Nov 2023 10:22:55 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Tue, 21 Nov 2023 10:22:55 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:bbf382c14c7b19b81c612f639e09e6a7b04eccd4481d0abac48b8ace9faae3b3`  
		Last Modified: Tue, 21 Nov 2023 06:30:47 GMT  
		Size: 53.7 MB (53707872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aa045892ab5d3693eb19355bad15725aa10139ceb2bfc2cb6141778f671e8e4`  
		Last Modified: Tue, 21 Nov 2023 10:23:29 GMT  
		Size: 39.2 MB (39247701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d77bfaecae2cacef431f4d68d17c26be0ab2300b5dfee893959aaae0c6427677`  
		Last Modified: Tue, 21 Nov 2023 10:23:21 GMT  
		Size: 386.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1364c7eb4b90daedaca80aff830c09309115f174a295c35ba7885c60557fa1e`  
		Last Modified: Tue, 21 Nov 2023 10:23:21 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:080b929d6ed912f11ed340726920967a938d3632641f4f86e15a30fc7b255888`  
		Last Modified: Tue, 21 Nov 2023 10:23:21 GMT  
		Size: 1.5 KB (1477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:633cfed53ab70b9e08d21a78973fc2a318d49c9cc54f3100604c9b91dd533c82`  
		Last Modified: Tue, 21 Nov 2023 10:23:22 GMT  
		Size: 1.4 MB (1386322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc610b080dd3b327bfe4b6ca8da59bc3a5555a295aff6c4f18d172f070b4e1ab`  
		Last Modified: Tue, 21 Nov 2023 10:23:21 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-standalone` - linux; 386

```console
$ docker pull adminer@sha256:173f2532a535a7780bffa43d6385797ba5335ab89832cb016cbb54cb0ab60fb2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.0 MB (96998974 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85b8488ee11e55b40364ca362184cc13095a7b83f1c1e65e524862cc27000db2`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Tue, 21 Nov 2023 04:40:03 GMT
ADD file:54170328827ccc52692c964f0c45a65ed6efdf39897f2c226672fdf526f3c412 in / 
# Tue, 21 Nov 2023 04:40:04 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 15:41:51 GMT
STOPSIGNAL SIGINT
# Tue, 21 Nov 2023 15:42:20 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 15:42:21 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 21 Nov 2023 15:42:22 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 21 Nov 2023 15:42:22 GMT
WORKDIR /var/www/html
# Tue, 21 Nov 2023 15:42:22 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 21 Nov 2023 15:42:22 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 21 Nov 2023 15:42:22 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 21 Nov 2023 15:42:22 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 21 Nov 2023 15:42:37 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Nov 2023 15:42:37 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 21 Nov 2023 15:42:37 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 21 Nov 2023 15:42:37 GMT
USER adminer
# Tue, 21 Nov 2023 15:42:37 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Tue, 21 Nov 2023 15:42:37 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:e33c1468a29e45636d4d9529b663048f7e8aa83ff428eb0681253bd4200e23ec`  
		Last Modified: Tue, 21 Nov 2023 04:44:57 GMT  
		Size: 56.0 MB (56046301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8137e600c481ac4ed29cae88512a113a2eadcc1d26e72628216670ef4f61ba30`  
		Last Modified: Tue, 21 Nov 2023 15:43:16 GMT  
		Size: 39.6 MB (39562172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e42a8870a081f3a4ab284980034bebec6585740c88e4c40ae98b2e1fa9955f5`  
		Last Modified: Tue, 21 Nov 2023 15:43:05 GMT  
		Size: 392.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48c728479be5016dacc84b6c0c244f327eff896df6a326af2826d6ad4c5387b6`  
		Last Modified: Tue, 21 Nov 2023 15:43:05 GMT  
		Size: 1.9 KB (1870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1000dcb7b3ee07a4d8a46142cda4b99b13051577e48599f89d62c8fd8c7e61a8`  
		Last Modified: Tue, 21 Nov 2023 15:43:05 GMT  
		Size: 1.5 KB (1482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d8473e68cd9a1e0940ff9bb80857e7d32bfde252766cc39fc1c3566222b0c1c`  
		Last Modified: Tue, 21 Nov 2023 15:43:06 GMT  
		Size: 1.4 MB (1386265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d7609e79a7e8443050102286e60b2022e9f3447043db395cabb7e2ad151b1e0`  
		Last Modified: Tue, 21 Nov 2023 15:43:05 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-standalone` - linux; mips64le

```console
$ docker pull adminer@sha256:84b1c19875f37b42946db21b87c80b8f8d9d9c7392eff0a7a065cf6d5fe769b2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.6 MB (92634921 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6454361a51d8f0d5781cd1854359c6b0812cc29466f516dd6386754b3583699`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Tue, 21 Nov 2023 04:10:25 GMT
ADD file:dbfc3d226166089c4db0c154fdcea8049b8758c6812f1c397dec1444985e8557 in / 
# Tue, 21 Nov 2023 04:10:31 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 12:14:44 GMT
STOPSIGNAL SIGINT
# Tue, 21 Nov 2023 12:16:43 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 12:16:50 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 21 Nov 2023 12:16:57 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 21 Nov 2023 12:17:00 GMT
WORKDIR /var/www/html
# Tue, 21 Nov 2023 12:17:04 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 21 Nov 2023 12:17:07 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 21 Nov 2023 12:17:10 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 21 Nov 2023 12:17:14 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 21 Nov 2023 12:18:08 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Nov 2023 12:18:11 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 21 Nov 2023 12:18:14 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 21 Nov 2023 12:18:17 GMT
USER adminer
# Tue, 21 Nov 2023 12:18:21 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Tue, 21 Nov 2023 12:18:24 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:ca31218601e95f4aafae0dcadda7600aeb04db374e1e829d5c123f8033ba3472`  
		Last Modified: Tue, 21 Nov 2023 04:21:21 GMT  
		Size: 53.3 MB (53289162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d172a1ce4463b8a1bb14b88d9f7c98a7f06f260dfc2849e77f3d41be6d17db9`  
		Last Modified: Tue, 21 Nov 2023 12:21:00 GMT  
		Size: 38.0 MB (37954467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbd3b039fbc0efa77466cfb045c80c120d45355cf2db0dd6533eeb1cee6296e1`  
		Last Modified: Tue, 21 Nov 2023 12:20:33 GMT  
		Size: 394.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bac97c667ed055993103f32b019a430a853a94eef6bf75086fda9949a9fd1d8`  
		Last Modified: Tue, 21 Nov 2023 12:20:34 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66eec20186701717a98146a63c5c8f88304d44243fe6f6505edf4d1135672446`  
		Last Modified: Tue, 21 Nov 2023 12:20:34 GMT  
		Size: 1.5 KB (1483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a56ddb348b2b13a6cac73829460bdcce2971790b6be59ac9da70b739453488b8`  
		Last Modified: Tue, 21 Nov 2023 12:20:34 GMT  
		Size: 1.4 MB (1387192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f922348b25af66b56cdd7a4863a9a120057afa01489fc9058cf7e975b198d05`  
		Last Modified: Tue, 21 Nov 2023 12:20:34 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-standalone` - linux; ppc64le

```console
$ docker pull adminer@sha256:3b96a3711e0e719557e514cb8870567e67ab545a7fe18b4feeca4e0e4c85d678
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.3 MB (101265448 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0c151160d019f74dfe13959cf16722a5172a0023a5f747201c90b752e001545`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Tue, 21 Nov 2023 04:24:26 GMT
ADD file:c21c2b6cb3f9bdf6cc3641e9ebf810a461174480c6cd1c25515cf9fce4aa2143 in / 
# Tue, 21 Nov 2023 04:24:30 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 06:49:59 GMT
STOPSIGNAL SIGINT
# Tue, 21 Nov 2023 06:50:40 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 06:50:42 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 21 Nov 2023 06:50:44 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 21 Nov 2023 06:50:44 GMT
WORKDIR /var/www/html
# Tue, 21 Nov 2023 06:50:44 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 21 Nov 2023 06:50:44 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 21 Nov 2023 06:50:45 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 21 Nov 2023 06:50:45 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 21 Nov 2023 06:51:03 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Nov 2023 06:51:03 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 21 Nov 2023 06:51:03 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 21 Nov 2023 06:51:03 GMT
USER adminer
# Tue, 21 Nov 2023 06:51:04 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Tue, 21 Nov 2023 06:51:04 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:23ebe74b854f8f6e2671f4c8cc147a6925fb7d929ce5898f7ca2af9781bf7d38`  
		Last Modified: Tue, 21 Nov 2023 04:29:21 GMT  
		Size: 58.9 MB (58929678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa255108512a37e57b2fdf827a0fdb4e3783a0649fb80ecdd431d4921dd6761c`  
		Last Modified: Tue, 21 Nov 2023 06:51:51 GMT  
		Size: 40.9 MB (40945122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5862ce535fc870ad9665c04e9816effde44c5f4469bc852265ba0bfe11ad7001`  
		Last Modified: Tue, 21 Nov 2023 06:51:41 GMT  
		Size: 391.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7204feb32d0a6fe6dd0348f7a8c2845b90b631ba893c08c48a724057c8a5e3d1`  
		Last Modified: Tue, 21 Nov 2023 06:51:41 GMT  
		Size: 1.9 KB (1879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb06eb196e5a191ad6e9d6d43052c2fd0f833100bf197c73f3f9c8df967003d1`  
		Last Modified: Tue, 21 Nov 2023 06:51:41 GMT  
		Size: 1.5 KB (1482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76df205e8013dede04db80018bebbabea233e0186671f2fd251fa440acde39ef`  
		Last Modified: Tue, 21 Nov 2023 06:51:41 GMT  
		Size: 1.4 MB (1386403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7099dfc32b7ad37a3cfe50e8aad19c609d5e9daf0535dd5cd0f853de87d0de8f`  
		Last Modified: Tue, 21 Nov 2023 06:51:41 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-standalone` - linux; s390x

```console
$ docker pull adminer@sha256:0832c83b0a0b564f962bc8f2f82974852bda2c876629b26a32e31e5b99e8fbc0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.7 MB (93709271 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72ed9e5473cf095c9f6c3263d8ff775ee9a240aa6597b921ebd51ec24f8978c1`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Tue, 21 Nov 2023 05:04:52 GMT
ADD file:b0a8fd50925b3555a0c10177e65551cae288917f9bad8fb4728ec83cc0765afe in / 
# Tue, 21 Nov 2023 05:05:01 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 06:04:07 GMT
STOPSIGNAL SIGINT
# Tue, 21 Nov 2023 06:04:29 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 06:04:35 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 21 Nov 2023 06:04:35 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 21 Nov 2023 06:04:36 GMT
WORKDIR /var/www/html
# Tue, 21 Nov 2023 06:04:36 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 21 Nov 2023 06:04:36 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 21 Nov 2023 06:04:36 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 21 Nov 2023 06:04:36 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 21 Nov 2023 06:04:45 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Nov 2023 06:04:46 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 21 Nov 2023 06:04:46 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 21 Nov 2023 06:04:46 GMT
USER adminer
# Tue, 21 Nov 2023 06:04:46 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Tue, 21 Nov 2023 06:04:47 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:9488c1539560318cb45b39150f91e365b928c0a246788663f5c72d185864bd3e`  
		Last Modified: Tue, 21 Nov 2023 05:10:34 GMT  
		Size: 53.3 MB (53296396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09efec12dc42685e3fe1693d18bc42d61971044de30a99ee3f044d942e93a470`  
		Last Modified: Tue, 21 Nov 2023 06:05:38 GMT  
		Size: 39.0 MB (39022251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d211af034ddf5d1e81df73b8d237d1c15d165b5443c533eedbeecc5659d4d4b`  
		Last Modified: Tue, 21 Nov 2023 06:05:31 GMT  
		Size: 393.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd2e9fc8bb5d1ec8686111ad3e20155b1ac539fc01b742c2318311374c9c3d29`  
		Last Modified: Tue, 21 Nov 2023 06:05:31 GMT  
		Size: 1.9 KB (1877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2acddcee94070eff9faaeaa170066fa650714281ae6b3094fc1d49c010f3902`  
		Last Modified: Tue, 21 Nov 2023 06:05:31 GMT  
		Size: 1.5 KB (1480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21ffbd0e004b4f2f9f75bdc6731ed7d644c91ee50221377d2ff00e82aa1f99b9`  
		Last Modified: Tue, 21 Nov 2023 06:05:31 GMT  
		Size: 1.4 MB (1386383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44baab47b2128777f4b94d45e4a91e7bd440dcb23e61b28ec31c8ac469b3cf40`  
		Last Modified: Tue, 21 Nov 2023 06:05:31 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `adminer:4.8.1`

```console
$ docker pull adminer@sha256:0ce7583815dabdd9f560ee0afed630ecb33df6756f4b66c85c197011559a0248
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
$ docker pull adminer@sha256:78d95e4c7a6cfb584a500e0e8ca7db956ab9ff1cd4b3239306b330c2637ecfa2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.9 MB (95942047 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7554c8e10d81e451e656e73d613de4f9c885b91255f46a2fdc03ccf275a1d449`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:46 GMT
ADD file:71543995e4d314b0c86da5ddf8e0cb74649767d30b3e5b6261360de354f0567b in / 
# Tue, 21 Nov 2023 05:21:46 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 09:49:06 GMT
STOPSIGNAL SIGINT
# Tue, 21 Nov 2023 09:49:25 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 09:49:26 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 21 Nov 2023 09:49:27 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 21 Nov 2023 09:49:27 GMT
WORKDIR /var/www/html
# Tue, 21 Nov 2023 09:49:27 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 21 Nov 2023 09:49:27 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 21 Nov 2023 09:49:27 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 21 Nov 2023 09:49:27 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 21 Nov 2023 09:49:39 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Nov 2023 09:49:39 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 21 Nov 2023 09:49:39 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 21 Nov 2023 09:49:39 GMT
USER adminer
# Tue, 21 Nov 2023 09:49:39 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Tue, 21 Nov 2023 09:49:39 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:d1da99c2f14827498c4a9bb3623ae909b44564bdabad1802f064169069df81fb`  
		Last Modified: Tue, 21 Nov 2023 05:26:17 GMT  
		Size: 55.1 MB (55057903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d7c776bdbb7e1224dedbc306fec7eb6e3842bd895a396927c36fa7f434312a3`  
		Last Modified: Tue, 21 Nov 2023 09:50:18 GMT  
		Size: 39.5 MB (39493553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:987d0f042e915521e94497a8e40892d4ec0532bd7641920df5ace1000310d793`  
		Last Modified: Tue, 21 Nov 2023 09:50:10 GMT  
		Size: 389.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb163dc8650b5fde5c72f76b8937b3c38d3dd4c7a2922d7b6f95a0890070c4d9`  
		Last Modified: Tue, 21 Nov 2023 09:50:10 GMT  
		Size: 1.9 KB (1878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98b256c86f3d5b1eab91122ae075d7b3b15d1185ebe1cc10a8b4d2fb6f2bdf5f`  
		Last Modified: Tue, 21 Nov 2023 09:50:10 GMT  
		Size: 1.5 KB (1480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7952b9a84b1867112d08313ef023ee4917d7bbd0f91f4d8ae3ce1b17376d345e`  
		Last Modified: Tue, 21 Nov 2023 09:50:11 GMT  
		Size: 1.4 MB (1386353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77cf83a8d79b963388e7d18d6836ac44d7832d08fa39ab46ba57f0c92e48e1f2`  
		Last Modified: Tue, 21 Nov 2023 09:50:10 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1` - linux; arm variant v5

```console
$ docker pull adminer@sha256:f6bb8e720054e43d3bc65a163e9fc4146ce4c215db05216f56be5cbac7428eb7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.2 MB (91205860 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9bd45b72f483757bdbd0f31b96e08578a127cc80966526aa0a9a897f5012203`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Tue, 21 Nov 2023 05:01:00 GMT
ADD file:a5c8bd4b0873bd9ad0402143df41b5fd89c50bd24bb071b7d010919e189d88f9 in / 
# Tue, 21 Nov 2023 05:01:00 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 05:46:09 GMT
STOPSIGNAL SIGINT
# Tue, 21 Nov 2023 05:46:38 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 05:46:39 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 21 Nov 2023 05:46:40 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 21 Nov 2023 05:46:40 GMT
WORKDIR /var/www/html
# Tue, 21 Nov 2023 05:46:40 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 21 Nov 2023 05:46:40 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 21 Nov 2023 05:46:40 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 21 Nov 2023 05:46:40 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 21 Nov 2023 05:46:55 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Nov 2023 05:46:55 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 21 Nov 2023 05:46:55 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 21 Nov 2023 05:46:55 GMT
USER adminer
# Tue, 21 Nov 2023 05:46:55 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Tue, 21 Nov 2023 05:46:55 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:7378d71ea16926a061a2edbf0eb3dd13563fcb3ba9cf139c25e8334b36db1adf`  
		Last Modified: Tue, 21 Nov 2023 05:04:15 GMT  
		Size: 52.6 MB (52562921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cde673c33e7bfa6c04aeb9e184923984b648ae971715981d598aca5162e3c911`  
		Last Modified: Tue, 21 Nov 2023 05:47:34 GMT  
		Size: 37.3 MB (37252430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4fee5ad01a4adcbc52d632521a683e83dd44bb905a3048fc20faaa96d58f747`  
		Last Modified: Tue, 21 Nov 2023 05:47:25 GMT  
		Size: 386.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:062df034c3a9a14a736fb1733f5f91b8c5cad9974f6b67df85f488a45026f47c`  
		Last Modified: Tue, 21 Nov 2023 05:47:24 GMT  
		Size: 1.9 KB (1869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:610f64ab71d9f5c7abad4551870c223a9b95603025384ef1e7a85f624f0b0467`  
		Last Modified: Tue, 21 Nov 2023 05:47:24 GMT  
		Size: 1.5 KB (1481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59cca3ff7ed68079f673662534d292a264aa5c1d7d4358251d8e25f21faa9f94`  
		Last Modified: Tue, 21 Nov 2023 05:47:25 GMT  
		Size: 1.4 MB (1386281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:753ad2913e083c1b5cb5b06853944934450629b0451d408743ddffc1f4c0a843`  
		Last Modified: Tue, 21 Nov 2023 05:47:24 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1` - linux; arm variant v7

```console
$ docker pull adminer@sha256:6faef276799d02bdd9abf0ba022b692fd46f8144584adcfa771a76d225131045
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.8 MB (87796870 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9bb280f29bbaaa440662c6cbd26fabd7313fb299195b0ff2ca0cc22cff61f1ab`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Tue, 21 Nov 2023 03:57:54 GMT
ADD file:ed8d88d0476fad37879d872d61d05a8cffff35609566f080f78bb882d1bae26b in / 
# Tue, 21 Nov 2023 03:57:54 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 06:58:56 GMT
STOPSIGNAL SIGINT
# Tue, 21 Nov 2023 06:59:20 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 06:59:21 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 21 Nov 2023 06:59:21 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 21 Nov 2023 06:59:21 GMT
WORKDIR /var/www/html
# Tue, 21 Nov 2023 06:59:21 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 21 Nov 2023 06:59:21 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 21 Nov 2023 06:59:21 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 21 Nov 2023 06:59:22 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 21 Nov 2023 06:59:37 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Nov 2023 06:59:37 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 21 Nov 2023 06:59:37 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 21 Nov 2023 06:59:37 GMT
USER adminer
# Tue, 21 Nov 2023 06:59:37 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Tue, 21 Nov 2023 06:59:37 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:1dac19092a737e476f9b096fe28463512ae21c4f596dd2f8b84d62530416dffe`  
		Last Modified: Tue, 21 Nov 2023 04:02:11 GMT  
		Size: 50.2 MB (50215653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2f8153e5d67bc5a0049a12eb2430f50747238b7d4023cacdfc5dad9cdbd244a`  
		Last Modified: Tue, 21 Nov 2023 07:00:24 GMT  
		Size: 36.2 MB (36190640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ea62b864a160dff0b693d9397a8b84a1bc65e8e381b223294a8ac5ac8c68b8a`  
		Last Modified: Tue, 21 Nov 2023 07:00:15 GMT  
		Size: 393.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e2dd6fa8973e47e4cce58445b7207793f22b2371aa58678dc17d4172eac0b32`  
		Last Modified: Tue, 21 Nov 2023 07:00:15 GMT  
		Size: 1.9 KB (1871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4d33015217bf866b0d2c44cd29bf71617469b2e87e38eb15795aa3a293c83fa`  
		Last Modified: Tue, 21 Nov 2023 07:00:16 GMT  
		Size: 1.5 KB (1478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24ee8e39b9683ef6aa34033169655e5585db29d9557c0e1eb9aa117e1c771047`  
		Last Modified: Tue, 21 Nov 2023 07:00:16 GMT  
		Size: 1.4 MB (1386341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c14859802a2676aa6a511bbd06ce80a759e38e94927cd4d4b60dd202568ef5b`  
		Last Modified: Tue, 21 Nov 2023 07:00:15 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1` - linux; arm64 variant v8

```console
$ docker pull adminer@sha256:e5fda74f5900f3c7ef8f74bda0392b45089f33f56374326bb331d8db26eb8b41
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.3 MB (94346130 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ccf82dd602ee08aa22718c108fcbcedbebb819a09c86b9f0fe8f2c1737bd08a7`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:13 GMT
ADD file:614987b9855939825ad2383e7bacbf14ea208d74906982bba3a67126702c8371 in / 
# Tue, 21 Nov 2023 06:27:13 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 10:22:26 GMT
STOPSIGNAL SIGINT
# Tue, 21 Nov 2023 10:22:43 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 10:22:44 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 21 Nov 2023 10:22:44 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 21 Nov 2023 10:22:44 GMT
WORKDIR /var/www/html
# Tue, 21 Nov 2023 10:22:44 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 21 Nov 2023 10:22:44 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 21 Nov 2023 10:22:45 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 21 Nov 2023 10:22:45 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 21 Nov 2023 10:22:54 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Nov 2023 10:22:54 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 21 Nov 2023 10:22:54 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 21 Nov 2023 10:22:54 GMT
USER adminer
# Tue, 21 Nov 2023 10:22:55 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Tue, 21 Nov 2023 10:22:55 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:bbf382c14c7b19b81c612f639e09e6a7b04eccd4481d0abac48b8ace9faae3b3`  
		Last Modified: Tue, 21 Nov 2023 06:30:47 GMT  
		Size: 53.7 MB (53707872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aa045892ab5d3693eb19355bad15725aa10139ceb2bfc2cb6141778f671e8e4`  
		Last Modified: Tue, 21 Nov 2023 10:23:29 GMT  
		Size: 39.2 MB (39247701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d77bfaecae2cacef431f4d68d17c26be0ab2300b5dfee893959aaae0c6427677`  
		Last Modified: Tue, 21 Nov 2023 10:23:21 GMT  
		Size: 386.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1364c7eb4b90daedaca80aff830c09309115f174a295c35ba7885c60557fa1e`  
		Last Modified: Tue, 21 Nov 2023 10:23:21 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:080b929d6ed912f11ed340726920967a938d3632641f4f86e15a30fc7b255888`  
		Last Modified: Tue, 21 Nov 2023 10:23:21 GMT  
		Size: 1.5 KB (1477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:633cfed53ab70b9e08d21a78973fc2a318d49c9cc54f3100604c9b91dd533c82`  
		Last Modified: Tue, 21 Nov 2023 10:23:22 GMT  
		Size: 1.4 MB (1386322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc610b080dd3b327bfe4b6ca8da59bc3a5555a295aff6c4f18d172f070b4e1ab`  
		Last Modified: Tue, 21 Nov 2023 10:23:21 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1` - linux; 386

```console
$ docker pull adminer@sha256:173f2532a535a7780bffa43d6385797ba5335ab89832cb016cbb54cb0ab60fb2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.0 MB (96998974 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85b8488ee11e55b40364ca362184cc13095a7b83f1c1e65e524862cc27000db2`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Tue, 21 Nov 2023 04:40:03 GMT
ADD file:54170328827ccc52692c964f0c45a65ed6efdf39897f2c226672fdf526f3c412 in / 
# Tue, 21 Nov 2023 04:40:04 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 15:41:51 GMT
STOPSIGNAL SIGINT
# Tue, 21 Nov 2023 15:42:20 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 15:42:21 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 21 Nov 2023 15:42:22 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 21 Nov 2023 15:42:22 GMT
WORKDIR /var/www/html
# Tue, 21 Nov 2023 15:42:22 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 21 Nov 2023 15:42:22 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 21 Nov 2023 15:42:22 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 21 Nov 2023 15:42:22 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 21 Nov 2023 15:42:37 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Nov 2023 15:42:37 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 21 Nov 2023 15:42:37 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 21 Nov 2023 15:42:37 GMT
USER adminer
# Tue, 21 Nov 2023 15:42:37 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Tue, 21 Nov 2023 15:42:37 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:e33c1468a29e45636d4d9529b663048f7e8aa83ff428eb0681253bd4200e23ec`  
		Last Modified: Tue, 21 Nov 2023 04:44:57 GMT  
		Size: 56.0 MB (56046301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8137e600c481ac4ed29cae88512a113a2eadcc1d26e72628216670ef4f61ba30`  
		Last Modified: Tue, 21 Nov 2023 15:43:16 GMT  
		Size: 39.6 MB (39562172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e42a8870a081f3a4ab284980034bebec6585740c88e4c40ae98b2e1fa9955f5`  
		Last Modified: Tue, 21 Nov 2023 15:43:05 GMT  
		Size: 392.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48c728479be5016dacc84b6c0c244f327eff896df6a326af2826d6ad4c5387b6`  
		Last Modified: Tue, 21 Nov 2023 15:43:05 GMT  
		Size: 1.9 KB (1870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1000dcb7b3ee07a4d8a46142cda4b99b13051577e48599f89d62c8fd8c7e61a8`  
		Last Modified: Tue, 21 Nov 2023 15:43:05 GMT  
		Size: 1.5 KB (1482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d8473e68cd9a1e0940ff9bb80857e7d32bfde252766cc39fc1c3566222b0c1c`  
		Last Modified: Tue, 21 Nov 2023 15:43:06 GMT  
		Size: 1.4 MB (1386265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d7609e79a7e8443050102286e60b2022e9f3447043db395cabb7e2ad151b1e0`  
		Last Modified: Tue, 21 Nov 2023 15:43:05 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1` - linux; mips64le

```console
$ docker pull adminer@sha256:84b1c19875f37b42946db21b87c80b8f8d9d9c7392eff0a7a065cf6d5fe769b2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.6 MB (92634921 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6454361a51d8f0d5781cd1854359c6b0812cc29466f516dd6386754b3583699`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Tue, 21 Nov 2023 04:10:25 GMT
ADD file:dbfc3d226166089c4db0c154fdcea8049b8758c6812f1c397dec1444985e8557 in / 
# Tue, 21 Nov 2023 04:10:31 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 12:14:44 GMT
STOPSIGNAL SIGINT
# Tue, 21 Nov 2023 12:16:43 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 12:16:50 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 21 Nov 2023 12:16:57 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 21 Nov 2023 12:17:00 GMT
WORKDIR /var/www/html
# Tue, 21 Nov 2023 12:17:04 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 21 Nov 2023 12:17:07 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 21 Nov 2023 12:17:10 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 21 Nov 2023 12:17:14 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 21 Nov 2023 12:18:08 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Nov 2023 12:18:11 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 21 Nov 2023 12:18:14 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 21 Nov 2023 12:18:17 GMT
USER adminer
# Tue, 21 Nov 2023 12:18:21 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Tue, 21 Nov 2023 12:18:24 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:ca31218601e95f4aafae0dcadda7600aeb04db374e1e829d5c123f8033ba3472`  
		Last Modified: Tue, 21 Nov 2023 04:21:21 GMT  
		Size: 53.3 MB (53289162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d172a1ce4463b8a1bb14b88d9f7c98a7f06f260dfc2849e77f3d41be6d17db9`  
		Last Modified: Tue, 21 Nov 2023 12:21:00 GMT  
		Size: 38.0 MB (37954467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbd3b039fbc0efa77466cfb045c80c120d45355cf2db0dd6533eeb1cee6296e1`  
		Last Modified: Tue, 21 Nov 2023 12:20:33 GMT  
		Size: 394.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bac97c667ed055993103f32b019a430a853a94eef6bf75086fda9949a9fd1d8`  
		Last Modified: Tue, 21 Nov 2023 12:20:34 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66eec20186701717a98146a63c5c8f88304d44243fe6f6505edf4d1135672446`  
		Last Modified: Tue, 21 Nov 2023 12:20:34 GMT  
		Size: 1.5 KB (1483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a56ddb348b2b13a6cac73829460bdcce2971790b6be59ac9da70b739453488b8`  
		Last Modified: Tue, 21 Nov 2023 12:20:34 GMT  
		Size: 1.4 MB (1387192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f922348b25af66b56cdd7a4863a9a120057afa01489fc9058cf7e975b198d05`  
		Last Modified: Tue, 21 Nov 2023 12:20:34 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1` - linux; ppc64le

```console
$ docker pull adminer@sha256:3b96a3711e0e719557e514cb8870567e67ab545a7fe18b4feeca4e0e4c85d678
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.3 MB (101265448 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0c151160d019f74dfe13959cf16722a5172a0023a5f747201c90b752e001545`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Tue, 21 Nov 2023 04:24:26 GMT
ADD file:c21c2b6cb3f9bdf6cc3641e9ebf810a461174480c6cd1c25515cf9fce4aa2143 in / 
# Tue, 21 Nov 2023 04:24:30 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 06:49:59 GMT
STOPSIGNAL SIGINT
# Tue, 21 Nov 2023 06:50:40 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 06:50:42 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 21 Nov 2023 06:50:44 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 21 Nov 2023 06:50:44 GMT
WORKDIR /var/www/html
# Tue, 21 Nov 2023 06:50:44 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 21 Nov 2023 06:50:44 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 21 Nov 2023 06:50:45 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 21 Nov 2023 06:50:45 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 21 Nov 2023 06:51:03 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Nov 2023 06:51:03 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 21 Nov 2023 06:51:03 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 21 Nov 2023 06:51:03 GMT
USER adminer
# Tue, 21 Nov 2023 06:51:04 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Tue, 21 Nov 2023 06:51:04 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:23ebe74b854f8f6e2671f4c8cc147a6925fb7d929ce5898f7ca2af9781bf7d38`  
		Last Modified: Tue, 21 Nov 2023 04:29:21 GMT  
		Size: 58.9 MB (58929678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa255108512a37e57b2fdf827a0fdb4e3783a0649fb80ecdd431d4921dd6761c`  
		Last Modified: Tue, 21 Nov 2023 06:51:51 GMT  
		Size: 40.9 MB (40945122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5862ce535fc870ad9665c04e9816effde44c5f4469bc852265ba0bfe11ad7001`  
		Last Modified: Tue, 21 Nov 2023 06:51:41 GMT  
		Size: 391.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7204feb32d0a6fe6dd0348f7a8c2845b90b631ba893c08c48a724057c8a5e3d1`  
		Last Modified: Tue, 21 Nov 2023 06:51:41 GMT  
		Size: 1.9 KB (1879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb06eb196e5a191ad6e9d6d43052c2fd0f833100bf197c73f3f9c8df967003d1`  
		Last Modified: Tue, 21 Nov 2023 06:51:41 GMT  
		Size: 1.5 KB (1482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76df205e8013dede04db80018bebbabea233e0186671f2fd251fa440acde39ef`  
		Last Modified: Tue, 21 Nov 2023 06:51:41 GMT  
		Size: 1.4 MB (1386403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7099dfc32b7ad37a3cfe50e8aad19c609d5e9daf0535dd5cd0f853de87d0de8f`  
		Last Modified: Tue, 21 Nov 2023 06:51:41 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1` - linux; s390x

```console
$ docker pull adminer@sha256:0832c83b0a0b564f962bc8f2f82974852bda2c876629b26a32e31e5b99e8fbc0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.7 MB (93709271 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72ed9e5473cf095c9f6c3263d8ff775ee9a240aa6597b921ebd51ec24f8978c1`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Tue, 21 Nov 2023 05:04:52 GMT
ADD file:b0a8fd50925b3555a0c10177e65551cae288917f9bad8fb4728ec83cc0765afe in / 
# Tue, 21 Nov 2023 05:05:01 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 06:04:07 GMT
STOPSIGNAL SIGINT
# Tue, 21 Nov 2023 06:04:29 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 06:04:35 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 21 Nov 2023 06:04:35 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 21 Nov 2023 06:04:36 GMT
WORKDIR /var/www/html
# Tue, 21 Nov 2023 06:04:36 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 21 Nov 2023 06:04:36 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 21 Nov 2023 06:04:36 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 21 Nov 2023 06:04:36 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 21 Nov 2023 06:04:45 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Nov 2023 06:04:46 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 21 Nov 2023 06:04:46 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 21 Nov 2023 06:04:46 GMT
USER adminer
# Tue, 21 Nov 2023 06:04:46 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Tue, 21 Nov 2023 06:04:47 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:9488c1539560318cb45b39150f91e365b928c0a246788663f5c72d185864bd3e`  
		Last Modified: Tue, 21 Nov 2023 05:10:34 GMT  
		Size: 53.3 MB (53296396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09efec12dc42685e3fe1693d18bc42d61971044de30a99ee3f044d942e93a470`  
		Last Modified: Tue, 21 Nov 2023 06:05:38 GMT  
		Size: 39.0 MB (39022251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d211af034ddf5d1e81df73b8d237d1c15d165b5443c533eedbeecc5659d4d4b`  
		Last Modified: Tue, 21 Nov 2023 06:05:31 GMT  
		Size: 393.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd2e9fc8bb5d1ec8686111ad3e20155b1ac539fc01b742c2318311374c9c3d29`  
		Last Modified: Tue, 21 Nov 2023 06:05:31 GMT  
		Size: 1.9 KB (1877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2acddcee94070eff9faaeaa170066fa650714281ae6b3094fc1d49c010f3902`  
		Last Modified: Tue, 21 Nov 2023 06:05:31 GMT  
		Size: 1.5 KB (1480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21ffbd0e004b4f2f9f75bdc6731ed7d644c91ee50221377d2ff00e82aa1f99b9`  
		Last Modified: Tue, 21 Nov 2023 06:05:31 GMT  
		Size: 1.4 MB (1386383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44baab47b2128777f4b94d45e4a91e7bd440dcb23e61b28ec31c8ac469b3cf40`  
		Last Modified: Tue, 21 Nov 2023 06:05:31 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `adminer:4.8.1-fastcgi`

```console
$ docker pull adminer@sha256:daa291dff0f15be3ba5d0a8cfdcf137d8dd0b1f9304d132c686a4e95dcd489dd
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
$ docker pull adminer@sha256:8440f4060b767baf10aa0a817bae4ebe1d2991721279fdc2656503639463bd7b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.9 MB (95944774 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e93286ecedd0f7ab872f2a51eafc625c321f348ed0da94d7f8364be85227c44`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:46 GMT
ADD file:71543995e4d314b0c86da5ddf8e0cb74649767d30b3e5b6261360de354f0567b in / 
# Tue, 21 Nov 2023 05:21:46 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 09:49:06 GMT
STOPSIGNAL SIGINT
# Tue, 21 Nov 2023 09:49:25 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 09:49:26 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 21 Nov 2023 09:49:47 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Tue, 21 Nov 2023 09:49:47 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 21 Nov 2023 09:49:48 GMT
WORKDIR /var/www/html
# Tue, 21 Nov 2023 09:49:48 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 21 Nov 2023 09:49:48 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 21 Nov 2023 09:49:48 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 21 Nov 2023 09:49:48 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 21 Nov 2023 09:49:59 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Nov 2023 09:49:59 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 21 Nov 2023 09:49:59 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 21 Nov 2023 09:49:59 GMT
USER adminer
# Tue, 21 Nov 2023 09:49:59 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:d1da99c2f14827498c4a9bb3623ae909b44564bdabad1802f064169069df81fb`  
		Last Modified: Tue, 21 Nov 2023 05:26:17 GMT  
		Size: 55.1 MB (55057903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d7c776bdbb7e1224dedbc306fec7eb6e3842bd895a396927c36fa7f434312a3`  
		Last Modified: Tue, 21 Nov 2023 09:50:18 GMT  
		Size: 39.5 MB (39493553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:987d0f042e915521e94497a8e40892d4ec0532bd7641920df5ace1000310d793`  
		Last Modified: Tue, 21 Nov 2023 09:50:10 GMT  
		Size: 389.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38f43fc128ac2c6808d4b9a8087484f11d8cd4105abf9cd319353086c9b3b1d6`  
		Last Modified: Tue, 21 Nov 2023 09:50:34 GMT  
		Size: 2.7 KB (2714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96fdd5fed3b41dde57c97813fce8fc18ab9b07901345f868f32d346cfc74eb01`  
		Last Modified: Tue, 21 Nov 2023 09:50:34 GMT  
		Size: 1.9 KB (1878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3322f8293171857aeafd5fe96548028722034a3151f51dc695cc3cbef006e6a8`  
		Last Modified: Tue, 21 Nov 2023 09:50:34 GMT  
		Size: 1.5 KB (1480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2653b5cb64efa6e1c82031fa6e50d69957ca93e7f1660cc5e97344e601703f8e`  
		Last Modified: Tue, 21 Nov 2023 09:50:34 GMT  
		Size: 1.4 MB (1386365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5038798e96f08d106fc18e6a12538f783f08af440d0957a26c321901ebbad4b`  
		Last Modified: Tue, 21 Nov 2023 09:50:34 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1-fastcgi` - linux; arm variant v5

```console
$ docker pull adminer@sha256:b8f1ebac81289510963e10734e0ac78c24878a69d7aebbb9a3a29789c26dbfac
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.2 MB (91208572 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f60ec0b531cc5d09c3980c35d88d86cc1f9b8542ad54fcf7ff77d98ac3dea22`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Tue, 21 Nov 2023 05:01:00 GMT
ADD file:a5c8bd4b0873bd9ad0402143df41b5fd89c50bd24bb071b7d010919e189d88f9 in / 
# Tue, 21 Nov 2023 05:01:00 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 05:46:09 GMT
STOPSIGNAL SIGINT
# Tue, 21 Nov 2023 05:46:38 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 05:46:39 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 21 Nov 2023 05:46:58 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Tue, 21 Nov 2023 05:46:58 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 21 Nov 2023 05:46:58 GMT
WORKDIR /var/www/html
# Tue, 21 Nov 2023 05:46:58 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 21 Nov 2023 05:46:58 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 21 Nov 2023 05:46:58 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 21 Nov 2023 05:46:59 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 21 Nov 2023 05:47:15 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Nov 2023 05:47:15 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 21 Nov 2023 05:47:15 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 21 Nov 2023 05:47:15 GMT
USER adminer
# Tue, 21 Nov 2023 05:47:15 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:7378d71ea16926a061a2edbf0eb3dd13563fcb3ba9cf139c25e8334b36db1adf`  
		Last Modified: Tue, 21 Nov 2023 05:04:15 GMT  
		Size: 52.6 MB (52562921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cde673c33e7bfa6c04aeb9e184923984b648ae971715981d598aca5162e3c911`  
		Last Modified: Tue, 21 Nov 2023 05:47:34 GMT  
		Size: 37.3 MB (37252430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4fee5ad01a4adcbc52d632521a683e83dd44bb905a3048fc20faaa96d58f747`  
		Last Modified: Tue, 21 Nov 2023 05:47:25 GMT  
		Size: 386.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5f71f261b85a2e069d758daa1be7f3e53672fa4b8902826510a9159db451264`  
		Last Modified: Tue, 21 Nov 2023 05:47:51 GMT  
		Size: 2.7 KB (2705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d67d58698593646eb7ab4b717360bf37ab36a671802cb216b3262ce695ef1e5`  
		Last Modified: Tue, 21 Nov 2023 05:47:51 GMT  
		Size: 1.9 KB (1870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d309e407d77f27b1a5409e0ce83c664cb9f080a3168176e8114376d8721a153e`  
		Last Modified: Tue, 21 Nov 2023 05:47:51 GMT  
		Size: 1.5 KB (1477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ee0aa3b9dd1374206375afa28a3b15aa7e6b58abf1b669705b9a86f43e0be79`  
		Last Modified: Tue, 21 Nov 2023 05:47:51 GMT  
		Size: 1.4 MB (1386292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74eeb313bede5967e1e4dd1a8bef17eda92f71136ff55d6ed522d984a8712436`  
		Last Modified: Tue, 21 Nov 2023 05:47:51 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1-fastcgi` - linux; arm variant v7

```console
$ docker pull adminer@sha256:1674e094629be082c484d9c7c974fa715e706fbf661bafc68bad546bed9ffe00
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.8 MB (87799571 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c995386759ce4cef4ffbcffb5be8163c9813d2a8220561e9a841f14fb07e0bd`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Tue, 21 Nov 2023 03:57:54 GMT
ADD file:ed8d88d0476fad37879d872d61d05a8cffff35609566f080f78bb882d1bae26b in / 
# Tue, 21 Nov 2023 03:57:54 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 06:58:56 GMT
STOPSIGNAL SIGINT
# Tue, 21 Nov 2023 06:59:20 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 06:59:21 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 21 Nov 2023 06:59:45 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Tue, 21 Nov 2023 06:59:46 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 21 Nov 2023 06:59:46 GMT
WORKDIR /var/www/html
# Tue, 21 Nov 2023 06:59:46 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 21 Nov 2023 06:59:46 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 21 Nov 2023 06:59:47 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 21 Nov 2023 06:59:47 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 21 Nov 2023 07:00:00 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Nov 2023 07:00:01 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 21 Nov 2023 07:00:01 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 21 Nov 2023 07:00:01 GMT
USER adminer
# Tue, 21 Nov 2023 07:00:01 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:1dac19092a737e476f9b096fe28463512ae21c4f596dd2f8b84d62530416dffe`  
		Last Modified: Tue, 21 Nov 2023 04:02:11 GMT  
		Size: 50.2 MB (50215653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2f8153e5d67bc5a0049a12eb2430f50747238b7d4023cacdfc5dad9cdbd244a`  
		Last Modified: Tue, 21 Nov 2023 07:00:24 GMT  
		Size: 36.2 MB (36190640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ea62b864a160dff0b693d9397a8b84a1bc65e8e381b223294a8ac5ac8c68b8a`  
		Last Modified: Tue, 21 Nov 2023 07:00:15 GMT  
		Size: 393.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e77dfeac49a3de3540eb4b5ade85851c08d2523b73c838b14a68fe81a3ec17a1`  
		Last Modified: Tue, 21 Nov 2023 07:00:40 GMT  
		Size: 2.7 KB (2715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e25f712f1f600f798ffd1261db13ef564f0af09c7c65533ed8ed59ec3b26552`  
		Last Modified: Tue, 21 Nov 2023 07:00:40 GMT  
		Size: 1.9 KB (1871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81cdb234e089dedc46386bbac8970166dab2d606288d8c1d426d4b4e617dc9dc`  
		Last Modified: Tue, 21 Nov 2023 07:00:41 GMT  
		Size: 1.5 KB (1476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fea6f1b6b2d8c666838e4a7ca42f2fbcfe498fc2a0eea88d569639836fa56140`  
		Last Modified: Tue, 21 Nov 2023 07:00:41 GMT  
		Size: 1.4 MB (1386332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fd0838894de2a37bd6487e6cf8b3c35ea2ee2e2793979871db8f810c871abd4`  
		Last Modified: Tue, 21 Nov 2023 07:00:41 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1-fastcgi` - linux; arm64 variant v8

```console
$ docker pull adminer@sha256:84a893178255bde14cc03ffe152122623fe05eb3839e5f5bae856fb7da83814b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.3 MB (94348838 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b1d17ed2083c8a28275848906f461bdfdb42e15994ac21d9a62087dc6d034d2`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:13 GMT
ADD file:614987b9855939825ad2383e7bacbf14ea208d74906982bba3a67126702c8371 in / 
# Tue, 21 Nov 2023 06:27:13 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 10:22:26 GMT
STOPSIGNAL SIGINT
# Tue, 21 Nov 2023 10:22:43 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 10:22:44 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 21 Nov 2023 10:23:00 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Tue, 21 Nov 2023 10:23:00 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 21 Nov 2023 10:23:00 GMT
WORKDIR /var/www/html
# Tue, 21 Nov 2023 10:23:00 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 21 Nov 2023 10:23:00 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 21 Nov 2023 10:23:00 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 21 Nov 2023 10:23:01 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 21 Nov 2023 10:23:10 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Nov 2023 10:23:11 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 21 Nov 2023 10:23:11 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 21 Nov 2023 10:23:11 GMT
USER adminer
# Tue, 21 Nov 2023 10:23:11 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:bbf382c14c7b19b81c612f639e09e6a7b04eccd4481d0abac48b8ace9faae3b3`  
		Last Modified: Tue, 21 Nov 2023 06:30:47 GMT  
		Size: 53.7 MB (53707872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aa045892ab5d3693eb19355bad15725aa10139ceb2bfc2cb6141778f671e8e4`  
		Last Modified: Tue, 21 Nov 2023 10:23:29 GMT  
		Size: 39.2 MB (39247701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d77bfaecae2cacef431f4d68d17c26be0ab2300b5dfee893959aaae0c6427677`  
		Last Modified: Tue, 21 Nov 2023 10:23:21 GMT  
		Size: 386.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0caf62f5f6228f681c738a20ff40e768d645f553295e9a804e07c9983f280b5`  
		Last Modified: Tue, 21 Nov 2023 10:23:46 GMT  
		Size: 2.7 KB (2705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2df7041a632dc747d7c856a4b14a181da3e49fb1fb8e613f35a8b25404cb7269`  
		Last Modified: Tue, 21 Nov 2023 10:23:46 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c1e97ecf3d9ca77aee6de698d163482237c5a78acbe0e5ff1e47768d6e3fcb6`  
		Last Modified: Tue, 21 Nov 2023 10:23:46 GMT  
		Size: 1.5 KB (1477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce1ef470c48dc65a0917a06d12f3b23a206308eedf67bb228f570870947eb345`  
		Last Modified: Tue, 21 Nov 2023 10:23:47 GMT  
		Size: 1.4 MB (1386324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9363d2b46e93f744f02df5f1ad6d68e5d6ec8debff805842925426c2c0853d95`  
		Last Modified: Tue, 21 Nov 2023 10:23:46 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1-fastcgi` - linux; 386

```console
$ docker pull adminer@sha256:063600a67051477eb2d252722e908e12954e92aa2f1103c08bc6ec0c98c81900
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.0 MB (97001696 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9faffd6534bfd19c55ba87d0ea06c0dec17f32f96aaf19d3d273080350957b57`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Tue, 21 Nov 2023 04:40:03 GMT
ADD file:54170328827ccc52692c964f0c45a65ed6efdf39897f2c226672fdf526f3c412 in / 
# Tue, 21 Nov 2023 04:40:04 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 15:41:51 GMT
STOPSIGNAL SIGINT
# Tue, 21 Nov 2023 15:42:20 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 15:42:21 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 21 Nov 2023 15:42:40 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Tue, 21 Nov 2023 15:42:40 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 21 Nov 2023 15:42:41 GMT
WORKDIR /var/www/html
# Tue, 21 Nov 2023 15:42:41 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 21 Nov 2023 15:42:41 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 21 Nov 2023 15:42:41 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 21 Nov 2023 15:42:41 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 21 Nov 2023 15:42:56 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Nov 2023 15:42:56 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 21 Nov 2023 15:42:56 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 21 Nov 2023 15:42:56 GMT
USER adminer
# Tue, 21 Nov 2023 15:42:56 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:e33c1468a29e45636d4d9529b663048f7e8aa83ff428eb0681253bd4200e23ec`  
		Last Modified: Tue, 21 Nov 2023 04:44:57 GMT  
		Size: 56.0 MB (56046301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8137e600c481ac4ed29cae88512a113a2eadcc1d26e72628216670ef4f61ba30`  
		Last Modified: Tue, 21 Nov 2023 15:43:16 GMT  
		Size: 39.6 MB (39562172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e42a8870a081f3a4ab284980034bebec6585740c88e4c40ae98b2e1fa9955f5`  
		Last Modified: Tue, 21 Nov 2023 15:43:05 GMT  
		Size: 392.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ea29f8bfe081038362130d161f4fce7184b04e8b23e4e6eb76012853b52eb29`  
		Last Modified: Tue, 21 Nov 2023 15:43:34 GMT  
		Size: 2.7 KB (2711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c61c47ded185575a69531bea47b571461b9b5a7dbe771c12d9a5351c2274616`  
		Last Modified: Tue, 21 Nov 2023 15:43:34 GMT  
		Size: 1.9 KB (1867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce13699c4877d6078a5c0d0891b3ab176e81a19c03c25322e69a1da82443611a`  
		Last Modified: Tue, 21 Nov 2023 15:43:34 GMT  
		Size: 1.5 KB (1480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:467cdaa3b936c126690238f64a0f87f1ea5c53e47ad6b7a300a08e68304b4c5e`  
		Last Modified: Tue, 21 Nov 2023 15:43:34 GMT  
		Size: 1.4 MB (1386283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08c8258bd975965d721bb178e601818437b2ec83ecf04991a03e7ac42e8262f1`  
		Last Modified: Tue, 21 Nov 2023 15:43:34 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1-fastcgi` - linux; mips64le

```console
$ docker pull adminer@sha256:a764c136226771f05874d428d466ab7617443109af05761f5a301d774d3d78ef
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.6 MB (92637624 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6dcb8d7570466b2e24f152459f05444501a2db6bec81dd770f36a922da335bf3`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Tue, 21 Nov 2023 04:10:25 GMT
ADD file:dbfc3d226166089c4db0c154fdcea8049b8758c6812f1c397dec1444985e8557 in / 
# Tue, 21 Nov 2023 04:10:31 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 12:14:44 GMT
STOPSIGNAL SIGINT
# Tue, 21 Nov 2023 12:16:43 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 12:16:50 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 21 Nov 2023 12:18:45 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Tue, 21 Nov 2023 12:18:52 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 21 Nov 2023 12:18:55 GMT
WORKDIR /var/www/html
# Tue, 21 Nov 2023 12:18:59 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 21 Nov 2023 12:19:02 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 21 Nov 2023 12:19:05 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 21 Nov 2023 12:19:09 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 21 Nov 2023 12:20:00 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Nov 2023 12:20:03 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 21 Nov 2023 12:20:06 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 21 Nov 2023 12:20:10 GMT
USER adminer
# Tue, 21 Nov 2023 12:20:13 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:ca31218601e95f4aafae0dcadda7600aeb04db374e1e829d5c123f8033ba3472`  
		Last Modified: Tue, 21 Nov 2023 04:21:21 GMT  
		Size: 53.3 MB (53289162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d172a1ce4463b8a1bb14b88d9f7c98a7f06f260dfc2849e77f3d41be6d17db9`  
		Last Modified: Tue, 21 Nov 2023 12:21:00 GMT  
		Size: 38.0 MB (37954467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbd3b039fbc0efa77466cfb045c80c120d45355cf2db0dd6533eeb1cee6296e1`  
		Last Modified: Tue, 21 Nov 2023 12:20:33 GMT  
		Size: 394.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:873ce81c2a5a659c6ba90c59b5fdd1a3c215439a655c8efe1b62a042ba6dc956`  
		Last Modified: Tue, 21 Nov 2023 12:21:19 GMT  
		Size: 2.7 KB (2714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:046c3c9cda84191a448b5676717eb2efd43aa616bd1a7936fd1ffa7333fe414d`  
		Last Modified: Tue, 21 Nov 2023 12:21:19 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d5fb1a0ccda92972577970b93a35e31e87aca9efdf320fe33d64fbb50e5f5be`  
		Last Modified: Tue, 21 Nov 2023 12:21:19 GMT  
		Size: 1.5 KB (1479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16f226ce3836498318ee4d4f1573efc49e08a2a6cdfd7403a3089f66f24194f3`  
		Last Modified: Tue, 21 Nov 2023 12:21:20 GMT  
		Size: 1.4 MB (1387178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc2ef37541c711003007d218f46c929098bfda475d45d9ced2d3700246c0d143`  
		Last Modified: Tue, 21 Nov 2023 12:21:19 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1-fastcgi` - linux; ppc64le

```console
$ docker pull adminer@sha256:988a50cb007ef650a43dfb195f4730d2268d36b717db2cdbc731914c725ee8df
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.3 MB (101268149 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f2e2a636068dd83fb84a9bcecd6a718528598da747489d7573b02bdfa6f20140`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Tue, 21 Nov 2023 04:24:26 GMT
ADD file:c21c2b6cb3f9bdf6cc3641e9ebf810a461174480c6cd1c25515cf9fce4aa2143 in / 
# Tue, 21 Nov 2023 04:24:30 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 06:49:59 GMT
STOPSIGNAL SIGINT
# Tue, 21 Nov 2023 06:50:40 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 06:50:42 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 21 Nov 2023 06:51:10 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Tue, 21 Nov 2023 06:51:11 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 21 Nov 2023 06:51:11 GMT
WORKDIR /var/www/html
# Tue, 21 Nov 2023 06:51:12 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 21 Nov 2023 06:51:12 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 21 Nov 2023 06:51:12 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 21 Nov 2023 06:51:13 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 21 Nov 2023 06:51:30 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Nov 2023 06:51:30 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 21 Nov 2023 06:51:30 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 21 Nov 2023 06:51:31 GMT
USER adminer
# Tue, 21 Nov 2023 06:51:31 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:23ebe74b854f8f6e2671f4c8cc147a6925fb7d929ce5898f7ca2af9781bf7d38`  
		Last Modified: Tue, 21 Nov 2023 04:29:21 GMT  
		Size: 58.9 MB (58929678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa255108512a37e57b2fdf827a0fdb4e3783a0649fb80ecdd431d4921dd6761c`  
		Last Modified: Tue, 21 Nov 2023 06:51:51 GMT  
		Size: 40.9 MB (40945122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5862ce535fc870ad9665c04e9816effde44c5f4469bc852265ba0bfe11ad7001`  
		Last Modified: Tue, 21 Nov 2023 06:51:41 GMT  
		Size: 391.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eb07c0427e1d513dc1c2e122ef9b33a7ce04c7f6e7ac25eb3cdc16b7c4f3dd0`  
		Last Modified: Tue, 21 Nov 2023 06:52:10 GMT  
		Size: 2.7 KB (2709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e1a3baf382e8ecd698319193729a0416bcdcbe069383e956a41029751483ab8`  
		Last Modified: Tue, 21 Nov 2023 06:52:10 GMT  
		Size: 1.9 KB (1878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd36769ccabc572d519d259cd2369096462f35a823d2817c593ce165f30f690b`  
		Last Modified: Tue, 21 Nov 2023 06:52:10 GMT  
		Size: 1.5 KB (1480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e35256cd8ee36eeca9a95cc2fc4ad45b213f5025c0d7211c00f76beae6c7a0bd`  
		Last Modified: Tue, 21 Nov 2023 06:52:11 GMT  
		Size: 1.4 MB (1386400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:417adc53867ad9b9d99a43bc9736c1285bc9af029e2938bd516928b92cad7093`  
		Last Modified: Tue, 21 Nov 2023 06:52:10 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1-fastcgi` - linux; s390x

```console
$ docker pull adminer@sha256:8920ecc20283083c9296766b19c975eabf1764eecadbcd7b97ed7bb11e30921e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.7 MB (93711989 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33df00454cb56b58abb106b0161ca460cdce0f5d1f8162177becb869dde24b99`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Tue, 21 Nov 2023 05:04:52 GMT
ADD file:b0a8fd50925b3555a0c10177e65551cae288917f9bad8fb4728ec83cc0765afe in / 
# Tue, 21 Nov 2023 05:05:01 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 06:04:07 GMT
STOPSIGNAL SIGINT
# Tue, 21 Nov 2023 06:04:29 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 06:04:35 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 21 Nov 2023 06:05:00 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Tue, 21 Nov 2023 06:05:00 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 21 Nov 2023 06:05:00 GMT
WORKDIR /var/www/html
# Tue, 21 Nov 2023 06:05:01 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 21 Nov 2023 06:05:01 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 21 Nov 2023 06:05:01 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 21 Nov 2023 06:05:01 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 21 Nov 2023 06:05:11 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Nov 2023 06:05:11 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 21 Nov 2023 06:05:11 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 21 Nov 2023 06:05:12 GMT
USER adminer
# Tue, 21 Nov 2023 06:05:12 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:9488c1539560318cb45b39150f91e365b928c0a246788663f5c72d185864bd3e`  
		Last Modified: Tue, 21 Nov 2023 05:10:34 GMT  
		Size: 53.3 MB (53296396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09efec12dc42685e3fe1693d18bc42d61971044de30a99ee3f044d942e93a470`  
		Last Modified: Tue, 21 Nov 2023 06:05:38 GMT  
		Size: 39.0 MB (39022251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d211af034ddf5d1e81df73b8d237d1c15d165b5443c533eedbeecc5659d4d4b`  
		Last Modified: Tue, 21 Nov 2023 06:05:31 GMT  
		Size: 393.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32f1b2d24e5fca07170540193831c2b4e39ddb10d4fc7736e631b2aa11ed601a`  
		Last Modified: Tue, 21 Nov 2023 06:05:48 GMT  
		Size: 2.7 KB (2711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6439585d05cece3d9af2be5ecb1d12bf8e78e1a23a419fb2f49451ede72e90ba`  
		Last Modified: Tue, 21 Nov 2023 06:05:48 GMT  
		Size: 1.9 KB (1879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aea2cdf22e5a5de0f7b5cc6c97c9c03a8fe82113a1d7d5153a55592fdf09568`  
		Last Modified: Tue, 21 Nov 2023 06:05:48 GMT  
		Size: 1.5 KB (1479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:922a0d106738cf725844ac8a3a5ef1352d0048149982aee61fe3d0f67bb8a041`  
		Last Modified: Tue, 21 Nov 2023 06:05:48 GMT  
		Size: 1.4 MB (1386389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:791aaf97ba65859a96b769218ea3ab780b809cc6bcacb784b88c24756e99ef6b`  
		Last Modified: Tue, 21 Nov 2023 06:05:48 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `adminer:4.8.1-standalone`

```console
$ docker pull adminer@sha256:0ce7583815dabdd9f560ee0afed630ecb33df6756f4b66c85c197011559a0248
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
$ docker pull adminer@sha256:78d95e4c7a6cfb584a500e0e8ca7db956ab9ff1cd4b3239306b330c2637ecfa2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.9 MB (95942047 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7554c8e10d81e451e656e73d613de4f9c885b91255f46a2fdc03ccf275a1d449`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:46 GMT
ADD file:71543995e4d314b0c86da5ddf8e0cb74649767d30b3e5b6261360de354f0567b in / 
# Tue, 21 Nov 2023 05:21:46 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 09:49:06 GMT
STOPSIGNAL SIGINT
# Tue, 21 Nov 2023 09:49:25 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 09:49:26 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 21 Nov 2023 09:49:27 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 21 Nov 2023 09:49:27 GMT
WORKDIR /var/www/html
# Tue, 21 Nov 2023 09:49:27 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 21 Nov 2023 09:49:27 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 21 Nov 2023 09:49:27 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 21 Nov 2023 09:49:27 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 21 Nov 2023 09:49:39 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Nov 2023 09:49:39 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 21 Nov 2023 09:49:39 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 21 Nov 2023 09:49:39 GMT
USER adminer
# Tue, 21 Nov 2023 09:49:39 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Tue, 21 Nov 2023 09:49:39 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:d1da99c2f14827498c4a9bb3623ae909b44564bdabad1802f064169069df81fb`  
		Last Modified: Tue, 21 Nov 2023 05:26:17 GMT  
		Size: 55.1 MB (55057903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d7c776bdbb7e1224dedbc306fec7eb6e3842bd895a396927c36fa7f434312a3`  
		Last Modified: Tue, 21 Nov 2023 09:50:18 GMT  
		Size: 39.5 MB (39493553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:987d0f042e915521e94497a8e40892d4ec0532bd7641920df5ace1000310d793`  
		Last Modified: Tue, 21 Nov 2023 09:50:10 GMT  
		Size: 389.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb163dc8650b5fde5c72f76b8937b3c38d3dd4c7a2922d7b6f95a0890070c4d9`  
		Last Modified: Tue, 21 Nov 2023 09:50:10 GMT  
		Size: 1.9 KB (1878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98b256c86f3d5b1eab91122ae075d7b3b15d1185ebe1cc10a8b4d2fb6f2bdf5f`  
		Last Modified: Tue, 21 Nov 2023 09:50:10 GMT  
		Size: 1.5 KB (1480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7952b9a84b1867112d08313ef023ee4917d7bbd0f91f4d8ae3ce1b17376d345e`  
		Last Modified: Tue, 21 Nov 2023 09:50:11 GMT  
		Size: 1.4 MB (1386353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77cf83a8d79b963388e7d18d6836ac44d7832d08fa39ab46ba57f0c92e48e1f2`  
		Last Modified: Tue, 21 Nov 2023 09:50:10 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1-standalone` - linux; arm variant v5

```console
$ docker pull adminer@sha256:f6bb8e720054e43d3bc65a163e9fc4146ce4c215db05216f56be5cbac7428eb7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.2 MB (91205860 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9bd45b72f483757bdbd0f31b96e08578a127cc80966526aa0a9a897f5012203`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Tue, 21 Nov 2023 05:01:00 GMT
ADD file:a5c8bd4b0873bd9ad0402143df41b5fd89c50bd24bb071b7d010919e189d88f9 in / 
# Tue, 21 Nov 2023 05:01:00 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 05:46:09 GMT
STOPSIGNAL SIGINT
# Tue, 21 Nov 2023 05:46:38 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 05:46:39 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 21 Nov 2023 05:46:40 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 21 Nov 2023 05:46:40 GMT
WORKDIR /var/www/html
# Tue, 21 Nov 2023 05:46:40 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 21 Nov 2023 05:46:40 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 21 Nov 2023 05:46:40 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 21 Nov 2023 05:46:40 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 21 Nov 2023 05:46:55 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Nov 2023 05:46:55 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 21 Nov 2023 05:46:55 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 21 Nov 2023 05:46:55 GMT
USER adminer
# Tue, 21 Nov 2023 05:46:55 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Tue, 21 Nov 2023 05:46:55 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:7378d71ea16926a061a2edbf0eb3dd13563fcb3ba9cf139c25e8334b36db1adf`  
		Last Modified: Tue, 21 Nov 2023 05:04:15 GMT  
		Size: 52.6 MB (52562921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cde673c33e7bfa6c04aeb9e184923984b648ae971715981d598aca5162e3c911`  
		Last Modified: Tue, 21 Nov 2023 05:47:34 GMT  
		Size: 37.3 MB (37252430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4fee5ad01a4adcbc52d632521a683e83dd44bb905a3048fc20faaa96d58f747`  
		Last Modified: Tue, 21 Nov 2023 05:47:25 GMT  
		Size: 386.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:062df034c3a9a14a736fb1733f5f91b8c5cad9974f6b67df85f488a45026f47c`  
		Last Modified: Tue, 21 Nov 2023 05:47:24 GMT  
		Size: 1.9 KB (1869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:610f64ab71d9f5c7abad4551870c223a9b95603025384ef1e7a85f624f0b0467`  
		Last Modified: Tue, 21 Nov 2023 05:47:24 GMT  
		Size: 1.5 KB (1481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59cca3ff7ed68079f673662534d292a264aa5c1d7d4358251d8e25f21faa9f94`  
		Last Modified: Tue, 21 Nov 2023 05:47:25 GMT  
		Size: 1.4 MB (1386281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:753ad2913e083c1b5cb5b06853944934450629b0451d408743ddffc1f4c0a843`  
		Last Modified: Tue, 21 Nov 2023 05:47:24 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1-standalone` - linux; arm variant v7

```console
$ docker pull adminer@sha256:6faef276799d02bdd9abf0ba022b692fd46f8144584adcfa771a76d225131045
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.8 MB (87796870 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9bb280f29bbaaa440662c6cbd26fabd7313fb299195b0ff2ca0cc22cff61f1ab`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Tue, 21 Nov 2023 03:57:54 GMT
ADD file:ed8d88d0476fad37879d872d61d05a8cffff35609566f080f78bb882d1bae26b in / 
# Tue, 21 Nov 2023 03:57:54 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 06:58:56 GMT
STOPSIGNAL SIGINT
# Tue, 21 Nov 2023 06:59:20 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 06:59:21 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 21 Nov 2023 06:59:21 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 21 Nov 2023 06:59:21 GMT
WORKDIR /var/www/html
# Tue, 21 Nov 2023 06:59:21 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 21 Nov 2023 06:59:21 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 21 Nov 2023 06:59:21 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 21 Nov 2023 06:59:22 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 21 Nov 2023 06:59:37 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Nov 2023 06:59:37 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 21 Nov 2023 06:59:37 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 21 Nov 2023 06:59:37 GMT
USER adminer
# Tue, 21 Nov 2023 06:59:37 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Tue, 21 Nov 2023 06:59:37 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:1dac19092a737e476f9b096fe28463512ae21c4f596dd2f8b84d62530416dffe`  
		Last Modified: Tue, 21 Nov 2023 04:02:11 GMT  
		Size: 50.2 MB (50215653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2f8153e5d67bc5a0049a12eb2430f50747238b7d4023cacdfc5dad9cdbd244a`  
		Last Modified: Tue, 21 Nov 2023 07:00:24 GMT  
		Size: 36.2 MB (36190640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ea62b864a160dff0b693d9397a8b84a1bc65e8e381b223294a8ac5ac8c68b8a`  
		Last Modified: Tue, 21 Nov 2023 07:00:15 GMT  
		Size: 393.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e2dd6fa8973e47e4cce58445b7207793f22b2371aa58678dc17d4172eac0b32`  
		Last Modified: Tue, 21 Nov 2023 07:00:15 GMT  
		Size: 1.9 KB (1871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4d33015217bf866b0d2c44cd29bf71617469b2e87e38eb15795aa3a293c83fa`  
		Last Modified: Tue, 21 Nov 2023 07:00:16 GMT  
		Size: 1.5 KB (1478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24ee8e39b9683ef6aa34033169655e5585db29d9557c0e1eb9aa117e1c771047`  
		Last Modified: Tue, 21 Nov 2023 07:00:16 GMT  
		Size: 1.4 MB (1386341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c14859802a2676aa6a511bbd06ce80a759e38e94927cd4d4b60dd202568ef5b`  
		Last Modified: Tue, 21 Nov 2023 07:00:15 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1-standalone` - linux; arm64 variant v8

```console
$ docker pull adminer@sha256:e5fda74f5900f3c7ef8f74bda0392b45089f33f56374326bb331d8db26eb8b41
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.3 MB (94346130 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ccf82dd602ee08aa22718c108fcbcedbebb819a09c86b9f0fe8f2c1737bd08a7`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:13 GMT
ADD file:614987b9855939825ad2383e7bacbf14ea208d74906982bba3a67126702c8371 in / 
# Tue, 21 Nov 2023 06:27:13 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 10:22:26 GMT
STOPSIGNAL SIGINT
# Tue, 21 Nov 2023 10:22:43 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 10:22:44 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 21 Nov 2023 10:22:44 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 21 Nov 2023 10:22:44 GMT
WORKDIR /var/www/html
# Tue, 21 Nov 2023 10:22:44 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 21 Nov 2023 10:22:44 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 21 Nov 2023 10:22:45 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 21 Nov 2023 10:22:45 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 21 Nov 2023 10:22:54 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Nov 2023 10:22:54 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 21 Nov 2023 10:22:54 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 21 Nov 2023 10:22:54 GMT
USER adminer
# Tue, 21 Nov 2023 10:22:55 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Tue, 21 Nov 2023 10:22:55 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:bbf382c14c7b19b81c612f639e09e6a7b04eccd4481d0abac48b8ace9faae3b3`  
		Last Modified: Tue, 21 Nov 2023 06:30:47 GMT  
		Size: 53.7 MB (53707872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aa045892ab5d3693eb19355bad15725aa10139ceb2bfc2cb6141778f671e8e4`  
		Last Modified: Tue, 21 Nov 2023 10:23:29 GMT  
		Size: 39.2 MB (39247701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d77bfaecae2cacef431f4d68d17c26be0ab2300b5dfee893959aaae0c6427677`  
		Last Modified: Tue, 21 Nov 2023 10:23:21 GMT  
		Size: 386.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1364c7eb4b90daedaca80aff830c09309115f174a295c35ba7885c60557fa1e`  
		Last Modified: Tue, 21 Nov 2023 10:23:21 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:080b929d6ed912f11ed340726920967a938d3632641f4f86e15a30fc7b255888`  
		Last Modified: Tue, 21 Nov 2023 10:23:21 GMT  
		Size: 1.5 KB (1477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:633cfed53ab70b9e08d21a78973fc2a318d49c9cc54f3100604c9b91dd533c82`  
		Last Modified: Tue, 21 Nov 2023 10:23:22 GMT  
		Size: 1.4 MB (1386322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc610b080dd3b327bfe4b6ca8da59bc3a5555a295aff6c4f18d172f070b4e1ab`  
		Last Modified: Tue, 21 Nov 2023 10:23:21 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1-standalone` - linux; 386

```console
$ docker pull adminer@sha256:173f2532a535a7780bffa43d6385797ba5335ab89832cb016cbb54cb0ab60fb2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.0 MB (96998974 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85b8488ee11e55b40364ca362184cc13095a7b83f1c1e65e524862cc27000db2`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Tue, 21 Nov 2023 04:40:03 GMT
ADD file:54170328827ccc52692c964f0c45a65ed6efdf39897f2c226672fdf526f3c412 in / 
# Tue, 21 Nov 2023 04:40:04 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 15:41:51 GMT
STOPSIGNAL SIGINT
# Tue, 21 Nov 2023 15:42:20 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 15:42:21 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 21 Nov 2023 15:42:22 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 21 Nov 2023 15:42:22 GMT
WORKDIR /var/www/html
# Tue, 21 Nov 2023 15:42:22 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 21 Nov 2023 15:42:22 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 21 Nov 2023 15:42:22 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 21 Nov 2023 15:42:22 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 21 Nov 2023 15:42:37 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Nov 2023 15:42:37 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 21 Nov 2023 15:42:37 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 21 Nov 2023 15:42:37 GMT
USER adminer
# Tue, 21 Nov 2023 15:42:37 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Tue, 21 Nov 2023 15:42:37 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:e33c1468a29e45636d4d9529b663048f7e8aa83ff428eb0681253bd4200e23ec`  
		Last Modified: Tue, 21 Nov 2023 04:44:57 GMT  
		Size: 56.0 MB (56046301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8137e600c481ac4ed29cae88512a113a2eadcc1d26e72628216670ef4f61ba30`  
		Last Modified: Tue, 21 Nov 2023 15:43:16 GMT  
		Size: 39.6 MB (39562172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e42a8870a081f3a4ab284980034bebec6585740c88e4c40ae98b2e1fa9955f5`  
		Last Modified: Tue, 21 Nov 2023 15:43:05 GMT  
		Size: 392.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48c728479be5016dacc84b6c0c244f327eff896df6a326af2826d6ad4c5387b6`  
		Last Modified: Tue, 21 Nov 2023 15:43:05 GMT  
		Size: 1.9 KB (1870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1000dcb7b3ee07a4d8a46142cda4b99b13051577e48599f89d62c8fd8c7e61a8`  
		Last Modified: Tue, 21 Nov 2023 15:43:05 GMT  
		Size: 1.5 KB (1482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d8473e68cd9a1e0940ff9bb80857e7d32bfde252766cc39fc1c3566222b0c1c`  
		Last Modified: Tue, 21 Nov 2023 15:43:06 GMT  
		Size: 1.4 MB (1386265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d7609e79a7e8443050102286e60b2022e9f3447043db395cabb7e2ad151b1e0`  
		Last Modified: Tue, 21 Nov 2023 15:43:05 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1-standalone` - linux; mips64le

```console
$ docker pull adminer@sha256:84b1c19875f37b42946db21b87c80b8f8d9d9c7392eff0a7a065cf6d5fe769b2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.6 MB (92634921 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6454361a51d8f0d5781cd1854359c6b0812cc29466f516dd6386754b3583699`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Tue, 21 Nov 2023 04:10:25 GMT
ADD file:dbfc3d226166089c4db0c154fdcea8049b8758c6812f1c397dec1444985e8557 in / 
# Tue, 21 Nov 2023 04:10:31 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 12:14:44 GMT
STOPSIGNAL SIGINT
# Tue, 21 Nov 2023 12:16:43 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 12:16:50 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 21 Nov 2023 12:16:57 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 21 Nov 2023 12:17:00 GMT
WORKDIR /var/www/html
# Tue, 21 Nov 2023 12:17:04 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 21 Nov 2023 12:17:07 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 21 Nov 2023 12:17:10 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 21 Nov 2023 12:17:14 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 21 Nov 2023 12:18:08 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Nov 2023 12:18:11 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 21 Nov 2023 12:18:14 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 21 Nov 2023 12:18:17 GMT
USER adminer
# Tue, 21 Nov 2023 12:18:21 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Tue, 21 Nov 2023 12:18:24 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:ca31218601e95f4aafae0dcadda7600aeb04db374e1e829d5c123f8033ba3472`  
		Last Modified: Tue, 21 Nov 2023 04:21:21 GMT  
		Size: 53.3 MB (53289162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d172a1ce4463b8a1bb14b88d9f7c98a7f06f260dfc2849e77f3d41be6d17db9`  
		Last Modified: Tue, 21 Nov 2023 12:21:00 GMT  
		Size: 38.0 MB (37954467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbd3b039fbc0efa77466cfb045c80c120d45355cf2db0dd6533eeb1cee6296e1`  
		Last Modified: Tue, 21 Nov 2023 12:20:33 GMT  
		Size: 394.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bac97c667ed055993103f32b019a430a853a94eef6bf75086fda9949a9fd1d8`  
		Last Modified: Tue, 21 Nov 2023 12:20:34 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66eec20186701717a98146a63c5c8f88304d44243fe6f6505edf4d1135672446`  
		Last Modified: Tue, 21 Nov 2023 12:20:34 GMT  
		Size: 1.5 KB (1483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a56ddb348b2b13a6cac73829460bdcce2971790b6be59ac9da70b739453488b8`  
		Last Modified: Tue, 21 Nov 2023 12:20:34 GMT  
		Size: 1.4 MB (1387192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f922348b25af66b56cdd7a4863a9a120057afa01489fc9058cf7e975b198d05`  
		Last Modified: Tue, 21 Nov 2023 12:20:34 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1-standalone` - linux; ppc64le

```console
$ docker pull adminer@sha256:3b96a3711e0e719557e514cb8870567e67ab545a7fe18b4feeca4e0e4c85d678
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.3 MB (101265448 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0c151160d019f74dfe13959cf16722a5172a0023a5f747201c90b752e001545`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Tue, 21 Nov 2023 04:24:26 GMT
ADD file:c21c2b6cb3f9bdf6cc3641e9ebf810a461174480c6cd1c25515cf9fce4aa2143 in / 
# Tue, 21 Nov 2023 04:24:30 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 06:49:59 GMT
STOPSIGNAL SIGINT
# Tue, 21 Nov 2023 06:50:40 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 06:50:42 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 21 Nov 2023 06:50:44 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 21 Nov 2023 06:50:44 GMT
WORKDIR /var/www/html
# Tue, 21 Nov 2023 06:50:44 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 21 Nov 2023 06:50:44 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 21 Nov 2023 06:50:45 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 21 Nov 2023 06:50:45 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 21 Nov 2023 06:51:03 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Nov 2023 06:51:03 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 21 Nov 2023 06:51:03 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 21 Nov 2023 06:51:03 GMT
USER adminer
# Tue, 21 Nov 2023 06:51:04 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Tue, 21 Nov 2023 06:51:04 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:23ebe74b854f8f6e2671f4c8cc147a6925fb7d929ce5898f7ca2af9781bf7d38`  
		Last Modified: Tue, 21 Nov 2023 04:29:21 GMT  
		Size: 58.9 MB (58929678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa255108512a37e57b2fdf827a0fdb4e3783a0649fb80ecdd431d4921dd6761c`  
		Last Modified: Tue, 21 Nov 2023 06:51:51 GMT  
		Size: 40.9 MB (40945122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5862ce535fc870ad9665c04e9816effde44c5f4469bc852265ba0bfe11ad7001`  
		Last Modified: Tue, 21 Nov 2023 06:51:41 GMT  
		Size: 391.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7204feb32d0a6fe6dd0348f7a8c2845b90b631ba893c08c48a724057c8a5e3d1`  
		Last Modified: Tue, 21 Nov 2023 06:51:41 GMT  
		Size: 1.9 KB (1879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb06eb196e5a191ad6e9d6d43052c2fd0f833100bf197c73f3f9c8df967003d1`  
		Last Modified: Tue, 21 Nov 2023 06:51:41 GMT  
		Size: 1.5 KB (1482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76df205e8013dede04db80018bebbabea233e0186671f2fd251fa440acde39ef`  
		Last Modified: Tue, 21 Nov 2023 06:51:41 GMT  
		Size: 1.4 MB (1386403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7099dfc32b7ad37a3cfe50e8aad19c609d5e9daf0535dd5cd0f853de87d0de8f`  
		Last Modified: Tue, 21 Nov 2023 06:51:41 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1-standalone` - linux; s390x

```console
$ docker pull adminer@sha256:0832c83b0a0b564f962bc8f2f82974852bda2c876629b26a32e31e5b99e8fbc0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.7 MB (93709271 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72ed9e5473cf095c9f6c3263d8ff775ee9a240aa6597b921ebd51ec24f8978c1`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Tue, 21 Nov 2023 05:04:52 GMT
ADD file:b0a8fd50925b3555a0c10177e65551cae288917f9bad8fb4728ec83cc0765afe in / 
# Tue, 21 Nov 2023 05:05:01 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 06:04:07 GMT
STOPSIGNAL SIGINT
# Tue, 21 Nov 2023 06:04:29 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 06:04:35 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 21 Nov 2023 06:04:35 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 21 Nov 2023 06:04:36 GMT
WORKDIR /var/www/html
# Tue, 21 Nov 2023 06:04:36 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 21 Nov 2023 06:04:36 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 21 Nov 2023 06:04:36 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 21 Nov 2023 06:04:36 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 21 Nov 2023 06:04:45 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Nov 2023 06:04:46 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 21 Nov 2023 06:04:46 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 21 Nov 2023 06:04:46 GMT
USER adminer
# Tue, 21 Nov 2023 06:04:46 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Tue, 21 Nov 2023 06:04:47 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:9488c1539560318cb45b39150f91e365b928c0a246788663f5c72d185864bd3e`  
		Last Modified: Tue, 21 Nov 2023 05:10:34 GMT  
		Size: 53.3 MB (53296396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09efec12dc42685e3fe1693d18bc42d61971044de30a99ee3f044d942e93a470`  
		Last Modified: Tue, 21 Nov 2023 06:05:38 GMT  
		Size: 39.0 MB (39022251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d211af034ddf5d1e81df73b8d237d1c15d165b5443c533eedbeecc5659d4d4b`  
		Last Modified: Tue, 21 Nov 2023 06:05:31 GMT  
		Size: 393.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd2e9fc8bb5d1ec8686111ad3e20155b1ac539fc01b742c2318311374c9c3d29`  
		Last Modified: Tue, 21 Nov 2023 06:05:31 GMT  
		Size: 1.9 KB (1877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2acddcee94070eff9faaeaa170066fa650714281ae6b3094fc1d49c010f3902`  
		Last Modified: Tue, 21 Nov 2023 06:05:31 GMT  
		Size: 1.5 KB (1480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21ffbd0e004b4f2f9f75bdc6731ed7d644c91ee50221377d2ff00e82aa1f99b9`  
		Last Modified: Tue, 21 Nov 2023 06:05:31 GMT  
		Size: 1.4 MB (1386383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44baab47b2128777f4b94d45e4a91e7bd440dcb23e61b28ec31c8ac469b3cf40`  
		Last Modified: Tue, 21 Nov 2023 06:05:31 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `adminer:fastcgi`

```console
$ docker pull adminer@sha256:daa291dff0f15be3ba5d0a8cfdcf137d8dd0b1f9304d132c686a4e95dcd489dd
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
$ docker pull adminer@sha256:8440f4060b767baf10aa0a817bae4ebe1d2991721279fdc2656503639463bd7b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.9 MB (95944774 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e93286ecedd0f7ab872f2a51eafc625c321f348ed0da94d7f8364be85227c44`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:46 GMT
ADD file:71543995e4d314b0c86da5ddf8e0cb74649767d30b3e5b6261360de354f0567b in / 
# Tue, 21 Nov 2023 05:21:46 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 09:49:06 GMT
STOPSIGNAL SIGINT
# Tue, 21 Nov 2023 09:49:25 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 09:49:26 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 21 Nov 2023 09:49:47 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Tue, 21 Nov 2023 09:49:47 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 21 Nov 2023 09:49:48 GMT
WORKDIR /var/www/html
# Tue, 21 Nov 2023 09:49:48 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 21 Nov 2023 09:49:48 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 21 Nov 2023 09:49:48 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 21 Nov 2023 09:49:48 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 21 Nov 2023 09:49:59 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Nov 2023 09:49:59 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 21 Nov 2023 09:49:59 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 21 Nov 2023 09:49:59 GMT
USER adminer
# Tue, 21 Nov 2023 09:49:59 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:d1da99c2f14827498c4a9bb3623ae909b44564bdabad1802f064169069df81fb`  
		Last Modified: Tue, 21 Nov 2023 05:26:17 GMT  
		Size: 55.1 MB (55057903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d7c776bdbb7e1224dedbc306fec7eb6e3842bd895a396927c36fa7f434312a3`  
		Last Modified: Tue, 21 Nov 2023 09:50:18 GMT  
		Size: 39.5 MB (39493553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:987d0f042e915521e94497a8e40892d4ec0532bd7641920df5ace1000310d793`  
		Last Modified: Tue, 21 Nov 2023 09:50:10 GMT  
		Size: 389.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38f43fc128ac2c6808d4b9a8087484f11d8cd4105abf9cd319353086c9b3b1d6`  
		Last Modified: Tue, 21 Nov 2023 09:50:34 GMT  
		Size: 2.7 KB (2714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96fdd5fed3b41dde57c97813fce8fc18ab9b07901345f868f32d346cfc74eb01`  
		Last Modified: Tue, 21 Nov 2023 09:50:34 GMT  
		Size: 1.9 KB (1878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3322f8293171857aeafd5fe96548028722034a3151f51dc695cc3cbef006e6a8`  
		Last Modified: Tue, 21 Nov 2023 09:50:34 GMT  
		Size: 1.5 KB (1480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2653b5cb64efa6e1c82031fa6e50d69957ca93e7f1660cc5e97344e601703f8e`  
		Last Modified: Tue, 21 Nov 2023 09:50:34 GMT  
		Size: 1.4 MB (1386365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5038798e96f08d106fc18e6a12538f783f08af440d0957a26c321901ebbad4b`  
		Last Modified: Tue, 21 Nov 2023 09:50:34 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:fastcgi` - linux; arm variant v5

```console
$ docker pull adminer@sha256:b8f1ebac81289510963e10734e0ac78c24878a69d7aebbb9a3a29789c26dbfac
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.2 MB (91208572 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f60ec0b531cc5d09c3980c35d88d86cc1f9b8542ad54fcf7ff77d98ac3dea22`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Tue, 21 Nov 2023 05:01:00 GMT
ADD file:a5c8bd4b0873bd9ad0402143df41b5fd89c50bd24bb071b7d010919e189d88f9 in / 
# Tue, 21 Nov 2023 05:01:00 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 05:46:09 GMT
STOPSIGNAL SIGINT
# Tue, 21 Nov 2023 05:46:38 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 05:46:39 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 21 Nov 2023 05:46:58 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Tue, 21 Nov 2023 05:46:58 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 21 Nov 2023 05:46:58 GMT
WORKDIR /var/www/html
# Tue, 21 Nov 2023 05:46:58 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 21 Nov 2023 05:46:58 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 21 Nov 2023 05:46:58 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 21 Nov 2023 05:46:59 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 21 Nov 2023 05:47:15 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Nov 2023 05:47:15 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 21 Nov 2023 05:47:15 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 21 Nov 2023 05:47:15 GMT
USER adminer
# Tue, 21 Nov 2023 05:47:15 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:7378d71ea16926a061a2edbf0eb3dd13563fcb3ba9cf139c25e8334b36db1adf`  
		Last Modified: Tue, 21 Nov 2023 05:04:15 GMT  
		Size: 52.6 MB (52562921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cde673c33e7bfa6c04aeb9e184923984b648ae971715981d598aca5162e3c911`  
		Last Modified: Tue, 21 Nov 2023 05:47:34 GMT  
		Size: 37.3 MB (37252430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4fee5ad01a4adcbc52d632521a683e83dd44bb905a3048fc20faaa96d58f747`  
		Last Modified: Tue, 21 Nov 2023 05:47:25 GMT  
		Size: 386.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5f71f261b85a2e069d758daa1be7f3e53672fa4b8902826510a9159db451264`  
		Last Modified: Tue, 21 Nov 2023 05:47:51 GMT  
		Size: 2.7 KB (2705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d67d58698593646eb7ab4b717360bf37ab36a671802cb216b3262ce695ef1e5`  
		Last Modified: Tue, 21 Nov 2023 05:47:51 GMT  
		Size: 1.9 KB (1870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d309e407d77f27b1a5409e0ce83c664cb9f080a3168176e8114376d8721a153e`  
		Last Modified: Tue, 21 Nov 2023 05:47:51 GMT  
		Size: 1.5 KB (1477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ee0aa3b9dd1374206375afa28a3b15aa7e6b58abf1b669705b9a86f43e0be79`  
		Last Modified: Tue, 21 Nov 2023 05:47:51 GMT  
		Size: 1.4 MB (1386292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74eeb313bede5967e1e4dd1a8bef17eda92f71136ff55d6ed522d984a8712436`  
		Last Modified: Tue, 21 Nov 2023 05:47:51 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:fastcgi` - linux; arm variant v7

```console
$ docker pull adminer@sha256:1674e094629be082c484d9c7c974fa715e706fbf661bafc68bad546bed9ffe00
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.8 MB (87799571 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c995386759ce4cef4ffbcffb5be8163c9813d2a8220561e9a841f14fb07e0bd`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Tue, 21 Nov 2023 03:57:54 GMT
ADD file:ed8d88d0476fad37879d872d61d05a8cffff35609566f080f78bb882d1bae26b in / 
# Tue, 21 Nov 2023 03:57:54 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 06:58:56 GMT
STOPSIGNAL SIGINT
# Tue, 21 Nov 2023 06:59:20 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 06:59:21 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 21 Nov 2023 06:59:45 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Tue, 21 Nov 2023 06:59:46 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 21 Nov 2023 06:59:46 GMT
WORKDIR /var/www/html
# Tue, 21 Nov 2023 06:59:46 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 21 Nov 2023 06:59:46 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 21 Nov 2023 06:59:47 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 21 Nov 2023 06:59:47 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 21 Nov 2023 07:00:00 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Nov 2023 07:00:01 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 21 Nov 2023 07:00:01 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 21 Nov 2023 07:00:01 GMT
USER adminer
# Tue, 21 Nov 2023 07:00:01 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:1dac19092a737e476f9b096fe28463512ae21c4f596dd2f8b84d62530416dffe`  
		Last Modified: Tue, 21 Nov 2023 04:02:11 GMT  
		Size: 50.2 MB (50215653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2f8153e5d67bc5a0049a12eb2430f50747238b7d4023cacdfc5dad9cdbd244a`  
		Last Modified: Tue, 21 Nov 2023 07:00:24 GMT  
		Size: 36.2 MB (36190640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ea62b864a160dff0b693d9397a8b84a1bc65e8e381b223294a8ac5ac8c68b8a`  
		Last Modified: Tue, 21 Nov 2023 07:00:15 GMT  
		Size: 393.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e77dfeac49a3de3540eb4b5ade85851c08d2523b73c838b14a68fe81a3ec17a1`  
		Last Modified: Tue, 21 Nov 2023 07:00:40 GMT  
		Size: 2.7 KB (2715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e25f712f1f600f798ffd1261db13ef564f0af09c7c65533ed8ed59ec3b26552`  
		Last Modified: Tue, 21 Nov 2023 07:00:40 GMT  
		Size: 1.9 KB (1871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81cdb234e089dedc46386bbac8970166dab2d606288d8c1d426d4b4e617dc9dc`  
		Last Modified: Tue, 21 Nov 2023 07:00:41 GMT  
		Size: 1.5 KB (1476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fea6f1b6b2d8c666838e4a7ca42f2fbcfe498fc2a0eea88d569639836fa56140`  
		Last Modified: Tue, 21 Nov 2023 07:00:41 GMT  
		Size: 1.4 MB (1386332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fd0838894de2a37bd6487e6cf8b3c35ea2ee2e2793979871db8f810c871abd4`  
		Last Modified: Tue, 21 Nov 2023 07:00:41 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:fastcgi` - linux; arm64 variant v8

```console
$ docker pull adminer@sha256:84a893178255bde14cc03ffe152122623fe05eb3839e5f5bae856fb7da83814b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.3 MB (94348838 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b1d17ed2083c8a28275848906f461bdfdb42e15994ac21d9a62087dc6d034d2`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:13 GMT
ADD file:614987b9855939825ad2383e7bacbf14ea208d74906982bba3a67126702c8371 in / 
# Tue, 21 Nov 2023 06:27:13 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 10:22:26 GMT
STOPSIGNAL SIGINT
# Tue, 21 Nov 2023 10:22:43 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 10:22:44 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 21 Nov 2023 10:23:00 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Tue, 21 Nov 2023 10:23:00 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 21 Nov 2023 10:23:00 GMT
WORKDIR /var/www/html
# Tue, 21 Nov 2023 10:23:00 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 21 Nov 2023 10:23:00 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 21 Nov 2023 10:23:00 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 21 Nov 2023 10:23:01 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 21 Nov 2023 10:23:10 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Nov 2023 10:23:11 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 21 Nov 2023 10:23:11 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 21 Nov 2023 10:23:11 GMT
USER adminer
# Tue, 21 Nov 2023 10:23:11 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:bbf382c14c7b19b81c612f639e09e6a7b04eccd4481d0abac48b8ace9faae3b3`  
		Last Modified: Tue, 21 Nov 2023 06:30:47 GMT  
		Size: 53.7 MB (53707872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aa045892ab5d3693eb19355bad15725aa10139ceb2bfc2cb6141778f671e8e4`  
		Last Modified: Tue, 21 Nov 2023 10:23:29 GMT  
		Size: 39.2 MB (39247701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d77bfaecae2cacef431f4d68d17c26be0ab2300b5dfee893959aaae0c6427677`  
		Last Modified: Tue, 21 Nov 2023 10:23:21 GMT  
		Size: 386.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0caf62f5f6228f681c738a20ff40e768d645f553295e9a804e07c9983f280b5`  
		Last Modified: Tue, 21 Nov 2023 10:23:46 GMT  
		Size: 2.7 KB (2705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2df7041a632dc747d7c856a4b14a181da3e49fb1fb8e613f35a8b25404cb7269`  
		Last Modified: Tue, 21 Nov 2023 10:23:46 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c1e97ecf3d9ca77aee6de698d163482237c5a78acbe0e5ff1e47768d6e3fcb6`  
		Last Modified: Tue, 21 Nov 2023 10:23:46 GMT  
		Size: 1.5 KB (1477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce1ef470c48dc65a0917a06d12f3b23a206308eedf67bb228f570870947eb345`  
		Last Modified: Tue, 21 Nov 2023 10:23:47 GMT  
		Size: 1.4 MB (1386324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9363d2b46e93f744f02df5f1ad6d68e5d6ec8debff805842925426c2c0853d95`  
		Last Modified: Tue, 21 Nov 2023 10:23:46 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:fastcgi` - linux; 386

```console
$ docker pull adminer@sha256:063600a67051477eb2d252722e908e12954e92aa2f1103c08bc6ec0c98c81900
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.0 MB (97001696 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9faffd6534bfd19c55ba87d0ea06c0dec17f32f96aaf19d3d273080350957b57`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Tue, 21 Nov 2023 04:40:03 GMT
ADD file:54170328827ccc52692c964f0c45a65ed6efdf39897f2c226672fdf526f3c412 in / 
# Tue, 21 Nov 2023 04:40:04 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 15:41:51 GMT
STOPSIGNAL SIGINT
# Tue, 21 Nov 2023 15:42:20 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 15:42:21 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 21 Nov 2023 15:42:40 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Tue, 21 Nov 2023 15:42:40 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 21 Nov 2023 15:42:41 GMT
WORKDIR /var/www/html
# Tue, 21 Nov 2023 15:42:41 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 21 Nov 2023 15:42:41 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 21 Nov 2023 15:42:41 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 21 Nov 2023 15:42:41 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 21 Nov 2023 15:42:56 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Nov 2023 15:42:56 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 21 Nov 2023 15:42:56 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 21 Nov 2023 15:42:56 GMT
USER adminer
# Tue, 21 Nov 2023 15:42:56 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:e33c1468a29e45636d4d9529b663048f7e8aa83ff428eb0681253bd4200e23ec`  
		Last Modified: Tue, 21 Nov 2023 04:44:57 GMT  
		Size: 56.0 MB (56046301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8137e600c481ac4ed29cae88512a113a2eadcc1d26e72628216670ef4f61ba30`  
		Last Modified: Tue, 21 Nov 2023 15:43:16 GMT  
		Size: 39.6 MB (39562172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e42a8870a081f3a4ab284980034bebec6585740c88e4c40ae98b2e1fa9955f5`  
		Last Modified: Tue, 21 Nov 2023 15:43:05 GMT  
		Size: 392.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ea29f8bfe081038362130d161f4fce7184b04e8b23e4e6eb76012853b52eb29`  
		Last Modified: Tue, 21 Nov 2023 15:43:34 GMT  
		Size: 2.7 KB (2711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c61c47ded185575a69531bea47b571461b9b5a7dbe771c12d9a5351c2274616`  
		Last Modified: Tue, 21 Nov 2023 15:43:34 GMT  
		Size: 1.9 KB (1867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce13699c4877d6078a5c0d0891b3ab176e81a19c03c25322e69a1da82443611a`  
		Last Modified: Tue, 21 Nov 2023 15:43:34 GMT  
		Size: 1.5 KB (1480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:467cdaa3b936c126690238f64a0f87f1ea5c53e47ad6b7a300a08e68304b4c5e`  
		Last Modified: Tue, 21 Nov 2023 15:43:34 GMT  
		Size: 1.4 MB (1386283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08c8258bd975965d721bb178e601818437b2ec83ecf04991a03e7ac42e8262f1`  
		Last Modified: Tue, 21 Nov 2023 15:43:34 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:fastcgi` - linux; mips64le

```console
$ docker pull adminer@sha256:a764c136226771f05874d428d466ab7617443109af05761f5a301d774d3d78ef
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.6 MB (92637624 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6dcb8d7570466b2e24f152459f05444501a2db6bec81dd770f36a922da335bf3`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Tue, 21 Nov 2023 04:10:25 GMT
ADD file:dbfc3d226166089c4db0c154fdcea8049b8758c6812f1c397dec1444985e8557 in / 
# Tue, 21 Nov 2023 04:10:31 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 12:14:44 GMT
STOPSIGNAL SIGINT
# Tue, 21 Nov 2023 12:16:43 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 12:16:50 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 21 Nov 2023 12:18:45 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Tue, 21 Nov 2023 12:18:52 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 21 Nov 2023 12:18:55 GMT
WORKDIR /var/www/html
# Tue, 21 Nov 2023 12:18:59 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 21 Nov 2023 12:19:02 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 21 Nov 2023 12:19:05 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 21 Nov 2023 12:19:09 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 21 Nov 2023 12:20:00 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Nov 2023 12:20:03 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 21 Nov 2023 12:20:06 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 21 Nov 2023 12:20:10 GMT
USER adminer
# Tue, 21 Nov 2023 12:20:13 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:ca31218601e95f4aafae0dcadda7600aeb04db374e1e829d5c123f8033ba3472`  
		Last Modified: Tue, 21 Nov 2023 04:21:21 GMT  
		Size: 53.3 MB (53289162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d172a1ce4463b8a1bb14b88d9f7c98a7f06f260dfc2849e77f3d41be6d17db9`  
		Last Modified: Tue, 21 Nov 2023 12:21:00 GMT  
		Size: 38.0 MB (37954467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbd3b039fbc0efa77466cfb045c80c120d45355cf2db0dd6533eeb1cee6296e1`  
		Last Modified: Tue, 21 Nov 2023 12:20:33 GMT  
		Size: 394.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:873ce81c2a5a659c6ba90c59b5fdd1a3c215439a655c8efe1b62a042ba6dc956`  
		Last Modified: Tue, 21 Nov 2023 12:21:19 GMT  
		Size: 2.7 KB (2714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:046c3c9cda84191a448b5676717eb2efd43aa616bd1a7936fd1ffa7333fe414d`  
		Last Modified: Tue, 21 Nov 2023 12:21:19 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d5fb1a0ccda92972577970b93a35e31e87aca9efdf320fe33d64fbb50e5f5be`  
		Last Modified: Tue, 21 Nov 2023 12:21:19 GMT  
		Size: 1.5 KB (1479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16f226ce3836498318ee4d4f1573efc49e08a2a6cdfd7403a3089f66f24194f3`  
		Last Modified: Tue, 21 Nov 2023 12:21:20 GMT  
		Size: 1.4 MB (1387178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc2ef37541c711003007d218f46c929098bfda475d45d9ced2d3700246c0d143`  
		Last Modified: Tue, 21 Nov 2023 12:21:19 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:fastcgi` - linux; ppc64le

```console
$ docker pull adminer@sha256:988a50cb007ef650a43dfb195f4730d2268d36b717db2cdbc731914c725ee8df
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.3 MB (101268149 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f2e2a636068dd83fb84a9bcecd6a718528598da747489d7573b02bdfa6f20140`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Tue, 21 Nov 2023 04:24:26 GMT
ADD file:c21c2b6cb3f9bdf6cc3641e9ebf810a461174480c6cd1c25515cf9fce4aa2143 in / 
# Tue, 21 Nov 2023 04:24:30 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 06:49:59 GMT
STOPSIGNAL SIGINT
# Tue, 21 Nov 2023 06:50:40 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 06:50:42 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 21 Nov 2023 06:51:10 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Tue, 21 Nov 2023 06:51:11 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 21 Nov 2023 06:51:11 GMT
WORKDIR /var/www/html
# Tue, 21 Nov 2023 06:51:12 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 21 Nov 2023 06:51:12 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 21 Nov 2023 06:51:12 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 21 Nov 2023 06:51:13 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 21 Nov 2023 06:51:30 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Nov 2023 06:51:30 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 21 Nov 2023 06:51:30 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 21 Nov 2023 06:51:31 GMT
USER adminer
# Tue, 21 Nov 2023 06:51:31 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:23ebe74b854f8f6e2671f4c8cc147a6925fb7d929ce5898f7ca2af9781bf7d38`  
		Last Modified: Tue, 21 Nov 2023 04:29:21 GMT  
		Size: 58.9 MB (58929678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa255108512a37e57b2fdf827a0fdb4e3783a0649fb80ecdd431d4921dd6761c`  
		Last Modified: Tue, 21 Nov 2023 06:51:51 GMT  
		Size: 40.9 MB (40945122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5862ce535fc870ad9665c04e9816effde44c5f4469bc852265ba0bfe11ad7001`  
		Last Modified: Tue, 21 Nov 2023 06:51:41 GMT  
		Size: 391.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eb07c0427e1d513dc1c2e122ef9b33a7ce04c7f6e7ac25eb3cdc16b7c4f3dd0`  
		Last Modified: Tue, 21 Nov 2023 06:52:10 GMT  
		Size: 2.7 KB (2709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e1a3baf382e8ecd698319193729a0416bcdcbe069383e956a41029751483ab8`  
		Last Modified: Tue, 21 Nov 2023 06:52:10 GMT  
		Size: 1.9 KB (1878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd36769ccabc572d519d259cd2369096462f35a823d2817c593ce165f30f690b`  
		Last Modified: Tue, 21 Nov 2023 06:52:10 GMT  
		Size: 1.5 KB (1480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e35256cd8ee36eeca9a95cc2fc4ad45b213f5025c0d7211c00f76beae6c7a0bd`  
		Last Modified: Tue, 21 Nov 2023 06:52:11 GMT  
		Size: 1.4 MB (1386400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:417adc53867ad9b9d99a43bc9736c1285bc9af029e2938bd516928b92cad7093`  
		Last Modified: Tue, 21 Nov 2023 06:52:10 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:fastcgi` - linux; s390x

```console
$ docker pull adminer@sha256:8920ecc20283083c9296766b19c975eabf1764eecadbcd7b97ed7bb11e30921e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.7 MB (93711989 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33df00454cb56b58abb106b0161ca460cdce0f5d1f8162177becb869dde24b99`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Tue, 21 Nov 2023 05:04:52 GMT
ADD file:b0a8fd50925b3555a0c10177e65551cae288917f9bad8fb4728ec83cc0765afe in / 
# Tue, 21 Nov 2023 05:05:01 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 06:04:07 GMT
STOPSIGNAL SIGINT
# Tue, 21 Nov 2023 06:04:29 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 06:04:35 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 21 Nov 2023 06:05:00 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Tue, 21 Nov 2023 06:05:00 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 21 Nov 2023 06:05:00 GMT
WORKDIR /var/www/html
# Tue, 21 Nov 2023 06:05:01 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 21 Nov 2023 06:05:01 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 21 Nov 2023 06:05:01 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 21 Nov 2023 06:05:01 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 21 Nov 2023 06:05:11 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Nov 2023 06:05:11 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 21 Nov 2023 06:05:11 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 21 Nov 2023 06:05:12 GMT
USER adminer
# Tue, 21 Nov 2023 06:05:12 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:9488c1539560318cb45b39150f91e365b928c0a246788663f5c72d185864bd3e`  
		Last Modified: Tue, 21 Nov 2023 05:10:34 GMT  
		Size: 53.3 MB (53296396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09efec12dc42685e3fe1693d18bc42d61971044de30a99ee3f044d942e93a470`  
		Last Modified: Tue, 21 Nov 2023 06:05:38 GMT  
		Size: 39.0 MB (39022251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d211af034ddf5d1e81df73b8d237d1c15d165b5443c533eedbeecc5659d4d4b`  
		Last Modified: Tue, 21 Nov 2023 06:05:31 GMT  
		Size: 393.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32f1b2d24e5fca07170540193831c2b4e39ddb10d4fc7736e631b2aa11ed601a`  
		Last Modified: Tue, 21 Nov 2023 06:05:48 GMT  
		Size: 2.7 KB (2711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6439585d05cece3d9af2be5ecb1d12bf8e78e1a23a419fb2f49451ede72e90ba`  
		Last Modified: Tue, 21 Nov 2023 06:05:48 GMT  
		Size: 1.9 KB (1879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aea2cdf22e5a5de0f7b5cc6c97c9c03a8fe82113a1d7d5153a55592fdf09568`  
		Last Modified: Tue, 21 Nov 2023 06:05:48 GMT  
		Size: 1.5 KB (1479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:922a0d106738cf725844ac8a3a5ef1352d0048149982aee61fe3d0f67bb8a041`  
		Last Modified: Tue, 21 Nov 2023 06:05:48 GMT  
		Size: 1.4 MB (1386389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:791aaf97ba65859a96b769218ea3ab780b809cc6bcacb784b88c24756e99ef6b`  
		Last Modified: Tue, 21 Nov 2023 06:05:48 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `adminer:latest`

```console
$ docker pull adminer@sha256:0ce7583815dabdd9f560ee0afed630ecb33df6756f4b66c85c197011559a0248
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
$ docker pull adminer@sha256:78d95e4c7a6cfb584a500e0e8ca7db956ab9ff1cd4b3239306b330c2637ecfa2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.9 MB (95942047 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7554c8e10d81e451e656e73d613de4f9c885b91255f46a2fdc03ccf275a1d449`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:46 GMT
ADD file:71543995e4d314b0c86da5ddf8e0cb74649767d30b3e5b6261360de354f0567b in / 
# Tue, 21 Nov 2023 05:21:46 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 09:49:06 GMT
STOPSIGNAL SIGINT
# Tue, 21 Nov 2023 09:49:25 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 09:49:26 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 21 Nov 2023 09:49:27 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 21 Nov 2023 09:49:27 GMT
WORKDIR /var/www/html
# Tue, 21 Nov 2023 09:49:27 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 21 Nov 2023 09:49:27 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 21 Nov 2023 09:49:27 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 21 Nov 2023 09:49:27 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 21 Nov 2023 09:49:39 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Nov 2023 09:49:39 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 21 Nov 2023 09:49:39 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 21 Nov 2023 09:49:39 GMT
USER adminer
# Tue, 21 Nov 2023 09:49:39 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Tue, 21 Nov 2023 09:49:39 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:d1da99c2f14827498c4a9bb3623ae909b44564bdabad1802f064169069df81fb`  
		Last Modified: Tue, 21 Nov 2023 05:26:17 GMT  
		Size: 55.1 MB (55057903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d7c776bdbb7e1224dedbc306fec7eb6e3842bd895a396927c36fa7f434312a3`  
		Last Modified: Tue, 21 Nov 2023 09:50:18 GMT  
		Size: 39.5 MB (39493553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:987d0f042e915521e94497a8e40892d4ec0532bd7641920df5ace1000310d793`  
		Last Modified: Tue, 21 Nov 2023 09:50:10 GMT  
		Size: 389.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb163dc8650b5fde5c72f76b8937b3c38d3dd4c7a2922d7b6f95a0890070c4d9`  
		Last Modified: Tue, 21 Nov 2023 09:50:10 GMT  
		Size: 1.9 KB (1878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98b256c86f3d5b1eab91122ae075d7b3b15d1185ebe1cc10a8b4d2fb6f2bdf5f`  
		Last Modified: Tue, 21 Nov 2023 09:50:10 GMT  
		Size: 1.5 KB (1480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7952b9a84b1867112d08313ef023ee4917d7bbd0f91f4d8ae3ce1b17376d345e`  
		Last Modified: Tue, 21 Nov 2023 09:50:11 GMT  
		Size: 1.4 MB (1386353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77cf83a8d79b963388e7d18d6836ac44d7832d08fa39ab46ba57f0c92e48e1f2`  
		Last Modified: Tue, 21 Nov 2023 09:50:10 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:latest` - linux; arm variant v5

```console
$ docker pull adminer@sha256:f6bb8e720054e43d3bc65a163e9fc4146ce4c215db05216f56be5cbac7428eb7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.2 MB (91205860 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9bd45b72f483757bdbd0f31b96e08578a127cc80966526aa0a9a897f5012203`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Tue, 21 Nov 2023 05:01:00 GMT
ADD file:a5c8bd4b0873bd9ad0402143df41b5fd89c50bd24bb071b7d010919e189d88f9 in / 
# Tue, 21 Nov 2023 05:01:00 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 05:46:09 GMT
STOPSIGNAL SIGINT
# Tue, 21 Nov 2023 05:46:38 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 05:46:39 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 21 Nov 2023 05:46:40 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 21 Nov 2023 05:46:40 GMT
WORKDIR /var/www/html
# Tue, 21 Nov 2023 05:46:40 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 21 Nov 2023 05:46:40 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 21 Nov 2023 05:46:40 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 21 Nov 2023 05:46:40 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 21 Nov 2023 05:46:55 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Nov 2023 05:46:55 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 21 Nov 2023 05:46:55 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 21 Nov 2023 05:46:55 GMT
USER adminer
# Tue, 21 Nov 2023 05:46:55 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Tue, 21 Nov 2023 05:46:55 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:7378d71ea16926a061a2edbf0eb3dd13563fcb3ba9cf139c25e8334b36db1adf`  
		Last Modified: Tue, 21 Nov 2023 05:04:15 GMT  
		Size: 52.6 MB (52562921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cde673c33e7bfa6c04aeb9e184923984b648ae971715981d598aca5162e3c911`  
		Last Modified: Tue, 21 Nov 2023 05:47:34 GMT  
		Size: 37.3 MB (37252430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4fee5ad01a4adcbc52d632521a683e83dd44bb905a3048fc20faaa96d58f747`  
		Last Modified: Tue, 21 Nov 2023 05:47:25 GMT  
		Size: 386.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:062df034c3a9a14a736fb1733f5f91b8c5cad9974f6b67df85f488a45026f47c`  
		Last Modified: Tue, 21 Nov 2023 05:47:24 GMT  
		Size: 1.9 KB (1869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:610f64ab71d9f5c7abad4551870c223a9b95603025384ef1e7a85f624f0b0467`  
		Last Modified: Tue, 21 Nov 2023 05:47:24 GMT  
		Size: 1.5 KB (1481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59cca3ff7ed68079f673662534d292a264aa5c1d7d4358251d8e25f21faa9f94`  
		Last Modified: Tue, 21 Nov 2023 05:47:25 GMT  
		Size: 1.4 MB (1386281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:753ad2913e083c1b5cb5b06853944934450629b0451d408743ddffc1f4c0a843`  
		Last Modified: Tue, 21 Nov 2023 05:47:24 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:latest` - linux; arm variant v7

```console
$ docker pull adminer@sha256:6faef276799d02bdd9abf0ba022b692fd46f8144584adcfa771a76d225131045
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.8 MB (87796870 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9bb280f29bbaaa440662c6cbd26fabd7313fb299195b0ff2ca0cc22cff61f1ab`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Tue, 21 Nov 2023 03:57:54 GMT
ADD file:ed8d88d0476fad37879d872d61d05a8cffff35609566f080f78bb882d1bae26b in / 
# Tue, 21 Nov 2023 03:57:54 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 06:58:56 GMT
STOPSIGNAL SIGINT
# Tue, 21 Nov 2023 06:59:20 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 06:59:21 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 21 Nov 2023 06:59:21 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 21 Nov 2023 06:59:21 GMT
WORKDIR /var/www/html
# Tue, 21 Nov 2023 06:59:21 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 21 Nov 2023 06:59:21 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 21 Nov 2023 06:59:21 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 21 Nov 2023 06:59:22 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 21 Nov 2023 06:59:37 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Nov 2023 06:59:37 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 21 Nov 2023 06:59:37 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 21 Nov 2023 06:59:37 GMT
USER adminer
# Tue, 21 Nov 2023 06:59:37 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Tue, 21 Nov 2023 06:59:37 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:1dac19092a737e476f9b096fe28463512ae21c4f596dd2f8b84d62530416dffe`  
		Last Modified: Tue, 21 Nov 2023 04:02:11 GMT  
		Size: 50.2 MB (50215653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2f8153e5d67bc5a0049a12eb2430f50747238b7d4023cacdfc5dad9cdbd244a`  
		Last Modified: Tue, 21 Nov 2023 07:00:24 GMT  
		Size: 36.2 MB (36190640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ea62b864a160dff0b693d9397a8b84a1bc65e8e381b223294a8ac5ac8c68b8a`  
		Last Modified: Tue, 21 Nov 2023 07:00:15 GMT  
		Size: 393.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e2dd6fa8973e47e4cce58445b7207793f22b2371aa58678dc17d4172eac0b32`  
		Last Modified: Tue, 21 Nov 2023 07:00:15 GMT  
		Size: 1.9 KB (1871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4d33015217bf866b0d2c44cd29bf71617469b2e87e38eb15795aa3a293c83fa`  
		Last Modified: Tue, 21 Nov 2023 07:00:16 GMT  
		Size: 1.5 KB (1478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24ee8e39b9683ef6aa34033169655e5585db29d9557c0e1eb9aa117e1c771047`  
		Last Modified: Tue, 21 Nov 2023 07:00:16 GMT  
		Size: 1.4 MB (1386341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c14859802a2676aa6a511bbd06ce80a759e38e94927cd4d4b60dd202568ef5b`  
		Last Modified: Tue, 21 Nov 2023 07:00:15 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:latest` - linux; arm64 variant v8

```console
$ docker pull adminer@sha256:e5fda74f5900f3c7ef8f74bda0392b45089f33f56374326bb331d8db26eb8b41
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.3 MB (94346130 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ccf82dd602ee08aa22718c108fcbcedbebb819a09c86b9f0fe8f2c1737bd08a7`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:13 GMT
ADD file:614987b9855939825ad2383e7bacbf14ea208d74906982bba3a67126702c8371 in / 
# Tue, 21 Nov 2023 06:27:13 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 10:22:26 GMT
STOPSIGNAL SIGINT
# Tue, 21 Nov 2023 10:22:43 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 10:22:44 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 21 Nov 2023 10:22:44 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 21 Nov 2023 10:22:44 GMT
WORKDIR /var/www/html
# Tue, 21 Nov 2023 10:22:44 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 21 Nov 2023 10:22:44 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 21 Nov 2023 10:22:45 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 21 Nov 2023 10:22:45 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 21 Nov 2023 10:22:54 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Nov 2023 10:22:54 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 21 Nov 2023 10:22:54 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 21 Nov 2023 10:22:54 GMT
USER adminer
# Tue, 21 Nov 2023 10:22:55 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Tue, 21 Nov 2023 10:22:55 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:bbf382c14c7b19b81c612f639e09e6a7b04eccd4481d0abac48b8ace9faae3b3`  
		Last Modified: Tue, 21 Nov 2023 06:30:47 GMT  
		Size: 53.7 MB (53707872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aa045892ab5d3693eb19355bad15725aa10139ceb2bfc2cb6141778f671e8e4`  
		Last Modified: Tue, 21 Nov 2023 10:23:29 GMT  
		Size: 39.2 MB (39247701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d77bfaecae2cacef431f4d68d17c26be0ab2300b5dfee893959aaae0c6427677`  
		Last Modified: Tue, 21 Nov 2023 10:23:21 GMT  
		Size: 386.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1364c7eb4b90daedaca80aff830c09309115f174a295c35ba7885c60557fa1e`  
		Last Modified: Tue, 21 Nov 2023 10:23:21 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:080b929d6ed912f11ed340726920967a938d3632641f4f86e15a30fc7b255888`  
		Last Modified: Tue, 21 Nov 2023 10:23:21 GMT  
		Size: 1.5 KB (1477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:633cfed53ab70b9e08d21a78973fc2a318d49c9cc54f3100604c9b91dd533c82`  
		Last Modified: Tue, 21 Nov 2023 10:23:22 GMT  
		Size: 1.4 MB (1386322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc610b080dd3b327bfe4b6ca8da59bc3a5555a295aff6c4f18d172f070b4e1ab`  
		Last Modified: Tue, 21 Nov 2023 10:23:21 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:latest` - linux; 386

```console
$ docker pull adminer@sha256:173f2532a535a7780bffa43d6385797ba5335ab89832cb016cbb54cb0ab60fb2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.0 MB (96998974 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85b8488ee11e55b40364ca362184cc13095a7b83f1c1e65e524862cc27000db2`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Tue, 21 Nov 2023 04:40:03 GMT
ADD file:54170328827ccc52692c964f0c45a65ed6efdf39897f2c226672fdf526f3c412 in / 
# Tue, 21 Nov 2023 04:40:04 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 15:41:51 GMT
STOPSIGNAL SIGINT
# Tue, 21 Nov 2023 15:42:20 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 15:42:21 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 21 Nov 2023 15:42:22 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 21 Nov 2023 15:42:22 GMT
WORKDIR /var/www/html
# Tue, 21 Nov 2023 15:42:22 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 21 Nov 2023 15:42:22 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 21 Nov 2023 15:42:22 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 21 Nov 2023 15:42:22 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 21 Nov 2023 15:42:37 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Nov 2023 15:42:37 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 21 Nov 2023 15:42:37 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 21 Nov 2023 15:42:37 GMT
USER adminer
# Tue, 21 Nov 2023 15:42:37 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Tue, 21 Nov 2023 15:42:37 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:e33c1468a29e45636d4d9529b663048f7e8aa83ff428eb0681253bd4200e23ec`  
		Last Modified: Tue, 21 Nov 2023 04:44:57 GMT  
		Size: 56.0 MB (56046301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8137e600c481ac4ed29cae88512a113a2eadcc1d26e72628216670ef4f61ba30`  
		Last Modified: Tue, 21 Nov 2023 15:43:16 GMT  
		Size: 39.6 MB (39562172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e42a8870a081f3a4ab284980034bebec6585740c88e4c40ae98b2e1fa9955f5`  
		Last Modified: Tue, 21 Nov 2023 15:43:05 GMT  
		Size: 392.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48c728479be5016dacc84b6c0c244f327eff896df6a326af2826d6ad4c5387b6`  
		Last Modified: Tue, 21 Nov 2023 15:43:05 GMT  
		Size: 1.9 KB (1870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1000dcb7b3ee07a4d8a46142cda4b99b13051577e48599f89d62c8fd8c7e61a8`  
		Last Modified: Tue, 21 Nov 2023 15:43:05 GMT  
		Size: 1.5 KB (1482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d8473e68cd9a1e0940ff9bb80857e7d32bfde252766cc39fc1c3566222b0c1c`  
		Last Modified: Tue, 21 Nov 2023 15:43:06 GMT  
		Size: 1.4 MB (1386265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d7609e79a7e8443050102286e60b2022e9f3447043db395cabb7e2ad151b1e0`  
		Last Modified: Tue, 21 Nov 2023 15:43:05 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:latest` - linux; mips64le

```console
$ docker pull adminer@sha256:84b1c19875f37b42946db21b87c80b8f8d9d9c7392eff0a7a065cf6d5fe769b2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.6 MB (92634921 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6454361a51d8f0d5781cd1854359c6b0812cc29466f516dd6386754b3583699`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Tue, 21 Nov 2023 04:10:25 GMT
ADD file:dbfc3d226166089c4db0c154fdcea8049b8758c6812f1c397dec1444985e8557 in / 
# Tue, 21 Nov 2023 04:10:31 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 12:14:44 GMT
STOPSIGNAL SIGINT
# Tue, 21 Nov 2023 12:16:43 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 12:16:50 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 21 Nov 2023 12:16:57 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 21 Nov 2023 12:17:00 GMT
WORKDIR /var/www/html
# Tue, 21 Nov 2023 12:17:04 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 21 Nov 2023 12:17:07 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 21 Nov 2023 12:17:10 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 21 Nov 2023 12:17:14 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 21 Nov 2023 12:18:08 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Nov 2023 12:18:11 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 21 Nov 2023 12:18:14 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 21 Nov 2023 12:18:17 GMT
USER adminer
# Tue, 21 Nov 2023 12:18:21 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Tue, 21 Nov 2023 12:18:24 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:ca31218601e95f4aafae0dcadda7600aeb04db374e1e829d5c123f8033ba3472`  
		Last Modified: Tue, 21 Nov 2023 04:21:21 GMT  
		Size: 53.3 MB (53289162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d172a1ce4463b8a1bb14b88d9f7c98a7f06f260dfc2849e77f3d41be6d17db9`  
		Last Modified: Tue, 21 Nov 2023 12:21:00 GMT  
		Size: 38.0 MB (37954467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbd3b039fbc0efa77466cfb045c80c120d45355cf2db0dd6533eeb1cee6296e1`  
		Last Modified: Tue, 21 Nov 2023 12:20:33 GMT  
		Size: 394.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bac97c667ed055993103f32b019a430a853a94eef6bf75086fda9949a9fd1d8`  
		Last Modified: Tue, 21 Nov 2023 12:20:34 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66eec20186701717a98146a63c5c8f88304d44243fe6f6505edf4d1135672446`  
		Last Modified: Tue, 21 Nov 2023 12:20:34 GMT  
		Size: 1.5 KB (1483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a56ddb348b2b13a6cac73829460bdcce2971790b6be59ac9da70b739453488b8`  
		Last Modified: Tue, 21 Nov 2023 12:20:34 GMT  
		Size: 1.4 MB (1387192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f922348b25af66b56cdd7a4863a9a120057afa01489fc9058cf7e975b198d05`  
		Last Modified: Tue, 21 Nov 2023 12:20:34 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:latest` - linux; ppc64le

```console
$ docker pull adminer@sha256:3b96a3711e0e719557e514cb8870567e67ab545a7fe18b4feeca4e0e4c85d678
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.3 MB (101265448 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0c151160d019f74dfe13959cf16722a5172a0023a5f747201c90b752e001545`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Tue, 21 Nov 2023 04:24:26 GMT
ADD file:c21c2b6cb3f9bdf6cc3641e9ebf810a461174480c6cd1c25515cf9fce4aa2143 in / 
# Tue, 21 Nov 2023 04:24:30 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 06:49:59 GMT
STOPSIGNAL SIGINT
# Tue, 21 Nov 2023 06:50:40 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 06:50:42 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 21 Nov 2023 06:50:44 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 21 Nov 2023 06:50:44 GMT
WORKDIR /var/www/html
# Tue, 21 Nov 2023 06:50:44 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 21 Nov 2023 06:50:44 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 21 Nov 2023 06:50:45 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 21 Nov 2023 06:50:45 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 21 Nov 2023 06:51:03 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Nov 2023 06:51:03 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 21 Nov 2023 06:51:03 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 21 Nov 2023 06:51:03 GMT
USER adminer
# Tue, 21 Nov 2023 06:51:04 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Tue, 21 Nov 2023 06:51:04 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:23ebe74b854f8f6e2671f4c8cc147a6925fb7d929ce5898f7ca2af9781bf7d38`  
		Last Modified: Tue, 21 Nov 2023 04:29:21 GMT  
		Size: 58.9 MB (58929678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa255108512a37e57b2fdf827a0fdb4e3783a0649fb80ecdd431d4921dd6761c`  
		Last Modified: Tue, 21 Nov 2023 06:51:51 GMT  
		Size: 40.9 MB (40945122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5862ce535fc870ad9665c04e9816effde44c5f4469bc852265ba0bfe11ad7001`  
		Last Modified: Tue, 21 Nov 2023 06:51:41 GMT  
		Size: 391.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7204feb32d0a6fe6dd0348f7a8c2845b90b631ba893c08c48a724057c8a5e3d1`  
		Last Modified: Tue, 21 Nov 2023 06:51:41 GMT  
		Size: 1.9 KB (1879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb06eb196e5a191ad6e9d6d43052c2fd0f833100bf197c73f3f9c8df967003d1`  
		Last Modified: Tue, 21 Nov 2023 06:51:41 GMT  
		Size: 1.5 KB (1482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76df205e8013dede04db80018bebbabea233e0186671f2fd251fa440acde39ef`  
		Last Modified: Tue, 21 Nov 2023 06:51:41 GMT  
		Size: 1.4 MB (1386403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7099dfc32b7ad37a3cfe50e8aad19c609d5e9daf0535dd5cd0f853de87d0de8f`  
		Last Modified: Tue, 21 Nov 2023 06:51:41 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:latest` - linux; s390x

```console
$ docker pull adminer@sha256:0832c83b0a0b564f962bc8f2f82974852bda2c876629b26a32e31e5b99e8fbc0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.7 MB (93709271 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72ed9e5473cf095c9f6c3263d8ff775ee9a240aa6597b921ebd51ec24f8978c1`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Tue, 21 Nov 2023 05:04:52 GMT
ADD file:b0a8fd50925b3555a0c10177e65551cae288917f9bad8fb4728ec83cc0765afe in / 
# Tue, 21 Nov 2023 05:05:01 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 06:04:07 GMT
STOPSIGNAL SIGINT
# Tue, 21 Nov 2023 06:04:29 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 06:04:35 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 21 Nov 2023 06:04:35 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 21 Nov 2023 06:04:36 GMT
WORKDIR /var/www/html
# Tue, 21 Nov 2023 06:04:36 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 21 Nov 2023 06:04:36 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 21 Nov 2023 06:04:36 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 21 Nov 2023 06:04:36 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 21 Nov 2023 06:04:45 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Nov 2023 06:04:46 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 21 Nov 2023 06:04:46 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 21 Nov 2023 06:04:46 GMT
USER adminer
# Tue, 21 Nov 2023 06:04:46 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Tue, 21 Nov 2023 06:04:47 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:9488c1539560318cb45b39150f91e365b928c0a246788663f5c72d185864bd3e`  
		Last Modified: Tue, 21 Nov 2023 05:10:34 GMT  
		Size: 53.3 MB (53296396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09efec12dc42685e3fe1693d18bc42d61971044de30a99ee3f044d942e93a470`  
		Last Modified: Tue, 21 Nov 2023 06:05:38 GMT  
		Size: 39.0 MB (39022251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d211af034ddf5d1e81df73b8d237d1c15d165b5443c533eedbeecc5659d4d4b`  
		Last Modified: Tue, 21 Nov 2023 06:05:31 GMT  
		Size: 393.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd2e9fc8bb5d1ec8686111ad3e20155b1ac539fc01b742c2318311374c9c3d29`  
		Last Modified: Tue, 21 Nov 2023 06:05:31 GMT  
		Size: 1.9 KB (1877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2acddcee94070eff9faaeaa170066fa650714281ae6b3094fc1d49c010f3902`  
		Last Modified: Tue, 21 Nov 2023 06:05:31 GMT  
		Size: 1.5 KB (1480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21ffbd0e004b4f2f9f75bdc6731ed7d644c91ee50221377d2ff00e82aa1f99b9`  
		Last Modified: Tue, 21 Nov 2023 06:05:31 GMT  
		Size: 1.4 MB (1386383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44baab47b2128777f4b94d45e4a91e7bd440dcb23e61b28ec31c8ac469b3cf40`  
		Last Modified: Tue, 21 Nov 2023 06:05:31 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `adminer:standalone`

```console
$ docker pull adminer@sha256:0ce7583815dabdd9f560ee0afed630ecb33df6756f4b66c85c197011559a0248
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
$ docker pull adminer@sha256:78d95e4c7a6cfb584a500e0e8ca7db956ab9ff1cd4b3239306b330c2637ecfa2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.9 MB (95942047 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7554c8e10d81e451e656e73d613de4f9c885b91255f46a2fdc03ccf275a1d449`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:46 GMT
ADD file:71543995e4d314b0c86da5ddf8e0cb74649767d30b3e5b6261360de354f0567b in / 
# Tue, 21 Nov 2023 05:21:46 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 09:49:06 GMT
STOPSIGNAL SIGINT
# Tue, 21 Nov 2023 09:49:25 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 09:49:26 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 21 Nov 2023 09:49:27 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 21 Nov 2023 09:49:27 GMT
WORKDIR /var/www/html
# Tue, 21 Nov 2023 09:49:27 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 21 Nov 2023 09:49:27 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 21 Nov 2023 09:49:27 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 21 Nov 2023 09:49:27 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 21 Nov 2023 09:49:39 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Nov 2023 09:49:39 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 21 Nov 2023 09:49:39 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 21 Nov 2023 09:49:39 GMT
USER adminer
# Tue, 21 Nov 2023 09:49:39 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Tue, 21 Nov 2023 09:49:39 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:d1da99c2f14827498c4a9bb3623ae909b44564bdabad1802f064169069df81fb`  
		Last Modified: Tue, 21 Nov 2023 05:26:17 GMT  
		Size: 55.1 MB (55057903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d7c776bdbb7e1224dedbc306fec7eb6e3842bd895a396927c36fa7f434312a3`  
		Last Modified: Tue, 21 Nov 2023 09:50:18 GMT  
		Size: 39.5 MB (39493553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:987d0f042e915521e94497a8e40892d4ec0532bd7641920df5ace1000310d793`  
		Last Modified: Tue, 21 Nov 2023 09:50:10 GMT  
		Size: 389.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb163dc8650b5fde5c72f76b8937b3c38d3dd4c7a2922d7b6f95a0890070c4d9`  
		Last Modified: Tue, 21 Nov 2023 09:50:10 GMT  
		Size: 1.9 KB (1878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98b256c86f3d5b1eab91122ae075d7b3b15d1185ebe1cc10a8b4d2fb6f2bdf5f`  
		Last Modified: Tue, 21 Nov 2023 09:50:10 GMT  
		Size: 1.5 KB (1480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7952b9a84b1867112d08313ef023ee4917d7bbd0f91f4d8ae3ce1b17376d345e`  
		Last Modified: Tue, 21 Nov 2023 09:50:11 GMT  
		Size: 1.4 MB (1386353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77cf83a8d79b963388e7d18d6836ac44d7832d08fa39ab46ba57f0c92e48e1f2`  
		Last Modified: Tue, 21 Nov 2023 09:50:10 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:standalone` - linux; arm variant v5

```console
$ docker pull adminer@sha256:f6bb8e720054e43d3bc65a163e9fc4146ce4c215db05216f56be5cbac7428eb7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.2 MB (91205860 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9bd45b72f483757bdbd0f31b96e08578a127cc80966526aa0a9a897f5012203`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Tue, 21 Nov 2023 05:01:00 GMT
ADD file:a5c8bd4b0873bd9ad0402143df41b5fd89c50bd24bb071b7d010919e189d88f9 in / 
# Tue, 21 Nov 2023 05:01:00 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 05:46:09 GMT
STOPSIGNAL SIGINT
# Tue, 21 Nov 2023 05:46:38 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 05:46:39 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 21 Nov 2023 05:46:40 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 21 Nov 2023 05:46:40 GMT
WORKDIR /var/www/html
# Tue, 21 Nov 2023 05:46:40 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 21 Nov 2023 05:46:40 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 21 Nov 2023 05:46:40 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 21 Nov 2023 05:46:40 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 21 Nov 2023 05:46:55 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Nov 2023 05:46:55 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 21 Nov 2023 05:46:55 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 21 Nov 2023 05:46:55 GMT
USER adminer
# Tue, 21 Nov 2023 05:46:55 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Tue, 21 Nov 2023 05:46:55 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:7378d71ea16926a061a2edbf0eb3dd13563fcb3ba9cf139c25e8334b36db1adf`  
		Last Modified: Tue, 21 Nov 2023 05:04:15 GMT  
		Size: 52.6 MB (52562921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cde673c33e7bfa6c04aeb9e184923984b648ae971715981d598aca5162e3c911`  
		Last Modified: Tue, 21 Nov 2023 05:47:34 GMT  
		Size: 37.3 MB (37252430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4fee5ad01a4adcbc52d632521a683e83dd44bb905a3048fc20faaa96d58f747`  
		Last Modified: Tue, 21 Nov 2023 05:47:25 GMT  
		Size: 386.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:062df034c3a9a14a736fb1733f5f91b8c5cad9974f6b67df85f488a45026f47c`  
		Last Modified: Tue, 21 Nov 2023 05:47:24 GMT  
		Size: 1.9 KB (1869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:610f64ab71d9f5c7abad4551870c223a9b95603025384ef1e7a85f624f0b0467`  
		Last Modified: Tue, 21 Nov 2023 05:47:24 GMT  
		Size: 1.5 KB (1481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59cca3ff7ed68079f673662534d292a264aa5c1d7d4358251d8e25f21faa9f94`  
		Last Modified: Tue, 21 Nov 2023 05:47:25 GMT  
		Size: 1.4 MB (1386281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:753ad2913e083c1b5cb5b06853944934450629b0451d408743ddffc1f4c0a843`  
		Last Modified: Tue, 21 Nov 2023 05:47:24 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:standalone` - linux; arm variant v7

```console
$ docker pull adminer@sha256:6faef276799d02bdd9abf0ba022b692fd46f8144584adcfa771a76d225131045
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.8 MB (87796870 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9bb280f29bbaaa440662c6cbd26fabd7313fb299195b0ff2ca0cc22cff61f1ab`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Tue, 21 Nov 2023 03:57:54 GMT
ADD file:ed8d88d0476fad37879d872d61d05a8cffff35609566f080f78bb882d1bae26b in / 
# Tue, 21 Nov 2023 03:57:54 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 06:58:56 GMT
STOPSIGNAL SIGINT
# Tue, 21 Nov 2023 06:59:20 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 06:59:21 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 21 Nov 2023 06:59:21 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 21 Nov 2023 06:59:21 GMT
WORKDIR /var/www/html
# Tue, 21 Nov 2023 06:59:21 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 21 Nov 2023 06:59:21 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 21 Nov 2023 06:59:21 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 21 Nov 2023 06:59:22 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 21 Nov 2023 06:59:37 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Nov 2023 06:59:37 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 21 Nov 2023 06:59:37 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 21 Nov 2023 06:59:37 GMT
USER adminer
# Tue, 21 Nov 2023 06:59:37 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Tue, 21 Nov 2023 06:59:37 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:1dac19092a737e476f9b096fe28463512ae21c4f596dd2f8b84d62530416dffe`  
		Last Modified: Tue, 21 Nov 2023 04:02:11 GMT  
		Size: 50.2 MB (50215653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2f8153e5d67bc5a0049a12eb2430f50747238b7d4023cacdfc5dad9cdbd244a`  
		Last Modified: Tue, 21 Nov 2023 07:00:24 GMT  
		Size: 36.2 MB (36190640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ea62b864a160dff0b693d9397a8b84a1bc65e8e381b223294a8ac5ac8c68b8a`  
		Last Modified: Tue, 21 Nov 2023 07:00:15 GMT  
		Size: 393.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e2dd6fa8973e47e4cce58445b7207793f22b2371aa58678dc17d4172eac0b32`  
		Last Modified: Tue, 21 Nov 2023 07:00:15 GMT  
		Size: 1.9 KB (1871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4d33015217bf866b0d2c44cd29bf71617469b2e87e38eb15795aa3a293c83fa`  
		Last Modified: Tue, 21 Nov 2023 07:00:16 GMT  
		Size: 1.5 KB (1478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24ee8e39b9683ef6aa34033169655e5585db29d9557c0e1eb9aa117e1c771047`  
		Last Modified: Tue, 21 Nov 2023 07:00:16 GMT  
		Size: 1.4 MB (1386341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c14859802a2676aa6a511bbd06ce80a759e38e94927cd4d4b60dd202568ef5b`  
		Last Modified: Tue, 21 Nov 2023 07:00:15 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:standalone` - linux; arm64 variant v8

```console
$ docker pull adminer@sha256:e5fda74f5900f3c7ef8f74bda0392b45089f33f56374326bb331d8db26eb8b41
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.3 MB (94346130 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ccf82dd602ee08aa22718c108fcbcedbebb819a09c86b9f0fe8f2c1737bd08a7`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:13 GMT
ADD file:614987b9855939825ad2383e7bacbf14ea208d74906982bba3a67126702c8371 in / 
# Tue, 21 Nov 2023 06:27:13 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 10:22:26 GMT
STOPSIGNAL SIGINT
# Tue, 21 Nov 2023 10:22:43 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 10:22:44 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 21 Nov 2023 10:22:44 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 21 Nov 2023 10:22:44 GMT
WORKDIR /var/www/html
# Tue, 21 Nov 2023 10:22:44 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 21 Nov 2023 10:22:44 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 21 Nov 2023 10:22:45 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 21 Nov 2023 10:22:45 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 21 Nov 2023 10:22:54 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Nov 2023 10:22:54 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 21 Nov 2023 10:22:54 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 21 Nov 2023 10:22:54 GMT
USER adminer
# Tue, 21 Nov 2023 10:22:55 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Tue, 21 Nov 2023 10:22:55 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:bbf382c14c7b19b81c612f639e09e6a7b04eccd4481d0abac48b8ace9faae3b3`  
		Last Modified: Tue, 21 Nov 2023 06:30:47 GMT  
		Size: 53.7 MB (53707872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aa045892ab5d3693eb19355bad15725aa10139ceb2bfc2cb6141778f671e8e4`  
		Last Modified: Tue, 21 Nov 2023 10:23:29 GMT  
		Size: 39.2 MB (39247701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d77bfaecae2cacef431f4d68d17c26be0ab2300b5dfee893959aaae0c6427677`  
		Last Modified: Tue, 21 Nov 2023 10:23:21 GMT  
		Size: 386.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1364c7eb4b90daedaca80aff830c09309115f174a295c35ba7885c60557fa1e`  
		Last Modified: Tue, 21 Nov 2023 10:23:21 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:080b929d6ed912f11ed340726920967a938d3632641f4f86e15a30fc7b255888`  
		Last Modified: Tue, 21 Nov 2023 10:23:21 GMT  
		Size: 1.5 KB (1477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:633cfed53ab70b9e08d21a78973fc2a318d49c9cc54f3100604c9b91dd533c82`  
		Last Modified: Tue, 21 Nov 2023 10:23:22 GMT  
		Size: 1.4 MB (1386322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc610b080dd3b327bfe4b6ca8da59bc3a5555a295aff6c4f18d172f070b4e1ab`  
		Last Modified: Tue, 21 Nov 2023 10:23:21 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:standalone` - linux; 386

```console
$ docker pull adminer@sha256:173f2532a535a7780bffa43d6385797ba5335ab89832cb016cbb54cb0ab60fb2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.0 MB (96998974 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85b8488ee11e55b40364ca362184cc13095a7b83f1c1e65e524862cc27000db2`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Tue, 21 Nov 2023 04:40:03 GMT
ADD file:54170328827ccc52692c964f0c45a65ed6efdf39897f2c226672fdf526f3c412 in / 
# Tue, 21 Nov 2023 04:40:04 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 15:41:51 GMT
STOPSIGNAL SIGINT
# Tue, 21 Nov 2023 15:42:20 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 15:42:21 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 21 Nov 2023 15:42:22 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 21 Nov 2023 15:42:22 GMT
WORKDIR /var/www/html
# Tue, 21 Nov 2023 15:42:22 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 21 Nov 2023 15:42:22 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 21 Nov 2023 15:42:22 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 21 Nov 2023 15:42:22 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 21 Nov 2023 15:42:37 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Nov 2023 15:42:37 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 21 Nov 2023 15:42:37 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 21 Nov 2023 15:42:37 GMT
USER adminer
# Tue, 21 Nov 2023 15:42:37 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Tue, 21 Nov 2023 15:42:37 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:e33c1468a29e45636d4d9529b663048f7e8aa83ff428eb0681253bd4200e23ec`  
		Last Modified: Tue, 21 Nov 2023 04:44:57 GMT  
		Size: 56.0 MB (56046301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8137e600c481ac4ed29cae88512a113a2eadcc1d26e72628216670ef4f61ba30`  
		Last Modified: Tue, 21 Nov 2023 15:43:16 GMT  
		Size: 39.6 MB (39562172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e42a8870a081f3a4ab284980034bebec6585740c88e4c40ae98b2e1fa9955f5`  
		Last Modified: Tue, 21 Nov 2023 15:43:05 GMT  
		Size: 392.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48c728479be5016dacc84b6c0c244f327eff896df6a326af2826d6ad4c5387b6`  
		Last Modified: Tue, 21 Nov 2023 15:43:05 GMT  
		Size: 1.9 KB (1870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1000dcb7b3ee07a4d8a46142cda4b99b13051577e48599f89d62c8fd8c7e61a8`  
		Last Modified: Tue, 21 Nov 2023 15:43:05 GMT  
		Size: 1.5 KB (1482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d8473e68cd9a1e0940ff9bb80857e7d32bfde252766cc39fc1c3566222b0c1c`  
		Last Modified: Tue, 21 Nov 2023 15:43:06 GMT  
		Size: 1.4 MB (1386265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d7609e79a7e8443050102286e60b2022e9f3447043db395cabb7e2ad151b1e0`  
		Last Modified: Tue, 21 Nov 2023 15:43:05 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:standalone` - linux; mips64le

```console
$ docker pull adminer@sha256:84b1c19875f37b42946db21b87c80b8f8d9d9c7392eff0a7a065cf6d5fe769b2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.6 MB (92634921 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6454361a51d8f0d5781cd1854359c6b0812cc29466f516dd6386754b3583699`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Tue, 21 Nov 2023 04:10:25 GMT
ADD file:dbfc3d226166089c4db0c154fdcea8049b8758c6812f1c397dec1444985e8557 in / 
# Tue, 21 Nov 2023 04:10:31 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 12:14:44 GMT
STOPSIGNAL SIGINT
# Tue, 21 Nov 2023 12:16:43 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 12:16:50 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 21 Nov 2023 12:16:57 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 21 Nov 2023 12:17:00 GMT
WORKDIR /var/www/html
# Tue, 21 Nov 2023 12:17:04 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 21 Nov 2023 12:17:07 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 21 Nov 2023 12:17:10 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 21 Nov 2023 12:17:14 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 21 Nov 2023 12:18:08 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Nov 2023 12:18:11 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 21 Nov 2023 12:18:14 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 21 Nov 2023 12:18:17 GMT
USER adminer
# Tue, 21 Nov 2023 12:18:21 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Tue, 21 Nov 2023 12:18:24 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:ca31218601e95f4aafae0dcadda7600aeb04db374e1e829d5c123f8033ba3472`  
		Last Modified: Tue, 21 Nov 2023 04:21:21 GMT  
		Size: 53.3 MB (53289162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d172a1ce4463b8a1bb14b88d9f7c98a7f06f260dfc2849e77f3d41be6d17db9`  
		Last Modified: Tue, 21 Nov 2023 12:21:00 GMT  
		Size: 38.0 MB (37954467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbd3b039fbc0efa77466cfb045c80c120d45355cf2db0dd6533eeb1cee6296e1`  
		Last Modified: Tue, 21 Nov 2023 12:20:33 GMT  
		Size: 394.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bac97c667ed055993103f32b019a430a853a94eef6bf75086fda9949a9fd1d8`  
		Last Modified: Tue, 21 Nov 2023 12:20:34 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66eec20186701717a98146a63c5c8f88304d44243fe6f6505edf4d1135672446`  
		Last Modified: Tue, 21 Nov 2023 12:20:34 GMT  
		Size: 1.5 KB (1483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a56ddb348b2b13a6cac73829460bdcce2971790b6be59ac9da70b739453488b8`  
		Last Modified: Tue, 21 Nov 2023 12:20:34 GMT  
		Size: 1.4 MB (1387192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f922348b25af66b56cdd7a4863a9a120057afa01489fc9058cf7e975b198d05`  
		Last Modified: Tue, 21 Nov 2023 12:20:34 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:standalone` - linux; ppc64le

```console
$ docker pull adminer@sha256:3b96a3711e0e719557e514cb8870567e67ab545a7fe18b4feeca4e0e4c85d678
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.3 MB (101265448 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0c151160d019f74dfe13959cf16722a5172a0023a5f747201c90b752e001545`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Tue, 21 Nov 2023 04:24:26 GMT
ADD file:c21c2b6cb3f9bdf6cc3641e9ebf810a461174480c6cd1c25515cf9fce4aa2143 in / 
# Tue, 21 Nov 2023 04:24:30 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 06:49:59 GMT
STOPSIGNAL SIGINT
# Tue, 21 Nov 2023 06:50:40 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 06:50:42 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 21 Nov 2023 06:50:44 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 21 Nov 2023 06:50:44 GMT
WORKDIR /var/www/html
# Tue, 21 Nov 2023 06:50:44 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 21 Nov 2023 06:50:44 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 21 Nov 2023 06:50:45 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 21 Nov 2023 06:50:45 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 21 Nov 2023 06:51:03 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Nov 2023 06:51:03 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 21 Nov 2023 06:51:03 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 21 Nov 2023 06:51:03 GMT
USER adminer
# Tue, 21 Nov 2023 06:51:04 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Tue, 21 Nov 2023 06:51:04 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:23ebe74b854f8f6e2671f4c8cc147a6925fb7d929ce5898f7ca2af9781bf7d38`  
		Last Modified: Tue, 21 Nov 2023 04:29:21 GMT  
		Size: 58.9 MB (58929678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa255108512a37e57b2fdf827a0fdb4e3783a0649fb80ecdd431d4921dd6761c`  
		Last Modified: Tue, 21 Nov 2023 06:51:51 GMT  
		Size: 40.9 MB (40945122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5862ce535fc870ad9665c04e9816effde44c5f4469bc852265ba0bfe11ad7001`  
		Last Modified: Tue, 21 Nov 2023 06:51:41 GMT  
		Size: 391.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7204feb32d0a6fe6dd0348f7a8c2845b90b631ba893c08c48a724057c8a5e3d1`  
		Last Modified: Tue, 21 Nov 2023 06:51:41 GMT  
		Size: 1.9 KB (1879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb06eb196e5a191ad6e9d6d43052c2fd0f833100bf197c73f3f9c8df967003d1`  
		Last Modified: Tue, 21 Nov 2023 06:51:41 GMT  
		Size: 1.5 KB (1482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76df205e8013dede04db80018bebbabea233e0186671f2fd251fa440acde39ef`  
		Last Modified: Tue, 21 Nov 2023 06:51:41 GMT  
		Size: 1.4 MB (1386403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7099dfc32b7ad37a3cfe50e8aad19c609d5e9daf0535dd5cd0f853de87d0de8f`  
		Last Modified: Tue, 21 Nov 2023 06:51:41 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:standalone` - linux; s390x

```console
$ docker pull adminer@sha256:0832c83b0a0b564f962bc8f2f82974852bda2c876629b26a32e31e5b99e8fbc0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.7 MB (93709271 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72ed9e5473cf095c9f6c3263d8ff775ee9a240aa6597b921ebd51ec24f8978c1`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Tue, 21 Nov 2023 05:04:52 GMT
ADD file:b0a8fd50925b3555a0c10177e65551cae288917f9bad8fb4728ec83cc0765afe in / 
# Tue, 21 Nov 2023 05:05:01 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 06:04:07 GMT
STOPSIGNAL SIGINT
# Tue, 21 Nov 2023 06:04:29 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 06:04:35 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 21 Nov 2023 06:04:35 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 21 Nov 2023 06:04:36 GMT
WORKDIR /var/www/html
# Tue, 21 Nov 2023 06:04:36 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 21 Nov 2023 06:04:36 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 21 Nov 2023 06:04:36 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 21 Nov 2023 06:04:36 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 21 Nov 2023 06:04:45 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Nov 2023 06:04:46 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 21 Nov 2023 06:04:46 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 21 Nov 2023 06:04:46 GMT
USER adminer
# Tue, 21 Nov 2023 06:04:46 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Tue, 21 Nov 2023 06:04:47 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:9488c1539560318cb45b39150f91e365b928c0a246788663f5c72d185864bd3e`  
		Last Modified: Tue, 21 Nov 2023 05:10:34 GMT  
		Size: 53.3 MB (53296396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09efec12dc42685e3fe1693d18bc42d61971044de30a99ee3f044d942e93a470`  
		Last Modified: Tue, 21 Nov 2023 06:05:38 GMT  
		Size: 39.0 MB (39022251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d211af034ddf5d1e81df73b8d237d1c15d165b5443c533eedbeecc5659d4d4b`  
		Last Modified: Tue, 21 Nov 2023 06:05:31 GMT  
		Size: 393.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd2e9fc8bb5d1ec8686111ad3e20155b1ac539fc01b742c2318311374c9c3d29`  
		Last Modified: Tue, 21 Nov 2023 06:05:31 GMT  
		Size: 1.9 KB (1877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2acddcee94070eff9faaeaa170066fa650714281ae6b3094fc1d49c010f3902`  
		Last Modified: Tue, 21 Nov 2023 06:05:31 GMT  
		Size: 1.5 KB (1480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21ffbd0e004b4f2f9f75bdc6731ed7d644c91ee50221377d2ff00e82aa1f99b9`  
		Last Modified: Tue, 21 Nov 2023 06:05:31 GMT  
		Size: 1.4 MB (1386383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44baab47b2128777f4b94d45e4a91e7bd440dcb23e61b28ec31c8ac469b3cf40`  
		Last Modified: Tue, 21 Nov 2023 06:05:31 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
