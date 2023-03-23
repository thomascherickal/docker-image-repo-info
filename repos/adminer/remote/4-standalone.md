## `adminer:4-standalone`

```console
$ docker pull adminer@sha256:44a1f797174b3f995b1dc1d2e20ec2a71f0b1e0b2953df54363141c3f9ab0181
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
$ docker pull adminer@sha256:ed6c99d9e94fb5e75bb8be1a8b1087f5da8b138639718b00f225ed000bfff029
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.2 MB (91185175 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:937eb2dd80e92aa16f0c91880b0621471b3e30c40555ba68e86e5f41cb068167`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 01 Mar 2023 01:48:43 GMT
ADD file:a4c8194220314bdada02b2e8d4a2aaa01f89c69eb66013a81a42903b7fa82e7a in / 
# Wed, 01 Mar 2023 01:48:44 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:11:09 GMT
STOPSIGNAL SIGINT
# Wed, 01 Mar 2023 02:11:45 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:11:45 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 01 Mar 2023 02:11:46 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 01 Mar 2023 02:11:46 GMT
WORKDIR /var/www/html
# Wed, 01 Mar 2023 02:11:46 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 01 Mar 2023 02:11:46 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 01 Mar 2023 02:11:46 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 01 Mar 2023 02:11:46 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 01 Mar 2023 02:12:01 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 01 Mar 2023 02:12:01 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 01 Mar 2023 02:12:02 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 01 Mar 2023 02:12:02 GMT
USER adminer
# Wed, 01 Mar 2023 02:12:02 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 01 Mar 2023 02:12:02 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:0e646b3de69bc5bf194fa10012b1ebb12aba169270858575517eba4a0019e696`  
		Last Modified: Wed, 01 Mar 2023 01:52:26 GMT  
		Size: 52.5 MB (52549820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00bf4027abeab611368338e45f58f4642e1d83d5a87ef8a375c2d83d02969dc6`  
		Last Modified: Wed, 01 Mar 2023 02:13:03 GMT  
		Size: 37.2 MB (37245976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c99bca1d37f231fa8bd33ea49e65ebf96ca034502f8985f0cbcc8c0a637f02d`  
		Last Modified: Wed, 01 Mar 2023 02:12:53 GMT  
		Size: 393.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:982b8c277f20681bc85b864b59699077b90a7c231e3adc83439edcc655d265d1`  
		Last Modified: Wed, 01 Mar 2023 02:12:53 GMT  
		Size: 1.9 KB (1870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9190a36ba5817ca33f0c2b2f47736f2615f077599cede924db93f4814ca1989`  
		Last Modified: Wed, 01 Mar 2023 02:12:53 GMT  
		Size: 1.5 KB (1478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fd15c00204f2106afe2e68fdb9c7c9e3a238d01e7379ca6558273d0271699fd`  
		Last Modified: Wed, 01 Mar 2023 02:12:53 GMT  
		Size: 1.4 MB (1385145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3ce6fbd852ba5827ecd4ee482deb80fc95fea453347043d995e0bbcafa62c14`  
		Last Modified: Wed, 01 Mar 2023 02:12:53 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-standalone` - linux; arm variant v7

```console
$ docker pull adminer@sha256:a7047172f1bf62468bbd024fde2cd30e1178685d097cae27646e1117a69d61e2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.8 MB (87782646 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:054116fa9af60f81e73db77bba41fdb4fb7b3114d14cb0b27c2a5a55c6d16d90`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 01 Mar 2023 01:57:45 GMT
ADD file:95a5e178e353a9a46c230d78b0ef83309dd487651c34e47e972ed3dae08ea00b in / 
# Wed, 01 Mar 2023 01:57:45 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:22:38 GMT
STOPSIGNAL SIGINT
# Wed, 01 Mar 2023 02:23:02 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:23:03 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 01 Mar 2023 02:23:03 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 01 Mar 2023 02:23:03 GMT
WORKDIR /var/www/html
# Wed, 01 Mar 2023 02:23:03 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 01 Mar 2023 02:23:04 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 01 Mar 2023 02:23:04 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 01 Mar 2023 02:23:04 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 01 Mar 2023 02:23:15 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 01 Mar 2023 02:23:15 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 01 Mar 2023 02:23:15 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 01 Mar 2023 02:23:15 GMT
USER adminer
# Wed, 01 Mar 2023 02:23:15 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 01 Mar 2023 02:23:15 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:30bee4bd8986478b5a9ecaaaba83525049f0b9b5a63ca88de878568bb6b83292`  
		Last Modified: Wed, 01 Mar 2023 02:02:32 GMT  
		Size: 50.2 MB (50212046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdd6b6627724e14462f46d693d6e6d571c26e42748a0d12b23dceb3bb3f76f38`  
		Last Modified: Wed, 01 Mar 2023 02:24:10 GMT  
		Size: 36.2 MB (36181310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:631947dc8f6343e1805e1c67d899e226d4747686ef46c6fc7902b90edc41c652`  
		Last Modified: Wed, 01 Mar 2023 02:24:01 GMT  
		Size: 386.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52668cb3df9893874330fb103dc278dc4b37129d4535d12b70585c166d658e3f`  
		Last Modified: Wed, 01 Mar 2023 02:24:02 GMT  
		Size: 1.9 KB (1868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:877da825c7e99e83cb7039bc5961bcd9620e0f9a1c56fe0added5a9fc7c6af2b`  
		Last Modified: Wed, 01 Mar 2023 02:24:01 GMT  
		Size: 1.5 KB (1479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0439c93e2dc13495497a94e7fbe8e4ff73f4958f1a1e11d2c747e8247033f84`  
		Last Modified: Wed, 01 Mar 2023 02:24:02 GMT  
		Size: 1.4 MB (1385064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e5373dda685e214742428841b243633aeff0a6f467547a997f5fcceadbc86b1`  
		Last Modified: Wed, 01 Mar 2023 02:24:01 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-standalone` - linux; arm64 variant v8

```console
$ docker pull adminer@sha256:7fe9245eaab6579d2f02b2c43ece653c6f014f78be767a77580df6401023b8b8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.3 MB (94334964 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da1ba2cdb7c1dcd745eda1a855a3c5d0cc50e77182d900a1a13fab7ecb94f0f1`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Thu, 23 Mar 2023 00:45:02 GMT
ADD file:70d18f9eea4e4fbdb941e66490ccb7233e182fe7ded1185de91c7d55580dd13e in / 
# Thu, 23 Mar 2023 00:45:02 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 06:50:38 GMT
STOPSIGNAL SIGINT
# Thu, 23 Mar 2023 06:50:56 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 06:50:57 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Thu, 23 Mar 2023 06:50:57 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 23 Mar 2023 06:50:58 GMT
WORKDIR /var/www/html
# Thu, 23 Mar 2023 06:50:58 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 23 Mar 2023 06:50:58 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 23 Mar 2023 06:50:58 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 23 Mar 2023 06:50:58 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 23 Mar 2023 06:51:08 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Mar 2023 06:51:08 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 23 Mar 2023 06:51:08 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 23 Mar 2023 06:51:08 GMT
USER adminer
# Thu, 23 Mar 2023 06:51:08 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Thu, 23 Mar 2023 06:51:08 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:8022b074731d9ecee7f4fba79b993920973811dda168bbc08636f18523b90122`  
		Last Modified: Thu, 23 Mar 2023 00:47:46 GMT  
		Size: 53.7 MB (53703099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98305094c7fd13042b057082ec8d7bcc2b6f08cf0bba01a567b6bc108039bdf1`  
		Last Modified: Thu, 23 Mar 2023 06:51:37 GMT  
		Size: 39.2 MB (39242570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdbbb9ddd2e012fdf94f2222f96fe1f8514ec4285c8acff371dd027ca67043c8`  
		Last Modified: Thu, 23 Mar 2023 06:51:30 GMT  
		Size: 389.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b3fa21b5eaa269a0e522ee6faa17c1942a9eb531a85d65093c785db3bf4ca32`  
		Last Modified: Thu, 23 Mar 2023 06:51:30 GMT  
		Size: 1.9 KB (1878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbcc9aba89fb8cb163ab7c6f00eaee21df2f499f9cfbb89de3b18e5f24ba0087`  
		Last Modified: Thu, 23 Mar 2023 06:51:30 GMT  
		Size: 1.5 KB (1482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abf77c8ff22b40bbe616794e9d54103a4a9648107d69c9057deb1a83342d3d58`  
		Last Modified: Thu, 23 Mar 2023 06:51:31 GMT  
		Size: 1.4 MB (1385053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25bd969a23b87a5402679ff8373fd3e9ce7af9a3e999bad556fe0cc25dda1cc6`  
		Last Modified: Thu, 23 Mar 2023 06:51:30 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-standalone` - linux; 386

```console
$ docker pull adminer@sha256:c4de7f047fc98b0bdcedf7be4bebce2041c3a7f990e89643d8dc4a3ae0935090
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.0 MB (96975392 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0163f995c51bfbe49ccdbd4a6eb18bac7e040ecd924376f8ff674c77da442570`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 01 Mar 2023 01:39:01 GMT
ADD file:881e5812ed9664defe9745d26894a268ec27de907c9a615a5204bbb5e8e94262 in / 
# Wed, 01 Mar 2023 01:39:02 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 09:17:34 GMT
STOPSIGNAL SIGINT
# Wed, 01 Mar 2023 09:18:02 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 09:18:03 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 01 Mar 2023 09:18:04 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 01 Mar 2023 09:18:04 GMT
WORKDIR /var/www/html
# Wed, 01 Mar 2023 09:18:04 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 01 Mar 2023 09:18:04 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 01 Mar 2023 09:18:04 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 01 Mar 2023 09:18:04 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 01 Mar 2023 09:18:17 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 01 Mar 2023 09:18:17 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 01 Mar 2023 09:18:17 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 01 Mar 2023 09:18:17 GMT
USER adminer
# Wed, 01 Mar 2023 09:18:17 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 01 Mar 2023 09:18:17 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:0a0c64c8f15c57499fa240b509d736a6e6b861478b11e52aadbc9551cfd10638`  
		Last Modified: Wed, 01 Mar 2023 01:44:12 GMT  
		Size: 56.0 MB (56028076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b148edf759c5b2d96f9a97d10d1b05c057dbb4d8ac7ffe3cbc726038bfb5c4d`  
		Last Modified: Wed, 01 Mar 2023 09:19:11 GMT  
		Size: 39.6 MB (39557973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2009ec4302073d8a17b85aceb5ccaa1390d5f03027f4f35ff831ad7f66afe9c`  
		Last Modified: Wed, 01 Mar 2023 09:19:01 GMT  
		Size: 389.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe108b9d04a99842776d112fcc81300f95226570acce3364d49c735d3559362d`  
		Last Modified: Wed, 01 Mar 2023 09:19:01 GMT  
		Size: 1.9 KB (1867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7006bdba0408a485a5f13bc3b4ca2eec9973032f19cdcf08248d7390038b68eb`  
		Last Modified: Wed, 01 Mar 2023 09:19:01 GMT  
		Size: 1.5 KB (1482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2fbe40968ea19d34d773c699b91806320565ea07c14f6453f437066e39400a4`  
		Last Modified: Wed, 01 Mar 2023 09:19:01 GMT  
		Size: 1.4 MB (1385114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3c9a7e8cde9b34fb43dab60217660a48a69cb72b6eaecd3cf92a2d0751c9818`  
		Last Modified: Wed, 01 Mar 2023 09:19:01 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-standalone` - linux; mips64le

```console
$ docker pull adminer@sha256:88395d56965f2a0ad761c7d9a22d89ab4548a32a2cd614509bf4bb3e7b751a62
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.6 MB (92606265 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1eaaca83a67289ee5c13370cfc221669ee0154f978e8c4b3f1cd0d4ba5962e7`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 01 Mar 2023 02:10:17 GMT
ADD file:bf6c5767a805dc84ce6187b7fb368f563954e5a7011c93d39fdd53a5dadecc9f in / 
# Wed, 01 Mar 2023 02:10:22 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 13:59:33 GMT
STOPSIGNAL SIGINT
# Wed, 01 Mar 2023 14:01:25 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 14:01:31 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Wed, 01 Mar 2023 14:01:38 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Wed, 01 Mar 2023 14:01:41 GMT
WORKDIR /var/www/html
# Wed, 01 Mar 2023 14:01:44 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Wed, 01 Mar 2023 14:01:47 GMT
ENV ADMINER_VERSION=4.8.1
# Wed, 01 Mar 2023 14:01:51 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Wed, 01 Mar 2023 14:01:54 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Wed, 01 Mar 2023 14:02:45 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Wed, 01 Mar 2023 14:02:48 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Wed, 01 Mar 2023 14:02:51 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 01 Mar 2023 14:02:54 GMT
USER adminer
# Wed, 01 Mar 2023 14:02:58 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Wed, 01 Mar 2023 14:03:01 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:c840827022f1ac884efb07d69c1c27fe594b8942edaba76884ed87691e1596a7`  
		Last Modified: Wed, 01 Mar 2023 02:18:09 GMT  
		Size: 53.3 MB (53265175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ef70b8c1aa76df155ee17f3de4ba576912f1b465f23a245590681557261c3cf`  
		Last Modified: Wed, 01 Mar 2023 14:05:31 GMT  
		Size: 38.0 MB (37950810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b085cd0066f08963b98bd9ed999777edd1901f78b54ff5648d22def1b572b7e`  
		Last Modified: Wed, 01 Mar 2023 14:05:05 GMT  
		Size: 397.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09371947d6e3ebd8155720c9afef7954918a35e3f775e826ffd25a1f3b588ddc`  
		Last Modified: Wed, 01 Mar 2023 14:05:05 GMT  
		Size: 1.7 KB (1726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb1d7f64e0b8a7174e6aa7f76935392760b59e2b285efc3a13ad2b0db526ea36`  
		Last Modified: Wed, 01 Mar 2023 14:05:05 GMT  
		Size: 1.5 KB (1478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15e61fbb27242f9c5db400342f6b1f6702d987ceae09de4190e28cf54ece1fbd`  
		Last Modified: Wed, 01 Mar 2023 14:05:06 GMT  
		Size: 1.4 MB (1386186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c4147c35a3936531f2285a81877dcca8b9bba6ab19e5eb232e207cdcb6680ef`  
		Last Modified: Wed, 01 Mar 2023 14:05:05 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-standalone` - linux; ppc64le

```console
$ docker pull adminer@sha256:ddf406bedb6ea27fd15da89331e085e564dcde0c98ba31f3914b14b4483aa56e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.2 MB (101249875 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac8b45276387b274e6256e8c13851f3460fdd98b29ca47a09f04a8fad8d02090`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Thu, 23 Mar 2023 01:19:25 GMT
ADD file:3eb86af6fda22c3e84548a6d0039be04819ce464b2700e8d8c140be49530ff7c in / 
# Thu, 23 Mar 2023 01:19:27 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 12:41:38 GMT
STOPSIGNAL SIGINT
# Thu, 23 Mar 2023 12:42:55 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 12:42:59 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Thu, 23 Mar 2023 12:43:01 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 23 Mar 2023 12:43:01 GMT
WORKDIR /var/www/html
# Thu, 23 Mar 2023 12:43:01 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 23 Mar 2023 12:43:02 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 23 Mar 2023 12:43:02 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 23 Mar 2023 12:43:03 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 23 Mar 2023 12:43:32 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Mar 2023 12:43:33 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 23 Mar 2023 12:43:33 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 23 Mar 2023 12:43:34 GMT
USER adminer
# Thu, 23 Mar 2023 12:43:35 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Thu, 23 Mar 2023 12:43:35 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:566bc84f2641b393ac5a2f4a2ca405c09943aa3ec679f38ea1588f6ee930219e`  
		Last Modified: Thu, 23 Mar 2023 01:23:52 GMT  
		Size: 58.9 MB (58921026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc2fbb285bf85ccfbb4c5282ba9f10d09cecbc5a0bab31ef237b51b3201089c2`  
		Last Modified: Thu, 23 Mar 2023 12:45:00 GMT  
		Size: 40.9 MB (40939153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c5c4d551007797e513e8983796e921a39828107b5d1309cb2783b12bc6aaac4`  
		Last Modified: Thu, 23 Mar 2023 12:44:46 GMT  
		Size: 394.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19dcdc4ed08a4d33d3c19d3c7a7fcb606bed16f514bbdf68d09ed75d0ef5a039`  
		Last Modified: Thu, 23 Mar 2023 12:44:47 GMT  
		Size: 1.9 KB (1876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f0187a4a30cb1c249de5010601f0912c92400f91482facb00198f8ba8e3691e`  
		Last Modified: Thu, 23 Mar 2023 12:44:46 GMT  
		Size: 1.5 KB (1481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3867a61f6a3237b86e8a6bb431978b79ef5a1320ee3ebe58670b7a68f930c0f`  
		Last Modified: Thu, 23 Mar 2023 12:44:47 GMT  
		Size: 1.4 MB (1385455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:553fdd9019949edcff0333970ef2dc5fa9af5479a21e08ecaf14a608524f497f`  
		Last Modified: Thu, 23 Mar 2023 12:44:46 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-standalone` - linux; s390x

```console
$ docker pull adminer@sha256:3a1427b2251efb24343fedded181036a73a9a9edd77c0241f1907db59654d4f5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.7 MB (93684414 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c2d7a2d888bb0da291a197f178923752e3a408b6b8002d6ae4d4c8595173ec84`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Thu, 23 Mar 2023 00:43:50 GMT
ADD file:1111f9325245c8edccf2d9480c39cf2368f783ad86c2700d452be4e8cbebef8a in / 
# Thu, 23 Mar 2023 00:43:54 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 07:12:38 GMT
STOPSIGNAL SIGINT
# Thu, 23 Mar 2023 07:12:56 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	apt-get update &&	apt-get install -y 		php7.4-cli 		php7.4-fpm 		php7.4-mbstring 		php7.4-mysql 		php7.4-odbc 		php7.4-pdo-dblib 		php7.4-pgsql 		php7.4-sqlite3 &&	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 07:12:59 GMT
RUN echo "upload_max_filesize = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini &&	echo "variables_order = \"EGPCS\"" >> /etc/php/7.4/cli/conf.d/0-env.ini &&	cp /etc/php/7.4/cli/conf.d/0-upload_large_dumps.ini /etc/php/7.4/fpm/conf.d/0-upload_large_dumps.ini
# Thu, 23 Mar 2023 07:12:59 GMT
RUN groupadd -r adminer &&	useradd -r -g adminer adminer &&	mkdir -p /var/www/html &&	mkdir /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 23 Mar 2023 07:12:59 GMT
WORKDIR /var/www/html
# Thu, 23 Mar 2023 07:12:59 GMT
COPY multi:8e2583c31626149dac766c1e81b6ba87f4289e683e42823f52b952fbab069922 in /var/www/html/ 
# Thu, 23 Mar 2023 07:12:59 GMT
ENV ADMINER_VERSION=4.8.1
# Thu, 23 Mar 2023 07:12:59 GMT
ENV ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3
# Thu, 23 Mar 2023 07:12:59 GMT
ENV ADMINER_COMMIT=1f173e18bdf0be29182e0d67989df56eadea4754
# Thu, 23 Mar 2023 07:13:07 GMT
RUN export DEBIAN_FRONTEND="noninteractive" &&	set -x &&	buildDeps='git curl ca-certificates' &&	apt-get update &&	apt-get install -y $buildDeps --no-install-recommends &&	rm -rf /var/lib/apt/lists/* &&	curl -fsSL "https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php" -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	git clone --recurse-submodules=designs --depth 1 --shallow-submodules --branch "v$ADMINER_VERSION" https://github.com/vrana/adminer.git /tmp/adminer &&	commit="$(git -C /tmp/adminer/ rev-parse HEAD)" &&	[ "$commit" = "$ADMINER_COMMIT" ] &&	cp -r /tmp/adminer/designs/ /tmp/adminer/plugins/ . &&	rm -rf /tmp/adminer/ &&	apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Mar 2023 07:13:07 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 23 Mar 2023 07:13:07 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 23 Mar 2023 07:13:08 GMT
USER adminer
# Thu, 23 Mar 2023 07:13:08 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Thu, 23 Mar 2023 07:13:08 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:00dac46cbc44f444bd1dffe5b00a1b239054295b96f7984793273e9d12e75591`  
		Last Modified: Thu, 23 Mar 2023 00:47:04 GMT  
		Size: 53.3 MB (53277499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef40e14df43903a504c3865251eb934e8f644d89890514fc292b06981fca7826`  
		Last Modified: Thu, 23 Mar 2023 07:13:44 GMT  
		Size: 39.0 MB (39017484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0f79bdf3c2e58c635953d9f0329b1010a5ff99b977d98975e467b7ab57a155e`  
		Last Modified: Thu, 23 Mar 2023 07:13:37 GMT  
		Size: 388.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ebc836b2a414afb40c1d84fa4fe4af21828a8f07dcbbbfe020a9a2270b0c467`  
		Last Modified: Thu, 23 Mar 2023 07:13:37 GMT  
		Size: 1.9 KB (1877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:395b8975dd5a57c4e6e30bccd71a2d34125566cbb50b6000d142e49fb27dc1ea`  
		Last Modified: Thu, 23 Mar 2023 07:13:37 GMT  
		Size: 1.5 KB (1475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f7cb7770c3999b7b71cb8bd67b1686854b1cf6a8fbd340c7da905fddae466c1`  
		Last Modified: Thu, 23 Mar 2023 07:13:37 GMT  
		Size: 1.4 MB (1385197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47125e4be7b760f757795627cf23bffd8efbadc93fd3f20e13ac58ddac7b2639`  
		Last Modified: Thu, 23 Mar 2023 07:13:37 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
