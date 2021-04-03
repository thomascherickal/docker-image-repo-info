## `buildpack-deps:groovy`

```console
$ docker pull buildpack-deps@sha256:8b00fcfaf58eb83080e7492de1f230c05ee765facbbc5aab0da7ca56e4cedcb8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:groovy` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:4791d9dfce7ba37c8211f3c16e61b399486c3e1fa3165db82b48ae3574d08b16
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **246.1 MB (246102702 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aebf61fcd4f88b7d3ed9fdf0ce1080c85023069e3307fed9ee1e2c102f7aa145`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Sat, 03 Apr 2021 00:53:17 GMT
ADD file:a71f81a0905a73eaeeca46fe893724cb2cef31b7e3bf46569bb3316d2337004f in / 
# Sat, 03 Apr 2021 00:53:18 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 03 Apr 2021 00:53:19 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Sat, 03 Apr 2021 00:53:21 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 03 Apr 2021 00:53:21 GMT
CMD ["/bin/bash"]
# Sat, 03 Apr 2021 01:53:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 01:53:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 03 Apr 2021 01:54:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 01:57:09 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2dee742ee950413083a1c44cfc3cd753eb7e33e8729dd3759d00f1e4d868b28d`  
		Last Modified: Mon, 29 Mar 2021 16:08:59 GMT  
		Size: 31.3 MB (31347935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8b7a6a9a438955cc85626e420648408aa254d4c2a452b07f89cb547c13ce1c0`  
		Last Modified: Sat, 03 Apr 2021 00:54:29 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58d6bf928b2da23c0ee37ef64428a55da677eb0d80cf4a98a41828b2cfe11fe3`  
		Last Modified: Sat, 03 Apr 2021 00:54:29 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab82c5a5469ad67bd2a316505b70d58082a27e30251494d428adc6e524e4cf71`  
		Last Modified: Sat, 03 Apr 2021 02:00:00 GMT  
		Size: 5.4 MB (5403491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10b95143b57c1dd91366a3ea5ea946585dc4ee536e979b4d42b936f292745dcc`  
		Last Modified: Sat, 03 Apr 2021 02:00:00 GMT  
		Size: 3.7 MB (3662585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99c4c66e4a8b48bbb333460a24455499150f3fa94a3062bbf4e4305da14e35d6`  
		Last Modified: Sat, 03 Apr 2021 02:00:21 GMT  
		Size: 55.5 MB (55472973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea5288531baea79adf3027c76f85f48b0734647393a5a8777c54a2bbd0b50ecb`  
		Last Modified: Sat, 03 Apr 2021 02:00:58 GMT  
		Size: 150.2 MB (150214682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:groovy` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:684a48f69740d8e211fb66cda1aed8d5f2d53b785d97015ee8c073e6026f29fb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **210.5 MB (210468683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44ce21525c73746513389a47857e36f7767cb7903790a9fb4002c4ba5bf38dee`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Sat, 03 Apr 2021 01:42:31 GMT
ADD file:2ae23ddda89705714d090c863b98cfe913d3a4901ddcc6c06ed383c1b4d4c350 in / 
# Sat, 03 Apr 2021 01:42:35 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 03 Apr 2021 01:42:37 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Sat, 03 Apr 2021 01:42:39 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 03 Apr 2021 01:42:40 GMT
CMD ["/bin/bash"]
# Sat, 03 Apr 2021 03:12:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 03:12:22 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 03 Apr 2021 03:13:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 03:15:03 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:67dd0c52fd3aa8afb3da610cb6d76e6fb7eee1833cfd7821a12dba43659ca049`  
		Last Modified: Mon, 29 Mar 2021 16:10:31 GMT  
		Size: 26.3 MB (26305223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ea96f330daf67e238cce47c52002d3776cc1e9a220e4de501396f4273e8c821`  
		Last Modified: Sat, 03 Apr 2021 01:44:18 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58c70d5d6d1fe2519441c3cd716eeb143d9cdf3cbfbba5a3e21af9be936fa976`  
		Last Modified: Sat, 03 Apr 2021 01:44:17 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0b73a4581d9459eff350bd69f3480f4b41d2b22d0b08a9e619040df4baae8d3`  
		Last Modified: Sat, 03 Apr 2021 03:18:28 GMT  
		Size: 4.8 MB (4839746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:924fd23aca983544f9a5306edced13605f8be0107732d4e03b757a6be9d2138a`  
		Last Modified: Sat, 03 Apr 2021 03:18:27 GMT  
		Size: 3.1 MB (3139678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cd2f207e97a3a06c16834609481d475bff37bf097c69f91459c02e5ba0ea43e`  
		Last Modified: Sat, 03 Apr 2021 03:18:53 GMT  
		Size: 50.3 MB (50287387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f09b4eb58d277fe8c47369cab65c5aef3a010e043de56eada67b4dba34477f7d`  
		Last Modified: Sat, 03 Apr 2021 03:19:41 GMT  
		Size: 125.9 MB (125895611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:groovy` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:722d40ae376b0ffcfce7598586b77308e0e5fbb9b5bb4d505e77985a3a268856
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **237.0 MB (237032541 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f31cf6e40d780822b4fa0f89af3dd661a0ebd915bec8dc667701af7f49f472e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Sat, 03 Apr 2021 04:10:28 GMT
ADD file:4b9d9af7c10506f5422abc99b8a2b67e73498b0aceb08d57154d8c3261616006 in / 
# Sat, 03 Apr 2021 04:10:32 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 03 Apr 2021 04:10:35 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Sat, 03 Apr 2021 04:10:37 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 03 Apr 2021 04:10:38 GMT
CMD ["/bin/bash"]
# Sat, 03 Apr 2021 06:07:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 06:07:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 03 Apr 2021 06:08:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 06:09:34 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3298a7c79fb420e0a763ee92bda8aa4dd2b1989a4d18328166da14a6c7c52cd6`  
		Last Modified: Mon, 29 Mar 2021 16:09:56 GMT  
		Size: 29.9 MB (29879434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0a0c80ff3aaf8d8d5e27b8fb630ec143371988160c3e78ae3657844955adb10`  
		Last Modified: Sat, 03 Apr 2021 04:12:05 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:881ee70970113ff00de5bae24a68f4184cf40f8c4d6c90026c3a6f5e19a9ea60`  
		Last Modified: Sat, 03 Apr 2021 04:12:05 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3099a31129f442743139c4db71bb6f2ce2c2571d4de2dc01861e2662646abd35`  
		Last Modified: Sat, 03 Apr 2021 06:12:53 GMT  
		Size: 5.4 MB (5371744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f3bb9c3dfe7559a1c3500d639b33928087403985b64039dfe7149713135ecf9`  
		Last Modified: Sat, 03 Apr 2021 06:12:53 GMT  
		Size: 3.6 MB (3634189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c63970d81dd9467a7d46cb489af5fdd5aa96a89b29a9ea25b48412e4e9ce9a00`  
		Last Modified: Sat, 03 Apr 2021 06:13:15 GMT  
		Size: 55.5 MB (55453538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:235e1775694db5350afccf8d547b5914afd6535f7a3116eb3492b2db08b0eae8`  
		Last Modified: Sat, 03 Apr 2021 06:13:56 GMT  
		Size: 142.7 MB (142692596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:groovy` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:5dca065698ed7061a199001def9ba1880796867d4f34ce09f6883fd1e59b57a4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **269.4 MB (269385505 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc9c40ea3674c1c81f83c9bf0bfa515572e7e94e1654e9a508334c4be68fed41`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Sat, 03 Apr 2021 02:12:56 GMT
ADD file:4c4f5eecccba79e189716f80611955e27faede2f1aceb49e3dbb6efc98b92cab in / 
# Sat, 03 Apr 2021 02:13:18 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 03 Apr 2021 02:13:43 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Sat, 03 Apr 2021 02:14:19 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 03 Apr 2021 02:14:29 GMT
CMD ["/bin/bash"]
# Sat, 03 Apr 2021 06:24:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 06:26:11 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 03 Apr 2021 06:28:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 06:38:37 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f13e0ef305fe52ff0aca7132d5d95a977d63297d77fa55fb6cc2255dd3a2561d`  
		Last Modified: Mon, 29 Mar 2021 16:11:03 GMT  
		Size: 36.5 MB (36543343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5b6abc22c0b444cf385e63169a745f4b5b5eb0e7d49a50e946dc36e569541db`  
		Last Modified: Sat, 03 Apr 2021 02:18:14 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:533d2befcb0f0219b577725ee49ee2fd0b919ff838549086e90293863e1857cf`  
		Last Modified: Sat, 03 Apr 2021 02:18:14 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d8d161239e1f87388eebded23079c99262b2b0f5d110faf24596107a2324328`  
		Last Modified: Sat, 03 Apr 2021 06:41:52 GMT  
		Size: 6.0 MB (6039743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c68ab3a14ec0316dd00c1514426ced0b12651481bd79fd141f71f9e46fc7335`  
		Last Modified: Sat, 03 Apr 2021 06:41:51 GMT  
		Size: 4.5 MB (4520779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bb78b5388af316372b375b0c19349c6295d554a8928fe6573749ce3b5d20932`  
		Last Modified: Sat, 03 Apr 2021 06:42:16 GMT  
		Size: 63.7 MB (63741858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca3fbd816a6d3d8629d8a0e62ca04b92c79980f4ce108698aada25b4491587d7`  
		Last Modified: Sat, 03 Apr 2021 06:43:04 GMT  
		Size: 158.5 MB (158538743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:groovy` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:8f19f39ac92b63f5d351c36d0fab3bc9c8eb4e7068269c2e8002dccba469f5b4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **246.0 MB (245986548 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e841dd2b3c740f4e94e52eb8a3c5a140b7714c96b790f4477d04f5b686a2bac`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Sat, 03 Apr 2021 00:53:22 GMT
ADD file:7530ca33c1e21fa75a86e229bb6200467b6e82b58b280f8e5b3f355a808a8878 in / 
# Sat, 03 Apr 2021 00:53:24 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 03 Apr 2021 00:53:25 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Sat, 03 Apr 2021 00:53:25 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 03 Apr 2021 00:53:25 GMT
CMD ["/bin/bash"]
# Sat, 03 Apr 2021 01:12:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 01:13:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 03 Apr 2021 01:13:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 01:14:06 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:61f6f92f4fe750924da758813989237f40f122d4fd179c61c92d2959f4061dab`  
		Last Modified: Mon, 29 Mar 2021 16:11:05 GMT  
		Size: 31.6 MB (31554982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe47d8812573abbcb0e18c773cb25b6a6a1d3c49bd528fe8b319cc581dd4fee4`  
		Last Modified: Sat, 03 Apr 2021 00:54:12 GMT  
		Size: 845.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:057d3d13d3419951c40bae7996b31fa816b951bf0091ae370f1d9fec6d8cd0b8`  
		Last Modified: Sat, 03 Apr 2021 00:54:12 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:017d70764310d4923a7939d20604adbd4808136dfcb56155d528db064efed3dc`  
		Last Modified: Sat, 03 Apr 2021 01:16:18 GMT  
		Size: 5.6 MB (5628655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fba5a93b9c325da0130ffbf39725f1e06031d958286db187341af0949fcbf844`  
		Last Modified: Sat, 03 Apr 2021 01:16:18 GMT  
		Size: 4.2 MB (4155802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ce7a223f4f26e6f5f2e6f0ca55688add4311816c957dd0604ff3604ad668f6f`  
		Last Modified: Sat, 03 Apr 2021 01:16:38 GMT  
		Size: 60.6 MB (60649008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45f01b8232518340ee6644a9f0f18a25a501e4375bf4ef39884fa4c582372bbd`  
		Last Modified: Sat, 03 Apr 2021 01:17:04 GMT  
		Size: 144.0 MB (143997068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
