## `adminer:4-fastcgi`

```console
$ docker pull adminer@sha256:db7bf0fa1725885b308aa37479d74f127a4248a68d97e08b83a3fd995fa78338
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
$ docker pull adminer@sha256:10abd75754d797bb3b6184385c55805ecb66ac5b72c4bdba88dab1bf0eff7d2a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.9 MB (95935628 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:067ad5886fd890ad5052518c2b98a4e56ae78def270cb31064f6c7db5d8d2316`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Thu, 27 Jul 2023 23:24:55 GMT
ADD file:b493776b6d91132ce50735e2d82076620774a1e0a690cf96777ddd6b85f513ef in / 
# Thu, 27 Jul 2023 23:24:55 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 02:57:00 GMT
STOPSIGNAL SIGINT
# Fri, 28 Jul 2023 02:57:20 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 02:57:21 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Fri, 28 Jul 2023 02:57:41 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Fri, 28 Jul 2023 02:57:42 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Fri, 28 Jul 2023 02:57:42 GMT
WORKDIR /var/www/html
# Fri, 28 Jul 2023 02:57:42 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Fri, 28 Jul 2023 02:57:42 GMT
ENV ADMINER_VERSION=4.8.1
# Fri, 28 Jul 2023 02:57:42 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Fri, 28 Jul 2023 02:57:42 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Fri, 28 Jul 2023 02:57:53 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 28 Jul 2023 02:57:53 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Fri, 28 Jul 2023 02:57:53 GMT
ENTRYPOINT ["entrypoint.sh"]
# Fri, 28 Jul 2023 02:57:53 GMT
USER adminer
# Fri, 28 Jul 2023 02:57:53 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:9a9e034800a1747ea288f38f6087c036acac99dd3ec5255bf7798abd8c23a304`  
		Last Modified: Thu, 27 Jul 2023 23:29:45 GMT  
		Size: 55.1 MB (55055571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a93e89405fb52039a3b5153466ad287e1095bcb5cc79650dfb3d3161c1fc3071`  
		Last Modified: Fri, 28 Jul 2023 02:58:15 GMT  
		Size: 39.5 MB (39487685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e87fd288de6c7f7252c630c1be310e591224e28db70b6d5156c1751f6a8f364`  
		Last Modified: Fri, 28 Jul 2023 02:58:07 GMT  
		Size: 391.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f81e44fa5add0b790d414c49a4fdc765b534a144eb652e0af7d45acb4cb90024`  
		Last Modified: Fri, 28 Jul 2023 02:58:32 GMT  
		Size: 2.7 KB (2705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d69b2e0e16c5fdb48b7d312707e25f96010d79ba03fddf6a27986b31aa89b94`  
		Last Modified: Fri, 28 Jul 2023 02:58:32 GMT  
		Size: 1.9 KB (1880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c967a8f1256fc87c0962f8a13979f3aacdfe4254b9fbdecd32543de23a808307`  
		Last Modified: Fri, 28 Jul 2023 02:58:32 GMT  
		Size: 1.5 KB (1475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee5a5d9d42f4b7d7214bf4ed131e9610f54d4e8d6a713fcca3f82266f82e27b3`  
		Last Modified: Fri, 28 Jul 2023 02:58:33 GMT  
		Size: 1.4 MB (1385429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bacf51620cd50e5d2862bf40ea86af4b1958666796a8f52fbc52e7164382fb3`  
		Last Modified: Fri, 28 Jul 2023 02:58:32 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-fastcgi` - linux; arm variant v5

```console
$ docker pull adminer@sha256:8a903e621fee341d4d23cff0d14b74be04230f993cbd6c3851d0e932d1c17cbe
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.2 MB (91198457 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63ed6b22cc6c8c6ebb0680382f4bbb56866c35561f5a0367d4b6525fc728710b`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Tue, 15 Aug 2023 23:48:40 GMT
ADD file:d044e64aab907424be649252b5ff1d9f5e8c9494db5b60c0e54f5962bfb73478 in / 
# Tue, 15 Aug 2023 23:48:40 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 00:50:17 GMT
STOPSIGNAL SIGINT
# Wed, 16 Aug 2023 00:50:44 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 00:50:45 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 16 Aug 2023 00:51:06 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Wed, 16 Aug 2023 00:51:07 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 16 Aug 2023 00:51:07 GMT
WORKDIR /var/www/html
# Wed, 16 Aug 2023 00:51:07 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 16 Aug 2023 00:51:07 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 16 Aug 2023 00:51:07 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 16 Aug 2023 00:51:07 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 16 Aug 2023 00:51:19 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 16 Aug 2023 00:51:19 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 16 Aug 2023 00:51:19 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 16 Aug 2023 00:51:19 GMT
USER adminer
# Wed, 16 Aug 2023 00:51:19 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:0b63bbf2e6f6026dfaed9cbedf777472a04812b7d291501b1d416e49e3ce885e`  
		Last Modified: Tue, 15 Aug 2023 23:51:54 GMT  
		Size: 52.6 MB (52558130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f7d19107e1a659808b9cf0e01e8326cb019bad1bd5e6d11666cd1e8a4d58f10`  
		Last Modified: Wed, 16 Aug 2023 00:51:40 GMT  
		Size: 37.2 MB (37248042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3402920c76f848974711afefbf633df8e1e5f0238e9d1923aa35d796a7e39775`  
		Last Modified: Wed, 16 Aug 2023 00:51:31 GMT  
		Size: 391.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ca5e5983358cb8df6f82ccca639a1c786b5ef126867cc630f85d1ed33dc9c1d`  
		Last Modified: Wed, 16 Aug 2023 00:51:57 GMT  
		Size: 2.7 KB (2707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b36f7c90bd79555d60c5f3bcc3afae34867f4ea464da49ec237a7ece749f223`  
		Last Modified: Wed, 16 Aug 2023 00:51:57 GMT  
		Size: 1.9 KB (1869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62cfdb20b5272a134da575104c9286054e5a9a67097cf91d37dcab3b7ff61fae`  
		Last Modified: Wed, 16 Aug 2023 00:51:57 GMT  
		Size: 1.5 KB (1476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:798235abe850cf839ee7ef49ea37e6cc9fe3f4effd122bd1cb6ed5a5cc03761c`  
		Last Modified: Wed, 16 Aug 2023 00:51:58 GMT  
		Size: 1.4 MB (1385348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27557ea7df0942f926d2c7870464abbadf23547ddbcd1e1f7f8441ba9f50f2c1`  
		Last Modified: Wed, 16 Aug 2023 00:51:57 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-fastcgi` - linux; arm variant v7

```console
$ docker pull adminer@sha256:b351aa1c77616bb60bc5bfbbe67e205113f934e19d4a5fdba458510a1328ff26
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.8 MB (87794093 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:249931306ce34ddda788eda999016de0eff9f9ee2ddf74794491fa85cb039612`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Thu, 27 Jul 2023 23:58:01 GMT
ADD file:3014d2ee0e0e882151b5295faeb81a24b4d6f9e0f92f3ba969ccffb2bd8a6d76 in / 
# Thu, 27 Jul 2023 23:58:03 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 03:59:47 GMT
STOPSIGNAL SIGINT
# Fri, 28 Jul 2023 04:00:13 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 04:00:13 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Fri, 28 Jul 2023 04:00:35 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Fri, 28 Jul 2023 04:00:36 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Fri, 28 Jul 2023 04:00:36 GMT
WORKDIR /var/www/html
# Fri, 28 Jul 2023 04:00:36 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Fri, 28 Jul 2023 04:00:36 GMT
ENV ADMINER_VERSION=4.8.1
# Fri, 28 Jul 2023 04:00:36 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Fri, 28 Jul 2023 04:00:36 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Fri, 28 Jul 2023 04:00:47 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 28 Jul 2023 04:00:47 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Fri, 28 Jul 2023 04:00:47 GMT
ENTRYPOINT ["entrypoint.sh"]
# Fri, 28 Jul 2023 04:00:47 GMT
USER adminer
# Fri, 28 Jul 2023 04:00:47 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:e8dff7ada2c26d71087c5ec6294d1adc4dcf7d688824a079e89e3bedd9a34fa6`  
		Last Modified: Fri, 28 Jul 2023 00:03:32 GMT  
		Size: 50.2 MB (50218549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ed4d02fb882790c38a99c13ddbaef5e77853b94fc86f6b04f62d441add2ef3e`  
		Last Modified: Fri, 28 Jul 2023 04:01:07 GMT  
		Size: 36.2 MB (36183206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78f0f2b99e14fee877a41491269ee8be6d838ff59d45b409dd9f37df5e17b9ce`  
		Last Modified: Fri, 28 Jul 2023 04:00:59 GMT  
		Size: 394.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69d551188db8fcb99faae97e05b4c8bc143110a5229585723f740efccfbd09a1`  
		Last Modified: Fri, 28 Jul 2023 04:01:24 GMT  
		Size: 2.7 KB (2711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8a8295cc00826788af8f45b42e0dbc947359715c214e76b022f2f6289f88464`  
		Last Modified: Fri, 28 Jul 2023 04:01:24 GMT  
		Size: 1.9 KB (1871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8de8aab5dcf003b320d56968a5f16c7b51e438673a046af60b5812ff86405568`  
		Last Modified: Fri, 28 Jul 2023 04:01:24 GMT  
		Size: 1.5 KB (1476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a5511ef2abfd1b603870047dfdc1181b0aa2b8febb924e69d844928a2d84de`  
		Last Modified: Fri, 28 Jul 2023 04:01:25 GMT  
		Size: 1.4 MB (1385394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e3c136b48d461d9c2efe4ec7f6e46e501596fca8ccebf5f1817ec1be2cd4ad7`  
		Last Modified: Fri, 28 Jul 2023 04:01:24 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-fastcgi` - linux; arm64 variant v8

```console
$ docker pull adminer@sha256:62a62e95e6e92f9e8510495f3cb436a6b4196b63bb07134596be3e010d33acd9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.3 MB (94340314 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:164e7749682325c1aa3417dd5bdd3315167af4c5b97129e7994a12bfc9a727bc`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Thu, 27 Jul 2023 23:43:07 GMT
ADD file:a0144d077c2c6b73bbb5f7e7b8e6b58e4127de2a5faf907cd4e83e4d83437fad in / 
# Thu, 27 Jul 2023 23:43:07 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 01:32:38 GMT
STOPSIGNAL SIGINT
# Fri, 28 Jul 2023 01:32:57 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 01:32:58 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Fri, 28 Jul 2023 01:33:11 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Fri, 28 Jul 2023 01:33:12 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Fri, 28 Jul 2023 01:33:12 GMT
WORKDIR /var/www/html
# Fri, 28 Jul 2023 01:33:12 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Fri, 28 Jul 2023 01:33:12 GMT
ENV ADMINER_VERSION=4.8.1
# Fri, 28 Jul 2023 01:33:12 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Fri, 28 Jul 2023 01:33:12 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Fri, 28 Jul 2023 01:33:22 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 28 Jul 2023 01:33:22 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Fri, 28 Jul 2023 01:33:22 GMT
ENTRYPOINT ["entrypoint.sh"]
# Fri, 28 Jul 2023 01:33:22 GMT
USER adminer
# Fri, 28 Jul 2023 01:33:22 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:49185a1a3bc353699370ac57d50a7b7234b59616b6aebde79ba6a0a0314bb107`  
		Last Modified: Thu, 27 Jul 2023 23:46:34 GMT  
		Size: 53.7 MB (53704790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71c936be3d46519b363d127d99d4a16afc2bcda8095c369d6962f2074106072b`  
		Last Modified: Fri, 28 Jul 2023 01:33:40 GMT  
		Size: 39.2 MB (39243229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2f330de399f2ce87df9e5548f572616f566f9e9c844ebe34b92acf948008cdd`  
		Last Modified: Fri, 28 Jul 2023 01:33:34 GMT  
		Size: 386.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8010fea9be3a6e42dfda4398bc8dd961f3cc38cd2b066ccc38d8b83b7b0dd3e4`  
		Last Modified: Fri, 28 Jul 2023 01:33:57 GMT  
		Size: 2.7 KB (2708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7694be696a7e8c7e0ca897c46b134bd20166b15352ab0c9c130f49b4334faebc`  
		Last Modified: Fri, 28 Jul 2023 01:33:57 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cec715a9f3239113933f55f76bc62d32455f3b1647d2867f143645ade0de0e60`  
		Last Modified: Fri, 28 Jul 2023 01:33:57 GMT  
		Size: 1.5 KB (1477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03e99cff7b42b42793347c1b48793f8d6340ba93fca1aa4a375b53344b9112c9`  
		Last Modified: Fri, 28 Jul 2023 01:33:58 GMT  
		Size: 1.4 MB (1385351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bea23c2e8231c1a0717f52f8aac5318af3412ac9f3481f18bf16428f83686358`  
		Last Modified: Fri, 28 Jul 2023 01:33:57 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-fastcgi` - linux; 386

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

### `adminer:4-fastcgi` - linux; mips64le

```console
$ docker pull adminer@sha256:de6ce6ccbea3572c047779ffcab12a086f4e5f8b1af96c50baa07534a6878d74
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.6 MB (92617937 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7108b48a68f93d3348a9a0f0458dc835bab2556f0c7cb5b1c5ddb7b476121b6b`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Thu, 27 Jul 2023 23:11:57 GMT
ADD file:ccccca3acf3759fd714159d3c3beff86d84a9751b947e148348d523272fc1bb9 in / 
# Thu, 27 Jul 2023 23:12:02 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 13:55:35 GMT
STOPSIGNAL SIGINT
# Fri, 28 Jul 2023 13:57:30 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 13:57:36 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Fri, 28 Jul 2023 13:59:22 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Fri, 28 Jul 2023 13:59:29 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Fri, 28 Jul 2023 13:59:32 GMT
WORKDIR /var/www/html
# Fri, 28 Jul 2023 13:59:35 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Fri, 28 Jul 2023 13:59:39 GMT
ENV ADMINER_VERSION=4.8.1
# Fri, 28 Jul 2023 13:59:42 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Fri, 28 Jul 2023 13:59:45 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Fri, 28 Jul 2023 14:00:37 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 28 Jul 2023 14:00:40 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Fri, 28 Jul 2023 14:00:43 GMT
ENTRYPOINT ["entrypoint.sh"]
# Fri, 28 Jul 2023 14:00:46 GMT
USER adminer
# Fri, 28 Jul 2023 14:00:50 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:9d9a0c35af83dc10b6307f02a48749b4d8024123530a89d5173f70981e00b9e3`  
		Last Modified: Thu, 27 Jul 2023 23:23:10 GMT  
		Size: 53.3 MB (53270927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca7a8edf82627413cef8f2eeb728d9b0757c9390dbaaff69f0e368e741369be1`  
		Last Modified: Fri, 28 Jul 2023 14:01:36 GMT  
		Size: 38.0 MB (37953869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a94981f4408e1cec66d3deff7404dd78684c1f3ff8a57a6cab5f47f5310e5d6`  
		Last Modified: Fri, 28 Jul 2023 14:01:10 GMT  
		Size: 393.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a84b0818f28a6c60d009cd7f22a133ea5bad82b55a4f32a5e80efb2a69b34c6`  
		Last Modified: Fri, 28 Jul 2023 14:01:57 GMT  
		Size: 2.7 KB (2712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:246135c88abf30dc5d5c17b1f91e851da2bd2e9d7bd0c2b761ed8a9fc5b37766`  
		Last Modified: Fri, 28 Jul 2023 14:01:57 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16a8408c565c166ea77301a73f6b7d3e5b3559305d68c5d6e599050255d5e15b`  
		Last Modified: Fri, 28 Jul 2023 14:01:57 GMT  
		Size: 1.5 KB (1480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64d029af1e71badb60d3925e0e433ad7dc881ed88a9f81f33de76df28b83b1ed`  
		Last Modified: Fri, 28 Jul 2023 14:01:58 GMT  
		Size: 1.4 MB (1386331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:869d366cf9c026146da90a023eadd2fdbc8e1e8b6196785fd4e552ebc2e91ec7`  
		Last Modified: Fri, 28 Jul 2023 14:01:57 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-fastcgi` - linux; ppc64le

```console
$ docker pull adminer@sha256:ef3f6de9a08d8614e269a832743a26a20f31fa08ac1d26a642839de0a0076c45
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.3 MB (101260301 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b84f377ef976bc4bba1d4bbd16460a1ffbf5cf430a27f0a6e1e26ff9b1bdde92`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Thu, 27 Jul 2023 23:23:20 GMT
ADD file:c9c051b70d4b5c059dc4dfc25c2ce056efb99058bbea4911c346eaf8c90ea938 in / 
# Thu, 27 Jul 2023 23:23:23 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 03:34:07 GMT
STOPSIGNAL SIGINT
# Fri, 28 Jul 2023 03:35:19 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 03:35:27 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Fri, 28 Jul 2023 03:36:32 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Fri, 28 Jul 2023 03:36:36 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Fri, 28 Jul 2023 03:36:37 GMT
WORKDIR /var/www/html
# Fri, 28 Jul 2023 03:36:38 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Fri, 28 Jul 2023 03:36:38 GMT
ENV ADMINER_VERSION=4.8.1
# Fri, 28 Jul 2023 03:36:38 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Fri, 28 Jul 2023 03:36:39 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Fri, 28 Jul 2023 03:37:12 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 28 Jul 2023 03:37:13 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Fri, 28 Jul 2023 03:37:14 GMT
ENTRYPOINT ["entrypoint.sh"]
# Fri, 28 Jul 2023 03:37:14 GMT
USER adminer
# Fri, 28 Jul 2023 03:37:14 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:ba7a048f0d1295609b34eb062a51486e1f3e5831711b4569a3583b1e8ad30aff`  
		Last Modified: Thu, 27 Jul 2023 23:29:55 GMT  
		Size: 58.9 MB (58927464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ba9f4dcf2cf661540f55aa430994db9976b0d0cf5c331ccb083fea9de76c3ba`  
		Last Modified: Fri, 28 Jul 2023 03:37:47 GMT  
		Size: 40.9 MB (40940233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d31b2900ea5c26c04bf525ec99856ed15bbf9d9898f624ab02e6cbcd2e60fcb`  
		Last Modified: Fri, 28 Jul 2023 03:37:34 GMT  
		Size: 396.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:529cf8a1db4349bd4f8ee705314ea40cb04343d19184aa59a894519bc520953a`  
		Last Modified: Fri, 28 Jul 2023 03:38:12 GMT  
		Size: 2.7 KB (2714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca599fe1e798b635e96d93d4cc078a1192c1b95f38cd72ac4731ccf97b55531f`  
		Last Modified: Fri, 28 Jul 2023 03:38:12 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8314df486462936fff0b9f0a1ddd02b31ab1e202cef6a9e6752c6ef3e5770263`  
		Last Modified: Fri, 28 Jul 2023 03:38:12 GMT  
		Size: 1.5 KB (1482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8dceb3698a58c57a572cc361bfad944c7f300ae19d84563cae50a85b8f1f947`  
		Last Modified: Fri, 28 Jul 2023 03:38:13 GMT  
		Size: 1.4 MB (1385637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeb4cc899b51bc199e73b04700c208ff8038d3d579fc6780f7759a9cd67bef6d`  
		Last Modified: Fri, 28 Jul 2023 03:38:12 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-fastcgi` - linux; s390x

```console
$ docker pull adminer@sha256:9fa1c4f7fa75a9b9325b3586d51594763c4eb061ae79ea477ad194ef6786698e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.7 MB (93701693 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9719bdd2c7db5ced4d9b223e02555231fa784bde63ef93d2f881bf581acb3b94`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Tue, 15 Aug 2023 23:42:43 GMT
ADD file:021ebd89eb6b326058b4fc3aeca5d0d93925ed29a443618fedef034618e8f2db in / 
# Tue, 15 Aug 2023 23:42:48 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 00:47:01 GMT
STOPSIGNAL SIGINT
# Wed, 16 Aug 2023 00:47:27 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 00:47:30 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 16 Aug 2023 00:47:55 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Wed, 16 Aug 2023 00:47:55 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 16 Aug 2023 00:47:56 GMT
WORKDIR /var/www/html
# Wed, 16 Aug 2023 00:47:56 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 16 Aug 2023 00:47:56 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 16 Aug 2023 00:47:56 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 16 Aug 2023 00:47:56 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 16 Aug 2023 00:48:07 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 16 Aug 2023 00:48:07 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 16 Aug 2023 00:48:07 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 16 Aug 2023 00:48:07 GMT
USER adminer
# Wed, 16 Aug 2023 00:48:07 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:cf9beb6f1941863d1df3b7a9c4f925894662762a3ceeba920f164d9e8c8bab57`  
		Last Modified: Tue, 15 Aug 2023 23:48:07 GMT  
		Size: 53.3 MB (53290642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:149dffe2a2896e8669cb349d5f67fe3b89051471d76167385fcab52080c46072`  
		Last Modified: Wed, 16 Aug 2023 00:48:32 GMT  
		Size: 39.0 MB (39018607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d19064071a2db22f3cd7e9ff62da91d06a100a18460f7afbdaba2b17275e469a`  
		Last Modified: Wed, 16 Aug 2023 00:48:25 GMT  
		Size: 388.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f4984abdce2d0e22ddd5708e45515083589343c64c7791d42b2f56fc2d96b1e`  
		Last Modified: Wed, 16 Aug 2023 00:48:42 GMT  
		Size: 2.7 KB (2707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86edcaab719cfd78ecc40e1b20146735a3e15be2afa63ed7d1f1ea437e27d9a0`  
		Last Modified: Wed, 16 Aug 2023 00:48:42 GMT  
		Size: 1.9 KB (1880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fb1e2221039e7a139c3bdfb0c56a40478d6d8e60bcf2c35187b144c59b906fc`  
		Last Modified: Wed, 16 Aug 2023 00:48:42 GMT  
		Size: 1.5 KB (1480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e2b7270c2add1c1ec9ee2e0ae846da3339a35af9953f862124a418c887bf27a`  
		Last Modified: Wed, 16 Aug 2023 00:48:42 GMT  
		Size: 1.4 MB (1385496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1eb6c6e2ad7edd5d645d00e8c4b98a6d3ce529a419d8bb40ab7c65a6e972a5a`  
		Last Modified: Wed, 16 Aug 2023 00:48:42 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
