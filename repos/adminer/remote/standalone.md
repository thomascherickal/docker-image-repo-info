## `adminer:standalone`

```console
$ docker pull adminer@sha256:d1dd4da85ada2da92b051c7dead671a7671e15789e17551773c703fd69e3c27d
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
$ docker pull adminer@sha256:c10c5bc6358c2dfe5f9d31d46642697641d670b89927898857962515f9e934e6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.9 MB (95925779 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc1ef98c263bc361fe31173b63e7e055e8c882725045a3cc7c646a34b7c4daf3`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Tue, 23 May 2023 01:20:00 GMT
ADD file:150a6453ab2258061c1a1549ab119df752bdc2c2c84028fa0e83a0663cd8cedf in / 
# Tue, 23 May 2023 01:20:01 GMT
CMD ["bash"]
# Tue, 23 May 2023 01:42:55 GMT
STOPSIGNAL SIGINT
# Tue, 23 May 2023 01:43:24 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 01:43:25 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 23 May 2023 01:43:25 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 23 May 2023 01:43:25 GMT
WORKDIR /var/www/html
# Tue, 23 May 2023 01:43:25 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 23 May 2023 01:43:26 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 23 May 2023 01:43:26 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 23 May 2023 01:43:26 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 23 May 2023 01:43:38 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 23 May 2023 01:43:38 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 23 May 2023 01:43:38 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 23 May 2023 01:43:38 GMT
USER adminer
# Tue, 23 May 2023 01:43:38 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Tue, 23 May 2023 01:43:38 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:bd73737482dd5575526c7207872963479808d979ab2741c321706b8553918474`  
		Last Modified: Tue, 23 May 2023 01:23:46 GMT  
		Size: 55.0 MB (55049027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:995991ad6a4107ed8bace373cccbc4f76d9b40e8e75b4d7130a28cae85d8eb39`  
		Last Modified: Tue, 23 May 2023 01:44:15 GMT  
		Size: 39.5 MB (39487120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0220fa348b69b540c076afc1f3ff56c663bcbf849f33aced7a0abd7f250aa41`  
		Last Modified: Tue, 23 May 2023 01:44:08 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc760e5aa65087b5226ab301584831b007e64a7b752e7f9f30e1bb7efcb16d40`  
		Last Modified: Tue, 23 May 2023 01:44:07 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:477a78c654ea0a40f22d4df52838b8e35d28eaba1822a555a81bb32f4704cbef`  
		Last Modified: Tue, 23 May 2023 01:44:08 GMT  
		Size: 1.5 KB (1476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68b41477645dfcc5cf81f4019f25dd2796116459ddf14963b2c8d32a9de74977`  
		Last Modified: Tue, 23 May 2023 01:44:08 GMT  
		Size: 1.4 MB (1385392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e612bbedc5306aa83354de0f379a488cb8fccef3befbea6c81f6d5d2f131c484`  
		Last Modified: Tue, 23 May 2023 01:44:08 GMT  
		Size: 493.0 B  
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
$ docker pull adminer@sha256:fff0e54f17db7998bc7171bba3c45888f7fe98332935e117d4d0bda9abd90835
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.8 MB (87782786 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad296bc467c6466b86d09eb2ba042eb3e238ab0d151c08beafcfb2025c5c176b`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Tue, 23 May 2023 00:57:45 GMT
ADD file:d8748d34e524d93a6df76d2a8ea8ca32ca04897521719f9f1f2a88ec692dd69e in / 
# Tue, 23 May 2023 00:57:45 GMT
CMD ["bash"]
# Tue, 23 May 2023 05:52:58 GMT
STOPSIGNAL SIGINT
# Tue, 23 May 2023 05:53:26 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 05:53:26 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 23 May 2023 05:53:27 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 23 May 2023 05:53:27 GMT
WORKDIR /var/www/html
# Tue, 23 May 2023 05:53:27 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 23 May 2023 05:53:27 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 23 May 2023 05:53:27 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 23 May 2023 05:53:27 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 23 May 2023 05:53:40 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 23 May 2023 05:53:40 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 23 May 2023 05:53:41 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 23 May 2023 05:53:41 GMT
USER adminer
# Tue, 23 May 2023 05:53:41 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Tue, 23 May 2023 05:53:41 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:29949e2d07dd1e283862cb4c3d4ec3043f1d54a1ac59f7b7a998ed9038a0243c`  
		Last Modified: Tue, 23 May 2023 01:01:23 GMT  
		Size: 50.2 MB (50210000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1e1941f5530f7a27a7722b021d0e04f545631a23185a5e61ad0ca0f09e6b62d`  
		Last Modified: Tue, 23 May 2023 05:54:16 GMT  
		Size: 36.2 MB (36183208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d828e807810f9c62c685b6c40c52595a9c0a4f79dbef844862daf12ecf116fe`  
		Last Modified: Tue, 23 May 2023 05:54:08 GMT  
		Size: 393.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca43e56cd7b197015f18457c51c1342767b40c844c0288aeacd170baf7599e1a`  
		Last Modified: Tue, 23 May 2023 05:54:08 GMT  
		Size: 1.9 KB (1872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2ae33bb24cfbf558ac5ae8d6cb98ea4d866563ecf6fdd2a065ee4caf18c950f`  
		Last Modified: Tue, 23 May 2023 05:54:08 GMT  
		Size: 1.5 KB (1479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0a836dc085030e77a7b1b79285c5c3bc2203c2a305d3e394e825046b2fba848`  
		Last Modified: Tue, 23 May 2023 05:54:09 GMT  
		Size: 1.4 MB (1385341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:027c2e77ce4f6308dfd0e4e8c48865093c1a331bf262e2b3430af923905ecf1b`  
		Last Modified: Tue, 23 May 2023 05:54:08 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:standalone` - linux; arm64 variant v8

```console
$ docker pull adminer@sha256:5c47bd19cef0242b3fd68a8f9d3391de1e5fde897ddbf8915c6b30438f3063bb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.3 MB (94325092 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c2bd14ed3796aa8481743bc95a7fc8dd8218d08c8b14983b764d3d0ff0dea045`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Tue, 23 May 2023 00:43:08 GMT
ADD file:a823391455122220a061ff349b66ee33413e968447ec5ba4bd544d9182fa2fbe in / 
# Tue, 23 May 2023 00:43:08 GMT
CMD ["bash"]
# Tue, 23 May 2023 05:50:11 GMT
STOPSIGNAL SIGINT
# Tue, 23 May 2023 05:50:32 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 05:50:33 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 23 May 2023 05:50:33 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 23 May 2023 05:50:33 GMT
WORKDIR /var/www/html
# Tue, 23 May 2023 05:50:33 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 23 May 2023 05:50:33 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 23 May 2023 05:50:33 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 23 May 2023 05:50:34 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 23 May 2023 05:50:43 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 23 May 2023 05:50:43 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 23 May 2023 05:50:44 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 23 May 2023 05:50:44 GMT
USER adminer
# Tue, 23 May 2023 05:50:44 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Tue, 23 May 2023 05:50:44 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:b04fae59f135dd79280e4a6da39408e04c6d703c617cbcb1c524dfe6f2962fe5`  
		Last Modified: Tue, 23 May 2023 00:45:45 GMT  
		Size: 53.7 MB (53692612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9efc47f16e1a38ba0dcb257d5ce8cdb437133352964cc19558d888d0932e82dc`  
		Last Modified: Tue, 23 May 2023 05:51:17 GMT  
		Size: 39.2 MB (39242969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71d893cd37b35b46043be34343f81e912e3f7802d60d2d2a8b8cc70f4e6940dd`  
		Last Modified: Tue, 23 May 2023 05:51:10 GMT  
		Size: 387.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc65de0120389b991d25f8734bd9373a7391404e080fdb9e484b37dc40e7644f`  
		Last Modified: Tue, 23 May 2023 05:51:10 GMT  
		Size: 1.9 KB (1884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27230442fa5e0410cf3de04256ccf57b2e7302728b4087e0f0590ba564e5675c`  
		Last Modified: Tue, 23 May 2023 05:51:10 GMT  
		Size: 1.5 KB (1477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10c5d0a18ff3f8031274083de4aa9ae8f319e6f788078ca689da0854380f121b`  
		Last Modified: Tue, 23 May 2023 05:51:11 GMT  
		Size: 1.4 MB (1385273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40241383ff75bdf25057bb86ad6c6fbd5a5521ded9c5714dc795d5772da27c31`  
		Last Modified: Tue, 23 May 2023 05:51:10 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:standalone` - linux; 386

```console
$ docker pull adminer@sha256:46c9179dfae160988ca0ca9287f2b99f8fa69578f07fa9f12d55b6834a5f006e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.0 MB (96977311 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e8c530ce1b0d669c252acd2f9795658f6723f0fa54849ce2909d38b4e1a1cc3`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Tue, 23 May 2023 00:39:14 GMT
ADD file:acdf45f51b991111aa6c929fedd4e8de03e5d42578cca2f895f74697c3c66e33 in / 
# Tue, 23 May 2023 00:39:15 GMT
CMD ["bash"]
# Tue, 23 May 2023 01:52:16 GMT
STOPSIGNAL SIGINT
# Tue, 23 May 2023 01:52:44 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 01:52:45 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 23 May 2023 01:52:46 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 23 May 2023 01:52:46 GMT
WORKDIR /var/www/html
# Tue, 23 May 2023 01:52:46 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 23 May 2023 01:52:46 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 23 May 2023 01:52:46 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 23 May 2023 01:52:46 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 23 May 2023 01:53:00 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 23 May 2023 01:53:00 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 23 May 2023 01:53:00 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 23 May 2023 01:53:00 GMT
USER adminer
# Tue, 23 May 2023 01:53:00 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Tue, 23 May 2023 01:53:00 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:c377769761bd9f2bd79d27a4f6dfa29be1047f4e6e8df1653027ef5262e020bb`  
		Last Modified: Tue, 23 May 2023 00:44:01 GMT  
		Size: 56.0 MB (56029173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ccfbef2dc091aa63e1c4068d4e51035fe70449929a0e82db9bb9d3730b07ca4`  
		Last Modified: Tue, 23 May 2023 01:53:38 GMT  
		Size: 39.6 MB (39558587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e9ff94ea7737d188f37d6bd28d8ec1dec20fbd26e2648dd5b2cea2dcbf11016`  
		Last Modified: Tue, 23 May 2023 01:53:28 GMT  
		Size: 388.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6de85ff0c36f6ae701d1a6bca9cd6c60b91eaed71146d073516bf0bb476041eb`  
		Last Modified: Tue, 23 May 2023 01:53:28 GMT  
		Size: 1.9 KB (1872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fde161dd0b56d09e57ed9225e0e3fa614aa6c14ea9a856b6a687c495650f52c`  
		Last Modified: Tue, 23 May 2023 01:53:29 GMT  
		Size: 1.5 KB (1477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:136b9a9560e895e23e37330f90686447d760e22ddc1ca5c4839e3a38f87ae9a3`  
		Last Modified: Tue, 23 May 2023 01:53:28 GMT  
		Size: 1.4 MB (1385323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a724f07aad7317bbf5b7692b36304b758f4720ca86d750560103b4ccc3f9767a`  
		Last Modified: Tue, 23 May 2023 01:53:28 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:standalone` - linux; mips64le

```console
$ docker pull adminer@sha256:17a7746cc27280ea06f4662bd60bc2ed6c9c02f919adf8066a3531fd5419e8af
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.6 MB (92605070 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:058cb35cd16719c7d4d1f8cf57101e056642ed2dad21501c5971601ee468858b`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Tue, 23 May 2023 01:09:32 GMT
ADD file:c4481c512145c216c0696b57b55890f49935871b934f1e23b24238871e88158c in / 
# Tue, 23 May 2023 01:09:38 GMT
CMD ["bash"]
# Tue, 23 May 2023 18:53:54 GMT
STOPSIGNAL SIGINT
# Tue, 23 May 2023 18:55:52 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 18:55:58 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 23 May 2023 18:56:05 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 23 May 2023 18:56:08 GMT
WORKDIR /var/www/html
# Tue, 23 May 2023 18:56:12 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 23 May 2023 18:56:15 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 23 May 2023 18:56:18 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 23 May 2023 18:56:22 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 23 May 2023 18:57:12 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 23 May 2023 18:57:15 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 23 May 2023 18:57:18 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 23 May 2023 18:57:22 GMT
USER adminer
# Tue, 23 May 2023 18:57:25 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Tue, 23 May 2023 18:57:28 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:3e72533d17b613b0fe30563d66f03850909770c19b7e44c2a94654ab9ba9aaad`  
		Last Modified: Tue, 23 May 2023 01:18:39 GMT  
		Size: 53.3 MB (53261128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ced00eabec79cf2e1b438aa231ce9e756ed81ac67669dd32e217a885a6f8793c`  
		Last Modified: Tue, 23 May 2023 18:59:53 GMT  
		Size: 38.0 MB (37953481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcb266ffac39a303c37c056478fa428825e137325288690405149c26d446492d`  
		Last Modified: Tue, 23 May 2023 18:59:26 GMT  
		Size: 397.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4117b89d7bcbc5a78e6052b4fd67ff9d80babad4b6aa980d2d5a16f6515a5b06`  
		Last Modified: Tue, 23 May 2023 18:59:26 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6680dc122c68c76ba358cfb5095259025f15304ed54679ecd485f6b4a619f06b`  
		Last Modified: Tue, 23 May 2023 18:59:26 GMT  
		Size: 1.5 KB (1484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e93a9f69f5974657e9a68bbada5915f0bda15cf95aa794e84e6bdbdcbfce1adf`  
		Last Modified: Tue, 23 May 2023 18:59:27 GMT  
		Size: 1.4 MB (1386352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e16f2eb96178b0ac395d733460a0b2f0bb45a98e8a2d303840e1f8895c8a0ffc`  
		Last Modified: Tue, 23 May 2023 18:59:26 GMT  
		Size: 493.0 B  
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
