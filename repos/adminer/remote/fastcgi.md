## `adminer:fastcgi`

```console
$ docker pull adminer@sha256:3621caa2caf129607cac044fa1518ad74df9b41ed8902491fd8cba4b012226aa
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
$ docker pull adminer@sha256:35e5285bea82c78b08355dc314739f980e2437cbf1c9e51291b5168fd5cd6f75
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.9 MB (95924422 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23fae11ad3f1ae58e8aa6d5af50bb131d52fd3b3fadbb2c8e22e67ceca7a76d7`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Thu, 23 Mar 2023 01:30:15 GMT
ADD file:459d1e92eb8c24ff4758f974d289ca8a2abe04cf50b6fe2bd760aa4589478289 in / 
# Thu, 23 Mar 2023 01:30:15 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 05:55:49 GMT
STOPSIGNAL SIGINT
# Thu, 23 Mar 2023 05:56:13 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 05:56:13 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Thu, 23 Mar 2023 05:56:30 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Thu, 23 Mar 2023 05:56:30 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 23 Mar 2023 05:56:30 GMT
WORKDIR /var/www/html
# Thu, 23 Mar 2023 05:56:30 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 23 Mar 2023 05:56:30 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 23 Mar 2023 05:56:31 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 23 Mar 2023 05:56:31 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 23 Mar 2023 05:56:41 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Mar 2023 05:56:41 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 23 Mar 2023 05:56:41 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 23 Mar 2023 05:56:41 GMT
USER adminer
# Thu, 23 Mar 2023 05:56:42 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:3e440a7045683e27f8e2fa04000e0e078d8dfac0c971358ae0f8c65c13321c8e`  
		Last Modified: Thu, 23 Mar 2023 01:34:00 GMT  
		Size: 55.0 MB (55045608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d6386bc062c6cf91f6c1451db68015d43a1afd7d67a8f0710050e557777a30a`  
		Last Modified: Thu, 23 Mar 2023 05:57:00 GMT  
		Size: 39.5 MB (39486568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dbc633dab938fa31a0afdfe3ac449318f04eb42e13b59c2602178aed2af127e`  
		Last Modified: Thu, 23 Mar 2023 05:56:53 GMT  
		Size: 394.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15e43c5bb8d604942de8a801fbd515cde458e8296cda94b628a1a311281fe880`  
		Last Modified: Thu, 23 Mar 2023 05:57:17 GMT  
		Size: 2.7 KB (2712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:991cbf4d6fdd0b401219e6f0c1474c3c379889e229e8305e5c7afc86459d6599`  
		Last Modified: Thu, 23 Mar 2023 05:57:16 GMT  
		Size: 1.9 KB (1878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:420cfe44d3089c8454b9568ad65803581ce9a8565536455cf2602d4b96ff6e35`  
		Last Modified: Thu, 23 Mar 2023 05:57:16 GMT  
		Size: 1.5 KB (1474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aad56f1c45901a03ae785f94f8dfc35d5689f400e95502fdf74ee2243dd5fd22`  
		Last Modified: Thu, 23 Mar 2023 05:57:17 GMT  
		Size: 1.4 MB (1385298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36974e24611dd62fec010effb08e11fdd389b0898bff3ee057b6bf9266aa3d8e`  
		Last Modified: Thu, 23 Mar 2023 05:57:16 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:fastcgi` - linux; arm variant v5

```console
$ docker pull adminer@sha256:af7d5cd843b0c5e0fa61f5f8bdf40ac5cce6a1d9e7548219b0375b0032c3db6a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.2 MB (91193295 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46e4a3d963ddf1fffc5b6dac3ba2387d5cd51a2ce92801b6ed0da6b2a30ac457`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Wed, 12 Apr 2023 00:48:34 GMT
ADD file:ae13a4cbeb20b92ec29dd7409de47a964fe373bdde2a4e8880b5a4d9dc64171e in / 
# Wed, 12 Apr 2023 00:48:35 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:08:49 GMT
STOPSIGNAL SIGINT
# Wed, 12 Apr 2023 01:09:23 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:09:24 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 12 Apr 2023 01:09:47 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Wed, 12 Apr 2023 01:09:47 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 12 Apr 2023 01:09:47 GMT
WORKDIR /var/www/html
# Wed, 12 Apr 2023 01:09:47 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 12 Apr 2023 01:09:48 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 12 Apr 2023 01:09:48 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 12 Apr 2023 01:09:48 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 12 Apr 2023 01:10:00 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 12 Apr 2023 01:10:00 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 12 Apr 2023 01:10:00 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 12 Apr 2023 01:10:00 GMT
USER adminer
# Wed, 12 Apr 2023 01:10:00 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:86cb8d774eca43d428d6a35506c172ba62358d2d5ec90c886e3b38b297f93b20`  
		Last Modified: Wed, 12 Apr 2023 00:50:46 GMT  
		Size: 52.6 MB (52555175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:476a3376b0ea735669902f869efa8f12e59c8a6a4b7c573898a30e3dd526b682`  
		Last Modified: Wed, 12 Apr 2023 01:10:19 GMT  
		Size: 37.2 MB (37245911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4807b6cf5250094660b54cd243e7aa564b521cd237dddc561ae89aa88ddddd25`  
		Last Modified: Wed, 12 Apr 2023 01:10:10 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad81c1b87298b76455a66adb13eea2dab57bcf70d7fc4b301cac720274fd4607`  
		Last Modified: Wed, 12 Apr 2023 01:10:37 GMT  
		Size: 2.7 KB (2705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91615642e1dc00926ccaa969a350cd5324f4f41c51ed14be6bfdb44e9e231aeb`  
		Last Modified: Wed, 12 Apr 2023 01:10:36 GMT  
		Size: 1.9 KB (1871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d38cdaf408b253fe3ca3adf3dee45f38463603462c4dbb4c07563c53e4b4136`  
		Last Modified: Wed, 12 Apr 2023 01:10:37 GMT  
		Size: 1.5 KB (1477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40ec88bddd643e8649490a6e5b86d6af8d12b2c87615c3d0e55d2d4a33d455f8`  
		Last Modified: Wed, 12 Apr 2023 01:10:37 GMT  
		Size: 1.4 MB (1385277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaa19133b119b1c0fddf06964679c75cbe65486156df3b55a8e78bf4549ed3e5`  
		Last Modified: Wed, 12 Apr 2023 01:10:36 GMT  
		Size: 489.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:fastcgi` - linux; arm variant v7

```console
$ docker pull adminer@sha256:bc666796aa3d0cee0b13bc0afeb827eddb224ac94c2825e90be0b7935f4e8122
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.8 MB (87785110 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8477e704cb362785d6fffb06bca6d401c7163028a20adb041de59c8927810ecc`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Thu, 23 Mar 2023 01:13:21 GMT
ADD file:fa1cbfdd44274e571cabd5ca7fafa08b17c6f497ecfca6368a9eec4d2527a364 in / 
# Thu, 23 Mar 2023 01:13:22 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 13:53:52 GMT
STOPSIGNAL SIGINT
# Thu, 23 Mar 2023 13:54:16 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 13:54:17 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Thu, 23 Mar 2023 13:54:32 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Thu, 23 Mar 2023 13:54:33 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 23 Mar 2023 13:54:33 GMT
WORKDIR /var/www/html
# Thu, 23 Mar 2023 13:54:33 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 23 Mar 2023 13:54:33 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 23 Mar 2023 13:54:33 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 23 Mar 2023 13:54:33 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 23 Mar 2023 13:54:44 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Mar 2023 13:54:44 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 23 Mar 2023 13:54:44 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 23 Mar 2023 13:54:44 GMT
USER adminer
# Thu, 23 Mar 2023 13:54:44 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:d50e868f9a626a3c456c0c52c3b013e87619bbac7798ac0c2acf2a2407303125`  
		Last Modified: Thu, 23 Mar 2023 01:33:00 GMT  
		Size: 50.2 MB (50211788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:750746172b8a677cb809244c17155d7b05d643b2d816de3d8090ff3593de19ea`  
		Last Modified: Thu, 23 Mar 2023 13:55:03 GMT  
		Size: 36.2 MB (36181275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79543298adbabe76f964cc3578ae398897a0bc10ee8ebf4a0a3338a8ee26b6e8`  
		Last Modified: Thu, 23 Mar 2023 13:54:55 GMT  
		Size: 387.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31633dada050baeaf275a6f4e00621a9f3e3224c8045210053670913ba6d6585`  
		Last Modified: Thu, 23 Mar 2023 13:55:19 GMT  
		Size: 2.7 KB (2709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c21aec687480c0c87c1badd06ad8d1bc38a37d87223bc20a78ba010fd626cac`  
		Last Modified: Thu, 23 Mar 2023 13:55:19 GMT  
		Size: 1.9 KB (1870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac9619b29c31046e1d85965461b5a590b86fb5f2f78c27167ec6cfca6f21651e`  
		Last Modified: Thu, 23 Mar 2023 13:55:19 GMT  
		Size: 1.5 KB (1474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bd30156b59e64f168057bb8a5fae751059636af01bb28f176af27932691211a`  
		Last Modified: Thu, 23 Mar 2023 13:55:20 GMT  
		Size: 1.4 MB (1385116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60631e91dd1890dcbae61adf6317c4a7be616954ef21fec67df71f340de0d351`  
		Last Modified: Thu, 23 Mar 2023 13:55:19 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:fastcgi` - linux; arm64 variant v8

```console
$ docker pull adminer@sha256:1bfb248e805a296b6ebbfbc0503dd9e63252493758d7473f8db39c4b5b6e701a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.3 MB (94340473 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:075d1ce35262ea3920f7ee415fbb4e70c8847766389550e31ca857b3c92b19b7`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:42 GMT
ADD file:dd3d4e5fe819950e7d01b44a29dbd790438cd722ba76198910e2597448ab0c6f in / 
# Wed, 12 Apr 2023 00:39:43 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:01:03 GMT
STOPSIGNAL SIGINT
# Wed, 12 Apr 2023 01:01:28 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:01:29 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 12 Apr 2023 01:01:43 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Wed, 12 Apr 2023 01:01:44 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 12 Apr 2023 01:01:44 GMT
WORKDIR /var/www/html
# Wed, 12 Apr 2023 01:01:44 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 12 Apr 2023 01:01:44 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 12 Apr 2023 01:01:44 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 12 Apr 2023 01:01:44 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 12 Apr 2023 01:01:54 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 12 Apr 2023 01:01:54 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 12 Apr 2023 01:01:54 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 12 Apr 2023 01:01:54 GMT
USER adminer
# Wed, 12 Apr 2023 01:01:54 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:dc80b8cdbfd36cb20231d807a50d704945d1df4da8f6e23197ccfcb629970491`  
		Last Modified: Wed, 12 Apr 2023 00:42:14 GMT  
		Size: 53.7 MB (53705529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b93ed407ae4977784108dcfd75cbe01b9fd3c56c91094a14ecb4adac22299329`  
		Last Modified: Wed, 12 Apr 2023 01:02:11 GMT  
		Size: 39.2 MB (39242725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:450caae39c26a307edec3fc846d7725d489f76490ed0ba8f0ca21526f6369999`  
		Last Modified: Wed, 12 Apr 2023 01:02:05 GMT  
		Size: 386.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:655969b296be27f07723b02a6c9779a2570f69d6682ed547069b2611a8ba04a4`  
		Last Modified: Wed, 12 Apr 2023 01:02:28 GMT  
		Size: 2.7 KB (2703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20fbecb1fc2aaf7aaa57c58d35af8a5b7a592a005719eddc315193cfd1299867`  
		Last Modified: Wed, 12 Apr 2023 01:02:28 GMT  
		Size: 1.9 KB (1879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8458447e719c0b332a4e764eee120ae3741dac9e260d7560339c884a8e75bfe0`  
		Last Modified: Wed, 12 Apr 2023 01:02:28 GMT  
		Size: 1.5 KB (1476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7196e16311ea367a868d7ea304af8c5f2a79029f14fb2b07a13e57240ceb4396`  
		Last Modified: Wed, 12 Apr 2023 01:02:29 GMT  
		Size: 1.4 MB (1385284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8a9fb06b011190b238ccb00beacefc9eefd68f4fadb1a213934f85aca24ab0b`  
		Last Modified: Wed, 12 Apr 2023 01:02:28 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:fastcgi` - linux; 386

```console
$ docker pull adminer@sha256:4fec14cf5a78e727b8c74c974ab7d5e4cecd7f2474147a58a4218ddebc02dd87
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.0 MB (96978049 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1b0466b7b74fdb561f8edf82d5292c2ae17b67cdff6e3c10539493ba7fd11f3`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Thu, 23 Mar 2023 00:39:08 GMT
ADD file:f331251c4c21fceff56d13f76442a6334dc355c29ec7450768c1c86a3db1adab in / 
# Thu, 23 Mar 2023 00:39:09 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 21:17:12 GMT
STOPSIGNAL SIGINT
# Thu, 23 Mar 2023 21:17:40 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 21:17:41 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Thu, 23 Mar 2023 21:18:01 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Thu, 23 Mar 2023 21:18:01 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 23 Mar 2023 21:18:01 GMT
WORKDIR /var/www/html
# Thu, 23 Mar 2023 21:18:02 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 23 Mar 2023 21:18:02 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 23 Mar 2023 21:18:02 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 23 Mar 2023 21:18:02 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 23 Mar 2023 21:18:14 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Mar 2023 21:18:14 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 23 Mar 2023 21:18:14 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 23 Mar 2023 21:18:14 GMT
USER adminer
# Thu, 23 Mar 2023 21:18:14 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:c1bb878cff31d37952c5c73ed15c167f599bb7f97b3eeaa1a17352b2473b3394`  
		Last Modified: Thu, 23 Mar 2023 00:42:44 GMT  
		Size: 56.0 MB (56027911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67239d163b3f7b443f91919b613775ed043520e6b06b413a9628905d01e98992`  
		Last Modified: Thu, 23 Mar 2023 21:18:34 GMT  
		Size: 39.6 MB (39558048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88061812377dcf7351518633da4694430dfe02ac13bdbc48516d26c18586a0d5`  
		Last Modified: Thu, 23 Mar 2023 21:18:24 GMT  
		Size: 392.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e265f46cc6fadbfde249ce57b0f1b54264aab3a0c6a1453f7f2699545e0b3204`  
		Last Modified: Thu, 23 Mar 2023 21:18:50 GMT  
		Size: 2.7 KB (2710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca518b34b603a08f7c5881dd84c944bb8236eb9f03a74636f1d2496138c0f756`  
		Last Modified: Thu, 23 Mar 2023 21:18:50 GMT  
		Size: 1.9 KB (1869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c12e6b62649c51d5b810142e53b66da078b62baadc21eecf203444c93de1263`  
		Last Modified: Thu, 23 Mar 2023 21:18:50 GMT  
		Size: 1.5 KB (1476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85f8a77bc64220b5352e77dfca8700a11755ee9d00cb280da618809bcaefc541`  
		Last Modified: Thu, 23 Mar 2023 21:18:50 GMT  
		Size: 1.4 MB (1385152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee9c79da4d828244f71b3b0c18abe0d34506e6202fb0c07c7b38bcb553ff9361`  
		Last Modified: Thu, 23 Mar 2023 21:18:50 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:fastcgi` - linux; mips64le

```console
$ docker pull adminer@sha256:6071b807c18fd9c3a868729b6c008a72c4f33193d038d3266c552a13c81c2ebe
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.6 MB (92608465 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8730ff222f47754b556a9a28db99999e3b00e5f51261ff97b8c794f168b61cdf`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Thu, 23 Mar 2023 05:17:18 GMT
ADD file:2337efa705c8772705fa8519e513f4299e72c9eb63e3a68069778ca95a1511e6 in / 
# Thu, 23 Mar 2023 05:17:24 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 20:06:00 GMT
STOPSIGNAL SIGINT
# Thu, 23 Mar 2023 20:07:56 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 20:08:02 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Thu, 23 Mar 2023 20:09:46 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Thu, 23 Mar 2023 20:09:52 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 23 Mar 2023 20:09:56 GMT
WORKDIR /var/www/html
# Thu, 23 Mar 2023 20:09:59 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 23 Mar 2023 20:10:02 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 23 Mar 2023 20:10:06 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 23 Mar 2023 20:10:09 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 23 Mar 2023 20:11:02 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Mar 2023 20:11:04 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 23 Mar 2023 20:11:08 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 23 Mar 2023 20:11:11 GMT
USER adminer
# Thu, 23 Mar 2023 20:11:14 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:f3951ee58695b4d906b37f2d9a07e6158f66a7328d0c70445d9607cd8367ede0`  
		Last Modified: Thu, 23 Mar 2023 05:25:08 GMT  
		Size: 53.3 MB (53264720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1180d0aa65a6936ad9b336fd7ddf64160d0a95203d7f3d82027fe8912c936d73`  
		Last Modified: Thu, 23 Mar 2023 20:11:59 GMT  
		Size: 38.0 MB (37950695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21a23105a66b5d86b4852f9dcf6753d154e1d5b3b76c178cf8baced410a4deb2`  
		Last Modified: Thu, 23 Mar 2023 20:11:33 GMT  
		Size: 396.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94f6b792b9dbc62affd1f59a5c64bae91e7a40650b891a2227ee50499b244671`  
		Last Modified: Thu, 23 Mar 2023 20:12:18 GMT  
		Size: 2.7 KB (2713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2bd7b3264510c2ff115b5bde0691e4507a8037e8afac4227a80c9b20927cd71`  
		Last Modified: Thu, 23 Mar 2023 20:12:18 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ede1a6707d65116cd7175d9a72eb51517e94fd922e91749a84b539c88f0c1cbc`  
		Last Modified: Thu, 23 Mar 2023 20:12:18 GMT  
		Size: 1.5 KB (1480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:532cd52f2b4a83b3f92484a39a21601e8bcf404137a7665b958c9589d2a56c97`  
		Last Modified: Thu, 23 Mar 2023 20:12:19 GMT  
		Size: 1.4 MB (1386242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:799eb60dea8fba148d5d409a75beb6c1f6decb8507259a122daedabe15408244`  
		Last Modified: Thu, 23 Mar 2023 20:12:18 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:fastcgi` - linux; ppc64le

```console
$ docker pull adminer@sha256:a035556296071d36e8a78a9fb4e6e566b030d8a04b2b961ce4a8874ed96af628
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.3 MB (101258778 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f3ec485bcf5a9208a03ffaaeffd1c6aa4408c565e11ce559ec629652c041a6a`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Wed, 12 Apr 2023 00:07:58 GMT
ADD file:c3c2a10473ddaa3d8a30ca99b19ad3599d0e60d826c4e0315bdb7463352ebc09 in / 
# Wed, 12 Apr 2023 00:08:02 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:18:49 GMT
STOPSIGNAL SIGINT
# Wed, 12 Apr 2023 01:20:27 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:20:34 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 12 Apr 2023 01:21:46 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Wed, 12 Apr 2023 01:21:51 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 12 Apr 2023 01:21:52 GMT
WORKDIR /var/www/html
# Wed, 12 Apr 2023 01:21:52 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 12 Apr 2023 01:21:53 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 12 Apr 2023 01:21:54 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 12 Apr 2023 01:21:56 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 12 Apr 2023 01:22:26 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 12 Apr 2023 01:22:27 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 12 Apr 2023 01:22:27 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 12 Apr 2023 01:22:28 GMT
USER adminer
# Wed, 12 Apr 2023 01:22:28 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:2d3ffdd4610a019889b845cc82b3d956ad85cca78ad4bff2d5e5522bd02c17e7`  
		Last Modified: Wed, 12 Apr 2023 00:12:37 GMT  
		Size: 58.9 MB (58926600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30b3857ba4d1c287f4bd1c09595f9053294a6077e3f60bd68c3fc212cec07ef7`  
		Last Modified: Wed, 12 Apr 2023 01:22:55 GMT  
		Size: 40.9 MB (40939523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa98a0c9bd42966fed41c5eda2aa7dcfe4f8c159749750edece4a361c0dc8f78`  
		Last Modified: Wed, 12 Apr 2023 01:22:40 GMT  
		Size: 396.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f3013369f8e95d2665949e23f195080aa4f2f49cf345bb284164747c93462b1`  
		Last Modified: Wed, 12 Apr 2023 01:23:13 GMT  
		Size: 2.7 KB (2716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d18d6e52ddde5322eb2c03d3776619d697508750da16a1a0f486064299a5e67c`  
		Last Modified: Wed, 12 Apr 2023 01:23:13 GMT  
		Size: 1.9 KB (1887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c6bceca607df37463b3d4edc6d7f1fdbd6c21fa7d17c23ea3f37029b4fef209`  
		Last Modified: Wed, 12 Apr 2023 01:23:13 GMT  
		Size: 1.5 KB (1481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7b5fb8c400ebb27e4513d1d29cc8ae5b6498e173b9ab0b418e0220d47eb350a`  
		Last Modified: Wed, 12 Apr 2023 01:23:13 GMT  
		Size: 1.4 MB (1385683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2f726494151054c4e7bb459b16a7c23209309d0be5221352f98027fed1913af`  
		Last Modified: Wed, 12 Apr 2023 01:23:13 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:fastcgi` - linux; s390x

```console
$ docker pull adminer@sha256:8fa537ed86e381074d357ce04c564bae5f507acf4188d3aa3e675a13e59716cf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.7 MB (93696767 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d7dcdae7e32897b325d716cb2131024c2344546e66d30f86aca7cb245499cf34`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Wed, 12 Apr 2023 00:00:25 GMT
ADD file:ab4e28724d04724a57e0f5bbe299d3361103f05ad1978dc3bfef243c1f9d6476 in / 
# Wed, 12 Apr 2023 00:00:38 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 00:22:19 GMT
STOPSIGNAL SIGINT
# Wed, 12 Apr 2023 00:22:42 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 00:22:45 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 12 Apr 2023 00:23:08 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Wed, 12 Apr 2023 00:23:09 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 12 Apr 2023 00:23:09 GMT
WORKDIR /var/www/html
# Wed, 12 Apr 2023 00:23:10 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 12 Apr 2023 00:23:10 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 12 Apr 2023 00:23:10 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 12 Apr 2023 00:23:10 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 12 Apr 2023 00:23:22 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 12 Apr 2023 00:23:22 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 12 Apr 2023 00:23:22 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 12 Apr 2023 00:23:23 GMT
USER adminer
# Wed, 12 Apr 2023 00:23:23 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:042263756d7dc47bf98a243871107aa3a2b41acda91d104d8b4e148749a43dda`  
		Last Modified: Wed, 12 Apr 2023 00:05:03 GMT  
		Size: 53.3 MB (53286682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7d938e9b1334125563c9088a8d038623c2c771370baf0646a8b00dc75c5022a`  
		Last Modified: Wed, 12 Apr 2023 00:23:48 GMT  
		Size: 39.0 MB (39017681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccf86a2177eddadeff3c335ab21b72d776f97342c6d260ba5574cb81c3eeda25`  
		Last Modified: Wed, 12 Apr 2023 00:23:41 GMT  
		Size: 386.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dea6db7217edba5f8e49cbee261ad2ea9c96c10c83038a17071518884d1c81e6`  
		Last Modified: Wed, 12 Apr 2023 00:23:56 GMT  
		Size: 2.7 KB (2707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:881082d16d120a5a8f050b1cdc4abefb32e4247674e69a600e1b2f019bf126e0`  
		Last Modified: Wed, 12 Apr 2023 00:23:55 GMT  
		Size: 1.9 KB (1875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e8b292e6ee64bda9332845e064826af581a04d7d69f09c6d33ea7f091742a1e`  
		Last Modified: Wed, 12 Apr 2023 00:23:55 GMT  
		Size: 1.5 KB (1473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d792e42a83bf2a4947f67042cf923515e418d9ec97cf08b7b58924d139a59f9b`  
		Last Modified: Wed, 12 Apr 2023 00:23:56 GMT  
		Size: 1.4 MB (1385474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecc070176a58f6105215209e8c6e8bcdc1d0f55c8540d08fb580df7d1f8b8ced`  
		Last Modified: Wed, 12 Apr 2023 00:23:55 GMT  
		Size: 489.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
