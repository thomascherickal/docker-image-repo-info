## `buildpack-deps:groovy-curl`

```console
$ docker pull buildpack-deps@sha256:dc871d03af4a321d894ac295dbfd6d3846b0ad30a756bb6c066bf67811df6012
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:groovy-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:4091985e8ab9d2a5ec548e56a8074969e69edc59d78b82b3782f0513ce5331ed
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.8 MB (38836085 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c32756943e91e5ac2e3aa393697f6a4b08e8c7250af587581b61ed0290e33dbf`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 24 Jul 2020 14:38:45 GMT
ADD file:8cda7bfcf6c3010f9498acf5db465d8affd86bacb786338974486e23ea62b05d in / 
# Fri, 24 Jul 2020 14:38:46 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 14:38:46 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:38:47 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:38:47 GMT
CMD ["/bin/bash"]
# Fri, 24 Jul 2020 15:02:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 15:02:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:5f55bfaf77a136f7c6b5063e591480c2e7690ed1c29b0ee354caf8f6c62741e0`  
		Last Modified: Fri, 24 Jul 2020 14:39:44 GMT  
		Size: 28.4 MB (28357957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eef373180da2631c7a56d9629e37de8010fe57414453617dde3a2c1e9861f1eb`  
		Last Modified: Fri, 24 Jul 2020 14:39:39 GMT  
		Size: 31.8 KB (31838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:675d10b513df5337d26a6e2ccaf4875267999084d7f0d2f3102c54d7430cfa35`  
		Last Modified: Fri, 24 Jul 2020 14:39:39 GMT  
		Size: 842.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:552f92805e8c6585c466083ac60f40092ae127e794d498c599a31bd67df21c09`  
		Last Modified: Fri, 24 Jul 2020 14:39:39 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41c003fe1ffd7eb86efa0bcd0d127f5dca3b2f9dcaa3ad54bdeaaf16602fff1a`  
		Last Modified: Fri, 24 Jul 2020 15:10:39 GMT  
		Size: 6.9 MB (6859149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3935824be9d9e08e1fe2b607c81e88e8128e36b84b36bdb20dfbc6a90fd43d96`  
		Last Modified: Fri, 24 Jul 2020 15:10:38 GMT  
		Size: 3.6 MB (3586137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:groovy-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:1689c0630c7c9d576bd0f16b95c196c794886f51432a20e20c45a3546142d55f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.1 MB (33130268 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dcff368460c3c3afb62f4756b2b72b900ea028b3ad54727b813997d64384c201`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 06 Jul 2020 20:08:43 GMT
ADD file:021612df98a3252c0018261734979dffe9cdc59bdd68707ae03cea58d0c65498 in / 
# Mon, 06 Jul 2020 20:08:48 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 23 Jul 2020 08:04:50 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 23 Jul 2020 08:04:54 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 23 Jul 2020 08:04:55 GMT
CMD ["/bin/bash"]
# Thu, 23 Jul 2020 08:12:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Jul 2020 08:12:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:008c40b75c61a21ea627c86505f910d9a47056dc120ce6996c3d080b08658308`  
		Last Modified: Mon, 06 Jul 2020 15:50:47 GMT  
		Size: 23.8 MB (23846810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:669074342c885ac270b199e748002596d0f32df7f77c659f5413f77f274cc91e`  
		Last Modified: Thu, 23 Jul 2020 08:05:45 GMT  
		Size: 31.9 KB (31856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca6860323f7121ae3ef42c0e5a729d9019a7d73fb9243d8a51943a2aa107c6b7`  
		Last Modified: Thu, 23 Jul 2020 08:05:45 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2afad5102492ecbe7ecd632b6fe604a800b86c249d9d2b3479b2da9647a22495`  
		Last Modified: Thu, 23 Jul 2020 08:05:44 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:468e38fb132bdeddfd36c0a893c4fb4814ed93c6e0c83eab5faeabf7deb892f6`  
		Last Modified: Thu, 23 Jul 2020 08:18:31 GMT  
		Size: 6.2 MB (6191330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:242b21b142e64cc1983d3d7e88a1255886de1d1c5c746eafc0b392be36a3aec8`  
		Last Modified: Thu, 23 Jul 2020 08:18:30 GMT  
		Size: 3.1 MB (3059236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:groovy-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:691a916b69b8c4a9a867742267e7b70e4d46bd875f2af34f75a6f0048888ad28
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.3 MB (37295014 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b57080b21443c8b16457d261d6d13f5a55c61ae75ad00090c92d418024c4443`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 06 Jul 2020 22:05:50 GMT
ADD file:35b0d977e8fc4305b3f988e3af2c52419e39aae68287af590636dfdb7487dbed in / 
# Mon, 06 Jul 2020 22:05:53 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Mon, 06 Jul 2020 22:05:55 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 06 Jul 2020 22:05:57 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 06 Jul 2020 22:05:58 GMT
CMD ["/bin/bash"]
# Mon, 06 Jul 2020 22:58:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Mon, 06 Jul 2020 22:58:33 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:bca3f99199d9260076c548f38af71788f901900c99316e357c1dfb0e06fafbd6`  
		Last Modified: Mon, 06 Jul 2020 15:50:50 GMT  
		Size: 27.0 MB (26969246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daf01b6284862c6caa2ce0e716ddb00705d21bb4f7cc4501c1fdf1130c17ffa7`  
		Last Modified: Mon, 06 Jul 2020 22:07:25 GMT  
		Size: 31.8 KB (31830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e991f38a848885cf9ff0e35cb51871c37ee33387f3159b4dbd1fa25146a3ecb`  
		Last Modified: Mon, 06 Jul 2020 22:07:26 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85b128a6106c13f4424dcc44fef4eaa219acaf5f3c8510660e77bd90c81e6227`  
		Last Modified: Mon, 06 Jul 2020 22:07:25 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac980152f16f03da3b03b8a6b0804bce8a1c28151d843524b791230e868b1b14`  
		Last Modified: Mon, 06 Jul 2020 23:08:19 GMT  
		Size: 6.7 MB (6722628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9d85f32459c314182a20d3c5effc3b5a3e1d981ed5cc5a38d6d9d1a22a68642`  
		Last Modified: Mon, 06 Jul 2020 23:08:19 GMT  
		Size: 3.6 MB (3570275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:groovy-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:b2f44bdc592a7824db7e7b36ed2c770a9949e19c6aa09a90b42021a8aa0e6f9e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.3 MB (45252123 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f379cd11de3ab215360d73c169f6f174699cd8c72110abdcf8fd531b04a3d7e3`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 06 Jul 2020 22:14:37 GMT
ADD file:4ce6882e512c279031700803ff45277278a6abe7c6418f436c85e0d066943302 in / 
# Mon, 06 Jul 2020 22:14:50 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Mon, 06 Jul 2020 22:15:08 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 06 Jul 2020 22:15:27 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 06 Jul 2020 22:15:38 GMT
CMD ["/bin/bash"]
# Tue, 07 Jul 2020 01:36:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 07 Jul 2020 01:37:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:de300362f1d644150544eb1523eefb5eb9d2d3fdf58be3aec349a0d3b02f33f9`  
		Last Modified: Mon, 06 Jul 2020 15:51:24 GMT  
		Size: 33.0 MB (32959640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d9c67b569feeae3f4167718dcc98be6f8ea149d7547a436363b4ddb15570933`  
		Last Modified: Mon, 06 Jul 2020 22:18:47 GMT  
		Size: 31.6 KB (31635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f7a367e520abe796341a0391780c5d1d14df2dea9ac76d1b4c0cdc833062895`  
		Last Modified: Mon, 06 Jul 2020 22:18:47 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bb6403ad0c2a89150f64679cb5bfe40a7f419582465b2b0cb91bbf6ca57844e`  
		Last Modified: Mon, 06 Jul 2020 22:18:47 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c11aa7997c34fac81ac44f0c030234ad75bac101bcdecb109b91e6171573ffe9`  
		Last Modified: Tue, 07 Jul 2020 02:23:51 GMT  
		Size: 7.8 MB (7812080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b56ea8d11e73fdab9482db3280b468c6014292335626ff160428d238325761d2`  
		Last Modified: Tue, 07 Jul 2020 02:23:51 GMT  
		Size: 4.4 MB (4447733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:groovy-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:0a06b39eb1e4b4e6e421812ff86337223922f153562b5ea2a50d705691b8653d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.3 MB (37333064 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ea6c900c9a29df442c6eef1e589cd39f189870b8a3418dac6884a5f34e16509`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 06 Jul 2020 20:20:33 GMT
ADD file:7c5297f390515aab00f66f663182cadbb3c5dbf52fb015526b80806df21de69d in / 
# Mon, 06 Jul 2020 20:20:35 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Mon, 06 Jul 2020 20:20:36 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 06 Jul 2020 20:20:37 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 06 Jul 2020 20:20:37 GMT
CMD ["/bin/bash"]
# Mon, 06 Jul 2020 20:46:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Mon, 06 Jul 2020 20:46:12 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:3c5e60e47f65a4306c7d2ad46d35b9ea6d4aaf9cb77add2bff5be52a742d23e4`  
		Last Modified: Mon, 06 Jul 2020 15:52:10 GMT  
		Size: 27.2 MB (27174117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b6ddf166e3f11601f2466edd2cfbfe9942c0f85314ffb2ea31f66bb6d0cf123`  
		Last Modified: Mon, 06 Jul 2020 20:21:35 GMT  
		Size: 32.5 KB (32456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:076f8572b34a88b603a66fc9eba9b5237c09e64670ac0d8a02e024d6e3ade52f`  
		Last Modified: Mon, 06 Jul 2020 20:21:35 GMT  
		Size: 840.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f928d1948ab604aafd2985aaa9196351c03043dee8e4bbbd73f4cbf190abb675`  
		Last Modified: Mon, 06 Jul 2020 20:21:41 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11eec02dfd95f6d6df751544a08b98b891c24c0ad561386ffd22b32592094376`  
		Last Modified: Mon, 06 Jul 2020 20:51:12 GMT  
		Size: 6.5 MB (6545554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40a9f1cd556b3c6d476e9540bdaec30b426c7e295beb757e67cbbb2a3bcfc3ca`  
		Last Modified: Mon, 06 Jul 2020 20:51:17 GMT  
		Size: 3.6 MB (3579909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
