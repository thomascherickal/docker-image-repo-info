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
$ docker pull adminer@sha256:47cb2b1d08526810b31337593d3de2a20a358498620ad53a28ef41dd13eb8c31
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
$ docker pull adminer@sha256:b5570962c3a9981b6572e61dd33f5cbd394a1a9d27ee6342b4241338af330449
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.9 MB (95921691 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5e1b3241b20061365693574e1c1241f64a48b15a7f439b8df760456d83009c7`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Thu, 23 Mar 2023 05:56:14 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 23 Mar 2023 05:56:14 GMT
WORKDIR /var/www/html
# Thu, 23 Mar 2023 05:56:14 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 23 Mar 2023 05:56:14 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 23 Mar 2023 05:56:14 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 23 Mar 2023 05:56:14 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 23 Mar 2023 05:56:25 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Mar 2023 05:56:26 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 23 Mar 2023 05:56:26 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 23 Mar 2023 05:56:26 GMT
USER adminer
# Thu, 23 Mar 2023 05:56:26 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Thu, 23 Mar 2023 05:56:26 GMT
EXPOSE 8080
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
	-	`sha256:39317196bba2d873b239492ba23f8f1d62f89b661fb1760b65f29b1404322c60`  
		Last Modified: Thu, 23 Mar 2023 05:56:53 GMT  
		Size: 1.9 KB (1879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31ea8e1da1f9854a8c3bf43a78f5b403bdfad3f2c2861edfbfd902566950a7a2`  
		Last Modified: Thu, 23 Mar 2023 05:56:53 GMT  
		Size: 1.5 KB (1477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3ce0ac056362cd982a31febaaf97daa568c31c2e95f1f4265e82cc6fbeaffd4`  
		Last Modified: Thu, 23 Mar 2023 05:56:53 GMT  
		Size: 1.4 MB (1385271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac3ee3b23021de0471ff83e0b10babf764acf8f57dbb17c2eef966f084eb314a`  
		Last Modified: Thu, 23 Mar 2023 05:56:53 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4` - linux; arm variant v5

```console
$ docker pull adminer@sha256:6626a30d9f62f8886368c855059bbbe5324d5cd5a21cfcec9d74cd3f62f423b9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.2 MB (91190563 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:858d6152778fac7508d2b7edad80c80dd39df9946d1c4c17d9b0d7a9d4bb2e5a`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Wed, 12 Apr 2023 01:09:24 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 12 Apr 2023 01:09:24 GMT
WORKDIR /var/www/html
# Wed, 12 Apr 2023 01:09:24 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 12 Apr 2023 01:09:25 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 12 Apr 2023 01:09:25 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 12 Apr 2023 01:09:25 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 12 Apr 2023 01:09:40 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 12 Apr 2023 01:09:40 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 12 Apr 2023 01:09:40 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 12 Apr 2023 01:09:40 GMT
USER adminer
# Wed, 12 Apr 2023 01:09:40 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 12 Apr 2023 01:09:40 GMT
EXPOSE 8080
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
	-	`sha256:3f470d2089a740ebc67390ccf884d98cffb79eafd885a0c2b5e0e7b43e69c1c4`  
		Last Modified: Wed, 12 Apr 2023 01:10:10 GMT  
		Size: 1.9 KB (1869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a752232d0c61a7c17d3f25d15b89e4d34c73fd0bffe83dd92258b692f657abf6`  
		Last Modified: Wed, 12 Apr 2023 01:10:10 GMT  
		Size: 1.5 KB (1477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77ec5152fc80b31c2b1f1935c7cc639c14373654830cceb8dfe8602826b16b10`  
		Last Modified: Wed, 12 Apr 2023 01:10:10 GMT  
		Size: 1.4 MB (1385249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10633b8059422ad2e0f668cedeb61e0815df56a24bf954e381f2e8ff79b4caa1`  
		Last Modified: Wed, 12 Apr 2023 01:10:10 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4` - linux; arm variant v7

```console
$ docker pull adminer@sha256:208e28dc00b696fd2786ae0fac00bbac135df7d327a78f1a3b07b430e8be29fa
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.8 MB (87782361 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:924e553786350523e3dabd52a79ebaa532e1ee1f1cd4f55c123b6f2debfd887b`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Thu, 23 Mar 2023 13:54:17 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 23 Mar 2023 13:54:18 GMT
WORKDIR /var/www/html
# Thu, 23 Mar 2023 13:54:18 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 23 Mar 2023 13:54:18 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 23 Mar 2023 13:54:18 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 23 Mar 2023 13:54:18 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 23 Mar 2023 13:54:30 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Mar 2023 13:54:30 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 23 Mar 2023 13:54:30 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 23 Mar 2023 13:54:30 GMT
USER adminer
# Thu, 23 Mar 2023 13:54:30 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Thu, 23 Mar 2023 13:54:30 GMT
EXPOSE 8080
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
	-	`sha256:6c7b7c098bbce560d98941c87164725c63999c701f19f2500e91578c8d994c8f`  
		Last Modified: Thu, 23 Mar 2023 13:54:56 GMT  
		Size: 1.9 KB (1871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90441e257dd07454f7d03e5aa41e80d43c14256ff5040356a29d4639b23d75fc`  
		Last Modified: Thu, 23 Mar 2023 13:54:55 GMT  
		Size: 1.5 KB (1482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65767342491a731ec4afa7560fd1b162f1ea5c932fc69e8326baad4bec228e7e`  
		Last Modified: Thu, 23 Mar 2023 13:54:56 GMT  
		Size: 1.4 MB (1385066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6a8450e329b8116e25e9fa7cb6b678d57084c5946b3167f2cb126880295263a`  
		Last Modified: Thu, 23 Mar 2023 13:54:55 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4` - linux; arm64 variant v8

```console
$ docker pull adminer@sha256:4cda3605cfb6ed0b47e9d450e4d1e8979f04c8a969392e39ae82335de95323d0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.3 MB (94337798 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37e35dd000bf1a912aa2f6512bae1303bf816e1fd62882c26f65a39453286360`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Wed, 12 Apr 2023 01:01:29 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 12 Apr 2023 01:01:29 GMT
WORKDIR /var/www/html
# Wed, 12 Apr 2023 01:01:29 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 12 Apr 2023 01:01:29 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 12 Apr 2023 01:01:29 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 12 Apr 2023 01:01:29 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 12 Apr 2023 01:01:40 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 12 Apr 2023 01:01:40 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 12 Apr 2023 01:01:40 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 12 Apr 2023 01:01:40 GMT
USER adminer
# Wed, 12 Apr 2023 01:01:40 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 12 Apr 2023 01:01:41 GMT
EXPOSE 8080
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
	-	`sha256:905fbef16ad4dc303ccf2c51b20f40e565af53c2cc7a27bc3119ba72fde51908`  
		Last Modified: Wed, 12 Apr 2023 01:02:05 GMT  
		Size: 1.9 KB (1878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83a3dd0ad962d2f3c8153433aca615dc5bb81758ae2622916f28f9ed0e922f62`  
		Last Modified: Wed, 12 Apr 2023 01:02:05 GMT  
		Size: 1.5 KB (1477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cc2dd04f15e567448b396b8a8670939cb5dab2da2304657c79bf8e0b3bd1916`  
		Last Modified: Wed, 12 Apr 2023 01:02:05 GMT  
		Size: 1.4 MB (1385314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36c34adc9404de2e7b713240d2c5712e9eb8eb5a670fbd293da353414fbfbc5c`  
		Last Modified: Wed, 12 Apr 2023 01:02:05 GMT  
		Size: 489.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4` - linux; 386

```console
$ docker pull adminer@sha256:ca2ee65836fd06aba737873c17718cd1ae4e52f6ba9a2869000be6794922ec0d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.0 MB (96975396 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47306ce39706e8ed333600b8d4399cb09c02ffe4e169f76bd59fa5b6569ae778`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Thu, 23 Mar 2023 21:17:41 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 23 Mar 2023 21:17:41 GMT
WORKDIR /var/www/html
# Thu, 23 Mar 2023 21:17:42 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 23 Mar 2023 21:17:42 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 23 Mar 2023 21:17:42 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 23 Mar 2023 21:17:42 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 23 Mar 2023 21:17:54 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Mar 2023 21:17:54 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 23 Mar 2023 21:17:54 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 23 Mar 2023 21:17:54 GMT
USER adminer
# Thu, 23 Mar 2023 21:17:55 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Thu, 23 Mar 2023 21:17:55 GMT
EXPOSE 8080
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
	-	`sha256:7c664bb8231af50f8a98b457a9e7c291444345b0066ed54ddbcc0b2129859965`  
		Last Modified: Thu, 23 Mar 2023 21:18:24 GMT  
		Size: 1.9 KB (1869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6a209358917bcf344993c93aad3b156d6a09b6ab64d43df3941ca51e6c414b9`  
		Last Modified: Thu, 23 Mar 2023 21:18:24 GMT  
		Size: 1.5 KB (1476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:061ad9c8d5ae0dc7e0d69094e0f6d09b29dea00ec113641833b5a37f404de058`  
		Last Modified: Thu, 23 Mar 2023 21:18:24 GMT  
		Size: 1.4 MB (1385210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2761eeb066c4b63e66ada920b87fc430284439f4c76fac14a274ef528430d3f`  
		Last Modified: Thu, 23 Mar 2023 21:18:24 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4` - linux; mips64le

```console
$ docker pull adminer@sha256:14de06501f131ba9f62a814f592d766d6f050b30eab65a15bb1e753a436aab3d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.6 MB (92605785 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ddae0bdce53fcfedd28644c8fc0df52f38f44000615def4d84b2c88db2aff3ab`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Thu, 23 Mar 2023 20:08:09 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 23 Mar 2023 20:08:13 GMT
WORKDIR /var/www/html
# Thu, 23 Mar 2023 20:08:16 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 23 Mar 2023 20:08:19 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 23 Mar 2023 20:08:22 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 23 Mar 2023 20:08:26 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 23 Mar 2023 20:09:18 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Mar 2023 20:09:20 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 23 Mar 2023 20:09:24 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 23 Mar 2023 20:09:27 GMT
USER adminer
# Thu, 23 Mar 2023 20:09:31 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Thu, 23 Mar 2023 20:09:34 GMT
EXPOSE 8080
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
	-	`sha256:0ba90b5b3033a3d6ba607430a17c7e37f0fae8f0664ac81a4e571e9ad9fca9e2`  
		Last Modified: Thu, 23 Mar 2023 20:11:33 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b1980d6708cacd2f28ca074bd917c1143a47040b425da5985915850214f197f`  
		Last Modified: Thu, 23 Mar 2023 20:11:33 GMT  
		Size: 1.5 KB (1481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acfbeda1e7451034cf22503ff221351a0d3f5e1f63a6f11dc71a81450a7aaadd`  
		Last Modified: Thu, 23 Mar 2023 20:11:34 GMT  
		Size: 1.4 MB (1386264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b87439fd13726c64bed775edf40ceb3cbc1b5dbf3f62fb9b127024394aaece4`  
		Last Modified: Thu, 23 Mar 2023 20:11:33 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4` - linux; ppc64le

```console
$ docker pull adminer@sha256:a55a2c1ff24d027a36e46d24a34dcbb8e854ae5392eec85f9620ba60c7b58694
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.3 MB (101256116 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4735ee16dfbcee3a436e08438e55c6dd5114b673eec23b536b6b3a2f043a76ad`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Wed, 12 Apr 2023 01:20:37 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 12 Apr 2023 01:20:38 GMT
WORKDIR /var/www/html
# Wed, 12 Apr 2023 01:20:38 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 12 Apr 2023 01:20:39 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 12 Apr 2023 01:20:39 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 12 Apr 2023 01:20:40 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 12 Apr 2023 01:21:30 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 12 Apr 2023 01:21:31 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 12 Apr 2023 01:21:32 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 12 Apr 2023 01:21:34 GMT
USER adminer
# Wed, 12 Apr 2023 01:21:34 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 12 Apr 2023 01:21:35 GMT
EXPOSE 8080
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
	-	`sha256:79148517f43f66f402dd39c8ce8a6104a51fe03f3ed892be0eb40a2bf3ac513e`  
		Last Modified: Wed, 12 Apr 2023 01:22:40 GMT  
		Size: 1.9 KB (1879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67bc627fe6d1eed682ead8566e47d1e2328da8a1df7864e5a52ac7d20d815572`  
		Last Modified: Wed, 12 Apr 2023 01:22:40 GMT  
		Size: 1.5 KB (1481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8eb7bbdc982c8e7f315e96ecd620a4c3a9d486beb72d36f89daddaaca429d14`  
		Last Modified: Wed, 12 Apr 2023 01:22:41 GMT  
		Size: 1.4 MB (1385746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7f1791e7b6ab1e976b9698dd6aed465ae1b9badc2ae1c6b6cb91197748b149d`  
		Last Modified: Wed, 12 Apr 2023 01:22:40 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4` - linux; s390x

```console
$ docker pull adminer@sha256:5472a0984af7a0bcb4f370188898007842266789e4d9cd931aea7e05ffa0c318
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.7 MB (93694065 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f21ca8c09f92e5cedf5daa80fc0e9a2a1b8b7e032b3719641feadef4e6294cf5`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Wed, 12 Apr 2023 00:22:45 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 12 Apr 2023 00:22:45 GMT
WORKDIR /var/www/html
# Wed, 12 Apr 2023 00:22:45 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 12 Apr 2023 00:22:46 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 12 Apr 2023 00:22:46 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 12 Apr 2023 00:22:46 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 12 Apr 2023 00:22:57 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 12 Apr 2023 00:22:57 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 12 Apr 2023 00:22:57 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 12 Apr 2023 00:22:58 GMT
USER adminer
# Wed, 12 Apr 2023 00:22:58 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 12 Apr 2023 00:22:58 GMT
EXPOSE 8080
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
	-	`sha256:b23597fac1b0ce84055df85a56ef40909911286a24879b39f37200567f8e6e63`  
		Last Modified: Wed, 12 Apr 2023 00:23:41 GMT  
		Size: 1.9 KB (1879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e88da54b627b523974ad186c33e429711d0e4968550bc7b513fae7d58b9f3de1`  
		Last Modified: Wed, 12 Apr 2023 00:23:41 GMT  
		Size: 1.5 KB (1478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b8c6c7cf39dd303de3dcb8c7c363f95bfcf24b7dfbd409557940ced6e28cd6e`  
		Last Modified: Wed, 12 Apr 2023 00:23:41 GMT  
		Size: 1.4 MB (1385468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:640f1f42167e00265be1505a797a83c7cf74946f47391b62064c6fd44e4fee4d`  
		Last Modified: Wed, 12 Apr 2023 00:23:41 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `adminer:4-fastcgi`

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

### `adminer:4-fastcgi` - linux; amd64

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

### `adminer:4-fastcgi` - linux; arm variant v5

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

### `adminer:4-fastcgi` - linux; arm variant v7

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

### `adminer:4-fastcgi` - linux; arm64 variant v8

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

### `adminer:4-fastcgi` - linux; 386

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

### `adminer:4-fastcgi` - linux; mips64le

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

### `adminer:4-fastcgi` - linux; ppc64le

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

### `adminer:4-fastcgi` - linux; s390x

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

## `adminer:4-standalone`

```console
$ docker pull adminer@sha256:47cb2b1d08526810b31337593d3de2a20a358498620ad53a28ef41dd13eb8c31
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
$ docker pull adminer@sha256:b5570962c3a9981b6572e61dd33f5cbd394a1a9d27ee6342b4241338af330449
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.9 MB (95921691 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5e1b3241b20061365693574e1c1241f64a48b15a7f439b8df760456d83009c7`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Thu, 23 Mar 2023 05:56:14 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 23 Mar 2023 05:56:14 GMT
WORKDIR /var/www/html
# Thu, 23 Mar 2023 05:56:14 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 23 Mar 2023 05:56:14 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 23 Mar 2023 05:56:14 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 23 Mar 2023 05:56:14 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 23 Mar 2023 05:56:25 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Mar 2023 05:56:26 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 23 Mar 2023 05:56:26 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 23 Mar 2023 05:56:26 GMT
USER adminer
# Thu, 23 Mar 2023 05:56:26 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Thu, 23 Mar 2023 05:56:26 GMT
EXPOSE 8080
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
	-	`sha256:39317196bba2d873b239492ba23f8f1d62f89b661fb1760b65f29b1404322c60`  
		Last Modified: Thu, 23 Mar 2023 05:56:53 GMT  
		Size: 1.9 KB (1879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31ea8e1da1f9854a8c3bf43a78f5b403bdfad3f2c2861edfbfd902566950a7a2`  
		Last Modified: Thu, 23 Mar 2023 05:56:53 GMT  
		Size: 1.5 KB (1477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3ce0ac056362cd982a31febaaf97daa568c31c2e95f1f4265e82cc6fbeaffd4`  
		Last Modified: Thu, 23 Mar 2023 05:56:53 GMT  
		Size: 1.4 MB (1385271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac3ee3b23021de0471ff83e0b10babf764acf8f57dbb17c2eef966f084eb314a`  
		Last Modified: Thu, 23 Mar 2023 05:56:53 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-standalone` - linux; arm variant v5

```console
$ docker pull adminer@sha256:6626a30d9f62f8886368c855059bbbe5324d5cd5a21cfcec9d74cd3f62f423b9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.2 MB (91190563 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:858d6152778fac7508d2b7edad80c80dd39df9946d1c4c17d9b0d7a9d4bb2e5a`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Wed, 12 Apr 2023 01:09:24 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 12 Apr 2023 01:09:24 GMT
WORKDIR /var/www/html
# Wed, 12 Apr 2023 01:09:24 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 12 Apr 2023 01:09:25 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 12 Apr 2023 01:09:25 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 12 Apr 2023 01:09:25 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 12 Apr 2023 01:09:40 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 12 Apr 2023 01:09:40 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 12 Apr 2023 01:09:40 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 12 Apr 2023 01:09:40 GMT
USER adminer
# Wed, 12 Apr 2023 01:09:40 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 12 Apr 2023 01:09:40 GMT
EXPOSE 8080
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
	-	`sha256:3f470d2089a740ebc67390ccf884d98cffb79eafd885a0c2b5e0e7b43e69c1c4`  
		Last Modified: Wed, 12 Apr 2023 01:10:10 GMT  
		Size: 1.9 KB (1869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a752232d0c61a7c17d3f25d15b89e4d34c73fd0bffe83dd92258b692f657abf6`  
		Last Modified: Wed, 12 Apr 2023 01:10:10 GMT  
		Size: 1.5 KB (1477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77ec5152fc80b31c2b1f1935c7cc639c14373654830cceb8dfe8602826b16b10`  
		Last Modified: Wed, 12 Apr 2023 01:10:10 GMT  
		Size: 1.4 MB (1385249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10633b8059422ad2e0f668cedeb61e0815df56a24bf954e381f2e8ff79b4caa1`  
		Last Modified: Wed, 12 Apr 2023 01:10:10 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-standalone` - linux; arm variant v7

```console
$ docker pull adminer@sha256:208e28dc00b696fd2786ae0fac00bbac135df7d327a78f1a3b07b430e8be29fa
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.8 MB (87782361 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:924e553786350523e3dabd52a79ebaa532e1ee1f1cd4f55c123b6f2debfd887b`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Thu, 23 Mar 2023 13:54:17 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 23 Mar 2023 13:54:18 GMT
WORKDIR /var/www/html
# Thu, 23 Mar 2023 13:54:18 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 23 Mar 2023 13:54:18 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 23 Mar 2023 13:54:18 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 23 Mar 2023 13:54:18 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 23 Mar 2023 13:54:30 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Mar 2023 13:54:30 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 23 Mar 2023 13:54:30 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 23 Mar 2023 13:54:30 GMT
USER adminer
# Thu, 23 Mar 2023 13:54:30 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Thu, 23 Mar 2023 13:54:30 GMT
EXPOSE 8080
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
	-	`sha256:6c7b7c098bbce560d98941c87164725c63999c701f19f2500e91578c8d994c8f`  
		Last Modified: Thu, 23 Mar 2023 13:54:56 GMT  
		Size: 1.9 KB (1871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90441e257dd07454f7d03e5aa41e80d43c14256ff5040356a29d4639b23d75fc`  
		Last Modified: Thu, 23 Mar 2023 13:54:55 GMT  
		Size: 1.5 KB (1482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65767342491a731ec4afa7560fd1b162f1ea5c932fc69e8326baad4bec228e7e`  
		Last Modified: Thu, 23 Mar 2023 13:54:56 GMT  
		Size: 1.4 MB (1385066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6a8450e329b8116e25e9fa7cb6b678d57084c5946b3167f2cb126880295263a`  
		Last Modified: Thu, 23 Mar 2023 13:54:55 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-standalone` - linux; arm64 variant v8

```console
$ docker pull adminer@sha256:4cda3605cfb6ed0b47e9d450e4d1e8979f04c8a969392e39ae82335de95323d0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.3 MB (94337798 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37e35dd000bf1a912aa2f6512bae1303bf816e1fd62882c26f65a39453286360`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Wed, 12 Apr 2023 01:01:29 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 12 Apr 2023 01:01:29 GMT
WORKDIR /var/www/html
# Wed, 12 Apr 2023 01:01:29 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 12 Apr 2023 01:01:29 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 12 Apr 2023 01:01:29 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 12 Apr 2023 01:01:29 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 12 Apr 2023 01:01:40 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 12 Apr 2023 01:01:40 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 12 Apr 2023 01:01:40 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 12 Apr 2023 01:01:40 GMT
USER adminer
# Wed, 12 Apr 2023 01:01:40 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 12 Apr 2023 01:01:41 GMT
EXPOSE 8080
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
	-	`sha256:905fbef16ad4dc303ccf2c51b20f40e565af53c2cc7a27bc3119ba72fde51908`  
		Last Modified: Wed, 12 Apr 2023 01:02:05 GMT  
		Size: 1.9 KB (1878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83a3dd0ad962d2f3c8153433aca615dc5bb81758ae2622916f28f9ed0e922f62`  
		Last Modified: Wed, 12 Apr 2023 01:02:05 GMT  
		Size: 1.5 KB (1477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cc2dd04f15e567448b396b8a8670939cb5dab2da2304657c79bf8e0b3bd1916`  
		Last Modified: Wed, 12 Apr 2023 01:02:05 GMT  
		Size: 1.4 MB (1385314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36c34adc9404de2e7b713240d2c5712e9eb8eb5a670fbd293da353414fbfbc5c`  
		Last Modified: Wed, 12 Apr 2023 01:02:05 GMT  
		Size: 489.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-standalone` - linux; 386

```console
$ docker pull adminer@sha256:ca2ee65836fd06aba737873c17718cd1ae4e52f6ba9a2869000be6794922ec0d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.0 MB (96975396 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47306ce39706e8ed333600b8d4399cb09c02ffe4e169f76bd59fa5b6569ae778`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Thu, 23 Mar 2023 21:17:41 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 23 Mar 2023 21:17:41 GMT
WORKDIR /var/www/html
# Thu, 23 Mar 2023 21:17:42 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 23 Mar 2023 21:17:42 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 23 Mar 2023 21:17:42 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 23 Mar 2023 21:17:42 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 23 Mar 2023 21:17:54 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Mar 2023 21:17:54 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 23 Mar 2023 21:17:54 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 23 Mar 2023 21:17:54 GMT
USER adminer
# Thu, 23 Mar 2023 21:17:55 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Thu, 23 Mar 2023 21:17:55 GMT
EXPOSE 8080
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
	-	`sha256:7c664bb8231af50f8a98b457a9e7c291444345b0066ed54ddbcc0b2129859965`  
		Last Modified: Thu, 23 Mar 2023 21:18:24 GMT  
		Size: 1.9 KB (1869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6a209358917bcf344993c93aad3b156d6a09b6ab64d43df3941ca51e6c414b9`  
		Last Modified: Thu, 23 Mar 2023 21:18:24 GMT  
		Size: 1.5 KB (1476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:061ad9c8d5ae0dc7e0d69094e0f6d09b29dea00ec113641833b5a37f404de058`  
		Last Modified: Thu, 23 Mar 2023 21:18:24 GMT  
		Size: 1.4 MB (1385210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2761eeb066c4b63e66ada920b87fc430284439f4c76fac14a274ef528430d3f`  
		Last Modified: Thu, 23 Mar 2023 21:18:24 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-standalone` - linux; mips64le

```console
$ docker pull adminer@sha256:14de06501f131ba9f62a814f592d766d6f050b30eab65a15bb1e753a436aab3d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.6 MB (92605785 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ddae0bdce53fcfedd28644c8fc0df52f38f44000615def4d84b2c88db2aff3ab`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Thu, 23 Mar 2023 20:08:09 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 23 Mar 2023 20:08:13 GMT
WORKDIR /var/www/html
# Thu, 23 Mar 2023 20:08:16 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 23 Mar 2023 20:08:19 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 23 Mar 2023 20:08:22 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 23 Mar 2023 20:08:26 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 23 Mar 2023 20:09:18 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Mar 2023 20:09:20 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 23 Mar 2023 20:09:24 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 23 Mar 2023 20:09:27 GMT
USER adminer
# Thu, 23 Mar 2023 20:09:31 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Thu, 23 Mar 2023 20:09:34 GMT
EXPOSE 8080
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
	-	`sha256:0ba90b5b3033a3d6ba607430a17c7e37f0fae8f0664ac81a4e571e9ad9fca9e2`  
		Last Modified: Thu, 23 Mar 2023 20:11:33 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b1980d6708cacd2f28ca074bd917c1143a47040b425da5985915850214f197f`  
		Last Modified: Thu, 23 Mar 2023 20:11:33 GMT  
		Size: 1.5 KB (1481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acfbeda1e7451034cf22503ff221351a0d3f5e1f63a6f11dc71a81450a7aaadd`  
		Last Modified: Thu, 23 Mar 2023 20:11:34 GMT  
		Size: 1.4 MB (1386264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b87439fd13726c64bed775edf40ceb3cbc1b5dbf3f62fb9b127024394aaece4`  
		Last Modified: Thu, 23 Mar 2023 20:11:33 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-standalone` - linux; ppc64le

```console
$ docker pull adminer@sha256:a55a2c1ff24d027a36e46d24a34dcbb8e854ae5392eec85f9620ba60c7b58694
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.3 MB (101256116 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4735ee16dfbcee3a436e08438e55c6dd5114b673eec23b536b6b3a2f043a76ad`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Wed, 12 Apr 2023 01:20:37 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 12 Apr 2023 01:20:38 GMT
WORKDIR /var/www/html
# Wed, 12 Apr 2023 01:20:38 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 12 Apr 2023 01:20:39 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 12 Apr 2023 01:20:39 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 12 Apr 2023 01:20:40 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 12 Apr 2023 01:21:30 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 12 Apr 2023 01:21:31 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 12 Apr 2023 01:21:32 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 12 Apr 2023 01:21:34 GMT
USER adminer
# Wed, 12 Apr 2023 01:21:34 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 12 Apr 2023 01:21:35 GMT
EXPOSE 8080
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
	-	`sha256:79148517f43f66f402dd39c8ce8a6104a51fe03f3ed892be0eb40a2bf3ac513e`  
		Last Modified: Wed, 12 Apr 2023 01:22:40 GMT  
		Size: 1.9 KB (1879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67bc627fe6d1eed682ead8566e47d1e2328da8a1df7864e5a52ac7d20d815572`  
		Last Modified: Wed, 12 Apr 2023 01:22:40 GMT  
		Size: 1.5 KB (1481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8eb7bbdc982c8e7f315e96ecd620a4c3a9d486beb72d36f89daddaaca429d14`  
		Last Modified: Wed, 12 Apr 2023 01:22:41 GMT  
		Size: 1.4 MB (1385746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7f1791e7b6ab1e976b9698dd6aed465ae1b9badc2ae1c6b6cb91197748b149d`  
		Last Modified: Wed, 12 Apr 2023 01:22:40 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-standalone` - linux; s390x

```console
$ docker pull adminer@sha256:5472a0984af7a0bcb4f370188898007842266789e4d9cd931aea7e05ffa0c318
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.7 MB (93694065 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f21ca8c09f92e5cedf5daa80fc0e9a2a1b8b7e032b3719641feadef4e6294cf5`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Wed, 12 Apr 2023 00:22:45 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 12 Apr 2023 00:22:45 GMT
WORKDIR /var/www/html
# Wed, 12 Apr 2023 00:22:45 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 12 Apr 2023 00:22:46 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 12 Apr 2023 00:22:46 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 12 Apr 2023 00:22:46 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 12 Apr 2023 00:22:57 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 12 Apr 2023 00:22:57 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 12 Apr 2023 00:22:57 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 12 Apr 2023 00:22:58 GMT
USER adminer
# Wed, 12 Apr 2023 00:22:58 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 12 Apr 2023 00:22:58 GMT
EXPOSE 8080
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
	-	`sha256:b23597fac1b0ce84055df85a56ef40909911286a24879b39f37200567f8e6e63`  
		Last Modified: Wed, 12 Apr 2023 00:23:41 GMT  
		Size: 1.9 KB (1879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e88da54b627b523974ad186c33e429711d0e4968550bc7b513fae7d58b9f3de1`  
		Last Modified: Wed, 12 Apr 2023 00:23:41 GMT  
		Size: 1.5 KB (1478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b8c6c7cf39dd303de3dcb8c7c363f95bfcf24b7dfbd409557940ced6e28cd6e`  
		Last Modified: Wed, 12 Apr 2023 00:23:41 GMT  
		Size: 1.4 MB (1385468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:640f1f42167e00265be1505a797a83c7cf74946f47391b62064c6fd44e4fee4d`  
		Last Modified: Wed, 12 Apr 2023 00:23:41 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `adminer:4.8.1`

```console
$ docker pull adminer@sha256:47cb2b1d08526810b31337593d3de2a20a358498620ad53a28ef41dd13eb8c31
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
$ docker pull adminer@sha256:b5570962c3a9981b6572e61dd33f5cbd394a1a9d27ee6342b4241338af330449
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.9 MB (95921691 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5e1b3241b20061365693574e1c1241f64a48b15a7f439b8df760456d83009c7`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Thu, 23 Mar 2023 05:56:14 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 23 Mar 2023 05:56:14 GMT
WORKDIR /var/www/html
# Thu, 23 Mar 2023 05:56:14 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 23 Mar 2023 05:56:14 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 23 Mar 2023 05:56:14 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 23 Mar 2023 05:56:14 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 23 Mar 2023 05:56:25 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Mar 2023 05:56:26 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 23 Mar 2023 05:56:26 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 23 Mar 2023 05:56:26 GMT
USER adminer
# Thu, 23 Mar 2023 05:56:26 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Thu, 23 Mar 2023 05:56:26 GMT
EXPOSE 8080
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
	-	`sha256:39317196bba2d873b239492ba23f8f1d62f89b661fb1760b65f29b1404322c60`  
		Last Modified: Thu, 23 Mar 2023 05:56:53 GMT  
		Size: 1.9 KB (1879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31ea8e1da1f9854a8c3bf43a78f5b403bdfad3f2c2861edfbfd902566950a7a2`  
		Last Modified: Thu, 23 Mar 2023 05:56:53 GMT  
		Size: 1.5 KB (1477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3ce0ac056362cd982a31febaaf97daa568c31c2e95f1f4265e82cc6fbeaffd4`  
		Last Modified: Thu, 23 Mar 2023 05:56:53 GMT  
		Size: 1.4 MB (1385271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac3ee3b23021de0471ff83e0b10babf764acf8f57dbb17c2eef966f084eb314a`  
		Last Modified: Thu, 23 Mar 2023 05:56:53 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1` - linux; arm variant v5

```console
$ docker pull adminer@sha256:6626a30d9f62f8886368c855059bbbe5324d5cd5a21cfcec9d74cd3f62f423b9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.2 MB (91190563 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:858d6152778fac7508d2b7edad80c80dd39df9946d1c4c17d9b0d7a9d4bb2e5a`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Wed, 12 Apr 2023 01:09:24 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 12 Apr 2023 01:09:24 GMT
WORKDIR /var/www/html
# Wed, 12 Apr 2023 01:09:24 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 12 Apr 2023 01:09:25 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 12 Apr 2023 01:09:25 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 12 Apr 2023 01:09:25 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 12 Apr 2023 01:09:40 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 12 Apr 2023 01:09:40 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 12 Apr 2023 01:09:40 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 12 Apr 2023 01:09:40 GMT
USER adminer
# Wed, 12 Apr 2023 01:09:40 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 12 Apr 2023 01:09:40 GMT
EXPOSE 8080
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
	-	`sha256:3f470d2089a740ebc67390ccf884d98cffb79eafd885a0c2b5e0e7b43e69c1c4`  
		Last Modified: Wed, 12 Apr 2023 01:10:10 GMT  
		Size: 1.9 KB (1869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a752232d0c61a7c17d3f25d15b89e4d34c73fd0bffe83dd92258b692f657abf6`  
		Last Modified: Wed, 12 Apr 2023 01:10:10 GMT  
		Size: 1.5 KB (1477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77ec5152fc80b31c2b1f1935c7cc639c14373654830cceb8dfe8602826b16b10`  
		Last Modified: Wed, 12 Apr 2023 01:10:10 GMT  
		Size: 1.4 MB (1385249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10633b8059422ad2e0f668cedeb61e0815df56a24bf954e381f2e8ff79b4caa1`  
		Last Modified: Wed, 12 Apr 2023 01:10:10 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1` - linux; arm variant v7

```console
$ docker pull adminer@sha256:208e28dc00b696fd2786ae0fac00bbac135df7d327a78f1a3b07b430e8be29fa
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.8 MB (87782361 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:924e553786350523e3dabd52a79ebaa532e1ee1f1cd4f55c123b6f2debfd887b`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Thu, 23 Mar 2023 13:54:17 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 23 Mar 2023 13:54:18 GMT
WORKDIR /var/www/html
# Thu, 23 Mar 2023 13:54:18 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 23 Mar 2023 13:54:18 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 23 Mar 2023 13:54:18 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 23 Mar 2023 13:54:18 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 23 Mar 2023 13:54:30 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Mar 2023 13:54:30 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 23 Mar 2023 13:54:30 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 23 Mar 2023 13:54:30 GMT
USER adminer
# Thu, 23 Mar 2023 13:54:30 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Thu, 23 Mar 2023 13:54:30 GMT
EXPOSE 8080
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
	-	`sha256:6c7b7c098bbce560d98941c87164725c63999c701f19f2500e91578c8d994c8f`  
		Last Modified: Thu, 23 Mar 2023 13:54:56 GMT  
		Size: 1.9 KB (1871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90441e257dd07454f7d03e5aa41e80d43c14256ff5040356a29d4639b23d75fc`  
		Last Modified: Thu, 23 Mar 2023 13:54:55 GMT  
		Size: 1.5 KB (1482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65767342491a731ec4afa7560fd1b162f1ea5c932fc69e8326baad4bec228e7e`  
		Last Modified: Thu, 23 Mar 2023 13:54:56 GMT  
		Size: 1.4 MB (1385066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6a8450e329b8116e25e9fa7cb6b678d57084c5946b3167f2cb126880295263a`  
		Last Modified: Thu, 23 Mar 2023 13:54:55 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1` - linux; arm64 variant v8

```console
$ docker pull adminer@sha256:4cda3605cfb6ed0b47e9d450e4d1e8979f04c8a969392e39ae82335de95323d0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.3 MB (94337798 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37e35dd000bf1a912aa2f6512bae1303bf816e1fd62882c26f65a39453286360`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Wed, 12 Apr 2023 01:01:29 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 12 Apr 2023 01:01:29 GMT
WORKDIR /var/www/html
# Wed, 12 Apr 2023 01:01:29 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 12 Apr 2023 01:01:29 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 12 Apr 2023 01:01:29 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 12 Apr 2023 01:01:29 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 12 Apr 2023 01:01:40 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 12 Apr 2023 01:01:40 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 12 Apr 2023 01:01:40 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 12 Apr 2023 01:01:40 GMT
USER adminer
# Wed, 12 Apr 2023 01:01:40 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 12 Apr 2023 01:01:41 GMT
EXPOSE 8080
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
	-	`sha256:905fbef16ad4dc303ccf2c51b20f40e565af53c2cc7a27bc3119ba72fde51908`  
		Last Modified: Wed, 12 Apr 2023 01:02:05 GMT  
		Size: 1.9 KB (1878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83a3dd0ad962d2f3c8153433aca615dc5bb81758ae2622916f28f9ed0e922f62`  
		Last Modified: Wed, 12 Apr 2023 01:02:05 GMT  
		Size: 1.5 KB (1477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cc2dd04f15e567448b396b8a8670939cb5dab2da2304657c79bf8e0b3bd1916`  
		Last Modified: Wed, 12 Apr 2023 01:02:05 GMT  
		Size: 1.4 MB (1385314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36c34adc9404de2e7b713240d2c5712e9eb8eb5a670fbd293da353414fbfbc5c`  
		Last Modified: Wed, 12 Apr 2023 01:02:05 GMT  
		Size: 489.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1` - linux; 386

```console
$ docker pull adminer@sha256:ca2ee65836fd06aba737873c17718cd1ae4e52f6ba9a2869000be6794922ec0d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.0 MB (96975396 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47306ce39706e8ed333600b8d4399cb09c02ffe4e169f76bd59fa5b6569ae778`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Thu, 23 Mar 2023 21:17:41 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 23 Mar 2023 21:17:41 GMT
WORKDIR /var/www/html
# Thu, 23 Mar 2023 21:17:42 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 23 Mar 2023 21:17:42 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 23 Mar 2023 21:17:42 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 23 Mar 2023 21:17:42 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 23 Mar 2023 21:17:54 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Mar 2023 21:17:54 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 23 Mar 2023 21:17:54 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 23 Mar 2023 21:17:54 GMT
USER adminer
# Thu, 23 Mar 2023 21:17:55 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Thu, 23 Mar 2023 21:17:55 GMT
EXPOSE 8080
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
	-	`sha256:7c664bb8231af50f8a98b457a9e7c291444345b0066ed54ddbcc0b2129859965`  
		Last Modified: Thu, 23 Mar 2023 21:18:24 GMT  
		Size: 1.9 KB (1869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6a209358917bcf344993c93aad3b156d6a09b6ab64d43df3941ca51e6c414b9`  
		Last Modified: Thu, 23 Mar 2023 21:18:24 GMT  
		Size: 1.5 KB (1476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:061ad9c8d5ae0dc7e0d69094e0f6d09b29dea00ec113641833b5a37f404de058`  
		Last Modified: Thu, 23 Mar 2023 21:18:24 GMT  
		Size: 1.4 MB (1385210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2761eeb066c4b63e66ada920b87fc430284439f4c76fac14a274ef528430d3f`  
		Last Modified: Thu, 23 Mar 2023 21:18:24 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1` - linux; mips64le

```console
$ docker pull adminer@sha256:14de06501f131ba9f62a814f592d766d6f050b30eab65a15bb1e753a436aab3d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.6 MB (92605785 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ddae0bdce53fcfedd28644c8fc0df52f38f44000615def4d84b2c88db2aff3ab`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Thu, 23 Mar 2023 20:08:09 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 23 Mar 2023 20:08:13 GMT
WORKDIR /var/www/html
# Thu, 23 Mar 2023 20:08:16 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 23 Mar 2023 20:08:19 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 23 Mar 2023 20:08:22 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 23 Mar 2023 20:08:26 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 23 Mar 2023 20:09:18 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Mar 2023 20:09:20 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 23 Mar 2023 20:09:24 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 23 Mar 2023 20:09:27 GMT
USER adminer
# Thu, 23 Mar 2023 20:09:31 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Thu, 23 Mar 2023 20:09:34 GMT
EXPOSE 8080
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
	-	`sha256:0ba90b5b3033a3d6ba607430a17c7e37f0fae8f0664ac81a4e571e9ad9fca9e2`  
		Last Modified: Thu, 23 Mar 2023 20:11:33 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b1980d6708cacd2f28ca074bd917c1143a47040b425da5985915850214f197f`  
		Last Modified: Thu, 23 Mar 2023 20:11:33 GMT  
		Size: 1.5 KB (1481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acfbeda1e7451034cf22503ff221351a0d3f5e1f63a6f11dc71a81450a7aaadd`  
		Last Modified: Thu, 23 Mar 2023 20:11:34 GMT  
		Size: 1.4 MB (1386264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b87439fd13726c64bed775edf40ceb3cbc1b5dbf3f62fb9b127024394aaece4`  
		Last Modified: Thu, 23 Mar 2023 20:11:33 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1` - linux; ppc64le

```console
$ docker pull adminer@sha256:a55a2c1ff24d027a36e46d24a34dcbb8e854ae5392eec85f9620ba60c7b58694
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.3 MB (101256116 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4735ee16dfbcee3a436e08438e55c6dd5114b673eec23b536b6b3a2f043a76ad`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Wed, 12 Apr 2023 01:20:37 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 12 Apr 2023 01:20:38 GMT
WORKDIR /var/www/html
# Wed, 12 Apr 2023 01:20:38 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 12 Apr 2023 01:20:39 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 12 Apr 2023 01:20:39 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 12 Apr 2023 01:20:40 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 12 Apr 2023 01:21:30 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 12 Apr 2023 01:21:31 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 12 Apr 2023 01:21:32 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 12 Apr 2023 01:21:34 GMT
USER adminer
# Wed, 12 Apr 2023 01:21:34 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 12 Apr 2023 01:21:35 GMT
EXPOSE 8080
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
	-	`sha256:79148517f43f66f402dd39c8ce8a6104a51fe03f3ed892be0eb40a2bf3ac513e`  
		Last Modified: Wed, 12 Apr 2023 01:22:40 GMT  
		Size: 1.9 KB (1879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67bc627fe6d1eed682ead8566e47d1e2328da8a1df7864e5a52ac7d20d815572`  
		Last Modified: Wed, 12 Apr 2023 01:22:40 GMT  
		Size: 1.5 KB (1481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8eb7bbdc982c8e7f315e96ecd620a4c3a9d486beb72d36f89daddaaca429d14`  
		Last Modified: Wed, 12 Apr 2023 01:22:41 GMT  
		Size: 1.4 MB (1385746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7f1791e7b6ab1e976b9698dd6aed465ae1b9badc2ae1c6b6cb91197748b149d`  
		Last Modified: Wed, 12 Apr 2023 01:22:40 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1` - linux; s390x

```console
$ docker pull adminer@sha256:5472a0984af7a0bcb4f370188898007842266789e4d9cd931aea7e05ffa0c318
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.7 MB (93694065 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f21ca8c09f92e5cedf5daa80fc0e9a2a1b8b7e032b3719641feadef4e6294cf5`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Wed, 12 Apr 2023 00:22:45 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 12 Apr 2023 00:22:45 GMT
WORKDIR /var/www/html
# Wed, 12 Apr 2023 00:22:45 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 12 Apr 2023 00:22:46 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 12 Apr 2023 00:22:46 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 12 Apr 2023 00:22:46 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 12 Apr 2023 00:22:57 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 12 Apr 2023 00:22:57 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 12 Apr 2023 00:22:57 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 12 Apr 2023 00:22:58 GMT
USER adminer
# Wed, 12 Apr 2023 00:22:58 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 12 Apr 2023 00:22:58 GMT
EXPOSE 8080
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
	-	`sha256:b23597fac1b0ce84055df85a56ef40909911286a24879b39f37200567f8e6e63`  
		Last Modified: Wed, 12 Apr 2023 00:23:41 GMT  
		Size: 1.9 KB (1879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e88da54b627b523974ad186c33e429711d0e4968550bc7b513fae7d58b9f3de1`  
		Last Modified: Wed, 12 Apr 2023 00:23:41 GMT  
		Size: 1.5 KB (1478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b8c6c7cf39dd303de3dcb8c7c363f95bfcf24b7dfbd409557940ced6e28cd6e`  
		Last Modified: Wed, 12 Apr 2023 00:23:41 GMT  
		Size: 1.4 MB (1385468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:640f1f42167e00265be1505a797a83c7cf74946f47391b62064c6fd44e4fee4d`  
		Last Modified: Wed, 12 Apr 2023 00:23:41 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `adminer:4.8.1-fastcgi`

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

### `adminer:4.8.1-fastcgi` - linux; amd64

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

### `adminer:4.8.1-fastcgi` - linux; arm variant v5

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

### `adminer:4.8.1-fastcgi` - linux; arm variant v7

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

### `adminer:4.8.1-fastcgi` - linux; arm64 variant v8

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

### `adminer:4.8.1-fastcgi` - linux; 386

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

### `adminer:4.8.1-fastcgi` - linux; mips64le

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

### `adminer:4.8.1-fastcgi` - linux; ppc64le

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

### `adminer:4.8.1-fastcgi` - linux; s390x

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

## `adminer:4.8.1-standalone`

```console
$ docker pull adminer@sha256:47cb2b1d08526810b31337593d3de2a20a358498620ad53a28ef41dd13eb8c31
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
$ docker pull adminer@sha256:b5570962c3a9981b6572e61dd33f5cbd394a1a9d27ee6342b4241338af330449
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.9 MB (95921691 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5e1b3241b20061365693574e1c1241f64a48b15a7f439b8df760456d83009c7`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Thu, 23 Mar 2023 05:56:14 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 23 Mar 2023 05:56:14 GMT
WORKDIR /var/www/html
# Thu, 23 Mar 2023 05:56:14 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 23 Mar 2023 05:56:14 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 23 Mar 2023 05:56:14 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 23 Mar 2023 05:56:14 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 23 Mar 2023 05:56:25 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Mar 2023 05:56:26 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 23 Mar 2023 05:56:26 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 23 Mar 2023 05:56:26 GMT
USER adminer
# Thu, 23 Mar 2023 05:56:26 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Thu, 23 Mar 2023 05:56:26 GMT
EXPOSE 8080
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
	-	`sha256:39317196bba2d873b239492ba23f8f1d62f89b661fb1760b65f29b1404322c60`  
		Last Modified: Thu, 23 Mar 2023 05:56:53 GMT  
		Size: 1.9 KB (1879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31ea8e1da1f9854a8c3bf43a78f5b403bdfad3f2c2861edfbfd902566950a7a2`  
		Last Modified: Thu, 23 Mar 2023 05:56:53 GMT  
		Size: 1.5 KB (1477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3ce0ac056362cd982a31febaaf97daa568c31c2e95f1f4265e82cc6fbeaffd4`  
		Last Modified: Thu, 23 Mar 2023 05:56:53 GMT  
		Size: 1.4 MB (1385271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac3ee3b23021de0471ff83e0b10babf764acf8f57dbb17c2eef966f084eb314a`  
		Last Modified: Thu, 23 Mar 2023 05:56:53 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1-standalone` - linux; arm variant v5

```console
$ docker pull adminer@sha256:6626a30d9f62f8886368c855059bbbe5324d5cd5a21cfcec9d74cd3f62f423b9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.2 MB (91190563 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:858d6152778fac7508d2b7edad80c80dd39df9946d1c4c17d9b0d7a9d4bb2e5a`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Wed, 12 Apr 2023 01:09:24 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 12 Apr 2023 01:09:24 GMT
WORKDIR /var/www/html
# Wed, 12 Apr 2023 01:09:24 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 12 Apr 2023 01:09:25 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 12 Apr 2023 01:09:25 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 12 Apr 2023 01:09:25 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 12 Apr 2023 01:09:40 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 12 Apr 2023 01:09:40 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 12 Apr 2023 01:09:40 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 12 Apr 2023 01:09:40 GMT
USER adminer
# Wed, 12 Apr 2023 01:09:40 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 12 Apr 2023 01:09:40 GMT
EXPOSE 8080
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
	-	`sha256:3f470d2089a740ebc67390ccf884d98cffb79eafd885a0c2b5e0e7b43e69c1c4`  
		Last Modified: Wed, 12 Apr 2023 01:10:10 GMT  
		Size: 1.9 KB (1869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a752232d0c61a7c17d3f25d15b89e4d34c73fd0bffe83dd92258b692f657abf6`  
		Last Modified: Wed, 12 Apr 2023 01:10:10 GMT  
		Size: 1.5 KB (1477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77ec5152fc80b31c2b1f1935c7cc639c14373654830cceb8dfe8602826b16b10`  
		Last Modified: Wed, 12 Apr 2023 01:10:10 GMT  
		Size: 1.4 MB (1385249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10633b8059422ad2e0f668cedeb61e0815df56a24bf954e381f2e8ff79b4caa1`  
		Last Modified: Wed, 12 Apr 2023 01:10:10 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1-standalone` - linux; arm variant v7

```console
$ docker pull adminer@sha256:208e28dc00b696fd2786ae0fac00bbac135df7d327a78f1a3b07b430e8be29fa
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.8 MB (87782361 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:924e553786350523e3dabd52a79ebaa532e1ee1f1cd4f55c123b6f2debfd887b`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Thu, 23 Mar 2023 13:54:17 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 23 Mar 2023 13:54:18 GMT
WORKDIR /var/www/html
# Thu, 23 Mar 2023 13:54:18 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 23 Mar 2023 13:54:18 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 23 Mar 2023 13:54:18 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 23 Mar 2023 13:54:18 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 23 Mar 2023 13:54:30 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Mar 2023 13:54:30 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 23 Mar 2023 13:54:30 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 23 Mar 2023 13:54:30 GMT
USER adminer
# Thu, 23 Mar 2023 13:54:30 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Thu, 23 Mar 2023 13:54:30 GMT
EXPOSE 8080
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
	-	`sha256:6c7b7c098bbce560d98941c87164725c63999c701f19f2500e91578c8d994c8f`  
		Last Modified: Thu, 23 Mar 2023 13:54:56 GMT  
		Size: 1.9 KB (1871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90441e257dd07454f7d03e5aa41e80d43c14256ff5040356a29d4639b23d75fc`  
		Last Modified: Thu, 23 Mar 2023 13:54:55 GMT  
		Size: 1.5 KB (1482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65767342491a731ec4afa7560fd1b162f1ea5c932fc69e8326baad4bec228e7e`  
		Last Modified: Thu, 23 Mar 2023 13:54:56 GMT  
		Size: 1.4 MB (1385066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6a8450e329b8116e25e9fa7cb6b678d57084c5946b3167f2cb126880295263a`  
		Last Modified: Thu, 23 Mar 2023 13:54:55 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1-standalone` - linux; arm64 variant v8

```console
$ docker pull adminer@sha256:4cda3605cfb6ed0b47e9d450e4d1e8979f04c8a969392e39ae82335de95323d0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.3 MB (94337798 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37e35dd000bf1a912aa2f6512bae1303bf816e1fd62882c26f65a39453286360`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Wed, 12 Apr 2023 01:01:29 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 12 Apr 2023 01:01:29 GMT
WORKDIR /var/www/html
# Wed, 12 Apr 2023 01:01:29 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 12 Apr 2023 01:01:29 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 12 Apr 2023 01:01:29 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 12 Apr 2023 01:01:29 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 12 Apr 2023 01:01:40 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 12 Apr 2023 01:01:40 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 12 Apr 2023 01:01:40 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 12 Apr 2023 01:01:40 GMT
USER adminer
# Wed, 12 Apr 2023 01:01:40 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 12 Apr 2023 01:01:41 GMT
EXPOSE 8080
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
	-	`sha256:905fbef16ad4dc303ccf2c51b20f40e565af53c2cc7a27bc3119ba72fde51908`  
		Last Modified: Wed, 12 Apr 2023 01:02:05 GMT  
		Size: 1.9 KB (1878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83a3dd0ad962d2f3c8153433aca615dc5bb81758ae2622916f28f9ed0e922f62`  
		Last Modified: Wed, 12 Apr 2023 01:02:05 GMT  
		Size: 1.5 KB (1477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cc2dd04f15e567448b396b8a8670939cb5dab2da2304657c79bf8e0b3bd1916`  
		Last Modified: Wed, 12 Apr 2023 01:02:05 GMT  
		Size: 1.4 MB (1385314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36c34adc9404de2e7b713240d2c5712e9eb8eb5a670fbd293da353414fbfbc5c`  
		Last Modified: Wed, 12 Apr 2023 01:02:05 GMT  
		Size: 489.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1-standalone` - linux; 386

```console
$ docker pull adminer@sha256:ca2ee65836fd06aba737873c17718cd1ae4e52f6ba9a2869000be6794922ec0d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.0 MB (96975396 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47306ce39706e8ed333600b8d4399cb09c02ffe4e169f76bd59fa5b6569ae778`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Thu, 23 Mar 2023 21:17:41 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 23 Mar 2023 21:17:41 GMT
WORKDIR /var/www/html
# Thu, 23 Mar 2023 21:17:42 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 23 Mar 2023 21:17:42 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 23 Mar 2023 21:17:42 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 23 Mar 2023 21:17:42 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 23 Mar 2023 21:17:54 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Mar 2023 21:17:54 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 23 Mar 2023 21:17:54 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 23 Mar 2023 21:17:54 GMT
USER adminer
# Thu, 23 Mar 2023 21:17:55 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Thu, 23 Mar 2023 21:17:55 GMT
EXPOSE 8080
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
	-	`sha256:7c664bb8231af50f8a98b457a9e7c291444345b0066ed54ddbcc0b2129859965`  
		Last Modified: Thu, 23 Mar 2023 21:18:24 GMT  
		Size: 1.9 KB (1869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6a209358917bcf344993c93aad3b156d6a09b6ab64d43df3941ca51e6c414b9`  
		Last Modified: Thu, 23 Mar 2023 21:18:24 GMT  
		Size: 1.5 KB (1476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:061ad9c8d5ae0dc7e0d69094e0f6d09b29dea00ec113641833b5a37f404de058`  
		Last Modified: Thu, 23 Mar 2023 21:18:24 GMT  
		Size: 1.4 MB (1385210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2761eeb066c4b63e66ada920b87fc430284439f4c76fac14a274ef528430d3f`  
		Last Modified: Thu, 23 Mar 2023 21:18:24 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1-standalone` - linux; mips64le

```console
$ docker pull adminer@sha256:14de06501f131ba9f62a814f592d766d6f050b30eab65a15bb1e753a436aab3d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.6 MB (92605785 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ddae0bdce53fcfedd28644c8fc0df52f38f44000615def4d84b2c88db2aff3ab`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Thu, 23 Mar 2023 20:08:09 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 23 Mar 2023 20:08:13 GMT
WORKDIR /var/www/html
# Thu, 23 Mar 2023 20:08:16 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 23 Mar 2023 20:08:19 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 23 Mar 2023 20:08:22 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 23 Mar 2023 20:08:26 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 23 Mar 2023 20:09:18 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Mar 2023 20:09:20 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 23 Mar 2023 20:09:24 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 23 Mar 2023 20:09:27 GMT
USER adminer
# Thu, 23 Mar 2023 20:09:31 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Thu, 23 Mar 2023 20:09:34 GMT
EXPOSE 8080
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
	-	`sha256:0ba90b5b3033a3d6ba607430a17c7e37f0fae8f0664ac81a4e571e9ad9fca9e2`  
		Last Modified: Thu, 23 Mar 2023 20:11:33 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b1980d6708cacd2f28ca074bd917c1143a47040b425da5985915850214f197f`  
		Last Modified: Thu, 23 Mar 2023 20:11:33 GMT  
		Size: 1.5 KB (1481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acfbeda1e7451034cf22503ff221351a0d3f5e1f63a6f11dc71a81450a7aaadd`  
		Last Modified: Thu, 23 Mar 2023 20:11:34 GMT  
		Size: 1.4 MB (1386264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b87439fd13726c64bed775edf40ceb3cbc1b5dbf3f62fb9b127024394aaece4`  
		Last Modified: Thu, 23 Mar 2023 20:11:33 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1-standalone` - linux; ppc64le

```console
$ docker pull adminer@sha256:a55a2c1ff24d027a36e46d24a34dcbb8e854ae5392eec85f9620ba60c7b58694
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.3 MB (101256116 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4735ee16dfbcee3a436e08438e55c6dd5114b673eec23b536b6b3a2f043a76ad`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Wed, 12 Apr 2023 01:20:37 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 12 Apr 2023 01:20:38 GMT
WORKDIR /var/www/html
# Wed, 12 Apr 2023 01:20:38 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 12 Apr 2023 01:20:39 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 12 Apr 2023 01:20:39 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 12 Apr 2023 01:20:40 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 12 Apr 2023 01:21:30 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 12 Apr 2023 01:21:31 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 12 Apr 2023 01:21:32 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 12 Apr 2023 01:21:34 GMT
USER adminer
# Wed, 12 Apr 2023 01:21:34 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 12 Apr 2023 01:21:35 GMT
EXPOSE 8080
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
	-	`sha256:79148517f43f66f402dd39c8ce8a6104a51fe03f3ed892be0eb40a2bf3ac513e`  
		Last Modified: Wed, 12 Apr 2023 01:22:40 GMT  
		Size: 1.9 KB (1879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67bc627fe6d1eed682ead8566e47d1e2328da8a1df7864e5a52ac7d20d815572`  
		Last Modified: Wed, 12 Apr 2023 01:22:40 GMT  
		Size: 1.5 KB (1481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8eb7bbdc982c8e7f315e96ecd620a4c3a9d486beb72d36f89daddaaca429d14`  
		Last Modified: Wed, 12 Apr 2023 01:22:41 GMT  
		Size: 1.4 MB (1385746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7f1791e7b6ab1e976b9698dd6aed465ae1b9badc2ae1c6b6cb91197748b149d`  
		Last Modified: Wed, 12 Apr 2023 01:22:40 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1-standalone` - linux; s390x

```console
$ docker pull adminer@sha256:5472a0984af7a0bcb4f370188898007842266789e4d9cd931aea7e05ffa0c318
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.7 MB (93694065 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f21ca8c09f92e5cedf5daa80fc0e9a2a1b8b7e032b3719641feadef4e6294cf5`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Wed, 12 Apr 2023 00:22:45 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 12 Apr 2023 00:22:45 GMT
WORKDIR /var/www/html
# Wed, 12 Apr 2023 00:22:45 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 12 Apr 2023 00:22:46 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 12 Apr 2023 00:22:46 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 12 Apr 2023 00:22:46 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 12 Apr 2023 00:22:57 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 12 Apr 2023 00:22:57 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 12 Apr 2023 00:22:57 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 12 Apr 2023 00:22:58 GMT
USER adminer
# Wed, 12 Apr 2023 00:22:58 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 12 Apr 2023 00:22:58 GMT
EXPOSE 8080
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
	-	`sha256:b23597fac1b0ce84055df85a56ef40909911286a24879b39f37200567f8e6e63`  
		Last Modified: Wed, 12 Apr 2023 00:23:41 GMT  
		Size: 1.9 KB (1879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e88da54b627b523974ad186c33e429711d0e4968550bc7b513fae7d58b9f3de1`  
		Last Modified: Wed, 12 Apr 2023 00:23:41 GMT  
		Size: 1.5 KB (1478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b8c6c7cf39dd303de3dcb8c7c363f95bfcf24b7dfbd409557940ced6e28cd6e`  
		Last Modified: Wed, 12 Apr 2023 00:23:41 GMT  
		Size: 1.4 MB (1385468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:640f1f42167e00265be1505a797a83c7cf74946f47391b62064c6fd44e4fee4d`  
		Last Modified: Wed, 12 Apr 2023 00:23:41 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

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

## `adminer:latest`

```console
$ docker pull adminer@sha256:47cb2b1d08526810b31337593d3de2a20a358498620ad53a28ef41dd13eb8c31
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
$ docker pull adminer@sha256:b5570962c3a9981b6572e61dd33f5cbd394a1a9d27ee6342b4241338af330449
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.9 MB (95921691 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5e1b3241b20061365693574e1c1241f64a48b15a7f439b8df760456d83009c7`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Thu, 23 Mar 2023 05:56:14 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 23 Mar 2023 05:56:14 GMT
WORKDIR /var/www/html
# Thu, 23 Mar 2023 05:56:14 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 23 Mar 2023 05:56:14 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 23 Mar 2023 05:56:14 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 23 Mar 2023 05:56:14 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 23 Mar 2023 05:56:25 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Mar 2023 05:56:26 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 23 Mar 2023 05:56:26 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 23 Mar 2023 05:56:26 GMT
USER adminer
# Thu, 23 Mar 2023 05:56:26 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Thu, 23 Mar 2023 05:56:26 GMT
EXPOSE 8080
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
	-	`sha256:39317196bba2d873b239492ba23f8f1d62f89b661fb1760b65f29b1404322c60`  
		Last Modified: Thu, 23 Mar 2023 05:56:53 GMT  
		Size: 1.9 KB (1879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31ea8e1da1f9854a8c3bf43a78f5b403bdfad3f2c2861edfbfd902566950a7a2`  
		Last Modified: Thu, 23 Mar 2023 05:56:53 GMT  
		Size: 1.5 KB (1477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3ce0ac056362cd982a31febaaf97daa568c31c2e95f1f4265e82cc6fbeaffd4`  
		Last Modified: Thu, 23 Mar 2023 05:56:53 GMT  
		Size: 1.4 MB (1385271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac3ee3b23021de0471ff83e0b10babf764acf8f57dbb17c2eef966f084eb314a`  
		Last Modified: Thu, 23 Mar 2023 05:56:53 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:latest` - linux; arm variant v5

```console
$ docker pull adminer@sha256:6626a30d9f62f8886368c855059bbbe5324d5cd5a21cfcec9d74cd3f62f423b9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.2 MB (91190563 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:858d6152778fac7508d2b7edad80c80dd39df9946d1c4c17d9b0d7a9d4bb2e5a`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Wed, 12 Apr 2023 01:09:24 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 12 Apr 2023 01:09:24 GMT
WORKDIR /var/www/html
# Wed, 12 Apr 2023 01:09:24 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 12 Apr 2023 01:09:25 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 12 Apr 2023 01:09:25 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 12 Apr 2023 01:09:25 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 12 Apr 2023 01:09:40 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 12 Apr 2023 01:09:40 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 12 Apr 2023 01:09:40 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 12 Apr 2023 01:09:40 GMT
USER adminer
# Wed, 12 Apr 2023 01:09:40 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 12 Apr 2023 01:09:40 GMT
EXPOSE 8080
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
	-	`sha256:3f470d2089a740ebc67390ccf884d98cffb79eafd885a0c2b5e0e7b43e69c1c4`  
		Last Modified: Wed, 12 Apr 2023 01:10:10 GMT  
		Size: 1.9 KB (1869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a752232d0c61a7c17d3f25d15b89e4d34c73fd0bffe83dd92258b692f657abf6`  
		Last Modified: Wed, 12 Apr 2023 01:10:10 GMT  
		Size: 1.5 KB (1477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77ec5152fc80b31c2b1f1935c7cc639c14373654830cceb8dfe8602826b16b10`  
		Last Modified: Wed, 12 Apr 2023 01:10:10 GMT  
		Size: 1.4 MB (1385249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10633b8059422ad2e0f668cedeb61e0815df56a24bf954e381f2e8ff79b4caa1`  
		Last Modified: Wed, 12 Apr 2023 01:10:10 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:latest` - linux; arm variant v7

```console
$ docker pull adminer@sha256:208e28dc00b696fd2786ae0fac00bbac135df7d327a78f1a3b07b430e8be29fa
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.8 MB (87782361 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:924e553786350523e3dabd52a79ebaa532e1ee1f1cd4f55c123b6f2debfd887b`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Thu, 23 Mar 2023 13:54:17 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 23 Mar 2023 13:54:18 GMT
WORKDIR /var/www/html
# Thu, 23 Mar 2023 13:54:18 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 23 Mar 2023 13:54:18 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 23 Mar 2023 13:54:18 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 23 Mar 2023 13:54:18 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 23 Mar 2023 13:54:30 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Mar 2023 13:54:30 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 23 Mar 2023 13:54:30 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 23 Mar 2023 13:54:30 GMT
USER adminer
# Thu, 23 Mar 2023 13:54:30 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Thu, 23 Mar 2023 13:54:30 GMT
EXPOSE 8080
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
	-	`sha256:6c7b7c098bbce560d98941c87164725c63999c701f19f2500e91578c8d994c8f`  
		Last Modified: Thu, 23 Mar 2023 13:54:56 GMT  
		Size: 1.9 KB (1871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90441e257dd07454f7d03e5aa41e80d43c14256ff5040356a29d4639b23d75fc`  
		Last Modified: Thu, 23 Mar 2023 13:54:55 GMT  
		Size: 1.5 KB (1482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65767342491a731ec4afa7560fd1b162f1ea5c932fc69e8326baad4bec228e7e`  
		Last Modified: Thu, 23 Mar 2023 13:54:56 GMT  
		Size: 1.4 MB (1385066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6a8450e329b8116e25e9fa7cb6b678d57084c5946b3167f2cb126880295263a`  
		Last Modified: Thu, 23 Mar 2023 13:54:55 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:latest` - linux; arm64 variant v8

```console
$ docker pull adminer@sha256:4cda3605cfb6ed0b47e9d450e4d1e8979f04c8a969392e39ae82335de95323d0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.3 MB (94337798 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37e35dd000bf1a912aa2f6512bae1303bf816e1fd62882c26f65a39453286360`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Wed, 12 Apr 2023 01:01:29 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 12 Apr 2023 01:01:29 GMT
WORKDIR /var/www/html
# Wed, 12 Apr 2023 01:01:29 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 12 Apr 2023 01:01:29 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 12 Apr 2023 01:01:29 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 12 Apr 2023 01:01:29 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 12 Apr 2023 01:01:40 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 12 Apr 2023 01:01:40 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 12 Apr 2023 01:01:40 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 12 Apr 2023 01:01:40 GMT
USER adminer
# Wed, 12 Apr 2023 01:01:40 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 12 Apr 2023 01:01:41 GMT
EXPOSE 8080
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
	-	`sha256:905fbef16ad4dc303ccf2c51b20f40e565af53c2cc7a27bc3119ba72fde51908`  
		Last Modified: Wed, 12 Apr 2023 01:02:05 GMT  
		Size: 1.9 KB (1878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83a3dd0ad962d2f3c8153433aca615dc5bb81758ae2622916f28f9ed0e922f62`  
		Last Modified: Wed, 12 Apr 2023 01:02:05 GMT  
		Size: 1.5 KB (1477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cc2dd04f15e567448b396b8a8670939cb5dab2da2304657c79bf8e0b3bd1916`  
		Last Modified: Wed, 12 Apr 2023 01:02:05 GMT  
		Size: 1.4 MB (1385314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36c34adc9404de2e7b713240d2c5712e9eb8eb5a670fbd293da353414fbfbc5c`  
		Last Modified: Wed, 12 Apr 2023 01:02:05 GMT  
		Size: 489.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:latest` - linux; 386

```console
$ docker pull adminer@sha256:ca2ee65836fd06aba737873c17718cd1ae4e52f6ba9a2869000be6794922ec0d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.0 MB (96975396 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47306ce39706e8ed333600b8d4399cb09c02ffe4e169f76bd59fa5b6569ae778`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Thu, 23 Mar 2023 21:17:41 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 23 Mar 2023 21:17:41 GMT
WORKDIR /var/www/html
# Thu, 23 Mar 2023 21:17:42 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 23 Mar 2023 21:17:42 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 23 Mar 2023 21:17:42 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 23 Mar 2023 21:17:42 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 23 Mar 2023 21:17:54 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Mar 2023 21:17:54 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 23 Mar 2023 21:17:54 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 23 Mar 2023 21:17:54 GMT
USER adminer
# Thu, 23 Mar 2023 21:17:55 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Thu, 23 Mar 2023 21:17:55 GMT
EXPOSE 8080
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
	-	`sha256:7c664bb8231af50f8a98b457a9e7c291444345b0066ed54ddbcc0b2129859965`  
		Last Modified: Thu, 23 Mar 2023 21:18:24 GMT  
		Size: 1.9 KB (1869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6a209358917bcf344993c93aad3b156d6a09b6ab64d43df3941ca51e6c414b9`  
		Last Modified: Thu, 23 Mar 2023 21:18:24 GMT  
		Size: 1.5 KB (1476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:061ad9c8d5ae0dc7e0d69094e0f6d09b29dea00ec113641833b5a37f404de058`  
		Last Modified: Thu, 23 Mar 2023 21:18:24 GMT  
		Size: 1.4 MB (1385210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2761eeb066c4b63e66ada920b87fc430284439f4c76fac14a274ef528430d3f`  
		Last Modified: Thu, 23 Mar 2023 21:18:24 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:latest` - linux; mips64le

```console
$ docker pull adminer@sha256:14de06501f131ba9f62a814f592d766d6f050b30eab65a15bb1e753a436aab3d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.6 MB (92605785 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ddae0bdce53fcfedd28644c8fc0df52f38f44000615def4d84b2c88db2aff3ab`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Thu, 23 Mar 2023 20:08:09 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 23 Mar 2023 20:08:13 GMT
WORKDIR /var/www/html
# Thu, 23 Mar 2023 20:08:16 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 23 Mar 2023 20:08:19 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 23 Mar 2023 20:08:22 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 23 Mar 2023 20:08:26 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 23 Mar 2023 20:09:18 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Mar 2023 20:09:20 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 23 Mar 2023 20:09:24 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 23 Mar 2023 20:09:27 GMT
USER adminer
# Thu, 23 Mar 2023 20:09:31 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Thu, 23 Mar 2023 20:09:34 GMT
EXPOSE 8080
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
	-	`sha256:0ba90b5b3033a3d6ba607430a17c7e37f0fae8f0664ac81a4e571e9ad9fca9e2`  
		Last Modified: Thu, 23 Mar 2023 20:11:33 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b1980d6708cacd2f28ca074bd917c1143a47040b425da5985915850214f197f`  
		Last Modified: Thu, 23 Mar 2023 20:11:33 GMT  
		Size: 1.5 KB (1481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acfbeda1e7451034cf22503ff221351a0d3f5e1f63a6f11dc71a81450a7aaadd`  
		Last Modified: Thu, 23 Mar 2023 20:11:34 GMT  
		Size: 1.4 MB (1386264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b87439fd13726c64bed775edf40ceb3cbc1b5dbf3f62fb9b127024394aaece4`  
		Last Modified: Thu, 23 Mar 2023 20:11:33 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:latest` - linux; ppc64le

```console
$ docker pull adminer@sha256:a55a2c1ff24d027a36e46d24a34dcbb8e854ae5392eec85f9620ba60c7b58694
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.3 MB (101256116 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4735ee16dfbcee3a436e08438e55c6dd5114b673eec23b536b6b3a2f043a76ad`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Wed, 12 Apr 2023 01:20:37 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 12 Apr 2023 01:20:38 GMT
WORKDIR /var/www/html
# Wed, 12 Apr 2023 01:20:38 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 12 Apr 2023 01:20:39 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 12 Apr 2023 01:20:39 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 12 Apr 2023 01:20:40 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 12 Apr 2023 01:21:30 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 12 Apr 2023 01:21:31 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 12 Apr 2023 01:21:32 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 12 Apr 2023 01:21:34 GMT
USER adminer
# Wed, 12 Apr 2023 01:21:34 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 12 Apr 2023 01:21:35 GMT
EXPOSE 8080
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
	-	`sha256:79148517f43f66f402dd39c8ce8a6104a51fe03f3ed892be0eb40a2bf3ac513e`  
		Last Modified: Wed, 12 Apr 2023 01:22:40 GMT  
		Size: 1.9 KB (1879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67bc627fe6d1eed682ead8566e47d1e2328da8a1df7864e5a52ac7d20d815572`  
		Last Modified: Wed, 12 Apr 2023 01:22:40 GMT  
		Size: 1.5 KB (1481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8eb7bbdc982c8e7f315e96ecd620a4c3a9d486beb72d36f89daddaaca429d14`  
		Last Modified: Wed, 12 Apr 2023 01:22:41 GMT  
		Size: 1.4 MB (1385746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7f1791e7b6ab1e976b9698dd6aed465ae1b9badc2ae1c6b6cb91197748b149d`  
		Last Modified: Wed, 12 Apr 2023 01:22:40 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:latest` - linux; s390x

```console
$ docker pull adminer@sha256:5472a0984af7a0bcb4f370188898007842266789e4d9cd931aea7e05ffa0c318
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.7 MB (93694065 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f21ca8c09f92e5cedf5daa80fc0e9a2a1b8b7e032b3719641feadef4e6294cf5`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Wed, 12 Apr 2023 00:22:45 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 12 Apr 2023 00:22:45 GMT
WORKDIR /var/www/html
# Wed, 12 Apr 2023 00:22:45 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 12 Apr 2023 00:22:46 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 12 Apr 2023 00:22:46 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 12 Apr 2023 00:22:46 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 12 Apr 2023 00:22:57 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 12 Apr 2023 00:22:57 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 12 Apr 2023 00:22:57 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 12 Apr 2023 00:22:58 GMT
USER adminer
# Wed, 12 Apr 2023 00:22:58 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 12 Apr 2023 00:22:58 GMT
EXPOSE 8080
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
	-	`sha256:b23597fac1b0ce84055df85a56ef40909911286a24879b39f37200567f8e6e63`  
		Last Modified: Wed, 12 Apr 2023 00:23:41 GMT  
		Size: 1.9 KB (1879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e88da54b627b523974ad186c33e429711d0e4968550bc7b513fae7d58b9f3de1`  
		Last Modified: Wed, 12 Apr 2023 00:23:41 GMT  
		Size: 1.5 KB (1478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b8c6c7cf39dd303de3dcb8c7c363f95bfcf24b7dfbd409557940ced6e28cd6e`  
		Last Modified: Wed, 12 Apr 2023 00:23:41 GMT  
		Size: 1.4 MB (1385468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:640f1f42167e00265be1505a797a83c7cf74946f47391b62064c6fd44e4fee4d`  
		Last Modified: Wed, 12 Apr 2023 00:23:41 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `adminer:standalone`

```console
$ docker pull adminer@sha256:47cb2b1d08526810b31337593d3de2a20a358498620ad53a28ef41dd13eb8c31
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
$ docker pull adminer@sha256:b5570962c3a9981b6572e61dd33f5cbd394a1a9d27ee6342b4241338af330449
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.9 MB (95921691 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5e1b3241b20061365693574e1c1241f64a48b15a7f439b8df760456d83009c7`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Thu, 23 Mar 2023 05:56:14 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 23 Mar 2023 05:56:14 GMT
WORKDIR /var/www/html
# Thu, 23 Mar 2023 05:56:14 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 23 Mar 2023 05:56:14 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 23 Mar 2023 05:56:14 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 23 Mar 2023 05:56:14 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 23 Mar 2023 05:56:25 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Mar 2023 05:56:26 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 23 Mar 2023 05:56:26 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 23 Mar 2023 05:56:26 GMT
USER adminer
# Thu, 23 Mar 2023 05:56:26 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Thu, 23 Mar 2023 05:56:26 GMT
EXPOSE 8080
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
	-	`sha256:39317196bba2d873b239492ba23f8f1d62f89b661fb1760b65f29b1404322c60`  
		Last Modified: Thu, 23 Mar 2023 05:56:53 GMT  
		Size: 1.9 KB (1879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31ea8e1da1f9854a8c3bf43a78f5b403bdfad3f2c2861edfbfd902566950a7a2`  
		Last Modified: Thu, 23 Mar 2023 05:56:53 GMT  
		Size: 1.5 KB (1477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3ce0ac056362cd982a31febaaf97daa568c31c2e95f1f4265e82cc6fbeaffd4`  
		Last Modified: Thu, 23 Mar 2023 05:56:53 GMT  
		Size: 1.4 MB (1385271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac3ee3b23021de0471ff83e0b10babf764acf8f57dbb17c2eef966f084eb314a`  
		Last Modified: Thu, 23 Mar 2023 05:56:53 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:standalone` - linux; arm variant v5

```console
$ docker pull adminer@sha256:6626a30d9f62f8886368c855059bbbe5324d5cd5a21cfcec9d74cd3f62f423b9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.2 MB (91190563 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:858d6152778fac7508d2b7edad80c80dd39df9946d1c4c17d9b0d7a9d4bb2e5a`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Wed, 12 Apr 2023 01:09:24 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 12 Apr 2023 01:09:24 GMT
WORKDIR /var/www/html
# Wed, 12 Apr 2023 01:09:24 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 12 Apr 2023 01:09:25 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 12 Apr 2023 01:09:25 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 12 Apr 2023 01:09:25 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 12 Apr 2023 01:09:40 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 12 Apr 2023 01:09:40 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 12 Apr 2023 01:09:40 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 12 Apr 2023 01:09:40 GMT
USER adminer
# Wed, 12 Apr 2023 01:09:40 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 12 Apr 2023 01:09:40 GMT
EXPOSE 8080
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
	-	`sha256:3f470d2089a740ebc67390ccf884d98cffb79eafd885a0c2b5e0e7b43e69c1c4`  
		Last Modified: Wed, 12 Apr 2023 01:10:10 GMT  
		Size: 1.9 KB (1869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a752232d0c61a7c17d3f25d15b89e4d34c73fd0bffe83dd92258b692f657abf6`  
		Last Modified: Wed, 12 Apr 2023 01:10:10 GMT  
		Size: 1.5 KB (1477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77ec5152fc80b31c2b1f1935c7cc639c14373654830cceb8dfe8602826b16b10`  
		Last Modified: Wed, 12 Apr 2023 01:10:10 GMT  
		Size: 1.4 MB (1385249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10633b8059422ad2e0f668cedeb61e0815df56a24bf954e381f2e8ff79b4caa1`  
		Last Modified: Wed, 12 Apr 2023 01:10:10 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:standalone` - linux; arm variant v7

```console
$ docker pull adminer@sha256:208e28dc00b696fd2786ae0fac00bbac135df7d327a78f1a3b07b430e8be29fa
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.8 MB (87782361 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:924e553786350523e3dabd52a79ebaa532e1ee1f1cd4f55c123b6f2debfd887b`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Thu, 23 Mar 2023 13:54:17 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 23 Mar 2023 13:54:18 GMT
WORKDIR /var/www/html
# Thu, 23 Mar 2023 13:54:18 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 23 Mar 2023 13:54:18 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 23 Mar 2023 13:54:18 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 23 Mar 2023 13:54:18 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 23 Mar 2023 13:54:30 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Mar 2023 13:54:30 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 23 Mar 2023 13:54:30 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 23 Mar 2023 13:54:30 GMT
USER adminer
# Thu, 23 Mar 2023 13:54:30 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Thu, 23 Mar 2023 13:54:30 GMT
EXPOSE 8080
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
	-	`sha256:6c7b7c098bbce560d98941c87164725c63999c701f19f2500e91578c8d994c8f`  
		Last Modified: Thu, 23 Mar 2023 13:54:56 GMT  
		Size: 1.9 KB (1871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90441e257dd07454f7d03e5aa41e80d43c14256ff5040356a29d4639b23d75fc`  
		Last Modified: Thu, 23 Mar 2023 13:54:55 GMT  
		Size: 1.5 KB (1482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65767342491a731ec4afa7560fd1b162f1ea5c932fc69e8326baad4bec228e7e`  
		Last Modified: Thu, 23 Mar 2023 13:54:56 GMT  
		Size: 1.4 MB (1385066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6a8450e329b8116e25e9fa7cb6b678d57084c5946b3167f2cb126880295263a`  
		Last Modified: Thu, 23 Mar 2023 13:54:55 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:standalone` - linux; arm64 variant v8

```console
$ docker pull adminer@sha256:4cda3605cfb6ed0b47e9d450e4d1e8979f04c8a969392e39ae82335de95323d0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.3 MB (94337798 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37e35dd000bf1a912aa2f6512bae1303bf816e1fd62882c26f65a39453286360`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Wed, 12 Apr 2023 01:01:29 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 12 Apr 2023 01:01:29 GMT
WORKDIR /var/www/html
# Wed, 12 Apr 2023 01:01:29 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 12 Apr 2023 01:01:29 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 12 Apr 2023 01:01:29 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 12 Apr 2023 01:01:29 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 12 Apr 2023 01:01:40 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 12 Apr 2023 01:01:40 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 12 Apr 2023 01:01:40 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 12 Apr 2023 01:01:40 GMT
USER adminer
# Wed, 12 Apr 2023 01:01:40 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 12 Apr 2023 01:01:41 GMT
EXPOSE 8080
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
	-	`sha256:905fbef16ad4dc303ccf2c51b20f40e565af53c2cc7a27bc3119ba72fde51908`  
		Last Modified: Wed, 12 Apr 2023 01:02:05 GMT  
		Size: 1.9 KB (1878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83a3dd0ad962d2f3c8153433aca615dc5bb81758ae2622916f28f9ed0e922f62`  
		Last Modified: Wed, 12 Apr 2023 01:02:05 GMT  
		Size: 1.5 KB (1477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cc2dd04f15e567448b396b8a8670939cb5dab2da2304657c79bf8e0b3bd1916`  
		Last Modified: Wed, 12 Apr 2023 01:02:05 GMT  
		Size: 1.4 MB (1385314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36c34adc9404de2e7b713240d2c5712e9eb8eb5a670fbd293da353414fbfbc5c`  
		Last Modified: Wed, 12 Apr 2023 01:02:05 GMT  
		Size: 489.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:standalone` - linux; 386

```console
$ docker pull adminer@sha256:ca2ee65836fd06aba737873c17718cd1ae4e52f6ba9a2869000be6794922ec0d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.0 MB (96975396 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47306ce39706e8ed333600b8d4399cb09c02ffe4e169f76bd59fa5b6569ae778`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Thu, 23 Mar 2023 21:17:41 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 23 Mar 2023 21:17:41 GMT
WORKDIR /var/www/html
# Thu, 23 Mar 2023 21:17:42 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 23 Mar 2023 21:17:42 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 23 Mar 2023 21:17:42 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 23 Mar 2023 21:17:42 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 23 Mar 2023 21:17:54 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Mar 2023 21:17:54 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 23 Mar 2023 21:17:54 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 23 Mar 2023 21:17:54 GMT
USER adminer
# Thu, 23 Mar 2023 21:17:55 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Thu, 23 Mar 2023 21:17:55 GMT
EXPOSE 8080
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
	-	`sha256:7c664bb8231af50f8a98b457a9e7c291444345b0066ed54ddbcc0b2129859965`  
		Last Modified: Thu, 23 Mar 2023 21:18:24 GMT  
		Size: 1.9 KB (1869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6a209358917bcf344993c93aad3b156d6a09b6ab64d43df3941ca51e6c414b9`  
		Last Modified: Thu, 23 Mar 2023 21:18:24 GMT  
		Size: 1.5 KB (1476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:061ad9c8d5ae0dc7e0d69094e0f6d09b29dea00ec113641833b5a37f404de058`  
		Last Modified: Thu, 23 Mar 2023 21:18:24 GMT  
		Size: 1.4 MB (1385210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2761eeb066c4b63e66ada920b87fc430284439f4c76fac14a274ef528430d3f`  
		Last Modified: Thu, 23 Mar 2023 21:18:24 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:standalone` - linux; mips64le

```console
$ docker pull adminer@sha256:14de06501f131ba9f62a814f592d766d6f050b30eab65a15bb1e753a436aab3d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.6 MB (92605785 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ddae0bdce53fcfedd28644c8fc0df52f38f44000615def4d84b2c88db2aff3ab`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Thu, 23 Mar 2023 20:08:09 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 23 Mar 2023 20:08:13 GMT
WORKDIR /var/www/html
# Thu, 23 Mar 2023 20:08:16 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 23 Mar 2023 20:08:19 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 23 Mar 2023 20:08:22 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 23 Mar 2023 20:08:26 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 23 Mar 2023 20:09:18 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Mar 2023 20:09:20 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 23 Mar 2023 20:09:24 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 23 Mar 2023 20:09:27 GMT
USER adminer
# Thu, 23 Mar 2023 20:09:31 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Thu, 23 Mar 2023 20:09:34 GMT
EXPOSE 8080
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
	-	`sha256:0ba90b5b3033a3d6ba607430a17c7e37f0fae8f0664ac81a4e571e9ad9fca9e2`  
		Last Modified: Thu, 23 Mar 2023 20:11:33 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b1980d6708cacd2f28ca074bd917c1143a47040b425da5985915850214f197f`  
		Last Modified: Thu, 23 Mar 2023 20:11:33 GMT  
		Size: 1.5 KB (1481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acfbeda1e7451034cf22503ff221351a0d3f5e1f63a6f11dc71a81450a7aaadd`  
		Last Modified: Thu, 23 Mar 2023 20:11:34 GMT  
		Size: 1.4 MB (1386264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b87439fd13726c64bed775edf40ceb3cbc1b5dbf3f62fb9b127024394aaece4`  
		Last Modified: Thu, 23 Mar 2023 20:11:33 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:standalone` - linux; ppc64le

```console
$ docker pull adminer@sha256:a55a2c1ff24d027a36e46d24a34dcbb8e854ae5392eec85f9620ba60c7b58694
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.3 MB (101256116 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4735ee16dfbcee3a436e08438e55c6dd5114b673eec23b536b6b3a2f043a76ad`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Wed, 12 Apr 2023 01:20:37 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 12 Apr 2023 01:20:38 GMT
WORKDIR /var/www/html
# Wed, 12 Apr 2023 01:20:38 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 12 Apr 2023 01:20:39 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 12 Apr 2023 01:20:39 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 12 Apr 2023 01:20:40 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 12 Apr 2023 01:21:30 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 12 Apr 2023 01:21:31 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 12 Apr 2023 01:21:32 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 12 Apr 2023 01:21:34 GMT
USER adminer
# Wed, 12 Apr 2023 01:21:34 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 12 Apr 2023 01:21:35 GMT
EXPOSE 8080
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
	-	`sha256:79148517f43f66f402dd39c8ce8a6104a51fe03f3ed892be0eb40a2bf3ac513e`  
		Last Modified: Wed, 12 Apr 2023 01:22:40 GMT  
		Size: 1.9 KB (1879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67bc627fe6d1eed682ead8566e47d1e2328da8a1df7864e5a52ac7d20d815572`  
		Last Modified: Wed, 12 Apr 2023 01:22:40 GMT  
		Size: 1.5 KB (1481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8eb7bbdc982c8e7f315e96ecd620a4c3a9d486beb72d36f89daddaaca429d14`  
		Last Modified: Wed, 12 Apr 2023 01:22:41 GMT  
		Size: 1.4 MB (1385746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7f1791e7b6ab1e976b9698dd6aed465ae1b9badc2ae1c6b6cb91197748b149d`  
		Last Modified: Wed, 12 Apr 2023 01:22:40 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:standalone` - linux; s390x

```console
$ docker pull adminer@sha256:5472a0984af7a0bcb4f370188898007842266789e4d9cd931aea7e05ffa0c318
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.7 MB (93694065 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f21ca8c09f92e5cedf5daa80fc0e9a2a1b8b7e032b3719641feadef4e6294cf5`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Wed, 12 Apr 2023 00:22:45 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 12 Apr 2023 00:22:45 GMT
WORKDIR /var/www/html
# Wed, 12 Apr 2023 00:22:45 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 12 Apr 2023 00:22:46 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 12 Apr 2023 00:22:46 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 12 Apr 2023 00:22:46 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 12 Apr 2023 00:22:57 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 12 Apr 2023 00:22:57 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 12 Apr 2023 00:22:57 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 12 Apr 2023 00:22:58 GMT
USER adminer
# Wed, 12 Apr 2023 00:22:58 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 12 Apr 2023 00:22:58 GMT
EXPOSE 8080
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
	-	`sha256:b23597fac1b0ce84055df85a56ef40909911286a24879b39f37200567f8e6e63`  
		Last Modified: Wed, 12 Apr 2023 00:23:41 GMT  
		Size: 1.9 KB (1879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e88da54b627b523974ad186c33e429711d0e4968550bc7b513fae7d58b9f3de1`  
		Last Modified: Wed, 12 Apr 2023 00:23:41 GMT  
		Size: 1.5 KB (1478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b8c6c7cf39dd303de3dcb8c7c363f95bfcf24b7dfbd409557940ced6e28cd6e`  
		Last Modified: Wed, 12 Apr 2023 00:23:41 GMT  
		Size: 1.4 MB (1385468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:640f1f42167e00265be1505a797a83c7cf74946f47391b62064c6fd44e4fee4d`  
		Last Modified: Wed, 12 Apr 2023 00:23:41 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
