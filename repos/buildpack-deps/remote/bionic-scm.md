## `buildpack-deps:bionic-scm`

```console
$ docker pull buildpack-deps@sha256:0a57ec3cdfea0f30ab322a3a29ccb17adafa778c894c22defabc6e6ffaf40830
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:bionic-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:2fca27ce716210dadbc5937d64e26e6c3e0ca877b93e446be48e7dc579feb56b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.1 MB (81110828 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:62d548ac80041ebcfabfeabbedf45bf803925395a8c5d9f8c15981ed366ed201`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 20 Mar 2020 19:20:20 GMT
ADD file:594fa35cf803361e69d817fc867b6a4069c064ffd20ed50caf42ad9bb11ca999 in / 
# Fri, 20 Mar 2020 19:20:21 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 20 Mar 2020 19:20:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 20 Mar 2020 19:20:22 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 20 Mar 2020 19:20:22 GMT
CMD ["/bin/bash"]
# Fri, 20 Mar 2020 19:45:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 20 Mar 2020 19:45:12 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 20 Mar 2020 19:45:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5bed26d33875e6da1d9ff9a1054c5fef3bbeb22ee979e14b72acf72528de007b`  
		Last Modified: Thu, 12 Mar 2020 13:21:29 GMT  
		Size: 26.7 MB (26690587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f11b29a9c7306674a9479158c1b4259938af11b97359d9ac02030cc1095e9ed1`  
		Last Modified: Fri, 20 Mar 2020 19:21:18 GMT  
		Size: 35.4 KB (35372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:930bda195c84cf132344bf38edcad255317382f910503fef234a9ce3bff0f4dd`  
		Last Modified: Fri, 20 Mar 2020 19:21:18 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78bf9a5ad49e4ae42a83f4995ade4efc096f78fd38299cf05bc041e8cdda2a36`  
		Last Modified: Fri, 20 Mar 2020 19:21:18 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4df973d9f31a2a8edee5ece2336ffe499905340fdcc9c6f13fbe54b080885d8c`  
		Last Modified: Fri, 20 Mar 2020 19:56:15 GMT  
		Size: 6.1 MB (6079944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02ee9caae01b55184f936f67ecbee9d7cd9c5fe20c069f0168e4512744aba805`  
		Last Modified: Fri, 20 Mar 2020 19:56:15 GMT  
		Size: 3.0 MB (2962401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99ca786abab337ef520f2921fcef9896078a660adc17c0aae1e9bb1772f49d0b`  
		Last Modified: Fri, 20 Mar 2020 19:56:28 GMT  
		Size: 45.3 MB (45341514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:f128bd2cd0ee9f8d35e9172daf2f100f11dbecc6b311db9e9845240cd4c3a773
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.5 MB (70529619 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d1eedcbb1a0fb1a9d0069eb225bdcbd39779970880c12a5e85e8cb66730ab59`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 23 Apr 2020 22:06:03 GMT
ADD file:7b716521aeb6ae372a2660a2e5fc6c55001a12772c5f808963363b3194c1b6f1 in / 
# Thu, 23 Apr 2020 22:06:07 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 23 Apr 2020 22:06:09 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 23 Apr 2020 22:06:11 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 23 Apr 2020 22:06:12 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 12:17:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 12:17:51 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 24 Apr 2020 12:18:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:bfb2710e7a499e5a0ecb4a694f4ec66c08a8a7501cdd43d1bcef61a54ca008b8`  
		Last Modified: Sun, 05 Apr 2020 20:24:11 GMT  
		Size: 22.3 MB (22276244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c78424bd0db4f26216c80c16f14cdbb94424732ed34e91c84303d4e9fe2a819a`  
		Last Modified: Thu, 23 Apr 2020 22:08:18 GMT  
		Size: 35.5 KB (35463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60330e98a48fe01f9fadb99c597930437c15e1a00006e43234404e20d5e5471b`  
		Last Modified: Thu, 23 Apr 2020 22:08:18 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fc5290c7dcf9b435262d02bb531959de9b08c5cc139b9ea46fda8061af60116`  
		Last Modified: Thu, 23 Apr 2020 22:08:18 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53837b8509aba69c46669c4ebdfe3f57f712b91afcc5933d6aa470595163a454`  
		Last Modified: Fri, 24 Apr 2020 12:46:36 GMT  
		Size: 5.1 MB (5146848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc501d1f2d1ab435a8ee8f050ff42068f757fee379b17b29ae8c82ba08ae0227`  
		Last Modified: Fri, 24 Apr 2020 12:46:35 GMT  
		Size: 2.5 MB (2525640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e66c16da35a2e1c5b668b8cdd0e351b90032e8c887ab9496a31427ed395e4aa2`  
		Last Modified: Fri, 24 Apr 2020 12:46:59 GMT  
		Size: 40.5 MB (40544381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:4d341d0e3dd36b1cfe1dbb38c40b1bc11afac9537e80b4ec8b0cfa030c5acf63
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.1 MB (75148248 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:88b651f9d5c996ab90029ec934dc484ad27fa10ee4110d239468530636500770`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 24 Apr 2020 00:16:45 GMT
ADD file:bd5b3470601aa4a28132ec60a8b1c33516d09a1391864fe1dbf82a4030397fd1 in / 
# Fri, 24 Apr 2020 00:16:54 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Apr 2020 00:16:58 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Apr 2020 00:17:03 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Apr 2020 00:17:05 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 15:57:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 15:58:14 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 24 Apr 2020 15:58:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c2cd007b69f7e5f37c851aa689e0e617fbaa3fe3e470f714337a03e569b7f434`  
		Last Modified: Sun, 05 Apr 2020 20:25:25 GMT  
		Size: 23.7 MB (23720401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c087f8bf83d28baa9c53fc5cfb0dfc79d5062cfad77563076553b04259e822f`  
		Last Modified: Fri, 24 Apr 2020 00:21:16 GMT  
		Size: 35.2 KB (35197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:474b5c43e9a24e1958763941a17a7cac60b13460a47f2ae9067ec03ceadab33a`  
		Last Modified: Fri, 24 Apr 2020 00:21:15 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7083e6591d76b9a6c13497a6a89bfbae3e7eb2eb31bec366bec3884c8e4517ce`  
		Last Modified: Fri, 24 Apr 2020 00:21:15 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fc61ade23307980ee6e100f821e1def9c6c6104e603ee192ae2d8cde88492ca`  
		Last Modified: Fri, 24 Apr 2020 16:11:25 GMT  
		Size: 5.5 MB (5521572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a584388019babd563a048194e062e9e4afe0a079e7a2f106f0483f33e26e9f1`  
		Last Modified: Fri, 24 Apr 2020 16:11:24 GMT  
		Size: 2.7 MB (2723793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e5d70401cdecb15ac30e81dd2ca0dacba10ffdbe59e90714945b877ce885631`  
		Last Modified: Fri, 24 Apr 2020 16:11:43 GMT  
		Size: 43.1 MB (43146247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:ab170e1445340e79c18ff0196f3d2a3839c5d6692ad94d933aece82b312ad892
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.6 MB (83648571 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0523d9cec21f4fd30071137a7b6b2466b58780b2837032ed923a74d5deabaa82`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 23 Apr 2020 21:17:02 GMT
ADD file:93916d8759465832704c50a78cd4ca1ad83e80baefd96a15563505b3374b8f3c in / 
# Thu, 23 Apr 2020 21:17:03 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 23 Apr 2020 21:17:04 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 23 Apr 2020 21:17:05 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 23 Apr 2020 21:17:05 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 09:01:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 09:01:30 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 24 Apr 2020 09:02:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:32febc939a10ccd7e09d79d3844314e0ddd7186a038a8129711026e33bb52944`  
		Last Modified: Sun, 05 Apr 2020 20:23:59 GMT  
		Size: 27.1 MB (27123063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1172dfcc3d758ff57c194883a4e3f387b056879cb1366a4b6917f0f111b57c0`  
		Last Modified: Thu, 23 Apr 2020 21:17:53 GMT  
		Size: 34.6 KB (34621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72cec8eab9aff7ebcd137e82043cc8bce36e7807a6101c176aeecb5f45229468`  
		Last Modified: Thu, 23 Apr 2020 21:17:53 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20d2624c94975a0cf9135648d1bfdbbbc91abd34977488f6fb47df8d674c34d8`  
		Last Modified: Thu, 23 Apr 2020 21:17:53 GMT  
		Size: 164.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f400c8e6781006db950f64a7c886c3dbb231ec438889a93fb7568df8b893c1e`  
		Last Modified: Fri, 24 Apr 2020 09:13:04 GMT  
		Size: 6.4 MB (6368585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52bf06a84da40b1ef0ebae01a7dea1e072309191baae95d09ce18e114ad7cf60`  
		Last Modified: Fri, 24 Apr 2020 09:13:04 GMT  
		Size: 3.2 MB (3192905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95f2e744e2e20042fe4cfc26e54c3596b2e2cce72462ee126984989ea30dae81`  
		Last Modified: Fri, 24 Apr 2020 09:13:22 GMT  
		Size: 46.9 MB (46928380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:e7615547b947475a407f0b1a0cb99b3a7c02c41f923690380881daf8f1ff8309
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.2 MB (94175998 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff11daf3483cf2b29320b418337c1271155d296097978b2050e5c7ae556b5667`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 23 Apr 2020 20:42:30 GMT
ADD file:726a32203fbcaae787c10740754e38dcb186778893e6d078db3cba0f49ee6b3c in / 
# Thu, 23 Apr 2020 20:42:37 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 23 Apr 2020 20:42:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 23 Apr 2020 20:42:48 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 23 Apr 2020 20:42:50 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 12:21:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 12:22:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 24 Apr 2020 12:25:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:beed3bd0a281cacead564771f079ed9ee8b272a2ed0e28f533e188f3d21fee6e`  
		Last Modified: Mon, 06 Apr 2020 15:40:20 GMT  
		Size: 30.4 MB (30400298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae14d2411b83450b8afe92058b998540c56ec42f1ddd7581e8e9fe629c442f89`  
		Last Modified: Thu, 23 Apr 2020 20:48:44 GMT  
		Size: 35.2 KB (35198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82678240be3a5c783512ff7336f2b10837ae126958bc6bd1b476a8d039c08771`  
		Last Modified: Thu, 23 Apr 2020 20:48:44 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7307ad4f24078fd763b41ec7c1772f2fd5238fed1bae36c5d42d28ec9adbffb9`  
		Last Modified: Thu, 23 Apr 2020 20:48:44 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d36cc2849670e80533ecb9cbd2eac7fa6d1b8fa2d318c78f419a766f192512ae`  
		Last Modified: Fri, 24 Apr 2020 13:16:17 GMT  
		Size: 6.5 MB (6494635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d6c79fe8ac5727136d9f0b8c1f3ed700a2394a061cf96ca5d0faa5e36be5c3c`  
		Last Modified: Fri, 24 Apr 2020 13:16:15 GMT  
		Size: 3.7 MB (3660114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c2ca9d90bce1a137acb71a0da13cdc691ab699a5ca31ca656f3101c0af1dbdf`  
		Last Modified: Fri, 24 Apr 2020 13:16:53 GMT  
		Size: 53.6 MB (53584713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:78c5746d4f657f9c7dffa15fbe4a980d0873c54a9e129a837e467dd303ef850f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **79.0 MB (78977452 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e8360e7cb787f35bcafd26f1952388233b160f6c66afb444799604046a47ce2`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 23 Apr 2020 17:52:20 GMT
ADD file:ea66ef2a01c547f771866bfa221969f8a30489c28d2a81be8dde7f40e73da33b in / 
# Thu, 23 Apr 2020 17:52:26 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 23 Apr 2020 17:52:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 23 Apr 2020 17:52:30 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 23 Apr 2020 17:52:31 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 07:47:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 07:47:26 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 24 Apr 2020 07:47:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:13b4c2e4bb97a2a80bb0e557eeba41e4adea0f5e18352e359bca3f847193899c`  
		Last Modified: Mon, 06 Apr 2020 15:41:16 GMT  
		Size: 25.4 MB (25365338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:471a80e39fb485b86610de915eaaad3d867cc97e460b6da3bb656e03520e8a63`  
		Last Modified: Thu, 23 Apr 2020 17:54:13 GMT  
		Size: 36.2 KB (36171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdb0c128ddabc6a980ec71426ade04fc9bba2e1afcdc243e2d09c316b635f814`  
		Last Modified: Thu, 23 Apr 2020 17:54:13 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:678052ac148ee123df2f0773eb3a0f5f90490ada8b9a5705363b18a2f45fbe88`  
		Last Modified: Thu, 23 Apr 2020 17:54:13 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25f640adbeff299c912d08ab0af607594ced4b9aa1bd9d665db1e5ed89ec216f`  
		Last Modified: Fri, 24 Apr 2020 07:54:38 GMT  
		Size: 5.8 MB (5769567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d3e24881318a773aa24c9ceaa07ca1bd45b6316b03d38ee7748e1679e140fb8`  
		Last Modified: Fri, 24 Apr 2020 07:54:43 GMT  
		Size: 2.9 MB (2916178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc2cc67fe40d21fe51c1e90a25fe30656c1cdd6e0467f4a727e9d900a2d37de4`  
		Last Modified: Fri, 24 Apr 2020 07:54:56 GMT  
		Size: 44.9 MB (44889160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
