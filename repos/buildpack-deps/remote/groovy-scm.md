## `buildpack-deps:groovy-scm`

```console
$ docker pull buildpack-deps@sha256:f34194571028ed3ae1304ac25e14e7cb0efb8ce4df58442614b999cd034e37eb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:groovy-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:cb24ae08658ee1af430eb80efaf3640f3654a9f1f8b9cbc7a272122f2d7db490
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.9 MB (95888020 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec301f2b29485bceb25a06989f8ba934dc9eb5e9635c8b838368d242e0ff0f7d`
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

### `buildpack-deps:groovy-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:7a04775177ed383915768bcd2d785f3839ff0bba6df8776e661f8af36190c8f7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.6 MB (84573072 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fcc7d6c0240609424d63e4e574feeba40dd17183a6e0fe7401a85548d5c252eb`
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

### `buildpack-deps:groovy-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:48bd3fab46e1a4005d939ab03d3f674d9ed78ca95c3a524bd9dadde4fc3342fc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.3 MB (94339945 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a88213b8858039fee38797aec9d13e425912ae1a91f5cccdce6e0f8f49a24780`
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

### `buildpack-deps:groovy-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:f72d9f64184303148b01d959fefb3eabe04070a1dc733b9ec866b8098912c471
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.8 MB (110846762 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5eb6f50d7594126599d5207010e654393309175eebcff618ddb25f99fb3f7bbe`
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

### `buildpack-deps:groovy-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:4365db4194b640025d023c8c14b624f76b88dd2de5725a17c89627ae7acd4fcb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.0 MB (101989480 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe3b8c27d659830aa54e5608cb515cdffd472c9ec02cf26a468b03950c8c282b`
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
