## `adminer:4-fastcgi`

```console
$ docker pull adminer@sha256:fc56eddd0952fc5033572ad8410ad097ef28ee28578ed59fe07577290250d970
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
$ docker pull adminer@sha256:1ce2e284c3c47a559ff7f7e6b92bbffcff760389365d970a224cf63426a1fc9a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.9 MB (95940128 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17feb3361bd1f28a7fe97b345849afa6083f8d29e95048ed457367046ed08a79`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Wed, 20 Sep 2023 04:55:51 GMT
ADD file:85db4f4c5016f51f7112a5d09cb7d4620f565a1379ae4b8a03c5ffc23886a876 in / 
# Wed, 20 Sep 2023 04:55:51 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 07:12:18 GMT
STOPSIGNAL SIGINT
# Wed, 20 Sep 2023 07:12:39 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 07:12:40 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 20 Sep 2023 07:13:00 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Wed, 20 Sep 2023 07:13:00 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 20 Sep 2023 07:13:00 GMT
WORKDIR /var/www/html
# Wed, 20 Sep 2023 07:13:00 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 20 Sep 2023 07:13:01 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 20 Sep 2023 07:13:01 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 20 Sep 2023 07:13:01 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 20 Sep 2023 07:13:13 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 20 Sep 2023 07:13:13 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 20 Sep 2023 07:13:13 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 20 Sep 2023 07:13:13 GMT
USER adminer
# Wed, 20 Sep 2023 07:13:13 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:ddf874abf16cc990e0fd75a154a34ca0a03ee310ad895a18fb62ae15bf4171fb`  
		Last Modified: Wed, 20 Sep 2023 05:00:41 GMT  
		Size: 55.1 MB (55056714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d75c017e041914cfa76f3e160bc849d010bf579f45a5dfd6a01ad9b937be976`  
		Last Modified: Wed, 20 Sep 2023 07:13:33 GMT  
		Size: 39.5 MB (39491043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86e22a4c35d4189406fea6973f81baf951b47e4f523bc8def43a87cf87d5a570`  
		Last Modified: Wed, 20 Sep 2023 07:13:25 GMT  
		Size: 396.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2be07b344c7479bcda7b0ac5662f1a1c76a976957d1ba8daae4a16e24d0c0091`  
		Last Modified: Wed, 20 Sep 2023 07:13:51 GMT  
		Size: 2.7 KB (2711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:713e5f32bbed181f7a83dc669eea89e88b4e4628dd3ab52f7891470c18873f1a`  
		Last Modified: Wed, 20 Sep 2023 07:13:51 GMT  
		Size: 1.9 KB (1878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:570be109bc7e23fb0ad176a5fcd9b7c0df6072e61510130a69b03ca7e29869fd`  
		Last Modified: Wed, 20 Sep 2023 07:13:51 GMT  
		Size: 1.5 KB (1476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9da3ed7669ca06c0c4c8683c52b834967fae0d70a00015c5c70ebc2d2e9c6459`  
		Last Modified: Wed, 20 Sep 2023 07:13:51 GMT  
		Size: 1.4 MB (1385419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d420c2ff91eeb3f7c3b62f9e40cc2e716a256f99792ef59f7ab1270c713dd9f`  
		Last Modified: Wed, 20 Sep 2023 07:13:51 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-fastcgi` - linux; arm variant v5

```console
$ docker pull adminer@sha256:30fb860d38111ae5e200e1bc72d797030c9cd6e0f9fcd9aa3a3b037ce76d2b02
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.2 MB (91198315 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:082971415d23929a8e07ff69a6747114eab59977e6ec92da0d76fc83cadc6fce`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Wed, 20 Sep 2023 00:50:08 GMT
ADD file:36b8026af7713ecb15198f7cb7beff053db2fb1d0cdbba2e05ede6d2067120be in / 
# Wed, 20 Sep 2023 00:50:08 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 09:36:33 GMT
STOPSIGNAL SIGINT
# Wed, 20 Sep 2023 09:37:03 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:37:04 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 20 Sep 2023 09:37:31 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Wed, 20 Sep 2023 09:37:32 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 20 Sep 2023 09:37:32 GMT
WORKDIR /var/www/html
# Wed, 20 Sep 2023 09:37:32 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 20 Sep 2023 09:37:32 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 20 Sep 2023 09:37:32 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 20 Sep 2023 09:37:32 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 20 Sep 2023 09:37:46 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 20 Sep 2023 09:37:46 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 20 Sep 2023 09:37:46 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 20 Sep 2023 09:37:46 GMT
USER adminer
# Wed, 20 Sep 2023 09:37:46 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:791ab9666f498037db4451bb82dd3cb63afd5ef69c2068959d5516a7832d373b`  
		Last Modified: Wed, 20 Sep 2023 00:55:10 GMT  
		Size: 52.6 MB (52558199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42c6a5c4114fda0a3d42472c8fd27d59859d0854ffcf94d2d76a003703271f94`  
		Last Modified: Wed, 20 Sep 2023 09:38:06 GMT  
		Size: 37.2 MB (37247819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:431cf5c7371a94a9f9956eddd018c5ee7b12bb5ee8e0a206bc2f201854619f2a`  
		Last Modified: Wed, 20 Sep 2023 09:37:57 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da17e0d1764a0c04ab883f9a77f2b5110524f48a3855be95815b8f5d90361e5a`  
		Last Modified: Wed, 20 Sep 2023 09:38:22 GMT  
		Size: 2.7 KB (2705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99370f60e8feb9b7b183b334ed1e7a3e906174b20e1589c7696538f605056b48`  
		Last Modified: Wed, 20 Sep 2023 09:38:22 GMT  
		Size: 1.9 KB (1870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d5baeb890050261e4c650617ef302533a3e09b084d7018996bdf325b38bce5a`  
		Last Modified: Wed, 20 Sep 2023 09:38:22 GMT  
		Size: 1.5 KB (1476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e502697173a4f682bf16c9acc3d0d7417879d62ba6018df9a1de445269649ceb`  
		Last Modified: Wed, 20 Sep 2023 09:38:23 GMT  
		Size: 1.4 MB (1385367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:361379c40577168dc19a349b6713cbed93f7b6f83f909ff47afa604152c69e6a`  
		Last Modified: Wed, 20 Sep 2023 09:38:22 GMT  
		Size: 489.0 B  
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
$ docker pull adminer@sha256:54f6ad6083d340774444cadeb370405fa6f38f23315739c9b965c1ddc62670c5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.6 MB (92615235 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6178cb38fde0107d277d5e8622b36566a8c7525e3e5308b49df7580bd818567e`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Wed, 20 Sep 2023 03:10:35 GMT
ADD file:bf259f6a910dbc8dc738b19ecb6ee305bd4c4542ed155da31ec4169aafd244ff in / 
# Wed, 20 Sep 2023 03:10:40 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 06:38:15 GMT
STOPSIGNAL SIGINT
# Wed, 20 Sep 2023 06:40:06 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 06:40:12 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 20 Sep 2023 06:42:03 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Wed, 20 Sep 2023 06:42:09 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 20 Sep 2023 06:42:13 GMT
WORKDIR /var/www/html
# Wed, 20 Sep 2023 06:42:16 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 20 Sep 2023 06:42:19 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 20 Sep 2023 06:42:22 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 20 Sep 2023 06:42:26 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 20 Sep 2023 06:43:14 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 20 Sep 2023 06:43:17 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 20 Sep 2023 06:43:20 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 20 Sep 2023 06:43:23 GMT
USER adminer
# Wed, 20 Sep 2023 06:43:27 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:0c3ff68a43fe24d06c5623f35f7584c7f4260e244cb03f0be25b1b638b3b2f12`  
		Last Modified: Wed, 20 Sep 2023 03:21:44 GMT  
		Size: 53.3 MB (53271571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca97cf489c2473fe79a050102af5653116104078a63aa4e5c4108dc9029c244e`  
		Last Modified: Wed, 20 Sep 2023 06:44:17 GMT  
		Size: 38.0 MB (37950548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:716a1add5214cc4c65a4591d5c09ce5233784d23f8c4d107ba2692d71999a5e6`  
		Last Modified: Wed, 20 Sep 2023 06:43:50 GMT  
		Size: 395.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcfaa38cfc1bf6e7abbde55da7104336c9a2cd9d5f415dbdff35fb70071795b8`  
		Last Modified: Wed, 20 Sep 2023 06:44:37 GMT  
		Size: 2.7 KB (2713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26b47ab7bd4aa42edb53a3872f4a7bf8e29b875fb7751760d15b2a70ce67d21e`  
		Last Modified: Wed, 20 Sep 2023 06:44:37 GMT  
		Size: 1.7 KB (1729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fd19a0d422cd8995c73b9b1ec74872cc9196d80375a3863f1707934d228b3b9`  
		Last Modified: Wed, 20 Sep 2023 06:44:37 GMT  
		Size: 1.5 KB (1480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67ecd1c280ff793bdce6bd27f710d0952217d921b0ab73f9914e15df5d76a178`  
		Last Modified: Wed, 20 Sep 2023 06:44:37 GMT  
		Size: 1.4 MB (1386308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2e61c50a8863f8f54e4a8767c875794075d6f43047e108a4a10ccb52e06591d`  
		Last Modified: Wed, 20 Sep 2023 06:44:37 GMT  
		Size: 491.0 B  
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
$ docker pull adminer@sha256:36a9da1a4184af8bc64dd0452fd17ce780470415ac871902128f6458a640eb44
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.7 MB (93703905 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cbe588cf10b49c5009c6f198767cbb7bc79936b7cda47e3a5a580a6bfa71ef18`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Wed, 20 Sep 2023 02:54:37 GMT
ADD file:eedfa120b98e158d4eeb9ecad39e28c5715c44bddec3545f61b78ecebd01cc11 in / 
# Wed, 20 Sep 2023 02:54:41 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 09:41:35 GMT
STOPSIGNAL SIGINT
# Wed, 20 Sep 2023 09:42:26 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:42:32 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 20 Sep 2023 09:43:11 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Wed, 20 Sep 2023 09:43:14 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 20 Sep 2023 09:43:14 GMT
WORKDIR /var/www/html
# Wed, 20 Sep 2023 09:43:15 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 20 Sep 2023 09:43:16 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 20 Sep 2023 09:43:16 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 20 Sep 2023 09:43:17 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 20 Sep 2023 09:43:38 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 20 Sep 2023 09:43:38 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 20 Sep 2023 09:43:38 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 20 Sep 2023 09:43:39 GMT
USER adminer
# Wed, 20 Sep 2023 09:43:40 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:d0496e15eebca8286145e6a2cb12c47bb17a28a89cc286a0f7a94763f7713716`  
		Last Modified: Wed, 20 Sep 2023 03:00:01 GMT  
		Size: 53.3 MB (53290747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:271067b46d6984a6b9255ec37e460431e80dd6cb3fb8ac08319a9dba996210fa`  
		Last Modified: Wed, 20 Sep 2023 09:44:05 GMT  
		Size: 39.0 MB (39020558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26dfe3dea64a68a2fce20b0d725a12e7eac50c17b8f845b6567f741009f048ee`  
		Last Modified: Wed, 20 Sep 2023 09:43:57 GMT  
		Size: 394.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72aeec152de0ca6d0060d12959523ee823d05a85332d86512093faeeec0824e1`  
		Last Modified: Wed, 20 Sep 2023 09:44:17 GMT  
		Size: 2.7 KB (2714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd0cf0ac8cd9a7a9343594d359c3d65f4481153d4ad15ab7fc92e248fe6bc43d`  
		Last Modified: Wed, 20 Sep 2023 09:44:17 GMT  
		Size: 1.9 KB (1883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdbe9ac07e2e5b1c404610ecc44f8cc95c0778af02ee58ee058d6b59cf86f1bc`  
		Last Modified: Wed, 20 Sep 2023 09:44:17 GMT  
		Size: 1.5 KB (1481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce13e3236c0515b25f160a6d13c0ce47133103642e0bdfeb76f261bce5052b61`  
		Last Modified: Wed, 20 Sep 2023 09:44:17 GMT  
		Size: 1.4 MB (1385636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:905d41fe127c09ce01f3a68370b5d0e11b813379a25718a8d3f2287a6b2e2cb6`  
		Last Modified: Wed, 20 Sep 2023 09:44:17 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
