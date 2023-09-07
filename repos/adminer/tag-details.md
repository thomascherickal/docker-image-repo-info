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
$ docker pull adminer@sha256:a607d96fbf114fefcdd34729b84a6cd379dedb3ead294c56f0f318f9981fb52a
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
$ docker pull adminer@sha256:5463cc7e5a3e4ad51aa0e98c419d04646fd9b3e14a1d960ab8b420b9ce9ecc80
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.9 MB (95937329 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1bb4da606dc1a8721442935ae417a1ff7d27b9eea6ef228797780679d81ba0b6`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Thu, 07 Sep 2023 00:21:01 GMT
ADD file:144dff349a666134b5e98a9f1c6650fd9d6e4a88a6f98857f26eb84989360b91 in / 
# Thu, 07 Sep 2023 00:21:02 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 03:10:23 GMT
STOPSIGNAL SIGINT
# Thu, 07 Sep 2023 03:10:44 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 03:10:45 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Thu, 07 Sep 2023 03:10:46 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 07 Sep 2023 03:10:46 GMT
WORKDIR /var/www/html
# Thu, 07 Sep 2023 03:10:46 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 07 Sep 2023 03:10:46 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 07 Sep 2023 03:10:46 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 07 Sep 2023 03:10:46 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 07 Sep 2023 03:10:58 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 07 Sep 2023 03:10:58 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 07 Sep 2023 03:10:58 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 07 Sep 2023 03:10:58 GMT
USER adminer
# Thu, 07 Sep 2023 03:10:58 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Thu, 07 Sep 2023 03:10:58 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:5dea071bb9782209397443f024a630052ab7583e365894d414f1e39cd0f65025`  
		Last Modified: Thu, 07 Sep 2023 00:25:41 GMT  
		Size: 55.1 MB (55056245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d84864d5d25a2386de4d3f48de320a52febc28bb28cb742aba6d777c4128696`  
		Last Modified: Thu, 07 Sep 2023 03:11:37 GMT  
		Size: 39.5 MB (39491426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:792bf43687eb38330b06a085a88b6c0505837ae192ac0fe027f7a07215f853a6`  
		Last Modified: Thu, 07 Sep 2023 03:11:29 GMT  
		Size: 395.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37ef5d260982b8b88f34270bbe7314228f686ac4bbbea7e647ab96feaf464e71`  
		Last Modified: Thu, 07 Sep 2023 03:11:29 GMT  
		Size: 1.9 KB (1879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81b9b963ca6d8427a310df0283abe6c6ef185569bb470cf8a0525da60989ecb6`  
		Last Modified: Thu, 07 Sep 2023 03:11:29 GMT  
		Size: 1.5 KB (1480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e57581023c92f337603ebe93de3ebca9a7eeb11706fdccc3f1b359714e0b65a6`  
		Last Modified: Thu, 07 Sep 2023 03:11:30 GMT  
		Size: 1.4 MB (1385412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e97ed40bb1db1cf97113d360f1b14422117cf4154eba611c2d2849d66958ecaa`  
		Last Modified: Thu, 07 Sep 2023 03:11:29 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4` - linux; arm variant v5

```console
$ docker pull adminer@sha256:dfd42b21fcc7d95faa4380a9bf051771e3bb79badd52e1005a8cbe551c64b6b4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.2 MB (91195063 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd44c48956465a566c168988d7201c27647c33ae7344305a32cd56f85cd46734`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Thu, 07 Sep 2023 00:48:38 GMT
ADD file:bad04cab9856def18134a0c7925a5f43816c14da597964b6d5567abc3ef6a8b9 in / 
# Thu, 07 Sep 2023 00:48:39 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 05:57:06 GMT
STOPSIGNAL SIGINT
# Thu, 07 Sep 2023 05:57:39 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 05:57:40 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Thu, 07 Sep 2023 05:57:41 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 07 Sep 2023 05:57:41 GMT
WORKDIR /var/www/html
# Thu, 07 Sep 2023 05:57:41 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 07 Sep 2023 05:57:41 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 07 Sep 2023 05:57:41 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 07 Sep 2023 05:57:41 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 07 Sep 2023 05:57:57 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 07 Sep 2023 05:57:57 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 07 Sep 2023 05:57:57 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 07 Sep 2023 05:57:57 GMT
USER adminer
# Thu, 07 Sep 2023 05:57:57 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Thu, 07 Sep 2023 05:57:57 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:c77da54c1e584356232e8207afbbe30938a9c2dda2ebc314c1d66e34c74245cc`  
		Last Modified: Thu, 07 Sep 2023 00:51:56 GMT  
		Size: 52.6 MB (52557684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f9ecd2f984b7ccbad8542193859188aa41052ff9a7f1b62ad82ac8bd8a4dc94`  
		Last Modified: Thu, 07 Sep 2023 05:58:40 GMT  
		Size: 37.2 MB (37247813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74f16b90817746d2df9ca8097b34f1a2a58ddea40f9d13b7661801e9d0cabeb6`  
		Last Modified: Thu, 07 Sep 2023 05:58:32 GMT  
		Size: 392.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2db198a220919fae8fc5093acd186481fdccff4b56654baf5ad81f5b16179f41`  
		Last Modified: Thu, 07 Sep 2023 05:58:31 GMT  
		Size: 1.9 KB (1869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bb71f0a31aaaedd68c31d3bd627d15c9a80f1fc8c77d787ae08509cea144944`  
		Last Modified: Thu, 07 Sep 2023 05:58:31 GMT  
		Size: 1.5 KB (1481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7345eee73a7d870b5e002cbc1ab741e76326b7bcedc039de45d03075a08f8bb5`  
		Last Modified: Thu, 07 Sep 2023 05:58:32 GMT  
		Size: 1.4 MB (1385331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d24fe8d24625441b6f9992c49257519dcd2a6962d677d2c96d6de6f440f16d9a`  
		Last Modified: Thu, 07 Sep 2023 05:58:31 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4` - linux; arm variant v7

```console
$ docker pull adminer@sha256:dde88e85f022908e040ce9f5627e989fca6cf4f796fb912e216bc91e85b80e9f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.8 MB (87795922 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1de3886b83d0afcea5f67dd340efd76d0ff0d7cc5d4d765d7ac24bdce5ac766`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Thu, 07 Sep 2023 00:57:59 GMT
ADD file:931564fb3c8ea78b763a6b98f2739bb7c6a38484122c560a87c7166b7d45c5e6 in / 
# Thu, 07 Sep 2023 00:58:00 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 01:50:52 GMT
STOPSIGNAL SIGINT
# Thu, 07 Sep 2023 01:51:32 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 01:51:33 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Thu, 07 Sep 2023 01:51:34 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 07 Sep 2023 01:51:34 GMT
WORKDIR /var/www/html
# Thu, 07 Sep 2023 01:51:34 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 07 Sep 2023 01:51:34 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 07 Sep 2023 01:51:34 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 07 Sep 2023 01:51:34 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 07 Sep 2023 01:51:48 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 07 Sep 2023 01:51:48 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 07 Sep 2023 01:51:48 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 07 Sep 2023 01:51:48 GMT
USER adminer
# Thu, 07 Sep 2023 01:51:48 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Thu, 07 Sep 2023 01:51:48 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:5826e0d927336e7231f9d05ec48f075045fb51f9b3f16f1e20972f2a3634d102`  
		Last Modified: Thu, 07 Sep 2023 01:02:50 GMT  
		Size: 50.2 MB (50219233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64126d7f6d5bc4ca6d42b71dc00598c67b9f6f17d6919fcce1f03a613722e16d`  
		Last Modified: Thu, 07 Sep 2023 01:52:33 GMT  
		Size: 36.2 MB (36187001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fd3d57a54c1b1fa49ef5fdece23637a20b7f8e985a804fc2c5135f097a549bb`  
		Last Modified: Thu, 07 Sep 2023 01:52:25 GMT  
		Size: 393.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2440750817c8e724091323e3903329ccc274561f1f1e61c49d9da560960899bb`  
		Last Modified: Thu, 07 Sep 2023 01:52:25 GMT  
		Size: 1.9 KB (1869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c56be7ee3fb4f5d4eec7601e51e91b41bf76a5ead2b87c1026930214ba51c2b8`  
		Last Modified: Thu, 07 Sep 2023 01:52:25 GMT  
		Size: 1.5 KB (1481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22e56804b3ad37bd9f7ff556ddf336fe3b2ed8503cb32b0dfee800e4c76d9451`  
		Last Modified: Thu, 07 Sep 2023 01:52:25 GMT  
		Size: 1.4 MB (1385452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:288264a2552805e7baa2b8233fa1aad54720bdba711d9147660fe31f59cc2f32`  
		Last Modified: Thu, 07 Sep 2023 01:52:25 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4` - linux; arm64 variant v8

```console
$ docker pull adminer@sha256:3b35134d84f9bb500b4ea3b9e5998209f9e587ef94982ee30e6357ae9f30d7c8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.3 MB (94338646 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6f05a6588020fe9fe371405a1735a4614daa30b4e299bd24afa4d2a017d0fa2`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Thu, 07 Sep 2023 00:39:45 GMT
ADD file:6bc001e951ef1280f566a92e65fcff57aefb8a280aa3510b7cd4b4e0a54c5cff in / 
# Thu, 07 Sep 2023 00:39:46 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 02:22:22 GMT
STOPSIGNAL SIGINT
# Thu, 07 Sep 2023 02:22:41 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 02:22:42 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Thu, 07 Sep 2023 02:22:42 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 07 Sep 2023 02:22:43 GMT
WORKDIR /var/www/html
# Thu, 07 Sep 2023 02:22:43 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 07 Sep 2023 02:22:43 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 07 Sep 2023 02:22:43 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 07 Sep 2023 02:22:43 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 07 Sep 2023 02:22:53 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 07 Sep 2023 02:22:53 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 07 Sep 2023 02:22:54 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 07 Sep 2023 02:22:54 GMT
USER adminer
# Thu, 07 Sep 2023 02:22:54 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Thu, 07 Sep 2023 02:22:54 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:61c16b7975697b00760ff9536c09eed29b6a76923d4d98be38e9cdc749506417`  
		Last Modified: Thu, 07 Sep 2023 00:43:21 GMT  
		Size: 53.7 MB (53704716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81f75bf1a78b692b687a603db539e512b761e91500113ab03d603be6cd108610`  
		Last Modified: Thu, 07 Sep 2023 02:23:31 GMT  
		Size: 39.2 MB (39244334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f3afc31326ca8d485c99b99322b549a89dd0db30062feaba0986df541301b45`  
		Last Modified: Thu, 07 Sep 2023 02:23:23 GMT  
		Size: 385.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c635f2e362703c71ad0c137ad3994b892ba8f342bd446e64f80d66d9c7c6965`  
		Last Modified: Thu, 07 Sep 2023 02:23:23 GMT  
		Size: 1.9 KB (1880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed650e87b8c0a626a5474dfdb12657fbf231ce26d8aef7302216b8b36e6c89f3`  
		Last Modified: Thu, 07 Sep 2023 02:23:24 GMT  
		Size: 1.5 KB (1481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e277a4a1ba7b301b2528764da6494b52a7e34668a0758bb6a9d5d0cb9ba10806`  
		Last Modified: Thu, 07 Sep 2023 02:23:24 GMT  
		Size: 1.4 MB (1385360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eea59163ae0d170091fc6d9eca39c3f6b9a6adaabf7b2a4cf5ecdd03cf72409c`  
		Last Modified: Thu, 07 Sep 2023 02:23:24 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4` - linux; 386

```console
$ docker pull adminer@sha256:664fc6a11ece4d60a18492c17eeb4ffffb3d6fe19d3c4f4c4c3cab52b83f3ec6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.0 MB (96988434 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d7ecc3592e5ee3a2de07572724acd9167630fa736fd16b373959b3f5e2297736`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Tue, 15 Aug 2023 23:39:11 GMT
ADD file:efc88a19b31e68ca41f555bcc51338b0f135cbbd72b90637d8c73969d53addd2 in / 
# Tue, 15 Aug 2023 23:39:12 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 00:23:36 GMT
STOPSIGNAL SIGINT
# Wed, 16 Aug 2023 00:24:03 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 00:24:04 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 16 Aug 2023 00:24:05 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 16 Aug 2023 00:24:05 GMT
WORKDIR /var/www/html
# Wed, 16 Aug 2023 00:24:05 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 16 Aug 2023 00:24:05 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 16 Aug 2023 00:24:05 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 16 Aug 2023 00:24:05 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 16 Aug 2023 00:24:19 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 16 Aug 2023 00:24:19 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 16 Aug 2023 00:24:19 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 16 Aug 2023 00:24:19 GMT
USER adminer
# Wed, 16 Aug 2023 00:24:19 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 16 Aug 2023 00:24:19 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:822e033fa7b169545d5890de01438a9dd87774ff938ff440e823a3ec3f73996d`  
		Last Modified: Tue, 15 Aug 2023 23:43:47 GMT  
		Size: 56.0 MB (56040520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7644269f7e699d335219a554e561f3817b7816e99351232b3646176246991895`  
		Last Modified: Wed, 16 Aug 2023 00:25:00 GMT  
		Size: 39.6 MB (39558428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d96338ff936c667ce1c89a75f7fd111e722685d882b1f36e7b26dcb33007029`  
		Last Modified: Wed, 16 Aug 2023 00:24:50 GMT  
		Size: 389.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5339c86a7bc7031718f83f0a9af19ad028c2fa751748057f9d97d9c94c5075f6`  
		Last Modified: Wed, 16 Aug 2023 00:24:50 GMT  
		Size: 1.9 KB (1868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cbd1ad590a03bbc3ee08a1c944135c7bf81b103067417f79cdb1f8d271b4472`  
		Last Modified: Wed, 16 Aug 2023 00:24:50 GMT  
		Size: 1.5 KB (1480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:225fb2c801a3d35820604ab9c5d6c19a65e18fca4c76dd468e7015b6cb7d5d6c`  
		Last Modified: Wed, 16 Aug 2023 00:24:50 GMT  
		Size: 1.4 MB (1385258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:367f82cd1a3d30bffd1420e0c950c92f859f903ad0b0711848862db96f363ff7`  
		Last Modified: Wed, 16 Aug 2023 00:24:50 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4` - linux; mips64le

```console
$ docker pull adminer@sha256:9cc962f9ae71f2c5b15623bc438ebb6d9a340e0ba8d278d98c031c39e1b5e407
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.6 MB (92612452 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c340fe4c80d84cb71a7948c0d3da3ae567112f144fa0d27c1320899c29a61f0`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Thu, 07 Sep 2023 01:09:47 GMT
ADD file:fdd438b39f1dce564715691d2a092378f02bc722e29cb80216efcbaf71cff0b8 in / 
# Thu, 07 Sep 2023 01:09:53 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 03:08:04 GMT
STOPSIGNAL SIGINT
# Thu, 07 Sep 2023 03:10:03 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 03:10:09 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Thu, 07 Sep 2023 03:10:16 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 07 Sep 2023 03:10:19 GMT
WORKDIR /var/www/html
# Thu, 07 Sep 2023 03:10:23 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 07 Sep 2023 03:10:26 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 07 Sep 2023 03:10:30 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 07 Sep 2023 03:10:33 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 07 Sep 2023 03:11:27 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 07 Sep 2023 03:11:30 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 07 Sep 2023 03:11:33 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 07 Sep 2023 03:11:36 GMT
USER adminer
# Thu, 07 Sep 2023 03:11:40 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Thu, 07 Sep 2023 03:11:43 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:0d1f1f4ccb1e0da4313c3ebcd521e7fa8073526c6f64ca7214ed31ae9bd0788e`  
		Last Modified: Thu, 07 Sep 2023 01:21:00 GMT  
		Size: 53.3 MB (53271469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b724451ca3bae07bf7da51b1c949189dc86f1e494be2830616fbe3cf4c7a447`  
		Last Modified: Thu, 07 Sep 2023 03:14:20 GMT  
		Size: 38.0 MB (37950499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:915c5f7e479b8d1cb1baf57fd9f07e06b962433d3a40fc832491c6f6614522bb`  
		Last Modified: Thu, 07 Sep 2023 03:13:55 GMT  
		Size: 394.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffcee722bb0f36a2975167c5ddf08d0da2cb56e72317f5f3e9d5cfbc3d4a4716`  
		Last Modified: Thu, 07 Sep 2023 03:13:54 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fc9ff6a8f7fb04dd6c3d6df59d01f1c9c7c34ad3cbe41553ecdff949bd20c1e`  
		Last Modified: Thu, 07 Sep 2023 03:13:54 GMT  
		Size: 1.5 KB (1482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cb2cbc2bc303d453e8e91cca3d170ccb3b27fd2bd03b89a3924e679e78c26e4`  
		Last Modified: Thu, 07 Sep 2023 03:13:55 GMT  
		Size: 1.4 MB (1386382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efe356c9d62e82baa2ebf75971c57e6fadf0e138988c966f6767875ff8843182`  
		Last Modified: Thu, 07 Sep 2023 03:13:54 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4` - linux; ppc64le

```console
$ docker pull adminer@sha256:af35710d0480902e87252a3b766b10d0f75285c0d22bafce974f049ed8128552
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.3 MB (101262505 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ec6c6c445d603cdb55b8e2df3d7ca3ab043dee3a4535b6dd28cd47284c99eed`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Thu, 07 Sep 2023 00:17:47 GMT
ADD file:da42a2ef7aa1ce7e6df281b469ac67db062d14c59066a6dfd7ac5cc91d7a3b8c in / 
# Thu, 07 Sep 2023 00:17:50 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 09:04:15 GMT
STOPSIGNAL SIGINT
# Thu, 07 Sep 2023 09:07:04 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 09:07:10 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Thu, 07 Sep 2023 09:07:13 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 07 Sep 2023 09:07:14 GMT
WORKDIR /var/www/html
# Thu, 07 Sep 2023 09:07:14 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 07 Sep 2023 09:07:15 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 07 Sep 2023 09:07:15 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 07 Sep 2023 09:07:16 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 07 Sep 2023 09:08:33 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 07 Sep 2023 09:08:33 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 07 Sep 2023 09:08:35 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 07 Sep 2023 09:08:36 GMT
USER adminer
# Thu, 07 Sep 2023 09:08:38 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Thu, 07 Sep 2023 09:08:39 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:fb3cfd509d4c62da47ee9c7eee6545472d58ceaab6fcd454a82d188766dd0c45`  
		Last Modified: Thu, 07 Sep 2023 00:23:55 GMT  
		Size: 58.9 MB (58928091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bffc3bba24bd4cd45431ae9c166638ec8595b5ecab4200290f8c176a1212b7c`  
		Last Modified: Thu, 07 Sep 2023 09:11:25 GMT  
		Size: 40.9 MB (40944217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d37dbbfa36efc1b986a9571f61c675f6dd3304c8b0f8ea6ce287be3e977d1976`  
		Last Modified: Thu, 07 Sep 2023 09:11:12 GMT  
		Size: 398.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:040ad87be7d0fd1ec4f721e5fd3acd35286b3f5dd90a2f50595443791d2c5f78`  
		Last Modified: Thu, 07 Sep 2023 09:11:12 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fde911bb7830da7a8226144a744f977069a6a35fc88a5f98301891261503ecf`  
		Last Modified: Thu, 07 Sep 2023 09:11:12 GMT  
		Size: 1.5 KB (1476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1ce36781194ed33448f80f0902704489627f8098ddd838fc8a41ca597ccbfab`  
		Last Modified: Thu, 07 Sep 2023 09:11:13 GMT  
		Size: 1.4 MB (1385951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d01192f86adad3c4b51a184a68865d082250b44614aa375d150dda8f5f36b927`  
		Last Modified: Thu, 07 Sep 2023 09:11:12 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4` - linux; s390x

```console
$ docker pull adminer@sha256:b3028b06f7c78024603ab547558cf83d4fe518c6bfd10a107ee923081d45c3a6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.7 MB (93700732 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40878d5b42fdc65d89e9d563be958aad831592c92455633ce54a025dc6bac4eb`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Thu, 07 Sep 2023 00:44:03 GMT
ADD file:a0582e191d0265b98e5d46c64ba9b4c46445cfa821c6e41d32db343b0e2a6fec in / 
# Thu, 07 Sep 2023 00:44:12 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 01:26:26 GMT
STOPSIGNAL SIGINT
# Thu, 07 Sep 2023 01:27:02 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 01:27:07 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Thu, 07 Sep 2023 01:27:08 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 07 Sep 2023 01:27:08 GMT
WORKDIR /var/www/html
# Thu, 07 Sep 2023 01:27:09 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 07 Sep 2023 01:27:09 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 07 Sep 2023 01:27:09 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 07 Sep 2023 01:27:09 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 07 Sep 2023 01:27:22 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 07 Sep 2023 01:27:22 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 07 Sep 2023 01:27:23 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 07 Sep 2023 01:27:24 GMT
USER adminer
# Thu, 07 Sep 2023 01:27:24 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Thu, 07 Sep 2023 01:27:24 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:6dd2d41f67a6666210e1a34694b8765e945a44014b53252ec0e1b50491e08d69`  
		Last Modified: Thu, 07 Sep 2023 00:49:54 GMT  
		Size: 53.3 MB (53290217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe4a876b44eaaf1ba3c702ea08a6af25e23abb30b7fcbef9b957a4c34ec5ad73`  
		Last Modified: Thu, 07 Sep 2023 01:28:21 GMT  
		Size: 39.0 MB (39020691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:529f8a0ebc99b919f45c296bfffe1d9aa35136c91542e626681a898a1e1dabb2`  
		Last Modified: Thu, 07 Sep 2023 01:28:14 GMT  
		Size: 393.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:322f53d9402212f75016bdbb862615c373419e902c2b0a0994373659dc9a40dc`  
		Last Modified: Thu, 07 Sep 2023 01:28:14 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c552fc3addf63a6a3c52100ad6a25209610153282a2977fc8234b019e7bfa4b8`  
		Last Modified: Thu, 07 Sep 2023 01:28:14 GMT  
		Size: 1.5 KB (1480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a4df5368a1108e415af1adad06e9925df044775278212b278f40db0c9e828b6`  
		Last Modified: Thu, 07 Sep 2023 01:28:15 GMT  
		Size: 1.4 MB (1385578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d8fa422b756819743a45bc63685472b1df2c01002596e8beb4231c6f1235f34`  
		Last Modified: Thu, 07 Sep 2023 01:28:14 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `adminer:4-fastcgi`

```console
$ docker pull adminer@sha256:3240fafaf56f18ec0d10835a26868e6022d637d213088732290b80fd613edcfa
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
$ docker pull adminer@sha256:15659f7db1e32df8ee184ace61ba9c86663fe995dcc68b5bee681676cd65c86d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.9 MB (95940089 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:88b4d4658217a7fbd5718733b47cfdfcd835cba81366d47a5edc8516a640bd9f`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Thu, 07 Sep 2023 00:21:01 GMT
ADD file:144dff349a666134b5e98a9f1c6650fd9d6e4a88a6f98857f26eb84989360b91 in / 
# Thu, 07 Sep 2023 00:21:02 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 03:10:23 GMT
STOPSIGNAL SIGINT
# Thu, 07 Sep 2023 03:10:44 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 03:10:45 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Thu, 07 Sep 2023 03:11:05 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Thu, 07 Sep 2023 03:11:05 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 07 Sep 2023 03:11:05 GMT
WORKDIR /var/www/html
# Thu, 07 Sep 2023 03:11:06 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 07 Sep 2023 03:11:06 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 07 Sep 2023 03:11:06 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 07 Sep 2023 03:11:06 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 07 Sep 2023 03:11:16 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 07 Sep 2023 03:11:16 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 07 Sep 2023 03:11:16 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 07 Sep 2023 03:11:17 GMT
USER adminer
# Thu, 07 Sep 2023 03:11:17 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:5dea071bb9782209397443f024a630052ab7583e365894d414f1e39cd0f65025`  
		Last Modified: Thu, 07 Sep 2023 00:25:41 GMT  
		Size: 55.1 MB (55056245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d84864d5d25a2386de4d3f48de320a52febc28bb28cb742aba6d777c4128696`  
		Last Modified: Thu, 07 Sep 2023 03:11:37 GMT  
		Size: 39.5 MB (39491426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:792bf43687eb38330b06a085a88b6c0505837ae192ac0fe027f7a07215f853a6`  
		Last Modified: Thu, 07 Sep 2023 03:11:29 GMT  
		Size: 395.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e01de01b95b38bf91fd08d70ff82b982b8dca2110bf77448cea418e95e126d9a`  
		Last Modified: Thu, 07 Sep 2023 03:11:54 GMT  
		Size: 2.7 KB (2712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15e0eed8de828090b43d0bbdb0fe4d095f18b39bea0ba03bdde09742311c98e2`  
		Last Modified: Thu, 07 Sep 2023 03:11:54 GMT  
		Size: 1.9 KB (1880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:871d9ee2bd875b8e07cda014c321142ca148c41385ad50db557708d53aeed910`  
		Last Modified: Thu, 07 Sep 2023 03:11:54 GMT  
		Size: 1.5 KB (1480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ea47c50e3a334983865aa3a1ac8269133885d8dc06e6bd3adfbdb41cb6b08c6`  
		Last Modified: Thu, 07 Sep 2023 03:11:55 GMT  
		Size: 1.4 MB (1385463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9fee1469c7254200561d4b1b94f32fc0485731de2477b06e6df7013098f6c7b`  
		Last Modified: Thu, 07 Sep 2023 03:11:54 GMT  
		Size: 488.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-fastcgi` - linux; arm variant v5

```console
$ docker pull adminer@sha256:68a8a35328fd756b490e1ee7bfe37451f377151d253bf2a13b8132dec21e0ce0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.2 MB (91197773 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ac4abb044959ec9100e2123e544a8bb1c39a3e7299cb2b54f30345e746092ce`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Thu, 07 Sep 2023 00:48:38 GMT
ADD file:bad04cab9856def18134a0c7925a5f43816c14da597964b6d5567abc3ef6a8b9 in / 
# Thu, 07 Sep 2023 00:48:39 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 05:57:06 GMT
STOPSIGNAL SIGINT
# Thu, 07 Sep 2023 05:57:39 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 05:57:40 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Thu, 07 Sep 2023 05:58:04 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Thu, 07 Sep 2023 05:58:05 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 07 Sep 2023 05:58:05 GMT
WORKDIR /var/www/html
# Thu, 07 Sep 2023 05:58:05 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 07 Sep 2023 05:58:05 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 07 Sep 2023 05:58:05 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 07 Sep 2023 05:58:05 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 07 Sep 2023 05:58:18 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 07 Sep 2023 05:58:18 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 07 Sep 2023 05:58:18 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 07 Sep 2023 05:58:18 GMT
USER adminer
# Thu, 07 Sep 2023 05:58:18 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:c77da54c1e584356232e8207afbbe30938a9c2dda2ebc314c1d66e34c74245cc`  
		Last Modified: Thu, 07 Sep 2023 00:51:56 GMT  
		Size: 52.6 MB (52557684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f9ecd2f984b7ccbad8542193859188aa41052ff9a7f1b62ad82ac8bd8a4dc94`  
		Last Modified: Thu, 07 Sep 2023 05:58:40 GMT  
		Size: 37.2 MB (37247813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74f16b90817746d2df9ca8097b34f1a2a58ddea40f9d13b7661801e9d0cabeb6`  
		Last Modified: Thu, 07 Sep 2023 05:58:32 GMT  
		Size: 392.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19291db959f5743b3fc9e761a855018f488f61c2f70012d7a14fb1319d0d61f3`  
		Last Modified: Thu, 07 Sep 2023 05:58:57 GMT  
		Size: 2.7 KB (2713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04fa7bdce9b8e241d877c81cd956b30e00826a78a5513355c03646ecab5c6a09`  
		Last Modified: Thu, 07 Sep 2023 05:58:57 GMT  
		Size: 1.9 KB (1869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0867e050c3c0c3917ee2ff18cf6b6becb88fe6053803081900c3382331506c8`  
		Last Modified: Thu, 07 Sep 2023 05:58:57 GMT  
		Size: 1.5 KB (1480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c35adb51769011f110acbf0514bab08249bcf812b1da24327bed43b4eb11ba2`  
		Last Modified: Thu, 07 Sep 2023 05:58:58 GMT  
		Size: 1.4 MB (1385331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:254cd97ad98c8e7fb70fe19de389cf9b2863df4d23f3885d54fd68242293a387`  
		Last Modified: Thu, 07 Sep 2023 05:58:57 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-fastcgi` - linux; arm variant v7

```console
$ docker pull adminer@sha256:a0d499c047e84848247c5a877bd3c4064625f4a64495f89e1ad95093fce1ac3f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.8 MB (87798646 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33f2770b6fe2af3a75e07d84e1b363bad6515ceb1b6972d4d9902323283d0694`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Thu, 07 Sep 2023 00:57:59 GMT
ADD file:931564fb3c8ea78b763a6b98f2739bb7c6a38484122c560a87c7166b7d45c5e6 in / 
# Thu, 07 Sep 2023 00:58:00 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 01:50:52 GMT
STOPSIGNAL SIGINT
# Thu, 07 Sep 2023 01:51:32 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 01:51:33 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Thu, 07 Sep 2023 01:52:01 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Thu, 07 Sep 2023 01:52:02 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 07 Sep 2023 01:52:02 GMT
WORKDIR /var/www/html
# Thu, 07 Sep 2023 01:52:02 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 07 Sep 2023 01:52:02 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 07 Sep 2023 01:52:02 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 07 Sep 2023 01:52:02 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 07 Sep 2023 01:52:14 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 07 Sep 2023 01:52:14 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 07 Sep 2023 01:52:14 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 07 Sep 2023 01:52:14 GMT
USER adminer
# Thu, 07 Sep 2023 01:52:15 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:5826e0d927336e7231f9d05ec48f075045fb51f9b3f16f1e20972f2a3634d102`  
		Last Modified: Thu, 07 Sep 2023 01:02:50 GMT  
		Size: 50.2 MB (50219233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64126d7f6d5bc4ca6d42b71dc00598c67b9f6f17d6919fcce1f03a613722e16d`  
		Last Modified: Thu, 07 Sep 2023 01:52:33 GMT  
		Size: 36.2 MB (36187001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fd3d57a54c1b1fa49ef5fdece23637a20b7f8e985a804fc2c5135f097a549bb`  
		Last Modified: Thu, 07 Sep 2023 01:52:25 GMT  
		Size: 393.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21903f65656bc64fb0c6609085b2d6702f7968442e7354cf234741fc68c2f5f4`  
		Last Modified: Thu, 07 Sep 2023 01:52:51 GMT  
		Size: 2.7 KB (2711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0113ab9766972272a3d4c016308b4e1e22c504b634d6941e6b9c059cad5b3d45`  
		Last Modified: Thu, 07 Sep 2023 01:52:51 GMT  
		Size: 1.9 KB (1871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d992cf32eddb4dbb575f70c5b565ee0fb23d47953ed8292e06ac9555ddeeb123`  
		Last Modified: Thu, 07 Sep 2023 01:52:52 GMT  
		Size: 1.5 KB (1480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47b5e7c51aefa173a76e0fa25e50964e84f858eba6e8225bb1f29ee18d6062b0`  
		Last Modified: Thu, 07 Sep 2023 01:52:52 GMT  
		Size: 1.4 MB (1385466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c65e533099f9039fa0e0df43fda417b7954478ea6aa401dedf1ee822938b5b7e`  
		Last Modified: Thu, 07 Sep 2023 01:52:51 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-fastcgi` - linux; arm64 variant v8

```console
$ docker pull adminer@sha256:a38ecc5faf0a8576b1bdd76c2f602a86daa9b6cd71b16633fb7ce005ef32bd8d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.3 MB (94341386 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a500c1c0d44c969c688bca9ba88bcb562155d2c6dace06dbe71086fdbdb6fb82`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Thu, 07 Sep 2023 00:39:45 GMT
ADD file:6bc001e951ef1280f566a92e65fcff57aefb8a280aa3510b7cd4b4e0a54c5cff in / 
# Thu, 07 Sep 2023 00:39:46 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 02:22:22 GMT
STOPSIGNAL SIGINT
# Thu, 07 Sep 2023 02:22:41 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 02:22:42 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Thu, 07 Sep 2023 02:23:02 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Thu, 07 Sep 2023 02:23:03 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 07 Sep 2023 02:23:03 GMT
WORKDIR /var/www/html
# Thu, 07 Sep 2023 02:23:03 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 07 Sep 2023 02:23:03 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 07 Sep 2023 02:23:03 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 07 Sep 2023 02:23:03 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 07 Sep 2023 02:23:13 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 07 Sep 2023 02:23:13 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 07 Sep 2023 02:23:13 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 07 Sep 2023 02:23:13 GMT
USER adminer
# Thu, 07 Sep 2023 02:23:13 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:61c16b7975697b00760ff9536c09eed29b6a76923d4d98be38e9cdc749506417`  
		Last Modified: Thu, 07 Sep 2023 00:43:21 GMT  
		Size: 53.7 MB (53704716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81f75bf1a78b692b687a603db539e512b761e91500113ab03d603be6cd108610`  
		Last Modified: Thu, 07 Sep 2023 02:23:31 GMT  
		Size: 39.2 MB (39244334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f3afc31326ca8d485c99b99322b549a89dd0db30062feaba0986df541301b45`  
		Last Modified: Thu, 07 Sep 2023 02:23:23 GMT  
		Size: 385.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efb65c5d18143c713fb41d912e5eb0419de652c480d7db9d798886f092df48a7`  
		Last Modified: Thu, 07 Sep 2023 02:23:47 GMT  
		Size: 2.7 KB (2709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f811d6324927c972ba66211edfdf8f3c83f50e55193712a29387b3787210591d`  
		Last Modified: Thu, 07 Sep 2023 02:23:47 GMT  
		Size: 1.9 KB (1883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e0bd6ef968ad02351f0b7c15001f9016c5be9aabf3c89e45d5d1347c663b6fa`  
		Last Modified: Thu, 07 Sep 2023 02:23:47 GMT  
		Size: 1.5 KB (1477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b21fc274312e94dc7ca9579a44d64426c71ea39388a81328c0a00f3bfc7a0ada`  
		Last Modified: Thu, 07 Sep 2023 02:23:47 GMT  
		Size: 1.4 MB (1385391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0360824626289cffd506daf3a7e018ae732cad6b53e2e81b212e909ebc93627e`  
		Last Modified: Thu, 07 Sep 2023 02:23:47 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-fastcgi` - linux; 386

```console
$ docker pull adminer@sha256:e069ad6357b6e472b22c167d7e6644c1829900d73629b9ebfc05888ce049bfe2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.0 MB (96991740 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb5eea91a8ed56f36a9c6995824b55264ceb8328a4941035def4679918353dd1`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Thu, 07 Sep 2023 00:39:12 GMT
ADD file:bf79261700cf8412eb759b5cfc3a37825dad004e81e864a5e2fd8e3bbbaf217e in / 
# Thu, 07 Sep 2023 00:39:12 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 12:09:39 GMT
STOPSIGNAL SIGINT
# Thu, 07 Sep 2023 12:10:10 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 12:10:11 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Thu, 07 Sep 2023 12:10:38 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Thu, 07 Sep 2023 12:10:38 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 07 Sep 2023 12:10:38 GMT
WORKDIR /var/www/html
# Thu, 07 Sep 2023 12:10:39 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 07 Sep 2023 12:10:39 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 07 Sep 2023 12:10:39 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 07 Sep 2023 12:10:39 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 07 Sep 2023 12:10:52 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 07 Sep 2023 12:10:52 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 07 Sep 2023 12:10:53 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 07 Sep 2023 12:10:53 GMT
USER adminer
# Thu, 07 Sep 2023 12:10:53 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:3a8f1bd5e39092e1e02a2c349cd4130e74a705d3d2b5f2f789f856632f3a25f1`  
		Last Modified: Thu, 07 Sep 2023 00:44:11 GMT  
		Size: 56.0 MB (56040528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef650b8daf931017283220f9b80654004afffa052c63a056e04426e98e922c89`  
		Last Modified: Thu, 07 Sep 2023 12:11:19 GMT  
		Size: 39.6 MB (39558962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1aadcb9575090ce09730ba3ef7d97c83290dc26159d7c19578334814b97d385c`  
		Last Modified: Thu, 07 Sep 2023 12:11:07 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:206b2630ac8f6aa6eb9676d5d718f3b1ca67165cfd573cefdf1e251331ef29b5`  
		Last Modified: Thu, 07 Sep 2023 12:11:37 GMT  
		Size: 2.7 KB (2706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32eb027a1b6db47b5e7792470a858de1751693bfad00275098ec7ae5339cb2dd`  
		Last Modified: Thu, 07 Sep 2023 12:11:37 GMT  
		Size: 1.9 KB (1868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f225674f1c59970df0a8b235c9341a870da5e62367b0fc9e04f9da95e07aebc6`  
		Last Modified: Thu, 07 Sep 2023 12:11:37 GMT  
		Size: 1.5 KB (1476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4f193a9bed4495ca1aaf2880bc9a5c91a310d1481061d98b0e69fe8378c9cba`  
		Last Modified: Thu, 07 Sep 2023 12:11:37 GMT  
		Size: 1.4 MB (1385318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b39ea62233bf837ee84ca7d0138bb7266ae225c1c1bcf8ed5ab724a85ceace5b`  
		Last Modified: Thu, 07 Sep 2023 12:11:37 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-fastcgi` - linux; mips64le

```console
$ docker pull adminer@sha256:2c3b4d978627105affcd060a2a4602bb97f1fd90187edd5cb30b338b22584e15
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.6 MB (92615139 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c2be39d77614a37ab8c0c9448232e1be6fb18fca8a2696bdb76f7ba90b69578`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Thu, 07 Sep 2023 01:09:47 GMT
ADD file:fdd438b39f1dce564715691d2a092378f02bc722e29cb80216efcbaf71cff0b8 in / 
# Thu, 07 Sep 2023 01:09:53 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 03:08:04 GMT
STOPSIGNAL SIGINT
# Thu, 07 Sep 2023 03:10:03 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 03:10:09 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Thu, 07 Sep 2023 03:12:06 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Thu, 07 Sep 2023 03:12:13 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 07 Sep 2023 03:12:16 GMT
WORKDIR /var/www/html
# Thu, 07 Sep 2023 03:12:19 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 07 Sep 2023 03:12:22 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 07 Sep 2023 03:12:26 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 07 Sep 2023 03:12:29 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 07 Sep 2023 03:13:20 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 07 Sep 2023 03:13:23 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 07 Sep 2023 03:13:27 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 07 Sep 2023 03:13:30 GMT
USER adminer
# Thu, 07 Sep 2023 03:13:34 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:0d1f1f4ccb1e0da4313c3ebcd521e7fa8073526c6f64ca7214ed31ae9bd0788e`  
		Last Modified: Thu, 07 Sep 2023 01:21:00 GMT  
		Size: 53.3 MB (53271469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b724451ca3bae07bf7da51b1c949189dc86f1e494be2830616fbe3cf4c7a447`  
		Last Modified: Thu, 07 Sep 2023 03:14:20 GMT  
		Size: 38.0 MB (37950499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:915c5f7e479b8d1cb1baf57fd9f07e06b962433d3a40fc832491c6f6614522bb`  
		Last Modified: Thu, 07 Sep 2023 03:13:55 GMT  
		Size: 394.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c089a408ed63eef86310ec1d3db9d84aa46d7f541e3ec1e90a4798aa6545d436`  
		Last Modified: Thu, 07 Sep 2023 03:14:41 GMT  
		Size: 2.7 KB (2713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56bb790d23ceab0acafe02823b5726a9a99319fc3ce2e215cbbc11d2e5b57a60`  
		Last Modified: Thu, 07 Sep 2023 03:14:41 GMT  
		Size: 1.7 KB (1725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c5b3c385bb7fe02cc10cefc1cc9bfd8a7c41d4d908b07bef77f7f7c0308086a`  
		Last Modified: Thu, 07 Sep 2023 03:14:41 GMT  
		Size: 1.5 KB (1479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ae8742bfc11fac37d1a8257111b0cdde75cd0c7d628fe1c99a1767583510d4f`  
		Last Modified: Thu, 07 Sep 2023 03:14:42 GMT  
		Size: 1.4 MB (1386368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd25dbfd1a8ef46f40a314361de018304317b3f157bf58c376b23d42d53e9f5a`  
		Last Modified: Thu, 07 Sep 2023 03:14:41 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-fastcgi` - linux; ppc64le

```console
$ docker pull adminer@sha256:b7224d5a014ff9f27bb1a4b1aff7ed321765e5f8ec175d34613ccdef6e2da361
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.3 MB (101265147 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70f1927913fd3d1b839c87d619e0d41128e9ac696c2e77895368025a38cdb9c0`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Thu, 07 Sep 2023 00:17:47 GMT
ADD file:da42a2ef7aa1ce7e6df281b469ac67db062d14c59066a6dfd7ac5cc91d7a3b8c in / 
# Thu, 07 Sep 2023 00:17:50 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 09:04:15 GMT
STOPSIGNAL SIGINT
# Thu, 07 Sep 2023 09:07:04 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 09:07:10 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Thu, 07 Sep 2023 09:08:56 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Thu, 07 Sep 2023 09:09:03 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 07 Sep 2023 09:09:06 GMT
WORKDIR /var/www/html
# Thu, 07 Sep 2023 09:09:06 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 07 Sep 2023 09:09:08 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 07 Sep 2023 09:09:09 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 07 Sep 2023 09:09:10 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 07 Sep 2023 09:10:21 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 07 Sep 2023 09:10:25 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 07 Sep 2023 09:10:33 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 07 Sep 2023 09:10:40 GMT
USER adminer
# Thu, 07 Sep 2023 09:10:52 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:fb3cfd509d4c62da47ee9c7eee6545472d58ceaab6fcd454a82d188766dd0c45`  
		Last Modified: Thu, 07 Sep 2023 00:23:55 GMT  
		Size: 58.9 MB (58928091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bffc3bba24bd4cd45431ae9c166638ec8595b5ecab4200290f8c176a1212b7c`  
		Last Modified: Thu, 07 Sep 2023 09:11:25 GMT  
		Size: 40.9 MB (40944217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d37dbbfa36efc1b986a9571f61c675f6dd3304c8b0f8ea6ce287be3e977d1976`  
		Last Modified: Thu, 07 Sep 2023 09:11:12 GMT  
		Size: 398.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6805ebe3dfb3654d46f5fc9a8cd6a74c2a86ade728959b1dfa0739f99c1b5428`  
		Last Modified: Thu, 07 Sep 2023 09:11:45 GMT  
		Size: 2.7 KB (2714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70c512e9728df1edeb0e0315c69e85528520cf302979f8f6ade2fca0b27185b5`  
		Last Modified: Thu, 07 Sep 2023 09:11:45 GMT  
		Size: 1.9 KB (1876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11e2e6a603583abf7085bdbf1f879974415c61c29c08962f4b96fb4fe3ce981d`  
		Last Modified: Thu, 07 Sep 2023 09:11:45 GMT  
		Size: 1.5 KB (1478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d971487f8cbfeaa9c06033dcafc7e63fa3556563916948e905fc7c62b4126c8b`  
		Last Modified: Thu, 07 Sep 2023 09:11:46 GMT  
		Size: 1.4 MB (1385882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbc9d316bb2a490069e9c690d1f2e1e73e0765b2cfa7fab34108868e6756e9a3`  
		Last Modified: Thu, 07 Sep 2023 09:11:45 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-fastcgi` - linux; s390x

```console
$ docker pull adminer@sha256:de471294d28d5750d41244ba8d44db2cb1aaab848922985f660b02eabbd197dc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.7 MB (93703439 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cde1549e5993997b294699895499c6549c361bd95ebd374a3c85442fd76eb165`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Thu, 07 Sep 2023 00:44:03 GMT
ADD file:a0582e191d0265b98e5d46c64ba9b4c46445cfa821c6e41d32db343b0e2a6fec in / 
# Thu, 07 Sep 2023 00:44:12 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 01:26:26 GMT
STOPSIGNAL SIGINT
# Thu, 07 Sep 2023 01:27:02 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 01:27:07 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Thu, 07 Sep 2023 01:27:36 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Thu, 07 Sep 2023 01:27:37 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 07 Sep 2023 01:27:38 GMT
WORKDIR /var/www/html
# Thu, 07 Sep 2023 01:27:38 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 07 Sep 2023 01:27:38 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 07 Sep 2023 01:27:38 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 07 Sep 2023 01:27:39 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 07 Sep 2023 01:27:53 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 07 Sep 2023 01:27:54 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 07 Sep 2023 01:27:54 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 07 Sep 2023 01:27:55 GMT
USER adminer
# Thu, 07 Sep 2023 01:27:55 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:6dd2d41f67a6666210e1a34694b8765e945a44014b53252ec0e1b50491e08d69`  
		Last Modified: Thu, 07 Sep 2023 00:49:54 GMT  
		Size: 53.3 MB (53290217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe4a876b44eaaf1ba3c702ea08a6af25e23abb30b7fcbef9b957a4c34ec5ad73`  
		Last Modified: Thu, 07 Sep 2023 01:28:21 GMT  
		Size: 39.0 MB (39020691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:529f8a0ebc99b919f45c296bfffe1d9aa35136c91542e626681a898a1e1dabb2`  
		Last Modified: Thu, 07 Sep 2023 01:28:14 GMT  
		Size: 393.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e241b68ed72809f13265cadec141405091d29c51cc7031a53fb1ac63e98370e4`  
		Last Modified: Thu, 07 Sep 2023 01:28:34 GMT  
		Size: 2.7 KB (2714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c554ebc3fa08021199bd77796a742b7ec9a23e27c9f301efd186c67355e26ea3`  
		Last Modified: Thu, 07 Sep 2023 01:28:34 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6ddeb9921e2ece9eabbc65206020cfc9fb9c53ebb491a85b96d5eb7ed308c6e`  
		Last Modified: Thu, 07 Sep 2023 01:28:34 GMT  
		Size: 1.5 KB (1481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5c07f366229478ef4b2de990c4de70ab31aa0982284cc7b192581b9c8e765eb`  
		Last Modified: Thu, 07 Sep 2023 01:28:34 GMT  
		Size: 1.4 MB (1385571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6878b99b931b3ddc6e0ae8ba87b925151a30fbb1ade42882571d878a53316bb0`  
		Last Modified: Thu, 07 Sep 2023 01:28:34 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `adminer:4-standalone`

```console
$ docker pull adminer@sha256:9e5d16eb26f60483abe2bf9408a577f19ee42fab1db78295397f5913f3970b67
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
$ docker pull adminer@sha256:5463cc7e5a3e4ad51aa0e98c419d04646fd9b3e14a1d960ab8b420b9ce9ecc80
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.9 MB (95937329 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1bb4da606dc1a8721442935ae417a1ff7d27b9eea6ef228797780679d81ba0b6`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Thu, 07 Sep 2023 00:21:01 GMT
ADD file:144dff349a666134b5e98a9f1c6650fd9d6e4a88a6f98857f26eb84989360b91 in / 
# Thu, 07 Sep 2023 00:21:02 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 03:10:23 GMT
STOPSIGNAL SIGINT
# Thu, 07 Sep 2023 03:10:44 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 03:10:45 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Thu, 07 Sep 2023 03:10:46 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 07 Sep 2023 03:10:46 GMT
WORKDIR /var/www/html
# Thu, 07 Sep 2023 03:10:46 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 07 Sep 2023 03:10:46 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 07 Sep 2023 03:10:46 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 07 Sep 2023 03:10:46 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 07 Sep 2023 03:10:58 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 07 Sep 2023 03:10:58 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 07 Sep 2023 03:10:58 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 07 Sep 2023 03:10:58 GMT
USER adminer
# Thu, 07 Sep 2023 03:10:58 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Thu, 07 Sep 2023 03:10:58 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:5dea071bb9782209397443f024a630052ab7583e365894d414f1e39cd0f65025`  
		Last Modified: Thu, 07 Sep 2023 00:25:41 GMT  
		Size: 55.1 MB (55056245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d84864d5d25a2386de4d3f48de320a52febc28bb28cb742aba6d777c4128696`  
		Last Modified: Thu, 07 Sep 2023 03:11:37 GMT  
		Size: 39.5 MB (39491426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:792bf43687eb38330b06a085a88b6c0505837ae192ac0fe027f7a07215f853a6`  
		Last Modified: Thu, 07 Sep 2023 03:11:29 GMT  
		Size: 395.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37ef5d260982b8b88f34270bbe7314228f686ac4bbbea7e647ab96feaf464e71`  
		Last Modified: Thu, 07 Sep 2023 03:11:29 GMT  
		Size: 1.9 KB (1879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81b9b963ca6d8427a310df0283abe6c6ef185569bb470cf8a0525da60989ecb6`  
		Last Modified: Thu, 07 Sep 2023 03:11:29 GMT  
		Size: 1.5 KB (1480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e57581023c92f337603ebe93de3ebca9a7eeb11706fdccc3f1b359714e0b65a6`  
		Last Modified: Thu, 07 Sep 2023 03:11:30 GMT  
		Size: 1.4 MB (1385412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e97ed40bb1db1cf97113d360f1b14422117cf4154eba611c2d2849d66958ecaa`  
		Last Modified: Thu, 07 Sep 2023 03:11:29 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-standalone` - linux; arm variant v5

```console
$ docker pull adminer@sha256:dfd42b21fcc7d95faa4380a9bf051771e3bb79badd52e1005a8cbe551c64b6b4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.2 MB (91195063 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd44c48956465a566c168988d7201c27647c33ae7344305a32cd56f85cd46734`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Thu, 07 Sep 2023 00:48:38 GMT
ADD file:bad04cab9856def18134a0c7925a5f43816c14da597964b6d5567abc3ef6a8b9 in / 
# Thu, 07 Sep 2023 00:48:39 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 05:57:06 GMT
STOPSIGNAL SIGINT
# Thu, 07 Sep 2023 05:57:39 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 05:57:40 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Thu, 07 Sep 2023 05:57:41 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 07 Sep 2023 05:57:41 GMT
WORKDIR /var/www/html
# Thu, 07 Sep 2023 05:57:41 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 07 Sep 2023 05:57:41 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 07 Sep 2023 05:57:41 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 07 Sep 2023 05:57:41 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 07 Sep 2023 05:57:57 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 07 Sep 2023 05:57:57 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 07 Sep 2023 05:57:57 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 07 Sep 2023 05:57:57 GMT
USER adminer
# Thu, 07 Sep 2023 05:57:57 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Thu, 07 Sep 2023 05:57:57 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:c77da54c1e584356232e8207afbbe30938a9c2dda2ebc314c1d66e34c74245cc`  
		Last Modified: Thu, 07 Sep 2023 00:51:56 GMT  
		Size: 52.6 MB (52557684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f9ecd2f984b7ccbad8542193859188aa41052ff9a7f1b62ad82ac8bd8a4dc94`  
		Last Modified: Thu, 07 Sep 2023 05:58:40 GMT  
		Size: 37.2 MB (37247813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74f16b90817746d2df9ca8097b34f1a2a58ddea40f9d13b7661801e9d0cabeb6`  
		Last Modified: Thu, 07 Sep 2023 05:58:32 GMT  
		Size: 392.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2db198a220919fae8fc5093acd186481fdccff4b56654baf5ad81f5b16179f41`  
		Last Modified: Thu, 07 Sep 2023 05:58:31 GMT  
		Size: 1.9 KB (1869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bb71f0a31aaaedd68c31d3bd627d15c9a80f1fc8c77d787ae08509cea144944`  
		Last Modified: Thu, 07 Sep 2023 05:58:31 GMT  
		Size: 1.5 KB (1481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7345eee73a7d870b5e002cbc1ab741e76326b7bcedc039de45d03075a08f8bb5`  
		Last Modified: Thu, 07 Sep 2023 05:58:32 GMT  
		Size: 1.4 MB (1385331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d24fe8d24625441b6f9992c49257519dcd2a6962d677d2c96d6de6f440f16d9a`  
		Last Modified: Thu, 07 Sep 2023 05:58:31 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-standalone` - linux; arm variant v7

```console
$ docker pull adminer@sha256:dde88e85f022908e040ce9f5627e989fca6cf4f796fb912e216bc91e85b80e9f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.8 MB (87795922 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1de3886b83d0afcea5f67dd340efd76d0ff0d7cc5d4d765d7ac24bdce5ac766`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Thu, 07 Sep 2023 00:57:59 GMT
ADD file:931564fb3c8ea78b763a6b98f2739bb7c6a38484122c560a87c7166b7d45c5e6 in / 
# Thu, 07 Sep 2023 00:58:00 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 01:50:52 GMT
STOPSIGNAL SIGINT
# Thu, 07 Sep 2023 01:51:32 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 01:51:33 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Thu, 07 Sep 2023 01:51:34 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 07 Sep 2023 01:51:34 GMT
WORKDIR /var/www/html
# Thu, 07 Sep 2023 01:51:34 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 07 Sep 2023 01:51:34 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 07 Sep 2023 01:51:34 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 07 Sep 2023 01:51:34 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 07 Sep 2023 01:51:48 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 07 Sep 2023 01:51:48 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 07 Sep 2023 01:51:48 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 07 Sep 2023 01:51:48 GMT
USER adminer
# Thu, 07 Sep 2023 01:51:48 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Thu, 07 Sep 2023 01:51:48 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:5826e0d927336e7231f9d05ec48f075045fb51f9b3f16f1e20972f2a3634d102`  
		Last Modified: Thu, 07 Sep 2023 01:02:50 GMT  
		Size: 50.2 MB (50219233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64126d7f6d5bc4ca6d42b71dc00598c67b9f6f17d6919fcce1f03a613722e16d`  
		Last Modified: Thu, 07 Sep 2023 01:52:33 GMT  
		Size: 36.2 MB (36187001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fd3d57a54c1b1fa49ef5fdece23637a20b7f8e985a804fc2c5135f097a549bb`  
		Last Modified: Thu, 07 Sep 2023 01:52:25 GMT  
		Size: 393.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2440750817c8e724091323e3903329ccc274561f1f1e61c49d9da560960899bb`  
		Last Modified: Thu, 07 Sep 2023 01:52:25 GMT  
		Size: 1.9 KB (1869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c56be7ee3fb4f5d4eec7601e51e91b41bf76a5ead2b87c1026930214ba51c2b8`  
		Last Modified: Thu, 07 Sep 2023 01:52:25 GMT  
		Size: 1.5 KB (1481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22e56804b3ad37bd9f7ff556ddf336fe3b2ed8503cb32b0dfee800e4c76d9451`  
		Last Modified: Thu, 07 Sep 2023 01:52:25 GMT  
		Size: 1.4 MB (1385452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:288264a2552805e7baa2b8233fa1aad54720bdba711d9147660fe31f59cc2f32`  
		Last Modified: Thu, 07 Sep 2023 01:52:25 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-standalone` - linux; arm64 variant v8

```console
$ docker pull adminer@sha256:3b35134d84f9bb500b4ea3b9e5998209f9e587ef94982ee30e6357ae9f30d7c8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.3 MB (94338646 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6f05a6588020fe9fe371405a1735a4614daa30b4e299bd24afa4d2a017d0fa2`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Thu, 07 Sep 2023 00:39:45 GMT
ADD file:6bc001e951ef1280f566a92e65fcff57aefb8a280aa3510b7cd4b4e0a54c5cff in / 
# Thu, 07 Sep 2023 00:39:46 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 02:22:22 GMT
STOPSIGNAL SIGINT
# Thu, 07 Sep 2023 02:22:41 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 02:22:42 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Thu, 07 Sep 2023 02:22:42 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 07 Sep 2023 02:22:43 GMT
WORKDIR /var/www/html
# Thu, 07 Sep 2023 02:22:43 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 07 Sep 2023 02:22:43 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 07 Sep 2023 02:22:43 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 07 Sep 2023 02:22:43 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 07 Sep 2023 02:22:53 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 07 Sep 2023 02:22:53 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 07 Sep 2023 02:22:54 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 07 Sep 2023 02:22:54 GMT
USER adminer
# Thu, 07 Sep 2023 02:22:54 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Thu, 07 Sep 2023 02:22:54 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:61c16b7975697b00760ff9536c09eed29b6a76923d4d98be38e9cdc749506417`  
		Last Modified: Thu, 07 Sep 2023 00:43:21 GMT  
		Size: 53.7 MB (53704716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81f75bf1a78b692b687a603db539e512b761e91500113ab03d603be6cd108610`  
		Last Modified: Thu, 07 Sep 2023 02:23:31 GMT  
		Size: 39.2 MB (39244334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f3afc31326ca8d485c99b99322b549a89dd0db30062feaba0986df541301b45`  
		Last Modified: Thu, 07 Sep 2023 02:23:23 GMT  
		Size: 385.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c635f2e362703c71ad0c137ad3994b892ba8f342bd446e64f80d66d9c7c6965`  
		Last Modified: Thu, 07 Sep 2023 02:23:23 GMT  
		Size: 1.9 KB (1880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed650e87b8c0a626a5474dfdb12657fbf231ce26d8aef7302216b8b36e6c89f3`  
		Last Modified: Thu, 07 Sep 2023 02:23:24 GMT  
		Size: 1.5 KB (1481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e277a4a1ba7b301b2528764da6494b52a7e34668a0758bb6a9d5d0cb9ba10806`  
		Last Modified: Thu, 07 Sep 2023 02:23:24 GMT  
		Size: 1.4 MB (1385360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eea59163ae0d170091fc6d9eca39c3f6b9a6adaabf7b2a4cf5ecdd03cf72409c`  
		Last Modified: Thu, 07 Sep 2023 02:23:24 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-standalone` - linux; 386

```console
$ docker pull adminer@sha256:71277e51e4144523793606f751c038e0d916c407170b76f6cfa658c0c68343d5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.0 MB (96989028 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a106263b0383ca702783152eabdd6eb8b1a95f18131c42c0d3e7d18b043e7766`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Thu, 07 Sep 2023 00:39:12 GMT
ADD file:bf79261700cf8412eb759b5cfc3a37825dad004e81e864a5e2fd8e3bbbaf217e in / 
# Thu, 07 Sep 2023 00:39:12 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 12:09:39 GMT
STOPSIGNAL SIGINT
# Thu, 07 Sep 2023 12:10:10 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 12:10:11 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Thu, 07 Sep 2023 12:10:12 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 07 Sep 2023 12:10:12 GMT
WORKDIR /var/www/html
# Thu, 07 Sep 2023 12:10:12 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 07 Sep 2023 12:10:12 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 07 Sep 2023 12:10:12 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 07 Sep 2023 12:10:13 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 07 Sep 2023 12:10:27 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 07 Sep 2023 12:10:27 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 07 Sep 2023 12:10:27 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 07 Sep 2023 12:10:27 GMT
USER adminer
# Thu, 07 Sep 2023 12:10:27 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Thu, 07 Sep 2023 12:10:28 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:3a8f1bd5e39092e1e02a2c349cd4130e74a705d3d2b5f2f789f856632f3a25f1`  
		Last Modified: Thu, 07 Sep 2023 00:44:11 GMT  
		Size: 56.0 MB (56040528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef650b8daf931017283220f9b80654004afffa052c63a056e04426e98e922c89`  
		Last Modified: Thu, 07 Sep 2023 12:11:19 GMT  
		Size: 39.6 MB (39558962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1aadcb9575090ce09730ba3ef7d97c83290dc26159d7c19578334814b97d385c`  
		Last Modified: Thu, 07 Sep 2023 12:11:07 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9f708d67412753311bfd807ee09e0c256ae0531c26a6c2d5075ed2aab302d86`  
		Last Modified: Thu, 07 Sep 2023 12:11:07 GMT  
		Size: 1.9 KB (1868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c66b98bb7e1695e588451617cdf75ddd0a944e24fac5d26f4e5dcae02a0d465`  
		Last Modified: Thu, 07 Sep 2023 12:11:07 GMT  
		Size: 1.5 KB (1477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a223a9d49f0399f82d2da1d359bdca68a494b10032f79ec5bf03c8bef97b901f`  
		Last Modified: Thu, 07 Sep 2023 12:11:08 GMT  
		Size: 1.4 MB (1385313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf4a0fda7c9aa7946db984687228316c0ed36e8dde882f6786834f088d6154b4`  
		Last Modified: Thu, 07 Sep 2023 12:11:07 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-standalone` - linux; mips64le

```console
$ docker pull adminer@sha256:9cc962f9ae71f2c5b15623bc438ebb6d9a340e0ba8d278d98c031c39e1b5e407
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.6 MB (92612452 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c340fe4c80d84cb71a7948c0d3da3ae567112f144fa0d27c1320899c29a61f0`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Thu, 07 Sep 2023 01:09:47 GMT
ADD file:fdd438b39f1dce564715691d2a092378f02bc722e29cb80216efcbaf71cff0b8 in / 
# Thu, 07 Sep 2023 01:09:53 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 03:08:04 GMT
STOPSIGNAL SIGINT
# Thu, 07 Sep 2023 03:10:03 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 03:10:09 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Thu, 07 Sep 2023 03:10:16 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 07 Sep 2023 03:10:19 GMT
WORKDIR /var/www/html
# Thu, 07 Sep 2023 03:10:23 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 07 Sep 2023 03:10:26 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 07 Sep 2023 03:10:30 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 07 Sep 2023 03:10:33 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 07 Sep 2023 03:11:27 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 07 Sep 2023 03:11:30 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 07 Sep 2023 03:11:33 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 07 Sep 2023 03:11:36 GMT
USER adminer
# Thu, 07 Sep 2023 03:11:40 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Thu, 07 Sep 2023 03:11:43 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:0d1f1f4ccb1e0da4313c3ebcd521e7fa8073526c6f64ca7214ed31ae9bd0788e`  
		Last Modified: Thu, 07 Sep 2023 01:21:00 GMT  
		Size: 53.3 MB (53271469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b724451ca3bae07bf7da51b1c949189dc86f1e494be2830616fbe3cf4c7a447`  
		Last Modified: Thu, 07 Sep 2023 03:14:20 GMT  
		Size: 38.0 MB (37950499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:915c5f7e479b8d1cb1baf57fd9f07e06b962433d3a40fc832491c6f6614522bb`  
		Last Modified: Thu, 07 Sep 2023 03:13:55 GMT  
		Size: 394.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffcee722bb0f36a2975167c5ddf08d0da2cb56e72317f5f3e9d5cfbc3d4a4716`  
		Last Modified: Thu, 07 Sep 2023 03:13:54 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fc9ff6a8f7fb04dd6c3d6df59d01f1c9c7c34ad3cbe41553ecdff949bd20c1e`  
		Last Modified: Thu, 07 Sep 2023 03:13:54 GMT  
		Size: 1.5 KB (1482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cb2cbc2bc303d453e8e91cca3d170ccb3b27fd2bd03b89a3924e679e78c26e4`  
		Last Modified: Thu, 07 Sep 2023 03:13:55 GMT  
		Size: 1.4 MB (1386382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efe356c9d62e82baa2ebf75971c57e6fadf0e138988c966f6767875ff8843182`  
		Last Modified: Thu, 07 Sep 2023 03:13:54 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-standalone` - linux; ppc64le

```console
$ docker pull adminer@sha256:af35710d0480902e87252a3b766b10d0f75285c0d22bafce974f049ed8128552
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.3 MB (101262505 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ec6c6c445d603cdb55b8e2df3d7ca3ab043dee3a4535b6dd28cd47284c99eed`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Thu, 07 Sep 2023 00:17:47 GMT
ADD file:da42a2ef7aa1ce7e6df281b469ac67db062d14c59066a6dfd7ac5cc91d7a3b8c in / 
# Thu, 07 Sep 2023 00:17:50 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 09:04:15 GMT
STOPSIGNAL SIGINT
# Thu, 07 Sep 2023 09:07:04 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 09:07:10 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Thu, 07 Sep 2023 09:07:13 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 07 Sep 2023 09:07:14 GMT
WORKDIR /var/www/html
# Thu, 07 Sep 2023 09:07:14 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 07 Sep 2023 09:07:15 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 07 Sep 2023 09:07:15 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 07 Sep 2023 09:07:16 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 07 Sep 2023 09:08:33 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 07 Sep 2023 09:08:33 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 07 Sep 2023 09:08:35 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 07 Sep 2023 09:08:36 GMT
USER adminer
# Thu, 07 Sep 2023 09:08:38 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Thu, 07 Sep 2023 09:08:39 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:fb3cfd509d4c62da47ee9c7eee6545472d58ceaab6fcd454a82d188766dd0c45`  
		Last Modified: Thu, 07 Sep 2023 00:23:55 GMT  
		Size: 58.9 MB (58928091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bffc3bba24bd4cd45431ae9c166638ec8595b5ecab4200290f8c176a1212b7c`  
		Last Modified: Thu, 07 Sep 2023 09:11:25 GMT  
		Size: 40.9 MB (40944217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d37dbbfa36efc1b986a9571f61c675f6dd3304c8b0f8ea6ce287be3e977d1976`  
		Last Modified: Thu, 07 Sep 2023 09:11:12 GMT  
		Size: 398.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:040ad87be7d0fd1ec4f721e5fd3acd35286b3f5dd90a2f50595443791d2c5f78`  
		Last Modified: Thu, 07 Sep 2023 09:11:12 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fde911bb7830da7a8226144a744f977069a6a35fc88a5f98301891261503ecf`  
		Last Modified: Thu, 07 Sep 2023 09:11:12 GMT  
		Size: 1.5 KB (1476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1ce36781194ed33448f80f0902704489627f8098ddd838fc8a41ca597ccbfab`  
		Last Modified: Thu, 07 Sep 2023 09:11:13 GMT  
		Size: 1.4 MB (1385951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d01192f86adad3c4b51a184a68865d082250b44614aa375d150dda8f5f36b927`  
		Last Modified: Thu, 07 Sep 2023 09:11:12 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-standalone` - linux; s390x

```console
$ docker pull adminer@sha256:b3028b06f7c78024603ab547558cf83d4fe518c6bfd10a107ee923081d45c3a6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.7 MB (93700732 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40878d5b42fdc65d89e9d563be958aad831592c92455633ce54a025dc6bac4eb`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Thu, 07 Sep 2023 00:44:03 GMT
ADD file:a0582e191d0265b98e5d46c64ba9b4c46445cfa821c6e41d32db343b0e2a6fec in / 
# Thu, 07 Sep 2023 00:44:12 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 01:26:26 GMT
STOPSIGNAL SIGINT
# Thu, 07 Sep 2023 01:27:02 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 01:27:07 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Thu, 07 Sep 2023 01:27:08 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 07 Sep 2023 01:27:08 GMT
WORKDIR /var/www/html
# Thu, 07 Sep 2023 01:27:09 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 07 Sep 2023 01:27:09 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 07 Sep 2023 01:27:09 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 07 Sep 2023 01:27:09 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 07 Sep 2023 01:27:22 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 07 Sep 2023 01:27:22 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 07 Sep 2023 01:27:23 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 07 Sep 2023 01:27:24 GMT
USER adminer
# Thu, 07 Sep 2023 01:27:24 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Thu, 07 Sep 2023 01:27:24 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:6dd2d41f67a6666210e1a34694b8765e945a44014b53252ec0e1b50491e08d69`  
		Last Modified: Thu, 07 Sep 2023 00:49:54 GMT  
		Size: 53.3 MB (53290217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe4a876b44eaaf1ba3c702ea08a6af25e23abb30b7fcbef9b957a4c34ec5ad73`  
		Last Modified: Thu, 07 Sep 2023 01:28:21 GMT  
		Size: 39.0 MB (39020691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:529f8a0ebc99b919f45c296bfffe1d9aa35136c91542e626681a898a1e1dabb2`  
		Last Modified: Thu, 07 Sep 2023 01:28:14 GMT  
		Size: 393.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:322f53d9402212f75016bdbb862615c373419e902c2b0a0994373659dc9a40dc`  
		Last Modified: Thu, 07 Sep 2023 01:28:14 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c552fc3addf63a6a3c52100ad6a25209610153282a2977fc8234b019e7bfa4b8`  
		Last Modified: Thu, 07 Sep 2023 01:28:14 GMT  
		Size: 1.5 KB (1480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a4df5368a1108e415af1adad06e9925df044775278212b278f40db0c9e828b6`  
		Last Modified: Thu, 07 Sep 2023 01:28:15 GMT  
		Size: 1.4 MB (1385578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d8fa422b756819743a45bc63685472b1df2c01002596e8beb4231c6f1235f34`  
		Last Modified: Thu, 07 Sep 2023 01:28:14 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `adminer:4.8.1`

```console
$ docker pull adminer@sha256:9e5d16eb26f60483abe2bf9408a577f19ee42fab1db78295397f5913f3970b67
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
$ docker pull adminer@sha256:5463cc7e5a3e4ad51aa0e98c419d04646fd9b3e14a1d960ab8b420b9ce9ecc80
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.9 MB (95937329 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1bb4da606dc1a8721442935ae417a1ff7d27b9eea6ef228797780679d81ba0b6`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Thu, 07 Sep 2023 00:21:01 GMT
ADD file:144dff349a666134b5e98a9f1c6650fd9d6e4a88a6f98857f26eb84989360b91 in / 
# Thu, 07 Sep 2023 00:21:02 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 03:10:23 GMT
STOPSIGNAL SIGINT
# Thu, 07 Sep 2023 03:10:44 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 03:10:45 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Thu, 07 Sep 2023 03:10:46 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 07 Sep 2023 03:10:46 GMT
WORKDIR /var/www/html
# Thu, 07 Sep 2023 03:10:46 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 07 Sep 2023 03:10:46 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 07 Sep 2023 03:10:46 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 07 Sep 2023 03:10:46 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 07 Sep 2023 03:10:58 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 07 Sep 2023 03:10:58 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 07 Sep 2023 03:10:58 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 07 Sep 2023 03:10:58 GMT
USER adminer
# Thu, 07 Sep 2023 03:10:58 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Thu, 07 Sep 2023 03:10:58 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:5dea071bb9782209397443f024a630052ab7583e365894d414f1e39cd0f65025`  
		Last Modified: Thu, 07 Sep 2023 00:25:41 GMT  
		Size: 55.1 MB (55056245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d84864d5d25a2386de4d3f48de320a52febc28bb28cb742aba6d777c4128696`  
		Last Modified: Thu, 07 Sep 2023 03:11:37 GMT  
		Size: 39.5 MB (39491426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:792bf43687eb38330b06a085a88b6c0505837ae192ac0fe027f7a07215f853a6`  
		Last Modified: Thu, 07 Sep 2023 03:11:29 GMT  
		Size: 395.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37ef5d260982b8b88f34270bbe7314228f686ac4bbbea7e647ab96feaf464e71`  
		Last Modified: Thu, 07 Sep 2023 03:11:29 GMT  
		Size: 1.9 KB (1879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81b9b963ca6d8427a310df0283abe6c6ef185569bb470cf8a0525da60989ecb6`  
		Last Modified: Thu, 07 Sep 2023 03:11:29 GMT  
		Size: 1.5 KB (1480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e57581023c92f337603ebe93de3ebca9a7eeb11706fdccc3f1b359714e0b65a6`  
		Last Modified: Thu, 07 Sep 2023 03:11:30 GMT  
		Size: 1.4 MB (1385412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e97ed40bb1db1cf97113d360f1b14422117cf4154eba611c2d2849d66958ecaa`  
		Last Modified: Thu, 07 Sep 2023 03:11:29 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1` - linux; arm variant v5

```console
$ docker pull adminer@sha256:dfd42b21fcc7d95faa4380a9bf051771e3bb79badd52e1005a8cbe551c64b6b4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.2 MB (91195063 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd44c48956465a566c168988d7201c27647c33ae7344305a32cd56f85cd46734`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Thu, 07 Sep 2023 00:48:38 GMT
ADD file:bad04cab9856def18134a0c7925a5f43816c14da597964b6d5567abc3ef6a8b9 in / 
# Thu, 07 Sep 2023 00:48:39 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 05:57:06 GMT
STOPSIGNAL SIGINT
# Thu, 07 Sep 2023 05:57:39 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 05:57:40 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Thu, 07 Sep 2023 05:57:41 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 07 Sep 2023 05:57:41 GMT
WORKDIR /var/www/html
# Thu, 07 Sep 2023 05:57:41 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 07 Sep 2023 05:57:41 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 07 Sep 2023 05:57:41 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 07 Sep 2023 05:57:41 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 07 Sep 2023 05:57:57 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 07 Sep 2023 05:57:57 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 07 Sep 2023 05:57:57 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 07 Sep 2023 05:57:57 GMT
USER adminer
# Thu, 07 Sep 2023 05:57:57 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Thu, 07 Sep 2023 05:57:57 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:c77da54c1e584356232e8207afbbe30938a9c2dda2ebc314c1d66e34c74245cc`  
		Last Modified: Thu, 07 Sep 2023 00:51:56 GMT  
		Size: 52.6 MB (52557684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f9ecd2f984b7ccbad8542193859188aa41052ff9a7f1b62ad82ac8bd8a4dc94`  
		Last Modified: Thu, 07 Sep 2023 05:58:40 GMT  
		Size: 37.2 MB (37247813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74f16b90817746d2df9ca8097b34f1a2a58ddea40f9d13b7661801e9d0cabeb6`  
		Last Modified: Thu, 07 Sep 2023 05:58:32 GMT  
		Size: 392.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2db198a220919fae8fc5093acd186481fdccff4b56654baf5ad81f5b16179f41`  
		Last Modified: Thu, 07 Sep 2023 05:58:31 GMT  
		Size: 1.9 KB (1869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bb71f0a31aaaedd68c31d3bd627d15c9a80f1fc8c77d787ae08509cea144944`  
		Last Modified: Thu, 07 Sep 2023 05:58:31 GMT  
		Size: 1.5 KB (1481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7345eee73a7d870b5e002cbc1ab741e76326b7bcedc039de45d03075a08f8bb5`  
		Last Modified: Thu, 07 Sep 2023 05:58:32 GMT  
		Size: 1.4 MB (1385331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d24fe8d24625441b6f9992c49257519dcd2a6962d677d2c96d6de6f440f16d9a`  
		Last Modified: Thu, 07 Sep 2023 05:58:31 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1` - linux; arm variant v7

```console
$ docker pull adminer@sha256:dde88e85f022908e040ce9f5627e989fca6cf4f796fb912e216bc91e85b80e9f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.8 MB (87795922 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1de3886b83d0afcea5f67dd340efd76d0ff0d7cc5d4d765d7ac24bdce5ac766`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Thu, 07 Sep 2023 00:57:59 GMT
ADD file:931564fb3c8ea78b763a6b98f2739bb7c6a38484122c560a87c7166b7d45c5e6 in / 
# Thu, 07 Sep 2023 00:58:00 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 01:50:52 GMT
STOPSIGNAL SIGINT
# Thu, 07 Sep 2023 01:51:32 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 01:51:33 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Thu, 07 Sep 2023 01:51:34 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 07 Sep 2023 01:51:34 GMT
WORKDIR /var/www/html
# Thu, 07 Sep 2023 01:51:34 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 07 Sep 2023 01:51:34 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 07 Sep 2023 01:51:34 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 07 Sep 2023 01:51:34 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 07 Sep 2023 01:51:48 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 07 Sep 2023 01:51:48 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 07 Sep 2023 01:51:48 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 07 Sep 2023 01:51:48 GMT
USER adminer
# Thu, 07 Sep 2023 01:51:48 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Thu, 07 Sep 2023 01:51:48 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:5826e0d927336e7231f9d05ec48f075045fb51f9b3f16f1e20972f2a3634d102`  
		Last Modified: Thu, 07 Sep 2023 01:02:50 GMT  
		Size: 50.2 MB (50219233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64126d7f6d5bc4ca6d42b71dc00598c67b9f6f17d6919fcce1f03a613722e16d`  
		Last Modified: Thu, 07 Sep 2023 01:52:33 GMT  
		Size: 36.2 MB (36187001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fd3d57a54c1b1fa49ef5fdece23637a20b7f8e985a804fc2c5135f097a549bb`  
		Last Modified: Thu, 07 Sep 2023 01:52:25 GMT  
		Size: 393.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2440750817c8e724091323e3903329ccc274561f1f1e61c49d9da560960899bb`  
		Last Modified: Thu, 07 Sep 2023 01:52:25 GMT  
		Size: 1.9 KB (1869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c56be7ee3fb4f5d4eec7601e51e91b41bf76a5ead2b87c1026930214ba51c2b8`  
		Last Modified: Thu, 07 Sep 2023 01:52:25 GMT  
		Size: 1.5 KB (1481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22e56804b3ad37bd9f7ff556ddf336fe3b2ed8503cb32b0dfee800e4c76d9451`  
		Last Modified: Thu, 07 Sep 2023 01:52:25 GMT  
		Size: 1.4 MB (1385452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:288264a2552805e7baa2b8233fa1aad54720bdba711d9147660fe31f59cc2f32`  
		Last Modified: Thu, 07 Sep 2023 01:52:25 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1` - linux; arm64 variant v8

```console
$ docker pull adminer@sha256:3b35134d84f9bb500b4ea3b9e5998209f9e587ef94982ee30e6357ae9f30d7c8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.3 MB (94338646 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6f05a6588020fe9fe371405a1735a4614daa30b4e299bd24afa4d2a017d0fa2`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Thu, 07 Sep 2023 00:39:45 GMT
ADD file:6bc001e951ef1280f566a92e65fcff57aefb8a280aa3510b7cd4b4e0a54c5cff in / 
# Thu, 07 Sep 2023 00:39:46 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 02:22:22 GMT
STOPSIGNAL SIGINT
# Thu, 07 Sep 2023 02:22:41 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 02:22:42 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Thu, 07 Sep 2023 02:22:42 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 07 Sep 2023 02:22:43 GMT
WORKDIR /var/www/html
# Thu, 07 Sep 2023 02:22:43 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 07 Sep 2023 02:22:43 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 07 Sep 2023 02:22:43 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 07 Sep 2023 02:22:43 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 07 Sep 2023 02:22:53 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 07 Sep 2023 02:22:53 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 07 Sep 2023 02:22:54 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 07 Sep 2023 02:22:54 GMT
USER adminer
# Thu, 07 Sep 2023 02:22:54 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Thu, 07 Sep 2023 02:22:54 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:61c16b7975697b00760ff9536c09eed29b6a76923d4d98be38e9cdc749506417`  
		Last Modified: Thu, 07 Sep 2023 00:43:21 GMT  
		Size: 53.7 MB (53704716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81f75bf1a78b692b687a603db539e512b761e91500113ab03d603be6cd108610`  
		Last Modified: Thu, 07 Sep 2023 02:23:31 GMT  
		Size: 39.2 MB (39244334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f3afc31326ca8d485c99b99322b549a89dd0db30062feaba0986df541301b45`  
		Last Modified: Thu, 07 Sep 2023 02:23:23 GMT  
		Size: 385.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c635f2e362703c71ad0c137ad3994b892ba8f342bd446e64f80d66d9c7c6965`  
		Last Modified: Thu, 07 Sep 2023 02:23:23 GMT  
		Size: 1.9 KB (1880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed650e87b8c0a626a5474dfdb12657fbf231ce26d8aef7302216b8b36e6c89f3`  
		Last Modified: Thu, 07 Sep 2023 02:23:24 GMT  
		Size: 1.5 KB (1481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e277a4a1ba7b301b2528764da6494b52a7e34668a0758bb6a9d5d0cb9ba10806`  
		Last Modified: Thu, 07 Sep 2023 02:23:24 GMT  
		Size: 1.4 MB (1385360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eea59163ae0d170091fc6d9eca39c3f6b9a6adaabf7b2a4cf5ecdd03cf72409c`  
		Last Modified: Thu, 07 Sep 2023 02:23:24 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1` - linux; 386

```console
$ docker pull adminer@sha256:71277e51e4144523793606f751c038e0d916c407170b76f6cfa658c0c68343d5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.0 MB (96989028 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a106263b0383ca702783152eabdd6eb8b1a95f18131c42c0d3e7d18b043e7766`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Thu, 07 Sep 2023 00:39:12 GMT
ADD file:bf79261700cf8412eb759b5cfc3a37825dad004e81e864a5e2fd8e3bbbaf217e in / 
# Thu, 07 Sep 2023 00:39:12 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 12:09:39 GMT
STOPSIGNAL SIGINT
# Thu, 07 Sep 2023 12:10:10 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 12:10:11 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Thu, 07 Sep 2023 12:10:12 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 07 Sep 2023 12:10:12 GMT
WORKDIR /var/www/html
# Thu, 07 Sep 2023 12:10:12 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 07 Sep 2023 12:10:12 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 07 Sep 2023 12:10:12 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 07 Sep 2023 12:10:13 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 07 Sep 2023 12:10:27 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 07 Sep 2023 12:10:27 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 07 Sep 2023 12:10:27 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 07 Sep 2023 12:10:27 GMT
USER adminer
# Thu, 07 Sep 2023 12:10:27 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Thu, 07 Sep 2023 12:10:28 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:3a8f1bd5e39092e1e02a2c349cd4130e74a705d3d2b5f2f789f856632f3a25f1`  
		Last Modified: Thu, 07 Sep 2023 00:44:11 GMT  
		Size: 56.0 MB (56040528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef650b8daf931017283220f9b80654004afffa052c63a056e04426e98e922c89`  
		Last Modified: Thu, 07 Sep 2023 12:11:19 GMT  
		Size: 39.6 MB (39558962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1aadcb9575090ce09730ba3ef7d97c83290dc26159d7c19578334814b97d385c`  
		Last Modified: Thu, 07 Sep 2023 12:11:07 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9f708d67412753311bfd807ee09e0c256ae0531c26a6c2d5075ed2aab302d86`  
		Last Modified: Thu, 07 Sep 2023 12:11:07 GMT  
		Size: 1.9 KB (1868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c66b98bb7e1695e588451617cdf75ddd0a944e24fac5d26f4e5dcae02a0d465`  
		Last Modified: Thu, 07 Sep 2023 12:11:07 GMT  
		Size: 1.5 KB (1477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a223a9d49f0399f82d2da1d359bdca68a494b10032f79ec5bf03c8bef97b901f`  
		Last Modified: Thu, 07 Sep 2023 12:11:08 GMT  
		Size: 1.4 MB (1385313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf4a0fda7c9aa7946db984687228316c0ed36e8dde882f6786834f088d6154b4`  
		Last Modified: Thu, 07 Sep 2023 12:11:07 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1` - linux; mips64le

```console
$ docker pull adminer@sha256:9cc962f9ae71f2c5b15623bc438ebb6d9a340e0ba8d278d98c031c39e1b5e407
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.6 MB (92612452 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c340fe4c80d84cb71a7948c0d3da3ae567112f144fa0d27c1320899c29a61f0`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Thu, 07 Sep 2023 01:09:47 GMT
ADD file:fdd438b39f1dce564715691d2a092378f02bc722e29cb80216efcbaf71cff0b8 in / 
# Thu, 07 Sep 2023 01:09:53 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 03:08:04 GMT
STOPSIGNAL SIGINT
# Thu, 07 Sep 2023 03:10:03 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 03:10:09 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Thu, 07 Sep 2023 03:10:16 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 07 Sep 2023 03:10:19 GMT
WORKDIR /var/www/html
# Thu, 07 Sep 2023 03:10:23 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 07 Sep 2023 03:10:26 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 07 Sep 2023 03:10:30 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 07 Sep 2023 03:10:33 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 07 Sep 2023 03:11:27 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 07 Sep 2023 03:11:30 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 07 Sep 2023 03:11:33 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 07 Sep 2023 03:11:36 GMT
USER adminer
# Thu, 07 Sep 2023 03:11:40 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Thu, 07 Sep 2023 03:11:43 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:0d1f1f4ccb1e0da4313c3ebcd521e7fa8073526c6f64ca7214ed31ae9bd0788e`  
		Last Modified: Thu, 07 Sep 2023 01:21:00 GMT  
		Size: 53.3 MB (53271469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b724451ca3bae07bf7da51b1c949189dc86f1e494be2830616fbe3cf4c7a447`  
		Last Modified: Thu, 07 Sep 2023 03:14:20 GMT  
		Size: 38.0 MB (37950499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:915c5f7e479b8d1cb1baf57fd9f07e06b962433d3a40fc832491c6f6614522bb`  
		Last Modified: Thu, 07 Sep 2023 03:13:55 GMT  
		Size: 394.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffcee722bb0f36a2975167c5ddf08d0da2cb56e72317f5f3e9d5cfbc3d4a4716`  
		Last Modified: Thu, 07 Sep 2023 03:13:54 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fc9ff6a8f7fb04dd6c3d6df59d01f1c9c7c34ad3cbe41553ecdff949bd20c1e`  
		Last Modified: Thu, 07 Sep 2023 03:13:54 GMT  
		Size: 1.5 KB (1482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cb2cbc2bc303d453e8e91cca3d170ccb3b27fd2bd03b89a3924e679e78c26e4`  
		Last Modified: Thu, 07 Sep 2023 03:13:55 GMT  
		Size: 1.4 MB (1386382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efe356c9d62e82baa2ebf75971c57e6fadf0e138988c966f6767875ff8843182`  
		Last Modified: Thu, 07 Sep 2023 03:13:54 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1` - linux; ppc64le

```console
$ docker pull adminer@sha256:af35710d0480902e87252a3b766b10d0f75285c0d22bafce974f049ed8128552
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.3 MB (101262505 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ec6c6c445d603cdb55b8e2df3d7ca3ab043dee3a4535b6dd28cd47284c99eed`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Thu, 07 Sep 2023 00:17:47 GMT
ADD file:da42a2ef7aa1ce7e6df281b469ac67db062d14c59066a6dfd7ac5cc91d7a3b8c in / 
# Thu, 07 Sep 2023 00:17:50 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 09:04:15 GMT
STOPSIGNAL SIGINT
# Thu, 07 Sep 2023 09:07:04 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 09:07:10 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Thu, 07 Sep 2023 09:07:13 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 07 Sep 2023 09:07:14 GMT
WORKDIR /var/www/html
# Thu, 07 Sep 2023 09:07:14 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 07 Sep 2023 09:07:15 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 07 Sep 2023 09:07:15 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 07 Sep 2023 09:07:16 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 07 Sep 2023 09:08:33 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 07 Sep 2023 09:08:33 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 07 Sep 2023 09:08:35 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 07 Sep 2023 09:08:36 GMT
USER adminer
# Thu, 07 Sep 2023 09:08:38 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Thu, 07 Sep 2023 09:08:39 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:fb3cfd509d4c62da47ee9c7eee6545472d58ceaab6fcd454a82d188766dd0c45`  
		Last Modified: Thu, 07 Sep 2023 00:23:55 GMT  
		Size: 58.9 MB (58928091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bffc3bba24bd4cd45431ae9c166638ec8595b5ecab4200290f8c176a1212b7c`  
		Last Modified: Thu, 07 Sep 2023 09:11:25 GMT  
		Size: 40.9 MB (40944217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d37dbbfa36efc1b986a9571f61c675f6dd3304c8b0f8ea6ce287be3e977d1976`  
		Last Modified: Thu, 07 Sep 2023 09:11:12 GMT  
		Size: 398.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:040ad87be7d0fd1ec4f721e5fd3acd35286b3f5dd90a2f50595443791d2c5f78`  
		Last Modified: Thu, 07 Sep 2023 09:11:12 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fde911bb7830da7a8226144a744f977069a6a35fc88a5f98301891261503ecf`  
		Last Modified: Thu, 07 Sep 2023 09:11:12 GMT  
		Size: 1.5 KB (1476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1ce36781194ed33448f80f0902704489627f8098ddd838fc8a41ca597ccbfab`  
		Last Modified: Thu, 07 Sep 2023 09:11:13 GMT  
		Size: 1.4 MB (1385951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d01192f86adad3c4b51a184a68865d082250b44614aa375d150dda8f5f36b927`  
		Last Modified: Thu, 07 Sep 2023 09:11:12 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1` - linux; s390x

```console
$ docker pull adminer@sha256:b3028b06f7c78024603ab547558cf83d4fe518c6bfd10a107ee923081d45c3a6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.7 MB (93700732 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40878d5b42fdc65d89e9d563be958aad831592c92455633ce54a025dc6bac4eb`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Thu, 07 Sep 2023 00:44:03 GMT
ADD file:a0582e191d0265b98e5d46c64ba9b4c46445cfa821c6e41d32db343b0e2a6fec in / 
# Thu, 07 Sep 2023 00:44:12 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 01:26:26 GMT
STOPSIGNAL SIGINT
# Thu, 07 Sep 2023 01:27:02 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 01:27:07 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Thu, 07 Sep 2023 01:27:08 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 07 Sep 2023 01:27:08 GMT
WORKDIR /var/www/html
# Thu, 07 Sep 2023 01:27:09 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 07 Sep 2023 01:27:09 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 07 Sep 2023 01:27:09 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 07 Sep 2023 01:27:09 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 07 Sep 2023 01:27:22 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 07 Sep 2023 01:27:22 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 07 Sep 2023 01:27:23 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 07 Sep 2023 01:27:24 GMT
USER adminer
# Thu, 07 Sep 2023 01:27:24 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Thu, 07 Sep 2023 01:27:24 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:6dd2d41f67a6666210e1a34694b8765e945a44014b53252ec0e1b50491e08d69`  
		Last Modified: Thu, 07 Sep 2023 00:49:54 GMT  
		Size: 53.3 MB (53290217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe4a876b44eaaf1ba3c702ea08a6af25e23abb30b7fcbef9b957a4c34ec5ad73`  
		Last Modified: Thu, 07 Sep 2023 01:28:21 GMT  
		Size: 39.0 MB (39020691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:529f8a0ebc99b919f45c296bfffe1d9aa35136c91542e626681a898a1e1dabb2`  
		Last Modified: Thu, 07 Sep 2023 01:28:14 GMT  
		Size: 393.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:322f53d9402212f75016bdbb862615c373419e902c2b0a0994373659dc9a40dc`  
		Last Modified: Thu, 07 Sep 2023 01:28:14 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c552fc3addf63a6a3c52100ad6a25209610153282a2977fc8234b019e7bfa4b8`  
		Last Modified: Thu, 07 Sep 2023 01:28:14 GMT  
		Size: 1.5 KB (1480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a4df5368a1108e415af1adad06e9925df044775278212b278f40db0c9e828b6`  
		Last Modified: Thu, 07 Sep 2023 01:28:15 GMT  
		Size: 1.4 MB (1385578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d8fa422b756819743a45bc63685472b1df2c01002596e8beb4231c6f1235f34`  
		Last Modified: Thu, 07 Sep 2023 01:28:14 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `adminer:4.8.1-fastcgi`

```console
$ docker pull adminer@sha256:3240fafaf56f18ec0d10835a26868e6022d637d213088732290b80fd613edcfa
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
$ docker pull adminer@sha256:15659f7db1e32df8ee184ace61ba9c86663fe995dcc68b5bee681676cd65c86d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.9 MB (95940089 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:88b4d4658217a7fbd5718733b47cfdfcd835cba81366d47a5edc8516a640bd9f`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Thu, 07 Sep 2023 00:21:01 GMT
ADD file:144dff349a666134b5e98a9f1c6650fd9d6e4a88a6f98857f26eb84989360b91 in / 
# Thu, 07 Sep 2023 00:21:02 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 03:10:23 GMT
STOPSIGNAL SIGINT
# Thu, 07 Sep 2023 03:10:44 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 03:10:45 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Thu, 07 Sep 2023 03:11:05 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Thu, 07 Sep 2023 03:11:05 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 07 Sep 2023 03:11:05 GMT
WORKDIR /var/www/html
# Thu, 07 Sep 2023 03:11:06 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 07 Sep 2023 03:11:06 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 07 Sep 2023 03:11:06 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 07 Sep 2023 03:11:06 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 07 Sep 2023 03:11:16 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 07 Sep 2023 03:11:16 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 07 Sep 2023 03:11:16 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 07 Sep 2023 03:11:17 GMT
USER adminer
# Thu, 07 Sep 2023 03:11:17 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:5dea071bb9782209397443f024a630052ab7583e365894d414f1e39cd0f65025`  
		Last Modified: Thu, 07 Sep 2023 00:25:41 GMT  
		Size: 55.1 MB (55056245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d84864d5d25a2386de4d3f48de320a52febc28bb28cb742aba6d777c4128696`  
		Last Modified: Thu, 07 Sep 2023 03:11:37 GMT  
		Size: 39.5 MB (39491426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:792bf43687eb38330b06a085a88b6c0505837ae192ac0fe027f7a07215f853a6`  
		Last Modified: Thu, 07 Sep 2023 03:11:29 GMT  
		Size: 395.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e01de01b95b38bf91fd08d70ff82b982b8dca2110bf77448cea418e95e126d9a`  
		Last Modified: Thu, 07 Sep 2023 03:11:54 GMT  
		Size: 2.7 KB (2712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15e0eed8de828090b43d0bbdb0fe4d095f18b39bea0ba03bdde09742311c98e2`  
		Last Modified: Thu, 07 Sep 2023 03:11:54 GMT  
		Size: 1.9 KB (1880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:871d9ee2bd875b8e07cda014c321142ca148c41385ad50db557708d53aeed910`  
		Last Modified: Thu, 07 Sep 2023 03:11:54 GMT  
		Size: 1.5 KB (1480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ea47c50e3a334983865aa3a1ac8269133885d8dc06e6bd3adfbdb41cb6b08c6`  
		Last Modified: Thu, 07 Sep 2023 03:11:55 GMT  
		Size: 1.4 MB (1385463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9fee1469c7254200561d4b1b94f32fc0485731de2477b06e6df7013098f6c7b`  
		Last Modified: Thu, 07 Sep 2023 03:11:54 GMT  
		Size: 488.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1-fastcgi` - linux; arm variant v5

```console
$ docker pull adminer@sha256:68a8a35328fd756b490e1ee7bfe37451f377151d253bf2a13b8132dec21e0ce0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.2 MB (91197773 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ac4abb044959ec9100e2123e544a8bb1c39a3e7299cb2b54f30345e746092ce`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Thu, 07 Sep 2023 00:48:38 GMT
ADD file:bad04cab9856def18134a0c7925a5f43816c14da597964b6d5567abc3ef6a8b9 in / 
# Thu, 07 Sep 2023 00:48:39 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 05:57:06 GMT
STOPSIGNAL SIGINT
# Thu, 07 Sep 2023 05:57:39 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 05:57:40 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Thu, 07 Sep 2023 05:58:04 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Thu, 07 Sep 2023 05:58:05 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 07 Sep 2023 05:58:05 GMT
WORKDIR /var/www/html
# Thu, 07 Sep 2023 05:58:05 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 07 Sep 2023 05:58:05 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 07 Sep 2023 05:58:05 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 07 Sep 2023 05:58:05 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 07 Sep 2023 05:58:18 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 07 Sep 2023 05:58:18 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 07 Sep 2023 05:58:18 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 07 Sep 2023 05:58:18 GMT
USER adminer
# Thu, 07 Sep 2023 05:58:18 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:c77da54c1e584356232e8207afbbe30938a9c2dda2ebc314c1d66e34c74245cc`  
		Last Modified: Thu, 07 Sep 2023 00:51:56 GMT  
		Size: 52.6 MB (52557684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f9ecd2f984b7ccbad8542193859188aa41052ff9a7f1b62ad82ac8bd8a4dc94`  
		Last Modified: Thu, 07 Sep 2023 05:58:40 GMT  
		Size: 37.2 MB (37247813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74f16b90817746d2df9ca8097b34f1a2a58ddea40f9d13b7661801e9d0cabeb6`  
		Last Modified: Thu, 07 Sep 2023 05:58:32 GMT  
		Size: 392.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19291db959f5743b3fc9e761a855018f488f61c2f70012d7a14fb1319d0d61f3`  
		Last Modified: Thu, 07 Sep 2023 05:58:57 GMT  
		Size: 2.7 KB (2713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04fa7bdce9b8e241d877c81cd956b30e00826a78a5513355c03646ecab5c6a09`  
		Last Modified: Thu, 07 Sep 2023 05:58:57 GMT  
		Size: 1.9 KB (1869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0867e050c3c0c3917ee2ff18cf6b6becb88fe6053803081900c3382331506c8`  
		Last Modified: Thu, 07 Sep 2023 05:58:57 GMT  
		Size: 1.5 KB (1480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c35adb51769011f110acbf0514bab08249bcf812b1da24327bed43b4eb11ba2`  
		Last Modified: Thu, 07 Sep 2023 05:58:58 GMT  
		Size: 1.4 MB (1385331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:254cd97ad98c8e7fb70fe19de389cf9b2863df4d23f3885d54fd68242293a387`  
		Last Modified: Thu, 07 Sep 2023 05:58:57 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1-fastcgi` - linux; arm variant v7

```console
$ docker pull adminer@sha256:a0d499c047e84848247c5a877bd3c4064625f4a64495f89e1ad95093fce1ac3f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.8 MB (87798646 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33f2770b6fe2af3a75e07d84e1b363bad6515ceb1b6972d4d9902323283d0694`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Thu, 07 Sep 2023 00:57:59 GMT
ADD file:931564fb3c8ea78b763a6b98f2739bb7c6a38484122c560a87c7166b7d45c5e6 in / 
# Thu, 07 Sep 2023 00:58:00 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 01:50:52 GMT
STOPSIGNAL SIGINT
# Thu, 07 Sep 2023 01:51:32 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 01:51:33 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Thu, 07 Sep 2023 01:52:01 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Thu, 07 Sep 2023 01:52:02 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 07 Sep 2023 01:52:02 GMT
WORKDIR /var/www/html
# Thu, 07 Sep 2023 01:52:02 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 07 Sep 2023 01:52:02 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 07 Sep 2023 01:52:02 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 07 Sep 2023 01:52:02 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 07 Sep 2023 01:52:14 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 07 Sep 2023 01:52:14 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 07 Sep 2023 01:52:14 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 07 Sep 2023 01:52:14 GMT
USER adminer
# Thu, 07 Sep 2023 01:52:15 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:5826e0d927336e7231f9d05ec48f075045fb51f9b3f16f1e20972f2a3634d102`  
		Last Modified: Thu, 07 Sep 2023 01:02:50 GMT  
		Size: 50.2 MB (50219233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64126d7f6d5bc4ca6d42b71dc00598c67b9f6f17d6919fcce1f03a613722e16d`  
		Last Modified: Thu, 07 Sep 2023 01:52:33 GMT  
		Size: 36.2 MB (36187001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fd3d57a54c1b1fa49ef5fdece23637a20b7f8e985a804fc2c5135f097a549bb`  
		Last Modified: Thu, 07 Sep 2023 01:52:25 GMT  
		Size: 393.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21903f65656bc64fb0c6609085b2d6702f7968442e7354cf234741fc68c2f5f4`  
		Last Modified: Thu, 07 Sep 2023 01:52:51 GMT  
		Size: 2.7 KB (2711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0113ab9766972272a3d4c016308b4e1e22c504b634d6941e6b9c059cad5b3d45`  
		Last Modified: Thu, 07 Sep 2023 01:52:51 GMT  
		Size: 1.9 KB (1871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d992cf32eddb4dbb575f70c5b565ee0fb23d47953ed8292e06ac9555ddeeb123`  
		Last Modified: Thu, 07 Sep 2023 01:52:52 GMT  
		Size: 1.5 KB (1480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47b5e7c51aefa173a76e0fa25e50964e84f858eba6e8225bb1f29ee18d6062b0`  
		Last Modified: Thu, 07 Sep 2023 01:52:52 GMT  
		Size: 1.4 MB (1385466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c65e533099f9039fa0e0df43fda417b7954478ea6aa401dedf1ee822938b5b7e`  
		Last Modified: Thu, 07 Sep 2023 01:52:51 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1-fastcgi` - linux; arm64 variant v8

```console
$ docker pull adminer@sha256:a38ecc5faf0a8576b1bdd76c2f602a86daa9b6cd71b16633fb7ce005ef32bd8d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.3 MB (94341386 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a500c1c0d44c969c688bca9ba88bcb562155d2c6dace06dbe71086fdbdb6fb82`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Thu, 07 Sep 2023 00:39:45 GMT
ADD file:6bc001e951ef1280f566a92e65fcff57aefb8a280aa3510b7cd4b4e0a54c5cff in / 
# Thu, 07 Sep 2023 00:39:46 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 02:22:22 GMT
STOPSIGNAL SIGINT
# Thu, 07 Sep 2023 02:22:41 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 02:22:42 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Thu, 07 Sep 2023 02:23:02 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Thu, 07 Sep 2023 02:23:03 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 07 Sep 2023 02:23:03 GMT
WORKDIR /var/www/html
# Thu, 07 Sep 2023 02:23:03 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 07 Sep 2023 02:23:03 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 07 Sep 2023 02:23:03 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 07 Sep 2023 02:23:03 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 07 Sep 2023 02:23:13 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 07 Sep 2023 02:23:13 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 07 Sep 2023 02:23:13 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 07 Sep 2023 02:23:13 GMT
USER adminer
# Thu, 07 Sep 2023 02:23:13 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:61c16b7975697b00760ff9536c09eed29b6a76923d4d98be38e9cdc749506417`  
		Last Modified: Thu, 07 Sep 2023 00:43:21 GMT  
		Size: 53.7 MB (53704716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81f75bf1a78b692b687a603db539e512b761e91500113ab03d603be6cd108610`  
		Last Modified: Thu, 07 Sep 2023 02:23:31 GMT  
		Size: 39.2 MB (39244334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f3afc31326ca8d485c99b99322b549a89dd0db30062feaba0986df541301b45`  
		Last Modified: Thu, 07 Sep 2023 02:23:23 GMT  
		Size: 385.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efb65c5d18143c713fb41d912e5eb0419de652c480d7db9d798886f092df48a7`  
		Last Modified: Thu, 07 Sep 2023 02:23:47 GMT  
		Size: 2.7 KB (2709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f811d6324927c972ba66211edfdf8f3c83f50e55193712a29387b3787210591d`  
		Last Modified: Thu, 07 Sep 2023 02:23:47 GMT  
		Size: 1.9 KB (1883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e0bd6ef968ad02351f0b7c15001f9016c5be9aabf3c89e45d5d1347c663b6fa`  
		Last Modified: Thu, 07 Sep 2023 02:23:47 GMT  
		Size: 1.5 KB (1477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b21fc274312e94dc7ca9579a44d64426c71ea39388a81328c0a00f3bfc7a0ada`  
		Last Modified: Thu, 07 Sep 2023 02:23:47 GMT  
		Size: 1.4 MB (1385391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0360824626289cffd506daf3a7e018ae732cad6b53e2e81b212e909ebc93627e`  
		Last Modified: Thu, 07 Sep 2023 02:23:47 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1-fastcgi` - linux; 386

```console
$ docker pull adminer@sha256:e069ad6357b6e472b22c167d7e6644c1829900d73629b9ebfc05888ce049bfe2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.0 MB (96991740 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb5eea91a8ed56f36a9c6995824b55264ceb8328a4941035def4679918353dd1`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Thu, 07 Sep 2023 00:39:12 GMT
ADD file:bf79261700cf8412eb759b5cfc3a37825dad004e81e864a5e2fd8e3bbbaf217e in / 
# Thu, 07 Sep 2023 00:39:12 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 12:09:39 GMT
STOPSIGNAL SIGINT
# Thu, 07 Sep 2023 12:10:10 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 12:10:11 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Thu, 07 Sep 2023 12:10:38 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Thu, 07 Sep 2023 12:10:38 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 07 Sep 2023 12:10:38 GMT
WORKDIR /var/www/html
# Thu, 07 Sep 2023 12:10:39 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 07 Sep 2023 12:10:39 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 07 Sep 2023 12:10:39 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 07 Sep 2023 12:10:39 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 07 Sep 2023 12:10:52 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 07 Sep 2023 12:10:52 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 07 Sep 2023 12:10:53 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 07 Sep 2023 12:10:53 GMT
USER adminer
# Thu, 07 Sep 2023 12:10:53 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:3a8f1bd5e39092e1e02a2c349cd4130e74a705d3d2b5f2f789f856632f3a25f1`  
		Last Modified: Thu, 07 Sep 2023 00:44:11 GMT  
		Size: 56.0 MB (56040528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef650b8daf931017283220f9b80654004afffa052c63a056e04426e98e922c89`  
		Last Modified: Thu, 07 Sep 2023 12:11:19 GMT  
		Size: 39.6 MB (39558962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1aadcb9575090ce09730ba3ef7d97c83290dc26159d7c19578334814b97d385c`  
		Last Modified: Thu, 07 Sep 2023 12:11:07 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:206b2630ac8f6aa6eb9676d5d718f3b1ca67165cfd573cefdf1e251331ef29b5`  
		Last Modified: Thu, 07 Sep 2023 12:11:37 GMT  
		Size: 2.7 KB (2706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32eb027a1b6db47b5e7792470a858de1751693bfad00275098ec7ae5339cb2dd`  
		Last Modified: Thu, 07 Sep 2023 12:11:37 GMT  
		Size: 1.9 KB (1868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f225674f1c59970df0a8b235c9341a870da5e62367b0fc9e04f9da95e07aebc6`  
		Last Modified: Thu, 07 Sep 2023 12:11:37 GMT  
		Size: 1.5 KB (1476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4f193a9bed4495ca1aaf2880bc9a5c91a310d1481061d98b0e69fe8378c9cba`  
		Last Modified: Thu, 07 Sep 2023 12:11:37 GMT  
		Size: 1.4 MB (1385318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b39ea62233bf837ee84ca7d0138bb7266ae225c1c1bcf8ed5ab724a85ceace5b`  
		Last Modified: Thu, 07 Sep 2023 12:11:37 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1-fastcgi` - linux; mips64le

```console
$ docker pull adminer@sha256:2c3b4d978627105affcd060a2a4602bb97f1fd90187edd5cb30b338b22584e15
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.6 MB (92615139 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c2be39d77614a37ab8c0c9448232e1be6fb18fca8a2696bdb76f7ba90b69578`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Thu, 07 Sep 2023 01:09:47 GMT
ADD file:fdd438b39f1dce564715691d2a092378f02bc722e29cb80216efcbaf71cff0b8 in / 
# Thu, 07 Sep 2023 01:09:53 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 03:08:04 GMT
STOPSIGNAL SIGINT
# Thu, 07 Sep 2023 03:10:03 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 03:10:09 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Thu, 07 Sep 2023 03:12:06 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Thu, 07 Sep 2023 03:12:13 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 07 Sep 2023 03:12:16 GMT
WORKDIR /var/www/html
# Thu, 07 Sep 2023 03:12:19 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 07 Sep 2023 03:12:22 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 07 Sep 2023 03:12:26 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 07 Sep 2023 03:12:29 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 07 Sep 2023 03:13:20 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 07 Sep 2023 03:13:23 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 07 Sep 2023 03:13:27 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 07 Sep 2023 03:13:30 GMT
USER adminer
# Thu, 07 Sep 2023 03:13:34 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:0d1f1f4ccb1e0da4313c3ebcd521e7fa8073526c6f64ca7214ed31ae9bd0788e`  
		Last Modified: Thu, 07 Sep 2023 01:21:00 GMT  
		Size: 53.3 MB (53271469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b724451ca3bae07bf7da51b1c949189dc86f1e494be2830616fbe3cf4c7a447`  
		Last Modified: Thu, 07 Sep 2023 03:14:20 GMT  
		Size: 38.0 MB (37950499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:915c5f7e479b8d1cb1baf57fd9f07e06b962433d3a40fc832491c6f6614522bb`  
		Last Modified: Thu, 07 Sep 2023 03:13:55 GMT  
		Size: 394.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c089a408ed63eef86310ec1d3db9d84aa46d7f541e3ec1e90a4798aa6545d436`  
		Last Modified: Thu, 07 Sep 2023 03:14:41 GMT  
		Size: 2.7 KB (2713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56bb790d23ceab0acafe02823b5726a9a99319fc3ce2e215cbbc11d2e5b57a60`  
		Last Modified: Thu, 07 Sep 2023 03:14:41 GMT  
		Size: 1.7 KB (1725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c5b3c385bb7fe02cc10cefc1cc9bfd8a7c41d4d908b07bef77f7f7c0308086a`  
		Last Modified: Thu, 07 Sep 2023 03:14:41 GMT  
		Size: 1.5 KB (1479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ae8742bfc11fac37d1a8257111b0cdde75cd0c7d628fe1c99a1767583510d4f`  
		Last Modified: Thu, 07 Sep 2023 03:14:42 GMT  
		Size: 1.4 MB (1386368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd25dbfd1a8ef46f40a314361de018304317b3f157bf58c376b23d42d53e9f5a`  
		Last Modified: Thu, 07 Sep 2023 03:14:41 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1-fastcgi` - linux; ppc64le

```console
$ docker pull adminer@sha256:b7224d5a014ff9f27bb1a4b1aff7ed321765e5f8ec175d34613ccdef6e2da361
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.3 MB (101265147 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70f1927913fd3d1b839c87d619e0d41128e9ac696c2e77895368025a38cdb9c0`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Thu, 07 Sep 2023 00:17:47 GMT
ADD file:da42a2ef7aa1ce7e6df281b469ac67db062d14c59066a6dfd7ac5cc91d7a3b8c in / 
# Thu, 07 Sep 2023 00:17:50 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 09:04:15 GMT
STOPSIGNAL SIGINT
# Thu, 07 Sep 2023 09:07:04 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 09:07:10 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Thu, 07 Sep 2023 09:08:56 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Thu, 07 Sep 2023 09:09:03 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 07 Sep 2023 09:09:06 GMT
WORKDIR /var/www/html
# Thu, 07 Sep 2023 09:09:06 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 07 Sep 2023 09:09:08 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 07 Sep 2023 09:09:09 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 07 Sep 2023 09:09:10 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 07 Sep 2023 09:10:21 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 07 Sep 2023 09:10:25 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 07 Sep 2023 09:10:33 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 07 Sep 2023 09:10:40 GMT
USER adminer
# Thu, 07 Sep 2023 09:10:52 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:fb3cfd509d4c62da47ee9c7eee6545472d58ceaab6fcd454a82d188766dd0c45`  
		Last Modified: Thu, 07 Sep 2023 00:23:55 GMT  
		Size: 58.9 MB (58928091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bffc3bba24bd4cd45431ae9c166638ec8595b5ecab4200290f8c176a1212b7c`  
		Last Modified: Thu, 07 Sep 2023 09:11:25 GMT  
		Size: 40.9 MB (40944217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d37dbbfa36efc1b986a9571f61c675f6dd3304c8b0f8ea6ce287be3e977d1976`  
		Last Modified: Thu, 07 Sep 2023 09:11:12 GMT  
		Size: 398.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6805ebe3dfb3654d46f5fc9a8cd6a74c2a86ade728959b1dfa0739f99c1b5428`  
		Last Modified: Thu, 07 Sep 2023 09:11:45 GMT  
		Size: 2.7 KB (2714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70c512e9728df1edeb0e0315c69e85528520cf302979f8f6ade2fca0b27185b5`  
		Last Modified: Thu, 07 Sep 2023 09:11:45 GMT  
		Size: 1.9 KB (1876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11e2e6a603583abf7085bdbf1f879974415c61c29c08962f4b96fb4fe3ce981d`  
		Last Modified: Thu, 07 Sep 2023 09:11:45 GMT  
		Size: 1.5 KB (1478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d971487f8cbfeaa9c06033dcafc7e63fa3556563916948e905fc7c62b4126c8b`  
		Last Modified: Thu, 07 Sep 2023 09:11:46 GMT  
		Size: 1.4 MB (1385882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbc9d316bb2a490069e9c690d1f2e1e73e0765b2cfa7fab34108868e6756e9a3`  
		Last Modified: Thu, 07 Sep 2023 09:11:45 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1-fastcgi` - linux; s390x

```console
$ docker pull adminer@sha256:de471294d28d5750d41244ba8d44db2cb1aaab848922985f660b02eabbd197dc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.7 MB (93703439 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cde1549e5993997b294699895499c6549c361bd95ebd374a3c85442fd76eb165`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Thu, 07 Sep 2023 00:44:03 GMT
ADD file:a0582e191d0265b98e5d46c64ba9b4c46445cfa821c6e41d32db343b0e2a6fec in / 
# Thu, 07 Sep 2023 00:44:12 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 01:26:26 GMT
STOPSIGNAL SIGINT
# Thu, 07 Sep 2023 01:27:02 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 01:27:07 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Thu, 07 Sep 2023 01:27:36 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Thu, 07 Sep 2023 01:27:37 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 07 Sep 2023 01:27:38 GMT
WORKDIR /var/www/html
# Thu, 07 Sep 2023 01:27:38 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 07 Sep 2023 01:27:38 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 07 Sep 2023 01:27:38 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 07 Sep 2023 01:27:39 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 07 Sep 2023 01:27:53 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 07 Sep 2023 01:27:54 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 07 Sep 2023 01:27:54 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 07 Sep 2023 01:27:55 GMT
USER adminer
# Thu, 07 Sep 2023 01:27:55 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:6dd2d41f67a6666210e1a34694b8765e945a44014b53252ec0e1b50491e08d69`  
		Last Modified: Thu, 07 Sep 2023 00:49:54 GMT  
		Size: 53.3 MB (53290217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe4a876b44eaaf1ba3c702ea08a6af25e23abb30b7fcbef9b957a4c34ec5ad73`  
		Last Modified: Thu, 07 Sep 2023 01:28:21 GMT  
		Size: 39.0 MB (39020691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:529f8a0ebc99b919f45c296bfffe1d9aa35136c91542e626681a898a1e1dabb2`  
		Last Modified: Thu, 07 Sep 2023 01:28:14 GMT  
		Size: 393.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e241b68ed72809f13265cadec141405091d29c51cc7031a53fb1ac63e98370e4`  
		Last Modified: Thu, 07 Sep 2023 01:28:34 GMT  
		Size: 2.7 KB (2714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c554ebc3fa08021199bd77796a742b7ec9a23e27c9f301efd186c67355e26ea3`  
		Last Modified: Thu, 07 Sep 2023 01:28:34 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6ddeb9921e2ece9eabbc65206020cfc9fb9c53ebb491a85b96d5eb7ed308c6e`  
		Last Modified: Thu, 07 Sep 2023 01:28:34 GMT  
		Size: 1.5 KB (1481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5c07f366229478ef4b2de990c4de70ab31aa0982284cc7b192581b9c8e765eb`  
		Last Modified: Thu, 07 Sep 2023 01:28:34 GMT  
		Size: 1.4 MB (1385571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6878b99b931b3ddc6e0ae8ba87b925151a30fbb1ade42882571d878a53316bb0`  
		Last Modified: Thu, 07 Sep 2023 01:28:34 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `adminer:4.8.1-standalone`

```console
$ docker pull adminer@sha256:a607d96fbf114fefcdd34729b84a6cd379dedb3ead294c56f0f318f9981fb52a
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
$ docker pull adminer@sha256:5463cc7e5a3e4ad51aa0e98c419d04646fd9b3e14a1d960ab8b420b9ce9ecc80
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.9 MB (95937329 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1bb4da606dc1a8721442935ae417a1ff7d27b9eea6ef228797780679d81ba0b6`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Thu, 07 Sep 2023 00:21:01 GMT
ADD file:144dff349a666134b5e98a9f1c6650fd9d6e4a88a6f98857f26eb84989360b91 in / 
# Thu, 07 Sep 2023 00:21:02 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 03:10:23 GMT
STOPSIGNAL SIGINT
# Thu, 07 Sep 2023 03:10:44 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 03:10:45 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Thu, 07 Sep 2023 03:10:46 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 07 Sep 2023 03:10:46 GMT
WORKDIR /var/www/html
# Thu, 07 Sep 2023 03:10:46 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 07 Sep 2023 03:10:46 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 07 Sep 2023 03:10:46 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 07 Sep 2023 03:10:46 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 07 Sep 2023 03:10:58 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 07 Sep 2023 03:10:58 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 07 Sep 2023 03:10:58 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 07 Sep 2023 03:10:58 GMT
USER adminer
# Thu, 07 Sep 2023 03:10:58 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Thu, 07 Sep 2023 03:10:58 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:5dea071bb9782209397443f024a630052ab7583e365894d414f1e39cd0f65025`  
		Last Modified: Thu, 07 Sep 2023 00:25:41 GMT  
		Size: 55.1 MB (55056245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d84864d5d25a2386de4d3f48de320a52febc28bb28cb742aba6d777c4128696`  
		Last Modified: Thu, 07 Sep 2023 03:11:37 GMT  
		Size: 39.5 MB (39491426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:792bf43687eb38330b06a085a88b6c0505837ae192ac0fe027f7a07215f853a6`  
		Last Modified: Thu, 07 Sep 2023 03:11:29 GMT  
		Size: 395.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37ef5d260982b8b88f34270bbe7314228f686ac4bbbea7e647ab96feaf464e71`  
		Last Modified: Thu, 07 Sep 2023 03:11:29 GMT  
		Size: 1.9 KB (1879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81b9b963ca6d8427a310df0283abe6c6ef185569bb470cf8a0525da60989ecb6`  
		Last Modified: Thu, 07 Sep 2023 03:11:29 GMT  
		Size: 1.5 KB (1480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e57581023c92f337603ebe93de3ebca9a7eeb11706fdccc3f1b359714e0b65a6`  
		Last Modified: Thu, 07 Sep 2023 03:11:30 GMT  
		Size: 1.4 MB (1385412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e97ed40bb1db1cf97113d360f1b14422117cf4154eba611c2d2849d66958ecaa`  
		Last Modified: Thu, 07 Sep 2023 03:11:29 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1-standalone` - linux; arm variant v5

```console
$ docker pull adminer@sha256:dfd42b21fcc7d95faa4380a9bf051771e3bb79badd52e1005a8cbe551c64b6b4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.2 MB (91195063 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd44c48956465a566c168988d7201c27647c33ae7344305a32cd56f85cd46734`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Thu, 07 Sep 2023 00:48:38 GMT
ADD file:bad04cab9856def18134a0c7925a5f43816c14da597964b6d5567abc3ef6a8b9 in / 
# Thu, 07 Sep 2023 00:48:39 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 05:57:06 GMT
STOPSIGNAL SIGINT
# Thu, 07 Sep 2023 05:57:39 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 05:57:40 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Thu, 07 Sep 2023 05:57:41 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 07 Sep 2023 05:57:41 GMT
WORKDIR /var/www/html
# Thu, 07 Sep 2023 05:57:41 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 07 Sep 2023 05:57:41 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 07 Sep 2023 05:57:41 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 07 Sep 2023 05:57:41 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 07 Sep 2023 05:57:57 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 07 Sep 2023 05:57:57 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 07 Sep 2023 05:57:57 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 07 Sep 2023 05:57:57 GMT
USER adminer
# Thu, 07 Sep 2023 05:57:57 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Thu, 07 Sep 2023 05:57:57 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:c77da54c1e584356232e8207afbbe30938a9c2dda2ebc314c1d66e34c74245cc`  
		Last Modified: Thu, 07 Sep 2023 00:51:56 GMT  
		Size: 52.6 MB (52557684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f9ecd2f984b7ccbad8542193859188aa41052ff9a7f1b62ad82ac8bd8a4dc94`  
		Last Modified: Thu, 07 Sep 2023 05:58:40 GMT  
		Size: 37.2 MB (37247813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74f16b90817746d2df9ca8097b34f1a2a58ddea40f9d13b7661801e9d0cabeb6`  
		Last Modified: Thu, 07 Sep 2023 05:58:32 GMT  
		Size: 392.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2db198a220919fae8fc5093acd186481fdccff4b56654baf5ad81f5b16179f41`  
		Last Modified: Thu, 07 Sep 2023 05:58:31 GMT  
		Size: 1.9 KB (1869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bb71f0a31aaaedd68c31d3bd627d15c9a80f1fc8c77d787ae08509cea144944`  
		Last Modified: Thu, 07 Sep 2023 05:58:31 GMT  
		Size: 1.5 KB (1481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7345eee73a7d870b5e002cbc1ab741e76326b7bcedc039de45d03075a08f8bb5`  
		Last Modified: Thu, 07 Sep 2023 05:58:32 GMT  
		Size: 1.4 MB (1385331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d24fe8d24625441b6f9992c49257519dcd2a6962d677d2c96d6de6f440f16d9a`  
		Last Modified: Thu, 07 Sep 2023 05:58:31 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1-standalone` - linux; arm variant v7

```console
$ docker pull adminer@sha256:dde88e85f022908e040ce9f5627e989fca6cf4f796fb912e216bc91e85b80e9f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.8 MB (87795922 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1de3886b83d0afcea5f67dd340efd76d0ff0d7cc5d4d765d7ac24bdce5ac766`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Thu, 07 Sep 2023 00:57:59 GMT
ADD file:931564fb3c8ea78b763a6b98f2739bb7c6a38484122c560a87c7166b7d45c5e6 in / 
# Thu, 07 Sep 2023 00:58:00 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 01:50:52 GMT
STOPSIGNAL SIGINT
# Thu, 07 Sep 2023 01:51:32 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 01:51:33 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Thu, 07 Sep 2023 01:51:34 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 07 Sep 2023 01:51:34 GMT
WORKDIR /var/www/html
# Thu, 07 Sep 2023 01:51:34 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 07 Sep 2023 01:51:34 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 07 Sep 2023 01:51:34 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 07 Sep 2023 01:51:34 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 07 Sep 2023 01:51:48 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 07 Sep 2023 01:51:48 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 07 Sep 2023 01:51:48 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 07 Sep 2023 01:51:48 GMT
USER adminer
# Thu, 07 Sep 2023 01:51:48 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Thu, 07 Sep 2023 01:51:48 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:5826e0d927336e7231f9d05ec48f075045fb51f9b3f16f1e20972f2a3634d102`  
		Last Modified: Thu, 07 Sep 2023 01:02:50 GMT  
		Size: 50.2 MB (50219233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64126d7f6d5bc4ca6d42b71dc00598c67b9f6f17d6919fcce1f03a613722e16d`  
		Last Modified: Thu, 07 Sep 2023 01:52:33 GMT  
		Size: 36.2 MB (36187001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fd3d57a54c1b1fa49ef5fdece23637a20b7f8e985a804fc2c5135f097a549bb`  
		Last Modified: Thu, 07 Sep 2023 01:52:25 GMT  
		Size: 393.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2440750817c8e724091323e3903329ccc274561f1f1e61c49d9da560960899bb`  
		Last Modified: Thu, 07 Sep 2023 01:52:25 GMT  
		Size: 1.9 KB (1869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c56be7ee3fb4f5d4eec7601e51e91b41bf76a5ead2b87c1026930214ba51c2b8`  
		Last Modified: Thu, 07 Sep 2023 01:52:25 GMT  
		Size: 1.5 KB (1481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22e56804b3ad37bd9f7ff556ddf336fe3b2ed8503cb32b0dfee800e4c76d9451`  
		Last Modified: Thu, 07 Sep 2023 01:52:25 GMT  
		Size: 1.4 MB (1385452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:288264a2552805e7baa2b8233fa1aad54720bdba711d9147660fe31f59cc2f32`  
		Last Modified: Thu, 07 Sep 2023 01:52:25 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1-standalone` - linux; arm64 variant v8

```console
$ docker pull adminer@sha256:3b35134d84f9bb500b4ea3b9e5998209f9e587ef94982ee30e6357ae9f30d7c8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.3 MB (94338646 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6f05a6588020fe9fe371405a1735a4614daa30b4e299bd24afa4d2a017d0fa2`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Thu, 07 Sep 2023 00:39:45 GMT
ADD file:6bc001e951ef1280f566a92e65fcff57aefb8a280aa3510b7cd4b4e0a54c5cff in / 
# Thu, 07 Sep 2023 00:39:46 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 02:22:22 GMT
STOPSIGNAL SIGINT
# Thu, 07 Sep 2023 02:22:41 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 02:22:42 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Thu, 07 Sep 2023 02:22:42 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 07 Sep 2023 02:22:43 GMT
WORKDIR /var/www/html
# Thu, 07 Sep 2023 02:22:43 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 07 Sep 2023 02:22:43 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 07 Sep 2023 02:22:43 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 07 Sep 2023 02:22:43 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 07 Sep 2023 02:22:53 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 07 Sep 2023 02:22:53 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 07 Sep 2023 02:22:54 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 07 Sep 2023 02:22:54 GMT
USER adminer
# Thu, 07 Sep 2023 02:22:54 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Thu, 07 Sep 2023 02:22:54 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:61c16b7975697b00760ff9536c09eed29b6a76923d4d98be38e9cdc749506417`  
		Last Modified: Thu, 07 Sep 2023 00:43:21 GMT  
		Size: 53.7 MB (53704716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81f75bf1a78b692b687a603db539e512b761e91500113ab03d603be6cd108610`  
		Last Modified: Thu, 07 Sep 2023 02:23:31 GMT  
		Size: 39.2 MB (39244334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f3afc31326ca8d485c99b99322b549a89dd0db30062feaba0986df541301b45`  
		Last Modified: Thu, 07 Sep 2023 02:23:23 GMT  
		Size: 385.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c635f2e362703c71ad0c137ad3994b892ba8f342bd446e64f80d66d9c7c6965`  
		Last Modified: Thu, 07 Sep 2023 02:23:23 GMT  
		Size: 1.9 KB (1880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed650e87b8c0a626a5474dfdb12657fbf231ce26d8aef7302216b8b36e6c89f3`  
		Last Modified: Thu, 07 Sep 2023 02:23:24 GMT  
		Size: 1.5 KB (1481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e277a4a1ba7b301b2528764da6494b52a7e34668a0758bb6a9d5d0cb9ba10806`  
		Last Modified: Thu, 07 Sep 2023 02:23:24 GMT  
		Size: 1.4 MB (1385360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eea59163ae0d170091fc6d9eca39c3f6b9a6adaabf7b2a4cf5ecdd03cf72409c`  
		Last Modified: Thu, 07 Sep 2023 02:23:24 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1-standalone` - linux; 386

```console
$ docker pull adminer@sha256:664fc6a11ece4d60a18492c17eeb4ffffb3d6fe19d3c4f4c4c3cab52b83f3ec6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.0 MB (96988434 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d7ecc3592e5ee3a2de07572724acd9167630fa736fd16b373959b3f5e2297736`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Tue, 15 Aug 2023 23:39:11 GMT
ADD file:efc88a19b31e68ca41f555bcc51338b0f135cbbd72b90637d8c73969d53addd2 in / 
# Tue, 15 Aug 2023 23:39:12 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 00:23:36 GMT
STOPSIGNAL SIGINT
# Wed, 16 Aug 2023 00:24:03 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 00:24:04 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 16 Aug 2023 00:24:05 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 16 Aug 2023 00:24:05 GMT
WORKDIR /var/www/html
# Wed, 16 Aug 2023 00:24:05 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 16 Aug 2023 00:24:05 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 16 Aug 2023 00:24:05 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 16 Aug 2023 00:24:05 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 16 Aug 2023 00:24:19 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 16 Aug 2023 00:24:19 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 16 Aug 2023 00:24:19 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 16 Aug 2023 00:24:19 GMT
USER adminer
# Wed, 16 Aug 2023 00:24:19 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 16 Aug 2023 00:24:19 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:822e033fa7b169545d5890de01438a9dd87774ff938ff440e823a3ec3f73996d`  
		Last Modified: Tue, 15 Aug 2023 23:43:47 GMT  
		Size: 56.0 MB (56040520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7644269f7e699d335219a554e561f3817b7816e99351232b3646176246991895`  
		Last Modified: Wed, 16 Aug 2023 00:25:00 GMT  
		Size: 39.6 MB (39558428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d96338ff936c667ce1c89a75f7fd111e722685d882b1f36e7b26dcb33007029`  
		Last Modified: Wed, 16 Aug 2023 00:24:50 GMT  
		Size: 389.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5339c86a7bc7031718f83f0a9af19ad028c2fa751748057f9d97d9c94c5075f6`  
		Last Modified: Wed, 16 Aug 2023 00:24:50 GMT  
		Size: 1.9 KB (1868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cbd1ad590a03bbc3ee08a1c944135c7bf81b103067417f79cdb1f8d271b4472`  
		Last Modified: Wed, 16 Aug 2023 00:24:50 GMT  
		Size: 1.5 KB (1480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:225fb2c801a3d35820604ab9c5d6c19a65e18fca4c76dd468e7015b6cb7d5d6c`  
		Last Modified: Wed, 16 Aug 2023 00:24:50 GMT  
		Size: 1.4 MB (1385258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:367f82cd1a3d30bffd1420e0c950c92f859f903ad0b0711848862db96f363ff7`  
		Last Modified: Wed, 16 Aug 2023 00:24:50 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1-standalone` - linux; mips64le

```console
$ docker pull adminer@sha256:9cc962f9ae71f2c5b15623bc438ebb6d9a340e0ba8d278d98c031c39e1b5e407
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.6 MB (92612452 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c340fe4c80d84cb71a7948c0d3da3ae567112f144fa0d27c1320899c29a61f0`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Thu, 07 Sep 2023 01:09:47 GMT
ADD file:fdd438b39f1dce564715691d2a092378f02bc722e29cb80216efcbaf71cff0b8 in / 
# Thu, 07 Sep 2023 01:09:53 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 03:08:04 GMT
STOPSIGNAL SIGINT
# Thu, 07 Sep 2023 03:10:03 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 03:10:09 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Thu, 07 Sep 2023 03:10:16 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 07 Sep 2023 03:10:19 GMT
WORKDIR /var/www/html
# Thu, 07 Sep 2023 03:10:23 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 07 Sep 2023 03:10:26 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 07 Sep 2023 03:10:30 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 07 Sep 2023 03:10:33 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 07 Sep 2023 03:11:27 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 07 Sep 2023 03:11:30 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 07 Sep 2023 03:11:33 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 07 Sep 2023 03:11:36 GMT
USER adminer
# Thu, 07 Sep 2023 03:11:40 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Thu, 07 Sep 2023 03:11:43 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:0d1f1f4ccb1e0da4313c3ebcd521e7fa8073526c6f64ca7214ed31ae9bd0788e`  
		Last Modified: Thu, 07 Sep 2023 01:21:00 GMT  
		Size: 53.3 MB (53271469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b724451ca3bae07bf7da51b1c949189dc86f1e494be2830616fbe3cf4c7a447`  
		Last Modified: Thu, 07 Sep 2023 03:14:20 GMT  
		Size: 38.0 MB (37950499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:915c5f7e479b8d1cb1baf57fd9f07e06b962433d3a40fc832491c6f6614522bb`  
		Last Modified: Thu, 07 Sep 2023 03:13:55 GMT  
		Size: 394.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffcee722bb0f36a2975167c5ddf08d0da2cb56e72317f5f3e9d5cfbc3d4a4716`  
		Last Modified: Thu, 07 Sep 2023 03:13:54 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fc9ff6a8f7fb04dd6c3d6df59d01f1c9c7c34ad3cbe41553ecdff949bd20c1e`  
		Last Modified: Thu, 07 Sep 2023 03:13:54 GMT  
		Size: 1.5 KB (1482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cb2cbc2bc303d453e8e91cca3d170ccb3b27fd2bd03b89a3924e679e78c26e4`  
		Last Modified: Thu, 07 Sep 2023 03:13:55 GMT  
		Size: 1.4 MB (1386382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efe356c9d62e82baa2ebf75971c57e6fadf0e138988c966f6767875ff8843182`  
		Last Modified: Thu, 07 Sep 2023 03:13:54 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1-standalone` - linux; ppc64le

```console
$ docker pull adminer@sha256:af35710d0480902e87252a3b766b10d0f75285c0d22bafce974f049ed8128552
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.3 MB (101262505 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ec6c6c445d603cdb55b8e2df3d7ca3ab043dee3a4535b6dd28cd47284c99eed`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Thu, 07 Sep 2023 00:17:47 GMT
ADD file:da42a2ef7aa1ce7e6df281b469ac67db062d14c59066a6dfd7ac5cc91d7a3b8c in / 
# Thu, 07 Sep 2023 00:17:50 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 09:04:15 GMT
STOPSIGNAL SIGINT
# Thu, 07 Sep 2023 09:07:04 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 09:07:10 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Thu, 07 Sep 2023 09:07:13 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 07 Sep 2023 09:07:14 GMT
WORKDIR /var/www/html
# Thu, 07 Sep 2023 09:07:14 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 07 Sep 2023 09:07:15 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 07 Sep 2023 09:07:15 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 07 Sep 2023 09:07:16 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 07 Sep 2023 09:08:33 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 07 Sep 2023 09:08:33 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 07 Sep 2023 09:08:35 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 07 Sep 2023 09:08:36 GMT
USER adminer
# Thu, 07 Sep 2023 09:08:38 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Thu, 07 Sep 2023 09:08:39 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:fb3cfd509d4c62da47ee9c7eee6545472d58ceaab6fcd454a82d188766dd0c45`  
		Last Modified: Thu, 07 Sep 2023 00:23:55 GMT  
		Size: 58.9 MB (58928091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bffc3bba24bd4cd45431ae9c166638ec8595b5ecab4200290f8c176a1212b7c`  
		Last Modified: Thu, 07 Sep 2023 09:11:25 GMT  
		Size: 40.9 MB (40944217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d37dbbfa36efc1b986a9571f61c675f6dd3304c8b0f8ea6ce287be3e977d1976`  
		Last Modified: Thu, 07 Sep 2023 09:11:12 GMT  
		Size: 398.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:040ad87be7d0fd1ec4f721e5fd3acd35286b3f5dd90a2f50595443791d2c5f78`  
		Last Modified: Thu, 07 Sep 2023 09:11:12 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fde911bb7830da7a8226144a744f977069a6a35fc88a5f98301891261503ecf`  
		Last Modified: Thu, 07 Sep 2023 09:11:12 GMT  
		Size: 1.5 KB (1476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1ce36781194ed33448f80f0902704489627f8098ddd838fc8a41ca597ccbfab`  
		Last Modified: Thu, 07 Sep 2023 09:11:13 GMT  
		Size: 1.4 MB (1385951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d01192f86adad3c4b51a184a68865d082250b44614aa375d150dda8f5f36b927`  
		Last Modified: Thu, 07 Sep 2023 09:11:12 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1-standalone` - linux; s390x

```console
$ docker pull adminer@sha256:b3028b06f7c78024603ab547558cf83d4fe518c6bfd10a107ee923081d45c3a6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.7 MB (93700732 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40878d5b42fdc65d89e9d563be958aad831592c92455633ce54a025dc6bac4eb`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Thu, 07 Sep 2023 00:44:03 GMT
ADD file:a0582e191d0265b98e5d46c64ba9b4c46445cfa821c6e41d32db343b0e2a6fec in / 
# Thu, 07 Sep 2023 00:44:12 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 01:26:26 GMT
STOPSIGNAL SIGINT
# Thu, 07 Sep 2023 01:27:02 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 01:27:07 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Thu, 07 Sep 2023 01:27:08 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 07 Sep 2023 01:27:08 GMT
WORKDIR /var/www/html
# Thu, 07 Sep 2023 01:27:09 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 07 Sep 2023 01:27:09 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 07 Sep 2023 01:27:09 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 07 Sep 2023 01:27:09 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 07 Sep 2023 01:27:22 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 07 Sep 2023 01:27:22 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 07 Sep 2023 01:27:23 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 07 Sep 2023 01:27:24 GMT
USER adminer
# Thu, 07 Sep 2023 01:27:24 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Thu, 07 Sep 2023 01:27:24 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:6dd2d41f67a6666210e1a34694b8765e945a44014b53252ec0e1b50491e08d69`  
		Last Modified: Thu, 07 Sep 2023 00:49:54 GMT  
		Size: 53.3 MB (53290217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe4a876b44eaaf1ba3c702ea08a6af25e23abb30b7fcbef9b957a4c34ec5ad73`  
		Last Modified: Thu, 07 Sep 2023 01:28:21 GMT  
		Size: 39.0 MB (39020691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:529f8a0ebc99b919f45c296bfffe1d9aa35136c91542e626681a898a1e1dabb2`  
		Last Modified: Thu, 07 Sep 2023 01:28:14 GMT  
		Size: 393.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:322f53d9402212f75016bdbb862615c373419e902c2b0a0994373659dc9a40dc`  
		Last Modified: Thu, 07 Sep 2023 01:28:14 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c552fc3addf63a6a3c52100ad6a25209610153282a2977fc8234b019e7bfa4b8`  
		Last Modified: Thu, 07 Sep 2023 01:28:14 GMT  
		Size: 1.5 KB (1480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a4df5368a1108e415af1adad06e9925df044775278212b278f40db0c9e828b6`  
		Last Modified: Thu, 07 Sep 2023 01:28:15 GMT  
		Size: 1.4 MB (1385578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d8fa422b756819743a45bc63685472b1df2c01002596e8beb4231c6f1235f34`  
		Last Modified: Thu, 07 Sep 2023 01:28:14 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `adminer:fastcgi`

```console
$ docker pull adminer@sha256:ddd5815490957bfdfce22db1504bb2ac9a5d3959d8c8f05ba9048d9d60029b85
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
$ docker pull adminer@sha256:15659f7db1e32df8ee184ace61ba9c86663fe995dcc68b5bee681676cd65c86d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.9 MB (95940089 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:88b4d4658217a7fbd5718733b47cfdfcd835cba81366d47a5edc8516a640bd9f`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Thu, 07 Sep 2023 00:21:01 GMT
ADD file:144dff349a666134b5e98a9f1c6650fd9d6e4a88a6f98857f26eb84989360b91 in / 
# Thu, 07 Sep 2023 00:21:02 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 03:10:23 GMT
STOPSIGNAL SIGINT
# Thu, 07 Sep 2023 03:10:44 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 03:10:45 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Thu, 07 Sep 2023 03:11:05 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Thu, 07 Sep 2023 03:11:05 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 07 Sep 2023 03:11:05 GMT
WORKDIR /var/www/html
# Thu, 07 Sep 2023 03:11:06 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 07 Sep 2023 03:11:06 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 07 Sep 2023 03:11:06 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 07 Sep 2023 03:11:06 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 07 Sep 2023 03:11:16 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 07 Sep 2023 03:11:16 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 07 Sep 2023 03:11:16 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 07 Sep 2023 03:11:17 GMT
USER adminer
# Thu, 07 Sep 2023 03:11:17 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:5dea071bb9782209397443f024a630052ab7583e365894d414f1e39cd0f65025`  
		Last Modified: Thu, 07 Sep 2023 00:25:41 GMT  
		Size: 55.1 MB (55056245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d84864d5d25a2386de4d3f48de320a52febc28bb28cb742aba6d777c4128696`  
		Last Modified: Thu, 07 Sep 2023 03:11:37 GMT  
		Size: 39.5 MB (39491426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:792bf43687eb38330b06a085a88b6c0505837ae192ac0fe027f7a07215f853a6`  
		Last Modified: Thu, 07 Sep 2023 03:11:29 GMT  
		Size: 395.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e01de01b95b38bf91fd08d70ff82b982b8dca2110bf77448cea418e95e126d9a`  
		Last Modified: Thu, 07 Sep 2023 03:11:54 GMT  
		Size: 2.7 KB (2712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15e0eed8de828090b43d0bbdb0fe4d095f18b39bea0ba03bdde09742311c98e2`  
		Last Modified: Thu, 07 Sep 2023 03:11:54 GMT  
		Size: 1.9 KB (1880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:871d9ee2bd875b8e07cda014c321142ca148c41385ad50db557708d53aeed910`  
		Last Modified: Thu, 07 Sep 2023 03:11:54 GMT  
		Size: 1.5 KB (1480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ea47c50e3a334983865aa3a1ac8269133885d8dc06e6bd3adfbdb41cb6b08c6`  
		Last Modified: Thu, 07 Sep 2023 03:11:55 GMT  
		Size: 1.4 MB (1385463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9fee1469c7254200561d4b1b94f32fc0485731de2477b06e6df7013098f6c7b`  
		Last Modified: Thu, 07 Sep 2023 03:11:54 GMT  
		Size: 488.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:fastcgi` - linux; arm variant v5

```console
$ docker pull adminer@sha256:68a8a35328fd756b490e1ee7bfe37451f377151d253bf2a13b8132dec21e0ce0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.2 MB (91197773 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ac4abb044959ec9100e2123e544a8bb1c39a3e7299cb2b54f30345e746092ce`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Thu, 07 Sep 2023 00:48:38 GMT
ADD file:bad04cab9856def18134a0c7925a5f43816c14da597964b6d5567abc3ef6a8b9 in / 
# Thu, 07 Sep 2023 00:48:39 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 05:57:06 GMT
STOPSIGNAL SIGINT
# Thu, 07 Sep 2023 05:57:39 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 05:57:40 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Thu, 07 Sep 2023 05:58:04 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Thu, 07 Sep 2023 05:58:05 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 07 Sep 2023 05:58:05 GMT
WORKDIR /var/www/html
# Thu, 07 Sep 2023 05:58:05 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 07 Sep 2023 05:58:05 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 07 Sep 2023 05:58:05 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 07 Sep 2023 05:58:05 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 07 Sep 2023 05:58:18 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 07 Sep 2023 05:58:18 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 07 Sep 2023 05:58:18 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 07 Sep 2023 05:58:18 GMT
USER adminer
# Thu, 07 Sep 2023 05:58:18 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:c77da54c1e584356232e8207afbbe30938a9c2dda2ebc314c1d66e34c74245cc`  
		Last Modified: Thu, 07 Sep 2023 00:51:56 GMT  
		Size: 52.6 MB (52557684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f9ecd2f984b7ccbad8542193859188aa41052ff9a7f1b62ad82ac8bd8a4dc94`  
		Last Modified: Thu, 07 Sep 2023 05:58:40 GMT  
		Size: 37.2 MB (37247813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74f16b90817746d2df9ca8097b34f1a2a58ddea40f9d13b7661801e9d0cabeb6`  
		Last Modified: Thu, 07 Sep 2023 05:58:32 GMT  
		Size: 392.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19291db959f5743b3fc9e761a855018f488f61c2f70012d7a14fb1319d0d61f3`  
		Last Modified: Thu, 07 Sep 2023 05:58:57 GMT  
		Size: 2.7 KB (2713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04fa7bdce9b8e241d877c81cd956b30e00826a78a5513355c03646ecab5c6a09`  
		Last Modified: Thu, 07 Sep 2023 05:58:57 GMT  
		Size: 1.9 KB (1869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0867e050c3c0c3917ee2ff18cf6b6becb88fe6053803081900c3382331506c8`  
		Last Modified: Thu, 07 Sep 2023 05:58:57 GMT  
		Size: 1.5 KB (1480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c35adb51769011f110acbf0514bab08249bcf812b1da24327bed43b4eb11ba2`  
		Last Modified: Thu, 07 Sep 2023 05:58:58 GMT  
		Size: 1.4 MB (1385331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:254cd97ad98c8e7fb70fe19de389cf9b2863df4d23f3885d54fd68242293a387`  
		Last Modified: Thu, 07 Sep 2023 05:58:57 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:fastcgi` - linux; arm variant v7

```console
$ docker pull adminer@sha256:a0d499c047e84848247c5a877bd3c4064625f4a64495f89e1ad95093fce1ac3f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.8 MB (87798646 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33f2770b6fe2af3a75e07d84e1b363bad6515ceb1b6972d4d9902323283d0694`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Thu, 07 Sep 2023 00:57:59 GMT
ADD file:931564fb3c8ea78b763a6b98f2739bb7c6a38484122c560a87c7166b7d45c5e6 in / 
# Thu, 07 Sep 2023 00:58:00 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 01:50:52 GMT
STOPSIGNAL SIGINT
# Thu, 07 Sep 2023 01:51:32 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 01:51:33 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Thu, 07 Sep 2023 01:52:01 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Thu, 07 Sep 2023 01:52:02 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 07 Sep 2023 01:52:02 GMT
WORKDIR /var/www/html
# Thu, 07 Sep 2023 01:52:02 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 07 Sep 2023 01:52:02 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 07 Sep 2023 01:52:02 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 07 Sep 2023 01:52:02 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 07 Sep 2023 01:52:14 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 07 Sep 2023 01:52:14 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 07 Sep 2023 01:52:14 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 07 Sep 2023 01:52:14 GMT
USER adminer
# Thu, 07 Sep 2023 01:52:15 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:5826e0d927336e7231f9d05ec48f075045fb51f9b3f16f1e20972f2a3634d102`  
		Last Modified: Thu, 07 Sep 2023 01:02:50 GMT  
		Size: 50.2 MB (50219233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64126d7f6d5bc4ca6d42b71dc00598c67b9f6f17d6919fcce1f03a613722e16d`  
		Last Modified: Thu, 07 Sep 2023 01:52:33 GMT  
		Size: 36.2 MB (36187001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fd3d57a54c1b1fa49ef5fdece23637a20b7f8e985a804fc2c5135f097a549bb`  
		Last Modified: Thu, 07 Sep 2023 01:52:25 GMT  
		Size: 393.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21903f65656bc64fb0c6609085b2d6702f7968442e7354cf234741fc68c2f5f4`  
		Last Modified: Thu, 07 Sep 2023 01:52:51 GMT  
		Size: 2.7 KB (2711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0113ab9766972272a3d4c016308b4e1e22c504b634d6941e6b9c059cad5b3d45`  
		Last Modified: Thu, 07 Sep 2023 01:52:51 GMT  
		Size: 1.9 KB (1871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d992cf32eddb4dbb575f70c5b565ee0fb23d47953ed8292e06ac9555ddeeb123`  
		Last Modified: Thu, 07 Sep 2023 01:52:52 GMT  
		Size: 1.5 KB (1480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47b5e7c51aefa173a76e0fa25e50964e84f858eba6e8225bb1f29ee18d6062b0`  
		Last Modified: Thu, 07 Sep 2023 01:52:52 GMT  
		Size: 1.4 MB (1385466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c65e533099f9039fa0e0df43fda417b7954478ea6aa401dedf1ee822938b5b7e`  
		Last Modified: Thu, 07 Sep 2023 01:52:51 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:fastcgi` - linux; arm64 variant v8

```console
$ docker pull adminer@sha256:a38ecc5faf0a8576b1bdd76c2f602a86daa9b6cd71b16633fb7ce005ef32bd8d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.3 MB (94341386 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a500c1c0d44c969c688bca9ba88bcb562155d2c6dace06dbe71086fdbdb6fb82`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Thu, 07 Sep 2023 00:39:45 GMT
ADD file:6bc001e951ef1280f566a92e65fcff57aefb8a280aa3510b7cd4b4e0a54c5cff in / 
# Thu, 07 Sep 2023 00:39:46 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 02:22:22 GMT
STOPSIGNAL SIGINT
# Thu, 07 Sep 2023 02:22:41 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 02:22:42 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Thu, 07 Sep 2023 02:23:02 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Thu, 07 Sep 2023 02:23:03 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 07 Sep 2023 02:23:03 GMT
WORKDIR /var/www/html
# Thu, 07 Sep 2023 02:23:03 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 07 Sep 2023 02:23:03 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 07 Sep 2023 02:23:03 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 07 Sep 2023 02:23:03 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 07 Sep 2023 02:23:13 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 07 Sep 2023 02:23:13 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 07 Sep 2023 02:23:13 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 07 Sep 2023 02:23:13 GMT
USER adminer
# Thu, 07 Sep 2023 02:23:13 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:61c16b7975697b00760ff9536c09eed29b6a76923d4d98be38e9cdc749506417`  
		Last Modified: Thu, 07 Sep 2023 00:43:21 GMT  
		Size: 53.7 MB (53704716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81f75bf1a78b692b687a603db539e512b761e91500113ab03d603be6cd108610`  
		Last Modified: Thu, 07 Sep 2023 02:23:31 GMT  
		Size: 39.2 MB (39244334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f3afc31326ca8d485c99b99322b549a89dd0db30062feaba0986df541301b45`  
		Last Modified: Thu, 07 Sep 2023 02:23:23 GMT  
		Size: 385.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efb65c5d18143c713fb41d912e5eb0419de652c480d7db9d798886f092df48a7`  
		Last Modified: Thu, 07 Sep 2023 02:23:47 GMT  
		Size: 2.7 KB (2709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f811d6324927c972ba66211edfdf8f3c83f50e55193712a29387b3787210591d`  
		Last Modified: Thu, 07 Sep 2023 02:23:47 GMT  
		Size: 1.9 KB (1883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e0bd6ef968ad02351f0b7c15001f9016c5be9aabf3c89e45d5d1347c663b6fa`  
		Last Modified: Thu, 07 Sep 2023 02:23:47 GMT  
		Size: 1.5 KB (1477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b21fc274312e94dc7ca9579a44d64426c71ea39388a81328c0a00f3bfc7a0ada`  
		Last Modified: Thu, 07 Sep 2023 02:23:47 GMT  
		Size: 1.4 MB (1385391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0360824626289cffd506daf3a7e018ae732cad6b53e2e81b212e909ebc93627e`  
		Last Modified: Thu, 07 Sep 2023 02:23:47 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:fastcgi` - linux; 386

```console
$ docker pull adminer@sha256:31005a66635aeb5741283bd8581f35dcc3418b74a8a92ecb7304893afeca9f3a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.0 MB (96991141 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c685db3c051c046189a4226ab8d58d2f036bc689989be2293960dd2b305b1c7`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Tue, 15 Aug 2023 23:39:11 GMT
ADD file:efc88a19b31e68ca41f555bcc51338b0f135cbbd72b90637d8c73969d53addd2 in / 
# Tue, 15 Aug 2023 23:39:12 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 00:23:36 GMT
STOPSIGNAL SIGINT
# Wed, 16 Aug 2023 00:24:03 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 00:24:04 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 16 Aug 2023 00:24:25 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Wed, 16 Aug 2023 00:24:25 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 16 Aug 2023 00:24:25 GMT
WORKDIR /var/www/html
# Wed, 16 Aug 2023 00:24:25 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 16 Aug 2023 00:24:26 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 16 Aug 2023 00:24:26 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 16 Aug 2023 00:24:26 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 16 Aug 2023 00:24:38 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 16 Aug 2023 00:24:38 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 16 Aug 2023 00:24:38 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 16 Aug 2023 00:24:38 GMT
USER adminer
# Wed, 16 Aug 2023 00:24:38 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:822e033fa7b169545d5890de01438a9dd87774ff938ff440e823a3ec3f73996d`  
		Last Modified: Tue, 15 Aug 2023 23:43:47 GMT  
		Size: 56.0 MB (56040520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7644269f7e699d335219a554e561f3817b7816e99351232b3646176246991895`  
		Last Modified: Wed, 16 Aug 2023 00:25:00 GMT  
		Size: 39.6 MB (39558428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d96338ff936c667ce1c89a75f7fd111e722685d882b1f36e7b26dcb33007029`  
		Last Modified: Wed, 16 Aug 2023 00:24:50 GMT  
		Size: 389.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:585dca01c1d637ee0076501f08e4c8dd8b467af8006ff57516ecb5cdd3de7a10`  
		Last Modified: Wed, 16 Aug 2023 00:25:17 GMT  
		Size: 2.7 KB (2711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8603b649d501de6381c6c255466548d9b5757633061fc51a99a8ae09461ba36f`  
		Last Modified: Wed, 16 Aug 2023 00:25:17 GMT  
		Size: 1.9 KB (1867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:123b0bf5a630ef1b094c6d6b927c1948125a80dd610422620ba4fdb36cc7e28d`  
		Last Modified: Wed, 16 Aug 2023 00:25:17 GMT  
		Size: 1.5 KB (1474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f5f2c7c1669f07ae595648970fde7e0a45018fea7e85e22f8e6db2215dd3caf`  
		Last Modified: Wed, 16 Aug 2023 00:25:18 GMT  
		Size: 1.4 MB (1385259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:619532a1fade63f393a4d4769b6eed50956558d2b6edaaaf7f026ec2c987f661`  
		Last Modified: Wed, 16 Aug 2023 00:25:17 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:fastcgi` - linux; mips64le

```console
$ docker pull adminer@sha256:2c3b4d978627105affcd060a2a4602bb97f1fd90187edd5cb30b338b22584e15
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.6 MB (92615139 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c2be39d77614a37ab8c0c9448232e1be6fb18fca8a2696bdb76f7ba90b69578`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Thu, 07 Sep 2023 01:09:47 GMT
ADD file:fdd438b39f1dce564715691d2a092378f02bc722e29cb80216efcbaf71cff0b8 in / 
# Thu, 07 Sep 2023 01:09:53 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 03:08:04 GMT
STOPSIGNAL SIGINT
# Thu, 07 Sep 2023 03:10:03 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 03:10:09 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Thu, 07 Sep 2023 03:12:06 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Thu, 07 Sep 2023 03:12:13 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 07 Sep 2023 03:12:16 GMT
WORKDIR /var/www/html
# Thu, 07 Sep 2023 03:12:19 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 07 Sep 2023 03:12:22 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 07 Sep 2023 03:12:26 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 07 Sep 2023 03:12:29 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 07 Sep 2023 03:13:20 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 07 Sep 2023 03:13:23 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 07 Sep 2023 03:13:27 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 07 Sep 2023 03:13:30 GMT
USER adminer
# Thu, 07 Sep 2023 03:13:34 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:0d1f1f4ccb1e0da4313c3ebcd521e7fa8073526c6f64ca7214ed31ae9bd0788e`  
		Last Modified: Thu, 07 Sep 2023 01:21:00 GMT  
		Size: 53.3 MB (53271469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b724451ca3bae07bf7da51b1c949189dc86f1e494be2830616fbe3cf4c7a447`  
		Last Modified: Thu, 07 Sep 2023 03:14:20 GMT  
		Size: 38.0 MB (37950499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:915c5f7e479b8d1cb1baf57fd9f07e06b962433d3a40fc832491c6f6614522bb`  
		Last Modified: Thu, 07 Sep 2023 03:13:55 GMT  
		Size: 394.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c089a408ed63eef86310ec1d3db9d84aa46d7f541e3ec1e90a4798aa6545d436`  
		Last Modified: Thu, 07 Sep 2023 03:14:41 GMT  
		Size: 2.7 KB (2713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56bb790d23ceab0acafe02823b5726a9a99319fc3ce2e215cbbc11d2e5b57a60`  
		Last Modified: Thu, 07 Sep 2023 03:14:41 GMT  
		Size: 1.7 KB (1725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c5b3c385bb7fe02cc10cefc1cc9bfd8a7c41d4d908b07bef77f7f7c0308086a`  
		Last Modified: Thu, 07 Sep 2023 03:14:41 GMT  
		Size: 1.5 KB (1479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ae8742bfc11fac37d1a8257111b0cdde75cd0c7d628fe1c99a1767583510d4f`  
		Last Modified: Thu, 07 Sep 2023 03:14:42 GMT  
		Size: 1.4 MB (1386368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd25dbfd1a8ef46f40a314361de018304317b3f157bf58c376b23d42d53e9f5a`  
		Last Modified: Thu, 07 Sep 2023 03:14:41 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:fastcgi` - linux; ppc64le

```console
$ docker pull adminer@sha256:b7224d5a014ff9f27bb1a4b1aff7ed321765e5f8ec175d34613ccdef6e2da361
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.3 MB (101265147 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70f1927913fd3d1b839c87d619e0d41128e9ac696c2e77895368025a38cdb9c0`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Thu, 07 Sep 2023 00:17:47 GMT
ADD file:da42a2ef7aa1ce7e6df281b469ac67db062d14c59066a6dfd7ac5cc91d7a3b8c in / 
# Thu, 07 Sep 2023 00:17:50 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 09:04:15 GMT
STOPSIGNAL SIGINT
# Thu, 07 Sep 2023 09:07:04 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 09:07:10 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Thu, 07 Sep 2023 09:08:56 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Thu, 07 Sep 2023 09:09:03 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 07 Sep 2023 09:09:06 GMT
WORKDIR /var/www/html
# Thu, 07 Sep 2023 09:09:06 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 07 Sep 2023 09:09:08 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 07 Sep 2023 09:09:09 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 07 Sep 2023 09:09:10 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 07 Sep 2023 09:10:21 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 07 Sep 2023 09:10:25 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 07 Sep 2023 09:10:33 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 07 Sep 2023 09:10:40 GMT
USER adminer
# Thu, 07 Sep 2023 09:10:52 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:fb3cfd509d4c62da47ee9c7eee6545472d58ceaab6fcd454a82d188766dd0c45`  
		Last Modified: Thu, 07 Sep 2023 00:23:55 GMT  
		Size: 58.9 MB (58928091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bffc3bba24bd4cd45431ae9c166638ec8595b5ecab4200290f8c176a1212b7c`  
		Last Modified: Thu, 07 Sep 2023 09:11:25 GMT  
		Size: 40.9 MB (40944217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d37dbbfa36efc1b986a9571f61c675f6dd3304c8b0f8ea6ce287be3e977d1976`  
		Last Modified: Thu, 07 Sep 2023 09:11:12 GMT  
		Size: 398.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6805ebe3dfb3654d46f5fc9a8cd6a74c2a86ade728959b1dfa0739f99c1b5428`  
		Last Modified: Thu, 07 Sep 2023 09:11:45 GMT  
		Size: 2.7 KB (2714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70c512e9728df1edeb0e0315c69e85528520cf302979f8f6ade2fca0b27185b5`  
		Last Modified: Thu, 07 Sep 2023 09:11:45 GMT  
		Size: 1.9 KB (1876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11e2e6a603583abf7085bdbf1f879974415c61c29c08962f4b96fb4fe3ce981d`  
		Last Modified: Thu, 07 Sep 2023 09:11:45 GMT  
		Size: 1.5 KB (1478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d971487f8cbfeaa9c06033dcafc7e63fa3556563916948e905fc7c62b4126c8b`  
		Last Modified: Thu, 07 Sep 2023 09:11:46 GMT  
		Size: 1.4 MB (1385882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbc9d316bb2a490069e9c690d1f2e1e73e0765b2cfa7fab34108868e6756e9a3`  
		Last Modified: Thu, 07 Sep 2023 09:11:45 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:fastcgi` - linux; s390x

```console
$ docker pull adminer@sha256:de471294d28d5750d41244ba8d44db2cb1aaab848922985f660b02eabbd197dc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.7 MB (93703439 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cde1549e5993997b294699895499c6549c361bd95ebd374a3c85442fd76eb165`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Thu, 07 Sep 2023 00:44:03 GMT
ADD file:a0582e191d0265b98e5d46c64ba9b4c46445cfa821c6e41d32db343b0e2a6fec in / 
# Thu, 07 Sep 2023 00:44:12 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 01:26:26 GMT
STOPSIGNAL SIGINT
# Thu, 07 Sep 2023 01:27:02 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 01:27:07 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Thu, 07 Sep 2023 01:27:36 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Thu, 07 Sep 2023 01:27:37 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 07 Sep 2023 01:27:38 GMT
WORKDIR /var/www/html
# Thu, 07 Sep 2023 01:27:38 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 07 Sep 2023 01:27:38 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 07 Sep 2023 01:27:38 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 07 Sep 2023 01:27:39 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 07 Sep 2023 01:27:53 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 07 Sep 2023 01:27:54 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 07 Sep 2023 01:27:54 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 07 Sep 2023 01:27:55 GMT
USER adminer
# Thu, 07 Sep 2023 01:27:55 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:6dd2d41f67a6666210e1a34694b8765e945a44014b53252ec0e1b50491e08d69`  
		Last Modified: Thu, 07 Sep 2023 00:49:54 GMT  
		Size: 53.3 MB (53290217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe4a876b44eaaf1ba3c702ea08a6af25e23abb30b7fcbef9b957a4c34ec5ad73`  
		Last Modified: Thu, 07 Sep 2023 01:28:21 GMT  
		Size: 39.0 MB (39020691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:529f8a0ebc99b919f45c296bfffe1d9aa35136c91542e626681a898a1e1dabb2`  
		Last Modified: Thu, 07 Sep 2023 01:28:14 GMT  
		Size: 393.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e241b68ed72809f13265cadec141405091d29c51cc7031a53fb1ac63e98370e4`  
		Last Modified: Thu, 07 Sep 2023 01:28:34 GMT  
		Size: 2.7 KB (2714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c554ebc3fa08021199bd77796a742b7ec9a23e27c9f301efd186c67355e26ea3`  
		Last Modified: Thu, 07 Sep 2023 01:28:34 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6ddeb9921e2ece9eabbc65206020cfc9fb9c53ebb491a85b96d5eb7ed308c6e`  
		Last Modified: Thu, 07 Sep 2023 01:28:34 GMT  
		Size: 1.5 KB (1481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5c07f366229478ef4b2de990c4de70ab31aa0982284cc7b192581b9c8e765eb`  
		Last Modified: Thu, 07 Sep 2023 01:28:34 GMT  
		Size: 1.4 MB (1385571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6878b99b931b3ddc6e0ae8ba87b925151a30fbb1ade42882571d878a53316bb0`  
		Last Modified: Thu, 07 Sep 2023 01:28:34 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `adminer:latest`

```console
$ docker pull adminer@sha256:a607d96fbf114fefcdd34729b84a6cd379dedb3ead294c56f0f318f9981fb52a
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
$ docker pull adminer@sha256:5463cc7e5a3e4ad51aa0e98c419d04646fd9b3e14a1d960ab8b420b9ce9ecc80
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.9 MB (95937329 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1bb4da606dc1a8721442935ae417a1ff7d27b9eea6ef228797780679d81ba0b6`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Thu, 07 Sep 2023 00:21:01 GMT
ADD file:144dff349a666134b5e98a9f1c6650fd9d6e4a88a6f98857f26eb84989360b91 in / 
# Thu, 07 Sep 2023 00:21:02 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 03:10:23 GMT
STOPSIGNAL SIGINT
# Thu, 07 Sep 2023 03:10:44 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 03:10:45 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Thu, 07 Sep 2023 03:10:46 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 07 Sep 2023 03:10:46 GMT
WORKDIR /var/www/html
# Thu, 07 Sep 2023 03:10:46 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 07 Sep 2023 03:10:46 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 07 Sep 2023 03:10:46 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 07 Sep 2023 03:10:46 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 07 Sep 2023 03:10:58 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 07 Sep 2023 03:10:58 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 07 Sep 2023 03:10:58 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 07 Sep 2023 03:10:58 GMT
USER adminer
# Thu, 07 Sep 2023 03:10:58 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Thu, 07 Sep 2023 03:10:58 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:5dea071bb9782209397443f024a630052ab7583e365894d414f1e39cd0f65025`  
		Last Modified: Thu, 07 Sep 2023 00:25:41 GMT  
		Size: 55.1 MB (55056245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d84864d5d25a2386de4d3f48de320a52febc28bb28cb742aba6d777c4128696`  
		Last Modified: Thu, 07 Sep 2023 03:11:37 GMT  
		Size: 39.5 MB (39491426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:792bf43687eb38330b06a085a88b6c0505837ae192ac0fe027f7a07215f853a6`  
		Last Modified: Thu, 07 Sep 2023 03:11:29 GMT  
		Size: 395.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37ef5d260982b8b88f34270bbe7314228f686ac4bbbea7e647ab96feaf464e71`  
		Last Modified: Thu, 07 Sep 2023 03:11:29 GMT  
		Size: 1.9 KB (1879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81b9b963ca6d8427a310df0283abe6c6ef185569bb470cf8a0525da60989ecb6`  
		Last Modified: Thu, 07 Sep 2023 03:11:29 GMT  
		Size: 1.5 KB (1480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e57581023c92f337603ebe93de3ebca9a7eeb11706fdccc3f1b359714e0b65a6`  
		Last Modified: Thu, 07 Sep 2023 03:11:30 GMT  
		Size: 1.4 MB (1385412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e97ed40bb1db1cf97113d360f1b14422117cf4154eba611c2d2849d66958ecaa`  
		Last Modified: Thu, 07 Sep 2023 03:11:29 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:latest` - linux; arm variant v5

```console
$ docker pull adminer@sha256:dfd42b21fcc7d95faa4380a9bf051771e3bb79badd52e1005a8cbe551c64b6b4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.2 MB (91195063 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd44c48956465a566c168988d7201c27647c33ae7344305a32cd56f85cd46734`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Thu, 07 Sep 2023 00:48:38 GMT
ADD file:bad04cab9856def18134a0c7925a5f43816c14da597964b6d5567abc3ef6a8b9 in / 
# Thu, 07 Sep 2023 00:48:39 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 05:57:06 GMT
STOPSIGNAL SIGINT
# Thu, 07 Sep 2023 05:57:39 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 05:57:40 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Thu, 07 Sep 2023 05:57:41 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 07 Sep 2023 05:57:41 GMT
WORKDIR /var/www/html
# Thu, 07 Sep 2023 05:57:41 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 07 Sep 2023 05:57:41 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 07 Sep 2023 05:57:41 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 07 Sep 2023 05:57:41 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 07 Sep 2023 05:57:57 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 07 Sep 2023 05:57:57 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 07 Sep 2023 05:57:57 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 07 Sep 2023 05:57:57 GMT
USER adminer
# Thu, 07 Sep 2023 05:57:57 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Thu, 07 Sep 2023 05:57:57 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:c77da54c1e584356232e8207afbbe30938a9c2dda2ebc314c1d66e34c74245cc`  
		Last Modified: Thu, 07 Sep 2023 00:51:56 GMT  
		Size: 52.6 MB (52557684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f9ecd2f984b7ccbad8542193859188aa41052ff9a7f1b62ad82ac8bd8a4dc94`  
		Last Modified: Thu, 07 Sep 2023 05:58:40 GMT  
		Size: 37.2 MB (37247813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74f16b90817746d2df9ca8097b34f1a2a58ddea40f9d13b7661801e9d0cabeb6`  
		Last Modified: Thu, 07 Sep 2023 05:58:32 GMT  
		Size: 392.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2db198a220919fae8fc5093acd186481fdccff4b56654baf5ad81f5b16179f41`  
		Last Modified: Thu, 07 Sep 2023 05:58:31 GMT  
		Size: 1.9 KB (1869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bb71f0a31aaaedd68c31d3bd627d15c9a80f1fc8c77d787ae08509cea144944`  
		Last Modified: Thu, 07 Sep 2023 05:58:31 GMT  
		Size: 1.5 KB (1481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7345eee73a7d870b5e002cbc1ab741e76326b7bcedc039de45d03075a08f8bb5`  
		Last Modified: Thu, 07 Sep 2023 05:58:32 GMT  
		Size: 1.4 MB (1385331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d24fe8d24625441b6f9992c49257519dcd2a6962d677d2c96d6de6f440f16d9a`  
		Last Modified: Thu, 07 Sep 2023 05:58:31 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:latest` - linux; arm variant v7

```console
$ docker pull adminer@sha256:dde88e85f022908e040ce9f5627e989fca6cf4f796fb912e216bc91e85b80e9f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.8 MB (87795922 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1de3886b83d0afcea5f67dd340efd76d0ff0d7cc5d4d765d7ac24bdce5ac766`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Thu, 07 Sep 2023 00:57:59 GMT
ADD file:931564fb3c8ea78b763a6b98f2739bb7c6a38484122c560a87c7166b7d45c5e6 in / 
# Thu, 07 Sep 2023 00:58:00 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 01:50:52 GMT
STOPSIGNAL SIGINT
# Thu, 07 Sep 2023 01:51:32 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 01:51:33 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Thu, 07 Sep 2023 01:51:34 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 07 Sep 2023 01:51:34 GMT
WORKDIR /var/www/html
# Thu, 07 Sep 2023 01:51:34 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 07 Sep 2023 01:51:34 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 07 Sep 2023 01:51:34 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 07 Sep 2023 01:51:34 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 07 Sep 2023 01:51:48 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 07 Sep 2023 01:51:48 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 07 Sep 2023 01:51:48 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 07 Sep 2023 01:51:48 GMT
USER adminer
# Thu, 07 Sep 2023 01:51:48 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Thu, 07 Sep 2023 01:51:48 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:5826e0d927336e7231f9d05ec48f075045fb51f9b3f16f1e20972f2a3634d102`  
		Last Modified: Thu, 07 Sep 2023 01:02:50 GMT  
		Size: 50.2 MB (50219233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64126d7f6d5bc4ca6d42b71dc00598c67b9f6f17d6919fcce1f03a613722e16d`  
		Last Modified: Thu, 07 Sep 2023 01:52:33 GMT  
		Size: 36.2 MB (36187001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fd3d57a54c1b1fa49ef5fdece23637a20b7f8e985a804fc2c5135f097a549bb`  
		Last Modified: Thu, 07 Sep 2023 01:52:25 GMT  
		Size: 393.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2440750817c8e724091323e3903329ccc274561f1f1e61c49d9da560960899bb`  
		Last Modified: Thu, 07 Sep 2023 01:52:25 GMT  
		Size: 1.9 KB (1869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c56be7ee3fb4f5d4eec7601e51e91b41bf76a5ead2b87c1026930214ba51c2b8`  
		Last Modified: Thu, 07 Sep 2023 01:52:25 GMT  
		Size: 1.5 KB (1481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22e56804b3ad37bd9f7ff556ddf336fe3b2ed8503cb32b0dfee800e4c76d9451`  
		Last Modified: Thu, 07 Sep 2023 01:52:25 GMT  
		Size: 1.4 MB (1385452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:288264a2552805e7baa2b8233fa1aad54720bdba711d9147660fe31f59cc2f32`  
		Last Modified: Thu, 07 Sep 2023 01:52:25 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:latest` - linux; arm64 variant v8

```console
$ docker pull adminer@sha256:3b35134d84f9bb500b4ea3b9e5998209f9e587ef94982ee30e6357ae9f30d7c8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.3 MB (94338646 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6f05a6588020fe9fe371405a1735a4614daa30b4e299bd24afa4d2a017d0fa2`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Thu, 07 Sep 2023 00:39:45 GMT
ADD file:6bc001e951ef1280f566a92e65fcff57aefb8a280aa3510b7cd4b4e0a54c5cff in / 
# Thu, 07 Sep 2023 00:39:46 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 02:22:22 GMT
STOPSIGNAL SIGINT
# Thu, 07 Sep 2023 02:22:41 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 02:22:42 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Thu, 07 Sep 2023 02:22:42 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 07 Sep 2023 02:22:43 GMT
WORKDIR /var/www/html
# Thu, 07 Sep 2023 02:22:43 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 07 Sep 2023 02:22:43 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 07 Sep 2023 02:22:43 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 07 Sep 2023 02:22:43 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 07 Sep 2023 02:22:53 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 07 Sep 2023 02:22:53 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 07 Sep 2023 02:22:54 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 07 Sep 2023 02:22:54 GMT
USER adminer
# Thu, 07 Sep 2023 02:22:54 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Thu, 07 Sep 2023 02:22:54 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:61c16b7975697b00760ff9536c09eed29b6a76923d4d98be38e9cdc749506417`  
		Last Modified: Thu, 07 Sep 2023 00:43:21 GMT  
		Size: 53.7 MB (53704716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81f75bf1a78b692b687a603db539e512b761e91500113ab03d603be6cd108610`  
		Last Modified: Thu, 07 Sep 2023 02:23:31 GMT  
		Size: 39.2 MB (39244334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f3afc31326ca8d485c99b99322b549a89dd0db30062feaba0986df541301b45`  
		Last Modified: Thu, 07 Sep 2023 02:23:23 GMT  
		Size: 385.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c635f2e362703c71ad0c137ad3994b892ba8f342bd446e64f80d66d9c7c6965`  
		Last Modified: Thu, 07 Sep 2023 02:23:23 GMT  
		Size: 1.9 KB (1880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed650e87b8c0a626a5474dfdb12657fbf231ce26d8aef7302216b8b36e6c89f3`  
		Last Modified: Thu, 07 Sep 2023 02:23:24 GMT  
		Size: 1.5 KB (1481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e277a4a1ba7b301b2528764da6494b52a7e34668a0758bb6a9d5d0cb9ba10806`  
		Last Modified: Thu, 07 Sep 2023 02:23:24 GMT  
		Size: 1.4 MB (1385360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eea59163ae0d170091fc6d9eca39c3f6b9a6adaabf7b2a4cf5ecdd03cf72409c`  
		Last Modified: Thu, 07 Sep 2023 02:23:24 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:latest` - linux; 386

```console
$ docker pull adminer@sha256:664fc6a11ece4d60a18492c17eeb4ffffb3d6fe19d3c4f4c4c3cab52b83f3ec6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.0 MB (96988434 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d7ecc3592e5ee3a2de07572724acd9167630fa736fd16b373959b3f5e2297736`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Tue, 15 Aug 2023 23:39:11 GMT
ADD file:efc88a19b31e68ca41f555bcc51338b0f135cbbd72b90637d8c73969d53addd2 in / 
# Tue, 15 Aug 2023 23:39:12 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 00:23:36 GMT
STOPSIGNAL SIGINT
# Wed, 16 Aug 2023 00:24:03 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 00:24:04 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 16 Aug 2023 00:24:05 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 16 Aug 2023 00:24:05 GMT
WORKDIR /var/www/html
# Wed, 16 Aug 2023 00:24:05 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 16 Aug 2023 00:24:05 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 16 Aug 2023 00:24:05 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 16 Aug 2023 00:24:05 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 16 Aug 2023 00:24:19 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 16 Aug 2023 00:24:19 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 16 Aug 2023 00:24:19 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 16 Aug 2023 00:24:19 GMT
USER adminer
# Wed, 16 Aug 2023 00:24:19 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 16 Aug 2023 00:24:19 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:822e033fa7b169545d5890de01438a9dd87774ff938ff440e823a3ec3f73996d`  
		Last Modified: Tue, 15 Aug 2023 23:43:47 GMT  
		Size: 56.0 MB (56040520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7644269f7e699d335219a554e561f3817b7816e99351232b3646176246991895`  
		Last Modified: Wed, 16 Aug 2023 00:25:00 GMT  
		Size: 39.6 MB (39558428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d96338ff936c667ce1c89a75f7fd111e722685d882b1f36e7b26dcb33007029`  
		Last Modified: Wed, 16 Aug 2023 00:24:50 GMT  
		Size: 389.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5339c86a7bc7031718f83f0a9af19ad028c2fa751748057f9d97d9c94c5075f6`  
		Last Modified: Wed, 16 Aug 2023 00:24:50 GMT  
		Size: 1.9 KB (1868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cbd1ad590a03bbc3ee08a1c944135c7bf81b103067417f79cdb1f8d271b4472`  
		Last Modified: Wed, 16 Aug 2023 00:24:50 GMT  
		Size: 1.5 KB (1480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:225fb2c801a3d35820604ab9c5d6c19a65e18fca4c76dd468e7015b6cb7d5d6c`  
		Last Modified: Wed, 16 Aug 2023 00:24:50 GMT  
		Size: 1.4 MB (1385258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:367f82cd1a3d30bffd1420e0c950c92f859f903ad0b0711848862db96f363ff7`  
		Last Modified: Wed, 16 Aug 2023 00:24:50 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:latest` - linux; mips64le

```console
$ docker pull adminer@sha256:9cc962f9ae71f2c5b15623bc438ebb6d9a340e0ba8d278d98c031c39e1b5e407
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.6 MB (92612452 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c340fe4c80d84cb71a7948c0d3da3ae567112f144fa0d27c1320899c29a61f0`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Thu, 07 Sep 2023 01:09:47 GMT
ADD file:fdd438b39f1dce564715691d2a092378f02bc722e29cb80216efcbaf71cff0b8 in / 
# Thu, 07 Sep 2023 01:09:53 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 03:08:04 GMT
STOPSIGNAL SIGINT
# Thu, 07 Sep 2023 03:10:03 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 03:10:09 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Thu, 07 Sep 2023 03:10:16 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 07 Sep 2023 03:10:19 GMT
WORKDIR /var/www/html
# Thu, 07 Sep 2023 03:10:23 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 07 Sep 2023 03:10:26 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 07 Sep 2023 03:10:30 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 07 Sep 2023 03:10:33 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 07 Sep 2023 03:11:27 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 07 Sep 2023 03:11:30 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 07 Sep 2023 03:11:33 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 07 Sep 2023 03:11:36 GMT
USER adminer
# Thu, 07 Sep 2023 03:11:40 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Thu, 07 Sep 2023 03:11:43 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:0d1f1f4ccb1e0da4313c3ebcd521e7fa8073526c6f64ca7214ed31ae9bd0788e`  
		Last Modified: Thu, 07 Sep 2023 01:21:00 GMT  
		Size: 53.3 MB (53271469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b724451ca3bae07bf7da51b1c949189dc86f1e494be2830616fbe3cf4c7a447`  
		Last Modified: Thu, 07 Sep 2023 03:14:20 GMT  
		Size: 38.0 MB (37950499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:915c5f7e479b8d1cb1baf57fd9f07e06b962433d3a40fc832491c6f6614522bb`  
		Last Modified: Thu, 07 Sep 2023 03:13:55 GMT  
		Size: 394.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffcee722bb0f36a2975167c5ddf08d0da2cb56e72317f5f3e9d5cfbc3d4a4716`  
		Last Modified: Thu, 07 Sep 2023 03:13:54 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fc9ff6a8f7fb04dd6c3d6df59d01f1c9c7c34ad3cbe41553ecdff949bd20c1e`  
		Last Modified: Thu, 07 Sep 2023 03:13:54 GMT  
		Size: 1.5 KB (1482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cb2cbc2bc303d453e8e91cca3d170ccb3b27fd2bd03b89a3924e679e78c26e4`  
		Last Modified: Thu, 07 Sep 2023 03:13:55 GMT  
		Size: 1.4 MB (1386382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efe356c9d62e82baa2ebf75971c57e6fadf0e138988c966f6767875ff8843182`  
		Last Modified: Thu, 07 Sep 2023 03:13:54 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:latest` - linux; ppc64le

```console
$ docker pull adminer@sha256:af35710d0480902e87252a3b766b10d0f75285c0d22bafce974f049ed8128552
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.3 MB (101262505 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ec6c6c445d603cdb55b8e2df3d7ca3ab043dee3a4535b6dd28cd47284c99eed`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Thu, 07 Sep 2023 00:17:47 GMT
ADD file:da42a2ef7aa1ce7e6df281b469ac67db062d14c59066a6dfd7ac5cc91d7a3b8c in / 
# Thu, 07 Sep 2023 00:17:50 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 09:04:15 GMT
STOPSIGNAL SIGINT
# Thu, 07 Sep 2023 09:07:04 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 09:07:10 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Thu, 07 Sep 2023 09:07:13 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 07 Sep 2023 09:07:14 GMT
WORKDIR /var/www/html
# Thu, 07 Sep 2023 09:07:14 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 07 Sep 2023 09:07:15 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 07 Sep 2023 09:07:15 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 07 Sep 2023 09:07:16 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 07 Sep 2023 09:08:33 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 07 Sep 2023 09:08:33 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 07 Sep 2023 09:08:35 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 07 Sep 2023 09:08:36 GMT
USER adminer
# Thu, 07 Sep 2023 09:08:38 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Thu, 07 Sep 2023 09:08:39 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:fb3cfd509d4c62da47ee9c7eee6545472d58ceaab6fcd454a82d188766dd0c45`  
		Last Modified: Thu, 07 Sep 2023 00:23:55 GMT  
		Size: 58.9 MB (58928091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bffc3bba24bd4cd45431ae9c166638ec8595b5ecab4200290f8c176a1212b7c`  
		Last Modified: Thu, 07 Sep 2023 09:11:25 GMT  
		Size: 40.9 MB (40944217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d37dbbfa36efc1b986a9571f61c675f6dd3304c8b0f8ea6ce287be3e977d1976`  
		Last Modified: Thu, 07 Sep 2023 09:11:12 GMT  
		Size: 398.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:040ad87be7d0fd1ec4f721e5fd3acd35286b3f5dd90a2f50595443791d2c5f78`  
		Last Modified: Thu, 07 Sep 2023 09:11:12 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fde911bb7830da7a8226144a744f977069a6a35fc88a5f98301891261503ecf`  
		Last Modified: Thu, 07 Sep 2023 09:11:12 GMT  
		Size: 1.5 KB (1476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1ce36781194ed33448f80f0902704489627f8098ddd838fc8a41ca597ccbfab`  
		Last Modified: Thu, 07 Sep 2023 09:11:13 GMT  
		Size: 1.4 MB (1385951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d01192f86adad3c4b51a184a68865d082250b44614aa375d150dda8f5f36b927`  
		Last Modified: Thu, 07 Sep 2023 09:11:12 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:latest` - linux; s390x

```console
$ docker pull adminer@sha256:b3028b06f7c78024603ab547558cf83d4fe518c6bfd10a107ee923081d45c3a6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.7 MB (93700732 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40878d5b42fdc65d89e9d563be958aad831592c92455633ce54a025dc6bac4eb`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Thu, 07 Sep 2023 00:44:03 GMT
ADD file:a0582e191d0265b98e5d46c64ba9b4c46445cfa821c6e41d32db343b0e2a6fec in / 
# Thu, 07 Sep 2023 00:44:12 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 01:26:26 GMT
STOPSIGNAL SIGINT
# Thu, 07 Sep 2023 01:27:02 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 01:27:07 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Thu, 07 Sep 2023 01:27:08 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 07 Sep 2023 01:27:08 GMT
WORKDIR /var/www/html
# Thu, 07 Sep 2023 01:27:09 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 07 Sep 2023 01:27:09 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 07 Sep 2023 01:27:09 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 07 Sep 2023 01:27:09 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 07 Sep 2023 01:27:22 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 07 Sep 2023 01:27:22 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 07 Sep 2023 01:27:23 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 07 Sep 2023 01:27:24 GMT
USER adminer
# Thu, 07 Sep 2023 01:27:24 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Thu, 07 Sep 2023 01:27:24 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:6dd2d41f67a6666210e1a34694b8765e945a44014b53252ec0e1b50491e08d69`  
		Last Modified: Thu, 07 Sep 2023 00:49:54 GMT  
		Size: 53.3 MB (53290217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe4a876b44eaaf1ba3c702ea08a6af25e23abb30b7fcbef9b957a4c34ec5ad73`  
		Last Modified: Thu, 07 Sep 2023 01:28:21 GMT  
		Size: 39.0 MB (39020691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:529f8a0ebc99b919f45c296bfffe1d9aa35136c91542e626681a898a1e1dabb2`  
		Last Modified: Thu, 07 Sep 2023 01:28:14 GMT  
		Size: 393.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:322f53d9402212f75016bdbb862615c373419e902c2b0a0994373659dc9a40dc`  
		Last Modified: Thu, 07 Sep 2023 01:28:14 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c552fc3addf63a6a3c52100ad6a25209610153282a2977fc8234b019e7bfa4b8`  
		Last Modified: Thu, 07 Sep 2023 01:28:14 GMT  
		Size: 1.5 KB (1480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a4df5368a1108e415af1adad06e9925df044775278212b278f40db0c9e828b6`  
		Last Modified: Thu, 07 Sep 2023 01:28:15 GMT  
		Size: 1.4 MB (1385578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d8fa422b756819743a45bc63685472b1df2c01002596e8beb4231c6f1235f34`  
		Last Modified: Thu, 07 Sep 2023 01:28:14 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `adminer:standalone`

```console
$ docker pull adminer@sha256:a607d96fbf114fefcdd34729b84a6cd379dedb3ead294c56f0f318f9981fb52a
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
$ docker pull adminer@sha256:5463cc7e5a3e4ad51aa0e98c419d04646fd9b3e14a1d960ab8b420b9ce9ecc80
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.9 MB (95937329 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1bb4da606dc1a8721442935ae417a1ff7d27b9eea6ef228797780679d81ba0b6`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Thu, 07 Sep 2023 00:21:01 GMT
ADD file:144dff349a666134b5e98a9f1c6650fd9d6e4a88a6f98857f26eb84989360b91 in / 
# Thu, 07 Sep 2023 00:21:02 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 03:10:23 GMT
STOPSIGNAL SIGINT
# Thu, 07 Sep 2023 03:10:44 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 03:10:45 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Thu, 07 Sep 2023 03:10:46 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 07 Sep 2023 03:10:46 GMT
WORKDIR /var/www/html
# Thu, 07 Sep 2023 03:10:46 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 07 Sep 2023 03:10:46 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 07 Sep 2023 03:10:46 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 07 Sep 2023 03:10:46 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 07 Sep 2023 03:10:58 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 07 Sep 2023 03:10:58 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 07 Sep 2023 03:10:58 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 07 Sep 2023 03:10:58 GMT
USER adminer
# Thu, 07 Sep 2023 03:10:58 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Thu, 07 Sep 2023 03:10:58 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:5dea071bb9782209397443f024a630052ab7583e365894d414f1e39cd0f65025`  
		Last Modified: Thu, 07 Sep 2023 00:25:41 GMT  
		Size: 55.1 MB (55056245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d84864d5d25a2386de4d3f48de320a52febc28bb28cb742aba6d777c4128696`  
		Last Modified: Thu, 07 Sep 2023 03:11:37 GMT  
		Size: 39.5 MB (39491426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:792bf43687eb38330b06a085a88b6c0505837ae192ac0fe027f7a07215f853a6`  
		Last Modified: Thu, 07 Sep 2023 03:11:29 GMT  
		Size: 395.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37ef5d260982b8b88f34270bbe7314228f686ac4bbbea7e647ab96feaf464e71`  
		Last Modified: Thu, 07 Sep 2023 03:11:29 GMT  
		Size: 1.9 KB (1879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81b9b963ca6d8427a310df0283abe6c6ef185569bb470cf8a0525da60989ecb6`  
		Last Modified: Thu, 07 Sep 2023 03:11:29 GMT  
		Size: 1.5 KB (1480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e57581023c92f337603ebe93de3ebca9a7eeb11706fdccc3f1b359714e0b65a6`  
		Last Modified: Thu, 07 Sep 2023 03:11:30 GMT  
		Size: 1.4 MB (1385412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e97ed40bb1db1cf97113d360f1b14422117cf4154eba611c2d2849d66958ecaa`  
		Last Modified: Thu, 07 Sep 2023 03:11:29 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:standalone` - linux; arm variant v5

```console
$ docker pull adminer@sha256:dfd42b21fcc7d95faa4380a9bf051771e3bb79badd52e1005a8cbe551c64b6b4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.2 MB (91195063 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd44c48956465a566c168988d7201c27647c33ae7344305a32cd56f85cd46734`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Thu, 07 Sep 2023 00:48:38 GMT
ADD file:bad04cab9856def18134a0c7925a5f43816c14da597964b6d5567abc3ef6a8b9 in / 
# Thu, 07 Sep 2023 00:48:39 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 05:57:06 GMT
STOPSIGNAL SIGINT
# Thu, 07 Sep 2023 05:57:39 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 05:57:40 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Thu, 07 Sep 2023 05:57:41 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 07 Sep 2023 05:57:41 GMT
WORKDIR /var/www/html
# Thu, 07 Sep 2023 05:57:41 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 07 Sep 2023 05:57:41 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 07 Sep 2023 05:57:41 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 07 Sep 2023 05:57:41 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 07 Sep 2023 05:57:57 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 07 Sep 2023 05:57:57 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 07 Sep 2023 05:57:57 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 07 Sep 2023 05:57:57 GMT
USER adminer
# Thu, 07 Sep 2023 05:57:57 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Thu, 07 Sep 2023 05:57:57 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:c77da54c1e584356232e8207afbbe30938a9c2dda2ebc314c1d66e34c74245cc`  
		Last Modified: Thu, 07 Sep 2023 00:51:56 GMT  
		Size: 52.6 MB (52557684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f9ecd2f984b7ccbad8542193859188aa41052ff9a7f1b62ad82ac8bd8a4dc94`  
		Last Modified: Thu, 07 Sep 2023 05:58:40 GMT  
		Size: 37.2 MB (37247813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74f16b90817746d2df9ca8097b34f1a2a58ddea40f9d13b7661801e9d0cabeb6`  
		Last Modified: Thu, 07 Sep 2023 05:58:32 GMT  
		Size: 392.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2db198a220919fae8fc5093acd186481fdccff4b56654baf5ad81f5b16179f41`  
		Last Modified: Thu, 07 Sep 2023 05:58:31 GMT  
		Size: 1.9 KB (1869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bb71f0a31aaaedd68c31d3bd627d15c9a80f1fc8c77d787ae08509cea144944`  
		Last Modified: Thu, 07 Sep 2023 05:58:31 GMT  
		Size: 1.5 KB (1481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7345eee73a7d870b5e002cbc1ab741e76326b7bcedc039de45d03075a08f8bb5`  
		Last Modified: Thu, 07 Sep 2023 05:58:32 GMT  
		Size: 1.4 MB (1385331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d24fe8d24625441b6f9992c49257519dcd2a6962d677d2c96d6de6f440f16d9a`  
		Last Modified: Thu, 07 Sep 2023 05:58:31 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:standalone` - linux; arm variant v7

```console
$ docker pull adminer@sha256:dde88e85f022908e040ce9f5627e989fca6cf4f796fb912e216bc91e85b80e9f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.8 MB (87795922 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1de3886b83d0afcea5f67dd340efd76d0ff0d7cc5d4d765d7ac24bdce5ac766`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Thu, 07 Sep 2023 00:57:59 GMT
ADD file:931564fb3c8ea78b763a6b98f2739bb7c6a38484122c560a87c7166b7d45c5e6 in / 
# Thu, 07 Sep 2023 00:58:00 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 01:50:52 GMT
STOPSIGNAL SIGINT
# Thu, 07 Sep 2023 01:51:32 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 01:51:33 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Thu, 07 Sep 2023 01:51:34 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 07 Sep 2023 01:51:34 GMT
WORKDIR /var/www/html
# Thu, 07 Sep 2023 01:51:34 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 07 Sep 2023 01:51:34 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 07 Sep 2023 01:51:34 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 07 Sep 2023 01:51:34 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 07 Sep 2023 01:51:48 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 07 Sep 2023 01:51:48 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 07 Sep 2023 01:51:48 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 07 Sep 2023 01:51:48 GMT
USER adminer
# Thu, 07 Sep 2023 01:51:48 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Thu, 07 Sep 2023 01:51:48 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:5826e0d927336e7231f9d05ec48f075045fb51f9b3f16f1e20972f2a3634d102`  
		Last Modified: Thu, 07 Sep 2023 01:02:50 GMT  
		Size: 50.2 MB (50219233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64126d7f6d5bc4ca6d42b71dc00598c67b9f6f17d6919fcce1f03a613722e16d`  
		Last Modified: Thu, 07 Sep 2023 01:52:33 GMT  
		Size: 36.2 MB (36187001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fd3d57a54c1b1fa49ef5fdece23637a20b7f8e985a804fc2c5135f097a549bb`  
		Last Modified: Thu, 07 Sep 2023 01:52:25 GMT  
		Size: 393.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2440750817c8e724091323e3903329ccc274561f1f1e61c49d9da560960899bb`  
		Last Modified: Thu, 07 Sep 2023 01:52:25 GMT  
		Size: 1.9 KB (1869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c56be7ee3fb4f5d4eec7601e51e91b41bf76a5ead2b87c1026930214ba51c2b8`  
		Last Modified: Thu, 07 Sep 2023 01:52:25 GMT  
		Size: 1.5 KB (1481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22e56804b3ad37bd9f7ff556ddf336fe3b2ed8503cb32b0dfee800e4c76d9451`  
		Last Modified: Thu, 07 Sep 2023 01:52:25 GMT  
		Size: 1.4 MB (1385452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:288264a2552805e7baa2b8233fa1aad54720bdba711d9147660fe31f59cc2f32`  
		Last Modified: Thu, 07 Sep 2023 01:52:25 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:standalone` - linux; arm64 variant v8

```console
$ docker pull adminer@sha256:3b35134d84f9bb500b4ea3b9e5998209f9e587ef94982ee30e6357ae9f30d7c8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.3 MB (94338646 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6f05a6588020fe9fe371405a1735a4614daa30b4e299bd24afa4d2a017d0fa2`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Thu, 07 Sep 2023 00:39:45 GMT
ADD file:6bc001e951ef1280f566a92e65fcff57aefb8a280aa3510b7cd4b4e0a54c5cff in / 
# Thu, 07 Sep 2023 00:39:46 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 02:22:22 GMT
STOPSIGNAL SIGINT
# Thu, 07 Sep 2023 02:22:41 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 02:22:42 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Thu, 07 Sep 2023 02:22:42 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 07 Sep 2023 02:22:43 GMT
WORKDIR /var/www/html
# Thu, 07 Sep 2023 02:22:43 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 07 Sep 2023 02:22:43 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 07 Sep 2023 02:22:43 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 07 Sep 2023 02:22:43 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 07 Sep 2023 02:22:53 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 07 Sep 2023 02:22:53 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 07 Sep 2023 02:22:54 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 07 Sep 2023 02:22:54 GMT
USER adminer
# Thu, 07 Sep 2023 02:22:54 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Thu, 07 Sep 2023 02:22:54 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:61c16b7975697b00760ff9536c09eed29b6a76923d4d98be38e9cdc749506417`  
		Last Modified: Thu, 07 Sep 2023 00:43:21 GMT  
		Size: 53.7 MB (53704716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81f75bf1a78b692b687a603db539e512b761e91500113ab03d603be6cd108610`  
		Last Modified: Thu, 07 Sep 2023 02:23:31 GMT  
		Size: 39.2 MB (39244334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f3afc31326ca8d485c99b99322b549a89dd0db30062feaba0986df541301b45`  
		Last Modified: Thu, 07 Sep 2023 02:23:23 GMT  
		Size: 385.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c635f2e362703c71ad0c137ad3994b892ba8f342bd446e64f80d66d9c7c6965`  
		Last Modified: Thu, 07 Sep 2023 02:23:23 GMT  
		Size: 1.9 KB (1880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed650e87b8c0a626a5474dfdb12657fbf231ce26d8aef7302216b8b36e6c89f3`  
		Last Modified: Thu, 07 Sep 2023 02:23:24 GMT  
		Size: 1.5 KB (1481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e277a4a1ba7b301b2528764da6494b52a7e34668a0758bb6a9d5d0cb9ba10806`  
		Last Modified: Thu, 07 Sep 2023 02:23:24 GMT  
		Size: 1.4 MB (1385360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eea59163ae0d170091fc6d9eca39c3f6b9a6adaabf7b2a4cf5ecdd03cf72409c`  
		Last Modified: Thu, 07 Sep 2023 02:23:24 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:standalone` - linux; 386

```console
$ docker pull adminer@sha256:664fc6a11ece4d60a18492c17eeb4ffffb3d6fe19d3c4f4c4c3cab52b83f3ec6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.0 MB (96988434 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d7ecc3592e5ee3a2de07572724acd9167630fa736fd16b373959b3f5e2297736`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Tue, 15 Aug 2023 23:39:11 GMT
ADD file:efc88a19b31e68ca41f555bcc51338b0f135cbbd72b90637d8c73969d53addd2 in / 
# Tue, 15 Aug 2023 23:39:12 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 00:23:36 GMT
STOPSIGNAL SIGINT
# Wed, 16 Aug 2023 00:24:03 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 00:24:04 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 16 Aug 2023 00:24:05 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 16 Aug 2023 00:24:05 GMT
WORKDIR /var/www/html
# Wed, 16 Aug 2023 00:24:05 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 16 Aug 2023 00:24:05 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 16 Aug 2023 00:24:05 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 16 Aug 2023 00:24:05 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 16 Aug 2023 00:24:19 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 16 Aug 2023 00:24:19 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 16 Aug 2023 00:24:19 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 16 Aug 2023 00:24:19 GMT
USER adminer
# Wed, 16 Aug 2023 00:24:19 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 16 Aug 2023 00:24:19 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:822e033fa7b169545d5890de01438a9dd87774ff938ff440e823a3ec3f73996d`  
		Last Modified: Tue, 15 Aug 2023 23:43:47 GMT  
		Size: 56.0 MB (56040520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7644269f7e699d335219a554e561f3817b7816e99351232b3646176246991895`  
		Last Modified: Wed, 16 Aug 2023 00:25:00 GMT  
		Size: 39.6 MB (39558428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d96338ff936c667ce1c89a75f7fd111e722685d882b1f36e7b26dcb33007029`  
		Last Modified: Wed, 16 Aug 2023 00:24:50 GMT  
		Size: 389.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5339c86a7bc7031718f83f0a9af19ad028c2fa751748057f9d97d9c94c5075f6`  
		Last Modified: Wed, 16 Aug 2023 00:24:50 GMT  
		Size: 1.9 KB (1868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cbd1ad590a03bbc3ee08a1c944135c7bf81b103067417f79cdb1f8d271b4472`  
		Last Modified: Wed, 16 Aug 2023 00:24:50 GMT  
		Size: 1.5 KB (1480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:225fb2c801a3d35820604ab9c5d6c19a65e18fca4c76dd468e7015b6cb7d5d6c`  
		Last Modified: Wed, 16 Aug 2023 00:24:50 GMT  
		Size: 1.4 MB (1385258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:367f82cd1a3d30bffd1420e0c950c92f859f903ad0b0711848862db96f363ff7`  
		Last Modified: Wed, 16 Aug 2023 00:24:50 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:standalone` - linux; mips64le

```console
$ docker pull adminer@sha256:9cc962f9ae71f2c5b15623bc438ebb6d9a340e0ba8d278d98c031c39e1b5e407
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.6 MB (92612452 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c340fe4c80d84cb71a7948c0d3da3ae567112f144fa0d27c1320899c29a61f0`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Thu, 07 Sep 2023 01:09:47 GMT
ADD file:fdd438b39f1dce564715691d2a092378f02bc722e29cb80216efcbaf71cff0b8 in / 
# Thu, 07 Sep 2023 01:09:53 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 03:08:04 GMT
STOPSIGNAL SIGINT
# Thu, 07 Sep 2023 03:10:03 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 03:10:09 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Thu, 07 Sep 2023 03:10:16 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 07 Sep 2023 03:10:19 GMT
WORKDIR /var/www/html
# Thu, 07 Sep 2023 03:10:23 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 07 Sep 2023 03:10:26 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 07 Sep 2023 03:10:30 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 07 Sep 2023 03:10:33 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 07 Sep 2023 03:11:27 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 07 Sep 2023 03:11:30 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 07 Sep 2023 03:11:33 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 07 Sep 2023 03:11:36 GMT
USER adminer
# Thu, 07 Sep 2023 03:11:40 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Thu, 07 Sep 2023 03:11:43 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:0d1f1f4ccb1e0da4313c3ebcd521e7fa8073526c6f64ca7214ed31ae9bd0788e`  
		Last Modified: Thu, 07 Sep 2023 01:21:00 GMT  
		Size: 53.3 MB (53271469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b724451ca3bae07bf7da51b1c949189dc86f1e494be2830616fbe3cf4c7a447`  
		Last Modified: Thu, 07 Sep 2023 03:14:20 GMT  
		Size: 38.0 MB (37950499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:915c5f7e479b8d1cb1baf57fd9f07e06b962433d3a40fc832491c6f6614522bb`  
		Last Modified: Thu, 07 Sep 2023 03:13:55 GMT  
		Size: 394.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffcee722bb0f36a2975167c5ddf08d0da2cb56e72317f5f3e9d5cfbc3d4a4716`  
		Last Modified: Thu, 07 Sep 2023 03:13:54 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fc9ff6a8f7fb04dd6c3d6df59d01f1c9c7c34ad3cbe41553ecdff949bd20c1e`  
		Last Modified: Thu, 07 Sep 2023 03:13:54 GMT  
		Size: 1.5 KB (1482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cb2cbc2bc303d453e8e91cca3d170ccb3b27fd2bd03b89a3924e679e78c26e4`  
		Last Modified: Thu, 07 Sep 2023 03:13:55 GMT  
		Size: 1.4 MB (1386382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efe356c9d62e82baa2ebf75971c57e6fadf0e138988c966f6767875ff8843182`  
		Last Modified: Thu, 07 Sep 2023 03:13:54 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:standalone` - linux; ppc64le

```console
$ docker pull adminer@sha256:af35710d0480902e87252a3b766b10d0f75285c0d22bafce974f049ed8128552
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.3 MB (101262505 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ec6c6c445d603cdb55b8e2df3d7ca3ab043dee3a4535b6dd28cd47284c99eed`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Thu, 07 Sep 2023 00:17:47 GMT
ADD file:da42a2ef7aa1ce7e6df281b469ac67db062d14c59066a6dfd7ac5cc91d7a3b8c in / 
# Thu, 07 Sep 2023 00:17:50 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 09:04:15 GMT
STOPSIGNAL SIGINT
# Thu, 07 Sep 2023 09:07:04 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 09:07:10 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Thu, 07 Sep 2023 09:07:13 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 07 Sep 2023 09:07:14 GMT
WORKDIR /var/www/html
# Thu, 07 Sep 2023 09:07:14 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 07 Sep 2023 09:07:15 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 07 Sep 2023 09:07:15 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 07 Sep 2023 09:07:16 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 07 Sep 2023 09:08:33 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 07 Sep 2023 09:08:33 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 07 Sep 2023 09:08:35 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 07 Sep 2023 09:08:36 GMT
USER adminer
# Thu, 07 Sep 2023 09:08:38 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Thu, 07 Sep 2023 09:08:39 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:fb3cfd509d4c62da47ee9c7eee6545472d58ceaab6fcd454a82d188766dd0c45`  
		Last Modified: Thu, 07 Sep 2023 00:23:55 GMT  
		Size: 58.9 MB (58928091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bffc3bba24bd4cd45431ae9c166638ec8595b5ecab4200290f8c176a1212b7c`  
		Last Modified: Thu, 07 Sep 2023 09:11:25 GMT  
		Size: 40.9 MB (40944217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d37dbbfa36efc1b986a9571f61c675f6dd3304c8b0f8ea6ce287be3e977d1976`  
		Last Modified: Thu, 07 Sep 2023 09:11:12 GMT  
		Size: 398.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:040ad87be7d0fd1ec4f721e5fd3acd35286b3f5dd90a2f50595443791d2c5f78`  
		Last Modified: Thu, 07 Sep 2023 09:11:12 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fde911bb7830da7a8226144a744f977069a6a35fc88a5f98301891261503ecf`  
		Last Modified: Thu, 07 Sep 2023 09:11:12 GMT  
		Size: 1.5 KB (1476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1ce36781194ed33448f80f0902704489627f8098ddd838fc8a41ca597ccbfab`  
		Last Modified: Thu, 07 Sep 2023 09:11:13 GMT  
		Size: 1.4 MB (1385951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d01192f86adad3c4b51a184a68865d082250b44614aa375d150dda8f5f36b927`  
		Last Modified: Thu, 07 Sep 2023 09:11:12 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:standalone` - linux; s390x

```console
$ docker pull adminer@sha256:b3028b06f7c78024603ab547558cf83d4fe518c6bfd10a107ee923081d45c3a6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.7 MB (93700732 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40878d5b42fdc65d89e9d563be958aad831592c92455633ce54a025dc6bac4eb`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Thu, 07 Sep 2023 00:44:03 GMT
ADD file:a0582e191d0265b98e5d46c64ba9b4c46445cfa821c6e41d32db343b0e2a6fec in / 
# Thu, 07 Sep 2023 00:44:12 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 01:26:26 GMT
STOPSIGNAL SIGINT
# Thu, 07 Sep 2023 01:27:02 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 01:27:07 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Thu, 07 Sep 2023 01:27:08 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 07 Sep 2023 01:27:08 GMT
WORKDIR /var/www/html
# Thu, 07 Sep 2023 01:27:09 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 07 Sep 2023 01:27:09 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 07 Sep 2023 01:27:09 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 07 Sep 2023 01:27:09 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 07 Sep 2023 01:27:22 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 07 Sep 2023 01:27:22 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 07 Sep 2023 01:27:23 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 07 Sep 2023 01:27:24 GMT
USER adminer
# Thu, 07 Sep 2023 01:27:24 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Thu, 07 Sep 2023 01:27:24 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:6dd2d41f67a6666210e1a34694b8765e945a44014b53252ec0e1b50491e08d69`  
		Last Modified: Thu, 07 Sep 2023 00:49:54 GMT  
		Size: 53.3 MB (53290217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe4a876b44eaaf1ba3c702ea08a6af25e23abb30b7fcbef9b957a4c34ec5ad73`  
		Last Modified: Thu, 07 Sep 2023 01:28:21 GMT  
		Size: 39.0 MB (39020691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:529f8a0ebc99b919f45c296bfffe1d9aa35136c91542e626681a898a1e1dabb2`  
		Last Modified: Thu, 07 Sep 2023 01:28:14 GMT  
		Size: 393.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:322f53d9402212f75016bdbb862615c373419e902c2b0a0994373659dc9a40dc`  
		Last Modified: Thu, 07 Sep 2023 01:28:14 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c552fc3addf63a6a3c52100ad6a25209610153282a2977fc8234b019e7bfa4b8`  
		Last Modified: Thu, 07 Sep 2023 01:28:14 GMT  
		Size: 1.5 KB (1480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a4df5368a1108e415af1adad06e9925df044775278212b278f40db0c9e828b6`  
		Last Modified: Thu, 07 Sep 2023 01:28:15 GMT  
		Size: 1.4 MB (1385578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d8fa422b756819743a45bc63685472b1df2c01002596e8beb4231c6f1235f34`  
		Last Modified: Thu, 07 Sep 2023 01:28:14 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
