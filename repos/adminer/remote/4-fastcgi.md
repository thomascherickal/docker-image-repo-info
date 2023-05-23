## `adminer:4-fastcgi`

```console
$ docker pull adminer@sha256:f329971451b740ba7f568d84d9f9815a8b74f54ba9cf47db66b48b179eee9891
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
$ docker pull adminer@sha256:0d87cb72964832994fc1354b8285fc0061a53a7ad5e774d8f3a494361ffdd477
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.9 MB (95928185 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bae1c10472424db29821e009ff60442012b8df12fdc2c5f3c975d669b9d96f0c`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

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
# Wed, 03 May 2023 19:49:40 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Wed, 03 May 2023 19:49:41 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 03 May 2023 19:49:41 GMT
WORKDIR /var/www/html
# Wed, 03 May 2023 19:49:41 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 03 May 2023 19:49:41 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 03 May 2023 19:49:41 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 03 May 2023 19:49:42 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 03 May 2023 19:49:52 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 03 May 2023 19:49:52 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 03 May 2023 19:49:52 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 03 May 2023 19:49:52 GMT
USER adminer
# Wed, 03 May 2023 19:49:53 GMT
CMD ["php-fpm7.4"]
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
	-	`sha256:35b78adfc36b0ceeee1593642aeb708ad89deafcc00169458bb2fb6b5fc1f7f8`  
		Last Modified: Wed, 03 May 2023 19:50:29 GMT  
		Size: 2.7 KB (2712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6da87e103242a5d24f75e634bf6e2e0cecff567d0cfb134cf8580ad6f72cf8f8`  
		Last Modified: Wed, 03 May 2023 19:50:29 GMT  
		Size: 1.9 KB (1880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d131f2b99e8963f94214d16359506ac31ccbe7b358cd1dfe48b52f93e3dfce56`  
		Last Modified: Wed, 03 May 2023 19:50:29 GMT  
		Size: 1.5 KB (1477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2715d1951ac6ca080298a7af6c5528d98926e52ea25c4c8992d39c43b6c8f0d3`  
		Last Modified: Wed, 03 May 2023 19:50:30 GMT  
		Size: 1.4 MB (1385478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7e908632d710029d146621117e58eedcfaabf3e27c23547b12e3292b9602802`  
		Last Modified: Wed, 03 May 2023 19:50:29 GMT  
		Size: 489.0 B  
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
$ docker pull adminer@sha256:646679bc63f653334613be5948da3aa1529627752196f8c1ad2d8e0989249e9e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.8 MB (87784770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e5674b024863ad12ccd950ab5f8913f802cf6dca92cb5e62698935a8a65d99b`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

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
# Wed, 03 May 2023 21:49:52 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Wed, 03 May 2023 21:49:53 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 03 May 2023 21:49:53 GMT
WORKDIR /var/www/html
# Wed, 03 May 2023 21:49:53 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 03 May 2023 21:49:53 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 03 May 2023 21:49:53 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 03 May 2023 21:49:53 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 03 May 2023 21:50:04 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 03 May 2023 21:50:04 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 03 May 2023 21:50:04 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 03 May 2023 21:50:04 GMT
USER adminer
# Wed, 03 May 2023 21:50:04 GMT
CMD ["php-fpm7.4"]
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
	-	`sha256:0e90698d60fb81f4c2ca9f4bbf0034e19c6f38ab8b80358727902b82f5d5008e`  
		Last Modified: Wed, 03 May 2023 21:50:37 GMT  
		Size: 2.7 KB (2706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71354c00eebfe761842cac938e9afb485ca92ca8467d86395513a008bfc1d041`  
		Last Modified: Wed, 03 May 2023 21:50:37 GMT  
		Size: 1.9 KB (1870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:631e79f4b3b776a89da2a62b5a0e64df51dc7173f8f221fd532804719b3ca583`  
		Last Modified: Wed, 03 May 2023 21:50:37 GMT  
		Size: 1.5 KB (1475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:944741757be8820dedc78d237fb2795c68b86a1418019aecc9f040352b8b5ffa`  
		Last Modified: Wed, 03 May 2023 21:50:38 GMT  
		Size: 1.4 MB (1385381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70d69b5316b480275572598ed2ab38467ad483e3184cebb4a149c122726f9673`  
		Last Modified: Wed, 03 May 2023 21:50:37 GMT  
		Size: 488.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-fastcgi` - linux; arm64 variant v8

```console
$ docker pull adminer@sha256:b27c31449632b9a65821b105ca7a98f4c07be23f490c615aa03a85535f55dc81
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.3 MB (94327532 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3fe023c677da662d509e1abc3623a760d8f4cefcb81fb742f24df648a056f06`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

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
# Wed, 03 May 2023 17:17:08 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Wed, 03 May 2023 17:17:09 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 03 May 2023 17:17:09 GMT
WORKDIR /var/www/html
# Wed, 03 May 2023 17:17:09 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 03 May 2023 17:17:09 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 03 May 2023 17:17:09 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 03 May 2023 17:17:09 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 03 May 2023 17:17:19 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 03 May 2023 17:17:19 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 03 May 2023 17:17:19 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 03 May 2023 17:17:19 GMT
USER adminer
# Wed, 03 May 2023 17:17:19 GMT
CMD ["php-fpm7.4"]
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
	-	`sha256:d4668f312f76168b5ec5ba462cd882cdb5dd938580a0f9d0ea34136fdd309c72`  
		Last Modified: Wed, 03 May 2023 17:17:50 GMT  
		Size: 2.7 KB (2709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:562094df7f95bedb11bf4ff8740f5df7952de583d03846e7c00d5de93af31879`  
		Last Modified: Wed, 03 May 2023 17:17:50 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0826dfda302501033f4c7310b25337cfbc0d74c8fc7f0ebf783fb1cfa5736969`  
		Last Modified: Wed, 03 May 2023 17:17:51 GMT  
		Size: 1.5 KB (1475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f74a7a67f6c6592e208a69eab35b38e43d39e7d9b0fc229867c1c5a266007e50`  
		Last Modified: Wed, 03 May 2023 17:17:51 GMT  
		Size: 1.4 MB (1385319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bf167363a0d5443d97b987ebeb028bb7549d031b7cf879b3873ff6fc85fa2d4`  
		Last Modified: Wed, 03 May 2023 17:17:50 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-fastcgi` - linux; 386

```console
$ docker pull adminer@sha256:d55625ac17606061655be73c0f4c5b32924b7da852a18106f026e371fd509872
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.0 MB (96979809 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dea6d4afd94dfcf10b4b24a4b041e39e4e11a021ebc4e496497e6e4599318d90`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

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
# Wed, 03 May 2023 22:24:54 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Wed, 03 May 2023 22:24:55 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 03 May 2023 22:24:55 GMT
WORKDIR /var/www/html
# Wed, 03 May 2023 22:24:55 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 03 May 2023 22:24:55 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 03 May 2023 22:24:55 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 03 May 2023 22:24:55 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 03 May 2023 22:25:08 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 03 May 2023 22:25:08 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 03 May 2023 22:25:08 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 03 May 2023 22:25:08 GMT
USER adminer
# Wed, 03 May 2023 22:25:09 GMT
CMD ["php-fpm7.4"]
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
	-	`sha256:cf737bf5edd1f0bd54061cd0e4e29cde149d9746d76c0713069aecbea3897791`  
		Last Modified: Wed, 03 May 2023 22:25:48 GMT  
		Size: 2.7 KB (2709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fc375123754fe30e5111b6103ada5347e07f773590d16f98775f244df1e9aa1`  
		Last Modified: Wed, 03 May 2023 22:25:47 GMT  
		Size: 1.9 KB (1871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b819f04679332b43e6f2fe689f9237b0b9e15b4bec6e7ddd421866ae3969520f`  
		Last Modified: Wed, 03 May 2023 22:25:47 GMT  
		Size: 1.5 KB (1474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e76b51242b22c69e07452401415aecc54e1ec41ae6b57bc7ab94435d6843366`  
		Last Modified: Wed, 03 May 2023 22:25:48 GMT  
		Size: 1.4 MB (1385325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5764dd7a1796e9d47d188c18b465e48d655f5c3bdeaa52f1df4db28ba5585e1c`  
		Last Modified: Wed, 03 May 2023 22:25:48 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-fastcgi` - linux; mips64le

```console
$ docker pull adminer@sha256:996c01eb89f4de0a8b44528863734bceca1924e645f3235c5809d39949d42dc9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.6 MB (92606469 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5df13426dfcf12cbf84a6c899b9fe3801f2e7ccd34896c112bba64d0a47d1906`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

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
# Thu, 04 May 2023 02:13:33 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Thu, 04 May 2023 02:13:39 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 04 May 2023 02:13:42 GMT
WORKDIR /var/www/html
# Thu, 04 May 2023 02:13:45 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 04 May 2023 02:13:48 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 04 May 2023 02:13:52 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 04 May 2023 02:13:55 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 04 May 2023 02:14:45 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 04 May 2023 02:14:48 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 04 May 2023 02:14:51 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 04 May 2023 02:14:54 GMT
USER adminer
# Thu, 04 May 2023 02:14:58 GMT
CMD ["php-fpm7.4"]
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
	-	`sha256:18799b12dd897d502f6909aa507f2a1d99dafaec0112b313a5fdc0129d8f699f`  
		Last Modified: Thu, 04 May 2023 02:16:03 GMT  
		Size: 2.7 KB (2716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44bfde8bb754c97f204ea60733274e9911a1ec60abe450cb3380353944f6fda8`  
		Last Modified: Thu, 04 May 2023 02:16:03 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdaa0ed0344d20ff73e5c0b0629b4e2a48a77653e0e8796fadf1560a613cd4eb`  
		Last Modified: Thu, 04 May 2023 02:16:03 GMT  
		Size: 1.5 KB (1479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aea8a2913a286fd80ef7c635dfd9c55c06b0dee3b0cc6d19198b11b347773508`  
		Last Modified: Thu, 04 May 2023 02:16:04 GMT  
		Size: 1.4 MB (1386295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e75492cddad11b445a548326a0fa92c25b5ef0d20859f1bad0d4de51793c190`  
		Last Modified: Thu, 04 May 2023 02:16:03 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-fastcgi` - linux; ppc64le

```console
$ docker pull adminer@sha256:596377ea14d0b4e013dd1dc8c27b8a5d2e652f91580ca0a5eb4c7eadaf4b475f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.3 MB (101256574 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cffb55cd093b679384dc7755a0e120762cdd9b39870418c961808b6e55868979`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

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
# Wed, 03 May 2023 23:46:22 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Wed, 03 May 2023 23:46:26 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 03 May 2023 23:46:27 GMT
WORKDIR /var/www/html
# Wed, 03 May 2023 23:46:27 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 03 May 2023 23:46:28 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 03 May 2023 23:46:28 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 03 May 2023 23:46:29 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 03 May 2023 23:46:53 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 03 May 2023 23:46:53 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 03 May 2023 23:46:54 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 03 May 2023 23:46:54 GMT
USER adminer
# Wed, 03 May 2023 23:46:54 GMT
CMD ["php-fpm7.4"]
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
	-	`sha256:ab78324061339154d6fef3e46f4aca105c18a570bb1dce099a3a9c6ee8635527`  
		Last Modified: Wed, 03 May 2023 23:47:41 GMT  
		Size: 2.7 KB (2713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25e162c45027d0f8f90d645874790e483b430334bcce6b4d07531145d81afc17`  
		Last Modified: Wed, 03 May 2023 23:47:41 GMT  
		Size: 1.9 KB (1885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebac1e51880f44c1625369cccb82df3dde5675456ca28d6a851177e6a97a22f7`  
		Last Modified: Wed, 03 May 2023 23:47:41 GMT  
		Size: 1.5 KB (1480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26501eefae998ad6d8b8aa80733c6f7b230a17959ca6a9b7725b3a3edeb96a5d`  
		Last Modified: Wed, 03 May 2023 23:47:41 GMT  
		Size: 1.4 MB (1385660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce06893db4ec804653a8e5738777cfcc72c14b6409054352a011226b26197fc2`  
		Last Modified: Wed, 03 May 2023 23:47:41 GMT  
		Size: 488.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-fastcgi` - linux; s390x

```console
$ docker pull adminer@sha256:53dd581f577325979a13aa06db43da4bf50dcaddbd9dc009509e9387da2f572e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.7 MB (93692976 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a2b33a6ce5b59bde136990c731cdfe5b320e8c7a0def62abc7ec6b94619d69a`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

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
# Wed, 03 May 2023 22:36:07 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Wed, 03 May 2023 22:36:08 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 03 May 2023 22:36:08 GMT
WORKDIR /var/www/html
# Wed, 03 May 2023 22:36:08 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 03 May 2023 22:36:08 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 03 May 2023 22:36:08 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 03 May 2023 22:36:08 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 03 May 2023 22:36:16 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 03 May 2023 22:36:16 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 03 May 2023 22:36:17 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 03 May 2023 22:36:17 GMT
USER adminer
# Wed, 03 May 2023 22:36:17 GMT
CMD ["php-fpm7.4"]
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
	-	`sha256:80905ff098486de407818741ff7a9b5703b2b76404e51143a52c88b232920633`  
		Last Modified: Wed, 03 May 2023 22:36:48 GMT  
		Size: 2.7 KB (2711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d47123c66d228bede90982668f04f911f8192d96fb454f7537e17973419e12c`  
		Last Modified: Wed, 03 May 2023 22:36:48 GMT  
		Size: 1.9 KB (1880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb848477561103709620550acd27d1fd4b33ee36878be7ee2cde8e4ea1244407`  
		Last Modified: Wed, 03 May 2023 22:36:48 GMT  
		Size: 1.5 KB (1475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64bc044ead6b8507a55089c94a91383bf0ab7697df6beb2628aa1dfb154badd1`  
		Last Modified: Wed, 03 May 2023 22:36:48 GMT  
		Size: 1.4 MB (1385441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94b39d7155767f9502319fef618ee97bd6882b307eb17b399edc047a7ae257e7`  
		Last Modified: Wed, 03 May 2023 22:36:48 GMT  
		Size: 489.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
