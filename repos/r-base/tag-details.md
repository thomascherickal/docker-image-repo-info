<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `r-base`

-	[`r-base:4.1.3`](#r-base413)
-	[`r-base:latest`](#r-baselatest)

## `r-base:4.1.3`

```console
$ docker pull r-base@sha256:3d2448e9077ecbe673c662acbefcbacf6e3515cf5507fdac0f37765208013425
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `r-base:4.1.3` - linux; amd64

```console
$ docker pull r-base@sha256:567cb8968827c97e1fb788e23e9a3acf8a5d95c6dbeeb88a48ae438e05fe2da0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **333.8 MB (333807683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f987362a590dd6659467713d5f78324a8965c8c2a6abc464f5613da3e969aa96`
-	Default Command: `["R"]`

```dockerfile
# Wed, 20 Apr 2022 04:45:35 GMT
ADD file:fb66d619557384a14385fa7b5371be954594c4aff1700edcbd9cff422c3498f0 in / 
# Wed, 20 Apr 2022 04:45:35 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 13:25:30 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Wed, 20 Apr 2022 13:25:31 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Wed, 20 Apr 2022 13:25:41 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 13:25:43 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Wed, 20 Apr 2022 13:25:43 GMT
ENV LC_ALL=en_US.UTF-8
# Wed, 20 Apr 2022 13:25:43 GMT
ENV LANG=en_US.UTF-8
# Wed, 20 Apr 2022 13:25:44 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Wed, 20 Apr 2022 13:25:44 GMT
ENV R_BASE_VERSION=4.1.3
# Wed, 20 Apr 2022 13:26:52 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-docopt                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 13:26:54 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:536039adbcd59ca1bf50e1393d4c116319d1f29168898c56d21c192d219c4832`  
		Last Modified: Wed, 20 Apr 2022 04:52:49 GMT  
		Size: 55.6 MB (55578869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b1da36bf8d2a06d8166a24f3477fb5137ed10b2e31479a8c502fb0011af0bc9`  
		Last Modified: Wed, 20 Apr 2022 13:27:14 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4afe378696fd472844089373e7b153a0f0a0d8293e12fa57f18cb850e2c4fe37`  
		Last Modified: Wed, 20 Apr 2022 13:27:17 GMT  
		Size: 25.9 MB (25851696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61b0b85413db82c6a0f17b355291dfd6bc4c1e251d67aa85b15a568f579c0655`  
		Last Modified: Wed, 20 Apr 2022 13:27:14 GMT  
		Size: 864.6 KB (864607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bf4cc3b4afb9b51cb673c32c8d3101da067c78e42701b7b84de52cf52c4f3a0`  
		Last Modified: Wed, 20 Apr 2022 13:27:14 GMT  
		Size: 348.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11f32de4c0e37f0cceca24bc8e6d29ee2ec0eb02a91f6f329586fbd342d22da6`  
		Last Modified: Wed, 20 Apr 2022 13:27:43 GMT  
		Size: 251.5 MB (251510282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:4.1.3` - linux; arm64 variant v8

```console
$ docker pull r-base@sha256:6511b580c48b285bef5082c7f17ac57edb7af926f5168985056952c08c4bd401
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **322.9 MB (322935119 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:587012b8220aa1be4c1ab670688e3ce7f4edd639863764982dbdf4aae0e72226`
-	Default Command: `["R"]`

```dockerfile
# Wed, 20 Apr 2022 04:31:45 GMT
ADD file:273f985806cb79b6f6b619ba5b9db50ba151174fde33bffc81c25187b0999170 in / 
# Wed, 20 Apr 2022 04:31:45 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 11:59:40 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Wed, 20 Apr 2022 11:59:41 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Wed, 20 Apr 2022 11:59:50 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 11:59:52 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Wed, 20 Apr 2022 11:59:53 GMT
ENV LC_ALL=en_US.UTF-8
# Wed, 20 Apr 2022 11:59:54 GMT
ENV LANG=en_US.UTF-8
# Wed, 20 Apr 2022 11:59:55 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Wed, 20 Apr 2022 11:59:56 GMT
ENV R_BASE_VERSION=4.1.3
# Wed, 20 Apr 2022 12:00:45 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-docopt                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 12:00:46 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:3124af2dc12fec2edfce6b676869cb7dbcea85f39bf473efd3b5674765b68351`  
		Last Modified: Wed, 20 Apr 2022 04:40:29 GMT  
		Size: 54.5 MB (54493338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86e730a7adab655457f2a985872a4b9bc5d0af23359a084ba069c602452f97f1`  
		Last Modified: Wed, 20 Apr 2022 12:00:59 GMT  
		Size: 1.8 KB (1823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f40c6eb1bebd6d176cdb1c752acf4612cdf94053b91410b654ca3a643443154`  
		Last Modified: Wed, 20 Apr 2022 12:01:02 GMT  
		Size: 25.8 MB (25841038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23547edafe1d3dec48a3eb14cac16816223e38e500ec3b14a1d4f9e7719b1d4e`  
		Last Modified: Wed, 20 Apr 2022 12:01:00 GMT  
		Size: 864.6 KB (864610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:232373586c238520cd70bb4f78a1cf585963b867f6d80f3ad76ef18d9256dadb`  
		Last Modified: Wed, 20 Apr 2022 12:00:59 GMT  
		Size: 348.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdff729dc60f243bf9bb3df1a95e763076dc3e078bae4c2c1968117716bcc946`  
		Last Modified: Wed, 20 Apr 2022 12:01:27 GMT  
		Size: 241.7 MB (241733962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:4.1.3` - linux; ppc64le

```console
$ docker pull r-base@sha256:9ae6f352909427c076540197dabae026c5df155c92e2e7d478bc3f69dcf004da
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **332.6 MB (332572962 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b9251ae80b4d9033f02ac83e391e7da112f170044baf10c8612f1de33341903`
-	Default Command: `["R"]`

```dockerfile
# Tue, 29 Mar 2022 00:25:37 GMT
ADD file:8974d32898b791c51a9fab708550a07b9a517c5d9bd6db47acd59606984b81aa in / 
# Tue, 29 Mar 2022 00:25:42 GMT
CMD ["bash"]
# Wed, 30 Mar 2022 06:55:50 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Wed, 30 Mar 2022 06:56:14 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Wed, 30 Mar 2022 06:57:36 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 06:57:53 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Wed, 30 Mar 2022 06:57:57 GMT
ENV LC_ALL=en_US.UTF-8
# Wed, 30 Mar 2022 06:58:01 GMT
ENV LANG=en_US.UTF-8
# Wed, 30 Mar 2022 06:58:12 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Wed, 30 Mar 2022 06:58:16 GMT
ENV R_BASE_VERSION=4.1.3
# Wed, 30 Mar 2022 07:06:00 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-docopt                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 07:06:06 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:4b9bd4aec57ee466c8fe8d1c7e0f4e5c7e7604e860d3e58360a2dcf666c0b516`  
		Last Modified: Tue, 29 Mar 2022 00:39:35 GMT  
		Size: 60.0 MB (59999357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8e7629080014bf7e1cf797458f57f116c1914cfa318370b7bcc0fef48826b40`  
		Last Modified: Wed, 30 Mar 2022 07:06:39 GMT  
		Size: 1.9 KB (1894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b04daefbeb0df85bcd04bd08db85228394794131d189bf674930253769105f9e`  
		Last Modified: Wed, 30 Mar 2022 07:06:42 GMT  
		Size: 26.1 MB (26070762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c572b1479da640b1b4532570c4f4910fc3cb9ee721148ff900650449edd61f89`  
		Last Modified: Wed, 30 Mar 2022 07:06:39 GMT  
		Size: 864.6 KB (864604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6592d90fe32e79e98cdd79559176018daa12bd61d59ce15305cac4da7d42a91e`  
		Last Modified: Wed, 30 Mar 2022 07:06:38 GMT  
		Size: 350.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cebb21397c6be81e1f9fdacd45f3cc9dc0f9ccb637c06fce4f596a8a58b10d0`  
		Last Modified: Wed, 30 Mar 2022 07:07:21 GMT  
		Size: 245.6 MB (245635995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:4.1.3` - linux; s390x

```console
$ docker pull r-base@sha256:3d11494acba1c9d2383b94a81e2448f6df0144a1e82d2f836b6a566c5755a336
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **298.4 MB (298352704 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af80ce35cb4eec5fafec3f7f46e1b4e2743dbe65977d67d02b7b0dcfbfa6c250`
-	Default Command: `["R"]`

```dockerfile
# Wed, 20 Apr 2022 08:44:07 GMT
ADD file:23684e7af9a096cf83a114c361e7879ed97ef5fbf7cb9607e40ffaf19dd0bed7 in / 
# Wed, 20 Apr 2022 08:44:14 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 16:03:35 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Wed, 20 Apr 2022 16:03:37 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Wed, 20 Apr 2022 16:04:04 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 16:04:10 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Wed, 20 Apr 2022 16:04:11 GMT
ENV LC_ALL=en_US.UTF-8
# Wed, 20 Apr 2022 16:04:12 GMT
ENV LANG=en_US.UTF-8
# Wed, 20 Apr 2022 16:04:14 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Wed, 20 Apr 2022 16:04:15 GMT
ENV R_BASE_VERSION=4.1.3
# Wed, 20 Apr 2022 16:06:16 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-docopt                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 16:06:38 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:362ce0a85fc3f682e0adac2df3a00133068c959c8dbf9d7872eb24b1b68f55a3`  
		Last Modified: Wed, 20 Apr 2022 08:52:12 GMT  
		Size: 53.8 MB (53813515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2d4c28aba12d4bb2ceb61042334706fd64afbf057777f6a85df8415801c4cb0`  
		Last Modified: Wed, 20 Apr 2022 16:07:38 GMT  
		Size: 1.9 KB (1884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf874736dd9bc2cbadd95f849168168927b6a65a00d071db95f2557f21e0e5a2`  
		Last Modified: Wed, 20 Apr 2022 16:07:35 GMT  
		Size: 25.9 MB (25864057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baab6b33b8fb34f72a25d67297e7488a42a69874c74b647c63094365dbdcae3c`  
		Last Modified: Wed, 20 Apr 2022 16:07:28 GMT  
		Size: 920.2 KB (920190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d02a7efd41932b75e4ec636c8073ddfdb99f915f7ff69c8ed0f0448e5eb9de5a`  
		Last Modified: Wed, 20 Apr 2022 16:07:38 GMT  
		Size: 351.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b9628e0d42c0dfdf290d06299b8174cf8368a670a2bbc8e8afc9ad6941a6812`  
		Last Modified: Wed, 20 Apr 2022 16:07:54 GMT  
		Size: 217.8 MB (217752707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `r-base:latest`

```console
$ docker pull r-base@sha256:3d2448e9077ecbe673c662acbefcbacf6e3515cf5507fdac0f37765208013425
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `r-base:latest` - linux; amd64

```console
$ docker pull r-base@sha256:567cb8968827c97e1fb788e23e9a3acf8a5d95c6dbeeb88a48ae438e05fe2da0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **333.8 MB (333807683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f987362a590dd6659467713d5f78324a8965c8c2a6abc464f5613da3e969aa96`
-	Default Command: `["R"]`

```dockerfile
# Wed, 20 Apr 2022 04:45:35 GMT
ADD file:fb66d619557384a14385fa7b5371be954594c4aff1700edcbd9cff422c3498f0 in / 
# Wed, 20 Apr 2022 04:45:35 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 13:25:30 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Wed, 20 Apr 2022 13:25:31 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Wed, 20 Apr 2022 13:25:41 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 13:25:43 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Wed, 20 Apr 2022 13:25:43 GMT
ENV LC_ALL=en_US.UTF-8
# Wed, 20 Apr 2022 13:25:43 GMT
ENV LANG=en_US.UTF-8
# Wed, 20 Apr 2022 13:25:44 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Wed, 20 Apr 2022 13:25:44 GMT
ENV R_BASE_VERSION=4.1.3
# Wed, 20 Apr 2022 13:26:52 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-docopt                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 13:26:54 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:536039adbcd59ca1bf50e1393d4c116319d1f29168898c56d21c192d219c4832`  
		Last Modified: Wed, 20 Apr 2022 04:52:49 GMT  
		Size: 55.6 MB (55578869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b1da36bf8d2a06d8166a24f3477fb5137ed10b2e31479a8c502fb0011af0bc9`  
		Last Modified: Wed, 20 Apr 2022 13:27:14 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4afe378696fd472844089373e7b153a0f0a0d8293e12fa57f18cb850e2c4fe37`  
		Last Modified: Wed, 20 Apr 2022 13:27:17 GMT  
		Size: 25.9 MB (25851696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61b0b85413db82c6a0f17b355291dfd6bc4c1e251d67aa85b15a568f579c0655`  
		Last Modified: Wed, 20 Apr 2022 13:27:14 GMT  
		Size: 864.6 KB (864607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bf4cc3b4afb9b51cb673c32c8d3101da067c78e42701b7b84de52cf52c4f3a0`  
		Last Modified: Wed, 20 Apr 2022 13:27:14 GMT  
		Size: 348.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11f32de4c0e37f0cceca24bc8e6d29ee2ec0eb02a91f6f329586fbd342d22da6`  
		Last Modified: Wed, 20 Apr 2022 13:27:43 GMT  
		Size: 251.5 MB (251510282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:latest` - linux; arm64 variant v8

```console
$ docker pull r-base@sha256:6511b580c48b285bef5082c7f17ac57edb7af926f5168985056952c08c4bd401
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **322.9 MB (322935119 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:587012b8220aa1be4c1ab670688e3ce7f4edd639863764982dbdf4aae0e72226`
-	Default Command: `["R"]`

```dockerfile
# Wed, 20 Apr 2022 04:31:45 GMT
ADD file:273f985806cb79b6f6b619ba5b9db50ba151174fde33bffc81c25187b0999170 in / 
# Wed, 20 Apr 2022 04:31:45 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 11:59:40 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Wed, 20 Apr 2022 11:59:41 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Wed, 20 Apr 2022 11:59:50 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 11:59:52 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Wed, 20 Apr 2022 11:59:53 GMT
ENV LC_ALL=en_US.UTF-8
# Wed, 20 Apr 2022 11:59:54 GMT
ENV LANG=en_US.UTF-8
# Wed, 20 Apr 2022 11:59:55 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Wed, 20 Apr 2022 11:59:56 GMT
ENV R_BASE_VERSION=4.1.3
# Wed, 20 Apr 2022 12:00:45 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-docopt                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 12:00:46 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:3124af2dc12fec2edfce6b676869cb7dbcea85f39bf473efd3b5674765b68351`  
		Last Modified: Wed, 20 Apr 2022 04:40:29 GMT  
		Size: 54.5 MB (54493338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86e730a7adab655457f2a985872a4b9bc5d0af23359a084ba069c602452f97f1`  
		Last Modified: Wed, 20 Apr 2022 12:00:59 GMT  
		Size: 1.8 KB (1823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f40c6eb1bebd6d176cdb1c752acf4612cdf94053b91410b654ca3a643443154`  
		Last Modified: Wed, 20 Apr 2022 12:01:02 GMT  
		Size: 25.8 MB (25841038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23547edafe1d3dec48a3eb14cac16816223e38e500ec3b14a1d4f9e7719b1d4e`  
		Last Modified: Wed, 20 Apr 2022 12:01:00 GMT  
		Size: 864.6 KB (864610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:232373586c238520cd70bb4f78a1cf585963b867f6d80f3ad76ef18d9256dadb`  
		Last Modified: Wed, 20 Apr 2022 12:00:59 GMT  
		Size: 348.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdff729dc60f243bf9bb3df1a95e763076dc3e078bae4c2c1968117716bcc946`  
		Last Modified: Wed, 20 Apr 2022 12:01:27 GMT  
		Size: 241.7 MB (241733962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:latest` - linux; ppc64le

```console
$ docker pull r-base@sha256:9ae6f352909427c076540197dabae026c5df155c92e2e7d478bc3f69dcf004da
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **332.6 MB (332572962 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b9251ae80b4d9033f02ac83e391e7da112f170044baf10c8612f1de33341903`
-	Default Command: `["R"]`

```dockerfile
# Tue, 29 Mar 2022 00:25:37 GMT
ADD file:8974d32898b791c51a9fab708550a07b9a517c5d9bd6db47acd59606984b81aa in / 
# Tue, 29 Mar 2022 00:25:42 GMT
CMD ["bash"]
# Wed, 30 Mar 2022 06:55:50 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Wed, 30 Mar 2022 06:56:14 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Wed, 30 Mar 2022 06:57:36 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 06:57:53 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Wed, 30 Mar 2022 06:57:57 GMT
ENV LC_ALL=en_US.UTF-8
# Wed, 30 Mar 2022 06:58:01 GMT
ENV LANG=en_US.UTF-8
# Wed, 30 Mar 2022 06:58:12 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Wed, 30 Mar 2022 06:58:16 GMT
ENV R_BASE_VERSION=4.1.3
# Wed, 30 Mar 2022 07:06:00 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-docopt                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 07:06:06 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:4b9bd4aec57ee466c8fe8d1c7e0f4e5c7e7604e860d3e58360a2dcf666c0b516`  
		Last Modified: Tue, 29 Mar 2022 00:39:35 GMT  
		Size: 60.0 MB (59999357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8e7629080014bf7e1cf797458f57f116c1914cfa318370b7bcc0fef48826b40`  
		Last Modified: Wed, 30 Mar 2022 07:06:39 GMT  
		Size: 1.9 KB (1894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b04daefbeb0df85bcd04bd08db85228394794131d189bf674930253769105f9e`  
		Last Modified: Wed, 30 Mar 2022 07:06:42 GMT  
		Size: 26.1 MB (26070762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c572b1479da640b1b4532570c4f4910fc3cb9ee721148ff900650449edd61f89`  
		Last Modified: Wed, 30 Mar 2022 07:06:39 GMT  
		Size: 864.6 KB (864604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6592d90fe32e79e98cdd79559176018daa12bd61d59ce15305cac4da7d42a91e`  
		Last Modified: Wed, 30 Mar 2022 07:06:38 GMT  
		Size: 350.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cebb21397c6be81e1f9fdacd45f3cc9dc0f9ccb637c06fce4f596a8a58b10d0`  
		Last Modified: Wed, 30 Mar 2022 07:07:21 GMT  
		Size: 245.6 MB (245635995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:latest` - linux; s390x

```console
$ docker pull r-base@sha256:3d11494acba1c9d2383b94a81e2448f6df0144a1e82d2f836b6a566c5755a336
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **298.4 MB (298352704 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af80ce35cb4eec5fafec3f7f46e1b4e2743dbe65977d67d02b7b0dcfbfa6c250`
-	Default Command: `["R"]`

```dockerfile
# Wed, 20 Apr 2022 08:44:07 GMT
ADD file:23684e7af9a096cf83a114c361e7879ed97ef5fbf7cb9607e40ffaf19dd0bed7 in / 
# Wed, 20 Apr 2022 08:44:14 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 16:03:35 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Wed, 20 Apr 2022 16:03:37 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Wed, 20 Apr 2022 16:04:04 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 16:04:10 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Wed, 20 Apr 2022 16:04:11 GMT
ENV LC_ALL=en_US.UTF-8
# Wed, 20 Apr 2022 16:04:12 GMT
ENV LANG=en_US.UTF-8
# Wed, 20 Apr 2022 16:04:14 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Wed, 20 Apr 2022 16:04:15 GMT
ENV R_BASE_VERSION=4.1.3
# Wed, 20 Apr 2022 16:06:16 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-docopt                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 16:06:38 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:362ce0a85fc3f682e0adac2df3a00133068c959c8dbf9d7872eb24b1b68f55a3`  
		Last Modified: Wed, 20 Apr 2022 08:52:12 GMT  
		Size: 53.8 MB (53813515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2d4c28aba12d4bb2ceb61042334706fd64afbf057777f6a85df8415801c4cb0`  
		Last Modified: Wed, 20 Apr 2022 16:07:38 GMT  
		Size: 1.9 KB (1884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf874736dd9bc2cbadd95f849168168927b6a65a00d071db95f2557f21e0e5a2`  
		Last Modified: Wed, 20 Apr 2022 16:07:35 GMT  
		Size: 25.9 MB (25864057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baab6b33b8fb34f72a25d67297e7488a42a69874c74b647c63094365dbdcae3c`  
		Last Modified: Wed, 20 Apr 2022 16:07:28 GMT  
		Size: 920.2 KB (920190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d02a7efd41932b75e4ec636c8073ddfdb99f915f7ff69c8ed0f0448e5eb9de5a`  
		Last Modified: Wed, 20 Apr 2022 16:07:38 GMT  
		Size: 351.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b9628e0d42c0dfdf290d06299b8174cf8368a670a2bbc8e8afc9ad6941a6812`  
		Last Modified: Wed, 20 Apr 2022 16:07:54 GMT  
		Size: 217.8 MB (217752707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
