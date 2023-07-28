## `adminer:4-standalone`

```console
$ docker pull adminer@sha256:049c27350c7a09912d5a5aeff371ebb5621e021874e38984efaecc90a1ef0315
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
$ docker pull adminer@sha256:30568818ab56dece2d843fd6c0066f2fa1a81aa77311fd79e66f237847e64310
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.9 MB (95932968 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd446bc7686fe85b462cccd3a0df105a2b3ed16e13419ee8c329276cc7ebad0f`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Fri, 28 Jul 2023 02:57:21 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Fri, 28 Jul 2023 02:57:21 GMT
WORKDIR /var/www/html
# Fri, 28 Jul 2023 02:57:21 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Fri, 28 Jul 2023 02:57:21 GMT
ENV ADMINER_VERSION=4.8.1
# Fri, 28 Jul 2023 02:57:22 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Fri, 28 Jul 2023 02:57:22 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Fri, 28 Jul 2023 02:57:33 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 28 Jul 2023 02:57:33 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Fri, 28 Jul 2023 02:57:33 GMT
ENTRYPOINT ["entrypoint.sh"]
# Fri, 28 Jul 2023 02:57:33 GMT
USER adminer
# Fri, 28 Jul 2023 02:57:33 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Fri, 28 Jul 2023 02:57:33 GMT
EXPOSE 8080
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
	-	`sha256:a71b1e29bbc6651cfe4b371c8e7520a4eb2f1264a2eab2e4b913a90b34e96c4a`  
		Last Modified: Fri, 28 Jul 2023 02:58:08 GMT  
		Size: 1.9 KB (1879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cba31560d4271d4cb08074a81e0fd7c5fb1527273607ec76de7de38ae4362d76`  
		Last Modified: Fri, 28 Jul 2023 02:58:07 GMT  
		Size: 1.5 KB (1477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9a622b0a973e460f29f89e9ee8ec702f035ed37420ac9ffa7be7fd2c83270f2`  
		Last Modified: Fri, 28 Jul 2023 02:58:08 GMT  
		Size: 1.4 MB (1385471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e93b37eef6ad5bec83727711d752120e404875e6916fc66c271200936fc953ef`  
		Last Modified: Fri, 28 Jul 2023 02:58:07 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-standalone` - linux; arm variant v5

```console
$ docker pull adminer@sha256:a4cab4a4dc5abe5bc6fb0ea171cc6f440182705b75b165a03c6f9d2bfaa5e91c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.2 MB (91194738 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d93d649448505897c502c7b10bc5917459d8803b31936e70b812e1e04dfcde40`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Thu, 27 Jul 2023 23:48:37 GMT
ADD file:58d46c9e9d20ce33072df369a18845e23a2b275e65c9d7da000c45c336c9c660 in / 
# Thu, 27 Jul 2023 23:48:37 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 06:27:58 GMT
STOPSIGNAL SIGINT
# Fri, 28 Jul 2023 06:28:29 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 06:28:29 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Fri, 28 Jul 2023 06:28:30 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Fri, 28 Jul 2023 06:28:30 GMT
WORKDIR /var/www/html
# Fri, 28 Jul 2023 06:28:30 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Fri, 28 Jul 2023 06:28:30 GMT
ENV ADMINER_VERSION=4.8.1
# Fri, 28 Jul 2023 06:28:30 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Fri, 28 Jul 2023 06:28:31 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Fri, 28 Jul 2023 06:28:43 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 28 Jul 2023 06:28:43 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Fri, 28 Jul 2023 06:28:43 GMT
ENTRYPOINT ["entrypoint.sh"]
# Fri, 28 Jul 2023 06:28:43 GMT
USER adminer
# Fri, 28 Jul 2023 06:28:43 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Fri, 28 Jul 2023 06:28:44 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:2d60a86478b61a7638bb5d1f275e9d6ae0ea994d53a8bb22fce9279ebe477749`  
		Last Modified: Thu, 27 Jul 2023 23:51:48 GMT  
		Size: 52.6 MB (52557094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80fd2ace69283299f6538cc28a7ad7ae32349b3492da875e989459fe02b85376`  
		Last Modified: Fri, 28 Jul 2023 06:29:18 GMT  
		Size: 37.2 MB (37248058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e65c1022b8c9320977b64242ee2c12fb319f6e177cb4b96419da7eb099bf9002`  
		Last Modified: Fri, 28 Jul 2023 06:29:10 GMT  
		Size: 384.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a028453f5b22b9a58effa3d11c1c30135798032b75d2121ec04e321954fd656`  
		Last Modified: Fri, 28 Jul 2023 06:29:10 GMT  
		Size: 1.9 KB (1871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0893d64c43218876f7228e36969ee66eb94d3455b11c928099b5023970b770f1`  
		Last Modified: Fri, 28 Jul 2023 06:29:10 GMT  
		Size: 1.5 KB (1478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11d94613fa65597dbbbedf9f7d8042989c15caa11c4a9d3474744db0d6208e79`  
		Last Modified: Fri, 28 Jul 2023 06:29:10 GMT  
		Size: 1.4 MB (1385360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67e6125be756da11bbd95bd61dbf23b0e5316fd202bbbdd88d7a0c80c43ae8b9`  
		Last Modified: Fri, 28 Jul 2023 06:29:10 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-standalone` - linux; arm variant v7

```console
$ docker pull adminer@sha256:88abb50068b04f3905ca39068b75ca4fddebf0fe616fa73011ce4cecaa5471e3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.8 MB (87791384 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09f0c793d4bbffd38e53d7c1c7d8ff2e487c8ea33d5d2bf28e78e5b08dbffad4`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Fri, 28 Jul 2023 04:00:14 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Fri, 28 Jul 2023 04:00:14 GMT
WORKDIR /var/www/html
# Fri, 28 Jul 2023 04:00:14 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Fri, 28 Jul 2023 04:00:14 GMT
ENV ADMINER_VERSION=4.8.1
# Fri, 28 Jul 2023 04:00:14 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Fri, 28 Jul 2023 04:00:14 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Fri, 28 Jul 2023 04:00:28 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 28 Jul 2023 04:00:28 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Fri, 28 Jul 2023 04:00:28 GMT
ENTRYPOINT ["entrypoint.sh"]
# Fri, 28 Jul 2023 04:00:28 GMT
USER adminer
# Fri, 28 Jul 2023 04:00:28 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Fri, 28 Jul 2023 04:00:28 GMT
EXPOSE 8080
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
	-	`sha256:484885916a404a1914d24800750eeab9b2224eabfed1d1aa196e41cd3c4b7756`  
		Last Modified: Fri, 28 Jul 2023 04:00:59 GMT  
		Size: 1.9 KB (1871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13d91d5e54a9ab045713b54bf9f960158813d4f24cb9a3e1f566090e43445ac0`  
		Last Modified: Fri, 28 Jul 2023 04:00:59 GMT  
		Size: 1.5 KB (1479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80f6b00bd4ec73f6a31fa60dd3cc6d81a64999f4e8ed6a71306bb07c180b303a`  
		Last Modified: Fri, 28 Jul 2023 04:00:59 GMT  
		Size: 1.4 MB (1385391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39f9219ba03997189d3e28f84722b24d2d258b8c5e1b98719b345d64f9ac64c5`  
		Last Modified: Fri, 28 Jul 2023 04:00:59 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-standalone` - linux; arm64 variant v8

```console
$ docker pull adminer@sha256:958990f6d1f66e6a9f854251e04835456490db94d5049bd0781b82a4535b79b8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.3 MB (94337590 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae8ec1ac6b42873905c2e49fe8b847346b584a9934045a9af7c5ad3a2f4ce533`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Fri, 28 Jul 2023 01:32:58 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Fri, 28 Jul 2023 01:32:58 GMT
WORKDIR /var/www/html
# Fri, 28 Jul 2023 01:32:59 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Fri, 28 Jul 2023 01:32:59 GMT
ENV ADMINER_VERSION=4.8.1
# Fri, 28 Jul 2023 01:32:59 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Fri, 28 Jul 2023 01:32:59 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Fri, 28 Jul 2023 01:33:09 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 28 Jul 2023 01:33:09 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Fri, 28 Jul 2023 01:33:09 GMT
ENTRYPOINT ["entrypoint.sh"]
# Fri, 28 Jul 2023 01:33:09 GMT
USER adminer
# Fri, 28 Jul 2023 01:33:09 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Fri, 28 Jul 2023 01:33:09 GMT
EXPOSE 8080
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
	-	`sha256:805759b30cc65928f6590a87df6374385bc4ab00bac8e6c082067cad6a0c8052`  
		Last Modified: Fri, 28 Jul 2023 01:33:33 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45c52d243051d0380315d262f0c75865d8dbaff27d5d57b1fc3090fbb76dbf44`  
		Last Modified: Fri, 28 Jul 2023 01:33:34 GMT  
		Size: 1.5 KB (1482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:966b32c0aa3641a21349bda0ace8e58c088db3cbbba1a6f262ea97e74e2ecd25`  
		Last Modified: Fri, 28 Jul 2023 01:33:34 GMT  
		Size: 1.4 MB (1385329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba7e6078a351dedfa26b1cd20ceca3b8cca8fc8e6aa765670fa373020469f9ef`  
		Last Modified: Fri, 28 Jul 2023 01:33:33 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-standalone` - linux; 386

```console
$ docker pull adminer@sha256:bdc6e709372b466fb7e150220100c2bb03570db55b38e32d7fa561c6284a419a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.0 MB (96988943 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82259b8b78ccd8ccee229b64a8d7ecbace76dfa5a84a574ace582e34eb103d21`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Thu, 27 Jul 2023 23:39:07 GMT
ADD file:6ae90664cb71d88535d2be8e87b3a14dadaa5dad7756db4b7c26638d53c55187 in / 
# Thu, 27 Jul 2023 23:39:08 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 09:20:26 GMT
STOPSIGNAL SIGINT
# Fri, 28 Jul 2023 09:20:49 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 09:20:50 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Fri, 28 Jul 2023 09:20:51 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Fri, 28 Jul 2023 09:20:51 GMT
WORKDIR /var/www/html
# Fri, 28 Jul 2023 09:20:51 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Fri, 28 Jul 2023 09:20:51 GMT
ENV ADMINER_VERSION=4.8.1
# Fri, 28 Jul 2023 09:20:51 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Fri, 28 Jul 2023 09:20:51 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Fri, 28 Jul 2023 09:21:04 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 28 Jul 2023 09:21:04 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Fri, 28 Jul 2023 09:21:04 GMT
ENTRYPOINT ["entrypoint.sh"]
# Fri, 28 Jul 2023 09:21:04 GMT
USER adminer
# Fri, 28 Jul 2023 09:21:04 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Fri, 28 Jul 2023 09:21:05 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:8de74d843a460b113b2683caf2d7e61b9d0ed2575871f77b575c62d4244922f7`  
		Last Modified: Thu, 27 Jul 2023 23:43:47 GMT  
		Size: 56.0 MB (56040964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2073aeb744950969cfe199e623dd38bcd736842f5f550903a30e2874a8f2fac`  
		Last Modified: Fri, 28 Jul 2023 09:21:53 GMT  
		Size: 39.6 MB (39558454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d9df87b1ae652e19b89cd41938a3a4f3e0e4b22adf88f7e04358656e519ba25`  
		Last Modified: Fri, 28 Jul 2023 09:21:43 GMT  
		Size: 385.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d7b655147c1bb0f682f5f8f0eccc028e5b3556180ad4b544234a4a3874024d3`  
		Last Modified: Fri, 28 Jul 2023 09:21:43 GMT  
		Size: 1.9 KB (1870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b358863c32e35b6ea0038272e35db8947439187c44379b1338a649dd4c8ba0e`  
		Last Modified: Fri, 28 Jul 2023 09:21:43 GMT  
		Size: 1.5 KB (1478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f5affa5e069cedb2203a06f7e84bd25dba25ebd0995cdb97e17f72f3be07b10`  
		Last Modified: Fri, 28 Jul 2023 09:21:43 GMT  
		Size: 1.4 MB (1385301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61e80d19e81f60c7bd13b01a1f5651cbac19713775def23c1b173ff93c5b4e7f`  
		Last Modified: Fri, 28 Jul 2023 09:21:43 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-standalone` - linux; mips64le

```console
$ docker pull adminer@sha256:bba236958f3ef20f85f094ef599957a623ea712aa38c6b16090a9d32b6b72d44
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.6 MB (92614180 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4507a99e483cae111243d540a169beaba5b2399ae32abbc24552dcc14c06646f`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Tue, 04 Jul 2023 01:10:02 GMT
ADD file:f7ddd7406e3aa24165fc80933583fc2298f9792865511fe65def2f571fed2207 in / 
# Tue, 04 Jul 2023 01:10:07 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 14:27:09 GMT
STOPSIGNAL SIGINT
# Tue, 04 Jul 2023 14:29:01 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:29:07 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 04 Jul 2023 14:29:13 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 04 Jul 2023 14:29:17 GMT
WORKDIR /var/www/html
# Tue, 04 Jul 2023 14:29:20 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 04 Jul 2023 14:29:23 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 04 Jul 2023 14:29:26 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 04 Jul 2023 14:29:29 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 04 Jul 2023 14:30:22 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 04 Jul 2023 14:30:24 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 04 Jul 2023 14:30:28 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 04 Jul 2023 14:30:31 GMT
USER adminer
# Tue, 04 Jul 2023 14:30:34 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Tue, 04 Jul 2023 14:30:38 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:af98e96208d7ce4cff5417a3e8a38f98d2ed3abbca318e1e6c323aa8b8c56690`  
		Last Modified: Tue, 04 Jul 2023 01:20:40 GMT  
		Size: 53.3 MB (53270472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b6791bd7eb8dda07e9d1530ff7401ec314ff7c191e0c85f206cc8cd86be855c`  
		Last Modified: Tue, 04 Jul 2023 14:33:08 GMT  
		Size: 38.0 MB (37953331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3920a88961362bf993802523f7cca2e85caaa4a60f7f1e3d63aaf5eb0c09a4a7`  
		Last Modified: Tue, 04 Jul 2023 14:32:41 GMT  
		Size: 395.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:206c7da25ad9de44c8075b26de39239e884bba5e188ad5b3c7d9d9f126ba5039`  
		Last Modified: Tue, 04 Jul 2023 14:32:41 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ddc446ac238027e91c76b2ed3e55af67046cf1742ec9ff8f1189b45b3226a14`  
		Last Modified: Tue, 04 Jul 2023 14:32:41 GMT  
		Size: 1.5 KB (1481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2686c97d6e8dd8d071fca9724489d4b249e53a9b029354c8668871b3725e5305`  
		Last Modified: Tue, 04 Jul 2023 14:32:42 GMT  
		Size: 1.4 MB (1386278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3ce629354f0a6b55bc416d4b4fcbb5e8ce6a197cb5708a017936c011662d82c`  
		Last Modified: Tue, 04 Jul 2023 14:32:41 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-standalone` - linux; ppc64le

```console
$ docker pull adminer@sha256:df5bf8d059feda3cda5e0e8a3aa06ac30dac906581158df0fc12c2ae5363626c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.3 MB (101257630 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f397ecc16b1985b700b4da7acaf23f9b376a406f2fdc2ed50087172f02535d32`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Fri, 28 Jul 2023 03:35:30 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Fri, 28 Jul 2023 03:35:30 GMT
WORKDIR /var/www/html
# Fri, 28 Jul 2023 03:35:31 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Fri, 28 Jul 2023 03:35:32 GMT
ENV ADMINER_VERSION=4.8.1
# Fri, 28 Jul 2023 03:35:33 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Fri, 28 Jul 2023 03:35:34 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Fri, 28 Jul 2023 03:36:17 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 28 Jul 2023 03:36:17 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Fri, 28 Jul 2023 03:36:17 GMT
ENTRYPOINT ["entrypoint.sh"]
# Fri, 28 Jul 2023 03:36:18 GMT
USER adminer
# Fri, 28 Jul 2023 03:36:19 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Fri, 28 Jul 2023 03:36:19 GMT
EXPOSE 8080
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
	-	`sha256:270eca19cafbfc5e2b916d92704fa54dd5db26822d9fd116dcf5d42819ab43d7`  
		Last Modified: Fri, 28 Jul 2023 03:37:34 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5378ef8434defa831abb7d992342c4194e9d56727147428104bbe782e5f79640`  
		Last Modified: Fri, 28 Jul 2023 03:37:34 GMT  
		Size: 1.5 KB (1482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6abbf44f9489b4695d344d5e39263bc82565fa2bedcda25ca6be5e34f35d4dd8`  
		Last Modified: Fri, 28 Jul 2023 03:37:35 GMT  
		Size: 1.4 MB (1385679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10ed08794ca6d7389a2373df1731a9605d8f862eef22516a2e433b11d19a210c`  
		Last Modified: Fri, 28 Jul 2023 03:37:34 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-standalone` - linux; s390x

```console
$ docker pull adminer@sha256:faca9d7d2872d5b55b86b5075e69a84c556c930258a875e13aa3fa72ecf2b17c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.7 MB (93697370 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d5204631a997d1234d7546fcb38705962f54c2530fc951f2daf73a073ad0969`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Thu, 27 Jul 2023 23:47:23 GMT
ADD file:6e134e7958a9106ced0feb988945d71421340aa36ed7d8ad28fe5e91ab70df62 in / 
# Thu, 27 Jul 2023 23:47:27 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 01:53:47 GMT
STOPSIGNAL SIGINT
# Fri, 28 Jul 2023 01:54:06 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 01:54:08 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Fri, 28 Jul 2023 01:54:09 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Fri, 28 Jul 2023 01:54:09 GMT
WORKDIR /var/www/html
# Fri, 28 Jul 2023 01:54:09 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Fri, 28 Jul 2023 01:54:09 GMT
ENV ADMINER_VERSION=4.8.1
# Fri, 28 Jul 2023 01:54:09 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Fri, 28 Jul 2023 01:54:09 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Fri, 28 Jul 2023 01:54:17 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 28 Jul 2023 01:54:17 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Fri, 28 Jul 2023 01:54:17 GMT
ENTRYPOINT ["entrypoint.sh"]
# Fri, 28 Jul 2023 01:54:18 GMT
USER adminer
# Fri, 28 Jul 2023 01:54:18 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Fri, 28 Jul 2023 01:54:18 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:4909b03e906e0e2f8a83103a5b44c902afcad9d1bdcabcbc71058f3165c169e4`  
		Last Modified: Thu, 27 Jul 2023 23:52:31 GMT  
		Size: 53.3 MB (53289052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cc8014a61d0196a352e2e57cc9351c1fa171b6a57905fe5921e55c00c7f634a`  
		Last Modified: Fri, 28 Jul 2023 01:55:01 GMT  
		Size: 39.0 MB (39018628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b39aa6cfe13181ba6359c2b4fb46225c562e58e7cb27fb1591637c521f9d70d0`  
		Last Modified: Fri, 28 Jul 2023 01:54:54 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2df1820f29b009a397fd193ee10f17404280d3b9228f8b36daf5bb815bce0307`  
		Last Modified: Fri, 28 Jul 2023 01:54:54 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61a3cdb65e8cd3b2cb9e3aceddb9e95864743111dc589908c4805fca9f9bf9b8`  
		Last Modified: Fri, 28 Jul 2023 01:54:54 GMT  
		Size: 1.5 KB (1478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11aee720253a711b2d402e08cb5cafdfa0cc5290a8f09f543174ff677614c67f`  
		Last Modified: Fri, 28 Jul 2023 01:54:54 GMT  
		Size: 1.4 MB (1385448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:748f7c164596b5009b686a6803bc457fe549e5272341bfa787cc8f342ad43442`  
		Last Modified: Fri, 28 Jul 2023 01:54:54 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
