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
$ docker pull adminer@sha256:cc582ae15c97b6e8c726519b17004e819016dd11d6fda5f5898361575c435236
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
$ docker pull adminer@sha256:eea72a21cf1f4a95a5369ea76cbcfcd253974d1f2bc6fff6129ecc07a8cb996c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.9 MB (95941425 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a935a78b9b29f6ad7c46d08e6266a8419f6f0f355bb0b017f7320b381a7a9dc`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 11 Oct 2023 18:35:01 GMT
ADD file:8a9222387b89a9ac763fd72610ce01ab17f64387cbfde30a6af1861a82030aad in / 
# Wed, 11 Oct 2023 18:35:01 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 21:37:54 GMT
STOPSIGNAL SIGINT
# Wed, 11 Oct 2023 21:38:15 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 21:38:15 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 11 Oct 2023 21:38:16 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 11 Oct 2023 21:38:16 GMT
WORKDIR /var/www/html
# Wed, 11 Oct 2023 21:38:16 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 11 Oct 2023 21:38:16 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 11 Oct 2023 21:38:16 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 11 Oct 2023 21:38:16 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 11 Oct 2023 21:38:28 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 11 Oct 2023 21:38:28 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 11 Oct 2023 21:38:28 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 11 Oct 2023 21:38:28 GMT
USER adminer
# Wed, 11 Oct 2023 21:38:28 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 11 Oct 2023 21:38:28 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:69b3efbf67c2d9a46fdfdc8480b5a03ef73e9999a53aad57213447784f01eb6e`  
		Last Modified: Wed, 11 Oct 2023 18:39:54 GMT  
		Size: 55.1 MB (55058028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a0fdd089fb3c19ecd415c0ec8697e76347c06547c6418f4e0c2598cf3e6a396`  
		Last Modified: Wed, 11 Oct 2023 21:39:07 GMT  
		Size: 39.5 MB (39492762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:689786b0c396fae2f867afea8b0678012d77de73f01087f0b87b2f65d69160e0`  
		Last Modified: Wed, 11 Oct 2023 21:39:00 GMT  
		Size: 388.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bcf42cdb6b507c0e95ea21dd205b3073a3cc03072bc5ecb0984571c9319a61b`  
		Last Modified: Wed, 11 Oct 2023 21:39:00 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d507b34ef5ac1588f61ab244f00d1d6c16c10c1b722ca88d305807950d239bda`  
		Last Modified: Wed, 11 Oct 2023 21:39:00 GMT  
		Size: 1.5 KB (1475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04b8d4f964a85630221b12d10d1dcc6b918a66337213d36c6d0e58d88684181f`  
		Last Modified: Wed, 11 Oct 2023 21:39:01 GMT  
		Size: 1.4 MB (1386398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a75f8703cd73af4a5226ed8767f2f4bb39476c3f3c65b2263700ef30f709ccd`  
		Last Modified: Wed, 11 Oct 2023 21:39:00 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4` - linux; arm variant v5

```console
$ docker pull adminer@sha256:a08d5ea30e6d3820954b4fabeaf9249a32a7b7572327ca1dd743b38f0cbd888f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.2 MB (91203171 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:baca868e51087a0125257821115f40dcdd565feb2f02c131e0752c41bf7edb03`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Wed, 11 Oct 2023 18:02:54 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 11 Oct 2023 18:02:55 GMT
WORKDIR /var/www/html
# Wed, 11 Oct 2023 18:02:55 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 11 Oct 2023 18:02:55 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 11 Oct 2023 18:02:55 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 11 Oct 2023 18:02:55 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 11 Oct 2023 18:03:10 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 11 Oct 2023 18:03:10 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 11 Oct 2023 18:03:10 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 11 Oct 2023 18:03:10 GMT
USER adminer
# Wed, 11 Oct 2023 18:03:11 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 11 Oct 2023 18:03:11 GMT
EXPOSE 8080
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
	-	`sha256:f882441c27deeb5eb8fbd7f5966d960e7df16b93ecdca98b2eda933479843de2`  
		Last Modified: Wed, 11 Oct 2023 18:03:47 GMT  
		Size: 1.9 KB (1871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5de4c1ac09f4beb23be8f166d5ac9e50f027246da8b704d4dcd1f55c56b1b293`  
		Last Modified: Wed, 11 Oct 2023 18:03:47 GMT  
		Size: 1.5 KB (1476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b04a8ddeb2dbd66e060775b6f617eb9966bc57bfe4a9188119fdce9f8b24305e`  
		Last Modified: Wed, 11 Oct 2023 18:03:47 GMT  
		Size: 1.4 MB (1386290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:574521a263f70127c05a1db8391a9f33d18c5844caaea07ea781626bd2156092`  
		Last Modified: Wed, 11 Oct 2023 18:03:47 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4` - linux; arm variant v7

```console
$ docker pull adminer@sha256:6690c92a774eeb7b3a4bd31947c0641da6f80e18d3d9b38ff91869472cbc4203
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.8 MB (87794407 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb1b05568fc173e70d7da07ef277288dd9dd7fc76372fe16397945516ed0a194`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 11 Oct 2023 17:42:19 GMT
ADD file:684f3634c6b747a4caad8f9f820cc02b53a2122591fe215935c5497ec234c3ad in / 
# Wed, 11 Oct 2023 17:42:20 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:07:19 GMT
STOPSIGNAL SIGINT
# Wed, 11 Oct 2023 18:07:44 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 18:07:45 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 11 Oct 2023 18:07:45 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 11 Oct 2023 18:07:45 GMT
WORKDIR /var/www/html
# Wed, 11 Oct 2023 18:07:45 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 11 Oct 2023 18:07:46 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 11 Oct 2023 18:07:46 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 11 Oct 2023 18:07:46 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 11 Oct 2023 18:07:59 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 11 Oct 2023 18:08:00 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 11 Oct 2023 18:08:00 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 11 Oct 2023 18:08:00 GMT
USER adminer
# Wed, 11 Oct 2023 18:08:00 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 11 Oct 2023 18:08:00 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:33d0c7672db93e653471872c639cd6129ec25c168942e15a008c4920cafe62d7`  
		Last Modified: Wed, 11 Oct 2023 17:46:42 GMT  
		Size: 50.2 MB (50215704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7566087b942379bfc2c6a78692dbbe71d4bd1573cb81ddf2ece5c0c93bf1fe76`  
		Last Modified: Wed, 11 Oct 2023 18:08:44 GMT  
		Size: 36.2 MB (36188142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:050d8c68cbad80d1919f535fae7d348cde6b6488d6688095aa47dadb0de2a8cf`  
		Last Modified: Wed, 11 Oct 2023 18:08:34 GMT  
		Size: 394.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbd3cd900e2690837d6a8cbd717999c5224939f51724c7b2ec553c1419e5ab86`  
		Last Modified: Wed, 11 Oct 2023 18:08:34 GMT  
		Size: 1.9 KB (1871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cce366bf543cd120f357c96573fa045f6c544189b422cbc2d49121b993af5e97`  
		Last Modified: Wed, 11 Oct 2023 18:08:34 GMT  
		Size: 1.5 KB (1476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff97645728e1b3ae0f3d4382f2919cf8e8f896b310af1b8a020cf1a4d4a151ce`  
		Last Modified: Wed, 11 Oct 2023 18:08:34 GMT  
		Size: 1.4 MB (1386329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa31a5f1d18ca530111bc2c3cc0da34e10ab6329822a5c075549811eda2e985b`  
		Last Modified: Wed, 11 Oct 2023 18:08:34 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4` - linux; arm64 variant v8

```console
$ docker pull adminer@sha256:af7089fbd20cb08f11edf0f60a254b18f0c90a32537952e5258781d4c2d9f2c7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.3 MB (94344062 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc6c706282e894e9fe8fabf7c797478428c1166e8f93f09e43c8db0a12d0da49`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 11 Oct 2023 18:24:58 GMT
ADD file:e1a6c6c976e5e7c53eb2a7343a7a763b46e56828588535f4c79e63d6ec08198d in / 
# Wed, 11 Oct 2023 18:24:58 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 19:41:39 GMT
STOPSIGNAL SIGINT
# Wed, 11 Oct 2023 19:41:57 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 19:41:58 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 11 Oct 2023 19:41:59 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 11 Oct 2023 19:41:59 GMT
WORKDIR /var/www/html
# Wed, 11 Oct 2023 19:41:59 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 11 Oct 2023 19:41:59 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 11 Oct 2023 19:41:59 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 11 Oct 2023 19:41:59 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 11 Oct 2023 19:42:10 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 11 Oct 2023 19:42:10 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 11 Oct 2023 19:42:10 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 11 Oct 2023 19:42:10 GMT
USER adminer
# Wed, 11 Oct 2023 19:42:10 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 11 Oct 2023 19:42:10 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:dd0dc10f921f4b3b65b17f20d367374079e6cb4e26531624ee64caaaf4adcc28`  
		Last Modified: Wed, 11 Oct 2023 18:28:45 GMT  
		Size: 53.7 MB (53707810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef257294e6993147657842c1db0af6b35567fa3f5f825478621ef5bf09c4871e`  
		Last Modified: Wed, 11 Oct 2023 19:42:42 GMT  
		Size: 39.2 MB (39245727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e6ecde2f3d45f8a48e3c2d5c819eb535ac0f9abdde2051c01995434568dbf32`  
		Last Modified: Wed, 11 Oct 2023 19:42:35 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:600639d0d6dc1311b99169e0d63c4eb8f44bf21239f7000efc992a95063feb0e`  
		Last Modified: Wed, 11 Oct 2023 19:42:35 GMT  
		Size: 1.9 KB (1893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd2c7fb421d92b300b1834fa1788dc075e72d3d714336d0ce5986fb9cc29f92e`  
		Last Modified: Wed, 11 Oct 2023 19:42:35 GMT  
		Size: 1.5 KB (1476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c25edb0911c704d6f7039cb4e9694ca2af7fe37d3cf7e825fb28da46df996c40`  
		Last Modified: Wed, 11 Oct 2023 19:42:36 GMT  
		Size: 1.4 MB (1386273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:791d46cf692de232a6b0c1559e87ee318a302d9bab8df4d08760a9ab2c43e5ea`  
		Last Modified: Wed, 11 Oct 2023 19:42:35 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4` - linux; 386

```console
$ docker pull adminer@sha256:2c88cc2fa606983f2b3d568ffdafa27d0921f965558d18a05c0f5fc712601568
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.0 MB (96997514 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1094610c44e2e9c6caabf29c90d7fb49c39abe003f1fb9e06fe79f6e27a100c9`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Wed, 11 Oct 2023 18:08:02 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 11 Oct 2023 18:08:02 GMT
WORKDIR /var/www/html
# Wed, 11 Oct 2023 18:08:03 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 11 Oct 2023 18:08:03 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 11 Oct 2023 18:08:03 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 11 Oct 2023 18:08:03 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 11 Oct 2023 18:08:17 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 11 Oct 2023 18:08:17 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 11 Oct 2023 18:08:18 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 11 Oct 2023 18:08:18 GMT
USER adminer
# Wed, 11 Oct 2023 18:08:18 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 11 Oct 2023 18:08:18 GMT
EXPOSE 8080
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
	-	`sha256:5af98b95747bee44ac0cecc31da7755e40f44dd413b84fad60e37ba626a3a76b`  
		Last Modified: Wed, 11 Oct 2023 18:08:55 GMT  
		Size: 1.9 KB (1872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d974feb0c9497f7a8c58f10a18c88495d5b32bdd268c62331003ea6a942c0bf6`  
		Last Modified: Wed, 11 Oct 2023 18:08:55 GMT  
		Size: 1.5 KB (1478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fddf1828c60c72f33daab3a87427a7d171829535753723072a1e152f3ef01936`  
		Last Modified: Wed, 11 Oct 2023 18:08:56 GMT  
		Size: 1.4 MB (1386295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f597ad0158e1ea3aba7a4659db12d0c0954bfeda5fdc974ca864e89343f4ea1`  
		Last Modified: Wed, 11 Oct 2023 18:08:56 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4` - linux; mips64le

```console
$ docker pull adminer@sha256:e381e86167d3c2d53a9ef282bbbed1cb1ad2b6d27ed29367d477725abc1990d5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.6 MB (92632507 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1aeac6ce5d2f041b164fd41e9a4e72cc4f87258015631c78beb750929038af75`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Wed, 11 Oct 2023 20:25:20 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 11 Oct 2023 20:25:24 GMT
WORKDIR /var/www/html
# Wed, 11 Oct 2023 20:25:27 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 11 Oct 2023 20:25:30 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 11 Oct 2023 20:25:33 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 11 Oct 2023 20:25:37 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 11 Oct 2023 20:26:28 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 11 Oct 2023 20:26:31 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 11 Oct 2023 20:26:34 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 11 Oct 2023 20:26:37 GMT
USER adminer
# Wed, 11 Oct 2023 20:26:41 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 11 Oct 2023 20:26:44 GMT
EXPOSE 8080
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
	-	`sha256:77f27392480e440c2af5f35bbde6cefd9ede01e8aa21a3d111efd094fc17b271`  
		Last Modified: Wed, 11 Oct 2023 20:28:45 GMT  
		Size: 1.7 KB (1725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50c5cd11cc98c1a54e90754494f029f090ae77165f66daa68bf0fdf8afe35164`  
		Last Modified: Wed, 11 Oct 2023 20:28:45 GMT  
		Size: 1.5 KB (1477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:189b23e8f1b3c5f076dc4fb8f2d4211ce1c2c45294ae102d55e7e2d5c4886638`  
		Last Modified: Wed, 11 Oct 2023 20:28:46 GMT  
		Size: 1.4 MB (1387201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f989b6c6ecf562ac1ecfc4d5e76f330865aa68f06628685975188203137108ba`  
		Last Modified: Wed, 11 Oct 2023 20:28:45 GMT  
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
$ docker pull adminer@sha256:8d528a08459cd4c9ecc04fb999a78ea15d277a9f29fc0a4c638d0c727bcad97f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.7 MB (93708701 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e249f7d8c4a58fb4500763a3034393abadfef052e113228f0eadcbb705c08848`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 11 Oct 2023 17:50:40 GMT
ADD file:bb3ee20a7ddf364b23163c517132146872491e85ef2f1465bf7fd2ed33f94827 in / 
# Wed, 11 Oct 2023 17:50:44 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 22:32:09 GMT
STOPSIGNAL SIGINT
# Wed, 11 Oct 2023 22:39:39 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 22:39:42 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 11 Oct 2023 22:39:42 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 11 Oct 2023 22:39:43 GMT
WORKDIR /var/www/html
# Wed, 11 Oct 2023 22:39:43 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 11 Oct 2023 22:39:43 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 11 Oct 2023 22:39:43 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 11 Oct 2023 22:39:43 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 11 Oct 2023 22:41:33 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 11 Oct 2023 22:41:33 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 11 Oct 2023 22:41:34 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 11 Oct 2023 22:41:34 GMT
USER adminer
# Wed, 11 Oct 2023 22:41:34 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 11 Oct 2023 22:41:34 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:e651436ffb848f56da62cd2c80f206a288b94da8113c4c23a7e5502fb597ce23`  
		Last Modified: Wed, 11 Oct 2023 17:56:38 GMT  
		Size: 53.3 MB (53296378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2c575fbf44a3a7083af3fc636aea30f1cf9b740f3dc76ae083cf2a2700d35d1`  
		Last Modified: Wed, 11 Oct 2023 22:42:17 GMT  
		Size: 39.0 MB (39021675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e9c0af74b1292b337ce2d9000343a38538b9de1da1852202b8c22270fb379b1`  
		Last Modified: Wed, 11 Oct 2023 22:42:10 GMT  
		Size: 388.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1da19d286a2d15e09d89a2b662a7b16fc76fcf802c22fda19ad7d5f08565873b`  
		Last Modified: Wed, 11 Oct 2023 22:42:10 GMT  
		Size: 1.9 KB (1883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46ab979985444a22f0ca6ab8a93f9b4769bf499999ec67287cf4d2d65c6953aa`  
		Last Modified: Wed, 11 Oct 2023 22:42:10 GMT  
		Size: 1.5 KB (1479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3db85b1ed6626145763486f33bdaec608755b157f7b4cb25001c5fcedec6bf85`  
		Last Modified: Wed, 11 Oct 2023 22:42:10 GMT  
		Size: 1.4 MB (1386408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4129932287f7751ae20bb2c5c2e2c3e46f36a8a6dbf657e2b4142fe3ec4fd25b`  
		Last Modified: Wed, 11 Oct 2023 22:42:10 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `adminer:4-fastcgi`

```console
$ docker pull adminer@sha256:758126116a30fbb5caab76eff3921842c41462a79b2ed7ef0c5110c63f339db5
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
$ docker pull adminer@sha256:365b467d3797a82c7b2970e9b9ccb7327ac536c857fed3c2a43a4441f3852c27
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.9 MB (95944131 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02e1df82dd5d4c2b29dc581ee316e3a7977d0e8fe76e9ba725c2f2238bf0b055`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Wed, 11 Oct 2023 18:35:01 GMT
ADD file:8a9222387b89a9ac763fd72610ce01ab17f64387cbfde30a6af1861a82030aad in / 
# Wed, 11 Oct 2023 18:35:01 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 21:37:54 GMT
STOPSIGNAL SIGINT
# Wed, 11 Oct 2023 21:38:15 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 21:38:15 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 11 Oct 2023 21:38:36 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Wed, 11 Oct 2023 21:38:36 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 11 Oct 2023 21:38:37 GMT
WORKDIR /var/www/html
# Wed, 11 Oct 2023 21:38:37 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 11 Oct 2023 21:38:37 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 11 Oct 2023 21:38:37 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 11 Oct 2023 21:38:37 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 11 Oct 2023 21:38:48 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 11 Oct 2023 21:38:48 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 11 Oct 2023 21:38:48 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 11 Oct 2023 21:38:48 GMT
USER adminer
# Wed, 11 Oct 2023 21:38:48 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:69b3efbf67c2d9a46fdfdc8480b5a03ef73e9999a53aad57213447784f01eb6e`  
		Last Modified: Wed, 11 Oct 2023 18:39:54 GMT  
		Size: 55.1 MB (55058028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a0fdd089fb3c19ecd415c0ec8697e76347c06547c6418f4e0c2598cf3e6a396`  
		Last Modified: Wed, 11 Oct 2023 21:39:07 GMT  
		Size: 39.5 MB (39492762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:689786b0c396fae2f867afea8b0678012d77de73f01087f0b87b2f65d69160e0`  
		Last Modified: Wed, 11 Oct 2023 21:39:00 GMT  
		Size: 388.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fcc466451edc6454cfec5ac3903b46ee74d8467b3d60667733a53be630a7c9a`  
		Last Modified: Wed, 11 Oct 2023 21:39:26 GMT  
		Size: 2.7 KB (2710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faf32def3c4b039b9c50fe370c0e3413b5957cc9558b53841eb3df7efe68e111`  
		Last Modified: Wed, 11 Oct 2023 21:39:26 GMT  
		Size: 1.9 KB (1880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb0ed43d69cbf62a58b09d71bc4a9e0f226f33c62ea2213bea257d78ba4da3d4`  
		Last Modified: Wed, 11 Oct 2023 21:39:26 GMT  
		Size: 1.5 KB (1480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d8396667041a0e42be602675a7e48c7214cf112e6cf5c9900090b2c55b1b808`  
		Last Modified: Wed, 11 Oct 2023 21:39:27 GMT  
		Size: 1.4 MB (1386393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19fa3b3e778d428e9a49f5cfd12bdca6d2b9f649ed6d277a73561f2a9f3bba29`  
		Last Modified: Wed, 11 Oct 2023 21:39:26 GMT  
		Size: 490.0 B  
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
$ docker pull adminer@sha256:d0f7be3c33a69941b5d13b2e09f238c5d344e7ebaa14fc6d3b1e21e1bdfceef7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.8 MB (87797148 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5697f934d29ce9507be08418152a2d8692e903ca2cb7f2ce33d4ac0aacec887f`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Wed, 11 Oct 2023 17:42:19 GMT
ADD file:684f3634c6b747a4caad8f9f820cc02b53a2122591fe215935c5497ec234c3ad in / 
# Wed, 11 Oct 2023 17:42:20 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:07:19 GMT
STOPSIGNAL SIGINT
# Wed, 11 Oct 2023 18:07:44 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 18:07:45 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 11 Oct 2023 18:08:08 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Wed, 11 Oct 2023 18:08:09 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 11 Oct 2023 18:08:09 GMT
WORKDIR /var/www/html
# Wed, 11 Oct 2023 18:08:09 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 11 Oct 2023 18:08:09 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 11 Oct 2023 18:08:09 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 11 Oct 2023 18:08:10 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 11 Oct 2023 18:08:21 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 11 Oct 2023 18:08:21 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 11 Oct 2023 18:08:22 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 11 Oct 2023 18:08:22 GMT
USER adminer
# Wed, 11 Oct 2023 18:08:22 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:33d0c7672db93e653471872c639cd6129ec25c168942e15a008c4920cafe62d7`  
		Last Modified: Wed, 11 Oct 2023 17:46:42 GMT  
		Size: 50.2 MB (50215704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7566087b942379bfc2c6a78692dbbe71d4bd1573cb81ddf2ece5c0c93bf1fe76`  
		Last Modified: Wed, 11 Oct 2023 18:08:44 GMT  
		Size: 36.2 MB (36188142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:050d8c68cbad80d1919f535fae7d348cde6b6488d6688095aa47dadb0de2a8cf`  
		Last Modified: Wed, 11 Oct 2023 18:08:34 GMT  
		Size: 394.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a92995a6bb4a0c8473437a396cc8c7e9a6f97c6feab742ae0e4fa3a431aaf28`  
		Last Modified: Wed, 11 Oct 2023 18:09:05 GMT  
		Size: 2.7 KB (2713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:951d939f38aae9d46d3a17140b1e857db86fd36cb348090762290ebcd55134dc`  
		Last Modified: Wed, 11 Oct 2023 18:09:05 GMT  
		Size: 1.9 KB (1871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84c74264968945b23b05484d21ab05b2b8bf0590013f837459bc62c9e0517bf5`  
		Last Modified: Wed, 11 Oct 2023 18:09:05 GMT  
		Size: 1.5 KB (1478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b8176f3ab765cbe7bddafad7b7922c1a86378d2a5219fc42fb5ad0ce93fdaf4`  
		Last Modified: Wed, 11 Oct 2023 18:09:06 GMT  
		Size: 1.4 MB (1386355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:234ecd122c8ae18778e69e6d12a67154aec70c13f1c60bc3bc6caa921e48b63e`  
		Last Modified: Wed, 11 Oct 2023 18:09:05 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-fastcgi` - linux; arm64 variant v8

```console
$ docker pull adminer@sha256:5edfe9270064e704cf9bde68ba402b94caf1854fef76e75b548d0d31e9bdd1c9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.3 MB (94346784 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce5155034e28ab1f7365367d9889bf9e156b0169481445cbdb24977025e38ea2`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Wed, 11 Oct 2023 18:24:58 GMT
ADD file:e1a6c6c976e5e7c53eb2a7343a7a763b46e56828588535f4c79e63d6ec08198d in / 
# Wed, 11 Oct 2023 18:24:58 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 19:41:39 GMT
STOPSIGNAL SIGINT
# Wed, 11 Oct 2023 19:41:57 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 19:41:58 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 11 Oct 2023 19:42:13 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Wed, 11 Oct 2023 19:42:14 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 11 Oct 2023 19:42:14 GMT
WORKDIR /var/www/html
# Wed, 11 Oct 2023 19:42:14 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 11 Oct 2023 19:42:14 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 11 Oct 2023 19:42:14 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 11 Oct 2023 19:42:14 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 11 Oct 2023 19:42:24 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 11 Oct 2023 19:42:24 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 11 Oct 2023 19:42:24 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 11 Oct 2023 19:42:24 GMT
USER adminer
# Wed, 11 Oct 2023 19:42:24 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:dd0dc10f921f4b3b65b17f20d367374079e6cb4e26531624ee64caaaf4adcc28`  
		Last Modified: Wed, 11 Oct 2023 18:28:45 GMT  
		Size: 53.7 MB (53707810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef257294e6993147657842c1db0af6b35567fa3f5f825478621ef5bf09c4871e`  
		Last Modified: Wed, 11 Oct 2023 19:42:42 GMT  
		Size: 39.2 MB (39245727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e6ecde2f3d45f8a48e3c2d5c819eb535ac0f9abdde2051c01995434568dbf32`  
		Last Modified: Wed, 11 Oct 2023 19:42:35 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f64e658f667dca7bccf64323569503f442d4b0a1bbd9a03dac2d02136282cd7`  
		Last Modified: Wed, 11 Oct 2023 19:43:00 GMT  
		Size: 2.7 KB (2706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc68db030221ab98bb1503df9e1916671b9038e50e36bbfb9b7dc971be70a8dc`  
		Last Modified: Wed, 11 Oct 2023 19:43:00 GMT  
		Size: 1.9 KB (1879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:791ab8b9486478a99c99099b6a4289f3845f0a86606e6d2d1292a3b15fb81678`  
		Last Modified: Wed, 11 Oct 2023 19:43:00 GMT  
		Size: 1.5 KB (1475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd58e7e52f93cebe229315c3b01a670c04a16f7dc13566794094a867fe6f4769`  
		Last Modified: Wed, 11 Oct 2023 19:43:01 GMT  
		Size: 1.4 MB (1386306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c5cbd4823ce571a24efbca62dbfdccdf39f86eebe2ad64c7cc35f123c77cf43`  
		Last Modified: Wed, 11 Oct 2023 19:43:01 GMT  
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
$ docker pull adminer@sha256:38f8da7d973afde1a9a3c566526cd015ad04a9c30977d0119ad1906a78c5ea03
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.7 MB (93711402 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c8d8771a841212b7b4e8644eaa71b6d3572943d195894c2c0d2ef6195884668b`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Wed, 11 Oct 2023 17:50:40 GMT
ADD file:bb3ee20a7ddf364b23163c517132146872491e85ef2f1465bf7fd2ed33f94827 in / 
# Wed, 11 Oct 2023 17:50:44 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 22:32:09 GMT
STOPSIGNAL SIGINT
# Wed, 11 Oct 2023 22:39:39 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 22:39:42 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 11 Oct 2023 22:41:42 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Wed, 11 Oct 2023 22:41:42 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 11 Oct 2023 22:41:42 GMT
WORKDIR /var/www/html
# Wed, 11 Oct 2023 22:41:43 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 11 Oct 2023 22:41:43 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 11 Oct 2023 22:41:43 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 11 Oct 2023 22:41:43 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 11 Oct 2023 22:41:54 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 11 Oct 2023 22:41:54 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 11 Oct 2023 22:41:54 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 11 Oct 2023 22:41:55 GMT
USER adminer
# Wed, 11 Oct 2023 22:41:55 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:e651436ffb848f56da62cd2c80f206a288b94da8113c4c23a7e5502fb597ce23`  
		Last Modified: Wed, 11 Oct 2023 17:56:38 GMT  
		Size: 53.3 MB (53296378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2c575fbf44a3a7083af3fc636aea30f1cf9b740f3dc76ae083cf2a2700d35d1`  
		Last Modified: Wed, 11 Oct 2023 22:42:17 GMT  
		Size: 39.0 MB (39021675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e9c0af74b1292b337ce2d9000343a38538b9de1da1852202b8c22270fb379b1`  
		Last Modified: Wed, 11 Oct 2023 22:42:10 GMT  
		Size: 388.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f9d48af134b6c3c6edecf7490a15a84b808b328448e77b1b927d8353d052789`  
		Last Modified: Wed, 11 Oct 2023 22:43:04 GMT  
		Size: 2.7 KB (2708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4207c1ebd1df10657435d4d8a88d9a053751c925eb04136d9160c1460bf218cc`  
		Last Modified: Wed, 11 Oct 2023 22:43:04 GMT  
		Size: 1.9 KB (1884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94b6c020da4baf0dd723e8f52e0f7f049db496f445532ae712e5fb2e0a117e39`  
		Last Modified: Wed, 11 Oct 2023 22:43:04 GMT  
		Size: 1.5 KB (1481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03281e39527574cfa9159434086dceb44607f13d3c100a10bf4fe01ba32151b8`  
		Last Modified: Wed, 11 Oct 2023 22:43:04 GMT  
		Size: 1.4 MB (1386398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55024cbd9a23515415613946264858ab0e8b80279df01e26f5f8f5421afa013c`  
		Last Modified: Wed, 11 Oct 2023 22:43:04 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `adminer:4-standalone`

```console
$ docker pull adminer@sha256:cc582ae15c97b6e8c726519b17004e819016dd11d6fda5f5898361575c435236
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
$ docker pull adminer@sha256:eea72a21cf1f4a95a5369ea76cbcfcd253974d1f2bc6fff6129ecc07a8cb996c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.9 MB (95941425 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a935a78b9b29f6ad7c46d08e6266a8419f6f0f355bb0b017f7320b381a7a9dc`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 11 Oct 2023 18:35:01 GMT
ADD file:8a9222387b89a9ac763fd72610ce01ab17f64387cbfde30a6af1861a82030aad in / 
# Wed, 11 Oct 2023 18:35:01 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 21:37:54 GMT
STOPSIGNAL SIGINT
# Wed, 11 Oct 2023 21:38:15 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 21:38:15 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 11 Oct 2023 21:38:16 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 11 Oct 2023 21:38:16 GMT
WORKDIR /var/www/html
# Wed, 11 Oct 2023 21:38:16 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 11 Oct 2023 21:38:16 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 11 Oct 2023 21:38:16 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 11 Oct 2023 21:38:16 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 11 Oct 2023 21:38:28 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 11 Oct 2023 21:38:28 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 11 Oct 2023 21:38:28 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 11 Oct 2023 21:38:28 GMT
USER adminer
# Wed, 11 Oct 2023 21:38:28 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 11 Oct 2023 21:38:28 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:69b3efbf67c2d9a46fdfdc8480b5a03ef73e9999a53aad57213447784f01eb6e`  
		Last Modified: Wed, 11 Oct 2023 18:39:54 GMT  
		Size: 55.1 MB (55058028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a0fdd089fb3c19ecd415c0ec8697e76347c06547c6418f4e0c2598cf3e6a396`  
		Last Modified: Wed, 11 Oct 2023 21:39:07 GMT  
		Size: 39.5 MB (39492762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:689786b0c396fae2f867afea8b0678012d77de73f01087f0b87b2f65d69160e0`  
		Last Modified: Wed, 11 Oct 2023 21:39:00 GMT  
		Size: 388.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bcf42cdb6b507c0e95ea21dd205b3073a3cc03072bc5ecb0984571c9319a61b`  
		Last Modified: Wed, 11 Oct 2023 21:39:00 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d507b34ef5ac1588f61ab244f00d1d6c16c10c1b722ca88d305807950d239bda`  
		Last Modified: Wed, 11 Oct 2023 21:39:00 GMT  
		Size: 1.5 KB (1475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04b8d4f964a85630221b12d10d1dcc6b918a66337213d36c6d0e58d88684181f`  
		Last Modified: Wed, 11 Oct 2023 21:39:01 GMT  
		Size: 1.4 MB (1386398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a75f8703cd73af4a5226ed8767f2f4bb39476c3f3c65b2263700ef30f709ccd`  
		Last Modified: Wed, 11 Oct 2023 21:39:00 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-standalone` - linux; arm variant v5

```console
$ docker pull adminer@sha256:a08d5ea30e6d3820954b4fabeaf9249a32a7b7572327ca1dd743b38f0cbd888f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.2 MB (91203171 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:baca868e51087a0125257821115f40dcdd565feb2f02c131e0752c41bf7edb03`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Wed, 11 Oct 2023 18:02:54 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 11 Oct 2023 18:02:55 GMT
WORKDIR /var/www/html
# Wed, 11 Oct 2023 18:02:55 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 11 Oct 2023 18:02:55 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 11 Oct 2023 18:02:55 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 11 Oct 2023 18:02:55 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 11 Oct 2023 18:03:10 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 11 Oct 2023 18:03:10 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 11 Oct 2023 18:03:10 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 11 Oct 2023 18:03:10 GMT
USER adminer
# Wed, 11 Oct 2023 18:03:11 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 11 Oct 2023 18:03:11 GMT
EXPOSE 8080
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
	-	`sha256:f882441c27deeb5eb8fbd7f5966d960e7df16b93ecdca98b2eda933479843de2`  
		Last Modified: Wed, 11 Oct 2023 18:03:47 GMT  
		Size: 1.9 KB (1871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5de4c1ac09f4beb23be8f166d5ac9e50f027246da8b704d4dcd1f55c56b1b293`  
		Last Modified: Wed, 11 Oct 2023 18:03:47 GMT  
		Size: 1.5 KB (1476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b04a8ddeb2dbd66e060775b6f617eb9966bc57bfe4a9188119fdce9f8b24305e`  
		Last Modified: Wed, 11 Oct 2023 18:03:47 GMT  
		Size: 1.4 MB (1386290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:574521a263f70127c05a1db8391a9f33d18c5844caaea07ea781626bd2156092`  
		Last Modified: Wed, 11 Oct 2023 18:03:47 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-standalone` - linux; arm variant v7

```console
$ docker pull adminer@sha256:6690c92a774eeb7b3a4bd31947c0641da6f80e18d3d9b38ff91869472cbc4203
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.8 MB (87794407 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb1b05568fc173e70d7da07ef277288dd9dd7fc76372fe16397945516ed0a194`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 11 Oct 2023 17:42:19 GMT
ADD file:684f3634c6b747a4caad8f9f820cc02b53a2122591fe215935c5497ec234c3ad in / 
# Wed, 11 Oct 2023 17:42:20 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:07:19 GMT
STOPSIGNAL SIGINT
# Wed, 11 Oct 2023 18:07:44 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 18:07:45 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 11 Oct 2023 18:07:45 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 11 Oct 2023 18:07:45 GMT
WORKDIR /var/www/html
# Wed, 11 Oct 2023 18:07:45 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 11 Oct 2023 18:07:46 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 11 Oct 2023 18:07:46 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 11 Oct 2023 18:07:46 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 11 Oct 2023 18:07:59 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 11 Oct 2023 18:08:00 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 11 Oct 2023 18:08:00 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 11 Oct 2023 18:08:00 GMT
USER adminer
# Wed, 11 Oct 2023 18:08:00 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 11 Oct 2023 18:08:00 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:33d0c7672db93e653471872c639cd6129ec25c168942e15a008c4920cafe62d7`  
		Last Modified: Wed, 11 Oct 2023 17:46:42 GMT  
		Size: 50.2 MB (50215704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7566087b942379bfc2c6a78692dbbe71d4bd1573cb81ddf2ece5c0c93bf1fe76`  
		Last Modified: Wed, 11 Oct 2023 18:08:44 GMT  
		Size: 36.2 MB (36188142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:050d8c68cbad80d1919f535fae7d348cde6b6488d6688095aa47dadb0de2a8cf`  
		Last Modified: Wed, 11 Oct 2023 18:08:34 GMT  
		Size: 394.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbd3cd900e2690837d6a8cbd717999c5224939f51724c7b2ec553c1419e5ab86`  
		Last Modified: Wed, 11 Oct 2023 18:08:34 GMT  
		Size: 1.9 KB (1871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cce366bf543cd120f357c96573fa045f6c544189b422cbc2d49121b993af5e97`  
		Last Modified: Wed, 11 Oct 2023 18:08:34 GMT  
		Size: 1.5 KB (1476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff97645728e1b3ae0f3d4382f2919cf8e8f896b310af1b8a020cf1a4d4a151ce`  
		Last Modified: Wed, 11 Oct 2023 18:08:34 GMT  
		Size: 1.4 MB (1386329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa31a5f1d18ca530111bc2c3cc0da34e10ab6329822a5c075549811eda2e985b`  
		Last Modified: Wed, 11 Oct 2023 18:08:34 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-standalone` - linux; arm64 variant v8

```console
$ docker pull adminer@sha256:af7089fbd20cb08f11edf0f60a254b18f0c90a32537952e5258781d4c2d9f2c7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.3 MB (94344062 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc6c706282e894e9fe8fabf7c797478428c1166e8f93f09e43c8db0a12d0da49`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 11 Oct 2023 18:24:58 GMT
ADD file:e1a6c6c976e5e7c53eb2a7343a7a763b46e56828588535f4c79e63d6ec08198d in / 
# Wed, 11 Oct 2023 18:24:58 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 19:41:39 GMT
STOPSIGNAL SIGINT
# Wed, 11 Oct 2023 19:41:57 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 19:41:58 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 11 Oct 2023 19:41:59 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 11 Oct 2023 19:41:59 GMT
WORKDIR /var/www/html
# Wed, 11 Oct 2023 19:41:59 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 11 Oct 2023 19:41:59 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 11 Oct 2023 19:41:59 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 11 Oct 2023 19:41:59 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 11 Oct 2023 19:42:10 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 11 Oct 2023 19:42:10 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 11 Oct 2023 19:42:10 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 11 Oct 2023 19:42:10 GMT
USER adminer
# Wed, 11 Oct 2023 19:42:10 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 11 Oct 2023 19:42:10 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:dd0dc10f921f4b3b65b17f20d367374079e6cb4e26531624ee64caaaf4adcc28`  
		Last Modified: Wed, 11 Oct 2023 18:28:45 GMT  
		Size: 53.7 MB (53707810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef257294e6993147657842c1db0af6b35567fa3f5f825478621ef5bf09c4871e`  
		Last Modified: Wed, 11 Oct 2023 19:42:42 GMT  
		Size: 39.2 MB (39245727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e6ecde2f3d45f8a48e3c2d5c819eb535ac0f9abdde2051c01995434568dbf32`  
		Last Modified: Wed, 11 Oct 2023 19:42:35 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:600639d0d6dc1311b99169e0d63c4eb8f44bf21239f7000efc992a95063feb0e`  
		Last Modified: Wed, 11 Oct 2023 19:42:35 GMT  
		Size: 1.9 KB (1893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd2c7fb421d92b300b1834fa1788dc075e72d3d714336d0ce5986fb9cc29f92e`  
		Last Modified: Wed, 11 Oct 2023 19:42:35 GMT  
		Size: 1.5 KB (1476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c25edb0911c704d6f7039cb4e9694ca2af7fe37d3cf7e825fb28da46df996c40`  
		Last Modified: Wed, 11 Oct 2023 19:42:36 GMT  
		Size: 1.4 MB (1386273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:791d46cf692de232a6b0c1559e87ee318a302d9bab8df4d08760a9ab2c43e5ea`  
		Last Modified: Wed, 11 Oct 2023 19:42:35 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-standalone` - linux; 386

```console
$ docker pull adminer@sha256:2c88cc2fa606983f2b3d568ffdafa27d0921f965558d18a05c0f5fc712601568
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.0 MB (96997514 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1094610c44e2e9c6caabf29c90d7fb49c39abe003f1fb9e06fe79f6e27a100c9`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Wed, 11 Oct 2023 18:08:02 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 11 Oct 2023 18:08:02 GMT
WORKDIR /var/www/html
# Wed, 11 Oct 2023 18:08:03 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 11 Oct 2023 18:08:03 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 11 Oct 2023 18:08:03 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 11 Oct 2023 18:08:03 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 11 Oct 2023 18:08:17 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 11 Oct 2023 18:08:17 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 11 Oct 2023 18:08:18 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 11 Oct 2023 18:08:18 GMT
USER adminer
# Wed, 11 Oct 2023 18:08:18 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 11 Oct 2023 18:08:18 GMT
EXPOSE 8080
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
	-	`sha256:5af98b95747bee44ac0cecc31da7755e40f44dd413b84fad60e37ba626a3a76b`  
		Last Modified: Wed, 11 Oct 2023 18:08:55 GMT  
		Size: 1.9 KB (1872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d974feb0c9497f7a8c58f10a18c88495d5b32bdd268c62331003ea6a942c0bf6`  
		Last Modified: Wed, 11 Oct 2023 18:08:55 GMT  
		Size: 1.5 KB (1478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fddf1828c60c72f33daab3a87427a7d171829535753723072a1e152f3ef01936`  
		Last Modified: Wed, 11 Oct 2023 18:08:56 GMT  
		Size: 1.4 MB (1386295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f597ad0158e1ea3aba7a4659db12d0c0954bfeda5fdc974ca864e89343f4ea1`  
		Last Modified: Wed, 11 Oct 2023 18:08:56 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-standalone` - linux; mips64le

```console
$ docker pull adminer@sha256:e381e86167d3c2d53a9ef282bbbed1cb1ad2b6d27ed29367d477725abc1990d5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.6 MB (92632507 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1aeac6ce5d2f041b164fd41e9a4e72cc4f87258015631c78beb750929038af75`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Wed, 11 Oct 2023 20:25:20 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 11 Oct 2023 20:25:24 GMT
WORKDIR /var/www/html
# Wed, 11 Oct 2023 20:25:27 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 11 Oct 2023 20:25:30 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 11 Oct 2023 20:25:33 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 11 Oct 2023 20:25:37 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 11 Oct 2023 20:26:28 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 11 Oct 2023 20:26:31 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 11 Oct 2023 20:26:34 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 11 Oct 2023 20:26:37 GMT
USER adminer
# Wed, 11 Oct 2023 20:26:41 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 11 Oct 2023 20:26:44 GMT
EXPOSE 8080
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
	-	`sha256:77f27392480e440c2af5f35bbde6cefd9ede01e8aa21a3d111efd094fc17b271`  
		Last Modified: Wed, 11 Oct 2023 20:28:45 GMT  
		Size: 1.7 KB (1725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50c5cd11cc98c1a54e90754494f029f090ae77165f66daa68bf0fdf8afe35164`  
		Last Modified: Wed, 11 Oct 2023 20:28:45 GMT  
		Size: 1.5 KB (1477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:189b23e8f1b3c5f076dc4fb8f2d4211ce1c2c45294ae102d55e7e2d5c4886638`  
		Last Modified: Wed, 11 Oct 2023 20:28:46 GMT  
		Size: 1.4 MB (1387201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f989b6c6ecf562ac1ecfc4d5e76f330865aa68f06628685975188203137108ba`  
		Last Modified: Wed, 11 Oct 2023 20:28:45 GMT  
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
$ docker pull adminer@sha256:8d528a08459cd4c9ecc04fb999a78ea15d277a9f29fc0a4c638d0c727bcad97f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.7 MB (93708701 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e249f7d8c4a58fb4500763a3034393abadfef052e113228f0eadcbb705c08848`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 11 Oct 2023 17:50:40 GMT
ADD file:bb3ee20a7ddf364b23163c517132146872491e85ef2f1465bf7fd2ed33f94827 in / 
# Wed, 11 Oct 2023 17:50:44 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 22:32:09 GMT
STOPSIGNAL SIGINT
# Wed, 11 Oct 2023 22:39:39 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 22:39:42 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 11 Oct 2023 22:39:42 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 11 Oct 2023 22:39:43 GMT
WORKDIR /var/www/html
# Wed, 11 Oct 2023 22:39:43 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 11 Oct 2023 22:39:43 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 11 Oct 2023 22:39:43 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 11 Oct 2023 22:39:43 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 11 Oct 2023 22:41:33 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 11 Oct 2023 22:41:33 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 11 Oct 2023 22:41:34 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 11 Oct 2023 22:41:34 GMT
USER adminer
# Wed, 11 Oct 2023 22:41:34 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 11 Oct 2023 22:41:34 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:e651436ffb848f56da62cd2c80f206a288b94da8113c4c23a7e5502fb597ce23`  
		Last Modified: Wed, 11 Oct 2023 17:56:38 GMT  
		Size: 53.3 MB (53296378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2c575fbf44a3a7083af3fc636aea30f1cf9b740f3dc76ae083cf2a2700d35d1`  
		Last Modified: Wed, 11 Oct 2023 22:42:17 GMT  
		Size: 39.0 MB (39021675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e9c0af74b1292b337ce2d9000343a38538b9de1da1852202b8c22270fb379b1`  
		Last Modified: Wed, 11 Oct 2023 22:42:10 GMT  
		Size: 388.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1da19d286a2d15e09d89a2b662a7b16fc76fcf802c22fda19ad7d5f08565873b`  
		Last Modified: Wed, 11 Oct 2023 22:42:10 GMT  
		Size: 1.9 KB (1883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46ab979985444a22f0ca6ab8a93f9b4769bf499999ec67287cf4d2d65c6953aa`  
		Last Modified: Wed, 11 Oct 2023 22:42:10 GMT  
		Size: 1.5 KB (1479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3db85b1ed6626145763486f33bdaec608755b157f7b4cb25001c5fcedec6bf85`  
		Last Modified: Wed, 11 Oct 2023 22:42:10 GMT  
		Size: 1.4 MB (1386408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4129932287f7751ae20bb2c5c2e2c3e46f36a8a6dbf657e2b4142fe3ec4fd25b`  
		Last Modified: Wed, 11 Oct 2023 22:42:10 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `adminer:4.8.1`

```console
$ docker pull adminer@sha256:cc582ae15c97b6e8c726519b17004e819016dd11d6fda5f5898361575c435236
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
$ docker pull adminer@sha256:eea72a21cf1f4a95a5369ea76cbcfcd253974d1f2bc6fff6129ecc07a8cb996c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.9 MB (95941425 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a935a78b9b29f6ad7c46d08e6266a8419f6f0f355bb0b017f7320b381a7a9dc`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 11 Oct 2023 18:35:01 GMT
ADD file:8a9222387b89a9ac763fd72610ce01ab17f64387cbfde30a6af1861a82030aad in / 
# Wed, 11 Oct 2023 18:35:01 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 21:37:54 GMT
STOPSIGNAL SIGINT
# Wed, 11 Oct 2023 21:38:15 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 21:38:15 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 11 Oct 2023 21:38:16 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 11 Oct 2023 21:38:16 GMT
WORKDIR /var/www/html
# Wed, 11 Oct 2023 21:38:16 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 11 Oct 2023 21:38:16 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 11 Oct 2023 21:38:16 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 11 Oct 2023 21:38:16 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 11 Oct 2023 21:38:28 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 11 Oct 2023 21:38:28 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 11 Oct 2023 21:38:28 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 11 Oct 2023 21:38:28 GMT
USER adminer
# Wed, 11 Oct 2023 21:38:28 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 11 Oct 2023 21:38:28 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:69b3efbf67c2d9a46fdfdc8480b5a03ef73e9999a53aad57213447784f01eb6e`  
		Last Modified: Wed, 11 Oct 2023 18:39:54 GMT  
		Size: 55.1 MB (55058028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a0fdd089fb3c19ecd415c0ec8697e76347c06547c6418f4e0c2598cf3e6a396`  
		Last Modified: Wed, 11 Oct 2023 21:39:07 GMT  
		Size: 39.5 MB (39492762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:689786b0c396fae2f867afea8b0678012d77de73f01087f0b87b2f65d69160e0`  
		Last Modified: Wed, 11 Oct 2023 21:39:00 GMT  
		Size: 388.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bcf42cdb6b507c0e95ea21dd205b3073a3cc03072bc5ecb0984571c9319a61b`  
		Last Modified: Wed, 11 Oct 2023 21:39:00 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d507b34ef5ac1588f61ab244f00d1d6c16c10c1b722ca88d305807950d239bda`  
		Last Modified: Wed, 11 Oct 2023 21:39:00 GMT  
		Size: 1.5 KB (1475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04b8d4f964a85630221b12d10d1dcc6b918a66337213d36c6d0e58d88684181f`  
		Last Modified: Wed, 11 Oct 2023 21:39:01 GMT  
		Size: 1.4 MB (1386398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a75f8703cd73af4a5226ed8767f2f4bb39476c3f3c65b2263700ef30f709ccd`  
		Last Modified: Wed, 11 Oct 2023 21:39:00 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1` - linux; arm variant v5

```console
$ docker pull adminer@sha256:a08d5ea30e6d3820954b4fabeaf9249a32a7b7572327ca1dd743b38f0cbd888f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.2 MB (91203171 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:baca868e51087a0125257821115f40dcdd565feb2f02c131e0752c41bf7edb03`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Wed, 11 Oct 2023 18:02:54 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 11 Oct 2023 18:02:55 GMT
WORKDIR /var/www/html
# Wed, 11 Oct 2023 18:02:55 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 11 Oct 2023 18:02:55 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 11 Oct 2023 18:02:55 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 11 Oct 2023 18:02:55 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 11 Oct 2023 18:03:10 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 11 Oct 2023 18:03:10 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 11 Oct 2023 18:03:10 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 11 Oct 2023 18:03:10 GMT
USER adminer
# Wed, 11 Oct 2023 18:03:11 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 11 Oct 2023 18:03:11 GMT
EXPOSE 8080
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
	-	`sha256:f882441c27deeb5eb8fbd7f5966d960e7df16b93ecdca98b2eda933479843de2`  
		Last Modified: Wed, 11 Oct 2023 18:03:47 GMT  
		Size: 1.9 KB (1871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5de4c1ac09f4beb23be8f166d5ac9e50f027246da8b704d4dcd1f55c56b1b293`  
		Last Modified: Wed, 11 Oct 2023 18:03:47 GMT  
		Size: 1.5 KB (1476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b04a8ddeb2dbd66e060775b6f617eb9966bc57bfe4a9188119fdce9f8b24305e`  
		Last Modified: Wed, 11 Oct 2023 18:03:47 GMT  
		Size: 1.4 MB (1386290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:574521a263f70127c05a1db8391a9f33d18c5844caaea07ea781626bd2156092`  
		Last Modified: Wed, 11 Oct 2023 18:03:47 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1` - linux; arm variant v7

```console
$ docker pull adminer@sha256:6690c92a774eeb7b3a4bd31947c0641da6f80e18d3d9b38ff91869472cbc4203
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.8 MB (87794407 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb1b05568fc173e70d7da07ef277288dd9dd7fc76372fe16397945516ed0a194`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 11 Oct 2023 17:42:19 GMT
ADD file:684f3634c6b747a4caad8f9f820cc02b53a2122591fe215935c5497ec234c3ad in / 
# Wed, 11 Oct 2023 17:42:20 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:07:19 GMT
STOPSIGNAL SIGINT
# Wed, 11 Oct 2023 18:07:44 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 18:07:45 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 11 Oct 2023 18:07:45 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 11 Oct 2023 18:07:45 GMT
WORKDIR /var/www/html
# Wed, 11 Oct 2023 18:07:45 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 11 Oct 2023 18:07:46 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 11 Oct 2023 18:07:46 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 11 Oct 2023 18:07:46 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 11 Oct 2023 18:07:59 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 11 Oct 2023 18:08:00 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 11 Oct 2023 18:08:00 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 11 Oct 2023 18:08:00 GMT
USER adminer
# Wed, 11 Oct 2023 18:08:00 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 11 Oct 2023 18:08:00 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:33d0c7672db93e653471872c639cd6129ec25c168942e15a008c4920cafe62d7`  
		Last Modified: Wed, 11 Oct 2023 17:46:42 GMT  
		Size: 50.2 MB (50215704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7566087b942379bfc2c6a78692dbbe71d4bd1573cb81ddf2ece5c0c93bf1fe76`  
		Last Modified: Wed, 11 Oct 2023 18:08:44 GMT  
		Size: 36.2 MB (36188142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:050d8c68cbad80d1919f535fae7d348cde6b6488d6688095aa47dadb0de2a8cf`  
		Last Modified: Wed, 11 Oct 2023 18:08:34 GMT  
		Size: 394.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbd3cd900e2690837d6a8cbd717999c5224939f51724c7b2ec553c1419e5ab86`  
		Last Modified: Wed, 11 Oct 2023 18:08:34 GMT  
		Size: 1.9 KB (1871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cce366bf543cd120f357c96573fa045f6c544189b422cbc2d49121b993af5e97`  
		Last Modified: Wed, 11 Oct 2023 18:08:34 GMT  
		Size: 1.5 KB (1476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff97645728e1b3ae0f3d4382f2919cf8e8f896b310af1b8a020cf1a4d4a151ce`  
		Last Modified: Wed, 11 Oct 2023 18:08:34 GMT  
		Size: 1.4 MB (1386329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa31a5f1d18ca530111bc2c3cc0da34e10ab6329822a5c075549811eda2e985b`  
		Last Modified: Wed, 11 Oct 2023 18:08:34 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1` - linux; arm64 variant v8

```console
$ docker pull adminer@sha256:af7089fbd20cb08f11edf0f60a254b18f0c90a32537952e5258781d4c2d9f2c7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.3 MB (94344062 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc6c706282e894e9fe8fabf7c797478428c1166e8f93f09e43c8db0a12d0da49`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 11 Oct 2023 18:24:58 GMT
ADD file:e1a6c6c976e5e7c53eb2a7343a7a763b46e56828588535f4c79e63d6ec08198d in / 
# Wed, 11 Oct 2023 18:24:58 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 19:41:39 GMT
STOPSIGNAL SIGINT
# Wed, 11 Oct 2023 19:41:57 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 19:41:58 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 11 Oct 2023 19:41:59 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 11 Oct 2023 19:41:59 GMT
WORKDIR /var/www/html
# Wed, 11 Oct 2023 19:41:59 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 11 Oct 2023 19:41:59 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 11 Oct 2023 19:41:59 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 11 Oct 2023 19:41:59 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 11 Oct 2023 19:42:10 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 11 Oct 2023 19:42:10 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 11 Oct 2023 19:42:10 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 11 Oct 2023 19:42:10 GMT
USER adminer
# Wed, 11 Oct 2023 19:42:10 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 11 Oct 2023 19:42:10 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:dd0dc10f921f4b3b65b17f20d367374079e6cb4e26531624ee64caaaf4adcc28`  
		Last Modified: Wed, 11 Oct 2023 18:28:45 GMT  
		Size: 53.7 MB (53707810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef257294e6993147657842c1db0af6b35567fa3f5f825478621ef5bf09c4871e`  
		Last Modified: Wed, 11 Oct 2023 19:42:42 GMT  
		Size: 39.2 MB (39245727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e6ecde2f3d45f8a48e3c2d5c819eb535ac0f9abdde2051c01995434568dbf32`  
		Last Modified: Wed, 11 Oct 2023 19:42:35 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:600639d0d6dc1311b99169e0d63c4eb8f44bf21239f7000efc992a95063feb0e`  
		Last Modified: Wed, 11 Oct 2023 19:42:35 GMT  
		Size: 1.9 KB (1893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd2c7fb421d92b300b1834fa1788dc075e72d3d714336d0ce5986fb9cc29f92e`  
		Last Modified: Wed, 11 Oct 2023 19:42:35 GMT  
		Size: 1.5 KB (1476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c25edb0911c704d6f7039cb4e9694ca2af7fe37d3cf7e825fb28da46df996c40`  
		Last Modified: Wed, 11 Oct 2023 19:42:36 GMT  
		Size: 1.4 MB (1386273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:791d46cf692de232a6b0c1559e87ee318a302d9bab8df4d08760a9ab2c43e5ea`  
		Last Modified: Wed, 11 Oct 2023 19:42:35 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1` - linux; 386

```console
$ docker pull adminer@sha256:2c88cc2fa606983f2b3d568ffdafa27d0921f965558d18a05c0f5fc712601568
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.0 MB (96997514 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1094610c44e2e9c6caabf29c90d7fb49c39abe003f1fb9e06fe79f6e27a100c9`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Wed, 11 Oct 2023 18:08:02 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 11 Oct 2023 18:08:02 GMT
WORKDIR /var/www/html
# Wed, 11 Oct 2023 18:08:03 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 11 Oct 2023 18:08:03 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 11 Oct 2023 18:08:03 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 11 Oct 2023 18:08:03 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 11 Oct 2023 18:08:17 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 11 Oct 2023 18:08:17 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 11 Oct 2023 18:08:18 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 11 Oct 2023 18:08:18 GMT
USER adminer
# Wed, 11 Oct 2023 18:08:18 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 11 Oct 2023 18:08:18 GMT
EXPOSE 8080
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
	-	`sha256:5af98b95747bee44ac0cecc31da7755e40f44dd413b84fad60e37ba626a3a76b`  
		Last Modified: Wed, 11 Oct 2023 18:08:55 GMT  
		Size: 1.9 KB (1872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d974feb0c9497f7a8c58f10a18c88495d5b32bdd268c62331003ea6a942c0bf6`  
		Last Modified: Wed, 11 Oct 2023 18:08:55 GMT  
		Size: 1.5 KB (1478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fddf1828c60c72f33daab3a87427a7d171829535753723072a1e152f3ef01936`  
		Last Modified: Wed, 11 Oct 2023 18:08:56 GMT  
		Size: 1.4 MB (1386295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f597ad0158e1ea3aba7a4659db12d0c0954bfeda5fdc974ca864e89343f4ea1`  
		Last Modified: Wed, 11 Oct 2023 18:08:56 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1` - linux; mips64le

```console
$ docker pull adminer@sha256:e381e86167d3c2d53a9ef282bbbed1cb1ad2b6d27ed29367d477725abc1990d5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.6 MB (92632507 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1aeac6ce5d2f041b164fd41e9a4e72cc4f87258015631c78beb750929038af75`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Wed, 11 Oct 2023 20:25:20 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 11 Oct 2023 20:25:24 GMT
WORKDIR /var/www/html
# Wed, 11 Oct 2023 20:25:27 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 11 Oct 2023 20:25:30 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 11 Oct 2023 20:25:33 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 11 Oct 2023 20:25:37 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 11 Oct 2023 20:26:28 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 11 Oct 2023 20:26:31 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 11 Oct 2023 20:26:34 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 11 Oct 2023 20:26:37 GMT
USER adminer
# Wed, 11 Oct 2023 20:26:41 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 11 Oct 2023 20:26:44 GMT
EXPOSE 8080
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
	-	`sha256:77f27392480e440c2af5f35bbde6cefd9ede01e8aa21a3d111efd094fc17b271`  
		Last Modified: Wed, 11 Oct 2023 20:28:45 GMT  
		Size: 1.7 KB (1725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50c5cd11cc98c1a54e90754494f029f090ae77165f66daa68bf0fdf8afe35164`  
		Last Modified: Wed, 11 Oct 2023 20:28:45 GMT  
		Size: 1.5 KB (1477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:189b23e8f1b3c5f076dc4fb8f2d4211ce1c2c45294ae102d55e7e2d5c4886638`  
		Last Modified: Wed, 11 Oct 2023 20:28:46 GMT  
		Size: 1.4 MB (1387201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f989b6c6ecf562ac1ecfc4d5e76f330865aa68f06628685975188203137108ba`  
		Last Modified: Wed, 11 Oct 2023 20:28:45 GMT  
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
$ docker pull adminer@sha256:8d528a08459cd4c9ecc04fb999a78ea15d277a9f29fc0a4c638d0c727bcad97f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.7 MB (93708701 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e249f7d8c4a58fb4500763a3034393abadfef052e113228f0eadcbb705c08848`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 11 Oct 2023 17:50:40 GMT
ADD file:bb3ee20a7ddf364b23163c517132146872491e85ef2f1465bf7fd2ed33f94827 in / 
# Wed, 11 Oct 2023 17:50:44 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 22:32:09 GMT
STOPSIGNAL SIGINT
# Wed, 11 Oct 2023 22:39:39 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 22:39:42 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 11 Oct 2023 22:39:42 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 11 Oct 2023 22:39:43 GMT
WORKDIR /var/www/html
# Wed, 11 Oct 2023 22:39:43 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 11 Oct 2023 22:39:43 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 11 Oct 2023 22:39:43 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 11 Oct 2023 22:39:43 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 11 Oct 2023 22:41:33 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 11 Oct 2023 22:41:33 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 11 Oct 2023 22:41:34 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 11 Oct 2023 22:41:34 GMT
USER adminer
# Wed, 11 Oct 2023 22:41:34 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 11 Oct 2023 22:41:34 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:e651436ffb848f56da62cd2c80f206a288b94da8113c4c23a7e5502fb597ce23`  
		Last Modified: Wed, 11 Oct 2023 17:56:38 GMT  
		Size: 53.3 MB (53296378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2c575fbf44a3a7083af3fc636aea30f1cf9b740f3dc76ae083cf2a2700d35d1`  
		Last Modified: Wed, 11 Oct 2023 22:42:17 GMT  
		Size: 39.0 MB (39021675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e9c0af74b1292b337ce2d9000343a38538b9de1da1852202b8c22270fb379b1`  
		Last Modified: Wed, 11 Oct 2023 22:42:10 GMT  
		Size: 388.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1da19d286a2d15e09d89a2b662a7b16fc76fcf802c22fda19ad7d5f08565873b`  
		Last Modified: Wed, 11 Oct 2023 22:42:10 GMT  
		Size: 1.9 KB (1883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46ab979985444a22f0ca6ab8a93f9b4769bf499999ec67287cf4d2d65c6953aa`  
		Last Modified: Wed, 11 Oct 2023 22:42:10 GMT  
		Size: 1.5 KB (1479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3db85b1ed6626145763486f33bdaec608755b157f7b4cb25001c5fcedec6bf85`  
		Last Modified: Wed, 11 Oct 2023 22:42:10 GMT  
		Size: 1.4 MB (1386408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4129932287f7751ae20bb2c5c2e2c3e46f36a8a6dbf657e2b4142fe3ec4fd25b`  
		Last Modified: Wed, 11 Oct 2023 22:42:10 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `adminer:4.8.1-fastcgi`

```console
$ docker pull adminer@sha256:758126116a30fbb5caab76eff3921842c41462a79b2ed7ef0c5110c63f339db5
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
$ docker pull adminer@sha256:365b467d3797a82c7b2970e9b9ccb7327ac536c857fed3c2a43a4441f3852c27
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.9 MB (95944131 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02e1df82dd5d4c2b29dc581ee316e3a7977d0e8fe76e9ba725c2f2238bf0b055`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Wed, 11 Oct 2023 18:35:01 GMT
ADD file:8a9222387b89a9ac763fd72610ce01ab17f64387cbfde30a6af1861a82030aad in / 
# Wed, 11 Oct 2023 18:35:01 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 21:37:54 GMT
STOPSIGNAL SIGINT
# Wed, 11 Oct 2023 21:38:15 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 21:38:15 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 11 Oct 2023 21:38:36 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Wed, 11 Oct 2023 21:38:36 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 11 Oct 2023 21:38:37 GMT
WORKDIR /var/www/html
# Wed, 11 Oct 2023 21:38:37 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 11 Oct 2023 21:38:37 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 11 Oct 2023 21:38:37 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 11 Oct 2023 21:38:37 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 11 Oct 2023 21:38:48 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 11 Oct 2023 21:38:48 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 11 Oct 2023 21:38:48 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 11 Oct 2023 21:38:48 GMT
USER adminer
# Wed, 11 Oct 2023 21:38:48 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:69b3efbf67c2d9a46fdfdc8480b5a03ef73e9999a53aad57213447784f01eb6e`  
		Last Modified: Wed, 11 Oct 2023 18:39:54 GMT  
		Size: 55.1 MB (55058028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a0fdd089fb3c19ecd415c0ec8697e76347c06547c6418f4e0c2598cf3e6a396`  
		Last Modified: Wed, 11 Oct 2023 21:39:07 GMT  
		Size: 39.5 MB (39492762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:689786b0c396fae2f867afea8b0678012d77de73f01087f0b87b2f65d69160e0`  
		Last Modified: Wed, 11 Oct 2023 21:39:00 GMT  
		Size: 388.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fcc466451edc6454cfec5ac3903b46ee74d8467b3d60667733a53be630a7c9a`  
		Last Modified: Wed, 11 Oct 2023 21:39:26 GMT  
		Size: 2.7 KB (2710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faf32def3c4b039b9c50fe370c0e3413b5957cc9558b53841eb3df7efe68e111`  
		Last Modified: Wed, 11 Oct 2023 21:39:26 GMT  
		Size: 1.9 KB (1880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb0ed43d69cbf62a58b09d71bc4a9e0f226f33c62ea2213bea257d78ba4da3d4`  
		Last Modified: Wed, 11 Oct 2023 21:39:26 GMT  
		Size: 1.5 KB (1480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d8396667041a0e42be602675a7e48c7214cf112e6cf5c9900090b2c55b1b808`  
		Last Modified: Wed, 11 Oct 2023 21:39:27 GMT  
		Size: 1.4 MB (1386393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19fa3b3e778d428e9a49f5cfd12bdca6d2b9f649ed6d277a73561f2a9f3bba29`  
		Last Modified: Wed, 11 Oct 2023 21:39:26 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1-fastcgi` - linux; arm variant v5

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

### `adminer:4.8.1-fastcgi` - linux; arm variant v7

```console
$ docker pull adminer@sha256:d0f7be3c33a69941b5d13b2e09f238c5d344e7ebaa14fc6d3b1e21e1bdfceef7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.8 MB (87797148 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5697f934d29ce9507be08418152a2d8692e903ca2cb7f2ce33d4ac0aacec887f`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Wed, 11 Oct 2023 17:42:19 GMT
ADD file:684f3634c6b747a4caad8f9f820cc02b53a2122591fe215935c5497ec234c3ad in / 
# Wed, 11 Oct 2023 17:42:20 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:07:19 GMT
STOPSIGNAL SIGINT
# Wed, 11 Oct 2023 18:07:44 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 18:07:45 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 11 Oct 2023 18:08:08 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Wed, 11 Oct 2023 18:08:09 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 11 Oct 2023 18:08:09 GMT
WORKDIR /var/www/html
# Wed, 11 Oct 2023 18:08:09 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 11 Oct 2023 18:08:09 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 11 Oct 2023 18:08:09 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 11 Oct 2023 18:08:10 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 11 Oct 2023 18:08:21 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 11 Oct 2023 18:08:21 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 11 Oct 2023 18:08:22 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 11 Oct 2023 18:08:22 GMT
USER adminer
# Wed, 11 Oct 2023 18:08:22 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:33d0c7672db93e653471872c639cd6129ec25c168942e15a008c4920cafe62d7`  
		Last Modified: Wed, 11 Oct 2023 17:46:42 GMT  
		Size: 50.2 MB (50215704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7566087b942379bfc2c6a78692dbbe71d4bd1573cb81ddf2ece5c0c93bf1fe76`  
		Last Modified: Wed, 11 Oct 2023 18:08:44 GMT  
		Size: 36.2 MB (36188142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:050d8c68cbad80d1919f535fae7d348cde6b6488d6688095aa47dadb0de2a8cf`  
		Last Modified: Wed, 11 Oct 2023 18:08:34 GMT  
		Size: 394.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a92995a6bb4a0c8473437a396cc8c7e9a6f97c6feab742ae0e4fa3a431aaf28`  
		Last Modified: Wed, 11 Oct 2023 18:09:05 GMT  
		Size: 2.7 KB (2713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:951d939f38aae9d46d3a17140b1e857db86fd36cb348090762290ebcd55134dc`  
		Last Modified: Wed, 11 Oct 2023 18:09:05 GMT  
		Size: 1.9 KB (1871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84c74264968945b23b05484d21ab05b2b8bf0590013f837459bc62c9e0517bf5`  
		Last Modified: Wed, 11 Oct 2023 18:09:05 GMT  
		Size: 1.5 KB (1478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b8176f3ab765cbe7bddafad7b7922c1a86378d2a5219fc42fb5ad0ce93fdaf4`  
		Last Modified: Wed, 11 Oct 2023 18:09:06 GMT  
		Size: 1.4 MB (1386355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:234ecd122c8ae18778e69e6d12a67154aec70c13f1c60bc3bc6caa921e48b63e`  
		Last Modified: Wed, 11 Oct 2023 18:09:05 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1-fastcgi` - linux; arm64 variant v8

```console
$ docker pull adminer@sha256:5edfe9270064e704cf9bde68ba402b94caf1854fef76e75b548d0d31e9bdd1c9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.3 MB (94346784 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce5155034e28ab1f7365367d9889bf9e156b0169481445cbdb24977025e38ea2`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Wed, 11 Oct 2023 18:24:58 GMT
ADD file:e1a6c6c976e5e7c53eb2a7343a7a763b46e56828588535f4c79e63d6ec08198d in / 
# Wed, 11 Oct 2023 18:24:58 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 19:41:39 GMT
STOPSIGNAL SIGINT
# Wed, 11 Oct 2023 19:41:57 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 19:41:58 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 11 Oct 2023 19:42:13 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Wed, 11 Oct 2023 19:42:14 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 11 Oct 2023 19:42:14 GMT
WORKDIR /var/www/html
# Wed, 11 Oct 2023 19:42:14 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 11 Oct 2023 19:42:14 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 11 Oct 2023 19:42:14 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 11 Oct 2023 19:42:14 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 11 Oct 2023 19:42:24 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 11 Oct 2023 19:42:24 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 11 Oct 2023 19:42:24 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 11 Oct 2023 19:42:24 GMT
USER adminer
# Wed, 11 Oct 2023 19:42:24 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:dd0dc10f921f4b3b65b17f20d367374079e6cb4e26531624ee64caaaf4adcc28`  
		Last Modified: Wed, 11 Oct 2023 18:28:45 GMT  
		Size: 53.7 MB (53707810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef257294e6993147657842c1db0af6b35567fa3f5f825478621ef5bf09c4871e`  
		Last Modified: Wed, 11 Oct 2023 19:42:42 GMT  
		Size: 39.2 MB (39245727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e6ecde2f3d45f8a48e3c2d5c819eb535ac0f9abdde2051c01995434568dbf32`  
		Last Modified: Wed, 11 Oct 2023 19:42:35 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f64e658f667dca7bccf64323569503f442d4b0a1bbd9a03dac2d02136282cd7`  
		Last Modified: Wed, 11 Oct 2023 19:43:00 GMT  
		Size: 2.7 KB (2706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc68db030221ab98bb1503df9e1916671b9038e50e36bbfb9b7dc971be70a8dc`  
		Last Modified: Wed, 11 Oct 2023 19:43:00 GMT  
		Size: 1.9 KB (1879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:791ab8b9486478a99c99099b6a4289f3845f0a86606e6d2d1292a3b15fb81678`  
		Last Modified: Wed, 11 Oct 2023 19:43:00 GMT  
		Size: 1.5 KB (1475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd58e7e52f93cebe229315c3b01a670c04a16f7dc13566794094a867fe6f4769`  
		Last Modified: Wed, 11 Oct 2023 19:43:01 GMT  
		Size: 1.4 MB (1386306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c5cbd4823ce571a24efbca62dbfdccdf39f86eebe2ad64c7cc35f123c77cf43`  
		Last Modified: Wed, 11 Oct 2023 19:43:01 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1-fastcgi` - linux; 386

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

### `adminer:4.8.1-fastcgi` - linux; mips64le

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
$ docker pull adminer@sha256:38f8da7d973afde1a9a3c566526cd015ad04a9c30977d0119ad1906a78c5ea03
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.7 MB (93711402 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c8d8771a841212b7b4e8644eaa71b6d3572943d195894c2c0d2ef6195884668b`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Wed, 11 Oct 2023 17:50:40 GMT
ADD file:bb3ee20a7ddf364b23163c517132146872491e85ef2f1465bf7fd2ed33f94827 in / 
# Wed, 11 Oct 2023 17:50:44 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 22:32:09 GMT
STOPSIGNAL SIGINT
# Wed, 11 Oct 2023 22:39:39 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 22:39:42 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 11 Oct 2023 22:41:42 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Wed, 11 Oct 2023 22:41:42 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 11 Oct 2023 22:41:42 GMT
WORKDIR /var/www/html
# Wed, 11 Oct 2023 22:41:43 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 11 Oct 2023 22:41:43 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 11 Oct 2023 22:41:43 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 11 Oct 2023 22:41:43 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 11 Oct 2023 22:41:54 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 11 Oct 2023 22:41:54 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 11 Oct 2023 22:41:54 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 11 Oct 2023 22:41:55 GMT
USER adminer
# Wed, 11 Oct 2023 22:41:55 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:e651436ffb848f56da62cd2c80f206a288b94da8113c4c23a7e5502fb597ce23`  
		Last Modified: Wed, 11 Oct 2023 17:56:38 GMT  
		Size: 53.3 MB (53296378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2c575fbf44a3a7083af3fc636aea30f1cf9b740f3dc76ae083cf2a2700d35d1`  
		Last Modified: Wed, 11 Oct 2023 22:42:17 GMT  
		Size: 39.0 MB (39021675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e9c0af74b1292b337ce2d9000343a38538b9de1da1852202b8c22270fb379b1`  
		Last Modified: Wed, 11 Oct 2023 22:42:10 GMT  
		Size: 388.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f9d48af134b6c3c6edecf7490a15a84b808b328448e77b1b927d8353d052789`  
		Last Modified: Wed, 11 Oct 2023 22:43:04 GMT  
		Size: 2.7 KB (2708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4207c1ebd1df10657435d4d8a88d9a053751c925eb04136d9160c1460bf218cc`  
		Last Modified: Wed, 11 Oct 2023 22:43:04 GMT  
		Size: 1.9 KB (1884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94b6c020da4baf0dd723e8f52e0f7f049db496f445532ae712e5fb2e0a117e39`  
		Last Modified: Wed, 11 Oct 2023 22:43:04 GMT  
		Size: 1.5 KB (1481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03281e39527574cfa9159434086dceb44607f13d3c100a10bf4fe01ba32151b8`  
		Last Modified: Wed, 11 Oct 2023 22:43:04 GMT  
		Size: 1.4 MB (1386398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55024cbd9a23515415613946264858ab0e8b80279df01e26f5f8f5421afa013c`  
		Last Modified: Wed, 11 Oct 2023 22:43:04 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `adminer:4.8.1-standalone`

```console
$ docker pull adminer@sha256:cc582ae15c97b6e8c726519b17004e819016dd11d6fda5f5898361575c435236
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
$ docker pull adminer@sha256:eea72a21cf1f4a95a5369ea76cbcfcd253974d1f2bc6fff6129ecc07a8cb996c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.9 MB (95941425 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a935a78b9b29f6ad7c46d08e6266a8419f6f0f355bb0b017f7320b381a7a9dc`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 11 Oct 2023 18:35:01 GMT
ADD file:8a9222387b89a9ac763fd72610ce01ab17f64387cbfde30a6af1861a82030aad in / 
# Wed, 11 Oct 2023 18:35:01 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 21:37:54 GMT
STOPSIGNAL SIGINT
# Wed, 11 Oct 2023 21:38:15 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 21:38:15 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 11 Oct 2023 21:38:16 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 11 Oct 2023 21:38:16 GMT
WORKDIR /var/www/html
# Wed, 11 Oct 2023 21:38:16 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 11 Oct 2023 21:38:16 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 11 Oct 2023 21:38:16 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 11 Oct 2023 21:38:16 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 11 Oct 2023 21:38:28 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 11 Oct 2023 21:38:28 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 11 Oct 2023 21:38:28 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 11 Oct 2023 21:38:28 GMT
USER adminer
# Wed, 11 Oct 2023 21:38:28 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 11 Oct 2023 21:38:28 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:69b3efbf67c2d9a46fdfdc8480b5a03ef73e9999a53aad57213447784f01eb6e`  
		Last Modified: Wed, 11 Oct 2023 18:39:54 GMT  
		Size: 55.1 MB (55058028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a0fdd089fb3c19ecd415c0ec8697e76347c06547c6418f4e0c2598cf3e6a396`  
		Last Modified: Wed, 11 Oct 2023 21:39:07 GMT  
		Size: 39.5 MB (39492762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:689786b0c396fae2f867afea8b0678012d77de73f01087f0b87b2f65d69160e0`  
		Last Modified: Wed, 11 Oct 2023 21:39:00 GMT  
		Size: 388.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bcf42cdb6b507c0e95ea21dd205b3073a3cc03072bc5ecb0984571c9319a61b`  
		Last Modified: Wed, 11 Oct 2023 21:39:00 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d507b34ef5ac1588f61ab244f00d1d6c16c10c1b722ca88d305807950d239bda`  
		Last Modified: Wed, 11 Oct 2023 21:39:00 GMT  
		Size: 1.5 KB (1475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04b8d4f964a85630221b12d10d1dcc6b918a66337213d36c6d0e58d88684181f`  
		Last Modified: Wed, 11 Oct 2023 21:39:01 GMT  
		Size: 1.4 MB (1386398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a75f8703cd73af4a5226ed8767f2f4bb39476c3f3c65b2263700ef30f709ccd`  
		Last Modified: Wed, 11 Oct 2023 21:39:00 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1-standalone` - linux; arm variant v5

```console
$ docker pull adminer@sha256:a08d5ea30e6d3820954b4fabeaf9249a32a7b7572327ca1dd743b38f0cbd888f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.2 MB (91203171 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:baca868e51087a0125257821115f40dcdd565feb2f02c131e0752c41bf7edb03`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Wed, 11 Oct 2023 18:02:54 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 11 Oct 2023 18:02:55 GMT
WORKDIR /var/www/html
# Wed, 11 Oct 2023 18:02:55 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 11 Oct 2023 18:02:55 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 11 Oct 2023 18:02:55 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 11 Oct 2023 18:02:55 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 11 Oct 2023 18:03:10 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 11 Oct 2023 18:03:10 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 11 Oct 2023 18:03:10 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 11 Oct 2023 18:03:10 GMT
USER adminer
# Wed, 11 Oct 2023 18:03:11 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 11 Oct 2023 18:03:11 GMT
EXPOSE 8080
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
	-	`sha256:f882441c27deeb5eb8fbd7f5966d960e7df16b93ecdca98b2eda933479843de2`  
		Last Modified: Wed, 11 Oct 2023 18:03:47 GMT  
		Size: 1.9 KB (1871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5de4c1ac09f4beb23be8f166d5ac9e50f027246da8b704d4dcd1f55c56b1b293`  
		Last Modified: Wed, 11 Oct 2023 18:03:47 GMT  
		Size: 1.5 KB (1476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b04a8ddeb2dbd66e060775b6f617eb9966bc57bfe4a9188119fdce9f8b24305e`  
		Last Modified: Wed, 11 Oct 2023 18:03:47 GMT  
		Size: 1.4 MB (1386290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:574521a263f70127c05a1db8391a9f33d18c5844caaea07ea781626bd2156092`  
		Last Modified: Wed, 11 Oct 2023 18:03:47 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1-standalone` - linux; arm variant v7

```console
$ docker pull adminer@sha256:6690c92a774eeb7b3a4bd31947c0641da6f80e18d3d9b38ff91869472cbc4203
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.8 MB (87794407 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb1b05568fc173e70d7da07ef277288dd9dd7fc76372fe16397945516ed0a194`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 11 Oct 2023 17:42:19 GMT
ADD file:684f3634c6b747a4caad8f9f820cc02b53a2122591fe215935c5497ec234c3ad in / 
# Wed, 11 Oct 2023 17:42:20 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:07:19 GMT
STOPSIGNAL SIGINT
# Wed, 11 Oct 2023 18:07:44 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 18:07:45 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 11 Oct 2023 18:07:45 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 11 Oct 2023 18:07:45 GMT
WORKDIR /var/www/html
# Wed, 11 Oct 2023 18:07:45 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 11 Oct 2023 18:07:46 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 11 Oct 2023 18:07:46 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 11 Oct 2023 18:07:46 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 11 Oct 2023 18:07:59 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 11 Oct 2023 18:08:00 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 11 Oct 2023 18:08:00 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 11 Oct 2023 18:08:00 GMT
USER adminer
# Wed, 11 Oct 2023 18:08:00 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 11 Oct 2023 18:08:00 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:33d0c7672db93e653471872c639cd6129ec25c168942e15a008c4920cafe62d7`  
		Last Modified: Wed, 11 Oct 2023 17:46:42 GMT  
		Size: 50.2 MB (50215704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7566087b942379bfc2c6a78692dbbe71d4bd1573cb81ddf2ece5c0c93bf1fe76`  
		Last Modified: Wed, 11 Oct 2023 18:08:44 GMT  
		Size: 36.2 MB (36188142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:050d8c68cbad80d1919f535fae7d348cde6b6488d6688095aa47dadb0de2a8cf`  
		Last Modified: Wed, 11 Oct 2023 18:08:34 GMT  
		Size: 394.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbd3cd900e2690837d6a8cbd717999c5224939f51724c7b2ec553c1419e5ab86`  
		Last Modified: Wed, 11 Oct 2023 18:08:34 GMT  
		Size: 1.9 KB (1871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cce366bf543cd120f357c96573fa045f6c544189b422cbc2d49121b993af5e97`  
		Last Modified: Wed, 11 Oct 2023 18:08:34 GMT  
		Size: 1.5 KB (1476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff97645728e1b3ae0f3d4382f2919cf8e8f896b310af1b8a020cf1a4d4a151ce`  
		Last Modified: Wed, 11 Oct 2023 18:08:34 GMT  
		Size: 1.4 MB (1386329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa31a5f1d18ca530111bc2c3cc0da34e10ab6329822a5c075549811eda2e985b`  
		Last Modified: Wed, 11 Oct 2023 18:08:34 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1-standalone` - linux; arm64 variant v8

```console
$ docker pull adminer@sha256:af7089fbd20cb08f11edf0f60a254b18f0c90a32537952e5258781d4c2d9f2c7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.3 MB (94344062 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc6c706282e894e9fe8fabf7c797478428c1166e8f93f09e43c8db0a12d0da49`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 11 Oct 2023 18:24:58 GMT
ADD file:e1a6c6c976e5e7c53eb2a7343a7a763b46e56828588535f4c79e63d6ec08198d in / 
# Wed, 11 Oct 2023 18:24:58 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 19:41:39 GMT
STOPSIGNAL SIGINT
# Wed, 11 Oct 2023 19:41:57 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 19:41:58 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 11 Oct 2023 19:41:59 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 11 Oct 2023 19:41:59 GMT
WORKDIR /var/www/html
# Wed, 11 Oct 2023 19:41:59 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 11 Oct 2023 19:41:59 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 11 Oct 2023 19:41:59 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 11 Oct 2023 19:41:59 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 11 Oct 2023 19:42:10 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 11 Oct 2023 19:42:10 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 11 Oct 2023 19:42:10 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 11 Oct 2023 19:42:10 GMT
USER adminer
# Wed, 11 Oct 2023 19:42:10 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 11 Oct 2023 19:42:10 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:dd0dc10f921f4b3b65b17f20d367374079e6cb4e26531624ee64caaaf4adcc28`  
		Last Modified: Wed, 11 Oct 2023 18:28:45 GMT  
		Size: 53.7 MB (53707810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef257294e6993147657842c1db0af6b35567fa3f5f825478621ef5bf09c4871e`  
		Last Modified: Wed, 11 Oct 2023 19:42:42 GMT  
		Size: 39.2 MB (39245727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e6ecde2f3d45f8a48e3c2d5c819eb535ac0f9abdde2051c01995434568dbf32`  
		Last Modified: Wed, 11 Oct 2023 19:42:35 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:600639d0d6dc1311b99169e0d63c4eb8f44bf21239f7000efc992a95063feb0e`  
		Last Modified: Wed, 11 Oct 2023 19:42:35 GMT  
		Size: 1.9 KB (1893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd2c7fb421d92b300b1834fa1788dc075e72d3d714336d0ce5986fb9cc29f92e`  
		Last Modified: Wed, 11 Oct 2023 19:42:35 GMT  
		Size: 1.5 KB (1476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c25edb0911c704d6f7039cb4e9694ca2af7fe37d3cf7e825fb28da46df996c40`  
		Last Modified: Wed, 11 Oct 2023 19:42:36 GMT  
		Size: 1.4 MB (1386273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:791d46cf692de232a6b0c1559e87ee318a302d9bab8df4d08760a9ab2c43e5ea`  
		Last Modified: Wed, 11 Oct 2023 19:42:35 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1-standalone` - linux; 386

```console
$ docker pull adminer@sha256:2c88cc2fa606983f2b3d568ffdafa27d0921f965558d18a05c0f5fc712601568
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.0 MB (96997514 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1094610c44e2e9c6caabf29c90d7fb49c39abe003f1fb9e06fe79f6e27a100c9`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Wed, 11 Oct 2023 18:08:02 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 11 Oct 2023 18:08:02 GMT
WORKDIR /var/www/html
# Wed, 11 Oct 2023 18:08:03 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 11 Oct 2023 18:08:03 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 11 Oct 2023 18:08:03 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 11 Oct 2023 18:08:03 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 11 Oct 2023 18:08:17 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 11 Oct 2023 18:08:17 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 11 Oct 2023 18:08:18 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 11 Oct 2023 18:08:18 GMT
USER adminer
# Wed, 11 Oct 2023 18:08:18 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 11 Oct 2023 18:08:18 GMT
EXPOSE 8080
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
	-	`sha256:5af98b95747bee44ac0cecc31da7755e40f44dd413b84fad60e37ba626a3a76b`  
		Last Modified: Wed, 11 Oct 2023 18:08:55 GMT  
		Size: 1.9 KB (1872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d974feb0c9497f7a8c58f10a18c88495d5b32bdd268c62331003ea6a942c0bf6`  
		Last Modified: Wed, 11 Oct 2023 18:08:55 GMT  
		Size: 1.5 KB (1478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fddf1828c60c72f33daab3a87427a7d171829535753723072a1e152f3ef01936`  
		Last Modified: Wed, 11 Oct 2023 18:08:56 GMT  
		Size: 1.4 MB (1386295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f597ad0158e1ea3aba7a4659db12d0c0954bfeda5fdc974ca864e89343f4ea1`  
		Last Modified: Wed, 11 Oct 2023 18:08:56 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1-standalone` - linux; mips64le

```console
$ docker pull adminer@sha256:e381e86167d3c2d53a9ef282bbbed1cb1ad2b6d27ed29367d477725abc1990d5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.6 MB (92632507 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1aeac6ce5d2f041b164fd41e9a4e72cc4f87258015631c78beb750929038af75`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Wed, 11 Oct 2023 20:25:20 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 11 Oct 2023 20:25:24 GMT
WORKDIR /var/www/html
# Wed, 11 Oct 2023 20:25:27 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 11 Oct 2023 20:25:30 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 11 Oct 2023 20:25:33 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 11 Oct 2023 20:25:37 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 11 Oct 2023 20:26:28 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 11 Oct 2023 20:26:31 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 11 Oct 2023 20:26:34 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 11 Oct 2023 20:26:37 GMT
USER adminer
# Wed, 11 Oct 2023 20:26:41 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 11 Oct 2023 20:26:44 GMT
EXPOSE 8080
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
	-	`sha256:77f27392480e440c2af5f35bbde6cefd9ede01e8aa21a3d111efd094fc17b271`  
		Last Modified: Wed, 11 Oct 2023 20:28:45 GMT  
		Size: 1.7 KB (1725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50c5cd11cc98c1a54e90754494f029f090ae77165f66daa68bf0fdf8afe35164`  
		Last Modified: Wed, 11 Oct 2023 20:28:45 GMT  
		Size: 1.5 KB (1477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:189b23e8f1b3c5f076dc4fb8f2d4211ce1c2c45294ae102d55e7e2d5c4886638`  
		Last Modified: Wed, 11 Oct 2023 20:28:46 GMT  
		Size: 1.4 MB (1387201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f989b6c6ecf562ac1ecfc4d5e76f330865aa68f06628685975188203137108ba`  
		Last Modified: Wed, 11 Oct 2023 20:28:45 GMT  
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
$ docker pull adminer@sha256:8d528a08459cd4c9ecc04fb999a78ea15d277a9f29fc0a4c638d0c727bcad97f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.7 MB (93708701 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e249f7d8c4a58fb4500763a3034393abadfef052e113228f0eadcbb705c08848`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 11 Oct 2023 17:50:40 GMT
ADD file:bb3ee20a7ddf364b23163c517132146872491e85ef2f1465bf7fd2ed33f94827 in / 
# Wed, 11 Oct 2023 17:50:44 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 22:32:09 GMT
STOPSIGNAL SIGINT
# Wed, 11 Oct 2023 22:39:39 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 22:39:42 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 11 Oct 2023 22:39:42 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 11 Oct 2023 22:39:43 GMT
WORKDIR /var/www/html
# Wed, 11 Oct 2023 22:39:43 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 11 Oct 2023 22:39:43 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 11 Oct 2023 22:39:43 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 11 Oct 2023 22:39:43 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 11 Oct 2023 22:41:33 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 11 Oct 2023 22:41:33 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 11 Oct 2023 22:41:34 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 11 Oct 2023 22:41:34 GMT
USER adminer
# Wed, 11 Oct 2023 22:41:34 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 11 Oct 2023 22:41:34 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:e651436ffb848f56da62cd2c80f206a288b94da8113c4c23a7e5502fb597ce23`  
		Last Modified: Wed, 11 Oct 2023 17:56:38 GMT  
		Size: 53.3 MB (53296378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2c575fbf44a3a7083af3fc636aea30f1cf9b740f3dc76ae083cf2a2700d35d1`  
		Last Modified: Wed, 11 Oct 2023 22:42:17 GMT  
		Size: 39.0 MB (39021675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e9c0af74b1292b337ce2d9000343a38538b9de1da1852202b8c22270fb379b1`  
		Last Modified: Wed, 11 Oct 2023 22:42:10 GMT  
		Size: 388.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1da19d286a2d15e09d89a2b662a7b16fc76fcf802c22fda19ad7d5f08565873b`  
		Last Modified: Wed, 11 Oct 2023 22:42:10 GMT  
		Size: 1.9 KB (1883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46ab979985444a22f0ca6ab8a93f9b4769bf499999ec67287cf4d2d65c6953aa`  
		Last Modified: Wed, 11 Oct 2023 22:42:10 GMT  
		Size: 1.5 KB (1479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3db85b1ed6626145763486f33bdaec608755b157f7b4cb25001c5fcedec6bf85`  
		Last Modified: Wed, 11 Oct 2023 22:42:10 GMT  
		Size: 1.4 MB (1386408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4129932287f7751ae20bb2c5c2e2c3e46f36a8a6dbf657e2b4142fe3ec4fd25b`  
		Last Modified: Wed, 11 Oct 2023 22:42:10 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `adminer:fastcgi`

```console
$ docker pull adminer@sha256:758126116a30fbb5caab76eff3921842c41462a79b2ed7ef0c5110c63f339db5
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
$ docker pull adminer@sha256:365b467d3797a82c7b2970e9b9ccb7327ac536c857fed3c2a43a4441f3852c27
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.9 MB (95944131 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02e1df82dd5d4c2b29dc581ee316e3a7977d0e8fe76e9ba725c2f2238bf0b055`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Wed, 11 Oct 2023 18:35:01 GMT
ADD file:8a9222387b89a9ac763fd72610ce01ab17f64387cbfde30a6af1861a82030aad in / 
# Wed, 11 Oct 2023 18:35:01 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 21:37:54 GMT
STOPSIGNAL SIGINT
# Wed, 11 Oct 2023 21:38:15 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 21:38:15 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 11 Oct 2023 21:38:36 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Wed, 11 Oct 2023 21:38:36 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 11 Oct 2023 21:38:37 GMT
WORKDIR /var/www/html
# Wed, 11 Oct 2023 21:38:37 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 11 Oct 2023 21:38:37 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 11 Oct 2023 21:38:37 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 11 Oct 2023 21:38:37 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 11 Oct 2023 21:38:48 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 11 Oct 2023 21:38:48 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 11 Oct 2023 21:38:48 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 11 Oct 2023 21:38:48 GMT
USER adminer
# Wed, 11 Oct 2023 21:38:48 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:69b3efbf67c2d9a46fdfdc8480b5a03ef73e9999a53aad57213447784f01eb6e`  
		Last Modified: Wed, 11 Oct 2023 18:39:54 GMT  
		Size: 55.1 MB (55058028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a0fdd089fb3c19ecd415c0ec8697e76347c06547c6418f4e0c2598cf3e6a396`  
		Last Modified: Wed, 11 Oct 2023 21:39:07 GMT  
		Size: 39.5 MB (39492762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:689786b0c396fae2f867afea8b0678012d77de73f01087f0b87b2f65d69160e0`  
		Last Modified: Wed, 11 Oct 2023 21:39:00 GMT  
		Size: 388.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fcc466451edc6454cfec5ac3903b46ee74d8467b3d60667733a53be630a7c9a`  
		Last Modified: Wed, 11 Oct 2023 21:39:26 GMT  
		Size: 2.7 KB (2710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faf32def3c4b039b9c50fe370c0e3413b5957cc9558b53841eb3df7efe68e111`  
		Last Modified: Wed, 11 Oct 2023 21:39:26 GMT  
		Size: 1.9 KB (1880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb0ed43d69cbf62a58b09d71bc4a9e0f226f33c62ea2213bea257d78ba4da3d4`  
		Last Modified: Wed, 11 Oct 2023 21:39:26 GMT  
		Size: 1.5 KB (1480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d8396667041a0e42be602675a7e48c7214cf112e6cf5c9900090b2c55b1b808`  
		Last Modified: Wed, 11 Oct 2023 21:39:27 GMT  
		Size: 1.4 MB (1386393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19fa3b3e778d428e9a49f5cfd12bdca6d2b9f649ed6d277a73561f2a9f3bba29`  
		Last Modified: Wed, 11 Oct 2023 21:39:26 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:fastcgi` - linux; arm variant v5

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

### `adminer:fastcgi` - linux; arm variant v7

```console
$ docker pull adminer@sha256:d0f7be3c33a69941b5d13b2e09f238c5d344e7ebaa14fc6d3b1e21e1bdfceef7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.8 MB (87797148 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5697f934d29ce9507be08418152a2d8692e903ca2cb7f2ce33d4ac0aacec887f`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Wed, 11 Oct 2023 17:42:19 GMT
ADD file:684f3634c6b747a4caad8f9f820cc02b53a2122591fe215935c5497ec234c3ad in / 
# Wed, 11 Oct 2023 17:42:20 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:07:19 GMT
STOPSIGNAL SIGINT
# Wed, 11 Oct 2023 18:07:44 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 18:07:45 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 11 Oct 2023 18:08:08 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Wed, 11 Oct 2023 18:08:09 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 11 Oct 2023 18:08:09 GMT
WORKDIR /var/www/html
# Wed, 11 Oct 2023 18:08:09 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 11 Oct 2023 18:08:09 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 11 Oct 2023 18:08:09 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 11 Oct 2023 18:08:10 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 11 Oct 2023 18:08:21 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 11 Oct 2023 18:08:21 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 11 Oct 2023 18:08:22 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 11 Oct 2023 18:08:22 GMT
USER adminer
# Wed, 11 Oct 2023 18:08:22 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:33d0c7672db93e653471872c639cd6129ec25c168942e15a008c4920cafe62d7`  
		Last Modified: Wed, 11 Oct 2023 17:46:42 GMT  
		Size: 50.2 MB (50215704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7566087b942379bfc2c6a78692dbbe71d4bd1573cb81ddf2ece5c0c93bf1fe76`  
		Last Modified: Wed, 11 Oct 2023 18:08:44 GMT  
		Size: 36.2 MB (36188142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:050d8c68cbad80d1919f535fae7d348cde6b6488d6688095aa47dadb0de2a8cf`  
		Last Modified: Wed, 11 Oct 2023 18:08:34 GMT  
		Size: 394.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a92995a6bb4a0c8473437a396cc8c7e9a6f97c6feab742ae0e4fa3a431aaf28`  
		Last Modified: Wed, 11 Oct 2023 18:09:05 GMT  
		Size: 2.7 KB (2713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:951d939f38aae9d46d3a17140b1e857db86fd36cb348090762290ebcd55134dc`  
		Last Modified: Wed, 11 Oct 2023 18:09:05 GMT  
		Size: 1.9 KB (1871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84c74264968945b23b05484d21ab05b2b8bf0590013f837459bc62c9e0517bf5`  
		Last Modified: Wed, 11 Oct 2023 18:09:05 GMT  
		Size: 1.5 KB (1478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b8176f3ab765cbe7bddafad7b7922c1a86378d2a5219fc42fb5ad0ce93fdaf4`  
		Last Modified: Wed, 11 Oct 2023 18:09:06 GMT  
		Size: 1.4 MB (1386355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:234ecd122c8ae18778e69e6d12a67154aec70c13f1c60bc3bc6caa921e48b63e`  
		Last Modified: Wed, 11 Oct 2023 18:09:05 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:fastcgi` - linux; arm64 variant v8

```console
$ docker pull adminer@sha256:5edfe9270064e704cf9bde68ba402b94caf1854fef76e75b548d0d31e9bdd1c9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.3 MB (94346784 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce5155034e28ab1f7365367d9889bf9e156b0169481445cbdb24977025e38ea2`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Wed, 11 Oct 2023 18:24:58 GMT
ADD file:e1a6c6c976e5e7c53eb2a7343a7a763b46e56828588535f4c79e63d6ec08198d in / 
# Wed, 11 Oct 2023 18:24:58 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 19:41:39 GMT
STOPSIGNAL SIGINT
# Wed, 11 Oct 2023 19:41:57 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 19:41:58 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 11 Oct 2023 19:42:13 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Wed, 11 Oct 2023 19:42:14 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 11 Oct 2023 19:42:14 GMT
WORKDIR /var/www/html
# Wed, 11 Oct 2023 19:42:14 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 11 Oct 2023 19:42:14 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 11 Oct 2023 19:42:14 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 11 Oct 2023 19:42:14 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 11 Oct 2023 19:42:24 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 11 Oct 2023 19:42:24 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 11 Oct 2023 19:42:24 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 11 Oct 2023 19:42:24 GMT
USER adminer
# Wed, 11 Oct 2023 19:42:24 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:dd0dc10f921f4b3b65b17f20d367374079e6cb4e26531624ee64caaaf4adcc28`  
		Last Modified: Wed, 11 Oct 2023 18:28:45 GMT  
		Size: 53.7 MB (53707810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef257294e6993147657842c1db0af6b35567fa3f5f825478621ef5bf09c4871e`  
		Last Modified: Wed, 11 Oct 2023 19:42:42 GMT  
		Size: 39.2 MB (39245727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e6ecde2f3d45f8a48e3c2d5c819eb535ac0f9abdde2051c01995434568dbf32`  
		Last Modified: Wed, 11 Oct 2023 19:42:35 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f64e658f667dca7bccf64323569503f442d4b0a1bbd9a03dac2d02136282cd7`  
		Last Modified: Wed, 11 Oct 2023 19:43:00 GMT  
		Size: 2.7 KB (2706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc68db030221ab98bb1503df9e1916671b9038e50e36bbfb9b7dc971be70a8dc`  
		Last Modified: Wed, 11 Oct 2023 19:43:00 GMT  
		Size: 1.9 KB (1879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:791ab8b9486478a99c99099b6a4289f3845f0a86606e6d2d1292a3b15fb81678`  
		Last Modified: Wed, 11 Oct 2023 19:43:00 GMT  
		Size: 1.5 KB (1475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd58e7e52f93cebe229315c3b01a670c04a16f7dc13566794094a867fe6f4769`  
		Last Modified: Wed, 11 Oct 2023 19:43:01 GMT  
		Size: 1.4 MB (1386306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c5cbd4823ce571a24efbca62dbfdccdf39f86eebe2ad64c7cc35f123c77cf43`  
		Last Modified: Wed, 11 Oct 2023 19:43:01 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:fastcgi` - linux; 386

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

### `adminer:fastcgi` - linux; mips64le

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
$ docker pull adminer@sha256:38f8da7d973afde1a9a3c566526cd015ad04a9c30977d0119ad1906a78c5ea03
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.7 MB (93711402 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c8d8771a841212b7b4e8644eaa71b6d3572943d195894c2c0d2ef6195884668b`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Wed, 11 Oct 2023 17:50:40 GMT
ADD file:bb3ee20a7ddf364b23163c517132146872491e85ef2f1465bf7fd2ed33f94827 in / 
# Wed, 11 Oct 2023 17:50:44 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 22:32:09 GMT
STOPSIGNAL SIGINT
# Wed, 11 Oct 2023 22:39:39 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 22:39:42 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 11 Oct 2023 22:41:42 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Wed, 11 Oct 2023 22:41:42 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 11 Oct 2023 22:41:42 GMT
WORKDIR /var/www/html
# Wed, 11 Oct 2023 22:41:43 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 11 Oct 2023 22:41:43 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 11 Oct 2023 22:41:43 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 11 Oct 2023 22:41:43 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 11 Oct 2023 22:41:54 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 11 Oct 2023 22:41:54 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 11 Oct 2023 22:41:54 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 11 Oct 2023 22:41:55 GMT
USER adminer
# Wed, 11 Oct 2023 22:41:55 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:e651436ffb848f56da62cd2c80f206a288b94da8113c4c23a7e5502fb597ce23`  
		Last Modified: Wed, 11 Oct 2023 17:56:38 GMT  
		Size: 53.3 MB (53296378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2c575fbf44a3a7083af3fc636aea30f1cf9b740f3dc76ae083cf2a2700d35d1`  
		Last Modified: Wed, 11 Oct 2023 22:42:17 GMT  
		Size: 39.0 MB (39021675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e9c0af74b1292b337ce2d9000343a38538b9de1da1852202b8c22270fb379b1`  
		Last Modified: Wed, 11 Oct 2023 22:42:10 GMT  
		Size: 388.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f9d48af134b6c3c6edecf7490a15a84b808b328448e77b1b927d8353d052789`  
		Last Modified: Wed, 11 Oct 2023 22:43:04 GMT  
		Size: 2.7 KB (2708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4207c1ebd1df10657435d4d8a88d9a053751c925eb04136d9160c1460bf218cc`  
		Last Modified: Wed, 11 Oct 2023 22:43:04 GMT  
		Size: 1.9 KB (1884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94b6c020da4baf0dd723e8f52e0f7f049db496f445532ae712e5fb2e0a117e39`  
		Last Modified: Wed, 11 Oct 2023 22:43:04 GMT  
		Size: 1.5 KB (1481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03281e39527574cfa9159434086dceb44607f13d3c100a10bf4fe01ba32151b8`  
		Last Modified: Wed, 11 Oct 2023 22:43:04 GMT  
		Size: 1.4 MB (1386398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55024cbd9a23515415613946264858ab0e8b80279df01e26f5f8f5421afa013c`  
		Last Modified: Wed, 11 Oct 2023 22:43:04 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `adminer:latest`

```console
$ docker pull adminer@sha256:cc582ae15c97b6e8c726519b17004e819016dd11d6fda5f5898361575c435236
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
$ docker pull adminer@sha256:eea72a21cf1f4a95a5369ea76cbcfcd253974d1f2bc6fff6129ecc07a8cb996c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.9 MB (95941425 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a935a78b9b29f6ad7c46d08e6266a8419f6f0f355bb0b017f7320b381a7a9dc`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 11 Oct 2023 18:35:01 GMT
ADD file:8a9222387b89a9ac763fd72610ce01ab17f64387cbfde30a6af1861a82030aad in / 
# Wed, 11 Oct 2023 18:35:01 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 21:37:54 GMT
STOPSIGNAL SIGINT
# Wed, 11 Oct 2023 21:38:15 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 21:38:15 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 11 Oct 2023 21:38:16 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 11 Oct 2023 21:38:16 GMT
WORKDIR /var/www/html
# Wed, 11 Oct 2023 21:38:16 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 11 Oct 2023 21:38:16 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 11 Oct 2023 21:38:16 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 11 Oct 2023 21:38:16 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 11 Oct 2023 21:38:28 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 11 Oct 2023 21:38:28 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 11 Oct 2023 21:38:28 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 11 Oct 2023 21:38:28 GMT
USER adminer
# Wed, 11 Oct 2023 21:38:28 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 11 Oct 2023 21:38:28 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:69b3efbf67c2d9a46fdfdc8480b5a03ef73e9999a53aad57213447784f01eb6e`  
		Last Modified: Wed, 11 Oct 2023 18:39:54 GMT  
		Size: 55.1 MB (55058028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a0fdd089fb3c19ecd415c0ec8697e76347c06547c6418f4e0c2598cf3e6a396`  
		Last Modified: Wed, 11 Oct 2023 21:39:07 GMT  
		Size: 39.5 MB (39492762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:689786b0c396fae2f867afea8b0678012d77de73f01087f0b87b2f65d69160e0`  
		Last Modified: Wed, 11 Oct 2023 21:39:00 GMT  
		Size: 388.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bcf42cdb6b507c0e95ea21dd205b3073a3cc03072bc5ecb0984571c9319a61b`  
		Last Modified: Wed, 11 Oct 2023 21:39:00 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d507b34ef5ac1588f61ab244f00d1d6c16c10c1b722ca88d305807950d239bda`  
		Last Modified: Wed, 11 Oct 2023 21:39:00 GMT  
		Size: 1.5 KB (1475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04b8d4f964a85630221b12d10d1dcc6b918a66337213d36c6d0e58d88684181f`  
		Last Modified: Wed, 11 Oct 2023 21:39:01 GMT  
		Size: 1.4 MB (1386398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a75f8703cd73af4a5226ed8767f2f4bb39476c3f3c65b2263700ef30f709ccd`  
		Last Modified: Wed, 11 Oct 2023 21:39:00 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:latest` - linux; arm variant v5

```console
$ docker pull adminer@sha256:a08d5ea30e6d3820954b4fabeaf9249a32a7b7572327ca1dd743b38f0cbd888f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.2 MB (91203171 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:baca868e51087a0125257821115f40dcdd565feb2f02c131e0752c41bf7edb03`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Wed, 11 Oct 2023 18:02:54 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 11 Oct 2023 18:02:55 GMT
WORKDIR /var/www/html
# Wed, 11 Oct 2023 18:02:55 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 11 Oct 2023 18:02:55 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 11 Oct 2023 18:02:55 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 11 Oct 2023 18:02:55 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 11 Oct 2023 18:03:10 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 11 Oct 2023 18:03:10 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 11 Oct 2023 18:03:10 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 11 Oct 2023 18:03:10 GMT
USER adminer
# Wed, 11 Oct 2023 18:03:11 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 11 Oct 2023 18:03:11 GMT
EXPOSE 8080
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
	-	`sha256:f882441c27deeb5eb8fbd7f5966d960e7df16b93ecdca98b2eda933479843de2`  
		Last Modified: Wed, 11 Oct 2023 18:03:47 GMT  
		Size: 1.9 KB (1871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5de4c1ac09f4beb23be8f166d5ac9e50f027246da8b704d4dcd1f55c56b1b293`  
		Last Modified: Wed, 11 Oct 2023 18:03:47 GMT  
		Size: 1.5 KB (1476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b04a8ddeb2dbd66e060775b6f617eb9966bc57bfe4a9188119fdce9f8b24305e`  
		Last Modified: Wed, 11 Oct 2023 18:03:47 GMT  
		Size: 1.4 MB (1386290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:574521a263f70127c05a1db8391a9f33d18c5844caaea07ea781626bd2156092`  
		Last Modified: Wed, 11 Oct 2023 18:03:47 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:latest` - linux; arm variant v7

```console
$ docker pull adminer@sha256:6690c92a774eeb7b3a4bd31947c0641da6f80e18d3d9b38ff91869472cbc4203
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.8 MB (87794407 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb1b05568fc173e70d7da07ef277288dd9dd7fc76372fe16397945516ed0a194`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 11 Oct 2023 17:42:19 GMT
ADD file:684f3634c6b747a4caad8f9f820cc02b53a2122591fe215935c5497ec234c3ad in / 
# Wed, 11 Oct 2023 17:42:20 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:07:19 GMT
STOPSIGNAL SIGINT
# Wed, 11 Oct 2023 18:07:44 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 18:07:45 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 11 Oct 2023 18:07:45 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 11 Oct 2023 18:07:45 GMT
WORKDIR /var/www/html
# Wed, 11 Oct 2023 18:07:45 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 11 Oct 2023 18:07:46 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 11 Oct 2023 18:07:46 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 11 Oct 2023 18:07:46 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 11 Oct 2023 18:07:59 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 11 Oct 2023 18:08:00 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 11 Oct 2023 18:08:00 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 11 Oct 2023 18:08:00 GMT
USER adminer
# Wed, 11 Oct 2023 18:08:00 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 11 Oct 2023 18:08:00 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:33d0c7672db93e653471872c639cd6129ec25c168942e15a008c4920cafe62d7`  
		Last Modified: Wed, 11 Oct 2023 17:46:42 GMT  
		Size: 50.2 MB (50215704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7566087b942379bfc2c6a78692dbbe71d4bd1573cb81ddf2ece5c0c93bf1fe76`  
		Last Modified: Wed, 11 Oct 2023 18:08:44 GMT  
		Size: 36.2 MB (36188142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:050d8c68cbad80d1919f535fae7d348cde6b6488d6688095aa47dadb0de2a8cf`  
		Last Modified: Wed, 11 Oct 2023 18:08:34 GMT  
		Size: 394.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbd3cd900e2690837d6a8cbd717999c5224939f51724c7b2ec553c1419e5ab86`  
		Last Modified: Wed, 11 Oct 2023 18:08:34 GMT  
		Size: 1.9 KB (1871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cce366bf543cd120f357c96573fa045f6c544189b422cbc2d49121b993af5e97`  
		Last Modified: Wed, 11 Oct 2023 18:08:34 GMT  
		Size: 1.5 KB (1476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff97645728e1b3ae0f3d4382f2919cf8e8f896b310af1b8a020cf1a4d4a151ce`  
		Last Modified: Wed, 11 Oct 2023 18:08:34 GMT  
		Size: 1.4 MB (1386329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa31a5f1d18ca530111bc2c3cc0da34e10ab6329822a5c075549811eda2e985b`  
		Last Modified: Wed, 11 Oct 2023 18:08:34 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:latest` - linux; arm64 variant v8

```console
$ docker pull adminer@sha256:af7089fbd20cb08f11edf0f60a254b18f0c90a32537952e5258781d4c2d9f2c7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.3 MB (94344062 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc6c706282e894e9fe8fabf7c797478428c1166e8f93f09e43c8db0a12d0da49`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 11 Oct 2023 18:24:58 GMT
ADD file:e1a6c6c976e5e7c53eb2a7343a7a763b46e56828588535f4c79e63d6ec08198d in / 
# Wed, 11 Oct 2023 18:24:58 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 19:41:39 GMT
STOPSIGNAL SIGINT
# Wed, 11 Oct 2023 19:41:57 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 19:41:58 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 11 Oct 2023 19:41:59 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 11 Oct 2023 19:41:59 GMT
WORKDIR /var/www/html
# Wed, 11 Oct 2023 19:41:59 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 11 Oct 2023 19:41:59 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 11 Oct 2023 19:41:59 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 11 Oct 2023 19:41:59 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 11 Oct 2023 19:42:10 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 11 Oct 2023 19:42:10 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 11 Oct 2023 19:42:10 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 11 Oct 2023 19:42:10 GMT
USER adminer
# Wed, 11 Oct 2023 19:42:10 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 11 Oct 2023 19:42:10 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:dd0dc10f921f4b3b65b17f20d367374079e6cb4e26531624ee64caaaf4adcc28`  
		Last Modified: Wed, 11 Oct 2023 18:28:45 GMT  
		Size: 53.7 MB (53707810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef257294e6993147657842c1db0af6b35567fa3f5f825478621ef5bf09c4871e`  
		Last Modified: Wed, 11 Oct 2023 19:42:42 GMT  
		Size: 39.2 MB (39245727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e6ecde2f3d45f8a48e3c2d5c819eb535ac0f9abdde2051c01995434568dbf32`  
		Last Modified: Wed, 11 Oct 2023 19:42:35 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:600639d0d6dc1311b99169e0d63c4eb8f44bf21239f7000efc992a95063feb0e`  
		Last Modified: Wed, 11 Oct 2023 19:42:35 GMT  
		Size: 1.9 KB (1893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd2c7fb421d92b300b1834fa1788dc075e72d3d714336d0ce5986fb9cc29f92e`  
		Last Modified: Wed, 11 Oct 2023 19:42:35 GMT  
		Size: 1.5 KB (1476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c25edb0911c704d6f7039cb4e9694ca2af7fe37d3cf7e825fb28da46df996c40`  
		Last Modified: Wed, 11 Oct 2023 19:42:36 GMT  
		Size: 1.4 MB (1386273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:791d46cf692de232a6b0c1559e87ee318a302d9bab8df4d08760a9ab2c43e5ea`  
		Last Modified: Wed, 11 Oct 2023 19:42:35 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:latest` - linux; 386

```console
$ docker pull adminer@sha256:2c88cc2fa606983f2b3d568ffdafa27d0921f965558d18a05c0f5fc712601568
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.0 MB (96997514 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1094610c44e2e9c6caabf29c90d7fb49c39abe003f1fb9e06fe79f6e27a100c9`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Wed, 11 Oct 2023 18:08:02 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 11 Oct 2023 18:08:02 GMT
WORKDIR /var/www/html
# Wed, 11 Oct 2023 18:08:03 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 11 Oct 2023 18:08:03 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 11 Oct 2023 18:08:03 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 11 Oct 2023 18:08:03 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 11 Oct 2023 18:08:17 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 11 Oct 2023 18:08:17 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 11 Oct 2023 18:08:18 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 11 Oct 2023 18:08:18 GMT
USER adminer
# Wed, 11 Oct 2023 18:08:18 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 11 Oct 2023 18:08:18 GMT
EXPOSE 8080
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
	-	`sha256:5af98b95747bee44ac0cecc31da7755e40f44dd413b84fad60e37ba626a3a76b`  
		Last Modified: Wed, 11 Oct 2023 18:08:55 GMT  
		Size: 1.9 KB (1872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d974feb0c9497f7a8c58f10a18c88495d5b32bdd268c62331003ea6a942c0bf6`  
		Last Modified: Wed, 11 Oct 2023 18:08:55 GMT  
		Size: 1.5 KB (1478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fddf1828c60c72f33daab3a87427a7d171829535753723072a1e152f3ef01936`  
		Last Modified: Wed, 11 Oct 2023 18:08:56 GMT  
		Size: 1.4 MB (1386295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f597ad0158e1ea3aba7a4659db12d0c0954bfeda5fdc974ca864e89343f4ea1`  
		Last Modified: Wed, 11 Oct 2023 18:08:56 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:latest` - linux; mips64le

```console
$ docker pull adminer@sha256:e381e86167d3c2d53a9ef282bbbed1cb1ad2b6d27ed29367d477725abc1990d5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.6 MB (92632507 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1aeac6ce5d2f041b164fd41e9a4e72cc4f87258015631c78beb750929038af75`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Wed, 11 Oct 2023 20:25:20 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 11 Oct 2023 20:25:24 GMT
WORKDIR /var/www/html
# Wed, 11 Oct 2023 20:25:27 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 11 Oct 2023 20:25:30 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 11 Oct 2023 20:25:33 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 11 Oct 2023 20:25:37 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 11 Oct 2023 20:26:28 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 11 Oct 2023 20:26:31 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 11 Oct 2023 20:26:34 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 11 Oct 2023 20:26:37 GMT
USER adminer
# Wed, 11 Oct 2023 20:26:41 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 11 Oct 2023 20:26:44 GMT
EXPOSE 8080
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
	-	`sha256:77f27392480e440c2af5f35bbde6cefd9ede01e8aa21a3d111efd094fc17b271`  
		Last Modified: Wed, 11 Oct 2023 20:28:45 GMT  
		Size: 1.7 KB (1725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50c5cd11cc98c1a54e90754494f029f090ae77165f66daa68bf0fdf8afe35164`  
		Last Modified: Wed, 11 Oct 2023 20:28:45 GMT  
		Size: 1.5 KB (1477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:189b23e8f1b3c5f076dc4fb8f2d4211ce1c2c45294ae102d55e7e2d5c4886638`  
		Last Modified: Wed, 11 Oct 2023 20:28:46 GMT  
		Size: 1.4 MB (1387201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f989b6c6ecf562ac1ecfc4d5e76f330865aa68f06628685975188203137108ba`  
		Last Modified: Wed, 11 Oct 2023 20:28:45 GMT  
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
$ docker pull adminer@sha256:8d528a08459cd4c9ecc04fb999a78ea15d277a9f29fc0a4c638d0c727bcad97f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.7 MB (93708701 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e249f7d8c4a58fb4500763a3034393abadfef052e113228f0eadcbb705c08848`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 11 Oct 2023 17:50:40 GMT
ADD file:bb3ee20a7ddf364b23163c517132146872491e85ef2f1465bf7fd2ed33f94827 in / 
# Wed, 11 Oct 2023 17:50:44 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 22:32:09 GMT
STOPSIGNAL SIGINT
# Wed, 11 Oct 2023 22:39:39 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 22:39:42 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 11 Oct 2023 22:39:42 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 11 Oct 2023 22:39:43 GMT
WORKDIR /var/www/html
# Wed, 11 Oct 2023 22:39:43 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 11 Oct 2023 22:39:43 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 11 Oct 2023 22:39:43 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 11 Oct 2023 22:39:43 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 11 Oct 2023 22:41:33 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 11 Oct 2023 22:41:33 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 11 Oct 2023 22:41:34 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 11 Oct 2023 22:41:34 GMT
USER adminer
# Wed, 11 Oct 2023 22:41:34 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 11 Oct 2023 22:41:34 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:e651436ffb848f56da62cd2c80f206a288b94da8113c4c23a7e5502fb597ce23`  
		Last Modified: Wed, 11 Oct 2023 17:56:38 GMT  
		Size: 53.3 MB (53296378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2c575fbf44a3a7083af3fc636aea30f1cf9b740f3dc76ae083cf2a2700d35d1`  
		Last Modified: Wed, 11 Oct 2023 22:42:17 GMT  
		Size: 39.0 MB (39021675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e9c0af74b1292b337ce2d9000343a38538b9de1da1852202b8c22270fb379b1`  
		Last Modified: Wed, 11 Oct 2023 22:42:10 GMT  
		Size: 388.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1da19d286a2d15e09d89a2b662a7b16fc76fcf802c22fda19ad7d5f08565873b`  
		Last Modified: Wed, 11 Oct 2023 22:42:10 GMT  
		Size: 1.9 KB (1883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46ab979985444a22f0ca6ab8a93f9b4769bf499999ec67287cf4d2d65c6953aa`  
		Last Modified: Wed, 11 Oct 2023 22:42:10 GMT  
		Size: 1.5 KB (1479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3db85b1ed6626145763486f33bdaec608755b157f7b4cb25001c5fcedec6bf85`  
		Last Modified: Wed, 11 Oct 2023 22:42:10 GMT  
		Size: 1.4 MB (1386408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4129932287f7751ae20bb2c5c2e2c3e46f36a8a6dbf657e2b4142fe3ec4fd25b`  
		Last Modified: Wed, 11 Oct 2023 22:42:10 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `adminer:standalone`

```console
$ docker pull adminer@sha256:cc582ae15c97b6e8c726519b17004e819016dd11d6fda5f5898361575c435236
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
$ docker pull adminer@sha256:eea72a21cf1f4a95a5369ea76cbcfcd253974d1f2bc6fff6129ecc07a8cb996c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.9 MB (95941425 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a935a78b9b29f6ad7c46d08e6266a8419f6f0f355bb0b017f7320b381a7a9dc`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 11 Oct 2023 18:35:01 GMT
ADD file:8a9222387b89a9ac763fd72610ce01ab17f64387cbfde30a6af1861a82030aad in / 
# Wed, 11 Oct 2023 18:35:01 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 21:37:54 GMT
STOPSIGNAL SIGINT
# Wed, 11 Oct 2023 21:38:15 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 21:38:15 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 11 Oct 2023 21:38:16 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 11 Oct 2023 21:38:16 GMT
WORKDIR /var/www/html
# Wed, 11 Oct 2023 21:38:16 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 11 Oct 2023 21:38:16 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 11 Oct 2023 21:38:16 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 11 Oct 2023 21:38:16 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 11 Oct 2023 21:38:28 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 11 Oct 2023 21:38:28 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 11 Oct 2023 21:38:28 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 11 Oct 2023 21:38:28 GMT
USER adminer
# Wed, 11 Oct 2023 21:38:28 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 11 Oct 2023 21:38:28 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:69b3efbf67c2d9a46fdfdc8480b5a03ef73e9999a53aad57213447784f01eb6e`  
		Last Modified: Wed, 11 Oct 2023 18:39:54 GMT  
		Size: 55.1 MB (55058028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a0fdd089fb3c19ecd415c0ec8697e76347c06547c6418f4e0c2598cf3e6a396`  
		Last Modified: Wed, 11 Oct 2023 21:39:07 GMT  
		Size: 39.5 MB (39492762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:689786b0c396fae2f867afea8b0678012d77de73f01087f0b87b2f65d69160e0`  
		Last Modified: Wed, 11 Oct 2023 21:39:00 GMT  
		Size: 388.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bcf42cdb6b507c0e95ea21dd205b3073a3cc03072bc5ecb0984571c9319a61b`  
		Last Modified: Wed, 11 Oct 2023 21:39:00 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d507b34ef5ac1588f61ab244f00d1d6c16c10c1b722ca88d305807950d239bda`  
		Last Modified: Wed, 11 Oct 2023 21:39:00 GMT  
		Size: 1.5 KB (1475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04b8d4f964a85630221b12d10d1dcc6b918a66337213d36c6d0e58d88684181f`  
		Last Modified: Wed, 11 Oct 2023 21:39:01 GMT  
		Size: 1.4 MB (1386398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a75f8703cd73af4a5226ed8767f2f4bb39476c3f3c65b2263700ef30f709ccd`  
		Last Modified: Wed, 11 Oct 2023 21:39:00 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:standalone` - linux; arm variant v5

```console
$ docker pull adminer@sha256:a08d5ea30e6d3820954b4fabeaf9249a32a7b7572327ca1dd743b38f0cbd888f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.2 MB (91203171 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:baca868e51087a0125257821115f40dcdd565feb2f02c131e0752c41bf7edb03`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Wed, 11 Oct 2023 18:02:54 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 11 Oct 2023 18:02:55 GMT
WORKDIR /var/www/html
# Wed, 11 Oct 2023 18:02:55 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 11 Oct 2023 18:02:55 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 11 Oct 2023 18:02:55 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 11 Oct 2023 18:02:55 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 11 Oct 2023 18:03:10 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 11 Oct 2023 18:03:10 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 11 Oct 2023 18:03:10 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 11 Oct 2023 18:03:10 GMT
USER adminer
# Wed, 11 Oct 2023 18:03:11 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 11 Oct 2023 18:03:11 GMT
EXPOSE 8080
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
	-	`sha256:f882441c27deeb5eb8fbd7f5966d960e7df16b93ecdca98b2eda933479843de2`  
		Last Modified: Wed, 11 Oct 2023 18:03:47 GMT  
		Size: 1.9 KB (1871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5de4c1ac09f4beb23be8f166d5ac9e50f027246da8b704d4dcd1f55c56b1b293`  
		Last Modified: Wed, 11 Oct 2023 18:03:47 GMT  
		Size: 1.5 KB (1476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b04a8ddeb2dbd66e060775b6f617eb9966bc57bfe4a9188119fdce9f8b24305e`  
		Last Modified: Wed, 11 Oct 2023 18:03:47 GMT  
		Size: 1.4 MB (1386290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:574521a263f70127c05a1db8391a9f33d18c5844caaea07ea781626bd2156092`  
		Last Modified: Wed, 11 Oct 2023 18:03:47 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:standalone` - linux; arm variant v7

```console
$ docker pull adminer@sha256:6690c92a774eeb7b3a4bd31947c0641da6f80e18d3d9b38ff91869472cbc4203
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.8 MB (87794407 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb1b05568fc173e70d7da07ef277288dd9dd7fc76372fe16397945516ed0a194`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 11 Oct 2023 17:42:19 GMT
ADD file:684f3634c6b747a4caad8f9f820cc02b53a2122591fe215935c5497ec234c3ad in / 
# Wed, 11 Oct 2023 17:42:20 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:07:19 GMT
STOPSIGNAL SIGINT
# Wed, 11 Oct 2023 18:07:44 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 18:07:45 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 11 Oct 2023 18:07:45 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 11 Oct 2023 18:07:45 GMT
WORKDIR /var/www/html
# Wed, 11 Oct 2023 18:07:45 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 11 Oct 2023 18:07:46 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 11 Oct 2023 18:07:46 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 11 Oct 2023 18:07:46 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 11 Oct 2023 18:07:59 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 11 Oct 2023 18:08:00 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 11 Oct 2023 18:08:00 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 11 Oct 2023 18:08:00 GMT
USER adminer
# Wed, 11 Oct 2023 18:08:00 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 11 Oct 2023 18:08:00 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:33d0c7672db93e653471872c639cd6129ec25c168942e15a008c4920cafe62d7`  
		Last Modified: Wed, 11 Oct 2023 17:46:42 GMT  
		Size: 50.2 MB (50215704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7566087b942379bfc2c6a78692dbbe71d4bd1573cb81ddf2ece5c0c93bf1fe76`  
		Last Modified: Wed, 11 Oct 2023 18:08:44 GMT  
		Size: 36.2 MB (36188142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:050d8c68cbad80d1919f535fae7d348cde6b6488d6688095aa47dadb0de2a8cf`  
		Last Modified: Wed, 11 Oct 2023 18:08:34 GMT  
		Size: 394.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbd3cd900e2690837d6a8cbd717999c5224939f51724c7b2ec553c1419e5ab86`  
		Last Modified: Wed, 11 Oct 2023 18:08:34 GMT  
		Size: 1.9 KB (1871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cce366bf543cd120f357c96573fa045f6c544189b422cbc2d49121b993af5e97`  
		Last Modified: Wed, 11 Oct 2023 18:08:34 GMT  
		Size: 1.5 KB (1476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff97645728e1b3ae0f3d4382f2919cf8e8f896b310af1b8a020cf1a4d4a151ce`  
		Last Modified: Wed, 11 Oct 2023 18:08:34 GMT  
		Size: 1.4 MB (1386329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa31a5f1d18ca530111bc2c3cc0da34e10ab6329822a5c075549811eda2e985b`  
		Last Modified: Wed, 11 Oct 2023 18:08:34 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:standalone` - linux; arm64 variant v8

```console
$ docker pull adminer@sha256:af7089fbd20cb08f11edf0f60a254b18f0c90a32537952e5258781d4c2d9f2c7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.3 MB (94344062 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc6c706282e894e9fe8fabf7c797478428c1166e8f93f09e43c8db0a12d0da49`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 11 Oct 2023 18:24:58 GMT
ADD file:e1a6c6c976e5e7c53eb2a7343a7a763b46e56828588535f4c79e63d6ec08198d in / 
# Wed, 11 Oct 2023 18:24:58 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 19:41:39 GMT
STOPSIGNAL SIGINT
# Wed, 11 Oct 2023 19:41:57 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 19:41:58 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 11 Oct 2023 19:41:59 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 11 Oct 2023 19:41:59 GMT
WORKDIR /var/www/html
# Wed, 11 Oct 2023 19:41:59 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 11 Oct 2023 19:41:59 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 11 Oct 2023 19:41:59 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 11 Oct 2023 19:41:59 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 11 Oct 2023 19:42:10 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 11 Oct 2023 19:42:10 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 11 Oct 2023 19:42:10 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 11 Oct 2023 19:42:10 GMT
USER adminer
# Wed, 11 Oct 2023 19:42:10 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 11 Oct 2023 19:42:10 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:dd0dc10f921f4b3b65b17f20d367374079e6cb4e26531624ee64caaaf4adcc28`  
		Last Modified: Wed, 11 Oct 2023 18:28:45 GMT  
		Size: 53.7 MB (53707810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef257294e6993147657842c1db0af6b35567fa3f5f825478621ef5bf09c4871e`  
		Last Modified: Wed, 11 Oct 2023 19:42:42 GMT  
		Size: 39.2 MB (39245727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e6ecde2f3d45f8a48e3c2d5c819eb535ac0f9abdde2051c01995434568dbf32`  
		Last Modified: Wed, 11 Oct 2023 19:42:35 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:600639d0d6dc1311b99169e0d63c4eb8f44bf21239f7000efc992a95063feb0e`  
		Last Modified: Wed, 11 Oct 2023 19:42:35 GMT  
		Size: 1.9 KB (1893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd2c7fb421d92b300b1834fa1788dc075e72d3d714336d0ce5986fb9cc29f92e`  
		Last Modified: Wed, 11 Oct 2023 19:42:35 GMT  
		Size: 1.5 KB (1476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c25edb0911c704d6f7039cb4e9694ca2af7fe37d3cf7e825fb28da46df996c40`  
		Last Modified: Wed, 11 Oct 2023 19:42:36 GMT  
		Size: 1.4 MB (1386273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:791d46cf692de232a6b0c1559e87ee318a302d9bab8df4d08760a9ab2c43e5ea`  
		Last Modified: Wed, 11 Oct 2023 19:42:35 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:standalone` - linux; 386

```console
$ docker pull adminer@sha256:2c88cc2fa606983f2b3d568ffdafa27d0921f965558d18a05c0f5fc712601568
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.0 MB (96997514 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1094610c44e2e9c6caabf29c90d7fb49c39abe003f1fb9e06fe79f6e27a100c9`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Wed, 11 Oct 2023 18:08:02 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 11 Oct 2023 18:08:02 GMT
WORKDIR /var/www/html
# Wed, 11 Oct 2023 18:08:03 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 11 Oct 2023 18:08:03 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 11 Oct 2023 18:08:03 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 11 Oct 2023 18:08:03 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 11 Oct 2023 18:08:17 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 11 Oct 2023 18:08:17 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 11 Oct 2023 18:08:18 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 11 Oct 2023 18:08:18 GMT
USER adminer
# Wed, 11 Oct 2023 18:08:18 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 11 Oct 2023 18:08:18 GMT
EXPOSE 8080
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
	-	`sha256:5af98b95747bee44ac0cecc31da7755e40f44dd413b84fad60e37ba626a3a76b`  
		Last Modified: Wed, 11 Oct 2023 18:08:55 GMT  
		Size: 1.9 KB (1872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d974feb0c9497f7a8c58f10a18c88495d5b32bdd268c62331003ea6a942c0bf6`  
		Last Modified: Wed, 11 Oct 2023 18:08:55 GMT  
		Size: 1.5 KB (1478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fddf1828c60c72f33daab3a87427a7d171829535753723072a1e152f3ef01936`  
		Last Modified: Wed, 11 Oct 2023 18:08:56 GMT  
		Size: 1.4 MB (1386295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f597ad0158e1ea3aba7a4659db12d0c0954bfeda5fdc974ca864e89343f4ea1`  
		Last Modified: Wed, 11 Oct 2023 18:08:56 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:standalone` - linux; mips64le

```console
$ docker pull adminer@sha256:e381e86167d3c2d53a9ef282bbbed1cb1ad2b6d27ed29367d477725abc1990d5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.6 MB (92632507 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1aeac6ce5d2f041b164fd41e9a4e72cc4f87258015631c78beb750929038af75`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Wed, 11 Oct 2023 20:25:20 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 11 Oct 2023 20:25:24 GMT
WORKDIR /var/www/html
# Wed, 11 Oct 2023 20:25:27 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 11 Oct 2023 20:25:30 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 11 Oct 2023 20:25:33 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 11 Oct 2023 20:25:37 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 11 Oct 2023 20:26:28 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 11 Oct 2023 20:26:31 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 11 Oct 2023 20:26:34 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 11 Oct 2023 20:26:37 GMT
USER adminer
# Wed, 11 Oct 2023 20:26:41 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 11 Oct 2023 20:26:44 GMT
EXPOSE 8080
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
	-	`sha256:77f27392480e440c2af5f35bbde6cefd9ede01e8aa21a3d111efd094fc17b271`  
		Last Modified: Wed, 11 Oct 2023 20:28:45 GMT  
		Size: 1.7 KB (1725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50c5cd11cc98c1a54e90754494f029f090ae77165f66daa68bf0fdf8afe35164`  
		Last Modified: Wed, 11 Oct 2023 20:28:45 GMT  
		Size: 1.5 KB (1477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:189b23e8f1b3c5f076dc4fb8f2d4211ce1c2c45294ae102d55e7e2d5c4886638`  
		Last Modified: Wed, 11 Oct 2023 20:28:46 GMT  
		Size: 1.4 MB (1387201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f989b6c6ecf562ac1ecfc4d5e76f330865aa68f06628685975188203137108ba`  
		Last Modified: Wed, 11 Oct 2023 20:28:45 GMT  
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
$ docker pull adminer@sha256:8d528a08459cd4c9ecc04fb999a78ea15d277a9f29fc0a4c638d0c727bcad97f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.7 MB (93708701 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e249f7d8c4a58fb4500763a3034393abadfef052e113228f0eadcbb705c08848`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 11 Oct 2023 17:50:40 GMT
ADD file:bb3ee20a7ddf364b23163c517132146872491e85ef2f1465bf7fd2ed33f94827 in / 
# Wed, 11 Oct 2023 17:50:44 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 22:32:09 GMT
STOPSIGNAL SIGINT
# Wed, 11 Oct 2023 22:39:39 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 22:39:42 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 11 Oct 2023 22:39:42 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 11 Oct 2023 22:39:43 GMT
WORKDIR /var/www/html
# Wed, 11 Oct 2023 22:39:43 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 11 Oct 2023 22:39:43 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 11 Oct 2023 22:39:43 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 11 Oct 2023 22:39:43 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 11 Oct 2023 22:41:33 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 11 Oct 2023 22:41:33 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 11 Oct 2023 22:41:34 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 11 Oct 2023 22:41:34 GMT
USER adminer
# Wed, 11 Oct 2023 22:41:34 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 11 Oct 2023 22:41:34 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:e651436ffb848f56da62cd2c80f206a288b94da8113c4c23a7e5502fb597ce23`  
		Last Modified: Wed, 11 Oct 2023 17:56:38 GMT  
		Size: 53.3 MB (53296378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2c575fbf44a3a7083af3fc636aea30f1cf9b740f3dc76ae083cf2a2700d35d1`  
		Last Modified: Wed, 11 Oct 2023 22:42:17 GMT  
		Size: 39.0 MB (39021675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e9c0af74b1292b337ce2d9000343a38538b9de1da1852202b8c22270fb379b1`  
		Last Modified: Wed, 11 Oct 2023 22:42:10 GMT  
		Size: 388.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1da19d286a2d15e09d89a2b662a7b16fc76fcf802c22fda19ad7d5f08565873b`  
		Last Modified: Wed, 11 Oct 2023 22:42:10 GMT  
		Size: 1.9 KB (1883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46ab979985444a22f0ca6ab8a93f9b4769bf499999ec67287cf4d2d65c6953aa`  
		Last Modified: Wed, 11 Oct 2023 22:42:10 GMT  
		Size: 1.5 KB (1479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3db85b1ed6626145763486f33bdaec608755b157f7b4cb25001c5fcedec6bf85`  
		Last Modified: Wed, 11 Oct 2023 22:42:10 GMT  
		Size: 1.4 MB (1386408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4129932287f7751ae20bb2c5c2e2c3e46f36a8a6dbf657e2b4142fe3ec4fd25b`  
		Last Modified: Wed, 11 Oct 2023 22:42:10 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
