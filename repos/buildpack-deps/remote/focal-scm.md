## `buildpack-deps:focal-scm`

```console
$ docker pull buildpack-deps@sha256:f0b959c9b5fed6e0e384b684296f2fb187525da6dea4a15f32cf4d58ce85de0a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:focal-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:30bfb154b6a70126bdd5ec5f9d68c4c64d681916eac4b3867456ee094ee8c97d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.6 MB (99567343 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90128fc9826099b181888bfaf4e0eab6fe4f2169ab030573770ccd0809cc5134`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 19 Aug 2020 21:14:34 GMT
ADD file:9f937f4889e7bf6467d34e7ac4f093054993a93399443dc7469d53750a62234f in / 
# Wed, 19 Aug 2020 21:14:35 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 Aug 2020 21:14:37 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 Aug 2020 21:14:38 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 Aug 2020 21:14:39 GMT
CMD ["/bin/bash"]
# Wed, 19 Aug 2020 22:24:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 22:24:12 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 19 Aug 2020 22:24:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:54ee1f796a1e650627269605cb8e6a596b77b324e6f0a1e4443dc41def0e58a6`  
		Last Modified: Wed, 29 Jul 2020 15:19:55 GMT  
		Size: 28.6 MB (28558017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7bfea53ad120b47cea5488f0b8331e737a97b33003517b0bd05e83925b578f0`  
		Last Modified: Wed, 19 Aug 2020 21:16:56 GMT  
		Size: 32.3 KB (32336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46d371e02073acecf750a166495a63358517af793de739a51b680c973fae8fb9`  
		Last Modified: Wed, 19 Aug 2020 21:16:55 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b66c17bbf772fa072c280b10fe87bc999420042b5fce5b111db38b4fe7c40b49`  
		Last Modified: Wed, 19 Aug 2020 21:16:56 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed4be23e86feed0329609922bc76125d36578b16149d7735932c1379565d6f68`  
		Last Modified: Wed, 19 Aug 2020 22:34:56 GMT  
		Size: 6.9 MB (6860022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6fdcd42dec2742f4f567d9faa5e8b238b548573a0b9a28c46bd34a9fde46e1c`  
		Last Modified: Wed, 19 Aug 2020 22:34:55 GMT  
		Size: 3.6 MB (3565493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9e6e5b03a2db596d5cd47364ced0e8706fee9cf73849df1109d3d252fa004b5`  
		Last Modified: Wed, 19 Aug 2020 22:35:19 GMT  
		Size: 60.6 MB (60550465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:4322c35e857cfe075b4e9015584cad3e8648524100e5979a2a6ea32aa2804409
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.2 MB (88219560 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf837e7a5163ae94bedb6968f6c494760239f144e8f68697c9ffa72867af36cb`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 19 Aug 2020 21:45:35 GMT
ADD file:bfe01aadc11b91c906991cb5cb5fe488e49855783a0cd38cf51edd0aa6bc8b98 in / 
# Wed, 19 Aug 2020 21:45:38 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 Aug 2020 21:45:41 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 Aug 2020 21:45:43 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 Aug 2020 21:45:44 GMT
CMD ["/bin/bash"]
# Wed, 19 Aug 2020 23:37:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 23:37:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 19 Aug 2020 23:39:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ceea98c5fa08244c844238a2ce484fa14c30ffa489edb9895fba50b77a7cfa60`  
		Last Modified: Mon, 03 Aug 2020 15:51:06 GMT  
		Size: 24.0 MB (24037952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f3da9874eeead204573f212800c6ade25da830235c0ad3548c26f722eace05b`  
		Last Modified: Wed, 19 Aug 2020 21:47:26 GMT  
		Size: 32.3 KB (32341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c68fbe4d8e6dd4748556d6ef14fdd8135f7443715086c717cdf274c94ecec8ad`  
		Last Modified: Wed, 19 Aug 2020 21:47:26 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03d3cf167993a17554b119a4afa4c1bc5ec478015827bf1e1f4ca23296e43f50`  
		Last Modified: Wed, 19 Aug 2020 21:47:26 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6110f525eb1611c149adb549c27097f3996d110da6cd54063a19bb32d80ec4e6`  
		Last Modified: Wed, 19 Aug 2020 23:55:24 GMT  
		Size: 5.9 MB (5855155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06511a717911fe1422ef4a1db0d0b24881aefa03f603b022a9ab17b4298fd69c`  
		Last Modified: Wed, 19 Aug 2020 23:55:23 GMT  
		Size: 3.0 MB (3044740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a102efff068b33d673c4980555704db251542daecaca0579c9c6b4f3772a1716`  
		Last Modified: Wed, 19 Aug 2020 23:55:52 GMT  
		Size: 55.2 MB (55248335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:10afb9c64c973bbe63da59e82daf7aab9b281ccdedb8dddebd4a44425efbb071
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **98.1 MB (98059975 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ebb3a927ffc43f2ba91c8c184df771f58d0f8dc84a56313ccaf9663c01f9b6fc`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 19 Aug 2020 21:30:23 GMT
ADD file:a332d170aaa2d4c28c85289b62d33de68027ce4d6b0616292ee2252dfdf2628b in / 
# Wed, 19 Aug 2020 21:30:27 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 Aug 2020 21:30:29 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 Aug 2020 21:30:31 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 Aug 2020 21:30:32 GMT
CMD ["/bin/bash"]
# Wed, 19 Aug 2020 22:03:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 22:03:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 19 Aug 2020 22:04:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:61ca5746b6ffb91caaaa0eb4b9678ae147ad24bd40ac203758a90af376976f98`  
		Last Modified: Wed, 29 Jul 2020 08:25:33 GMT  
		Size: 27.2 MB (27162745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8d07cd4558d7ea5ba152468ba362cbf62a56cfab14976467187d3943013a932`  
		Last Modified: Wed, 19 Aug 2020 21:32:25 GMT  
		Size: 32.3 KB (32335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b56ef536d7ca531a0dce4a70ac7ad7d9b7ed27c56c7f0953bbec370e4299b951`  
		Last Modified: Wed, 19 Aug 2020 21:32:25 GMT  
		Size: 846.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:177d5c7c4a6e93095601576a7663dde336974f6a96329ae2a613511662ed8744`  
		Last Modified: Wed, 19 Aug 2020 21:32:25 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:839c7e889f293fd2ccbcce7d51d38ff0f526b2316f548b6b87f93a982586b721`  
		Last Modified: Wed, 19 Aug 2020 22:13:16 GMT  
		Size: 6.7 MB (6723920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d755996aa0edd6b45422b915be99b4f3835b18ed78d94552db2a2dddf22c5031`  
		Last Modified: Wed, 19 Aug 2020 22:13:14 GMT  
		Size: 3.5 MB (3541956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbcc5a70ec61b7d7d78f9c88ad296b88f697245ecdfa65037712db27222d258f`  
		Last Modified: Wed, 19 Aug 2020 22:13:41 GMT  
		Size: 60.6 MB (60597985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:9f020b13cae28ed205cc6f2a45e5d7604584b7cc225da3e374d8e38476bbde80
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.9 MB (114860239 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f90beae01b8c712937b06db83c9e767dfa5035a4d8fe98ea3a04e6efe9c902cd`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 24 Jul 2020 14:35:30 GMT
ADD file:fec1d8aac4ab3a3c2326e15808c04b0df4c06c2c4e66d3f34e3e31d3408fd793 in / 
# Fri, 24 Jul 2020 14:35:51 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 14:36:13 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:36:36 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:36:43 GMT
CMD ["/bin/bash"]
# Fri, 24 Jul 2020 18:02:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 18:03:22 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 24 Jul 2020 18:10:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4739cd2f4f486596c583c79f6033f1a9dee019389d512603609494678c8ccd53`  
		Last Modified: Mon, 20 Jul 2020 15:51:10 GMT  
		Size: 33.3 MB (33279182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f57f5c67707a22a55ae858c6c54f236321b919889f34c321e1a3cc35b9a7988`  
		Last Modified: Fri, 24 Jul 2020 14:42:20 GMT  
		Size: 32.2 KB (32166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:169b0395dde9514c1a521632a61afda1494fe836f816badcab196bd067b4891c`  
		Last Modified: Fri, 24 Jul 2020 14:42:20 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b459fe5e4dff59e4cc2b4b5207df42a369d6f0ac774f26c55184b3ccd491996`  
		Last Modified: Fri, 24 Jul 2020 14:42:20 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:595dfa7aa2023f65b441c28c9412f7ceaefa19a7a2dd3fb399a6ae5ee57937b6`  
		Last Modified: Fri, 24 Jul 2020 19:15:09 GMT  
		Size: 7.8 MB (7813527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8940bf8a991181bc1642a5f54b6d000b8b1a466c7edb85172bb5e9e361766449`  
		Last Modified: Fri, 24 Jul 2020 19:15:04 GMT  
		Size: 4.4 MB (4399121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d101b17ef943c6c1b34f096b192971235fd78ba6d787fe3c9ba518fb3961282e`  
		Last Modified: Fri, 24 Jul 2020 19:16:46 GMT  
		Size: 69.3 MB (69335201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:b47d838ebdc413f494bcbb7ca836c2369ee7e568a14724d30b51c0553dae5dcf
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.7 MB (97731698 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09b2f2dcfef495004d90b1c0d1149ead6699ff3570d270c6d0bb44167061abbd`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 19 Aug 2020 21:10:17 GMT
ADD file:b512f53b78fef64c2c5c665a881883d34a04c2a26116015454fe7d4b41fefc15 in / 
# Wed, 19 Aug 2020 21:10:20 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 Aug 2020 21:10:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 Aug 2020 21:10:21 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 Aug 2020 21:10:22 GMT
CMD ["/bin/bash"]
# Wed, 19 Aug 2020 21:46:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 21:46:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 19 Aug 2020 21:46:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e743f10403cdde6a752838a8e4dd09fda2f8704eb11d2831c8bad7d9eaf27b21`  
		Last Modified: Mon, 03 Aug 2020 15:57:01 GMT  
		Size: 27.3 MB (27271952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58a230d59853de2044db12e7d10ebebc2f3ca91fc50cb45c0296e3449b519188`  
		Last Modified: Wed, 19 Aug 2020 21:11:18 GMT  
		Size: 33.0 KB (32966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8105b7c36a53d2e52f8798d6301d96e4538951b4c5f96a298c9bfcc9cd60422e`  
		Last Modified: Wed, 19 Aug 2020 21:11:18 GMT  
		Size: 845.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43a2dcb94208ae8b5626b66d01e401d21bca6d0de008a445e1827a0fce7e72ba`  
		Last Modified: Wed, 19 Aug 2020 21:11:18 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:913a02c204e8c5003175dcf005532558b9eb20de315234ef553140f23ea7b7c4`  
		Last Modified: Wed, 19 Aug 2020 21:53:17 GMT  
		Size: 6.5 MB (6547232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:181e17f6491b425d2cf59e1d10d02e3888063ab2906cbf3be1732c0943bd0b77`  
		Last Modified: Wed, 19 Aug 2020 21:53:16 GMT  
		Size: 3.6 MB (3563369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03fda8c3e2699086a49e3fc51ce3bb584d3eefa4e77ab785bdc0ed0606f889e6`  
		Last Modified: Wed, 19 Aug 2020 21:53:33 GMT  
		Size: 60.3 MB (60315147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
