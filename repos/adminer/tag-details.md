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
$ docker pull adminer@sha256:521aae780cec6678443058ecb03e3b20fd815e1c1220dc8370c3a3381acc736c
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
$ docker pull adminer@sha256:203c8ee52640268c28f5ce5f57b192d967da40a91d6443b57ae1da4064e2ed8b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.9 MB (95931867 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e4345c1c3dc89b4c31146abe340fa39e143d922d1e3401233d7ac32db2d985d`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Mon, 12 Jun 2023 23:20:54 GMT
ADD file:e530b0563ea53d97b2f28e62149a665900196f86611df99a88c7a8ab2097b95d in / 
# Mon, 12 Jun 2023 23:20:54 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 03:24:37 GMT
STOPSIGNAL SIGINT
# Tue, 13 Jun 2023 03:25:04 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 03:25:05 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 13 Jun 2023 03:25:06 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 13 Jun 2023 03:25:06 GMT
WORKDIR /var/www/html
# Tue, 13 Jun 2023 03:25:06 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 13 Jun 2023 03:25:06 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 13 Jun 2023 03:25:06 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 13 Jun 2023 03:25:06 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 13 Jun 2023 03:25:19 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Jun 2023 03:25:19 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 13 Jun 2023 03:25:19 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 13 Jun 2023 03:25:19 GMT
USER adminer
# Tue, 13 Jun 2023 03:25:19 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Tue, 13 Jun 2023 03:25:19 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:93c2d578e4211e82e47e7ada9ed05d1869a2362c6f7509f2ee8d91ccebfb7fbd`  
		Last Modified: Mon, 12 Jun 2023 23:26:08 GMT  
		Size: 55.1 MB (55055162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e099cf7ea37ba8ff2169a70f6743bf40675a661f0dc9b6a8abaa4e43050979c`  
		Last Modified: Tue, 13 Jun 2023 03:25:56 GMT  
		Size: 39.5 MB (39487054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d12c699384cbfa0b30a07efef5ad3b7f104e0e1f33e6a094e489150e4ef3838`  
		Last Modified: Tue, 13 Jun 2023 03:25:48 GMT  
		Size: 391.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05c66113a52b479d99efec54808f4045c5fe1400714639a6c750317ad501bc9c`  
		Last Modified: Tue, 13 Jun 2023 03:25:48 GMT  
		Size: 1.9 KB (1874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:677df7ad2be6c1e9f14d49043358dc765759c7f2cd0184ca55a55dc81dcb2263`  
		Last Modified: Tue, 13 Jun 2023 03:25:48 GMT  
		Size: 1.5 KB (1478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:598f6ab1ce2900168e83fbb661f1edc77e27dd8261b23a1f22af28e991facd6e`  
		Last Modified: Tue, 13 Jun 2023 03:25:49 GMT  
		Size: 1.4 MB (1385416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41ed709cb4bc1b53001ba47d24d74fb415c6142dd35194346fdac370144df45a`  
		Last Modified: Tue, 13 Jun 2023 03:25:48 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4` - linux; arm variant v5

```console
$ docker pull adminer@sha256:15bb2436532d59fdbf58c3cbc74f61d47be5ad45e30d65bc01adcfc449dd0951
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.2 MB (91183934 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:267345bcacc239fd7427ea82c255b704e164984dbff20209a9e8439820a662d3`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Tue, 23 May 2023 00:48:32 GMT
ADD file:9572a8fcb9c86e8a9dbfe623c732cc4ba1c4f5670490191a7e639a272d5b6e97 in / 
# Tue, 23 May 2023 00:48:33 GMT
CMD ["bash"]
# Tue, 23 May 2023 01:09:52 GMT
STOPSIGNAL SIGINT
# Tue, 23 May 2023 01:10:29 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 01:10:30 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 23 May 2023 01:10:31 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 23 May 2023 01:10:31 GMT
WORKDIR /var/www/html
# Tue, 23 May 2023 01:10:31 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 23 May 2023 01:10:31 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 23 May 2023 01:10:31 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 23 May 2023 01:10:31 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 23 May 2023 01:10:46 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 23 May 2023 01:10:46 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 23 May 2023 01:10:46 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 23 May 2023 01:10:46 GMT
USER adminer
# Tue, 23 May 2023 01:10:46 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Tue, 23 May 2023 01:10:46 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:b053976742ca5b01bcefb7df8fc77a58d0becb4ce508792491574463930569c4`  
		Last Modified: Tue, 23 May 2023 00:50:55 GMT  
		Size: 52.5 MB (52546536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6448799a9363993edd93e5fb6040955191b829140af65c88550e510326878903`  
		Last Modified: Tue, 23 May 2023 01:11:21 GMT  
		Size: 37.2 MB (37247839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b03dc69db3dc4061f823e5e9025874ab539e706b64af3b103bf2a3e839890b8`  
		Last Modified: Tue, 23 May 2023 01:11:13 GMT  
		Size: 388.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ed315aa6041fcfd6bafc18c55ef5be23f10e057e9f941675330807b39d1e54a`  
		Last Modified: Tue, 23 May 2023 01:11:13 GMT  
		Size: 1.9 KB (1872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2d328016feebec5e083e36300e6444d56a5aedfba59d4be438549c64ebcb44f`  
		Last Modified: Tue, 23 May 2023 01:11:13 GMT  
		Size: 1.5 KB (1480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c98954d02c72cf9c2513f055817ac1435ded02424a3418c8d3b9164746bdf3c`  
		Last Modified: Tue, 23 May 2023 01:11:13 GMT  
		Size: 1.4 MB (1385327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aac95e0f74f942d3cfb111cf9949811151a49733af863c919807b2dcbb3a85a1`  
		Last Modified: Tue, 23 May 2023 01:11:13 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4` - linux; arm variant v7

```console
$ docker pull adminer@sha256:98b76b0878cf9cc2684e5bbbdade79a5f2f6f269e230203870a1f1a752f7e7f1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.8 MB (87790748 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b51c4364b99328a719594799d5c3d616aeb43a95308f9cd320cb70d27dda4c17`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Mon, 12 Jun 2023 23:58:34 GMT
ADD file:6edc8f94d2ebc83d6081e1c4567963d0060a842c767eaff959a6e5c6d09247b5 in / 
# Mon, 12 Jun 2023 23:58:34 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 04:50:43 GMT
STOPSIGNAL SIGINT
# Tue, 13 Jun 2023 04:51:12 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 04:51:12 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 13 Jun 2023 04:51:13 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 13 Jun 2023 04:51:13 GMT
WORKDIR /var/www/html
# Tue, 13 Jun 2023 04:51:13 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 13 Jun 2023 04:51:13 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 13 Jun 2023 04:51:13 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 13 Jun 2023 04:51:13 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 13 Jun 2023 04:51:41 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Jun 2023 04:51:41 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 13 Jun 2023 04:51:41 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 13 Jun 2023 04:51:41 GMT
USER adminer
# Tue, 13 Jun 2023 04:51:42 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Tue, 13 Jun 2023 04:51:42 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:23807bbf2a5fd14b7975a9e82f4a5530bbba520f31b382cc4b4ce2e77e075ace`  
		Last Modified: Tue, 13 Jun 2023 00:04:02 GMT  
		Size: 50.2 MB (50218141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed9435d7956e105f98b0ce0d774c24da59c523bdcf4ec8fff644876978300c69`  
		Last Modified: Tue, 13 Jun 2023 04:52:24 GMT  
		Size: 36.2 MB (36183011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbf6d7965eb59f39902f271310a767cdf68bdc38bf15c4ee7bc3cfc5c2d025f8`  
		Last Modified: Tue, 13 Jun 2023 04:52:16 GMT  
		Size: 392.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da256b5543040f6999ae9a8cc020bfd0542286ecf71c77feb6cd08a4ecd9be37`  
		Last Modified: Tue, 13 Jun 2023 04:52:16 GMT  
		Size: 1.9 KB (1863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fac8d202305e7ac73502fb63bb1618ac53766c99e8cd03bcb0412c313a25dd83`  
		Last Modified: Tue, 13 Jun 2023 04:52:16 GMT  
		Size: 1.5 KB (1479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b96b3d518c63ab16389a582e075ae88f7225f3c35483203c7c52dcfa52f2daa5`  
		Last Modified: Tue, 13 Jun 2023 04:52:16 GMT  
		Size: 1.4 MB (1385372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eb5818f5b2f148baf53286364c0c6cd2df86e21ed76bfcbc6ff0688a5d2726c`  
		Last Modified: Tue, 13 Jun 2023 04:52:16 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4` - linux; arm64 variant v8

```console
$ docker pull adminer@sha256:92cdfd552b3557e293045fc3d5f01d58871958912197649f3c818e312856bf85
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.3 MB (94336689 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b7e1c530248708005dc78825e6702d078b51bbd4eae6c82b2df135ce82d2961`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:22 GMT
ADD file:caddd2f40296ec5c1bf7487617ca8694cfff9a1d9b7484159e203b6514cb5f5f in / 
# Mon, 12 Jun 2023 23:40:23 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 04:45:49 GMT
STOPSIGNAL SIGINT
# Tue, 13 Jun 2023 04:46:10 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 04:46:11 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 13 Jun 2023 04:46:12 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 13 Jun 2023 04:46:12 GMT
WORKDIR /var/www/html
# Tue, 13 Jun 2023 04:46:12 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 13 Jun 2023 04:46:12 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 13 Jun 2023 04:46:12 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 13 Jun 2023 04:46:12 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 13 Jun 2023 04:46:22 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Jun 2023 04:46:22 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 13 Jun 2023 04:46:22 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 13 Jun 2023 04:46:22 GMT
USER adminer
# Tue, 13 Jun 2023 04:46:22 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Tue, 13 Jun 2023 04:46:23 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:663ccfaf62a5d7b997bca03d1dc6d5dfff01b9e0de08d86dbea8957ea92d7d16`  
		Last Modified: Mon, 12 Jun 2023 23:44:25 GMT  
		Size: 53.7 MB (53704136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80aa39d9a9c198e71855c642bc21b287cd96a68f1ca6f6095933aebd07835b55`  
		Last Modified: Tue, 13 Jun 2023 04:46:57 GMT  
		Size: 39.2 MB (39243014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35aba8c7c961932b274149a03d0e4ded7ce7529e514d523d33c6c6972b149b3d`  
		Last Modified: Tue, 13 Jun 2023 04:46:50 GMT  
		Size: 393.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe596da7a5da4c53bb7e8a57c4bca7d95147969f3fcfa27a9ac63992faacad68`  
		Last Modified: Tue, 13 Jun 2023 04:46:51 GMT  
		Size: 1.9 KB (1875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9f19157c079ccd39ddc0b6c916dec64e367d7b29ff37f7d51348654868ffeea`  
		Last Modified: Tue, 13 Jun 2023 04:46:51 GMT  
		Size: 1.5 KB (1482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e9f6bc36eded234b1a9ca40497b6b08e4a5ebd85b8077cfd4951499ef134c78`  
		Last Modified: Tue, 13 Jun 2023 04:46:51 GMT  
		Size: 1.4 MB (1385300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4689e75de5a00a90b25e2ae66464fad25ea65b849b83d549503bdfb11f72be63`  
		Last Modified: Tue, 13 Jun 2023 04:46:51 GMT  
		Size: 489.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4` - linux; 386

```console
$ docker pull adminer@sha256:e0bb773bce27da86e8bba771ce6fb58fef553b675ea0e0e2c7eaa0d2bd7dd9f9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.0 MB (96988803 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77720ee3233be6352493a8d99e983f977b3e182750f1526bba6d67134b1bf7ee`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Mon, 12 Jun 2023 23:39:39 GMT
ADD file:4b1f447e0b75fbe493bd68bb77b74f4ba1c61ac8e14226e3c511b3a1c3d5721a in / 
# Mon, 12 Jun 2023 23:39:40 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 00:59:39 GMT
STOPSIGNAL SIGINT
# Tue, 13 Jun 2023 01:00:06 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 01:00:07 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 13 Jun 2023 01:00:07 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 13 Jun 2023 01:00:08 GMT
WORKDIR /var/www/html
# Tue, 13 Jun 2023 01:00:08 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 13 Jun 2023 01:00:08 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 13 Jun 2023 01:00:08 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 13 Jun 2023 01:00:08 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 13 Jun 2023 01:00:20 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Jun 2023 01:00:20 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 13 Jun 2023 01:00:20 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 13 Jun 2023 01:00:21 GMT
USER adminer
# Tue, 13 Jun 2023 01:00:21 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Tue, 13 Jun 2023 01:00:21 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:0997ae72d27731326552ad4699d630b4932f3d31abc07a62105a0eb16b54173a`  
		Last Modified: Mon, 12 Jun 2023 23:46:43 GMT  
		Size: 56.0 MB (56040665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dac97babbe48fc6ee5134482bf3dd02a0763c71618911c97beab64bec3147a8`  
		Last Modified: Tue, 13 Jun 2023 01:01:02 GMT  
		Size: 39.6 MB (39558608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df44f63ded7015da79f717c9dbf6dfd057bcafc06012bc1e415f53113e6fc1e5`  
		Last Modified: Tue, 13 Jun 2023 01:00:51 GMT  
		Size: 389.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ae3ce4c7547485956e0bd1180cc66032006af3b33c6ae582d77834096391752`  
		Last Modified: Tue, 13 Jun 2023 01:00:51 GMT  
		Size: 1.9 KB (1864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83417b3fe0dbbaed7076986fd209d6704b096ecd961a111cfb42cba80a11dc93`  
		Last Modified: Tue, 13 Jun 2023 01:00:51 GMT  
		Size: 1.5 KB (1480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbdb97551a1780228aac70017b847d497ec088d6ad3e46d5c8b9b48083efe5a0`  
		Last Modified: Tue, 13 Jun 2023 01:00:52 GMT  
		Size: 1.4 MB (1385307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbef3e3e2b3156ba5eca052ebf766f2f4474f980905836f0c0ea9eec319f7a6e`  
		Last Modified: Tue, 13 Jun 2023 01:00:51 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4` - linux; mips64le

```console
$ docker pull adminer@sha256:2591b1f0dffbc4f123a4a3bd12c1cb46669c54383e8e23e13c83edaecc2541d1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.6 MB (92614104 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9a417a537dc4187139ad39c01263d6bd8b79a728bf005ad51d3bb4d42ec1d5f`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Tue, 13 Jun 2023 00:09:46 GMT
ADD file:7ba4829e0a582c8a2e5a1d362ca30cfba3fa2911594faf9598927255100965b0 in / 
# Tue, 13 Jun 2023 00:09:51 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 01:46:11 GMT
STOPSIGNAL SIGINT
# Tue, 13 Jun 2023 01:48:01 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 01:48:08 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 13 Jun 2023 01:48:14 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 13 Jun 2023 01:48:18 GMT
WORKDIR /var/www/html
# Tue, 13 Jun 2023 01:48:21 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 13 Jun 2023 01:48:24 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 13 Jun 2023 01:48:28 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 13 Jun 2023 01:48:31 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 13 Jun 2023 01:49:21 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Jun 2023 01:49:24 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 13 Jun 2023 01:49:27 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 13 Jun 2023 01:49:31 GMT
USER adminer
# Tue, 13 Jun 2023 01:49:34 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Tue, 13 Jun 2023 01:49:37 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:ec034d426521af0a9addba08124f06b364f3364fd20ec9aec4e3364104a793d1`  
		Last Modified: Tue, 13 Jun 2023 00:23:13 GMT  
		Size: 53.3 MB (53270410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:901a0f1a33bd58f6d5e7b1de7a90c5fbe79c192cbbabfd8c7a98214496b73c1b`  
		Last Modified: Tue, 13 Jun 2023 01:52:11 GMT  
		Size: 38.0 MB (37953313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c616df06cfce4fa5e3f76b4147041f55275dd885295b9a2e1b9884f710f5a63`  
		Last Modified: Tue, 13 Jun 2023 01:51:45 GMT  
		Size: 395.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84487562d4b36a6a1112b198b725b1a727e91a77be9899c0d74b1a4a9c022dba`  
		Last Modified: Tue, 13 Jun 2023 01:51:45 GMT  
		Size: 1.7 KB (1723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5dde6303cb52a3de95ebac876b6f8590487f4ffa08f8c0e80844f4d89b75072`  
		Last Modified: Tue, 13 Jun 2023 01:51:45 GMT  
		Size: 1.5 KB (1480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:499702681379ddde7be8cc76c78d9b9c764ceea9af16c336da3a99169971feb1`  
		Last Modified: Tue, 13 Jun 2023 01:51:46 GMT  
		Size: 1.4 MB (1386295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63d75b2d63e14c568323dc0897c171f4d71efe33d94bb1423a59c555514d35ae`  
		Last Modified: Tue, 13 Jun 2023 01:51:45 GMT  
		Size: 488.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4` - linux; ppc64le

```console
$ docker pull adminer@sha256:e0a0e907c5c635e5e363e08b1dffd85143970ad1e4dee8cd2acdbd2c47f59f30
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.3 MB (101253778 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0759ab5b0827c3e5903a54d9e690f3911052bcece85af789658d87469a6c4e41`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Tue, 23 May 2023 01:17:14 GMT
ADD file:ed39869ee4bb8e1901b71feb9cadfe754e42304e134f2542e516e162ca710ec8 in / 
# Tue, 23 May 2023 01:17:17 GMT
CMD ["bash"]
# Tue, 23 May 2023 01:40:42 GMT
STOPSIGNAL SIGINT
# Tue, 23 May 2023 01:41:54 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 01:41:58 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 23 May 2023 01:42:00 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 23 May 2023 01:42:01 GMT
WORKDIR /var/www/html
# Tue, 23 May 2023 01:42:01 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 23 May 2023 01:42:02 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 23 May 2023 01:42:02 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 23 May 2023 01:42:02 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 23 May 2023 01:42:36 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 23 May 2023 01:42:37 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 23 May 2023 01:42:37 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 23 May 2023 01:42:38 GMT
USER adminer
# Tue, 23 May 2023 01:42:39 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Tue, 23 May 2023 01:42:40 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:f530a46e89ee571046fe19b22f563df6c84a31f6593a1e6ed49dbd16e34145de`  
		Last Modified: Tue, 23 May 2023 01:21:34 GMT  
		Size: 58.9 MB (58923948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b328a5c7e2019a9edf5b5d571d37da0261097706c34bafabd5196936aac3fc1b`  
		Last Modified: Tue, 23 May 2023 01:44:03 GMT  
		Size: 40.9 MB (40939928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b29d269a712c093f32a0be4629a0f17bc22fd6dad4be88d5f0af5ce757d809f`  
		Last Modified: Tue, 23 May 2023 01:43:51 GMT  
		Size: 393.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:904564df90e41e35afa3221ab3277e3aa554b7c686393785c1b07372bc0c4d4d`  
		Last Modified: Tue, 23 May 2023 01:43:51 GMT  
		Size: 1.9 KB (1880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55a789415d78b4a3befd6b003659799bcf3d20cb06639a961c96a980640e8991`  
		Last Modified: Tue, 23 May 2023 01:43:51 GMT  
		Size: 1.5 KB (1479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78c991997ea0a176dc01a5a08f6ac61143299aef87572cd7e8578e479aae772b`  
		Last Modified: Tue, 23 May 2023 01:43:52 GMT  
		Size: 1.4 MB (1385657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd039d869a125163f2302899c7b0fcf2db140dad2eecedc648b3ca229cb86460`  
		Last Modified: Tue, 23 May 2023 01:43:51 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4` - linux; s390x

```console
$ docker pull adminer@sha256:b48c2c7360476d0f6ce0723abeef59ed2cc19493ffedd144d64ee2b5d0a21683
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.7 MB (93690153 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:008c852f84add504c1031fabd62a8ede6758604b42d91789507acf3c08df5507`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Tue, 23 May 2023 00:42:35 GMT
ADD file:a054112be60c3f2d7811b27cde82bccfd1c2747f29b7611ee68b21cd9f3d3d54 in / 
# Tue, 23 May 2023 00:42:41 GMT
CMD ["bash"]
# Tue, 23 May 2023 02:26:55 GMT
STOPSIGNAL SIGINT
# Tue, 23 May 2023 02:27:12 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 02:27:15 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 23 May 2023 02:27:15 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 23 May 2023 02:27:15 GMT
WORKDIR /var/www/html
# Tue, 23 May 2023 02:27:15 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 23 May 2023 02:27:15 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 23 May 2023 02:27:16 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 23 May 2023 02:27:16 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 23 May 2023 02:27:23 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 23 May 2023 02:27:23 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 23 May 2023 02:27:23 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 23 May 2023 02:27:24 GMT
USER adminer
# Tue, 23 May 2023 02:27:24 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Tue, 23 May 2023 02:27:24 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:44d1d02f91725dd9ae742f7c70add814dc3da3fde438adb01e65e1f8b0eba613`  
		Last Modified: Tue, 23 May 2023 00:45:33 GMT  
		Size: 53.3 MB (53282114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a714865cdf8c711665c7b864ae5f1e6c7100e6079a9d6bb3d8925f6a0cceaff2`  
		Last Modified: Tue, 23 May 2023 02:28:00 GMT  
		Size: 39.0 MB (39018332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a6faa7559a991fd1e86474adae5128141983567ad4587e50e92ce5d32755bbb`  
		Last Modified: Tue, 23 May 2023 02:27:53 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f55cc440fda23758bbfb18b1a3881ac61d06ad9e0a4b35da688b713c1b8611be`  
		Last Modified: Tue, 23 May 2023 02:27:53 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d16d617d4904a95242ab9db1204e6fa0d844358dc62528fed7ad368f57b1251d`  
		Last Modified: Tue, 23 May 2023 02:27:53 GMT  
		Size: 1.5 KB (1478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c753b23f0be5c140b7bed93c7220f68e38f138d53d3e7e9aade64a9d4b45038e`  
		Last Modified: Tue, 23 May 2023 02:27:53 GMT  
		Size: 1.4 MB (1385466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a436f3a56433ffbdc8b5e6a7bda069a68625447867738966931d19c9db78365c`  
		Last Modified: Tue, 23 May 2023 02:27:53 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `adminer:4-fastcgi`

```console
$ docker pull adminer@sha256:f67d780396297178e7b0d659328093579772caa59834ea077b2d00edc2b2d3c3
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
$ docker pull adminer@sha256:19e342979ee9fe7dbce42adf4070530e4fab8743bc177b4b401efc984ab1e40b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.9 MB (95934602 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:452a956cc7253ee0c04d3736127b355e67a5cd14dda7c0aaf0c2d18ab50277f1`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Mon, 12 Jun 2023 23:20:54 GMT
ADD file:e530b0563ea53d97b2f28e62149a665900196f86611df99a88c7a8ab2097b95d in / 
# Mon, 12 Jun 2023 23:20:54 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 03:24:37 GMT
STOPSIGNAL SIGINT
# Tue, 13 Jun 2023 03:25:04 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 03:25:05 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 13 Jun 2023 03:25:26 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Tue, 13 Jun 2023 03:25:26 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 13 Jun 2023 03:25:26 GMT
WORKDIR /var/www/html
# Tue, 13 Jun 2023 03:25:26 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 13 Jun 2023 03:25:26 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 13 Jun 2023 03:25:26 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 13 Jun 2023 03:25:27 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 13 Jun 2023 03:25:37 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Jun 2023 03:25:37 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 13 Jun 2023 03:25:37 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 13 Jun 2023 03:25:37 GMT
USER adminer
# Tue, 13 Jun 2023 03:25:38 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:93c2d578e4211e82e47e7ada9ed05d1869a2362c6f7509f2ee8d91ccebfb7fbd`  
		Last Modified: Mon, 12 Jun 2023 23:26:08 GMT  
		Size: 55.1 MB (55055162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e099cf7ea37ba8ff2169a70f6743bf40675a661f0dc9b6a8abaa4e43050979c`  
		Last Modified: Tue, 13 Jun 2023 03:25:56 GMT  
		Size: 39.5 MB (39487054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d12c699384cbfa0b30a07efef5ad3b7f104e0e1f33e6a094e489150e4ef3838`  
		Last Modified: Tue, 13 Jun 2023 03:25:48 GMT  
		Size: 391.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a83e8c3036470b387287b92b025e756b2d38926bd08a60b788905721b2710970`  
		Last Modified: Tue, 13 Jun 2023 03:26:11 GMT  
		Size: 2.7 KB (2706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4474445ef61d8bccb5f84a0c1af50393a4283332687b853db43b67b7c8ea97ac`  
		Last Modified: Tue, 13 Jun 2023 03:26:11 GMT  
		Size: 1.9 KB (1869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9d7d23c4974a9d08d6b18826eb53254571cb1eae70efa61ee681248a11cdcdc`  
		Last Modified: Tue, 13 Jun 2023 03:26:11 GMT  
		Size: 1.5 KB (1475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:420c1637804f967bec0a6f2d1c8e796d18bad5b8a06dadd562b9e930aa597924`  
		Last Modified: Tue, 13 Jun 2023 03:26:11 GMT  
		Size: 1.4 MB (1385457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1963affabab6ca86abab89a12ea096a70efa4ae2aae5c58c80a429a8c88afab2`  
		Last Modified: Tue, 13 Jun 2023 03:26:11 GMT  
		Size: 488.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-fastcgi` - linux; arm variant v5

```console
$ docker pull adminer@sha256:874aa6f218690a93c384b0f19fc246af20d395854f936f59bc3547bacd22ac8d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.2 MB (91186662 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad52da629ff3a29fd1d27c9c82784df59d0303ac68e619208119f622c79f3f32`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Tue, 23 May 2023 00:48:32 GMT
ADD file:9572a8fcb9c86e8a9dbfe623c732cc4ba1c4f5670490191a7e639a272d5b6e97 in / 
# Tue, 23 May 2023 00:48:33 GMT
CMD ["bash"]
# Tue, 23 May 2023 01:09:52 GMT
STOPSIGNAL SIGINT
# Tue, 23 May 2023 01:10:29 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 01:10:30 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 23 May 2023 01:10:49 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Tue, 23 May 2023 01:10:50 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 23 May 2023 01:10:50 GMT
WORKDIR /var/www/html
# Tue, 23 May 2023 01:10:50 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 23 May 2023 01:10:50 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 23 May 2023 01:10:50 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 23 May 2023 01:10:50 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 23 May 2023 01:11:03 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 23 May 2023 01:11:03 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 23 May 2023 01:11:03 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 23 May 2023 01:11:03 GMT
USER adminer
# Tue, 23 May 2023 01:11:04 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:b053976742ca5b01bcefb7df8fc77a58d0becb4ce508792491574463930569c4`  
		Last Modified: Tue, 23 May 2023 00:50:55 GMT  
		Size: 52.5 MB (52546536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6448799a9363993edd93e5fb6040955191b829140af65c88550e510326878903`  
		Last Modified: Tue, 23 May 2023 01:11:21 GMT  
		Size: 37.2 MB (37247839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b03dc69db3dc4061f823e5e9025874ab539e706b64af3b103bf2a3e839890b8`  
		Last Modified: Tue, 23 May 2023 01:11:13 GMT  
		Size: 388.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b485dfbb13977609126b9a2977c8377b44b256b17a3eb1ca752d5dcd2f1c355`  
		Last Modified: Tue, 23 May 2023 01:11:38 GMT  
		Size: 2.7 KB (2710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:468ca8e69b40ea1983b6fcb3612d2309983339ff59fb02fc827a331cfe0ec7e8`  
		Last Modified: Tue, 23 May 2023 01:11:38 GMT  
		Size: 1.9 KB (1872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e58c31f850be84c6af0b0a6110b43a6541e2866463803132254f3a9fe3d934a7`  
		Last Modified: Tue, 23 May 2023 01:11:38 GMT  
		Size: 1.5 KB (1476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3e8c00c90d7ae0b153ebfdc785a5a8a92eb1b7c2f784dd565dc5a72d95e9405`  
		Last Modified: Tue, 23 May 2023 01:11:38 GMT  
		Size: 1.4 MB (1385350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27dade8d0c809034087f2b30ac15a8b8c57d45108d908e8d1cb020afb23eae9a`  
		Last Modified: Tue, 23 May 2023 01:11:38 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-fastcgi` - linux; arm variant v7

```console
$ docker pull adminer@sha256:11ec19aff2d26fc95a54fd3df142b2150c3a377c2d75480bf89b34bb1959dcf0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.8 MB (87793463 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c9707286206384175f44f5f53306cea1139c30c01a275936f88f3677f591726`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Mon, 12 Jun 2023 23:58:34 GMT
ADD file:6edc8f94d2ebc83d6081e1c4567963d0060a842c767eaff959a6e5c6d09247b5 in / 
# Mon, 12 Jun 2023 23:58:34 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 04:50:43 GMT
STOPSIGNAL SIGINT
# Tue, 13 Jun 2023 04:51:12 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 04:51:12 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 13 Jun 2023 04:51:52 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Tue, 13 Jun 2023 04:51:53 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 13 Jun 2023 04:51:53 GMT
WORKDIR /var/www/html
# Tue, 13 Jun 2023 04:51:53 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 13 Jun 2023 04:51:53 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 13 Jun 2023 04:51:53 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 13 Jun 2023 04:51:54 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 13 Jun 2023 04:52:04 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Jun 2023 04:52:04 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 13 Jun 2023 04:52:05 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 13 Jun 2023 04:52:05 GMT
USER adminer
# Tue, 13 Jun 2023 04:52:05 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:23807bbf2a5fd14b7975a9e82f4a5530bbba520f31b382cc4b4ce2e77e075ace`  
		Last Modified: Tue, 13 Jun 2023 00:04:02 GMT  
		Size: 50.2 MB (50218141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed9435d7956e105f98b0ce0d774c24da59c523bdcf4ec8fff644876978300c69`  
		Last Modified: Tue, 13 Jun 2023 04:52:24 GMT  
		Size: 36.2 MB (36183011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbf6d7965eb59f39902f271310a767cdf68bdc38bf15c4ee7bc3cfc5c2d025f8`  
		Last Modified: Tue, 13 Jun 2023 04:52:16 GMT  
		Size: 392.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:916d17fb0f8882d23121f554813421100e94760e2e0cdaf751935eaa1a19ab46`  
		Last Modified: Tue, 13 Jun 2023 04:52:39 GMT  
		Size: 2.7 KB (2713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb697d34af45737a34d3f2956db7be64dda1aea6ed409568e658cb341633ede7`  
		Last Modified: Tue, 13 Jun 2023 04:52:39 GMT  
		Size: 1.9 KB (1863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8ada7f7a7eb464a51e2dae5756d43b13a9d97ee91354ed06525718c56c80881`  
		Last Modified: Tue, 13 Jun 2023 04:52:39 GMT  
		Size: 1.5 KB (1476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdce229253f3ee410f2b1f7535a88835f7283d187bb2e8038132fc61d5705691`  
		Last Modified: Tue, 13 Jun 2023 04:52:40 GMT  
		Size: 1.4 MB (1385378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eee6f724498f44554404d3f27bfb20c948b0c3644918c575d594ad887ecb2a31`  
		Last Modified: Tue, 13 Jun 2023 04:52:39 GMT  
		Size: 489.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-fastcgi` - linux; arm64 variant v8

```console
$ docker pull adminer@sha256:3dd032bfdb7eb723810a29735b8e01eb4466194e6c2843355eb9a4d70243f534
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.3 MB (94339383 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d48c97b1d9e6d66f743a4b29f2deada7524b544850c7671e594390b07d8c02f4`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:22 GMT
ADD file:caddd2f40296ec5c1bf7487617ca8694cfff9a1d9b7484159e203b6514cb5f5f in / 
# Mon, 12 Jun 2023 23:40:23 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 04:45:49 GMT
STOPSIGNAL SIGINT
# Tue, 13 Jun 2023 04:46:10 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 04:46:11 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 13 Jun 2023 04:46:30 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Tue, 13 Jun 2023 04:46:30 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 13 Jun 2023 04:46:30 GMT
WORKDIR /var/www/html
# Tue, 13 Jun 2023 04:46:31 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 13 Jun 2023 04:46:31 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 13 Jun 2023 04:46:31 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 13 Jun 2023 04:46:31 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 13 Jun 2023 04:46:40 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Jun 2023 04:46:40 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 13 Jun 2023 04:46:41 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 13 Jun 2023 04:46:41 GMT
USER adminer
# Tue, 13 Jun 2023 04:46:41 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:663ccfaf62a5d7b997bca03d1dc6d5dfff01b9e0de08d86dbea8957ea92d7d16`  
		Last Modified: Mon, 12 Jun 2023 23:44:25 GMT  
		Size: 53.7 MB (53704136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80aa39d9a9c198e71855c642bc21b287cd96a68f1ca6f6095933aebd07835b55`  
		Last Modified: Tue, 13 Jun 2023 04:46:57 GMT  
		Size: 39.2 MB (39243014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35aba8c7c961932b274149a03d0e4ded7ce7529e514d523d33c6c6972b149b3d`  
		Last Modified: Tue, 13 Jun 2023 04:46:50 GMT  
		Size: 393.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2162693a46ec477e8b49e0b80d0001f2eda79016865c9dc2158bb2ef09e7f9b`  
		Last Modified: Tue, 13 Jun 2023 04:47:13 GMT  
		Size: 2.7 KB (2714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:050d9afd2370b260f1761c086dbd5b74588dd70e17c533745afae53f5c1418f8`  
		Last Modified: Tue, 13 Jun 2023 04:47:13 GMT  
		Size: 1.9 KB (1876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:194f7cc3086811f97e24a54110a1ab966bcd8e3ff0c53f3bc2dd92d1e1186375`  
		Last Modified: Tue, 13 Jun 2023 04:47:13 GMT  
		Size: 1.5 KB (1475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f69e51ee2ca7c113fff7852d477f2060974ccb554779d3252647aa566bb161a4`  
		Last Modified: Tue, 13 Jun 2023 04:47:14 GMT  
		Size: 1.4 MB (1385287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44aea086a6384d7d2bd997d4c3c0d0b5344e0d91e9ca0128c0daaebb6f65bd9c`  
		Last Modified: Tue, 13 Jun 2023 04:47:13 GMT  
		Size: 488.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-fastcgi` - linux; 386

```console
$ docker pull adminer@sha256:b4aec10e1691950dfa2dc0805c974f93383bb86817b1dfeb8e31a7302fca7740
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.0 MB (96991518 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f2428d60bf69f5e123fd00c3307326cf15efc62cdfbe175764ff4f431296a3ea`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Mon, 12 Jun 2023 23:39:39 GMT
ADD file:4b1f447e0b75fbe493bd68bb77b74f4ba1c61ac8e14226e3c511b3a1c3d5721a in / 
# Mon, 12 Jun 2023 23:39:40 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 00:59:39 GMT
STOPSIGNAL SIGINT
# Tue, 13 Jun 2023 01:00:06 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 01:00:07 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 13 Jun 2023 01:00:28 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Tue, 13 Jun 2023 01:00:28 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 13 Jun 2023 01:00:28 GMT
WORKDIR /var/www/html
# Tue, 13 Jun 2023 01:00:29 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 13 Jun 2023 01:00:29 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 13 Jun 2023 01:00:29 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 13 Jun 2023 01:00:29 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 13 Jun 2023 01:00:41 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Jun 2023 01:00:41 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 13 Jun 2023 01:00:41 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 13 Jun 2023 01:00:41 GMT
USER adminer
# Tue, 13 Jun 2023 01:00:41 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:0997ae72d27731326552ad4699d630b4932f3d31abc07a62105a0eb16b54173a`  
		Last Modified: Mon, 12 Jun 2023 23:46:43 GMT  
		Size: 56.0 MB (56040665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dac97babbe48fc6ee5134482bf3dd02a0763c71618911c97beab64bec3147a8`  
		Last Modified: Tue, 13 Jun 2023 01:01:02 GMT  
		Size: 39.6 MB (39558608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df44f63ded7015da79f717c9dbf6dfd057bcafc06012bc1e415f53113e6fc1e5`  
		Last Modified: Tue, 13 Jun 2023 01:00:51 GMT  
		Size: 389.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8cfabfd56ee8b764abdf6f8cb20c091bea2ffae807bf04792799aa0ed635fb2`  
		Last Modified: Tue, 13 Jun 2023 01:01:18 GMT  
		Size: 2.7 KB (2708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:863747f21248ccdd5a53cf90d3ec3352b8cb75e1399bc41cdb2718127f287dd8`  
		Last Modified: Tue, 13 Jun 2023 01:01:18 GMT  
		Size: 1.9 KB (1863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee87568b44fcbd69476382c97061b27d53cae0b400d370e9825d16d684d27fa9`  
		Last Modified: Tue, 13 Jun 2023 01:01:18 GMT  
		Size: 1.5 KB (1476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b813c8ca03ebf5bac2b11cbbea4a8c154671aed01beacf714dd7337ac69228bc`  
		Last Modified: Tue, 13 Jun 2023 01:01:19 GMT  
		Size: 1.4 MB (1385320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3bf942bd785c5bd0709d7397f37a7b4de4e4359f2e16602e948dd4aeaaec333`  
		Last Modified: Tue, 13 Jun 2023 01:01:18 GMT  
		Size: 489.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-fastcgi` - linux; mips64le

```console
$ docker pull adminer@sha256:7c0ad002201eb7dba5d626c2e579249040821e733ac15405eac08b37f6819e18
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.6 MB (92616828 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e14b2773cb94782f55002ad5736b49d8d1715c22f62f831629a2edae0af93bc6`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Tue, 13 Jun 2023 00:09:46 GMT
ADD file:7ba4829e0a582c8a2e5a1d362ca30cfba3fa2911594faf9598927255100965b0 in / 
# Tue, 13 Jun 2023 00:09:51 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 01:46:11 GMT
STOPSIGNAL SIGINT
# Tue, 13 Jun 2023 01:48:01 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 01:48:08 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 13 Jun 2023 01:49:58 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Tue, 13 Jun 2023 01:50:04 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 13 Jun 2023 01:50:07 GMT
WORKDIR /var/www/html
# Tue, 13 Jun 2023 01:50:10 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 13 Jun 2023 01:50:14 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 13 Jun 2023 01:50:17 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 13 Jun 2023 01:50:20 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 13 Jun 2023 01:51:08 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Jun 2023 01:51:11 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 13 Jun 2023 01:51:14 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 13 Jun 2023 01:51:18 GMT
USER adminer
# Tue, 13 Jun 2023 01:51:21 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:ec034d426521af0a9addba08124f06b364f3364fd20ec9aec4e3364104a793d1`  
		Last Modified: Tue, 13 Jun 2023 00:23:13 GMT  
		Size: 53.3 MB (53270410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:901a0f1a33bd58f6d5e7b1de7a90c5fbe79c192cbbabfd8c7a98214496b73c1b`  
		Last Modified: Tue, 13 Jun 2023 01:52:11 GMT  
		Size: 38.0 MB (37953313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c616df06cfce4fa5e3f76b4147041f55275dd885295b9a2e1b9884f710f5a63`  
		Last Modified: Tue, 13 Jun 2023 01:51:45 GMT  
		Size: 395.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68463d39b900d79d99d0b981ac4de2e7b97ed79424dbbab27775b457b526f553`  
		Last Modified: Tue, 13 Jun 2023 01:52:30 GMT  
		Size: 2.7 KB (2711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecf4c4f53ea5745d056c4cf51430f6362a894011418ab8fc004aab4cac8818e8`  
		Last Modified: Tue, 13 Jun 2023 01:52:30 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:660f7e28cfd4cddb76bc3c880db1190a7a88b2d9b9d93d3e82f5c9b316d3dac5`  
		Last Modified: Tue, 13 Jun 2023 01:52:30 GMT  
		Size: 1.5 KB (1478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17fb5ff54e4d36c97aa5b67854279381fc77880b82436f347c9144327a7ba026`  
		Last Modified: Tue, 13 Jun 2023 01:52:31 GMT  
		Size: 1.4 MB (1386301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1fbe725d5b33c64787888d5b86edbf2d81e345c52311c4d0cd4b5631e8ce365`  
		Last Modified: Tue, 13 Jun 2023 01:52:31 GMT  
		Size: 489.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-fastcgi` - linux; ppc64le

```console
$ docker pull adminer@sha256:f08c2d2d4f6a743fd667ccd77b6e2ea2b906b925e0f09a35df232f82c4692e65
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.3 MB (101256485 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c3935c8e6ae819dd2093e8de8304a6e11a3aae1550d802ad8af7ed871d3cdb02`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Tue, 23 May 2023 01:17:14 GMT
ADD file:ed39869ee4bb8e1901b71feb9cadfe754e42304e134f2542e516e162ca710ec8 in / 
# Tue, 23 May 2023 01:17:17 GMT
CMD ["bash"]
# Tue, 23 May 2023 01:40:42 GMT
STOPSIGNAL SIGINT
# Tue, 23 May 2023 01:41:54 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 01:41:58 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 23 May 2023 01:42:53 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Tue, 23 May 2023 01:42:56 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 23 May 2023 01:42:56 GMT
WORKDIR /var/www/html
# Tue, 23 May 2023 01:42:57 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 23 May 2023 01:42:57 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 23 May 2023 01:42:58 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 23 May 2023 01:42:58 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 23 May 2023 01:43:32 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 23 May 2023 01:43:33 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 23 May 2023 01:43:34 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 23 May 2023 01:43:35 GMT
USER adminer
# Tue, 23 May 2023 01:43:36 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:f530a46e89ee571046fe19b22f563df6c84a31f6593a1e6ed49dbd16e34145de`  
		Last Modified: Tue, 23 May 2023 01:21:34 GMT  
		Size: 58.9 MB (58923948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b328a5c7e2019a9edf5b5d571d37da0261097706c34bafabd5196936aac3fc1b`  
		Last Modified: Tue, 23 May 2023 01:44:03 GMT  
		Size: 40.9 MB (40939928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b29d269a712c093f32a0be4629a0f17bc22fd6dad4be88d5f0af5ce757d809f`  
		Last Modified: Tue, 23 May 2023 01:43:51 GMT  
		Size: 393.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14b5ab23d41e8f1aea6954e2f0b6047fc125e9406f7c560374fe0316f980197e`  
		Last Modified: Tue, 23 May 2023 01:44:22 GMT  
		Size: 2.7 KB (2714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:977b08266ee6cbb32edd6f84d2a98dc861be41484b1401b545d9b0581c1bd174`  
		Last Modified: Tue, 23 May 2023 01:44:22 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92c78939508c16fc88e03d22beb6d700276d381b5a8262d3ff4658b877bad32a`  
		Last Modified: Tue, 23 May 2023 01:44:22 GMT  
		Size: 1.5 KB (1478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bce4c7c01da83a8e67c7a518b162fed2c676be30cdc2c055b920ee658f243cc`  
		Last Modified: Tue, 23 May 2023 01:44:22 GMT  
		Size: 1.4 MB (1385651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5548d29e362ba040749a780b4f79dc74ada494b0aaccaad9e4fbcd61a4b10c61`  
		Last Modified: Tue, 23 May 2023 01:44:22 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-fastcgi` - linux; s390x

```console
$ docker pull adminer@sha256:a194086c2f327aa2f518b1bde88023cd5f0d1cc9d8e0438ef5b392d68f1c3c79
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.7 MB (93692849 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5b04e5e9f13ffd3710ed52616df2923026fc40f821ca1f6247ca708b6decac7`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Tue, 23 May 2023 00:42:35 GMT
ADD file:a054112be60c3f2d7811b27cde82bccfd1c2747f29b7611ee68b21cd9f3d3d54 in / 
# Tue, 23 May 2023 00:42:41 GMT
CMD ["bash"]
# Tue, 23 May 2023 02:26:55 GMT
STOPSIGNAL SIGINT
# Tue, 23 May 2023 02:27:12 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 02:27:15 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 23 May 2023 02:27:31 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Tue, 23 May 2023 02:27:31 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 23 May 2023 02:27:31 GMT
WORKDIR /var/www/html
# Tue, 23 May 2023 02:27:31 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 23 May 2023 02:27:31 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 23 May 2023 02:27:32 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 23 May 2023 02:27:32 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 23 May 2023 02:27:39 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 23 May 2023 02:27:39 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 23 May 2023 02:27:39 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 23 May 2023 02:27:40 GMT
USER adminer
# Tue, 23 May 2023 02:27:40 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:44d1d02f91725dd9ae742f7c70add814dc3da3fde438adb01e65e1f8b0eba613`  
		Last Modified: Tue, 23 May 2023 00:45:33 GMT  
		Size: 53.3 MB (53282114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a714865cdf8c711665c7b864ae5f1e6c7100e6079a9d6bb3d8925f6a0cceaff2`  
		Last Modified: Tue, 23 May 2023 02:28:00 GMT  
		Size: 39.0 MB (39018332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a6faa7559a991fd1e86474adae5128141983567ad4587e50e92ce5d32755bbb`  
		Last Modified: Tue, 23 May 2023 02:27:53 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9101661d5aa45e85b42ae59aa229ccb0658ea3ab2507142a937c15393886927b`  
		Last Modified: Tue, 23 May 2023 02:28:10 GMT  
		Size: 2.7 KB (2708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70537aeb5de09054327e77121e9ac1e2c9309cd67388d6c9f3c6a246c0980aa7`  
		Last Modified: Tue, 23 May 2023 02:28:10 GMT  
		Size: 1.9 KB (1883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42f4125a64e5befb7b5b1dfe94aa43aa55cb192155eb38a12a6d86a3bf660210`  
		Last Modified: Tue, 23 May 2023 02:28:10 GMT  
		Size: 1.5 KB (1477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d338cb5258e7079119cbfe96033d5b49ee9e23aeb5860c5ffd0c1a8bb4342bcf`  
		Last Modified: Tue, 23 May 2023 02:28:11 GMT  
		Size: 1.4 MB (1385455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41ca25d71e32f1c6ef50badf5308e74f4afedccd9f322e5c0c4e2a75bc7a092d`  
		Last Modified: Tue, 23 May 2023 02:28:10 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `adminer:4-standalone`

```console
$ docker pull adminer@sha256:521aae780cec6678443058ecb03e3b20fd815e1c1220dc8370c3a3381acc736c
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
$ docker pull adminer@sha256:203c8ee52640268c28f5ce5f57b192d967da40a91d6443b57ae1da4064e2ed8b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.9 MB (95931867 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e4345c1c3dc89b4c31146abe340fa39e143d922d1e3401233d7ac32db2d985d`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Mon, 12 Jun 2023 23:20:54 GMT
ADD file:e530b0563ea53d97b2f28e62149a665900196f86611df99a88c7a8ab2097b95d in / 
# Mon, 12 Jun 2023 23:20:54 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 03:24:37 GMT
STOPSIGNAL SIGINT
# Tue, 13 Jun 2023 03:25:04 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 03:25:05 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 13 Jun 2023 03:25:06 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 13 Jun 2023 03:25:06 GMT
WORKDIR /var/www/html
# Tue, 13 Jun 2023 03:25:06 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 13 Jun 2023 03:25:06 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 13 Jun 2023 03:25:06 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 13 Jun 2023 03:25:06 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 13 Jun 2023 03:25:19 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Jun 2023 03:25:19 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 13 Jun 2023 03:25:19 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 13 Jun 2023 03:25:19 GMT
USER adminer
# Tue, 13 Jun 2023 03:25:19 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Tue, 13 Jun 2023 03:25:19 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:93c2d578e4211e82e47e7ada9ed05d1869a2362c6f7509f2ee8d91ccebfb7fbd`  
		Last Modified: Mon, 12 Jun 2023 23:26:08 GMT  
		Size: 55.1 MB (55055162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e099cf7ea37ba8ff2169a70f6743bf40675a661f0dc9b6a8abaa4e43050979c`  
		Last Modified: Tue, 13 Jun 2023 03:25:56 GMT  
		Size: 39.5 MB (39487054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d12c699384cbfa0b30a07efef5ad3b7f104e0e1f33e6a094e489150e4ef3838`  
		Last Modified: Tue, 13 Jun 2023 03:25:48 GMT  
		Size: 391.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05c66113a52b479d99efec54808f4045c5fe1400714639a6c750317ad501bc9c`  
		Last Modified: Tue, 13 Jun 2023 03:25:48 GMT  
		Size: 1.9 KB (1874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:677df7ad2be6c1e9f14d49043358dc765759c7f2cd0184ca55a55dc81dcb2263`  
		Last Modified: Tue, 13 Jun 2023 03:25:48 GMT  
		Size: 1.5 KB (1478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:598f6ab1ce2900168e83fbb661f1edc77e27dd8261b23a1f22af28e991facd6e`  
		Last Modified: Tue, 13 Jun 2023 03:25:49 GMT  
		Size: 1.4 MB (1385416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41ed709cb4bc1b53001ba47d24d74fb415c6142dd35194346fdac370144df45a`  
		Last Modified: Tue, 13 Jun 2023 03:25:48 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-standalone` - linux; arm variant v5

```console
$ docker pull adminer@sha256:15bb2436532d59fdbf58c3cbc74f61d47be5ad45e30d65bc01adcfc449dd0951
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.2 MB (91183934 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:267345bcacc239fd7427ea82c255b704e164984dbff20209a9e8439820a662d3`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Tue, 23 May 2023 00:48:32 GMT
ADD file:9572a8fcb9c86e8a9dbfe623c732cc4ba1c4f5670490191a7e639a272d5b6e97 in / 
# Tue, 23 May 2023 00:48:33 GMT
CMD ["bash"]
# Tue, 23 May 2023 01:09:52 GMT
STOPSIGNAL SIGINT
# Tue, 23 May 2023 01:10:29 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 01:10:30 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 23 May 2023 01:10:31 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 23 May 2023 01:10:31 GMT
WORKDIR /var/www/html
# Tue, 23 May 2023 01:10:31 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 23 May 2023 01:10:31 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 23 May 2023 01:10:31 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 23 May 2023 01:10:31 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 23 May 2023 01:10:46 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 23 May 2023 01:10:46 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 23 May 2023 01:10:46 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 23 May 2023 01:10:46 GMT
USER adminer
# Tue, 23 May 2023 01:10:46 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Tue, 23 May 2023 01:10:46 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:b053976742ca5b01bcefb7df8fc77a58d0becb4ce508792491574463930569c4`  
		Last Modified: Tue, 23 May 2023 00:50:55 GMT  
		Size: 52.5 MB (52546536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6448799a9363993edd93e5fb6040955191b829140af65c88550e510326878903`  
		Last Modified: Tue, 23 May 2023 01:11:21 GMT  
		Size: 37.2 MB (37247839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b03dc69db3dc4061f823e5e9025874ab539e706b64af3b103bf2a3e839890b8`  
		Last Modified: Tue, 23 May 2023 01:11:13 GMT  
		Size: 388.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ed315aa6041fcfd6bafc18c55ef5be23f10e057e9f941675330807b39d1e54a`  
		Last Modified: Tue, 23 May 2023 01:11:13 GMT  
		Size: 1.9 KB (1872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2d328016feebec5e083e36300e6444d56a5aedfba59d4be438549c64ebcb44f`  
		Last Modified: Tue, 23 May 2023 01:11:13 GMT  
		Size: 1.5 KB (1480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c98954d02c72cf9c2513f055817ac1435ded02424a3418c8d3b9164746bdf3c`  
		Last Modified: Tue, 23 May 2023 01:11:13 GMT  
		Size: 1.4 MB (1385327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aac95e0f74f942d3cfb111cf9949811151a49733af863c919807b2dcbb3a85a1`  
		Last Modified: Tue, 23 May 2023 01:11:13 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-standalone` - linux; arm variant v7

```console
$ docker pull adminer@sha256:98b76b0878cf9cc2684e5bbbdade79a5f2f6f269e230203870a1f1a752f7e7f1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.8 MB (87790748 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b51c4364b99328a719594799d5c3d616aeb43a95308f9cd320cb70d27dda4c17`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Mon, 12 Jun 2023 23:58:34 GMT
ADD file:6edc8f94d2ebc83d6081e1c4567963d0060a842c767eaff959a6e5c6d09247b5 in / 
# Mon, 12 Jun 2023 23:58:34 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 04:50:43 GMT
STOPSIGNAL SIGINT
# Tue, 13 Jun 2023 04:51:12 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 04:51:12 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 13 Jun 2023 04:51:13 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 13 Jun 2023 04:51:13 GMT
WORKDIR /var/www/html
# Tue, 13 Jun 2023 04:51:13 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 13 Jun 2023 04:51:13 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 13 Jun 2023 04:51:13 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 13 Jun 2023 04:51:13 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 13 Jun 2023 04:51:41 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Jun 2023 04:51:41 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 13 Jun 2023 04:51:41 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 13 Jun 2023 04:51:41 GMT
USER adminer
# Tue, 13 Jun 2023 04:51:42 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Tue, 13 Jun 2023 04:51:42 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:23807bbf2a5fd14b7975a9e82f4a5530bbba520f31b382cc4b4ce2e77e075ace`  
		Last Modified: Tue, 13 Jun 2023 00:04:02 GMT  
		Size: 50.2 MB (50218141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed9435d7956e105f98b0ce0d774c24da59c523bdcf4ec8fff644876978300c69`  
		Last Modified: Tue, 13 Jun 2023 04:52:24 GMT  
		Size: 36.2 MB (36183011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbf6d7965eb59f39902f271310a767cdf68bdc38bf15c4ee7bc3cfc5c2d025f8`  
		Last Modified: Tue, 13 Jun 2023 04:52:16 GMT  
		Size: 392.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da256b5543040f6999ae9a8cc020bfd0542286ecf71c77feb6cd08a4ecd9be37`  
		Last Modified: Tue, 13 Jun 2023 04:52:16 GMT  
		Size: 1.9 KB (1863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fac8d202305e7ac73502fb63bb1618ac53766c99e8cd03bcb0412c313a25dd83`  
		Last Modified: Tue, 13 Jun 2023 04:52:16 GMT  
		Size: 1.5 KB (1479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b96b3d518c63ab16389a582e075ae88f7225f3c35483203c7c52dcfa52f2daa5`  
		Last Modified: Tue, 13 Jun 2023 04:52:16 GMT  
		Size: 1.4 MB (1385372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eb5818f5b2f148baf53286364c0c6cd2df86e21ed76bfcbc6ff0688a5d2726c`  
		Last Modified: Tue, 13 Jun 2023 04:52:16 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-standalone` - linux; arm64 variant v8

```console
$ docker pull adminer@sha256:92cdfd552b3557e293045fc3d5f01d58871958912197649f3c818e312856bf85
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.3 MB (94336689 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b7e1c530248708005dc78825e6702d078b51bbd4eae6c82b2df135ce82d2961`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:22 GMT
ADD file:caddd2f40296ec5c1bf7487617ca8694cfff9a1d9b7484159e203b6514cb5f5f in / 
# Mon, 12 Jun 2023 23:40:23 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 04:45:49 GMT
STOPSIGNAL SIGINT
# Tue, 13 Jun 2023 04:46:10 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 04:46:11 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 13 Jun 2023 04:46:12 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 13 Jun 2023 04:46:12 GMT
WORKDIR /var/www/html
# Tue, 13 Jun 2023 04:46:12 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 13 Jun 2023 04:46:12 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 13 Jun 2023 04:46:12 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 13 Jun 2023 04:46:12 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 13 Jun 2023 04:46:22 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Jun 2023 04:46:22 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 13 Jun 2023 04:46:22 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 13 Jun 2023 04:46:22 GMT
USER adminer
# Tue, 13 Jun 2023 04:46:22 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Tue, 13 Jun 2023 04:46:23 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:663ccfaf62a5d7b997bca03d1dc6d5dfff01b9e0de08d86dbea8957ea92d7d16`  
		Last Modified: Mon, 12 Jun 2023 23:44:25 GMT  
		Size: 53.7 MB (53704136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80aa39d9a9c198e71855c642bc21b287cd96a68f1ca6f6095933aebd07835b55`  
		Last Modified: Tue, 13 Jun 2023 04:46:57 GMT  
		Size: 39.2 MB (39243014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35aba8c7c961932b274149a03d0e4ded7ce7529e514d523d33c6c6972b149b3d`  
		Last Modified: Tue, 13 Jun 2023 04:46:50 GMT  
		Size: 393.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe596da7a5da4c53bb7e8a57c4bca7d95147969f3fcfa27a9ac63992faacad68`  
		Last Modified: Tue, 13 Jun 2023 04:46:51 GMT  
		Size: 1.9 KB (1875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9f19157c079ccd39ddc0b6c916dec64e367d7b29ff37f7d51348654868ffeea`  
		Last Modified: Tue, 13 Jun 2023 04:46:51 GMT  
		Size: 1.5 KB (1482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e9f6bc36eded234b1a9ca40497b6b08e4a5ebd85b8077cfd4951499ef134c78`  
		Last Modified: Tue, 13 Jun 2023 04:46:51 GMT  
		Size: 1.4 MB (1385300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4689e75de5a00a90b25e2ae66464fad25ea65b849b83d549503bdfb11f72be63`  
		Last Modified: Tue, 13 Jun 2023 04:46:51 GMT  
		Size: 489.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-standalone` - linux; 386

```console
$ docker pull adminer@sha256:e0bb773bce27da86e8bba771ce6fb58fef553b675ea0e0e2c7eaa0d2bd7dd9f9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.0 MB (96988803 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77720ee3233be6352493a8d99e983f977b3e182750f1526bba6d67134b1bf7ee`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Mon, 12 Jun 2023 23:39:39 GMT
ADD file:4b1f447e0b75fbe493bd68bb77b74f4ba1c61ac8e14226e3c511b3a1c3d5721a in / 
# Mon, 12 Jun 2023 23:39:40 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 00:59:39 GMT
STOPSIGNAL SIGINT
# Tue, 13 Jun 2023 01:00:06 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 01:00:07 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 13 Jun 2023 01:00:07 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 13 Jun 2023 01:00:08 GMT
WORKDIR /var/www/html
# Tue, 13 Jun 2023 01:00:08 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 13 Jun 2023 01:00:08 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 13 Jun 2023 01:00:08 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 13 Jun 2023 01:00:08 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 13 Jun 2023 01:00:20 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Jun 2023 01:00:20 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 13 Jun 2023 01:00:20 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 13 Jun 2023 01:00:21 GMT
USER adminer
# Tue, 13 Jun 2023 01:00:21 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Tue, 13 Jun 2023 01:00:21 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:0997ae72d27731326552ad4699d630b4932f3d31abc07a62105a0eb16b54173a`  
		Last Modified: Mon, 12 Jun 2023 23:46:43 GMT  
		Size: 56.0 MB (56040665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dac97babbe48fc6ee5134482bf3dd02a0763c71618911c97beab64bec3147a8`  
		Last Modified: Tue, 13 Jun 2023 01:01:02 GMT  
		Size: 39.6 MB (39558608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df44f63ded7015da79f717c9dbf6dfd057bcafc06012bc1e415f53113e6fc1e5`  
		Last Modified: Tue, 13 Jun 2023 01:00:51 GMT  
		Size: 389.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ae3ce4c7547485956e0bd1180cc66032006af3b33c6ae582d77834096391752`  
		Last Modified: Tue, 13 Jun 2023 01:00:51 GMT  
		Size: 1.9 KB (1864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83417b3fe0dbbaed7076986fd209d6704b096ecd961a111cfb42cba80a11dc93`  
		Last Modified: Tue, 13 Jun 2023 01:00:51 GMT  
		Size: 1.5 KB (1480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbdb97551a1780228aac70017b847d497ec088d6ad3e46d5c8b9b48083efe5a0`  
		Last Modified: Tue, 13 Jun 2023 01:00:52 GMT  
		Size: 1.4 MB (1385307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbef3e3e2b3156ba5eca052ebf766f2f4474f980905836f0c0ea9eec319f7a6e`  
		Last Modified: Tue, 13 Jun 2023 01:00:51 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-standalone` - linux; mips64le

```console
$ docker pull adminer@sha256:2591b1f0dffbc4f123a4a3bd12c1cb46669c54383e8e23e13c83edaecc2541d1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.6 MB (92614104 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9a417a537dc4187139ad39c01263d6bd8b79a728bf005ad51d3bb4d42ec1d5f`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Tue, 13 Jun 2023 00:09:46 GMT
ADD file:7ba4829e0a582c8a2e5a1d362ca30cfba3fa2911594faf9598927255100965b0 in / 
# Tue, 13 Jun 2023 00:09:51 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 01:46:11 GMT
STOPSIGNAL SIGINT
# Tue, 13 Jun 2023 01:48:01 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 01:48:08 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 13 Jun 2023 01:48:14 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 13 Jun 2023 01:48:18 GMT
WORKDIR /var/www/html
# Tue, 13 Jun 2023 01:48:21 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 13 Jun 2023 01:48:24 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 13 Jun 2023 01:48:28 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 13 Jun 2023 01:48:31 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 13 Jun 2023 01:49:21 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Jun 2023 01:49:24 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 13 Jun 2023 01:49:27 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 13 Jun 2023 01:49:31 GMT
USER adminer
# Tue, 13 Jun 2023 01:49:34 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Tue, 13 Jun 2023 01:49:37 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:ec034d426521af0a9addba08124f06b364f3364fd20ec9aec4e3364104a793d1`  
		Last Modified: Tue, 13 Jun 2023 00:23:13 GMT  
		Size: 53.3 MB (53270410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:901a0f1a33bd58f6d5e7b1de7a90c5fbe79c192cbbabfd8c7a98214496b73c1b`  
		Last Modified: Tue, 13 Jun 2023 01:52:11 GMT  
		Size: 38.0 MB (37953313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c616df06cfce4fa5e3f76b4147041f55275dd885295b9a2e1b9884f710f5a63`  
		Last Modified: Tue, 13 Jun 2023 01:51:45 GMT  
		Size: 395.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84487562d4b36a6a1112b198b725b1a727e91a77be9899c0d74b1a4a9c022dba`  
		Last Modified: Tue, 13 Jun 2023 01:51:45 GMT  
		Size: 1.7 KB (1723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5dde6303cb52a3de95ebac876b6f8590487f4ffa08f8c0e80844f4d89b75072`  
		Last Modified: Tue, 13 Jun 2023 01:51:45 GMT  
		Size: 1.5 KB (1480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:499702681379ddde7be8cc76c78d9b9c764ceea9af16c336da3a99169971feb1`  
		Last Modified: Tue, 13 Jun 2023 01:51:46 GMT  
		Size: 1.4 MB (1386295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63d75b2d63e14c568323dc0897c171f4d71efe33d94bb1423a59c555514d35ae`  
		Last Modified: Tue, 13 Jun 2023 01:51:45 GMT  
		Size: 488.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-standalone` - linux; ppc64le

```console
$ docker pull adminer@sha256:e0a0e907c5c635e5e363e08b1dffd85143970ad1e4dee8cd2acdbd2c47f59f30
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.3 MB (101253778 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0759ab5b0827c3e5903a54d9e690f3911052bcece85af789658d87469a6c4e41`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Tue, 23 May 2023 01:17:14 GMT
ADD file:ed39869ee4bb8e1901b71feb9cadfe754e42304e134f2542e516e162ca710ec8 in / 
# Tue, 23 May 2023 01:17:17 GMT
CMD ["bash"]
# Tue, 23 May 2023 01:40:42 GMT
STOPSIGNAL SIGINT
# Tue, 23 May 2023 01:41:54 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 01:41:58 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 23 May 2023 01:42:00 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 23 May 2023 01:42:01 GMT
WORKDIR /var/www/html
# Tue, 23 May 2023 01:42:01 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 23 May 2023 01:42:02 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 23 May 2023 01:42:02 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 23 May 2023 01:42:02 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 23 May 2023 01:42:36 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 23 May 2023 01:42:37 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 23 May 2023 01:42:37 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 23 May 2023 01:42:38 GMT
USER adminer
# Tue, 23 May 2023 01:42:39 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Tue, 23 May 2023 01:42:40 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:f530a46e89ee571046fe19b22f563df6c84a31f6593a1e6ed49dbd16e34145de`  
		Last Modified: Tue, 23 May 2023 01:21:34 GMT  
		Size: 58.9 MB (58923948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b328a5c7e2019a9edf5b5d571d37da0261097706c34bafabd5196936aac3fc1b`  
		Last Modified: Tue, 23 May 2023 01:44:03 GMT  
		Size: 40.9 MB (40939928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b29d269a712c093f32a0be4629a0f17bc22fd6dad4be88d5f0af5ce757d809f`  
		Last Modified: Tue, 23 May 2023 01:43:51 GMT  
		Size: 393.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:904564df90e41e35afa3221ab3277e3aa554b7c686393785c1b07372bc0c4d4d`  
		Last Modified: Tue, 23 May 2023 01:43:51 GMT  
		Size: 1.9 KB (1880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55a789415d78b4a3befd6b003659799bcf3d20cb06639a961c96a980640e8991`  
		Last Modified: Tue, 23 May 2023 01:43:51 GMT  
		Size: 1.5 KB (1479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78c991997ea0a176dc01a5a08f6ac61143299aef87572cd7e8578e479aae772b`  
		Last Modified: Tue, 23 May 2023 01:43:52 GMT  
		Size: 1.4 MB (1385657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd039d869a125163f2302899c7b0fcf2db140dad2eecedc648b3ca229cb86460`  
		Last Modified: Tue, 23 May 2023 01:43:51 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-standalone` - linux; s390x

```console
$ docker pull adminer@sha256:b48c2c7360476d0f6ce0723abeef59ed2cc19493ffedd144d64ee2b5d0a21683
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.7 MB (93690153 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:008c852f84add504c1031fabd62a8ede6758604b42d91789507acf3c08df5507`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Tue, 23 May 2023 00:42:35 GMT
ADD file:a054112be60c3f2d7811b27cde82bccfd1c2747f29b7611ee68b21cd9f3d3d54 in / 
# Tue, 23 May 2023 00:42:41 GMT
CMD ["bash"]
# Tue, 23 May 2023 02:26:55 GMT
STOPSIGNAL SIGINT
# Tue, 23 May 2023 02:27:12 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 02:27:15 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 23 May 2023 02:27:15 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 23 May 2023 02:27:15 GMT
WORKDIR /var/www/html
# Tue, 23 May 2023 02:27:15 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 23 May 2023 02:27:15 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 23 May 2023 02:27:16 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 23 May 2023 02:27:16 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 23 May 2023 02:27:23 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 23 May 2023 02:27:23 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 23 May 2023 02:27:23 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 23 May 2023 02:27:24 GMT
USER adminer
# Tue, 23 May 2023 02:27:24 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Tue, 23 May 2023 02:27:24 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:44d1d02f91725dd9ae742f7c70add814dc3da3fde438adb01e65e1f8b0eba613`  
		Last Modified: Tue, 23 May 2023 00:45:33 GMT  
		Size: 53.3 MB (53282114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a714865cdf8c711665c7b864ae5f1e6c7100e6079a9d6bb3d8925f6a0cceaff2`  
		Last Modified: Tue, 23 May 2023 02:28:00 GMT  
		Size: 39.0 MB (39018332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a6faa7559a991fd1e86474adae5128141983567ad4587e50e92ce5d32755bbb`  
		Last Modified: Tue, 23 May 2023 02:27:53 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f55cc440fda23758bbfb18b1a3881ac61d06ad9e0a4b35da688b713c1b8611be`  
		Last Modified: Tue, 23 May 2023 02:27:53 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d16d617d4904a95242ab9db1204e6fa0d844358dc62528fed7ad368f57b1251d`  
		Last Modified: Tue, 23 May 2023 02:27:53 GMT  
		Size: 1.5 KB (1478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c753b23f0be5c140b7bed93c7220f68e38f138d53d3e7e9aade64a9d4b45038e`  
		Last Modified: Tue, 23 May 2023 02:27:53 GMT  
		Size: 1.4 MB (1385466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a436f3a56433ffbdc8b5e6a7bda069a68625447867738966931d19c9db78365c`  
		Last Modified: Tue, 23 May 2023 02:27:53 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `adminer:4.8.1`

```console
$ docker pull adminer@sha256:521aae780cec6678443058ecb03e3b20fd815e1c1220dc8370c3a3381acc736c
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
$ docker pull adminer@sha256:203c8ee52640268c28f5ce5f57b192d967da40a91d6443b57ae1da4064e2ed8b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.9 MB (95931867 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e4345c1c3dc89b4c31146abe340fa39e143d922d1e3401233d7ac32db2d985d`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Mon, 12 Jun 2023 23:20:54 GMT
ADD file:e530b0563ea53d97b2f28e62149a665900196f86611df99a88c7a8ab2097b95d in / 
# Mon, 12 Jun 2023 23:20:54 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 03:24:37 GMT
STOPSIGNAL SIGINT
# Tue, 13 Jun 2023 03:25:04 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 03:25:05 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 13 Jun 2023 03:25:06 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 13 Jun 2023 03:25:06 GMT
WORKDIR /var/www/html
# Tue, 13 Jun 2023 03:25:06 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 13 Jun 2023 03:25:06 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 13 Jun 2023 03:25:06 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 13 Jun 2023 03:25:06 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 13 Jun 2023 03:25:19 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Jun 2023 03:25:19 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 13 Jun 2023 03:25:19 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 13 Jun 2023 03:25:19 GMT
USER adminer
# Tue, 13 Jun 2023 03:25:19 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Tue, 13 Jun 2023 03:25:19 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:93c2d578e4211e82e47e7ada9ed05d1869a2362c6f7509f2ee8d91ccebfb7fbd`  
		Last Modified: Mon, 12 Jun 2023 23:26:08 GMT  
		Size: 55.1 MB (55055162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e099cf7ea37ba8ff2169a70f6743bf40675a661f0dc9b6a8abaa4e43050979c`  
		Last Modified: Tue, 13 Jun 2023 03:25:56 GMT  
		Size: 39.5 MB (39487054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d12c699384cbfa0b30a07efef5ad3b7f104e0e1f33e6a094e489150e4ef3838`  
		Last Modified: Tue, 13 Jun 2023 03:25:48 GMT  
		Size: 391.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05c66113a52b479d99efec54808f4045c5fe1400714639a6c750317ad501bc9c`  
		Last Modified: Tue, 13 Jun 2023 03:25:48 GMT  
		Size: 1.9 KB (1874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:677df7ad2be6c1e9f14d49043358dc765759c7f2cd0184ca55a55dc81dcb2263`  
		Last Modified: Tue, 13 Jun 2023 03:25:48 GMT  
		Size: 1.5 KB (1478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:598f6ab1ce2900168e83fbb661f1edc77e27dd8261b23a1f22af28e991facd6e`  
		Last Modified: Tue, 13 Jun 2023 03:25:49 GMT  
		Size: 1.4 MB (1385416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41ed709cb4bc1b53001ba47d24d74fb415c6142dd35194346fdac370144df45a`  
		Last Modified: Tue, 13 Jun 2023 03:25:48 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1` - linux; arm variant v5

```console
$ docker pull adminer@sha256:15bb2436532d59fdbf58c3cbc74f61d47be5ad45e30d65bc01adcfc449dd0951
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.2 MB (91183934 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:267345bcacc239fd7427ea82c255b704e164984dbff20209a9e8439820a662d3`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Tue, 23 May 2023 00:48:32 GMT
ADD file:9572a8fcb9c86e8a9dbfe623c732cc4ba1c4f5670490191a7e639a272d5b6e97 in / 
# Tue, 23 May 2023 00:48:33 GMT
CMD ["bash"]
# Tue, 23 May 2023 01:09:52 GMT
STOPSIGNAL SIGINT
# Tue, 23 May 2023 01:10:29 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 01:10:30 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 23 May 2023 01:10:31 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 23 May 2023 01:10:31 GMT
WORKDIR /var/www/html
# Tue, 23 May 2023 01:10:31 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 23 May 2023 01:10:31 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 23 May 2023 01:10:31 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 23 May 2023 01:10:31 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 23 May 2023 01:10:46 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 23 May 2023 01:10:46 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 23 May 2023 01:10:46 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 23 May 2023 01:10:46 GMT
USER adminer
# Tue, 23 May 2023 01:10:46 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Tue, 23 May 2023 01:10:46 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:b053976742ca5b01bcefb7df8fc77a58d0becb4ce508792491574463930569c4`  
		Last Modified: Tue, 23 May 2023 00:50:55 GMT  
		Size: 52.5 MB (52546536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6448799a9363993edd93e5fb6040955191b829140af65c88550e510326878903`  
		Last Modified: Tue, 23 May 2023 01:11:21 GMT  
		Size: 37.2 MB (37247839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b03dc69db3dc4061f823e5e9025874ab539e706b64af3b103bf2a3e839890b8`  
		Last Modified: Tue, 23 May 2023 01:11:13 GMT  
		Size: 388.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ed315aa6041fcfd6bafc18c55ef5be23f10e057e9f941675330807b39d1e54a`  
		Last Modified: Tue, 23 May 2023 01:11:13 GMT  
		Size: 1.9 KB (1872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2d328016feebec5e083e36300e6444d56a5aedfba59d4be438549c64ebcb44f`  
		Last Modified: Tue, 23 May 2023 01:11:13 GMT  
		Size: 1.5 KB (1480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c98954d02c72cf9c2513f055817ac1435ded02424a3418c8d3b9164746bdf3c`  
		Last Modified: Tue, 23 May 2023 01:11:13 GMT  
		Size: 1.4 MB (1385327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aac95e0f74f942d3cfb111cf9949811151a49733af863c919807b2dcbb3a85a1`  
		Last Modified: Tue, 23 May 2023 01:11:13 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1` - linux; arm variant v7

```console
$ docker pull adminer@sha256:98b76b0878cf9cc2684e5bbbdade79a5f2f6f269e230203870a1f1a752f7e7f1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.8 MB (87790748 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b51c4364b99328a719594799d5c3d616aeb43a95308f9cd320cb70d27dda4c17`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Mon, 12 Jun 2023 23:58:34 GMT
ADD file:6edc8f94d2ebc83d6081e1c4567963d0060a842c767eaff959a6e5c6d09247b5 in / 
# Mon, 12 Jun 2023 23:58:34 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 04:50:43 GMT
STOPSIGNAL SIGINT
# Tue, 13 Jun 2023 04:51:12 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 04:51:12 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 13 Jun 2023 04:51:13 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 13 Jun 2023 04:51:13 GMT
WORKDIR /var/www/html
# Tue, 13 Jun 2023 04:51:13 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 13 Jun 2023 04:51:13 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 13 Jun 2023 04:51:13 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 13 Jun 2023 04:51:13 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 13 Jun 2023 04:51:41 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Jun 2023 04:51:41 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 13 Jun 2023 04:51:41 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 13 Jun 2023 04:51:41 GMT
USER adminer
# Tue, 13 Jun 2023 04:51:42 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Tue, 13 Jun 2023 04:51:42 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:23807bbf2a5fd14b7975a9e82f4a5530bbba520f31b382cc4b4ce2e77e075ace`  
		Last Modified: Tue, 13 Jun 2023 00:04:02 GMT  
		Size: 50.2 MB (50218141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed9435d7956e105f98b0ce0d774c24da59c523bdcf4ec8fff644876978300c69`  
		Last Modified: Tue, 13 Jun 2023 04:52:24 GMT  
		Size: 36.2 MB (36183011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbf6d7965eb59f39902f271310a767cdf68bdc38bf15c4ee7bc3cfc5c2d025f8`  
		Last Modified: Tue, 13 Jun 2023 04:52:16 GMT  
		Size: 392.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da256b5543040f6999ae9a8cc020bfd0542286ecf71c77feb6cd08a4ecd9be37`  
		Last Modified: Tue, 13 Jun 2023 04:52:16 GMT  
		Size: 1.9 KB (1863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fac8d202305e7ac73502fb63bb1618ac53766c99e8cd03bcb0412c313a25dd83`  
		Last Modified: Tue, 13 Jun 2023 04:52:16 GMT  
		Size: 1.5 KB (1479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b96b3d518c63ab16389a582e075ae88f7225f3c35483203c7c52dcfa52f2daa5`  
		Last Modified: Tue, 13 Jun 2023 04:52:16 GMT  
		Size: 1.4 MB (1385372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eb5818f5b2f148baf53286364c0c6cd2df86e21ed76bfcbc6ff0688a5d2726c`  
		Last Modified: Tue, 13 Jun 2023 04:52:16 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1` - linux; arm64 variant v8

```console
$ docker pull adminer@sha256:92cdfd552b3557e293045fc3d5f01d58871958912197649f3c818e312856bf85
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.3 MB (94336689 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b7e1c530248708005dc78825e6702d078b51bbd4eae6c82b2df135ce82d2961`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:22 GMT
ADD file:caddd2f40296ec5c1bf7487617ca8694cfff9a1d9b7484159e203b6514cb5f5f in / 
# Mon, 12 Jun 2023 23:40:23 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 04:45:49 GMT
STOPSIGNAL SIGINT
# Tue, 13 Jun 2023 04:46:10 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 04:46:11 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 13 Jun 2023 04:46:12 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 13 Jun 2023 04:46:12 GMT
WORKDIR /var/www/html
# Tue, 13 Jun 2023 04:46:12 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 13 Jun 2023 04:46:12 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 13 Jun 2023 04:46:12 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 13 Jun 2023 04:46:12 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 13 Jun 2023 04:46:22 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Jun 2023 04:46:22 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 13 Jun 2023 04:46:22 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 13 Jun 2023 04:46:22 GMT
USER adminer
# Tue, 13 Jun 2023 04:46:22 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Tue, 13 Jun 2023 04:46:23 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:663ccfaf62a5d7b997bca03d1dc6d5dfff01b9e0de08d86dbea8957ea92d7d16`  
		Last Modified: Mon, 12 Jun 2023 23:44:25 GMT  
		Size: 53.7 MB (53704136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80aa39d9a9c198e71855c642bc21b287cd96a68f1ca6f6095933aebd07835b55`  
		Last Modified: Tue, 13 Jun 2023 04:46:57 GMT  
		Size: 39.2 MB (39243014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35aba8c7c961932b274149a03d0e4ded7ce7529e514d523d33c6c6972b149b3d`  
		Last Modified: Tue, 13 Jun 2023 04:46:50 GMT  
		Size: 393.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe596da7a5da4c53bb7e8a57c4bca7d95147969f3fcfa27a9ac63992faacad68`  
		Last Modified: Tue, 13 Jun 2023 04:46:51 GMT  
		Size: 1.9 KB (1875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9f19157c079ccd39ddc0b6c916dec64e367d7b29ff37f7d51348654868ffeea`  
		Last Modified: Tue, 13 Jun 2023 04:46:51 GMT  
		Size: 1.5 KB (1482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e9f6bc36eded234b1a9ca40497b6b08e4a5ebd85b8077cfd4951499ef134c78`  
		Last Modified: Tue, 13 Jun 2023 04:46:51 GMT  
		Size: 1.4 MB (1385300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4689e75de5a00a90b25e2ae66464fad25ea65b849b83d549503bdfb11f72be63`  
		Last Modified: Tue, 13 Jun 2023 04:46:51 GMT  
		Size: 489.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1` - linux; 386

```console
$ docker pull adminer@sha256:e0bb773bce27da86e8bba771ce6fb58fef553b675ea0e0e2c7eaa0d2bd7dd9f9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.0 MB (96988803 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77720ee3233be6352493a8d99e983f977b3e182750f1526bba6d67134b1bf7ee`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Mon, 12 Jun 2023 23:39:39 GMT
ADD file:4b1f447e0b75fbe493bd68bb77b74f4ba1c61ac8e14226e3c511b3a1c3d5721a in / 
# Mon, 12 Jun 2023 23:39:40 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 00:59:39 GMT
STOPSIGNAL SIGINT
# Tue, 13 Jun 2023 01:00:06 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 01:00:07 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 13 Jun 2023 01:00:07 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 13 Jun 2023 01:00:08 GMT
WORKDIR /var/www/html
# Tue, 13 Jun 2023 01:00:08 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 13 Jun 2023 01:00:08 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 13 Jun 2023 01:00:08 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 13 Jun 2023 01:00:08 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 13 Jun 2023 01:00:20 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Jun 2023 01:00:20 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 13 Jun 2023 01:00:20 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 13 Jun 2023 01:00:21 GMT
USER adminer
# Tue, 13 Jun 2023 01:00:21 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Tue, 13 Jun 2023 01:00:21 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:0997ae72d27731326552ad4699d630b4932f3d31abc07a62105a0eb16b54173a`  
		Last Modified: Mon, 12 Jun 2023 23:46:43 GMT  
		Size: 56.0 MB (56040665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dac97babbe48fc6ee5134482bf3dd02a0763c71618911c97beab64bec3147a8`  
		Last Modified: Tue, 13 Jun 2023 01:01:02 GMT  
		Size: 39.6 MB (39558608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df44f63ded7015da79f717c9dbf6dfd057bcafc06012bc1e415f53113e6fc1e5`  
		Last Modified: Tue, 13 Jun 2023 01:00:51 GMT  
		Size: 389.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ae3ce4c7547485956e0bd1180cc66032006af3b33c6ae582d77834096391752`  
		Last Modified: Tue, 13 Jun 2023 01:00:51 GMT  
		Size: 1.9 KB (1864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83417b3fe0dbbaed7076986fd209d6704b096ecd961a111cfb42cba80a11dc93`  
		Last Modified: Tue, 13 Jun 2023 01:00:51 GMT  
		Size: 1.5 KB (1480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbdb97551a1780228aac70017b847d497ec088d6ad3e46d5c8b9b48083efe5a0`  
		Last Modified: Tue, 13 Jun 2023 01:00:52 GMT  
		Size: 1.4 MB (1385307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbef3e3e2b3156ba5eca052ebf766f2f4474f980905836f0c0ea9eec319f7a6e`  
		Last Modified: Tue, 13 Jun 2023 01:00:51 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1` - linux; mips64le

```console
$ docker pull adminer@sha256:2591b1f0dffbc4f123a4a3bd12c1cb46669c54383e8e23e13c83edaecc2541d1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.6 MB (92614104 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9a417a537dc4187139ad39c01263d6bd8b79a728bf005ad51d3bb4d42ec1d5f`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Tue, 13 Jun 2023 00:09:46 GMT
ADD file:7ba4829e0a582c8a2e5a1d362ca30cfba3fa2911594faf9598927255100965b0 in / 
# Tue, 13 Jun 2023 00:09:51 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 01:46:11 GMT
STOPSIGNAL SIGINT
# Tue, 13 Jun 2023 01:48:01 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 01:48:08 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 13 Jun 2023 01:48:14 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 13 Jun 2023 01:48:18 GMT
WORKDIR /var/www/html
# Tue, 13 Jun 2023 01:48:21 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 13 Jun 2023 01:48:24 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 13 Jun 2023 01:48:28 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 13 Jun 2023 01:48:31 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 13 Jun 2023 01:49:21 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Jun 2023 01:49:24 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 13 Jun 2023 01:49:27 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 13 Jun 2023 01:49:31 GMT
USER adminer
# Tue, 13 Jun 2023 01:49:34 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Tue, 13 Jun 2023 01:49:37 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:ec034d426521af0a9addba08124f06b364f3364fd20ec9aec4e3364104a793d1`  
		Last Modified: Tue, 13 Jun 2023 00:23:13 GMT  
		Size: 53.3 MB (53270410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:901a0f1a33bd58f6d5e7b1de7a90c5fbe79c192cbbabfd8c7a98214496b73c1b`  
		Last Modified: Tue, 13 Jun 2023 01:52:11 GMT  
		Size: 38.0 MB (37953313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c616df06cfce4fa5e3f76b4147041f55275dd885295b9a2e1b9884f710f5a63`  
		Last Modified: Tue, 13 Jun 2023 01:51:45 GMT  
		Size: 395.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84487562d4b36a6a1112b198b725b1a727e91a77be9899c0d74b1a4a9c022dba`  
		Last Modified: Tue, 13 Jun 2023 01:51:45 GMT  
		Size: 1.7 KB (1723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5dde6303cb52a3de95ebac876b6f8590487f4ffa08f8c0e80844f4d89b75072`  
		Last Modified: Tue, 13 Jun 2023 01:51:45 GMT  
		Size: 1.5 KB (1480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:499702681379ddde7be8cc76c78d9b9c764ceea9af16c336da3a99169971feb1`  
		Last Modified: Tue, 13 Jun 2023 01:51:46 GMT  
		Size: 1.4 MB (1386295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63d75b2d63e14c568323dc0897c171f4d71efe33d94bb1423a59c555514d35ae`  
		Last Modified: Tue, 13 Jun 2023 01:51:45 GMT  
		Size: 488.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1` - linux; ppc64le

```console
$ docker pull adminer@sha256:e0a0e907c5c635e5e363e08b1dffd85143970ad1e4dee8cd2acdbd2c47f59f30
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.3 MB (101253778 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0759ab5b0827c3e5903a54d9e690f3911052bcece85af789658d87469a6c4e41`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Tue, 23 May 2023 01:17:14 GMT
ADD file:ed39869ee4bb8e1901b71feb9cadfe754e42304e134f2542e516e162ca710ec8 in / 
# Tue, 23 May 2023 01:17:17 GMT
CMD ["bash"]
# Tue, 23 May 2023 01:40:42 GMT
STOPSIGNAL SIGINT
# Tue, 23 May 2023 01:41:54 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 01:41:58 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 23 May 2023 01:42:00 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 23 May 2023 01:42:01 GMT
WORKDIR /var/www/html
# Tue, 23 May 2023 01:42:01 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 23 May 2023 01:42:02 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 23 May 2023 01:42:02 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 23 May 2023 01:42:02 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 23 May 2023 01:42:36 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 23 May 2023 01:42:37 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 23 May 2023 01:42:37 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 23 May 2023 01:42:38 GMT
USER adminer
# Tue, 23 May 2023 01:42:39 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Tue, 23 May 2023 01:42:40 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:f530a46e89ee571046fe19b22f563df6c84a31f6593a1e6ed49dbd16e34145de`  
		Last Modified: Tue, 23 May 2023 01:21:34 GMT  
		Size: 58.9 MB (58923948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b328a5c7e2019a9edf5b5d571d37da0261097706c34bafabd5196936aac3fc1b`  
		Last Modified: Tue, 23 May 2023 01:44:03 GMT  
		Size: 40.9 MB (40939928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b29d269a712c093f32a0be4629a0f17bc22fd6dad4be88d5f0af5ce757d809f`  
		Last Modified: Tue, 23 May 2023 01:43:51 GMT  
		Size: 393.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:904564df90e41e35afa3221ab3277e3aa554b7c686393785c1b07372bc0c4d4d`  
		Last Modified: Tue, 23 May 2023 01:43:51 GMT  
		Size: 1.9 KB (1880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55a789415d78b4a3befd6b003659799bcf3d20cb06639a961c96a980640e8991`  
		Last Modified: Tue, 23 May 2023 01:43:51 GMT  
		Size: 1.5 KB (1479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78c991997ea0a176dc01a5a08f6ac61143299aef87572cd7e8578e479aae772b`  
		Last Modified: Tue, 23 May 2023 01:43:52 GMT  
		Size: 1.4 MB (1385657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd039d869a125163f2302899c7b0fcf2db140dad2eecedc648b3ca229cb86460`  
		Last Modified: Tue, 23 May 2023 01:43:51 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1` - linux; s390x

```console
$ docker pull adminer@sha256:b48c2c7360476d0f6ce0723abeef59ed2cc19493ffedd144d64ee2b5d0a21683
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.7 MB (93690153 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:008c852f84add504c1031fabd62a8ede6758604b42d91789507acf3c08df5507`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Tue, 23 May 2023 00:42:35 GMT
ADD file:a054112be60c3f2d7811b27cde82bccfd1c2747f29b7611ee68b21cd9f3d3d54 in / 
# Tue, 23 May 2023 00:42:41 GMT
CMD ["bash"]
# Tue, 23 May 2023 02:26:55 GMT
STOPSIGNAL SIGINT
# Tue, 23 May 2023 02:27:12 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 02:27:15 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 23 May 2023 02:27:15 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 23 May 2023 02:27:15 GMT
WORKDIR /var/www/html
# Tue, 23 May 2023 02:27:15 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 23 May 2023 02:27:15 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 23 May 2023 02:27:16 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 23 May 2023 02:27:16 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 23 May 2023 02:27:23 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 23 May 2023 02:27:23 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 23 May 2023 02:27:23 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 23 May 2023 02:27:24 GMT
USER adminer
# Tue, 23 May 2023 02:27:24 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Tue, 23 May 2023 02:27:24 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:44d1d02f91725dd9ae742f7c70add814dc3da3fde438adb01e65e1f8b0eba613`  
		Last Modified: Tue, 23 May 2023 00:45:33 GMT  
		Size: 53.3 MB (53282114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a714865cdf8c711665c7b864ae5f1e6c7100e6079a9d6bb3d8925f6a0cceaff2`  
		Last Modified: Tue, 23 May 2023 02:28:00 GMT  
		Size: 39.0 MB (39018332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a6faa7559a991fd1e86474adae5128141983567ad4587e50e92ce5d32755bbb`  
		Last Modified: Tue, 23 May 2023 02:27:53 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f55cc440fda23758bbfb18b1a3881ac61d06ad9e0a4b35da688b713c1b8611be`  
		Last Modified: Tue, 23 May 2023 02:27:53 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d16d617d4904a95242ab9db1204e6fa0d844358dc62528fed7ad368f57b1251d`  
		Last Modified: Tue, 23 May 2023 02:27:53 GMT  
		Size: 1.5 KB (1478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c753b23f0be5c140b7bed93c7220f68e38f138d53d3e7e9aade64a9d4b45038e`  
		Last Modified: Tue, 23 May 2023 02:27:53 GMT  
		Size: 1.4 MB (1385466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a436f3a56433ffbdc8b5e6a7bda069a68625447867738966931d19c9db78365c`  
		Last Modified: Tue, 23 May 2023 02:27:53 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `adminer:4.8.1-fastcgi`

```console
$ docker pull adminer@sha256:f67d780396297178e7b0d659328093579772caa59834ea077b2d00edc2b2d3c3
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
$ docker pull adminer@sha256:19e342979ee9fe7dbce42adf4070530e4fab8743bc177b4b401efc984ab1e40b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.9 MB (95934602 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:452a956cc7253ee0c04d3736127b355e67a5cd14dda7c0aaf0c2d18ab50277f1`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Mon, 12 Jun 2023 23:20:54 GMT
ADD file:e530b0563ea53d97b2f28e62149a665900196f86611df99a88c7a8ab2097b95d in / 
# Mon, 12 Jun 2023 23:20:54 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 03:24:37 GMT
STOPSIGNAL SIGINT
# Tue, 13 Jun 2023 03:25:04 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 03:25:05 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 13 Jun 2023 03:25:26 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Tue, 13 Jun 2023 03:25:26 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 13 Jun 2023 03:25:26 GMT
WORKDIR /var/www/html
# Tue, 13 Jun 2023 03:25:26 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 13 Jun 2023 03:25:26 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 13 Jun 2023 03:25:26 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 13 Jun 2023 03:25:27 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 13 Jun 2023 03:25:37 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Jun 2023 03:25:37 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 13 Jun 2023 03:25:37 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 13 Jun 2023 03:25:37 GMT
USER adminer
# Tue, 13 Jun 2023 03:25:38 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:93c2d578e4211e82e47e7ada9ed05d1869a2362c6f7509f2ee8d91ccebfb7fbd`  
		Last Modified: Mon, 12 Jun 2023 23:26:08 GMT  
		Size: 55.1 MB (55055162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e099cf7ea37ba8ff2169a70f6743bf40675a661f0dc9b6a8abaa4e43050979c`  
		Last Modified: Tue, 13 Jun 2023 03:25:56 GMT  
		Size: 39.5 MB (39487054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d12c699384cbfa0b30a07efef5ad3b7f104e0e1f33e6a094e489150e4ef3838`  
		Last Modified: Tue, 13 Jun 2023 03:25:48 GMT  
		Size: 391.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a83e8c3036470b387287b92b025e756b2d38926bd08a60b788905721b2710970`  
		Last Modified: Tue, 13 Jun 2023 03:26:11 GMT  
		Size: 2.7 KB (2706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4474445ef61d8bccb5f84a0c1af50393a4283332687b853db43b67b7c8ea97ac`  
		Last Modified: Tue, 13 Jun 2023 03:26:11 GMT  
		Size: 1.9 KB (1869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9d7d23c4974a9d08d6b18826eb53254571cb1eae70efa61ee681248a11cdcdc`  
		Last Modified: Tue, 13 Jun 2023 03:26:11 GMT  
		Size: 1.5 KB (1475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:420c1637804f967bec0a6f2d1c8e796d18bad5b8a06dadd562b9e930aa597924`  
		Last Modified: Tue, 13 Jun 2023 03:26:11 GMT  
		Size: 1.4 MB (1385457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1963affabab6ca86abab89a12ea096a70efa4ae2aae5c58c80a429a8c88afab2`  
		Last Modified: Tue, 13 Jun 2023 03:26:11 GMT  
		Size: 488.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1-fastcgi` - linux; arm variant v5

```console
$ docker pull adminer@sha256:874aa6f218690a93c384b0f19fc246af20d395854f936f59bc3547bacd22ac8d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.2 MB (91186662 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad52da629ff3a29fd1d27c9c82784df59d0303ac68e619208119f622c79f3f32`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Tue, 23 May 2023 00:48:32 GMT
ADD file:9572a8fcb9c86e8a9dbfe623c732cc4ba1c4f5670490191a7e639a272d5b6e97 in / 
# Tue, 23 May 2023 00:48:33 GMT
CMD ["bash"]
# Tue, 23 May 2023 01:09:52 GMT
STOPSIGNAL SIGINT
# Tue, 23 May 2023 01:10:29 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 01:10:30 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 23 May 2023 01:10:49 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Tue, 23 May 2023 01:10:50 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 23 May 2023 01:10:50 GMT
WORKDIR /var/www/html
# Tue, 23 May 2023 01:10:50 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 23 May 2023 01:10:50 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 23 May 2023 01:10:50 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 23 May 2023 01:10:50 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 23 May 2023 01:11:03 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 23 May 2023 01:11:03 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 23 May 2023 01:11:03 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 23 May 2023 01:11:03 GMT
USER adminer
# Tue, 23 May 2023 01:11:04 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:b053976742ca5b01bcefb7df8fc77a58d0becb4ce508792491574463930569c4`  
		Last Modified: Tue, 23 May 2023 00:50:55 GMT  
		Size: 52.5 MB (52546536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6448799a9363993edd93e5fb6040955191b829140af65c88550e510326878903`  
		Last Modified: Tue, 23 May 2023 01:11:21 GMT  
		Size: 37.2 MB (37247839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b03dc69db3dc4061f823e5e9025874ab539e706b64af3b103bf2a3e839890b8`  
		Last Modified: Tue, 23 May 2023 01:11:13 GMT  
		Size: 388.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b485dfbb13977609126b9a2977c8377b44b256b17a3eb1ca752d5dcd2f1c355`  
		Last Modified: Tue, 23 May 2023 01:11:38 GMT  
		Size: 2.7 KB (2710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:468ca8e69b40ea1983b6fcb3612d2309983339ff59fb02fc827a331cfe0ec7e8`  
		Last Modified: Tue, 23 May 2023 01:11:38 GMT  
		Size: 1.9 KB (1872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e58c31f850be84c6af0b0a6110b43a6541e2866463803132254f3a9fe3d934a7`  
		Last Modified: Tue, 23 May 2023 01:11:38 GMT  
		Size: 1.5 KB (1476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3e8c00c90d7ae0b153ebfdc785a5a8a92eb1b7c2f784dd565dc5a72d95e9405`  
		Last Modified: Tue, 23 May 2023 01:11:38 GMT  
		Size: 1.4 MB (1385350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27dade8d0c809034087f2b30ac15a8b8c57d45108d908e8d1cb020afb23eae9a`  
		Last Modified: Tue, 23 May 2023 01:11:38 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1-fastcgi` - linux; arm variant v7

```console
$ docker pull adminer@sha256:11ec19aff2d26fc95a54fd3df142b2150c3a377c2d75480bf89b34bb1959dcf0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.8 MB (87793463 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c9707286206384175f44f5f53306cea1139c30c01a275936f88f3677f591726`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Mon, 12 Jun 2023 23:58:34 GMT
ADD file:6edc8f94d2ebc83d6081e1c4567963d0060a842c767eaff959a6e5c6d09247b5 in / 
# Mon, 12 Jun 2023 23:58:34 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 04:50:43 GMT
STOPSIGNAL SIGINT
# Tue, 13 Jun 2023 04:51:12 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 04:51:12 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 13 Jun 2023 04:51:52 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Tue, 13 Jun 2023 04:51:53 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 13 Jun 2023 04:51:53 GMT
WORKDIR /var/www/html
# Tue, 13 Jun 2023 04:51:53 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 13 Jun 2023 04:51:53 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 13 Jun 2023 04:51:53 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 13 Jun 2023 04:51:54 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 13 Jun 2023 04:52:04 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Jun 2023 04:52:04 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 13 Jun 2023 04:52:05 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 13 Jun 2023 04:52:05 GMT
USER adminer
# Tue, 13 Jun 2023 04:52:05 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:23807bbf2a5fd14b7975a9e82f4a5530bbba520f31b382cc4b4ce2e77e075ace`  
		Last Modified: Tue, 13 Jun 2023 00:04:02 GMT  
		Size: 50.2 MB (50218141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed9435d7956e105f98b0ce0d774c24da59c523bdcf4ec8fff644876978300c69`  
		Last Modified: Tue, 13 Jun 2023 04:52:24 GMT  
		Size: 36.2 MB (36183011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbf6d7965eb59f39902f271310a767cdf68bdc38bf15c4ee7bc3cfc5c2d025f8`  
		Last Modified: Tue, 13 Jun 2023 04:52:16 GMT  
		Size: 392.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:916d17fb0f8882d23121f554813421100e94760e2e0cdaf751935eaa1a19ab46`  
		Last Modified: Tue, 13 Jun 2023 04:52:39 GMT  
		Size: 2.7 KB (2713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb697d34af45737a34d3f2956db7be64dda1aea6ed409568e658cb341633ede7`  
		Last Modified: Tue, 13 Jun 2023 04:52:39 GMT  
		Size: 1.9 KB (1863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8ada7f7a7eb464a51e2dae5756d43b13a9d97ee91354ed06525718c56c80881`  
		Last Modified: Tue, 13 Jun 2023 04:52:39 GMT  
		Size: 1.5 KB (1476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdce229253f3ee410f2b1f7535a88835f7283d187bb2e8038132fc61d5705691`  
		Last Modified: Tue, 13 Jun 2023 04:52:40 GMT  
		Size: 1.4 MB (1385378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eee6f724498f44554404d3f27bfb20c948b0c3644918c575d594ad887ecb2a31`  
		Last Modified: Tue, 13 Jun 2023 04:52:39 GMT  
		Size: 489.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1-fastcgi` - linux; arm64 variant v8

```console
$ docker pull adminer@sha256:3dd032bfdb7eb723810a29735b8e01eb4466194e6c2843355eb9a4d70243f534
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.3 MB (94339383 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d48c97b1d9e6d66f743a4b29f2deada7524b544850c7671e594390b07d8c02f4`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:22 GMT
ADD file:caddd2f40296ec5c1bf7487617ca8694cfff9a1d9b7484159e203b6514cb5f5f in / 
# Mon, 12 Jun 2023 23:40:23 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 04:45:49 GMT
STOPSIGNAL SIGINT
# Tue, 13 Jun 2023 04:46:10 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 04:46:11 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 13 Jun 2023 04:46:30 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Tue, 13 Jun 2023 04:46:30 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 13 Jun 2023 04:46:30 GMT
WORKDIR /var/www/html
# Tue, 13 Jun 2023 04:46:31 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 13 Jun 2023 04:46:31 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 13 Jun 2023 04:46:31 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 13 Jun 2023 04:46:31 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 13 Jun 2023 04:46:40 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Jun 2023 04:46:40 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 13 Jun 2023 04:46:41 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 13 Jun 2023 04:46:41 GMT
USER adminer
# Tue, 13 Jun 2023 04:46:41 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:663ccfaf62a5d7b997bca03d1dc6d5dfff01b9e0de08d86dbea8957ea92d7d16`  
		Last Modified: Mon, 12 Jun 2023 23:44:25 GMT  
		Size: 53.7 MB (53704136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80aa39d9a9c198e71855c642bc21b287cd96a68f1ca6f6095933aebd07835b55`  
		Last Modified: Tue, 13 Jun 2023 04:46:57 GMT  
		Size: 39.2 MB (39243014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35aba8c7c961932b274149a03d0e4ded7ce7529e514d523d33c6c6972b149b3d`  
		Last Modified: Tue, 13 Jun 2023 04:46:50 GMT  
		Size: 393.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2162693a46ec477e8b49e0b80d0001f2eda79016865c9dc2158bb2ef09e7f9b`  
		Last Modified: Tue, 13 Jun 2023 04:47:13 GMT  
		Size: 2.7 KB (2714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:050d9afd2370b260f1761c086dbd5b74588dd70e17c533745afae53f5c1418f8`  
		Last Modified: Tue, 13 Jun 2023 04:47:13 GMT  
		Size: 1.9 KB (1876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:194f7cc3086811f97e24a54110a1ab966bcd8e3ff0c53f3bc2dd92d1e1186375`  
		Last Modified: Tue, 13 Jun 2023 04:47:13 GMT  
		Size: 1.5 KB (1475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f69e51ee2ca7c113fff7852d477f2060974ccb554779d3252647aa566bb161a4`  
		Last Modified: Tue, 13 Jun 2023 04:47:14 GMT  
		Size: 1.4 MB (1385287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44aea086a6384d7d2bd997d4c3c0d0b5344e0d91e9ca0128c0daaebb6f65bd9c`  
		Last Modified: Tue, 13 Jun 2023 04:47:13 GMT  
		Size: 488.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1-fastcgi` - linux; 386

```console
$ docker pull adminer@sha256:b4aec10e1691950dfa2dc0805c974f93383bb86817b1dfeb8e31a7302fca7740
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.0 MB (96991518 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f2428d60bf69f5e123fd00c3307326cf15efc62cdfbe175764ff4f431296a3ea`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Mon, 12 Jun 2023 23:39:39 GMT
ADD file:4b1f447e0b75fbe493bd68bb77b74f4ba1c61ac8e14226e3c511b3a1c3d5721a in / 
# Mon, 12 Jun 2023 23:39:40 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 00:59:39 GMT
STOPSIGNAL SIGINT
# Tue, 13 Jun 2023 01:00:06 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 01:00:07 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 13 Jun 2023 01:00:28 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Tue, 13 Jun 2023 01:00:28 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 13 Jun 2023 01:00:28 GMT
WORKDIR /var/www/html
# Tue, 13 Jun 2023 01:00:29 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 13 Jun 2023 01:00:29 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 13 Jun 2023 01:00:29 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 13 Jun 2023 01:00:29 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 13 Jun 2023 01:00:41 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Jun 2023 01:00:41 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 13 Jun 2023 01:00:41 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 13 Jun 2023 01:00:41 GMT
USER adminer
# Tue, 13 Jun 2023 01:00:41 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:0997ae72d27731326552ad4699d630b4932f3d31abc07a62105a0eb16b54173a`  
		Last Modified: Mon, 12 Jun 2023 23:46:43 GMT  
		Size: 56.0 MB (56040665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dac97babbe48fc6ee5134482bf3dd02a0763c71618911c97beab64bec3147a8`  
		Last Modified: Tue, 13 Jun 2023 01:01:02 GMT  
		Size: 39.6 MB (39558608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df44f63ded7015da79f717c9dbf6dfd057bcafc06012bc1e415f53113e6fc1e5`  
		Last Modified: Tue, 13 Jun 2023 01:00:51 GMT  
		Size: 389.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8cfabfd56ee8b764abdf6f8cb20c091bea2ffae807bf04792799aa0ed635fb2`  
		Last Modified: Tue, 13 Jun 2023 01:01:18 GMT  
		Size: 2.7 KB (2708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:863747f21248ccdd5a53cf90d3ec3352b8cb75e1399bc41cdb2718127f287dd8`  
		Last Modified: Tue, 13 Jun 2023 01:01:18 GMT  
		Size: 1.9 KB (1863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee87568b44fcbd69476382c97061b27d53cae0b400d370e9825d16d684d27fa9`  
		Last Modified: Tue, 13 Jun 2023 01:01:18 GMT  
		Size: 1.5 KB (1476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b813c8ca03ebf5bac2b11cbbea4a8c154671aed01beacf714dd7337ac69228bc`  
		Last Modified: Tue, 13 Jun 2023 01:01:19 GMT  
		Size: 1.4 MB (1385320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3bf942bd785c5bd0709d7397f37a7b4de4e4359f2e16602e948dd4aeaaec333`  
		Last Modified: Tue, 13 Jun 2023 01:01:18 GMT  
		Size: 489.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1-fastcgi` - linux; mips64le

```console
$ docker pull adminer@sha256:7c0ad002201eb7dba5d626c2e579249040821e733ac15405eac08b37f6819e18
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.6 MB (92616828 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e14b2773cb94782f55002ad5736b49d8d1715c22f62f831629a2edae0af93bc6`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Tue, 13 Jun 2023 00:09:46 GMT
ADD file:7ba4829e0a582c8a2e5a1d362ca30cfba3fa2911594faf9598927255100965b0 in / 
# Tue, 13 Jun 2023 00:09:51 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 01:46:11 GMT
STOPSIGNAL SIGINT
# Tue, 13 Jun 2023 01:48:01 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 01:48:08 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 13 Jun 2023 01:49:58 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Tue, 13 Jun 2023 01:50:04 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 13 Jun 2023 01:50:07 GMT
WORKDIR /var/www/html
# Tue, 13 Jun 2023 01:50:10 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 13 Jun 2023 01:50:14 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 13 Jun 2023 01:50:17 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 13 Jun 2023 01:50:20 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 13 Jun 2023 01:51:08 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Jun 2023 01:51:11 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 13 Jun 2023 01:51:14 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 13 Jun 2023 01:51:18 GMT
USER adminer
# Tue, 13 Jun 2023 01:51:21 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:ec034d426521af0a9addba08124f06b364f3364fd20ec9aec4e3364104a793d1`  
		Last Modified: Tue, 13 Jun 2023 00:23:13 GMT  
		Size: 53.3 MB (53270410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:901a0f1a33bd58f6d5e7b1de7a90c5fbe79c192cbbabfd8c7a98214496b73c1b`  
		Last Modified: Tue, 13 Jun 2023 01:52:11 GMT  
		Size: 38.0 MB (37953313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c616df06cfce4fa5e3f76b4147041f55275dd885295b9a2e1b9884f710f5a63`  
		Last Modified: Tue, 13 Jun 2023 01:51:45 GMT  
		Size: 395.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68463d39b900d79d99d0b981ac4de2e7b97ed79424dbbab27775b457b526f553`  
		Last Modified: Tue, 13 Jun 2023 01:52:30 GMT  
		Size: 2.7 KB (2711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecf4c4f53ea5745d056c4cf51430f6362a894011418ab8fc004aab4cac8818e8`  
		Last Modified: Tue, 13 Jun 2023 01:52:30 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:660f7e28cfd4cddb76bc3c880db1190a7a88b2d9b9d93d3e82f5c9b316d3dac5`  
		Last Modified: Tue, 13 Jun 2023 01:52:30 GMT  
		Size: 1.5 KB (1478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17fb5ff54e4d36c97aa5b67854279381fc77880b82436f347c9144327a7ba026`  
		Last Modified: Tue, 13 Jun 2023 01:52:31 GMT  
		Size: 1.4 MB (1386301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1fbe725d5b33c64787888d5b86edbf2d81e345c52311c4d0cd4b5631e8ce365`  
		Last Modified: Tue, 13 Jun 2023 01:52:31 GMT  
		Size: 489.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1-fastcgi` - linux; ppc64le

```console
$ docker pull adminer@sha256:f08c2d2d4f6a743fd667ccd77b6e2ea2b906b925e0f09a35df232f82c4692e65
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.3 MB (101256485 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c3935c8e6ae819dd2093e8de8304a6e11a3aae1550d802ad8af7ed871d3cdb02`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Tue, 23 May 2023 01:17:14 GMT
ADD file:ed39869ee4bb8e1901b71feb9cadfe754e42304e134f2542e516e162ca710ec8 in / 
# Tue, 23 May 2023 01:17:17 GMT
CMD ["bash"]
# Tue, 23 May 2023 01:40:42 GMT
STOPSIGNAL SIGINT
# Tue, 23 May 2023 01:41:54 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 01:41:58 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 23 May 2023 01:42:53 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Tue, 23 May 2023 01:42:56 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 23 May 2023 01:42:56 GMT
WORKDIR /var/www/html
# Tue, 23 May 2023 01:42:57 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 23 May 2023 01:42:57 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 23 May 2023 01:42:58 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 23 May 2023 01:42:58 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 23 May 2023 01:43:32 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 23 May 2023 01:43:33 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 23 May 2023 01:43:34 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 23 May 2023 01:43:35 GMT
USER adminer
# Tue, 23 May 2023 01:43:36 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:f530a46e89ee571046fe19b22f563df6c84a31f6593a1e6ed49dbd16e34145de`  
		Last Modified: Tue, 23 May 2023 01:21:34 GMT  
		Size: 58.9 MB (58923948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b328a5c7e2019a9edf5b5d571d37da0261097706c34bafabd5196936aac3fc1b`  
		Last Modified: Tue, 23 May 2023 01:44:03 GMT  
		Size: 40.9 MB (40939928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b29d269a712c093f32a0be4629a0f17bc22fd6dad4be88d5f0af5ce757d809f`  
		Last Modified: Tue, 23 May 2023 01:43:51 GMT  
		Size: 393.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14b5ab23d41e8f1aea6954e2f0b6047fc125e9406f7c560374fe0316f980197e`  
		Last Modified: Tue, 23 May 2023 01:44:22 GMT  
		Size: 2.7 KB (2714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:977b08266ee6cbb32edd6f84d2a98dc861be41484b1401b545d9b0581c1bd174`  
		Last Modified: Tue, 23 May 2023 01:44:22 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92c78939508c16fc88e03d22beb6d700276d381b5a8262d3ff4658b877bad32a`  
		Last Modified: Tue, 23 May 2023 01:44:22 GMT  
		Size: 1.5 KB (1478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bce4c7c01da83a8e67c7a518b162fed2c676be30cdc2c055b920ee658f243cc`  
		Last Modified: Tue, 23 May 2023 01:44:22 GMT  
		Size: 1.4 MB (1385651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5548d29e362ba040749a780b4f79dc74ada494b0aaccaad9e4fbcd61a4b10c61`  
		Last Modified: Tue, 23 May 2023 01:44:22 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1-fastcgi` - linux; s390x

```console
$ docker pull adminer@sha256:a194086c2f327aa2f518b1bde88023cd5f0d1cc9d8e0438ef5b392d68f1c3c79
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.7 MB (93692849 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5b04e5e9f13ffd3710ed52616df2923026fc40f821ca1f6247ca708b6decac7`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Tue, 23 May 2023 00:42:35 GMT
ADD file:a054112be60c3f2d7811b27cde82bccfd1c2747f29b7611ee68b21cd9f3d3d54 in / 
# Tue, 23 May 2023 00:42:41 GMT
CMD ["bash"]
# Tue, 23 May 2023 02:26:55 GMT
STOPSIGNAL SIGINT
# Tue, 23 May 2023 02:27:12 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 02:27:15 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 23 May 2023 02:27:31 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Tue, 23 May 2023 02:27:31 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 23 May 2023 02:27:31 GMT
WORKDIR /var/www/html
# Tue, 23 May 2023 02:27:31 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 23 May 2023 02:27:31 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 23 May 2023 02:27:32 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 23 May 2023 02:27:32 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 23 May 2023 02:27:39 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 23 May 2023 02:27:39 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 23 May 2023 02:27:39 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 23 May 2023 02:27:40 GMT
USER adminer
# Tue, 23 May 2023 02:27:40 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:44d1d02f91725dd9ae742f7c70add814dc3da3fde438adb01e65e1f8b0eba613`  
		Last Modified: Tue, 23 May 2023 00:45:33 GMT  
		Size: 53.3 MB (53282114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a714865cdf8c711665c7b864ae5f1e6c7100e6079a9d6bb3d8925f6a0cceaff2`  
		Last Modified: Tue, 23 May 2023 02:28:00 GMT  
		Size: 39.0 MB (39018332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a6faa7559a991fd1e86474adae5128141983567ad4587e50e92ce5d32755bbb`  
		Last Modified: Tue, 23 May 2023 02:27:53 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9101661d5aa45e85b42ae59aa229ccb0658ea3ab2507142a937c15393886927b`  
		Last Modified: Tue, 23 May 2023 02:28:10 GMT  
		Size: 2.7 KB (2708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70537aeb5de09054327e77121e9ac1e2c9309cd67388d6c9f3c6a246c0980aa7`  
		Last Modified: Tue, 23 May 2023 02:28:10 GMT  
		Size: 1.9 KB (1883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42f4125a64e5befb7b5b1dfe94aa43aa55cb192155eb38a12a6d86a3bf660210`  
		Last Modified: Tue, 23 May 2023 02:28:10 GMT  
		Size: 1.5 KB (1477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d338cb5258e7079119cbfe96033d5b49ee9e23aeb5860c5ffd0c1a8bb4342bcf`  
		Last Modified: Tue, 23 May 2023 02:28:11 GMT  
		Size: 1.4 MB (1385455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41ca25d71e32f1c6ef50badf5308e74f4afedccd9f322e5c0c4e2a75bc7a092d`  
		Last Modified: Tue, 23 May 2023 02:28:10 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `adminer:4.8.1-standalone`

```console
$ docker pull adminer@sha256:521aae780cec6678443058ecb03e3b20fd815e1c1220dc8370c3a3381acc736c
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
$ docker pull adminer@sha256:203c8ee52640268c28f5ce5f57b192d967da40a91d6443b57ae1da4064e2ed8b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.9 MB (95931867 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e4345c1c3dc89b4c31146abe340fa39e143d922d1e3401233d7ac32db2d985d`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Mon, 12 Jun 2023 23:20:54 GMT
ADD file:e530b0563ea53d97b2f28e62149a665900196f86611df99a88c7a8ab2097b95d in / 
# Mon, 12 Jun 2023 23:20:54 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 03:24:37 GMT
STOPSIGNAL SIGINT
# Tue, 13 Jun 2023 03:25:04 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 03:25:05 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 13 Jun 2023 03:25:06 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 13 Jun 2023 03:25:06 GMT
WORKDIR /var/www/html
# Tue, 13 Jun 2023 03:25:06 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 13 Jun 2023 03:25:06 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 13 Jun 2023 03:25:06 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 13 Jun 2023 03:25:06 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 13 Jun 2023 03:25:19 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Jun 2023 03:25:19 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 13 Jun 2023 03:25:19 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 13 Jun 2023 03:25:19 GMT
USER adminer
# Tue, 13 Jun 2023 03:25:19 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Tue, 13 Jun 2023 03:25:19 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:93c2d578e4211e82e47e7ada9ed05d1869a2362c6f7509f2ee8d91ccebfb7fbd`  
		Last Modified: Mon, 12 Jun 2023 23:26:08 GMT  
		Size: 55.1 MB (55055162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e099cf7ea37ba8ff2169a70f6743bf40675a661f0dc9b6a8abaa4e43050979c`  
		Last Modified: Tue, 13 Jun 2023 03:25:56 GMT  
		Size: 39.5 MB (39487054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d12c699384cbfa0b30a07efef5ad3b7f104e0e1f33e6a094e489150e4ef3838`  
		Last Modified: Tue, 13 Jun 2023 03:25:48 GMT  
		Size: 391.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05c66113a52b479d99efec54808f4045c5fe1400714639a6c750317ad501bc9c`  
		Last Modified: Tue, 13 Jun 2023 03:25:48 GMT  
		Size: 1.9 KB (1874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:677df7ad2be6c1e9f14d49043358dc765759c7f2cd0184ca55a55dc81dcb2263`  
		Last Modified: Tue, 13 Jun 2023 03:25:48 GMT  
		Size: 1.5 KB (1478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:598f6ab1ce2900168e83fbb661f1edc77e27dd8261b23a1f22af28e991facd6e`  
		Last Modified: Tue, 13 Jun 2023 03:25:49 GMT  
		Size: 1.4 MB (1385416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41ed709cb4bc1b53001ba47d24d74fb415c6142dd35194346fdac370144df45a`  
		Last Modified: Tue, 13 Jun 2023 03:25:48 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1-standalone` - linux; arm variant v5

```console
$ docker pull adminer@sha256:15bb2436532d59fdbf58c3cbc74f61d47be5ad45e30d65bc01adcfc449dd0951
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.2 MB (91183934 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:267345bcacc239fd7427ea82c255b704e164984dbff20209a9e8439820a662d3`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Tue, 23 May 2023 00:48:32 GMT
ADD file:9572a8fcb9c86e8a9dbfe623c732cc4ba1c4f5670490191a7e639a272d5b6e97 in / 
# Tue, 23 May 2023 00:48:33 GMT
CMD ["bash"]
# Tue, 23 May 2023 01:09:52 GMT
STOPSIGNAL SIGINT
# Tue, 23 May 2023 01:10:29 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 01:10:30 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 23 May 2023 01:10:31 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 23 May 2023 01:10:31 GMT
WORKDIR /var/www/html
# Tue, 23 May 2023 01:10:31 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 23 May 2023 01:10:31 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 23 May 2023 01:10:31 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 23 May 2023 01:10:31 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 23 May 2023 01:10:46 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 23 May 2023 01:10:46 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 23 May 2023 01:10:46 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 23 May 2023 01:10:46 GMT
USER adminer
# Tue, 23 May 2023 01:10:46 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Tue, 23 May 2023 01:10:46 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:b053976742ca5b01bcefb7df8fc77a58d0becb4ce508792491574463930569c4`  
		Last Modified: Tue, 23 May 2023 00:50:55 GMT  
		Size: 52.5 MB (52546536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6448799a9363993edd93e5fb6040955191b829140af65c88550e510326878903`  
		Last Modified: Tue, 23 May 2023 01:11:21 GMT  
		Size: 37.2 MB (37247839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b03dc69db3dc4061f823e5e9025874ab539e706b64af3b103bf2a3e839890b8`  
		Last Modified: Tue, 23 May 2023 01:11:13 GMT  
		Size: 388.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ed315aa6041fcfd6bafc18c55ef5be23f10e057e9f941675330807b39d1e54a`  
		Last Modified: Tue, 23 May 2023 01:11:13 GMT  
		Size: 1.9 KB (1872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2d328016feebec5e083e36300e6444d56a5aedfba59d4be438549c64ebcb44f`  
		Last Modified: Tue, 23 May 2023 01:11:13 GMT  
		Size: 1.5 KB (1480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c98954d02c72cf9c2513f055817ac1435ded02424a3418c8d3b9164746bdf3c`  
		Last Modified: Tue, 23 May 2023 01:11:13 GMT  
		Size: 1.4 MB (1385327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aac95e0f74f942d3cfb111cf9949811151a49733af863c919807b2dcbb3a85a1`  
		Last Modified: Tue, 23 May 2023 01:11:13 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1-standalone` - linux; arm variant v7

```console
$ docker pull adminer@sha256:98b76b0878cf9cc2684e5bbbdade79a5f2f6f269e230203870a1f1a752f7e7f1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.8 MB (87790748 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b51c4364b99328a719594799d5c3d616aeb43a95308f9cd320cb70d27dda4c17`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Mon, 12 Jun 2023 23:58:34 GMT
ADD file:6edc8f94d2ebc83d6081e1c4567963d0060a842c767eaff959a6e5c6d09247b5 in / 
# Mon, 12 Jun 2023 23:58:34 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 04:50:43 GMT
STOPSIGNAL SIGINT
# Tue, 13 Jun 2023 04:51:12 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 04:51:12 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 13 Jun 2023 04:51:13 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 13 Jun 2023 04:51:13 GMT
WORKDIR /var/www/html
# Tue, 13 Jun 2023 04:51:13 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 13 Jun 2023 04:51:13 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 13 Jun 2023 04:51:13 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 13 Jun 2023 04:51:13 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 13 Jun 2023 04:51:41 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Jun 2023 04:51:41 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 13 Jun 2023 04:51:41 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 13 Jun 2023 04:51:41 GMT
USER adminer
# Tue, 13 Jun 2023 04:51:42 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Tue, 13 Jun 2023 04:51:42 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:23807bbf2a5fd14b7975a9e82f4a5530bbba520f31b382cc4b4ce2e77e075ace`  
		Last Modified: Tue, 13 Jun 2023 00:04:02 GMT  
		Size: 50.2 MB (50218141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed9435d7956e105f98b0ce0d774c24da59c523bdcf4ec8fff644876978300c69`  
		Last Modified: Tue, 13 Jun 2023 04:52:24 GMT  
		Size: 36.2 MB (36183011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbf6d7965eb59f39902f271310a767cdf68bdc38bf15c4ee7bc3cfc5c2d025f8`  
		Last Modified: Tue, 13 Jun 2023 04:52:16 GMT  
		Size: 392.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da256b5543040f6999ae9a8cc020bfd0542286ecf71c77feb6cd08a4ecd9be37`  
		Last Modified: Tue, 13 Jun 2023 04:52:16 GMT  
		Size: 1.9 KB (1863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fac8d202305e7ac73502fb63bb1618ac53766c99e8cd03bcb0412c313a25dd83`  
		Last Modified: Tue, 13 Jun 2023 04:52:16 GMT  
		Size: 1.5 KB (1479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b96b3d518c63ab16389a582e075ae88f7225f3c35483203c7c52dcfa52f2daa5`  
		Last Modified: Tue, 13 Jun 2023 04:52:16 GMT  
		Size: 1.4 MB (1385372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eb5818f5b2f148baf53286364c0c6cd2df86e21ed76bfcbc6ff0688a5d2726c`  
		Last Modified: Tue, 13 Jun 2023 04:52:16 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1-standalone` - linux; arm64 variant v8

```console
$ docker pull adminer@sha256:92cdfd552b3557e293045fc3d5f01d58871958912197649f3c818e312856bf85
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.3 MB (94336689 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b7e1c530248708005dc78825e6702d078b51bbd4eae6c82b2df135ce82d2961`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:22 GMT
ADD file:caddd2f40296ec5c1bf7487617ca8694cfff9a1d9b7484159e203b6514cb5f5f in / 
# Mon, 12 Jun 2023 23:40:23 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 04:45:49 GMT
STOPSIGNAL SIGINT
# Tue, 13 Jun 2023 04:46:10 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 04:46:11 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 13 Jun 2023 04:46:12 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 13 Jun 2023 04:46:12 GMT
WORKDIR /var/www/html
# Tue, 13 Jun 2023 04:46:12 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 13 Jun 2023 04:46:12 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 13 Jun 2023 04:46:12 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 13 Jun 2023 04:46:12 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 13 Jun 2023 04:46:22 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Jun 2023 04:46:22 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 13 Jun 2023 04:46:22 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 13 Jun 2023 04:46:22 GMT
USER adminer
# Tue, 13 Jun 2023 04:46:22 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Tue, 13 Jun 2023 04:46:23 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:663ccfaf62a5d7b997bca03d1dc6d5dfff01b9e0de08d86dbea8957ea92d7d16`  
		Last Modified: Mon, 12 Jun 2023 23:44:25 GMT  
		Size: 53.7 MB (53704136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80aa39d9a9c198e71855c642bc21b287cd96a68f1ca6f6095933aebd07835b55`  
		Last Modified: Tue, 13 Jun 2023 04:46:57 GMT  
		Size: 39.2 MB (39243014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35aba8c7c961932b274149a03d0e4ded7ce7529e514d523d33c6c6972b149b3d`  
		Last Modified: Tue, 13 Jun 2023 04:46:50 GMT  
		Size: 393.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe596da7a5da4c53bb7e8a57c4bca7d95147969f3fcfa27a9ac63992faacad68`  
		Last Modified: Tue, 13 Jun 2023 04:46:51 GMT  
		Size: 1.9 KB (1875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9f19157c079ccd39ddc0b6c916dec64e367d7b29ff37f7d51348654868ffeea`  
		Last Modified: Tue, 13 Jun 2023 04:46:51 GMT  
		Size: 1.5 KB (1482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e9f6bc36eded234b1a9ca40497b6b08e4a5ebd85b8077cfd4951499ef134c78`  
		Last Modified: Tue, 13 Jun 2023 04:46:51 GMT  
		Size: 1.4 MB (1385300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4689e75de5a00a90b25e2ae66464fad25ea65b849b83d549503bdfb11f72be63`  
		Last Modified: Tue, 13 Jun 2023 04:46:51 GMT  
		Size: 489.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1-standalone` - linux; 386

```console
$ docker pull adminer@sha256:e0bb773bce27da86e8bba771ce6fb58fef553b675ea0e0e2c7eaa0d2bd7dd9f9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.0 MB (96988803 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77720ee3233be6352493a8d99e983f977b3e182750f1526bba6d67134b1bf7ee`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Mon, 12 Jun 2023 23:39:39 GMT
ADD file:4b1f447e0b75fbe493bd68bb77b74f4ba1c61ac8e14226e3c511b3a1c3d5721a in / 
# Mon, 12 Jun 2023 23:39:40 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 00:59:39 GMT
STOPSIGNAL SIGINT
# Tue, 13 Jun 2023 01:00:06 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 01:00:07 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 13 Jun 2023 01:00:07 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 13 Jun 2023 01:00:08 GMT
WORKDIR /var/www/html
# Tue, 13 Jun 2023 01:00:08 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 13 Jun 2023 01:00:08 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 13 Jun 2023 01:00:08 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 13 Jun 2023 01:00:08 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 13 Jun 2023 01:00:20 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Jun 2023 01:00:20 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 13 Jun 2023 01:00:20 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 13 Jun 2023 01:00:21 GMT
USER adminer
# Tue, 13 Jun 2023 01:00:21 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Tue, 13 Jun 2023 01:00:21 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:0997ae72d27731326552ad4699d630b4932f3d31abc07a62105a0eb16b54173a`  
		Last Modified: Mon, 12 Jun 2023 23:46:43 GMT  
		Size: 56.0 MB (56040665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dac97babbe48fc6ee5134482bf3dd02a0763c71618911c97beab64bec3147a8`  
		Last Modified: Tue, 13 Jun 2023 01:01:02 GMT  
		Size: 39.6 MB (39558608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df44f63ded7015da79f717c9dbf6dfd057bcafc06012bc1e415f53113e6fc1e5`  
		Last Modified: Tue, 13 Jun 2023 01:00:51 GMT  
		Size: 389.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ae3ce4c7547485956e0bd1180cc66032006af3b33c6ae582d77834096391752`  
		Last Modified: Tue, 13 Jun 2023 01:00:51 GMT  
		Size: 1.9 KB (1864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83417b3fe0dbbaed7076986fd209d6704b096ecd961a111cfb42cba80a11dc93`  
		Last Modified: Tue, 13 Jun 2023 01:00:51 GMT  
		Size: 1.5 KB (1480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbdb97551a1780228aac70017b847d497ec088d6ad3e46d5c8b9b48083efe5a0`  
		Last Modified: Tue, 13 Jun 2023 01:00:52 GMT  
		Size: 1.4 MB (1385307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbef3e3e2b3156ba5eca052ebf766f2f4474f980905836f0c0ea9eec319f7a6e`  
		Last Modified: Tue, 13 Jun 2023 01:00:51 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1-standalone` - linux; mips64le

```console
$ docker pull adminer@sha256:2591b1f0dffbc4f123a4a3bd12c1cb46669c54383e8e23e13c83edaecc2541d1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.6 MB (92614104 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9a417a537dc4187139ad39c01263d6bd8b79a728bf005ad51d3bb4d42ec1d5f`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Tue, 13 Jun 2023 00:09:46 GMT
ADD file:7ba4829e0a582c8a2e5a1d362ca30cfba3fa2911594faf9598927255100965b0 in / 
# Tue, 13 Jun 2023 00:09:51 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 01:46:11 GMT
STOPSIGNAL SIGINT
# Tue, 13 Jun 2023 01:48:01 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 01:48:08 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 13 Jun 2023 01:48:14 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 13 Jun 2023 01:48:18 GMT
WORKDIR /var/www/html
# Tue, 13 Jun 2023 01:48:21 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 13 Jun 2023 01:48:24 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 13 Jun 2023 01:48:28 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 13 Jun 2023 01:48:31 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 13 Jun 2023 01:49:21 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Jun 2023 01:49:24 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 13 Jun 2023 01:49:27 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 13 Jun 2023 01:49:31 GMT
USER adminer
# Tue, 13 Jun 2023 01:49:34 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Tue, 13 Jun 2023 01:49:37 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:ec034d426521af0a9addba08124f06b364f3364fd20ec9aec4e3364104a793d1`  
		Last Modified: Tue, 13 Jun 2023 00:23:13 GMT  
		Size: 53.3 MB (53270410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:901a0f1a33bd58f6d5e7b1de7a90c5fbe79c192cbbabfd8c7a98214496b73c1b`  
		Last Modified: Tue, 13 Jun 2023 01:52:11 GMT  
		Size: 38.0 MB (37953313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c616df06cfce4fa5e3f76b4147041f55275dd885295b9a2e1b9884f710f5a63`  
		Last Modified: Tue, 13 Jun 2023 01:51:45 GMT  
		Size: 395.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84487562d4b36a6a1112b198b725b1a727e91a77be9899c0d74b1a4a9c022dba`  
		Last Modified: Tue, 13 Jun 2023 01:51:45 GMT  
		Size: 1.7 KB (1723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5dde6303cb52a3de95ebac876b6f8590487f4ffa08f8c0e80844f4d89b75072`  
		Last Modified: Tue, 13 Jun 2023 01:51:45 GMT  
		Size: 1.5 KB (1480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:499702681379ddde7be8cc76c78d9b9c764ceea9af16c336da3a99169971feb1`  
		Last Modified: Tue, 13 Jun 2023 01:51:46 GMT  
		Size: 1.4 MB (1386295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63d75b2d63e14c568323dc0897c171f4d71efe33d94bb1423a59c555514d35ae`  
		Last Modified: Tue, 13 Jun 2023 01:51:45 GMT  
		Size: 488.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1-standalone` - linux; ppc64le

```console
$ docker pull adminer@sha256:e0a0e907c5c635e5e363e08b1dffd85143970ad1e4dee8cd2acdbd2c47f59f30
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.3 MB (101253778 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0759ab5b0827c3e5903a54d9e690f3911052bcece85af789658d87469a6c4e41`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Tue, 23 May 2023 01:17:14 GMT
ADD file:ed39869ee4bb8e1901b71feb9cadfe754e42304e134f2542e516e162ca710ec8 in / 
# Tue, 23 May 2023 01:17:17 GMT
CMD ["bash"]
# Tue, 23 May 2023 01:40:42 GMT
STOPSIGNAL SIGINT
# Tue, 23 May 2023 01:41:54 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 01:41:58 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 23 May 2023 01:42:00 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 23 May 2023 01:42:01 GMT
WORKDIR /var/www/html
# Tue, 23 May 2023 01:42:01 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 23 May 2023 01:42:02 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 23 May 2023 01:42:02 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 23 May 2023 01:42:02 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 23 May 2023 01:42:36 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 23 May 2023 01:42:37 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 23 May 2023 01:42:37 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 23 May 2023 01:42:38 GMT
USER adminer
# Tue, 23 May 2023 01:42:39 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Tue, 23 May 2023 01:42:40 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:f530a46e89ee571046fe19b22f563df6c84a31f6593a1e6ed49dbd16e34145de`  
		Last Modified: Tue, 23 May 2023 01:21:34 GMT  
		Size: 58.9 MB (58923948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b328a5c7e2019a9edf5b5d571d37da0261097706c34bafabd5196936aac3fc1b`  
		Last Modified: Tue, 23 May 2023 01:44:03 GMT  
		Size: 40.9 MB (40939928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b29d269a712c093f32a0be4629a0f17bc22fd6dad4be88d5f0af5ce757d809f`  
		Last Modified: Tue, 23 May 2023 01:43:51 GMT  
		Size: 393.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:904564df90e41e35afa3221ab3277e3aa554b7c686393785c1b07372bc0c4d4d`  
		Last Modified: Tue, 23 May 2023 01:43:51 GMT  
		Size: 1.9 KB (1880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55a789415d78b4a3befd6b003659799bcf3d20cb06639a961c96a980640e8991`  
		Last Modified: Tue, 23 May 2023 01:43:51 GMT  
		Size: 1.5 KB (1479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78c991997ea0a176dc01a5a08f6ac61143299aef87572cd7e8578e479aae772b`  
		Last Modified: Tue, 23 May 2023 01:43:52 GMT  
		Size: 1.4 MB (1385657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd039d869a125163f2302899c7b0fcf2db140dad2eecedc648b3ca229cb86460`  
		Last Modified: Tue, 23 May 2023 01:43:51 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1-standalone` - linux; s390x

```console
$ docker pull adminer@sha256:b48c2c7360476d0f6ce0723abeef59ed2cc19493ffedd144d64ee2b5d0a21683
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.7 MB (93690153 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:008c852f84add504c1031fabd62a8ede6758604b42d91789507acf3c08df5507`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Tue, 23 May 2023 00:42:35 GMT
ADD file:a054112be60c3f2d7811b27cde82bccfd1c2747f29b7611ee68b21cd9f3d3d54 in / 
# Tue, 23 May 2023 00:42:41 GMT
CMD ["bash"]
# Tue, 23 May 2023 02:26:55 GMT
STOPSIGNAL SIGINT
# Tue, 23 May 2023 02:27:12 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 02:27:15 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 23 May 2023 02:27:15 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 23 May 2023 02:27:15 GMT
WORKDIR /var/www/html
# Tue, 23 May 2023 02:27:15 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 23 May 2023 02:27:15 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 23 May 2023 02:27:16 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 23 May 2023 02:27:16 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 23 May 2023 02:27:23 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 23 May 2023 02:27:23 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 23 May 2023 02:27:23 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 23 May 2023 02:27:24 GMT
USER adminer
# Tue, 23 May 2023 02:27:24 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Tue, 23 May 2023 02:27:24 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:44d1d02f91725dd9ae742f7c70add814dc3da3fde438adb01e65e1f8b0eba613`  
		Last Modified: Tue, 23 May 2023 00:45:33 GMT  
		Size: 53.3 MB (53282114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a714865cdf8c711665c7b864ae5f1e6c7100e6079a9d6bb3d8925f6a0cceaff2`  
		Last Modified: Tue, 23 May 2023 02:28:00 GMT  
		Size: 39.0 MB (39018332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a6faa7559a991fd1e86474adae5128141983567ad4587e50e92ce5d32755bbb`  
		Last Modified: Tue, 23 May 2023 02:27:53 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f55cc440fda23758bbfb18b1a3881ac61d06ad9e0a4b35da688b713c1b8611be`  
		Last Modified: Tue, 23 May 2023 02:27:53 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d16d617d4904a95242ab9db1204e6fa0d844358dc62528fed7ad368f57b1251d`  
		Last Modified: Tue, 23 May 2023 02:27:53 GMT  
		Size: 1.5 KB (1478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c753b23f0be5c140b7bed93c7220f68e38f138d53d3e7e9aade64a9d4b45038e`  
		Last Modified: Tue, 23 May 2023 02:27:53 GMT  
		Size: 1.4 MB (1385466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a436f3a56433ffbdc8b5e6a7bda069a68625447867738966931d19c9db78365c`  
		Last Modified: Tue, 23 May 2023 02:27:53 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `adminer:fastcgi`

```console
$ docker pull adminer@sha256:f67d780396297178e7b0d659328093579772caa59834ea077b2d00edc2b2d3c3
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
$ docker pull adminer@sha256:19e342979ee9fe7dbce42adf4070530e4fab8743bc177b4b401efc984ab1e40b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.9 MB (95934602 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:452a956cc7253ee0c04d3736127b355e67a5cd14dda7c0aaf0c2d18ab50277f1`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Mon, 12 Jun 2023 23:20:54 GMT
ADD file:e530b0563ea53d97b2f28e62149a665900196f86611df99a88c7a8ab2097b95d in / 
# Mon, 12 Jun 2023 23:20:54 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 03:24:37 GMT
STOPSIGNAL SIGINT
# Tue, 13 Jun 2023 03:25:04 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 03:25:05 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 13 Jun 2023 03:25:26 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Tue, 13 Jun 2023 03:25:26 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 13 Jun 2023 03:25:26 GMT
WORKDIR /var/www/html
# Tue, 13 Jun 2023 03:25:26 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 13 Jun 2023 03:25:26 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 13 Jun 2023 03:25:26 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 13 Jun 2023 03:25:27 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 13 Jun 2023 03:25:37 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Jun 2023 03:25:37 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 13 Jun 2023 03:25:37 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 13 Jun 2023 03:25:37 GMT
USER adminer
# Tue, 13 Jun 2023 03:25:38 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:93c2d578e4211e82e47e7ada9ed05d1869a2362c6f7509f2ee8d91ccebfb7fbd`  
		Last Modified: Mon, 12 Jun 2023 23:26:08 GMT  
		Size: 55.1 MB (55055162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e099cf7ea37ba8ff2169a70f6743bf40675a661f0dc9b6a8abaa4e43050979c`  
		Last Modified: Tue, 13 Jun 2023 03:25:56 GMT  
		Size: 39.5 MB (39487054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d12c699384cbfa0b30a07efef5ad3b7f104e0e1f33e6a094e489150e4ef3838`  
		Last Modified: Tue, 13 Jun 2023 03:25:48 GMT  
		Size: 391.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a83e8c3036470b387287b92b025e756b2d38926bd08a60b788905721b2710970`  
		Last Modified: Tue, 13 Jun 2023 03:26:11 GMT  
		Size: 2.7 KB (2706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4474445ef61d8bccb5f84a0c1af50393a4283332687b853db43b67b7c8ea97ac`  
		Last Modified: Tue, 13 Jun 2023 03:26:11 GMT  
		Size: 1.9 KB (1869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9d7d23c4974a9d08d6b18826eb53254571cb1eae70efa61ee681248a11cdcdc`  
		Last Modified: Tue, 13 Jun 2023 03:26:11 GMT  
		Size: 1.5 KB (1475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:420c1637804f967bec0a6f2d1c8e796d18bad5b8a06dadd562b9e930aa597924`  
		Last Modified: Tue, 13 Jun 2023 03:26:11 GMT  
		Size: 1.4 MB (1385457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1963affabab6ca86abab89a12ea096a70efa4ae2aae5c58c80a429a8c88afab2`  
		Last Modified: Tue, 13 Jun 2023 03:26:11 GMT  
		Size: 488.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:fastcgi` - linux; arm variant v5

```console
$ docker pull adminer@sha256:874aa6f218690a93c384b0f19fc246af20d395854f936f59bc3547bacd22ac8d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.2 MB (91186662 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad52da629ff3a29fd1d27c9c82784df59d0303ac68e619208119f622c79f3f32`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Tue, 23 May 2023 00:48:32 GMT
ADD file:9572a8fcb9c86e8a9dbfe623c732cc4ba1c4f5670490191a7e639a272d5b6e97 in / 
# Tue, 23 May 2023 00:48:33 GMT
CMD ["bash"]
# Tue, 23 May 2023 01:09:52 GMT
STOPSIGNAL SIGINT
# Tue, 23 May 2023 01:10:29 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 01:10:30 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 23 May 2023 01:10:49 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Tue, 23 May 2023 01:10:50 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 23 May 2023 01:10:50 GMT
WORKDIR /var/www/html
# Tue, 23 May 2023 01:10:50 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 23 May 2023 01:10:50 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 23 May 2023 01:10:50 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 23 May 2023 01:10:50 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 23 May 2023 01:11:03 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 23 May 2023 01:11:03 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 23 May 2023 01:11:03 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 23 May 2023 01:11:03 GMT
USER adminer
# Tue, 23 May 2023 01:11:04 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:b053976742ca5b01bcefb7df8fc77a58d0becb4ce508792491574463930569c4`  
		Last Modified: Tue, 23 May 2023 00:50:55 GMT  
		Size: 52.5 MB (52546536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6448799a9363993edd93e5fb6040955191b829140af65c88550e510326878903`  
		Last Modified: Tue, 23 May 2023 01:11:21 GMT  
		Size: 37.2 MB (37247839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b03dc69db3dc4061f823e5e9025874ab539e706b64af3b103bf2a3e839890b8`  
		Last Modified: Tue, 23 May 2023 01:11:13 GMT  
		Size: 388.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b485dfbb13977609126b9a2977c8377b44b256b17a3eb1ca752d5dcd2f1c355`  
		Last Modified: Tue, 23 May 2023 01:11:38 GMT  
		Size: 2.7 KB (2710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:468ca8e69b40ea1983b6fcb3612d2309983339ff59fb02fc827a331cfe0ec7e8`  
		Last Modified: Tue, 23 May 2023 01:11:38 GMT  
		Size: 1.9 KB (1872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e58c31f850be84c6af0b0a6110b43a6541e2866463803132254f3a9fe3d934a7`  
		Last Modified: Tue, 23 May 2023 01:11:38 GMT  
		Size: 1.5 KB (1476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3e8c00c90d7ae0b153ebfdc785a5a8a92eb1b7c2f784dd565dc5a72d95e9405`  
		Last Modified: Tue, 23 May 2023 01:11:38 GMT  
		Size: 1.4 MB (1385350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27dade8d0c809034087f2b30ac15a8b8c57d45108d908e8d1cb020afb23eae9a`  
		Last Modified: Tue, 23 May 2023 01:11:38 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:fastcgi` - linux; arm variant v7

```console
$ docker pull adminer@sha256:11ec19aff2d26fc95a54fd3df142b2150c3a377c2d75480bf89b34bb1959dcf0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.8 MB (87793463 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c9707286206384175f44f5f53306cea1139c30c01a275936f88f3677f591726`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Mon, 12 Jun 2023 23:58:34 GMT
ADD file:6edc8f94d2ebc83d6081e1c4567963d0060a842c767eaff959a6e5c6d09247b5 in / 
# Mon, 12 Jun 2023 23:58:34 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 04:50:43 GMT
STOPSIGNAL SIGINT
# Tue, 13 Jun 2023 04:51:12 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 04:51:12 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 13 Jun 2023 04:51:52 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Tue, 13 Jun 2023 04:51:53 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 13 Jun 2023 04:51:53 GMT
WORKDIR /var/www/html
# Tue, 13 Jun 2023 04:51:53 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 13 Jun 2023 04:51:53 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 13 Jun 2023 04:51:53 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 13 Jun 2023 04:51:54 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 13 Jun 2023 04:52:04 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Jun 2023 04:52:04 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 13 Jun 2023 04:52:05 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 13 Jun 2023 04:52:05 GMT
USER adminer
# Tue, 13 Jun 2023 04:52:05 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:23807bbf2a5fd14b7975a9e82f4a5530bbba520f31b382cc4b4ce2e77e075ace`  
		Last Modified: Tue, 13 Jun 2023 00:04:02 GMT  
		Size: 50.2 MB (50218141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed9435d7956e105f98b0ce0d774c24da59c523bdcf4ec8fff644876978300c69`  
		Last Modified: Tue, 13 Jun 2023 04:52:24 GMT  
		Size: 36.2 MB (36183011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbf6d7965eb59f39902f271310a767cdf68bdc38bf15c4ee7bc3cfc5c2d025f8`  
		Last Modified: Tue, 13 Jun 2023 04:52:16 GMT  
		Size: 392.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:916d17fb0f8882d23121f554813421100e94760e2e0cdaf751935eaa1a19ab46`  
		Last Modified: Tue, 13 Jun 2023 04:52:39 GMT  
		Size: 2.7 KB (2713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb697d34af45737a34d3f2956db7be64dda1aea6ed409568e658cb341633ede7`  
		Last Modified: Tue, 13 Jun 2023 04:52:39 GMT  
		Size: 1.9 KB (1863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8ada7f7a7eb464a51e2dae5756d43b13a9d97ee91354ed06525718c56c80881`  
		Last Modified: Tue, 13 Jun 2023 04:52:39 GMT  
		Size: 1.5 KB (1476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdce229253f3ee410f2b1f7535a88835f7283d187bb2e8038132fc61d5705691`  
		Last Modified: Tue, 13 Jun 2023 04:52:40 GMT  
		Size: 1.4 MB (1385378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eee6f724498f44554404d3f27bfb20c948b0c3644918c575d594ad887ecb2a31`  
		Last Modified: Tue, 13 Jun 2023 04:52:39 GMT  
		Size: 489.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:fastcgi` - linux; arm64 variant v8

```console
$ docker pull adminer@sha256:3dd032bfdb7eb723810a29735b8e01eb4466194e6c2843355eb9a4d70243f534
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.3 MB (94339383 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d48c97b1d9e6d66f743a4b29f2deada7524b544850c7671e594390b07d8c02f4`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:22 GMT
ADD file:caddd2f40296ec5c1bf7487617ca8694cfff9a1d9b7484159e203b6514cb5f5f in / 
# Mon, 12 Jun 2023 23:40:23 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 04:45:49 GMT
STOPSIGNAL SIGINT
# Tue, 13 Jun 2023 04:46:10 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 04:46:11 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 13 Jun 2023 04:46:30 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Tue, 13 Jun 2023 04:46:30 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 13 Jun 2023 04:46:30 GMT
WORKDIR /var/www/html
# Tue, 13 Jun 2023 04:46:31 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 13 Jun 2023 04:46:31 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 13 Jun 2023 04:46:31 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 13 Jun 2023 04:46:31 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 13 Jun 2023 04:46:40 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Jun 2023 04:46:40 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 13 Jun 2023 04:46:41 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 13 Jun 2023 04:46:41 GMT
USER adminer
# Tue, 13 Jun 2023 04:46:41 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:663ccfaf62a5d7b997bca03d1dc6d5dfff01b9e0de08d86dbea8957ea92d7d16`  
		Last Modified: Mon, 12 Jun 2023 23:44:25 GMT  
		Size: 53.7 MB (53704136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80aa39d9a9c198e71855c642bc21b287cd96a68f1ca6f6095933aebd07835b55`  
		Last Modified: Tue, 13 Jun 2023 04:46:57 GMT  
		Size: 39.2 MB (39243014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35aba8c7c961932b274149a03d0e4ded7ce7529e514d523d33c6c6972b149b3d`  
		Last Modified: Tue, 13 Jun 2023 04:46:50 GMT  
		Size: 393.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2162693a46ec477e8b49e0b80d0001f2eda79016865c9dc2158bb2ef09e7f9b`  
		Last Modified: Tue, 13 Jun 2023 04:47:13 GMT  
		Size: 2.7 KB (2714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:050d9afd2370b260f1761c086dbd5b74588dd70e17c533745afae53f5c1418f8`  
		Last Modified: Tue, 13 Jun 2023 04:47:13 GMT  
		Size: 1.9 KB (1876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:194f7cc3086811f97e24a54110a1ab966bcd8e3ff0c53f3bc2dd92d1e1186375`  
		Last Modified: Tue, 13 Jun 2023 04:47:13 GMT  
		Size: 1.5 KB (1475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f69e51ee2ca7c113fff7852d477f2060974ccb554779d3252647aa566bb161a4`  
		Last Modified: Tue, 13 Jun 2023 04:47:14 GMT  
		Size: 1.4 MB (1385287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44aea086a6384d7d2bd997d4c3c0d0b5344e0d91e9ca0128c0daaebb6f65bd9c`  
		Last Modified: Tue, 13 Jun 2023 04:47:13 GMT  
		Size: 488.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:fastcgi` - linux; 386

```console
$ docker pull adminer@sha256:b4aec10e1691950dfa2dc0805c974f93383bb86817b1dfeb8e31a7302fca7740
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.0 MB (96991518 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f2428d60bf69f5e123fd00c3307326cf15efc62cdfbe175764ff4f431296a3ea`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Mon, 12 Jun 2023 23:39:39 GMT
ADD file:4b1f447e0b75fbe493bd68bb77b74f4ba1c61ac8e14226e3c511b3a1c3d5721a in / 
# Mon, 12 Jun 2023 23:39:40 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 00:59:39 GMT
STOPSIGNAL SIGINT
# Tue, 13 Jun 2023 01:00:06 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 01:00:07 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 13 Jun 2023 01:00:28 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Tue, 13 Jun 2023 01:00:28 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 13 Jun 2023 01:00:28 GMT
WORKDIR /var/www/html
# Tue, 13 Jun 2023 01:00:29 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 13 Jun 2023 01:00:29 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 13 Jun 2023 01:00:29 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 13 Jun 2023 01:00:29 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 13 Jun 2023 01:00:41 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Jun 2023 01:00:41 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 13 Jun 2023 01:00:41 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 13 Jun 2023 01:00:41 GMT
USER adminer
# Tue, 13 Jun 2023 01:00:41 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:0997ae72d27731326552ad4699d630b4932f3d31abc07a62105a0eb16b54173a`  
		Last Modified: Mon, 12 Jun 2023 23:46:43 GMT  
		Size: 56.0 MB (56040665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dac97babbe48fc6ee5134482bf3dd02a0763c71618911c97beab64bec3147a8`  
		Last Modified: Tue, 13 Jun 2023 01:01:02 GMT  
		Size: 39.6 MB (39558608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df44f63ded7015da79f717c9dbf6dfd057bcafc06012bc1e415f53113e6fc1e5`  
		Last Modified: Tue, 13 Jun 2023 01:00:51 GMT  
		Size: 389.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8cfabfd56ee8b764abdf6f8cb20c091bea2ffae807bf04792799aa0ed635fb2`  
		Last Modified: Tue, 13 Jun 2023 01:01:18 GMT  
		Size: 2.7 KB (2708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:863747f21248ccdd5a53cf90d3ec3352b8cb75e1399bc41cdb2718127f287dd8`  
		Last Modified: Tue, 13 Jun 2023 01:01:18 GMT  
		Size: 1.9 KB (1863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee87568b44fcbd69476382c97061b27d53cae0b400d370e9825d16d684d27fa9`  
		Last Modified: Tue, 13 Jun 2023 01:01:18 GMT  
		Size: 1.5 KB (1476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b813c8ca03ebf5bac2b11cbbea4a8c154671aed01beacf714dd7337ac69228bc`  
		Last Modified: Tue, 13 Jun 2023 01:01:19 GMT  
		Size: 1.4 MB (1385320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3bf942bd785c5bd0709d7397f37a7b4de4e4359f2e16602e948dd4aeaaec333`  
		Last Modified: Tue, 13 Jun 2023 01:01:18 GMT  
		Size: 489.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:fastcgi` - linux; mips64le

```console
$ docker pull adminer@sha256:7c0ad002201eb7dba5d626c2e579249040821e733ac15405eac08b37f6819e18
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.6 MB (92616828 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e14b2773cb94782f55002ad5736b49d8d1715c22f62f831629a2edae0af93bc6`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Tue, 13 Jun 2023 00:09:46 GMT
ADD file:7ba4829e0a582c8a2e5a1d362ca30cfba3fa2911594faf9598927255100965b0 in / 
# Tue, 13 Jun 2023 00:09:51 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 01:46:11 GMT
STOPSIGNAL SIGINT
# Tue, 13 Jun 2023 01:48:01 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 01:48:08 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 13 Jun 2023 01:49:58 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Tue, 13 Jun 2023 01:50:04 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 13 Jun 2023 01:50:07 GMT
WORKDIR /var/www/html
# Tue, 13 Jun 2023 01:50:10 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 13 Jun 2023 01:50:14 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 13 Jun 2023 01:50:17 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 13 Jun 2023 01:50:20 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 13 Jun 2023 01:51:08 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Jun 2023 01:51:11 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 13 Jun 2023 01:51:14 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 13 Jun 2023 01:51:18 GMT
USER adminer
# Tue, 13 Jun 2023 01:51:21 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:ec034d426521af0a9addba08124f06b364f3364fd20ec9aec4e3364104a793d1`  
		Last Modified: Tue, 13 Jun 2023 00:23:13 GMT  
		Size: 53.3 MB (53270410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:901a0f1a33bd58f6d5e7b1de7a90c5fbe79c192cbbabfd8c7a98214496b73c1b`  
		Last Modified: Tue, 13 Jun 2023 01:52:11 GMT  
		Size: 38.0 MB (37953313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c616df06cfce4fa5e3f76b4147041f55275dd885295b9a2e1b9884f710f5a63`  
		Last Modified: Tue, 13 Jun 2023 01:51:45 GMT  
		Size: 395.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68463d39b900d79d99d0b981ac4de2e7b97ed79424dbbab27775b457b526f553`  
		Last Modified: Tue, 13 Jun 2023 01:52:30 GMT  
		Size: 2.7 KB (2711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecf4c4f53ea5745d056c4cf51430f6362a894011418ab8fc004aab4cac8818e8`  
		Last Modified: Tue, 13 Jun 2023 01:52:30 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:660f7e28cfd4cddb76bc3c880db1190a7a88b2d9b9d93d3e82f5c9b316d3dac5`  
		Last Modified: Tue, 13 Jun 2023 01:52:30 GMT  
		Size: 1.5 KB (1478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17fb5ff54e4d36c97aa5b67854279381fc77880b82436f347c9144327a7ba026`  
		Last Modified: Tue, 13 Jun 2023 01:52:31 GMT  
		Size: 1.4 MB (1386301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1fbe725d5b33c64787888d5b86edbf2d81e345c52311c4d0cd4b5631e8ce365`  
		Last Modified: Tue, 13 Jun 2023 01:52:31 GMT  
		Size: 489.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:fastcgi` - linux; ppc64le

```console
$ docker pull adminer@sha256:f08c2d2d4f6a743fd667ccd77b6e2ea2b906b925e0f09a35df232f82c4692e65
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.3 MB (101256485 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c3935c8e6ae819dd2093e8de8304a6e11a3aae1550d802ad8af7ed871d3cdb02`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Tue, 23 May 2023 01:17:14 GMT
ADD file:ed39869ee4bb8e1901b71feb9cadfe754e42304e134f2542e516e162ca710ec8 in / 
# Tue, 23 May 2023 01:17:17 GMT
CMD ["bash"]
# Tue, 23 May 2023 01:40:42 GMT
STOPSIGNAL SIGINT
# Tue, 23 May 2023 01:41:54 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 01:41:58 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 23 May 2023 01:42:53 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Tue, 23 May 2023 01:42:56 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 23 May 2023 01:42:56 GMT
WORKDIR /var/www/html
# Tue, 23 May 2023 01:42:57 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 23 May 2023 01:42:57 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 23 May 2023 01:42:58 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 23 May 2023 01:42:58 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 23 May 2023 01:43:32 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 23 May 2023 01:43:33 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 23 May 2023 01:43:34 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 23 May 2023 01:43:35 GMT
USER adminer
# Tue, 23 May 2023 01:43:36 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:f530a46e89ee571046fe19b22f563df6c84a31f6593a1e6ed49dbd16e34145de`  
		Last Modified: Tue, 23 May 2023 01:21:34 GMT  
		Size: 58.9 MB (58923948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b328a5c7e2019a9edf5b5d571d37da0261097706c34bafabd5196936aac3fc1b`  
		Last Modified: Tue, 23 May 2023 01:44:03 GMT  
		Size: 40.9 MB (40939928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b29d269a712c093f32a0be4629a0f17bc22fd6dad4be88d5f0af5ce757d809f`  
		Last Modified: Tue, 23 May 2023 01:43:51 GMT  
		Size: 393.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14b5ab23d41e8f1aea6954e2f0b6047fc125e9406f7c560374fe0316f980197e`  
		Last Modified: Tue, 23 May 2023 01:44:22 GMT  
		Size: 2.7 KB (2714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:977b08266ee6cbb32edd6f84d2a98dc861be41484b1401b545d9b0581c1bd174`  
		Last Modified: Tue, 23 May 2023 01:44:22 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92c78939508c16fc88e03d22beb6d700276d381b5a8262d3ff4658b877bad32a`  
		Last Modified: Tue, 23 May 2023 01:44:22 GMT  
		Size: 1.5 KB (1478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bce4c7c01da83a8e67c7a518b162fed2c676be30cdc2c055b920ee658f243cc`  
		Last Modified: Tue, 23 May 2023 01:44:22 GMT  
		Size: 1.4 MB (1385651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5548d29e362ba040749a780b4f79dc74ada494b0aaccaad9e4fbcd61a4b10c61`  
		Last Modified: Tue, 23 May 2023 01:44:22 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:fastcgi` - linux; s390x

```console
$ docker pull adminer@sha256:a194086c2f327aa2f518b1bde88023cd5f0d1cc9d8e0438ef5b392d68f1c3c79
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.7 MB (93692849 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5b04e5e9f13ffd3710ed52616df2923026fc40f821ca1f6247ca708b6decac7`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Tue, 23 May 2023 00:42:35 GMT
ADD file:a054112be60c3f2d7811b27cde82bccfd1c2747f29b7611ee68b21cd9f3d3d54 in / 
# Tue, 23 May 2023 00:42:41 GMT
CMD ["bash"]
# Tue, 23 May 2023 02:26:55 GMT
STOPSIGNAL SIGINT
# Tue, 23 May 2023 02:27:12 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 02:27:15 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 23 May 2023 02:27:31 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Tue, 23 May 2023 02:27:31 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 23 May 2023 02:27:31 GMT
WORKDIR /var/www/html
# Tue, 23 May 2023 02:27:31 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 23 May 2023 02:27:31 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 23 May 2023 02:27:32 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 23 May 2023 02:27:32 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 23 May 2023 02:27:39 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 23 May 2023 02:27:39 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 23 May 2023 02:27:39 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 23 May 2023 02:27:40 GMT
USER adminer
# Tue, 23 May 2023 02:27:40 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:44d1d02f91725dd9ae742f7c70add814dc3da3fde438adb01e65e1f8b0eba613`  
		Last Modified: Tue, 23 May 2023 00:45:33 GMT  
		Size: 53.3 MB (53282114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a714865cdf8c711665c7b864ae5f1e6c7100e6079a9d6bb3d8925f6a0cceaff2`  
		Last Modified: Tue, 23 May 2023 02:28:00 GMT  
		Size: 39.0 MB (39018332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a6faa7559a991fd1e86474adae5128141983567ad4587e50e92ce5d32755bbb`  
		Last Modified: Tue, 23 May 2023 02:27:53 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9101661d5aa45e85b42ae59aa229ccb0658ea3ab2507142a937c15393886927b`  
		Last Modified: Tue, 23 May 2023 02:28:10 GMT  
		Size: 2.7 KB (2708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70537aeb5de09054327e77121e9ac1e2c9309cd67388d6c9f3c6a246c0980aa7`  
		Last Modified: Tue, 23 May 2023 02:28:10 GMT  
		Size: 1.9 KB (1883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42f4125a64e5befb7b5b1dfe94aa43aa55cb192155eb38a12a6d86a3bf660210`  
		Last Modified: Tue, 23 May 2023 02:28:10 GMT  
		Size: 1.5 KB (1477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d338cb5258e7079119cbfe96033d5b49ee9e23aeb5860c5ffd0c1a8bb4342bcf`  
		Last Modified: Tue, 23 May 2023 02:28:11 GMT  
		Size: 1.4 MB (1385455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41ca25d71e32f1c6ef50badf5308e74f4afedccd9f322e5c0c4e2a75bc7a092d`  
		Last Modified: Tue, 23 May 2023 02:28:10 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `adminer:latest`

```console
$ docker pull adminer@sha256:521aae780cec6678443058ecb03e3b20fd815e1c1220dc8370c3a3381acc736c
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
$ docker pull adminer@sha256:203c8ee52640268c28f5ce5f57b192d967da40a91d6443b57ae1da4064e2ed8b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.9 MB (95931867 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e4345c1c3dc89b4c31146abe340fa39e143d922d1e3401233d7ac32db2d985d`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Mon, 12 Jun 2023 23:20:54 GMT
ADD file:e530b0563ea53d97b2f28e62149a665900196f86611df99a88c7a8ab2097b95d in / 
# Mon, 12 Jun 2023 23:20:54 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 03:24:37 GMT
STOPSIGNAL SIGINT
# Tue, 13 Jun 2023 03:25:04 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 03:25:05 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 13 Jun 2023 03:25:06 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 13 Jun 2023 03:25:06 GMT
WORKDIR /var/www/html
# Tue, 13 Jun 2023 03:25:06 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 13 Jun 2023 03:25:06 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 13 Jun 2023 03:25:06 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 13 Jun 2023 03:25:06 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 13 Jun 2023 03:25:19 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Jun 2023 03:25:19 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 13 Jun 2023 03:25:19 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 13 Jun 2023 03:25:19 GMT
USER adminer
# Tue, 13 Jun 2023 03:25:19 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Tue, 13 Jun 2023 03:25:19 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:93c2d578e4211e82e47e7ada9ed05d1869a2362c6f7509f2ee8d91ccebfb7fbd`  
		Last Modified: Mon, 12 Jun 2023 23:26:08 GMT  
		Size: 55.1 MB (55055162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e099cf7ea37ba8ff2169a70f6743bf40675a661f0dc9b6a8abaa4e43050979c`  
		Last Modified: Tue, 13 Jun 2023 03:25:56 GMT  
		Size: 39.5 MB (39487054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d12c699384cbfa0b30a07efef5ad3b7f104e0e1f33e6a094e489150e4ef3838`  
		Last Modified: Tue, 13 Jun 2023 03:25:48 GMT  
		Size: 391.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05c66113a52b479d99efec54808f4045c5fe1400714639a6c750317ad501bc9c`  
		Last Modified: Tue, 13 Jun 2023 03:25:48 GMT  
		Size: 1.9 KB (1874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:677df7ad2be6c1e9f14d49043358dc765759c7f2cd0184ca55a55dc81dcb2263`  
		Last Modified: Tue, 13 Jun 2023 03:25:48 GMT  
		Size: 1.5 KB (1478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:598f6ab1ce2900168e83fbb661f1edc77e27dd8261b23a1f22af28e991facd6e`  
		Last Modified: Tue, 13 Jun 2023 03:25:49 GMT  
		Size: 1.4 MB (1385416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41ed709cb4bc1b53001ba47d24d74fb415c6142dd35194346fdac370144df45a`  
		Last Modified: Tue, 13 Jun 2023 03:25:48 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:latest` - linux; arm variant v5

```console
$ docker pull adminer@sha256:15bb2436532d59fdbf58c3cbc74f61d47be5ad45e30d65bc01adcfc449dd0951
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.2 MB (91183934 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:267345bcacc239fd7427ea82c255b704e164984dbff20209a9e8439820a662d3`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Tue, 23 May 2023 00:48:32 GMT
ADD file:9572a8fcb9c86e8a9dbfe623c732cc4ba1c4f5670490191a7e639a272d5b6e97 in / 
# Tue, 23 May 2023 00:48:33 GMT
CMD ["bash"]
# Tue, 23 May 2023 01:09:52 GMT
STOPSIGNAL SIGINT
# Tue, 23 May 2023 01:10:29 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 01:10:30 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 23 May 2023 01:10:31 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 23 May 2023 01:10:31 GMT
WORKDIR /var/www/html
# Tue, 23 May 2023 01:10:31 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 23 May 2023 01:10:31 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 23 May 2023 01:10:31 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 23 May 2023 01:10:31 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 23 May 2023 01:10:46 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 23 May 2023 01:10:46 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 23 May 2023 01:10:46 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 23 May 2023 01:10:46 GMT
USER adminer
# Tue, 23 May 2023 01:10:46 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Tue, 23 May 2023 01:10:46 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:b053976742ca5b01bcefb7df8fc77a58d0becb4ce508792491574463930569c4`  
		Last Modified: Tue, 23 May 2023 00:50:55 GMT  
		Size: 52.5 MB (52546536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6448799a9363993edd93e5fb6040955191b829140af65c88550e510326878903`  
		Last Modified: Tue, 23 May 2023 01:11:21 GMT  
		Size: 37.2 MB (37247839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b03dc69db3dc4061f823e5e9025874ab539e706b64af3b103bf2a3e839890b8`  
		Last Modified: Tue, 23 May 2023 01:11:13 GMT  
		Size: 388.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ed315aa6041fcfd6bafc18c55ef5be23f10e057e9f941675330807b39d1e54a`  
		Last Modified: Tue, 23 May 2023 01:11:13 GMT  
		Size: 1.9 KB (1872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2d328016feebec5e083e36300e6444d56a5aedfba59d4be438549c64ebcb44f`  
		Last Modified: Tue, 23 May 2023 01:11:13 GMT  
		Size: 1.5 KB (1480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c98954d02c72cf9c2513f055817ac1435ded02424a3418c8d3b9164746bdf3c`  
		Last Modified: Tue, 23 May 2023 01:11:13 GMT  
		Size: 1.4 MB (1385327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aac95e0f74f942d3cfb111cf9949811151a49733af863c919807b2dcbb3a85a1`  
		Last Modified: Tue, 23 May 2023 01:11:13 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:latest` - linux; arm variant v7

```console
$ docker pull adminer@sha256:98b76b0878cf9cc2684e5bbbdade79a5f2f6f269e230203870a1f1a752f7e7f1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.8 MB (87790748 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b51c4364b99328a719594799d5c3d616aeb43a95308f9cd320cb70d27dda4c17`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Mon, 12 Jun 2023 23:58:34 GMT
ADD file:6edc8f94d2ebc83d6081e1c4567963d0060a842c767eaff959a6e5c6d09247b5 in / 
# Mon, 12 Jun 2023 23:58:34 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 04:50:43 GMT
STOPSIGNAL SIGINT
# Tue, 13 Jun 2023 04:51:12 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 04:51:12 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 13 Jun 2023 04:51:13 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 13 Jun 2023 04:51:13 GMT
WORKDIR /var/www/html
# Tue, 13 Jun 2023 04:51:13 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 13 Jun 2023 04:51:13 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 13 Jun 2023 04:51:13 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 13 Jun 2023 04:51:13 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 13 Jun 2023 04:51:41 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Jun 2023 04:51:41 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 13 Jun 2023 04:51:41 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 13 Jun 2023 04:51:41 GMT
USER adminer
# Tue, 13 Jun 2023 04:51:42 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Tue, 13 Jun 2023 04:51:42 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:23807bbf2a5fd14b7975a9e82f4a5530bbba520f31b382cc4b4ce2e77e075ace`  
		Last Modified: Tue, 13 Jun 2023 00:04:02 GMT  
		Size: 50.2 MB (50218141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed9435d7956e105f98b0ce0d774c24da59c523bdcf4ec8fff644876978300c69`  
		Last Modified: Tue, 13 Jun 2023 04:52:24 GMT  
		Size: 36.2 MB (36183011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbf6d7965eb59f39902f271310a767cdf68bdc38bf15c4ee7bc3cfc5c2d025f8`  
		Last Modified: Tue, 13 Jun 2023 04:52:16 GMT  
		Size: 392.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da256b5543040f6999ae9a8cc020bfd0542286ecf71c77feb6cd08a4ecd9be37`  
		Last Modified: Tue, 13 Jun 2023 04:52:16 GMT  
		Size: 1.9 KB (1863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fac8d202305e7ac73502fb63bb1618ac53766c99e8cd03bcb0412c313a25dd83`  
		Last Modified: Tue, 13 Jun 2023 04:52:16 GMT  
		Size: 1.5 KB (1479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b96b3d518c63ab16389a582e075ae88f7225f3c35483203c7c52dcfa52f2daa5`  
		Last Modified: Tue, 13 Jun 2023 04:52:16 GMT  
		Size: 1.4 MB (1385372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eb5818f5b2f148baf53286364c0c6cd2df86e21ed76bfcbc6ff0688a5d2726c`  
		Last Modified: Tue, 13 Jun 2023 04:52:16 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:latest` - linux; arm64 variant v8

```console
$ docker pull adminer@sha256:92cdfd552b3557e293045fc3d5f01d58871958912197649f3c818e312856bf85
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.3 MB (94336689 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b7e1c530248708005dc78825e6702d078b51bbd4eae6c82b2df135ce82d2961`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:22 GMT
ADD file:caddd2f40296ec5c1bf7487617ca8694cfff9a1d9b7484159e203b6514cb5f5f in / 
# Mon, 12 Jun 2023 23:40:23 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 04:45:49 GMT
STOPSIGNAL SIGINT
# Tue, 13 Jun 2023 04:46:10 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 04:46:11 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 13 Jun 2023 04:46:12 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 13 Jun 2023 04:46:12 GMT
WORKDIR /var/www/html
# Tue, 13 Jun 2023 04:46:12 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 13 Jun 2023 04:46:12 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 13 Jun 2023 04:46:12 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 13 Jun 2023 04:46:12 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 13 Jun 2023 04:46:22 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Jun 2023 04:46:22 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 13 Jun 2023 04:46:22 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 13 Jun 2023 04:46:22 GMT
USER adminer
# Tue, 13 Jun 2023 04:46:22 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Tue, 13 Jun 2023 04:46:23 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:663ccfaf62a5d7b997bca03d1dc6d5dfff01b9e0de08d86dbea8957ea92d7d16`  
		Last Modified: Mon, 12 Jun 2023 23:44:25 GMT  
		Size: 53.7 MB (53704136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80aa39d9a9c198e71855c642bc21b287cd96a68f1ca6f6095933aebd07835b55`  
		Last Modified: Tue, 13 Jun 2023 04:46:57 GMT  
		Size: 39.2 MB (39243014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35aba8c7c961932b274149a03d0e4ded7ce7529e514d523d33c6c6972b149b3d`  
		Last Modified: Tue, 13 Jun 2023 04:46:50 GMT  
		Size: 393.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe596da7a5da4c53bb7e8a57c4bca7d95147969f3fcfa27a9ac63992faacad68`  
		Last Modified: Tue, 13 Jun 2023 04:46:51 GMT  
		Size: 1.9 KB (1875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9f19157c079ccd39ddc0b6c916dec64e367d7b29ff37f7d51348654868ffeea`  
		Last Modified: Tue, 13 Jun 2023 04:46:51 GMT  
		Size: 1.5 KB (1482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e9f6bc36eded234b1a9ca40497b6b08e4a5ebd85b8077cfd4951499ef134c78`  
		Last Modified: Tue, 13 Jun 2023 04:46:51 GMT  
		Size: 1.4 MB (1385300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4689e75de5a00a90b25e2ae66464fad25ea65b849b83d549503bdfb11f72be63`  
		Last Modified: Tue, 13 Jun 2023 04:46:51 GMT  
		Size: 489.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:latest` - linux; 386

```console
$ docker pull adminer@sha256:e0bb773bce27da86e8bba771ce6fb58fef553b675ea0e0e2c7eaa0d2bd7dd9f9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.0 MB (96988803 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77720ee3233be6352493a8d99e983f977b3e182750f1526bba6d67134b1bf7ee`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Mon, 12 Jun 2023 23:39:39 GMT
ADD file:4b1f447e0b75fbe493bd68bb77b74f4ba1c61ac8e14226e3c511b3a1c3d5721a in / 
# Mon, 12 Jun 2023 23:39:40 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 00:59:39 GMT
STOPSIGNAL SIGINT
# Tue, 13 Jun 2023 01:00:06 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 01:00:07 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 13 Jun 2023 01:00:07 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 13 Jun 2023 01:00:08 GMT
WORKDIR /var/www/html
# Tue, 13 Jun 2023 01:00:08 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 13 Jun 2023 01:00:08 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 13 Jun 2023 01:00:08 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 13 Jun 2023 01:00:08 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 13 Jun 2023 01:00:20 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Jun 2023 01:00:20 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 13 Jun 2023 01:00:20 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 13 Jun 2023 01:00:21 GMT
USER adminer
# Tue, 13 Jun 2023 01:00:21 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Tue, 13 Jun 2023 01:00:21 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:0997ae72d27731326552ad4699d630b4932f3d31abc07a62105a0eb16b54173a`  
		Last Modified: Mon, 12 Jun 2023 23:46:43 GMT  
		Size: 56.0 MB (56040665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dac97babbe48fc6ee5134482bf3dd02a0763c71618911c97beab64bec3147a8`  
		Last Modified: Tue, 13 Jun 2023 01:01:02 GMT  
		Size: 39.6 MB (39558608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df44f63ded7015da79f717c9dbf6dfd057bcafc06012bc1e415f53113e6fc1e5`  
		Last Modified: Tue, 13 Jun 2023 01:00:51 GMT  
		Size: 389.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ae3ce4c7547485956e0bd1180cc66032006af3b33c6ae582d77834096391752`  
		Last Modified: Tue, 13 Jun 2023 01:00:51 GMT  
		Size: 1.9 KB (1864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83417b3fe0dbbaed7076986fd209d6704b096ecd961a111cfb42cba80a11dc93`  
		Last Modified: Tue, 13 Jun 2023 01:00:51 GMT  
		Size: 1.5 KB (1480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbdb97551a1780228aac70017b847d497ec088d6ad3e46d5c8b9b48083efe5a0`  
		Last Modified: Tue, 13 Jun 2023 01:00:52 GMT  
		Size: 1.4 MB (1385307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbef3e3e2b3156ba5eca052ebf766f2f4474f980905836f0c0ea9eec319f7a6e`  
		Last Modified: Tue, 13 Jun 2023 01:00:51 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:latest` - linux; mips64le

```console
$ docker pull adminer@sha256:2591b1f0dffbc4f123a4a3bd12c1cb46669c54383e8e23e13c83edaecc2541d1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.6 MB (92614104 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9a417a537dc4187139ad39c01263d6bd8b79a728bf005ad51d3bb4d42ec1d5f`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Tue, 13 Jun 2023 00:09:46 GMT
ADD file:7ba4829e0a582c8a2e5a1d362ca30cfba3fa2911594faf9598927255100965b0 in / 
# Tue, 13 Jun 2023 00:09:51 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 01:46:11 GMT
STOPSIGNAL SIGINT
# Tue, 13 Jun 2023 01:48:01 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 01:48:08 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 13 Jun 2023 01:48:14 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 13 Jun 2023 01:48:18 GMT
WORKDIR /var/www/html
# Tue, 13 Jun 2023 01:48:21 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 13 Jun 2023 01:48:24 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 13 Jun 2023 01:48:28 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 13 Jun 2023 01:48:31 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 13 Jun 2023 01:49:21 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Jun 2023 01:49:24 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 13 Jun 2023 01:49:27 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 13 Jun 2023 01:49:31 GMT
USER adminer
# Tue, 13 Jun 2023 01:49:34 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Tue, 13 Jun 2023 01:49:37 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:ec034d426521af0a9addba08124f06b364f3364fd20ec9aec4e3364104a793d1`  
		Last Modified: Tue, 13 Jun 2023 00:23:13 GMT  
		Size: 53.3 MB (53270410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:901a0f1a33bd58f6d5e7b1de7a90c5fbe79c192cbbabfd8c7a98214496b73c1b`  
		Last Modified: Tue, 13 Jun 2023 01:52:11 GMT  
		Size: 38.0 MB (37953313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c616df06cfce4fa5e3f76b4147041f55275dd885295b9a2e1b9884f710f5a63`  
		Last Modified: Tue, 13 Jun 2023 01:51:45 GMT  
		Size: 395.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84487562d4b36a6a1112b198b725b1a727e91a77be9899c0d74b1a4a9c022dba`  
		Last Modified: Tue, 13 Jun 2023 01:51:45 GMT  
		Size: 1.7 KB (1723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5dde6303cb52a3de95ebac876b6f8590487f4ffa08f8c0e80844f4d89b75072`  
		Last Modified: Tue, 13 Jun 2023 01:51:45 GMT  
		Size: 1.5 KB (1480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:499702681379ddde7be8cc76c78d9b9c764ceea9af16c336da3a99169971feb1`  
		Last Modified: Tue, 13 Jun 2023 01:51:46 GMT  
		Size: 1.4 MB (1386295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63d75b2d63e14c568323dc0897c171f4d71efe33d94bb1423a59c555514d35ae`  
		Last Modified: Tue, 13 Jun 2023 01:51:45 GMT  
		Size: 488.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:latest` - linux; ppc64le

```console
$ docker pull adminer@sha256:e0a0e907c5c635e5e363e08b1dffd85143970ad1e4dee8cd2acdbd2c47f59f30
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.3 MB (101253778 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0759ab5b0827c3e5903a54d9e690f3911052bcece85af789658d87469a6c4e41`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Tue, 23 May 2023 01:17:14 GMT
ADD file:ed39869ee4bb8e1901b71feb9cadfe754e42304e134f2542e516e162ca710ec8 in / 
# Tue, 23 May 2023 01:17:17 GMT
CMD ["bash"]
# Tue, 23 May 2023 01:40:42 GMT
STOPSIGNAL SIGINT
# Tue, 23 May 2023 01:41:54 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 01:41:58 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 23 May 2023 01:42:00 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 23 May 2023 01:42:01 GMT
WORKDIR /var/www/html
# Tue, 23 May 2023 01:42:01 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 23 May 2023 01:42:02 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 23 May 2023 01:42:02 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 23 May 2023 01:42:02 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 23 May 2023 01:42:36 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 23 May 2023 01:42:37 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 23 May 2023 01:42:37 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 23 May 2023 01:42:38 GMT
USER adminer
# Tue, 23 May 2023 01:42:39 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Tue, 23 May 2023 01:42:40 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:f530a46e89ee571046fe19b22f563df6c84a31f6593a1e6ed49dbd16e34145de`  
		Last Modified: Tue, 23 May 2023 01:21:34 GMT  
		Size: 58.9 MB (58923948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b328a5c7e2019a9edf5b5d571d37da0261097706c34bafabd5196936aac3fc1b`  
		Last Modified: Tue, 23 May 2023 01:44:03 GMT  
		Size: 40.9 MB (40939928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b29d269a712c093f32a0be4629a0f17bc22fd6dad4be88d5f0af5ce757d809f`  
		Last Modified: Tue, 23 May 2023 01:43:51 GMT  
		Size: 393.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:904564df90e41e35afa3221ab3277e3aa554b7c686393785c1b07372bc0c4d4d`  
		Last Modified: Tue, 23 May 2023 01:43:51 GMT  
		Size: 1.9 KB (1880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55a789415d78b4a3befd6b003659799bcf3d20cb06639a961c96a980640e8991`  
		Last Modified: Tue, 23 May 2023 01:43:51 GMT  
		Size: 1.5 KB (1479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78c991997ea0a176dc01a5a08f6ac61143299aef87572cd7e8578e479aae772b`  
		Last Modified: Tue, 23 May 2023 01:43:52 GMT  
		Size: 1.4 MB (1385657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd039d869a125163f2302899c7b0fcf2db140dad2eecedc648b3ca229cb86460`  
		Last Modified: Tue, 23 May 2023 01:43:51 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:latest` - linux; s390x

```console
$ docker pull adminer@sha256:b48c2c7360476d0f6ce0723abeef59ed2cc19493ffedd144d64ee2b5d0a21683
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.7 MB (93690153 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:008c852f84add504c1031fabd62a8ede6758604b42d91789507acf3c08df5507`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Tue, 23 May 2023 00:42:35 GMT
ADD file:a054112be60c3f2d7811b27cde82bccfd1c2747f29b7611ee68b21cd9f3d3d54 in / 
# Tue, 23 May 2023 00:42:41 GMT
CMD ["bash"]
# Tue, 23 May 2023 02:26:55 GMT
STOPSIGNAL SIGINT
# Tue, 23 May 2023 02:27:12 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 02:27:15 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 23 May 2023 02:27:15 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 23 May 2023 02:27:15 GMT
WORKDIR /var/www/html
# Tue, 23 May 2023 02:27:15 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 23 May 2023 02:27:15 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 23 May 2023 02:27:16 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 23 May 2023 02:27:16 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 23 May 2023 02:27:23 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 23 May 2023 02:27:23 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 23 May 2023 02:27:23 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 23 May 2023 02:27:24 GMT
USER adminer
# Tue, 23 May 2023 02:27:24 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Tue, 23 May 2023 02:27:24 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:44d1d02f91725dd9ae742f7c70add814dc3da3fde438adb01e65e1f8b0eba613`  
		Last Modified: Tue, 23 May 2023 00:45:33 GMT  
		Size: 53.3 MB (53282114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a714865cdf8c711665c7b864ae5f1e6c7100e6079a9d6bb3d8925f6a0cceaff2`  
		Last Modified: Tue, 23 May 2023 02:28:00 GMT  
		Size: 39.0 MB (39018332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a6faa7559a991fd1e86474adae5128141983567ad4587e50e92ce5d32755bbb`  
		Last Modified: Tue, 23 May 2023 02:27:53 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f55cc440fda23758bbfb18b1a3881ac61d06ad9e0a4b35da688b713c1b8611be`  
		Last Modified: Tue, 23 May 2023 02:27:53 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d16d617d4904a95242ab9db1204e6fa0d844358dc62528fed7ad368f57b1251d`  
		Last Modified: Tue, 23 May 2023 02:27:53 GMT  
		Size: 1.5 KB (1478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c753b23f0be5c140b7bed93c7220f68e38f138d53d3e7e9aade64a9d4b45038e`  
		Last Modified: Tue, 23 May 2023 02:27:53 GMT  
		Size: 1.4 MB (1385466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a436f3a56433ffbdc8b5e6a7bda069a68625447867738966931d19c9db78365c`  
		Last Modified: Tue, 23 May 2023 02:27:53 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `adminer:standalone`

```console
$ docker pull adminer@sha256:521aae780cec6678443058ecb03e3b20fd815e1c1220dc8370c3a3381acc736c
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
$ docker pull adminer@sha256:203c8ee52640268c28f5ce5f57b192d967da40a91d6443b57ae1da4064e2ed8b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.9 MB (95931867 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e4345c1c3dc89b4c31146abe340fa39e143d922d1e3401233d7ac32db2d985d`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Mon, 12 Jun 2023 23:20:54 GMT
ADD file:e530b0563ea53d97b2f28e62149a665900196f86611df99a88c7a8ab2097b95d in / 
# Mon, 12 Jun 2023 23:20:54 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 03:24:37 GMT
STOPSIGNAL SIGINT
# Tue, 13 Jun 2023 03:25:04 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 03:25:05 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 13 Jun 2023 03:25:06 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 13 Jun 2023 03:25:06 GMT
WORKDIR /var/www/html
# Tue, 13 Jun 2023 03:25:06 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 13 Jun 2023 03:25:06 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 13 Jun 2023 03:25:06 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 13 Jun 2023 03:25:06 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 13 Jun 2023 03:25:19 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Jun 2023 03:25:19 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 13 Jun 2023 03:25:19 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 13 Jun 2023 03:25:19 GMT
USER adminer
# Tue, 13 Jun 2023 03:25:19 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Tue, 13 Jun 2023 03:25:19 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:93c2d578e4211e82e47e7ada9ed05d1869a2362c6f7509f2ee8d91ccebfb7fbd`  
		Last Modified: Mon, 12 Jun 2023 23:26:08 GMT  
		Size: 55.1 MB (55055162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e099cf7ea37ba8ff2169a70f6743bf40675a661f0dc9b6a8abaa4e43050979c`  
		Last Modified: Tue, 13 Jun 2023 03:25:56 GMT  
		Size: 39.5 MB (39487054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d12c699384cbfa0b30a07efef5ad3b7f104e0e1f33e6a094e489150e4ef3838`  
		Last Modified: Tue, 13 Jun 2023 03:25:48 GMT  
		Size: 391.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05c66113a52b479d99efec54808f4045c5fe1400714639a6c750317ad501bc9c`  
		Last Modified: Tue, 13 Jun 2023 03:25:48 GMT  
		Size: 1.9 KB (1874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:677df7ad2be6c1e9f14d49043358dc765759c7f2cd0184ca55a55dc81dcb2263`  
		Last Modified: Tue, 13 Jun 2023 03:25:48 GMT  
		Size: 1.5 KB (1478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:598f6ab1ce2900168e83fbb661f1edc77e27dd8261b23a1f22af28e991facd6e`  
		Last Modified: Tue, 13 Jun 2023 03:25:49 GMT  
		Size: 1.4 MB (1385416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41ed709cb4bc1b53001ba47d24d74fb415c6142dd35194346fdac370144df45a`  
		Last Modified: Tue, 13 Jun 2023 03:25:48 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:standalone` - linux; arm variant v5

```console
$ docker pull adminer@sha256:15bb2436532d59fdbf58c3cbc74f61d47be5ad45e30d65bc01adcfc449dd0951
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.2 MB (91183934 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:267345bcacc239fd7427ea82c255b704e164984dbff20209a9e8439820a662d3`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Tue, 23 May 2023 00:48:32 GMT
ADD file:9572a8fcb9c86e8a9dbfe623c732cc4ba1c4f5670490191a7e639a272d5b6e97 in / 
# Tue, 23 May 2023 00:48:33 GMT
CMD ["bash"]
# Tue, 23 May 2023 01:09:52 GMT
STOPSIGNAL SIGINT
# Tue, 23 May 2023 01:10:29 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 01:10:30 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 23 May 2023 01:10:31 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 23 May 2023 01:10:31 GMT
WORKDIR /var/www/html
# Tue, 23 May 2023 01:10:31 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 23 May 2023 01:10:31 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 23 May 2023 01:10:31 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 23 May 2023 01:10:31 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 23 May 2023 01:10:46 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 23 May 2023 01:10:46 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 23 May 2023 01:10:46 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 23 May 2023 01:10:46 GMT
USER adminer
# Tue, 23 May 2023 01:10:46 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Tue, 23 May 2023 01:10:46 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:b053976742ca5b01bcefb7df8fc77a58d0becb4ce508792491574463930569c4`  
		Last Modified: Tue, 23 May 2023 00:50:55 GMT  
		Size: 52.5 MB (52546536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6448799a9363993edd93e5fb6040955191b829140af65c88550e510326878903`  
		Last Modified: Tue, 23 May 2023 01:11:21 GMT  
		Size: 37.2 MB (37247839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b03dc69db3dc4061f823e5e9025874ab539e706b64af3b103bf2a3e839890b8`  
		Last Modified: Tue, 23 May 2023 01:11:13 GMT  
		Size: 388.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ed315aa6041fcfd6bafc18c55ef5be23f10e057e9f941675330807b39d1e54a`  
		Last Modified: Tue, 23 May 2023 01:11:13 GMT  
		Size: 1.9 KB (1872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2d328016feebec5e083e36300e6444d56a5aedfba59d4be438549c64ebcb44f`  
		Last Modified: Tue, 23 May 2023 01:11:13 GMT  
		Size: 1.5 KB (1480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c98954d02c72cf9c2513f055817ac1435ded02424a3418c8d3b9164746bdf3c`  
		Last Modified: Tue, 23 May 2023 01:11:13 GMT  
		Size: 1.4 MB (1385327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aac95e0f74f942d3cfb111cf9949811151a49733af863c919807b2dcbb3a85a1`  
		Last Modified: Tue, 23 May 2023 01:11:13 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:standalone` - linux; arm variant v7

```console
$ docker pull adminer@sha256:98b76b0878cf9cc2684e5bbbdade79a5f2f6f269e230203870a1f1a752f7e7f1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.8 MB (87790748 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b51c4364b99328a719594799d5c3d616aeb43a95308f9cd320cb70d27dda4c17`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Mon, 12 Jun 2023 23:58:34 GMT
ADD file:6edc8f94d2ebc83d6081e1c4567963d0060a842c767eaff959a6e5c6d09247b5 in / 
# Mon, 12 Jun 2023 23:58:34 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 04:50:43 GMT
STOPSIGNAL SIGINT
# Tue, 13 Jun 2023 04:51:12 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 04:51:12 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 13 Jun 2023 04:51:13 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 13 Jun 2023 04:51:13 GMT
WORKDIR /var/www/html
# Tue, 13 Jun 2023 04:51:13 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 13 Jun 2023 04:51:13 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 13 Jun 2023 04:51:13 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 13 Jun 2023 04:51:13 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 13 Jun 2023 04:51:41 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Jun 2023 04:51:41 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 13 Jun 2023 04:51:41 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 13 Jun 2023 04:51:41 GMT
USER adminer
# Tue, 13 Jun 2023 04:51:42 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Tue, 13 Jun 2023 04:51:42 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:23807bbf2a5fd14b7975a9e82f4a5530bbba520f31b382cc4b4ce2e77e075ace`  
		Last Modified: Tue, 13 Jun 2023 00:04:02 GMT  
		Size: 50.2 MB (50218141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed9435d7956e105f98b0ce0d774c24da59c523bdcf4ec8fff644876978300c69`  
		Last Modified: Tue, 13 Jun 2023 04:52:24 GMT  
		Size: 36.2 MB (36183011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbf6d7965eb59f39902f271310a767cdf68bdc38bf15c4ee7bc3cfc5c2d025f8`  
		Last Modified: Tue, 13 Jun 2023 04:52:16 GMT  
		Size: 392.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da256b5543040f6999ae9a8cc020bfd0542286ecf71c77feb6cd08a4ecd9be37`  
		Last Modified: Tue, 13 Jun 2023 04:52:16 GMT  
		Size: 1.9 KB (1863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fac8d202305e7ac73502fb63bb1618ac53766c99e8cd03bcb0412c313a25dd83`  
		Last Modified: Tue, 13 Jun 2023 04:52:16 GMT  
		Size: 1.5 KB (1479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b96b3d518c63ab16389a582e075ae88f7225f3c35483203c7c52dcfa52f2daa5`  
		Last Modified: Tue, 13 Jun 2023 04:52:16 GMT  
		Size: 1.4 MB (1385372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eb5818f5b2f148baf53286364c0c6cd2df86e21ed76bfcbc6ff0688a5d2726c`  
		Last Modified: Tue, 13 Jun 2023 04:52:16 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:standalone` - linux; arm64 variant v8

```console
$ docker pull adminer@sha256:92cdfd552b3557e293045fc3d5f01d58871958912197649f3c818e312856bf85
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.3 MB (94336689 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b7e1c530248708005dc78825e6702d078b51bbd4eae6c82b2df135ce82d2961`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:22 GMT
ADD file:caddd2f40296ec5c1bf7487617ca8694cfff9a1d9b7484159e203b6514cb5f5f in / 
# Mon, 12 Jun 2023 23:40:23 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 04:45:49 GMT
STOPSIGNAL SIGINT
# Tue, 13 Jun 2023 04:46:10 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 04:46:11 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 13 Jun 2023 04:46:12 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 13 Jun 2023 04:46:12 GMT
WORKDIR /var/www/html
# Tue, 13 Jun 2023 04:46:12 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 13 Jun 2023 04:46:12 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 13 Jun 2023 04:46:12 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 13 Jun 2023 04:46:12 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 13 Jun 2023 04:46:22 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Jun 2023 04:46:22 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 13 Jun 2023 04:46:22 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 13 Jun 2023 04:46:22 GMT
USER adminer
# Tue, 13 Jun 2023 04:46:22 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Tue, 13 Jun 2023 04:46:23 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:663ccfaf62a5d7b997bca03d1dc6d5dfff01b9e0de08d86dbea8957ea92d7d16`  
		Last Modified: Mon, 12 Jun 2023 23:44:25 GMT  
		Size: 53.7 MB (53704136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80aa39d9a9c198e71855c642bc21b287cd96a68f1ca6f6095933aebd07835b55`  
		Last Modified: Tue, 13 Jun 2023 04:46:57 GMT  
		Size: 39.2 MB (39243014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35aba8c7c961932b274149a03d0e4ded7ce7529e514d523d33c6c6972b149b3d`  
		Last Modified: Tue, 13 Jun 2023 04:46:50 GMT  
		Size: 393.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe596da7a5da4c53bb7e8a57c4bca7d95147969f3fcfa27a9ac63992faacad68`  
		Last Modified: Tue, 13 Jun 2023 04:46:51 GMT  
		Size: 1.9 KB (1875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9f19157c079ccd39ddc0b6c916dec64e367d7b29ff37f7d51348654868ffeea`  
		Last Modified: Tue, 13 Jun 2023 04:46:51 GMT  
		Size: 1.5 KB (1482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e9f6bc36eded234b1a9ca40497b6b08e4a5ebd85b8077cfd4951499ef134c78`  
		Last Modified: Tue, 13 Jun 2023 04:46:51 GMT  
		Size: 1.4 MB (1385300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4689e75de5a00a90b25e2ae66464fad25ea65b849b83d549503bdfb11f72be63`  
		Last Modified: Tue, 13 Jun 2023 04:46:51 GMT  
		Size: 489.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:standalone` - linux; 386

```console
$ docker pull adminer@sha256:e0bb773bce27da86e8bba771ce6fb58fef553b675ea0e0e2c7eaa0d2bd7dd9f9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.0 MB (96988803 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77720ee3233be6352493a8d99e983f977b3e182750f1526bba6d67134b1bf7ee`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Mon, 12 Jun 2023 23:39:39 GMT
ADD file:4b1f447e0b75fbe493bd68bb77b74f4ba1c61ac8e14226e3c511b3a1c3d5721a in / 
# Mon, 12 Jun 2023 23:39:40 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 00:59:39 GMT
STOPSIGNAL SIGINT
# Tue, 13 Jun 2023 01:00:06 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 01:00:07 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 13 Jun 2023 01:00:07 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 13 Jun 2023 01:00:08 GMT
WORKDIR /var/www/html
# Tue, 13 Jun 2023 01:00:08 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 13 Jun 2023 01:00:08 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 13 Jun 2023 01:00:08 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 13 Jun 2023 01:00:08 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 13 Jun 2023 01:00:20 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Jun 2023 01:00:20 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 13 Jun 2023 01:00:20 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 13 Jun 2023 01:00:21 GMT
USER adminer
# Tue, 13 Jun 2023 01:00:21 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Tue, 13 Jun 2023 01:00:21 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:0997ae72d27731326552ad4699d630b4932f3d31abc07a62105a0eb16b54173a`  
		Last Modified: Mon, 12 Jun 2023 23:46:43 GMT  
		Size: 56.0 MB (56040665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dac97babbe48fc6ee5134482bf3dd02a0763c71618911c97beab64bec3147a8`  
		Last Modified: Tue, 13 Jun 2023 01:01:02 GMT  
		Size: 39.6 MB (39558608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df44f63ded7015da79f717c9dbf6dfd057bcafc06012bc1e415f53113e6fc1e5`  
		Last Modified: Tue, 13 Jun 2023 01:00:51 GMT  
		Size: 389.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ae3ce4c7547485956e0bd1180cc66032006af3b33c6ae582d77834096391752`  
		Last Modified: Tue, 13 Jun 2023 01:00:51 GMT  
		Size: 1.9 KB (1864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83417b3fe0dbbaed7076986fd209d6704b096ecd961a111cfb42cba80a11dc93`  
		Last Modified: Tue, 13 Jun 2023 01:00:51 GMT  
		Size: 1.5 KB (1480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbdb97551a1780228aac70017b847d497ec088d6ad3e46d5c8b9b48083efe5a0`  
		Last Modified: Tue, 13 Jun 2023 01:00:52 GMT  
		Size: 1.4 MB (1385307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbef3e3e2b3156ba5eca052ebf766f2f4474f980905836f0c0ea9eec319f7a6e`  
		Last Modified: Tue, 13 Jun 2023 01:00:51 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:standalone` - linux; mips64le

```console
$ docker pull adminer@sha256:2591b1f0dffbc4f123a4a3bd12c1cb46669c54383e8e23e13c83edaecc2541d1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.6 MB (92614104 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9a417a537dc4187139ad39c01263d6bd8b79a728bf005ad51d3bb4d42ec1d5f`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Tue, 13 Jun 2023 00:09:46 GMT
ADD file:7ba4829e0a582c8a2e5a1d362ca30cfba3fa2911594faf9598927255100965b0 in / 
# Tue, 13 Jun 2023 00:09:51 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 01:46:11 GMT
STOPSIGNAL SIGINT
# Tue, 13 Jun 2023 01:48:01 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 01:48:08 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 13 Jun 2023 01:48:14 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 13 Jun 2023 01:48:18 GMT
WORKDIR /var/www/html
# Tue, 13 Jun 2023 01:48:21 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 13 Jun 2023 01:48:24 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 13 Jun 2023 01:48:28 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 13 Jun 2023 01:48:31 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 13 Jun 2023 01:49:21 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Jun 2023 01:49:24 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 13 Jun 2023 01:49:27 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 13 Jun 2023 01:49:31 GMT
USER adminer
# Tue, 13 Jun 2023 01:49:34 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Tue, 13 Jun 2023 01:49:37 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:ec034d426521af0a9addba08124f06b364f3364fd20ec9aec4e3364104a793d1`  
		Last Modified: Tue, 13 Jun 2023 00:23:13 GMT  
		Size: 53.3 MB (53270410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:901a0f1a33bd58f6d5e7b1de7a90c5fbe79c192cbbabfd8c7a98214496b73c1b`  
		Last Modified: Tue, 13 Jun 2023 01:52:11 GMT  
		Size: 38.0 MB (37953313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c616df06cfce4fa5e3f76b4147041f55275dd885295b9a2e1b9884f710f5a63`  
		Last Modified: Tue, 13 Jun 2023 01:51:45 GMT  
		Size: 395.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84487562d4b36a6a1112b198b725b1a727e91a77be9899c0d74b1a4a9c022dba`  
		Last Modified: Tue, 13 Jun 2023 01:51:45 GMT  
		Size: 1.7 KB (1723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5dde6303cb52a3de95ebac876b6f8590487f4ffa08f8c0e80844f4d89b75072`  
		Last Modified: Tue, 13 Jun 2023 01:51:45 GMT  
		Size: 1.5 KB (1480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:499702681379ddde7be8cc76c78d9b9c764ceea9af16c336da3a99169971feb1`  
		Last Modified: Tue, 13 Jun 2023 01:51:46 GMT  
		Size: 1.4 MB (1386295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63d75b2d63e14c568323dc0897c171f4d71efe33d94bb1423a59c555514d35ae`  
		Last Modified: Tue, 13 Jun 2023 01:51:45 GMT  
		Size: 488.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:standalone` - linux; ppc64le

```console
$ docker pull adminer@sha256:e0a0e907c5c635e5e363e08b1dffd85143970ad1e4dee8cd2acdbd2c47f59f30
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.3 MB (101253778 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0759ab5b0827c3e5903a54d9e690f3911052bcece85af789658d87469a6c4e41`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Tue, 23 May 2023 01:17:14 GMT
ADD file:ed39869ee4bb8e1901b71feb9cadfe754e42304e134f2542e516e162ca710ec8 in / 
# Tue, 23 May 2023 01:17:17 GMT
CMD ["bash"]
# Tue, 23 May 2023 01:40:42 GMT
STOPSIGNAL SIGINT
# Tue, 23 May 2023 01:41:54 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 01:41:58 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 23 May 2023 01:42:00 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 23 May 2023 01:42:01 GMT
WORKDIR /var/www/html
# Tue, 23 May 2023 01:42:01 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 23 May 2023 01:42:02 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 23 May 2023 01:42:02 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 23 May 2023 01:42:02 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 23 May 2023 01:42:36 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 23 May 2023 01:42:37 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 23 May 2023 01:42:37 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 23 May 2023 01:42:38 GMT
USER adminer
# Tue, 23 May 2023 01:42:39 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Tue, 23 May 2023 01:42:40 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:f530a46e89ee571046fe19b22f563df6c84a31f6593a1e6ed49dbd16e34145de`  
		Last Modified: Tue, 23 May 2023 01:21:34 GMT  
		Size: 58.9 MB (58923948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b328a5c7e2019a9edf5b5d571d37da0261097706c34bafabd5196936aac3fc1b`  
		Last Modified: Tue, 23 May 2023 01:44:03 GMT  
		Size: 40.9 MB (40939928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b29d269a712c093f32a0be4629a0f17bc22fd6dad4be88d5f0af5ce757d809f`  
		Last Modified: Tue, 23 May 2023 01:43:51 GMT  
		Size: 393.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:904564df90e41e35afa3221ab3277e3aa554b7c686393785c1b07372bc0c4d4d`  
		Last Modified: Tue, 23 May 2023 01:43:51 GMT  
		Size: 1.9 KB (1880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55a789415d78b4a3befd6b003659799bcf3d20cb06639a961c96a980640e8991`  
		Last Modified: Tue, 23 May 2023 01:43:51 GMT  
		Size: 1.5 KB (1479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78c991997ea0a176dc01a5a08f6ac61143299aef87572cd7e8578e479aae772b`  
		Last Modified: Tue, 23 May 2023 01:43:52 GMT  
		Size: 1.4 MB (1385657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd039d869a125163f2302899c7b0fcf2db140dad2eecedc648b3ca229cb86460`  
		Last Modified: Tue, 23 May 2023 01:43:51 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:standalone` - linux; s390x

```console
$ docker pull adminer@sha256:b48c2c7360476d0f6ce0723abeef59ed2cc19493ffedd144d64ee2b5d0a21683
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.7 MB (93690153 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:008c852f84add504c1031fabd62a8ede6758604b42d91789507acf3c08df5507`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Tue, 23 May 2023 00:42:35 GMT
ADD file:a054112be60c3f2d7811b27cde82bccfd1c2747f29b7611ee68b21cd9f3d3d54 in / 
# Tue, 23 May 2023 00:42:41 GMT
CMD ["bash"]
# Tue, 23 May 2023 02:26:55 GMT
STOPSIGNAL SIGINT
# Tue, 23 May 2023 02:27:12 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 02:27:15 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 23 May 2023 02:27:15 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 23 May 2023 02:27:15 GMT
WORKDIR /var/www/html
# Tue, 23 May 2023 02:27:15 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 23 May 2023 02:27:15 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 23 May 2023 02:27:16 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 23 May 2023 02:27:16 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 23 May 2023 02:27:23 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 23 May 2023 02:27:23 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 23 May 2023 02:27:23 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 23 May 2023 02:27:24 GMT
USER adminer
# Tue, 23 May 2023 02:27:24 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Tue, 23 May 2023 02:27:24 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:44d1d02f91725dd9ae742f7c70add814dc3da3fde438adb01e65e1f8b0eba613`  
		Last Modified: Tue, 23 May 2023 00:45:33 GMT  
		Size: 53.3 MB (53282114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a714865cdf8c711665c7b864ae5f1e6c7100e6079a9d6bb3d8925f6a0cceaff2`  
		Last Modified: Tue, 23 May 2023 02:28:00 GMT  
		Size: 39.0 MB (39018332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a6faa7559a991fd1e86474adae5128141983567ad4587e50e92ce5d32755bbb`  
		Last Modified: Tue, 23 May 2023 02:27:53 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f55cc440fda23758bbfb18b1a3881ac61d06ad9e0a4b35da688b713c1b8611be`  
		Last Modified: Tue, 23 May 2023 02:27:53 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d16d617d4904a95242ab9db1204e6fa0d844358dc62528fed7ad368f57b1251d`  
		Last Modified: Tue, 23 May 2023 02:27:53 GMT  
		Size: 1.5 KB (1478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c753b23f0be5c140b7bed93c7220f68e38f138d53d3e7e9aade64a9d4b45038e`  
		Last Modified: Tue, 23 May 2023 02:27:53 GMT  
		Size: 1.4 MB (1385466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a436f3a56433ffbdc8b5e6a7bda069a68625447867738966931d19c9db78365c`  
		Last Modified: Tue, 23 May 2023 02:27:53 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
