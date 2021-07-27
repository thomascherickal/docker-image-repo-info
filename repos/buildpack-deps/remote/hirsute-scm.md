## `buildpack-deps:hirsute-scm`

```console
$ docker pull buildpack-deps@sha256:e03a0154c04ce601f22cbeb97f1213a8e524a5531889f08183f76bac6633f8fa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `buildpack-deps:hirsute-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:03c440ab93f47f6f25a8234febc88184480f28020791200b902ad758cc4fc7fa
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.5 MB (84470558 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:823cef2ec1834c9343ac135b8763c224793328b28dd2afae1dad1a2da3016cac`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:54 GMT
ADD file:6ae44786caae9af1c6b70dc9cc244e7d4e06fffc0696f68877527d69aa3fc735 in / 
# Mon, 26 Jul 2021 21:21:54 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 21:54:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 21:55:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Mon, 26 Jul 2021 21:55:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4451f5c7eb7af74432585f5ebfbeb01bbfc87ec4a74dc93703bdd89330559cd1`  
		Last Modified: Mon, 26 Jul 2021 21:23:44 GMT  
		Size: 31.8 MB (31837572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a0f50de6f11a7b6e208c43425014772ef0610d5f771979c6704e166be5c0499`  
		Last Modified: Mon, 26 Jul 2021 22:13:33 GMT  
		Size: 5.4 MB (5431174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03bfd280fb76c1b9717ecd762750a8e603d628c6cffebe143f0b34966a47bae5`  
		Last Modified: Mon, 26 Jul 2021 22:13:32 GMT  
		Size: 3.7 MB (3661446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cde9939f009cb8ebf9ee9b4f6b6f99c0a7ca437c96b046a6345f065cbfcc3dde`  
		Last Modified: Mon, 26 Jul 2021 22:13:53 GMT  
		Size: 43.5 MB (43540366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:hirsute-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:c6a571a602edab91b448ce62b430ca45c7ad7576a84aa8dd8b5c25283ab0642a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.8 MB (74806580 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5daa09014953167a85d14e2635dee913d419c47f5c18660e58ca04445481f7d3`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 23:21:58 GMT
ADD file:5175798ab209bbc3941a05787751ecf9e7ba0b4e9cda31b044bd6d75e25976c8 in / 
# Tue, 13 Jul 2021 23:21:59 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 01:58:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 01:59:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 14 Jul 2021 01:59:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fb746c2c12b45d26860f880a6e953018e4e9b83f9de17d11528fa484e1eb0f9f`  
		Last Modified: Tue, 13 Jul 2021 23:27:31 GMT  
		Size: 26.9 MB (26853751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eece18331508c76042ad235a876e23b49181f5ec1a12bc249810a5c1054ecc4`  
		Last Modified: Wed, 14 Jul 2021 02:21:44 GMT  
		Size: 4.9 MB (4858455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29ceee6719a049da986bf7137392215103a2329991689f89b7c21e4d6c154ea0`  
		Last Modified: Wed, 14 Jul 2021 02:21:42 GMT  
		Size: 3.1 MB (3138473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b42a764a798d56ca11ab0dd698ae53b182225ec31f170dcb1be9839ec6479ff6`  
		Last Modified: Wed, 14 Jul 2021 02:22:26 GMT  
		Size: 40.0 MB (39955901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:hirsute-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:dc39d4d5ad2393f751cf3c63f3554a86fd36ec973743ec05e74c87c96be0f1a2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.9 MB (82871381 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d45b3ee151b13a9ba4dfa1e59a49779f6fd06172ce632529f3c030bc2ebda616`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:49:12 GMT
ADD file:878284607eb47bd96d58adc1bce14366656e20fede92cc0ff58787c14419cffe in / 
# Mon, 26 Jul 2021 21:49:13 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 22:32:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 22:32:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Mon, 26 Jul 2021 22:32:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e34e08490be30f2dbe7ff29e0668c6e5aeba97f012896805dc1c38253e41bf42`  
		Last Modified: Mon, 26 Jul 2021 21:51:45 GMT  
		Size: 30.3 MB (30299715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55f88e5c290191a11d04a6a70e2c9d084f4f65a3b98566dd7aa057aa01e790de`  
		Last Modified: Mon, 26 Jul 2021 22:42:41 GMT  
		Size: 5.4 MB (5402637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86e43382b5ae512202c4b72ab829799e18bf61bf87928a28767164981394ea8d`  
		Last Modified: Mon, 26 Jul 2021 22:42:40 GMT  
		Size: 3.6 MB (3637846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d15bb320d287ed358835906f8dfabfecbcf99b47c08f1fafb1b0e95ca69ab20`  
		Last Modified: Mon, 26 Jul 2021 22:43:00 GMT  
		Size: 43.5 MB (43531183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:hirsute-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:fd35c4a1dbb59be60310176f265c1b3df47b76f31104f8e4a7867e159252dd56
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.5 MB (97488425 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd5c5afb32677672a0074e8a5de548b644593d70677cd70e4545a7b71c282150`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 23:23:07 GMT
ADD file:20ba7c85b0d967e38fdb53a91f37ff0266687978ecc0791861d4d1afb8c79899 in / 
# Tue, 13 Jul 2021 23:23:15 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 04:38:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 04:39:15 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 22 Jul 2021 04:41:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2aeaf089064656dca36cf8480e9c7933a8c61fcc2a4c009ac61cbe442299cb68`  
		Last Modified: Tue, 13 Jul 2021 23:28:23 GMT  
		Size: 37.4 MB (37353027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e56fc28c2da5e76c5798bfbc3de1f85434a42d191df7391b5ab1329ea4f8953`  
		Last Modified: Thu, 22 Jul 2021 05:22:49 GMT  
		Size: 6.1 MB (6132655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9375a3d4e03a069ebacb822be250889976e19ca796cf3cb46a35c232e7b684bb`  
		Last Modified: Thu, 22 Jul 2021 05:22:43 GMT  
		Size: 4.5 MB (4523285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf67f7cc14051aa9f2a70c724250b91f8118dc7b56fa2d68f567c91d594e4954`  
		Last Modified: Thu, 22 Jul 2021 05:23:47 GMT  
		Size: 49.5 MB (49479458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:hirsute-scm` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:c7feb8b2814ea8ded0a17260a7a7ac99bad50629756985a26a74b390710e1d1c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.6 MB (75595229 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:50a0dfbd696fcfe90ca2bb0e5b1f657720ce568c85d30575fb93c6565517296c`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 23:24:43 GMT
ADD file:399cdf15e2e703457111e0585186fa94182dcefce41f795abd41eddd1b10cefd in / 
# Mon, 26 Jul 2021 23:24:44 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 00:16:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:17:26 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 27 Jul 2021 00:20:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8f03e05f8f3a48ff7994fd656018adf1f6bd707a2827d3bce0fa7435fafe04db`  
		Last Modified: Mon, 26 Jul 2021 23:44:22 GMT  
		Size: 27.1 MB (27140041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b18328c2ee0bb5276608140b8a8467b6a2ee03da83bc425802e0b076060fc29`  
		Last Modified: Tue, 27 Jul 2021 01:10:03 GMT  
		Size: 4.9 MB (4945324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3afb0382af3d5aa29a9736f3967604d202347f0fa55cf43d804d2b204bf6d3f1`  
		Last Modified: Tue, 27 Jul 2021 01:09:59 GMT  
		Size: 3.2 MB (3177613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:039d531e9f9a40c9a15969b59f3504018fbb8782d1dc9c079e15a99c5f1b4349`  
		Last Modified: Tue, 27 Jul 2021 01:12:00 GMT  
		Size: 40.3 MB (40332251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:hirsute-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:bf8ff828a8c44bbab2367facb42dcde50721599bf5efa35a5643a8200479c90d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.7 MB (90749117 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10390433921267d86fac2e3e998d424494e12fae0488134e025e29c223695d3e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 21 Jan 2021 04:02:00 GMT
ADD file:8ec30abb851d24263f13b8ab93a9889626368053d325848b2f951e43ccac9a0c in / 
# Thu, 21 Jan 2021 04:02:07 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 04:02:09 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 21 Jan 2021 04:02:11 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 04:02:12 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 05:24:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 05:25:15 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 21 Jan 2021 05:25:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:35d604bd00566c6cbc331e49db9228af41b973581b365975622efcddfda24580`  
		Last Modified: Thu, 21 Jan 2021 04:04:14 GMT  
		Size: 32.5 MB (32534356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8645fe124321a0a9ceca773d8bd654c8edfb63087f69654dc33b005cd936031`  
		Last Modified: Thu, 21 Jan 2021 04:04:09 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:811acaaa59ef2c29c645ec90173a876498cec8129d2051e6826881ba068508fb`  
		Last Modified: Thu, 21 Jan 2021 04:04:09 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1c0a035e1b4479247e30498cb38c95743838097221a8aafc70ede4da8e1b6bf`  
		Last Modified: Thu, 21 Jan 2021 05:34:30 GMT  
		Size: 5.7 MB (5691508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:476bdd8305678676c465817a601000b79a702ef2feb7d9fc199dd171304f9712`  
		Last Modified: Thu, 21 Jan 2021 05:34:29 GMT  
		Size: 4.5 MB (4458912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9928f3c621a6ce2274dfc19b3cdbaa1fb5d4b0bb2c1e5b4e0a4bcd581247ff79`  
		Last Modified: Thu, 21 Jan 2021 05:34:47 GMT  
		Size: 48.1 MB (48063304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
