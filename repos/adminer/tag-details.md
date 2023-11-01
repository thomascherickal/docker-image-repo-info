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
$ docker pull adminer@sha256:b7f0e6681e9a77916daf2f070616d25e3fd687b84550aa6673de9a24407dd613
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
$ docker pull adminer@sha256:b96876e1c6d4eda21b2653d54bb8c9d4674fc177749254c5a44d097f92e2362e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.9 MB (95941196 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5cec1739340987c68ebd5535d5297dc62cc4fa489a253b4d84bb800b461e129`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Wed, 01 Nov 2023 02:53:39 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 01 Nov 2023 02:53:39 GMT
WORKDIR /var/www/html
# Wed, 01 Nov 2023 02:53:39 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 01 Nov 2023 02:53:39 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 01 Nov 2023 02:53:39 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 01 Nov 2023 02:53:39 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 01 Nov 2023 02:53:50 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 01 Nov 2023 02:53:50 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 01 Nov 2023 02:53:50 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 01 Nov 2023 02:53:50 GMT
USER adminer
# Wed, 01 Nov 2023 02:53:50 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 01 Nov 2023 02:53:50 GMT
EXPOSE 8080
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
	-	`sha256:bf435083814d20c35b08cac2c04f42a971fe8c772a6ff6ab5ea2dbb4c5365923`  
		Last Modified: Wed, 01 Nov 2023 02:54:24 GMT  
		Size: 1.9 KB (1876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:298e667e63eeffb2a143be3c3aeed4888c95d316e453939646663ae94cb39b38`  
		Last Modified: Wed, 01 Nov 2023 02:54:25 GMT  
		Size: 1.5 KB (1482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:009b4e930c2c0c866efcbe990a45b4aaa86c6ae9428410afb5842ed5a4a61a2f`  
		Last Modified: Wed, 01 Nov 2023 02:54:25 GMT  
		Size: 1.4 MB (1386349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:795fdddea697817d7c6a47b855376bc15a2ece944ad41fb076688cf55c7a749a`  
		Last Modified: Wed, 01 Nov 2023 02:54:24 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4` - linux; arm variant v5

```console
$ docker pull adminer@sha256:37f77f5ee6832c7e087446aedd7fbc4759897435702305e7331410f4ccf749a9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.2 MB (91203583 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4428e260c8ac1e52db7ab4bca8db1cc7baafd67bb17a2206f99ccb97cb9c167`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 01 Nov 2023 00:48:39 GMT
ADD file:6fcdedd346da0744f7f45d0e7df77336a37ce87345bd414bd4e198804980781e in / 
# Wed, 01 Nov 2023 00:48:40 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 06:41:07 GMT
STOPSIGNAL SIGINT
# Wed, 01 Nov 2023 06:41:38 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 06:41:39 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 01 Nov 2023 06:41:40 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 01 Nov 2023 06:41:40 GMT
WORKDIR /var/www/html
# Wed, 01 Nov 2023 06:41:40 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 01 Nov 2023 06:41:40 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 01 Nov 2023 06:41:40 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 01 Nov 2023 06:41:40 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 01 Nov 2023 06:41:55 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 01 Nov 2023 06:41:55 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 01 Nov 2023 06:41:55 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 01 Nov 2023 06:41:56 GMT
USER adminer
# Wed, 01 Nov 2023 06:41:56 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 01 Nov 2023 06:41:56 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:e0adb3cac2906548cd3544bf3c384be3e3bdca9d41c37e11c160813af74301b9`  
		Last Modified: Wed, 01 Nov 2023 00:51:49 GMT  
		Size: 52.6 MB (52563334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e3623d9fb2289bbcd9a4586d409f13e8c27695bdb11f4c43599571aa1229528`  
		Last Modified: Wed, 01 Nov 2023 06:42:42 GMT  
		Size: 37.2 MB (37249740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28eac10d8db23ee6ea32d6b0c826db4a2dcbcd194ce18e99629fef2b283b4168`  
		Last Modified: Wed, 01 Nov 2023 06:42:33 GMT  
		Size: 389.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5779125ab319b67fbc7cf3bcaa969968771e9e472e58c08976728bb8d7569d56`  
		Last Modified: Wed, 01 Nov 2023 06:42:33 GMT  
		Size: 1.9 KB (1869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1952b238fb472fe6155a5c880e5d83d4c58dee30db79ba608c878282838500e`  
		Last Modified: Wed, 01 Nov 2023 06:42:33 GMT  
		Size: 1.5 KB (1476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85025f444620cafd6192a2667af59fdf4aca316094a82a43909a7e9f96e254f9`  
		Last Modified: Wed, 01 Nov 2023 06:42:33 GMT  
		Size: 1.4 MB (1386285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56f0c59e7ad269f06b6107635f33308fe74056eebdde42c8932886bf95c1885b`  
		Last Modified: Wed, 01 Nov 2023 06:42:33 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4` - linux; arm variant v7

```console
$ docker pull adminer@sha256:03812b425c6b805691941ae806db34dc0b8a3f161f3a4e11ea0c54eb783037fb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.8 MB (87794095 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c9e7020270d790860f62ddf4e490a5409714c8f1d910f0e5552e34467640d9d`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Wed, 01 Nov 2023 02:13:44 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 01 Nov 2023 02:13:44 GMT
WORKDIR /var/www/html
# Wed, 01 Nov 2023 02:13:44 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 01 Nov 2023 02:13:44 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 01 Nov 2023 02:13:44 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 01 Nov 2023 02:13:44 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 01 Nov 2023 02:14:02 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 01 Nov 2023 02:14:02 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 01 Nov 2023 02:14:02 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 01 Nov 2023 02:14:02 GMT
USER adminer
# Wed, 01 Nov 2023 02:14:02 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 01 Nov 2023 02:14:02 GMT
EXPOSE 8080
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
	-	`sha256:b5ff4543277751a4ec131370a18afcbdcefbb299cac4f8b46d83ca0bb7e2fbb5`  
		Last Modified: Wed, 01 Nov 2023 02:14:32 GMT  
		Size: 1.9 KB (1867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8035a3dd0d4bf0c16736f3dc9982fdf586cb8db7c9c17bdfc7b7857d8236a5f8`  
		Last Modified: Wed, 01 Nov 2023 02:14:32 GMT  
		Size: 1.5 KB (1482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3e860a8d0ed1174c57c59e038d17c8c011e9262aac708373f223685b8a474c3`  
		Last Modified: Wed, 01 Nov 2023 02:14:32 GMT  
		Size: 1.4 MB (1386280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46610df748fd7888da3ef3e1419131554e3c580380b72af8c2182bd4b0c868d3`  
		Last Modified: Wed, 01 Nov 2023 02:14:32 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4` - linux; arm64 variant v8

```console
$ docker pull adminer@sha256:63e8c57d2e82e0d50f641f56ce18316ba1f8a12a4640c2b6966453d198a8f14f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.3 MB (94343887 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e729f030ea5398e5fb915c10c2a7b811bffbcfd0932c22b49cba6738c053e8b6`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Wed, 01 Nov 2023 02:01:40 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 01 Nov 2023 02:01:40 GMT
WORKDIR /var/www/html
# Wed, 01 Nov 2023 02:01:40 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 01 Nov 2023 02:01:40 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 01 Nov 2023 02:01:40 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 01 Nov 2023 02:01:40 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 01 Nov 2023 02:01:50 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 01 Nov 2023 02:01:50 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 01 Nov 2023 02:01:50 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 01 Nov 2023 02:01:51 GMT
USER adminer
# Wed, 01 Nov 2023 02:01:51 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 01 Nov 2023 02:01:51 GMT
EXPOSE 8080
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
	-	`sha256:96cc754b457a6496cd3a8ba90b44ea5d39534c43f26dc2cb557b71a76902a3d6`  
		Last Modified: Wed, 01 Nov 2023 02:02:15 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:535170e27a39ee08c1372464244541113d3a4d899c1c7676ebca43a9f09b2421`  
		Last Modified: Wed, 01 Nov 2023 02:02:15 GMT  
		Size: 1.5 KB (1482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83e4006979461007bc0f7c1b0bb3b0675f29b405562d0cc37f5cf5b0711a309e`  
		Last Modified: Wed, 01 Nov 2023 02:02:16 GMT  
		Size: 1.4 MB (1386269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aecfb4d8f96734c7035d67c5e3b751eb15f305ae0b1d2855921c5d1d0d83b5bc`  
		Last Modified: Wed, 01 Nov 2023 02:02:15 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4` - linux; 386

```console
$ docker pull adminer@sha256:a21c1d6915687a26e34d9f2f09f9b5104e64bc71aa36e19afae9c5d8c67a9040
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.0 MB (96997500 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3517f7704a6b833432e5e5e0144c6ce4e15ba0199adde89fb66fba372920f37`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 01 Nov 2023 00:39:06 GMT
ADD file:4095d27bc1a281dda044919be3bb570d581df169c01f22b0963b38e0dd6d9eff in / 
# Wed, 01 Nov 2023 00:39:07 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 08:16:42 GMT
STOPSIGNAL SIGINT
# Wed, 01 Nov 2023 08:17:12 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 08:17:13 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 01 Nov 2023 08:17:14 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 01 Nov 2023 08:17:14 GMT
WORKDIR /var/www/html
# Wed, 01 Nov 2023 08:17:14 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 01 Nov 2023 08:17:14 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 01 Nov 2023 08:17:14 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 01 Nov 2023 08:17:14 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 01 Nov 2023 08:17:28 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 01 Nov 2023 08:17:28 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 01 Nov 2023 08:17:28 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 01 Nov 2023 08:17:28 GMT
USER adminer
# Wed, 01 Nov 2023 08:17:28 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 01 Nov 2023 08:17:28 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:95d6aa56ba74b8ed0a732c4676a2c45c84a18076696d466cd9bf0b459c600e02`  
		Last Modified: Wed, 01 Nov 2023 00:43:49 GMT  
		Size: 56.0 MB (56046261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80589068561f705cd353c87358a0cecc8311057c942f023093c00c5ae59b0da4`  
		Last Modified: Wed, 01 Nov 2023 08:18:18 GMT  
		Size: 39.6 MB (39560745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c2dcd79bac9186cbea2e89e7c6085867c2ec84a4322ad7e80642bbe4e78fc42`  
		Last Modified: Wed, 01 Nov 2023 08:18:07 GMT  
		Size: 389.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c684759995fea1dd384d011644236354c8d098a591ea7926cac740391deb251`  
		Last Modified: Wed, 01 Nov 2023 08:18:07 GMT  
		Size: 1.9 KB (1866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a604bb0980f5b877ea1cfe73a85385ed541f85c82b22348d27f8d97a04d1ef76`  
		Last Modified: Wed, 01 Nov 2023 08:18:07 GMT  
		Size: 1.5 KB (1476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e27ee00f7fee2ee221e39d45b4abcfd90c63753f5e7263e8f30c67520aebc624`  
		Last Modified: Wed, 01 Nov 2023 08:18:08 GMT  
		Size: 1.4 MB (1386271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efa1816dcac43959f858ffcdbab80217277171e01d1c9a8fe3ebdd1c15db6697`  
		Last Modified: Wed, 01 Nov 2023 08:18:07 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4` - linux; mips64le

```console
$ docker pull adminer@sha256:ab1415fc7ebc72555fc80c9a4f64e05dae784d0acf5368241c39bf74ddf5bce4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.6 MB (92632325 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7faddbe6a665e6871431356947ac3c57cd3c6c20b85c84172da87b3f93017faa`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 01 Nov 2023 01:09:34 GMT
ADD file:2c9f9140e731974a497825454c08d67829f514a83742973e30454cc905ebac6c in / 
# Wed, 01 Nov 2023 01:09:39 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 06:47:42 GMT
STOPSIGNAL SIGINT
# Wed, 01 Nov 2023 06:49:39 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 06:49:45 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 01 Nov 2023 06:49:52 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 01 Nov 2023 06:49:55 GMT
WORKDIR /var/www/html
# Wed, 01 Nov 2023 06:49:58 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 01 Nov 2023 06:50:02 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 01 Nov 2023 06:50:05 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 01 Nov 2023 06:50:08 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 01 Nov 2023 06:51:01 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 01 Nov 2023 06:51:04 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 01 Nov 2023 06:51:07 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 01 Nov 2023 06:51:10 GMT
USER adminer
# Wed, 01 Nov 2023 06:51:14 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 01 Nov 2023 06:51:17 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:a10c6e715fcf314db953339b3e58b9e0167f6cd2d02bf633e20282058eb83331`  
		Last Modified: Wed, 01 Nov 2023 01:20:31 GMT  
		Size: 53.3 MB (53288991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3e05f3781dcb9702ce843ce679283bdea07c6614cdcba5a271127fd6bc7bb81`  
		Last Modified: Wed, 01 Nov 2023 06:53:43 GMT  
		Size: 38.0 MB (37952018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c67397db1f05d9d07b2053012f95d10c64b397e5f8578a8252c397958089cc7`  
		Last Modified: Wed, 01 Nov 2023 06:53:16 GMT  
		Size: 395.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12601b86b1fe6286ef174f4194db89610719071fc99b6004600546e313b75afc`  
		Last Modified: Wed, 01 Nov 2023 06:53:16 GMT  
		Size: 1.7 KB (1725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cf53f1325a00115717e22a2ad400917ea970c2863a9f0aa384c81111fe5f754`  
		Last Modified: Wed, 01 Nov 2023 06:53:16 GMT  
		Size: 1.5 KB (1481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fb917f0d920d8d2969e5b26d77d9384c94934f2c5d72677b658a9483e180240`  
		Last Modified: Wed, 01 Nov 2023 06:53:17 GMT  
		Size: 1.4 MB (1387222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af14639f108dd10f1d2bd5ea098b67c59009583ed8e393315c464ec4223e37d8`  
		Last Modified: Wed, 01 Nov 2023 06:53:16 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4` - linux; ppc64le

```console
$ docker pull adminer@sha256:489934d719089bd1c3827bdf673dcf7636376fbcbcfe837c4b7fa275ba366b62
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.3 MB (101265232 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6176ac38dfe8ab4e16662cc637ab4fb4b6f98c2e489cf4b4e6a66d578229ac6a`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Wed, 01 Nov 2023 02:50:13 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 01 Nov 2023 02:50:15 GMT
WORKDIR /var/www/html
# Wed, 01 Nov 2023 02:50:15 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 01 Nov 2023 02:50:15 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 01 Nov 2023 02:50:16 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 01 Nov 2023 02:50:16 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 01 Nov 2023 02:50:41 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 01 Nov 2023 02:50:42 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 01 Nov 2023 02:50:42 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 01 Nov 2023 02:50:43 GMT
USER adminer
# Wed, 01 Nov 2023 02:50:43 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 01 Nov 2023 02:50:44 GMT
EXPOSE 8080
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
	-	`sha256:c949ba7225949db3835c8321c7fd3fc61042abadd084780530933f2490a389ac`  
		Last Modified: Wed, 01 Nov 2023 02:51:40 GMT  
		Size: 1.9 KB (1878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69b23613e6440faf4dd53e85cce3379a37d371a55de8c3711313d4e8c2bdfcc7`  
		Last Modified: Wed, 01 Nov 2023 02:51:41 GMT  
		Size: 1.5 KB (1480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7424b8a43895b887591228e0a253d09fc56191f47ab5b4ab56d6fac2e6cbd9af`  
		Last Modified: Wed, 01 Nov 2023 02:51:41 GMT  
		Size: 1.4 MB (1386466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ee20cb0c3714aa128b4be5cdf5911002f2596f04b95e7e03962e22f45920bd3`  
		Last Modified: Wed, 01 Nov 2023 02:51:40 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4` - linux; s390x

```console
$ docker pull adminer@sha256:febeaf64eb35379728a191c91b4c0fd744f0f25716db5b3a6383382bd813875b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.7 MB (93708845 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f56dc24645f9175629077bc05d2d1ef72a10391d530b75320409f480c64d72b5`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Wed, 01 Nov 2023 01:50:10 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 01 Nov 2023 01:50:10 GMT
WORKDIR /var/www/html
# Wed, 01 Nov 2023 01:50:10 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 01 Nov 2023 01:50:10 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 01 Nov 2023 01:50:10 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 01 Nov 2023 01:50:10 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 01 Nov 2023 01:50:18 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 01 Nov 2023 01:50:18 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 01 Nov 2023 01:50:18 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 01 Nov 2023 01:50:18 GMT
USER adminer
# Wed, 01 Nov 2023 01:50:18 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 01 Nov 2023 01:50:19 GMT
EXPOSE 8080
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
	-	`sha256:0ddb015dd3525d29ecb468826e1900bd5a42aedf948d046cf67cbb849116174a`  
		Last Modified: Wed, 01 Nov 2023 01:50:54 GMT  
		Size: 1.9 KB (1879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eeda1242b7f2fccc214b7bce16debf257837f0e99de553d8b0899289fdf4381`  
		Last Modified: Wed, 01 Nov 2023 01:50:54 GMT  
		Size: 1.5 KB (1477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b79f82c6e4dc3c8fa378683a146466b55a41e4a9b35103811abe39ff47528f4`  
		Last Modified: Wed, 01 Nov 2023 01:50:55 GMT  
		Size: 1.4 MB (1386366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:245a8a7cccf20a91e5d673ee924ca9853c1d060c66fdb377e8b8ca63166ac4cc`  
		Last Modified: Wed, 01 Nov 2023 01:50:54 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `adminer:4-fastcgi`

```console
$ docker pull adminer@sha256:312c0213bc482710a1129efafd0e8a9df7c8f74203cfc2effce3bd1273d8483c
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
$ docker pull adminer@sha256:640e60b56e718fd2129bc9dcf1cb60e4ae5be47614831844f3ae58081ef992a3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.2 MB (91206303 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:148a1a15fd20132f8babeb810dd6b79f0ad5b9affc91c2f8541b13ff8460c027`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Wed, 01 Nov 2023 00:48:39 GMT
ADD file:6fcdedd346da0744f7f45d0e7df77336a37ce87345bd414bd4e198804980781e in / 
# Wed, 01 Nov 2023 00:48:40 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 06:41:07 GMT
STOPSIGNAL SIGINT
# Wed, 01 Nov 2023 06:41:38 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 06:41:39 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 01 Nov 2023 06:42:05 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Wed, 01 Nov 2023 06:42:06 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 01 Nov 2023 06:42:06 GMT
WORKDIR /var/www/html
# Wed, 01 Nov 2023 06:42:06 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 01 Nov 2023 06:42:06 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 01 Nov 2023 06:42:06 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 01 Nov 2023 06:42:07 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 01 Nov 2023 06:42:20 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 01 Nov 2023 06:42:20 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 01 Nov 2023 06:42:21 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 01 Nov 2023 06:42:21 GMT
USER adminer
# Wed, 01 Nov 2023 06:42:21 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:e0adb3cac2906548cd3544bf3c384be3e3bdca9d41c37e11c160813af74301b9`  
		Last Modified: Wed, 01 Nov 2023 00:51:49 GMT  
		Size: 52.6 MB (52563334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e3623d9fb2289bbcd9a4586d409f13e8c27695bdb11f4c43599571aa1229528`  
		Last Modified: Wed, 01 Nov 2023 06:42:42 GMT  
		Size: 37.2 MB (37249740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28eac10d8db23ee6ea32d6b0c826db4a2dcbcd194ce18e99629fef2b283b4168`  
		Last Modified: Wed, 01 Nov 2023 06:42:33 GMT  
		Size: 389.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2319565cc3ff6648a187190305386506317c8e8b916e4c68a2fc7c4901bfade4`  
		Last Modified: Wed, 01 Nov 2023 06:42:59 GMT  
		Size: 2.7 KB (2712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d82fa5f5f057baa718cb408944b78d134414e710547b7fefe9e313b157794f83`  
		Last Modified: Wed, 01 Nov 2023 06:42:59 GMT  
		Size: 1.9 KB (1867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26294c9823754b7b6c80e1e42807e3d303d36ebf56f05c24f0267cb9f42f1a5c`  
		Last Modified: Wed, 01 Nov 2023 06:42:58 GMT  
		Size: 1.5 KB (1476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1805ed31823bd60aec3a510dc6813b3e6df00428670492f806313f056d98accc`  
		Last Modified: Wed, 01 Nov 2023 06:42:59 GMT  
		Size: 1.4 MB (1386295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3379baf5fcc5e2ee2f374067c687e3614bb3a564ce83ec47aa3088df5900c339`  
		Last Modified: Wed, 01 Nov 2023 06:42:59 GMT  
		Size: 490.0 B  
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
$ docker pull adminer@sha256:baf03604dff500f1ff723513a538bd2632e854534952802ef3c2757ab9ec7284
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.0 MB (97000221 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a29b774050e6bb60654c4629b38274b8039fbff780360aa51ab5c918374888e`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Wed, 01 Nov 2023 00:39:06 GMT
ADD file:4095d27bc1a281dda044919be3bb570d581df169c01f22b0963b38e0dd6d9eff in / 
# Wed, 01 Nov 2023 00:39:07 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 08:16:42 GMT
STOPSIGNAL SIGINT
# Wed, 01 Nov 2023 08:17:12 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 08:17:13 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 01 Nov 2023 08:17:40 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Wed, 01 Nov 2023 08:17:41 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 01 Nov 2023 08:17:41 GMT
WORKDIR /var/www/html
# Wed, 01 Nov 2023 08:17:41 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 01 Nov 2023 08:17:41 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 01 Nov 2023 08:17:41 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 01 Nov 2023 08:17:41 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 01 Nov 2023 08:17:54 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 01 Nov 2023 08:17:55 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 01 Nov 2023 08:17:55 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 01 Nov 2023 08:17:55 GMT
USER adminer
# Wed, 01 Nov 2023 08:17:55 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:95d6aa56ba74b8ed0a732c4676a2c45c84a18076696d466cd9bf0b459c600e02`  
		Last Modified: Wed, 01 Nov 2023 00:43:49 GMT  
		Size: 56.0 MB (56046261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80589068561f705cd353c87358a0cecc8311057c942f023093c00c5ae59b0da4`  
		Last Modified: Wed, 01 Nov 2023 08:18:18 GMT  
		Size: 39.6 MB (39560745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c2dcd79bac9186cbea2e89e7c6085867c2ec84a4322ad7e80642bbe4e78fc42`  
		Last Modified: Wed, 01 Nov 2023 08:18:07 GMT  
		Size: 389.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce8777aa37435cb70275cafb5973d4c38ade71490ab02d4690e7243d7f42fa99`  
		Last Modified: Wed, 01 Nov 2023 08:18:38 GMT  
		Size: 2.7 KB (2708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3092383d86bf2247454565915d60711072083b945827d3a71d04b2e8e7d5a24`  
		Last Modified: Wed, 01 Nov 2023 08:18:38 GMT  
		Size: 1.9 KB (1866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58ab83e0c0b5af9550f8219863a015b9f64aac19bfd190214266dddcdae1987d`  
		Last Modified: Wed, 01 Nov 2023 08:18:38 GMT  
		Size: 1.5 KB (1479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1ad071ea7480f652575c1ff65ee4ef869a9eb9b6f053ca5f2dae11776838485`  
		Last Modified: Wed, 01 Nov 2023 08:18:38 GMT  
		Size: 1.4 MB (1386283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31f82fe0941deccb9e97f691bccd364714153f8af834bfb61010a0edeed7d95b`  
		Last Modified: Wed, 01 Nov 2023 08:18:38 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-fastcgi` - linux; mips64le

```console
$ docker pull adminer@sha256:d5005a80e57907d2bf1e882cd453c47a7c6e2044997f7f5f2d6c1737a73c8e53
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.6 MB (92635040 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46fee5e1b1c3fefa23d38e502f9c95f79c82daaf2e4a9015a2f079af2d582ea5`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Wed, 01 Nov 2023 01:09:34 GMT
ADD file:2c9f9140e731974a497825454c08d67829f514a83742973e30454cc905ebac6c in / 
# Wed, 01 Nov 2023 01:09:39 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 06:47:42 GMT
STOPSIGNAL SIGINT
# Wed, 01 Nov 2023 06:49:39 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 06:49:45 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 01 Nov 2023 06:51:29 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Wed, 01 Nov 2023 06:51:36 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 01 Nov 2023 06:51:39 GMT
WORKDIR /var/www/html
# Wed, 01 Nov 2023 06:51:42 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 01 Nov 2023 06:51:46 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 01 Nov 2023 06:51:49 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 01 Nov 2023 06:51:52 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 01 Nov 2023 06:52:43 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 01 Nov 2023 06:52:46 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 01 Nov 2023 06:52:50 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 01 Nov 2023 06:52:53 GMT
USER adminer
# Wed, 01 Nov 2023 06:52:56 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:a10c6e715fcf314db953339b3e58b9e0167f6cd2d02bf633e20282058eb83331`  
		Last Modified: Wed, 01 Nov 2023 01:20:31 GMT  
		Size: 53.3 MB (53288991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3e05f3781dcb9702ce843ce679283bdea07c6614cdcba5a271127fd6bc7bb81`  
		Last Modified: Wed, 01 Nov 2023 06:53:43 GMT  
		Size: 38.0 MB (37952018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c67397db1f05d9d07b2053012f95d10c64b397e5f8578a8252c397958089cc7`  
		Last Modified: Wed, 01 Nov 2023 06:53:16 GMT  
		Size: 395.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1efe29ad2e6399b06c40a1f74ef708babaf49feb6d4a81ffc433dbe62507869a`  
		Last Modified: Wed, 01 Nov 2023 06:54:03 GMT  
		Size: 2.7 KB (2714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5e18030af38a29600f3748bcbad3e59b6ec984e1949a992135f469b7a511bb4`  
		Last Modified: Wed, 01 Nov 2023 06:54:03 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a32ef85d04c2f926ef96c9ffa9dcac7659bc192103442cb5a3c6496c49d1f32`  
		Last Modified: Wed, 01 Nov 2023 06:54:03 GMT  
		Size: 1.5 KB (1482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce599942d3ca2661bbeab5bf9752328464303caf6cfbfa70875693cadebd96ec`  
		Last Modified: Wed, 01 Nov 2023 06:54:05 GMT  
		Size: 1.4 MB (1387212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba28223ab0fd0ba91b6c220a2f17cd52d8fec220e52b4a693c92712fed5aa474`  
		Last Modified: Wed, 01 Nov 2023 06:54:03 GMT  
		Size: 493.0 B  
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

## `adminer:4-standalone`

```console
$ docker pull adminer@sha256:b7f0e6681e9a77916daf2f070616d25e3fd687b84550aa6673de9a24407dd613
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
$ docker pull adminer@sha256:b96876e1c6d4eda21b2653d54bb8c9d4674fc177749254c5a44d097f92e2362e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.9 MB (95941196 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5cec1739340987c68ebd5535d5297dc62cc4fa489a253b4d84bb800b461e129`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Wed, 01 Nov 2023 02:53:39 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 01 Nov 2023 02:53:39 GMT
WORKDIR /var/www/html
# Wed, 01 Nov 2023 02:53:39 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 01 Nov 2023 02:53:39 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 01 Nov 2023 02:53:39 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 01 Nov 2023 02:53:39 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 01 Nov 2023 02:53:50 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 01 Nov 2023 02:53:50 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 01 Nov 2023 02:53:50 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 01 Nov 2023 02:53:50 GMT
USER adminer
# Wed, 01 Nov 2023 02:53:50 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 01 Nov 2023 02:53:50 GMT
EXPOSE 8080
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
	-	`sha256:bf435083814d20c35b08cac2c04f42a971fe8c772a6ff6ab5ea2dbb4c5365923`  
		Last Modified: Wed, 01 Nov 2023 02:54:24 GMT  
		Size: 1.9 KB (1876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:298e667e63eeffb2a143be3c3aeed4888c95d316e453939646663ae94cb39b38`  
		Last Modified: Wed, 01 Nov 2023 02:54:25 GMT  
		Size: 1.5 KB (1482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:009b4e930c2c0c866efcbe990a45b4aaa86c6ae9428410afb5842ed5a4a61a2f`  
		Last Modified: Wed, 01 Nov 2023 02:54:25 GMT  
		Size: 1.4 MB (1386349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:795fdddea697817d7c6a47b855376bc15a2ece944ad41fb076688cf55c7a749a`  
		Last Modified: Wed, 01 Nov 2023 02:54:24 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-standalone` - linux; arm variant v5

```console
$ docker pull adminer@sha256:37f77f5ee6832c7e087446aedd7fbc4759897435702305e7331410f4ccf749a9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.2 MB (91203583 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4428e260c8ac1e52db7ab4bca8db1cc7baafd67bb17a2206f99ccb97cb9c167`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 01 Nov 2023 00:48:39 GMT
ADD file:6fcdedd346da0744f7f45d0e7df77336a37ce87345bd414bd4e198804980781e in / 
# Wed, 01 Nov 2023 00:48:40 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 06:41:07 GMT
STOPSIGNAL SIGINT
# Wed, 01 Nov 2023 06:41:38 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 06:41:39 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 01 Nov 2023 06:41:40 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 01 Nov 2023 06:41:40 GMT
WORKDIR /var/www/html
# Wed, 01 Nov 2023 06:41:40 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 01 Nov 2023 06:41:40 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 01 Nov 2023 06:41:40 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 01 Nov 2023 06:41:40 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 01 Nov 2023 06:41:55 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 01 Nov 2023 06:41:55 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 01 Nov 2023 06:41:55 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 01 Nov 2023 06:41:56 GMT
USER adminer
# Wed, 01 Nov 2023 06:41:56 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 01 Nov 2023 06:41:56 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:e0adb3cac2906548cd3544bf3c384be3e3bdca9d41c37e11c160813af74301b9`  
		Last Modified: Wed, 01 Nov 2023 00:51:49 GMT  
		Size: 52.6 MB (52563334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e3623d9fb2289bbcd9a4586d409f13e8c27695bdb11f4c43599571aa1229528`  
		Last Modified: Wed, 01 Nov 2023 06:42:42 GMT  
		Size: 37.2 MB (37249740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28eac10d8db23ee6ea32d6b0c826db4a2dcbcd194ce18e99629fef2b283b4168`  
		Last Modified: Wed, 01 Nov 2023 06:42:33 GMT  
		Size: 389.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5779125ab319b67fbc7cf3bcaa969968771e9e472e58c08976728bb8d7569d56`  
		Last Modified: Wed, 01 Nov 2023 06:42:33 GMT  
		Size: 1.9 KB (1869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1952b238fb472fe6155a5c880e5d83d4c58dee30db79ba608c878282838500e`  
		Last Modified: Wed, 01 Nov 2023 06:42:33 GMT  
		Size: 1.5 KB (1476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85025f444620cafd6192a2667af59fdf4aca316094a82a43909a7e9f96e254f9`  
		Last Modified: Wed, 01 Nov 2023 06:42:33 GMT  
		Size: 1.4 MB (1386285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56f0c59e7ad269f06b6107635f33308fe74056eebdde42c8932886bf95c1885b`  
		Last Modified: Wed, 01 Nov 2023 06:42:33 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-standalone` - linux; arm variant v7

```console
$ docker pull adminer@sha256:03812b425c6b805691941ae806db34dc0b8a3f161f3a4e11ea0c54eb783037fb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.8 MB (87794095 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c9e7020270d790860f62ddf4e490a5409714c8f1d910f0e5552e34467640d9d`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Wed, 01 Nov 2023 02:13:44 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 01 Nov 2023 02:13:44 GMT
WORKDIR /var/www/html
# Wed, 01 Nov 2023 02:13:44 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 01 Nov 2023 02:13:44 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 01 Nov 2023 02:13:44 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 01 Nov 2023 02:13:44 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 01 Nov 2023 02:14:02 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 01 Nov 2023 02:14:02 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 01 Nov 2023 02:14:02 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 01 Nov 2023 02:14:02 GMT
USER adminer
# Wed, 01 Nov 2023 02:14:02 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 01 Nov 2023 02:14:02 GMT
EXPOSE 8080
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
	-	`sha256:b5ff4543277751a4ec131370a18afcbdcefbb299cac4f8b46d83ca0bb7e2fbb5`  
		Last Modified: Wed, 01 Nov 2023 02:14:32 GMT  
		Size: 1.9 KB (1867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8035a3dd0d4bf0c16736f3dc9982fdf586cb8db7c9c17bdfc7b7857d8236a5f8`  
		Last Modified: Wed, 01 Nov 2023 02:14:32 GMT  
		Size: 1.5 KB (1482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3e860a8d0ed1174c57c59e038d17c8c011e9262aac708373f223685b8a474c3`  
		Last Modified: Wed, 01 Nov 2023 02:14:32 GMT  
		Size: 1.4 MB (1386280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46610df748fd7888da3ef3e1419131554e3c580380b72af8c2182bd4b0c868d3`  
		Last Modified: Wed, 01 Nov 2023 02:14:32 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-standalone` - linux; arm64 variant v8

```console
$ docker pull adminer@sha256:63e8c57d2e82e0d50f641f56ce18316ba1f8a12a4640c2b6966453d198a8f14f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.3 MB (94343887 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e729f030ea5398e5fb915c10c2a7b811bffbcfd0932c22b49cba6738c053e8b6`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Wed, 01 Nov 2023 02:01:40 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 01 Nov 2023 02:01:40 GMT
WORKDIR /var/www/html
# Wed, 01 Nov 2023 02:01:40 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 01 Nov 2023 02:01:40 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 01 Nov 2023 02:01:40 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 01 Nov 2023 02:01:40 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 01 Nov 2023 02:01:50 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 01 Nov 2023 02:01:50 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 01 Nov 2023 02:01:50 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 01 Nov 2023 02:01:51 GMT
USER adminer
# Wed, 01 Nov 2023 02:01:51 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 01 Nov 2023 02:01:51 GMT
EXPOSE 8080
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
	-	`sha256:96cc754b457a6496cd3a8ba90b44ea5d39534c43f26dc2cb557b71a76902a3d6`  
		Last Modified: Wed, 01 Nov 2023 02:02:15 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:535170e27a39ee08c1372464244541113d3a4d899c1c7676ebca43a9f09b2421`  
		Last Modified: Wed, 01 Nov 2023 02:02:15 GMT  
		Size: 1.5 KB (1482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83e4006979461007bc0f7c1b0bb3b0675f29b405562d0cc37f5cf5b0711a309e`  
		Last Modified: Wed, 01 Nov 2023 02:02:16 GMT  
		Size: 1.4 MB (1386269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aecfb4d8f96734c7035d67c5e3b751eb15f305ae0b1d2855921c5d1d0d83b5bc`  
		Last Modified: Wed, 01 Nov 2023 02:02:15 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-standalone` - linux; 386

```console
$ docker pull adminer@sha256:a21c1d6915687a26e34d9f2f09f9b5104e64bc71aa36e19afae9c5d8c67a9040
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.0 MB (96997500 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3517f7704a6b833432e5e5e0144c6ce4e15ba0199adde89fb66fba372920f37`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 01 Nov 2023 00:39:06 GMT
ADD file:4095d27bc1a281dda044919be3bb570d581df169c01f22b0963b38e0dd6d9eff in / 
# Wed, 01 Nov 2023 00:39:07 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 08:16:42 GMT
STOPSIGNAL SIGINT
# Wed, 01 Nov 2023 08:17:12 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 08:17:13 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 01 Nov 2023 08:17:14 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 01 Nov 2023 08:17:14 GMT
WORKDIR /var/www/html
# Wed, 01 Nov 2023 08:17:14 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 01 Nov 2023 08:17:14 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 01 Nov 2023 08:17:14 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 01 Nov 2023 08:17:14 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 01 Nov 2023 08:17:28 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 01 Nov 2023 08:17:28 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 01 Nov 2023 08:17:28 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 01 Nov 2023 08:17:28 GMT
USER adminer
# Wed, 01 Nov 2023 08:17:28 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 01 Nov 2023 08:17:28 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:95d6aa56ba74b8ed0a732c4676a2c45c84a18076696d466cd9bf0b459c600e02`  
		Last Modified: Wed, 01 Nov 2023 00:43:49 GMT  
		Size: 56.0 MB (56046261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80589068561f705cd353c87358a0cecc8311057c942f023093c00c5ae59b0da4`  
		Last Modified: Wed, 01 Nov 2023 08:18:18 GMT  
		Size: 39.6 MB (39560745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c2dcd79bac9186cbea2e89e7c6085867c2ec84a4322ad7e80642bbe4e78fc42`  
		Last Modified: Wed, 01 Nov 2023 08:18:07 GMT  
		Size: 389.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c684759995fea1dd384d011644236354c8d098a591ea7926cac740391deb251`  
		Last Modified: Wed, 01 Nov 2023 08:18:07 GMT  
		Size: 1.9 KB (1866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a604bb0980f5b877ea1cfe73a85385ed541f85c82b22348d27f8d97a04d1ef76`  
		Last Modified: Wed, 01 Nov 2023 08:18:07 GMT  
		Size: 1.5 KB (1476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e27ee00f7fee2ee221e39d45b4abcfd90c63753f5e7263e8f30c67520aebc624`  
		Last Modified: Wed, 01 Nov 2023 08:18:08 GMT  
		Size: 1.4 MB (1386271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efa1816dcac43959f858ffcdbab80217277171e01d1c9a8fe3ebdd1c15db6697`  
		Last Modified: Wed, 01 Nov 2023 08:18:07 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-standalone` - linux; mips64le

```console
$ docker pull adminer@sha256:ab1415fc7ebc72555fc80c9a4f64e05dae784d0acf5368241c39bf74ddf5bce4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.6 MB (92632325 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7faddbe6a665e6871431356947ac3c57cd3c6c20b85c84172da87b3f93017faa`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 01 Nov 2023 01:09:34 GMT
ADD file:2c9f9140e731974a497825454c08d67829f514a83742973e30454cc905ebac6c in / 
# Wed, 01 Nov 2023 01:09:39 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 06:47:42 GMT
STOPSIGNAL SIGINT
# Wed, 01 Nov 2023 06:49:39 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 06:49:45 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 01 Nov 2023 06:49:52 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 01 Nov 2023 06:49:55 GMT
WORKDIR /var/www/html
# Wed, 01 Nov 2023 06:49:58 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 01 Nov 2023 06:50:02 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 01 Nov 2023 06:50:05 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 01 Nov 2023 06:50:08 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 01 Nov 2023 06:51:01 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 01 Nov 2023 06:51:04 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 01 Nov 2023 06:51:07 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 01 Nov 2023 06:51:10 GMT
USER adminer
# Wed, 01 Nov 2023 06:51:14 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 01 Nov 2023 06:51:17 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:a10c6e715fcf314db953339b3e58b9e0167f6cd2d02bf633e20282058eb83331`  
		Last Modified: Wed, 01 Nov 2023 01:20:31 GMT  
		Size: 53.3 MB (53288991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3e05f3781dcb9702ce843ce679283bdea07c6614cdcba5a271127fd6bc7bb81`  
		Last Modified: Wed, 01 Nov 2023 06:53:43 GMT  
		Size: 38.0 MB (37952018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c67397db1f05d9d07b2053012f95d10c64b397e5f8578a8252c397958089cc7`  
		Last Modified: Wed, 01 Nov 2023 06:53:16 GMT  
		Size: 395.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12601b86b1fe6286ef174f4194db89610719071fc99b6004600546e313b75afc`  
		Last Modified: Wed, 01 Nov 2023 06:53:16 GMT  
		Size: 1.7 KB (1725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cf53f1325a00115717e22a2ad400917ea970c2863a9f0aa384c81111fe5f754`  
		Last Modified: Wed, 01 Nov 2023 06:53:16 GMT  
		Size: 1.5 KB (1481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fb917f0d920d8d2969e5b26d77d9384c94934f2c5d72677b658a9483e180240`  
		Last Modified: Wed, 01 Nov 2023 06:53:17 GMT  
		Size: 1.4 MB (1387222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af14639f108dd10f1d2bd5ea098b67c59009583ed8e393315c464ec4223e37d8`  
		Last Modified: Wed, 01 Nov 2023 06:53:16 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-standalone` - linux; ppc64le

```console
$ docker pull adminer@sha256:489934d719089bd1c3827bdf673dcf7636376fbcbcfe837c4b7fa275ba366b62
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.3 MB (101265232 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6176ac38dfe8ab4e16662cc637ab4fb4b6f98c2e489cf4b4e6a66d578229ac6a`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Wed, 01 Nov 2023 02:50:13 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 01 Nov 2023 02:50:15 GMT
WORKDIR /var/www/html
# Wed, 01 Nov 2023 02:50:15 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 01 Nov 2023 02:50:15 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 01 Nov 2023 02:50:16 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 01 Nov 2023 02:50:16 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 01 Nov 2023 02:50:41 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 01 Nov 2023 02:50:42 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 01 Nov 2023 02:50:42 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 01 Nov 2023 02:50:43 GMT
USER adminer
# Wed, 01 Nov 2023 02:50:43 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 01 Nov 2023 02:50:44 GMT
EXPOSE 8080
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
	-	`sha256:c949ba7225949db3835c8321c7fd3fc61042abadd084780530933f2490a389ac`  
		Last Modified: Wed, 01 Nov 2023 02:51:40 GMT  
		Size: 1.9 KB (1878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69b23613e6440faf4dd53e85cce3379a37d371a55de8c3711313d4e8c2bdfcc7`  
		Last Modified: Wed, 01 Nov 2023 02:51:41 GMT  
		Size: 1.5 KB (1480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7424b8a43895b887591228e0a253d09fc56191f47ab5b4ab56d6fac2e6cbd9af`  
		Last Modified: Wed, 01 Nov 2023 02:51:41 GMT  
		Size: 1.4 MB (1386466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ee20cb0c3714aa128b4be5cdf5911002f2596f04b95e7e03962e22f45920bd3`  
		Last Modified: Wed, 01 Nov 2023 02:51:40 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-standalone` - linux; s390x

```console
$ docker pull adminer@sha256:febeaf64eb35379728a191c91b4c0fd744f0f25716db5b3a6383382bd813875b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.7 MB (93708845 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f56dc24645f9175629077bc05d2d1ef72a10391d530b75320409f480c64d72b5`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Wed, 01 Nov 2023 01:50:10 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 01 Nov 2023 01:50:10 GMT
WORKDIR /var/www/html
# Wed, 01 Nov 2023 01:50:10 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 01 Nov 2023 01:50:10 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 01 Nov 2023 01:50:10 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 01 Nov 2023 01:50:10 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 01 Nov 2023 01:50:18 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 01 Nov 2023 01:50:18 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 01 Nov 2023 01:50:18 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 01 Nov 2023 01:50:18 GMT
USER adminer
# Wed, 01 Nov 2023 01:50:18 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 01 Nov 2023 01:50:19 GMT
EXPOSE 8080
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
	-	`sha256:0ddb015dd3525d29ecb468826e1900bd5a42aedf948d046cf67cbb849116174a`  
		Last Modified: Wed, 01 Nov 2023 01:50:54 GMT  
		Size: 1.9 KB (1879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eeda1242b7f2fccc214b7bce16debf257837f0e99de553d8b0899289fdf4381`  
		Last Modified: Wed, 01 Nov 2023 01:50:54 GMT  
		Size: 1.5 KB (1477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b79f82c6e4dc3c8fa378683a146466b55a41e4a9b35103811abe39ff47528f4`  
		Last Modified: Wed, 01 Nov 2023 01:50:55 GMT  
		Size: 1.4 MB (1386366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:245a8a7cccf20a91e5d673ee924ca9853c1d060c66fdb377e8b8ca63166ac4cc`  
		Last Modified: Wed, 01 Nov 2023 01:50:54 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `adminer:4.8.1`

```console
$ docker pull adminer@sha256:b7f0e6681e9a77916daf2f070616d25e3fd687b84550aa6673de9a24407dd613
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
$ docker pull adminer@sha256:b96876e1c6d4eda21b2653d54bb8c9d4674fc177749254c5a44d097f92e2362e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.9 MB (95941196 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5cec1739340987c68ebd5535d5297dc62cc4fa489a253b4d84bb800b461e129`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Wed, 01 Nov 2023 02:53:39 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 01 Nov 2023 02:53:39 GMT
WORKDIR /var/www/html
# Wed, 01 Nov 2023 02:53:39 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 01 Nov 2023 02:53:39 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 01 Nov 2023 02:53:39 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 01 Nov 2023 02:53:39 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 01 Nov 2023 02:53:50 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 01 Nov 2023 02:53:50 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 01 Nov 2023 02:53:50 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 01 Nov 2023 02:53:50 GMT
USER adminer
# Wed, 01 Nov 2023 02:53:50 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 01 Nov 2023 02:53:50 GMT
EXPOSE 8080
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
	-	`sha256:bf435083814d20c35b08cac2c04f42a971fe8c772a6ff6ab5ea2dbb4c5365923`  
		Last Modified: Wed, 01 Nov 2023 02:54:24 GMT  
		Size: 1.9 KB (1876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:298e667e63eeffb2a143be3c3aeed4888c95d316e453939646663ae94cb39b38`  
		Last Modified: Wed, 01 Nov 2023 02:54:25 GMT  
		Size: 1.5 KB (1482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:009b4e930c2c0c866efcbe990a45b4aaa86c6ae9428410afb5842ed5a4a61a2f`  
		Last Modified: Wed, 01 Nov 2023 02:54:25 GMT  
		Size: 1.4 MB (1386349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:795fdddea697817d7c6a47b855376bc15a2ece944ad41fb076688cf55c7a749a`  
		Last Modified: Wed, 01 Nov 2023 02:54:24 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1` - linux; arm variant v5

```console
$ docker pull adminer@sha256:37f77f5ee6832c7e087446aedd7fbc4759897435702305e7331410f4ccf749a9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.2 MB (91203583 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4428e260c8ac1e52db7ab4bca8db1cc7baafd67bb17a2206f99ccb97cb9c167`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 01 Nov 2023 00:48:39 GMT
ADD file:6fcdedd346da0744f7f45d0e7df77336a37ce87345bd414bd4e198804980781e in / 
# Wed, 01 Nov 2023 00:48:40 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 06:41:07 GMT
STOPSIGNAL SIGINT
# Wed, 01 Nov 2023 06:41:38 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 06:41:39 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 01 Nov 2023 06:41:40 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 01 Nov 2023 06:41:40 GMT
WORKDIR /var/www/html
# Wed, 01 Nov 2023 06:41:40 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 01 Nov 2023 06:41:40 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 01 Nov 2023 06:41:40 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 01 Nov 2023 06:41:40 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 01 Nov 2023 06:41:55 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 01 Nov 2023 06:41:55 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 01 Nov 2023 06:41:55 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 01 Nov 2023 06:41:56 GMT
USER adminer
# Wed, 01 Nov 2023 06:41:56 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 01 Nov 2023 06:41:56 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:e0adb3cac2906548cd3544bf3c384be3e3bdca9d41c37e11c160813af74301b9`  
		Last Modified: Wed, 01 Nov 2023 00:51:49 GMT  
		Size: 52.6 MB (52563334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e3623d9fb2289bbcd9a4586d409f13e8c27695bdb11f4c43599571aa1229528`  
		Last Modified: Wed, 01 Nov 2023 06:42:42 GMT  
		Size: 37.2 MB (37249740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28eac10d8db23ee6ea32d6b0c826db4a2dcbcd194ce18e99629fef2b283b4168`  
		Last Modified: Wed, 01 Nov 2023 06:42:33 GMT  
		Size: 389.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5779125ab319b67fbc7cf3bcaa969968771e9e472e58c08976728bb8d7569d56`  
		Last Modified: Wed, 01 Nov 2023 06:42:33 GMT  
		Size: 1.9 KB (1869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1952b238fb472fe6155a5c880e5d83d4c58dee30db79ba608c878282838500e`  
		Last Modified: Wed, 01 Nov 2023 06:42:33 GMT  
		Size: 1.5 KB (1476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85025f444620cafd6192a2667af59fdf4aca316094a82a43909a7e9f96e254f9`  
		Last Modified: Wed, 01 Nov 2023 06:42:33 GMT  
		Size: 1.4 MB (1386285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56f0c59e7ad269f06b6107635f33308fe74056eebdde42c8932886bf95c1885b`  
		Last Modified: Wed, 01 Nov 2023 06:42:33 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1` - linux; arm variant v7

```console
$ docker pull adminer@sha256:03812b425c6b805691941ae806db34dc0b8a3f161f3a4e11ea0c54eb783037fb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.8 MB (87794095 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c9e7020270d790860f62ddf4e490a5409714c8f1d910f0e5552e34467640d9d`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Wed, 01 Nov 2023 02:13:44 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 01 Nov 2023 02:13:44 GMT
WORKDIR /var/www/html
# Wed, 01 Nov 2023 02:13:44 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 01 Nov 2023 02:13:44 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 01 Nov 2023 02:13:44 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 01 Nov 2023 02:13:44 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 01 Nov 2023 02:14:02 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 01 Nov 2023 02:14:02 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 01 Nov 2023 02:14:02 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 01 Nov 2023 02:14:02 GMT
USER adminer
# Wed, 01 Nov 2023 02:14:02 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 01 Nov 2023 02:14:02 GMT
EXPOSE 8080
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
	-	`sha256:b5ff4543277751a4ec131370a18afcbdcefbb299cac4f8b46d83ca0bb7e2fbb5`  
		Last Modified: Wed, 01 Nov 2023 02:14:32 GMT  
		Size: 1.9 KB (1867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8035a3dd0d4bf0c16736f3dc9982fdf586cb8db7c9c17bdfc7b7857d8236a5f8`  
		Last Modified: Wed, 01 Nov 2023 02:14:32 GMT  
		Size: 1.5 KB (1482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3e860a8d0ed1174c57c59e038d17c8c011e9262aac708373f223685b8a474c3`  
		Last Modified: Wed, 01 Nov 2023 02:14:32 GMT  
		Size: 1.4 MB (1386280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46610df748fd7888da3ef3e1419131554e3c580380b72af8c2182bd4b0c868d3`  
		Last Modified: Wed, 01 Nov 2023 02:14:32 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1` - linux; arm64 variant v8

```console
$ docker pull adminer@sha256:63e8c57d2e82e0d50f641f56ce18316ba1f8a12a4640c2b6966453d198a8f14f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.3 MB (94343887 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e729f030ea5398e5fb915c10c2a7b811bffbcfd0932c22b49cba6738c053e8b6`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Wed, 01 Nov 2023 02:01:40 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 01 Nov 2023 02:01:40 GMT
WORKDIR /var/www/html
# Wed, 01 Nov 2023 02:01:40 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 01 Nov 2023 02:01:40 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 01 Nov 2023 02:01:40 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 01 Nov 2023 02:01:40 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 01 Nov 2023 02:01:50 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 01 Nov 2023 02:01:50 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 01 Nov 2023 02:01:50 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 01 Nov 2023 02:01:51 GMT
USER adminer
# Wed, 01 Nov 2023 02:01:51 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 01 Nov 2023 02:01:51 GMT
EXPOSE 8080
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
	-	`sha256:96cc754b457a6496cd3a8ba90b44ea5d39534c43f26dc2cb557b71a76902a3d6`  
		Last Modified: Wed, 01 Nov 2023 02:02:15 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:535170e27a39ee08c1372464244541113d3a4d899c1c7676ebca43a9f09b2421`  
		Last Modified: Wed, 01 Nov 2023 02:02:15 GMT  
		Size: 1.5 KB (1482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83e4006979461007bc0f7c1b0bb3b0675f29b405562d0cc37f5cf5b0711a309e`  
		Last Modified: Wed, 01 Nov 2023 02:02:16 GMT  
		Size: 1.4 MB (1386269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aecfb4d8f96734c7035d67c5e3b751eb15f305ae0b1d2855921c5d1d0d83b5bc`  
		Last Modified: Wed, 01 Nov 2023 02:02:15 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1` - linux; 386

```console
$ docker pull adminer@sha256:a21c1d6915687a26e34d9f2f09f9b5104e64bc71aa36e19afae9c5d8c67a9040
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.0 MB (96997500 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3517f7704a6b833432e5e5e0144c6ce4e15ba0199adde89fb66fba372920f37`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 01 Nov 2023 00:39:06 GMT
ADD file:4095d27bc1a281dda044919be3bb570d581df169c01f22b0963b38e0dd6d9eff in / 
# Wed, 01 Nov 2023 00:39:07 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 08:16:42 GMT
STOPSIGNAL SIGINT
# Wed, 01 Nov 2023 08:17:12 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 08:17:13 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 01 Nov 2023 08:17:14 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 01 Nov 2023 08:17:14 GMT
WORKDIR /var/www/html
# Wed, 01 Nov 2023 08:17:14 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 01 Nov 2023 08:17:14 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 01 Nov 2023 08:17:14 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 01 Nov 2023 08:17:14 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 01 Nov 2023 08:17:28 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 01 Nov 2023 08:17:28 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 01 Nov 2023 08:17:28 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 01 Nov 2023 08:17:28 GMT
USER adminer
# Wed, 01 Nov 2023 08:17:28 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 01 Nov 2023 08:17:28 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:95d6aa56ba74b8ed0a732c4676a2c45c84a18076696d466cd9bf0b459c600e02`  
		Last Modified: Wed, 01 Nov 2023 00:43:49 GMT  
		Size: 56.0 MB (56046261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80589068561f705cd353c87358a0cecc8311057c942f023093c00c5ae59b0da4`  
		Last Modified: Wed, 01 Nov 2023 08:18:18 GMT  
		Size: 39.6 MB (39560745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c2dcd79bac9186cbea2e89e7c6085867c2ec84a4322ad7e80642bbe4e78fc42`  
		Last Modified: Wed, 01 Nov 2023 08:18:07 GMT  
		Size: 389.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c684759995fea1dd384d011644236354c8d098a591ea7926cac740391deb251`  
		Last Modified: Wed, 01 Nov 2023 08:18:07 GMT  
		Size: 1.9 KB (1866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a604bb0980f5b877ea1cfe73a85385ed541f85c82b22348d27f8d97a04d1ef76`  
		Last Modified: Wed, 01 Nov 2023 08:18:07 GMT  
		Size: 1.5 KB (1476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e27ee00f7fee2ee221e39d45b4abcfd90c63753f5e7263e8f30c67520aebc624`  
		Last Modified: Wed, 01 Nov 2023 08:18:08 GMT  
		Size: 1.4 MB (1386271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efa1816dcac43959f858ffcdbab80217277171e01d1c9a8fe3ebdd1c15db6697`  
		Last Modified: Wed, 01 Nov 2023 08:18:07 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1` - linux; mips64le

```console
$ docker pull adminer@sha256:ab1415fc7ebc72555fc80c9a4f64e05dae784d0acf5368241c39bf74ddf5bce4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.6 MB (92632325 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7faddbe6a665e6871431356947ac3c57cd3c6c20b85c84172da87b3f93017faa`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 01 Nov 2023 01:09:34 GMT
ADD file:2c9f9140e731974a497825454c08d67829f514a83742973e30454cc905ebac6c in / 
# Wed, 01 Nov 2023 01:09:39 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 06:47:42 GMT
STOPSIGNAL SIGINT
# Wed, 01 Nov 2023 06:49:39 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 06:49:45 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 01 Nov 2023 06:49:52 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 01 Nov 2023 06:49:55 GMT
WORKDIR /var/www/html
# Wed, 01 Nov 2023 06:49:58 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 01 Nov 2023 06:50:02 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 01 Nov 2023 06:50:05 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 01 Nov 2023 06:50:08 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 01 Nov 2023 06:51:01 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 01 Nov 2023 06:51:04 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 01 Nov 2023 06:51:07 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 01 Nov 2023 06:51:10 GMT
USER adminer
# Wed, 01 Nov 2023 06:51:14 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 01 Nov 2023 06:51:17 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:a10c6e715fcf314db953339b3e58b9e0167f6cd2d02bf633e20282058eb83331`  
		Last Modified: Wed, 01 Nov 2023 01:20:31 GMT  
		Size: 53.3 MB (53288991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3e05f3781dcb9702ce843ce679283bdea07c6614cdcba5a271127fd6bc7bb81`  
		Last Modified: Wed, 01 Nov 2023 06:53:43 GMT  
		Size: 38.0 MB (37952018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c67397db1f05d9d07b2053012f95d10c64b397e5f8578a8252c397958089cc7`  
		Last Modified: Wed, 01 Nov 2023 06:53:16 GMT  
		Size: 395.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12601b86b1fe6286ef174f4194db89610719071fc99b6004600546e313b75afc`  
		Last Modified: Wed, 01 Nov 2023 06:53:16 GMT  
		Size: 1.7 KB (1725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cf53f1325a00115717e22a2ad400917ea970c2863a9f0aa384c81111fe5f754`  
		Last Modified: Wed, 01 Nov 2023 06:53:16 GMT  
		Size: 1.5 KB (1481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fb917f0d920d8d2969e5b26d77d9384c94934f2c5d72677b658a9483e180240`  
		Last Modified: Wed, 01 Nov 2023 06:53:17 GMT  
		Size: 1.4 MB (1387222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af14639f108dd10f1d2bd5ea098b67c59009583ed8e393315c464ec4223e37d8`  
		Last Modified: Wed, 01 Nov 2023 06:53:16 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1` - linux; ppc64le

```console
$ docker pull adminer@sha256:489934d719089bd1c3827bdf673dcf7636376fbcbcfe837c4b7fa275ba366b62
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.3 MB (101265232 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6176ac38dfe8ab4e16662cc637ab4fb4b6f98c2e489cf4b4e6a66d578229ac6a`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Wed, 01 Nov 2023 02:50:13 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 01 Nov 2023 02:50:15 GMT
WORKDIR /var/www/html
# Wed, 01 Nov 2023 02:50:15 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 01 Nov 2023 02:50:15 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 01 Nov 2023 02:50:16 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 01 Nov 2023 02:50:16 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 01 Nov 2023 02:50:41 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 01 Nov 2023 02:50:42 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 01 Nov 2023 02:50:42 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 01 Nov 2023 02:50:43 GMT
USER adminer
# Wed, 01 Nov 2023 02:50:43 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 01 Nov 2023 02:50:44 GMT
EXPOSE 8080
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
	-	`sha256:c949ba7225949db3835c8321c7fd3fc61042abadd084780530933f2490a389ac`  
		Last Modified: Wed, 01 Nov 2023 02:51:40 GMT  
		Size: 1.9 KB (1878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69b23613e6440faf4dd53e85cce3379a37d371a55de8c3711313d4e8c2bdfcc7`  
		Last Modified: Wed, 01 Nov 2023 02:51:41 GMT  
		Size: 1.5 KB (1480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7424b8a43895b887591228e0a253d09fc56191f47ab5b4ab56d6fac2e6cbd9af`  
		Last Modified: Wed, 01 Nov 2023 02:51:41 GMT  
		Size: 1.4 MB (1386466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ee20cb0c3714aa128b4be5cdf5911002f2596f04b95e7e03962e22f45920bd3`  
		Last Modified: Wed, 01 Nov 2023 02:51:40 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1` - linux; s390x

```console
$ docker pull adminer@sha256:febeaf64eb35379728a191c91b4c0fd744f0f25716db5b3a6383382bd813875b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.7 MB (93708845 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f56dc24645f9175629077bc05d2d1ef72a10391d530b75320409f480c64d72b5`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Wed, 01 Nov 2023 01:50:10 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 01 Nov 2023 01:50:10 GMT
WORKDIR /var/www/html
# Wed, 01 Nov 2023 01:50:10 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 01 Nov 2023 01:50:10 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 01 Nov 2023 01:50:10 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 01 Nov 2023 01:50:10 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 01 Nov 2023 01:50:18 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 01 Nov 2023 01:50:18 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 01 Nov 2023 01:50:18 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 01 Nov 2023 01:50:18 GMT
USER adminer
# Wed, 01 Nov 2023 01:50:18 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 01 Nov 2023 01:50:19 GMT
EXPOSE 8080
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
	-	`sha256:0ddb015dd3525d29ecb468826e1900bd5a42aedf948d046cf67cbb849116174a`  
		Last Modified: Wed, 01 Nov 2023 01:50:54 GMT  
		Size: 1.9 KB (1879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eeda1242b7f2fccc214b7bce16debf257837f0e99de553d8b0899289fdf4381`  
		Last Modified: Wed, 01 Nov 2023 01:50:54 GMT  
		Size: 1.5 KB (1477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b79f82c6e4dc3c8fa378683a146466b55a41e4a9b35103811abe39ff47528f4`  
		Last Modified: Wed, 01 Nov 2023 01:50:55 GMT  
		Size: 1.4 MB (1386366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:245a8a7cccf20a91e5d673ee924ca9853c1d060c66fdb377e8b8ca63166ac4cc`  
		Last Modified: Wed, 01 Nov 2023 01:50:54 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `adminer:4.8.1-fastcgi`

```console
$ docker pull adminer@sha256:312c0213bc482710a1129efafd0e8a9df7c8f74203cfc2effce3bd1273d8483c
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

### `adminer:4.8.1-fastcgi` - linux; arm variant v5

```console
$ docker pull adminer@sha256:640e60b56e718fd2129bc9dcf1cb60e4ae5be47614831844f3ae58081ef992a3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.2 MB (91206303 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:148a1a15fd20132f8babeb810dd6b79f0ad5b9affc91c2f8541b13ff8460c027`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Wed, 01 Nov 2023 00:48:39 GMT
ADD file:6fcdedd346da0744f7f45d0e7df77336a37ce87345bd414bd4e198804980781e in / 
# Wed, 01 Nov 2023 00:48:40 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 06:41:07 GMT
STOPSIGNAL SIGINT
# Wed, 01 Nov 2023 06:41:38 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 06:41:39 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 01 Nov 2023 06:42:05 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Wed, 01 Nov 2023 06:42:06 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 01 Nov 2023 06:42:06 GMT
WORKDIR /var/www/html
# Wed, 01 Nov 2023 06:42:06 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 01 Nov 2023 06:42:06 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 01 Nov 2023 06:42:06 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 01 Nov 2023 06:42:07 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 01 Nov 2023 06:42:20 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 01 Nov 2023 06:42:20 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 01 Nov 2023 06:42:21 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 01 Nov 2023 06:42:21 GMT
USER adminer
# Wed, 01 Nov 2023 06:42:21 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:e0adb3cac2906548cd3544bf3c384be3e3bdca9d41c37e11c160813af74301b9`  
		Last Modified: Wed, 01 Nov 2023 00:51:49 GMT  
		Size: 52.6 MB (52563334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e3623d9fb2289bbcd9a4586d409f13e8c27695bdb11f4c43599571aa1229528`  
		Last Modified: Wed, 01 Nov 2023 06:42:42 GMT  
		Size: 37.2 MB (37249740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28eac10d8db23ee6ea32d6b0c826db4a2dcbcd194ce18e99629fef2b283b4168`  
		Last Modified: Wed, 01 Nov 2023 06:42:33 GMT  
		Size: 389.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2319565cc3ff6648a187190305386506317c8e8b916e4c68a2fc7c4901bfade4`  
		Last Modified: Wed, 01 Nov 2023 06:42:59 GMT  
		Size: 2.7 KB (2712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d82fa5f5f057baa718cb408944b78d134414e710547b7fefe9e313b157794f83`  
		Last Modified: Wed, 01 Nov 2023 06:42:59 GMT  
		Size: 1.9 KB (1867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26294c9823754b7b6c80e1e42807e3d303d36ebf56f05c24f0267cb9f42f1a5c`  
		Last Modified: Wed, 01 Nov 2023 06:42:58 GMT  
		Size: 1.5 KB (1476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1805ed31823bd60aec3a510dc6813b3e6df00428670492f806313f056d98accc`  
		Last Modified: Wed, 01 Nov 2023 06:42:59 GMT  
		Size: 1.4 MB (1386295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3379baf5fcc5e2ee2f374067c687e3614bb3a564ce83ec47aa3088df5900c339`  
		Last Modified: Wed, 01 Nov 2023 06:42:59 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1-fastcgi` - linux; arm variant v7

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

### `adminer:4.8.1-fastcgi` - linux; arm64 variant v8

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

### `adminer:4.8.1-fastcgi` - linux; 386

```console
$ docker pull adminer@sha256:baf03604dff500f1ff723513a538bd2632e854534952802ef3c2757ab9ec7284
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.0 MB (97000221 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a29b774050e6bb60654c4629b38274b8039fbff780360aa51ab5c918374888e`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Wed, 01 Nov 2023 00:39:06 GMT
ADD file:4095d27bc1a281dda044919be3bb570d581df169c01f22b0963b38e0dd6d9eff in / 
# Wed, 01 Nov 2023 00:39:07 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 08:16:42 GMT
STOPSIGNAL SIGINT
# Wed, 01 Nov 2023 08:17:12 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 08:17:13 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 01 Nov 2023 08:17:40 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Wed, 01 Nov 2023 08:17:41 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 01 Nov 2023 08:17:41 GMT
WORKDIR /var/www/html
# Wed, 01 Nov 2023 08:17:41 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 01 Nov 2023 08:17:41 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 01 Nov 2023 08:17:41 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 01 Nov 2023 08:17:41 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 01 Nov 2023 08:17:54 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 01 Nov 2023 08:17:55 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 01 Nov 2023 08:17:55 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 01 Nov 2023 08:17:55 GMT
USER adminer
# Wed, 01 Nov 2023 08:17:55 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:95d6aa56ba74b8ed0a732c4676a2c45c84a18076696d466cd9bf0b459c600e02`  
		Last Modified: Wed, 01 Nov 2023 00:43:49 GMT  
		Size: 56.0 MB (56046261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80589068561f705cd353c87358a0cecc8311057c942f023093c00c5ae59b0da4`  
		Last Modified: Wed, 01 Nov 2023 08:18:18 GMT  
		Size: 39.6 MB (39560745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c2dcd79bac9186cbea2e89e7c6085867c2ec84a4322ad7e80642bbe4e78fc42`  
		Last Modified: Wed, 01 Nov 2023 08:18:07 GMT  
		Size: 389.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce8777aa37435cb70275cafb5973d4c38ade71490ab02d4690e7243d7f42fa99`  
		Last Modified: Wed, 01 Nov 2023 08:18:38 GMT  
		Size: 2.7 KB (2708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3092383d86bf2247454565915d60711072083b945827d3a71d04b2e8e7d5a24`  
		Last Modified: Wed, 01 Nov 2023 08:18:38 GMT  
		Size: 1.9 KB (1866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58ab83e0c0b5af9550f8219863a015b9f64aac19bfd190214266dddcdae1987d`  
		Last Modified: Wed, 01 Nov 2023 08:18:38 GMT  
		Size: 1.5 KB (1479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1ad071ea7480f652575c1ff65ee4ef869a9eb9b6f053ca5f2dae11776838485`  
		Last Modified: Wed, 01 Nov 2023 08:18:38 GMT  
		Size: 1.4 MB (1386283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31f82fe0941deccb9e97f691bccd364714153f8af834bfb61010a0edeed7d95b`  
		Last Modified: Wed, 01 Nov 2023 08:18:38 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1-fastcgi` - linux; mips64le

```console
$ docker pull adminer@sha256:d5005a80e57907d2bf1e882cd453c47a7c6e2044997f7f5f2d6c1737a73c8e53
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.6 MB (92635040 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46fee5e1b1c3fefa23d38e502f9c95f79c82daaf2e4a9015a2f079af2d582ea5`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Wed, 01 Nov 2023 01:09:34 GMT
ADD file:2c9f9140e731974a497825454c08d67829f514a83742973e30454cc905ebac6c in / 
# Wed, 01 Nov 2023 01:09:39 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 06:47:42 GMT
STOPSIGNAL SIGINT
# Wed, 01 Nov 2023 06:49:39 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 06:49:45 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 01 Nov 2023 06:51:29 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Wed, 01 Nov 2023 06:51:36 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 01 Nov 2023 06:51:39 GMT
WORKDIR /var/www/html
# Wed, 01 Nov 2023 06:51:42 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 01 Nov 2023 06:51:46 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 01 Nov 2023 06:51:49 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 01 Nov 2023 06:51:52 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 01 Nov 2023 06:52:43 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 01 Nov 2023 06:52:46 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 01 Nov 2023 06:52:50 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 01 Nov 2023 06:52:53 GMT
USER adminer
# Wed, 01 Nov 2023 06:52:56 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:a10c6e715fcf314db953339b3e58b9e0167f6cd2d02bf633e20282058eb83331`  
		Last Modified: Wed, 01 Nov 2023 01:20:31 GMT  
		Size: 53.3 MB (53288991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3e05f3781dcb9702ce843ce679283bdea07c6614cdcba5a271127fd6bc7bb81`  
		Last Modified: Wed, 01 Nov 2023 06:53:43 GMT  
		Size: 38.0 MB (37952018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c67397db1f05d9d07b2053012f95d10c64b397e5f8578a8252c397958089cc7`  
		Last Modified: Wed, 01 Nov 2023 06:53:16 GMT  
		Size: 395.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1efe29ad2e6399b06c40a1f74ef708babaf49feb6d4a81ffc433dbe62507869a`  
		Last Modified: Wed, 01 Nov 2023 06:54:03 GMT  
		Size: 2.7 KB (2714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5e18030af38a29600f3748bcbad3e59b6ec984e1949a992135f469b7a511bb4`  
		Last Modified: Wed, 01 Nov 2023 06:54:03 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a32ef85d04c2f926ef96c9ffa9dcac7659bc192103442cb5a3c6496c49d1f32`  
		Last Modified: Wed, 01 Nov 2023 06:54:03 GMT  
		Size: 1.5 KB (1482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce599942d3ca2661bbeab5bf9752328464303caf6cfbfa70875693cadebd96ec`  
		Last Modified: Wed, 01 Nov 2023 06:54:05 GMT  
		Size: 1.4 MB (1387212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba28223ab0fd0ba91b6c220a2f17cd52d8fec220e52b4a693c92712fed5aa474`  
		Last Modified: Wed, 01 Nov 2023 06:54:03 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1-fastcgi` - linux; ppc64le

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

### `adminer:4.8.1-fastcgi` - linux; s390x

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

## `adminer:4.8.1-standalone`

```console
$ docker pull adminer@sha256:b7f0e6681e9a77916daf2f070616d25e3fd687b84550aa6673de9a24407dd613
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
$ docker pull adminer@sha256:b96876e1c6d4eda21b2653d54bb8c9d4674fc177749254c5a44d097f92e2362e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.9 MB (95941196 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5cec1739340987c68ebd5535d5297dc62cc4fa489a253b4d84bb800b461e129`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Wed, 01 Nov 2023 02:53:39 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 01 Nov 2023 02:53:39 GMT
WORKDIR /var/www/html
# Wed, 01 Nov 2023 02:53:39 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 01 Nov 2023 02:53:39 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 01 Nov 2023 02:53:39 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 01 Nov 2023 02:53:39 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 01 Nov 2023 02:53:50 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 01 Nov 2023 02:53:50 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 01 Nov 2023 02:53:50 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 01 Nov 2023 02:53:50 GMT
USER adminer
# Wed, 01 Nov 2023 02:53:50 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 01 Nov 2023 02:53:50 GMT
EXPOSE 8080
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
	-	`sha256:bf435083814d20c35b08cac2c04f42a971fe8c772a6ff6ab5ea2dbb4c5365923`  
		Last Modified: Wed, 01 Nov 2023 02:54:24 GMT  
		Size: 1.9 KB (1876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:298e667e63eeffb2a143be3c3aeed4888c95d316e453939646663ae94cb39b38`  
		Last Modified: Wed, 01 Nov 2023 02:54:25 GMT  
		Size: 1.5 KB (1482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:009b4e930c2c0c866efcbe990a45b4aaa86c6ae9428410afb5842ed5a4a61a2f`  
		Last Modified: Wed, 01 Nov 2023 02:54:25 GMT  
		Size: 1.4 MB (1386349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:795fdddea697817d7c6a47b855376bc15a2ece944ad41fb076688cf55c7a749a`  
		Last Modified: Wed, 01 Nov 2023 02:54:24 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1-standalone` - linux; arm variant v5

```console
$ docker pull adminer@sha256:37f77f5ee6832c7e087446aedd7fbc4759897435702305e7331410f4ccf749a9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.2 MB (91203583 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4428e260c8ac1e52db7ab4bca8db1cc7baafd67bb17a2206f99ccb97cb9c167`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 01 Nov 2023 00:48:39 GMT
ADD file:6fcdedd346da0744f7f45d0e7df77336a37ce87345bd414bd4e198804980781e in / 
# Wed, 01 Nov 2023 00:48:40 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 06:41:07 GMT
STOPSIGNAL SIGINT
# Wed, 01 Nov 2023 06:41:38 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 06:41:39 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 01 Nov 2023 06:41:40 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 01 Nov 2023 06:41:40 GMT
WORKDIR /var/www/html
# Wed, 01 Nov 2023 06:41:40 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 01 Nov 2023 06:41:40 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 01 Nov 2023 06:41:40 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 01 Nov 2023 06:41:40 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 01 Nov 2023 06:41:55 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 01 Nov 2023 06:41:55 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 01 Nov 2023 06:41:55 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 01 Nov 2023 06:41:56 GMT
USER adminer
# Wed, 01 Nov 2023 06:41:56 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 01 Nov 2023 06:41:56 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:e0adb3cac2906548cd3544bf3c384be3e3bdca9d41c37e11c160813af74301b9`  
		Last Modified: Wed, 01 Nov 2023 00:51:49 GMT  
		Size: 52.6 MB (52563334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e3623d9fb2289bbcd9a4586d409f13e8c27695bdb11f4c43599571aa1229528`  
		Last Modified: Wed, 01 Nov 2023 06:42:42 GMT  
		Size: 37.2 MB (37249740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28eac10d8db23ee6ea32d6b0c826db4a2dcbcd194ce18e99629fef2b283b4168`  
		Last Modified: Wed, 01 Nov 2023 06:42:33 GMT  
		Size: 389.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5779125ab319b67fbc7cf3bcaa969968771e9e472e58c08976728bb8d7569d56`  
		Last Modified: Wed, 01 Nov 2023 06:42:33 GMT  
		Size: 1.9 KB (1869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1952b238fb472fe6155a5c880e5d83d4c58dee30db79ba608c878282838500e`  
		Last Modified: Wed, 01 Nov 2023 06:42:33 GMT  
		Size: 1.5 KB (1476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85025f444620cafd6192a2667af59fdf4aca316094a82a43909a7e9f96e254f9`  
		Last Modified: Wed, 01 Nov 2023 06:42:33 GMT  
		Size: 1.4 MB (1386285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56f0c59e7ad269f06b6107635f33308fe74056eebdde42c8932886bf95c1885b`  
		Last Modified: Wed, 01 Nov 2023 06:42:33 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1-standalone` - linux; arm variant v7

```console
$ docker pull adminer@sha256:03812b425c6b805691941ae806db34dc0b8a3f161f3a4e11ea0c54eb783037fb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.8 MB (87794095 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c9e7020270d790860f62ddf4e490a5409714c8f1d910f0e5552e34467640d9d`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Wed, 01 Nov 2023 02:13:44 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 01 Nov 2023 02:13:44 GMT
WORKDIR /var/www/html
# Wed, 01 Nov 2023 02:13:44 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 01 Nov 2023 02:13:44 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 01 Nov 2023 02:13:44 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 01 Nov 2023 02:13:44 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 01 Nov 2023 02:14:02 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 01 Nov 2023 02:14:02 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 01 Nov 2023 02:14:02 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 01 Nov 2023 02:14:02 GMT
USER adminer
# Wed, 01 Nov 2023 02:14:02 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 01 Nov 2023 02:14:02 GMT
EXPOSE 8080
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
	-	`sha256:b5ff4543277751a4ec131370a18afcbdcefbb299cac4f8b46d83ca0bb7e2fbb5`  
		Last Modified: Wed, 01 Nov 2023 02:14:32 GMT  
		Size: 1.9 KB (1867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8035a3dd0d4bf0c16736f3dc9982fdf586cb8db7c9c17bdfc7b7857d8236a5f8`  
		Last Modified: Wed, 01 Nov 2023 02:14:32 GMT  
		Size: 1.5 KB (1482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3e860a8d0ed1174c57c59e038d17c8c011e9262aac708373f223685b8a474c3`  
		Last Modified: Wed, 01 Nov 2023 02:14:32 GMT  
		Size: 1.4 MB (1386280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46610df748fd7888da3ef3e1419131554e3c580380b72af8c2182bd4b0c868d3`  
		Last Modified: Wed, 01 Nov 2023 02:14:32 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1-standalone` - linux; arm64 variant v8

```console
$ docker pull adminer@sha256:63e8c57d2e82e0d50f641f56ce18316ba1f8a12a4640c2b6966453d198a8f14f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.3 MB (94343887 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e729f030ea5398e5fb915c10c2a7b811bffbcfd0932c22b49cba6738c053e8b6`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Wed, 01 Nov 2023 02:01:40 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 01 Nov 2023 02:01:40 GMT
WORKDIR /var/www/html
# Wed, 01 Nov 2023 02:01:40 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 01 Nov 2023 02:01:40 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 01 Nov 2023 02:01:40 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 01 Nov 2023 02:01:40 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 01 Nov 2023 02:01:50 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 01 Nov 2023 02:01:50 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 01 Nov 2023 02:01:50 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 01 Nov 2023 02:01:51 GMT
USER adminer
# Wed, 01 Nov 2023 02:01:51 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 01 Nov 2023 02:01:51 GMT
EXPOSE 8080
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
	-	`sha256:96cc754b457a6496cd3a8ba90b44ea5d39534c43f26dc2cb557b71a76902a3d6`  
		Last Modified: Wed, 01 Nov 2023 02:02:15 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:535170e27a39ee08c1372464244541113d3a4d899c1c7676ebca43a9f09b2421`  
		Last Modified: Wed, 01 Nov 2023 02:02:15 GMT  
		Size: 1.5 KB (1482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83e4006979461007bc0f7c1b0bb3b0675f29b405562d0cc37f5cf5b0711a309e`  
		Last Modified: Wed, 01 Nov 2023 02:02:16 GMT  
		Size: 1.4 MB (1386269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aecfb4d8f96734c7035d67c5e3b751eb15f305ae0b1d2855921c5d1d0d83b5bc`  
		Last Modified: Wed, 01 Nov 2023 02:02:15 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1-standalone` - linux; 386

```console
$ docker pull adminer@sha256:a21c1d6915687a26e34d9f2f09f9b5104e64bc71aa36e19afae9c5d8c67a9040
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.0 MB (96997500 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3517f7704a6b833432e5e5e0144c6ce4e15ba0199adde89fb66fba372920f37`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 01 Nov 2023 00:39:06 GMT
ADD file:4095d27bc1a281dda044919be3bb570d581df169c01f22b0963b38e0dd6d9eff in / 
# Wed, 01 Nov 2023 00:39:07 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 08:16:42 GMT
STOPSIGNAL SIGINT
# Wed, 01 Nov 2023 08:17:12 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 08:17:13 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 01 Nov 2023 08:17:14 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 01 Nov 2023 08:17:14 GMT
WORKDIR /var/www/html
# Wed, 01 Nov 2023 08:17:14 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 01 Nov 2023 08:17:14 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 01 Nov 2023 08:17:14 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 01 Nov 2023 08:17:14 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 01 Nov 2023 08:17:28 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 01 Nov 2023 08:17:28 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 01 Nov 2023 08:17:28 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 01 Nov 2023 08:17:28 GMT
USER adminer
# Wed, 01 Nov 2023 08:17:28 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 01 Nov 2023 08:17:28 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:95d6aa56ba74b8ed0a732c4676a2c45c84a18076696d466cd9bf0b459c600e02`  
		Last Modified: Wed, 01 Nov 2023 00:43:49 GMT  
		Size: 56.0 MB (56046261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80589068561f705cd353c87358a0cecc8311057c942f023093c00c5ae59b0da4`  
		Last Modified: Wed, 01 Nov 2023 08:18:18 GMT  
		Size: 39.6 MB (39560745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c2dcd79bac9186cbea2e89e7c6085867c2ec84a4322ad7e80642bbe4e78fc42`  
		Last Modified: Wed, 01 Nov 2023 08:18:07 GMT  
		Size: 389.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c684759995fea1dd384d011644236354c8d098a591ea7926cac740391deb251`  
		Last Modified: Wed, 01 Nov 2023 08:18:07 GMT  
		Size: 1.9 KB (1866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a604bb0980f5b877ea1cfe73a85385ed541f85c82b22348d27f8d97a04d1ef76`  
		Last Modified: Wed, 01 Nov 2023 08:18:07 GMT  
		Size: 1.5 KB (1476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e27ee00f7fee2ee221e39d45b4abcfd90c63753f5e7263e8f30c67520aebc624`  
		Last Modified: Wed, 01 Nov 2023 08:18:08 GMT  
		Size: 1.4 MB (1386271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efa1816dcac43959f858ffcdbab80217277171e01d1c9a8fe3ebdd1c15db6697`  
		Last Modified: Wed, 01 Nov 2023 08:18:07 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1-standalone` - linux; mips64le

```console
$ docker pull adminer@sha256:ab1415fc7ebc72555fc80c9a4f64e05dae784d0acf5368241c39bf74ddf5bce4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.6 MB (92632325 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7faddbe6a665e6871431356947ac3c57cd3c6c20b85c84172da87b3f93017faa`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 01 Nov 2023 01:09:34 GMT
ADD file:2c9f9140e731974a497825454c08d67829f514a83742973e30454cc905ebac6c in / 
# Wed, 01 Nov 2023 01:09:39 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 06:47:42 GMT
STOPSIGNAL SIGINT
# Wed, 01 Nov 2023 06:49:39 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 06:49:45 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 01 Nov 2023 06:49:52 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 01 Nov 2023 06:49:55 GMT
WORKDIR /var/www/html
# Wed, 01 Nov 2023 06:49:58 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 01 Nov 2023 06:50:02 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 01 Nov 2023 06:50:05 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 01 Nov 2023 06:50:08 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 01 Nov 2023 06:51:01 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 01 Nov 2023 06:51:04 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 01 Nov 2023 06:51:07 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 01 Nov 2023 06:51:10 GMT
USER adminer
# Wed, 01 Nov 2023 06:51:14 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 01 Nov 2023 06:51:17 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:a10c6e715fcf314db953339b3e58b9e0167f6cd2d02bf633e20282058eb83331`  
		Last Modified: Wed, 01 Nov 2023 01:20:31 GMT  
		Size: 53.3 MB (53288991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3e05f3781dcb9702ce843ce679283bdea07c6614cdcba5a271127fd6bc7bb81`  
		Last Modified: Wed, 01 Nov 2023 06:53:43 GMT  
		Size: 38.0 MB (37952018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c67397db1f05d9d07b2053012f95d10c64b397e5f8578a8252c397958089cc7`  
		Last Modified: Wed, 01 Nov 2023 06:53:16 GMT  
		Size: 395.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12601b86b1fe6286ef174f4194db89610719071fc99b6004600546e313b75afc`  
		Last Modified: Wed, 01 Nov 2023 06:53:16 GMT  
		Size: 1.7 KB (1725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cf53f1325a00115717e22a2ad400917ea970c2863a9f0aa384c81111fe5f754`  
		Last Modified: Wed, 01 Nov 2023 06:53:16 GMT  
		Size: 1.5 KB (1481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fb917f0d920d8d2969e5b26d77d9384c94934f2c5d72677b658a9483e180240`  
		Last Modified: Wed, 01 Nov 2023 06:53:17 GMT  
		Size: 1.4 MB (1387222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af14639f108dd10f1d2bd5ea098b67c59009583ed8e393315c464ec4223e37d8`  
		Last Modified: Wed, 01 Nov 2023 06:53:16 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1-standalone` - linux; ppc64le

```console
$ docker pull adminer@sha256:489934d719089bd1c3827bdf673dcf7636376fbcbcfe837c4b7fa275ba366b62
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.3 MB (101265232 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6176ac38dfe8ab4e16662cc637ab4fb4b6f98c2e489cf4b4e6a66d578229ac6a`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Wed, 01 Nov 2023 02:50:13 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 01 Nov 2023 02:50:15 GMT
WORKDIR /var/www/html
# Wed, 01 Nov 2023 02:50:15 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 01 Nov 2023 02:50:15 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 01 Nov 2023 02:50:16 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 01 Nov 2023 02:50:16 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 01 Nov 2023 02:50:41 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 01 Nov 2023 02:50:42 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 01 Nov 2023 02:50:42 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 01 Nov 2023 02:50:43 GMT
USER adminer
# Wed, 01 Nov 2023 02:50:43 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 01 Nov 2023 02:50:44 GMT
EXPOSE 8080
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
	-	`sha256:c949ba7225949db3835c8321c7fd3fc61042abadd084780530933f2490a389ac`  
		Last Modified: Wed, 01 Nov 2023 02:51:40 GMT  
		Size: 1.9 KB (1878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69b23613e6440faf4dd53e85cce3379a37d371a55de8c3711313d4e8c2bdfcc7`  
		Last Modified: Wed, 01 Nov 2023 02:51:41 GMT  
		Size: 1.5 KB (1480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7424b8a43895b887591228e0a253d09fc56191f47ab5b4ab56d6fac2e6cbd9af`  
		Last Modified: Wed, 01 Nov 2023 02:51:41 GMT  
		Size: 1.4 MB (1386466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ee20cb0c3714aa128b4be5cdf5911002f2596f04b95e7e03962e22f45920bd3`  
		Last Modified: Wed, 01 Nov 2023 02:51:40 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.1-standalone` - linux; s390x

```console
$ docker pull adminer@sha256:febeaf64eb35379728a191c91b4c0fd744f0f25716db5b3a6383382bd813875b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.7 MB (93708845 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f56dc24645f9175629077bc05d2d1ef72a10391d530b75320409f480c64d72b5`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Wed, 01 Nov 2023 01:50:10 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 01 Nov 2023 01:50:10 GMT
WORKDIR /var/www/html
# Wed, 01 Nov 2023 01:50:10 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 01 Nov 2023 01:50:10 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 01 Nov 2023 01:50:10 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 01 Nov 2023 01:50:10 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 01 Nov 2023 01:50:18 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 01 Nov 2023 01:50:18 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 01 Nov 2023 01:50:18 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 01 Nov 2023 01:50:18 GMT
USER adminer
# Wed, 01 Nov 2023 01:50:18 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 01 Nov 2023 01:50:19 GMT
EXPOSE 8080
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
	-	`sha256:0ddb015dd3525d29ecb468826e1900bd5a42aedf948d046cf67cbb849116174a`  
		Last Modified: Wed, 01 Nov 2023 01:50:54 GMT  
		Size: 1.9 KB (1879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eeda1242b7f2fccc214b7bce16debf257837f0e99de553d8b0899289fdf4381`  
		Last Modified: Wed, 01 Nov 2023 01:50:54 GMT  
		Size: 1.5 KB (1477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b79f82c6e4dc3c8fa378683a146466b55a41e4a9b35103811abe39ff47528f4`  
		Last Modified: Wed, 01 Nov 2023 01:50:55 GMT  
		Size: 1.4 MB (1386366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:245a8a7cccf20a91e5d673ee924ca9853c1d060c66fdb377e8b8ca63166ac4cc`  
		Last Modified: Wed, 01 Nov 2023 01:50:54 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `adminer:fastcgi`

```console
$ docker pull adminer@sha256:312c0213bc482710a1129efafd0e8a9df7c8f74203cfc2effce3bd1273d8483c
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

### `adminer:fastcgi` - linux; arm variant v5

```console
$ docker pull adminer@sha256:640e60b56e718fd2129bc9dcf1cb60e4ae5be47614831844f3ae58081ef992a3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.2 MB (91206303 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:148a1a15fd20132f8babeb810dd6b79f0ad5b9affc91c2f8541b13ff8460c027`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Wed, 01 Nov 2023 00:48:39 GMT
ADD file:6fcdedd346da0744f7f45d0e7df77336a37ce87345bd414bd4e198804980781e in / 
# Wed, 01 Nov 2023 00:48:40 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 06:41:07 GMT
STOPSIGNAL SIGINT
# Wed, 01 Nov 2023 06:41:38 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 06:41:39 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 01 Nov 2023 06:42:05 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Wed, 01 Nov 2023 06:42:06 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 01 Nov 2023 06:42:06 GMT
WORKDIR /var/www/html
# Wed, 01 Nov 2023 06:42:06 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 01 Nov 2023 06:42:06 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 01 Nov 2023 06:42:06 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 01 Nov 2023 06:42:07 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 01 Nov 2023 06:42:20 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 01 Nov 2023 06:42:20 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 01 Nov 2023 06:42:21 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 01 Nov 2023 06:42:21 GMT
USER adminer
# Wed, 01 Nov 2023 06:42:21 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:e0adb3cac2906548cd3544bf3c384be3e3bdca9d41c37e11c160813af74301b9`  
		Last Modified: Wed, 01 Nov 2023 00:51:49 GMT  
		Size: 52.6 MB (52563334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e3623d9fb2289bbcd9a4586d409f13e8c27695bdb11f4c43599571aa1229528`  
		Last Modified: Wed, 01 Nov 2023 06:42:42 GMT  
		Size: 37.2 MB (37249740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28eac10d8db23ee6ea32d6b0c826db4a2dcbcd194ce18e99629fef2b283b4168`  
		Last Modified: Wed, 01 Nov 2023 06:42:33 GMT  
		Size: 389.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2319565cc3ff6648a187190305386506317c8e8b916e4c68a2fc7c4901bfade4`  
		Last Modified: Wed, 01 Nov 2023 06:42:59 GMT  
		Size: 2.7 KB (2712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d82fa5f5f057baa718cb408944b78d134414e710547b7fefe9e313b157794f83`  
		Last Modified: Wed, 01 Nov 2023 06:42:59 GMT  
		Size: 1.9 KB (1867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26294c9823754b7b6c80e1e42807e3d303d36ebf56f05c24f0267cb9f42f1a5c`  
		Last Modified: Wed, 01 Nov 2023 06:42:58 GMT  
		Size: 1.5 KB (1476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1805ed31823bd60aec3a510dc6813b3e6df00428670492f806313f056d98accc`  
		Last Modified: Wed, 01 Nov 2023 06:42:59 GMT  
		Size: 1.4 MB (1386295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3379baf5fcc5e2ee2f374067c687e3614bb3a564ce83ec47aa3088df5900c339`  
		Last Modified: Wed, 01 Nov 2023 06:42:59 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:fastcgi` - linux; arm variant v7

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

### `adminer:fastcgi` - linux; arm64 variant v8

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

### `adminer:fastcgi` - linux; 386

```console
$ docker pull adminer@sha256:baf03604dff500f1ff723513a538bd2632e854534952802ef3c2757ab9ec7284
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.0 MB (97000221 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a29b774050e6bb60654c4629b38274b8039fbff780360aa51ab5c918374888e`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Wed, 01 Nov 2023 00:39:06 GMT
ADD file:4095d27bc1a281dda044919be3bb570d581df169c01f22b0963b38e0dd6d9eff in / 
# Wed, 01 Nov 2023 00:39:07 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 08:16:42 GMT
STOPSIGNAL SIGINT
# Wed, 01 Nov 2023 08:17:12 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 08:17:13 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 01 Nov 2023 08:17:40 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Wed, 01 Nov 2023 08:17:41 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 01 Nov 2023 08:17:41 GMT
WORKDIR /var/www/html
# Wed, 01 Nov 2023 08:17:41 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 01 Nov 2023 08:17:41 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 01 Nov 2023 08:17:41 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 01 Nov 2023 08:17:41 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 01 Nov 2023 08:17:54 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 01 Nov 2023 08:17:55 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 01 Nov 2023 08:17:55 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 01 Nov 2023 08:17:55 GMT
USER adminer
# Wed, 01 Nov 2023 08:17:55 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:95d6aa56ba74b8ed0a732c4676a2c45c84a18076696d466cd9bf0b459c600e02`  
		Last Modified: Wed, 01 Nov 2023 00:43:49 GMT  
		Size: 56.0 MB (56046261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80589068561f705cd353c87358a0cecc8311057c942f023093c00c5ae59b0da4`  
		Last Modified: Wed, 01 Nov 2023 08:18:18 GMT  
		Size: 39.6 MB (39560745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c2dcd79bac9186cbea2e89e7c6085867c2ec84a4322ad7e80642bbe4e78fc42`  
		Last Modified: Wed, 01 Nov 2023 08:18:07 GMT  
		Size: 389.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce8777aa37435cb70275cafb5973d4c38ade71490ab02d4690e7243d7f42fa99`  
		Last Modified: Wed, 01 Nov 2023 08:18:38 GMT  
		Size: 2.7 KB (2708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3092383d86bf2247454565915d60711072083b945827d3a71d04b2e8e7d5a24`  
		Last Modified: Wed, 01 Nov 2023 08:18:38 GMT  
		Size: 1.9 KB (1866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58ab83e0c0b5af9550f8219863a015b9f64aac19bfd190214266dddcdae1987d`  
		Last Modified: Wed, 01 Nov 2023 08:18:38 GMT  
		Size: 1.5 KB (1479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1ad071ea7480f652575c1ff65ee4ef869a9eb9b6f053ca5f2dae11776838485`  
		Last Modified: Wed, 01 Nov 2023 08:18:38 GMT  
		Size: 1.4 MB (1386283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31f82fe0941deccb9e97f691bccd364714153f8af834bfb61010a0edeed7d95b`  
		Last Modified: Wed, 01 Nov 2023 08:18:38 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:fastcgi` - linux; mips64le

```console
$ docker pull adminer@sha256:d5005a80e57907d2bf1e882cd453c47a7c6e2044997f7f5f2d6c1737a73c8e53
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.6 MB (92635040 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46fee5e1b1c3fefa23d38e502f9c95f79c82daaf2e4a9015a2f079af2d582ea5`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php-fpm7.4"]`

```dockerfile
# Wed, 01 Nov 2023 01:09:34 GMT
ADD file:2c9f9140e731974a497825454c08d67829f514a83742973e30454cc905ebac6c in / 
# Wed, 01 Nov 2023 01:09:39 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 06:47:42 GMT
STOPSIGNAL SIGINT
# Wed, 01 Nov 2023 06:49:39 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 06:49:45 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 01 Nov 2023 06:51:29 GMT
RUN set -ex;	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee /etc/php/7.4/fpm/pool.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee /etc/php/7.4/fpm/pool.d/zz-docker.conf; 	sed -i '/^pid =/d' /etc/php/7.4/fpm/php-fpm.conf
# Wed, 01 Nov 2023 06:51:36 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 01 Nov 2023 06:51:39 GMT
WORKDIR /var/www/html
# Wed, 01 Nov 2023 06:51:42 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 01 Nov 2023 06:51:46 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 01 Nov 2023 06:51:49 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 01 Nov 2023 06:51:52 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 01 Nov 2023 06:52:43 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 01 Nov 2023 06:52:46 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 01 Nov 2023 06:52:50 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 01 Nov 2023 06:52:53 GMT
USER adminer
# Wed, 01 Nov 2023 06:52:56 GMT
CMD ["php-fpm7.4"]
```

-	Layers:
	-	`sha256:a10c6e715fcf314db953339b3e58b9e0167f6cd2d02bf633e20282058eb83331`  
		Last Modified: Wed, 01 Nov 2023 01:20:31 GMT  
		Size: 53.3 MB (53288991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3e05f3781dcb9702ce843ce679283bdea07c6614cdcba5a271127fd6bc7bb81`  
		Last Modified: Wed, 01 Nov 2023 06:53:43 GMT  
		Size: 38.0 MB (37952018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c67397db1f05d9d07b2053012f95d10c64b397e5f8578a8252c397958089cc7`  
		Last Modified: Wed, 01 Nov 2023 06:53:16 GMT  
		Size: 395.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1efe29ad2e6399b06c40a1f74ef708babaf49feb6d4a81ffc433dbe62507869a`  
		Last Modified: Wed, 01 Nov 2023 06:54:03 GMT  
		Size: 2.7 KB (2714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5e18030af38a29600f3748bcbad3e59b6ec984e1949a992135f469b7a511bb4`  
		Last Modified: Wed, 01 Nov 2023 06:54:03 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a32ef85d04c2f926ef96c9ffa9dcac7659bc192103442cb5a3c6496c49d1f32`  
		Last Modified: Wed, 01 Nov 2023 06:54:03 GMT  
		Size: 1.5 KB (1482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce599942d3ca2661bbeab5bf9752328464303caf6cfbfa70875693cadebd96ec`  
		Last Modified: Wed, 01 Nov 2023 06:54:05 GMT  
		Size: 1.4 MB (1387212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba28223ab0fd0ba91b6c220a2f17cd52d8fec220e52b4a693c92712fed5aa474`  
		Last Modified: Wed, 01 Nov 2023 06:54:03 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:fastcgi` - linux; ppc64le

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

### `adminer:fastcgi` - linux; s390x

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

## `adminer:latest`

```console
$ docker pull adminer@sha256:b7f0e6681e9a77916daf2f070616d25e3fd687b84550aa6673de9a24407dd613
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
$ docker pull adminer@sha256:b96876e1c6d4eda21b2653d54bb8c9d4674fc177749254c5a44d097f92e2362e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.9 MB (95941196 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5cec1739340987c68ebd5535d5297dc62cc4fa489a253b4d84bb800b461e129`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Wed, 01 Nov 2023 02:53:39 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 01 Nov 2023 02:53:39 GMT
WORKDIR /var/www/html
# Wed, 01 Nov 2023 02:53:39 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 01 Nov 2023 02:53:39 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 01 Nov 2023 02:53:39 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 01 Nov 2023 02:53:39 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 01 Nov 2023 02:53:50 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 01 Nov 2023 02:53:50 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 01 Nov 2023 02:53:50 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 01 Nov 2023 02:53:50 GMT
USER adminer
# Wed, 01 Nov 2023 02:53:50 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 01 Nov 2023 02:53:50 GMT
EXPOSE 8080
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
	-	`sha256:bf435083814d20c35b08cac2c04f42a971fe8c772a6ff6ab5ea2dbb4c5365923`  
		Last Modified: Wed, 01 Nov 2023 02:54:24 GMT  
		Size: 1.9 KB (1876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:298e667e63eeffb2a143be3c3aeed4888c95d316e453939646663ae94cb39b38`  
		Last Modified: Wed, 01 Nov 2023 02:54:25 GMT  
		Size: 1.5 KB (1482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:009b4e930c2c0c866efcbe990a45b4aaa86c6ae9428410afb5842ed5a4a61a2f`  
		Last Modified: Wed, 01 Nov 2023 02:54:25 GMT  
		Size: 1.4 MB (1386349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:795fdddea697817d7c6a47b855376bc15a2ece944ad41fb076688cf55c7a749a`  
		Last Modified: Wed, 01 Nov 2023 02:54:24 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:latest` - linux; arm variant v5

```console
$ docker pull adminer@sha256:37f77f5ee6832c7e087446aedd7fbc4759897435702305e7331410f4ccf749a9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.2 MB (91203583 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4428e260c8ac1e52db7ab4bca8db1cc7baafd67bb17a2206f99ccb97cb9c167`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 01 Nov 2023 00:48:39 GMT
ADD file:6fcdedd346da0744f7f45d0e7df77336a37ce87345bd414bd4e198804980781e in / 
# Wed, 01 Nov 2023 00:48:40 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 06:41:07 GMT
STOPSIGNAL SIGINT
# Wed, 01 Nov 2023 06:41:38 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 06:41:39 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 01 Nov 2023 06:41:40 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 01 Nov 2023 06:41:40 GMT
WORKDIR /var/www/html
# Wed, 01 Nov 2023 06:41:40 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 01 Nov 2023 06:41:40 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 01 Nov 2023 06:41:40 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 01 Nov 2023 06:41:40 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 01 Nov 2023 06:41:55 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 01 Nov 2023 06:41:55 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 01 Nov 2023 06:41:55 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 01 Nov 2023 06:41:56 GMT
USER adminer
# Wed, 01 Nov 2023 06:41:56 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 01 Nov 2023 06:41:56 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:e0adb3cac2906548cd3544bf3c384be3e3bdca9d41c37e11c160813af74301b9`  
		Last Modified: Wed, 01 Nov 2023 00:51:49 GMT  
		Size: 52.6 MB (52563334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e3623d9fb2289bbcd9a4586d409f13e8c27695bdb11f4c43599571aa1229528`  
		Last Modified: Wed, 01 Nov 2023 06:42:42 GMT  
		Size: 37.2 MB (37249740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28eac10d8db23ee6ea32d6b0c826db4a2dcbcd194ce18e99629fef2b283b4168`  
		Last Modified: Wed, 01 Nov 2023 06:42:33 GMT  
		Size: 389.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5779125ab319b67fbc7cf3bcaa969968771e9e472e58c08976728bb8d7569d56`  
		Last Modified: Wed, 01 Nov 2023 06:42:33 GMT  
		Size: 1.9 KB (1869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1952b238fb472fe6155a5c880e5d83d4c58dee30db79ba608c878282838500e`  
		Last Modified: Wed, 01 Nov 2023 06:42:33 GMT  
		Size: 1.5 KB (1476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85025f444620cafd6192a2667af59fdf4aca316094a82a43909a7e9f96e254f9`  
		Last Modified: Wed, 01 Nov 2023 06:42:33 GMT  
		Size: 1.4 MB (1386285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56f0c59e7ad269f06b6107635f33308fe74056eebdde42c8932886bf95c1885b`  
		Last Modified: Wed, 01 Nov 2023 06:42:33 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:latest` - linux; arm variant v7

```console
$ docker pull adminer@sha256:03812b425c6b805691941ae806db34dc0b8a3f161f3a4e11ea0c54eb783037fb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.8 MB (87794095 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c9e7020270d790860f62ddf4e490a5409714c8f1d910f0e5552e34467640d9d`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Wed, 01 Nov 2023 02:13:44 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 01 Nov 2023 02:13:44 GMT
WORKDIR /var/www/html
# Wed, 01 Nov 2023 02:13:44 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 01 Nov 2023 02:13:44 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 01 Nov 2023 02:13:44 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 01 Nov 2023 02:13:44 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 01 Nov 2023 02:14:02 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 01 Nov 2023 02:14:02 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 01 Nov 2023 02:14:02 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 01 Nov 2023 02:14:02 GMT
USER adminer
# Wed, 01 Nov 2023 02:14:02 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 01 Nov 2023 02:14:02 GMT
EXPOSE 8080
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
	-	`sha256:b5ff4543277751a4ec131370a18afcbdcefbb299cac4f8b46d83ca0bb7e2fbb5`  
		Last Modified: Wed, 01 Nov 2023 02:14:32 GMT  
		Size: 1.9 KB (1867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8035a3dd0d4bf0c16736f3dc9982fdf586cb8db7c9c17bdfc7b7857d8236a5f8`  
		Last Modified: Wed, 01 Nov 2023 02:14:32 GMT  
		Size: 1.5 KB (1482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3e860a8d0ed1174c57c59e038d17c8c011e9262aac708373f223685b8a474c3`  
		Last Modified: Wed, 01 Nov 2023 02:14:32 GMT  
		Size: 1.4 MB (1386280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46610df748fd7888da3ef3e1419131554e3c580380b72af8c2182bd4b0c868d3`  
		Last Modified: Wed, 01 Nov 2023 02:14:32 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:latest` - linux; arm64 variant v8

```console
$ docker pull adminer@sha256:63e8c57d2e82e0d50f641f56ce18316ba1f8a12a4640c2b6966453d198a8f14f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.3 MB (94343887 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e729f030ea5398e5fb915c10c2a7b811bffbcfd0932c22b49cba6738c053e8b6`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Wed, 01 Nov 2023 02:01:40 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 01 Nov 2023 02:01:40 GMT
WORKDIR /var/www/html
# Wed, 01 Nov 2023 02:01:40 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 01 Nov 2023 02:01:40 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 01 Nov 2023 02:01:40 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 01 Nov 2023 02:01:40 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 01 Nov 2023 02:01:50 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 01 Nov 2023 02:01:50 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 01 Nov 2023 02:01:50 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 01 Nov 2023 02:01:51 GMT
USER adminer
# Wed, 01 Nov 2023 02:01:51 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 01 Nov 2023 02:01:51 GMT
EXPOSE 8080
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
	-	`sha256:96cc754b457a6496cd3a8ba90b44ea5d39534c43f26dc2cb557b71a76902a3d6`  
		Last Modified: Wed, 01 Nov 2023 02:02:15 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:535170e27a39ee08c1372464244541113d3a4d899c1c7676ebca43a9f09b2421`  
		Last Modified: Wed, 01 Nov 2023 02:02:15 GMT  
		Size: 1.5 KB (1482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83e4006979461007bc0f7c1b0bb3b0675f29b405562d0cc37f5cf5b0711a309e`  
		Last Modified: Wed, 01 Nov 2023 02:02:16 GMT  
		Size: 1.4 MB (1386269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aecfb4d8f96734c7035d67c5e3b751eb15f305ae0b1d2855921c5d1d0d83b5bc`  
		Last Modified: Wed, 01 Nov 2023 02:02:15 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:latest` - linux; 386

```console
$ docker pull adminer@sha256:a21c1d6915687a26e34d9f2f09f9b5104e64bc71aa36e19afae9c5d8c67a9040
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.0 MB (96997500 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3517f7704a6b833432e5e5e0144c6ce4e15ba0199adde89fb66fba372920f37`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 01 Nov 2023 00:39:06 GMT
ADD file:4095d27bc1a281dda044919be3bb570d581df169c01f22b0963b38e0dd6d9eff in / 
# Wed, 01 Nov 2023 00:39:07 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 08:16:42 GMT
STOPSIGNAL SIGINT
# Wed, 01 Nov 2023 08:17:12 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 08:17:13 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 01 Nov 2023 08:17:14 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 01 Nov 2023 08:17:14 GMT
WORKDIR /var/www/html
# Wed, 01 Nov 2023 08:17:14 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 01 Nov 2023 08:17:14 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 01 Nov 2023 08:17:14 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 01 Nov 2023 08:17:14 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 01 Nov 2023 08:17:28 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 01 Nov 2023 08:17:28 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 01 Nov 2023 08:17:28 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 01 Nov 2023 08:17:28 GMT
USER adminer
# Wed, 01 Nov 2023 08:17:28 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 01 Nov 2023 08:17:28 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:95d6aa56ba74b8ed0a732c4676a2c45c84a18076696d466cd9bf0b459c600e02`  
		Last Modified: Wed, 01 Nov 2023 00:43:49 GMT  
		Size: 56.0 MB (56046261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80589068561f705cd353c87358a0cecc8311057c942f023093c00c5ae59b0da4`  
		Last Modified: Wed, 01 Nov 2023 08:18:18 GMT  
		Size: 39.6 MB (39560745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c2dcd79bac9186cbea2e89e7c6085867c2ec84a4322ad7e80642bbe4e78fc42`  
		Last Modified: Wed, 01 Nov 2023 08:18:07 GMT  
		Size: 389.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c684759995fea1dd384d011644236354c8d098a591ea7926cac740391deb251`  
		Last Modified: Wed, 01 Nov 2023 08:18:07 GMT  
		Size: 1.9 KB (1866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a604bb0980f5b877ea1cfe73a85385ed541f85c82b22348d27f8d97a04d1ef76`  
		Last Modified: Wed, 01 Nov 2023 08:18:07 GMT  
		Size: 1.5 KB (1476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e27ee00f7fee2ee221e39d45b4abcfd90c63753f5e7263e8f30c67520aebc624`  
		Last Modified: Wed, 01 Nov 2023 08:18:08 GMT  
		Size: 1.4 MB (1386271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efa1816dcac43959f858ffcdbab80217277171e01d1c9a8fe3ebdd1c15db6697`  
		Last Modified: Wed, 01 Nov 2023 08:18:07 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:latest` - linux; mips64le

```console
$ docker pull adminer@sha256:ab1415fc7ebc72555fc80c9a4f64e05dae784d0acf5368241c39bf74ddf5bce4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.6 MB (92632325 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7faddbe6a665e6871431356947ac3c57cd3c6c20b85c84172da87b3f93017faa`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 01 Nov 2023 01:09:34 GMT
ADD file:2c9f9140e731974a497825454c08d67829f514a83742973e30454cc905ebac6c in / 
# Wed, 01 Nov 2023 01:09:39 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 06:47:42 GMT
STOPSIGNAL SIGINT
# Wed, 01 Nov 2023 06:49:39 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 06:49:45 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 01 Nov 2023 06:49:52 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 01 Nov 2023 06:49:55 GMT
WORKDIR /var/www/html
# Wed, 01 Nov 2023 06:49:58 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 01 Nov 2023 06:50:02 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 01 Nov 2023 06:50:05 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 01 Nov 2023 06:50:08 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 01 Nov 2023 06:51:01 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 01 Nov 2023 06:51:04 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 01 Nov 2023 06:51:07 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 01 Nov 2023 06:51:10 GMT
USER adminer
# Wed, 01 Nov 2023 06:51:14 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 01 Nov 2023 06:51:17 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:a10c6e715fcf314db953339b3e58b9e0167f6cd2d02bf633e20282058eb83331`  
		Last Modified: Wed, 01 Nov 2023 01:20:31 GMT  
		Size: 53.3 MB (53288991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3e05f3781dcb9702ce843ce679283bdea07c6614cdcba5a271127fd6bc7bb81`  
		Last Modified: Wed, 01 Nov 2023 06:53:43 GMT  
		Size: 38.0 MB (37952018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c67397db1f05d9d07b2053012f95d10c64b397e5f8578a8252c397958089cc7`  
		Last Modified: Wed, 01 Nov 2023 06:53:16 GMT  
		Size: 395.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12601b86b1fe6286ef174f4194db89610719071fc99b6004600546e313b75afc`  
		Last Modified: Wed, 01 Nov 2023 06:53:16 GMT  
		Size: 1.7 KB (1725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cf53f1325a00115717e22a2ad400917ea970c2863a9f0aa384c81111fe5f754`  
		Last Modified: Wed, 01 Nov 2023 06:53:16 GMT  
		Size: 1.5 KB (1481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fb917f0d920d8d2969e5b26d77d9384c94934f2c5d72677b658a9483e180240`  
		Last Modified: Wed, 01 Nov 2023 06:53:17 GMT  
		Size: 1.4 MB (1387222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af14639f108dd10f1d2bd5ea098b67c59009583ed8e393315c464ec4223e37d8`  
		Last Modified: Wed, 01 Nov 2023 06:53:16 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:latest` - linux; ppc64le

```console
$ docker pull adminer@sha256:489934d719089bd1c3827bdf673dcf7636376fbcbcfe837c4b7fa275ba366b62
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.3 MB (101265232 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6176ac38dfe8ab4e16662cc637ab4fb4b6f98c2e489cf4b4e6a66d578229ac6a`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Wed, 01 Nov 2023 02:50:13 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 01 Nov 2023 02:50:15 GMT
WORKDIR /var/www/html
# Wed, 01 Nov 2023 02:50:15 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 01 Nov 2023 02:50:15 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 01 Nov 2023 02:50:16 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 01 Nov 2023 02:50:16 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 01 Nov 2023 02:50:41 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 01 Nov 2023 02:50:42 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 01 Nov 2023 02:50:42 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 01 Nov 2023 02:50:43 GMT
USER adminer
# Wed, 01 Nov 2023 02:50:43 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 01 Nov 2023 02:50:44 GMT
EXPOSE 8080
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
	-	`sha256:c949ba7225949db3835c8321c7fd3fc61042abadd084780530933f2490a389ac`  
		Last Modified: Wed, 01 Nov 2023 02:51:40 GMT  
		Size: 1.9 KB (1878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69b23613e6440faf4dd53e85cce3379a37d371a55de8c3711313d4e8c2bdfcc7`  
		Last Modified: Wed, 01 Nov 2023 02:51:41 GMT  
		Size: 1.5 KB (1480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7424b8a43895b887591228e0a253d09fc56191f47ab5b4ab56d6fac2e6cbd9af`  
		Last Modified: Wed, 01 Nov 2023 02:51:41 GMT  
		Size: 1.4 MB (1386466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ee20cb0c3714aa128b4be5cdf5911002f2596f04b95e7e03962e22f45920bd3`  
		Last Modified: Wed, 01 Nov 2023 02:51:40 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:latest` - linux; s390x

```console
$ docker pull adminer@sha256:febeaf64eb35379728a191c91b4c0fd744f0f25716db5b3a6383382bd813875b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.7 MB (93708845 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f56dc24645f9175629077bc05d2d1ef72a10391d530b75320409f480c64d72b5`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Wed, 01 Nov 2023 01:50:10 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 01 Nov 2023 01:50:10 GMT
WORKDIR /var/www/html
# Wed, 01 Nov 2023 01:50:10 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 01 Nov 2023 01:50:10 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 01 Nov 2023 01:50:10 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 01 Nov 2023 01:50:10 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 01 Nov 2023 01:50:18 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 01 Nov 2023 01:50:18 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 01 Nov 2023 01:50:18 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 01 Nov 2023 01:50:18 GMT
USER adminer
# Wed, 01 Nov 2023 01:50:18 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 01 Nov 2023 01:50:19 GMT
EXPOSE 8080
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
	-	`sha256:0ddb015dd3525d29ecb468826e1900bd5a42aedf948d046cf67cbb849116174a`  
		Last Modified: Wed, 01 Nov 2023 01:50:54 GMT  
		Size: 1.9 KB (1879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eeda1242b7f2fccc214b7bce16debf257837f0e99de553d8b0899289fdf4381`  
		Last Modified: Wed, 01 Nov 2023 01:50:54 GMT  
		Size: 1.5 KB (1477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b79f82c6e4dc3c8fa378683a146466b55a41e4a9b35103811abe39ff47528f4`  
		Last Modified: Wed, 01 Nov 2023 01:50:55 GMT  
		Size: 1.4 MB (1386366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:245a8a7cccf20a91e5d673ee924ca9853c1d060c66fdb377e8b8ca63166ac4cc`  
		Last Modified: Wed, 01 Nov 2023 01:50:54 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `adminer:standalone`

```console
$ docker pull adminer@sha256:b7f0e6681e9a77916daf2f070616d25e3fd687b84550aa6673de9a24407dd613
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
$ docker pull adminer@sha256:b96876e1c6d4eda21b2653d54bb8c9d4674fc177749254c5a44d097f92e2362e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.9 MB (95941196 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5cec1739340987c68ebd5535d5297dc62cc4fa489a253b4d84bb800b461e129`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Wed, 01 Nov 2023 02:53:39 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 01 Nov 2023 02:53:39 GMT
WORKDIR /var/www/html
# Wed, 01 Nov 2023 02:53:39 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 01 Nov 2023 02:53:39 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 01 Nov 2023 02:53:39 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 01 Nov 2023 02:53:39 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 01 Nov 2023 02:53:50 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 01 Nov 2023 02:53:50 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 01 Nov 2023 02:53:50 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 01 Nov 2023 02:53:50 GMT
USER adminer
# Wed, 01 Nov 2023 02:53:50 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 01 Nov 2023 02:53:50 GMT
EXPOSE 8080
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
	-	`sha256:bf435083814d20c35b08cac2c04f42a971fe8c772a6ff6ab5ea2dbb4c5365923`  
		Last Modified: Wed, 01 Nov 2023 02:54:24 GMT  
		Size: 1.9 KB (1876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:298e667e63eeffb2a143be3c3aeed4888c95d316e453939646663ae94cb39b38`  
		Last Modified: Wed, 01 Nov 2023 02:54:25 GMT  
		Size: 1.5 KB (1482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:009b4e930c2c0c866efcbe990a45b4aaa86c6ae9428410afb5842ed5a4a61a2f`  
		Last Modified: Wed, 01 Nov 2023 02:54:25 GMT  
		Size: 1.4 MB (1386349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:795fdddea697817d7c6a47b855376bc15a2ece944ad41fb076688cf55c7a749a`  
		Last Modified: Wed, 01 Nov 2023 02:54:24 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:standalone` - linux; arm variant v5

```console
$ docker pull adminer@sha256:37f77f5ee6832c7e087446aedd7fbc4759897435702305e7331410f4ccf749a9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.2 MB (91203583 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4428e260c8ac1e52db7ab4bca8db1cc7baafd67bb17a2206f99ccb97cb9c167`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 01 Nov 2023 00:48:39 GMT
ADD file:6fcdedd346da0744f7f45d0e7df77336a37ce87345bd414bd4e198804980781e in / 
# Wed, 01 Nov 2023 00:48:40 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 06:41:07 GMT
STOPSIGNAL SIGINT
# Wed, 01 Nov 2023 06:41:38 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 06:41:39 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 01 Nov 2023 06:41:40 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 01 Nov 2023 06:41:40 GMT
WORKDIR /var/www/html
# Wed, 01 Nov 2023 06:41:40 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 01 Nov 2023 06:41:40 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 01 Nov 2023 06:41:40 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 01 Nov 2023 06:41:40 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 01 Nov 2023 06:41:55 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 01 Nov 2023 06:41:55 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 01 Nov 2023 06:41:55 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 01 Nov 2023 06:41:56 GMT
USER adminer
# Wed, 01 Nov 2023 06:41:56 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 01 Nov 2023 06:41:56 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:e0adb3cac2906548cd3544bf3c384be3e3bdca9d41c37e11c160813af74301b9`  
		Last Modified: Wed, 01 Nov 2023 00:51:49 GMT  
		Size: 52.6 MB (52563334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e3623d9fb2289bbcd9a4586d409f13e8c27695bdb11f4c43599571aa1229528`  
		Last Modified: Wed, 01 Nov 2023 06:42:42 GMT  
		Size: 37.2 MB (37249740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28eac10d8db23ee6ea32d6b0c826db4a2dcbcd194ce18e99629fef2b283b4168`  
		Last Modified: Wed, 01 Nov 2023 06:42:33 GMT  
		Size: 389.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5779125ab319b67fbc7cf3bcaa969968771e9e472e58c08976728bb8d7569d56`  
		Last Modified: Wed, 01 Nov 2023 06:42:33 GMT  
		Size: 1.9 KB (1869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1952b238fb472fe6155a5c880e5d83d4c58dee30db79ba608c878282838500e`  
		Last Modified: Wed, 01 Nov 2023 06:42:33 GMT  
		Size: 1.5 KB (1476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85025f444620cafd6192a2667af59fdf4aca316094a82a43909a7e9f96e254f9`  
		Last Modified: Wed, 01 Nov 2023 06:42:33 GMT  
		Size: 1.4 MB (1386285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56f0c59e7ad269f06b6107635f33308fe74056eebdde42c8932886bf95c1885b`  
		Last Modified: Wed, 01 Nov 2023 06:42:33 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:standalone` - linux; arm variant v7

```console
$ docker pull adminer@sha256:03812b425c6b805691941ae806db34dc0b8a3f161f3a4e11ea0c54eb783037fb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.8 MB (87794095 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c9e7020270d790860f62ddf4e490a5409714c8f1d910f0e5552e34467640d9d`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Wed, 01 Nov 2023 02:13:44 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 01 Nov 2023 02:13:44 GMT
WORKDIR /var/www/html
# Wed, 01 Nov 2023 02:13:44 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 01 Nov 2023 02:13:44 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 01 Nov 2023 02:13:44 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 01 Nov 2023 02:13:44 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 01 Nov 2023 02:14:02 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 01 Nov 2023 02:14:02 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 01 Nov 2023 02:14:02 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 01 Nov 2023 02:14:02 GMT
USER adminer
# Wed, 01 Nov 2023 02:14:02 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 01 Nov 2023 02:14:02 GMT
EXPOSE 8080
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
	-	`sha256:b5ff4543277751a4ec131370a18afcbdcefbb299cac4f8b46d83ca0bb7e2fbb5`  
		Last Modified: Wed, 01 Nov 2023 02:14:32 GMT  
		Size: 1.9 KB (1867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8035a3dd0d4bf0c16736f3dc9982fdf586cb8db7c9c17bdfc7b7857d8236a5f8`  
		Last Modified: Wed, 01 Nov 2023 02:14:32 GMT  
		Size: 1.5 KB (1482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3e860a8d0ed1174c57c59e038d17c8c011e9262aac708373f223685b8a474c3`  
		Last Modified: Wed, 01 Nov 2023 02:14:32 GMT  
		Size: 1.4 MB (1386280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46610df748fd7888da3ef3e1419131554e3c580380b72af8c2182bd4b0c868d3`  
		Last Modified: Wed, 01 Nov 2023 02:14:32 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:standalone` - linux; arm64 variant v8

```console
$ docker pull adminer@sha256:63e8c57d2e82e0d50f641f56ce18316ba1f8a12a4640c2b6966453d198a8f14f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.3 MB (94343887 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e729f030ea5398e5fb915c10c2a7b811bffbcfd0932c22b49cba6738c053e8b6`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Wed, 01 Nov 2023 02:01:40 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 01 Nov 2023 02:01:40 GMT
WORKDIR /var/www/html
# Wed, 01 Nov 2023 02:01:40 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 01 Nov 2023 02:01:40 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 01 Nov 2023 02:01:40 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 01 Nov 2023 02:01:40 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 01 Nov 2023 02:01:50 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 01 Nov 2023 02:01:50 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 01 Nov 2023 02:01:50 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 01 Nov 2023 02:01:51 GMT
USER adminer
# Wed, 01 Nov 2023 02:01:51 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 01 Nov 2023 02:01:51 GMT
EXPOSE 8080
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
	-	`sha256:96cc754b457a6496cd3a8ba90b44ea5d39534c43f26dc2cb557b71a76902a3d6`  
		Last Modified: Wed, 01 Nov 2023 02:02:15 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:535170e27a39ee08c1372464244541113d3a4d899c1c7676ebca43a9f09b2421`  
		Last Modified: Wed, 01 Nov 2023 02:02:15 GMT  
		Size: 1.5 KB (1482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83e4006979461007bc0f7c1b0bb3b0675f29b405562d0cc37f5cf5b0711a309e`  
		Last Modified: Wed, 01 Nov 2023 02:02:16 GMT  
		Size: 1.4 MB (1386269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aecfb4d8f96734c7035d67c5e3b751eb15f305ae0b1d2855921c5d1d0d83b5bc`  
		Last Modified: Wed, 01 Nov 2023 02:02:15 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:standalone` - linux; 386

```console
$ docker pull adminer@sha256:a21c1d6915687a26e34d9f2f09f9b5104e64bc71aa36e19afae9c5d8c67a9040
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.0 MB (96997500 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3517f7704a6b833432e5e5e0144c6ce4e15ba0199adde89fb66fba372920f37`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 01 Nov 2023 00:39:06 GMT
ADD file:4095d27bc1a281dda044919be3bb570d581df169c01f22b0963b38e0dd6d9eff in / 
# Wed, 01 Nov 2023 00:39:07 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 08:16:42 GMT
STOPSIGNAL SIGINT
# Wed, 01 Nov 2023 08:17:12 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 08:17:13 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 01 Nov 2023 08:17:14 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 01 Nov 2023 08:17:14 GMT
WORKDIR /var/www/html
# Wed, 01 Nov 2023 08:17:14 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 01 Nov 2023 08:17:14 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 01 Nov 2023 08:17:14 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 01 Nov 2023 08:17:14 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 01 Nov 2023 08:17:28 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 01 Nov 2023 08:17:28 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 01 Nov 2023 08:17:28 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 01 Nov 2023 08:17:28 GMT
USER adminer
# Wed, 01 Nov 2023 08:17:28 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 01 Nov 2023 08:17:28 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:95d6aa56ba74b8ed0a732c4676a2c45c84a18076696d466cd9bf0b459c600e02`  
		Last Modified: Wed, 01 Nov 2023 00:43:49 GMT  
		Size: 56.0 MB (56046261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80589068561f705cd353c87358a0cecc8311057c942f023093c00c5ae59b0da4`  
		Last Modified: Wed, 01 Nov 2023 08:18:18 GMT  
		Size: 39.6 MB (39560745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c2dcd79bac9186cbea2e89e7c6085867c2ec84a4322ad7e80642bbe4e78fc42`  
		Last Modified: Wed, 01 Nov 2023 08:18:07 GMT  
		Size: 389.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c684759995fea1dd384d011644236354c8d098a591ea7926cac740391deb251`  
		Last Modified: Wed, 01 Nov 2023 08:18:07 GMT  
		Size: 1.9 KB (1866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a604bb0980f5b877ea1cfe73a85385ed541f85c82b22348d27f8d97a04d1ef76`  
		Last Modified: Wed, 01 Nov 2023 08:18:07 GMT  
		Size: 1.5 KB (1476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e27ee00f7fee2ee221e39d45b4abcfd90c63753f5e7263e8f30c67520aebc624`  
		Last Modified: Wed, 01 Nov 2023 08:18:08 GMT  
		Size: 1.4 MB (1386271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efa1816dcac43959f858ffcdbab80217277171e01d1c9a8fe3ebdd1c15db6697`  
		Last Modified: Wed, 01 Nov 2023 08:18:07 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:standalone` - linux; mips64le

```console
$ docker pull adminer@sha256:ab1415fc7ebc72555fc80c9a4f64e05dae784d0acf5368241c39bf74ddf5bce4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.6 MB (92632325 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7faddbe6a665e6871431356947ac3c57cd3c6c20b85c84172da87b3f93017faa`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 01 Nov 2023 01:09:34 GMT
ADD file:2c9f9140e731974a497825454c08d67829f514a83742973e30454cc905ebac6c in / 
# Wed, 01 Nov 2023 01:09:39 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 06:47:42 GMT
STOPSIGNAL SIGINT
# Wed, 01 Nov 2023 06:49:39 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 06:49:45 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 01 Nov 2023 06:49:52 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 01 Nov 2023 06:49:55 GMT
WORKDIR /var/www/html
# Wed, 01 Nov 2023 06:49:58 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 01 Nov 2023 06:50:02 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 01 Nov 2023 06:50:05 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 01 Nov 2023 06:50:08 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 01 Nov 2023 06:51:01 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 01 Nov 2023 06:51:04 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 01 Nov 2023 06:51:07 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 01 Nov 2023 06:51:10 GMT
USER adminer
# Wed, 01 Nov 2023 06:51:14 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 01 Nov 2023 06:51:17 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:a10c6e715fcf314db953339b3e58b9e0167f6cd2d02bf633e20282058eb83331`  
		Last Modified: Wed, 01 Nov 2023 01:20:31 GMT  
		Size: 53.3 MB (53288991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3e05f3781dcb9702ce843ce679283bdea07c6614cdcba5a271127fd6bc7bb81`  
		Last Modified: Wed, 01 Nov 2023 06:53:43 GMT  
		Size: 38.0 MB (37952018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c67397db1f05d9d07b2053012f95d10c64b397e5f8578a8252c397958089cc7`  
		Last Modified: Wed, 01 Nov 2023 06:53:16 GMT  
		Size: 395.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12601b86b1fe6286ef174f4194db89610719071fc99b6004600546e313b75afc`  
		Last Modified: Wed, 01 Nov 2023 06:53:16 GMT  
		Size: 1.7 KB (1725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cf53f1325a00115717e22a2ad400917ea970c2863a9f0aa384c81111fe5f754`  
		Last Modified: Wed, 01 Nov 2023 06:53:16 GMT  
		Size: 1.5 KB (1481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fb917f0d920d8d2969e5b26d77d9384c94934f2c5d72677b658a9483e180240`  
		Last Modified: Wed, 01 Nov 2023 06:53:17 GMT  
		Size: 1.4 MB (1387222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af14639f108dd10f1d2bd5ea098b67c59009583ed8e393315c464ec4223e37d8`  
		Last Modified: Wed, 01 Nov 2023 06:53:16 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:standalone` - linux; ppc64le

```console
$ docker pull adminer@sha256:489934d719089bd1c3827bdf673dcf7636376fbcbcfe837c4b7fa275ba366b62
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.3 MB (101265232 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6176ac38dfe8ab4e16662cc637ab4fb4b6f98c2e489cf4b4e6a66d578229ac6a`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Wed, 01 Nov 2023 02:50:13 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 01 Nov 2023 02:50:15 GMT
WORKDIR /var/www/html
# Wed, 01 Nov 2023 02:50:15 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 01 Nov 2023 02:50:15 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 01 Nov 2023 02:50:16 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 01 Nov 2023 02:50:16 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 01 Nov 2023 02:50:41 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 01 Nov 2023 02:50:42 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 01 Nov 2023 02:50:42 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 01 Nov 2023 02:50:43 GMT
USER adminer
# Wed, 01 Nov 2023 02:50:43 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 01 Nov 2023 02:50:44 GMT
EXPOSE 8080
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
	-	`sha256:c949ba7225949db3835c8321c7fd3fc61042abadd084780530933f2490a389ac`  
		Last Modified: Wed, 01 Nov 2023 02:51:40 GMT  
		Size: 1.9 KB (1878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69b23613e6440faf4dd53e85cce3379a37d371a55de8c3711313d4e8c2bdfcc7`  
		Last Modified: Wed, 01 Nov 2023 02:51:41 GMT  
		Size: 1.5 KB (1480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7424b8a43895b887591228e0a253d09fc56191f47ab5b4ab56d6fac2e6cbd9af`  
		Last Modified: Wed, 01 Nov 2023 02:51:41 GMT  
		Size: 1.4 MB (1386466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ee20cb0c3714aa128b4be5cdf5911002f2596f04b95e7e03962e22f45920bd3`  
		Last Modified: Wed, 01 Nov 2023 02:51:40 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:standalone` - linux; s390x

```console
$ docker pull adminer@sha256:febeaf64eb35379728a191c91b4c0fd744f0f25716db5b3a6383382bd813875b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.7 MB (93708845 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f56dc24645f9175629077bc05d2d1ef72a10391d530b75320409f480c64d72b5`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Wed, 01 Nov 2023 01:50:10 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 01 Nov 2023 01:50:10 GMT
WORKDIR /var/www/html
# Wed, 01 Nov 2023 01:50:10 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 01 Nov 2023 01:50:10 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 01 Nov 2023 01:50:10 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 01 Nov 2023 01:50:10 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 01 Nov 2023 01:50:18 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 01 Nov 2023 01:50:18 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 01 Nov 2023 01:50:18 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 01 Nov 2023 01:50:18 GMT
USER adminer
# Wed, 01 Nov 2023 01:50:18 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 01 Nov 2023 01:50:19 GMT
EXPOSE 8080
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
	-	`sha256:0ddb015dd3525d29ecb468826e1900bd5a42aedf948d046cf67cbb849116174a`  
		Last Modified: Wed, 01 Nov 2023 01:50:54 GMT  
		Size: 1.9 KB (1879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eeda1242b7f2fccc214b7bce16debf257837f0e99de553d8b0899289fdf4381`  
		Last Modified: Wed, 01 Nov 2023 01:50:54 GMT  
		Size: 1.5 KB (1477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b79f82c6e4dc3c8fa378683a146466b55a41e4a9b35103811abe39ff47528f4`  
		Last Modified: Wed, 01 Nov 2023 01:50:55 GMT  
		Size: 1.4 MB (1386366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:245a8a7cccf20a91e5d673ee924ca9853c1d060c66fdb377e8b8ca63166ac4cc`  
		Last Modified: Wed, 01 Nov 2023 01:50:54 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
