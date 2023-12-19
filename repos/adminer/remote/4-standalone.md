## `adminer:4-standalone`

```console
$ docker pull adminer@sha256:6c67673feeb79c1708ab15a8fbc527b88f591aac900ba0f060937f5dc116ce12
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
$ docker pull adminer@sha256:1e11a196781b6e587eebff87d17c27831956cce283d98e48a667d7282144fdd8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.9 MB (95941930 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8485d1424e611494d30993c6426bdb2609d1f7b4b530920b7dd7a7154b7490a3`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Tue, 19 Dec 2023 01:20:38 GMT
ADD file:d3a2f1f42338ba7066e352cea3b7bf4c7576e6b96fef785e8da763114f337c0e in / 
# Tue, 19 Dec 2023 01:20:38 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 04:28:09 GMT
STOPSIGNAL SIGINT
# Tue, 19 Dec 2023 04:28:30 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 04:28:31 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 19 Dec 2023 04:28:32 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 19 Dec 2023 04:28:32 GMT
WORKDIR /var/www/html
# Tue, 19 Dec 2023 04:28:32 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 19 Dec 2023 04:28:32 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 19 Dec 2023 04:28:32 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 19 Dec 2023 04:28:32 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 19 Dec 2023 04:28:44 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 19 Dec 2023 04:28:44 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 19 Dec 2023 04:28:45 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 19 Dec 2023 04:28:45 GMT
USER adminer
# Tue, 19 Dec 2023 04:28:45 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Tue, 19 Dec 2023 04:28:45 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:18f2c3b7ca52caba205d748b9ce41784eb010ca83ece9e84e2a09130a5ec3cbc`  
		Last Modified: Tue, 19 Dec 2023 01:25:17 GMT  
		Size: 55.1 MB (55057340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bad63e83ac4c7f1414e4ccf6b362fac0878f822163680267ba24479578ac9401`  
		Last Modified: Tue, 19 Dec 2023 04:29:21 GMT  
		Size: 39.5 MB (39493907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:166c45dad258f94381476c950ee7ef88d72c5fda27a88c3ad91ca7c10521feca`  
		Last Modified: Tue, 19 Dec 2023 04:29:14 GMT  
		Size: 389.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68b27bedb41b2ab18240fe6c7340627c45c086fdbf2cfd47dc3ac8b29aca66aa`  
		Last Modified: Tue, 19 Dec 2023 04:29:14 GMT  
		Size: 1.9 KB (1877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:731df483e3ef3d520887ccb30bde62423f0ac2050f05e66ecd48be414a11a44f`  
		Last Modified: Tue, 19 Dec 2023 04:29:14 GMT  
		Size: 1.5 KB (1476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13b2794b03eb00fa03fd4c11b02eedff5efb0f7377dd14d4a00102cd7ad0bca3`  
		Last Modified: Tue, 19 Dec 2023 04:29:14 GMT  
		Size: 1.4 MB (1386450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6ebbba76d2ece99e6d7a27de40258e36164a7e96018a7e8eaf8c4bd4e03ed2b`  
		Last Modified: Tue, 19 Dec 2023 04:29:14 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-standalone` - linux; arm variant v5

```console
$ docker pull adminer@sha256:4810ea72abb576d9555e124b94a485aceaa97c6dbd22a0ae118af99233a3aba2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.2 MB (91205413 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b884d4d284b14c7f34bdb3a9c78d2ea68a57a0c1989a5ec0c501fb26006cf53`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Tue, 19 Dec 2023 01:55:29 GMT
ADD file:10a67a16f03367965d9105db3d368f8cf27493769f1551c2bfdc274485bd7f6d in / 
# Tue, 19 Dec 2023 01:55:30 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 05:19:19 GMT
STOPSIGNAL SIGINT
# Tue, 19 Dec 2023 05:19:48 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 05:19:49 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 19 Dec 2023 05:19:50 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 19 Dec 2023 05:19:50 GMT
WORKDIR /var/www/html
# Tue, 19 Dec 2023 05:19:50 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 19 Dec 2023 05:19:50 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 19 Dec 2023 05:19:50 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 19 Dec 2023 05:19:50 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 19 Dec 2023 05:20:04 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 19 Dec 2023 05:20:05 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 19 Dec 2023 05:20:05 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 19 Dec 2023 05:20:05 GMT
USER adminer
# Tue, 19 Dec 2023 05:20:05 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Tue, 19 Dec 2023 05:20:05 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:476954b0dbc0bbf3e36983f98ae01dfefa01670a85ffcb7ed6916095b71bdd38`  
		Last Modified: Tue, 19 Dec 2023 01:58:55 GMT  
		Size: 52.6 MB (52562242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e44cc4eabb8ab5cb58a1f898eb13f385aed7944d04795cc8f88496258b490372`  
		Last Modified: Tue, 19 Dec 2023 05:20:44 GMT  
		Size: 37.3 MB (37252666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10250a7e9e6e5bf39a628a4d1b5d5bfade40db8d12fcdff38e7f70451f7b90af`  
		Last Modified: Tue, 19 Dec 2023 05:20:34 GMT  
		Size: 389.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c779bed6a14ab54afc6969b0113cb9ded0c22ab9abcd969a440c926d2723d7bf`  
		Last Modified: Tue, 19 Dec 2023 05:20:34 GMT  
		Size: 1.9 KB (1874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bd026fe62c3edf45d7f23f182ce375834f313f60253a1e9e07fbf71a254de08`  
		Last Modified: Tue, 19 Dec 2023 05:20:34 GMT  
		Size: 1.5 KB (1477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eb01e600b0d30f7e442d2f828ece0dece790f9aa23c931039d480b6a28e34ca`  
		Last Modified: Tue, 19 Dec 2023 05:20:35 GMT  
		Size: 1.4 MB (1386272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94b0a7a3d4085fe90602f3e706f1059c77cccbc92cfb9db2464527cfcdf7cb78`  
		Last Modified: Tue, 19 Dec 2023 05:20:34 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-standalone` - linux; arm variant v7

```console
$ docker pull adminer@sha256:8940872f96b0f7cf5ce87d55458ae6ffb3731f524ad4063ff432d590b5e82dcc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.8 MB (87797415 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75593297f9c2dc4f473d1eb9060245794085eeb5b31e249c5aab20df2f582497`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Tue, 19 Dec 2023 02:07:59 GMT
ADD file:3b623bed8ec2536cb513edda1de6f79d2c8e06d6f82df2543202544dbba3ae3e in / 
# Tue, 19 Dec 2023 02:08:00 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 08:23:04 GMT
STOPSIGNAL SIGINT
# Tue, 19 Dec 2023 08:23:36 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 08:23:37 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 19 Dec 2023 08:23:37 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 19 Dec 2023 08:23:38 GMT
WORKDIR /var/www/html
# Tue, 19 Dec 2023 08:23:38 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 19 Dec 2023 08:23:38 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 19 Dec 2023 08:23:38 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 19 Dec 2023 08:23:38 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 19 Dec 2023 08:23:49 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 19 Dec 2023 08:23:49 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 19 Dec 2023 08:23:49 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 19 Dec 2023 08:23:49 GMT
USER adminer
# Tue, 19 Dec 2023 08:23:50 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Tue, 19 Dec 2023 08:23:50 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:1b42212018867046767b36eb95cf15c4b66bbb7b4fb552aab446d9822de5765c`  
		Last Modified: Tue, 19 Dec 2023 02:12:11 GMT  
		Size: 50.2 MB (50215775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4af1df80133b5abe2a3bdb18a519e0d9a46ff65f6d03be8112f7f5d17bbf258f`  
		Last Modified: Tue, 19 Dec 2023 08:24:25 GMT  
		Size: 36.2 MB (36191039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5512945806d39a0f111223c3d619a80e6f2d05ee09e6303ba271d6d978eda49`  
		Last Modified: Tue, 19 Dec 2023 08:24:16 GMT  
		Size: 391.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f417b1e1ebc7b26c159030a5f67ee3ca232cc9925cbb108e09b12c00acef290`  
		Last Modified: Tue, 19 Dec 2023 08:24:16 GMT  
		Size: 1.9 KB (1871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d541735c4435d0cdb7b31df534048ef0e3deee7ca38c09e72309c038a83c0797`  
		Last Modified: Tue, 19 Dec 2023 08:24:16 GMT  
		Size: 1.5 KB (1482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a21eb56fec41f7eea57361dbcd54761286b95d1609abb8a79308653d5a4a55ae`  
		Last Modified: Tue, 19 Dec 2023 08:24:16 GMT  
		Size: 1.4 MB (1386363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38393cf6a9a2fa889f7742fd6dd598ce2d0bc7e9662898ae948c1805a751c5ac`  
		Last Modified: Tue, 19 Dec 2023 08:24:16 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-standalone` - linux; arm64 variant v8

```console
$ docker pull adminer@sha256:3cc8c9bcd9de764e88c912cd7a7834eb817a4fd90ba833a29bb1adc54081a5f1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.3 MB (94346551 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cff0a470993d19168a4e619c0ae1ddbee9f0c234917aaea8aa261d97a9e9526b`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Tue, 19 Dec 2023 01:41:17 GMT
ADD file:06ba7e39a2f8e1a7bcbb929fa9d1e6fb1f8bdcf5096dc903576af8f7014e353b in / 
# Tue, 19 Dec 2023 01:41:18 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 06:49:50 GMT
STOPSIGNAL SIGINT
# Tue, 19 Dec 2023 06:50:08 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 06:50:09 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 19 Dec 2023 06:50:10 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 19 Dec 2023 06:50:10 GMT
WORKDIR /var/www/html
# Tue, 19 Dec 2023 06:50:10 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 19 Dec 2023 06:50:10 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 19 Dec 2023 06:50:10 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 19 Dec 2023 06:50:10 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 19 Dec 2023 06:50:20 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 19 Dec 2023 06:50:20 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 19 Dec 2023 06:50:20 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 19 Dec 2023 06:50:21 GMT
USER adminer
# Tue, 19 Dec 2023 06:50:21 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Tue, 19 Dec 2023 06:50:21 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:396a672fee8bade1a7c9f228d919717447f110f39046d8b5ed21ad45ae13ab61`  
		Last Modified: Tue, 19 Dec 2023 01:44:57 GMT  
		Size: 53.7 MB (53708091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5ed26c5188b9e4a04138b32bfd04e17c836f5b1efc61588c60d5bc52345a16c`  
		Last Modified: Tue, 19 Dec 2023 06:50:51 GMT  
		Size: 39.2 MB (39247941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3fe407ff0bf13ebf2f07e204841637120d4ecbcad377fd08216b87b29881b08`  
		Last Modified: Tue, 19 Dec 2023 06:50:44 GMT  
		Size: 393.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17acd802459e90d9c37fb4de9ac35c3a36ef626a87e1c47a8832b652846c9a56`  
		Last Modified: Tue, 19 Dec 2023 06:50:44 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c26177b8067c3b3a7275ddb52478d09f92b8a08da0a4cd637325058ca301d660`  
		Last Modified: Tue, 19 Dec 2023 06:50:44 GMT  
		Size: 1.5 KB (1476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e3d8592ee5cfa7a68558fd4c5935dfbf3f424a32a4865eab630d0e4583d0713`  
		Last Modified: Tue, 19 Dec 2023 06:50:45 GMT  
		Size: 1.4 MB (1386279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0c892659cb453676dc0f09c3a85aa933decf1723a747909b9e0a4c16bc24f66`  
		Last Modified: Tue, 19 Dec 2023 06:50:44 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-standalone` - linux; 386

```console
$ docker pull adminer@sha256:e1929fdf5439f8774f2d77c56c3944c0aa08c2311ba9edb906437a621d4ae568
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.0 MB (96999008 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:177e1fd602f84f811f29edb98beb4deee04dc4894db58cc40cdeb7dadf4f793c`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Tue, 19 Dec 2023 01:39:19 GMT
ADD file:8a328fced7ae3a6fc868bbb95c23191103e595c9d22b2626c16f155bc48b51a8 in / 
# Tue, 19 Dec 2023 01:39:20 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 03:22:24 GMT
STOPSIGNAL SIGINT
# Tue, 19 Dec 2023 03:22:52 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 03:22:53 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 19 Dec 2023 03:22:53 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 19 Dec 2023 03:22:53 GMT
WORKDIR /var/www/html
# Tue, 19 Dec 2023 03:22:53 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 19 Dec 2023 03:22:54 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 19 Dec 2023 03:22:54 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 19 Dec 2023 03:22:54 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 19 Dec 2023 03:23:07 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 19 Dec 2023 03:23:07 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 19 Dec 2023 03:23:07 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 19 Dec 2023 03:23:08 GMT
USER adminer
# Tue, 19 Dec 2023 03:23:08 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Tue, 19 Dec 2023 03:23:08 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:a789657fd5416b1ccfd519597a8f5e57bd5a80d04d1b1b7b2770df4469f4dd44`  
		Last Modified: Tue, 19 Dec 2023 01:44:07 GMT  
		Size: 56.0 MB (56046336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:036f0911d89d9e328491b83337936442eb0490afd3a8124ae61ff283dcef35f8`  
		Last Modified: Tue, 19 Dec 2023 03:23:51 GMT  
		Size: 39.6 MB (39562137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f22576bb4fcebae9c7f3032c0595103daa8f7aca1cc64ad6afe41b296d7e49b`  
		Last Modified: Tue, 19 Dec 2023 03:23:39 GMT  
		Size: 388.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6e01495f57284f740e52aca3ba0d4a049ad0549bfa13077d0a696561283fd85`  
		Last Modified: Tue, 19 Dec 2023 03:23:39 GMT  
		Size: 1.9 KB (1872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:828b47c4bd237c6bc6fdcd53678bd6cb1c598cf85434c9c96c8a7823ea01401d`  
		Last Modified: Tue, 19 Dec 2023 03:23:39 GMT  
		Size: 1.5 KB (1479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1059ba7a0b504b0be641cfe6e50efaaa46bed12d4cb6d8f27fea6b790e4eb903`  
		Last Modified: Tue, 19 Dec 2023 03:23:40 GMT  
		Size: 1.4 MB (1386303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26b98e582eac18f55fc9bb20b0c898dcd324e080bd945ca91a97f424e6c21858`  
		Last Modified: Tue, 19 Dec 2023 03:23:39 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-standalone` - linux; mips64le

```console
$ docker pull adminer@sha256:84b1c19875f37b42946db21b87c80b8f8d9d9c7392eff0a7a065cf6d5fe769b2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.6 MB (92634921 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6454361a51d8f0d5781cd1854359c6b0812cc29466f516dd6386754b3583699`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Tue, 21 Nov 2023 04:10:25 GMT
ADD file:dbfc3d226166089c4db0c154fdcea8049b8758c6812f1c397dec1444985e8557 in / 
# Tue, 21 Nov 2023 04:10:31 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 12:14:44 GMT
STOPSIGNAL SIGINT
# Tue, 21 Nov 2023 12:16:43 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 12:16:50 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 21 Nov 2023 12:16:57 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 21 Nov 2023 12:17:00 GMT
WORKDIR /var/www/html
# Tue, 21 Nov 2023 12:17:04 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 21 Nov 2023 12:17:07 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 21 Nov 2023 12:17:10 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 21 Nov 2023 12:17:14 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 21 Nov 2023 12:18:08 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 21 Nov 2023 12:18:11 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 21 Nov 2023 12:18:14 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 21 Nov 2023 12:18:17 GMT
USER adminer
# Tue, 21 Nov 2023 12:18:21 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Tue, 21 Nov 2023 12:18:24 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:ca31218601e95f4aafae0dcadda7600aeb04db374e1e829d5c123f8033ba3472`  
		Last Modified: Tue, 21 Nov 2023 04:21:21 GMT  
		Size: 53.3 MB (53289162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d172a1ce4463b8a1bb14b88d9f7c98a7f06f260dfc2849e77f3d41be6d17db9`  
		Last Modified: Tue, 21 Nov 2023 12:21:00 GMT  
		Size: 38.0 MB (37954467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbd3b039fbc0efa77466cfb045c80c120d45355cf2db0dd6533eeb1cee6296e1`  
		Last Modified: Tue, 21 Nov 2023 12:20:33 GMT  
		Size: 394.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bac97c667ed055993103f32b019a430a853a94eef6bf75086fda9949a9fd1d8`  
		Last Modified: Tue, 21 Nov 2023 12:20:34 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66eec20186701717a98146a63c5c8f88304d44243fe6f6505edf4d1135672446`  
		Last Modified: Tue, 21 Nov 2023 12:20:34 GMT  
		Size: 1.5 KB (1483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a56ddb348b2b13a6cac73829460bdcce2971790b6be59ac9da70b739453488b8`  
		Last Modified: Tue, 21 Nov 2023 12:20:34 GMT  
		Size: 1.4 MB (1387192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f922348b25af66b56cdd7a4863a9a120057afa01489fc9058cf7e975b198d05`  
		Last Modified: Tue, 21 Nov 2023 12:20:34 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-standalone` - linux; ppc64le

```console
$ docker pull adminer@sha256:7e3b01da0a8247f68c860055b22ea7902fb5537ead5dbbb589b5a9ba0cef20f0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.3 MB (101266015 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac5943edc0ff4abb6bd975a653d8bf8afdf7413331b393e8e74d3f13b836706c`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Tue, 19 Dec 2023 01:22:03 GMT
ADD file:240a318dbc8a7ec4b3a6af5afec173d3579c94c27738b0f79750242acce5dd2f in / 
# Tue, 19 Dec 2023 01:22:06 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 11:29:17 GMT
STOPSIGNAL SIGINT
# Tue, 19 Dec 2023 11:30:13 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 11:30:17 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 19 Dec 2023 11:30:18 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 19 Dec 2023 11:30:19 GMT
WORKDIR /var/www/html
# Tue, 19 Dec 2023 11:30:19 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 19 Dec 2023 11:30:20 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 19 Dec 2023 11:30:20 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 19 Dec 2023 11:30:21 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 19 Dec 2023 11:30:45 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 19 Dec 2023 11:30:45 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 19 Dec 2023 11:30:45 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 19 Dec 2023 11:30:46 GMT
USER adminer
# Tue, 19 Dec 2023 11:30:47 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Tue, 19 Dec 2023 11:30:47 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:bdab4f9926bc1dc6c30480616baa760641ee4feeca1b5215d5c420b718c5a1a3`  
		Last Modified: Tue, 19 Dec 2023 01:26:44 GMT  
		Size: 58.9 MB (58929912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4cf89234bdf1920a832942017d9ae3ff7294a0f1f05a9fb3cb67e7b7f733a4e`  
		Last Modified: Tue, 19 Dec 2023 11:31:54 GMT  
		Size: 40.9 MB (40945360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa97daebd213b3ad16d1bd6dbbedf28201b72cbcf0a72e6434fcdd515b1a8503`  
		Last Modified: Tue, 19 Dec 2023 11:31:45 GMT  
		Size: 395.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7207e114fe7ccd8ef1fa89f0bfe4158e08d6eb60118ece3353985cf711266b5`  
		Last Modified: Tue, 19 Dec 2023 11:31:45 GMT  
		Size: 1.9 KB (1878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92228dde13893a9f1c0578816b70fd7ccd69fe35a154ff0b5e5e55e90a9df966`  
		Last Modified: Tue, 19 Dec 2023 11:31:45 GMT  
		Size: 1.5 KB (1482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9672fde51b0787a8334b9ef36e7c2f415f9ec33095a7b7b771e977644a751634`  
		Last Modified: Tue, 19 Dec 2023 11:31:45 GMT  
		Size: 1.4 MB (1386494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd9e56046790c0b173ebcd4b0084317e2af5953e0349d3fb458cc07e0eb351ef`  
		Last Modified: Tue, 19 Dec 2023 11:31:45 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-standalone` - linux; s390x

```console
$ docker pull adminer@sha256:6fc80d10f0998408f5637c9a624191dd169e77371ca49e13b3f7a9df3aedd59e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.7 MB (93708808 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7d5a38491a0a50639c5ace2e633925557360e230867dfb202a84f15fcd74124`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Tue, 19 Dec 2023 01:42:51 GMT
ADD file:f3ff7311d9c8e7c83e0b7746d9402fed156fb05bd0c704d49535b4ece7f33177 in / 
# Tue, 19 Dec 2023 01:42:55 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 08:25:25 GMT
STOPSIGNAL SIGINT
# Tue, 19 Dec 2023 08:25:42 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 08:25:45 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 19 Dec 2023 08:25:45 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 19 Dec 2023 08:25:46 GMT
WORKDIR /var/www/html
# Tue, 19 Dec 2023 08:25:46 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 19 Dec 2023 08:25:46 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 19 Dec 2023 08:25:46 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 19 Dec 2023 08:25:46 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 19 Dec 2023 08:25:54 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 19 Dec 2023 08:25:54 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 19 Dec 2023 08:25:54 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 19 Dec 2023 08:25:54 GMT
USER adminer
# Tue, 19 Dec 2023 08:25:54 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Tue, 19 Dec 2023 08:25:54 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:a7334865824cce0a21e0af9d1f48eaee160e0ac01a54ca220a9814e8d2059646`  
		Last Modified: Tue, 19 Dec 2023 01:47:52 GMT  
		Size: 53.3 MB (53295959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d3db6dd567b86ae988b6977d7df33d24408ada7139b6210b245b6d6464c6158`  
		Last Modified: Tue, 19 Dec 2023 08:26:36 GMT  
		Size: 39.0 MB (39022207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0af1c9faf2e463f5a5ccb69a266a470708823f07bf1ac960f8a0628274872110`  
		Last Modified: Tue, 19 Dec 2023 08:26:29 GMT  
		Size: 395.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9e2680113dcaa0f97a892815ea1faa1b85bc563d9ba06811aae8eede323e60f`  
		Last Modified: Tue, 19 Dec 2023 08:26:29 GMT  
		Size: 1.9 KB (1884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db5083c859302660191bc80008604c4457adc1b369e68009d21560ac49dae4fc`  
		Last Modified: Tue, 19 Dec 2023 08:26:29 GMT  
		Size: 1.5 KB (1481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:065f443fb57166f1cd6177b404995ea6cdddb1a744cf6b2ef8102a077f93fb5b`  
		Last Modified: Tue, 19 Dec 2023 08:26:29 GMT  
		Size: 1.4 MB (1386389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cedb578f2c76e16d38d704a420469cf0e13d757dec887619d539bd5a5c423cd`  
		Last Modified: Tue, 19 Dec 2023 08:26:29 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
