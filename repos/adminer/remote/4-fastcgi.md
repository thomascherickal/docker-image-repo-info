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
