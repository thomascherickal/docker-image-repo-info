## `adminer:4-fastcgi`

```console
$ docker pull adminer@sha256:75c94332fac70eb4b08bfdfc58a5bc6e2b5bf5d72430e0e85328135ff415a42d
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
$ docker pull adminer@sha256:2678cfe1bac45aff1cce3d35cb8619c66c1fae70b9eefd481d3067779ba67f1b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.9 MB (95943930 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75613f9996e37b744f9ddd5867e5daaa901ef4e8f48d528c43dd7aefea7c82e8`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Wed, 01 Nov 2023 00:20:59 GMT
ADD file:da3938f00f114fa8f5948fb7182da39c43e5ce57a334ba528681cb29aff0d2f6 in / 
# Wed, 01 Nov 2023 00:21:00 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:53:18 GMT
STOPSIGNAL SIGINT
# Wed, 01 Nov 2023 02:53:37 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:53:38 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 01 Nov 2023 02:53:59 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Wed, 01 Nov 2023 02:54:00 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 01 Nov 2023 02:54:00 GMT
WORKDIR /var/www/html
# Wed, 01 Nov 2023 02:54:00 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 01 Nov 2023 02:54:00 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 01 Nov 2023 02:54:00 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 01 Nov 2023 02:54:00 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 01 Nov 2023 02:54:11 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 01 Nov 2023 02:54:11 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 01 Nov 2023 02:54:11 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 01 Nov 2023 02:54:11 GMT
USER adminer
# Wed, 01 Nov 2023 02:54:11 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:2f088d622efd8dbaa13d01eafd0aac8f9f33bb335edd3be897ae8059338c7bf7`  
		Last Modified: Wed, 01 Nov 2023 00:25:49 GMT  
		Size: 55.1 MB (55058052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd255731bd34ffbaeeb0e7122cdcfaf791a378401b03bfef73da5f788aacec61`  
		Last Modified: Wed, 01 Nov 2023 02:54:32 GMT  
		Size: 39.5 MB (39492562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57b2e70d364cdf760120433daf3df38518ee4e5b81ec1d93d6fc291d3608975c`  
		Last Modified: Wed, 01 Nov 2023 02:54:24 GMT  
		Size: 385.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d8cd29f8617a8a6475c7def037cd28689fafd9d39ccad4a5ef248ad7b4db1c5`  
		Last Modified: Wed, 01 Nov 2023 02:54:50 GMT  
		Size: 2.7 KB (2708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41c27cf0f45a20bf4551dbf4606a1b65e1be973cffd2aac8e4f54a461e02df0e`  
		Last Modified: Wed, 01 Nov 2023 02:54:50 GMT  
		Size: 1.9 KB (1876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c639f2506b71131d1822febe3a4145d2727083406102e3a180d2488f46c389b2`  
		Last Modified: Wed, 01 Nov 2023 02:54:50 GMT  
		Size: 1.5 KB (1478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f9899132a5c1851176d9eba2260c954c7b227a0c3dd7287bb4ce930135c2dca`  
		Last Modified: Wed, 01 Nov 2023 02:54:51 GMT  
		Size: 1.4 MB (1386378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:608c8edc058d26a233dc77fb4b0d67671dda46c41663c4dfd4e1236752a1d57e`  
		Last Modified: Wed, 01 Nov 2023 02:54:50 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-fastcgi` - linux; arm variant v5

```console
$ docker pull adminer@sha256:cf54637c6bab998c72c9678a04d9218750adcaebe9f67fd6854cc94dc0ccecb2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.2 MB (91205859 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ce16013b8f7e48113e20e1e26ba7f4c9c7d04bed540f0f50ce28edc227e1be5`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Wed, 11 Oct 2023 17:37:51 GMT
ADD file:dd011733a11e4681328b2d45bbfc478e1dab88a95554fe817e238ef27b1865c2 in / 
# Wed, 11 Oct 2023 17:37:51 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:02:22 GMT
STOPSIGNAL SIGINT
# Wed, 11 Oct 2023 18:02:53 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 18:02:54 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 11 Oct 2023 18:03:20 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Wed, 11 Oct 2023 18:03:21 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 11 Oct 2023 18:03:21 GMT
WORKDIR /var/www/html
# Wed, 11 Oct 2023 18:03:21 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 11 Oct 2023 18:03:21 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 11 Oct 2023 18:03:21 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 11 Oct 2023 18:03:21 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 11 Oct 2023 18:03:34 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 11 Oct 2023 18:03:34 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 11 Oct 2023 18:03:34 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 11 Oct 2023 18:03:34 GMT
USER adminer
# Wed, 11 Oct 2023 18:03:34 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:d310e2405531cf391481a06c9f4d0fc75165ad8e3025e4035c6be5245b6cc754`  
		Last Modified: Wed, 11 Oct 2023 17:41:07 GMT  
		Size: 52.6 MB (52563098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:443e9cae56b2f77ad484572dc0a9714a64bdf1f0c17d3cd769c05ba64acd3318`  
		Last Modified: Wed, 11 Oct 2023 18:03:55 GMT  
		Size: 37.2 MB (37249551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c40a8a6c6f0cb66cd7fc373fe0d13745ee64fd34dfa62bf917040ee74c9c7b4`  
		Last Modified: Wed, 11 Oct 2023 18:03:47 GMT  
		Size: 392.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67db8d6b55c143d145cfeb8c65086e8ab582f16bc87b2b6a9e4bdd870125381e`  
		Last Modified: Wed, 11 Oct 2023 18:04:14 GMT  
		Size: 2.7 KB (2706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ff8a9dc30c5235a8da565ca53d6648a47aa6f04a6c763b778650063d001b36f`  
		Last Modified: Wed, 11 Oct 2023 18:04:14 GMT  
		Size: 1.9 KB (1869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3738b901e2622cecf651abf71e5db4c15046df4102128e60ac4baf38f8a9203d`  
		Last Modified: Wed, 11 Oct 2023 18:04:14 GMT  
		Size: 1.5 KB (1476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2053721087a07bd8ee2716fda82f67f904ce1976febd99b527d396568c198d2`  
		Last Modified: Wed, 11 Oct 2023 18:04:14 GMT  
		Size: 1.4 MB (1386276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:876a7f13c646765145ca55814d3448b1a1c2cfd8c404946503dc759a34e0d716`  
		Last Modified: Wed, 11 Oct 2023 18:04:14 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-fastcgi` - linux; arm variant v7

```console
$ docker pull adminer@sha256:c395427bb1c62231a4e51d6c22f82b627f5bcc1dab6df167779659c93007f0fe
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.8 MB (87796830 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bdc75e7f795b1ae3b9f7fd8da5e07aea4a2e4c38f342b6a3fb11dd4671a3bb93`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Wed, 01 Nov 2023 00:58:01 GMT
ADD file:5e11ff51eeca3d0b7e760186b5792864fee2bfe7e8a1fa531a89870abaebfc89 in / 
# Wed, 01 Nov 2023 00:58:02 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:13:19 GMT
STOPSIGNAL SIGINT
# Wed, 01 Nov 2023 02:13:42 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:13:43 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 01 Nov 2023 02:14:07 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Wed, 01 Nov 2023 02:14:08 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 01 Nov 2023 02:14:08 GMT
WORKDIR /var/www/html
# Wed, 01 Nov 2023 02:14:08 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 01 Nov 2023 02:14:08 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 01 Nov 2023 02:14:08 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 01 Nov 2023 02:14:08 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 01 Nov 2023 02:14:20 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 01 Nov 2023 02:14:20 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 01 Nov 2023 02:14:20 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 01 Nov 2023 02:14:20 GMT
USER adminer
# Wed, 01 Nov 2023 02:14:20 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:17b69ad2612f8fffb539ede3765dcc1fbd121518fd38fe89720482d622dbc960`  
		Last Modified: Wed, 01 Nov 2023 01:02:32 GMT  
		Size: 50.2 MB (50215350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:635ef947586fb2e27bda071f71f4a9180a2bb3e6123995011e82a0a0ce9852cb`  
		Last Modified: Wed, 01 Nov 2023 02:14:40 GMT  
		Size: 36.2 MB (36188235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8124aa326159d3153b18938925162256fff4af20771817f02c9e4774eb60d2d`  
		Last Modified: Wed, 01 Nov 2023 02:14:32 GMT  
		Size: 389.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a33623ce3a57bb9255ea0ef2d86764b90971f93f149f95bf7ad45cb9f1f1af7`  
		Last Modified: Wed, 01 Nov 2023 02:14:58 GMT  
		Size: 2.7 KB (2709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91f64fd86ec605c0027de8d1c32a23b5399516d484b792ced733c95fc78adc04`  
		Last Modified: Wed, 01 Nov 2023 02:14:58 GMT  
		Size: 1.9 KB (1869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a810f2c96e39ad259cdbec8173b08af962499d830021250620c49596f53761ac`  
		Last Modified: Wed, 01 Nov 2023 02:14:58 GMT  
		Size: 1.5 KB (1481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f93e04802d36ad782691b235ae3504c3a4dd6c80b898ce0863de8518b43d5eb`  
		Last Modified: Wed, 01 Nov 2023 02:14:59 GMT  
		Size: 1.4 MB (1386306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4137fd861cde50b6d5c0db8464f2bd7ac743e2e8b7145aa5fe910c5d9752f000`  
		Last Modified: Wed, 01 Nov 2023 02:14:58 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-fastcgi` - linux; arm64 variant v8

```console
$ docker pull adminer@sha256:c901345d5e4b20a6c9f5ea0251ec9f4ab9935f12bec08e6937775408b243fe2e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.3 MB (94346570 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f06afa436e79e23f6612cb17b654c62b943cd4e4d977bee73fa024d725028e77`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Wed, 01 Nov 2023 00:39:48 GMT
ADD file:f5677286e85ce6a345c7f5937e1ec576c37228e49c0fafe33574614c81cb7f76 in / 
# Wed, 01 Nov 2023 00:39:48 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:01:19 GMT
STOPSIGNAL SIGINT
# Wed, 01 Nov 2023 02:01:38 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:01:39 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 01 Nov 2023 02:01:53 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Wed, 01 Nov 2023 02:01:54 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 01 Nov 2023 02:01:54 GMT
WORKDIR /var/www/html
# Wed, 01 Nov 2023 02:01:54 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 01 Nov 2023 02:01:54 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 01 Nov 2023 02:01:54 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 01 Nov 2023 02:01:54 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 01 Nov 2023 02:02:04 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 01 Nov 2023 02:02:05 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 01 Nov 2023 02:02:05 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 01 Nov 2023 02:02:05 GMT
USER adminer
# Wed, 01 Nov 2023 02:02:05 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:d42ebdfc37acca5c3acbe173ac11133e691b402003a525c2b8431baf6935291e`  
		Last Modified: Wed, 01 Nov 2023 00:43:25 GMT  
		Size: 53.7 MB (53707757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a8faaa0e4b3fa7576a18cf79350128bcabc7be2af68de8151a44858d4bd415d`  
		Last Modified: Wed, 01 Nov 2023 02:02:22 GMT  
		Size: 39.2 MB (39245613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a5707356671f48388aa2feae2306f112707a0279084767d7b67d54446689739`  
		Last Modified: Wed, 01 Nov 2023 02:02:15 GMT  
		Size: 391.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21b6774d828bbd5f253cd3ed65db500b421ce842d836da200e7d1ef9e2524e18`  
		Last Modified: Wed, 01 Nov 2023 02:02:40 GMT  
		Size: 2.7 KB (2705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f695e03ad4044720262a1ad0c39bf2b10af31482d5edc78a5177a4a864026c5d`  
		Last Modified: Wed, 01 Nov 2023 02:02:40 GMT  
		Size: 1.9 KB (1877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec5fce5d6ad56c7bb4638b4c672df97512584e0eb0f0502a458bdf4e6744c980`  
		Last Modified: Wed, 01 Nov 2023 02:02:40 GMT  
		Size: 1.5 KB (1476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37c2e5d298c29f859475dda49f90f4b78442b90ca78db0528a29fcfb00df9acf`  
		Last Modified: Wed, 01 Nov 2023 02:02:41 GMT  
		Size: 1.4 MB (1386260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a297c34b866c8d430f191f7d4cfb0fa802114db721c88f46dc50d1a5f76cc1b2`  
		Last Modified: Wed, 01 Nov 2023 02:02:40 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-fastcgi` - linux; 386

```console
$ docker pull adminer@sha256:a111a65f1623cfabc9bdd62a184acb88c4c0d454462ab6c01b84580a68b24983
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.0 MB (97000234 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a1d810fef61fcab3cc4f3dd37b7f298cf025d41ab27dc9785eb010da5b2c43f`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Wed, 11 Oct 2023 17:40:52 GMT
ADD file:a3c1e94bb116d940a614a5275c69bacbac46e00da2070b5c7a561e64b975acc6 in / 
# Wed, 11 Oct 2023 17:40:53 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:07:31 GMT
STOPSIGNAL SIGINT
# Wed, 11 Oct 2023 18:08:01 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 18:08:02 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 11 Oct 2023 18:08:30 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Wed, 11 Oct 2023 18:08:30 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 11 Oct 2023 18:08:30 GMT
WORKDIR /var/www/html
# Wed, 11 Oct 2023 18:08:30 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 11 Oct 2023 18:08:30 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 11 Oct 2023 18:08:31 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 11 Oct 2023 18:08:31 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 11 Oct 2023 18:08:43 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 11 Oct 2023 18:08:43 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 11 Oct 2023 18:08:44 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 11 Oct 2023 18:08:44 GMT
USER adminer
# Wed, 11 Oct 2023 18:08:44 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:081c634ff059d5636b4292d84d0b49429030b3dca70ca56828543b295adb9d47`  
		Last Modified: Wed, 11 Oct 2023 17:45:55 GMT  
		Size: 56.0 MB (56046358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1baa986d052fcee62df8ea7961807d40dbe2dfe7e59dd142133401f557bf3261`  
		Last Modified: Wed, 11 Oct 2023 18:09:06 GMT  
		Size: 39.6 MB (39560625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da6f6ea237aab0ba5befaca621f1d6a6e4cd5ca24f194cf46ad6081f70f20167`  
		Last Modified: Wed, 11 Oct 2023 18:08:55 GMT  
		Size: 393.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b698a7bf082d1e03ce767a5723794b51eb72f60caaca4400af1ec095c5390ae9`  
		Last Modified: Wed, 11 Oct 2023 18:09:26 GMT  
		Size: 2.7 KB (2711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1859dc319a792f9c82c46abcbe08c302520739ffa26ea51f2393cd51aa081f58`  
		Last Modified: Wed, 11 Oct 2023 18:09:27 GMT  
		Size: 1.9 KB (1873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23ac0ab1892e27fc7e5d1559fc31cc9ad96d9158ead73647af1a94a712a6e66d`  
		Last Modified: Wed, 11 Oct 2023 18:09:26 GMT  
		Size: 1.5 KB (1477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cc539514b47d07799366f03e8745b42be4749281b8d8e8b80ffc5fd37179641`  
		Last Modified: Wed, 11 Oct 2023 18:09:27 GMT  
		Size: 1.4 MB (1386306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1d99501989b9a06d57a67b252c1af1aed5d1db16100fe414cd200b4d5129bd5`  
		Last Modified: Wed, 11 Oct 2023 18:09:26 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-fastcgi` - linux; mips64le

```console
$ docker pull adminer@sha256:328d66769d19a331588385e848a8ce1f0f687c16e4dca32dc081a853ab7e55a7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.6 MB (92635209 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5f3531a02b497a897f5b79d2b9b3af053d914fbb73614d1a000a126e460712d`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Wed, 11 Oct 2023 17:50:06 GMT
ADD file:c4be7fca661f2a8181ee1e05fda057c18a2d7c1ae0e08ab63b2c5567ef9cc0a7 in / 
# Wed, 11 Oct 2023 17:50:12 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 20:23:09 GMT
STOPSIGNAL SIGINT
# Wed, 11 Oct 2023 20:25:08 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 20:25:14 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 11 Oct 2023 20:26:56 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Wed, 11 Oct 2023 20:27:03 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 11 Oct 2023 20:27:06 GMT
WORKDIR /var/www/html
# Wed, 11 Oct 2023 20:27:09 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 11 Oct 2023 20:27:12 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 11 Oct 2023 20:27:16 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 11 Oct 2023 20:27:19 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 11 Oct 2023 20:28:09 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 11 Oct 2023 20:28:12 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 11 Oct 2023 20:28:15 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 11 Oct 2023 20:28:18 GMT
USER adminer
# Wed, 11 Oct 2023 20:28:22 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:d237f50a9f05adf465246bef37e194e1d7a226224c7f90ae7b55925c5b509d15`  
		Last Modified: Wed, 11 Oct 2023 18:01:27 GMT  
		Size: 53.3 MB (53289043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c47d62de6e8ad724b1d6e6f03c856be01bb1fce075661d19c22f55750e44be6`  
		Last Modified: Wed, 11 Oct 2023 20:29:11 GMT  
		Size: 38.0 MB (37952175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2946dbeadd8fac118c8daca691914f39feb250dfa5bbd8cc62c35456691daf4b`  
		Last Modified: Wed, 11 Oct 2023 20:28:45 GMT  
		Size: 393.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a8fafb0aca4889ea70fab3e7ab7e9718887a60641872248bfa0cbff9b4a3a25`  
		Last Modified: Wed, 11 Oct 2023 20:29:33 GMT  
		Size: 2.7 KB (2712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69727416efe4eddc03f73b08121915499edf2d565678d0b7872a31b219edc2ec`  
		Last Modified: Wed, 11 Oct 2023 20:29:33 GMT  
		Size: 1.7 KB (1729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4afe1a45577a26cc2e1c3819869c0480af33ddc05832299d5eb8d7af75aad20c`  
		Last Modified: Wed, 11 Oct 2023 20:29:33 GMT  
		Size: 1.5 KB (1479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca972504c1f037f89d2afc734001c4c2d47920003a78984a76138fdff963796b`  
		Last Modified: Wed, 11 Oct 2023 20:29:34 GMT  
		Size: 1.4 MB (1387186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2286a562844acde2f2fdf442f1b230f3387d80e78ea2eb4189d7f61019aacf98`  
		Last Modified: Wed, 11 Oct 2023 20:29:33 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-fastcgi` - linux; ppc64le

```console
$ docker pull adminer@sha256:44e1446e068c82daabe6fa0f88996d227d515d0132909c61025a87bf1ca8bd8a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.3 MB (101267942 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a46eaa8f02d5f28b76ae06bf00efbdafb5a09180fd9b90f169b8a486cf822f24`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Wed, 01 Nov 2023 00:21:51 GMT
ADD file:68e9024f0c99fe38d7046b4ad1aee044d14b93d248ec431380a1cefcacb7dea3 in / 
# Wed, 01 Nov 2023 00:21:54 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:49:04 GMT
STOPSIGNAL SIGINT
# Wed, 01 Nov 2023 02:50:05 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:50:09 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 01 Nov 2023 02:50:58 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Wed, 01 Nov 2023 02:51:00 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 01 Nov 2023 02:51:00 GMT
WORKDIR /var/www/html
# Wed, 01 Nov 2023 02:51:00 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 01 Nov 2023 02:51:01 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 01 Nov 2023 02:51:01 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 01 Nov 2023 02:51:02 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 01 Nov 2023 02:51:24 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 01 Nov 2023 02:51:24 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 01 Nov 2023 02:51:24 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 01 Nov 2023 02:51:24 GMT
USER adminer
# Wed, 01 Nov 2023 02:51:25 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:d002f39ef040587852c73a806a7f49edd2ae7eb78b997c05ca1c5bfedad0506d`  
		Last Modified: Wed, 01 Nov 2023 00:26:33 GMT  
		Size: 58.9 MB (58929494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e777b1c96b7d329900d55d149ff06e1d8e53b10d66d23ccdf70dc13ddf3c015`  
		Last Modified: Wed, 01 Nov 2023 02:51:50 GMT  
		Size: 40.9 MB (40945027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b93c565d3bf6de65a9b0059e37b9c0a6bd056346c6f9c1378364d49ffd169edf`  
		Last Modified: Wed, 01 Nov 2023 02:51:41 GMT  
		Size: 394.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41cec21ca437a44d714ef4e9e66ef5e5d5a86eac1f7ccfb3820961691a875647`  
		Last Modified: Wed, 01 Nov 2023 02:52:09 GMT  
		Size: 2.7 KB (2713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a6ce23fc43606e7913e7e0e11ae22046a6e5d8873a0ed715970a2fad7275d7d`  
		Last Modified: Wed, 01 Nov 2023 02:52:09 GMT  
		Size: 1.9 KB (1878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb219645ef37f681f1c495fdd906826a26a0583067a87285e7178485e546352e`  
		Last Modified: Wed, 01 Nov 2023 02:52:09 GMT  
		Size: 1.5 KB (1480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a68c4c2203cc5dac2f6c3efa0c1cda7a70e95434fdc0566b02ea18c8f2632460`  
		Last Modified: Wed, 01 Nov 2023 02:52:09 GMT  
		Size: 1.4 MB (1386465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:034dbcf0d1ac8a3ce47aafe33dfe8b012e1927f63f6d649ac6bf87e6b2809055`  
		Last Modified: Wed, 01 Nov 2023 02:52:09 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-fastcgi` - linux; s390x

```console
$ docker pull adminer@sha256:18440dd8c4a5041c6c472736692bd88824faf0aaf0f0446f98ebac0a0c49f490
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.7 MB (93711511 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3776269d784356537bcfa563e0c6b1d8b301168c03b8ddf95eb4c7433a55dfdb`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Wed, 01 Nov 2023 00:42:50 GMT
ADD file:5c168741fe0b80d3b365ae703c082556326a889730963a304b218ab3361d2e8a in / 
# Wed, 01 Nov 2023 00:42:54 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 01:49:50 GMT
STOPSIGNAL SIGINT
# Wed, 01 Nov 2023 01:50:07 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 01:50:09 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 01 Nov 2023 01:50:28 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Wed, 01 Nov 2023 01:50:28 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 01 Nov 2023 01:50:28 GMT
WORKDIR /var/www/html
# Wed, 01 Nov 2023 01:50:28 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 01 Nov 2023 01:50:29 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 01 Nov 2023 01:50:29 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 01 Nov 2023 01:50:29 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 01 Nov 2023 01:50:37 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 01 Nov 2023 01:50:37 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 01 Nov 2023 01:50:37 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 01 Nov 2023 01:50:37 GMT
USER adminer
# Wed, 01 Nov 2023 01:50:37 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:a21b3124d41be76bb35d41f49b041980e640c1ea030b4099c4eaa419414f1618`  
		Last Modified: Wed, 01 Nov 2023 00:48:19 GMT  
		Size: 53.3 MB (53296572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef22009f839660d6623265e3627693ea3cb57b069bf34be815e28b0a21748859`  
		Last Modified: Wed, 01 Nov 2023 01:51:01 GMT  
		Size: 39.0 MB (39021669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a36c0fc03e6b3decb01866174c4d3c2c715ea87f9eb9ea407518df283369db59`  
		Last Modified: Wed, 01 Nov 2023 01:50:54 GMT  
		Size: 389.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b69b4544ed776c8991808409478226900e001a1d62823a44d6279e19c4a89f5`  
		Last Modified: Wed, 01 Nov 2023 01:51:13 GMT  
		Size: 2.7 KB (2712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d2651baa94037faca7d0b9b35c0d9de23cdc4b6fb0e72d621ef5c3017e4f219`  
		Last Modified: Wed, 01 Nov 2023 01:51:12 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31e9c3bc67d0aeabcfd3b04842ae2d28bbf9c779763129db821d8bf379b1f485`  
		Last Modified: Wed, 01 Nov 2023 01:51:13 GMT  
		Size: 1.5 KB (1476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb32b3e0b9f7e160acd80f77c1d3c19f4c145e42d1eeeac1f3abe827a0fbec10`  
		Last Modified: Wed, 01 Nov 2023 01:51:13 GMT  
		Size: 1.4 MB (1386321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:723fdbf97ad70f4b73870d191ca584b35d1582d8bb432c45549cd5deb1e9b9a4`  
		Last Modified: Wed, 01 Nov 2023 01:51:13 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
