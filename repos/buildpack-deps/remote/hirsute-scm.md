## `buildpack-deps:hirsute-scm`

```console
$ docker pull buildpack-deps@sha256:c4bcf52f517fb23e6b8f196c1ba184a95b92a873ec6641caef1b58ce7d4f9a23
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; s390x

### `buildpack-deps:hirsute-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:0a3c33d82bf84b591c2de3120924db231c9fdd821501eed31e8069a03d597e6c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.2 MB (76232948 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:373f1fe6520ba7d230c95537c0e1de8b09072f57890f1407ccb15cf17fc3e6b3`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 25 Nov 2020 23:00:24 GMT
ADD file:efa60bd7da49bad0a724434362f77d98c9f3c786170c7fef64ecb57aa808b18e in / 
# Wed, 25 Nov 2020 23:00:26 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 25 Nov 2020 23:00:28 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 25 Nov 2020 23:00:30 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 25 Nov 2020 23:00:31 GMT
CMD ["/bin/bash"]
# Thu, 17 Dec 2020 08:41:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Dec 2020 08:41:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 17 Dec 2020 08:42:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cf5d8cf40e57262478b56493eaf1bb9d9a8ecde1d37cfc10e81f73798a0a5b7a`  
		Last Modified: Mon, 23 Nov 2020 22:54:17 GMT  
		Size: 26.3 MB (26336795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0d0e651346be2ec39fb01f211210fa42a2ec5212300b3a6d73f450dd1dc709d`  
		Last Modified: Wed, 25 Nov 2020 23:02:22 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffe721ee3adfabbef45101e3cdd00ff12aa4ea18319502279b4da2389a2c153f`  
		Last Modified: Wed, 25 Nov 2020 23:02:22 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b6b39ed7adb6a7a6d999508a6ae30fe04c7a403accfe529f05acf9a5e742833`  
		Last Modified: Thu, 17 Dec 2020 09:01:48 GMT  
		Size: 4.8 MB (4849916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f9e63643887e8142d918de418503ee33102967776ae4dcda5389138288430ec`  
		Last Modified: Thu, 17 Dec 2020 09:01:48 GMT  
		Size: 3.1 MB (3126212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1eaf6ce3ed47b1a43b079ba4bed46a379c125af9ddec54251aaeeb847f941f2`  
		Last Modified: Thu, 17 Dec 2020 09:02:13 GMT  
		Size: 41.9 MB (41918985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:hirsute-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:a436f91924bc8aaef0a435e168524194d1ac5defbefc17f70027b0ed3297d811
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **85.3 MB (85261072 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a921027bf4557955b67cc377f351011fe1972df62063019bfe58c36baa610099`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 25 Nov 2020 22:43:49 GMT
ADD file:684109072834ffe6e5130fb786fe91fb344b842b0adfdfed022c072948606081 in / 
# Wed, 25 Nov 2020 22:43:52 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 25 Nov 2020 22:43:54 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 25 Nov 2020 22:43:56 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 25 Nov 2020 22:43:57 GMT
CMD ["/bin/bash"]
# Thu, 17 Dec 2020 10:27:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Dec 2020 10:27:52 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 17 Dec 2020 10:28:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4de913dcc000107d6987a8212435904776bb6d08325b00bcf57becd50f5aacde`  
		Last Modified: Mon, 23 Nov 2020 22:53:53 GMT  
		Size: 29.9 MB (29924288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1104249546118ee3a916a469a5b852ee61a921a17589c55aadd35286f864487d`  
		Last Modified: Wed, 25 Nov 2020 22:45:25 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff31b6873067a11ca32a6a935eae861c6cfa61b77f3d57b7e7223bda5e9162ac`  
		Last Modified: Wed, 25 Nov 2020 22:45:25 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86b531874dd96010e121cdf89631969afcb00ff3b121dd2aba82b26af641b141`  
		Last Modified: Thu, 17 Dec 2020 10:47:13 GMT  
		Size: 5.4 MB (5390356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce68abf4d50703a9e41c0014aa88574581434e05e9a1128a80de5c8beedd6fbb`  
		Last Modified: Thu, 17 Dec 2020 10:47:13 GMT  
		Size: 3.6 MB (3637680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4ffda80240334287fbfd80ba24324f45c5c796de703a186c9e214abf84b17bd`  
		Last Modified: Thu, 17 Dec 2020 10:47:35 GMT  
		Size: 46.3 MB (46307713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:hirsute-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:6dfe6e52ff7766c5a0437e8c800a2368a8c9985abfb25da4081a21f4265da36a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.5 MB (91506318 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57afced181881ecfbde9da40206d91244f5b7138f75747609b277eddb4f8bd5f`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 25 Nov 2020 22:46:04 GMT
ADD file:ab12e008ff291c18206f1e8490e1672e3ea2aaf390bc444f49317287a034af37 in / 
# Wed, 25 Nov 2020 22:46:11 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 25 Nov 2020 22:46:13 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 25 Nov 2020 22:46:15 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 25 Nov 2020 22:46:15 GMT
CMD ["/bin/bash"]
# Thu, 17 Dec 2020 11:35:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Dec 2020 11:35:51 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 17 Dec 2020 11:36:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b3e953add5ac1dcec2264f9083ff5d7dee945c64eb63c1f15f7dec6e9e257095`  
		Last Modified: Mon, 23 Nov 2020 22:55:01 GMT  
		Size: 31.7 MB (31703544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b16aa65d410ea610c84dcc79a64a6ab6587c25f53847b375c660cb1d320946d`  
		Last Modified: Wed, 25 Nov 2020 22:47:46 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a93420f7924d968c4d93a439a147955351d7e1a8169caa9b28ae2bbb7d0339cf`  
		Last Modified: Wed, 25 Nov 2020 22:47:46 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6935d839a42a9a1159cba983cd08b88aaf5f8429c1131a8391da35a1216876f`  
		Last Modified: Thu, 17 Dec 2020 11:51:49 GMT  
		Size: 5.6 MB (5644141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd7b74d50fc8289baab6caa8d019fdb678050fab25290d215eb451a501ec6ad9`  
		Last Modified: Thu, 17 Dec 2020 11:51:49 GMT  
		Size: 3.7 MB (3674886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ce32436fbfd60f98a1fbfc020cdd306bee49367e04c45ceb09e5636110e9569`  
		Last Modified: Thu, 17 Dec 2020 11:52:06 GMT  
		Size: 50.5 MB (50482711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
