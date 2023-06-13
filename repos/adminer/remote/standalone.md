## `adminer:standalone`

```console
$ docker pull adminer@sha256:bb57616441db7d9bcf04f9e231bf8fd066b209374f0e30384d17988cbb4e889b
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
$ docker pull adminer@sha256:203c8ee52640268c28f5ce5f57b192d967da40a91d6443b57ae1da4064e2ed8b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.9 MB (95931867 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e4345c1c3dc89b4c31146abe340fa39e143d922d1e3401233d7ac32db2d985d`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Mon, 12 Jun 2023 23:20:54 GMT
ADD file:e530b0563ea53d97b2f28e62149a665900196f86611df99a88c7a8ab2097b95d in / 
# Mon, 12 Jun 2023 23:20:54 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 03:24:37 GMT
STOPSIGNAL SIGINT
# Tue, 13 Jun 2023 03:25:04 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 03:25:05 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 13 Jun 2023 03:25:06 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 13 Jun 2023 03:25:06 GMT
WORKDIR /var/www/html
# Tue, 13 Jun 2023 03:25:06 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 13 Jun 2023 03:25:06 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 13 Jun 2023 03:25:06 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 13 Jun 2023 03:25:06 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 13 Jun 2023 03:25:19 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Jun 2023 03:25:19 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 13 Jun 2023 03:25:19 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 13 Jun 2023 03:25:19 GMT
USER adminer
# Tue, 13 Jun 2023 03:25:19 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Tue, 13 Jun 2023 03:25:19 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:93c2d578e4211e82e47e7ada9ed05d1869a2362c6f7509f2ee8d91ccebfb7fbd`  
		Last Modified: Mon, 12 Jun 2023 23:26:08 GMT  
		Size: 55.1 MB (55055162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e099cf7ea37ba8ff2169a70f6743bf40675a661f0dc9b6a8abaa4e43050979c`  
		Last Modified: Tue, 13 Jun 2023 03:25:56 GMT  
		Size: 39.5 MB (39487054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d12c699384cbfa0b30a07efef5ad3b7f104e0e1f33e6a094e489150e4ef3838`  
		Last Modified: Tue, 13 Jun 2023 03:25:48 GMT  
		Size: 391.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05c66113a52b479d99efec54808f4045c5fe1400714639a6c750317ad501bc9c`  
		Last Modified: Tue, 13 Jun 2023 03:25:48 GMT  
		Size: 1.9 KB (1874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:677df7ad2be6c1e9f14d49043358dc765759c7f2cd0184ca55a55dc81dcb2263`  
		Last Modified: Tue, 13 Jun 2023 03:25:48 GMT  
		Size: 1.5 KB (1478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:598f6ab1ce2900168e83fbb661f1edc77e27dd8261b23a1f22af28e991facd6e`  
		Last Modified: Tue, 13 Jun 2023 03:25:49 GMT  
		Size: 1.4 MB (1385416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41ed709cb4bc1b53001ba47d24d74fb415c6142dd35194346fdac370144df45a`  
		Last Modified: Tue, 13 Jun 2023 03:25:48 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:standalone` - linux; arm variant v5

```console
$ docker pull adminer@sha256:e9553c7c6493873a7d8db85d33fda5a59909e3f04b96187cf82d9b31220f69b0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.2 MB (91193892 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01b032634f5c51c674e1250eaf96c978ac50e52552e6a2f878cf760f50c7b8f4`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Mon, 12 Jun 2023 23:48:38 GMT
ADD file:74586d6297f91fb43eb1f367e32039cdb4f30bb86ee4a094d0cba8e0263b1c16 in / 
# Mon, 12 Jun 2023 23:48:39 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 09:24:31 GMT
STOPSIGNAL SIGINT
# Tue, 13 Jun 2023 09:24:59 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 09:25:00 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 13 Jun 2023 09:25:01 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 13 Jun 2023 09:25:01 GMT
WORKDIR /var/www/html
# Tue, 13 Jun 2023 09:25:01 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 13 Jun 2023 09:25:01 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 13 Jun 2023 09:25:01 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 13 Jun 2023 09:25:01 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 13 Jun 2023 09:25:14 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Jun 2023 09:25:15 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 13 Jun 2023 09:25:15 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 13 Jun 2023 09:25:15 GMT
USER adminer
# Tue, 13 Jun 2023 09:25:15 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Tue, 13 Jun 2023 09:25:15 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:6d43c9c52ecc2ee6ecfb5eca6f12c77b0c13f02c1f5b0ca4f7af79eec88842db`  
		Last Modified: Mon, 12 Jun 2023 23:51:44 GMT  
		Size: 52.6 MB (52556725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5110dba9c70245cc37def7ae51a142a8dc22a6a6f551f278ce345f86815708cf`  
		Last Modified: Tue, 13 Jun 2023 09:25:51 GMT  
		Size: 37.2 MB (37247588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86a82b756104b5b2f6d1b1d5b8308da124a6ece770146866df621037b78b1868`  
		Last Modified: Tue, 13 Jun 2023 09:25:43 GMT  
		Size: 391.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:780f1fa84d676ec8213bb36d5fc6dfd91d8409d1f67ee1672da58012cb8f0fe2`  
		Last Modified: Tue, 13 Jun 2023 09:25:43 GMT  
		Size: 1.9 KB (1865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd32666b103cccaac811b4afa9520cb0ddcf9a712a316d1ae1edc213525e6fbb`  
		Last Modified: Tue, 13 Jun 2023 09:25:43 GMT  
		Size: 1.5 KB (1481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3468003f25f868f838adca84760fad26cad9a26af379a2b6d81ce12bb3338fb2`  
		Last Modified: Tue, 13 Jun 2023 09:25:43 GMT  
		Size: 1.4 MB (1385353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deb42466cd70dc773bba31d4b7613262535c9dca8518b1dc90a5df7c8dbd71b0`  
		Last Modified: Tue, 13 Jun 2023 09:25:43 GMT  
		Size: 489.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:standalone` - linux; arm variant v7

```console
$ docker pull adminer@sha256:98b76b0878cf9cc2684e5bbbdade79a5f2f6f269e230203870a1f1a752f7e7f1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.8 MB (87790748 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b51c4364b99328a719594799d5c3d616aeb43a95308f9cd320cb70d27dda4c17`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Mon, 12 Jun 2023 23:58:34 GMT
ADD file:6edc8f94d2ebc83d6081e1c4567963d0060a842c767eaff959a6e5c6d09247b5 in / 
# Mon, 12 Jun 2023 23:58:34 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 04:50:43 GMT
STOPSIGNAL SIGINT
# Tue, 13 Jun 2023 04:51:12 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 04:51:12 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 13 Jun 2023 04:51:13 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 13 Jun 2023 04:51:13 GMT
WORKDIR /var/www/html
# Tue, 13 Jun 2023 04:51:13 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 13 Jun 2023 04:51:13 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 13 Jun 2023 04:51:13 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 13 Jun 2023 04:51:13 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 13 Jun 2023 04:51:41 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Jun 2023 04:51:41 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 13 Jun 2023 04:51:41 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 13 Jun 2023 04:51:41 GMT
USER adminer
# Tue, 13 Jun 2023 04:51:42 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Tue, 13 Jun 2023 04:51:42 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:23807bbf2a5fd14b7975a9e82f4a5530bbba520f31b382cc4b4ce2e77e075ace`  
		Last Modified: Tue, 13 Jun 2023 00:04:02 GMT  
		Size: 50.2 MB (50218141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed9435d7956e105f98b0ce0d774c24da59c523bdcf4ec8fff644876978300c69`  
		Last Modified: Tue, 13 Jun 2023 04:52:24 GMT  
		Size: 36.2 MB (36183011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbf6d7965eb59f39902f271310a767cdf68bdc38bf15c4ee7bc3cfc5c2d025f8`  
		Last Modified: Tue, 13 Jun 2023 04:52:16 GMT  
		Size: 392.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da256b5543040f6999ae9a8cc020bfd0542286ecf71c77feb6cd08a4ecd9be37`  
		Last Modified: Tue, 13 Jun 2023 04:52:16 GMT  
		Size: 1.9 KB (1863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fac8d202305e7ac73502fb63bb1618ac53766c99e8cd03bcb0412c313a25dd83`  
		Last Modified: Tue, 13 Jun 2023 04:52:16 GMT  
		Size: 1.5 KB (1479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b96b3d518c63ab16389a582e075ae88f7225f3c35483203c7c52dcfa52f2daa5`  
		Last Modified: Tue, 13 Jun 2023 04:52:16 GMT  
		Size: 1.4 MB (1385372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eb5818f5b2f148baf53286364c0c6cd2df86e21ed76bfcbc6ff0688a5d2726c`  
		Last Modified: Tue, 13 Jun 2023 04:52:16 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:standalone` - linux; arm64 variant v8

```console
$ docker pull adminer@sha256:92cdfd552b3557e293045fc3d5f01d58871958912197649f3c818e312856bf85
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.3 MB (94336689 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b7e1c530248708005dc78825e6702d078b51bbd4eae6c82b2df135ce82d2961`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:22 GMT
ADD file:caddd2f40296ec5c1bf7487617ca8694cfff9a1d9b7484159e203b6514cb5f5f in / 
# Mon, 12 Jun 2023 23:40:23 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 04:45:49 GMT
STOPSIGNAL SIGINT
# Tue, 13 Jun 2023 04:46:10 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 04:46:11 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 13 Jun 2023 04:46:12 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 13 Jun 2023 04:46:12 GMT
WORKDIR /var/www/html
# Tue, 13 Jun 2023 04:46:12 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 13 Jun 2023 04:46:12 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 13 Jun 2023 04:46:12 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 13 Jun 2023 04:46:12 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 13 Jun 2023 04:46:22 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Jun 2023 04:46:22 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 13 Jun 2023 04:46:22 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 13 Jun 2023 04:46:22 GMT
USER adminer
# Tue, 13 Jun 2023 04:46:22 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Tue, 13 Jun 2023 04:46:23 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:663ccfaf62a5d7b997bca03d1dc6d5dfff01b9e0de08d86dbea8957ea92d7d16`  
		Last Modified: Mon, 12 Jun 2023 23:44:25 GMT  
		Size: 53.7 MB (53704136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80aa39d9a9c198e71855c642bc21b287cd96a68f1ca6f6095933aebd07835b55`  
		Last Modified: Tue, 13 Jun 2023 04:46:57 GMT  
		Size: 39.2 MB (39243014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35aba8c7c961932b274149a03d0e4ded7ce7529e514d523d33c6c6972b149b3d`  
		Last Modified: Tue, 13 Jun 2023 04:46:50 GMT  
		Size: 393.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe596da7a5da4c53bb7e8a57c4bca7d95147969f3fcfa27a9ac63992faacad68`  
		Last Modified: Tue, 13 Jun 2023 04:46:51 GMT  
		Size: 1.9 KB (1875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9f19157c079ccd39ddc0b6c916dec64e367d7b29ff37f7d51348654868ffeea`  
		Last Modified: Tue, 13 Jun 2023 04:46:51 GMT  
		Size: 1.5 KB (1482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e9f6bc36eded234b1a9ca40497b6b08e4a5ebd85b8077cfd4951499ef134c78`  
		Last Modified: Tue, 13 Jun 2023 04:46:51 GMT  
		Size: 1.4 MB (1385300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4689e75de5a00a90b25e2ae66464fad25ea65b849b83d549503bdfb11f72be63`  
		Last Modified: Tue, 13 Jun 2023 04:46:51 GMT  
		Size: 489.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:standalone` - linux; 386

```console
$ docker pull adminer@sha256:e0bb773bce27da86e8bba771ce6fb58fef553b675ea0e0e2c7eaa0d2bd7dd9f9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.0 MB (96988803 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77720ee3233be6352493a8d99e983f977b3e182750f1526bba6d67134b1bf7ee`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Mon, 12 Jun 2023 23:39:39 GMT
ADD file:4b1f447e0b75fbe493bd68bb77b74f4ba1c61ac8e14226e3c511b3a1c3d5721a in / 
# Mon, 12 Jun 2023 23:39:40 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 00:59:39 GMT
STOPSIGNAL SIGINT
# Tue, 13 Jun 2023 01:00:06 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 01:00:07 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 13 Jun 2023 01:00:07 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 13 Jun 2023 01:00:08 GMT
WORKDIR /var/www/html
# Tue, 13 Jun 2023 01:00:08 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 13 Jun 2023 01:00:08 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 13 Jun 2023 01:00:08 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 13 Jun 2023 01:00:08 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 13 Jun 2023 01:00:20 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Jun 2023 01:00:20 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 13 Jun 2023 01:00:20 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 13 Jun 2023 01:00:21 GMT
USER adminer
# Tue, 13 Jun 2023 01:00:21 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Tue, 13 Jun 2023 01:00:21 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:0997ae72d27731326552ad4699d630b4932f3d31abc07a62105a0eb16b54173a`  
		Last Modified: Mon, 12 Jun 2023 23:46:43 GMT  
		Size: 56.0 MB (56040665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dac97babbe48fc6ee5134482bf3dd02a0763c71618911c97beab64bec3147a8`  
		Last Modified: Tue, 13 Jun 2023 01:01:02 GMT  
		Size: 39.6 MB (39558608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df44f63ded7015da79f717c9dbf6dfd057bcafc06012bc1e415f53113e6fc1e5`  
		Last Modified: Tue, 13 Jun 2023 01:00:51 GMT  
		Size: 389.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ae3ce4c7547485956e0bd1180cc66032006af3b33c6ae582d77834096391752`  
		Last Modified: Tue, 13 Jun 2023 01:00:51 GMT  
		Size: 1.9 KB (1864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83417b3fe0dbbaed7076986fd209d6704b096ecd961a111cfb42cba80a11dc93`  
		Last Modified: Tue, 13 Jun 2023 01:00:51 GMT  
		Size: 1.5 KB (1480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbdb97551a1780228aac70017b847d497ec088d6ad3e46d5c8b9b48083efe5a0`  
		Last Modified: Tue, 13 Jun 2023 01:00:52 GMT  
		Size: 1.4 MB (1385307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbef3e3e2b3156ba5eca052ebf766f2f4474f980905836f0c0ea9eec319f7a6e`  
		Last Modified: Tue, 13 Jun 2023 01:00:51 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:standalone` - linux; mips64le

```console
$ docker pull adminer@sha256:2591b1f0dffbc4f123a4a3bd12c1cb46669c54383e8e23e13c83edaecc2541d1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.6 MB (92614104 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9a417a537dc4187139ad39c01263d6bd8b79a728bf005ad51d3bb4d42ec1d5f`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Tue, 13 Jun 2023 00:09:46 GMT
ADD file:7ba4829e0a582c8a2e5a1d362ca30cfba3fa2911594faf9598927255100965b0 in / 
# Tue, 13 Jun 2023 00:09:51 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 01:46:11 GMT
STOPSIGNAL SIGINT
# Tue, 13 Jun 2023 01:48:01 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 01:48:08 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 13 Jun 2023 01:48:14 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 13 Jun 2023 01:48:18 GMT
WORKDIR /var/www/html
# Tue, 13 Jun 2023 01:48:21 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 13 Jun 2023 01:48:24 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 13 Jun 2023 01:48:28 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 13 Jun 2023 01:48:31 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 13 Jun 2023 01:49:21 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Jun 2023 01:49:24 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 13 Jun 2023 01:49:27 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 13 Jun 2023 01:49:31 GMT
USER adminer
# Tue, 13 Jun 2023 01:49:34 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Tue, 13 Jun 2023 01:49:37 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:ec034d426521af0a9addba08124f06b364f3364fd20ec9aec4e3364104a793d1`  
		Last Modified: Tue, 13 Jun 2023 00:23:13 GMT  
		Size: 53.3 MB (53270410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:901a0f1a33bd58f6d5e7b1de7a90c5fbe79c192cbbabfd8c7a98214496b73c1b`  
		Last Modified: Tue, 13 Jun 2023 01:52:11 GMT  
		Size: 38.0 MB (37953313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c616df06cfce4fa5e3f76b4147041f55275dd885295b9a2e1b9884f710f5a63`  
		Last Modified: Tue, 13 Jun 2023 01:51:45 GMT  
		Size: 395.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84487562d4b36a6a1112b198b725b1a727e91a77be9899c0d74b1a4a9c022dba`  
		Last Modified: Tue, 13 Jun 2023 01:51:45 GMT  
		Size: 1.7 KB (1723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5dde6303cb52a3de95ebac876b6f8590487f4ffa08f8c0e80844f4d89b75072`  
		Last Modified: Tue, 13 Jun 2023 01:51:45 GMT  
		Size: 1.5 KB (1480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:499702681379ddde7be8cc76c78d9b9c764ceea9af16c336da3a99169971feb1`  
		Last Modified: Tue, 13 Jun 2023 01:51:46 GMT  
		Size: 1.4 MB (1386295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63d75b2d63e14c568323dc0897c171f4d71efe33d94bb1423a59c555514d35ae`  
		Last Modified: Tue, 13 Jun 2023 01:51:45 GMT  
		Size: 488.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:standalone` - linux; ppc64le

```console
$ docker pull adminer@sha256:013d0c050b77551b5357486fb1e82d08f32a53c82947a1b457683a3418b6af9c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.3 MB (101256599 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df82aea7df55443c0a14ed256c8dd82bf1eb7cac2aedd58b82267c5b8b5ced7b`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Mon, 12 Jun 2023 23:17:54 GMT
ADD file:93fa83ca9c503a09001edab8e277ae6c67636f805f8bb49986e0ed2ad3ea8360 in / 
# Mon, 12 Jun 2023 23:17:57 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 09:08:19 GMT
STOPSIGNAL SIGINT
# Tue, 13 Jun 2023 09:09:07 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 09:09:10 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 13 Jun 2023 09:09:11 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 13 Jun 2023 09:09:11 GMT
WORKDIR /var/www/html
# Tue, 13 Jun 2023 09:09:12 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 13 Jun 2023 09:09:12 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 13 Jun 2023 09:09:12 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 13 Jun 2023 09:09:12 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 13 Jun 2023 09:09:34 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Jun 2023 09:09:35 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 13 Jun 2023 09:09:35 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 13 Jun 2023 09:09:35 GMT
USER adminer
# Tue, 13 Jun 2023 09:09:36 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Tue, 13 Jun 2023 09:09:36 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:ebc829b9a845100e0e82d2b659a5cd374121460e523a23fa55a97ac0ddb14460`  
		Last Modified: Mon, 12 Jun 2023 23:24:35 GMT  
		Size: 58.9 MB (58927438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d304253c00cda5d6c90e79c9b36e46c4455bbd126020f17b7169bc234c480cca`  
		Last Modified: Tue, 13 Jun 2023 09:10:32 GMT  
		Size: 40.9 MB (40939387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:237c05054c26964b88d5a4100f4f6f43e17ad63d013a43fc5747abf9c28e7b06`  
		Last Modified: Tue, 13 Jun 2023 09:10:20 GMT  
		Size: 392.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:585b216b36632020ab603105a6f22716e8ac2ac644551a7e922f790d67da5bf8`  
		Last Modified: Tue, 13 Jun 2023 09:10:20 GMT  
		Size: 1.9 KB (1874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18d440285d9c8be71bce4681d80fe4262235bdd20221ecc6534754bcb9e440d2`  
		Last Modified: Tue, 13 Jun 2023 09:10:20 GMT  
		Size: 1.5 KB (1477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8eed483473112dc2c38510a7c51a8b03b57366c4572318c832392420f444c15d`  
		Last Modified: Tue, 13 Jun 2023 09:10:20 GMT  
		Size: 1.4 MB (1385539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:778fea6b251be19305e5c619a6405b1314d448d05fcb6055cdaa1f33e499836b`  
		Last Modified: Tue, 13 Jun 2023 09:10:20 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:standalone` - linux; s390x

```console
$ docker pull adminer@sha256:b0ffe4f969dffd34c3dbe3e71d59063b59656ff0041a3432ca289d1fbc9812a4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.7 MB (93696096 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ba9b6f2571a8dd2baff58687a77b47d8c544794af1b7d5eb5a35a6562b1a5dd`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Tue, 13 Jun 2023 04:29:54 GMT
ADD file:fa60f19da2df43542549a5dd89b364d30fff981d1655f9cce8900778a7b841b9 in / 
# Tue, 13 Jun 2023 04:29:57 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 18:28:19 GMT
STOPSIGNAL SIGINT
# Tue, 13 Jun 2023 18:28:38 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 18:28:41 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Tue, 13 Jun 2023 18:28:41 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Tue, 13 Jun 2023 18:28:41 GMT
WORKDIR /var/www/html
# Tue, 13 Jun 2023 18:28:41 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Tue, 13 Jun 2023 18:28:41 GMT
ENV ADMINER_VERSION=4.8.1
# Tue, 13 Jun 2023 18:28:41 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Tue, 13 Jun 2023 18:28:41 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Tue, 13 Jun 2023 18:28:50 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Tue, 13 Jun 2023 18:28:50 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Tue, 13 Jun 2023 18:28:50 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 13 Jun 2023 18:28:50 GMT
USER adminer
# Tue, 13 Jun 2023 18:28:50 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Tue, 13 Jun 2023 18:28:50 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:2bef9d7959742dda03e39c77232808f6559cd696f21fab76fc714bdd24cae18d`  
		Last Modified: Tue, 13 Jun 2023 04:34:33 GMT  
		Size: 53.3 MB (53288042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:041f14e1e03498f73d2812d4e314dad072efa6e0e10a723ac4d6c669ba74ee6f`  
		Last Modified: Tue, 13 Jun 2023 18:29:29 GMT  
		Size: 39.0 MB (39018366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d373ef386eb7b27bd1820d70320dc6e56fbd92b6f9e9fdf87ea87270021cfc69`  
		Last Modified: Tue, 13 Jun 2023 18:29:22 GMT  
		Size: 386.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c969a5b5597cfe9ffc35987963dd486112774ae4b6aa92253ed91826df6f4b9`  
		Last Modified: Tue, 13 Jun 2023 18:29:23 GMT  
		Size: 1.9 KB (1875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:470182e50b9536e5a583649af984506bab4f6f17965a116a7cc6dd0524107fa0`  
		Last Modified: Tue, 13 Jun 2023 18:29:22 GMT  
		Size: 1.5 KB (1478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb842daac7794425df52dcc95e559eb44e625f9cd3f71149e4cd62f358f3c388`  
		Last Modified: Tue, 13 Jun 2023 18:29:22 GMT  
		Size: 1.4 MB (1385459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22cf6667e460c65791e765dcae758a7b8edf9fa7bf5166bd8854138af14de0fb`  
		Last Modified: Tue, 13 Jun 2023 18:29:23 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
