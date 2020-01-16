## `buildpack-deps:eoan-scm`

```console
$ docker pull buildpack-deps@sha256:91b6e8f2332c5c479eee74ab5b5fc27449a0eb5a14f6baddabeb46d924b73975
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:eoan-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:e635cf152c29f2bafc5fc879d280689f872df3d8328a320b6dbcf8c2e7396897
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **85.7 MB (85700377 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:664caac50be261cce41d3d815b415a4d38eeced4839306a9891bc8e447a71cc4`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 19 Dec 2019 04:22:52 GMT
ADD file:9cf0c9e2d83fd1f85ac0ca5e96b2fba6474f4bda7c20911811337fe11817a45a in / 
# Thu, 19 Dec 2019 04:22:54 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 19 Dec 2019 04:22:55 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 19 Dec 2019 04:22:55 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 19 Dec 2019 04:22:56 GMT
CMD ["/bin/bash"]
# Thu, 19 Dec 2019 07:29:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 19 Dec 2019 07:29:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 19 Dec 2019 07:29:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cc5a81c29aabc68f3accf136ad5d1738904898296a367f807e0afb82c2f76d6e`  
		Last Modified: Thu, 28 Nov 2019 16:34:20 GMT  
		Size: 28.3 MB (28272270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81c62728355f60c09e71f3706586cce3f15677526dccb3c47d25abd61ad46e1b`  
		Last Modified: Thu, 19 Dec 2019 04:25:19 GMT  
		Size: 30.6 KB (30581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed9cffdd962a232b1d4ac5c63042f1c3bd032ad7be970ad7d2bf2ab18a336781`  
		Last Modified: Thu, 19 Dec 2019 04:25:19 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a46f000fce20f9ea03fcec6689eb2208e780af6528ce7d851a1e287d0e96c22`  
		Last Modified: Thu, 19 Dec 2019 04:25:19 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e72e8b0d951ead0e6ef0ad9e865ecae5405c33385a24ea8975e888e6716db982`  
		Last Modified: Thu, 19 Dec 2019 07:41:04 GMT  
		Size: 6.5 MB (6511154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd178d4d1544f0f01ee5733f0ea8642e495243c617b5d15821521ba53886e66d`  
		Last Modified: Thu, 19 Dec 2019 07:41:04 GMT  
		Size: 3.5 MB (3516328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f17b21b0cf9cd26ee276a44910cbb1385690c0f600ea4848ed6a793044a10c8`  
		Last Modified: Thu, 19 Dec 2019 07:41:21 GMT  
		Size: 47.4 MB (47369034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:eoan-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:50796e879bee7f74d9f2cf48eed5df705d81db0bc7ba15fc4eccf2e159c79fc9
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.4 MB (75356507 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c129fcc29e13109caf3a9b0e2c31aee9aa6813be6c6c8ff67341bee211911b4`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 19 Dec 2019 06:11:05 GMT
ADD file:1d649875b914193de549cfee5af0147c9ba102f2a9ff6b1b9da1fce7bcdb8c96 in / 
# Thu, 19 Dec 2019 06:11:15 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 19 Dec 2019 06:11:23 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 19 Dec 2019 06:11:28 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 19 Dec 2019 06:11:30 GMT
CMD ["/bin/bash"]
# Thu, 19 Dec 2019 07:46:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 19 Dec 2019 07:47:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 19 Dec 2019 07:47:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0d9ed73febf75e7373e7cf94c3b56a7dbca57ece77a2936b9e104aa05bb57de9`  
		Last Modified: Thu, 28 Nov 2019 16:57:26 GMT  
		Size: 23.7 MB (23729416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a0ee2639229470d35e076f07de393afbc7996c074307da61d34b523eab703d6`  
		Last Modified: Thu, 19 Dec 2019 06:15:11 GMT  
		Size: 30.6 KB (30593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac6374b86e241049a98de23ce22789a03361d0db3d2e3bfc2e05607c9bc14f18`  
		Last Modified: Thu, 19 Dec 2019 06:15:11 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e010d470fd3c21c69efd25118eba9301df9b4e5e6586ddbdb807b4cee82e5aa9`  
		Last Modified: Thu, 19 Dec 2019 06:15:11 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a58a8f48bdf590d777082ac17237478735888814daa9f177c526bbcfc1a5ebb4`  
		Last Modified: Thu, 19 Dec 2019 08:01:41 GMT  
		Size: 5.5 MB (5529860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4a64b48ab7795f0dc8b8fda368504df08a44b5b3b25b87a0492df61ff9a12aa`  
		Last Modified: Thu, 19 Dec 2019 08:01:41 GMT  
		Size: 3.0 MB (2981428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d51cb926fd0f15900cd58a9534380a1d776dc27a5c1bd4c87d7eade9341a6400`  
		Last Modified: Thu, 19 Dec 2019 08:02:04 GMT  
		Size: 43.1 MB (43084170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:eoan-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:f5535a6075caa11955a4a26bbdb3a0f7b44c8a8a4b44b75bacd36d7cb252b922
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.2 MB (84162511 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:601efc6a021f6e8898640b556538505e14a5ac798831a67fd9223f1d47bfc1bc`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 19 Dec 2019 03:52:11 GMT
ADD file:ab7860d075764dd37397c3e6b5cbc424a20f7908293aec76a22f2ee8b74e938d in / 
# Thu, 19 Dec 2019 03:52:16 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 19 Dec 2019 03:52:24 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 19 Dec 2019 03:52:35 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 19 Dec 2019 03:52:38 GMT
CMD ["/bin/bash"]
# Thu, 19 Dec 2019 08:16:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 19 Dec 2019 08:17:11 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 19 Dec 2019 08:17:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:87616e97cc89200ca46486ff9c1aa984dacdac7d86cfae973850319782203732`  
		Last Modified: Thu, 28 Nov 2019 16:54:17 GMT  
		Size: 26.9 MB (26874945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07583dc448658d9c9966c3ed29abc9474a5cd3aba4fbf16daa34af3ca349568b`  
		Last Modified: Thu, 19 Dec 2019 03:56:10 GMT  
		Size: 30.4 KB (30421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1bfc19bd90414621995cb195c00410e195445c8a89a21abdc4e4bb36706de8a`  
		Last Modified: Thu, 19 Dec 2019 03:56:10 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e64eda46f22fb8ea87f48be3e7c0a31d18ad7c5743bda3162e5b9c3382d0db97`  
		Last Modified: Thu, 19 Dec 2019 03:56:10 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffefd37a86721e1b893f6fe101ecaba34d1dfb713cb2dda10a3e1e26058dc7ef`  
		Last Modified: Thu, 19 Dec 2019 08:31:18 GMT  
		Size: 6.4 MB (6368516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93f588a7e4f146b9dd3ea6168dbca57ff4a5beffee6bdfe6e5d8855f8e3f7b8e`  
		Last Modified: Thu, 19 Dec 2019 08:31:18 GMT  
		Size: 3.5 MB (3510060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2650cee108cd4ffc4651807ade67e56d4f06b5cc05b1927ad41d94a687ad5db2`  
		Last Modified: Thu, 19 Dec 2019 08:31:41 GMT  
		Size: 47.4 MB (47377532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:eoan-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:7233dd762060710a18366065a4ce4249494ae2a13399dd043846cdd189a15892
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.7 MB (88684351 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa79362e4dae79e7bf76e8550d994047c45d07d121a4824ed31d6e956dec923c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 16 Jan 2020 00:39:21 GMT
ADD file:4c13e98f6fc840e5da5cb0f7785a8e82a92e72983a5cd05d0e5bddab446fee18 in / 
# Thu, 16 Jan 2020 00:39:22 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 00:39:23 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 00:39:23 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 00:39:24 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 01:22:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 01:22:51 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Jan 2020 01:23:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c291135c9b01620912513c1f0d8a0504da7354edc25070352cc18166738a84a3`  
		Last Modified: Thu, 16 Jan 2020 00:40:22 GMT  
		Size: 29.0 MB (29041359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:294dba4d145edfc7c6ca873f6b60ed7ae65c2c3970ba7caca8cef7c8fefe0b33`  
		Last Modified: Thu, 16 Jan 2020 00:40:15 GMT  
		Size: 30.7 KB (30693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a30417049082ff7a0aa58802fb490045b812cc7756938f3d86b99233e174f97`  
		Last Modified: Thu, 16 Jan 2020 00:40:15 GMT  
		Size: 846.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0d0f1731d2bb5ffe106dc27137344e67f68f8667937027f4ba0d0d439eab39f`  
		Last Modified: Thu, 16 Jan 2020 00:40:15 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83eb774020dcccdf794257e9bd87184d1c9183ed4ffb22b1a997a236e58bf1c0`  
		Last Modified: Thu, 16 Jan 2020 01:32:38 GMT  
		Size: 6.8 MB (6839651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31f9fe4a81a6b01eafcd211c7899e28e9f065491d964930b48f901bd17c7c72e`  
		Last Modified: Thu, 16 Jan 2020 01:32:37 GMT  
		Size: 3.8 MB (3809439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:155d0a19a1738038412e507aa67192ee499ae0ec3b564db251280b4fa45344a6`  
		Last Modified: Thu, 16 Jan 2020 01:32:57 GMT  
		Size: 49.0 MB (48962201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:eoan-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:70df3042a565f5052a2f33d274a8c53ef00560070e136e7d4a0148b51c2464cf
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.7 MB (99694859 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c60d174f1736bef7141c2f337459d8b3e1aa8a56d923c7567eb91857db8506f`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 19 Dec 2019 04:19:15 GMT
ADD file:65740b49d4423d432ed0f452be965c7914820e1c5049a89b6d7da7ce623457a3 in / 
# Thu, 19 Dec 2019 04:19:20 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 19 Dec 2019 04:19:26 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 19 Dec 2019 04:19:31 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 19 Dec 2019 04:19:33 GMT
CMD ["/bin/bash"]
# Thu, 19 Dec 2019 09:38:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 19 Dec 2019 09:39:30 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 19 Dec 2019 09:41:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5ea80ec4eb655fb9a87d258b7dd3b1479f2bf1468624049062b2ed2d993db09d`  
		Last Modified: Mon, 02 Dec 2019 15:36:38 GMT  
		Size: 33.0 MB (33004101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab887723a4b5c4fe94a3ed96e01f50b3eedb239717df0658a69b9be70c6b6c75`  
		Last Modified: Thu, 19 Dec 2019 04:25:27 GMT  
		Size: 30.4 KB (30447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cab79b96749c4d30e6e00c6301db28f910d3465bad04d918f501d1f9be5763c`  
		Last Modified: Thu, 19 Dec 2019 04:25:27 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbd7ec6dc5602f7ec303abba71aee3459cca1128c6f491e69cfcc1d007ac23a6`  
		Last Modified: Thu, 19 Dec 2019 04:25:27 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a39fe44525bf18b92cc80600e097ca6273ecba5e1784ec1f1084d75d6965b923`  
		Last Modified: Thu, 19 Dec 2019 10:29:12 GMT  
		Size: 7.4 MB (7418701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9adc91137c102bcbd34438d8d740eed0250fcd9180b2b3aeca3caf50ab333394`  
		Last Modified: Thu, 19 Dec 2019 10:29:11 GMT  
		Size: 4.5 MB (4462027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbdbbc486798b63c73586e73747c4a60bfe2f851e87d2c075eef562ef46868a0`  
		Last Modified: Thu, 19 Dec 2019 10:31:03 GMT  
		Size: 54.8 MB (54778543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:eoan-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:657848e03c0bee0400a37900870ad0d9acd5204cad1e56e87f9ea7332c0e6641
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.2 MB (83241220 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f63c8d771ab8a4c3a9e1ed0c0b5e8c07456e0d4a38a2f44c0dbce17dce8b7988`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 16 Jan 2020 00:45:39 GMT
ADD file:d11f2d3df95bd823f561f866f276b3e1133a10b4fd24cd0af59926336d9c7fdc in / 
# Thu, 16 Jan 2020 00:45:40 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 00:45:40 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 00:45:41 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 00:45:41 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 01:27:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 01:28:08 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Jan 2020 01:28:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9f8ad320e3910721bade3f69e3e74f5511ad7245eafdd183ab893dbae79842dd`  
		Last Modified: Thu, 16 Jan 2020 00:46:37 GMT  
		Size: 26.7 MB (26682542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e16061b26415dae4023599d79fe632126958d9fff628811e9eb72e6adc656eb3`  
		Last Modified: Thu, 16 Jan 2020 00:46:29 GMT  
		Size: 31.1 KB (31101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b599496909204045d2cdfb755a0ccd4b24ccb49453c1eee59a0d492116d92191`  
		Last Modified: Thu, 16 Jan 2020 00:46:29 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:436a550ce4958735714f310a9a407b7b63e71e5aefda4ad33e3dc544c5905daa`  
		Last Modified: Thu, 16 Jan 2020 00:46:29 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccb1dc48f917af334169d5f5577144fa5617932504db6cd77242eec024099815`  
		Last Modified: Thu, 16 Jan 2020 01:34:21 GMT  
		Size: 6.1 MB (6136750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e40dba93fae8b1cc3eeddcb3f58dd229b7c561bc6abbb803f6afb4ba74e1dc5e`  
		Last Modified: Thu, 16 Jan 2020 01:34:21 GMT  
		Size: 3.4 MB (3432414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb12efdd91f40d153ceb81d5647477bd3bbb1a49e34129fb35c4d519ffef5017`  
		Last Modified: Thu, 16 Jan 2020 01:34:39 GMT  
		Size: 47.0 MB (46957408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
