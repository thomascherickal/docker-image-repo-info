<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `adminer`

-	[`adminer:4`](#adminer4)
-	[`adminer:4-fastcgi`](#adminer4-fastcgi)
-	[`adminer:4-standalone`](#adminer4-standalone)
-	[`adminer:4.8.1`](#adminer481)
-	[`adminer:4.8.1-fastcgi`](#adminer481-fastcgi)
-	[`adminer:4.8.1-standalone`](#adminer481-standalone)
-	[`adminer:fastcgi`](#adminerfastcgi)
-	[`adminer:latest`](#adminerlatest)
-	[`adminer:standalone`](#adminerstandalone)

## `adminer:4`

```console
$ docker pull adminer@sha256:40c1d6691703a8ca102dc108c4a6fc11863e928b6ae6014fb8557b6e083a29ff
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

### `adminer:4` - linux; amd64

```console
$ docker pull adminer@sha256:7fb4cb76b1a979671c18bba6ad81fc80d50cb56069b7fb542f75efb921b5e714
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.9 MB (95937427 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b672f480fc7a76f4b04207143a6b693b2a6eec24ac981709e626b16505609fd`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Wed, 20 Sep 2023 07:12:40 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 20 Sep 2023 07:12:40 GMT
WORKDIR /var/www/html
# Wed, 20 Sep 2023 07:12:41 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 20 Sep 2023 07:12:41 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 20 Sep 2023 07:12:41 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 20 Sep 2023 07:12:41 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 20 Sep 2023 07:12:53 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 20 Sep 2023 07:12:53 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 20 Sep 2023 07:12:53 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 20 Sep 2023 07:12:53 GMT
USER adminer
# Wed, 20 Sep 2023 07:12:53 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 20 Sep 2023 07:12:53 GMT
EXPOSE 8080
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
	-	`sha256:eb4bd38d1031bd7c467d8bce4c95f0b7697c26030cc73874381860ce97d0cdcd`  
		Last Modified: Wed, 20 Sep 2023 07:13:25 GMT  
		Size: 1.9 KB (1880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3bc33b7b683bc4196fbd1738ad588e8334ddb171c5d50c48429546f10cb487a`  
		Last Modified: Wed, 20 Sep 2023 07:13:25 GMT  
		Size: 1.5 KB (1477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d61d710f98a6cd583cbb61f1ace245ab27b2b69e7e606afdff85fe75a17f685`  
		Last Modified: Wed, 20 Sep 2023 07:13:26 GMT  
		Size: 1.4 MB (1385429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8441003ca946127323e284e8685841d9e549a658468e76be7cf68a2b08203f3`  
		Last Modified: Wed, 20 Sep 2023 07:13:25 GMT  
		Size: 488.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4` - linux; arm variant v5

```console
$ docker pull adminer@sha256:fc1ddb9f0a1b7781c7281f79851e7141b11e10f5cc915355b6cf6ff7824ede94
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.2 MB (91195621 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f410041bfb5c56158771bc68b88310247a497e74186a3dfdb22358729c1fd47e`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Wed, 20 Sep 2023 09:37:05 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 20 Sep 2023 09:37:05 GMT
WORKDIR /var/www/html
# Wed, 20 Sep 2023 09:37:05 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 20 Sep 2023 09:37:05 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 20 Sep 2023 09:37:05 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 20 Sep 2023 09:37:05 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 20 Sep 2023 09:37:21 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 20 Sep 2023 09:37:21 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 20 Sep 2023 09:37:21 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 20 Sep 2023 09:37:21 GMT
USER adminer
# Wed, 20 Sep 2023 09:37:21 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 20 Sep 2023 09:37:21 GMT
EXPOSE 8080
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
	-	`sha256:1cba35ed39d8d7c05cb37696f20ecdc7fde0f2d7fcbe968f50892aaabfdd84f2`  
		Last Modified: Wed, 20 Sep 2023 09:37:57 GMT  
		Size: 1.9 KB (1871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df6f0945f3469cf4fdd867a2409be0fc2b79d33a4267fb743edb64842be147f3`  
		Last Modified: Wed, 20 Sep 2023 09:37:57 GMT  
		Size: 1.5 KB (1476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb77accf421b5a1954871ae06a2ed8550b59f6ea59dfc1773263a25757e67757`  
		Last Modified: Wed, 20 Sep 2023 09:37:58 GMT  
		Size: 1.4 MB (1385374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1004d2eab86228b351246a3406fff91074ab91bf1c83691d49831a343972504f`  
		Last Modified: Wed, 20 Sep 2023 09:37:57 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4` - linux; arm variant v7

```console
$ docker pull adminer@sha256:d8a19218a54fe4fb52cb32cfc4d0ba0207b2976a94106cc4587ae23ef2796f6a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.8 MB (87795777 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2953870e043e0f3e517f17cce5c6d2e2d06f74d372de15043ba3193f11862b48`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 20 Sep 2023 04:57:26 GMT
ADD file:3bf3380482840b3a4166e82c3f951812076851ba1527261fdd1da780662b2de1 in / 
# Wed, 20 Sep 2023 04:57:26 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 15:43:10 GMT
STOPSIGNAL SIGINT
# Wed, 20 Sep 2023 15:43:35 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 15:43:36 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 20 Sep 2023 15:43:37 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 20 Sep 2023 15:43:37 GMT
WORKDIR /var/www/html
# Wed, 20 Sep 2023 15:43:37 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 20 Sep 2023 15:43:37 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 20 Sep 2023 15:43:37 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 20 Sep 2023 15:43:37 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 20 Sep 2023 15:43:50 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 20 Sep 2023 15:43:50 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 20 Sep 2023 15:43:50 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 20 Sep 2023 15:43:50 GMT
USER adminer
# Wed, 20 Sep 2023 15:43:50 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 20 Sep 2023 15:43:50 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:1d4e041d2204b383d6d6893cfcf5b852394f34744a85cea9ec0b3fb65cbc6143`  
		Last Modified: Wed, 20 Sep 2023 05:01:34 GMT  
		Size: 50.2 MB (50219551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4ca4acdacd0b759547187250427f6845ca2fc092c757b2e2f6667b1add9ba8d`  
		Last Modified: Wed, 20 Sep 2023 15:44:32 GMT  
		Size: 36.2 MB (36186615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc8798178b90f7264865be9cbfe742803f21777526c5ba6c86e1526c78998f64`  
		Last Modified: Wed, 20 Sep 2023 15:44:23 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e44ef76b17f1c1b9f8fa8b3c28b236740ee52ee91c0bf1a5967949aa44b1d46`  
		Last Modified: Wed, 20 Sep 2023 15:44:23 GMT  
		Size: 1.9 KB (1871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02874a9e593b60862b1fa6079ec21abf9b108ff79ed1afb0fea2f5fb92c31bc0`  
		Last Modified: Wed, 20 Sep 2023 15:44:23 GMT  
		Size: 1.5 KB (1478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92715c2cab25dd578e4272162c7e32c5e783506711541b3e2cd6a0dd12e62fcf`  
		Last Modified: Wed, 20 Sep 2023 15:44:23 GMT  
		Size: 1.4 MB (1385383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6187ee8021740cf1e9d2e67c8904adc77f0ed4503d7f9ada0dec4b5537eaa35f`  
		Last Modified: Wed, 20 Sep 2023 15:44:23 GMT  
		Size: 489.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4` - linux; arm64 variant v8

```console
$ docker pull adminer@sha256:82f1435981ebaa969cfd9cb3f452c46655dcf1715947a90a8c64dd3284db36d3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.3 MB (94338726 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51817ad17de2ccc468c81b03aa1f7c122e2d802f5411b384d4b8d341c711b3ff`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 20 Sep 2023 02:44:20 GMT
ADD file:46dcdcde338d2c01fed5db3fac9041736d9305145d8fc2039dd5b3714d38ede8 in / 
# Wed, 20 Sep 2023 02:44:21 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 18:04:43 GMT
STOPSIGNAL SIGINT
# Wed, 20 Sep 2023 18:05:03 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 18:05:04 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 20 Sep 2023 18:05:05 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 20 Sep 2023 18:05:05 GMT
WORKDIR /var/www/html
# Wed, 20 Sep 2023 18:05:05 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 20 Sep 2023 18:05:05 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 20 Sep 2023 18:05:05 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 20 Sep 2023 18:05:05 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 20 Sep 2023 18:05:16 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 20 Sep 2023 18:05:16 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 20 Sep 2023 18:05:16 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 20 Sep 2023 18:05:16 GMT
USER adminer
# Wed, 20 Sep 2023 18:05:16 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 20 Sep 2023 18:05:16 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:31f5dc1f52c865588c43d8ec718f14d430e149b28f0b28232da825da7ae28f76`  
		Last Modified: Wed, 20 Sep 2023 02:47:53 GMT  
		Size: 53.7 MB (53704892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c82c17c7529e7d3125d9a7f12b8359fac7e9cc29dbb6555d30cbe9bdda203722`  
		Last Modified: Wed, 20 Sep 2023 18:05:50 GMT  
		Size: 39.2 MB (39244274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27290e9432136a39923f648bd1220a36cdd54a4f8baacd87b500eed4d5018d2a`  
		Last Modified: Wed, 20 Sep 2023 18:05:44 GMT  
		Size: 393.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0029f07058cb36f9b27d218954d9e733b152fe47d9875b8d062632100f585d58`  
		Last Modified: Wed, 20 Sep 2023 18:05:44 GMT  
		Size: 1.9 KB (1883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f9ca9fda73283aac009ee0add3e063260cc5c09a89cbdaddef5d3e623c8ae3f`  
		Last Modified: Wed, 20 Sep 2023 18:05:44 GMT  
		Size: 1.5 KB (1477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99dc3e204c8096f4463277e628be5a5860db3a123dd45a87f99df2b8d1d76f77`  
		Last Modified: Wed, 20 Sep 2023 18:05:44 GMT  
		Size: 1.4 MB (1385317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5dbe53bc88443a7def3aa5bed48f19d4bc849da97d88790bf9701396443acac`  
		Last Modified: Wed, 20 Sep 2023 18:05:44 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4` - linux; 386

```console
$ docker pull adminer@sha256:24a953b70c62fedfe7da2846b84d0a3133b442f0721e17fbf5df2d222ae440f8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.0 MB (96989218 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0cbe365ed04581b1b00d6390c52f9260afab49677042b95a947b6ca499d98bdc`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 20 Sep 2023 00:42:07 GMT
ADD file:342c36522089238a534c0912491a4cf64b89133969e051cdad2e694ec761142c in / 
# Wed, 20 Sep 2023 00:42:07 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 15:10:00 GMT
STOPSIGNAL SIGINT
# Wed, 20 Sep 2023 15:10:29 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 15:10:30 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 20 Sep 2023 15:10:31 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 20 Sep 2023 15:10:31 GMT
WORKDIR /var/www/html
# Wed, 20 Sep 2023 15:10:31 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 20 Sep 2023 15:10:31 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 20 Sep 2023 15:10:31 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 20 Sep 2023 15:10:31 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 20 Sep 2023 15:10:47 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 20 Sep 2023 15:10:47 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 20 Sep 2023 15:10:47 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 20 Sep 2023 15:10:47 GMT
USER adminer
# Wed, 20 Sep 2023 15:10:47 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 20 Sep 2023 15:10:47 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:00121bf241b18e981bcc804f905be7b34f95cce415db622599e21dc1a496ee8d`  
		Last Modified: Wed, 20 Sep 2023 00:47:11 GMT  
		Size: 56.0 MB (56040498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:964fa70975aa8c3eb5838cf9120935712a93ec197f9adce227a0d97a7df9d131`  
		Last Modified: Wed, 20 Sep 2023 15:11:38 GMT  
		Size: 39.6 MB (39559141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cf7eb9be8cf86ff0edfb0e7026187487f60c1b234c068e76b9d90c4bb2e56b5`  
		Last Modified: Wed, 20 Sep 2023 15:11:27 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7986b40b588b21caefc32e63e9bf4259713bd637125de9f9e6c415339b62bdb8`  
		Last Modified: Wed, 20 Sep 2023 15:11:27 GMT  
		Size: 1.9 KB (1869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da42b96b0425edc1796b564789c33a81ba8cc1bd8e95886fb24cba7bf6e830f9`  
		Last Modified: Wed, 20 Sep 2023 15:11:27 GMT  
		Size: 1.5 KB (1481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cb8907e77be88986e418354768b790c2a227d56ea26b7a7cdb7027c2958aa71`  
		Last Modified: Wed, 20 Sep 2023 15:11:27 GMT  
		Size: 1.4 MB (1385349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9fdcba82893748b7e9f6211dc3cd3248fa29ee6f78a24482d34339bb1fd857f`  
		Last Modified: Wed, 20 Sep 2023 15:11:27 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4` - linux; mips64le

```console
$ docker pull adminer@sha256:ec803d54e73e17da91a36b9ce59b261f4f312dacabb7e0556302bce0443f75b7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.6 MB (92612531 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:215cf7d1502bb244df43b52290a34650eafce425c56c967b8c9e153a5ada9557`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Wed, 20 Sep 2023 06:40:19 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 20 Sep 2023 06:40:22 GMT
WORKDIR /var/www/html
# Wed, 20 Sep 2023 06:40:25 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 20 Sep 2023 06:40:28 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 20 Sep 2023 06:40:32 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 20 Sep 2023 06:40:35 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 20 Sep 2023 06:41:26 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 20 Sep 2023 06:41:29 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 20 Sep 2023 06:41:32 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 20 Sep 2023 06:41:35 GMT
USER adminer
# Wed, 20 Sep 2023 06:41:39 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 20 Sep 2023 06:41:42 GMT
EXPOSE 8080
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
	-	`sha256:4f0fa2061f2328806a3e6442dc58a5750d76966e9542efd972a12fd49f53cd69`  
		Last Modified: Wed, 20 Sep 2023 06:43:50 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04163c23cec6352cfd6ce393d04f5900400ea72c83d04af1552865c916a1c459`  
		Last Modified: Wed, 20 Sep 2023 06:43:50 GMT  
		Size: 1.5 KB (1481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d726d9d0dfbf6bba7fc6b01578c0a26c84fafdbe71a4e69674dfd1284ce0826`  
		Last Modified: Wed, 20 Sep 2023 06:43:51 GMT  
		Size: 1.4 MB (1386315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e96e2db0e4c5751ce57381cb92f2f2fff089adb321644959f5de599a271ebedc`  
		Last Modified: Wed, 20 Sep 2023 06:43:50 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4` - linux; ppc64le

```console
$ docker pull adminer@sha256:e0809520a8bd4f91b86c0bfd4a871ce4707fd119706f564057dffe5e7c91f5fe
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.3 MB (101262041 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ad347a3c52aeda1176962cc50fcedfab4a87a129219de1394700476d688d49e`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 20 Sep 2023 07:53:09 GMT
ADD file:c12b11abfba27478510c84d05abdd8fec539db9ec30af6d042671f4d5bf793e5 in / 
# Wed, 20 Sep 2023 07:53:12 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 10:27:30 GMT
STOPSIGNAL SIGINT
# Wed, 20 Sep 2023 10:28:24 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 10:28:27 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 20 Sep 2023 10:28:28 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 20 Sep 2023 10:28:28 GMT
WORKDIR /var/www/html
# Wed, 20 Sep 2023 10:28:29 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 20 Sep 2023 10:28:29 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 20 Sep 2023 10:28:30 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 20 Sep 2023 10:28:30 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 20 Sep 2023 10:28:54 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 20 Sep 2023 10:28:54 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 20 Sep 2023 10:28:55 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 20 Sep 2023 10:28:55 GMT
USER adminer
# Wed, 20 Sep 2023 10:28:55 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 20 Sep 2023 10:28:55 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:9f3507d882ae95f06b3672497cdd3317bd4f8e0255e73d10f1f263e5d780f102`  
		Last Modified: Wed, 20 Sep 2023 08:50:16 GMT  
		Size: 58.9 MB (58928499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dc55ae4eee76ca2700dbf8d4554951df837121cc96140f29cbcc2d7308b4d72`  
		Last Modified: Wed, 20 Sep 2023 10:29:59 GMT  
		Size: 40.9 MB (40943739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:413bf430ecd0a8d3a68dc7841be8802fccca3af99645087fbb82e476cd335965`  
		Last Modified: Wed, 20 Sep 2023 10:29:47 GMT  
		Size: 396.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df2720d6c627570256eb0bc8943ba052f2b617c5dd972a3eb74196fc91a3dbbb`  
		Last Modified: Wed, 20 Sep 2023 10:29:47 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b6b255e136e7ac31afc340c04be397be6d98a39da922310d73ffbfff9687a2a`  
		Last Modified: Wed, 20 Sep 2023 10:29:47 GMT  
		Size: 1.5 KB (1481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36bfcc7e4826d80f455356e3a88eb31b2e5c559a49a733a25490d6becb652045`  
		Last Modified: Wed, 20 Sep 2023 10:29:47 GMT  
		Size: 1.4 MB (1385554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36a5f297e715a97e0af1984e9f7dd3cb60fa2226b31fc95bbfb6a3c5d85549af`  
		Last Modified: Wed, 20 Sep 2023 10:29:47 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4` - linux; s390x

```console
$ docker pull adminer@sha256:120087fff0a708c70334e38726cab4a7703516787b7d901b1adc69fde470d694
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.7 MB (93701227 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42031d8d4365bb267d464fac6d7ab8b6e0ad4b097eb47e3e4b2dd8d14b64371d`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Wed, 20 Sep 2023 09:42:33 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 20 Sep 2023 09:42:33 GMT
WORKDIR /var/www/html
# Wed, 20 Sep 2023 09:42:33 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 20 Sep 2023 09:42:34 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 20 Sep 2023 09:42:34 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 20 Sep 2023 09:42:34 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 20 Sep 2023 09:42:57 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 20 Sep 2023 09:42:58 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 20 Sep 2023 09:42:58 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 20 Sep 2023 09:42:59 GMT
USER adminer
# Wed, 20 Sep 2023 09:42:59 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 20 Sep 2023 09:43:00 GMT
EXPOSE 8080
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
	-	`sha256:a0dfeb4132e2fe11e348c94294b33e51684a77419be87fae2d715412dc40e9c1`  
		Last Modified: Wed, 20 Sep 2023 09:43:57 GMT  
		Size: 1.9 KB (1883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:800a5df8795fcb07b6a7efb2135a2a662b31533cd779cc532445e86eae286b9f`  
		Last Modified: Wed, 20 Sep 2023 09:43:57 GMT  
		Size: 1.5 KB (1481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:321185c09a4e5d7e9a145855613f743ef531836df1355ae7593208920ad68541`  
		Last Modified: Wed, 20 Sep 2023 09:43:58 GMT  
		Size: 1.4 MB (1385674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c30b98bdcd0d0b081524334dc05d7905ceb45b6e8230e8156267e4759d587a2c`  
		Last Modified: Wed, 20 Sep 2023 09:43:57 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `adminer:4-fastcgi`

```console
$ docker pull adminer@sha256:b1eb6b4fef1cbe8aae2448f5ff246547904ddde8353382e40fd999fa7cd90047
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
$ docker pull adminer@sha256:542098b1184f641c16a22b9b0d3a814b99a7bffca9593133e604d06e76cfb2f8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.8 MB (87798559 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7fe9e2628383acfd8d7c700d2a4881cfe1815fbee052c129294f79bce56e1b5`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Wed, 20 Sep 2023 04:57:26 GMT
ADD file:3bf3380482840b3a4166e82c3f951812076851ba1527261fdd1da780662b2de1 in / 
# Wed, 20 Sep 2023 04:57:26 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 15:43:10 GMT
STOPSIGNAL SIGINT
# Wed, 20 Sep 2023 15:43:35 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 15:43:36 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 20 Sep 2023 15:43:59 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Wed, 20 Sep 2023 15:44:00 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 20 Sep 2023 15:44:00 GMT
WORKDIR /var/www/html
# Wed, 20 Sep 2023 15:44:00 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 20 Sep 2023 15:44:00 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 20 Sep 2023 15:44:00 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 20 Sep 2023 15:44:00 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 20 Sep 2023 15:44:11 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 20 Sep 2023 15:44:11 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 20 Sep 2023 15:44:12 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 20 Sep 2023 15:44:12 GMT
USER adminer
# Wed, 20 Sep 2023 15:44:12 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:1d4e041d2204b383d6d6893cfcf5b852394f34744a85cea9ec0b3fb65cbc6143`  
		Last Modified: Wed, 20 Sep 2023 05:01:34 GMT  
		Size: 50.2 MB (50219551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4ca4acdacd0b759547187250427f6845ca2fc092c757b2e2f6667b1add9ba8d`  
		Last Modified: Wed, 20 Sep 2023 15:44:32 GMT  
		Size: 36.2 MB (36186615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc8798178b90f7264865be9cbfe742803f21777526c5ba6c86e1526c78998f64`  
		Last Modified: Wed, 20 Sep 2023 15:44:23 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3364c0b2504d3af9b0175a6e77522d257e70f24251cfd629dd6bd3ef24b5f119`  
		Last Modified: Wed, 20 Sep 2023 15:44:49 GMT  
		Size: 2.7 KB (2713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62a19c34bb68631c5d5858d4245052d13f760c8cf841e4a4cd1f02343aed2d5f`  
		Last Modified: Wed, 20 Sep 2023 15:44:49 GMT  
		Size: 1.9 KB (1869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08676442b17b4a0cc0ffff5e52fe487a0107e28a668edfdff6ad54606481fb05`  
		Last Modified: Wed, 20 Sep 2023 15:44:49 GMT  
		Size: 1.5 KB (1480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82515cdefa5e1215ed49066547b07fa57d1b9da8fabd0522836ba51ad7e9ab82`  
		Last Modified: Wed, 20 Sep 2023 15:44:49 GMT  
		Size: 1.4 MB (1385449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cf0ebb373156a781676a77242c49b21185c9e025e5104d6b83fec00a1a77b78`  
		Last Modified: Wed, 20 Sep 2023 15:44:49 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-fastcgi` - linux; arm64 variant v8

```console
$ docker pull adminer@sha256:1cff0be1992c13ea25123e8139fc1179c0f722357c1f54f6be3a143db8a52899
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.3 MB (94341405 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ce755452b4733c8b45e4d8e12c142771d8fd25391360bfaff9353b77d3a7296`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Wed, 20 Sep 2023 02:44:20 GMT
ADD file:46dcdcde338d2c01fed5db3fac9041736d9305145d8fc2039dd5b3714d38ede8 in / 
# Wed, 20 Sep 2023 02:44:21 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 18:04:43 GMT
STOPSIGNAL SIGINT
# Wed, 20 Sep 2023 18:05:03 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 18:05:04 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 20 Sep 2023 18:05:23 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Wed, 20 Sep 2023 18:05:23 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 20 Sep 2023 18:05:23 GMT
WORKDIR /var/www/html
# Wed, 20 Sep 2023 18:05:24 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 20 Sep 2023 18:05:24 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 20 Sep 2023 18:05:24 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 20 Sep 2023 18:05:24 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 20 Sep 2023 18:05:34 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 20 Sep 2023 18:05:34 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 20 Sep 2023 18:05:34 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 20 Sep 2023 18:05:35 GMT
USER adminer
# Wed, 20 Sep 2023 18:05:35 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:31f5dc1f52c865588c43d8ec718f14d430e149b28f0b28232da825da7ae28f76`  
		Last Modified: Wed, 20 Sep 2023 02:47:53 GMT  
		Size: 53.7 MB (53704892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c82c17c7529e7d3125d9a7f12b8359fac7e9cc29dbb6555d30cbe9bdda203722`  
		Last Modified: Wed, 20 Sep 2023 18:05:50 GMT  
		Size: 39.2 MB (39244274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27290e9432136a39923f648bd1220a36cdd54a4f8baacd87b500eed4d5018d2a`  
		Last Modified: Wed, 20 Sep 2023 18:05:44 GMT  
		Size: 393.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4d0cfb12b1cdc502f0839f004aa983a25ea38bb788e0b734aa01a54303ae0e2`  
		Last Modified: Wed, 20 Sep 2023 18:06:08 GMT  
		Size: 2.7 KB (2711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76b68d0109bf502fae5cb6a017bbb0e37d31131dc631b3ae9ce75b6603690194`  
		Last Modified: Wed, 20 Sep 2023 18:06:08 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4abe36926b3c359fc35e36926f70d35534faf595ccb23765fd12a141f764e821`  
		Last Modified: Wed, 20 Sep 2023 18:06:08 GMT  
		Size: 1.5 KB (1478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42b5d424d36cd52afb1439ff8165fbc761f2319ec3e4e891eadb0f03a089199b`  
		Last Modified: Wed, 20 Sep 2023 18:06:08 GMT  
		Size: 1.4 MB (1385285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a545cd65be7574c61d9c4d38924911eeffdabb28d5d74e8198afda6043e8579`  
		Last Modified: Wed, 20 Sep 2023 18:06:08 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-fastcgi` - linux; 386

```console
$ docker pull adminer@sha256:846388f4f74cf512bb64bf84c6b64a14c87e97c2082957de704afb301f49a8f3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.0 MB (96991935 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d51e9267cebf41d916c5538d54fa90a930c77844a72ea2d84572bf9b9c7feba`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Wed, 20 Sep 2023 00:42:07 GMT
ADD file:342c36522089238a534c0912491a4cf64b89133969e051cdad2e694ec761142c in / 
# Wed, 20 Sep 2023 00:42:07 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 15:10:00 GMT
STOPSIGNAL SIGINT
# Wed, 20 Sep 2023 15:10:29 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 15:10:30 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 20 Sep 2023 15:10:58 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Wed, 20 Sep 2023 15:10:59 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 20 Sep 2023 15:10:59 GMT
WORKDIR /var/www/html
# Wed, 20 Sep 2023 15:10:59 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 20 Sep 2023 15:10:59 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 20 Sep 2023 15:10:59 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 20 Sep 2023 15:10:59 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 20 Sep 2023 15:11:15 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 20 Sep 2023 15:11:15 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 20 Sep 2023 15:11:15 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 20 Sep 2023 15:11:15 GMT
USER adminer
# Wed, 20 Sep 2023 15:11:15 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:00121bf241b18e981bcc804f905be7b34f95cce415db622599e21dc1a496ee8d`  
		Last Modified: Wed, 20 Sep 2023 00:47:11 GMT  
		Size: 56.0 MB (56040498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:964fa70975aa8c3eb5838cf9120935712a93ec197f9adce227a0d97a7df9d131`  
		Last Modified: Wed, 20 Sep 2023 15:11:38 GMT  
		Size: 39.6 MB (39559141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cf7eb9be8cf86ff0edfb0e7026187487f60c1b234c068e76b9d90c4bb2e56b5`  
		Last Modified: Wed, 20 Sep 2023 15:11:27 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14739144aeefcf6bb5b82efb1be6c8c36061cb79988c3d04e94ac3af2889703d`  
		Last Modified: Wed, 20 Sep 2023 15:11:57 GMT  
		Size: 2.7 KB (2707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be431c45e4957603c8fc57e2e1c75ca225cf90bdaee782e22140bd61fb848bd2`  
		Last Modified: Wed, 20 Sep 2023 15:11:58 GMT  
		Size: 1.9 KB (1870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af4bb02c3c060fffe6e6033ae734961cbe056f312fe14b88a19af87c4f244f12`  
		Last Modified: Wed, 20 Sep 2023 15:11:57 GMT  
		Size: 1.5 KB (1472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ed951e5e4331a40e2299fe20b587b7ac277d2561486420e3f603a26eaf55c7f`  
		Last Modified: Wed, 20 Sep 2023 15:11:57 GMT  
		Size: 1.4 MB (1385367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e84da2513a7218dd7201673bcd22e26b222c95847fcf06c9b8a7151d89c1b1f0`  
		Last Modified: Wed, 20 Sep 2023 15:11:56 GMT  
		Size: 490.0 B  
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
$ docker pull adminer@sha256:79299ee4e64a10ed155d4b0e07c0b513251f6730c593768c6e3ed11269d0b296
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.3 MB (101264733 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc0562129b0dc47471215a72b69dc9de21102422b16b11725a10b19d56f6b30c`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Wed, 20 Sep 2023 07:53:09 GMT
ADD file:c12b11abfba27478510c84d05abdd8fec539db9ec30af6d042671f4d5bf793e5 in / 
# Wed, 20 Sep 2023 07:53:12 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 10:27:30 GMT
STOPSIGNAL SIGINT
# Wed, 20 Sep 2023 10:28:24 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 10:28:27 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 20 Sep 2023 10:29:10 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Wed, 20 Sep 2023 10:29:11 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 20 Sep 2023 10:29:11 GMT
WORKDIR /var/www/html
# Wed, 20 Sep 2023 10:29:11 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 20 Sep 2023 10:29:12 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 20 Sep 2023 10:29:12 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 20 Sep 2023 10:29:12 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 20 Sep 2023 10:29:34 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 20 Sep 2023 10:29:34 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 20 Sep 2023 10:29:34 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 20 Sep 2023 10:29:35 GMT
USER adminer
# Wed, 20 Sep 2023 10:29:35 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:9f3507d882ae95f06b3672497cdd3317bd4f8e0255e73d10f1f263e5d780f102`  
		Last Modified: Wed, 20 Sep 2023 08:50:16 GMT  
		Size: 58.9 MB (58928499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dc55ae4eee76ca2700dbf8d4554951df837121cc96140f29cbcc2d7308b4d72`  
		Last Modified: Wed, 20 Sep 2023 10:29:59 GMT  
		Size: 40.9 MB (40943739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:413bf430ecd0a8d3a68dc7841be8802fccca3af99645087fbb82e476cd335965`  
		Last Modified: Wed, 20 Sep 2023 10:29:47 GMT  
		Size: 396.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33c90f4bc93f05165b4c2a576055f2d0614e44beb75f656246a36dab518a167e`  
		Last Modified: Wed, 20 Sep 2023 10:30:20 GMT  
		Size: 2.7 KB (2712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8042ccb66d3f41a43740fe4d53cf23c908f55c921ebbdd7f85a713640e21b71`  
		Last Modified: Wed, 20 Sep 2023 10:30:20 GMT  
		Size: 1.9 KB (1877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9687767d889f697b2273a34c6066aa7a3319201ef0abe10a52e58cd6192f18e0`  
		Last Modified: Wed, 20 Sep 2023 10:30:20 GMT  
		Size: 1.5 KB (1480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:373f9256ef78f4c4f1ce5dcac32e6c33dc0c75c189e9d0fe44e89efc9ad1e68e`  
		Last Modified: Wed, 20 Sep 2023 10:30:21 GMT  
		Size: 1.4 MB (1385537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f063a3c5af7dc109b9e33bbf3c86fea2b892e631c1128300364996aa081e72d`  
		Last Modified: Wed, 20 Sep 2023 10:30:20 GMT  
		Size: 493.0 B  
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

## `adminer:4-standalone`

```console
$ docker pull adminer@sha256:40c1d6691703a8ca102dc108c4a6fc11863e928b6ae6014fb8557b6e083a29ff
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
$ docker pull adminer@sha256:7fb4cb76b1a979671c18bba6ad81fc80d50cb56069b7fb542f75efb921b5e714
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.9 MB (95937427 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b672f480fc7a76f4b04207143a6b693b2a6eec24ac981709e626b16505609fd`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Wed, 20 Sep 2023 07:12:40 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 20 Sep 2023 07:12:40 GMT
WORKDIR /var/www/html
# Wed, 20 Sep 2023 07:12:41 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 20 Sep 2023 07:12:41 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 20 Sep 2023 07:12:41 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 20 Sep 2023 07:12:41 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 20 Sep 2023 07:12:53 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 20 Sep 2023 07:12:53 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 20 Sep 2023 07:12:53 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 20 Sep 2023 07:12:53 GMT
USER adminer
# Wed, 20 Sep 2023 07:12:53 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 20 Sep 2023 07:12:53 GMT
EXPOSE 8080
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
	-	`sha256:eb4bd38d1031bd7c467d8bce4c95f0b7697c26030cc73874381860ce97d0cdcd`  
		Last Modified: Wed, 20 Sep 2023 07:13:25 GMT  
		Size: 1.9 KB (1880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3bc33b7b683bc4196fbd1738ad588e8334ddb171c5d50c48429546f10cb487a`  
		Last Modified: Wed, 20 Sep 2023 07:13:25 GMT  
		Size: 1.5 KB (1477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d61d710f98a6cd583cbb61f1ace245ab27b2b69e7e606afdff85fe75a17f685`  
		Last Modified: Wed, 20 Sep 2023 07:13:26 GMT  
		Size: 1.4 MB (1385429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8441003ca946127323e284e8685841d9e549a658468e76be7cf68a2b08203f3`  
		Last Modified: Wed, 20 Sep 2023 07:13:25 GMT  
		Size: 488.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-standalone` - linux; arm variant v5

```console
$ docker pull adminer@sha256:fc1ddb9f0a1b7781c7281f79851e7141b11e10f5cc915355b6cf6ff7824ede94
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.2 MB (91195621 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f410041bfb5c56158771bc68b88310247a497e74186a3dfdb22358729c1fd47e`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Wed, 20 Sep 2023 09:37:05 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 20 Sep 2023 09:37:05 GMT
WORKDIR /var/www/html
# Wed, 20 Sep 2023 09:37:05 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 20 Sep 2023 09:37:05 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 20 Sep 2023 09:37:05 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 20 Sep 2023 09:37:05 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 20 Sep 2023 09:37:21 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 20 Sep 2023 09:37:21 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 20 Sep 2023 09:37:21 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 20 Sep 2023 09:37:21 GMT
USER adminer
# Wed, 20 Sep 2023 09:37:21 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 20 Sep 2023 09:37:21 GMT
EXPOSE 8080
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
	-	`sha256:1cba35ed39d8d7c05cb37696f20ecdc7fde0f2d7fcbe968f50892aaabfdd84f2`  
		Last Modified: Wed, 20 Sep 2023 09:37:57 GMT  
		Size: 1.9 KB (1871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df6f0945f3469cf4fdd867a2409be0fc2b79d33a4267fb743edb64842be147f3`  
		Last Modified: Wed, 20 Sep 2023 09:37:57 GMT  
		Size: 1.5 KB (1476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb77accf421b5a1954871ae06a2ed8550b59f6ea59dfc1773263a25757e67757`  
		Last Modified: Wed, 20 Sep 2023 09:37:58 GMT  
		Size: 1.4 MB (1385374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1004d2eab86228b351246a3406fff91074ab91bf1c83691d49831a343972504f`  
		Last Modified: Wed, 20 Sep 2023 09:37:57 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-standalone` - linux; arm variant v7

```console
$ docker pull adminer@sha256:d8a19218a54fe4fb52cb32cfc4d0ba0207b2976a94106cc4587ae23ef2796f6a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.8 MB (87795777 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2953870e043e0f3e517f17cce5c6d2e2d06f74d372de15043ba3193f11862b48`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 20 Sep 2023 04:57:26 GMT
ADD file:3bf3380482840b3a4166e82c3f951812076851ba1527261fdd1da780662b2de1 in / 
# Wed, 20 Sep 2023 04:57:26 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 15:43:10 GMT
STOPSIGNAL SIGINT
# Wed, 20 Sep 2023 15:43:35 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 15:43:36 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 20 Sep 2023 15:43:37 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 20 Sep 2023 15:43:37 GMT
WORKDIR /var/www/html
# Wed, 20 Sep 2023 15:43:37 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 20 Sep 2023 15:43:37 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 20 Sep 2023 15:43:37 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 20 Sep 2023 15:43:37 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 20 Sep 2023 15:43:50 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 20 Sep 2023 15:43:50 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 20 Sep 2023 15:43:50 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 20 Sep 2023 15:43:50 GMT
USER adminer
# Wed, 20 Sep 2023 15:43:50 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 20 Sep 2023 15:43:50 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:1d4e041d2204b383d6d6893cfcf5b852394f34744a85cea9ec0b3fb65cbc6143`  
		Last Modified: Wed, 20 Sep 2023 05:01:34 GMT  
		Size: 50.2 MB (50219551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4ca4acdacd0b759547187250427f6845ca2fc092c757b2e2f6667b1add9ba8d`  
		Last Modified: Wed, 20 Sep 2023 15:44:32 GMT  
		Size: 36.2 MB (36186615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc8798178b90f7264865be9cbfe742803f21777526c5ba6c86e1526c78998f64`  
		Last Modified: Wed, 20 Sep 2023 15:44:23 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e44ef76b17f1c1b9f8fa8b3c28b236740ee52ee91c0bf1a5967949aa44b1d46`  
		Last Modified: Wed, 20 Sep 2023 15:44:23 GMT  
		Size: 1.9 KB (1871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02874a9e593b60862b1fa6079ec21abf9b108ff79ed1afb0fea2f5fb92c31bc0`  
		Last Modified: Wed, 20 Sep 2023 15:44:23 GMT  
		Size: 1.5 KB (1478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92715c2cab25dd578e4272162c7e32c5e783506711541b3e2cd6a0dd12e62fcf`  
		Last Modified: Wed, 20 Sep 2023 15:44:23 GMT  
		Size: 1.4 MB (1385383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6187ee8021740cf1e9d2e67c8904adc77f0ed4503d7f9ada0dec4b5537eaa35f`  
		Last Modified: Wed, 20 Sep 2023 15:44:23 GMT  
		Size: 489.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-standalone` - linux; arm64 variant v8

```console
$ docker pull adminer@sha256:82f1435981ebaa969cfd9cb3f452c46655dcf1715947a90a8c64dd3284db36d3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.3 MB (94338726 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51817ad17de2ccc468c81b03aa1f7c122e2d802f5411b384d4b8d341c711b3ff`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 20 Sep 2023 02:44:20 GMT
ADD file:46dcdcde338d2c01fed5db3fac9041736d9305145d8fc2039dd5b3714d38ede8 in / 
# Wed, 20 Sep 2023 02:44:21 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 18:04:43 GMT
STOPSIGNAL SIGINT
# Wed, 20 Sep 2023 18:05:03 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 18:05:04 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 20 Sep 2023 18:05:05 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 20 Sep 2023 18:05:05 GMT
WORKDIR /var/www/html
# Wed, 20 Sep 2023 18:05:05 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 20 Sep 2023 18:05:05 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 20 Sep 2023 18:05:05 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 20 Sep 2023 18:05:05 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 20 Sep 2023 18:05:16 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 20 Sep 2023 18:05:16 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 20 Sep 2023 18:05:16 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 20 Sep 2023 18:05:16 GMT
USER adminer
# Wed, 20 Sep 2023 18:05:16 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 20 Sep 2023 18:05:16 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:31f5dc1f52c865588c43d8ec718f14d430e149b28f0b28232da825da7ae28f76`  
		Last Modified: Wed, 20 Sep 2023 02:47:53 GMT  
		Size: 53.7 MB (53704892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c82c17c7529e7d3125d9a7f12b8359fac7e9cc29dbb6555d30cbe9bdda203722`  
		Last Modified: Wed, 20 Sep 2023 18:05:50 GMT  
		Size: 39.2 MB (39244274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27290e9432136a39923f648bd1220a36cdd54a4f8baacd87b500eed4d5018d2a`  
		Last Modified: Wed, 20 Sep 2023 18:05:44 GMT  
		Size: 393.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0029f07058cb36f9b27d218954d9e733b152fe47d9875b8d062632100f585d58`  
		Last Modified: Wed, 20 Sep 2023 18:05:44 GMT  
		Size: 1.9 KB (1883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f9ca9fda73283aac009ee0add3e063260cc5c09a89cbdaddef5d3e623c8ae3f`  
		Last Modified: Wed, 20 Sep 2023 18:05:44 GMT  
		Size: 1.5 KB (1477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99dc3e204c8096f4463277e628be5a5860db3a123dd45a87f99df2b8d1d76f77`  
		Last Modified: Wed, 20 Sep 2023 18:05:44 GMT  
		Size: 1.4 MB (1385317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5dbe53bc88443a7def3aa5bed48f19d4bc849da97d88790bf9701396443acac`  
		Last Modified: Wed, 20 Sep 2023 18:05:44 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-standalone` - linux; 386

```console
$ docker pull adminer@sha256:24a953b70c62fedfe7da2846b84d0a3133b442f0721e17fbf5df2d222ae440f8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.0 MB (96989218 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0cbe365ed04581b1b00d6390c52f9260afab49677042b95a947b6ca499d98bdc`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 20 Sep 2023 00:42:07 GMT
ADD file:342c36522089238a534c0912491a4cf64b89133969e051cdad2e694ec761142c in / 
# Wed, 20 Sep 2023 00:42:07 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 15:10:00 GMT
STOPSIGNAL SIGINT
# Wed, 20 Sep 2023 15:10:29 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 15:10:30 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 20 Sep 2023 15:10:31 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 20 Sep 2023 15:10:31 GMT
WORKDIR /var/www/html
# Wed, 20 Sep 2023 15:10:31 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 20 Sep 2023 15:10:31 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 20 Sep 2023 15:10:31 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 20 Sep 2023 15:10:31 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 20 Sep 2023 15:10:47 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 20 Sep 2023 15:10:47 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 20 Sep 2023 15:10:47 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 20 Sep 2023 15:10:47 GMT
USER adminer
# Wed, 20 Sep 2023 15:10:47 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 20 Sep 2023 15:10:47 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:00121bf241b18e981bcc804f905be7b34f95cce415db622599e21dc1a496ee8d`  
		Last Modified: Wed, 20 Sep 2023 00:47:11 GMT  
		Size: 56.0 MB (56040498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:964fa70975aa8c3eb5838cf9120935712a93ec197f9adce227a0d97a7df9d131`  
		Last Modified: Wed, 20 Sep 2023 15:11:38 GMT  
		Size: 39.6 MB (39559141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cf7eb9be8cf86ff0edfb0e7026187487f60c1b234c068e76b9d90c4bb2e56b5`  
		Last Modified: Wed, 20 Sep 2023 15:11:27 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7986b40b588b21caefc32e63e9bf4259713bd637125de9f9e6c415339b62bdb8`  
		Last Modified: Wed, 20 Sep 2023 15:11:27 GMT  
		Size: 1.9 KB (1869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da42b96b0425edc1796b564789c33a81ba8cc1bd8e95886fb24cba7bf6e830f9`  
		Last Modified: Wed, 20 Sep 2023 15:11:27 GMT  
		Size: 1.5 KB (1481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cb8907e77be88986e418354768b790c2a227d56ea26b7a7cdb7027c2958aa71`  
		Last Modified: Wed, 20 Sep 2023 15:11:27 GMT  
		Size: 1.4 MB (1385349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9fdcba82893748b7e9f6211dc3cd3248fa29ee6f78a24482d34339bb1fd857f`  
		Last Modified: Wed, 20 Sep 2023 15:11:27 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-standalone` - linux; mips64le

```console
$ docker pull adminer@sha256:ec803d54e73e17da91a36b9ce59b261f4f312dacabb7e0556302bce0443f75b7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.6 MB (92612531 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:215cf7d1502bb244df43b52290a34650eafce425c56c967b8c9e153a5ada9557`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Wed, 20 Sep 2023 06:40:19 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 20 Sep 2023 06:40:22 GMT
WORKDIR /var/www/html
# Wed, 20 Sep 2023 06:40:25 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 20 Sep 2023 06:40:28 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 20 Sep 2023 06:40:32 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 20 Sep 2023 06:40:35 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 20 Sep 2023 06:41:26 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 20 Sep 2023 06:41:29 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 20 Sep 2023 06:41:32 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 20 Sep 2023 06:41:35 GMT
USER adminer
# Wed, 20 Sep 2023 06:41:39 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 20 Sep 2023 06:41:42 GMT
EXPOSE 8080
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
	-	`sha256:4f0fa2061f2328806a3e6442dc58a5750d76966e9542efd972a12fd49f53cd69`  
		Last Modified: Wed, 20 Sep 2023 06:43:50 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04163c23cec6352cfd6ce393d04f5900400ea72c83d04af1552865c916a1c459`  
		Last Modified: Wed, 20 Sep 2023 06:43:50 GMT  
		Size: 1.5 KB (1481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d726d9d0dfbf6bba7fc6b01578c0a26c84fafdbe71a4e69674dfd1284ce0826`  
		Last Modified: Wed, 20 Sep 2023 06:43:51 GMT  
		Size: 1.4 MB (1386315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e96e2db0e4c5751ce57381cb92f2f2fff089adb321644959f5de599a271ebedc`  
		Last Modified: Wed, 20 Sep 2023 06:43:50 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-standalone` - linux; ppc64le

```console
$ docker pull adminer@sha256:e0809520a8bd4f91b86c0bfd4a871ce4707fd119706f564057dffe5e7c91f5fe
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.3 MB (101262041 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ad347a3c52aeda1176962cc50fcedfab4a87a129219de1394700476d688d49e`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 20 Sep 2023 07:53:09 GMT
ADD file:c12b11abfba27478510c84d05abdd8fec539db9ec30af6d042671f4d5bf793e5 in / 
# Wed, 20 Sep 2023 07:53:12 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 10:27:30 GMT
STOPSIGNAL SIGINT
# Wed, 20 Sep 2023 10:28:24 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 10:28:27 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 20 Sep 2023 10:28:28 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 20 Sep 2023 10:28:28 GMT
WORKDIR /var/www/html
# Wed, 20 Sep 2023 10:28:29 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 20 Sep 2023 10:28:29 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 20 Sep 2023 10:28:30 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 20 Sep 2023 10:28:30 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 20 Sep 2023 10:28:54 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 20 Sep 2023 10:28:54 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 20 Sep 2023 10:28:55 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 20 Sep 2023 10:28:55 GMT
USER adminer
# Wed, 20 Sep 2023 10:28:55 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 20 Sep 2023 10:28:55 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:9f3507d882ae95f06b3672497cdd3317bd4f8e0255e73d10f1f263e5d780f102`  
		Last Modified: Wed, 20 Sep 2023 08:50:16 GMT  
		Size: 58.9 MB (58928499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dc55ae4eee76ca2700dbf8d4554951df837121cc96140f29cbcc2d7308b4d72`  
		Last Modified: Wed, 20 Sep 2023 10:29:59 GMT  
		Size: 40.9 MB (40943739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:413bf430ecd0a8d3a68dc7841be8802fccca3af99645087fbb82e476cd335965`  
		Last Modified: Wed, 20 Sep 2023 10:29:47 GMT  
		Size: 396.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df2720d6c627570256eb0bc8943ba052f2b617c5dd972a3eb74196fc91a3dbbb`  
		Last Modified: Wed, 20 Sep 2023 10:29:47 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b6b255e136e7ac31afc340c04be397be6d98a39da922310d73ffbfff9687a2a`  
		Last Modified: Wed, 20 Sep 2023 10:29:47 GMT  
		Size: 1.5 KB (1481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36bfcc7e4826d80f455356e3a88eb31b2e5c559a49a733a25490d6becb652045`  
		Last Modified: Wed, 20 Sep 2023 10:29:47 GMT  
		Size: 1.4 MB (1385554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36a5f297e715a97e0af1984e9f7dd3cb60fa2226b31fc95bbfb6a3c5d85549af`  
		Last Modified: Wed, 20 Sep 2023 10:29:47 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-standalone` - linux; s390x

```console
$ docker pull adminer@sha256:120087fff0a708c70334e38726cab4a7703516787b7d901b1adc69fde470d694
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.7 MB (93701227 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42031d8d4365bb267d464fac6d7ab8b6e0ad4b097eb47e3e4b2dd8d14b64371d`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Wed, 20 Sep 2023 09:42:33 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 20 Sep 2023 09:42:33 GMT
WORKDIR /var/www/html
# Wed, 20 Sep 2023 09:42:33 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 20 Sep 2023 09:42:34 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 20 Sep 2023 09:42:34 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 20 Sep 2023 09:42:34 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 20 Sep 2023 09:42:57 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 20 Sep 2023 09:42:58 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 20 Sep 2023 09:42:58 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 20 Sep 2023 09:42:59 GMT
USER adminer
# Wed, 20 Sep 2023 09:42:59 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 20 Sep 2023 09:43:00 GMT
EXPOSE 8080
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
	-	`sha256:a0dfeb4132e2fe11e348c94294b33e51684a77419be87fae2d715412dc40e9c1`  
		Last Modified: Wed, 20 Sep 2023 09:43:57 GMT  
		Size: 1.9 KB (1883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:800a5df8795fcb07b6a7efb2135a2a662b31533cd779cc532445e86eae286b9f`  
		Last Modified: Wed, 20 Sep 2023 09:43:57 GMT  
		Size: 1.5 KB (1481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:321185c09a4e5d7e9a145855613f743ef531836df1355ae7593208920ad68541`  
		Last Modified: Wed, 20 Sep 2023 09:43:58 GMT  
		Size: 1.4 MB (1385674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c30b98bdcd0d0b081524334dc05d7905ceb45b6e8230e8156267e4759d587a2c`  
		Last Modified: Wed, 20 Sep 2023 09:43:57 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `adminer:4.8.1`

```console
$ docker pull adminer@sha256:40c1d6691703a8ca102dc108c4a6fc11863e928b6ae6014fb8557b6e083a29ff
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

### `adminer:4.8.1` - linux; amd64

```console
$ docker pull adminer@sha256:7fb4cb76b1a979671c18bba6ad81fc80d50cb56069b7fb542f75efb921b5e714
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.9 MB (95937427 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b672f480fc7a76f4b04207143a6b693b2a6eec24ac981709e626b16505609fd`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Wed, 20 Sep 2023 07:12:40 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 20 Sep 2023 07:12:40 GMT
WORKDIR /var/www/html
# Wed, 20 Sep 2023 07:12:41 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 20 Sep 2023 07:12:41 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 20 Sep 2023 07:12:41 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 20 Sep 2023 07:12:41 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 20 Sep 2023 07:12:53 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 20 Sep 2023 07:12:53 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 20 Sep 2023 07:12:53 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 20 Sep 2023 07:12:53 GMT
USER adminer
# Wed, 20 Sep 2023 07:12:53 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 20 Sep 2023 07:12:53 GMT
EXPOSE 8080
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
	-	`sha256:eb4bd38d1031bd7c467d8bce4c95f0b7697c26030cc73874381860ce97d0cdcd`  
		Last Modified: Wed, 20 Sep 2023 07:13:25 GMT  
		Size: 1.9 KB (1880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3bc33b7b683bc4196fbd1738ad588e8334ddb171c5d50c48429546f10cb487a`  
		Last Modified: Wed, 20 Sep 2023 07:13:25 GMT  
		Size: 1.5 KB (1477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d61d710f98a6cd583cbb61f1ace245ab27b2b69e7e606afdff85fe75a17f685`  
		Last Modified: Wed, 20 Sep 2023 07:13:26 GMT  
		Size: 1.4 MB (1385429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8441003ca946127323e284e8685841d9e549a658468e76be7cf68a2b08203f3`  
		Last Modified: Wed, 20 Sep 2023 07:13:25 GMT  
		Size: 488.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1` - linux; arm variant v5

```console
$ docker pull adminer@sha256:fc1ddb9f0a1b7781c7281f79851e7141b11e10f5cc915355b6cf6ff7824ede94
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.2 MB (91195621 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f410041bfb5c56158771bc68b88310247a497e74186a3dfdb22358729c1fd47e`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Wed, 20 Sep 2023 09:37:05 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 20 Sep 2023 09:37:05 GMT
WORKDIR /var/www/html
# Wed, 20 Sep 2023 09:37:05 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 20 Sep 2023 09:37:05 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 20 Sep 2023 09:37:05 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 20 Sep 2023 09:37:05 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 20 Sep 2023 09:37:21 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 20 Sep 2023 09:37:21 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 20 Sep 2023 09:37:21 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 20 Sep 2023 09:37:21 GMT
USER adminer
# Wed, 20 Sep 2023 09:37:21 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 20 Sep 2023 09:37:21 GMT
EXPOSE 8080
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
	-	`sha256:1cba35ed39d8d7c05cb37696f20ecdc7fde0f2d7fcbe968f50892aaabfdd84f2`  
		Last Modified: Wed, 20 Sep 2023 09:37:57 GMT  
		Size: 1.9 KB (1871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df6f0945f3469cf4fdd867a2409be0fc2b79d33a4267fb743edb64842be147f3`  
		Last Modified: Wed, 20 Sep 2023 09:37:57 GMT  
		Size: 1.5 KB (1476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb77accf421b5a1954871ae06a2ed8550b59f6ea59dfc1773263a25757e67757`  
		Last Modified: Wed, 20 Sep 2023 09:37:58 GMT  
		Size: 1.4 MB (1385374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1004d2eab86228b351246a3406fff91074ab91bf1c83691d49831a343972504f`  
		Last Modified: Wed, 20 Sep 2023 09:37:57 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1` - linux; arm variant v7

```console
$ docker pull adminer@sha256:d8a19218a54fe4fb52cb32cfc4d0ba0207b2976a94106cc4587ae23ef2796f6a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.8 MB (87795777 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2953870e043e0f3e517f17cce5c6d2e2d06f74d372de15043ba3193f11862b48`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 20 Sep 2023 04:57:26 GMT
ADD file:3bf3380482840b3a4166e82c3f951812076851ba1527261fdd1da780662b2de1 in / 
# Wed, 20 Sep 2023 04:57:26 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 15:43:10 GMT
STOPSIGNAL SIGINT
# Wed, 20 Sep 2023 15:43:35 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 15:43:36 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 20 Sep 2023 15:43:37 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 20 Sep 2023 15:43:37 GMT
WORKDIR /var/www/html
# Wed, 20 Sep 2023 15:43:37 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 20 Sep 2023 15:43:37 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 20 Sep 2023 15:43:37 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 20 Sep 2023 15:43:37 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 20 Sep 2023 15:43:50 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 20 Sep 2023 15:43:50 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 20 Sep 2023 15:43:50 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 20 Sep 2023 15:43:50 GMT
USER adminer
# Wed, 20 Sep 2023 15:43:50 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 20 Sep 2023 15:43:50 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:1d4e041d2204b383d6d6893cfcf5b852394f34744a85cea9ec0b3fb65cbc6143`  
		Last Modified: Wed, 20 Sep 2023 05:01:34 GMT  
		Size: 50.2 MB (50219551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4ca4acdacd0b759547187250427f6845ca2fc092c757b2e2f6667b1add9ba8d`  
		Last Modified: Wed, 20 Sep 2023 15:44:32 GMT  
		Size: 36.2 MB (36186615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc8798178b90f7264865be9cbfe742803f21777526c5ba6c86e1526c78998f64`  
		Last Modified: Wed, 20 Sep 2023 15:44:23 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e44ef76b17f1c1b9f8fa8b3c28b236740ee52ee91c0bf1a5967949aa44b1d46`  
		Last Modified: Wed, 20 Sep 2023 15:44:23 GMT  
		Size: 1.9 KB (1871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02874a9e593b60862b1fa6079ec21abf9b108ff79ed1afb0fea2f5fb92c31bc0`  
		Last Modified: Wed, 20 Sep 2023 15:44:23 GMT  
		Size: 1.5 KB (1478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92715c2cab25dd578e4272162c7e32c5e783506711541b3e2cd6a0dd12e62fcf`  
		Last Modified: Wed, 20 Sep 2023 15:44:23 GMT  
		Size: 1.4 MB (1385383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6187ee8021740cf1e9d2e67c8904adc77f0ed4503d7f9ada0dec4b5537eaa35f`  
		Last Modified: Wed, 20 Sep 2023 15:44:23 GMT  
		Size: 489.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1` - linux; arm64 variant v8

```console
$ docker pull adminer@sha256:82f1435981ebaa969cfd9cb3f452c46655dcf1715947a90a8c64dd3284db36d3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.3 MB (94338726 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51817ad17de2ccc468c81b03aa1f7c122e2d802f5411b384d4b8d341c711b3ff`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 20 Sep 2023 02:44:20 GMT
ADD file:46dcdcde338d2c01fed5db3fac9041736d9305145d8fc2039dd5b3714d38ede8 in / 
# Wed, 20 Sep 2023 02:44:21 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 18:04:43 GMT
STOPSIGNAL SIGINT
# Wed, 20 Sep 2023 18:05:03 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 18:05:04 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 20 Sep 2023 18:05:05 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 20 Sep 2023 18:05:05 GMT
WORKDIR /var/www/html
# Wed, 20 Sep 2023 18:05:05 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 20 Sep 2023 18:05:05 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 20 Sep 2023 18:05:05 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 20 Sep 2023 18:05:05 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 20 Sep 2023 18:05:16 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 20 Sep 2023 18:05:16 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 20 Sep 2023 18:05:16 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 20 Sep 2023 18:05:16 GMT
USER adminer
# Wed, 20 Sep 2023 18:05:16 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 20 Sep 2023 18:05:16 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:31f5dc1f52c865588c43d8ec718f14d430e149b28f0b28232da825da7ae28f76`  
		Last Modified: Wed, 20 Sep 2023 02:47:53 GMT  
		Size: 53.7 MB (53704892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c82c17c7529e7d3125d9a7f12b8359fac7e9cc29dbb6555d30cbe9bdda203722`  
		Last Modified: Wed, 20 Sep 2023 18:05:50 GMT  
		Size: 39.2 MB (39244274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27290e9432136a39923f648bd1220a36cdd54a4f8baacd87b500eed4d5018d2a`  
		Last Modified: Wed, 20 Sep 2023 18:05:44 GMT  
		Size: 393.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0029f07058cb36f9b27d218954d9e733b152fe47d9875b8d062632100f585d58`  
		Last Modified: Wed, 20 Sep 2023 18:05:44 GMT  
		Size: 1.9 KB (1883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f9ca9fda73283aac009ee0add3e063260cc5c09a89cbdaddef5d3e623c8ae3f`  
		Last Modified: Wed, 20 Sep 2023 18:05:44 GMT  
		Size: 1.5 KB (1477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99dc3e204c8096f4463277e628be5a5860db3a123dd45a87f99df2b8d1d76f77`  
		Last Modified: Wed, 20 Sep 2023 18:05:44 GMT  
		Size: 1.4 MB (1385317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5dbe53bc88443a7def3aa5bed48f19d4bc849da97d88790bf9701396443acac`  
		Last Modified: Wed, 20 Sep 2023 18:05:44 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1` - linux; 386

```console
$ docker pull adminer@sha256:24a953b70c62fedfe7da2846b84d0a3133b442f0721e17fbf5df2d222ae440f8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.0 MB (96989218 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0cbe365ed04581b1b00d6390c52f9260afab49677042b95a947b6ca499d98bdc`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 20 Sep 2023 00:42:07 GMT
ADD file:342c36522089238a534c0912491a4cf64b89133969e051cdad2e694ec761142c in / 
# Wed, 20 Sep 2023 00:42:07 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 15:10:00 GMT
STOPSIGNAL SIGINT
# Wed, 20 Sep 2023 15:10:29 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 15:10:30 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 20 Sep 2023 15:10:31 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 20 Sep 2023 15:10:31 GMT
WORKDIR /var/www/html
# Wed, 20 Sep 2023 15:10:31 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 20 Sep 2023 15:10:31 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 20 Sep 2023 15:10:31 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 20 Sep 2023 15:10:31 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 20 Sep 2023 15:10:47 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 20 Sep 2023 15:10:47 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 20 Sep 2023 15:10:47 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 20 Sep 2023 15:10:47 GMT
USER adminer
# Wed, 20 Sep 2023 15:10:47 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 20 Sep 2023 15:10:47 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:00121bf241b18e981bcc804f905be7b34f95cce415db622599e21dc1a496ee8d`  
		Last Modified: Wed, 20 Sep 2023 00:47:11 GMT  
		Size: 56.0 MB (56040498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:964fa70975aa8c3eb5838cf9120935712a93ec197f9adce227a0d97a7df9d131`  
		Last Modified: Wed, 20 Sep 2023 15:11:38 GMT  
		Size: 39.6 MB (39559141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cf7eb9be8cf86ff0edfb0e7026187487f60c1b234c068e76b9d90c4bb2e56b5`  
		Last Modified: Wed, 20 Sep 2023 15:11:27 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7986b40b588b21caefc32e63e9bf4259713bd637125de9f9e6c415339b62bdb8`  
		Last Modified: Wed, 20 Sep 2023 15:11:27 GMT  
		Size: 1.9 KB (1869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da42b96b0425edc1796b564789c33a81ba8cc1bd8e95886fb24cba7bf6e830f9`  
		Last Modified: Wed, 20 Sep 2023 15:11:27 GMT  
		Size: 1.5 KB (1481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cb8907e77be88986e418354768b790c2a227d56ea26b7a7cdb7027c2958aa71`  
		Last Modified: Wed, 20 Sep 2023 15:11:27 GMT  
		Size: 1.4 MB (1385349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9fdcba82893748b7e9f6211dc3cd3248fa29ee6f78a24482d34339bb1fd857f`  
		Last Modified: Wed, 20 Sep 2023 15:11:27 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1` - linux; mips64le

```console
$ docker pull adminer@sha256:ec803d54e73e17da91a36b9ce59b261f4f312dacabb7e0556302bce0443f75b7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.6 MB (92612531 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:215cf7d1502bb244df43b52290a34650eafce425c56c967b8c9e153a5ada9557`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Wed, 20 Sep 2023 06:40:19 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 20 Sep 2023 06:40:22 GMT
WORKDIR /var/www/html
# Wed, 20 Sep 2023 06:40:25 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 20 Sep 2023 06:40:28 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 20 Sep 2023 06:40:32 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 20 Sep 2023 06:40:35 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 20 Sep 2023 06:41:26 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 20 Sep 2023 06:41:29 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 20 Sep 2023 06:41:32 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 20 Sep 2023 06:41:35 GMT
USER adminer
# Wed, 20 Sep 2023 06:41:39 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 20 Sep 2023 06:41:42 GMT
EXPOSE 8080
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
	-	`sha256:4f0fa2061f2328806a3e6442dc58a5750d76966e9542efd972a12fd49f53cd69`  
		Last Modified: Wed, 20 Sep 2023 06:43:50 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04163c23cec6352cfd6ce393d04f5900400ea72c83d04af1552865c916a1c459`  
		Last Modified: Wed, 20 Sep 2023 06:43:50 GMT  
		Size: 1.5 KB (1481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d726d9d0dfbf6bba7fc6b01578c0a26c84fafdbe71a4e69674dfd1284ce0826`  
		Last Modified: Wed, 20 Sep 2023 06:43:51 GMT  
		Size: 1.4 MB (1386315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e96e2db0e4c5751ce57381cb92f2f2fff089adb321644959f5de599a271ebedc`  
		Last Modified: Wed, 20 Sep 2023 06:43:50 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1` - linux; ppc64le

```console
$ docker pull adminer@sha256:e0809520a8bd4f91b86c0bfd4a871ce4707fd119706f564057dffe5e7c91f5fe
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.3 MB (101262041 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ad347a3c52aeda1176962cc50fcedfab4a87a129219de1394700476d688d49e`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 20 Sep 2023 07:53:09 GMT
ADD file:c12b11abfba27478510c84d05abdd8fec539db9ec30af6d042671f4d5bf793e5 in / 
# Wed, 20 Sep 2023 07:53:12 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 10:27:30 GMT
STOPSIGNAL SIGINT
# Wed, 20 Sep 2023 10:28:24 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 10:28:27 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 20 Sep 2023 10:28:28 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 20 Sep 2023 10:28:28 GMT
WORKDIR /var/www/html
# Wed, 20 Sep 2023 10:28:29 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 20 Sep 2023 10:28:29 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 20 Sep 2023 10:28:30 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 20 Sep 2023 10:28:30 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 20 Sep 2023 10:28:54 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 20 Sep 2023 10:28:54 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 20 Sep 2023 10:28:55 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 20 Sep 2023 10:28:55 GMT
USER adminer
# Wed, 20 Sep 2023 10:28:55 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 20 Sep 2023 10:28:55 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:9f3507d882ae95f06b3672497cdd3317bd4f8e0255e73d10f1f263e5d780f102`  
		Last Modified: Wed, 20 Sep 2023 08:50:16 GMT  
		Size: 58.9 MB (58928499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dc55ae4eee76ca2700dbf8d4554951df837121cc96140f29cbcc2d7308b4d72`  
		Last Modified: Wed, 20 Sep 2023 10:29:59 GMT  
		Size: 40.9 MB (40943739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:413bf430ecd0a8d3a68dc7841be8802fccca3af99645087fbb82e476cd335965`  
		Last Modified: Wed, 20 Sep 2023 10:29:47 GMT  
		Size: 396.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df2720d6c627570256eb0bc8943ba052f2b617c5dd972a3eb74196fc91a3dbbb`  
		Last Modified: Wed, 20 Sep 2023 10:29:47 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b6b255e136e7ac31afc340c04be397be6d98a39da922310d73ffbfff9687a2a`  
		Last Modified: Wed, 20 Sep 2023 10:29:47 GMT  
		Size: 1.5 KB (1481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36bfcc7e4826d80f455356e3a88eb31b2e5c559a49a733a25490d6becb652045`  
		Last Modified: Wed, 20 Sep 2023 10:29:47 GMT  
		Size: 1.4 MB (1385554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36a5f297e715a97e0af1984e9f7dd3cb60fa2226b31fc95bbfb6a3c5d85549af`  
		Last Modified: Wed, 20 Sep 2023 10:29:47 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1` - linux; s390x

```console
$ docker pull adminer@sha256:120087fff0a708c70334e38726cab4a7703516787b7d901b1adc69fde470d694
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.7 MB (93701227 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42031d8d4365bb267d464fac6d7ab8b6e0ad4b097eb47e3e4b2dd8d14b64371d`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Wed, 20 Sep 2023 09:42:33 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 20 Sep 2023 09:42:33 GMT
WORKDIR /var/www/html
# Wed, 20 Sep 2023 09:42:33 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 20 Sep 2023 09:42:34 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 20 Sep 2023 09:42:34 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 20 Sep 2023 09:42:34 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 20 Sep 2023 09:42:57 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 20 Sep 2023 09:42:58 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 20 Sep 2023 09:42:58 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 20 Sep 2023 09:42:59 GMT
USER adminer
# Wed, 20 Sep 2023 09:42:59 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 20 Sep 2023 09:43:00 GMT
EXPOSE 8080
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
	-	`sha256:a0dfeb4132e2fe11e348c94294b33e51684a77419be87fae2d715412dc40e9c1`  
		Last Modified: Wed, 20 Sep 2023 09:43:57 GMT  
		Size: 1.9 KB (1883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:800a5df8795fcb07b6a7efb2135a2a662b31533cd779cc532445e86eae286b9f`  
		Last Modified: Wed, 20 Sep 2023 09:43:57 GMT  
		Size: 1.5 KB (1481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:321185c09a4e5d7e9a145855613f743ef531836df1355ae7593208920ad68541`  
		Last Modified: Wed, 20 Sep 2023 09:43:58 GMT  
		Size: 1.4 MB (1385674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c30b98bdcd0d0b081524334dc05d7905ceb45b6e8230e8156267e4759d587a2c`  
		Last Modified: Wed, 20 Sep 2023 09:43:57 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `adminer:4.8.1-fastcgi`

```console
$ docker pull adminer@sha256:b1eb6b4fef1cbe8aae2448f5ff246547904ddde8353382e40fd999fa7cd90047
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

### `adminer:4.8.1-fastcgi` - linux; amd64

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

### `adminer:4.8.1-fastcgi` - linux; arm variant v5

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

### `adminer:4.8.1-fastcgi` - linux; arm variant v7

```console
$ docker pull adminer@sha256:542098b1184f641c16a22b9b0d3a814b99a7bffca9593133e604d06e76cfb2f8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.8 MB (87798559 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7fe9e2628383acfd8d7c700d2a4881cfe1815fbee052c129294f79bce56e1b5`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Wed, 20 Sep 2023 04:57:26 GMT
ADD file:3bf3380482840b3a4166e82c3f951812076851ba1527261fdd1da780662b2de1 in / 
# Wed, 20 Sep 2023 04:57:26 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 15:43:10 GMT
STOPSIGNAL SIGINT
# Wed, 20 Sep 2023 15:43:35 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 15:43:36 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 20 Sep 2023 15:43:59 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Wed, 20 Sep 2023 15:44:00 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 20 Sep 2023 15:44:00 GMT
WORKDIR /var/www/html
# Wed, 20 Sep 2023 15:44:00 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 20 Sep 2023 15:44:00 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 20 Sep 2023 15:44:00 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 20 Sep 2023 15:44:00 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 20 Sep 2023 15:44:11 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 20 Sep 2023 15:44:11 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 20 Sep 2023 15:44:12 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 20 Sep 2023 15:44:12 GMT
USER adminer
# Wed, 20 Sep 2023 15:44:12 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:1d4e041d2204b383d6d6893cfcf5b852394f34744a85cea9ec0b3fb65cbc6143`  
		Last Modified: Wed, 20 Sep 2023 05:01:34 GMT  
		Size: 50.2 MB (50219551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4ca4acdacd0b759547187250427f6845ca2fc092c757b2e2f6667b1add9ba8d`  
		Last Modified: Wed, 20 Sep 2023 15:44:32 GMT  
		Size: 36.2 MB (36186615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc8798178b90f7264865be9cbfe742803f21777526c5ba6c86e1526c78998f64`  
		Last Modified: Wed, 20 Sep 2023 15:44:23 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3364c0b2504d3af9b0175a6e77522d257e70f24251cfd629dd6bd3ef24b5f119`  
		Last Modified: Wed, 20 Sep 2023 15:44:49 GMT  
		Size: 2.7 KB (2713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62a19c34bb68631c5d5858d4245052d13f760c8cf841e4a4cd1f02343aed2d5f`  
		Last Modified: Wed, 20 Sep 2023 15:44:49 GMT  
		Size: 1.9 KB (1869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08676442b17b4a0cc0ffff5e52fe487a0107e28a668edfdff6ad54606481fb05`  
		Last Modified: Wed, 20 Sep 2023 15:44:49 GMT  
		Size: 1.5 KB (1480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82515cdefa5e1215ed49066547b07fa57d1b9da8fabd0522836ba51ad7e9ab82`  
		Last Modified: Wed, 20 Sep 2023 15:44:49 GMT  
		Size: 1.4 MB (1385449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cf0ebb373156a781676a77242c49b21185c9e025e5104d6b83fec00a1a77b78`  
		Last Modified: Wed, 20 Sep 2023 15:44:49 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1-fastcgi` - linux; arm64 variant v8

```console
$ docker pull adminer@sha256:1cff0be1992c13ea25123e8139fc1179c0f722357c1f54f6be3a143db8a52899
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.3 MB (94341405 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ce755452b4733c8b45e4d8e12c142771d8fd25391360bfaff9353b77d3a7296`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Wed, 20 Sep 2023 02:44:20 GMT
ADD file:46dcdcde338d2c01fed5db3fac9041736d9305145d8fc2039dd5b3714d38ede8 in / 
# Wed, 20 Sep 2023 02:44:21 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 18:04:43 GMT
STOPSIGNAL SIGINT
# Wed, 20 Sep 2023 18:05:03 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 18:05:04 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 20 Sep 2023 18:05:23 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Wed, 20 Sep 2023 18:05:23 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 20 Sep 2023 18:05:23 GMT
WORKDIR /var/www/html
# Wed, 20 Sep 2023 18:05:24 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 20 Sep 2023 18:05:24 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 20 Sep 2023 18:05:24 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 20 Sep 2023 18:05:24 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 20 Sep 2023 18:05:34 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 20 Sep 2023 18:05:34 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 20 Sep 2023 18:05:34 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 20 Sep 2023 18:05:35 GMT
USER adminer
# Wed, 20 Sep 2023 18:05:35 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:31f5dc1f52c865588c43d8ec718f14d430e149b28f0b28232da825da7ae28f76`  
		Last Modified: Wed, 20 Sep 2023 02:47:53 GMT  
		Size: 53.7 MB (53704892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c82c17c7529e7d3125d9a7f12b8359fac7e9cc29dbb6555d30cbe9bdda203722`  
		Last Modified: Wed, 20 Sep 2023 18:05:50 GMT  
		Size: 39.2 MB (39244274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27290e9432136a39923f648bd1220a36cdd54a4f8baacd87b500eed4d5018d2a`  
		Last Modified: Wed, 20 Sep 2023 18:05:44 GMT  
		Size: 393.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4d0cfb12b1cdc502f0839f004aa983a25ea38bb788e0b734aa01a54303ae0e2`  
		Last Modified: Wed, 20 Sep 2023 18:06:08 GMT  
		Size: 2.7 KB (2711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76b68d0109bf502fae5cb6a017bbb0e37d31131dc631b3ae9ce75b6603690194`  
		Last Modified: Wed, 20 Sep 2023 18:06:08 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4abe36926b3c359fc35e36926f70d35534faf595ccb23765fd12a141f764e821`  
		Last Modified: Wed, 20 Sep 2023 18:06:08 GMT  
		Size: 1.5 KB (1478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42b5d424d36cd52afb1439ff8165fbc761f2319ec3e4e891eadb0f03a089199b`  
		Last Modified: Wed, 20 Sep 2023 18:06:08 GMT  
		Size: 1.4 MB (1385285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a545cd65be7574c61d9c4d38924911eeffdabb28d5d74e8198afda6043e8579`  
		Last Modified: Wed, 20 Sep 2023 18:06:08 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1-fastcgi` - linux; 386

```console
$ docker pull adminer@sha256:846388f4f74cf512bb64bf84c6b64a14c87e97c2082957de704afb301f49a8f3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.0 MB (96991935 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d51e9267cebf41d916c5538d54fa90a930c77844a72ea2d84572bf9b9c7feba`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Wed, 20 Sep 2023 00:42:07 GMT
ADD file:342c36522089238a534c0912491a4cf64b89133969e051cdad2e694ec761142c in / 
# Wed, 20 Sep 2023 00:42:07 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 15:10:00 GMT
STOPSIGNAL SIGINT
# Wed, 20 Sep 2023 15:10:29 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 15:10:30 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 20 Sep 2023 15:10:58 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Wed, 20 Sep 2023 15:10:59 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 20 Sep 2023 15:10:59 GMT
WORKDIR /var/www/html
# Wed, 20 Sep 2023 15:10:59 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 20 Sep 2023 15:10:59 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 20 Sep 2023 15:10:59 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 20 Sep 2023 15:10:59 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 20 Sep 2023 15:11:15 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 20 Sep 2023 15:11:15 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 20 Sep 2023 15:11:15 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 20 Sep 2023 15:11:15 GMT
USER adminer
# Wed, 20 Sep 2023 15:11:15 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:00121bf241b18e981bcc804f905be7b34f95cce415db622599e21dc1a496ee8d`  
		Last Modified: Wed, 20 Sep 2023 00:47:11 GMT  
		Size: 56.0 MB (56040498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:964fa70975aa8c3eb5838cf9120935712a93ec197f9adce227a0d97a7df9d131`  
		Last Modified: Wed, 20 Sep 2023 15:11:38 GMT  
		Size: 39.6 MB (39559141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cf7eb9be8cf86ff0edfb0e7026187487f60c1b234c068e76b9d90c4bb2e56b5`  
		Last Modified: Wed, 20 Sep 2023 15:11:27 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14739144aeefcf6bb5b82efb1be6c8c36061cb79988c3d04e94ac3af2889703d`  
		Last Modified: Wed, 20 Sep 2023 15:11:57 GMT  
		Size: 2.7 KB (2707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be431c45e4957603c8fc57e2e1c75ca225cf90bdaee782e22140bd61fb848bd2`  
		Last Modified: Wed, 20 Sep 2023 15:11:58 GMT  
		Size: 1.9 KB (1870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af4bb02c3c060fffe6e6033ae734961cbe056f312fe14b88a19af87c4f244f12`  
		Last Modified: Wed, 20 Sep 2023 15:11:57 GMT  
		Size: 1.5 KB (1472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ed951e5e4331a40e2299fe20b587b7ac277d2561486420e3f603a26eaf55c7f`  
		Last Modified: Wed, 20 Sep 2023 15:11:57 GMT  
		Size: 1.4 MB (1385367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e84da2513a7218dd7201673bcd22e26b222c95847fcf06c9b8a7151d89c1b1f0`  
		Last Modified: Wed, 20 Sep 2023 15:11:56 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1-fastcgi` - linux; mips64le

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

### `adminer:4.8.1-fastcgi` - linux; ppc64le

```console
$ docker pull adminer@sha256:79299ee4e64a10ed155d4b0e07c0b513251f6730c593768c6e3ed11269d0b296
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.3 MB (101264733 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc0562129b0dc47471215a72b69dc9de21102422b16b11725a10b19d56f6b30c`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Wed, 20 Sep 2023 07:53:09 GMT
ADD file:c12b11abfba27478510c84d05abdd8fec539db9ec30af6d042671f4d5bf793e5 in / 
# Wed, 20 Sep 2023 07:53:12 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 10:27:30 GMT
STOPSIGNAL SIGINT
# Wed, 20 Sep 2023 10:28:24 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 10:28:27 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 20 Sep 2023 10:29:10 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Wed, 20 Sep 2023 10:29:11 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 20 Sep 2023 10:29:11 GMT
WORKDIR /var/www/html
# Wed, 20 Sep 2023 10:29:11 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 20 Sep 2023 10:29:12 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 20 Sep 2023 10:29:12 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 20 Sep 2023 10:29:12 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 20 Sep 2023 10:29:34 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 20 Sep 2023 10:29:34 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 20 Sep 2023 10:29:34 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 20 Sep 2023 10:29:35 GMT
USER adminer
# Wed, 20 Sep 2023 10:29:35 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:9f3507d882ae95f06b3672497cdd3317bd4f8e0255e73d10f1f263e5d780f102`  
		Last Modified: Wed, 20 Sep 2023 08:50:16 GMT  
		Size: 58.9 MB (58928499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dc55ae4eee76ca2700dbf8d4554951df837121cc96140f29cbcc2d7308b4d72`  
		Last Modified: Wed, 20 Sep 2023 10:29:59 GMT  
		Size: 40.9 MB (40943739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:413bf430ecd0a8d3a68dc7841be8802fccca3af99645087fbb82e476cd335965`  
		Last Modified: Wed, 20 Sep 2023 10:29:47 GMT  
		Size: 396.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33c90f4bc93f05165b4c2a576055f2d0614e44beb75f656246a36dab518a167e`  
		Last Modified: Wed, 20 Sep 2023 10:30:20 GMT  
		Size: 2.7 KB (2712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8042ccb66d3f41a43740fe4d53cf23c908f55c921ebbdd7f85a713640e21b71`  
		Last Modified: Wed, 20 Sep 2023 10:30:20 GMT  
		Size: 1.9 KB (1877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9687767d889f697b2273a34c6066aa7a3319201ef0abe10a52e58cd6192f18e0`  
		Last Modified: Wed, 20 Sep 2023 10:30:20 GMT  
		Size: 1.5 KB (1480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:373f9256ef78f4c4f1ce5dcac32e6c33dc0c75c189e9d0fe44e89efc9ad1e68e`  
		Last Modified: Wed, 20 Sep 2023 10:30:21 GMT  
		Size: 1.4 MB (1385537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f063a3c5af7dc109b9e33bbf3c86fea2b892e631c1128300364996aa081e72d`  
		Last Modified: Wed, 20 Sep 2023 10:30:20 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1-fastcgi` - linux; s390x

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

## `adminer:4.8.1-standalone`

```console
$ docker pull adminer@sha256:40c1d6691703a8ca102dc108c4a6fc11863e928b6ae6014fb8557b6e083a29ff
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

### `adminer:4.8.1-standalone` - linux; amd64

```console
$ docker pull adminer@sha256:7fb4cb76b1a979671c18bba6ad81fc80d50cb56069b7fb542f75efb921b5e714
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.9 MB (95937427 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b672f480fc7a76f4b04207143a6b693b2a6eec24ac981709e626b16505609fd`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Wed, 20 Sep 2023 07:12:40 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 20 Sep 2023 07:12:40 GMT
WORKDIR /var/www/html
# Wed, 20 Sep 2023 07:12:41 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 20 Sep 2023 07:12:41 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 20 Sep 2023 07:12:41 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 20 Sep 2023 07:12:41 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 20 Sep 2023 07:12:53 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 20 Sep 2023 07:12:53 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 20 Sep 2023 07:12:53 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 20 Sep 2023 07:12:53 GMT
USER adminer
# Wed, 20 Sep 2023 07:12:53 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 20 Sep 2023 07:12:53 GMT
EXPOSE 8080
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
	-	`sha256:eb4bd38d1031bd7c467d8bce4c95f0b7697c26030cc73874381860ce97d0cdcd`  
		Last Modified: Wed, 20 Sep 2023 07:13:25 GMT  
		Size: 1.9 KB (1880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3bc33b7b683bc4196fbd1738ad588e8334ddb171c5d50c48429546f10cb487a`  
		Last Modified: Wed, 20 Sep 2023 07:13:25 GMT  
		Size: 1.5 KB (1477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d61d710f98a6cd583cbb61f1ace245ab27b2b69e7e606afdff85fe75a17f685`  
		Last Modified: Wed, 20 Sep 2023 07:13:26 GMT  
		Size: 1.4 MB (1385429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8441003ca946127323e284e8685841d9e549a658468e76be7cf68a2b08203f3`  
		Last Modified: Wed, 20 Sep 2023 07:13:25 GMT  
		Size: 488.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1-standalone` - linux; arm variant v5

```console
$ docker pull adminer@sha256:fc1ddb9f0a1b7781c7281f79851e7141b11e10f5cc915355b6cf6ff7824ede94
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.2 MB (91195621 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f410041bfb5c56158771bc68b88310247a497e74186a3dfdb22358729c1fd47e`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Wed, 20 Sep 2023 09:37:05 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 20 Sep 2023 09:37:05 GMT
WORKDIR /var/www/html
# Wed, 20 Sep 2023 09:37:05 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 20 Sep 2023 09:37:05 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 20 Sep 2023 09:37:05 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 20 Sep 2023 09:37:05 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 20 Sep 2023 09:37:21 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 20 Sep 2023 09:37:21 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 20 Sep 2023 09:37:21 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 20 Sep 2023 09:37:21 GMT
USER adminer
# Wed, 20 Sep 2023 09:37:21 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 20 Sep 2023 09:37:21 GMT
EXPOSE 8080
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
	-	`sha256:1cba35ed39d8d7c05cb37696f20ecdc7fde0f2d7fcbe968f50892aaabfdd84f2`  
		Last Modified: Wed, 20 Sep 2023 09:37:57 GMT  
		Size: 1.9 KB (1871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df6f0945f3469cf4fdd867a2409be0fc2b79d33a4267fb743edb64842be147f3`  
		Last Modified: Wed, 20 Sep 2023 09:37:57 GMT  
		Size: 1.5 KB (1476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb77accf421b5a1954871ae06a2ed8550b59f6ea59dfc1773263a25757e67757`  
		Last Modified: Wed, 20 Sep 2023 09:37:58 GMT  
		Size: 1.4 MB (1385374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1004d2eab86228b351246a3406fff91074ab91bf1c83691d49831a343972504f`  
		Last Modified: Wed, 20 Sep 2023 09:37:57 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1-standalone` - linux; arm variant v7

```console
$ docker pull adminer@sha256:d8a19218a54fe4fb52cb32cfc4d0ba0207b2976a94106cc4587ae23ef2796f6a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.8 MB (87795777 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2953870e043e0f3e517f17cce5c6d2e2d06f74d372de15043ba3193f11862b48`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 20 Sep 2023 04:57:26 GMT
ADD file:3bf3380482840b3a4166e82c3f951812076851ba1527261fdd1da780662b2de1 in / 
# Wed, 20 Sep 2023 04:57:26 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 15:43:10 GMT
STOPSIGNAL SIGINT
# Wed, 20 Sep 2023 15:43:35 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 15:43:36 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 20 Sep 2023 15:43:37 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 20 Sep 2023 15:43:37 GMT
WORKDIR /var/www/html
# Wed, 20 Sep 2023 15:43:37 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 20 Sep 2023 15:43:37 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 20 Sep 2023 15:43:37 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 20 Sep 2023 15:43:37 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 20 Sep 2023 15:43:50 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 20 Sep 2023 15:43:50 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 20 Sep 2023 15:43:50 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 20 Sep 2023 15:43:50 GMT
USER adminer
# Wed, 20 Sep 2023 15:43:50 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 20 Sep 2023 15:43:50 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:1d4e041d2204b383d6d6893cfcf5b852394f34744a85cea9ec0b3fb65cbc6143`  
		Last Modified: Wed, 20 Sep 2023 05:01:34 GMT  
		Size: 50.2 MB (50219551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4ca4acdacd0b759547187250427f6845ca2fc092c757b2e2f6667b1add9ba8d`  
		Last Modified: Wed, 20 Sep 2023 15:44:32 GMT  
		Size: 36.2 MB (36186615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc8798178b90f7264865be9cbfe742803f21777526c5ba6c86e1526c78998f64`  
		Last Modified: Wed, 20 Sep 2023 15:44:23 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e44ef76b17f1c1b9f8fa8b3c28b236740ee52ee91c0bf1a5967949aa44b1d46`  
		Last Modified: Wed, 20 Sep 2023 15:44:23 GMT  
		Size: 1.9 KB (1871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02874a9e593b60862b1fa6079ec21abf9b108ff79ed1afb0fea2f5fb92c31bc0`  
		Last Modified: Wed, 20 Sep 2023 15:44:23 GMT  
		Size: 1.5 KB (1478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92715c2cab25dd578e4272162c7e32c5e783506711541b3e2cd6a0dd12e62fcf`  
		Last Modified: Wed, 20 Sep 2023 15:44:23 GMT  
		Size: 1.4 MB (1385383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6187ee8021740cf1e9d2e67c8904adc77f0ed4503d7f9ada0dec4b5537eaa35f`  
		Last Modified: Wed, 20 Sep 2023 15:44:23 GMT  
		Size: 489.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1-standalone` - linux; arm64 variant v8

```console
$ docker pull adminer@sha256:82f1435981ebaa969cfd9cb3f452c46655dcf1715947a90a8c64dd3284db36d3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.3 MB (94338726 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51817ad17de2ccc468c81b03aa1f7c122e2d802f5411b384d4b8d341c711b3ff`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 20 Sep 2023 02:44:20 GMT
ADD file:46dcdcde338d2c01fed5db3fac9041736d9305145d8fc2039dd5b3714d38ede8 in / 
# Wed, 20 Sep 2023 02:44:21 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 18:04:43 GMT
STOPSIGNAL SIGINT
# Wed, 20 Sep 2023 18:05:03 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 18:05:04 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 20 Sep 2023 18:05:05 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 20 Sep 2023 18:05:05 GMT
WORKDIR /var/www/html
# Wed, 20 Sep 2023 18:05:05 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 20 Sep 2023 18:05:05 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 20 Sep 2023 18:05:05 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 20 Sep 2023 18:05:05 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 20 Sep 2023 18:05:16 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 20 Sep 2023 18:05:16 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 20 Sep 2023 18:05:16 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 20 Sep 2023 18:05:16 GMT
USER adminer
# Wed, 20 Sep 2023 18:05:16 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 20 Sep 2023 18:05:16 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:31f5dc1f52c865588c43d8ec718f14d430e149b28f0b28232da825da7ae28f76`  
		Last Modified: Wed, 20 Sep 2023 02:47:53 GMT  
		Size: 53.7 MB (53704892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c82c17c7529e7d3125d9a7f12b8359fac7e9cc29dbb6555d30cbe9bdda203722`  
		Last Modified: Wed, 20 Sep 2023 18:05:50 GMT  
		Size: 39.2 MB (39244274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27290e9432136a39923f648bd1220a36cdd54a4f8baacd87b500eed4d5018d2a`  
		Last Modified: Wed, 20 Sep 2023 18:05:44 GMT  
		Size: 393.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0029f07058cb36f9b27d218954d9e733b152fe47d9875b8d062632100f585d58`  
		Last Modified: Wed, 20 Sep 2023 18:05:44 GMT  
		Size: 1.9 KB (1883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f9ca9fda73283aac009ee0add3e063260cc5c09a89cbdaddef5d3e623c8ae3f`  
		Last Modified: Wed, 20 Sep 2023 18:05:44 GMT  
		Size: 1.5 KB (1477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99dc3e204c8096f4463277e628be5a5860db3a123dd45a87f99df2b8d1d76f77`  
		Last Modified: Wed, 20 Sep 2023 18:05:44 GMT  
		Size: 1.4 MB (1385317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5dbe53bc88443a7def3aa5bed48f19d4bc849da97d88790bf9701396443acac`  
		Last Modified: Wed, 20 Sep 2023 18:05:44 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1-standalone` - linux; 386

```console
$ docker pull adminer@sha256:24a953b70c62fedfe7da2846b84d0a3133b442f0721e17fbf5df2d222ae440f8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.0 MB (96989218 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0cbe365ed04581b1b00d6390c52f9260afab49677042b95a947b6ca499d98bdc`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 20 Sep 2023 00:42:07 GMT
ADD file:342c36522089238a534c0912491a4cf64b89133969e051cdad2e694ec761142c in / 
# Wed, 20 Sep 2023 00:42:07 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 15:10:00 GMT
STOPSIGNAL SIGINT
# Wed, 20 Sep 2023 15:10:29 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 15:10:30 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 20 Sep 2023 15:10:31 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 20 Sep 2023 15:10:31 GMT
WORKDIR /var/www/html
# Wed, 20 Sep 2023 15:10:31 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 20 Sep 2023 15:10:31 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 20 Sep 2023 15:10:31 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 20 Sep 2023 15:10:31 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 20 Sep 2023 15:10:47 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 20 Sep 2023 15:10:47 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 20 Sep 2023 15:10:47 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 20 Sep 2023 15:10:47 GMT
USER adminer
# Wed, 20 Sep 2023 15:10:47 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 20 Sep 2023 15:10:47 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:00121bf241b18e981bcc804f905be7b34f95cce415db622599e21dc1a496ee8d`  
		Last Modified: Wed, 20 Sep 2023 00:47:11 GMT  
		Size: 56.0 MB (56040498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:964fa70975aa8c3eb5838cf9120935712a93ec197f9adce227a0d97a7df9d131`  
		Last Modified: Wed, 20 Sep 2023 15:11:38 GMT  
		Size: 39.6 MB (39559141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cf7eb9be8cf86ff0edfb0e7026187487f60c1b234c068e76b9d90c4bb2e56b5`  
		Last Modified: Wed, 20 Sep 2023 15:11:27 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7986b40b588b21caefc32e63e9bf4259713bd637125de9f9e6c415339b62bdb8`  
		Last Modified: Wed, 20 Sep 2023 15:11:27 GMT  
		Size: 1.9 KB (1869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da42b96b0425edc1796b564789c33a81ba8cc1bd8e95886fb24cba7bf6e830f9`  
		Last Modified: Wed, 20 Sep 2023 15:11:27 GMT  
		Size: 1.5 KB (1481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cb8907e77be88986e418354768b790c2a227d56ea26b7a7cdb7027c2958aa71`  
		Last Modified: Wed, 20 Sep 2023 15:11:27 GMT  
		Size: 1.4 MB (1385349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9fdcba82893748b7e9f6211dc3cd3248fa29ee6f78a24482d34339bb1fd857f`  
		Last Modified: Wed, 20 Sep 2023 15:11:27 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1-standalone` - linux; mips64le

```console
$ docker pull adminer@sha256:ec803d54e73e17da91a36b9ce59b261f4f312dacabb7e0556302bce0443f75b7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.6 MB (92612531 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:215cf7d1502bb244df43b52290a34650eafce425c56c967b8c9e153a5ada9557`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Wed, 20 Sep 2023 06:40:19 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 20 Sep 2023 06:40:22 GMT
WORKDIR /var/www/html
# Wed, 20 Sep 2023 06:40:25 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 20 Sep 2023 06:40:28 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 20 Sep 2023 06:40:32 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 20 Sep 2023 06:40:35 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 20 Sep 2023 06:41:26 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 20 Sep 2023 06:41:29 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 20 Sep 2023 06:41:32 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 20 Sep 2023 06:41:35 GMT
USER adminer
# Wed, 20 Sep 2023 06:41:39 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 20 Sep 2023 06:41:42 GMT
EXPOSE 8080
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
	-	`sha256:4f0fa2061f2328806a3e6442dc58a5750d76966e9542efd972a12fd49f53cd69`  
		Last Modified: Wed, 20 Sep 2023 06:43:50 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04163c23cec6352cfd6ce393d04f5900400ea72c83d04af1552865c916a1c459`  
		Last Modified: Wed, 20 Sep 2023 06:43:50 GMT  
		Size: 1.5 KB (1481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d726d9d0dfbf6bba7fc6b01578c0a26c84fafdbe71a4e69674dfd1284ce0826`  
		Last Modified: Wed, 20 Sep 2023 06:43:51 GMT  
		Size: 1.4 MB (1386315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e96e2db0e4c5751ce57381cb92f2f2fff089adb321644959f5de599a271ebedc`  
		Last Modified: Wed, 20 Sep 2023 06:43:50 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1-standalone` - linux; ppc64le

```console
$ docker pull adminer@sha256:e0809520a8bd4f91b86c0bfd4a871ce4707fd119706f564057dffe5e7c91f5fe
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.3 MB (101262041 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ad347a3c52aeda1176962cc50fcedfab4a87a129219de1394700476d688d49e`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 20 Sep 2023 07:53:09 GMT
ADD file:c12b11abfba27478510c84d05abdd8fec539db9ec30af6d042671f4d5bf793e5 in / 
# Wed, 20 Sep 2023 07:53:12 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 10:27:30 GMT
STOPSIGNAL SIGINT
# Wed, 20 Sep 2023 10:28:24 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 10:28:27 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 20 Sep 2023 10:28:28 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 20 Sep 2023 10:28:28 GMT
WORKDIR /var/www/html
# Wed, 20 Sep 2023 10:28:29 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 20 Sep 2023 10:28:29 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 20 Sep 2023 10:28:30 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 20 Sep 2023 10:28:30 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 20 Sep 2023 10:28:54 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 20 Sep 2023 10:28:54 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 20 Sep 2023 10:28:55 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 20 Sep 2023 10:28:55 GMT
USER adminer
# Wed, 20 Sep 2023 10:28:55 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 20 Sep 2023 10:28:55 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:9f3507d882ae95f06b3672497cdd3317bd4f8e0255e73d10f1f263e5d780f102`  
		Last Modified: Wed, 20 Sep 2023 08:50:16 GMT  
		Size: 58.9 MB (58928499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dc55ae4eee76ca2700dbf8d4554951df837121cc96140f29cbcc2d7308b4d72`  
		Last Modified: Wed, 20 Sep 2023 10:29:59 GMT  
		Size: 40.9 MB (40943739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:413bf430ecd0a8d3a68dc7841be8802fccca3af99645087fbb82e476cd335965`  
		Last Modified: Wed, 20 Sep 2023 10:29:47 GMT  
		Size: 396.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df2720d6c627570256eb0bc8943ba052f2b617c5dd972a3eb74196fc91a3dbbb`  
		Last Modified: Wed, 20 Sep 2023 10:29:47 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b6b255e136e7ac31afc340c04be397be6d98a39da922310d73ffbfff9687a2a`  
		Last Modified: Wed, 20 Sep 2023 10:29:47 GMT  
		Size: 1.5 KB (1481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36bfcc7e4826d80f455356e3a88eb31b2e5c559a49a733a25490d6becb652045`  
		Last Modified: Wed, 20 Sep 2023 10:29:47 GMT  
		Size: 1.4 MB (1385554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36a5f297e715a97e0af1984e9f7dd3cb60fa2226b31fc95bbfb6a3c5d85549af`  
		Last Modified: Wed, 20 Sep 2023 10:29:47 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1-standalone` - linux; s390x

```console
$ docker pull adminer@sha256:120087fff0a708c70334e38726cab4a7703516787b7d901b1adc69fde470d694
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.7 MB (93701227 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42031d8d4365bb267d464fac6d7ab8b6e0ad4b097eb47e3e4b2dd8d14b64371d`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Wed, 20 Sep 2023 09:42:33 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 20 Sep 2023 09:42:33 GMT
WORKDIR /var/www/html
# Wed, 20 Sep 2023 09:42:33 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 20 Sep 2023 09:42:34 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 20 Sep 2023 09:42:34 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 20 Sep 2023 09:42:34 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 20 Sep 2023 09:42:57 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 20 Sep 2023 09:42:58 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 20 Sep 2023 09:42:58 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 20 Sep 2023 09:42:59 GMT
USER adminer
# Wed, 20 Sep 2023 09:42:59 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 20 Sep 2023 09:43:00 GMT
EXPOSE 8080
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
	-	`sha256:a0dfeb4132e2fe11e348c94294b33e51684a77419be87fae2d715412dc40e9c1`  
		Last Modified: Wed, 20 Sep 2023 09:43:57 GMT  
		Size: 1.9 KB (1883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:800a5df8795fcb07b6a7efb2135a2a662b31533cd779cc532445e86eae286b9f`  
		Last Modified: Wed, 20 Sep 2023 09:43:57 GMT  
		Size: 1.5 KB (1481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:321185c09a4e5d7e9a145855613f743ef531836df1355ae7593208920ad68541`  
		Last Modified: Wed, 20 Sep 2023 09:43:58 GMT  
		Size: 1.4 MB (1385674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c30b98bdcd0d0b081524334dc05d7905ceb45b6e8230e8156267e4759d587a2c`  
		Last Modified: Wed, 20 Sep 2023 09:43:57 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `adminer:fastcgi`

```console
$ docker pull adminer@sha256:b1eb6b4fef1cbe8aae2448f5ff246547904ddde8353382e40fd999fa7cd90047
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

### `adminer:fastcgi` - linux; arm variant v5

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

### `adminer:fastcgi` - linux; arm variant v7

```console
$ docker pull adminer@sha256:542098b1184f641c16a22b9b0d3a814b99a7bffca9593133e604d06e76cfb2f8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.8 MB (87798559 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7fe9e2628383acfd8d7c700d2a4881cfe1815fbee052c129294f79bce56e1b5`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Wed, 20 Sep 2023 04:57:26 GMT
ADD file:3bf3380482840b3a4166e82c3f951812076851ba1527261fdd1da780662b2de1 in / 
# Wed, 20 Sep 2023 04:57:26 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 15:43:10 GMT
STOPSIGNAL SIGINT
# Wed, 20 Sep 2023 15:43:35 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 15:43:36 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 20 Sep 2023 15:43:59 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Wed, 20 Sep 2023 15:44:00 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 20 Sep 2023 15:44:00 GMT
WORKDIR /var/www/html
# Wed, 20 Sep 2023 15:44:00 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 20 Sep 2023 15:44:00 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 20 Sep 2023 15:44:00 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 20 Sep 2023 15:44:00 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 20 Sep 2023 15:44:11 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 20 Sep 2023 15:44:11 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 20 Sep 2023 15:44:12 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 20 Sep 2023 15:44:12 GMT
USER adminer
# Wed, 20 Sep 2023 15:44:12 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:1d4e041d2204b383d6d6893cfcf5b852394f34744a85cea9ec0b3fb65cbc6143`  
		Last Modified: Wed, 20 Sep 2023 05:01:34 GMT  
		Size: 50.2 MB (50219551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4ca4acdacd0b759547187250427f6845ca2fc092c757b2e2f6667b1add9ba8d`  
		Last Modified: Wed, 20 Sep 2023 15:44:32 GMT  
		Size: 36.2 MB (36186615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc8798178b90f7264865be9cbfe742803f21777526c5ba6c86e1526c78998f64`  
		Last Modified: Wed, 20 Sep 2023 15:44:23 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3364c0b2504d3af9b0175a6e77522d257e70f24251cfd629dd6bd3ef24b5f119`  
		Last Modified: Wed, 20 Sep 2023 15:44:49 GMT  
		Size: 2.7 KB (2713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62a19c34bb68631c5d5858d4245052d13f760c8cf841e4a4cd1f02343aed2d5f`  
		Last Modified: Wed, 20 Sep 2023 15:44:49 GMT  
		Size: 1.9 KB (1869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08676442b17b4a0cc0ffff5e52fe487a0107e28a668edfdff6ad54606481fb05`  
		Last Modified: Wed, 20 Sep 2023 15:44:49 GMT  
		Size: 1.5 KB (1480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82515cdefa5e1215ed49066547b07fa57d1b9da8fabd0522836ba51ad7e9ab82`  
		Last Modified: Wed, 20 Sep 2023 15:44:49 GMT  
		Size: 1.4 MB (1385449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cf0ebb373156a781676a77242c49b21185c9e025e5104d6b83fec00a1a77b78`  
		Last Modified: Wed, 20 Sep 2023 15:44:49 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:fastcgi` - linux; arm64 variant v8

```console
$ docker pull adminer@sha256:1cff0be1992c13ea25123e8139fc1179c0f722357c1f54f6be3a143db8a52899
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.3 MB (94341405 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ce755452b4733c8b45e4d8e12c142771d8fd25391360bfaff9353b77d3a7296`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Wed, 20 Sep 2023 02:44:20 GMT
ADD file:46dcdcde338d2c01fed5db3fac9041736d9305145d8fc2039dd5b3714d38ede8 in / 
# Wed, 20 Sep 2023 02:44:21 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 18:04:43 GMT
STOPSIGNAL SIGINT
# Wed, 20 Sep 2023 18:05:03 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 18:05:04 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 20 Sep 2023 18:05:23 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Wed, 20 Sep 2023 18:05:23 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 20 Sep 2023 18:05:23 GMT
WORKDIR /var/www/html
# Wed, 20 Sep 2023 18:05:24 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 20 Sep 2023 18:05:24 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 20 Sep 2023 18:05:24 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 20 Sep 2023 18:05:24 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 20 Sep 2023 18:05:34 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 20 Sep 2023 18:05:34 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 20 Sep 2023 18:05:34 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 20 Sep 2023 18:05:35 GMT
USER adminer
# Wed, 20 Sep 2023 18:05:35 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:31f5dc1f52c865588c43d8ec718f14d430e149b28f0b28232da825da7ae28f76`  
		Last Modified: Wed, 20 Sep 2023 02:47:53 GMT  
		Size: 53.7 MB (53704892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c82c17c7529e7d3125d9a7f12b8359fac7e9cc29dbb6555d30cbe9bdda203722`  
		Last Modified: Wed, 20 Sep 2023 18:05:50 GMT  
		Size: 39.2 MB (39244274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27290e9432136a39923f648bd1220a36cdd54a4f8baacd87b500eed4d5018d2a`  
		Last Modified: Wed, 20 Sep 2023 18:05:44 GMT  
		Size: 393.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4d0cfb12b1cdc502f0839f004aa983a25ea38bb788e0b734aa01a54303ae0e2`  
		Last Modified: Wed, 20 Sep 2023 18:06:08 GMT  
		Size: 2.7 KB (2711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76b68d0109bf502fae5cb6a017bbb0e37d31131dc631b3ae9ce75b6603690194`  
		Last Modified: Wed, 20 Sep 2023 18:06:08 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4abe36926b3c359fc35e36926f70d35534faf595ccb23765fd12a141f764e821`  
		Last Modified: Wed, 20 Sep 2023 18:06:08 GMT  
		Size: 1.5 KB (1478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42b5d424d36cd52afb1439ff8165fbc761f2319ec3e4e891eadb0f03a089199b`  
		Last Modified: Wed, 20 Sep 2023 18:06:08 GMT  
		Size: 1.4 MB (1385285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a545cd65be7574c61d9c4d38924911eeffdabb28d5d74e8198afda6043e8579`  
		Last Modified: Wed, 20 Sep 2023 18:06:08 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:fastcgi` - linux; 386

```console
$ docker pull adminer@sha256:846388f4f74cf512bb64bf84c6b64a14c87e97c2082957de704afb301f49a8f3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.0 MB (96991935 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d51e9267cebf41d916c5538d54fa90a930c77844a72ea2d84572bf9b9c7feba`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Wed, 20 Sep 2023 00:42:07 GMT
ADD file:342c36522089238a534c0912491a4cf64b89133969e051cdad2e694ec761142c in / 
# Wed, 20 Sep 2023 00:42:07 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 15:10:00 GMT
STOPSIGNAL SIGINT
# Wed, 20 Sep 2023 15:10:29 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 15:10:30 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 20 Sep 2023 15:10:58 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Wed, 20 Sep 2023 15:10:59 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 20 Sep 2023 15:10:59 GMT
WORKDIR /var/www/html
# Wed, 20 Sep 2023 15:10:59 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 20 Sep 2023 15:10:59 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 20 Sep 2023 15:10:59 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 20 Sep 2023 15:10:59 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 20 Sep 2023 15:11:15 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 20 Sep 2023 15:11:15 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 20 Sep 2023 15:11:15 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 20 Sep 2023 15:11:15 GMT
USER adminer
# Wed, 20 Sep 2023 15:11:15 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:00121bf241b18e981bcc804f905be7b34f95cce415db622599e21dc1a496ee8d`  
		Last Modified: Wed, 20 Sep 2023 00:47:11 GMT  
		Size: 56.0 MB (56040498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:964fa70975aa8c3eb5838cf9120935712a93ec197f9adce227a0d97a7df9d131`  
		Last Modified: Wed, 20 Sep 2023 15:11:38 GMT  
		Size: 39.6 MB (39559141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cf7eb9be8cf86ff0edfb0e7026187487f60c1b234c068e76b9d90c4bb2e56b5`  
		Last Modified: Wed, 20 Sep 2023 15:11:27 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14739144aeefcf6bb5b82efb1be6c8c36061cb79988c3d04e94ac3af2889703d`  
		Last Modified: Wed, 20 Sep 2023 15:11:57 GMT  
		Size: 2.7 KB (2707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be431c45e4957603c8fc57e2e1c75ca225cf90bdaee782e22140bd61fb848bd2`  
		Last Modified: Wed, 20 Sep 2023 15:11:58 GMT  
		Size: 1.9 KB (1870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af4bb02c3c060fffe6e6033ae734961cbe056f312fe14b88a19af87c4f244f12`  
		Last Modified: Wed, 20 Sep 2023 15:11:57 GMT  
		Size: 1.5 KB (1472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ed951e5e4331a40e2299fe20b587b7ac277d2561486420e3f603a26eaf55c7f`  
		Last Modified: Wed, 20 Sep 2023 15:11:57 GMT  
		Size: 1.4 MB (1385367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e84da2513a7218dd7201673bcd22e26b222c95847fcf06c9b8a7151d89c1b1f0`  
		Last Modified: Wed, 20 Sep 2023 15:11:56 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:fastcgi` - linux; mips64le

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

### `adminer:fastcgi` - linux; ppc64le

```console
$ docker pull adminer@sha256:79299ee4e64a10ed155d4b0e07c0b513251f6730c593768c6e3ed11269d0b296
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.3 MB (101264733 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc0562129b0dc47471215a72b69dc9de21102422b16b11725a10b19d56f6b30c`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Wed, 20 Sep 2023 07:53:09 GMT
ADD file:c12b11abfba27478510c84d05abdd8fec539db9ec30af6d042671f4d5bf793e5 in / 
# Wed, 20 Sep 2023 07:53:12 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 10:27:30 GMT
STOPSIGNAL SIGINT
# Wed, 20 Sep 2023 10:28:24 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 10:28:27 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 20 Sep 2023 10:29:10 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Wed, 20 Sep 2023 10:29:11 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 20 Sep 2023 10:29:11 GMT
WORKDIR /var/www/html
# Wed, 20 Sep 2023 10:29:11 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 20 Sep 2023 10:29:12 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 20 Sep 2023 10:29:12 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 20 Sep 2023 10:29:12 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 20 Sep 2023 10:29:34 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 20 Sep 2023 10:29:34 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 20 Sep 2023 10:29:34 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 20 Sep 2023 10:29:35 GMT
USER adminer
# Wed, 20 Sep 2023 10:29:35 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:9f3507d882ae95f06b3672497cdd3317bd4f8e0255e73d10f1f263e5d780f102`  
		Last Modified: Wed, 20 Sep 2023 08:50:16 GMT  
		Size: 58.9 MB (58928499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dc55ae4eee76ca2700dbf8d4554951df837121cc96140f29cbcc2d7308b4d72`  
		Last Modified: Wed, 20 Sep 2023 10:29:59 GMT  
		Size: 40.9 MB (40943739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:413bf430ecd0a8d3a68dc7841be8802fccca3af99645087fbb82e476cd335965`  
		Last Modified: Wed, 20 Sep 2023 10:29:47 GMT  
		Size: 396.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33c90f4bc93f05165b4c2a576055f2d0614e44beb75f656246a36dab518a167e`  
		Last Modified: Wed, 20 Sep 2023 10:30:20 GMT  
		Size: 2.7 KB (2712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8042ccb66d3f41a43740fe4d53cf23c908f55c921ebbdd7f85a713640e21b71`  
		Last Modified: Wed, 20 Sep 2023 10:30:20 GMT  
		Size: 1.9 KB (1877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9687767d889f697b2273a34c6066aa7a3319201ef0abe10a52e58cd6192f18e0`  
		Last Modified: Wed, 20 Sep 2023 10:30:20 GMT  
		Size: 1.5 KB (1480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:373f9256ef78f4c4f1ce5dcac32e6c33dc0c75c189e9d0fe44e89efc9ad1e68e`  
		Last Modified: Wed, 20 Sep 2023 10:30:21 GMT  
		Size: 1.4 MB (1385537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f063a3c5af7dc109b9e33bbf3c86fea2b892e631c1128300364996aa081e72d`  
		Last Modified: Wed, 20 Sep 2023 10:30:20 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:fastcgi` - linux; s390x

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

## `adminer:latest`

```console
$ docker pull adminer@sha256:40c1d6691703a8ca102dc108c4a6fc11863e928b6ae6014fb8557b6e083a29ff
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

### `adminer:latest` - linux; amd64

```console
$ docker pull adminer@sha256:7fb4cb76b1a979671c18bba6ad81fc80d50cb56069b7fb542f75efb921b5e714
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.9 MB (95937427 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b672f480fc7a76f4b04207143a6b693b2a6eec24ac981709e626b16505609fd`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Wed, 20 Sep 2023 07:12:40 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 20 Sep 2023 07:12:40 GMT
WORKDIR /var/www/html
# Wed, 20 Sep 2023 07:12:41 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 20 Sep 2023 07:12:41 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 20 Sep 2023 07:12:41 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 20 Sep 2023 07:12:41 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 20 Sep 2023 07:12:53 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 20 Sep 2023 07:12:53 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 20 Sep 2023 07:12:53 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 20 Sep 2023 07:12:53 GMT
USER adminer
# Wed, 20 Sep 2023 07:12:53 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 20 Sep 2023 07:12:53 GMT
EXPOSE 8080
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
	-	`sha256:eb4bd38d1031bd7c467d8bce4c95f0b7697c26030cc73874381860ce97d0cdcd`  
		Last Modified: Wed, 20 Sep 2023 07:13:25 GMT  
		Size: 1.9 KB (1880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3bc33b7b683bc4196fbd1738ad588e8334ddb171c5d50c48429546f10cb487a`  
		Last Modified: Wed, 20 Sep 2023 07:13:25 GMT  
		Size: 1.5 KB (1477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d61d710f98a6cd583cbb61f1ace245ab27b2b69e7e606afdff85fe75a17f685`  
		Last Modified: Wed, 20 Sep 2023 07:13:26 GMT  
		Size: 1.4 MB (1385429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8441003ca946127323e284e8685841d9e549a658468e76be7cf68a2b08203f3`  
		Last Modified: Wed, 20 Sep 2023 07:13:25 GMT  
		Size: 488.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:latest` - linux; arm variant v5

```console
$ docker pull adminer@sha256:fc1ddb9f0a1b7781c7281f79851e7141b11e10f5cc915355b6cf6ff7824ede94
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.2 MB (91195621 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f410041bfb5c56158771bc68b88310247a497e74186a3dfdb22358729c1fd47e`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Wed, 20 Sep 2023 09:37:05 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 20 Sep 2023 09:37:05 GMT
WORKDIR /var/www/html
# Wed, 20 Sep 2023 09:37:05 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 20 Sep 2023 09:37:05 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 20 Sep 2023 09:37:05 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 20 Sep 2023 09:37:05 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 20 Sep 2023 09:37:21 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 20 Sep 2023 09:37:21 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 20 Sep 2023 09:37:21 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 20 Sep 2023 09:37:21 GMT
USER adminer
# Wed, 20 Sep 2023 09:37:21 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 20 Sep 2023 09:37:21 GMT
EXPOSE 8080
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
	-	`sha256:1cba35ed39d8d7c05cb37696f20ecdc7fde0f2d7fcbe968f50892aaabfdd84f2`  
		Last Modified: Wed, 20 Sep 2023 09:37:57 GMT  
		Size: 1.9 KB (1871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df6f0945f3469cf4fdd867a2409be0fc2b79d33a4267fb743edb64842be147f3`  
		Last Modified: Wed, 20 Sep 2023 09:37:57 GMT  
		Size: 1.5 KB (1476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb77accf421b5a1954871ae06a2ed8550b59f6ea59dfc1773263a25757e67757`  
		Last Modified: Wed, 20 Sep 2023 09:37:58 GMT  
		Size: 1.4 MB (1385374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1004d2eab86228b351246a3406fff91074ab91bf1c83691d49831a343972504f`  
		Last Modified: Wed, 20 Sep 2023 09:37:57 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:latest` - linux; arm variant v7

```console
$ docker pull adminer@sha256:d8a19218a54fe4fb52cb32cfc4d0ba0207b2976a94106cc4587ae23ef2796f6a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.8 MB (87795777 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2953870e043e0f3e517f17cce5c6d2e2d06f74d372de15043ba3193f11862b48`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 20 Sep 2023 04:57:26 GMT
ADD file:3bf3380482840b3a4166e82c3f951812076851ba1527261fdd1da780662b2de1 in / 
# Wed, 20 Sep 2023 04:57:26 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 15:43:10 GMT
STOPSIGNAL SIGINT
# Wed, 20 Sep 2023 15:43:35 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 15:43:36 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 20 Sep 2023 15:43:37 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 20 Sep 2023 15:43:37 GMT
WORKDIR /var/www/html
# Wed, 20 Sep 2023 15:43:37 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 20 Sep 2023 15:43:37 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 20 Sep 2023 15:43:37 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 20 Sep 2023 15:43:37 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 20 Sep 2023 15:43:50 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 20 Sep 2023 15:43:50 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 20 Sep 2023 15:43:50 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 20 Sep 2023 15:43:50 GMT
USER adminer
# Wed, 20 Sep 2023 15:43:50 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 20 Sep 2023 15:43:50 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:1d4e041d2204b383d6d6893cfcf5b852394f34744a85cea9ec0b3fb65cbc6143`  
		Last Modified: Wed, 20 Sep 2023 05:01:34 GMT  
		Size: 50.2 MB (50219551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4ca4acdacd0b759547187250427f6845ca2fc092c757b2e2f6667b1add9ba8d`  
		Last Modified: Wed, 20 Sep 2023 15:44:32 GMT  
		Size: 36.2 MB (36186615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc8798178b90f7264865be9cbfe742803f21777526c5ba6c86e1526c78998f64`  
		Last Modified: Wed, 20 Sep 2023 15:44:23 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e44ef76b17f1c1b9f8fa8b3c28b236740ee52ee91c0bf1a5967949aa44b1d46`  
		Last Modified: Wed, 20 Sep 2023 15:44:23 GMT  
		Size: 1.9 KB (1871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02874a9e593b60862b1fa6079ec21abf9b108ff79ed1afb0fea2f5fb92c31bc0`  
		Last Modified: Wed, 20 Sep 2023 15:44:23 GMT  
		Size: 1.5 KB (1478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92715c2cab25dd578e4272162c7e32c5e783506711541b3e2cd6a0dd12e62fcf`  
		Last Modified: Wed, 20 Sep 2023 15:44:23 GMT  
		Size: 1.4 MB (1385383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6187ee8021740cf1e9d2e67c8904adc77f0ed4503d7f9ada0dec4b5537eaa35f`  
		Last Modified: Wed, 20 Sep 2023 15:44:23 GMT  
		Size: 489.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:latest` - linux; arm64 variant v8

```console
$ docker pull adminer@sha256:82f1435981ebaa969cfd9cb3f452c46655dcf1715947a90a8c64dd3284db36d3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.3 MB (94338726 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51817ad17de2ccc468c81b03aa1f7c122e2d802f5411b384d4b8d341c711b3ff`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 20 Sep 2023 02:44:20 GMT
ADD file:46dcdcde338d2c01fed5db3fac9041736d9305145d8fc2039dd5b3714d38ede8 in / 
# Wed, 20 Sep 2023 02:44:21 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 18:04:43 GMT
STOPSIGNAL SIGINT
# Wed, 20 Sep 2023 18:05:03 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 18:05:04 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 20 Sep 2023 18:05:05 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 20 Sep 2023 18:05:05 GMT
WORKDIR /var/www/html
# Wed, 20 Sep 2023 18:05:05 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 20 Sep 2023 18:05:05 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 20 Sep 2023 18:05:05 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 20 Sep 2023 18:05:05 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 20 Sep 2023 18:05:16 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 20 Sep 2023 18:05:16 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 20 Sep 2023 18:05:16 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 20 Sep 2023 18:05:16 GMT
USER adminer
# Wed, 20 Sep 2023 18:05:16 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 20 Sep 2023 18:05:16 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:31f5dc1f52c865588c43d8ec718f14d430e149b28f0b28232da825da7ae28f76`  
		Last Modified: Wed, 20 Sep 2023 02:47:53 GMT  
		Size: 53.7 MB (53704892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c82c17c7529e7d3125d9a7f12b8359fac7e9cc29dbb6555d30cbe9bdda203722`  
		Last Modified: Wed, 20 Sep 2023 18:05:50 GMT  
		Size: 39.2 MB (39244274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27290e9432136a39923f648bd1220a36cdd54a4f8baacd87b500eed4d5018d2a`  
		Last Modified: Wed, 20 Sep 2023 18:05:44 GMT  
		Size: 393.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0029f07058cb36f9b27d218954d9e733b152fe47d9875b8d062632100f585d58`  
		Last Modified: Wed, 20 Sep 2023 18:05:44 GMT  
		Size: 1.9 KB (1883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f9ca9fda73283aac009ee0add3e063260cc5c09a89cbdaddef5d3e623c8ae3f`  
		Last Modified: Wed, 20 Sep 2023 18:05:44 GMT  
		Size: 1.5 KB (1477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99dc3e204c8096f4463277e628be5a5860db3a123dd45a87f99df2b8d1d76f77`  
		Last Modified: Wed, 20 Sep 2023 18:05:44 GMT  
		Size: 1.4 MB (1385317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5dbe53bc88443a7def3aa5bed48f19d4bc849da97d88790bf9701396443acac`  
		Last Modified: Wed, 20 Sep 2023 18:05:44 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:latest` - linux; 386

```console
$ docker pull adminer@sha256:24a953b70c62fedfe7da2846b84d0a3133b442f0721e17fbf5df2d222ae440f8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.0 MB (96989218 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0cbe365ed04581b1b00d6390c52f9260afab49677042b95a947b6ca499d98bdc`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 20 Sep 2023 00:42:07 GMT
ADD file:342c36522089238a534c0912491a4cf64b89133969e051cdad2e694ec761142c in / 
# Wed, 20 Sep 2023 00:42:07 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 15:10:00 GMT
STOPSIGNAL SIGINT
# Wed, 20 Sep 2023 15:10:29 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 15:10:30 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 20 Sep 2023 15:10:31 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 20 Sep 2023 15:10:31 GMT
WORKDIR /var/www/html
# Wed, 20 Sep 2023 15:10:31 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 20 Sep 2023 15:10:31 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 20 Sep 2023 15:10:31 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 20 Sep 2023 15:10:31 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 20 Sep 2023 15:10:47 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 20 Sep 2023 15:10:47 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 20 Sep 2023 15:10:47 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 20 Sep 2023 15:10:47 GMT
USER adminer
# Wed, 20 Sep 2023 15:10:47 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 20 Sep 2023 15:10:47 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:00121bf241b18e981bcc804f905be7b34f95cce415db622599e21dc1a496ee8d`  
		Last Modified: Wed, 20 Sep 2023 00:47:11 GMT  
		Size: 56.0 MB (56040498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:964fa70975aa8c3eb5838cf9120935712a93ec197f9adce227a0d97a7df9d131`  
		Last Modified: Wed, 20 Sep 2023 15:11:38 GMT  
		Size: 39.6 MB (39559141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cf7eb9be8cf86ff0edfb0e7026187487f60c1b234c068e76b9d90c4bb2e56b5`  
		Last Modified: Wed, 20 Sep 2023 15:11:27 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7986b40b588b21caefc32e63e9bf4259713bd637125de9f9e6c415339b62bdb8`  
		Last Modified: Wed, 20 Sep 2023 15:11:27 GMT  
		Size: 1.9 KB (1869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da42b96b0425edc1796b564789c33a81ba8cc1bd8e95886fb24cba7bf6e830f9`  
		Last Modified: Wed, 20 Sep 2023 15:11:27 GMT  
		Size: 1.5 KB (1481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cb8907e77be88986e418354768b790c2a227d56ea26b7a7cdb7027c2958aa71`  
		Last Modified: Wed, 20 Sep 2023 15:11:27 GMT  
		Size: 1.4 MB (1385349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9fdcba82893748b7e9f6211dc3cd3248fa29ee6f78a24482d34339bb1fd857f`  
		Last Modified: Wed, 20 Sep 2023 15:11:27 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:latest` - linux; mips64le

```console
$ docker pull adminer@sha256:ec803d54e73e17da91a36b9ce59b261f4f312dacabb7e0556302bce0443f75b7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.6 MB (92612531 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:215cf7d1502bb244df43b52290a34650eafce425c56c967b8c9e153a5ada9557`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Wed, 20 Sep 2023 06:40:19 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 20 Sep 2023 06:40:22 GMT
WORKDIR /var/www/html
# Wed, 20 Sep 2023 06:40:25 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 20 Sep 2023 06:40:28 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 20 Sep 2023 06:40:32 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 20 Sep 2023 06:40:35 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 20 Sep 2023 06:41:26 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 20 Sep 2023 06:41:29 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 20 Sep 2023 06:41:32 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 20 Sep 2023 06:41:35 GMT
USER adminer
# Wed, 20 Sep 2023 06:41:39 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 20 Sep 2023 06:41:42 GMT
EXPOSE 8080
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
	-	`sha256:4f0fa2061f2328806a3e6442dc58a5750d76966e9542efd972a12fd49f53cd69`  
		Last Modified: Wed, 20 Sep 2023 06:43:50 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04163c23cec6352cfd6ce393d04f5900400ea72c83d04af1552865c916a1c459`  
		Last Modified: Wed, 20 Sep 2023 06:43:50 GMT  
		Size: 1.5 KB (1481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d726d9d0dfbf6bba7fc6b01578c0a26c84fafdbe71a4e69674dfd1284ce0826`  
		Last Modified: Wed, 20 Sep 2023 06:43:51 GMT  
		Size: 1.4 MB (1386315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e96e2db0e4c5751ce57381cb92f2f2fff089adb321644959f5de599a271ebedc`  
		Last Modified: Wed, 20 Sep 2023 06:43:50 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:latest` - linux; ppc64le

```console
$ docker pull adminer@sha256:e0809520a8bd4f91b86c0bfd4a871ce4707fd119706f564057dffe5e7c91f5fe
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.3 MB (101262041 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ad347a3c52aeda1176962cc50fcedfab4a87a129219de1394700476d688d49e`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 20 Sep 2023 07:53:09 GMT
ADD file:c12b11abfba27478510c84d05abdd8fec539db9ec30af6d042671f4d5bf793e5 in / 
# Wed, 20 Sep 2023 07:53:12 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 10:27:30 GMT
STOPSIGNAL SIGINT
# Wed, 20 Sep 2023 10:28:24 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 10:28:27 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 20 Sep 2023 10:28:28 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 20 Sep 2023 10:28:28 GMT
WORKDIR /var/www/html
# Wed, 20 Sep 2023 10:28:29 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 20 Sep 2023 10:28:29 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 20 Sep 2023 10:28:30 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 20 Sep 2023 10:28:30 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 20 Sep 2023 10:28:54 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 20 Sep 2023 10:28:54 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 20 Sep 2023 10:28:55 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 20 Sep 2023 10:28:55 GMT
USER adminer
# Wed, 20 Sep 2023 10:28:55 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 20 Sep 2023 10:28:55 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:9f3507d882ae95f06b3672497cdd3317bd4f8e0255e73d10f1f263e5d780f102`  
		Last Modified: Wed, 20 Sep 2023 08:50:16 GMT  
		Size: 58.9 MB (58928499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dc55ae4eee76ca2700dbf8d4554951df837121cc96140f29cbcc2d7308b4d72`  
		Last Modified: Wed, 20 Sep 2023 10:29:59 GMT  
		Size: 40.9 MB (40943739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:413bf430ecd0a8d3a68dc7841be8802fccca3af99645087fbb82e476cd335965`  
		Last Modified: Wed, 20 Sep 2023 10:29:47 GMT  
		Size: 396.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df2720d6c627570256eb0bc8943ba052f2b617c5dd972a3eb74196fc91a3dbbb`  
		Last Modified: Wed, 20 Sep 2023 10:29:47 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b6b255e136e7ac31afc340c04be397be6d98a39da922310d73ffbfff9687a2a`  
		Last Modified: Wed, 20 Sep 2023 10:29:47 GMT  
		Size: 1.5 KB (1481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36bfcc7e4826d80f455356e3a88eb31b2e5c559a49a733a25490d6becb652045`  
		Last Modified: Wed, 20 Sep 2023 10:29:47 GMT  
		Size: 1.4 MB (1385554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36a5f297e715a97e0af1984e9f7dd3cb60fa2226b31fc95bbfb6a3c5d85549af`  
		Last Modified: Wed, 20 Sep 2023 10:29:47 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:latest` - linux; s390x

```console
$ docker pull adminer@sha256:120087fff0a708c70334e38726cab4a7703516787b7d901b1adc69fde470d694
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.7 MB (93701227 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42031d8d4365bb267d464fac6d7ab8b6e0ad4b097eb47e3e4b2dd8d14b64371d`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Wed, 20 Sep 2023 09:42:33 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 20 Sep 2023 09:42:33 GMT
WORKDIR /var/www/html
# Wed, 20 Sep 2023 09:42:33 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 20 Sep 2023 09:42:34 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 20 Sep 2023 09:42:34 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 20 Sep 2023 09:42:34 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 20 Sep 2023 09:42:57 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 20 Sep 2023 09:42:58 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 20 Sep 2023 09:42:58 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 20 Sep 2023 09:42:59 GMT
USER adminer
# Wed, 20 Sep 2023 09:42:59 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 20 Sep 2023 09:43:00 GMT
EXPOSE 8080
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
	-	`sha256:a0dfeb4132e2fe11e348c94294b33e51684a77419be87fae2d715412dc40e9c1`  
		Last Modified: Wed, 20 Sep 2023 09:43:57 GMT  
		Size: 1.9 KB (1883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:800a5df8795fcb07b6a7efb2135a2a662b31533cd779cc532445e86eae286b9f`  
		Last Modified: Wed, 20 Sep 2023 09:43:57 GMT  
		Size: 1.5 KB (1481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:321185c09a4e5d7e9a145855613f743ef531836df1355ae7593208920ad68541`  
		Last Modified: Wed, 20 Sep 2023 09:43:58 GMT  
		Size: 1.4 MB (1385674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c30b98bdcd0d0b081524334dc05d7905ceb45b6e8230e8156267e4759d587a2c`  
		Last Modified: Wed, 20 Sep 2023 09:43:57 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `adminer:standalone`

```console
$ docker pull adminer@sha256:40c1d6691703a8ca102dc108c4a6fc11863e928b6ae6014fb8557b6e083a29ff
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
$ docker pull adminer@sha256:7fb4cb76b1a979671c18bba6ad81fc80d50cb56069b7fb542f75efb921b5e714
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.9 MB (95937427 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b672f480fc7a76f4b04207143a6b693b2a6eec24ac981709e626b16505609fd`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Wed, 20 Sep 2023 07:12:40 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 20 Sep 2023 07:12:40 GMT
WORKDIR /var/www/html
# Wed, 20 Sep 2023 07:12:41 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 20 Sep 2023 07:12:41 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 20 Sep 2023 07:12:41 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 20 Sep 2023 07:12:41 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 20 Sep 2023 07:12:53 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 20 Sep 2023 07:12:53 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 20 Sep 2023 07:12:53 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 20 Sep 2023 07:12:53 GMT
USER adminer
# Wed, 20 Sep 2023 07:12:53 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 20 Sep 2023 07:12:53 GMT
EXPOSE 8080
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
	-	`sha256:eb4bd38d1031bd7c467d8bce4c95f0b7697c26030cc73874381860ce97d0cdcd`  
		Last Modified: Wed, 20 Sep 2023 07:13:25 GMT  
		Size: 1.9 KB (1880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3bc33b7b683bc4196fbd1738ad588e8334ddb171c5d50c48429546f10cb487a`  
		Last Modified: Wed, 20 Sep 2023 07:13:25 GMT  
		Size: 1.5 KB (1477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d61d710f98a6cd583cbb61f1ace245ab27b2b69e7e606afdff85fe75a17f685`  
		Last Modified: Wed, 20 Sep 2023 07:13:26 GMT  
		Size: 1.4 MB (1385429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8441003ca946127323e284e8685841d9e549a658468e76be7cf68a2b08203f3`  
		Last Modified: Wed, 20 Sep 2023 07:13:25 GMT  
		Size: 488.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:standalone` - linux; arm variant v5

```console
$ docker pull adminer@sha256:fc1ddb9f0a1b7781c7281f79851e7141b11e10f5cc915355b6cf6ff7824ede94
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.2 MB (91195621 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f410041bfb5c56158771bc68b88310247a497e74186a3dfdb22358729c1fd47e`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Wed, 20 Sep 2023 09:37:05 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 20 Sep 2023 09:37:05 GMT
WORKDIR /var/www/html
# Wed, 20 Sep 2023 09:37:05 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 20 Sep 2023 09:37:05 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 20 Sep 2023 09:37:05 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 20 Sep 2023 09:37:05 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 20 Sep 2023 09:37:21 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 20 Sep 2023 09:37:21 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 20 Sep 2023 09:37:21 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 20 Sep 2023 09:37:21 GMT
USER adminer
# Wed, 20 Sep 2023 09:37:21 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 20 Sep 2023 09:37:21 GMT
EXPOSE 8080
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
	-	`sha256:1cba35ed39d8d7c05cb37696f20ecdc7fde0f2d7fcbe968f50892aaabfdd84f2`  
		Last Modified: Wed, 20 Sep 2023 09:37:57 GMT  
		Size: 1.9 KB (1871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df6f0945f3469cf4fdd867a2409be0fc2b79d33a4267fb743edb64842be147f3`  
		Last Modified: Wed, 20 Sep 2023 09:37:57 GMT  
		Size: 1.5 KB (1476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb77accf421b5a1954871ae06a2ed8550b59f6ea59dfc1773263a25757e67757`  
		Last Modified: Wed, 20 Sep 2023 09:37:58 GMT  
		Size: 1.4 MB (1385374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1004d2eab86228b351246a3406fff91074ab91bf1c83691d49831a343972504f`  
		Last Modified: Wed, 20 Sep 2023 09:37:57 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:standalone` - linux; arm variant v7

```console
$ docker pull adminer@sha256:d8a19218a54fe4fb52cb32cfc4d0ba0207b2976a94106cc4587ae23ef2796f6a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.8 MB (87795777 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2953870e043e0f3e517f17cce5c6d2e2d06f74d372de15043ba3193f11862b48`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 20 Sep 2023 04:57:26 GMT
ADD file:3bf3380482840b3a4166e82c3f951812076851ba1527261fdd1da780662b2de1 in / 
# Wed, 20 Sep 2023 04:57:26 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 15:43:10 GMT
STOPSIGNAL SIGINT
# Wed, 20 Sep 2023 15:43:35 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 15:43:36 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 20 Sep 2023 15:43:37 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 20 Sep 2023 15:43:37 GMT
WORKDIR /var/www/html
# Wed, 20 Sep 2023 15:43:37 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 20 Sep 2023 15:43:37 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 20 Sep 2023 15:43:37 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 20 Sep 2023 15:43:37 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 20 Sep 2023 15:43:50 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 20 Sep 2023 15:43:50 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 20 Sep 2023 15:43:50 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 20 Sep 2023 15:43:50 GMT
USER adminer
# Wed, 20 Sep 2023 15:43:50 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 20 Sep 2023 15:43:50 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:1d4e041d2204b383d6d6893cfcf5b852394f34744a85cea9ec0b3fb65cbc6143`  
		Last Modified: Wed, 20 Sep 2023 05:01:34 GMT  
		Size: 50.2 MB (50219551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4ca4acdacd0b759547187250427f6845ca2fc092c757b2e2f6667b1add9ba8d`  
		Last Modified: Wed, 20 Sep 2023 15:44:32 GMT  
		Size: 36.2 MB (36186615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc8798178b90f7264865be9cbfe742803f21777526c5ba6c86e1526c78998f64`  
		Last Modified: Wed, 20 Sep 2023 15:44:23 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e44ef76b17f1c1b9f8fa8b3c28b236740ee52ee91c0bf1a5967949aa44b1d46`  
		Last Modified: Wed, 20 Sep 2023 15:44:23 GMT  
		Size: 1.9 KB (1871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02874a9e593b60862b1fa6079ec21abf9b108ff79ed1afb0fea2f5fb92c31bc0`  
		Last Modified: Wed, 20 Sep 2023 15:44:23 GMT  
		Size: 1.5 KB (1478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92715c2cab25dd578e4272162c7e32c5e783506711541b3e2cd6a0dd12e62fcf`  
		Last Modified: Wed, 20 Sep 2023 15:44:23 GMT  
		Size: 1.4 MB (1385383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6187ee8021740cf1e9d2e67c8904adc77f0ed4503d7f9ada0dec4b5537eaa35f`  
		Last Modified: Wed, 20 Sep 2023 15:44:23 GMT  
		Size: 489.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:standalone` - linux; arm64 variant v8

```console
$ docker pull adminer@sha256:82f1435981ebaa969cfd9cb3f452c46655dcf1715947a90a8c64dd3284db36d3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.3 MB (94338726 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51817ad17de2ccc468c81b03aa1f7c122e2d802f5411b384d4b8d341c711b3ff`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 20 Sep 2023 02:44:20 GMT
ADD file:46dcdcde338d2c01fed5db3fac9041736d9305145d8fc2039dd5b3714d38ede8 in / 
# Wed, 20 Sep 2023 02:44:21 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 18:04:43 GMT
STOPSIGNAL SIGINT
# Wed, 20 Sep 2023 18:05:03 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 18:05:04 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 20 Sep 2023 18:05:05 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 20 Sep 2023 18:05:05 GMT
WORKDIR /var/www/html
# Wed, 20 Sep 2023 18:05:05 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 20 Sep 2023 18:05:05 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 20 Sep 2023 18:05:05 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 20 Sep 2023 18:05:05 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 20 Sep 2023 18:05:16 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 20 Sep 2023 18:05:16 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 20 Sep 2023 18:05:16 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 20 Sep 2023 18:05:16 GMT
USER adminer
# Wed, 20 Sep 2023 18:05:16 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 20 Sep 2023 18:05:16 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:31f5dc1f52c865588c43d8ec718f14d430e149b28f0b28232da825da7ae28f76`  
		Last Modified: Wed, 20 Sep 2023 02:47:53 GMT  
		Size: 53.7 MB (53704892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c82c17c7529e7d3125d9a7f12b8359fac7e9cc29dbb6555d30cbe9bdda203722`  
		Last Modified: Wed, 20 Sep 2023 18:05:50 GMT  
		Size: 39.2 MB (39244274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27290e9432136a39923f648bd1220a36cdd54a4f8baacd87b500eed4d5018d2a`  
		Last Modified: Wed, 20 Sep 2023 18:05:44 GMT  
		Size: 393.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0029f07058cb36f9b27d218954d9e733b152fe47d9875b8d062632100f585d58`  
		Last Modified: Wed, 20 Sep 2023 18:05:44 GMT  
		Size: 1.9 KB (1883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f9ca9fda73283aac009ee0add3e063260cc5c09a89cbdaddef5d3e623c8ae3f`  
		Last Modified: Wed, 20 Sep 2023 18:05:44 GMT  
		Size: 1.5 KB (1477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99dc3e204c8096f4463277e628be5a5860db3a123dd45a87f99df2b8d1d76f77`  
		Last Modified: Wed, 20 Sep 2023 18:05:44 GMT  
		Size: 1.4 MB (1385317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5dbe53bc88443a7def3aa5bed48f19d4bc849da97d88790bf9701396443acac`  
		Last Modified: Wed, 20 Sep 2023 18:05:44 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:standalone` - linux; 386

```console
$ docker pull adminer@sha256:24a953b70c62fedfe7da2846b84d0a3133b442f0721e17fbf5df2d222ae440f8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.0 MB (96989218 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0cbe365ed04581b1b00d6390c52f9260afab49677042b95a947b6ca499d98bdc`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 20 Sep 2023 00:42:07 GMT
ADD file:342c36522089238a534c0912491a4cf64b89133969e051cdad2e694ec761142c in / 
# Wed, 20 Sep 2023 00:42:07 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 15:10:00 GMT
STOPSIGNAL SIGINT
# Wed, 20 Sep 2023 15:10:29 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 15:10:30 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 20 Sep 2023 15:10:31 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 20 Sep 2023 15:10:31 GMT
WORKDIR /var/www/html
# Wed, 20 Sep 2023 15:10:31 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 20 Sep 2023 15:10:31 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 20 Sep 2023 15:10:31 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 20 Sep 2023 15:10:31 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 20 Sep 2023 15:10:47 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 20 Sep 2023 15:10:47 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 20 Sep 2023 15:10:47 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 20 Sep 2023 15:10:47 GMT
USER adminer
# Wed, 20 Sep 2023 15:10:47 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 20 Sep 2023 15:10:47 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:00121bf241b18e981bcc804f905be7b34f95cce415db622599e21dc1a496ee8d`  
		Last Modified: Wed, 20 Sep 2023 00:47:11 GMT  
		Size: 56.0 MB (56040498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:964fa70975aa8c3eb5838cf9120935712a93ec197f9adce227a0d97a7df9d131`  
		Last Modified: Wed, 20 Sep 2023 15:11:38 GMT  
		Size: 39.6 MB (39559141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cf7eb9be8cf86ff0edfb0e7026187487f60c1b234c068e76b9d90c4bb2e56b5`  
		Last Modified: Wed, 20 Sep 2023 15:11:27 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7986b40b588b21caefc32e63e9bf4259713bd637125de9f9e6c415339b62bdb8`  
		Last Modified: Wed, 20 Sep 2023 15:11:27 GMT  
		Size: 1.9 KB (1869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da42b96b0425edc1796b564789c33a81ba8cc1bd8e95886fb24cba7bf6e830f9`  
		Last Modified: Wed, 20 Sep 2023 15:11:27 GMT  
		Size: 1.5 KB (1481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cb8907e77be88986e418354768b790c2a227d56ea26b7a7cdb7027c2958aa71`  
		Last Modified: Wed, 20 Sep 2023 15:11:27 GMT  
		Size: 1.4 MB (1385349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9fdcba82893748b7e9f6211dc3cd3248fa29ee6f78a24482d34339bb1fd857f`  
		Last Modified: Wed, 20 Sep 2023 15:11:27 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:standalone` - linux; mips64le

```console
$ docker pull adminer@sha256:ec803d54e73e17da91a36b9ce59b261f4f312dacabb7e0556302bce0443f75b7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.6 MB (92612531 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:215cf7d1502bb244df43b52290a34650eafce425c56c967b8c9e153a5ada9557`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Wed, 20 Sep 2023 06:40:19 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 20 Sep 2023 06:40:22 GMT
WORKDIR /var/www/html
# Wed, 20 Sep 2023 06:40:25 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 20 Sep 2023 06:40:28 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 20 Sep 2023 06:40:32 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 20 Sep 2023 06:40:35 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 20 Sep 2023 06:41:26 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 20 Sep 2023 06:41:29 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 20 Sep 2023 06:41:32 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 20 Sep 2023 06:41:35 GMT
USER adminer
# Wed, 20 Sep 2023 06:41:39 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 20 Sep 2023 06:41:42 GMT
EXPOSE 8080
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
	-	`sha256:4f0fa2061f2328806a3e6442dc58a5750d76966e9542efd972a12fd49f53cd69`  
		Last Modified: Wed, 20 Sep 2023 06:43:50 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04163c23cec6352cfd6ce393d04f5900400ea72c83d04af1552865c916a1c459`  
		Last Modified: Wed, 20 Sep 2023 06:43:50 GMT  
		Size: 1.5 KB (1481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d726d9d0dfbf6bba7fc6b01578c0a26c84fafdbe71a4e69674dfd1284ce0826`  
		Last Modified: Wed, 20 Sep 2023 06:43:51 GMT  
		Size: 1.4 MB (1386315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e96e2db0e4c5751ce57381cb92f2f2fff089adb321644959f5de599a271ebedc`  
		Last Modified: Wed, 20 Sep 2023 06:43:50 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:standalone` - linux; ppc64le

```console
$ docker pull adminer@sha256:e0809520a8bd4f91b86c0bfd4a871ce4707fd119706f564057dffe5e7c91f5fe
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.3 MB (101262041 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ad347a3c52aeda1176962cc50fcedfab4a87a129219de1394700476d688d49e`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 20 Sep 2023 07:53:09 GMT
ADD file:c12b11abfba27478510c84d05abdd8fec539db9ec30af6d042671f4d5bf793e5 in / 
# Wed, 20 Sep 2023 07:53:12 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 10:27:30 GMT
STOPSIGNAL SIGINT
# Wed, 20 Sep 2023 10:28:24 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 10:28:27 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 20 Sep 2023 10:28:28 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 20 Sep 2023 10:28:28 GMT
WORKDIR /var/www/html
# Wed, 20 Sep 2023 10:28:29 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 20 Sep 2023 10:28:29 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 20 Sep 2023 10:28:30 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 20 Sep 2023 10:28:30 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 20 Sep 2023 10:28:54 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 20 Sep 2023 10:28:54 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 20 Sep 2023 10:28:55 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 20 Sep 2023 10:28:55 GMT
USER adminer
# Wed, 20 Sep 2023 10:28:55 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 20 Sep 2023 10:28:55 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:9f3507d882ae95f06b3672497cdd3317bd4f8e0255e73d10f1f263e5d780f102`  
		Last Modified: Wed, 20 Sep 2023 08:50:16 GMT  
		Size: 58.9 MB (58928499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dc55ae4eee76ca2700dbf8d4554951df837121cc96140f29cbcc2d7308b4d72`  
		Last Modified: Wed, 20 Sep 2023 10:29:59 GMT  
		Size: 40.9 MB (40943739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:413bf430ecd0a8d3a68dc7841be8802fccca3af99645087fbb82e476cd335965`  
		Last Modified: Wed, 20 Sep 2023 10:29:47 GMT  
		Size: 396.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df2720d6c627570256eb0bc8943ba052f2b617c5dd972a3eb74196fc91a3dbbb`  
		Last Modified: Wed, 20 Sep 2023 10:29:47 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b6b255e136e7ac31afc340c04be397be6d98a39da922310d73ffbfff9687a2a`  
		Last Modified: Wed, 20 Sep 2023 10:29:47 GMT  
		Size: 1.5 KB (1481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36bfcc7e4826d80f455356e3a88eb31b2e5c559a49a733a25490d6becb652045`  
		Last Modified: Wed, 20 Sep 2023 10:29:47 GMT  
		Size: 1.4 MB (1385554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36a5f297e715a97e0af1984e9f7dd3cb60fa2226b31fc95bbfb6a3c5d85549af`  
		Last Modified: Wed, 20 Sep 2023 10:29:47 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:standalone` - linux; s390x

```console
$ docker pull adminer@sha256:120087fff0a708c70334e38726cab4a7703516787b7d901b1adc69fde470d694
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.7 MB (93701227 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42031d8d4365bb267d464fac6d7ab8b6e0ad4b097eb47e3e4b2dd8d14b64371d`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Wed, 20 Sep 2023 09:42:33 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 20 Sep 2023 09:42:33 GMT
WORKDIR /var/www/html
# Wed, 20 Sep 2023 09:42:33 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 20 Sep 2023 09:42:34 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 20 Sep 2023 09:42:34 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 20 Sep 2023 09:42:34 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 20 Sep 2023 09:42:57 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 20 Sep 2023 09:42:58 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 20 Sep 2023 09:42:58 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 20 Sep 2023 09:42:59 GMT
USER adminer
# Wed, 20 Sep 2023 09:42:59 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 20 Sep 2023 09:43:00 GMT
EXPOSE 8080
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
	-	`sha256:a0dfeb4132e2fe11e348c94294b33e51684a77419be87fae2d715412dc40e9c1`  
		Last Modified: Wed, 20 Sep 2023 09:43:57 GMT  
		Size: 1.9 KB (1883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:800a5df8795fcb07b6a7efb2135a2a662b31533cd779cc532445e86eae286b9f`  
		Last Modified: Wed, 20 Sep 2023 09:43:57 GMT  
		Size: 1.5 KB (1481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:321185c09a4e5d7e9a145855613f743ef531836df1355ae7593208920ad68541`  
		Last Modified: Wed, 20 Sep 2023 09:43:58 GMT  
		Size: 1.4 MB (1385674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c30b98bdcd0d0b081524334dc05d7905ceb45b6e8230e8156267e4759d587a2c`  
		Last Modified: Wed, 20 Sep 2023 09:43:57 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
