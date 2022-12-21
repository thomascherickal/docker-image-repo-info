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
$ docker pull adminer@sha256:895823d11ab87b3ef3db1230b33d9347b0c4fd58e6188906af37b3e7353f383f
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
$ docker pull adminer@sha256:11d6176cead328bcc234f740d98dccda987d03c17d77e03bdceb508c9d35ba30
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.6 MB (95639696 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c207e90c34520f27508ac0a18405256f981ecb45aae2baa2835c91a8f1963f0a`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 21 Dec 2022 01:20:21 GMT
ADD file:c13b430c8699df107ffd9ea5230b92238bc037a8e1cbbe35d6ab664941d575da in / 
# Wed, 21 Dec 2022 01:20:22 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 01:43:34 GMT
STOPSIGNAL SIGINT
# Wed, 21 Dec 2022 01:43:57 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 01:43:58 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 21 Dec 2022 01:43:59 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 21 Dec 2022 01:43:59 GMT
WORKDIR /var/www/html
# Wed, 21 Dec 2022 01:43:59 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 21 Dec 2022 01:43:59 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 21 Dec 2022 01:43:59 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 21 Dec 2022 01:43:59 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 21 Dec 2022 01:44:12 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 21 Dec 2022 01:44:12 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 21 Dec 2022 01:44:12 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 21 Dec 2022 01:44:12 GMT
USER adminer
# Wed, 21 Dec 2022 01:44:12 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 21 Dec 2022 01:44:12 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:32de3c850997ce03b6ff4ae8fb00b34b9d7d7f9a35bfcdb8538e22cc7b77c29d`  
		Last Modified: Wed, 21 Dec 2022 01:24:10 GMT  
		Size: 55.0 MB (55025166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bddad460143b31cc21fc89d836e6d417bb718a19c27f93eb137aebd91b79660`  
		Last Modified: Wed, 21 Dec 2022 01:44:51 GMT  
		Size: 39.2 MB (39226473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bf0beaa0412c7e762322b7311a449203a96c1e115d99efca0dddce016279e6a`  
		Last Modified: Wed, 21 Dec 2022 01:44:43 GMT  
		Size: 394.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e7ee08ea648165938f5fde9ae603f33b34b10c2d4ad2e40ea8c04913db12b65`  
		Last Modified: Wed, 21 Dec 2022 01:44:43 GMT  
		Size: 1.9 KB (1888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd9f958670d2c87349fd96a19d4254adbc404b54b3911c6962d9119d1a6fe901`  
		Last Modified: Wed, 21 Dec 2022 01:44:43 GMT  
		Size: 1.5 KB (1477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:292984a5d9c1d2f389b01937cbdf2a19e8b9de4ed6719500f1310467b1a19ff5`  
		Last Modified: Wed, 21 Dec 2022 01:44:44 GMT  
		Size: 1.4 MB (1383807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20a148ad3aa6178c7d0e684fcbc70c4ca4ba27ea5f13560aef5219a63b2b6874`  
		Last Modified: Wed, 21 Dec 2022 01:44:43 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4` - linux; arm variant v5

```console
$ docker pull adminer@sha256:50640fef3243132e1ea5d5081f834e0ca156c8264c0b0441a43492f4a4eeca23
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.9 MB (90901373 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:250a1b3ad0e6461afc53655c14f3a5b1378d898200c7bdef2f11ad58335fe9a2`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 21 Dec 2022 01:48:53 GMT
ADD file:81ccc74e0ea343972e2f3f46d2da7e9b808d9718be44d4afa7bec6904b7ab9c6 in / 
# Wed, 21 Dec 2022 01:48:55 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 02:12:35 GMT
STOPSIGNAL SIGINT
# Wed, 21 Dec 2022 02:13:07 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 02:13:09 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 21 Dec 2022 02:13:10 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 21 Dec 2022 02:13:10 GMT
WORKDIR /var/www/html
# Wed, 21 Dec 2022 02:13:10 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 21 Dec 2022 02:13:10 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 21 Dec 2022 02:13:10 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 21 Dec 2022 02:13:10 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 21 Dec 2022 02:13:27 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 21 Dec 2022 02:13:27 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 21 Dec 2022 02:13:27 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 21 Dec 2022 02:13:27 GMT
USER adminer
# Wed, 21 Dec 2022 02:13:27 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 21 Dec 2022 02:13:27 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:89b6e4f9f2f811282495a047e873c20d6ac2d53c72ad576a6907b1449eb3e635`  
		Last Modified: Wed, 21 Dec 2022 01:53:30 GMT  
		Size: 52.5 MB (52529974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2473783a5bf521f1fdf370edfbbd3a71c7d41bd6ad586832334a5359d21e0937`  
		Last Modified: Wed, 21 Dec 2022 02:14:50 GMT  
		Size: 37.0 MB (36983598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fb144c6fa4674d630705477694c2b1a78efcb47a43b11b84d11420c6672d849`  
		Last Modified: Wed, 21 Dec 2022 02:14:41 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7d2eaadeb68edbb519fcd0f769e3e17f2744670df98e1f42b2dd32755e43260`  
		Last Modified: Wed, 21 Dec 2022 02:14:41 GMT  
		Size: 1.8 KB (1840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57c2b47fd023120badcfed4eb901caaff2b0fb6b5d48de329e15232469b9af23`  
		Last Modified: Wed, 21 Dec 2022 02:14:41 GMT  
		Size: 1.5 KB (1481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54fcbf1f604d9098ea8ed2239603e5aa978d84db1258c72c4a54a6aa095ec76f`  
		Last Modified: Wed, 21 Dec 2022 02:14:41 GMT  
		Size: 1.4 MB (1383596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:216e1a8363d45d45df8c6cbfe9f7ee9909da57c723cd447b01a248fb042840f3`  
		Last Modified: Wed, 21 Dec 2022 02:14:41 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4` - linux; arm variant v7

```console
$ docker pull adminer@sha256:667b9904f45244f6db8f25daad4eea200d6c4a4f91c68de564a5caf5a4c6a5c5
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.5 MB (87525670 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4da555d48a0530a78c590fbbf78d89a6283e3bf8436c4028fc44739c58ed9fd4`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 21 Dec 2022 01:58:09 GMT
ADD file:4b6f71680de34554595f062f9e52037b48edf19ca8f34c75877caa85c42caad3 in / 
# Wed, 21 Dec 2022 01:58:10 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 16:55:05 GMT
STOPSIGNAL SIGINT
# Wed, 21 Dec 2022 16:55:27 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 16:55:28 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 21 Dec 2022 16:55:29 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 21 Dec 2022 16:55:29 GMT
WORKDIR /var/www/html
# Wed, 21 Dec 2022 16:55:29 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 21 Dec 2022 16:55:29 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 21 Dec 2022 16:55:29 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 21 Dec 2022 16:55:29 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 21 Dec 2022 16:55:42 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 21 Dec 2022 16:55:42 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 21 Dec 2022 16:55:42 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 21 Dec 2022 16:55:42 GMT
USER adminer
# Wed, 21 Dec 2022 16:55:42 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 21 Dec 2022 16:55:42 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:706bb1d74512e1fb9ba97aa9212a32d07726fbfe77e4c7e609406d2065418f57`  
		Last Modified: Wed, 21 Dec 2022 02:04:37 GMT  
		Size: 50.2 MB (50190771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a1c5cd5ac0e733e02567c893f1028628f441423281df1c54fa1042b317bb758`  
		Last Modified: Wed, 21 Dec 2022 16:56:48 GMT  
		Size: 35.9 MB (35947077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3d69909ab6c9fd65668b2d644bbb5375f5617c8bba9e82704145b53e895ad98`  
		Last Modified: Wed, 21 Dec 2022 16:56:39 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be622d99b39d413b273b3c6344f0cf7b97883297c9e7fb52951cca9bafd33f3a`  
		Last Modified: Wed, 21 Dec 2022 16:56:39 GMT  
		Size: 1.8 KB (1840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:546d6a7c782f341de9ea0c0c9aa227a5fa0d870146d87f59cb4d319c5b895028`  
		Last Modified: Wed, 21 Dec 2022 16:56:39 GMT  
		Size: 1.5 KB (1479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e94d73593abc9542a40f6e2f989f35a2bebbb21e554c4d2452cee59089701ca5`  
		Last Modified: Wed, 21 Dec 2022 16:56:39 GMT  
		Size: 1.4 MB (1383619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f3795d41125166e2051354d7af4622abe6b7610551670476d49ad99c372bad6`  
		Last Modified: Wed, 21 Dec 2022 16:56:39 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4` - linux; arm64 variant v8

```console
$ docker pull adminer@sha256:2e15c1b18293cc812ca73063a33ca295e6e5b4011ab43006f371bf3d63f7a387
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.0 MB (94046599 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f2678931127cd62d7af0ee195d7008f84b549fb9374257d1696f7cc5c9dab049`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 21 Dec 2022 01:39:40 GMT
ADD file:5bbdc914ec8ed60ac85293e88ee1aafc3f0290762e320fc86dc9d79fa201834e in / 
# Wed, 21 Dec 2022 01:39:41 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 02:01:54 GMT
STOPSIGNAL SIGINT
# Wed, 21 Dec 2022 02:02:11 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 02:02:12 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 21 Dec 2022 02:02:12 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 21 Dec 2022 02:02:13 GMT
WORKDIR /var/www/html
# Wed, 21 Dec 2022 02:02:13 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 21 Dec 2022 02:02:13 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 21 Dec 2022 02:02:13 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 21 Dec 2022 02:02:13 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 21 Dec 2022 02:02:23 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 21 Dec 2022 02:02:24 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 21 Dec 2022 02:02:24 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 21 Dec 2022 02:02:24 GMT
USER adminer
# Wed, 21 Dec 2022 02:02:24 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 21 Dec 2022 02:02:24 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:c3e6129b48b69d14c5e7a5605e2b94003fb71aac82eac46b8689f5b8007af2c5`  
		Last Modified: Wed, 21 Dec 2022 01:42:49 GMT  
		Size: 53.7 MB (53681797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:235cb929f19f47af31496a0a93a9cb1fd8f5104f0d34a160f4d2e4d6b9463df1`  
		Last Modified: Wed, 21 Dec 2022 02:02:59 GMT  
		Size: 39.0 MB (38976852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a72d5ac588c6b24f2d8a511e934c2745420b4536a9fa914031e10c9d384efd2b`  
		Last Modified: Wed, 21 Dec 2022 02:02:52 GMT  
		Size: 392.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c1912d1c0826d94d3aa328472384e502a58e992b77df780de62bbe9ba9f744e`  
		Last Modified: Wed, 21 Dec 2022 02:02:52 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f6d91a33867afb4cdea48a709f3cd43416c387bbf8a96e04840822e05a249eb`  
		Last Modified: Wed, 21 Dec 2022 02:02:52 GMT  
		Size: 1.5 KB (1481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a85debe3d62cce517ab60af785fce8ae30d5633d41e755d25700acfaa96f427`  
		Last Modified: Wed, 21 Dec 2022 02:02:53 GMT  
		Size: 1.4 MB (1383704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c707a54ab9eee88dee88a920652b121430b0f93f2599e1f3d29cd8ee7f91a359`  
		Last Modified: Wed, 21 Dec 2022 02:02:52 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4` - linux; 386

```console
$ docker pull adminer@sha256:d219efb2aecebb6bd16280905d0c7ff80b18ad7269350fec6bd034d2a093976d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.7 MB (96663116 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a504b1b6ca371056530865e9620cc9e4dabcd05dd93ab1f5b1dc2092bf6656e2`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 21 Dec 2022 01:39:08 GMT
ADD file:10d2f443f55d8ba9512899b3dff08f6e9a6c7ca096f407e3477e9798e1063785 in / 
# Wed, 21 Dec 2022 01:39:09 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 02:04:14 GMT
STOPSIGNAL SIGINT
# Wed, 21 Dec 2022 02:04:35 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 02:04:36 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 21 Dec 2022 02:04:37 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 21 Dec 2022 02:04:38 GMT
WORKDIR /var/www/html
# Wed, 21 Dec 2022 02:04:40 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 21 Dec 2022 02:04:40 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 21 Dec 2022 02:04:41 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 21 Dec 2022 02:04:42 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 21 Dec 2022 02:04:55 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 21 Dec 2022 02:04:57 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 21 Dec 2022 02:04:57 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 21 Dec 2022 02:04:58 GMT
USER adminer
# Wed, 21 Dec 2022 02:04:59 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 21 Dec 2022 02:05:00 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:bde501e1d960005aee2bdf2fc8c89b26bf694dace8740c72deda4d7705995ab7`  
		Last Modified: Wed, 21 Dec 2022 01:44:18 GMT  
		Size: 56.0 MB (56005267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd60bbc5dc31d7ec1db0a2fbd068c29f7583f7d3e2d0599f0706680ce602ee9d`  
		Last Modified: Wed, 21 Dec 2022 02:06:03 GMT  
		Size: 39.3 MB (39269700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b30e5dcb4252f7f6ded0a9c044209070412dbf7df3daab7e7343bc6bf568fe67`  
		Last Modified: Wed, 21 Dec 2022 02:05:50 GMT  
		Size: 394.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:387e2851bc00ff07433e8e9d3d12cdc6590937cbf4a9de8a035771e386a0e3c4`  
		Last Modified: Wed, 21 Dec 2022 02:05:50 GMT  
		Size: 1.7 KB (1718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c04056306aff55b02341e716626152ea622c4326e3f31a4a39bce3d631152fea`  
		Last Modified: Wed, 21 Dec 2022 02:05:50 GMT  
		Size: 1.5 KB (1478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31f79e3e185cbecc304f97fe83e64bc102e782154ed533744186d41a6de680fb`  
		Last Modified: Wed, 21 Dec 2022 02:05:51 GMT  
		Size: 1.4 MB (1384066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce0359a7ffb52c577cc47d0136aeed97a19a7e826d80ebb7b304977f271a6f7d`  
		Last Modified: Wed, 21 Dec 2022 02:05:51 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4` - linux; mips64le

```console
$ docker pull adminer@sha256:74a7ae91c85961c3ad967ae1cf25d79b8d7a69a6668843b885aebcc169a7f88f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.3 MB (92326851 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0992a9b14a478d0bfd67839ed2e77e40a770492ebd4daa67c6141cd734519bb1`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Tue, 06 Dec 2022 01:54:55 GMT
ADD file:09d48994a41c54566f7123db033773e6246c0703a518af76843198196cd39645 in / 
# Tue, 06 Dec 2022 01:55:00 GMT
CMD ["bash"]
# Sat, 17 Dec 2022 01:31:42 GMT
STOPSIGNAL SIGINT
# Sat, 17 Dec 2022 01:33:37 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Sat, 17 Dec 2022 01:33:43 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Sat, 17 Dec 2022 01:33:49 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Sat, 17 Dec 2022 01:33:53 GMT
WORKDIR /var/www/html
# Sat, 17 Dec 2022 01:33:56 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Sat, 17 Dec 2022 01:33:59 GMT
ENV ADMINER_VERSION=4.8.1
# Sat, 17 Dec 2022 01:34:02 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Sat, 17 Dec 2022 01:34:05 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Sat, 17 Dec 2022 01:34:57 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 17 Dec 2022 01:35:00 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Sat, 17 Dec 2022 01:35:03 GMT
ENTRYPOINT ["entrypoint.sh"]
# Sat, 17 Dec 2022 01:35:06 GMT
USER adminer
# Sat, 17 Dec 2022 01:35:09 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Sat, 17 Dec 2022 01:35:13 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:acb57a81743c28ead1a32571c107ac15cd970593fea4f2954b57f22e6bbad1d0`  
		Last Modified: Tue, 06 Dec 2022 02:02:59 GMT  
		Size: 53.3 MB (53260631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16a0a73e4e15363c91b94686e7609b1d84bd3ab5f4c13b2302e76c23e58ca18f`  
		Last Modified: Sat, 17 Dec 2022 01:38:30 GMT  
		Size: 37.7 MB (37676049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8aebeb122c3b2bc8c5262621178cece53cdab93feb29828240f598aa1c86637`  
		Last Modified: Sat, 17 Dec 2022 01:38:02 GMT  
		Size: 395.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3c1363529deb53f7595176aa5b55b04ab1cdf841a6cd3cdb88c41d6ec75615f`  
		Last Modified: Sat, 17 Dec 2022 01:38:02 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0923c943bb7440a1b68c2494f1f23c0a3199d4d3a6cdb87bdca8067acfbe4d4`  
		Last Modified: Sat, 17 Dec 2022 01:38:02 GMT  
		Size: 1.5 KB (1485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47a69745dad2c95e6d8ff413ca73cc902100c3848af39c316ae44ec375f8aae7`  
		Last Modified: Sat, 17 Dec 2022 01:38:03 GMT  
		Size: 1.4 MB (1386065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2548a3e7b136720a8c94faa9137694506f95bcf701a80d8b49486c2a3be6205b`  
		Last Modified: Sat, 17 Dec 2022 01:38:02 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4` - linux; ppc64le

```console
$ docker pull adminer@sha256:86fbf5aa76cfa4052c3d9bf35b81e34daf0fb53fbc674d612c071ca9a60de5ce
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.9 MB (100903714 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:075df6bcff3df963b2eec2efff06fef0b4f316e1751a5ebc98880754503bcf54`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 21 Dec 2022 01:17:21 GMT
ADD file:c95bdb0df70fa9ce48b31a7ceb8a7be0c5b925efcf01c43595868b86994dc192 in / 
# Wed, 21 Dec 2022 01:17:25 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 05:10:17 GMT
STOPSIGNAL SIGINT
# Wed, 21 Dec 2022 05:11:02 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 05:11:05 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 21 Dec 2022 05:11:07 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 21 Dec 2022 05:11:07 GMT
WORKDIR /var/www/html
# Wed, 21 Dec 2022 05:11:07 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 21 Dec 2022 05:11:08 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 21 Dec 2022 05:11:08 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 21 Dec 2022 05:11:09 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 21 Dec 2022 05:11:31 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 21 Dec 2022 05:11:31 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 21 Dec 2022 05:11:32 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 21 Dec 2022 05:11:32 GMT
USER adminer
# Wed, 21 Dec 2022 05:11:32 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 21 Dec 2022 05:11:33 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:542880f4d15404af17d342ecbb76bb92724fc7cb8a91a5e18f26bd8f8811a38a`  
		Last Modified: Wed, 21 Dec 2022 01:22:46 GMT  
		Size: 58.9 MB (58897040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8c91d3a2eff19ff3291563333f250447b70f82929a98b439e9253b9d8909332`  
		Last Modified: Wed, 21 Dec 2022 05:12:53 GMT  
		Size: 40.6 MB (40618582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1fc5014e613c79f385d0565b105dfdc45badae00ab5a50f9b06955eb34e874d`  
		Last Modified: Wed, 21 Dec 2022 05:12:39 GMT  
		Size: 394.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc90d97148640f4f164e3dc4b1f043c6ba7d8b5cddd21ede8a947339a13e3c3f`  
		Last Modified: Wed, 21 Dec 2022 05:12:39 GMT  
		Size: 1.9 KB (1879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdfe2d4e5fb66793ea99cc5959183331088d985dc203754a30a8bf6bbffb186a`  
		Last Modified: Wed, 21 Dec 2022 05:12:39 GMT  
		Size: 1.5 KB (1482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0da8c96b4d9b013ebbf00af4b8693e634764cf159be7af73d3152403cabe71e5`  
		Last Modified: Wed, 21 Dec 2022 05:12:40 GMT  
		Size: 1.4 MB (1383844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:061e859636ca9e27f80e25b38a893f2e38d08dd68c7a53bc8fb9f428dfb0f328`  
		Last Modified: Wed, 21 Dec 2022 05:12:39 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4` - linux; s390x

```console
$ docker pull adminer@sha256:4ad639f239b5117cf7381d37948390122d8f514592dade423c1fbdc4870c04b4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.4 MB (93401988 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac7114a00edb645cd010878538757f757f872e25c530cb9159f5bc03cc191726`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 21 Dec 2022 01:42:51 GMT
ADD file:22c4f2d41083ce4433bec4a71e7e6ddc5bec8e44e9cf2c9f93d0874b5b4de7c3 in / 
# Wed, 21 Dec 2022 01:42:54 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 02:06:42 GMT
STOPSIGNAL SIGINT
# Wed, 21 Dec 2022 02:07:51 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 02:08:00 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 21 Dec 2022 02:08:02 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 21 Dec 2022 02:08:03 GMT
WORKDIR /var/www/html
# Wed, 21 Dec 2022 02:08:04 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 21 Dec 2022 02:08:04 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 21 Dec 2022 02:08:05 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 21 Dec 2022 02:08:06 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 21 Dec 2022 02:08:33 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 21 Dec 2022 02:08:33 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 21 Dec 2022 02:08:34 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 21 Dec 2022 02:08:35 GMT
USER adminer
# Wed, 21 Dec 2022 02:08:35 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 21 Dec 2022 02:08:36 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:7f45294776f4c97d23f8dbfca98d4b57701b478eedfcb154a7e7dc6d6954ba44`  
		Last Modified: Wed, 21 Dec 2022 01:48:50 GMT  
		Size: 53.3 MB (53258472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8610ee81c430b6503a5ee2d7cc451175bdfc868fc17ef5a675b43679da433867`  
		Last Modified: Wed, 21 Dec 2022 02:10:03 GMT  
		Size: 38.8 MB (38755148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:211b726eee70a0c5ff85337d1e98c7987025435a41ca5421f47d96fc164b5b27`  
		Last Modified: Wed, 21 Dec 2022 02:09:56 GMT  
		Size: 395.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c6a1fa2154f900c32f87164afe347f0dddbb7a641dc81b7fc436b1d15a5349d`  
		Last Modified: Wed, 21 Dec 2022 02:09:56 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e030c793dfbf87ef1f5dbbecd22117bcf1695eb293e41bca267fb29d0e98d59d`  
		Last Modified: Wed, 21 Dec 2022 02:09:56 GMT  
		Size: 1.5 KB (1478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:965c9f68e6765f8a5967198527ce6ff7bf0646cab60aa30ecef97747554c0869`  
		Last Modified: Wed, 21 Dec 2022 02:09:56 GMT  
		Size: 1.4 MB (1384122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d34b801ca3351132a2f2914bc4ef3ca0f91a2c87c2b42fce3662fd5f20593aea`  
		Last Modified: Wed, 21 Dec 2022 02:09:56 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `adminer:4-fastcgi`

```console
$ docker pull adminer@sha256:37807622785148a8a96b6b2d9314e7db8e7202306531a9e674f9735b07ce17d3
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
$ docker pull adminer@sha256:1e1e6130a4906493f3dcda03ec0eb19eeec7d747868d8e7526583e93b90377ed
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.6 MB (95642424 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ec85d40ab3aa8923f6295358e72e000090652b9a26b7b9c7774d997a844e842`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Wed, 21 Dec 2022 01:20:21 GMT
ADD file:c13b430c8699df107ffd9ea5230b92238bc037a8e1cbbe35d6ab664941d575da in / 
# Wed, 21 Dec 2022 01:20:22 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 01:43:34 GMT
STOPSIGNAL SIGINT
# Wed, 21 Dec 2022 01:43:57 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 01:43:58 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 21 Dec 2022 01:44:15 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Wed, 21 Dec 2022 01:44:16 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 21 Dec 2022 01:44:16 GMT
WORKDIR /var/www/html
# Wed, 21 Dec 2022 01:44:16 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 21 Dec 2022 01:44:16 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 21 Dec 2022 01:44:16 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 21 Dec 2022 01:44:17 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 21 Dec 2022 01:44:28 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 21 Dec 2022 01:44:28 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 21 Dec 2022 01:44:28 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 21 Dec 2022 01:44:29 GMT
USER adminer
# Wed, 21 Dec 2022 01:44:29 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:32de3c850997ce03b6ff4ae8fb00b34b9d7d7f9a35bfcdb8538e22cc7b77c29d`  
		Last Modified: Wed, 21 Dec 2022 01:24:10 GMT  
		Size: 55.0 MB (55025166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bddad460143b31cc21fc89d836e6d417bb718a19c27f93eb137aebd91b79660`  
		Last Modified: Wed, 21 Dec 2022 01:44:51 GMT  
		Size: 39.2 MB (39226473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bf0beaa0412c7e762322b7311a449203a96c1e115d99efca0dddce016279e6a`  
		Last Modified: Wed, 21 Dec 2022 01:44:43 GMT  
		Size: 394.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e85c5399c00e75eb8dd783e68be98aeef85fb6e2e50ab17a1f3d0fb977496970`  
		Last Modified: Wed, 21 Dec 2022 01:45:09 GMT  
		Size: 2.7 KB (2712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fa2e6155707c0c71fe403f845f4a9061a2bba300a1a1c18f480f59742b9036a`  
		Last Modified: Wed, 21 Dec 2022 01:45:09 GMT  
		Size: 1.9 KB (1879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48c9c38ec5f03fab46adc653af92a4b0c326aa93c7533ff5e7c2166e3ef8cf40`  
		Last Modified: Wed, 21 Dec 2022 01:45:09 GMT  
		Size: 1.5 KB (1478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a19f8c5c89b7131c03f16fdc1f9c0c0bf07fbc0d9bfe1cecb756a290c47fbd6b`  
		Last Modified: Wed, 21 Dec 2022 01:45:10 GMT  
		Size: 1.4 MB (1383831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a5ef3fdf80e2ac647453715c908b46bb54a9310430fed3a3bb6e8f418740b8e`  
		Last Modified: Wed, 21 Dec 2022 01:45:09 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-fastcgi` - linux; arm variant v5

```console
$ docker pull adminer@sha256:f6452248c81bf0aa2cecfa804a14cd9b14a2503be250138828d035b75e2896a9
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.9 MB (90904118 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d18173eb6830d6ef3ae8c8a231cb8ea70b230991680c62578ac47461b434c398`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Wed, 21 Dec 2022 01:48:53 GMT
ADD file:81ccc74e0ea343972e2f3f46d2da7e9b808d9718be44d4afa7bec6904b7ab9c6 in / 
# Wed, 21 Dec 2022 01:48:55 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 02:12:35 GMT
STOPSIGNAL SIGINT
# Wed, 21 Dec 2022 02:13:07 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 02:13:09 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 21 Dec 2022 02:13:39 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Wed, 21 Dec 2022 02:13:40 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 21 Dec 2022 02:13:41 GMT
WORKDIR /var/www/html
# Wed, 21 Dec 2022 02:13:41 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 21 Dec 2022 02:13:42 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 21 Dec 2022 02:13:42 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 21 Dec 2022 02:13:42 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 21 Dec 2022 02:14:02 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 21 Dec 2022 02:14:02 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 21 Dec 2022 02:14:02 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 21 Dec 2022 02:14:02 GMT
USER adminer
# Wed, 21 Dec 2022 02:14:03 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:89b6e4f9f2f811282495a047e873c20d6ac2d53c72ad576a6907b1449eb3e635`  
		Last Modified: Wed, 21 Dec 2022 01:53:30 GMT  
		Size: 52.5 MB (52529974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2473783a5bf521f1fdf370edfbbd3a71c7d41bd6ad586832334a5359d21e0937`  
		Last Modified: Wed, 21 Dec 2022 02:14:50 GMT  
		Size: 37.0 MB (36983598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fb144c6fa4674d630705477694c2b1a78efcb47a43b11b84d11420c6672d849`  
		Last Modified: Wed, 21 Dec 2022 02:14:41 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26063a58f85ffe38619444fe9e9ea1012e4e7fdb2b4d72cdcac7a8aae808f733`  
		Last Modified: Wed, 21 Dec 2022 02:15:15 GMT  
		Size: 2.7 KB (2710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41851614d9620c865a301e15f38ab0d4c8ddd9a1f4202edbf3a691d918884cf7`  
		Last Modified: Wed, 21 Dec 2022 02:15:15 GMT  
		Size: 1.8 KB (1839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ab4a9eecfe7e71f9ca3e31e0de304dbd42f4d4078f5feecb1c7c6f4f42005cc`  
		Last Modified: Wed, 21 Dec 2022 02:15:15 GMT  
		Size: 1.5 KB (1481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:606df83e76d99dd227ac689ddcd3e7f8434d06d4e46042bc2419167493a3b188`  
		Last Modified: Wed, 21 Dec 2022 02:15:15 GMT  
		Size: 1.4 MB (1383635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6018be7539eedb016a02d6429a6c60eaa072ee9ea161b1d74167953aa3a9de72`  
		Last Modified: Wed, 21 Dec 2022 02:15:15 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-fastcgi` - linux; arm variant v7

```console
$ docker pull adminer@sha256:9928846ee8fb76c681b35c87ebfed49499f447a0c1c81393d30ab2bcba70a6c2
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.5 MB (87528433 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99681162737fb62edc07a8e79538b32ebe15b415a91f8e6c9e8d2c0f6f224b9a`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Wed, 21 Dec 2022 01:58:09 GMT
ADD file:4b6f71680de34554595f062f9e52037b48edf19ca8f34c75877caa85c42caad3 in / 
# Wed, 21 Dec 2022 01:58:10 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 16:55:05 GMT
STOPSIGNAL SIGINT
# Wed, 21 Dec 2022 16:55:27 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 16:55:28 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 21 Dec 2022 16:55:49 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Wed, 21 Dec 2022 16:55:50 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 21 Dec 2022 16:55:50 GMT
WORKDIR /var/www/html
# Wed, 21 Dec 2022 16:55:50 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 21 Dec 2022 16:55:50 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 21 Dec 2022 16:55:50 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 21 Dec 2022 16:55:50 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 21 Dec 2022 16:56:04 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 21 Dec 2022 16:56:04 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 21 Dec 2022 16:56:04 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 21 Dec 2022 16:56:04 GMT
USER adminer
# Wed, 21 Dec 2022 16:56:04 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:706bb1d74512e1fb9ba97aa9212a32d07726fbfe77e4c7e609406d2065418f57`  
		Last Modified: Wed, 21 Dec 2022 02:04:37 GMT  
		Size: 50.2 MB (50190771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a1c5cd5ac0e733e02567c893f1028628f441423281df1c54fa1042b317bb758`  
		Last Modified: Wed, 21 Dec 2022 16:56:48 GMT  
		Size: 35.9 MB (35947077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3d69909ab6c9fd65668b2d644bbb5375f5617c8bba9e82704145b53e895ad98`  
		Last Modified: Wed, 21 Dec 2022 16:56:39 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0e39a1a73560e658bd05d5621c5e241ea6c658eeb4d6d40fab42c2d0e049dd9`  
		Last Modified: Wed, 21 Dec 2022 16:57:11 GMT  
		Size: 2.7 KB (2707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:570ddb9aaf5affd1f0db7ce02160f1220f1f786028eb2dc3304d29faec9a812c`  
		Last Modified: Wed, 21 Dec 2022 16:57:11 GMT  
		Size: 1.8 KB (1841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5278a6d095ca223fab850a965a90f10b571dee63613450a5c305743288a3db7`  
		Last Modified: Wed, 21 Dec 2022 16:57:11 GMT  
		Size: 1.5 KB (1476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f0a1888014f0f3ae5844f8d80c0707d886f7e951a2583d43345fb59abe5e97c`  
		Last Modified: Wed, 21 Dec 2022 16:57:12 GMT  
		Size: 1.4 MB (1383680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6e719bcd08751a23a74658e85fc4e47ae42d98213576128a573499661a743b9`  
		Last Modified: Wed, 21 Dec 2022 16:57:11 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-fastcgi` - linux; arm64 variant v8

```console
$ docker pull adminer@sha256:deace6e0488124187d0f03d131c3f503f66d5532f6cba7a2c9bbd9f4e92c9639
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.0 MB (94049324 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5eaa4905b3a6a204b45fc4e4608dc8de2ee6e3a8b386c2a8daed65b7ea308fa`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Wed, 21 Dec 2022 01:39:40 GMT
ADD file:5bbdc914ec8ed60ac85293e88ee1aafc3f0290762e320fc86dc9d79fa201834e in / 
# Wed, 21 Dec 2022 01:39:41 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 02:01:54 GMT
STOPSIGNAL SIGINT
# Wed, 21 Dec 2022 02:02:11 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 02:02:12 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 21 Dec 2022 02:02:27 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Wed, 21 Dec 2022 02:02:28 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 21 Dec 2022 02:02:28 GMT
WORKDIR /var/www/html
# Wed, 21 Dec 2022 02:02:28 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 21 Dec 2022 02:02:28 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 21 Dec 2022 02:02:28 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 21 Dec 2022 02:02:28 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 21 Dec 2022 02:02:38 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 21 Dec 2022 02:02:38 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 21 Dec 2022 02:02:38 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 21 Dec 2022 02:02:38 GMT
USER adminer
# Wed, 21 Dec 2022 02:02:38 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:c3e6129b48b69d14c5e7a5605e2b94003fb71aac82eac46b8689f5b8007af2c5`  
		Last Modified: Wed, 21 Dec 2022 01:42:49 GMT  
		Size: 53.7 MB (53681797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:235cb929f19f47af31496a0a93a9cb1fd8f5104f0d34a160f4d2e4d6b9463df1`  
		Last Modified: Wed, 21 Dec 2022 02:02:59 GMT  
		Size: 39.0 MB (38976852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a72d5ac588c6b24f2d8a511e934c2745420b4536a9fa914031e10c9d384efd2b`  
		Last Modified: Wed, 21 Dec 2022 02:02:52 GMT  
		Size: 392.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13819a4b0fdaaf0d610656691e268b84f62b9bc6f1978b10b2fd66d30bfc61a0`  
		Last Modified: Wed, 21 Dec 2022 02:03:18 GMT  
		Size: 2.7 KB (2705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e39e3b462a156c2eb8929e5b29025db6c8048ec880966c1e891e12db93bfb103`  
		Last Modified: Wed, 21 Dec 2022 02:03:18 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c2102a525d7aa1a32b03261d2429812840b08fab7cc2175e391f84857823539`  
		Last Modified: Wed, 21 Dec 2022 02:03:18 GMT  
		Size: 1.5 KB (1476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4364503e41b1e8f317d4c98b8da4b7d28551f47d554987462dfbc04169e893da`  
		Last Modified: Wed, 21 Dec 2022 02:03:19 GMT  
		Size: 1.4 MB (1383730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e279f93f23126fbc1db29d1577bf87115d79396ca7c78cb6b2bda1279cdaa269`  
		Last Modified: Wed, 21 Dec 2022 02:03:18 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-fastcgi` - linux; 386

```console
$ docker pull adminer@sha256:9a434bc61ca7023a8f2c77a9d0958ab597cd69f03685202d1661614ba76c346f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.7 MB (96665821 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c32a28f670f6878d3ca957e9fc114d3736d77b40db0223160324a35254c19e3`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Wed, 21 Dec 2022 01:39:08 GMT
ADD file:10d2f443f55d8ba9512899b3dff08f6e9a6c7ca096f407e3477e9798e1063785 in / 
# Wed, 21 Dec 2022 01:39:09 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 02:04:14 GMT
STOPSIGNAL SIGINT
# Wed, 21 Dec 2022 02:04:35 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 02:04:36 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 21 Dec 2022 02:05:05 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Wed, 21 Dec 2022 02:05:06 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 21 Dec 2022 02:05:07 GMT
WORKDIR /var/www/html
# Wed, 21 Dec 2022 02:05:09 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 21 Dec 2022 02:05:09 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 21 Dec 2022 02:05:10 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 21 Dec 2022 02:05:11 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 21 Dec 2022 02:05:24 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 21 Dec 2022 02:05:25 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 21 Dec 2022 02:05:25 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 21 Dec 2022 02:05:26 GMT
USER adminer
# Wed, 21 Dec 2022 02:05:27 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:bde501e1d960005aee2bdf2fc8c89b26bf694dace8740c72deda4d7705995ab7`  
		Last Modified: Wed, 21 Dec 2022 01:44:18 GMT  
		Size: 56.0 MB (56005267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd60bbc5dc31d7ec1db0a2fbd068c29f7583f7d3e2d0599f0706680ce602ee9d`  
		Last Modified: Wed, 21 Dec 2022 02:06:03 GMT  
		Size: 39.3 MB (39269700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b30e5dcb4252f7f6ded0a9c044209070412dbf7df3daab7e7343bc6bf568fe67`  
		Last Modified: Wed, 21 Dec 2022 02:05:50 GMT  
		Size: 394.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44b71679c4856448b64de04f5a85f11611e00ec6255adf5430d19216fda4b172`  
		Last Modified: Wed, 21 Dec 2022 02:06:25 GMT  
		Size: 2.7 KB (2708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba4434a757058f98902edee00915212df3d942d3675e23589ab4b5b5ff27a41f`  
		Last Modified: Wed, 21 Dec 2022 02:06:24 GMT  
		Size: 1.7 KB (1718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b87eb7dde4067b918229c1df6d6f6890a97ab78c902accb2240718ff2d3e1145`  
		Last Modified: Wed, 21 Dec 2022 02:06:25 GMT  
		Size: 1.5 KB (1479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc82102410ace2a3805c07a9de9d7d5e319e8b7903eebcb983e7ac7c0f69b585`  
		Last Modified: Wed, 21 Dec 2022 02:06:25 GMT  
		Size: 1.4 MB (1384064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dafaed69f8eded599f349c789c94fec52eac63054f3692ca4755826853857a33`  
		Last Modified: Wed, 21 Dec 2022 02:06:25 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-fastcgi` - linux; mips64le

```console
$ docker pull adminer@sha256:e7a494809199392e1931b1b28a4f4331784fa3d2bcba37ce44f3cbf895e33e37
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.3 MB (92329550 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e351ec1ac27e9afe073b5935a1450c40ddd4d5fbb496b42509bde8929705b8d1`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Tue, 06 Dec 2022 01:54:55 GMT
ADD file:09d48994a41c54566f7123db033773e6246c0703a518af76843198196cd39645 in / 
# Tue, 06 Dec 2022 01:55:00 GMT
CMD ["bash"]
# Sat, 17 Dec 2022 01:31:42 GMT
STOPSIGNAL SIGINT
# Sat, 17 Dec 2022 01:33:37 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Sat, 17 Dec 2022 01:33:43 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Sat, 17 Dec 2022 01:35:28 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Sat, 17 Dec 2022 01:35:34 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Sat, 17 Dec 2022 01:35:38 GMT
WORKDIR /var/www/html
# Sat, 17 Dec 2022 01:35:40 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Sat, 17 Dec 2022 01:35:44 GMT
ENV ADMINER_VERSION=4.8.1
# Sat, 17 Dec 2022 01:35:47 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Sat, 17 Dec 2022 01:35:50 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Sat, 17 Dec 2022 01:36:39 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 17 Dec 2022 01:36:41 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Sat, 17 Dec 2022 01:36:45 GMT
ENTRYPOINT ["entrypoint.sh"]
# Sat, 17 Dec 2022 01:36:48 GMT
USER adminer
# Sat, 17 Dec 2022 01:36:51 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:acb57a81743c28ead1a32571c107ac15cd970593fea4f2954b57f22e6bbad1d0`  
		Last Modified: Tue, 06 Dec 2022 02:02:59 GMT  
		Size: 53.3 MB (53260631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16a0a73e4e15363c91b94686e7609b1d84bd3ab5f4c13b2302e76c23e58ca18f`  
		Last Modified: Sat, 17 Dec 2022 01:38:30 GMT  
		Size: 37.7 MB (37676049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8aebeb122c3b2bc8c5262621178cece53cdab93feb29828240f598aa1c86637`  
		Last Modified: Sat, 17 Dec 2022 01:38:02 GMT  
		Size: 395.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2edf7b726c889078b8d32ddaeb1eb6051a11a8f855dad5390aae1cdb3688615`  
		Last Modified: Sat, 17 Dec 2022 01:38:50 GMT  
		Size: 2.7 KB (2712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af0218fe073275ed5c7c0432527e394ba32d894ee6751a1eff961b6bdc775443`  
		Last Modified: Sat, 17 Dec 2022 01:38:50 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f299876d55c3b91c269c41873c488d741613390f000b3104546c0329410c51d8`  
		Last Modified: Sat, 17 Dec 2022 01:38:50 GMT  
		Size: 1.5 KB (1481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae1c4a189325330ffbce29139b4535443d6c162e063032ca30ada9bdc5e8ba60`  
		Last Modified: Sat, 17 Dec 2022 01:38:50 GMT  
		Size: 1.4 MB (1386058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d6e400fdc50315e82b9a184d27fff83deb7028bf757fefea876e9e20247a70d`  
		Last Modified: Sat, 17 Dec 2022 01:38:50 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-fastcgi` - linux; ppc64le

```console
$ docker pull adminer@sha256:248833c195a726561a4627fd9c8ef5a3ddc6b4350809c298ad4a9f2e9cf1203f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.9 MB (100906397 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1156cafbf63d82f8a2d9663ffb1652e3b3b0ae96e2efb8e523cc0c422d1da1a5`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Wed, 21 Dec 2022 01:17:21 GMT
ADD file:c95bdb0df70fa9ce48b31a7ceb8a7be0c5b925efcf01c43595868b86994dc192 in / 
# Wed, 21 Dec 2022 01:17:25 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 05:10:17 GMT
STOPSIGNAL SIGINT
# Wed, 21 Dec 2022 05:11:02 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 05:11:05 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 21 Dec 2022 05:11:43 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Wed, 21 Dec 2022 05:11:44 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 21 Dec 2022 05:11:44 GMT
WORKDIR /var/www/html
# Wed, 21 Dec 2022 05:11:45 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 21 Dec 2022 05:11:45 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 21 Dec 2022 05:11:45 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 21 Dec 2022 05:11:46 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 21 Dec 2022 05:12:07 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 21 Dec 2022 05:12:07 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 21 Dec 2022 05:12:08 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 21 Dec 2022 05:12:08 GMT
USER adminer
# Wed, 21 Dec 2022 05:12:08 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:542880f4d15404af17d342ecbb76bb92724fc7cb8a91a5e18f26bd8f8811a38a`  
		Last Modified: Wed, 21 Dec 2022 01:22:46 GMT  
		Size: 58.9 MB (58897040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8c91d3a2eff19ff3291563333f250447b70f82929a98b439e9253b9d8909332`  
		Last Modified: Wed, 21 Dec 2022 05:12:53 GMT  
		Size: 40.6 MB (40618582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1fc5014e613c79f385d0565b105dfdc45badae00ab5a50f9b06955eb34e874d`  
		Last Modified: Wed, 21 Dec 2022 05:12:39 GMT  
		Size: 394.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5b74bb738e578f210c95db9d4fc2c314ce3454b4454d48e9fd0269bc6c207e8`  
		Last Modified: Wed, 21 Dec 2022 05:13:17 GMT  
		Size: 2.7 KB (2712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fd43780f4a97de99f2a70cbdeb1e9b998a4a0b78d33e413d5b202dfdc938ebb`  
		Last Modified: Wed, 21 Dec 2022 05:13:17 GMT  
		Size: 1.9 KB (1878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf0b6261dedf5bb3e0f0d3f02c0c41d44c78abd343b214d5e105040aecdbead8`  
		Last Modified: Wed, 21 Dec 2022 05:13:17 GMT  
		Size: 1.5 KB (1480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ffa54700428e518453fb0a542abf4e41ba28e7f58c380d6540691f0d3ded1a1`  
		Last Modified: Wed, 21 Dec 2022 05:13:17 GMT  
		Size: 1.4 MB (1383821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92c025b84e6aa9a000bd19d3eded000fba61196718941820ae5d1eba78d131c8`  
		Last Modified: Wed, 21 Dec 2022 05:13:17 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-fastcgi` - linux; s390x

```console
$ docker pull adminer@sha256:a1fa0d120584828c961ce0b29ab5d38c4bd62a7c4832051e8a59bdd185eaa72e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.4 MB (93404712 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:078ace26e901a591bccbb767862313e0b30444a61969a6f9563f56d8172155d7`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Wed, 21 Dec 2022 01:42:51 GMT
ADD file:22c4f2d41083ce4433bec4a71e7e6ddc5bec8e44e9cf2c9f93d0874b5b4de7c3 in / 
# Wed, 21 Dec 2022 01:42:54 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 02:06:42 GMT
STOPSIGNAL SIGINT
# Wed, 21 Dec 2022 02:07:51 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 02:08:00 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 21 Dec 2022 02:08:48 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Wed, 21 Dec 2022 02:08:50 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 21 Dec 2022 02:08:51 GMT
WORKDIR /var/www/html
# Wed, 21 Dec 2022 02:08:51 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 21 Dec 2022 02:08:52 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 21 Dec 2022 02:08:53 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 21 Dec 2022 02:08:53 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 21 Dec 2022 02:09:20 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 21 Dec 2022 02:09:21 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 21 Dec 2022 02:09:21 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 21 Dec 2022 02:09:22 GMT
USER adminer
# Wed, 21 Dec 2022 02:09:23 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:7f45294776f4c97d23f8dbfca98d4b57701b478eedfcb154a7e7dc6d6954ba44`  
		Last Modified: Wed, 21 Dec 2022 01:48:50 GMT  
		Size: 53.3 MB (53258472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8610ee81c430b6503a5ee2d7cc451175bdfc868fc17ef5a675b43679da433867`  
		Last Modified: Wed, 21 Dec 2022 02:10:03 GMT  
		Size: 38.8 MB (38755148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:211b726eee70a0c5ff85337d1e98c7987025435a41ca5421f47d96fc164b5b27`  
		Last Modified: Wed, 21 Dec 2022 02:09:56 GMT  
		Size: 395.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:548dc4ca6b10efd03438d3ef399c3d858053ec103194dba6350126f59b0cc988`  
		Last Modified: Wed, 21 Dec 2022 02:10:20 GMT  
		Size: 2.7 KB (2713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcd20979228556508e9e2424f45667a2246d9c409f2557492271740f4840e889`  
		Last Modified: Wed, 21 Dec 2022 02:10:20 GMT  
		Size: 1.9 KB (1883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2e7ff5c1ff35711cc296fbbe902ca0db4bc13c6b5863ba4c3adc2640e16177e`  
		Last Modified: Wed, 21 Dec 2022 02:10:20 GMT  
		Size: 1.5 KB (1481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:334c0739b3be2b837dcd345afc1a5bd12f907a3080d438abf00d8706d01e99c8`  
		Last Modified: Wed, 21 Dec 2022 02:10:20 GMT  
		Size: 1.4 MB (1384126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd966444e211f7ff2ff5aca0482cee29884580acd8b4114e8bd25b616618c89c`  
		Last Modified: Wed, 21 Dec 2022 02:10:21 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `adminer:4-standalone`

```console
$ docker pull adminer@sha256:895823d11ab87b3ef3db1230b33d9347b0c4fd58e6188906af37b3e7353f383f
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
$ docker pull adminer@sha256:11d6176cead328bcc234f740d98dccda987d03c17d77e03bdceb508c9d35ba30
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.6 MB (95639696 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c207e90c34520f27508ac0a18405256f981ecb45aae2baa2835c91a8f1963f0a`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 21 Dec 2022 01:20:21 GMT
ADD file:c13b430c8699df107ffd9ea5230b92238bc037a8e1cbbe35d6ab664941d575da in / 
# Wed, 21 Dec 2022 01:20:22 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 01:43:34 GMT
STOPSIGNAL SIGINT
# Wed, 21 Dec 2022 01:43:57 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 01:43:58 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 21 Dec 2022 01:43:59 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 21 Dec 2022 01:43:59 GMT
WORKDIR /var/www/html
# Wed, 21 Dec 2022 01:43:59 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 21 Dec 2022 01:43:59 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 21 Dec 2022 01:43:59 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 21 Dec 2022 01:43:59 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 21 Dec 2022 01:44:12 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 21 Dec 2022 01:44:12 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 21 Dec 2022 01:44:12 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 21 Dec 2022 01:44:12 GMT
USER adminer
# Wed, 21 Dec 2022 01:44:12 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 21 Dec 2022 01:44:12 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:32de3c850997ce03b6ff4ae8fb00b34b9d7d7f9a35bfcdb8538e22cc7b77c29d`  
		Last Modified: Wed, 21 Dec 2022 01:24:10 GMT  
		Size: 55.0 MB (55025166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bddad460143b31cc21fc89d836e6d417bb718a19c27f93eb137aebd91b79660`  
		Last Modified: Wed, 21 Dec 2022 01:44:51 GMT  
		Size: 39.2 MB (39226473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bf0beaa0412c7e762322b7311a449203a96c1e115d99efca0dddce016279e6a`  
		Last Modified: Wed, 21 Dec 2022 01:44:43 GMT  
		Size: 394.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e7ee08ea648165938f5fde9ae603f33b34b10c2d4ad2e40ea8c04913db12b65`  
		Last Modified: Wed, 21 Dec 2022 01:44:43 GMT  
		Size: 1.9 KB (1888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd9f958670d2c87349fd96a19d4254adbc404b54b3911c6962d9119d1a6fe901`  
		Last Modified: Wed, 21 Dec 2022 01:44:43 GMT  
		Size: 1.5 KB (1477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:292984a5d9c1d2f389b01937cbdf2a19e8b9de4ed6719500f1310467b1a19ff5`  
		Last Modified: Wed, 21 Dec 2022 01:44:44 GMT  
		Size: 1.4 MB (1383807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20a148ad3aa6178c7d0e684fcbc70c4ca4ba27ea5f13560aef5219a63b2b6874`  
		Last Modified: Wed, 21 Dec 2022 01:44:43 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-standalone` - linux; arm variant v5

```console
$ docker pull adminer@sha256:50640fef3243132e1ea5d5081f834e0ca156c8264c0b0441a43492f4a4eeca23
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.9 MB (90901373 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:250a1b3ad0e6461afc53655c14f3a5b1378d898200c7bdef2f11ad58335fe9a2`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 21 Dec 2022 01:48:53 GMT
ADD file:81ccc74e0ea343972e2f3f46d2da7e9b808d9718be44d4afa7bec6904b7ab9c6 in / 
# Wed, 21 Dec 2022 01:48:55 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 02:12:35 GMT
STOPSIGNAL SIGINT
# Wed, 21 Dec 2022 02:13:07 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 02:13:09 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 21 Dec 2022 02:13:10 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 21 Dec 2022 02:13:10 GMT
WORKDIR /var/www/html
# Wed, 21 Dec 2022 02:13:10 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 21 Dec 2022 02:13:10 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 21 Dec 2022 02:13:10 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 21 Dec 2022 02:13:10 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 21 Dec 2022 02:13:27 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 21 Dec 2022 02:13:27 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 21 Dec 2022 02:13:27 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 21 Dec 2022 02:13:27 GMT
USER adminer
# Wed, 21 Dec 2022 02:13:27 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 21 Dec 2022 02:13:27 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:89b6e4f9f2f811282495a047e873c20d6ac2d53c72ad576a6907b1449eb3e635`  
		Last Modified: Wed, 21 Dec 2022 01:53:30 GMT  
		Size: 52.5 MB (52529974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2473783a5bf521f1fdf370edfbbd3a71c7d41bd6ad586832334a5359d21e0937`  
		Last Modified: Wed, 21 Dec 2022 02:14:50 GMT  
		Size: 37.0 MB (36983598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fb144c6fa4674d630705477694c2b1a78efcb47a43b11b84d11420c6672d849`  
		Last Modified: Wed, 21 Dec 2022 02:14:41 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7d2eaadeb68edbb519fcd0f769e3e17f2744670df98e1f42b2dd32755e43260`  
		Last Modified: Wed, 21 Dec 2022 02:14:41 GMT  
		Size: 1.8 KB (1840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57c2b47fd023120badcfed4eb901caaff2b0fb6b5d48de329e15232469b9af23`  
		Last Modified: Wed, 21 Dec 2022 02:14:41 GMT  
		Size: 1.5 KB (1481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54fcbf1f604d9098ea8ed2239603e5aa978d84db1258c72c4a54a6aa095ec76f`  
		Last Modified: Wed, 21 Dec 2022 02:14:41 GMT  
		Size: 1.4 MB (1383596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:216e1a8363d45d45df8c6cbfe9f7ee9909da57c723cd447b01a248fb042840f3`  
		Last Modified: Wed, 21 Dec 2022 02:14:41 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-standalone` - linux; arm variant v7

```console
$ docker pull adminer@sha256:667b9904f45244f6db8f25daad4eea200d6c4a4f91c68de564a5caf5a4c6a5c5
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.5 MB (87525670 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4da555d48a0530a78c590fbbf78d89a6283e3bf8436c4028fc44739c58ed9fd4`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 21 Dec 2022 01:58:09 GMT
ADD file:4b6f71680de34554595f062f9e52037b48edf19ca8f34c75877caa85c42caad3 in / 
# Wed, 21 Dec 2022 01:58:10 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 16:55:05 GMT
STOPSIGNAL SIGINT
# Wed, 21 Dec 2022 16:55:27 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 16:55:28 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 21 Dec 2022 16:55:29 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 21 Dec 2022 16:55:29 GMT
WORKDIR /var/www/html
# Wed, 21 Dec 2022 16:55:29 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 21 Dec 2022 16:55:29 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 21 Dec 2022 16:55:29 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 21 Dec 2022 16:55:29 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 21 Dec 2022 16:55:42 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 21 Dec 2022 16:55:42 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 21 Dec 2022 16:55:42 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 21 Dec 2022 16:55:42 GMT
USER adminer
# Wed, 21 Dec 2022 16:55:42 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 21 Dec 2022 16:55:42 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:706bb1d74512e1fb9ba97aa9212a32d07726fbfe77e4c7e609406d2065418f57`  
		Last Modified: Wed, 21 Dec 2022 02:04:37 GMT  
		Size: 50.2 MB (50190771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a1c5cd5ac0e733e02567c893f1028628f441423281df1c54fa1042b317bb758`  
		Last Modified: Wed, 21 Dec 2022 16:56:48 GMT  
		Size: 35.9 MB (35947077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3d69909ab6c9fd65668b2d644bbb5375f5617c8bba9e82704145b53e895ad98`  
		Last Modified: Wed, 21 Dec 2022 16:56:39 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be622d99b39d413b273b3c6344f0cf7b97883297c9e7fb52951cca9bafd33f3a`  
		Last Modified: Wed, 21 Dec 2022 16:56:39 GMT  
		Size: 1.8 KB (1840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:546d6a7c782f341de9ea0c0c9aa227a5fa0d870146d87f59cb4d319c5b895028`  
		Last Modified: Wed, 21 Dec 2022 16:56:39 GMT  
		Size: 1.5 KB (1479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e94d73593abc9542a40f6e2f989f35a2bebbb21e554c4d2452cee59089701ca5`  
		Last Modified: Wed, 21 Dec 2022 16:56:39 GMT  
		Size: 1.4 MB (1383619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f3795d41125166e2051354d7af4622abe6b7610551670476d49ad99c372bad6`  
		Last Modified: Wed, 21 Dec 2022 16:56:39 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-standalone` - linux; arm64 variant v8

```console
$ docker pull adminer@sha256:2e15c1b18293cc812ca73063a33ca295e6e5b4011ab43006f371bf3d63f7a387
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.0 MB (94046599 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f2678931127cd62d7af0ee195d7008f84b549fb9374257d1696f7cc5c9dab049`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 21 Dec 2022 01:39:40 GMT
ADD file:5bbdc914ec8ed60ac85293e88ee1aafc3f0290762e320fc86dc9d79fa201834e in / 
# Wed, 21 Dec 2022 01:39:41 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 02:01:54 GMT
STOPSIGNAL SIGINT
# Wed, 21 Dec 2022 02:02:11 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 02:02:12 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 21 Dec 2022 02:02:12 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 21 Dec 2022 02:02:13 GMT
WORKDIR /var/www/html
# Wed, 21 Dec 2022 02:02:13 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 21 Dec 2022 02:02:13 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 21 Dec 2022 02:02:13 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 21 Dec 2022 02:02:13 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 21 Dec 2022 02:02:23 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 21 Dec 2022 02:02:24 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 21 Dec 2022 02:02:24 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 21 Dec 2022 02:02:24 GMT
USER adminer
# Wed, 21 Dec 2022 02:02:24 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 21 Dec 2022 02:02:24 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:c3e6129b48b69d14c5e7a5605e2b94003fb71aac82eac46b8689f5b8007af2c5`  
		Last Modified: Wed, 21 Dec 2022 01:42:49 GMT  
		Size: 53.7 MB (53681797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:235cb929f19f47af31496a0a93a9cb1fd8f5104f0d34a160f4d2e4d6b9463df1`  
		Last Modified: Wed, 21 Dec 2022 02:02:59 GMT  
		Size: 39.0 MB (38976852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a72d5ac588c6b24f2d8a511e934c2745420b4536a9fa914031e10c9d384efd2b`  
		Last Modified: Wed, 21 Dec 2022 02:02:52 GMT  
		Size: 392.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c1912d1c0826d94d3aa328472384e502a58e992b77df780de62bbe9ba9f744e`  
		Last Modified: Wed, 21 Dec 2022 02:02:52 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f6d91a33867afb4cdea48a709f3cd43416c387bbf8a96e04840822e05a249eb`  
		Last Modified: Wed, 21 Dec 2022 02:02:52 GMT  
		Size: 1.5 KB (1481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a85debe3d62cce517ab60af785fce8ae30d5633d41e755d25700acfaa96f427`  
		Last Modified: Wed, 21 Dec 2022 02:02:53 GMT  
		Size: 1.4 MB (1383704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c707a54ab9eee88dee88a920652b121430b0f93f2599e1f3d29cd8ee7f91a359`  
		Last Modified: Wed, 21 Dec 2022 02:02:52 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-standalone` - linux; 386

```console
$ docker pull adminer@sha256:d219efb2aecebb6bd16280905d0c7ff80b18ad7269350fec6bd034d2a093976d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.7 MB (96663116 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a504b1b6ca371056530865e9620cc9e4dabcd05dd93ab1f5b1dc2092bf6656e2`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 21 Dec 2022 01:39:08 GMT
ADD file:10d2f443f55d8ba9512899b3dff08f6e9a6c7ca096f407e3477e9798e1063785 in / 
# Wed, 21 Dec 2022 01:39:09 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 02:04:14 GMT
STOPSIGNAL SIGINT
# Wed, 21 Dec 2022 02:04:35 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 02:04:36 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 21 Dec 2022 02:04:37 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 21 Dec 2022 02:04:38 GMT
WORKDIR /var/www/html
# Wed, 21 Dec 2022 02:04:40 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 21 Dec 2022 02:04:40 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 21 Dec 2022 02:04:41 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 21 Dec 2022 02:04:42 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 21 Dec 2022 02:04:55 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 21 Dec 2022 02:04:57 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 21 Dec 2022 02:04:57 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 21 Dec 2022 02:04:58 GMT
USER adminer
# Wed, 21 Dec 2022 02:04:59 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 21 Dec 2022 02:05:00 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:bde501e1d960005aee2bdf2fc8c89b26bf694dace8740c72deda4d7705995ab7`  
		Last Modified: Wed, 21 Dec 2022 01:44:18 GMT  
		Size: 56.0 MB (56005267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd60bbc5dc31d7ec1db0a2fbd068c29f7583f7d3e2d0599f0706680ce602ee9d`  
		Last Modified: Wed, 21 Dec 2022 02:06:03 GMT  
		Size: 39.3 MB (39269700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b30e5dcb4252f7f6ded0a9c044209070412dbf7df3daab7e7343bc6bf568fe67`  
		Last Modified: Wed, 21 Dec 2022 02:05:50 GMT  
		Size: 394.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:387e2851bc00ff07433e8e9d3d12cdc6590937cbf4a9de8a035771e386a0e3c4`  
		Last Modified: Wed, 21 Dec 2022 02:05:50 GMT  
		Size: 1.7 KB (1718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c04056306aff55b02341e716626152ea622c4326e3f31a4a39bce3d631152fea`  
		Last Modified: Wed, 21 Dec 2022 02:05:50 GMT  
		Size: 1.5 KB (1478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31f79e3e185cbecc304f97fe83e64bc102e782154ed533744186d41a6de680fb`  
		Last Modified: Wed, 21 Dec 2022 02:05:51 GMT  
		Size: 1.4 MB (1384066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce0359a7ffb52c577cc47d0136aeed97a19a7e826d80ebb7b304977f271a6f7d`  
		Last Modified: Wed, 21 Dec 2022 02:05:51 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-standalone` - linux; mips64le

```console
$ docker pull adminer@sha256:74a7ae91c85961c3ad967ae1cf25d79b8d7a69a6668843b885aebcc169a7f88f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.3 MB (92326851 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0992a9b14a478d0bfd67839ed2e77e40a770492ebd4daa67c6141cd734519bb1`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Tue, 06 Dec 2022 01:54:55 GMT
ADD file:09d48994a41c54566f7123db033773e6246c0703a518af76843198196cd39645 in / 
# Tue, 06 Dec 2022 01:55:00 GMT
CMD ["bash"]
# Sat, 17 Dec 2022 01:31:42 GMT
STOPSIGNAL SIGINT
# Sat, 17 Dec 2022 01:33:37 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Sat, 17 Dec 2022 01:33:43 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Sat, 17 Dec 2022 01:33:49 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Sat, 17 Dec 2022 01:33:53 GMT
WORKDIR /var/www/html
# Sat, 17 Dec 2022 01:33:56 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Sat, 17 Dec 2022 01:33:59 GMT
ENV ADMINER_VERSION=4.8.1
# Sat, 17 Dec 2022 01:34:02 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Sat, 17 Dec 2022 01:34:05 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Sat, 17 Dec 2022 01:34:57 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 17 Dec 2022 01:35:00 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Sat, 17 Dec 2022 01:35:03 GMT
ENTRYPOINT ["entrypoint.sh"]
# Sat, 17 Dec 2022 01:35:06 GMT
USER adminer
# Sat, 17 Dec 2022 01:35:09 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Sat, 17 Dec 2022 01:35:13 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:acb57a81743c28ead1a32571c107ac15cd970593fea4f2954b57f22e6bbad1d0`  
		Last Modified: Tue, 06 Dec 2022 02:02:59 GMT  
		Size: 53.3 MB (53260631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16a0a73e4e15363c91b94686e7609b1d84bd3ab5f4c13b2302e76c23e58ca18f`  
		Last Modified: Sat, 17 Dec 2022 01:38:30 GMT  
		Size: 37.7 MB (37676049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8aebeb122c3b2bc8c5262621178cece53cdab93feb29828240f598aa1c86637`  
		Last Modified: Sat, 17 Dec 2022 01:38:02 GMT  
		Size: 395.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3c1363529deb53f7595176aa5b55b04ab1cdf841a6cd3cdb88c41d6ec75615f`  
		Last Modified: Sat, 17 Dec 2022 01:38:02 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0923c943bb7440a1b68c2494f1f23c0a3199d4d3a6cdb87bdca8067acfbe4d4`  
		Last Modified: Sat, 17 Dec 2022 01:38:02 GMT  
		Size: 1.5 KB (1485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47a69745dad2c95e6d8ff413ca73cc902100c3848af39c316ae44ec375f8aae7`  
		Last Modified: Sat, 17 Dec 2022 01:38:03 GMT  
		Size: 1.4 MB (1386065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2548a3e7b136720a8c94faa9137694506f95bcf701a80d8b49486c2a3be6205b`  
		Last Modified: Sat, 17 Dec 2022 01:38:02 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-standalone` - linux; ppc64le

```console
$ docker pull adminer@sha256:86fbf5aa76cfa4052c3d9bf35b81e34daf0fb53fbc674d612c071ca9a60de5ce
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.9 MB (100903714 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:075df6bcff3df963b2eec2efff06fef0b4f316e1751a5ebc98880754503bcf54`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 21 Dec 2022 01:17:21 GMT
ADD file:c95bdb0df70fa9ce48b31a7ceb8a7be0c5b925efcf01c43595868b86994dc192 in / 
# Wed, 21 Dec 2022 01:17:25 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 05:10:17 GMT
STOPSIGNAL SIGINT
# Wed, 21 Dec 2022 05:11:02 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 05:11:05 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 21 Dec 2022 05:11:07 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 21 Dec 2022 05:11:07 GMT
WORKDIR /var/www/html
# Wed, 21 Dec 2022 05:11:07 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 21 Dec 2022 05:11:08 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 21 Dec 2022 05:11:08 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 21 Dec 2022 05:11:09 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 21 Dec 2022 05:11:31 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 21 Dec 2022 05:11:31 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 21 Dec 2022 05:11:32 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 21 Dec 2022 05:11:32 GMT
USER adminer
# Wed, 21 Dec 2022 05:11:32 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 21 Dec 2022 05:11:33 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:542880f4d15404af17d342ecbb76bb92724fc7cb8a91a5e18f26bd8f8811a38a`  
		Last Modified: Wed, 21 Dec 2022 01:22:46 GMT  
		Size: 58.9 MB (58897040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8c91d3a2eff19ff3291563333f250447b70f82929a98b439e9253b9d8909332`  
		Last Modified: Wed, 21 Dec 2022 05:12:53 GMT  
		Size: 40.6 MB (40618582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1fc5014e613c79f385d0565b105dfdc45badae00ab5a50f9b06955eb34e874d`  
		Last Modified: Wed, 21 Dec 2022 05:12:39 GMT  
		Size: 394.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc90d97148640f4f164e3dc4b1f043c6ba7d8b5cddd21ede8a947339a13e3c3f`  
		Last Modified: Wed, 21 Dec 2022 05:12:39 GMT  
		Size: 1.9 KB (1879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdfe2d4e5fb66793ea99cc5959183331088d985dc203754a30a8bf6bbffb186a`  
		Last Modified: Wed, 21 Dec 2022 05:12:39 GMT  
		Size: 1.5 KB (1482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0da8c96b4d9b013ebbf00af4b8693e634764cf159be7af73d3152403cabe71e5`  
		Last Modified: Wed, 21 Dec 2022 05:12:40 GMT  
		Size: 1.4 MB (1383844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:061e859636ca9e27f80e25b38a893f2e38d08dd68c7a53bc8fb9f428dfb0f328`  
		Last Modified: Wed, 21 Dec 2022 05:12:39 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-standalone` - linux; s390x

```console
$ docker pull adminer@sha256:4ad639f239b5117cf7381d37948390122d8f514592dade423c1fbdc4870c04b4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.4 MB (93401988 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac7114a00edb645cd010878538757f757f872e25c530cb9159f5bc03cc191726`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 21 Dec 2022 01:42:51 GMT
ADD file:22c4f2d41083ce4433bec4a71e7e6ddc5bec8e44e9cf2c9f93d0874b5b4de7c3 in / 
# Wed, 21 Dec 2022 01:42:54 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 02:06:42 GMT
STOPSIGNAL SIGINT
# Wed, 21 Dec 2022 02:07:51 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 02:08:00 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 21 Dec 2022 02:08:02 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 21 Dec 2022 02:08:03 GMT
WORKDIR /var/www/html
# Wed, 21 Dec 2022 02:08:04 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 21 Dec 2022 02:08:04 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 21 Dec 2022 02:08:05 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 21 Dec 2022 02:08:06 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 21 Dec 2022 02:08:33 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 21 Dec 2022 02:08:33 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 21 Dec 2022 02:08:34 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 21 Dec 2022 02:08:35 GMT
USER adminer
# Wed, 21 Dec 2022 02:08:35 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 21 Dec 2022 02:08:36 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:7f45294776f4c97d23f8dbfca98d4b57701b478eedfcb154a7e7dc6d6954ba44`  
		Last Modified: Wed, 21 Dec 2022 01:48:50 GMT  
		Size: 53.3 MB (53258472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8610ee81c430b6503a5ee2d7cc451175bdfc868fc17ef5a675b43679da433867`  
		Last Modified: Wed, 21 Dec 2022 02:10:03 GMT  
		Size: 38.8 MB (38755148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:211b726eee70a0c5ff85337d1e98c7987025435a41ca5421f47d96fc164b5b27`  
		Last Modified: Wed, 21 Dec 2022 02:09:56 GMT  
		Size: 395.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c6a1fa2154f900c32f87164afe347f0dddbb7a641dc81b7fc436b1d15a5349d`  
		Last Modified: Wed, 21 Dec 2022 02:09:56 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e030c793dfbf87ef1f5dbbecd22117bcf1695eb293e41bca267fb29d0e98d59d`  
		Last Modified: Wed, 21 Dec 2022 02:09:56 GMT  
		Size: 1.5 KB (1478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:965c9f68e6765f8a5967198527ce6ff7bf0646cab60aa30ecef97747554c0869`  
		Last Modified: Wed, 21 Dec 2022 02:09:56 GMT  
		Size: 1.4 MB (1384122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d34b801ca3351132a2f2914bc4ef3ca0f91a2c87c2b42fce3662fd5f20593aea`  
		Last Modified: Wed, 21 Dec 2022 02:09:56 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `adminer:4.8.1`

```console
$ docker pull adminer@sha256:895823d11ab87b3ef3db1230b33d9347b0c4fd58e6188906af37b3e7353f383f
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
$ docker pull adminer@sha256:11d6176cead328bcc234f740d98dccda987d03c17d77e03bdceb508c9d35ba30
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.6 MB (95639696 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c207e90c34520f27508ac0a18405256f981ecb45aae2baa2835c91a8f1963f0a`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 21 Dec 2022 01:20:21 GMT
ADD file:c13b430c8699df107ffd9ea5230b92238bc037a8e1cbbe35d6ab664941d575da in / 
# Wed, 21 Dec 2022 01:20:22 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 01:43:34 GMT
STOPSIGNAL SIGINT
# Wed, 21 Dec 2022 01:43:57 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 01:43:58 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 21 Dec 2022 01:43:59 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 21 Dec 2022 01:43:59 GMT
WORKDIR /var/www/html
# Wed, 21 Dec 2022 01:43:59 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 21 Dec 2022 01:43:59 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 21 Dec 2022 01:43:59 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 21 Dec 2022 01:43:59 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 21 Dec 2022 01:44:12 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 21 Dec 2022 01:44:12 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 21 Dec 2022 01:44:12 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 21 Dec 2022 01:44:12 GMT
USER adminer
# Wed, 21 Dec 2022 01:44:12 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 21 Dec 2022 01:44:12 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:32de3c850997ce03b6ff4ae8fb00b34b9d7d7f9a35bfcdb8538e22cc7b77c29d`  
		Last Modified: Wed, 21 Dec 2022 01:24:10 GMT  
		Size: 55.0 MB (55025166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bddad460143b31cc21fc89d836e6d417bb718a19c27f93eb137aebd91b79660`  
		Last Modified: Wed, 21 Dec 2022 01:44:51 GMT  
		Size: 39.2 MB (39226473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bf0beaa0412c7e762322b7311a449203a96c1e115d99efca0dddce016279e6a`  
		Last Modified: Wed, 21 Dec 2022 01:44:43 GMT  
		Size: 394.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e7ee08ea648165938f5fde9ae603f33b34b10c2d4ad2e40ea8c04913db12b65`  
		Last Modified: Wed, 21 Dec 2022 01:44:43 GMT  
		Size: 1.9 KB (1888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd9f958670d2c87349fd96a19d4254adbc404b54b3911c6962d9119d1a6fe901`  
		Last Modified: Wed, 21 Dec 2022 01:44:43 GMT  
		Size: 1.5 KB (1477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:292984a5d9c1d2f389b01937cbdf2a19e8b9de4ed6719500f1310467b1a19ff5`  
		Last Modified: Wed, 21 Dec 2022 01:44:44 GMT  
		Size: 1.4 MB (1383807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20a148ad3aa6178c7d0e684fcbc70c4ca4ba27ea5f13560aef5219a63b2b6874`  
		Last Modified: Wed, 21 Dec 2022 01:44:43 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1` - linux; arm variant v5

```console
$ docker pull adminer@sha256:50640fef3243132e1ea5d5081f834e0ca156c8264c0b0441a43492f4a4eeca23
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.9 MB (90901373 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:250a1b3ad0e6461afc53655c14f3a5b1378d898200c7bdef2f11ad58335fe9a2`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 21 Dec 2022 01:48:53 GMT
ADD file:81ccc74e0ea343972e2f3f46d2da7e9b808d9718be44d4afa7bec6904b7ab9c6 in / 
# Wed, 21 Dec 2022 01:48:55 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 02:12:35 GMT
STOPSIGNAL SIGINT
# Wed, 21 Dec 2022 02:13:07 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 02:13:09 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 21 Dec 2022 02:13:10 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 21 Dec 2022 02:13:10 GMT
WORKDIR /var/www/html
# Wed, 21 Dec 2022 02:13:10 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 21 Dec 2022 02:13:10 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 21 Dec 2022 02:13:10 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 21 Dec 2022 02:13:10 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 21 Dec 2022 02:13:27 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 21 Dec 2022 02:13:27 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 21 Dec 2022 02:13:27 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 21 Dec 2022 02:13:27 GMT
USER adminer
# Wed, 21 Dec 2022 02:13:27 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 21 Dec 2022 02:13:27 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:89b6e4f9f2f811282495a047e873c20d6ac2d53c72ad576a6907b1449eb3e635`  
		Last Modified: Wed, 21 Dec 2022 01:53:30 GMT  
		Size: 52.5 MB (52529974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2473783a5bf521f1fdf370edfbbd3a71c7d41bd6ad586832334a5359d21e0937`  
		Last Modified: Wed, 21 Dec 2022 02:14:50 GMT  
		Size: 37.0 MB (36983598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fb144c6fa4674d630705477694c2b1a78efcb47a43b11b84d11420c6672d849`  
		Last Modified: Wed, 21 Dec 2022 02:14:41 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7d2eaadeb68edbb519fcd0f769e3e17f2744670df98e1f42b2dd32755e43260`  
		Last Modified: Wed, 21 Dec 2022 02:14:41 GMT  
		Size: 1.8 KB (1840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57c2b47fd023120badcfed4eb901caaff2b0fb6b5d48de329e15232469b9af23`  
		Last Modified: Wed, 21 Dec 2022 02:14:41 GMT  
		Size: 1.5 KB (1481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54fcbf1f604d9098ea8ed2239603e5aa978d84db1258c72c4a54a6aa095ec76f`  
		Last Modified: Wed, 21 Dec 2022 02:14:41 GMT  
		Size: 1.4 MB (1383596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:216e1a8363d45d45df8c6cbfe9f7ee9909da57c723cd447b01a248fb042840f3`  
		Last Modified: Wed, 21 Dec 2022 02:14:41 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1` - linux; arm variant v7

```console
$ docker pull adminer@sha256:667b9904f45244f6db8f25daad4eea200d6c4a4f91c68de564a5caf5a4c6a5c5
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.5 MB (87525670 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4da555d48a0530a78c590fbbf78d89a6283e3bf8436c4028fc44739c58ed9fd4`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 21 Dec 2022 01:58:09 GMT
ADD file:4b6f71680de34554595f062f9e52037b48edf19ca8f34c75877caa85c42caad3 in / 
# Wed, 21 Dec 2022 01:58:10 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 16:55:05 GMT
STOPSIGNAL SIGINT
# Wed, 21 Dec 2022 16:55:27 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 16:55:28 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 21 Dec 2022 16:55:29 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 21 Dec 2022 16:55:29 GMT
WORKDIR /var/www/html
# Wed, 21 Dec 2022 16:55:29 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 21 Dec 2022 16:55:29 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 21 Dec 2022 16:55:29 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 21 Dec 2022 16:55:29 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 21 Dec 2022 16:55:42 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 21 Dec 2022 16:55:42 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 21 Dec 2022 16:55:42 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 21 Dec 2022 16:55:42 GMT
USER adminer
# Wed, 21 Dec 2022 16:55:42 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 21 Dec 2022 16:55:42 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:706bb1d74512e1fb9ba97aa9212a32d07726fbfe77e4c7e609406d2065418f57`  
		Last Modified: Wed, 21 Dec 2022 02:04:37 GMT  
		Size: 50.2 MB (50190771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a1c5cd5ac0e733e02567c893f1028628f441423281df1c54fa1042b317bb758`  
		Last Modified: Wed, 21 Dec 2022 16:56:48 GMT  
		Size: 35.9 MB (35947077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3d69909ab6c9fd65668b2d644bbb5375f5617c8bba9e82704145b53e895ad98`  
		Last Modified: Wed, 21 Dec 2022 16:56:39 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be622d99b39d413b273b3c6344f0cf7b97883297c9e7fb52951cca9bafd33f3a`  
		Last Modified: Wed, 21 Dec 2022 16:56:39 GMT  
		Size: 1.8 KB (1840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:546d6a7c782f341de9ea0c0c9aa227a5fa0d870146d87f59cb4d319c5b895028`  
		Last Modified: Wed, 21 Dec 2022 16:56:39 GMT  
		Size: 1.5 KB (1479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e94d73593abc9542a40f6e2f989f35a2bebbb21e554c4d2452cee59089701ca5`  
		Last Modified: Wed, 21 Dec 2022 16:56:39 GMT  
		Size: 1.4 MB (1383619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f3795d41125166e2051354d7af4622abe6b7610551670476d49ad99c372bad6`  
		Last Modified: Wed, 21 Dec 2022 16:56:39 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1` - linux; arm64 variant v8

```console
$ docker pull adminer@sha256:2e15c1b18293cc812ca73063a33ca295e6e5b4011ab43006f371bf3d63f7a387
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.0 MB (94046599 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f2678931127cd62d7af0ee195d7008f84b549fb9374257d1696f7cc5c9dab049`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 21 Dec 2022 01:39:40 GMT
ADD file:5bbdc914ec8ed60ac85293e88ee1aafc3f0290762e320fc86dc9d79fa201834e in / 
# Wed, 21 Dec 2022 01:39:41 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 02:01:54 GMT
STOPSIGNAL SIGINT
# Wed, 21 Dec 2022 02:02:11 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 02:02:12 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 21 Dec 2022 02:02:12 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 21 Dec 2022 02:02:13 GMT
WORKDIR /var/www/html
# Wed, 21 Dec 2022 02:02:13 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 21 Dec 2022 02:02:13 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 21 Dec 2022 02:02:13 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 21 Dec 2022 02:02:13 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 21 Dec 2022 02:02:23 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 21 Dec 2022 02:02:24 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 21 Dec 2022 02:02:24 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 21 Dec 2022 02:02:24 GMT
USER adminer
# Wed, 21 Dec 2022 02:02:24 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 21 Dec 2022 02:02:24 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:c3e6129b48b69d14c5e7a5605e2b94003fb71aac82eac46b8689f5b8007af2c5`  
		Last Modified: Wed, 21 Dec 2022 01:42:49 GMT  
		Size: 53.7 MB (53681797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:235cb929f19f47af31496a0a93a9cb1fd8f5104f0d34a160f4d2e4d6b9463df1`  
		Last Modified: Wed, 21 Dec 2022 02:02:59 GMT  
		Size: 39.0 MB (38976852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a72d5ac588c6b24f2d8a511e934c2745420b4536a9fa914031e10c9d384efd2b`  
		Last Modified: Wed, 21 Dec 2022 02:02:52 GMT  
		Size: 392.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c1912d1c0826d94d3aa328472384e502a58e992b77df780de62bbe9ba9f744e`  
		Last Modified: Wed, 21 Dec 2022 02:02:52 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f6d91a33867afb4cdea48a709f3cd43416c387bbf8a96e04840822e05a249eb`  
		Last Modified: Wed, 21 Dec 2022 02:02:52 GMT  
		Size: 1.5 KB (1481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a85debe3d62cce517ab60af785fce8ae30d5633d41e755d25700acfaa96f427`  
		Last Modified: Wed, 21 Dec 2022 02:02:53 GMT  
		Size: 1.4 MB (1383704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c707a54ab9eee88dee88a920652b121430b0f93f2599e1f3d29cd8ee7f91a359`  
		Last Modified: Wed, 21 Dec 2022 02:02:52 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1` - linux; 386

```console
$ docker pull adminer@sha256:d219efb2aecebb6bd16280905d0c7ff80b18ad7269350fec6bd034d2a093976d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.7 MB (96663116 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a504b1b6ca371056530865e9620cc9e4dabcd05dd93ab1f5b1dc2092bf6656e2`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 21 Dec 2022 01:39:08 GMT
ADD file:10d2f443f55d8ba9512899b3dff08f6e9a6c7ca096f407e3477e9798e1063785 in / 
# Wed, 21 Dec 2022 01:39:09 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 02:04:14 GMT
STOPSIGNAL SIGINT
# Wed, 21 Dec 2022 02:04:35 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 02:04:36 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 21 Dec 2022 02:04:37 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 21 Dec 2022 02:04:38 GMT
WORKDIR /var/www/html
# Wed, 21 Dec 2022 02:04:40 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 21 Dec 2022 02:04:40 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 21 Dec 2022 02:04:41 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 21 Dec 2022 02:04:42 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 21 Dec 2022 02:04:55 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 21 Dec 2022 02:04:57 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 21 Dec 2022 02:04:57 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 21 Dec 2022 02:04:58 GMT
USER adminer
# Wed, 21 Dec 2022 02:04:59 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 21 Dec 2022 02:05:00 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:bde501e1d960005aee2bdf2fc8c89b26bf694dace8740c72deda4d7705995ab7`  
		Last Modified: Wed, 21 Dec 2022 01:44:18 GMT  
		Size: 56.0 MB (56005267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd60bbc5dc31d7ec1db0a2fbd068c29f7583f7d3e2d0599f0706680ce602ee9d`  
		Last Modified: Wed, 21 Dec 2022 02:06:03 GMT  
		Size: 39.3 MB (39269700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b30e5dcb4252f7f6ded0a9c044209070412dbf7df3daab7e7343bc6bf568fe67`  
		Last Modified: Wed, 21 Dec 2022 02:05:50 GMT  
		Size: 394.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:387e2851bc00ff07433e8e9d3d12cdc6590937cbf4a9de8a035771e386a0e3c4`  
		Last Modified: Wed, 21 Dec 2022 02:05:50 GMT  
		Size: 1.7 KB (1718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c04056306aff55b02341e716626152ea622c4326e3f31a4a39bce3d631152fea`  
		Last Modified: Wed, 21 Dec 2022 02:05:50 GMT  
		Size: 1.5 KB (1478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31f79e3e185cbecc304f97fe83e64bc102e782154ed533744186d41a6de680fb`  
		Last Modified: Wed, 21 Dec 2022 02:05:51 GMT  
		Size: 1.4 MB (1384066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce0359a7ffb52c577cc47d0136aeed97a19a7e826d80ebb7b304977f271a6f7d`  
		Last Modified: Wed, 21 Dec 2022 02:05:51 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1` - linux; mips64le

```console
$ docker pull adminer@sha256:74a7ae91c85961c3ad967ae1cf25d79b8d7a69a6668843b885aebcc169a7f88f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.3 MB (92326851 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0992a9b14a478d0bfd67839ed2e77e40a770492ebd4daa67c6141cd734519bb1`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Tue, 06 Dec 2022 01:54:55 GMT
ADD file:09d48994a41c54566f7123db033773e6246c0703a518af76843198196cd39645 in / 
# Tue, 06 Dec 2022 01:55:00 GMT
CMD ["bash"]
# Sat, 17 Dec 2022 01:31:42 GMT
STOPSIGNAL SIGINT
# Sat, 17 Dec 2022 01:33:37 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Sat, 17 Dec 2022 01:33:43 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Sat, 17 Dec 2022 01:33:49 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Sat, 17 Dec 2022 01:33:53 GMT
WORKDIR /var/www/html
# Sat, 17 Dec 2022 01:33:56 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Sat, 17 Dec 2022 01:33:59 GMT
ENV ADMINER_VERSION=4.8.1
# Sat, 17 Dec 2022 01:34:02 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Sat, 17 Dec 2022 01:34:05 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Sat, 17 Dec 2022 01:34:57 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 17 Dec 2022 01:35:00 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Sat, 17 Dec 2022 01:35:03 GMT
ENTRYPOINT ["entrypoint.sh"]
# Sat, 17 Dec 2022 01:35:06 GMT
USER adminer
# Sat, 17 Dec 2022 01:35:09 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Sat, 17 Dec 2022 01:35:13 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:acb57a81743c28ead1a32571c107ac15cd970593fea4f2954b57f22e6bbad1d0`  
		Last Modified: Tue, 06 Dec 2022 02:02:59 GMT  
		Size: 53.3 MB (53260631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16a0a73e4e15363c91b94686e7609b1d84bd3ab5f4c13b2302e76c23e58ca18f`  
		Last Modified: Sat, 17 Dec 2022 01:38:30 GMT  
		Size: 37.7 MB (37676049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8aebeb122c3b2bc8c5262621178cece53cdab93feb29828240f598aa1c86637`  
		Last Modified: Sat, 17 Dec 2022 01:38:02 GMT  
		Size: 395.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3c1363529deb53f7595176aa5b55b04ab1cdf841a6cd3cdb88c41d6ec75615f`  
		Last Modified: Sat, 17 Dec 2022 01:38:02 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0923c943bb7440a1b68c2494f1f23c0a3199d4d3a6cdb87bdca8067acfbe4d4`  
		Last Modified: Sat, 17 Dec 2022 01:38:02 GMT  
		Size: 1.5 KB (1485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47a69745dad2c95e6d8ff413ca73cc902100c3848af39c316ae44ec375f8aae7`  
		Last Modified: Sat, 17 Dec 2022 01:38:03 GMT  
		Size: 1.4 MB (1386065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2548a3e7b136720a8c94faa9137694506f95bcf701a80d8b49486c2a3be6205b`  
		Last Modified: Sat, 17 Dec 2022 01:38:02 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1` - linux; ppc64le

```console
$ docker pull adminer@sha256:86fbf5aa76cfa4052c3d9bf35b81e34daf0fb53fbc674d612c071ca9a60de5ce
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.9 MB (100903714 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:075df6bcff3df963b2eec2efff06fef0b4f316e1751a5ebc98880754503bcf54`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 21 Dec 2022 01:17:21 GMT
ADD file:c95bdb0df70fa9ce48b31a7ceb8a7be0c5b925efcf01c43595868b86994dc192 in / 
# Wed, 21 Dec 2022 01:17:25 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 05:10:17 GMT
STOPSIGNAL SIGINT
# Wed, 21 Dec 2022 05:11:02 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 05:11:05 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 21 Dec 2022 05:11:07 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 21 Dec 2022 05:11:07 GMT
WORKDIR /var/www/html
# Wed, 21 Dec 2022 05:11:07 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 21 Dec 2022 05:11:08 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 21 Dec 2022 05:11:08 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 21 Dec 2022 05:11:09 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 21 Dec 2022 05:11:31 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 21 Dec 2022 05:11:31 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 21 Dec 2022 05:11:32 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 21 Dec 2022 05:11:32 GMT
USER adminer
# Wed, 21 Dec 2022 05:11:32 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 21 Dec 2022 05:11:33 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:542880f4d15404af17d342ecbb76bb92724fc7cb8a91a5e18f26bd8f8811a38a`  
		Last Modified: Wed, 21 Dec 2022 01:22:46 GMT  
		Size: 58.9 MB (58897040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8c91d3a2eff19ff3291563333f250447b70f82929a98b439e9253b9d8909332`  
		Last Modified: Wed, 21 Dec 2022 05:12:53 GMT  
		Size: 40.6 MB (40618582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1fc5014e613c79f385d0565b105dfdc45badae00ab5a50f9b06955eb34e874d`  
		Last Modified: Wed, 21 Dec 2022 05:12:39 GMT  
		Size: 394.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc90d97148640f4f164e3dc4b1f043c6ba7d8b5cddd21ede8a947339a13e3c3f`  
		Last Modified: Wed, 21 Dec 2022 05:12:39 GMT  
		Size: 1.9 KB (1879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdfe2d4e5fb66793ea99cc5959183331088d985dc203754a30a8bf6bbffb186a`  
		Last Modified: Wed, 21 Dec 2022 05:12:39 GMT  
		Size: 1.5 KB (1482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0da8c96b4d9b013ebbf00af4b8693e634764cf159be7af73d3152403cabe71e5`  
		Last Modified: Wed, 21 Dec 2022 05:12:40 GMT  
		Size: 1.4 MB (1383844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:061e859636ca9e27f80e25b38a893f2e38d08dd68c7a53bc8fb9f428dfb0f328`  
		Last Modified: Wed, 21 Dec 2022 05:12:39 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1` - linux; s390x

```console
$ docker pull adminer@sha256:4ad639f239b5117cf7381d37948390122d8f514592dade423c1fbdc4870c04b4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.4 MB (93401988 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac7114a00edb645cd010878538757f757f872e25c530cb9159f5bc03cc191726`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 21 Dec 2022 01:42:51 GMT
ADD file:22c4f2d41083ce4433bec4a71e7e6ddc5bec8e44e9cf2c9f93d0874b5b4de7c3 in / 
# Wed, 21 Dec 2022 01:42:54 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 02:06:42 GMT
STOPSIGNAL SIGINT
# Wed, 21 Dec 2022 02:07:51 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 02:08:00 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 21 Dec 2022 02:08:02 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 21 Dec 2022 02:08:03 GMT
WORKDIR /var/www/html
# Wed, 21 Dec 2022 02:08:04 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 21 Dec 2022 02:08:04 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 21 Dec 2022 02:08:05 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 21 Dec 2022 02:08:06 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 21 Dec 2022 02:08:33 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 21 Dec 2022 02:08:33 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 21 Dec 2022 02:08:34 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 21 Dec 2022 02:08:35 GMT
USER adminer
# Wed, 21 Dec 2022 02:08:35 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 21 Dec 2022 02:08:36 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:7f45294776f4c97d23f8dbfca98d4b57701b478eedfcb154a7e7dc6d6954ba44`  
		Last Modified: Wed, 21 Dec 2022 01:48:50 GMT  
		Size: 53.3 MB (53258472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8610ee81c430b6503a5ee2d7cc451175bdfc868fc17ef5a675b43679da433867`  
		Last Modified: Wed, 21 Dec 2022 02:10:03 GMT  
		Size: 38.8 MB (38755148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:211b726eee70a0c5ff85337d1e98c7987025435a41ca5421f47d96fc164b5b27`  
		Last Modified: Wed, 21 Dec 2022 02:09:56 GMT  
		Size: 395.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c6a1fa2154f900c32f87164afe347f0dddbb7a641dc81b7fc436b1d15a5349d`  
		Last Modified: Wed, 21 Dec 2022 02:09:56 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e030c793dfbf87ef1f5dbbecd22117bcf1695eb293e41bca267fb29d0e98d59d`  
		Last Modified: Wed, 21 Dec 2022 02:09:56 GMT  
		Size: 1.5 KB (1478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:965c9f68e6765f8a5967198527ce6ff7bf0646cab60aa30ecef97747554c0869`  
		Last Modified: Wed, 21 Dec 2022 02:09:56 GMT  
		Size: 1.4 MB (1384122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d34b801ca3351132a2f2914bc4ef3ca0f91a2c87c2b42fce3662fd5f20593aea`  
		Last Modified: Wed, 21 Dec 2022 02:09:56 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `adminer:4.8.1-fastcgi`

```console
$ docker pull adminer@sha256:37807622785148a8a96b6b2d9314e7db8e7202306531a9e674f9735b07ce17d3
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
$ docker pull adminer@sha256:1e1e6130a4906493f3dcda03ec0eb19eeec7d747868d8e7526583e93b90377ed
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.6 MB (95642424 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ec85d40ab3aa8923f6295358e72e000090652b9a26b7b9c7774d997a844e842`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Wed, 21 Dec 2022 01:20:21 GMT
ADD file:c13b430c8699df107ffd9ea5230b92238bc037a8e1cbbe35d6ab664941d575da in / 
# Wed, 21 Dec 2022 01:20:22 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 01:43:34 GMT
STOPSIGNAL SIGINT
# Wed, 21 Dec 2022 01:43:57 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 01:43:58 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 21 Dec 2022 01:44:15 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Wed, 21 Dec 2022 01:44:16 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 21 Dec 2022 01:44:16 GMT
WORKDIR /var/www/html
# Wed, 21 Dec 2022 01:44:16 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 21 Dec 2022 01:44:16 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 21 Dec 2022 01:44:16 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 21 Dec 2022 01:44:17 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 21 Dec 2022 01:44:28 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 21 Dec 2022 01:44:28 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 21 Dec 2022 01:44:28 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 21 Dec 2022 01:44:29 GMT
USER adminer
# Wed, 21 Dec 2022 01:44:29 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:32de3c850997ce03b6ff4ae8fb00b34b9d7d7f9a35bfcdb8538e22cc7b77c29d`  
		Last Modified: Wed, 21 Dec 2022 01:24:10 GMT  
		Size: 55.0 MB (55025166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bddad460143b31cc21fc89d836e6d417bb718a19c27f93eb137aebd91b79660`  
		Last Modified: Wed, 21 Dec 2022 01:44:51 GMT  
		Size: 39.2 MB (39226473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bf0beaa0412c7e762322b7311a449203a96c1e115d99efca0dddce016279e6a`  
		Last Modified: Wed, 21 Dec 2022 01:44:43 GMT  
		Size: 394.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e85c5399c00e75eb8dd783e68be98aeef85fb6e2e50ab17a1f3d0fb977496970`  
		Last Modified: Wed, 21 Dec 2022 01:45:09 GMT  
		Size: 2.7 KB (2712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fa2e6155707c0c71fe403f845f4a9061a2bba300a1a1c18f480f59742b9036a`  
		Last Modified: Wed, 21 Dec 2022 01:45:09 GMT  
		Size: 1.9 KB (1879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48c9c38ec5f03fab46adc653af92a4b0c326aa93c7533ff5e7c2166e3ef8cf40`  
		Last Modified: Wed, 21 Dec 2022 01:45:09 GMT  
		Size: 1.5 KB (1478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a19f8c5c89b7131c03f16fdc1f9c0c0bf07fbc0d9bfe1cecb756a290c47fbd6b`  
		Last Modified: Wed, 21 Dec 2022 01:45:10 GMT  
		Size: 1.4 MB (1383831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a5ef3fdf80e2ac647453715c908b46bb54a9310430fed3a3bb6e8f418740b8e`  
		Last Modified: Wed, 21 Dec 2022 01:45:09 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1-fastcgi` - linux; arm variant v5

```console
$ docker pull adminer@sha256:f6452248c81bf0aa2cecfa804a14cd9b14a2503be250138828d035b75e2896a9
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.9 MB (90904118 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d18173eb6830d6ef3ae8c8a231cb8ea70b230991680c62578ac47461b434c398`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Wed, 21 Dec 2022 01:48:53 GMT
ADD file:81ccc74e0ea343972e2f3f46d2da7e9b808d9718be44d4afa7bec6904b7ab9c6 in / 
# Wed, 21 Dec 2022 01:48:55 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 02:12:35 GMT
STOPSIGNAL SIGINT
# Wed, 21 Dec 2022 02:13:07 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 02:13:09 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 21 Dec 2022 02:13:39 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Wed, 21 Dec 2022 02:13:40 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 21 Dec 2022 02:13:41 GMT
WORKDIR /var/www/html
# Wed, 21 Dec 2022 02:13:41 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 21 Dec 2022 02:13:42 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 21 Dec 2022 02:13:42 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 21 Dec 2022 02:13:42 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 21 Dec 2022 02:14:02 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 21 Dec 2022 02:14:02 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 21 Dec 2022 02:14:02 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 21 Dec 2022 02:14:02 GMT
USER adminer
# Wed, 21 Dec 2022 02:14:03 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:89b6e4f9f2f811282495a047e873c20d6ac2d53c72ad576a6907b1449eb3e635`  
		Last Modified: Wed, 21 Dec 2022 01:53:30 GMT  
		Size: 52.5 MB (52529974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2473783a5bf521f1fdf370edfbbd3a71c7d41bd6ad586832334a5359d21e0937`  
		Last Modified: Wed, 21 Dec 2022 02:14:50 GMT  
		Size: 37.0 MB (36983598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fb144c6fa4674d630705477694c2b1a78efcb47a43b11b84d11420c6672d849`  
		Last Modified: Wed, 21 Dec 2022 02:14:41 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26063a58f85ffe38619444fe9e9ea1012e4e7fdb2b4d72cdcac7a8aae808f733`  
		Last Modified: Wed, 21 Dec 2022 02:15:15 GMT  
		Size: 2.7 KB (2710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41851614d9620c865a301e15f38ab0d4c8ddd9a1f4202edbf3a691d918884cf7`  
		Last Modified: Wed, 21 Dec 2022 02:15:15 GMT  
		Size: 1.8 KB (1839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ab4a9eecfe7e71f9ca3e31e0de304dbd42f4d4078f5feecb1c7c6f4f42005cc`  
		Last Modified: Wed, 21 Dec 2022 02:15:15 GMT  
		Size: 1.5 KB (1481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:606df83e76d99dd227ac689ddcd3e7f8434d06d4e46042bc2419167493a3b188`  
		Last Modified: Wed, 21 Dec 2022 02:15:15 GMT  
		Size: 1.4 MB (1383635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6018be7539eedb016a02d6429a6c60eaa072ee9ea161b1d74167953aa3a9de72`  
		Last Modified: Wed, 21 Dec 2022 02:15:15 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1-fastcgi` - linux; arm variant v7

```console
$ docker pull adminer@sha256:9928846ee8fb76c681b35c87ebfed49499f447a0c1c81393d30ab2bcba70a6c2
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.5 MB (87528433 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99681162737fb62edc07a8e79538b32ebe15b415a91f8e6c9e8d2c0f6f224b9a`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Wed, 21 Dec 2022 01:58:09 GMT
ADD file:4b6f71680de34554595f062f9e52037b48edf19ca8f34c75877caa85c42caad3 in / 
# Wed, 21 Dec 2022 01:58:10 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 16:55:05 GMT
STOPSIGNAL SIGINT
# Wed, 21 Dec 2022 16:55:27 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 16:55:28 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 21 Dec 2022 16:55:49 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Wed, 21 Dec 2022 16:55:50 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 21 Dec 2022 16:55:50 GMT
WORKDIR /var/www/html
# Wed, 21 Dec 2022 16:55:50 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 21 Dec 2022 16:55:50 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 21 Dec 2022 16:55:50 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 21 Dec 2022 16:55:50 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 21 Dec 2022 16:56:04 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 21 Dec 2022 16:56:04 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 21 Dec 2022 16:56:04 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 21 Dec 2022 16:56:04 GMT
USER adminer
# Wed, 21 Dec 2022 16:56:04 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:706bb1d74512e1fb9ba97aa9212a32d07726fbfe77e4c7e609406d2065418f57`  
		Last Modified: Wed, 21 Dec 2022 02:04:37 GMT  
		Size: 50.2 MB (50190771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a1c5cd5ac0e733e02567c893f1028628f441423281df1c54fa1042b317bb758`  
		Last Modified: Wed, 21 Dec 2022 16:56:48 GMT  
		Size: 35.9 MB (35947077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3d69909ab6c9fd65668b2d644bbb5375f5617c8bba9e82704145b53e895ad98`  
		Last Modified: Wed, 21 Dec 2022 16:56:39 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0e39a1a73560e658bd05d5621c5e241ea6c658eeb4d6d40fab42c2d0e049dd9`  
		Last Modified: Wed, 21 Dec 2022 16:57:11 GMT  
		Size: 2.7 KB (2707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:570ddb9aaf5affd1f0db7ce02160f1220f1f786028eb2dc3304d29faec9a812c`  
		Last Modified: Wed, 21 Dec 2022 16:57:11 GMT  
		Size: 1.8 KB (1841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5278a6d095ca223fab850a965a90f10b571dee63613450a5c305743288a3db7`  
		Last Modified: Wed, 21 Dec 2022 16:57:11 GMT  
		Size: 1.5 KB (1476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f0a1888014f0f3ae5844f8d80c0707d886f7e951a2583d43345fb59abe5e97c`  
		Last Modified: Wed, 21 Dec 2022 16:57:12 GMT  
		Size: 1.4 MB (1383680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6e719bcd08751a23a74658e85fc4e47ae42d98213576128a573499661a743b9`  
		Last Modified: Wed, 21 Dec 2022 16:57:11 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1-fastcgi` - linux; arm64 variant v8

```console
$ docker pull adminer@sha256:deace6e0488124187d0f03d131c3f503f66d5532f6cba7a2c9bbd9f4e92c9639
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.0 MB (94049324 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5eaa4905b3a6a204b45fc4e4608dc8de2ee6e3a8b386c2a8daed65b7ea308fa`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Wed, 21 Dec 2022 01:39:40 GMT
ADD file:5bbdc914ec8ed60ac85293e88ee1aafc3f0290762e320fc86dc9d79fa201834e in / 
# Wed, 21 Dec 2022 01:39:41 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 02:01:54 GMT
STOPSIGNAL SIGINT
# Wed, 21 Dec 2022 02:02:11 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 02:02:12 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 21 Dec 2022 02:02:27 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Wed, 21 Dec 2022 02:02:28 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 21 Dec 2022 02:02:28 GMT
WORKDIR /var/www/html
# Wed, 21 Dec 2022 02:02:28 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 21 Dec 2022 02:02:28 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 21 Dec 2022 02:02:28 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 21 Dec 2022 02:02:28 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 21 Dec 2022 02:02:38 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 21 Dec 2022 02:02:38 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 21 Dec 2022 02:02:38 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 21 Dec 2022 02:02:38 GMT
USER adminer
# Wed, 21 Dec 2022 02:02:38 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:c3e6129b48b69d14c5e7a5605e2b94003fb71aac82eac46b8689f5b8007af2c5`  
		Last Modified: Wed, 21 Dec 2022 01:42:49 GMT  
		Size: 53.7 MB (53681797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:235cb929f19f47af31496a0a93a9cb1fd8f5104f0d34a160f4d2e4d6b9463df1`  
		Last Modified: Wed, 21 Dec 2022 02:02:59 GMT  
		Size: 39.0 MB (38976852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a72d5ac588c6b24f2d8a511e934c2745420b4536a9fa914031e10c9d384efd2b`  
		Last Modified: Wed, 21 Dec 2022 02:02:52 GMT  
		Size: 392.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13819a4b0fdaaf0d610656691e268b84f62b9bc6f1978b10b2fd66d30bfc61a0`  
		Last Modified: Wed, 21 Dec 2022 02:03:18 GMT  
		Size: 2.7 KB (2705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e39e3b462a156c2eb8929e5b29025db6c8048ec880966c1e891e12db93bfb103`  
		Last Modified: Wed, 21 Dec 2022 02:03:18 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c2102a525d7aa1a32b03261d2429812840b08fab7cc2175e391f84857823539`  
		Last Modified: Wed, 21 Dec 2022 02:03:18 GMT  
		Size: 1.5 KB (1476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4364503e41b1e8f317d4c98b8da4b7d28551f47d554987462dfbc04169e893da`  
		Last Modified: Wed, 21 Dec 2022 02:03:19 GMT  
		Size: 1.4 MB (1383730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e279f93f23126fbc1db29d1577bf87115d79396ca7c78cb6b2bda1279cdaa269`  
		Last Modified: Wed, 21 Dec 2022 02:03:18 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1-fastcgi` - linux; 386

```console
$ docker pull adminer@sha256:9a434bc61ca7023a8f2c77a9d0958ab597cd69f03685202d1661614ba76c346f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.7 MB (96665821 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c32a28f670f6878d3ca957e9fc114d3736d77b40db0223160324a35254c19e3`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Wed, 21 Dec 2022 01:39:08 GMT
ADD file:10d2f443f55d8ba9512899b3dff08f6e9a6c7ca096f407e3477e9798e1063785 in / 
# Wed, 21 Dec 2022 01:39:09 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 02:04:14 GMT
STOPSIGNAL SIGINT
# Wed, 21 Dec 2022 02:04:35 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 02:04:36 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 21 Dec 2022 02:05:05 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Wed, 21 Dec 2022 02:05:06 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 21 Dec 2022 02:05:07 GMT
WORKDIR /var/www/html
# Wed, 21 Dec 2022 02:05:09 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 21 Dec 2022 02:05:09 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 21 Dec 2022 02:05:10 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 21 Dec 2022 02:05:11 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 21 Dec 2022 02:05:24 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 21 Dec 2022 02:05:25 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 21 Dec 2022 02:05:25 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 21 Dec 2022 02:05:26 GMT
USER adminer
# Wed, 21 Dec 2022 02:05:27 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:bde501e1d960005aee2bdf2fc8c89b26bf694dace8740c72deda4d7705995ab7`  
		Last Modified: Wed, 21 Dec 2022 01:44:18 GMT  
		Size: 56.0 MB (56005267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd60bbc5dc31d7ec1db0a2fbd068c29f7583f7d3e2d0599f0706680ce602ee9d`  
		Last Modified: Wed, 21 Dec 2022 02:06:03 GMT  
		Size: 39.3 MB (39269700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b30e5dcb4252f7f6ded0a9c044209070412dbf7df3daab7e7343bc6bf568fe67`  
		Last Modified: Wed, 21 Dec 2022 02:05:50 GMT  
		Size: 394.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44b71679c4856448b64de04f5a85f11611e00ec6255adf5430d19216fda4b172`  
		Last Modified: Wed, 21 Dec 2022 02:06:25 GMT  
		Size: 2.7 KB (2708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba4434a757058f98902edee00915212df3d942d3675e23589ab4b5b5ff27a41f`  
		Last Modified: Wed, 21 Dec 2022 02:06:24 GMT  
		Size: 1.7 KB (1718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b87eb7dde4067b918229c1df6d6f6890a97ab78c902accb2240718ff2d3e1145`  
		Last Modified: Wed, 21 Dec 2022 02:06:25 GMT  
		Size: 1.5 KB (1479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc82102410ace2a3805c07a9de9d7d5e319e8b7903eebcb983e7ac7c0f69b585`  
		Last Modified: Wed, 21 Dec 2022 02:06:25 GMT  
		Size: 1.4 MB (1384064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dafaed69f8eded599f349c789c94fec52eac63054f3692ca4755826853857a33`  
		Last Modified: Wed, 21 Dec 2022 02:06:25 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1-fastcgi` - linux; mips64le

```console
$ docker pull adminer@sha256:e7a494809199392e1931b1b28a4f4331784fa3d2bcba37ce44f3cbf895e33e37
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.3 MB (92329550 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e351ec1ac27e9afe073b5935a1450c40ddd4d5fbb496b42509bde8929705b8d1`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Tue, 06 Dec 2022 01:54:55 GMT
ADD file:09d48994a41c54566f7123db033773e6246c0703a518af76843198196cd39645 in / 
# Tue, 06 Dec 2022 01:55:00 GMT
CMD ["bash"]
# Sat, 17 Dec 2022 01:31:42 GMT
STOPSIGNAL SIGINT
# Sat, 17 Dec 2022 01:33:37 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Sat, 17 Dec 2022 01:33:43 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Sat, 17 Dec 2022 01:35:28 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Sat, 17 Dec 2022 01:35:34 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Sat, 17 Dec 2022 01:35:38 GMT
WORKDIR /var/www/html
# Sat, 17 Dec 2022 01:35:40 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Sat, 17 Dec 2022 01:35:44 GMT
ENV ADMINER_VERSION=4.8.1
# Sat, 17 Dec 2022 01:35:47 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Sat, 17 Dec 2022 01:35:50 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Sat, 17 Dec 2022 01:36:39 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 17 Dec 2022 01:36:41 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Sat, 17 Dec 2022 01:36:45 GMT
ENTRYPOINT ["entrypoint.sh"]
# Sat, 17 Dec 2022 01:36:48 GMT
USER adminer
# Sat, 17 Dec 2022 01:36:51 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:acb57a81743c28ead1a32571c107ac15cd970593fea4f2954b57f22e6bbad1d0`  
		Last Modified: Tue, 06 Dec 2022 02:02:59 GMT  
		Size: 53.3 MB (53260631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16a0a73e4e15363c91b94686e7609b1d84bd3ab5f4c13b2302e76c23e58ca18f`  
		Last Modified: Sat, 17 Dec 2022 01:38:30 GMT  
		Size: 37.7 MB (37676049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8aebeb122c3b2bc8c5262621178cece53cdab93feb29828240f598aa1c86637`  
		Last Modified: Sat, 17 Dec 2022 01:38:02 GMT  
		Size: 395.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2edf7b726c889078b8d32ddaeb1eb6051a11a8f855dad5390aae1cdb3688615`  
		Last Modified: Sat, 17 Dec 2022 01:38:50 GMT  
		Size: 2.7 KB (2712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af0218fe073275ed5c7c0432527e394ba32d894ee6751a1eff961b6bdc775443`  
		Last Modified: Sat, 17 Dec 2022 01:38:50 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f299876d55c3b91c269c41873c488d741613390f000b3104546c0329410c51d8`  
		Last Modified: Sat, 17 Dec 2022 01:38:50 GMT  
		Size: 1.5 KB (1481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae1c4a189325330ffbce29139b4535443d6c162e063032ca30ada9bdc5e8ba60`  
		Last Modified: Sat, 17 Dec 2022 01:38:50 GMT  
		Size: 1.4 MB (1386058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d6e400fdc50315e82b9a184d27fff83deb7028bf757fefea876e9e20247a70d`  
		Last Modified: Sat, 17 Dec 2022 01:38:50 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1-fastcgi` - linux; ppc64le

```console
$ docker pull adminer@sha256:248833c195a726561a4627fd9c8ef5a3ddc6b4350809c298ad4a9f2e9cf1203f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.9 MB (100906397 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1156cafbf63d82f8a2d9663ffb1652e3b3b0ae96e2efb8e523cc0c422d1da1a5`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Wed, 21 Dec 2022 01:17:21 GMT
ADD file:c95bdb0df70fa9ce48b31a7ceb8a7be0c5b925efcf01c43595868b86994dc192 in / 
# Wed, 21 Dec 2022 01:17:25 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 05:10:17 GMT
STOPSIGNAL SIGINT
# Wed, 21 Dec 2022 05:11:02 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 05:11:05 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 21 Dec 2022 05:11:43 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Wed, 21 Dec 2022 05:11:44 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 21 Dec 2022 05:11:44 GMT
WORKDIR /var/www/html
# Wed, 21 Dec 2022 05:11:45 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 21 Dec 2022 05:11:45 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 21 Dec 2022 05:11:45 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 21 Dec 2022 05:11:46 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 21 Dec 2022 05:12:07 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 21 Dec 2022 05:12:07 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 21 Dec 2022 05:12:08 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 21 Dec 2022 05:12:08 GMT
USER adminer
# Wed, 21 Dec 2022 05:12:08 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:542880f4d15404af17d342ecbb76bb92724fc7cb8a91a5e18f26bd8f8811a38a`  
		Last Modified: Wed, 21 Dec 2022 01:22:46 GMT  
		Size: 58.9 MB (58897040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8c91d3a2eff19ff3291563333f250447b70f82929a98b439e9253b9d8909332`  
		Last Modified: Wed, 21 Dec 2022 05:12:53 GMT  
		Size: 40.6 MB (40618582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1fc5014e613c79f385d0565b105dfdc45badae00ab5a50f9b06955eb34e874d`  
		Last Modified: Wed, 21 Dec 2022 05:12:39 GMT  
		Size: 394.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5b74bb738e578f210c95db9d4fc2c314ce3454b4454d48e9fd0269bc6c207e8`  
		Last Modified: Wed, 21 Dec 2022 05:13:17 GMT  
		Size: 2.7 KB (2712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fd43780f4a97de99f2a70cbdeb1e9b998a4a0b78d33e413d5b202dfdc938ebb`  
		Last Modified: Wed, 21 Dec 2022 05:13:17 GMT  
		Size: 1.9 KB (1878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf0b6261dedf5bb3e0f0d3f02c0c41d44c78abd343b214d5e105040aecdbead8`  
		Last Modified: Wed, 21 Dec 2022 05:13:17 GMT  
		Size: 1.5 KB (1480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ffa54700428e518453fb0a542abf4e41ba28e7f58c380d6540691f0d3ded1a1`  
		Last Modified: Wed, 21 Dec 2022 05:13:17 GMT  
		Size: 1.4 MB (1383821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92c025b84e6aa9a000bd19d3eded000fba61196718941820ae5d1eba78d131c8`  
		Last Modified: Wed, 21 Dec 2022 05:13:17 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1-fastcgi` - linux; s390x

```console
$ docker pull adminer@sha256:a1fa0d120584828c961ce0b29ab5d38c4bd62a7c4832051e8a59bdd185eaa72e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.4 MB (93404712 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:078ace26e901a591bccbb767862313e0b30444a61969a6f9563f56d8172155d7`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Wed, 21 Dec 2022 01:42:51 GMT
ADD file:22c4f2d41083ce4433bec4a71e7e6ddc5bec8e44e9cf2c9f93d0874b5b4de7c3 in / 
# Wed, 21 Dec 2022 01:42:54 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 02:06:42 GMT
STOPSIGNAL SIGINT
# Wed, 21 Dec 2022 02:07:51 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 02:08:00 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 21 Dec 2022 02:08:48 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Wed, 21 Dec 2022 02:08:50 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 21 Dec 2022 02:08:51 GMT
WORKDIR /var/www/html
# Wed, 21 Dec 2022 02:08:51 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 21 Dec 2022 02:08:52 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 21 Dec 2022 02:08:53 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 21 Dec 2022 02:08:53 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 21 Dec 2022 02:09:20 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 21 Dec 2022 02:09:21 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 21 Dec 2022 02:09:21 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 21 Dec 2022 02:09:22 GMT
USER adminer
# Wed, 21 Dec 2022 02:09:23 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:7f45294776f4c97d23f8dbfca98d4b57701b478eedfcb154a7e7dc6d6954ba44`  
		Last Modified: Wed, 21 Dec 2022 01:48:50 GMT  
		Size: 53.3 MB (53258472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8610ee81c430b6503a5ee2d7cc451175bdfc868fc17ef5a675b43679da433867`  
		Last Modified: Wed, 21 Dec 2022 02:10:03 GMT  
		Size: 38.8 MB (38755148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:211b726eee70a0c5ff85337d1e98c7987025435a41ca5421f47d96fc164b5b27`  
		Last Modified: Wed, 21 Dec 2022 02:09:56 GMT  
		Size: 395.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:548dc4ca6b10efd03438d3ef399c3d858053ec103194dba6350126f59b0cc988`  
		Last Modified: Wed, 21 Dec 2022 02:10:20 GMT  
		Size: 2.7 KB (2713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcd20979228556508e9e2424f45667a2246d9c409f2557492271740f4840e889`  
		Last Modified: Wed, 21 Dec 2022 02:10:20 GMT  
		Size: 1.9 KB (1883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2e7ff5c1ff35711cc296fbbe902ca0db4bc13c6b5863ba4c3adc2640e16177e`  
		Last Modified: Wed, 21 Dec 2022 02:10:20 GMT  
		Size: 1.5 KB (1481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:334c0739b3be2b837dcd345afc1a5bd12f907a3080d438abf00d8706d01e99c8`  
		Last Modified: Wed, 21 Dec 2022 02:10:20 GMT  
		Size: 1.4 MB (1384126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd966444e211f7ff2ff5aca0482cee29884580acd8b4114e8bd25b616618c89c`  
		Last Modified: Wed, 21 Dec 2022 02:10:21 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `adminer:4.8.1-standalone`

```console
$ docker pull adminer@sha256:895823d11ab87b3ef3db1230b33d9347b0c4fd58e6188906af37b3e7353f383f
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
$ docker pull adminer@sha256:11d6176cead328bcc234f740d98dccda987d03c17d77e03bdceb508c9d35ba30
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.6 MB (95639696 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c207e90c34520f27508ac0a18405256f981ecb45aae2baa2835c91a8f1963f0a`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 21 Dec 2022 01:20:21 GMT
ADD file:c13b430c8699df107ffd9ea5230b92238bc037a8e1cbbe35d6ab664941d575da in / 
# Wed, 21 Dec 2022 01:20:22 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 01:43:34 GMT
STOPSIGNAL SIGINT
# Wed, 21 Dec 2022 01:43:57 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 01:43:58 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 21 Dec 2022 01:43:59 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 21 Dec 2022 01:43:59 GMT
WORKDIR /var/www/html
# Wed, 21 Dec 2022 01:43:59 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 21 Dec 2022 01:43:59 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 21 Dec 2022 01:43:59 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 21 Dec 2022 01:43:59 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 21 Dec 2022 01:44:12 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 21 Dec 2022 01:44:12 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 21 Dec 2022 01:44:12 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 21 Dec 2022 01:44:12 GMT
USER adminer
# Wed, 21 Dec 2022 01:44:12 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 21 Dec 2022 01:44:12 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:32de3c850997ce03b6ff4ae8fb00b34b9d7d7f9a35bfcdb8538e22cc7b77c29d`  
		Last Modified: Wed, 21 Dec 2022 01:24:10 GMT  
		Size: 55.0 MB (55025166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bddad460143b31cc21fc89d836e6d417bb718a19c27f93eb137aebd91b79660`  
		Last Modified: Wed, 21 Dec 2022 01:44:51 GMT  
		Size: 39.2 MB (39226473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bf0beaa0412c7e762322b7311a449203a96c1e115d99efca0dddce016279e6a`  
		Last Modified: Wed, 21 Dec 2022 01:44:43 GMT  
		Size: 394.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e7ee08ea648165938f5fde9ae603f33b34b10c2d4ad2e40ea8c04913db12b65`  
		Last Modified: Wed, 21 Dec 2022 01:44:43 GMT  
		Size: 1.9 KB (1888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd9f958670d2c87349fd96a19d4254adbc404b54b3911c6962d9119d1a6fe901`  
		Last Modified: Wed, 21 Dec 2022 01:44:43 GMT  
		Size: 1.5 KB (1477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:292984a5d9c1d2f389b01937cbdf2a19e8b9de4ed6719500f1310467b1a19ff5`  
		Last Modified: Wed, 21 Dec 2022 01:44:44 GMT  
		Size: 1.4 MB (1383807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20a148ad3aa6178c7d0e684fcbc70c4ca4ba27ea5f13560aef5219a63b2b6874`  
		Last Modified: Wed, 21 Dec 2022 01:44:43 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1-standalone` - linux; arm variant v5

```console
$ docker pull adminer@sha256:50640fef3243132e1ea5d5081f834e0ca156c8264c0b0441a43492f4a4eeca23
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.9 MB (90901373 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:250a1b3ad0e6461afc53655c14f3a5b1378d898200c7bdef2f11ad58335fe9a2`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 21 Dec 2022 01:48:53 GMT
ADD file:81ccc74e0ea343972e2f3f46d2da7e9b808d9718be44d4afa7bec6904b7ab9c6 in / 
# Wed, 21 Dec 2022 01:48:55 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 02:12:35 GMT
STOPSIGNAL SIGINT
# Wed, 21 Dec 2022 02:13:07 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 02:13:09 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 21 Dec 2022 02:13:10 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 21 Dec 2022 02:13:10 GMT
WORKDIR /var/www/html
# Wed, 21 Dec 2022 02:13:10 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 21 Dec 2022 02:13:10 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 21 Dec 2022 02:13:10 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 21 Dec 2022 02:13:10 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 21 Dec 2022 02:13:27 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 21 Dec 2022 02:13:27 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 21 Dec 2022 02:13:27 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 21 Dec 2022 02:13:27 GMT
USER adminer
# Wed, 21 Dec 2022 02:13:27 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 21 Dec 2022 02:13:27 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:89b6e4f9f2f811282495a047e873c20d6ac2d53c72ad576a6907b1449eb3e635`  
		Last Modified: Wed, 21 Dec 2022 01:53:30 GMT  
		Size: 52.5 MB (52529974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2473783a5bf521f1fdf370edfbbd3a71c7d41bd6ad586832334a5359d21e0937`  
		Last Modified: Wed, 21 Dec 2022 02:14:50 GMT  
		Size: 37.0 MB (36983598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fb144c6fa4674d630705477694c2b1a78efcb47a43b11b84d11420c6672d849`  
		Last Modified: Wed, 21 Dec 2022 02:14:41 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7d2eaadeb68edbb519fcd0f769e3e17f2744670df98e1f42b2dd32755e43260`  
		Last Modified: Wed, 21 Dec 2022 02:14:41 GMT  
		Size: 1.8 KB (1840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57c2b47fd023120badcfed4eb901caaff2b0fb6b5d48de329e15232469b9af23`  
		Last Modified: Wed, 21 Dec 2022 02:14:41 GMT  
		Size: 1.5 KB (1481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54fcbf1f604d9098ea8ed2239603e5aa978d84db1258c72c4a54a6aa095ec76f`  
		Last Modified: Wed, 21 Dec 2022 02:14:41 GMT  
		Size: 1.4 MB (1383596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:216e1a8363d45d45df8c6cbfe9f7ee9909da57c723cd447b01a248fb042840f3`  
		Last Modified: Wed, 21 Dec 2022 02:14:41 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1-standalone` - linux; arm variant v7

```console
$ docker pull adminer@sha256:667b9904f45244f6db8f25daad4eea200d6c4a4f91c68de564a5caf5a4c6a5c5
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.5 MB (87525670 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4da555d48a0530a78c590fbbf78d89a6283e3bf8436c4028fc44739c58ed9fd4`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 21 Dec 2022 01:58:09 GMT
ADD file:4b6f71680de34554595f062f9e52037b48edf19ca8f34c75877caa85c42caad3 in / 
# Wed, 21 Dec 2022 01:58:10 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 16:55:05 GMT
STOPSIGNAL SIGINT
# Wed, 21 Dec 2022 16:55:27 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 16:55:28 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 21 Dec 2022 16:55:29 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 21 Dec 2022 16:55:29 GMT
WORKDIR /var/www/html
# Wed, 21 Dec 2022 16:55:29 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 21 Dec 2022 16:55:29 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 21 Dec 2022 16:55:29 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 21 Dec 2022 16:55:29 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 21 Dec 2022 16:55:42 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 21 Dec 2022 16:55:42 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 21 Dec 2022 16:55:42 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 21 Dec 2022 16:55:42 GMT
USER adminer
# Wed, 21 Dec 2022 16:55:42 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 21 Dec 2022 16:55:42 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:706bb1d74512e1fb9ba97aa9212a32d07726fbfe77e4c7e609406d2065418f57`  
		Last Modified: Wed, 21 Dec 2022 02:04:37 GMT  
		Size: 50.2 MB (50190771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a1c5cd5ac0e733e02567c893f1028628f441423281df1c54fa1042b317bb758`  
		Last Modified: Wed, 21 Dec 2022 16:56:48 GMT  
		Size: 35.9 MB (35947077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3d69909ab6c9fd65668b2d644bbb5375f5617c8bba9e82704145b53e895ad98`  
		Last Modified: Wed, 21 Dec 2022 16:56:39 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be622d99b39d413b273b3c6344f0cf7b97883297c9e7fb52951cca9bafd33f3a`  
		Last Modified: Wed, 21 Dec 2022 16:56:39 GMT  
		Size: 1.8 KB (1840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:546d6a7c782f341de9ea0c0c9aa227a5fa0d870146d87f59cb4d319c5b895028`  
		Last Modified: Wed, 21 Dec 2022 16:56:39 GMT  
		Size: 1.5 KB (1479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e94d73593abc9542a40f6e2f989f35a2bebbb21e554c4d2452cee59089701ca5`  
		Last Modified: Wed, 21 Dec 2022 16:56:39 GMT  
		Size: 1.4 MB (1383619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f3795d41125166e2051354d7af4622abe6b7610551670476d49ad99c372bad6`  
		Last Modified: Wed, 21 Dec 2022 16:56:39 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1-standalone` - linux; arm64 variant v8

```console
$ docker pull adminer@sha256:2e15c1b18293cc812ca73063a33ca295e6e5b4011ab43006f371bf3d63f7a387
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.0 MB (94046599 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f2678931127cd62d7af0ee195d7008f84b549fb9374257d1696f7cc5c9dab049`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 21 Dec 2022 01:39:40 GMT
ADD file:5bbdc914ec8ed60ac85293e88ee1aafc3f0290762e320fc86dc9d79fa201834e in / 
# Wed, 21 Dec 2022 01:39:41 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 02:01:54 GMT
STOPSIGNAL SIGINT
# Wed, 21 Dec 2022 02:02:11 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 02:02:12 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 21 Dec 2022 02:02:12 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 21 Dec 2022 02:02:13 GMT
WORKDIR /var/www/html
# Wed, 21 Dec 2022 02:02:13 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 21 Dec 2022 02:02:13 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 21 Dec 2022 02:02:13 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 21 Dec 2022 02:02:13 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 21 Dec 2022 02:02:23 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 21 Dec 2022 02:02:24 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 21 Dec 2022 02:02:24 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 21 Dec 2022 02:02:24 GMT
USER adminer
# Wed, 21 Dec 2022 02:02:24 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 21 Dec 2022 02:02:24 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:c3e6129b48b69d14c5e7a5605e2b94003fb71aac82eac46b8689f5b8007af2c5`  
		Last Modified: Wed, 21 Dec 2022 01:42:49 GMT  
		Size: 53.7 MB (53681797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:235cb929f19f47af31496a0a93a9cb1fd8f5104f0d34a160f4d2e4d6b9463df1`  
		Last Modified: Wed, 21 Dec 2022 02:02:59 GMT  
		Size: 39.0 MB (38976852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a72d5ac588c6b24f2d8a511e934c2745420b4536a9fa914031e10c9d384efd2b`  
		Last Modified: Wed, 21 Dec 2022 02:02:52 GMT  
		Size: 392.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c1912d1c0826d94d3aa328472384e502a58e992b77df780de62bbe9ba9f744e`  
		Last Modified: Wed, 21 Dec 2022 02:02:52 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f6d91a33867afb4cdea48a709f3cd43416c387bbf8a96e04840822e05a249eb`  
		Last Modified: Wed, 21 Dec 2022 02:02:52 GMT  
		Size: 1.5 KB (1481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a85debe3d62cce517ab60af785fce8ae30d5633d41e755d25700acfaa96f427`  
		Last Modified: Wed, 21 Dec 2022 02:02:53 GMT  
		Size: 1.4 MB (1383704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c707a54ab9eee88dee88a920652b121430b0f93f2599e1f3d29cd8ee7f91a359`  
		Last Modified: Wed, 21 Dec 2022 02:02:52 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1-standalone` - linux; 386

```console
$ docker pull adminer@sha256:d219efb2aecebb6bd16280905d0c7ff80b18ad7269350fec6bd034d2a093976d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.7 MB (96663116 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a504b1b6ca371056530865e9620cc9e4dabcd05dd93ab1f5b1dc2092bf6656e2`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 21 Dec 2022 01:39:08 GMT
ADD file:10d2f443f55d8ba9512899b3dff08f6e9a6c7ca096f407e3477e9798e1063785 in / 
# Wed, 21 Dec 2022 01:39:09 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 02:04:14 GMT
STOPSIGNAL SIGINT
# Wed, 21 Dec 2022 02:04:35 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 02:04:36 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 21 Dec 2022 02:04:37 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 21 Dec 2022 02:04:38 GMT
WORKDIR /var/www/html
# Wed, 21 Dec 2022 02:04:40 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 21 Dec 2022 02:04:40 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 21 Dec 2022 02:04:41 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 21 Dec 2022 02:04:42 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 21 Dec 2022 02:04:55 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 21 Dec 2022 02:04:57 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 21 Dec 2022 02:04:57 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 21 Dec 2022 02:04:58 GMT
USER adminer
# Wed, 21 Dec 2022 02:04:59 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 21 Dec 2022 02:05:00 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:bde501e1d960005aee2bdf2fc8c89b26bf694dace8740c72deda4d7705995ab7`  
		Last Modified: Wed, 21 Dec 2022 01:44:18 GMT  
		Size: 56.0 MB (56005267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd60bbc5dc31d7ec1db0a2fbd068c29f7583f7d3e2d0599f0706680ce602ee9d`  
		Last Modified: Wed, 21 Dec 2022 02:06:03 GMT  
		Size: 39.3 MB (39269700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b30e5dcb4252f7f6ded0a9c044209070412dbf7df3daab7e7343bc6bf568fe67`  
		Last Modified: Wed, 21 Dec 2022 02:05:50 GMT  
		Size: 394.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:387e2851bc00ff07433e8e9d3d12cdc6590937cbf4a9de8a035771e386a0e3c4`  
		Last Modified: Wed, 21 Dec 2022 02:05:50 GMT  
		Size: 1.7 KB (1718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c04056306aff55b02341e716626152ea622c4326e3f31a4a39bce3d631152fea`  
		Last Modified: Wed, 21 Dec 2022 02:05:50 GMT  
		Size: 1.5 KB (1478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31f79e3e185cbecc304f97fe83e64bc102e782154ed533744186d41a6de680fb`  
		Last Modified: Wed, 21 Dec 2022 02:05:51 GMT  
		Size: 1.4 MB (1384066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce0359a7ffb52c577cc47d0136aeed97a19a7e826d80ebb7b304977f271a6f7d`  
		Last Modified: Wed, 21 Dec 2022 02:05:51 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1-standalone` - linux; mips64le

```console
$ docker pull adminer@sha256:74a7ae91c85961c3ad967ae1cf25d79b8d7a69a6668843b885aebcc169a7f88f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.3 MB (92326851 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0992a9b14a478d0bfd67839ed2e77e40a770492ebd4daa67c6141cd734519bb1`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Tue, 06 Dec 2022 01:54:55 GMT
ADD file:09d48994a41c54566f7123db033773e6246c0703a518af76843198196cd39645 in / 
# Tue, 06 Dec 2022 01:55:00 GMT
CMD ["bash"]
# Sat, 17 Dec 2022 01:31:42 GMT
STOPSIGNAL SIGINT
# Sat, 17 Dec 2022 01:33:37 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Sat, 17 Dec 2022 01:33:43 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Sat, 17 Dec 2022 01:33:49 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Sat, 17 Dec 2022 01:33:53 GMT
WORKDIR /var/www/html
# Sat, 17 Dec 2022 01:33:56 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Sat, 17 Dec 2022 01:33:59 GMT
ENV ADMINER_VERSION=4.8.1
# Sat, 17 Dec 2022 01:34:02 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Sat, 17 Dec 2022 01:34:05 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Sat, 17 Dec 2022 01:34:57 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 17 Dec 2022 01:35:00 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Sat, 17 Dec 2022 01:35:03 GMT
ENTRYPOINT ["entrypoint.sh"]
# Sat, 17 Dec 2022 01:35:06 GMT
USER adminer
# Sat, 17 Dec 2022 01:35:09 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Sat, 17 Dec 2022 01:35:13 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:acb57a81743c28ead1a32571c107ac15cd970593fea4f2954b57f22e6bbad1d0`  
		Last Modified: Tue, 06 Dec 2022 02:02:59 GMT  
		Size: 53.3 MB (53260631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16a0a73e4e15363c91b94686e7609b1d84bd3ab5f4c13b2302e76c23e58ca18f`  
		Last Modified: Sat, 17 Dec 2022 01:38:30 GMT  
		Size: 37.7 MB (37676049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8aebeb122c3b2bc8c5262621178cece53cdab93feb29828240f598aa1c86637`  
		Last Modified: Sat, 17 Dec 2022 01:38:02 GMT  
		Size: 395.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3c1363529deb53f7595176aa5b55b04ab1cdf841a6cd3cdb88c41d6ec75615f`  
		Last Modified: Sat, 17 Dec 2022 01:38:02 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0923c943bb7440a1b68c2494f1f23c0a3199d4d3a6cdb87bdca8067acfbe4d4`  
		Last Modified: Sat, 17 Dec 2022 01:38:02 GMT  
		Size: 1.5 KB (1485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47a69745dad2c95e6d8ff413ca73cc902100c3848af39c316ae44ec375f8aae7`  
		Last Modified: Sat, 17 Dec 2022 01:38:03 GMT  
		Size: 1.4 MB (1386065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2548a3e7b136720a8c94faa9137694506f95bcf701a80d8b49486c2a3be6205b`  
		Last Modified: Sat, 17 Dec 2022 01:38:02 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1-standalone` - linux; ppc64le

```console
$ docker pull adminer@sha256:86fbf5aa76cfa4052c3d9bf35b81e34daf0fb53fbc674d612c071ca9a60de5ce
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.9 MB (100903714 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:075df6bcff3df963b2eec2efff06fef0b4f316e1751a5ebc98880754503bcf54`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 21 Dec 2022 01:17:21 GMT
ADD file:c95bdb0df70fa9ce48b31a7ceb8a7be0c5b925efcf01c43595868b86994dc192 in / 
# Wed, 21 Dec 2022 01:17:25 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 05:10:17 GMT
STOPSIGNAL SIGINT
# Wed, 21 Dec 2022 05:11:02 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 05:11:05 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 21 Dec 2022 05:11:07 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 21 Dec 2022 05:11:07 GMT
WORKDIR /var/www/html
# Wed, 21 Dec 2022 05:11:07 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 21 Dec 2022 05:11:08 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 21 Dec 2022 05:11:08 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 21 Dec 2022 05:11:09 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 21 Dec 2022 05:11:31 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 21 Dec 2022 05:11:31 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 21 Dec 2022 05:11:32 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 21 Dec 2022 05:11:32 GMT
USER adminer
# Wed, 21 Dec 2022 05:11:32 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 21 Dec 2022 05:11:33 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:542880f4d15404af17d342ecbb76bb92724fc7cb8a91a5e18f26bd8f8811a38a`  
		Last Modified: Wed, 21 Dec 2022 01:22:46 GMT  
		Size: 58.9 MB (58897040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8c91d3a2eff19ff3291563333f250447b70f82929a98b439e9253b9d8909332`  
		Last Modified: Wed, 21 Dec 2022 05:12:53 GMT  
		Size: 40.6 MB (40618582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1fc5014e613c79f385d0565b105dfdc45badae00ab5a50f9b06955eb34e874d`  
		Last Modified: Wed, 21 Dec 2022 05:12:39 GMT  
		Size: 394.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc90d97148640f4f164e3dc4b1f043c6ba7d8b5cddd21ede8a947339a13e3c3f`  
		Last Modified: Wed, 21 Dec 2022 05:12:39 GMT  
		Size: 1.9 KB (1879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdfe2d4e5fb66793ea99cc5959183331088d985dc203754a30a8bf6bbffb186a`  
		Last Modified: Wed, 21 Dec 2022 05:12:39 GMT  
		Size: 1.5 KB (1482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0da8c96b4d9b013ebbf00af4b8693e634764cf159be7af73d3152403cabe71e5`  
		Last Modified: Wed, 21 Dec 2022 05:12:40 GMT  
		Size: 1.4 MB (1383844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:061e859636ca9e27f80e25b38a893f2e38d08dd68c7a53bc8fb9f428dfb0f328`  
		Last Modified: Wed, 21 Dec 2022 05:12:39 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1-standalone` - linux; s390x

```console
$ docker pull adminer@sha256:4ad639f239b5117cf7381d37948390122d8f514592dade423c1fbdc4870c04b4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.4 MB (93401988 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac7114a00edb645cd010878538757f757f872e25c530cb9159f5bc03cc191726`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 21 Dec 2022 01:42:51 GMT
ADD file:22c4f2d41083ce4433bec4a71e7e6ddc5bec8e44e9cf2c9f93d0874b5b4de7c3 in / 
# Wed, 21 Dec 2022 01:42:54 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 02:06:42 GMT
STOPSIGNAL SIGINT
# Wed, 21 Dec 2022 02:07:51 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 02:08:00 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 21 Dec 2022 02:08:02 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 21 Dec 2022 02:08:03 GMT
WORKDIR /var/www/html
# Wed, 21 Dec 2022 02:08:04 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 21 Dec 2022 02:08:04 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 21 Dec 2022 02:08:05 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 21 Dec 2022 02:08:06 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 21 Dec 2022 02:08:33 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 21 Dec 2022 02:08:33 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 21 Dec 2022 02:08:34 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 21 Dec 2022 02:08:35 GMT
USER adminer
# Wed, 21 Dec 2022 02:08:35 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 21 Dec 2022 02:08:36 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:7f45294776f4c97d23f8dbfca98d4b57701b478eedfcb154a7e7dc6d6954ba44`  
		Last Modified: Wed, 21 Dec 2022 01:48:50 GMT  
		Size: 53.3 MB (53258472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8610ee81c430b6503a5ee2d7cc451175bdfc868fc17ef5a675b43679da433867`  
		Last Modified: Wed, 21 Dec 2022 02:10:03 GMT  
		Size: 38.8 MB (38755148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:211b726eee70a0c5ff85337d1e98c7987025435a41ca5421f47d96fc164b5b27`  
		Last Modified: Wed, 21 Dec 2022 02:09:56 GMT  
		Size: 395.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c6a1fa2154f900c32f87164afe347f0dddbb7a641dc81b7fc436b1d15a5349d`  
		Last Modified: Wed, 21 Dec 2022 02:09:56 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e030c793dfbf87ef1f5dbbecd22117bcf1695eb293e41bca267fb29d0e98d59d`  
		Last Modified: Wed, 21 Dec 2022 02:09:56 GMT  
		Size: 1.5 KB (1478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:965c9f68e6765f8a5967198527ce6ff7bf0646cab60aa30ecef97747554c0869`  
		Last Modified: Wed, 21 Dec 2022 02:09:56 GMT  
		Size: 1.4 MB (1384122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d34b801ca3351132a2f2914bc4ef3ca0f91a2c87c2b42fce3662fd5f20593aea`  
		Last Modified: Wed, 21 Dec 2022 02:09:56 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `adminer:fastcgi`

```console
$ docker pull adminer@sha256:37807622785148a8a96b6b2d9314e7db8e7202306531a9e674f9735b07ce17d3
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
$ docker pull adminer@sha256:1e1e6130a4906493f3dcda03ec0eb19eeec7d747868d8e7526583e93b90377ed
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.6 MB (95642424 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ec85d40ab3aa8923f6295358e72e000090652b9a26b7b9c7774d997a844e842`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Wed, 21 Dec 2022 01:20:21 GMT
ADD file:c13b430c8699df107ffd9ea5230b92238bc037a8e1cbbe35d6ab664941d575da in / 
# Wed, 21 Dec 2022 01:20:22 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 01:43:34 GMT
STOPSIGNAL SIGINT
# Wed, 21 Dec 2022 01:43:57 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 01:43:58 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 21 Dec 2022 01:44:15 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Wed, 21 Dec 2022 01:44:16 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 21 Dec 2022 01:44:16 GMT
WORKDIR /var/www/html
# Wed, 21 Dec 2022 01:44:16 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 21 Dec 2022 01:44:16 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 21 Dec 2022 01:44:16 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 21 Dec 2022 01:44:17 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 21 Dec 2022 01:44:28 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 21 Dec 2022 01:44:28 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 21 Dec 2022 01:44:28 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 21 Dec 2022 01:44:29 GMT
USER adminer
# Wed, 21 Dec 2022 01:44:29 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:32de3c850997ce03b6ff4ae8fb00b34b9d7d7f9a35bfcdb8538e22cc7b77c29d`  
		Last Modified: Wed, 21 Dec 2022 01:24:10 GMT  
		Size: 55.0 MB (55025166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bddad460143b31cc21fc89d836e6d417bb718a19c27f93eb137aebd91b79660`  
		Last Modified: Wed, 21 Dec 2022 01:44:51 GMT  
		Size: 39.2 MB (39226473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bf0beaa0412c7e762322b7311a449203a96c1e115d99efca0dddce016279e6a`  
		Last Modified: Wed, 21 Dec 2022 01:44:43 GMT  
		Size: 394.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e85c5399c00e75eb8dd783e68be98aeef85fb6e2e50ab17a1f3d0fb977496970`  
		Last Modified: Wed, 21 Dec 2022 01:45:09 GMT  
		Size: 2.7 KB (2712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fa2e6155707c0c71fe403f845f4a9061a2bba300a1a1c18f480f59742b9036a`  
		Last Modified: Wed, 21 Dec 2022 01:45:09 GMT  
		Size: 1.9 KB (1879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48c9c38ec5f03fab46adc653af92a4b0c326aa93c7533ff5e7c2166e3ef8cf40`  
		Last Modified: Wed, 21 Dec 2022 01:45:09 GMT  
		Size: 1.5 KB (1478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a19f8c5c89b7131c03f16fdc1f9c0c0bf07fbc0d9bfe1cecb756a290c47fbd6b`  
		Last Modified: Wed, 21 Dec 2022 01:45:10 GMT  
		Size: 1.4 MB (1383831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a5ef3fdf80e2ac647453715c908b46bb54a9310430fed3a3bb6e8f418740b8e`  
		Last Modified: Wed, 21 Dec 2022 01:45:09 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:fastcgi` - linux; arm variant v5

```console
$ docker pull adminer@sha256:f6452248c81bf0aa2cecfa804a14cd9b14a2503be250138828d035b75e2896a9
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.9 MB (90904118 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d18173eb6830d6ef3ae8c8a231cb8ea70b230991680c62578ac47461b434c398`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Wed, 21 Dec 2022 01:48:53 GMT
ADD file:81ccc74e0ea343972e2f3f46d2da7e9b808d9718be44d4afa7bec6904b7ab9c6 in / 
# Wed, 21 Dec 2022 01:48:55 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 02:12:35 GMT
STOPSIGNAL SIGINT
# Wed, 21 Dec 2022 02:13:07 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 02:13:09 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 21 Dec 2022 02:13:39 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Wed, 21 Dec 2022 02:13:40 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 21 Dec 2022 02:13:41 GMT
WORKDIR /var/www/html
# Wed, 21 Dec 2022 02:13:41 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 21 Dec 2022 02:13:42 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 21 Dec 2022 02:13:42 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 21 Dec 2022 02:13:42 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 21 Dec 2022 02:14:02 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 21 Dec 2022 02:14:02 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 21 Dec 2022 02:14:02 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 21 Dec 2022 02:14:02 GMT
USER adminer
# Wed, 21 Dec 2022 02:14:03 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:89b6e4f9f2f811282495a047e873c20d6ac2d53c72ad576a6907b1449eb3e635`  
		Last Modified: Wed, 21 Dec 2022 01:53:30 GMT  
		Size: 52.5 MB (52529974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2473783a5bf521f1fdf370edfbbd3a71c7d41bd6ad586832334a5359d21e0937`  
		Last Modified: Wed, 21 Dec 2022 02:14:50 GMT  
		Size: 37.0 MB (36983598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fb144c6fa4674d630705477694c2b1a78efcb47a43b11b84d11420c6672d849`  
		Last Modified: Wed, 21 Dec 2022 02:14:41 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26063a58f85ffe38619444fe9e9ea1012e4e7fdb2b4d72cdcac7a8aae808f733`  
		Last Modified: Wed, 21 Dec 2022 02:15:15 GMT  
		Size: 2.7 KB (2710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41851614d9620c865a301e15f38ab0d4c8ddd9a1f4202edbf3a691d918884cf7`  
		Last Modified: Wed, 21 Dec 2022 02:15:15 GMT  
		Size: 1.8 KB (1839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ab4a9eecfe7e71f9ca3e31e0de304dbd42f4d4078f5feecb1c7c6f4f42005cc`  
		Last Modified: Wed, 21 Dec 2022 02:15:15 GMT  
		Size: 1.5 KB (1481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:606df83e76d99dd227ac689ddcd3e7f8434d06d4e46042bc2419167493a3b188`  
		Last Modified: Wed, 21 Dec 2022 02:15:15 GMT  
		Size: 1.4 MB (1383635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6018be7539eedb016a02d6429a6c60eaa072ee9ea161b1d74167953aa3a9de72`  
		Last Modified: Wed, 21 Dec 2022 02:15:15 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:fastcgi` - linux; arm variant v7

```console
$ docker pull adminer@sha256:9928846ee8fb76c681b35c87ebfed49499f447a0c1c81393d30ab2bcba70a6c2
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.5 MB (87528433 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99681162737fb62edc07a8e79538b32ebe15b415a91f8e6c9e8d2c0f6f224b9a`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Wed, 21 Dec 2022 01:58:09 GMT
ADD file:4b6f71680de34554595f062f9e52037b48edf19ca8f34c75877caa85c42caad3 in / 
# Wed, 21 Dec 2022 01:58:10 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 16:55:05 GMT
STOPSIGNAL SIGINT
# Wed, 21 Dec 2022 16:55:27 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 16:55:28 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 21 Dec 2022 16:55:49 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Wed, 21 Dec 2022 16:55:50 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 21 Dec 2022 16:55:50 GMT
WORKDIR /var/www/html
# Wed, 21 Dec 2022 16:55:50 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 21 Dec 2022 16:55:50 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 21 Dec 2022 16:55:50 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 21 Dec 2022 16:55:50 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 21 Dec 2022 16:56:04 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 21 Dec 2022 16:56:04 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 21 Dec 2022 16:56:04 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 21 Dec 2022 16:56:04 GMT
USER adminer
# Wed, 21 Dec 2022 16:56:04 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:706bb1d74512e1fb9ba97aa9212a32d07726fbfe77e4c7e609406d2065418f57`  
		Last Modified: Wed, 21 Dec 2022 02:04:37 GMT  
		Size: 50.2 MB (50190771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a1c5cd5ac0e733e02567c893f1028628f441423281df1c54fa1042b317bb758`  
		Last Modified: Wed, 21 Dec 2022 16:56:48 GMT  
		Size: 35.9 MB (35947077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3d69909ab6c9fd65668b2d644bbb5375f5617c8bba9e82704145b53e895ad98`  
		Last Modified: Wed, 21 Dec 2022 16:56:39 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0e39a1a73560e658bd05d5621c5e241ea6c658eeb4d6d40fab42c2d0e049dd9`  
		Last Modified: Wed, 21 Dec 2022 16:57:11 GMT  
		Size: 2.7 KB (2707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:570ddb9aaf5affd1f0db7ce02160f1220f1f786028eb2dc3304d29faec9a812c`  
		Last Modified: Wed, 21 Dec 2022 16:57:11 GMT  
		Size: 1.8 KB (1841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5278a6d095ca223fab850a965a90f10b571dee63613450a5c305743288a3db7`  
		Last Modified: Wed, 21 Dec 2022 16:57:11 GMT  
		Size: 1.5 KB (1476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f0a1888014f0f3ae5844f8d80c0707d886f7e951a2583d43345fb59abe5e97c`  
		Last Modified: Wed, 21 Dec 2022 16:57:12 GMT  
		Size: 1.4 MB (1383680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6e719bcd08751a23a74658e85fc4e47ae42d98213576128a573499661a743b9`  
		Last Modified: Wed, 21 Dec 2022 16:57:11 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:fastcgi` - linux; arm64 variant v8

```console
$ docker pull adminer@sha256:deace6e0488124187d0f03d131c3f503f66d5532f6cba7a2c9bbd9f4e92c9639
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.0 MB (94049324 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5eaa4905b3a6a204b45fc4e4608dc8de2ee6e3a8b386c2a8daed65b7ea308fa`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Wed, 21 Dec 2022 01:39:40 GMT
ADD file:5bbdc914ec8ed60ac85293e88ee1aafc3f0290762e320fc86dc9d79fa201834e in / 
# Wed, 21 Dec 2022 01:39:41 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 02:01:54 GMT
STOPSIGNAL SIGINT
# Wed, 21 Dec 2022 02:02:11 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 02:02:12 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 21 Dec 2022 02:02:27 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Wed, 21 Dec 2022 02:02:28 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 21 Dec 2022 02:02:28 GMT
WORKDIR /var/www/html
# Wed, 21 Dec 2022 02:02:28 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 21 Dec 2022 02:02:28 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 21 Dec 2022 02:02:28 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 21 Dec 2022 02:02:28 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 21 Dec 2022 02:02:38 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 21 Dec 2022 02:02:38 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 21 Dec 2022 02:02:38 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 21 Dec 2022 02:02:38 GMT
USER adminer
# Wed, 21 Dec 2022 02:02:38 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:c3e6129b48b69d14c5e7a5605e2b94003fb71aac82eac46b8689f5b8007af2c5`  
		Last Modified: Wed, 21 Dec 2022 01:42:49 GMT  
		Size: 53.7 MB (53681797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:235cb929f19f47af31496a0a93a9cb1fd8f5104f0d34a160f4d2e4d6b9463df1`  
		Last Modified: Wed, 21 Dec 2022 02:02:59 GMT  
		Size: 39.0 MB (38976852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a72d5ac588c6b24f2d8a511e934c2745420b4536a9fa914031e10c9d384efd2b`  
		Last Modified: Wed, 21 Dec 2022 02:02:52 GMT  
		Size: 392.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13819a4b0fdaaf0d610656691e268b84f62b9bc6f1978b10b2fd66d30bfc61a0`  
		Last Modified: Wed, 21 Dec 2022 02:03:18 GMT  
		Size: 2.7 KB (2705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e39e3b462a156c2eb8929e5b29025db6c8048ec880966c1e891e12db93bfb103`  
		Last Modified: Wed, 21 Dec 2022 02:03:18 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c2102a525d7aa1a32b03261d2429812840b08fab7cc2175e391f84857823539`  
		Last Modified: Wed, 21 Dec 2022 02:03:18 GMT  
		Size: 1.5 KB (1476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4364503e41b1e8f317d4c98b8da4b7d28551f47d554987462dfbc04169e893da`  
		Last Modified: Wed, 21 Dec 2022 02:03:19 GMT  
		Size: 1.4 MB (1383730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e279f93f23126fbc1db29d1577bf87115d79396ca7c78cb6b2bda1279cdaa269`  
		Last Modified: Wed, 21 Dec 2022 02:03:18 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:fastcgi` - linux; 386

```console
$ docker pull adminer@sha256:9a434bc61ca7023a8f2c77a9d0958ab597cd69f03685202d1661614ba76c346f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.7 MB (96665821 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c32a28f670f6878d3ca957e9fc114d3736d77b40db0223160324a35254c19e3`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Wed, 21 Dec 2022 01:39:08 GMT
ADD file:10d2f443f55d8ba9512899b3dff08f6e9a6c7ca096f407e3477e9798e1063785 in / 
# Wed, 21 Dec 2022 01:39:09 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 02:04:14 GMT
STOPSIGNAL SIGINT
# Wed, 21 Dec 2022 02:04:35 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 02:04:36 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 21 Dec 2022 02:05:05 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Wed, 21 Dec 2022 02:05:06 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 21 Dec 2022 02:05:07 GMT
WORKDIR /var/www/html
# Wed, 21 Dec 2022 02:05:09 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 21 Dec 2022 02:05:09 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 21 Dec 2022 02:05:10 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 21 Dec 2022 02:05:11 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 21 Dec 2022 02:05:24 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 21 Dec 2022 02:05:25 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 21 Dec 2022 02:05:25 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 21 Dec 2022 02:05:26 GMT
USER adminer
# Wed, 21 Dec 2022 02:05:27 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:bde501e1d960005aee2bdf2fc8c89b26bf694dace8740c72deda4d7705995ab7`  
		Last Modified: Wed, 21 Dec 2022 01:44:18 GMT  
		Size: 56.0 MB (56005267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd60bbc5dc31d7ec1db0a2fbd068c29f7583f7d3e2d0599f0706680ce602ee9d`  
		Last Modified: Wed, 21 Dec 2022 02:06:03 GMT  
		Size: 39.3 MB (39269700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b30e5dcb4252f7f6ded0a9c044209070412dbf7df3daab7e7343bc6bf568fe67`  
		Last Modified: Wed, 21 Dec 2022 02:05:50 GMT  
		Size: 394.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44b71679c4856448b64de04f5a85f11611e00ec6255adf5430d19216fda4b172`  
		Last Modified: Wed, 21 Dec 2022 02:06:25 GMT  
		Size: 2.7 KB (2708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba4434a757058f98902edee00915212df3d942d3675e23589ab4b5b5ff27a41f`  
		Last Modified: Wed, 21 Dec 2022 02:06:24 GMT  
		Size: 1.7 KB (1718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b87eb7dde4067b918229c1df6d6f6890a97ab78c902accb2240718ff2d3e1145`  
		Last Modified: Wed, 21 Dec 2022 02:06:25 GMT  
		Size: 1.5 KB (1479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc82102410ace2a3805c07a9de9d7d5e319e8b7903eebcb983e7ac7c0f69b585`  
		Last Modified: Wed, 21 Dec 2022 02:06:25 GMT  
		Size: 1.4 MB (1384064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dafaed69f8eded599f349c789c94fec52eac63054f3692ca4755826853857a33`  
		Last Modified: Wed, 21 Dec 2022 02:06:25 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:fastcgi` - linux; mips64le

```console
$ docker pull adminer@sha256:e7a494809199392e1931b1b28a4f4331784fa3d2bcba37ce44f3cbf895e33e37
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.3 MB (92329550 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e351ec1ac27e9afe073b5935a1450c40ddd4d5fbb496b42509bde8929705b8d1`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Tue, 06 Dec 2022 01:54:55 GMT
ADD file:09d48994a41c54566f7123db033773e6246c0703a518af76843198196cd39645 in / 
# Tue, 06 Dec 2022 01:55:00 GMT
CMD ["bash"]
# Sat, 17 Dec 2022 01:31:42 GMT
STOPSIGNAL SIGINT
# Sat, 17 Dec 2022 01:33:37 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Sat, 17 Dec 2022 01:33:43 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Sat, 17 Dec 2022 01:35:28 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Sat, 17 Dec 2022 01:35:34 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Sat, 17 Dec 2022 01:35:38 GMT
WORKDIR /var/www/html
# Sat, 17 Dec 2022 01:35:40 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Sat, 17 Dec 2022 01:35:44 GMT
ENV ADMINER_VERSION=4.8.1
# Sat, 17 Dec 2022 01:35:47 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Sat, 17 Dec 2022 01:35:50 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Sat, 17 Dec 2022 01:36:39 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 17 Dec 2022 01:36:41 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Sat, 17 Dec 2022 01:36:45 GMT
ENTRYPOINT ["entrypoint.sh"]
# Sat, 17 Dec 2022 01:36:48 GMT
USER adminer
# Sat, 17 Dec 2022 01:36:51 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:acb57a81743c28ead1a32571c107ac15cd970593fea4f2954b57f22e6bbad1d0`  
		Last Modified: Tue, 06 Dec 2022 02:02:59 GMT  
		Size: 53.3 MB (53260631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16a0a73e4e15363c91b94686e7609b1d84bd3ab5f4c13b2302e76c23e58ca18f`  
		Last Modified: Sat, 17 Dec 2022 01:38:30 GMT  
		Size: 37.7 MB (37676049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8aebeb122c3b2bc8c5262621178cece53cdab93feb29828240f598aa1c86637`  
		Last Modified: Sat, 17 Dec 2022 01:38:02 GMT  
		Size: 395.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2edf7b726c889078b8d32ddaeb1eb6051a11a8f855dad5390aae1cdb3688615`  
		Last Modified: Sat, 17 Dec 2022 01:38:50 GMT  
		Size: 2.7 KB (2712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af0218fe073275ed5c7c0432527e394ba32d894ee6751a1eff961b6bdc775443`  
		Last Modified: Sat, 17 Dec 2022 01:38:50 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f299876d55c3b91c269c41873c488d741613390f000b3104546c0329410c51d8`  
		Last Modified: Sat, 17 Dec 2022 01:38:50 GMT  
		Size: 1.5 KB (1481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae1c4a189325330ffbce29139b4535443d6c162e063032ca30ada9bdc5e8ba60`  
		Last Modified: Sat, 17 Dec 2022 01:38:50 GMT  
		Size: 1.4 MB (1386058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d6e400fdc50315e82b9a184d27fff83deb7028bf757fefea876e9e20247a70d`  
		Last Modified: Sat, 17 Dec 2022 01:38:50 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:fastcgi` - linux; ppc64le

```console
$ docker pull adminer@sha256:248833c195a726561a4627fd9c8ef5a3ddc6b4350809c298ad4a9f2e9cf1203f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.9 MB (100906397 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1156cafbf63d82f8a2d9663ffb1652e3b3b0ae96e2efb8e523cc0c422d1da1a5`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Wed, 21 Dec 2022 01:17:21 GMT
ADD file:c95bdb0df70fa9ce48b31a7ceb8a7be0c5b925efcf01c43595868b86994dc192 in / 
# Wed, 21 Dec 2022 01:17:25 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 05:10:17 GMT
STOPSIGNAL SIGINT
# Wed, 21 Dec 2022 05:11:02 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 05:11:05 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 21 Dec 2022 05:11:43 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Wed, 21 Dec 2022 05:11:44 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 21 Dec 2022 05:11:44 GMT
WORKDIR /var/www/html
# Wed, 21 Dec 2022 05:11:45 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 21 Dec 2022 05:11:45 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 21 Dec 2022 05:11:45 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 21 Dec 2022 05:11:46 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 21 Dec 2022 05:12:07 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 21 Dec 2022 05:12:07 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 21 Dec 2022 05:12:08 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 21 Dec 2022 05:12:08 GMT
USER adminer
# Wed, 21 Dec 2022 05:12:08 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:542880f4d15404af17d342ecbb76bb92724fc7cb8a91a5e18f26bd8f8811a38a`  
		Last Modified: Wed, 21 Dec 2022 01:22:46 GMT  
		Size: 58.9 MB (58897040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8c91d3a2eff19ff3291563333f250447b70f82929a98b439e9253b9d8909332`  
		Last Modified: Wed, 21 Dec 2022 05:12:53 GMT  
		Size: 40.6 MB (40618582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1fc5014e613c79f385d0565b105dfdc45badae00ab5a50f9b06955eb34e874d`  
		Last Modified: Wed, 21 Dec 2022 05:12:39 GMT  
		Size: 394.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5b74bb738e578f210c95db9d4fc2c314ce3454b4454d48e9fd0269bc6c207e8`  
		Last Modified: Wed, 21 Dec 2022 05:13:17 GMT  
		Size: 2.7 KB (2712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fd43780f4a97de99f2a70cbdeb1e9b998a4a0b78d33e413d5b202dfdc938ebb`  
		Last Modified: Wed, 21 Dec 2022 05:13:17 GMT  
		Size: 1.9 KB (1878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf0b6261dedf5bb3e0f0d3f02c0c41d44c78abd343b214d5e105040aecdbead8`  
		Last Modified: Wed, 21 Dec 2022 05:13:17 GMT  
		Size: 1.5 KB (1480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ffa54700428e518453fb0a542abf4e41ba28e7f58c380d6540691f0d3ded1a1`  
		Last Modified: Wed, 21 Dec 2022 05:13:17 GMT  
		Size: 1.4 MB (1383821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92c025b84e6aa9a000bd19d3eded000fba61196718941820ae5d1eba78d131c8`  
		Last Modified: Wed, 21 Dec 2022 05:13:17 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:fastcgi` - linux; s390x

```console
$ docker pull adminer@sha256:a1fa0d120584828c961ce0b29ab5d38c4bd62a7c4832051e8a59bdd185eaa72e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.4 MB (93404712 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:078ace26e901a591bccbb767862313e0b30444a61969a6f9563f56d8172155d7`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Wed, 21 Dec 2022 01:42:51 GMT
ADD file:22c4f2d41083ce4433bec4a71e7e6ddc5bec8e44e9cf2c9f93d0874b5b4de7c3 in / 
# Wed, 21 Dec 2022 01:42:54 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 02:06:42 GMT
STOPSIGNAL SIGINT
# Wed, 21 Dec 2022 02:07:51 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 02:08:00 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 21 Dec 2022 02:08:48 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Wed, 21 Dec 2022 02:08:50 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 21 Dec 2022 02:08:51 GMT
WORKDIR /var/www/html
# Wed, 21 Dec 2022 02:08:51 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 21 Dec 2022 02:08:52 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 21 Dec 2022 02:08:53 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 21 Dec 2022 02:08:53 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 21 Dec 2022 02:09:20 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 21 Dec 2022 02:09:21 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 21 Dec 2022 02:09:21 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 21 Dec 2022 02:09:22 GMT
USER adminer
# Wed, 21 Dec 2022 02:09:23 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:7f45294776f4c97d23f8dbfca98d4b57701b478eedfcb154a7e7dc6d6954ba44`  
		Last Modified: Wed, 21 Dec 2022 01:48:50 GMT  
		Size: 53.3 MB (53258472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8610ee81c430b6503a5ee2d7cc451175bdfc868fc17ef5a675b43679da433867`  
		Last Modified: Wed, 21 Dec 2022 02:10:03 GMT  
		Size: 38.8 MB (38755148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:211b726eee70a0c5ff85337d1e98c7987025435a41ca5421f47d96fc164b5b27`  
		Last Modified: Wed, 21 Dec 2022 02:09:56 GMT  
		Size: 395.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:548dc4ca6b10efd03438d3ef399c3d858053ec103194dba6350126f59b0cc988`  
		Last Modified: Wed, 21 Dec 2022 02:10:20 GMT  
		Size: 2.7 KB (2713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcd20979228556508e9e2424f45667a2246d9c409f2557492271740f4840e889`  
		Last Modified: Wed, 21 Dec 2022 02:10:20 GMT  
		Size: 1.9 KB (1883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2e7ff5c1ff35711cc296fbbe902ca0db4bc13c6b5863ba4c3adc2640e16177e`  
		Last Modified: Wed, 21 Dec 2022 02:10:20 GMT  
		Size: 1.5 KB (1481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:334c0739b3be2b837dcd345afc1a5bd12f907a3080d438abf00d8706d01e99c8`  
		Last Modified: Wed, 21 Dec 2022 02:10:20 GMT  
		Size: 1.4 MB (1384126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd966444e211f7ff2ff5aca0482cee29884580acd8b4114e8bd25b616618c89c`  
		Last Modified: Wed, 21 Dec 2022 02:10:21 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `adminer:latest`

```console
$ docker pull adminer@sha256:895823d11ab87b3ef3db1230b33d9347b0c4fd58e6188906af37b3e7353f383f
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
$ docker pull adminer@sha256:11d6176cead328bcc234f740d98dccda987d03c17d77e03bdceb508c9d35ba30
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.6 MB (95639696 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c207e90c34520f27508ac0a18405256f981ecb45aae2baa2835c91a8f1963f0a`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 21 Dec 2022 01:20:21 GMT
ADD file:c13b430c8699df107ffd9ea5230b92238bc037a8e1cbbe35d6ab664941d575da in / 
# Wed, 21 Dec 2022 01:20:22 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 01:43:34 GMT
STOPSIGNAL SIGINT
# Wed, 21 Dec 2022 01:43:57 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 01:43:58 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 21 Dec 2022 01:43:59 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 21 Dec 2022 01:43:59 GMT
WORKDIR /var/www/html
# Wed, 21 Dec 2022 01:43:59 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 21 Dec 2022 01:43:59 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 21 Dec 2022 01:43:59 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 21 Dec 2022 01:43:59 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 21 Dec 2022 01:44:12 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 21 Dec 2022 01:44:12 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 21 Dec 2022 01:44:12 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 21 Dec 2022 01:44:12 GMT
USER adminer
# Wed, 21 Dec 2022 01:44:12 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 21 Dec 2022 01:44:12 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:32de3c850997ce03b6ff4ae8fb00b34b9d7d7f9a35bfcdb8538e22cc7b77c29d`  
		Last Modified: Wed, 21 Dec 2022 01:24:10 GMT  
		Size: 55.0 MB (55025166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bddad460143b31cc21fc89d836e6d417bb718a19c27f93eb137aebd91b79660`  
		Last Modified: Wed, 21 Dec 2022 01:44:51 GMT  
		Size: 39.2 MB (39226473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bf0beaa0412c7e762322b7311a449203a96c1e115d99efca0dddce016279e6a`  
		Last Modified: Wed, 21 Dec 2022 01:44:43 GMT  
		Size: 394.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e7ee08ea648165938f5fde9ae603f33b34b10c2d4ad2e40ea8c04913db12b65`  
		Last Modified: Wed, 21 Dec 2022 01:44:43 GMT  
		Size: 1.9 KB (1888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd9f958670d2c87349fd96a19d4254adbc404b54b3911c6962d9119d1a6fe901`  
		Last Modified: Wed, 21 Dec 2022 01:44:43 GMT  
		Size: 1.5 KB (1477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:292984a5d9c1d2f389b01937cbdf2a19e8b9de4ed6719500f1310467b1a19ff5`  
		Last Modified: Wed, 21 Dec 2022 01:44:44 GMT  
		Size: 1.4 MB (1383807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20a148ad3aa6178c7d0e684fcbc70c4ca4ba27ea5f13560aef5219a63b2b6874`  
		Last Modified: Wed, 21 Dec 2022 01:44:43 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:latest` - linux; arm variant v5

```console
$ docker pull adminer@sha256:50640fef3243132e1ea5d5081f834e0ca156c8264c0b0441a43492f4a4eeca23
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.9 MB (90901373 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:250a1b3ad0e6461afc53655c14f3a5b1378d898200c7bdef2f11ad58335fe9a2`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 21 Dec 2022 01:48:53 GMT
ADD file:81ccc74e0ea343972e2f3f46d2da7e9b808d9718be44d4afa7bec6904b7ab9c6 in / 
# Wed, 21 Dec 2022 01:48:55 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 02:12:35 GMT
STOPSIGNAL SIGINT
# Wed, 21 Dec 2022 02:13:07 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 02:13:09 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 21 Dec 2022 02:13:10 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 21 Dec 2022 02:13:10 GMT
WORKDIR /var/www/html
# Wed, 21 Dec 2022 02:13:10 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 21 Dec 2022 02:13:10 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 21 Dec 2022 02:13:10 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 21 Dec 2022 02:13:10 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 21 Dec 2022 02:13:27 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 21 Dec 2022 02:13:27 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 21 Dec 2022 02:13:27 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 21 Dec 2022 02:13:27 GMT
USER adminer
# Wed, 21 Dec 2022 02:13:27 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 21 Dec 2022 02:13:27 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:89b6e4f9f2f811282495a047e873c20d6ac2d53c72ad576a6907b1449eb3e635`  
		Last Modified: Wed, 21 Dec 2022 01:53:30 GMT  
		Size: 52.5 MB (52529974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2473783a5bf521f1fdf370edfbbd3a71c7d41bd6ad586832334a5359d21e0937`  
		Last Modified: Wed, 21 Dec 2022 02:14:50 GMT  
		Size: 37.0 MB (36983598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fb144c6fa4674d630705477694c2b1a78efcb47a43b11b84d11420c6672d849`  
		Last Modified: Wed, 21 Dec 2022 02:14:41 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7d2eaadeb68edbb519fcd0f769e3e17f2744670df98e1f42b2dd32755e43260`  
		Last Modified: Wed, 21 Dec 2022 02:14:41 GMT  
		Size: 1.8 KB (1840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57c2b47fd023120badcfed4eb901caaff2b0fb6b5d48de329e15232469b9af23`  
		Last Modified: Wed, 21 Dec 2022 02:14:41 GMT  
		Size: 1.5 KB (1481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54fcbf1f604d9098ea8ed2239603e5aa978d84db1258c72c4a54a6aa095ec76f`  
		Last Modified: Wed, 21 Dec 2022 02:14:41 GMT  
		Size: 1.4 MB (1383596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:216e1a8363d45d45df8c6cbfe9f7ee9909da57c723cd447b01a248fb042840f3`  
		Last Modified: Wed, 21 Dec 2022 02:14:41 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:latest` - linux; arm variant v7

```console
$ docker pull adminer@sha256:667b9904f45244f6db8f25daad4eea200d6c4a4f91c68de564a5caf5a4c6a5c5
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.5 MB (87525670 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4da555d48a0530a78c590fbbf78d89a6283e3bf8436c4028fc44739c58ed9fd4`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 21 Dec 2022 01:58:09 GMT
ADD file:4b6f71680de34554595f062f9e52037b48edf19ca8f34c75877caa85c42caad3 in / 
# Wed, 21 Dec 2022 01:58:10 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 16:55:05 GMT
STOPSIGNAL SIGINT
# Wed, 21 Dec 2022 16:55:27 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 16:55:28 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 21 Dec 2022 16:55:29 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 21 Dec 2022 16:55:29 GMT
WORKDIR /var/www/html
# Wed, 21 Dec 2022 16:55:29 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 21 Dec 2022 16:55:29 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 21 Dec 2022 16:55:29 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 21 Dec 2022 16:55:29 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 21 Dec 2022 16:55:42 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 21 Dec 2022 16:55:42 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 21 Dec 2022 16:55:42 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 21 Dec 2022 16:55:42 GMT
USER adminer
# Wed, 21 Dec 2022 16:55:42 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 21 Dec 2022 16:55:42 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:706bb1d74512e1fb9ba97aa9212a32d07726fbfe77e4c7e609406d2065418f57`  
		Last Modified: Wed, 21 Dec 2022 02:04:37 GMT  
		Size: 50.2 MB (50190771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a1c5cd5ac0e733e02567c893f1028628f441423281df1c54fa1042b317bb758`  
		Last Modified: Wed, 21 Dec 2022 16:56:48 GMT  
		Size: 35.9 MB (35947077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3d69909ab6c9fd65668b2d644bbb5375f5617c8bba9e82704145b53e895ad98`  
		Last Modified: Wed, 21 Dec 2022 16:56:39 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be622d99b39d413b273b3c6344f0cf7b97883297c9e7fb52951cca9bafd33f3a`  
		Last Modified: Wed, 21 Dec 2022 16:56:39 GMT  
		Size: 1.8 KB (1840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:546d6a7c782f341de9ea0c0c9aa227a5fa0d870146d87f59cb4d319c5b895028`  
		Last Modified: Wed, 21 Dec 2022 16:56:39 GMT  
		Size: 1.5 KB (1479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e94d73593abc9542a40f6e2f989f35a2bebbb21e554c4d2452cee59089701ca5`  
		Last Modified: Wed, 21 Dec 2022 16:56:39 GMT  
		Size: 1.4 MB (1383619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f3795d41125166e2051354d7af4622abe6b7610551670476d49ad99c372bad6`  
		Last Modified: Wed, 21 Dec 2022 16:56:39 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:latest` - linux; arm64 variant v8

```console
$ docker pull adminer@sha256:2e15c1b18293cc812ca73063a33ca295e6e5b4011ab43006f371bf3d63f7a387
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.0 MB (94046599 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f2678931127cd62d7af0ee195d7008f84b549fb9374257d1696f7cc5c9dab049`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 21 Dec 2022 01:39:40 GMT
ADD file:5bbdc914ec8ed60ac85293e88ee1aafc3f0290762e320fc86dc9d79fa201834e in / 
# Wed, 21 Dec 2022 01:39:41 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 02:01:54 GMT
STOPSIGNAL SIGINT
# Wed, 21 Dec 2022 02:02:11 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 02:02:12 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 21 Dec 2022 02:02:12 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 21 Dec 2022 02:02:13 GMT
WORKDIR /var/www/html
# Wed, 21 Dec 2022 02:02:13 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 21 Dec 2022 02:02:13 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 21 Dec 2022 02:02:13 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 21 Dec 2022 02:02:13 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 21 Dec 2022 02:02:23 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 21 Dec 2022 02:02:24 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 21 Dec 2022 02:02:24 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 21 Dec 2022 02:02:24 GMT
USER adminer
# Wed, 21 Dec 2022 02:02:24 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 21 Dec 2022 02:02:24 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:c3e6129b48b69d14c5e7a5605e2b94003fb71aac82eac46b8689f5b8007af2c5`  
		Last Modified: Wed, 21 Dec 2022 01:42:49 GMT  
		Size: 53.7 MB (53681797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:235cb929f19f47af31496a0a93a9cb1fd8f5104f0d34a160f4d2e4d6b9463df1`  
		Last Modified: Wed, 21 Dec 2022 02:02:59 GMT  
		Size: 39.0 MB (38976852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a72d5ac588c6b24f2d8a511e934c2745420b4536a9fa914031e10c9d384efd2b`  
		Last Modified: Wed, 21 Dec 2022 02:02:52 GMT  
		Size: 392.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c1912d1c0826d94d3aa328472384e502a58e992b77df780de62bbe9ba9f744e`  
		Last Modified: Wed, 21 Dec 2022 02:02:52 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f6d91a33867afb4cdea48a709f3cd43416c387bbf8a96e04840822e05a249eb`  
		Last Modified: Wed, 21 Dec 2022 02:02:52 GMT  
		Size: 1.5 KB (1481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a85debe3d62cce517ab60af785fce8ae30d5633d41e755d25700acfaa96f427`  
		Last Modified: Wed, 21 Dec 2022 02:02:53 GMT  
		Size: 1.4 MB (1383704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c707a54ab9eee88dee88a920652b121430b0f93f2599e1f3d29cd8ee7f91a359`  
		Last Modified: Wed, 21 Dec 2022 02:02:52 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:latest` - linux; 386

```console
$ docker pull adminer@sha256:d219efb2aecebb6bd16280905d0c7ff80b18ad7269350fec6bd034d2a093976d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.7 MB (96663116 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a504b1b6ca371056530865e9620cc9e4dabcd05dd93ab1f5b1dc2092bf6656e2`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 21 Dec 2022 01:39:08 GMT
ADD file:10d2f443f55d8ba9512899b3dff08f6e9a6c7ca096f407e3477e9798e1063785 in / 
# Wed, 21 Dec 2022 01:39:09 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 02:04:14 GMT
STOPSIGNAL SIGINT
# Wed, 21 Dec 2022 02:04:35 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 02:04:36 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 21 Dec 2022 02:04:37 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 21 Dec 2022 02:04:38 GMT
WORKDIR /var/www/html
# Wed, 21 Dec 2022 02:04:40 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 21 Dec 2022 02:04:40 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 21 Dec 2022 02:04:41 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 21 Dec 2022 02:04:42 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 21 Dec 2022 02:04:55 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 21 Dec 2022 02:04:57 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 21 Dec 2022 02:04:57 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 21 Dec 2022 02:04:58 GMT
USER adminer
# Wed, 21 Dec 2022 02:04:59 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 21 Dec 2022 02:05:00 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:bde501e1d960005aee2bdf2fc8c89b26bf694dace8740c72deda4d7705995ab7`  
		Last Modified: Wed, 21 Dec 2022 01:44:18 GMT  
		Size: 56.0 MB (56005267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd60bbc5dc31d7ec1db0a2fbd068c29f7583f7d3e2d0599f0706680ce602ee9d`  
		Last Modified: Wed, 21 Dec 2022 02:06:03 GMT  
		Size: 39.3 MB (39269700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b30e5dcb4252f7f6ded0a9c044209070412dbf7df3daab7e7343bc6bf568fe67`  
		Last Modified: Wed, 21 Dec 2022 02:05:50 GMT  
		Size: 394.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:387e2851bc00ff07433e8e9d3d12cdc6590937cbf4a9de8a035771e386a0e3c4`  
		Last Modified: Wed, 21 Dec 2022 02:05:50 GMT  
		Size: 1.7 KB (1718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c04056306aff55b02341e716626152ea622c4326e3f31a4a39bce3d631152fea`  
		Last Modified: Wed, 21 Dec 2022 02:05:50 GMT  
		Size: 1.5 KB (1478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31f79e3e185cbecc304f97fe83e64bc102e782154ed533744186d41a6de680fb`  
		Last Modified: Wed, 21 Dec 2022 02:05:51 GMT  
		Size: 1.4 MB (1384066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce0359a7ffb52c577cc47d0136aeed97a19a7e826d80ebb7b304977f271a6f7d`  
		Last Modified: Wed, 21 Dec 2022 02:05:51 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:latest` - linux; mips64le

```console
$ docker pull adminer@sha256:74a7ae91c85961c3ad967ae1cf25d79b8d7a69a6668843b885aebcc169a7f88f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.3 MB (92326851 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0992a9b14a478d0bfd67839ed2e77e40a770492ebd4daa67c6141cd734519bb1`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Tue, 06 Dec 2022 01:54:55 GMT
ADD file:09d48994a41c54566f7123db033773e6246c0703a518af76843198196cd39645 in / 
# Tue, 06 Dec 2022 01:55:00 GMT
CMD ["bash"]
# Sat, 17 Dec 2022 01:31:42 GMT
STOPSIGNAL SIGINT
# Sat, 17 Dec 2022 01:33:37 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Sat, 17 Dec 2022 01:33:43 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Sat, 17 Dec 2022 01:33:49 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Sat, 17 Dec 2022 01:33:53 GMT
WORKDIR /var/www/html
# Sat, 17 Dec 2022 01:33:56 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Sat, 17 Dec 2022 01:33:59 GMT
ENV ADMINER_VERSION=4.8.1
# Sat, 17 Dec 2022 01:34:02 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Sat, 17 Dec 2022 01:34:05 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Sat, 17 Dec 2022 01:34:57 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 17 Dec 2022 01:35:00 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Sat, 17 Dec 2022 01:35:03 GMT
ENTRYPOINT ["entrypoint.sh"]
# Sat, 17 Dec 2022 01:35:06 GMT
USER adminer
# Sat, 17 Dec 2022 01:35:09 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Sat, 17 Dec 2022 01:35:13 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:acb57a81743c28ead1a32571c107ac15cd970593fea4f2954b57f22e6bbad1d0`  
		Last Modified: Tue, 06 Dec 2022 02:02:59 GMT  
		Size: 53.3 MB (53260631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16a0a73e4e15363c91b94686e7609b1d84bd3ab5f4c13b2302e76c23e58ca18f`  
		Last Modified: Sat, 17 Dec 2022 01:38:30 GMT  
		Size: 37.7 MB (37676049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8aebeb122c3b2bc8c5262621178cece53cdab93feb29828240f598aa1c86637`  
		Last Modified: Sat, 17 Dec 2022 01:38:02 GMT  
		Size: 395.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3c1363529deb53f7595176aa5b55b04ab1cdf841a6cd3cdb88c41d6ec75615f`  
		Last Modified: Sat, 17 Dec 2022 01:38:02 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0923c943bb7440a1b68c2494f1f23c0a3199d4d3a6cdb87bdca8067acfbe4d4`  
		Last Modified: Sat, 17 Dec 2022 01:38:02 GMT  
		Size: 1.5 KB (1485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47a69745dad2c95e6d8ff413ca73cc902100c3848af39c316ae44ec375f8aae7`  
		Last Modified: Sat, 17 Dec 2022 01:38:03 GMT  
		Size: 1.4 MB (1386065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2548a3e7b136720a8c94faa9137694506f95bcf701a80d8b49486c2a3be6205b`  
		Last Modified: Sat, 17 Dec 2022 01:38:02 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:latest` - linux; ppc64le

```console
$ docker pull adminer@sha256:86fbf5aa76cfa4052c3d9bf35b81e34daf0fb53fbc674d612c071ca9a60de5ce
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.9 MB (100903714 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:075df6bcff3df963b2eec2efff06fef0b4f316e1751a5ebc98880754503bcf54`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 21 Dec 2022 01:17:21 GMT
ADD file:c95bdb0df70fa9ce48b31a7ceb8a7be0c5b925efcf01c43595868b86994dc192 in / 
# Wed, 21 Dec 2022 01:17:25 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 05:10:17 GMT
STOPSIGNAL SIGINT
# Wed, 21 Dec 2022 05:11:02 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 05:11:05 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 21 Dec 2022 05:11:07 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 21 Dec 2022 05:11:07 GMT
WORKDIR /var/www/html
# Wed, 21 Dec 2022 05:11:07 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 21 Dec 2022 05:11:08 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 21 Dec 2022 05:11:08 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 21 Dec 2022 05:11:09 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 21 Dec 2022 05:11:31 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 21 Dec 2022 05:11:31 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 21 Dec 2022 05:11:32 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 21 Dec 2022 05:11:32 GMT
USER adminer
# Wed, 21 Dec 2022 05:11:32 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 21 Dec 2022 05:11:33 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:542880f4d15404af17d342ecbb76bb92724fc7cb8a91a5e18f26bd8f8811a38a`  
		Last Modified: Wed, 21 Dec 2022 01:22:46 GMT  
		Size: 58.9 MB (58897040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8c91d3a2eff19ff3291563333f250447b70f82929a98b439e9253b9d8909332`  
		Last Modified: Wed, 21 Dec 2022 05:12:53 GMT  
		Size: 40.6 MB (40618582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1fc5014e613c79f385d0565b105dfdc45badae00ab5a50f9b06955eb34e874d`  
		Last Modified: Wed, 21 Dec 2022 05:12:39 GMT  
		Size: 394.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc90d97148640f4f164e3dc4b1f043c6ba7d8b5cddd21ede8a947339a13e3c3f`  
		Last Modified: Wed, 21 Dec 2022 05:12:39 GMT  
		Size: 1.9 KB (1879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdfe2d4e5fb66793ea99cc5959183331088d985dc203754a30a8bf6bbffb186a`  
		Last Modified: Wed, 21 Dec 2022 05:12:39 GMT  
		Size: 1.5 KB (1482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0da8c96b4d9b013ebbf00af4b8693e634764cf159be7af73d3152403cabe71e5`  
		Last Modified: Wed, 21 Dec 2022 05:12:40 GMT  
		Size: 1.4 MB (1383844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:061e859636ca9e27f80e25b38a893f2e38d08dd68c7a53bc8fb9f428dfb0f328`  
		Last Modified: Wed, 21 Dec 2022 05:12:39 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:latest` - linux; s390x

```console
$ docker pull adminer@sha256:4ad639f239b5117cf7381d37948390122d8f514592dade423c1fbdc4870c04b4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.4 MB (93401988 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac7114a00edb645cd010878538757f757f872e25c530cb9159f5bc03cc191726`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 21 Dec 2022 01:42:51 GMT
ADD file:22c4f2d41083ce4433bec4a71e7e6ddc5bec8e44e9cf2c9f93d0874b5b4de7c3 in / 
# Wed, 21 Dec 2022 01:42:54 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 02:06:42 GMT
STOPSIGNAL SIGINT
# Wed, 21 Dec 2022 02:07:51 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 02:08:00 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 21 Dec 2022 02:08:02 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 21 Dec 2022 02:08:03 GMT
WORKDIR /var/www/html
# Wed, 21 Dec 2022 02:08:04 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 21 Dec 2022 02:08:04 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 21 Dec 2022 02:08:05 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 21 Dec 2022 02:08:06 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 21 Dec 2022 02:08:33 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 21 Dec 2022 02:08:33 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 21 Dec 2022 02:08:34 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 21 Dec 2022 02:08:35 GMT
USER adminer
# Wed, 21 Dec 2022 02:08:35 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 21 Dec 2022 02:08:36 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:7f45294776f4c97d23f8dbfca98d4b57701b478eedfcb154a7e7dc6d6954ba44`  
		Last Modified: Wed, 21 Dec 2022 01:48:50 GMT  
		Size: 53.3 MB (53258472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8610ee81c430b6503a5ee2d7cc451175bdfc868fc17ef5a675b43679da433867`  
		Last Modified: Wed, 21 Dec 2022 02:10:03 GMT  
		Size: 38.8 MB (38755148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:211b726eee70a0c5ff85337d1e98c7987025435a41ca5421f47d96fc164b5b27`  
		Last Modified: Wed, 21 Dec 2022 02:09:56 GMT  
		Size: 395.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c6a1fa2154f900c32f87164afe347f0dddbb7a641dc81b7fc436b1d15a5349d`  
		Last Modified: Wed, 21 Dec 2022 02:09:56 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e030c793dfbf87ef1f5dbbecd22117bcf1695eb293e41bca267fb29d0e98d59d`  
		Last Modified: Wed, 21 Dec 2022 02:09:56 GMT  
		Size: 1.5 KB (1478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:965c9f68e6765f8a5967198527ce6ff7bf0646cab60aa30ecef97747554c0869`  
		Last Modified: Wed, 21 Dec 2022 02:09:56 GMT  
		Size: 1.4 MB (1384122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d34b801ca3351132a2f2914bc4ef3ca0f91a2c87c2b42fce3662fd5f20593aea`  
		Last Modified: Wed, 21 Dec 2022 02:09:56 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `adminer:standalone`

```console
$ docker pull adminer@sha256:895823d11ab87b3ef3db1230b33d9347b0c4fd58e6188906af37b3e7353f383f
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
$ docker pull adminer@sha256:11d6176cead328bcc234f740d98dccda987d03c17d77e03bdceb508c9d35ba30
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.6 MB (95639696 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c207e90c34520f27508ac0a18405256f981ecb45aae2baa2835c91a8f1963f0a`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 21 Dec 2022 01:20:21 GMT
ADD file:c13b430c8699df107ffd9ea5230b92238bc037a8e1cbbe35d6ab664941d575da in / 
# Wed, 21 Dec 2022 01:20:22 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 01:43:34 GMT
STOPSIGNAL SIGINT
# Wed, 21 Dec 2022 01:43:57 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 01:43:58 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 21 Dec 2022 01:43:59 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 21 Dec 2022 01:43:59 GMT
WORKDIR /var/www/html
# Wed, 21 Dec 2022 01:43:59 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 21 Dec 2022 01:43:59 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 21 Dec 2022 01:43:59 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 21 Dec 2022 01:43:59 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 21 Dec 2022 01:44:12 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 21 Dec 2022 01:44:12 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 21 Dec 2022 01:44:12 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 21 Dec 2022 01:44:12 GMT
USER adminer
# Wed, 21 Dec 2022 01:44:12 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 21 Dec 2022 01:44:12 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:32de3c850997ce03b6ff4ae8fb00b34b9d7d7f9a35bfcdb8538e22cc7b77c29d`  
		Last Modified: Wed, 21 Dec 2022 01:24:10 GMT  
		Size: 55.0 MB (55025166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bddad460143b31cc21fc89d836e6d417bb718a19c27f93eb137aebd91b79660`  
		Last Modified: Wed, 21 Dec 2022 01:44:51 GMT  
		Size: 39.2 MB (39226473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bf0beaa0412c7e762322b7311a449203a96c1e115d99efca0dddce016279e6a`  
		Last Modified: Wed, 21 Dec 2022 01:44:43 GMT  
		Size: 394.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e7ee08ea648165938f5fde9ae603f33b34b10c2d4ad2e40ea8c04913db12b65`  
		Last Modified: Wed, 21 Dec 2022 01:44:43 GMT  
		Size: 1.9 KB (1888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd9f958670d2c87349fd96a19d4254adbc404b54b3911c6962d9119d1a6fe901`  
		Last Modified: Wed, 21 Dec 2022 01:44:43 GMT  
		Size: 1.5 KB (1477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:292984a5d9c1d2f389b01937cbdf2a19e8b9de4ed6719500f1310467b1a19ff5`  
		Last Modified: Wed, 21 Dec 2022 01:44:44 GMT  
		Size: 1.4 MB (1383807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20a148ad3aa6178c7d0e684fcbc70c4ca4ba27ea5f13560aef5219a63b2b6874`  
		Last Modified: Wed, 21 Dec 2022 01:44:43 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:standalone` - linux; arm variant v5

```console
$ docker pull adminer@sha256:50640fef3243132e1ea5d5081f834e0ca156c8264c0b0441a43492f4a4eeca23
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.9 MB (90901373 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:250a1b3ad0e6461afc53655c14f3a5b1378d898200c7bdef2f11ad58335fe9a2`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 21 Dec 2022 01:48:53 GMT
ADD file:81ccc74e0ea343972e2f3f46d2da7e9b808d9718be44d4afa7bec6904b7ab9c6 in / 
# Wed, 21 Dec 2022 01:48:55 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 02:12:35 GMT
STOPSIGNAL SIGINT
# Wed, 21 Dec 2022 02:13:07 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 02:13:09 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 21 Dec 2022 02:13:10 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 21 Dec 2022 02:13:10 GMT
WORKDIR /var/www/html
# Wed, 21 Dec 2022 02:13:10 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 21 Dec 2022 02:13:10 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 21 Dec 2022 02:13:10 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 21 Dec 2022 02:13:10 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 21 Dec 2022 02:13:27 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 21 Dec 2022 02:13:27 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 21 Dec 2022 02:13:27 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 21 Dec 2022 02:13:27 GMT
USER adminer
# Wed, 21 Dec 2022 02:13:27 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 21 Dec 2022 02:13:27 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:89b6e4f9f2f811282495a047e873c20d6ac2d53c72ad576a6907b1449eb3e635`  
		Last Modified: Wed, 21 Dec 2022 01:53:30 GMT  
		Size: 52.5 MB (52529974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2473783a5bf521f1fdf370edfbbd3a71c7d41bd6ad586832334a5359d21e0937`  
		Last Modified: Wed, 21 Dec 2022 02:14:50 GMT  
		Size: 37.0 MB (36983598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fb144c6fa4674d630705477694c2b1a78efcb47a43b11b84d11420c6672d849`  
		Last Modified: Wed, 21 Dec 2022 02:14:41 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7d2eaadeb68edbb519fcd0f769e3e17f2744670df98e1f42b2dd32755e43260`  
		Last Modified: Wed, 21 Dec 2022 02:14:41 GMT  
		Size: 1.8 KB (1840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57c2b47fd023120badcfed4eb901caaff2b0fb6b5d48de329e15232469b9af23`  
		Last Modified: Wed, 21 Dec 2022 02:14:41 GMT  
		Size: 1.5 KB (1481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54fcbf1f604d9098ea8ed2239603e5aa978d84db1258c72c4a54a6aa095ec76f`  
		Last Modified: Wed, 21 Dec 2022 02:14:41 GMT  
		Size: 1.4 MB (1383596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:216e1a8363d45d45df8c6cbfe9f7ee9909da57c723cd447b01a248fb042840f3`  
		Last Modified: Wed, 21 Dec 2022 02:14:41 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:standalone` - linux; arm variant v7

```console
$ docker pull adminer@sha256:667b9904f45244f6db8f25daad4eea200d6c4a4f91c68de564a5caf5a4c6a5c5
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.5 MB (87525670 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4da555d48a0530a78c590fbbf78d89a6283e3bf8436c4028fc44739c58ed9fd4`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 21 Dec 2022 01:58:09 GMT
ADD file:4b6f71680de34554595f062f9e52037b48edf19ca8f34c75877caa85c42caad3 in / 
# Wed, 21 Dec 2022 01:58:10 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 16:55:05 GMT
STOPSIGNAL SIGINT
# Wed, 21 Dec 2022 16:55:27 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 16:55:28 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 21 Dec 2022 16:55:29 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 21 Dec 2022 16:55:29 GMT
WORKDIR /var/www/html
# Wed, 21 Dec 2022 16:55:29 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 21 Dec 2022 16:55:29 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 21 Dec 2022 16:55:29 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 21 Dec 2022 16:55:29 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 21 Dec 2022 16:55:42 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 21 Dec 2022 16:55:42 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 21 Dec 2022 16:55:42 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 21 Dec 2022 16:55:42 GMT
USER adminer
# Wed, 21 Dec 2022 16:55:42 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 21 Dec 2022 16:55:42 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:706bb1d74512e1fb9ba97aa9212a32d07726fbfe77e4c7e609406d2065418f57`  
		Last Modified: Wed, 21 Dec 2022 02:04:37 GMT  
		Size: 50.2 MB (50190771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a1c5cd5ac0e733e02567c893f1028628f441423281df1c54fa1042b317bb758`  
		Last Modified: Wed, 21 Dec 2022 16:56:48 GMT  
		Size: 35.9 MB (35947077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3d69909ab6c9fd65668b2d644bbb5375f5617c8bba9e82704145b53e895ad98`  
		Last Modified: Wed, 21 Dec 2022 16:56:39 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be622d99b39d413b273b3c6344f0cf7b97883297c9e7fb52951cca9bafd33f3a`  
		Last Modified: Wed, 21 Dec 2022 16:56:39 GMT  
		Size: 1.8 KB (1840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:546d6a7c782f341de9ea0c0c9aa227a5fa0d870146d87f59cb4d319c5b895028`  
		Last Modified: Wed, 21 Dec 2022 16:56:39 GMT  
		Size: 1.5 KB (1479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e94d73593abc9542a40f6e2f989f35a2bebbb21e554c4d2452cee59089701ca5`  
		Last Modified: Wed, 21 Dec 2022 16:56:39 GMT  
		Size: 1.4 MB (1383619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f3795d41125166e2051354d7af4622abe6b7610551670476d49ad99c372bad6`  
		Last Modified: Wed, 21 Dec 2022 16:56:39 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:standalone` - linux; arm64 variant v8

```console
$ docker pull adminer@sha256:2e15c1b18293cc812ca73063a33ca295e6e5b4011ab43006f371bf3d63f7a387
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.0 MB (94046599 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f2678931127cd62d7af0ee195d7008f84b549fb9374257d1696f7cc5c9dab049`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 21 Dec 2022 01:39:40 GMT
ADD file:5bbdc914ec8ed60ac85293e88ee1aafc3f0290762e320fc86dc9d79fa201834e in / 
# Wed, 21 Dec 2022 01:39:41 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 02:01:54 GMT
STOPSIGNAL SIGINT
# Wed, 21 Dec 2022 02:02:11 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 02:02:12 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 21 Dec 2022 02:02:12 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 21 Dec 2022 02:02:13 GMT
WORKDIR /var/www/html
# Wed, 21 Dec 2022 02:02:13 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 21 Dec 2022 02:02:13 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 21 Dec 2022 02:02:13 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 21 Dec 2022 02:02:13 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 21 Dec 2022 02:02:23 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 21 Dec 2022 02:02:24 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 21 Dec 2022 02:02:24 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 21 Dec 2022 02:02:24 GMT
USER adminer
# Wed, 21 Dec 2022 02:02:24 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 21 Dec 2022 02:02:24 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:c3e6129b48b69d14c5e7a5605e2b94003fb71aac82eac46b8689f5b8007af2c5`  
		Last Modified: Wed, 21 Dec 2022 01:42:49 GMT  
		Size: 53.7 MB (53681797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:235cb929f19f47af31496a0a93a9cb1fd8f5104f0d34a160f4d2e4d6b9463df1`  
		Last Modified: Wed, 21 Dec 2022 02:02:59 GMT  
		Size: 39.0 MB (38976852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a72d5ac588c6b24f2d8a511e934c2745420b4536a9fa914031e10c9d384efd2b`  
		Last Modified: Wed, 21 Dec 2022 02:02:52 GMT  
		Size: 392.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c1912d1c0826d94d3aa328472384e502a58e992b77df780de62bbe9ba9f744e`  
		Last Modified: Wed, 21 Dec 2022 02:02:52 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f6d91a33867afb4cdea48a709f3cd43416c387bbf8a96e04840822e05a249eb`  
		Last Modified: Wed, 21 Dec 2022 02:02:52 GMT  
		Size: 1.5 KB (1481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a85debe3d62cce517ab60af785fce8ae30d5633d41e755d25700acfaa96f427`  
		Last Modified: Wed, 21 Dec 2022 02:02:53 GMT  
		Size: 1.4 MB (1383704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c707a54ab9eee88dee88a920652b121430b0f93f2599e1f3d29cd8ee7f91a359`  
		Last Modified: Wed, 21 Dec 2022 02:02:52 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:standalone` - linux; 386

```console
$ docker pull adminer@sha256:d219efb2aecebb6bd16280905d0c7ff80b18ad7269350fec6bd034d2a093976d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.7 MB (96663116 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a504b1b6ca371056530865e9620cc9e4dabcd05dd93ab1f5b1dc2092bf6656e2`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 21 Dec 2022 01:39:08 GMT
ADD file:10d2f443f55d8ba9512899b3dff08f6e9a6c7ca096f407e3477e9798e1063785 in / 
# Wed, 21 Dec 2022 01:39:09 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 02:04:14 GMT
STOPSIGNAL SIGINT
# Wed, 21 Dec 2022 02:04:35 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 02:04:36 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 21 Dec 2022 02:04:37 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 21 Dec 2022 02:04:38 GMT
WORKDIR /var/www/html
# Wed, 21 Dec 2022 02:04:40 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 21 Dec 2022 02:04:40 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 21 Dec 2022 02:04:41 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 21 Dec 2022 02:04:42 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 21 Dec 2022 02:04:55 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 21 Dec 2022 02:04:57 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 21 Dec 2022 02:04:57 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 21 Dec 2022 02:04:58 GMT
USER adminer
# Wed, 21 Dec 2022 02:04:59 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 21 Dec 2022 02:05:00 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:bde501e1d960005aee2bdf2fc8c89b26bf694dace8740c72deda4d7705995ab7`  
		Last Modified: Wed, 21 Dec 2022 01:44:18 GMT  
		Size: 56.0 MB (56005267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd60bbc5dc31d7ec1db0a2fbd068c29f7583f7d3e2d0599f0706680ce602ee9d`  
		Last Modified: Wed, 21 Dec 2022 02:06:03 GMT  
		Size: 39.3 MB (39269700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b30e5dcb4252f7f6ded0a9c044209070412dbf7df3daab7e7343bc6bf568fe67`  
		Last Modified: Wed, 21 Dec 2022 02:05:50 GMT  
		Size: 394.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:387e2851bc00ff07433e8e9d3d12cdc6590937cbf4a9de8a035771e386a0e3c4`  
		Last Modified: Wed, 21 Dec 2022 02:05:50 GMT  
		Size: 1.7 KB (1718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c04056306aff55b02341e716626152ea622c4326e3f31a4a39bce3d631152fea`  
		Last Modified: Wed, 21 Dec 2022 02:05:50 GMT  
		Size: 1.5 KB (1478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31f79e3e185cbecc304f97fe83e64bc102e782154ed533744186d41a6de680fb`  
		Last Modified: Wed, 21 Dec 2022 02:05:51 GMT  
		Size: 1.4 MB (1384066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce0359a7ffb52c577cc47d0136aeed97a19a7e826d80ebb7b304977f271a6f7d`  
		Last Modified: Wed, 21 Dec 2022 02:05:51 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:standalone` - linux; mips64le

```console
$ docker pull adminer@sha256:74a7ae91c85961c3ad967ae1cf25d79b8d7a69a6668843b885aebcc169a7f88f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.3 MB (92326851 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0992a9b14a478d0bfd67839ed2e77e40a770492ebd4daa67c6141cd734519bb1`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Tue, 06 Dec 2022 01:54:55 GMT
ADD file:09d48994a41c54566f7123db033773e6246c0703a518af76843198196cd39645 in / 
# Tue, 06 Dec 2022 01:55:00 GMT
CMD ["bash"]
# Sat, 17 Dec 2022 01:31:42 GMT
STOPSIGNAL SIGINT
# Sat, 17 Dec 2022 01:33:37 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Sat, 17 Dec 2022 01:33:43 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Sat, 17 Dec 2022 01:33:49 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Sat, 17 Dec 2022 01:33:53 GMT
WORKDIR /var/www/html
# Sat, 17 Dec 2022 01:33:56 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Sat, 17 Dec 2022 01:33:59 GMT
ENV ADMINER_VERSION=4.8.1
# Sat, 17 Dec 2022 01:34:02 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Sat, 17 Dec 2022 01:34:05 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Sat, 17 Dec 2022 01:34:57 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Sat, 17 Dec 2022 01:35:00 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Sat, 17 Dec 2022 01:35:03 GMT
ENTRYPOINT ["entrypoint.sh"]
# Sat, 17 Dec 2022 01:35:06 GMT
USER adminer
# Sat, 17 Dec 2022 01:35:09 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Sat, 17 Dec 2022 01:35:13 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:acb57a81743c28ead1a32571c107ac15cd970593fea4f2954b57f22e6bbad1d0`  
		Last Modified: Tue, 06 Dec 2022 02:02:59 GMT  
		Size: 53.3 MB (53260631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16a0a73e4e15363c91b94686e7609b1d84bd3ab5f4c13b2302e76c23e58ca18f`  
		Last Modified: Sat, 17 Dec 2022 01:38:30 GMT  
		Size: 37.7 MB (37676049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8aebeb122c3b2bc8c5262621178cece53cdab93feb29828240f598aa1c86637`  
		Last Modified: Sat, 17 Dec 2022 01:38:02 GMT  
		Size: 395.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3c1363529deb53f7595176aa5b55b04ab1cdf841a6cd3cdb88c41d6ec75615f`  
		Last Modified: Sat, 17 Dec 2022 01:38:02 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0923c943bb7440a1b68c2494f1f23c0a3199d4d3a6cdb87bdca8067acfbe4d4`  
		Last Modified: Sat, 17 Dec 2022 01:38:02 GMT  
		Size: 1.5 KB (1485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47a69745dad2c95e6d8ff413ca73cc902100c3848af39c316ae44ec375f8aae7`  
		Last Modified: Sat, 17 Dec 2022 01:38:03 GMT  
		Size: 1.4 MB (1386065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2548a3e7b136720a8c94faa9137694506f95bcf701a80d8b49486c2a3be6205b`  
		Last Modified: Sat, 17 Dec 2022 01:38:02 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:standalone` - linux; ppc64le

```console
$ docker pull adminer@sha256:86fbf5aa76cfa4052c3d9bf35b81e34daf0fb53fbc674d612c071ca9a60de5ce
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.9 MB (100903714 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:075df6bcff3df963b2eec2efff06fef0b4f316e1751a5ebc98880754503bcf54`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 21 Dec 2022 01:17:21 GMT
ADD file:c95bdb0df70fa9ce48b31a7ceb8a7be0c5b925efcf01c43595868b86994dc192 in / 
# Wed, 21 Dec 2022 01:17:25 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 05:10:17 GMT
STOPSIGNAL SIGINT
# Wed, 21 Dec 2022 05:11:02 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 05:11:05 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 21 Dec 2022 05:11:07 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 21 Dec 2022 05:11:07 GMT
WORKDIR /var/www/html
# Wed, 21 Dec 2022 05:11:07 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 21 Dec 2022 05:11:08 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 21 Dec 2022 05:11:08 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 21 Dec 2022 05:11:09 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 21 Dec 2022 05:11:31 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 21 Dec 2022 05:11:31 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 21 Dec 2022 05:11:32 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 21 Dec 2022 05:11:32 GMT
USER adminer
# Wed, 21 Dec 2022 05:11:32 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 21 Dec 2022 05:11:33 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:542880f4d15404af17d342ecbb76bb92724fc7cb8a91a5e18f26bd8f8811a38a`  
		Last Modified: Wed, 21 Dec 2022 01:22:46 GMT  
		Size: 58.9 MB (58897040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8c91d3a2eff19ff3291563333f250447b70f82929a98b439e9253b9d8909332`  
		Last Modified: Wed, 21 Dec 2022 05:12:53 GMT  
		Size: 40.6 MB (40618582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1fc5014e613c79f385d0565b105dfdc45badae00ab5a50f9b06955eb34e874d`  
		Last Modified: Wed, 21 Dec 2022 05:12:39 GMT  
		Size: 394.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc90d97148640f4f164e3dc4b1f043c6ba7d8b5cddd21ede8a947339a13e3c3f`  
		Last Modified: Wed, 21 Dec 2022 05:12:39 GMT  
		Size: 1.9 KB (1879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdfe2d4e5fb66793ea99cc5959183331088d985dc203754a30a8bf6bbffb186a`  
		Last Modified: Wed, 21 Dec 2022 05:12:39 GMT  
		Size: 1.5 KB (1482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0da8c96b4d9b013ebbf00af4b8693e634764cf159be7af73d3152403cabe71e5`  
		Last Modified: Wed, 21 Dec 2022 05:12:40 GMT  
		Size: 1.4 MB (1383844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:061e859636ca9e27f80e25b38a893f2e38d08dd68c7a53bc8fb9f428dfb0f328`  
		Last Modified: Wed, 21 Dec 2022 05:12:39 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:standalone` - linux; s390x

```console
$ docker pull adminer@sha256:4ad639f239b5117cf7381d37948390122d8f514592dade423c1fbdc4870c04b4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.4 MB (93401988 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac7114a00edb645cd010878538757f757f872e25c530cb9159f5bc03cc191726`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 21 Dec 2022 01:42:51 GMT
ADD file:22c4f2d41083ce4433bec4a71e7e6ddc5bec8e44e9cf2c9f93d0874b5b4de7c3 in / 
# Wed, 21 Dec 2022 01:42:54 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 02:06:42 GMT
STOPSIGNAL SIGINT
# Wed, 21 Dec 2022 02:07:51 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 02:08:00 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 21 Dec 2022 02:08:02 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 21 Dec 2022 02:08:03 GMT
WORKDIR /var/www/html
# Wed, 21 Dec 2022 02:08:04 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 21 Dec 2022 02:08:04 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 21 Dec 2022 02:08:05 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 21 Dec 2022 02:08:06 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 21 Dec 2022 02:08:33 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 21 Dec 2022 02:08:33 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 21 Dec 2022 02:08:34 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 21 Dec 2022 02:08:35 GMT
USER adminer
# Wed, 21 Dec 2022 02:08:35 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 21 Dec 2022 02:08:36 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:7f45294776f4c97d23f8dbfca98d4b57701b478eedfcb154a7e7dc6d6954ba44`  
		Last Modified: Wed, 21 Dec 2022 01:48:50 GMT  
		Size: 53.3 MB (53258472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8610ee81c430b6503a5ee2d7cc451175bdfc868fc17ef5a675b43679da433867`  
		Last Modified: Wed, 21 Dec 2022 02:10:03 GMT  
		Size: 38.8 MB (38755148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:211b726eee70a0c5ff85337d1e98c7987025435a41ca5421f47d96fc164b5b27`  
		Last Modified: Wed, 21 Dec 2022 02:09:56 GMT  
		Size: 395.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c6a1fa2154f900c32f87164afe347f0dddbb7a641dc81b7fc436b1d15a5349d`  
		Last Modified: Wed, 21 Dec 2022 02:09:56 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e030c793dfbf87ef1f5dbbecd22117bcf1695eb293e41bca267fb29d0e98d59d`  
		Last Modified: Wed, 21 Dec 2022 02:09:56 GMT  
		Size: 1.5 KB (1478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:965c9f68e6765f8a5967198527ce6ff7bf0646cab60aa30ecef97747554c0869`  
		Last Modified: Wed, 21 Dec 2022 02:09:56 GMT  
		Size: 1.4 MB (1384122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d34b801ca3351132a2f2914bc4ef3ca0f91a2c87c2b42fce3662fd5f20593aea`  
		Last Modified: Wed, 21 Dec 2022 02:09:56 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
