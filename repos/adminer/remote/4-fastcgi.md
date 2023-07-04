## `adminer:4-fastcgi`

```console
$ docker pull adminer@sha256:d71cd093c2ac5e507d9b130473cea55992b97cc0b6424b0a15ac6f4cea2ca5db
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
$ docker pull adminer@sha256:6caa807820ca7c9cdbadf1ab1d45db1bd786efc37ef5aa47cbe10708dd12d998
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.9 MB (95935139 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:98e5a487eafbb1e1c54550a075a220d824e930146fccd78c5a4afdb74a2bc50a`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Tue, 04 Jul 2023 01:20:09 GMT
ADD file:b7c0be2bb90e88689b1c16da78dea0b85760b55b90ef2e5bc4a529c89e4fa25b in / 
# Tue, 04 Jul 2023 01:20:10 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 03:25:51 GMT
STOPSIGNAL SIGINT
# Tue, 04 Jul 2023 03:26:14 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 03:26:15 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 04 Jul 2023 03:26:33 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Tue, 04 Jul 2023 03:26:33 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 04 Jul 2023 03:26:33 GMT
WORKDIR /var/www/html
# Tue, 04 Jul 2023 03:26:33 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 04 Jul 2023 03:26:33 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 04 Jul 2023 03:26:34 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 04 Jul 2023 03:26:34 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 04 Jul 2023 03:26:44 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 04 Jul 2023 03:26:44 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 04 Jul 2023 03:26:44 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 04 Jul 2023 03:26:44 GMT
USER adminer
# Tue, 04 Jul 2023 03:26:44 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:34df401c391c7595044379e04e8ad4856a5a3974cdbf5a160f0a204d761e88aa`  
		Last Modified: Tue, 04 Jul 2023 01:25:21 GMT  
		Size: 55.1 MB (55055300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:942860e9b081ab6c14dea841e13d6b8e230b5c3a7482ddc73980c866338f81bd`  
		Last Modified: Tue, 04 Jul 2023 03:27:06 GMT  
		Size: 39.5 MB (39487448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f571177b537e8c4f94f8bd4920e829d50ef7d56e541695ba67a448487efc1bf1`  
		Last Modified: Tue, 04 Jul 2023 03:26:58 GMT  
		Size: 391.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d76a56a3771369c6e704d5e35bd1766d6e549b0d66ed49c4ad0f11e9606374f`  
		Last Modified: Tue, 04 Jul 2023 03:27:22 GMT  
		Size: 2.7 KB (2706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc7ccb20f3a0eece3e90efca525e5571942cf228298324515c02198d05777cb9`  
		Last Modified: Tue, 04 Jul 2023 03:27:22 GMT  
		Size: 1.9 KB (1877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c8c7d8cd6f443d542fd01782eed5dc03b0a74d0f0714683dc176561ba235edf`  
		Last Modified: Tue, 04 Jul 2023 03:27:22 GMT  
		Size: 1.5 KB (1475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3db1d8f59a146868100bd71857251dc11b79dbc9b8b8cb776a4d89e05748ac88`  
		Last Modified: Tue, 04 Jul 2023 03:27:22 GMT  
		Size: 1.4 MB (1385454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8979c84db28ce690caecdf197ecff4c3fa9fd09b8da2aed722a745e415edae28`  
		Last Modified: Tue, 04 Jul 2023 03:27:22 GMT  
		Size: 488.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-fastcgi` - linux; arm variant v5

```console
$ docker pull adminer@sha256:000c82eff38911214c7db7c3a511c0a57cba0bda80bcf27ee035587d3eed20be
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.2 MB (91197097 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:610a0bd191c5498d32fa7dcb44808b310a87072810de50eba2ae2654de87ca3c`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Tue, 04 Jul 2023 00:48:39 GMT
ADD file:fe1b9f9f6c7d67ad23a2ee839774be4bcee33c60c7b34c48df5a08eb33cafd1b in / 
# Tue, 04 Jul 2023 00:48:40 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 04:31:35 GMT
STOPSIGNAL SIGINT
# Tue, 04 Jul 2023 04:32:04 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 04:32:05 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 04 Jul 2023 04:32:22 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Tue, 04 Jul 2023 04:32:23 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 04 Jul 2023 04:32:23 GMT
WORKDIR /var/www/html
# Tue, 04 Jul 2023 04:32:23 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 04 Jul 2023 04:32:23 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 04 Jul 2023 04:32:24 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 04 Jul 2023 04:32:24 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 04 Jul 2023 04:32:37 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 04 Jul 2023 04:32:37 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 04 Jul 2023 04:32:37 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 04 Jul 2023 04:32:37 GMT
USER adminer
# Tue, 04 Jul 2023 04:32:37 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:702dd8b607f626c689176debe921fe96009c1ce6dbd66f4f238c7def50080e3d`  
		Last Modified: Tue, 04 Jul 2023 00:52:15 GMT  
		Size: 52.6 MB (52556778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9d374e7d45666fbc1903d32400cd401880366876db459c5ab206a54ab0d0411`  
		Last Modified: Tue, 04 Jul 2023 04:32:58 GMT  
		Size: 37.2 MB (37248008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fa5b59f67ee61ca2a807576d30a1cc008c51081eae0849e200e60ce47af498c`  
		Last Modified: Tue, 04 Jul 2023 04:32:49 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea75e47d8dcfa6ad8c28efd5221051c57745479e4c9be773a174ed053c964fdc`  
		Last Modified: Tue, 04 Jul 2023 04:33:14 GMT  
		Size: 2.7 KB (2711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c6d17752c4fc62ce532477600101cfe5b1108020f93a8c97e4d220d8ef823ba`  
		Last Modified: Tue, 04 Jul 2023 04:33:14 GMT  
		Size: 1.9 KB (1869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:888b637b24bf6e78648f068b8a4683cf6f28db889ba791c3134c6524a347b7ca`  
		Last Modified: Tue, 04 Jul 2023 04:33:14 GMT  
		Size: 1.5 KB (1476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f07ec511505a60a6fad31428b9d54cf218f5256afd31101c81098d87db2a5e3`  
		Last Modified: Tue, 04 Jul 2023 04:33:14 GMT  
		Size: 1.4 MB (1385376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b106734e44f3b038b26d8a5c64f653c388d92572b121d6ce448372a7ff16c2f`  
		Last Modified: Tue, 04 Jul 2023 04:33:14 GMT  
		Size: 489.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-fastcgi` - linux; arm variant v7

```console
$ docker pull adminer@sha256:0be94bd6202f72f371789c8c37780bf657de3d1c590e6ca57b0bfc52b20b6904
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.8 MB (87793947 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1678a0b92255b8085e7baec25267827d874cf221fc98c542e2979a62d5def219`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Tue, 04 Jul 2023 00:58:06 GMT
ADD file:17e02296458241d9441f8da6a5dafb747d528a729106b17cec2f4c1c8cfe0ad8 in / 
# Tue, 04 Jul 2023 00:58:07 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 05:47:35 GMT
STOPSIGNAL SIGINT
# Tue, 04 Jul 2023 05:48:06 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 05:48:07 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 04 Jul 2023 05:48:33 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Tue, 04 Jul 2023 05:48:34 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 04 Jul 2023 05:48:34 GMT
WORKDIR /var/www/html
# Tue, 04 Jul 2023 05:48:34 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 04 Jul 2023 05:48:34 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 04 Jul 2023 05:48:34 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 04 Jul 2023 05:48:34 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 04 Jul 2023 05:48:45 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 04 Jul 2023 05:48:45 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 04 Jul 2023 05:48:46 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 04 Jul 2023 05:48:46 GMT
USER adminer
# Tue, 04 Jul 2023 05:48:46 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:31edf2db9ca1650aa08e2d42e9b5bb7349413d7212110149a1a5d202ac20914b`  
		Last Modified: Tue, 04 Jul 2023 01:03:12 GMT  
		Size: 50.2 MB (50218247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcfcd0af927af2ef5ff85003d2efb7bec343ebb0e0ae33e33a182aba3044318c`  
		Last Modified: Tue, 04 Jul 2023 05:49:03 GMT  
		Size: 36.2 MB (36183362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b4b63416f4c6f052acc74f92deae27e302df97dc86efe776938f5064b98a90f`  
		Last Modified: Tue, 04 Jul 2023 05:48:55 GMT  
		Size: 388.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:611383b899e8a30dc5ee74865f6ad93b4b59b676b48f4c4a9fe5eb0d92d9a8a3`  
		Last Modified: Tue, 04 Jul 2023 05:49:19 GMT  
		Size: 2.7 KB (2706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2e604c1e6cce082e392b473dcdc2824c86f055c7e910560c81eb54d7dbf758c`  
		Last Modified: Tue, 04 Jul 2023 05:49:19 GMT  
		Size: 1.9 KB (1866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:282e04bf6ee13b97e03f675aa27139cac7931f5cd1c735d6a6e078abf6ab8004`  
		Last Modified: Tue, 04 Jul 2023 05:49:19 GMT  
		Size: 1.5 KB (1480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9348a926275a93bc78151de56c3200f5f3d15827e53cd9c50db6ef4557513b6`  
		Last Modified: Tue, 04 Jul 2023 05:49:19 GMT  
		Size: 1.4 MB (1385410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07644552098791dbe95267ac6756b65b68cdced2563aa3f7d54135b1c72de7dc`  
		Last Modified: Tue, 04 Jul 2023 05:49:19 GMT  
		Size: 488.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-fastcgi` - linux; arm64 variant v8

```console
$ docker pull adminer@sha256:ea982df61c67cda812f3db71135e82f0193d1c2dfb26baed684ecaf1f64fd9e1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.3 MB (94339498 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b191e3e843fb791bf5ada65d97c51c5122ad50391c04f939e42ec397162e0107`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:43 GMT
ADD file:e626446584d8094b7b58d72a717380ca64d3e9ab924fc625406fe26a83fe1d8b in / 
# Tue, 04 Jul 2023 01:57:43 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 05:51:15 GMT
STOPSIGNAL SIGINT
# Tue, 04 Jul 2023 05:51:38 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 05:51:39 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 04 Jul 2023 05:51:56 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Tue, 04 Jul 2023 05:51:56 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 04 Jul 2023 05:51:56 GMT
WORKDIR /var/www/html
# Tue, 04 Jul 2023 05:51:56 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 04 Jul 2023 05:51:56 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 04 Jul 2023 05:51:56 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 04 Jul 2023 05:51:56 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 04 Jul 2023 05:52:06 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 04 Jul 2023 05:52:06 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 04 Jul 2023 05:52:06 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 04 Jul 2023 05:52:06 GMT
USER adminer
# Tue, 04 Jul 2023 05:52:07 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:29279ac7c19f9c667f1c6b07bfba6fba20ca0d945b9fbc6edad6f75d13361fae`  
		Last Modified: Tue, 04 Jul 2023 02:01:38 GMT  
		Size: 53.7 MB (53703979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f67950e101bf9ffd94a4f3bcf1ed33a0198579ad66648c058d9cf02cf8718da3`  
		Last Modified: Tue, 04 Jul 2023 05:52:23 GMT  
		Size: 39.2 MB (39243182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47884375b752c5be2429af8ad660f8adf9fe1791c29ccaa459a99fb6b49cd480`  
		Last Modified: Tue, 04 Jul 2023 05:52:16 GMT  
		Size: 388.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a36b9ae8ef8dc8836bc9cebb965bb5a95feb625fb94cf9bd7a2fbad141882ee`  
		Last Modified: Tue, 04 Jul 2023 05:52:38 GMT  
		Size: 2.7 KB (2707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:110eafa4978602a23e592883e753488138ec621288afdf88b035846c62e8e637`  
		Last Modified: Tue, 04 Jul 2023 05:52:38 GMT  
		Size: 1.9 KB (1880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f1b42d96d2db5a9617e2daa90692d221de9ca8587b5da169de22801d1f751c9`  
		Last Modified: Tue, 04 Jul 2023 05:52:38 GMT  
		Size: 1.5 KB (1477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:add1f08f25301e10f14bd85cd6e469e3f5217ee20090cbb753800202d38bbf0c`  
		Last Modified: Tue, 04 Jul 2023 05:52:39 GMT  
		Size: 1.4 MB (1385395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:192fc4f875edc6c1d4a96c649506651f13abe414fca8165a3f28dad83fd96f49`  
		Last Modified: Tue, 04 Jul 2023 05:52:38 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-fastcgi` - linux; 386

```console
$ docker pull adminer@sha256:f28603ea4c880db60110049c6cf22720545bc6be296659ec3bb3d320c7343d55
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.0 MB (96991589 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4cf9f1de498d643ae57669878101b1e59fcebf70db1074d81ceea8801ccd8f7`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Tue, 04 Jul 2023 01:38:48 GMT
ADD file:c5739407c2c257fbb85ab4b9dcd2dc07e6fe172d7309aaaaab544c8df6c42b92 in / 
# Tue, 04 Jul 2023 01:38:49 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 05:26:00 GMT
STOPSIGNAL SIGINT
# Tue, 04 Jul 2023 05:26:29 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 05:26:30 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 04 Jul 2023 05:26:49 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Tue, 04 Jul 2023 05:26:49 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 04 Jul 2023 05:26:49 GMT
WORKDIR /var/www/html
# Tue, 04 Jul 2023 05:26:50 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 04 Jul 2023 05:26:50 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 04 Jul 2023 05:26:50 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 04 Jul 2023 05:26:50 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 04 Jul 2023 05:27:02 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 04 Jul 2023 05:27:02 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 04 Jul 2023 05:27:02 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 04 Jul 2023 05:27:02 GMT
USER adminer
# Tue, 04 Jul 2023 05:27:02 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:b700c8b35944e0d5f6ab9049dbe2262492e26327a8efad518b1011428393653f`  
		Last Modified: Tue, 04 Jul 2023 01:43:49 GMT  
		Size: 56.0 MB (56040756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a902a66c5c608f61d35dd264eb84af9a969f2d77d57ec06ad874647c6357d0e`  
		Last Modified: Tue, 04 Jul 2023 05:27:24 GMT  
		Size: 39.6 MB (39558591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:718cd99c580c15e79afcf178eb77f3c0ac0432c212f50ccd720a2680b26373d1`  
		Last Modified: Tue, 04 Jul 2023 05:27:14 GMT  
		Size: 387.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a55ca2f23f925c98c51f8a734f76590fb5f3be47a5f8dee895176e2c49ce49cf`  
		Last Modified: Tue, 04 Jul 2023 05:27:41 GMT  
		Size: 2.7 KB (2709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37e6f54f2eebdc0908a5bb0ea1bf013ce274873f298ca9b3516e231f378666da`  
		Last Modified: Tue, 04 Jul 2023 05:27:41 GMT  
		Size: 1.9 KB (1870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e88228cdb9c571deaf46d3473a01ca87db8a9b15747155e4fa4acb1dfd7978eb`  
		Last Modified: Tue, 04 Jul 2023 05:27:41 GMT  
		Size: 1.5 KB (1480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23222c8c9b4ecdd9417f8199b026bbfb4764f3a4b1eb9bb2e36a6fdae431afdb`  
		Last Modified: Tue, 04 Jul 2023 05:27:41 GMT  
		Size: 1.4 MB (1385307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51719e58ff78bcdbb9022589936f75bbe7a64df0048c6777578f0f2461600a3d`  
		Last Modified: Tue, 04 Jul 2023 05:27:41 GMT  
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
$ docker pull adminer@sha256:9364792ada1b2eb7211f622b7a788103b4abd9fcf3b97c8768924f6e09b6690e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.3 MB (101260839 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb8a36421f33b53c1c0f63f968861fd66876c3ea0c6830325f9681e900bd5d2f`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Tue, 04 Jul 2023 01:18:11 GMT
ADD file:ff86c25854c28609c2852c1615270f0acd4c4efaa38ff8ed9c23afe5132f2135 in / 
# Tue, 04 Jul 2023 01:18:15 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 04:50:59 GMT
STOPSIGNAL SIGINT
# Tue, 04 Jul 2023 04:52:51 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 04:53:00 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 04 Jul 2023 04:54:41 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Tue, 04 Jul 2023 04:54:44 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 04 Jul 2023 04:54:46 GMT
WORKDIR /var/www/html
# Tue, 04 Jul 2023 04:54:46 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 04 Jul 2023 04:54:47 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 04 Jul 2023 04:54:47 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 04 Jul 2023 04:54:48 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 04 Jul 2023 04:55:24 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 04 Jul 2023 04:55:25 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 04 Jul 2023 04:55:25 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 04 Jul 2023 04:55:26 GMT
USER adminer
# Tue, 04 Jul 2023 04:55:27 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:a792749f62225048efdf85841bea6f3999f586371852f3dbce13a6c3d89b1fa7`  
		Last Modified: Tue, 04 Jul 2023 01:25:06 GMT  
		Size: 58.9 MB (58927745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44790fdc65745caeec0d36cb605fed307ff2f9e2ef066a8d2b1522e8221f18f3`  
		Last Modified: Tue, 04 Jul 2023 04:56:04 GMT  
		Size: 40.9 MB (40940332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24457876d46dbb125dbcfa9f211d86229bb07a8f9864412462d6c795573177a8`  
		Last Modified: Tue, 04 Jul 2023 04:55:51 GMT  
		Size: 395.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd2011aca228bf492e49980db4d7f382fb149bfcdd0d23cb67659c0df6737226`  
		Last Modified: Tue, 04 Jul 2023 04:56:28 GMT  
		Size: 2.7 KB (2715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:859d3a288f61883dc684d9157c6cd5075a0b1a74f011c4e69e987c11f886bbd7`  
		Last Modified: Tue, 04 Jul 2023 04:56:28 GMT  
		Size: 1.9 KB (1873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e5d0aacdd54eb059e402c26939fdccb4fe827cc7b1fb89571221e11e2bc6e62`  
		Last Modified: Tue, 04 Jul 2023 04:56:28 GMT  
		Size: 1.5 KB (1477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c456356bca8fc124638a22b16275bb5b2ba5380b47c6af4c3cf3683ce4f8d0b5`  
		Last Modified: Tue, 04 Jul 2023 04:56:29 GMT  
		Size: 1.4 MB (1385813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49dc45753ebe2ef73c8d7aece8aa163f83dfbbc85299390556dd5a5d9854b65b`  
		Last Modified: Tue, 04 Jul 2023 04:56:28 GMT  
		Size: 489.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-fastcgi` - linux; s390x

```console
$ docker pull adminer@sha256:0216b502b2fbaf203aa216f755a6ac87ad38ef1a03b6cb2c0933632a51e49803
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.7 MB (93699071 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:00fcb8c0621022af131025bc924f46d6d895c4c360e188064ea759011b4b76e2`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Tue, 04 Jul 2023 01:32:26 GMT
ADD file:231ba6ce8d3ee30318948799a94cb007f1517ea0d14c2b84863012cac37d6c6b in / 
# Tue, 04 Jul 2023 01:32:29 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 10:13:42 GMT
STOPSIGNAL SIGINT
# Tue, 04 Jul 2023 10:14:02 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 10:14:05 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 04 Jul 2023 10:14:25 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Tue, 04 Jul 2023 10:14:25 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 04 Jul 2023 10:14:26 GMT
WORKDIR /var/www/html
# Tue, 04 Jul 2023 10:14:26 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 04 Jul 2023 10:14:26 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 04 Jul 2023 10:14:26 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 04 Jul 2023 10:14:26 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 04 Jul 2023 10:14:35 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 04 Jul 2023 10:14:35 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 04 Jul 2023 10:14:35 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 04 Jul 2023 10:14:35 GMT
USER adminer
# Tue, 04 Jul 2023 10:14:35 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:1e40ed2a44a8c2786b06584afad765d97e9b1c910f58ae426622ba17fbf3d4c3`  
		Last Modified: Tue, 04 Jul 2023 01:37:21 GMT  
		Size: 53.3 MB (53288197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f455bf175cdcb09fa6b7ff2fd1ff4fc270ef66c10a07cdf9a5ab96296f09bc29`  
		Last Modified: Tue, 04 Jul 2023 10:15:01 GMT  
		Size: 39.0 MB (39018533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:741d094c89a2584874245eee735be1fee9c3f4efb3b4d0e6556a6c762d8bff88`  
		Last Modified: Tue, 04 Jul 2023 10:14:54 GMT  
		Size: 388.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbc443321070cade53e070f72bb677a7454d4e6850c079e8596bfbea4c776bd3`  
		Last Modified: Tue, 04 Jul 2023 10:15:13 GMT  
		Size: 2.7 KB (2707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f79e6de62f0982c2034159a72c0504ece5091310812fe01eb1f7e32aebb4f195`  
		Last Modified: Tue, 04 Jul 2023 10:15:13 GMT  
		Size: 1.9 KB (1880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d93f23d3091d2fbcc5ca629f301c0d9d91bb68816bf3b40daba87d8f4f0cee4c`  
		Last Modified: Tue, 04 Jul 2023 10:15:13 GMT  
		Size: 1.5 KB (1475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78beb5d3d1066c39733928730a1f1979268e8cdc6c2cdc546f9980610fdeb1b9`  
		Last Modified: Tue, 04 Jul 2023 10:15:13 GMT  
		Size: 1.4 MB (1385401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4208f056525ccdfc6caf19c1def13954f7c4ac7dd58890e825545de0a8dc7c9d`  
		Last Modified: Tue, 04 Jul 2023 10:15:13 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
