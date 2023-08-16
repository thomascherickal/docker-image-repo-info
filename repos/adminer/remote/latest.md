## `adminer:latest`

```console
$ docker pull adminer@sha256:5bdaf4ee42746c5c99090a1a660f00d5cd78f17661ba526a9edd214dac8f8112
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
$ docker pull adminer@sha256:9425248036f84c766be7ad564108fb92efe3d5744965dcfccf4b3a620461c2c1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.9 MB (95934004 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f95e22ea33363f920444f99f0d5821865efafa5e585ef3d1324f8e7d1845c2e`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 16 Aug 2023 00:59:57 GMT
ADD file:20f89ff93bfbd6c9fb1a97058a1f3de4485a8974e8a83892072c511fbd2e4134 in / 
# Wed, 16 Aug 2023 00:59:58 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 06:53:20 GMT
STOPSIGNAL SIGINT
# Wed, 16 Aug 2023 06:53:39 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 06:53:40 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 16 Aug 2023 06:53:41 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 16 Aug 2023 06:53:41 GMT
WORKDIR /var/www/html
# Wed, 16 Aug 2023 06:53:41 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 16 Aug 2023 06:53:41 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 16 Aug 2023 06:53:41 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 16 Aug 2023 06:53:41 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 16 Aug 2023 06:53:52 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 16 Aug 2023 06:53:52 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 16 Aug 2023 06:53:52 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 16 Aug 2023 06:53:52 GMT
USER adminer
# Wed, 16 Aug 2023 06:53:52 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 16 Aug 2023 06:53:52 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:6a70103cc499a199e10e379794c60aa524d9598587cc2bdfe2995642c2da8df7`  
		Last Modified: Wed, 16 Aug 2023 01:04:50 GMT  
		Size: 55.1 MB (55056621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf8a57c267c9896b9b3a23126904b5afa97725963cd737515552f4f0382f0fb8`  
		Last Modified: Wed, 16 Aug 2023 06:54:33 GMT  
		Size: 39.5 MB (39487700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b06d2d5387c889ac3907b3b914ba88ef244281459b91f585f182651fe071988`  
		Last Modified: Wed, 16 Aug 2023 06:54:25 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f454e9d758af3cab52e296b29b4b2834a02b1068634c628ed818e7a2a0262f1`  
		Last Modified: Wed, 16 Aug 2023 06:54:25 GMT  
		Size: 1.9 KB (1878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76584d0b042e10b1a4377b5b5383b0e2de3acd6e210aa5995e0c1316c3494a27`  
		Last Modified: Wed, 16 Aug 2023 06:54:25 GMT  
		Size: 1.5 KB (1482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94811d9090123101027253a2c9c8cd707849e7a3172541a3047b08e43642a71b`  
		Last Modified: Wed, 16 Aug 2023 06:54:26 GMT  
		Size: 1.4 MB (1385444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79906cbc9e7cf2bcf86c91d2fb9a4c4c1765d07298ae8e8cf92b2a7b283d21a7`  
		Last Modified: Wed, 16 Aug 2023 06:54:25 GMT  
		Size: 489.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:latest` - linux; arm variant v5

```console
$ docker pull adminer@sha256:af5badffa86e9c336396019f12d013465f5dbd9c8278aaa1604f78d69ce590ee
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.2 MB (91195737 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bed132a0fc8bb7ca878cf1d94ddfc31902e58f3e494f5e837b61cbd725af3105`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Wed, 16 Aug 2023 00:50:46 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 16 Aug 2023 00:50:46 GMT
WORKDIR /var/www/html
# Wed, 16 Aug 2023 00:50:46 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 16 Aug 2023 00:50:46 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 16 Aug 2023 00:50:46 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 16 Aug 2023 00:50:46 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 16 Aug 2023 00:51:01 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 16 Aug 2023 00:51:01 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 16 Aug 2023 00:51:01 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 16 Aug 2023 00:51:01 GMT
USER adminer
# Wed, 16 Aug 2023 00:51:01 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 16 Aug 2023 00:51:01 GMT
EXPOSE 8080
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
	-	`sha256:d2e8b5522694d8b0cc1d26eec03ac2f2f97ff57d7f3e9056358d86b1d4b1a6b3`  
		Last Modified: Wed, 16 Aug 2023 00:51:31 GMT  
		Size: 1.9 KB (1874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1905db25ca9335b07bf248a97ffc1d0cd746030a8833f0aa7c276c21fae5a31`  
		Last Modified: Wed, 16 Aug 2023 00:51:31 GMT  
		Size: 1.5 KB (1477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a3bd225c7201b09ef66598154ae9aa6fbc5b03eb1e143e1b3da8e48a776d928`  
		Last Modified: Wed, 16 Aug 2023 00:51:32 GMT  
		Size: 1.4 MB (1385333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52be3c490603e9c865e303bdb12043abf070af90b245bc1b2188218ef6ea13fb`  
		Last Modified: Wed, 16 Aug 2023 00:51:31 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:latest` - linux; arm variant v7

```console
$ docker pull adminer@sha256:4f9929fcc96d3097f039ee1bd96cbb742a475a5fcf0ef0f2ff216dd1f3a177aa
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.8 MB (87792405 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:618065af60d5a1e01d21ece740f51cbd5d559d52bc3a16643a30b168a909dd3f`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 16 Aug 2023 00:17:21 GMT
ADD file:b529de8b48c1e507ad6f29320c3c5cd83d8d06fa66e8d89bb62faff62700e9f2 in / 
# Wed, 16 Aug 2023 00:17:22 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 05:26:21 GMT
STOPSIGNAL SIGINT
# Wed, 16 Aug 2023 05:26:42 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 05:26:43 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 16 Aug 2023 05:26:43 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 16 Aug 2023 05:26:44 GMT
WORKDIR /var/www/html
# Wed, 16 Aug 2023 05:26:44 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 16 Aug 2023 05:26:44 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 16 Aug 2023 05:26:44 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 16 Aug 2023 05:26:44 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 16 Aug 2023 05:26:55 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 16 Aug 2023 05:26:56 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 16 Aug 2023 05:26:56 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 16 Aug 2023 05:26:56 GMT
USER adminer
# Wed, 16 Aug 2023 05:26:56 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 16 Aug 2023 05:26:56 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:c53151c23650f086e15d3652b8a931fb4623765c0112e8adc74eb8853c8c9232`  
		Last Modified: Wed, 16 Aug 2023 00:21:46 GMT  
		Size: 50.2 MB (50219496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a3ff56cbb8ed6634a40dd277c6c79d73fda021e6eb6dbc64474e489dd6a2254`  
		Last Modified: Wed, 16 Aug 2023 05:27:35 GMT  
		Size: 36.2 MB (36183315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b68c9a798032d63f0755e95cb7d996b79a46ce83104723afb7d8b720ecc37b0d`  
		Last Modified: Wed, 16 Aug 2023 05:27:27 GMT  
		Size: 386.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf6401f5c7d3150ce0ff19cafcbdbebd9896fed4bb0b7cc1586a21e1e57c3dd4`  
		Last Modified: Wed, 16 Aug 2023 05:27:27 GMT  
		Size: 1.9 KB (1870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d384349da1f667ec25a5ae8a7fa18c12fab48e6a045ab7979cbec310051a2e6d`  
		Last Modified: Wed, 16 Aug 2023 05:27:27 GMT  
		Size: 1.5 KB (1483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9036faca944c792cb03a1e45f876fc1ebd681d4495016eba91f0e6954ee5e86d`  
		Last Modified: Wed, 16 Aug 2023 05:27:27 GMT  
		Size: 1.4 MB (1385364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45adeb75fd04efcf491df34c12a1c5a973ecdfecc9e5612497b2ff01b30e8b98`  
		Last Modified: Wed, 16 Aug 2023 05:27:27 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:latest` - linux; arm64 variant v8

```console
$ docker pull adminer@sha256:9af34f1f23a0f4545e9c8a8c25b96f752722ccba2f4009884b342c6abc821cfd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.3 MB (94337581 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ceaf57ddeaa0bc790c02948c5b1496cfb51217e6f7a736329cea0d9b6bf68657`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Tue, 15 Aug 2023 23:40:03 GMT
ADD file:8973cddb2d84a543b71001635599951bea6485a3526ae4ff916443b584864c83 in / 
# Tue, 15 Aug 2023 23:40:04 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:18:33 GMT
STOPSIGNAL SIGINT
# Wed, 16 Aug 2023 01:18:50 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:18:51 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 16 Aug 2023 01:18:51 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 16 Aug 2023 01:18:51 GMT
WORKDIR /var/www/html
# Wed, 16 Aug 2023 01:18:51 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 16 Aug 2023 01:18:51 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 16 Aug 2023 01:18:51 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 16 Aug 2023 01:18:52 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 16 Aug 2023 01:19:01 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 16 Aug 2023 01:19:01 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 16 Aug 2023 01:19:01 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 16 Aug 2023 01:19:01 GMT
USER adminer
# Wed, 16 Aug 2023 01:19:01 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 16 Aug 2023 01:19:01 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:e837d9f05c625de5b814b851adbc03559ba02ea7078f57c81a01e18fc65bf42b`  
		Last Modified: Tue, 15 Aug 2023 23:43:37 GMT  
		Size: 53.7 MB (53704779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ff6bad57ecba5e0579dd6bd721667f3324e23a3ac5b9bc982bd0dc37a0aac41`  
		Last Modified: Wed, 16 Aug 2023 01:19:36 GMT  
		Size: 39.2 MB (39243216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:973b3c539dd5c8609744bf1dfcf0263ed819d43d42b1c7f966a7061631d16973`  
		Last Modified: Wed, 16 Aug 2023 01:19:29 GMT  
		Size: 386.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35373a7e6f06f9c65bd009346d157ef68551477b1e8e69ee02b327b758410fd3`  
		Last Modified: Wed, 16 Aug 2023 01:19:29 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79f0e4e65576bf9748b2afc91c98f1c8a3b329fe242ebbb4121fd0bb35330384`  
		Last Modified: Wed, 16 Aug 2023 01:19:29 GMT  
		Size: 1.5 KB (1478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:287a444e72e39e2823868a7ea5000b6bb3ea13793adab1f8e6bb510b275a78e3`  
		Last Modified: Wed, 16 Aug 2023 01:19:30 GMT  
		Size: 1.4 MB (1385347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df6ddf076b8c62e818266a757bfb81507ec9a219fecf5c0bb790419e67d9b982`  
		Last Modified: Wed, 16 Aug 2023 01:19:29 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:latest` - linux; 386

```console
$ docker pull adminer@sha256:664fc6a11ece4d60a18492c17eeb4ffffb3d6fe19d3c4f4c4c3cab52b83f3ec6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.0 MB (96988434 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d7ecc3592e5ee3a2de07572724acd9167630fa736fd16b373959b3f5e2297736`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Wed, 16 Aug 2023 00:24:05 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 16 Aug 2023 00:24:05 GMT
WORKDIR /var/www/html
# Wed, 16 Aug 2023 00:24:05 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 16 Aug 2023 00:24:05 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 16 Aug 2023 00:24:05 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 16 Aug 2023 00:24:05 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 16 Aug 2023 00:24:19 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 16 Aug 2023 00:24:19 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 16 Aug 2023 00:24:19 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 16 Aug 2023 00:24:19 GMT
USER adminer
# Wed, 16 Aug 2023 00:24:19 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 16 Aug 2023 00:24:19 GMT
EXPOSE 8080
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
	-	`sha256:5339c86a7bc7031718f83f0a9af19ad028c2fa751748057f9d97d9c94c5075f6`  
		Last Modified: Wed, 16 Aug 2023 00:24:50 GMT  
		Size: 1.9 KB (1868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cbd1ad590a03bbc3ee08a1c944135c7bf81b103067417f79cdb1f8d271b4472`  
		Last Modified: Wed, 16 Aug 2023 00:24:50 GMT  
		Size: 1.5 KB (1480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:225fb2c801a3d35820604ab9c5d6c19a65e18fca4c76dd468e7015b6cb7d5d6c`  
		Last Modified: Wed, 16 Aug 2023 00:24:50 GMT  
		Size: 1.4 MB (1385258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:367f82cd1a3d30bffd1420e0c950c92f859f903ad0b0711848862db96f363ff7`  
		Last Modified: Wed, 16 Aug 2023 00:24:50 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:latest` - linux; mips64le

```console
$ docker pull adminer@sha256:a29c69364f1ac112624f371b0f557513ae4343bde1370f0a761199bdaed2cc7f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.6 MB (92615202 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d777757b9212c5b1ffde973161ffce343ff7c18fb6aa28e064f1388788651aee`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Fri, 28 Jul 2023 13:57:43 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Fri, 28 Jul 2023 13:57:46 GMT
WORKDIR /var/www/html
# Fri, 28 Jul 2023 13:57:50 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Fri, 28 Jul 2023 13:57:53 GMT
ENV ADMINER_VERSION=4.8.1
# Fri, 28 Jul 2023 13:57:56 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Fri, 28 Jul 2023 13:58:00 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Fri, 28 Jul 2023 13:58:50 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Fri, 28 Jul 2023 13:58:53 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Fri, 28 Jul 2023 13:58:56 GMT
ENTRYPOINT ["entrypoint.sh"]
# Fri, 28 Jul 2023 13:59:00 GMT
USER adminer
# Fri, 28 Jul 2023 13:59:03 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Fri, 28 Jul 2023 13:59:07 GMT
EXPOSE 8080
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
	-	`sha256:2c079d4f59d959d3b52679deb70efd87f85ac9f13d2960bfac20429dc12ccb6f`  
		Last Modified: Fri, 28 Jul 2023 14:01:10 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b253457b64ca74b828a87f38122bb4b14f19bc299543c82ee702f99cbe5cfe8`  
		Last Modified: Fri, 28 Jul 2023 14:01:10 GMT  
		Size: 1.5 KB (1480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dce220f8fa5d2ceaf1a3470bb9fdfa63c06011270b54b0f8f902bf9c5db753ae`  
		Last Modified: Fri, 28 Jul 2023 14:01:11 GMT  
		Size: 1.4 MB (1386302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:277394a64fd570b76e5484b451d1fc51bf49249846ea3ec3b800f22326304abb`  
		Last Modified: Fri, 28 Jul 2023 14:01:10 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:latest` - linux; ppc64le

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

### `adminer:latest` - linux; s390x

```console
$ docker pull adminer@sha256:997fd11205399ec69d65bfa3ef3cf8a2bcc2441faf87952793b2ff4bb101eefc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.7 MB (93698928 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4455f8d9fa281f3bb6c42caa6bc664e1bc6d42fdd2d336775a0fc5aa31ad0583`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

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
# Wed, 16 Aug 2023 00:47:31 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 16 Aug 2023 00:47:31 GMT
WORKDIR /var/www/html
# Wed, 16 Aug 2023 00:47:31 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 16 Aug 2023 00:47:31 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 16 Aug 2023 00:47:32 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 16 Aug 2023 00:47:32 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 16 Aug 2023 00:47:41 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 16 Aug 2023 00:47:41 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 16 Aug 2023 00:47:41 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 16 Aug 2023 00:47:41 GMT
USER adminer
# Wed, 16 Aug 2023 00:47:41 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 16 Aug 2023 00:47:42 GMT
EXPOSE 8080
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
	-	`sha256:e87458774af67be669151057c3b428a6b7ea6303c2425dc18643c162942ff809`  
		Last Modified: Wed, 16 Aug 2023 00:48:25 GMT  
		Size: 1.9 KB (1877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eab1a52c0a0fcb42d6249cd58409d589a25f54af523d0f0d398b110f68eb136a`  
		Last Modified: Wed, 16 Aug 2023 00:48:26 GMT  
		Size: 1.5 KB (1477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ddcb8f0c7a74ae5f0a74a5400a653342e2830e9fcd5f7add9c5ed8bb9025f97`  
		Last Modified: Wed, 16 Aug 2023 00:48:26 GMT  
		Size: 1.4 MB (1385448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b058febc5c6ae7970e1309f95d79319a73b4f7dffee134bc9bf12659f45e27f`  
		Last Modified: Wed, 16 Aug 2023 00:48:25 GMT  
		Size: 489.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
