## `buildpack-deps:xenial-scm`

```console
$ docker pull buildpack-deps@sha256:702babfd524e6524bd440f56dd7c9592a3cbcfc675ea114efa8d4cd8a6d8d138
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:xenial-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:d6fe086038a06ae3ecbd4d8cbafdd6781893fc8cffa8cfb63a06d6e8b91421c6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.2 MB (96194248 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d19b9e5ac076fc24a3c202ded649fbc93a6de904da2a85eb0b4be31db54dd330`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:32:06 GMT
ADD file:4dd75f16753c9c921fd05b1d0ed5b425d74d87405a76a0b3afcbf9723a50d1ce in / 
# Thu, 17 Jun 2021 23:32:07 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 17 Jun 2021 23:32:08 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 17 Jun 2021 23:32:09 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 17 Jun 2021 23:32:09 GMT
CMD ["/bin/bash"]
# Fri, 18 Jun 2021 01:02:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:02:07 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 18 Jun 2021 01:02:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:61e03ba1d4149ac4eb681c6bf75aef8ac4b3f0d6fbb08e9623c4089889396fc8`  
		Last Modified: Sat, 12 Jun 2021 00:25:16 GMT  
		Size: 46.5 MB (46496785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4afb39f216bd4e336f9b78584bae0f6bcb77150107471d8d67d3b8abfbdea46a`  
		Last Modified: Thu, 17 Jun 2021 23:34:09 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e489abdc9f902f737bfef2c0c7ff5c35ca9b3ca11e73405a472f31a25f2dcc69`  
		Last Modified: Thu, 17 Jun 2021 23:34:08 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:999fff7bcc2450fcf1210182802f3907e35cd7cf7569568bd2a179b9144d9c57`  
		Last Modified: Thu, 17 Jun 2021 23:34:08 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a8e0bb8deb4f1e4f4b65af4c59761e74cc40622594aac268f41f8aaa44716e9`  
		Last Modified: Fri, 18 Jun 2021 01:10:02 GMT  
		Size: 7.8 MB (7790447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:270c707205faec2464cd25c5da2f432bfa07c092915bfa0c3bceee0fa525f3fc`  
		Last Modified: Fri, 18 Jun 2021 01:10:21 GMT  
		Size: 41.9 MB (41905470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:xenial-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:062f83cb3bf647fa3ffc4c8566c54241ee15253be98f9cc32f0aa31cdf0d2019
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **85.1 MB (85108315 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8b7751a3ced674f5b76dede2741868f99beb020812ccb75e06e9c6f954655e8`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 13 Jul 2021 23:23:36 GMT
ADD file:ef24ce1c15acdd071b2d61cd27d2840f1fa5eda4937dfe8746997eb677b1451b in / 
# Tue, 13 Jul 2021 23:23:39 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 13 Jul 2021 23:23:41 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 23:23:43 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 13 Jul 2021 23:23:44 GMT
CMD ["/bin/bash"]
# Wed, 14 Jul 2021 02:05:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:05:51 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 14 Jul 2021 02:06:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:bee35c084ef2789f844b87c031d55b07186255622024a15b526838f71500485a`  
		Last Modified: Thu, 17 Jun 2021 23:36:42 GMT  
		Size: 40.3 MB (40312433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82fe22c8ad83979c361a3c4d3e782f4a311856511042ff7a107356ea1e21e694`  
		Last Modified: Tue, 13 Jul 2021 23:29:28 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a6b9c580e9f54a056423dc1ea3c0923d41d6f18b5abd11a5364db40a8f79fc7`  
		Last Modified: Tue, 13 Jul 2021 23:29:28 GMT  
		Size: 511.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f964743b5fd175c6240d9e2a4d592ff013029f4edea14efaec9813e6c65607e5`  
		Last Modified: Tue, 13 Jul 2021 23:29:28 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8185dbb38ebe165f6bc0b1ed706280d0ff8e905cdf2514f1d1e7655d4ca4c599`  
		Last Modified: Wed, 14 Jul 2021 02:26:54 GMT  
		Size: 6.6 MB (6631659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:323d8e1609db7157faaf70540cc34727009ca838954f9dfaca2c3879f81c41f4`  
		Last Modified: Wed, 14 Jul 2021 02:27:34 GMT  
		Size: 38.2 MB (38162692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:xenial-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:7789432a00873054b3545618049bc3ad47445625c752c8595acb53902d9b1a55
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.9 MB (87888648 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dde0c3d0cde9be02d8378ac3b95ede47bd0cacdc1c8c2b076b1ce0b828a23b2d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:54:40 GMT
ADD file:2675f90ace0ec88b2cdadc737d15d701b544bf2113480e898d0014a79dca13c7 in / 
# Thu, 17 Jun 2021 23:54:41 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 17 Jun 2021 23:54:42 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 17 Jun 2021 23:54:43 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 17 Jun 2021 23:54:43 GMT
CMD ["/bin/bash"]
# Fri, 18 Jun 2021 00:19:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:19:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 18 Jun 2021 00:19:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e2a24739a48e2c634f94c2cb69ead6b0ff1c84cedd9624eb29560b83c3eb6e0e`  
		Last Modified: Sat, 12 Jun 2021 00:25:19 GMT  
		Size: 41.2 MB (41239907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6732798425e9389fa6bd92caa59cd7de853b4cf01a7166724e26a430ec7211f`  
		Last Modified: Thu, 17 Jun 2021 23:57:28 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d0af2bd04c3cb9d221318d494c05b29dd4b7c46886de97baee11fbd40723ab8`  
		Last Modified: Thu, 17 Jun 2021 23:57:28 GMT  
		Size: 470.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:835469060484e7130eb258c8dfae8e4b1f8035c63bba23ab6e4f3e9b53a6cf1e`  
		Last Modified: Thu, 17 Jun 2021 23:57:28 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d705f2e3ef332ead85b43a8fb48db55afbf0571895d5e0eec464d2d652e473aa`  
		Last Modified: Fri, 18 Jun 2021 00:26:16 GMT  
		Size: 6.8 MB (6839003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1d68f38be1a6a6cff73b3a9fadb1667073a78f0aeee43f84556fc04a9279dfc`  
		Last Modified: Fri, 18 Jun 2021 00:26:35 GMT  
		Size: 39.8 MB (39808251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:xenial-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:ea7fc80b3b2aa152d5f199f5f804a4118922de6c45b8444265e06fb3a43286ee
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.6 MB (96640885 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:36951459e79c8565df4d8d36b41e3f5c33f0582e7b97df1d683fc26c7798d8f1`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:48:13 GMT
ADD file:405fb6ba2e4fcf060e027f7a0aad340b7aee637d50ec097aff59e15609bfc2c1 in / 
# Thu, 17 Jun 2021 23:48:14 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 17 Jun 2021 23:48:15 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 17 Jun 2021 23:48:16 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 17 Jun 2021 23:48:16 GMT
CMD ["/bin/bash"]
# Fri, 18 Jun 2021 00:11:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:11:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 18 Jun 2021 00:12:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:eca348360c85efd796e52ecf73e5add735eabf7e041356b47c87947e8a749e00`  
		Last Modified: Thu, 17 Jun 2021 23:49:12 GMT  
		Size: 45.8 MB (45815621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07150c0d356ea8abd3017d76adc6703dd76f0d1a9b03dfb86c9cb300b1a72d36`  
		Last Modified: Thu, 17 Jun 2021 23:49:03 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aaa5e08eb74cc48d87e687b4a660f7f9475de83f25661f2709740db81c41849`  
		Last Modified: Thu, 17 Jun 2021 23:49:03 GMT  
		Size: 517.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:febb5fbfe0775e00dd59ff4f626d510952d83748697c62d0c6d18cd9bc8a256c`  
		Last Modified: Thu, 17 Jun 2021 23:49:03 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a57c9be074ecc87d11deaf0b5771178e00cfbd91f8a31ae612372a1e5052bdd`  
		Last Modified: Fri, 18 Jun 2021 00:19:32 GMT  
		Size: 7.9 MB (7933154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45360778e7105c7e9af7c57eb94d78235bd752eff85b6f9f1b81fe21edb09f04`  
		Last Modified: Fri, 18 Jun 2021 00:19:55 GMT  
		Size: 42.9 MB (42890572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:xenial-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:7c731390a99a8647b0da956cf918497ceb2cdf1b05ba8305f55e33c4e27dfde4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.4 MB (100364602 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d1ec0492bf7b678d9bea3ca40a3bcc992b44dfd59a44c78527fa0c5fa1bc2b3`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 13 Jul 2021 23:25:11 GMT
ADD file:02f85c6f12364eaad4f80464effd781403b4c13c7732005ee3731d0d19a353c2 in / 
# Tue, 13 Jul 2021 23:25:25 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 13 Jul 2021 23:25:39 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 23:25:53 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 13 Jul 2021 23:25:59 GMT
CMD ["/bin/bash"]
# Wed, 14 Jul 2021 02:55:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:56:22 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 14 Jul 2021 02:59:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:77800700d823a40e3888379b1764dd49f1e6630a1848579e18e69c1dcc8f2558`  
		Last Modified: Thu, 17 Jun 2021 23:30:08 GMT  
		Size: 47.5 MB (47522284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0babf75a176b58db3a5df6096af29a306bf0ab34aed69816ecea017482b6ba6`  
		Last Modified: Tue, 13 Jul 2021 23:29:36 GMT  
		Size: 859.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aeb0805a3ad55f25fa2e52d341de43543d44705d05021e2d6a3ed9944915319`  
		Last Modified: Tue, 13 Jul 2021 23:29:36 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4421ae6a1a8096772ab2b5bb7d32cf300fbe5ffbe18cb6c742591febaf3bd7f`  
		Last Modified: Tue, 13 Jul 2021 23:29:36 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaa538407c039fa89484c0b7633543d422d242bb02e9f813952284af6da6916a`  
		Last Modified: Wed, 14 Jul 2021 03:28:32 GMT  
		Size: 7.7 MB (7693105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9c4028b9ddc607ca711efadce656bd48105dfb6d3faf101d2f3e81aa5935d43`  
		Last Modified: Wed, 14 Jul 2021 03:29:48 GMT  
		Size: 45.1 MB (45147707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:xenial-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:0d43270e2bfba25d8d92e52d555d47beb35ccb8ad89bc0d782839cf08c61aa9a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.3 MB (94299272 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0370f03fed3c04e04c4540aca53a522e94808dc854f9c634a7f506b10a5c6a2e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 13 Jul 2021 22:54:28 GMT
ADD file:fe2f2172ef6c28729fe2906a3edd50a39e2ff612da510584327898429dd0b2c8 in / 
# Tue, 13 Jul 2021 22:54:32 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 13 Jul 2021 22:54:34 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 22:54:36 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 13 Jul 2021 22:54:36 GMT
CMD ["/bin/bash"]
# Tue, 13 Jul 2021 23:46:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 23:46:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Jul 2021 23:47:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5e94e6b2e2a61afc38e8c32f4b5cadc2ec32d2f223781d4ee4203e2e6b096a37`  
		Last Modified: Thu, 17 Jun 2021 23:46:23 GMT  
		Size: 44.1 MB (44088123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dabfb1a7eacd3ce7cebc95a8e4a2552e56450e2ec1b036516b1bb09c4d22df48`  
		Last Modified: Tue, 13 Jul 2021 22:56:42 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c115486bffc8ae23d8bc9beb85e9cbd574b177de6a231bb437729902809aaf2`  
		Last Modified: Tue, 13 Jul 2021 22:56:42 GMT  
		Size: 470.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ddfacfd07c012e416dfec6566c58456afbfad6dd84efd5d26b0339376edb6f1`  
		Last Modified: Tue, 13 Jul 2021 22:56:42 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37cad89fa876f64f8213e6203320233397d4ff4d511e425bd17d65f3156a6c34`  
		Last Modified: Tue, 13 Jul 2021 23:53:12 GMT  
		Size: 7.5 MB (7522114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f00d06593b472f1cb38c4817774c1175db5435c933a2e026e4e0724ecbb3a0af`  
		Last Modified: Tue, 13 Jul 2021 23:53:26 GMT  
		Size: 42.7 MB (42687541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
