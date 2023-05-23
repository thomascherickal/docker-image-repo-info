## `adminer:4-standalone`

```console
$ docker pull adminer@sha256:f6a7c6402956a6c898297cf69d5edd9c92864290b5c58de6024dfbb8b5887d73
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
$ docker pull adminer@sha256:d91de255f3d3597661309ce8d4c1227022011c1a52125940bb05a2477f6d8db0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.9 MB (95925419 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78893d63a9ccd60034e130ecf636ab8454c0107ecd4b764a67a18d7f32010bb2`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Tue, 02 May 2023 23:46:50 GMT
ADD file:fc290cf8ddb984325474583faa79c5a98c5ea0ec7f606bf360251f63acecf389 in / 
# Tue, 02 May 2023 23:46:51 GMT
CMD ["bash"]
# Wed, 03 May 2023 19:49:00 GMT
STOPSIGNAL SIGINT
# Wed, 03 May 2023 19:49:21 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 19:49:22 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 03 May 2023 19:49:22 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 03 May 2023 19:49:22 GMT
WORKDIR /var/www/html
# Wed, 03 May 2023 19:49:22 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 03 May 2023 19:49:22 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 03 May 2023 19:49:22 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 03 May 2023 19:49:22 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 03 May 2023 19:49:36 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 03 May 2023 19:49:36 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 03 May 2023 19:49:36 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 03 May 2023 19:49:36 GMT
USER adminer
# Wed, 03 May 2023 19:49:36 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 03 May 2023 19:49:36 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:918547b9432687b1e1d238e82dc1e0ea0b736aafbf3c402eea98c6db81a9cb65`  
		Last Modified: Tue, 02 May 2023 23:49:58 GMT  
		Size: 55.0 MB (55049070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bf072a3c195640cfbba5c4eb88052f27aee1f9da5123dda872846243732750f`  
		Last Modified: Wed, 03 May 2023 19:50:13 GMT  
		Size: 39.5 MB (39486685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3683a3b1017a786123671e0857d74739255f46ee16376a6855db0c322c919a3d`  
		Last Modified: Wed, 03 May 2023 19:50:05 GMT  
		Size: 394.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51a450f50bf33686348806dbff92cd96b1a2053ac929f969b2cf3c0acee62835`  
		Last Modified: Wed, 03 May 2023 19:50:05 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9988d325d7ed56c3f96299601c8fd0daed11708badf604a60a75c2ff28d317d`  
		Last Modified: Wed, 03 May 2023 19:50:05 GMT  
		Size: 1.5 KB (1478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d88de51838f21c05c13e3170be01f945f3c3bcbb575b562e8ed076b7a47f7b9d`  
		Last Modified: Wed, 03 May 2023 19:50:05 GMT  
		Size: 1.4 MB (1385419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccbdbbaee470be350f6253a8513cdd0aeecddfc1d934d3266f90c5577b5df9f2`  
		Last Modified: Wed, 03 May 2023 19:50:05 GMT  
		Size: 491.0 B  
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
$ docker pull adminer@sha256:dbb3bb5cfaf6fa4f99c880a9171306b3752153656592b4dff4d9aa92b1ba847e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.8 MB (87781999 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee7f1cc429b88e4cbde5db9596043ebea60e58cc1068dca2b153afb53bc094f2`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Tue, 02 May 2023 23:47:46 GMT
ADD file:668ced72eb3825a6cfd123f77fed6c64b8ad5bf1f4aa8e78ede9512198ca65ad in / 
# Tue, 02 May 2023 23:47:47 GMT
CMD ["bash"]
# Wed, 03 May 2023 21:49:12 GMT
STOPSIGNAL SIGINT
# Wed, 03 May 2023 21:49:34 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:49:35 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 03 May 2023 21:49:35 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 03 May 2023 21:49:35 GMT
WORKDIR /var/www/html
# Wed, 03 May 2023 21:49:35 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 03 May 2023 21:49:35 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 03 May 2023 21:49:35 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 03 May 2023 21:49:36 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 03 May 2023 21:49:47 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 03 May 2023 21:49:47 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 03 May 2023 21:49:47 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 03 May 2023 21:49:47 GMT
USER adminer
# Wed, 03 May 2023 21:49:47 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 03 May 2023 21:49:47 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:755944445ece6eac276e067f465680b57daac59a0ed9ce97e7c501f1cde8621d`  
		Last Modified: Tue, 02 May 2023 23:51:06 GMT  
		Size: 50.2 MB (50210011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4484dc44c04f72dc48099f09709fc3899b8d4b4bb1136a349395035a546dffad`  
		Last Modified: Wed, 03 May 2023 21:50:22 GMT  
		Size: 36.2 MB (36182453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b33b475a175bcefacd90b909ac03e5552e23425efe2470f17f08d6afb2c3e512`  
		Last Modified: Wed, 03 May 2023 21:50:14 GMT  
		Size: 386.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db9479c6dff0b42486f52cd4ce1f7fa2f1613302e1fcf892bdb7a17d36024cb8`  
		Last Modified: Wed, 03 May 2023 21:50:14 GMT  
		Size: 1.9 KB (1870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9443b2852d24e296cf30eb4ac8a89e8981dba03543c57d1a3a1f4b72eba01d87`  
		Last Modified: Wed, 03 May 2023 21:50:14 GMT  
		Size: 1.5 KB (1476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6e517a92f41f859fd277d6b6de143c017c4f0f6623f95c355a771e2b8f81787`  
		Last Modified: Wed, 03 May 2023 21:50:14 GMT  
		Size: 1.4 MB (1385314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d03da9a1407bd14fe6b654504046d233ee553b31ab2b8e70a372b961ed33d90`  
		Last Modified: Wed, 03 May 2023 21:50:14 GMT  
		Size: 489.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-standalone` - linux; arm64 variant v8

```console
$ docker pull adminer@sha256:195c05e88c549ff323f21435965c2e6677fe8cb8c5d8ee7b76a6de45404ccef6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.3 MB (94324844 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:116d9739cd4b1dcd81fff9a99d2363ec5d41f2ad74bdd346bd8fac26bbff9d06`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 03 May 2023 00:22:41 GMT
ADD file:f930fdb659332a615b0042ca415d6d7feda9ba6b2f58222e3e5bbed326db4d40 in / 
# Wed, 03 May 2023 00:22:42 GMT
CMD ["bash"]
# Wed, 03 May 2023 17:16:28 GMT
STOPSIGNAL SIGINT
# Wed, 03 May 2023 17:16:48 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 17:16:48 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 03 May 2023 17:16:49 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 03 May 2023 17:16:49 GMT
WORKDIR /var/www/html
# Wed, 03 May 2023 17:16:49 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 03 May 2023 17:16:49 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 03 May 2023 17:16:49 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 03 May 2023 17:16:49 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 03 May 2023 17:17:01 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 03 May 2023 17:17:01 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 03 May 2023 17:17:01 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 03 May 2023 17:17:01 GMT
USER adminer
# Wed, 03 May 2023 17:17:01 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 03 May 2023 17:17:01 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:d677c78be691f8dcbe9d44ce576b97ad205b3dd78557dc62794e59eb19553ee9`  
		Last Modified: Wed, 03 May 2023 00:25:31 GMT  
		Size: 53.7 MB (53692705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f390884cbdf7437b9adc33383ab11920275f677b21cac4528c0f1de12655fd9`  
		Last Modified: Wed, 03 May 2023 17:17:34 GMT  
		Size: 39.2 MB (39242564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a168533f0631d50dbab6d3eb2174b05de1644496fc8c5936489f20c2d691f898`  
		Last Modified: Wed, 03 May 2023 17:17:28 GMT  
		Size: 389.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:822087af0bdecd28923ab32fa9fc2e00566083e121bcaf67c0a2e6598c52d149`  
		Last Modified: Wed, 03 May 2023 17:17:28 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f5107c70315eac1012c7e38609673cccd890714b8fcf925196c063dcac78e70`  
		Last Modified: Wed, 03 May 2023 17:17:28 GMT  
		Size: 1.5 KB (1478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56a12d03495dfb72be5d6277086be719ff559fa5ef937eef42793040eab4138a`  
		Last Modified: Wed, 03 May 2023 17:17:29 GMT  
		Size: 1.4 MB (1385335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eca70bf37e696c8b2a1c3fad1f023f0c22794bcd2204a7ea0a5fa5de57829ff`  
		Last Modified: Wed, 03 May 2023 17:17:28 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-standalone` - linux; 386

```console
$ docker pull adminer@sha256:e5e906fafadd242d3947ff7a91e16ed086da26deca9cfa76db116943301c2753
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.0 MB (96977075 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f57b6c754f54bbc8be58f5323c9e60014dc7f4778c03b2ea35c9fc643497cb7`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 03 May 2023 00:00:45 GMT
ADD file:59d53253d7691be0330c735eb4b57791a8fc5894572d3deaeb7138cce45132ad in / 
# Wed, 03 May 2023 00:00:46 GMT
CMD ["bash"]
# Wed, 03 May 2023 22:24:06 GMT
STOPSIGNAL SIGINT
# Wed, 03 May 2023 22:24:33 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 22:24:35 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 03 May 2023 22:24:35 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 03 May 2023 22:24:35 GMT
WORKDIR /var/www/html
# Wed, 03 May 2023 22:24:35 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 03 May 2023 22:24:35 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 03 May 2023 22:24:36 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 03 May 2023 22:24:36 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 03 May 2023 22:24:49 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 03 May 2023 22:24:49 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 03 May 2023 22:24:49 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 03 May 2023 22:24:49 GMT
USER adminer
# Wed, 03 May 2023 22:24:50 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 03 May 2023 22:24:50 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:6ac0eb37fce5e6fca952bf804df5de5ebb63724d4d44bf23abc5d5736ee32afd`  
		Last Modified: Wed, 03 May 2023 00:04:44 GMT  
		Size: 56.0 MB (56029150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cae728af6fba3d6528233874fa5b3b171e220be7e7b44a9bd9abacfd0feb22d`  
		Last Modified: Wed, 03 May 2023 22:25:31 GMT  
		Size: 39.6 MB (39558398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1037b8cc7a58279264bc3170e115ec9c44bc4d092cdf46140a9e8dcb932aacf`  
		Last Modified: Wed, 03 May 2023 22:25:21 GMT  
		Size: 391.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ec6f63c3dcb7f6e79bd316877e6c325582cc60ef273140751deb3269b3cd1b7`  
		Last Modified: Wed, 03 May 2023 22:25:21 GMT  
		Size: 1.9 KB (1870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a583c069cffab4f61bf420d69b8998e5292ba0ef9c96037d8918e683d946bb3`  
		Last Modified: Wed, 03 May 2023 22:25:21 GMT  
		Size: 1.5 KB (1477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9e5c64850b3828949a1a717004d1be719a8f39998693f62cb72864f4f0df1b6`  
		Last Modified: Wed, 03 May 2023 22:25:21 GMT  
		Size: 1.4 MB (1385299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15fc8bb0e2bcda06beb495530dc8cb3a049eb559b769ef65a2030ce875b4fee2`  
		Last Modified: Wed, 03 May 2023 22:25:21 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-standalone` - linux; mips64le

```console
$ docker pull adminer@sha256:2151d2d2c1ac42085137c3f80a64dcd3b212051aed1f4f2fb1e648fc8164c959
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.6 MB (92603745 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9c42f1be3fdbd9ef409ffe2e82241d5713f0026d5df02b66cbfa628c007a318`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Tue, 02 May 2023 23:49:00 GMT
ADD file:578ecc56a9b7fe8d8ebea195fcf6c3a8d78941e9c4b5da71f8b4b821b6db9f87 in / 
# Tue, 02 May 2023 23:49:06 GMT
CMD ["bash"]
# Thu, 04 May 2023 02:09:47 GMT
STOPSIGNAL SIGINT
# Thu, 04 May 2023 02:11:39 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Thu, 04 May 2023 02:11:45 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Thu, 04 May 2023 02:11:52 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 04 May 2023 02:11:55 GMT
WORKDIR /var/www/html
# Thu, 04 May 2023 02:11:58 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 04 May 2023 02:12:02 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 04 May 2023 02:12:05 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 04 May 2023 02:12:08 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 04 May 2023 02:12:59 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 04 May 2023 02:13:02 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 04 May 2023 02:13:05 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 04 May 2023 02:13:08 GMT
USER adminer
# Thu, 04 May 2023 02:13:11 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Thu, 04 May 2023 02:13:15 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:4753f7ffbf9149ce1d9cc543018c00a2946e14c08b1a2aa37a0ac347d08b0e29`  
		Last Modified: Tue, 02 May 2023 23:57:30 GMT  
		Size: 53.3 MB (53261131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fbaadac6c79d2d9500484c388cf7882f73216f4710b4d3353960b19a23c4d15`  
		Last Modified: Thu, 04 May 2023 02:15:45 GMT  
		Size: 38.0 MB (37952226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e7a0d66f0135bf7a91f2083af0457778bea9129372b3d2366f7d0f7d82368f8`  
		Last Modified: Thu, 04 May 2023 02:15:18 GMT  
		Size: 394.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dbabe4b2df1fdb7e9b73fa02bcc7b1cc2b18711cac7085ea3b322e25ac05112`  
		Last Modified: Thu, 04 May 2023 02:15:18 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bc0e79d70d5bff66df877a51e0890c1e81c0fa5cf1878e0f05541fd41cc3999`  
		Last Modified: Thu, 04 May 2023 02:15:18 GMT  
		Size: 1.5 KB (1483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93a3c4e06641c75d169f92921d976676b0f592cb7739da26f6b8e23742628a2b`  
		Last Modified: Thu, 04 May 2023 02:15:19 GMT  
		Size: 1.4 MB (1386287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2355ccb81311529d35b80c63ec556b82a63b8b89e88bdfbb153016d48bd43ec1`  
		Last Modified: Thu, 04 May 2023 02:15:19 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-standalone` - linux; ppc64le

```console
$ docker pull adminer@sha256:45cbccffc5655429c06fd52ae22905487f7d1c99b8deb5b1910d1e7c32dc13a5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.3 MB (101253884 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a82b56420b534a15a2e77e7db5d92218d3db19f7205c96a23f25db01247cf631`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 03 May 2023 00:31:28 GMT
ADD file:39e4cb0fbb759c45690e34c0392acb89ac2b180e261843426f24ce0fe0189e84 in / 
# Wed, 03 May 2023 00:31:32 GMT
CMD ["bash"]
# Wed, 03 May 2023 23:43:57 GMT
STOPSIGNAL SIGINT
# Wed, 03 May 2023 23:45:35 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 23:45:39 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 03 May 2023 23:45:42 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 03 May 2023 23:45:42 GMT
WORKDIR /var/www/html
# Wed, 03 May 2023 23:45:43 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 03 May 2023 23:45:43 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 03 May 2023 23:45:44 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 03 May 2023 23:45:45 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 03 May 2023 23:46:13 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 03 May 2023 23:46:13 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 03 May 2023 23:46:14 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 03 May 2023 23:46:14 GMT
USER adminer
# Wed, 03 May 2023 23:46:14 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 03 May 2023 23:46:15 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:0c356fc795c1bdfb3883bd87c64008fffdc0d8bdc8f0ecb386016a31fe5864fb`  
		Last Modified: Wed, 03 May 2023 00:36:26 GMT  
		Size: 58.9 MB (58924002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aecc1e39e985f420d8864679a74694229a7c9158c5b1e1fe8f9205862df74e62`  
		Last Modified: Wed, 03 May 2023 23:47:23 GMT  
		Size: 40.9 MB (40939949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4728deff688fccf04b30db5cc3f38a0de4465c2a9b6ad3a1c27c3a0b09aaf2e`  
		Last Modified: Wed, 03 May 2023 23:47:10 GMT  
		Size: 397.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66347f5c3955c3b5e7941771e52c89fb19898cc1743fbc07fbba27be78c3bf2b`  
		Last Modified: Wed, 03 May 2023 23:47:10 GMT  
		Size: 1.9 KB (1877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1db2be9fe69919c5a20ff442f1946faa16f2fc2625d8040d89e4394156e6ad0e`  
		Last Modified: Wed, 03 May 2023 23:47:10 GMT  
		Size: 1.5 KB (1481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89168b7cf83d4b0299c1eb43b4a0d80a4411b2b151be7a9f490deaa496092595`  
		Last Modified: Wed, 03 May 2023 23:47:10 GMT  
		Size: 1.4 MB (1385685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70bff4386c8edcebeb1632c87b6016770835ce402f9b07a3b46cc5378d08aea4`  
		Last Modified: Wed, 03 May 2023 23:47:10 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-standalone` - linux; s390x

```console
$ docker pull adminer@sha256:2609f0f660d45880a6913419ed99f4e294091a5d7fab49931611f2a2e8fa7a9e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.7 MB (93690280 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e04cde3340f6213e9c551b7ef188ef212574a72ecba99e32b004816ecba717c`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 03 May 2023 03:41:38 GMT
ADD file:c518f614279e4b34edf6331c6ed36be5ff220ae28cf9bda3433158c45c858caa in / 
# Wed, 03 May 2023 03:41:43 GMT
CMD ["bash"]
# Wed, 03 May 2023 22:35:26 GMT
STOPSIGNAL SIGINT
# Wed, 03 May 2023 22:35:47 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 22:35:50 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 03 May 2023 22:35:51 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 03 May 2023 22:35:51 GMT
WORKDIR /var/www/html
# Wed, 03 May 2023 22:35:51 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 03 May 2023 22:35:51 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 03 May 2023 22:35:51 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 03 May 2023 22:35:51 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 03 May 2023 22:36:01 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 03 May 2023 22:36:01 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 03 May 2023 22:36:01 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 03 May 2023 22:36:01 GMT
USER adminer
# Wed, 03 May 2023 22:36:01 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 03 May 2023 22:36:02 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:c05abc724fd71022253a33351707dac122d940b2d0569f0bf779ac1416f31abd`  
		Last Modified: Wed, 03 May 2023 03:44:45 GMT  
		Size: 53.3 MB (53282138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44687bf78162855c3156d48d92e8a919fda5922bd1619551e4a22ac2de603f9b`  
		Last Modified: Wed, 03 May 2023 22:36:39 GMT  
		Size: 39.0 MB (39018454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ff2c29bb9a356e05b8af3c228678a4589d166a251a4e54ea650c3c331f3cad8`  
		Last Modified: Wed, 03 May 2023 22:36:32 GMT  
		Size: 388.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c48866ad7c370b808f1e8ff374a01dfe9c37fbf3efb7e5f39dc5e5759b49052b`  
		Last Modified: Wed, 03 May 2023 22:36:32 GMT  
		Size: 1.9 KB (1880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d130ca3dddb7ce629d8e889a54b0bdb04ae63f05f8e3e7e09c07b74e8632889`  
		Last Modified: Wed, 03 May 2023 22:36:32 GMT  
		Size: 1.5 KB (1476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9afac261a3dca06612a5da791e63cb428dee7dfbdd096385b02268376ba846e`  
		Last Modified: Wed, 03 May 2023 22:36:32 GMT  
		Size: 1.4 MB (1385451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3b44ffdf8e3a1aaaccca75652e4d57738db98275be5014fd8aaa4849f67820b`  
		Last Modified: Wed, 03 May 2023 22:36:32 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
