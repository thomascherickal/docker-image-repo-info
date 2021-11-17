<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `r-base`

-	[`r-base:4.1.2`](#r-base412)
-	[`r-base:latest`](#r-baselatest)

## `r-base:4.1.2`

```console
$ docker pull r-base@sha256:f897331f87e9b39e535e7fd529887f959ed7ee068c1fb043df0181a943376b70
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `r-base:4.1.2` - linux; amd64

```console
$ docker pull r-base@sha256:2df02621f2fc45e6c06c685e2f358b58b50d10f70b81339657bf9fa1d7bb9ce9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **549.1 MB (549086675 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:087b0ff8b59ff8585a1fe18883a9f191108e7b21023c2105f51c6f28eb583763`
-	Default Command: `["R"]`

```dockerfile
# Wed, 17 Nov 2021 02:22:48 GMT
ADD file:61e992a8cfedc03feb12ae278ba2f7ab32f2845c5dea31869b10861104700c33 in / 
# Wed, 17 Nov 2021 02:22:48 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 21:51:45 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Wed, 17 Nov 2021 21:51:47 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Wed, 17 Nov 2021 21:51:56 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 21:51:58 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Wed, 17 Nov 2021 21:51:59 GMT
ENV LC_ALL=en_US.UTF-8
# Wed, 17 Nov 2021 21:51:59 GMT
ENV LANG=en_US.UTF-8
# Wed, 17 Nov 2021 21:51:59 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Wed, 17 Nov 2021 21:52:00 GMT
ENV R_BASE_VERSION=4.1.2
# Wed, 17 Nov 2021 21:52:00 GMT
RUN echo "deb http://deb.debian.org/debian experimental main" > /etc/apt/sources.list.d/experimental.list     && echo "deb [trusted=yes] https://eddelbuettel.github.io/ppaR400 ./" > /etc/apt/sources.list.d/edd-r4.list
# Wed, 17 Nov 2021 21:53:07 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 21:53:11 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:99a9589829e41c216113b415d3c0c9233e7e6498d6291141cdf85cc3042e2b65`  
		Last Modified: Wed, 17 Nov 2021 02:29:54 GMT  
		Size: 55.5 MB (55457188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:734cf1edf8df2d2f932b529cde2a174131f7542f841d8a3f965fa8e385d951e9`  
		Last Modified: Wed, 17 Nov 2021 21:53:31 GMT  
		Size: 1.9 KB (1874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39010a7e8f58a2fc060db087692c662f88349a8d99db05475cb4589be2a54ba6`  
		Last Modified: Wed, 17 Nov 2021 21:53:32 GMT  
		Size: 25.7 MB (25734401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea26568ecc644a0f34b1c13bbf61d9088853b2cafaf2d669f622073315119bbc`  
		Last Modified: Wed, 17 Nov 2021 21:53:29 GMT  
		Size: 864.6 KB (864611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3de5d44e8850d9b3591418b4cc4d54ca5ebde5ad4ef9f92606edb1cab90f9b88`  
		Last Modified: Wed, 17 Nov 2021 21:53:28 GMT  
		Size: 349.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71eba4e39d7edcad142ee35c87a755c18d485284a7133e33a774aebd911a2902`  
		Last Modified: Wed, 17 Nov 2021 21:53:29 GMT  
		Size: 291.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:243aa39b56400abe056d49901be10c76707de3080b983defa27c53039b174d8a`  
		Last Modified: Wed, 17 Nov 2021 21:54:25 GMT  
		Size: 467.0 MB (467027961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:4.1.2` - linux; arm64 variant v8

```console
$ docker pull r-base@sha256:96f97b2394aa9427b2e267a0923260c72c53b923a4a7f7f95385753588b0cac2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **537.8 MB (537845813 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8db25e6538797cf684141e8c8bd68947e1299e5a9ea2b27318a60cba942bbe78`
-	Default Command: `["R"]`

```dockerfile
# Wed, 17 Nov 2021 02:42:59 GMT
ADD file:c4d68bcae684e69a17ac01569a16c332bc925c4359383dbf3f27066f3abb295c in / 
# Wed, 17 Nov 2021 02:43:01 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 09:24:11 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Wed, 17 Nov 2021 09:24:12 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Wed, 17 Nov 2021 09:24:22 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:24:25 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Wed, 17 Nov 2021 09:24:26 GMT
ENV LC_ALL=en_US.UTF-8
# Wed, 17 Nov 2021 09:24:27 GMT
ENV LANG=en_US.UTF-8
# Wed, 17 Nov 2021 09:24:28 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Wed, 17 Nov 2021 09:24:29 GMT
ENV R_BASE_VERSION=4.1.2
# Wed, 17 Nov 2021 09:24:30 GMT
RUN echo "deb http://deb.debian.org/debian experimental main" > /etc/apt/sources.list.d/experimental.list     && echo "deb [trusted=yes] https://eddelbuettel.github.io/ppaR400 ./" > /etc/apt/sources.list.d/edd-r4.list
# Wed, 17 Nov 2021 09:25:55 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:25:56 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:3306c77e3ba6c6431765bbac6b0bbfb35079cfb5d567c3db405aad7687a02603`  
		Last Modified: Wed, 17 Nov 2021 02:52:02 GMT  
		Size: 54.5 MB (54464394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88850b877e844f037a3b637d162846c422434fc9ac156475fbc4491818d3800e`  
		Last Modified: Wed, 17 Nov 2021 09:26:17 GMT  
		Size: 1.8 KB (1760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16bab85edfcf4887dc348fb329c664aaa73da6fca768498ae1ef4c18143410f0`  
		Last Modified: Wed, 17 Nov 2021 09:26:18 GMT  
		Size: 25.7 MB (25725458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:214d9090f79499ab89198766182c5ea16e6e66a4329acefe66c98d33bbff5993`  
		Last Modified: Wed, 17 Nov 2021 09:26:15 GMT  
		Size: 864.6 KB (864612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ba744f38b2c9cdd8eb1afe1e0a05269894dd4bb3835a814ad1067186dec7302`  
		Last Modified: Wed, 17 Nov 2021 09:26:15 GMT  
		Size: 348.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb1c2c8ed5135dfb9531de18cbb591aea65d1388706d68211e447f00ffe1aa6a`  
		Last Modified: Wed, 17 Nov 2021 09:26:14 GMT  
		Size: 291.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45e32ec19a0ecdb3e2ef10e6be0e11af03c5850e4fc303c093370d6afa686f3b`  
		Last Modified: Wed, 17 Nov 2021 09:27:12 GMT  
		Size: 456.8 MB (456788950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:4.1.2` - linux; ppc64le

```console
$ docker pull r-base@sha256:1319918fb43d8e1ae8209ea7dc9117bd49a8d5f39af8fd042fe231b3cce28521
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **532.3 MB (532262775 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d534e51f0b28de723c5d3758c46efa4eb8ab1de46ea26dcc05b007c6b8e296dc`
-	Default Command: `["R"]`

```dockerfile
# Wed, 17 Nov 2021 03:35:47 GMT
ADD file:6ec33732a5ce54ae880804c7d4ce9bbc89ad76007b04d23e694d60679162abdc in / 
# Wed, 17 Nov 2021 03:36:09 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 14:36:04 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Wed, 17 Nov 2021 14:36:13 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Wed, 17 Nov 2021 14:37:04 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 14:37:12 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Wed, 17 Nov 2021 14:37:15 GMT
ENV LC_ALL=en_US.UTF-8
# Wed, 17 Nov 2021 14:37:17 GMT
ENV LANG=en_US.UTF-8
# Wed, 17 Nov 2021 14:37:23 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Wed, 17 Nov 2021 14:37:26 GMT
ENV R_BASE_VERSION=4.1.2
# Wed, 17 Nov 2021 14:37:31 GMT
RUN echo "deb http://deb.debian.org/debian experimental main" > /etc/apt/sources.list.d/experimental.list     && echo "deb [trusted=yes] https://eddelbuettel.github.io/ppaR400 ./" > /etc/apt/sources.list.d/edd-r4.list
# Wed, 17 Nov 2021 14:42:46 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 14:42:54 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:1c92bc8c2e6cbcb9f02ae352b98981f7632bf82483d2ab5a0394f4a3139b3c5b`  
		Last Modified: Wed, 17 Nov 2021 04:12:49 GMT  
		Size: 59.7 MB (59706108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a41091a6c5466c5f119f349015272ea5d9f60e438df65a19eec29aed40a748aa`  
		Last Modified: Wed, 17 Nov 2021 14:43:19 GMT  
		Size: 1.9 KB (1886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ee9788fbadb1fcccd7993a3740b96cf4b5df64a276961ad6b63e70e957c1d7e`  
		Last Modified: Wed, 17 Nov 2021 14:43:20 GMT  
		Size: 26.0 MB (25958946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:848fe08e27f2d543ede8fefd36f42933772911ba2b7f0e923743c37b030b134c`  
		Last Modified: Wed, 17 Nov 2021 14:43:17 GMT  
		Size: 864.6 KB (864617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6429b9ed205043e375a354efa42a61c9eab91c5212f97ca7d6e10729c094977a`  
		Last Modified: Wed, 17 Nov 2021 14:43:16 GMT  
		Size: 351.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ebbf6b1480dbd78c5fe8b0564e79d14f161cc3c5299d33b9e25780f013f2920`  
		Last Modified: Wed, 17 Nov 2021 14:43:17 GMT  
		Size: 295.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d88faad6b04ed2fcec177b3b962494c18eb2fcf4108e5b934c564aae3fe6327`  
		Last Modified: Wed, 17 Nov 2021 14:44:26 GMT  
		Size: 445.7 MB (445730572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:4.1.2` - linux; s390x

```console
$ docker pull r-base@sha256:7b106be8884de22200d90e98b91b6b5274674316fa60f77de191353fd0c29680
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **488.9 MB (488884420 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7bde100730619821ee674761426150280663cff2c51998f7190d9900e6bee0d`
-	Default Command: `["R"]`

```dockerfile
# Wed, 17 Nov 2021 02:44:42 GMT
ADD file:6b07f3691aed718fdd31338ceb571ce22ffe4f9410f48df5c16f190258ace5ae in / 
# Wed, 17 Nov 2021 02:44:44 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 09:11:12 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Wed, 17 Nov 2021 09:11:13 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Wed, 17 Nov 2021 09:11:21 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:11:24 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Wed, 17 Nov 2021 09:11:24 GMT
ENV LC_ALL=en_US.UTF-8
# Wed, 17 Nov 2021 09:11:24 GMT
ENV LANG=en_US.UTF-8
# Wed, 17 Nov 2021 09:11:25 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Wed, 17 Nov 2021 09:11:25 GMT
ENV R_BASE_VERSION=4.1.2
# Wed, 17 Nov 2021 09:11:26 GMT
RUN echo "deb http://deb.debian.org/debian experimental main" > /etc/apt/sources.list.d/experimental.list     && echo "deb [trusted=yes] https://eddelbuettel.github.io/ppaR400 ./" > /etc/apt/sources.list.d/edd-r4.list
# Wed, 17 Nov 2021 09:12:34 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:12:48 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:1c02d7cb6bfcee3d40b1f3c9461f47e72e2f51d514b5df5ddb147d175da65910`  
		Last Modified: Wed, 17 Nov 2021 02:50:40 GMT  
		Size: 53.7 MB (53669187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:220be3db1df6258f3aebc2b3c4622ad1d8680871a31543d38ebe7489e54c2315`  
		Last Modified: Wed, 17 Nov 2021 09:13:10 GMT  
		Size: 1.9 KB (1878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56f884dbcc2d3fd82fbc93f59166b00e406e6a07742a0157b11a80334a41be2d`  
		Last Modified: Wed, 17 Nov 2021 09:13:11 GMT  
		Size: 25.7 MB (25730683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b66636dbcba0824a55dc895f4aaabefc24bae27999399c2ebc34234a6b3774cf`  
		Last Modified: Wed, 17 Nov 2021 09:13:08 GMT  
		Size: 920.2 KB (920188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c9afafbdb33d3171de360b123042c9933ec5bc0f41d7587f550e3b2d2a9dc6e`  
		Last Modified: Wed, 17 Nov 2021 09:13:08 GMT  
		Size: 351.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f886d7f25bf1d3e5164054de008592d645d12c6b8c7e8046304ac3271379d893`  
		Last Modified: Wed, 17 Nov 2021 09:13:08 GMT  
		Size: 294.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ced9a75a566e4589e4973141f9de7e687f32d617e6a47a3222b9f1c7c49ac17`  
		Last Modified: Wed, 17 Nov 2021 09:13:51 GMT  
		Size: 408.6 MB (408561839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `r-base:latest`

```console
$ docker pull r-base@sha256:f897331f87e9b39e535e7fd529887f959ed7ee068c1fb043df0181a943376b70
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `r-base:latest` - linux; amd64

```console
$ docker pull r-base@sha256:2df02621f2fc45e6c06c685e2f358b58b50d10f70b81339657bf9fa1d7bb9ce9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **549.1 MB (549086675 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:087b0ff8b59ff8585a1fe18883a9f191108e7b21023c2105f51c6f28eb583763`
-	Default Command: `["R"]`

```dockerfile
# Wed, 17 Nov 2021 02:22:48 GMT
ADD file:61e992a8cfedc03feb12ae278ba2f7ab32f2845c5dea31869b10861104700c33 in / 
# Wed, 17 Nov 2021 02:22:48 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 21:51:45 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Wed, 17 Nov 2021 21:51:47 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Wed, 17 Nov 2021 21:51:56 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 21:51:58 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Wed, 17 Nov 2021 21:51:59 GMT
ENV LC_ALL=en_US.UTF-8
# Wed, 17 Nov 2021 21:51:59 GMT
ENV LANG=en_US.UTF-8
# Wed, 17 Nov 2021 21:51:59 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Wed, 17 Nov 2021 21:52:00 GMT
ENV R_BASE_VERSION=4.1.2
# Wed, 17 Nov 2021 21:52:00 GMT
RUN echo "deb http://deb.debian.org/debian experimental main" > /etc/apt/sources.list.d/experimental.list     && echo "deb [trusted=yes] https://eddelbuettel.github.io/ppaR400 ./" > /etc/apt/sources.list.d/edd-r4.list
# Wed, 17 Nov 2021 21:53:07 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 21:53:11 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:99a9589829e41c216113b415d3c0c9233e7e6498d6291141cdf85cc3042e2b65`  
		Last Modified: Wed, 17 Nov 2021 02:29:54 GMT  
		Size: 55.5 MB (55457188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:734cf1edf8df2d2f932b529cde2a174131f7542f841d8a3f965fa8e385d951e9`  
		Last Modified: Wed, 17 Nov 2021 21:53:31 GMT  
		Size: 1.9 KB (1874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39010a7e8f58a2fc060db087692c662f88349a8d99db05475cb4589be2a54ba6`  
		Last Modified: Wed, 17 Nov 2021 21:53:32 GMT  
		Size: 25.7 MB (25734401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea26568ecc644a0f34b1c13bbf61d9088853b2cafaf2d669f622073315119bbc`  
		Last Modified: Wed, 17 Nov 2021 21:53:29 GMT  
		Size: 864.6 KB (864611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3de5d44e8850d9b3591418b4cc4d54ca5ebde5ad4ef9f92606edb1cab90f9b88`  
		Last Modified: Wed, 17 Nov 2021 21:53:28 GMT  
		Size: 349.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71eba4e39d7edcad142ee35c87a755c18d485284a7133e33a774aebd911a2902`  
		Last Modified: Wed, 17 Nov 2021 21:53:29 GMT  
		Size: 291.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:243aa39b56400abe056d49901be10c76707de3080b983defa27c53039b174d8a`  
		Last Modified: Wed, 17 Nov 2021 21:54:25 GMT  
		Size: 467.0 MB (467027961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:latest` - linux; arm64 variant v8

```console
$ docker pull r-base@sha256:96f97b2394aa9427b2e267a0923260c72c53b923a4a7f7f95385753588b0cac2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **537.8 MB (537845813 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8db25e6538797cf684141e8c8bd68947e1299e5a9ea2b27318a60cba942bbe78`
-	Default Command: `["R"]`

```dockerfile
# Wed, 17 Nov 2021 02:42:59 GMT
ADD file:c4d68bcae684e69a17ac01569a16c332bc925c4359383dbf3f27066f3abb295c in / 
# Wed, 17 Nov 2021 02:43:01 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 09:24:11 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Wed, 17 Nov 2021 09:24:12 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Wed, 17 Nov 2021 09:24:22 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:24:25 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Wed, 17 Nov 2021 09:24:26 GMT
ENV LC_ALL=en_US.UTF-8
# Wed, 17 Nov 2021 09:24:27 GMT
ENV LANG=en_US.UTF-8
# Wed, 17 Nov 2021 09:24:28 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Wed, 17 Nov 2021 09:24:29 GMT
ENV R_BASE_VERSION=4.1.2
# Wed, 17 Nov 2021 09:24:30 GMT
RUN echo "deb http://deb.debian.org/debian experimental main" > /etc/apt/sources.list.d/experimental.list     && echo "deb [trusted=yes] https://eddelbuettel.github.io/ppaR400 ./" > /etc/apt/sources.list.d/edd-r4.list
# Wed, 17 Nov 2021 09:25:55 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:25:56 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:3306c77e3ba6c6431765bbac6b0bbfb35079cfb5d567c3db405aad7687a02603`  
		Last Modified: Wed, 17 Nov 2021 02:52:02 GMT  
		Size: 54.5 MB (54464394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88850b877e844f037a3b637d162846c422434fc9ac156475fbc4491818d3800e`  
		Last Modified: Wed, 17 Nov 2021 09:26:17 GMT  
		Size: 1.8 KB (1760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16bab85edfcf4887dc348fb329c664aaa73da6fca768498ae1ef4c18143410f0`  
		Last Modified: Wed, 17 Nov 2021 09:26:18 GMT  
		Size: 25.7 MB (25725458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:214d9090f79499ab89198766182c5ea16e6e66a4329acefe66c98d33bbff5993`  
		Last Modified: Wed, 17 Nov 2021 09:26:15 GMT  
		Size: 864.6 KB (864612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ba744f38b2c9cdd8eb1afe1e0a05269894dd4bb3835a814ad1067186dec7302`  
		Last Modified: Wed, 17 Nov 2021 09:26:15 GMT  
		Size: 348.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb1c2c8ed5135dfb9531de18cbb591aea65d1388706d68211e447f00ffe1aa6a`  
		Last Modified: Wed, 17 Nov 2021 09:26:14 GMT  
		Size: 291.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45e32ec19a0ecdb3e2ef10e6be0e11af03c5850e4fc303c093370d6afa686f3b`  
		Last Modified: Wed, 17 Nov 2021 09:27:12 GMT  
		Size: 456.8 MB (456788950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:latest` - linux; ppc64le

```console
$ docker pull r-base@sha256:1319918fb43d8e1ae8209ea7dc9117bd49a8d5f39af8fd042fe231b3cce28521
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **532.3 MB (532262775 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d534e51f0b28de723c5d3758c46efa4eb8ab1de46ea26dcc05b007c6b8e296dc`
-	Default Command: `["R"]`

```dockerfile
# Wed, 17 Nov 2021 03:35:47 GMT
ADD file:6ec33732a5ce54ae880804c7d4ce9bbc89ad76007b04d23e694d60679162abdc in / 
# Wed, 17 Nov 2021 03:36:09 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 14:36:04 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Wed, 17 Nov 2021 14:36:13 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Wed, 17 Nov 2021 14:37:04 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 14:37:12 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Wed, 17 Nov 2021 14:37:15 GMT
ENV LC_ALL=en_US.UTF-8
# Wed, 17 Nov 2021 14:37:17 GMT
ENV LANG=en_US.UTF-8
# Wed, 17 Nov 2021 14:37:23 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Wed, 17 Nov 2021 14:37:26 GMT
ENV R_BASE_VERSION=4.1.2
# Wed, 17 Nov 2021 14:37:31 GMT
RUN echo "deb http://deb.debian.org/debian experimental main" > /etc/apt/sources.list.d/experimental.list     && echo "deb [trusted=yes] https://eddelbuettel.github.io/ppaR400 ./" > /etc/apt/sources.list.d/edd-r4.list
# Wed, 17 Nov 2021 14:42:46 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 14:42:54 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:1c92bc8c2e6cbcb9f02ae352b98981f7632bf82483d2ab5a0394f4a3139b3c5b`  
		Last Modified: Wed, 17 Nov 2021 04:12:49 GMT  
		Size: 59.7 MB (59706108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a41091a6c5466c5f119f349015272ea5d9f60e438df65a19eec29aed40a748aa`  
		Last Modified: Wed, 17 Nov 2021 14:43:19 GMT  
		Size: 1.9 KB (1886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ee9788fbadb1fcccd7993a3740b96cf4b5df64a276961ad6b63e70e957c1d7e`  
		Last Modified: Wed, 17 Nov 2021 14:43:20 GMT  
		Size: 26.0 MB (25958946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:848fe08e27f2d543ede8fefd36f42933772911ba2b7f0e923743c37b030b134c`  
		Last Modified: Wed, 17 Nov 2021 14:43:17 GMT  
		Size: 864.6 KB (864617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6429b9ed205043e375a354efa42a61c9eab91c5212f97ca7d6e10729c094977a`  
		Last Modified: Wed, 17 Nov 2021 14:43:16 GMT  
		Size: 351.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ebbf6b1480dbd78c5fe8b0564e79d14f161cc3c5299d33b9e25780f013f2920`  
		Last Modified: Wed, 17 Nov 2021 14:43:17 GMT  
		Size: 295.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d88faad6b04ed2fcec177b3b962494c18eb2fcf4108e5b934c564aae3fe6327`  
		Last Modified: Wed, 17 Nov 2021 14:44:26 GMT  
		Size: 445.7 MB (445730572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:latest` - linux; s390x

```console
$ docker pull r-base@sha256:7b106be8884de22200d90e98b91b6b5274674316fa60f77de191353fd0c29680
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **488.9 MB (488884420 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7bde100730619821ee674761426150280663cff2c51998f7190d9900e6bee0d`
-	Default Command: `["R"]`

```dockerfile
# Wed, 17 Nov 2021 02:44:42 GMT
ADD file:6b07f3691aed718fdd31338ceb571ce22ffe4f9410f48df5c16f190258ace5ae in / 
# Wed, 17 Nov 2021 02:44:44 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 09:11:12 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Wed, 17 Nov 2021 09:11:13 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Wed, 17 Nov 2021 09:11:21 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:11:24 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Wed, 17 Nov 2021 09:11:24 GMT
ENV LC_ALL=en_US.UTF-8
# Wed, 17 Nov 2021 09:11:24 GMT
ENV LANG=en_US.UTF-8
# Wed, 17 Nov 2021 09:11:25 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Wed, 17 Nov 2021 09:11:25 GMT
ENV R_BASE_VERSION=4.1.2
# Wed, 17 Nov 2021 09:11:26 GMT
RUN echo "deb http://deb.debian.org/debian experimental main" > /etc/apt/sources.list.d/experimental.list     && echo "deb [trusted=yes] https://eddelbuettel.github.io/ppaR400 ./" > /etc/apt/sources.list.d/edd-r4.list
# Wed, 17 Nov 2021 09:12:34 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:12:48 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:1c02d7cb6bfcee3d40b1f3c9461f47e72e2f51d514b5df5ddb147d175da65910`  
		Last Modified: Wed, 17 Nov 2021 02:50:40 GMT  
		Size: 53.7 MB (53669187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:220be3db1df6258f3aebc2b3c4622ad1d8680871a31543d38ebe7489e54c2315`  
		Last Modified: Wed, 17 Nov 2021 09:13:10 GMT  
		Size: 1.9 KB (1878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56f884dbcc2d3fd82fbc93f59166b00e406e6a07742a0157b11a80334a41be2d`  
		Last Modified: Wed, 17 Nov 2021 09:13:11 GMT  
		Size: 25.7 MB (25730683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b66636dbcba0824a55dc895f4aaabefc24bae27999399c2ebc34234a6b3774cf`  
		Last Modified: Wed, 17 Nov 2021 09:13:08 GMT  
		Size: 920.2 KB (920188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c9afafbdb33d3171de360b123042c9933ec5bc0f41d7587f550e3b2d2a9dc6e`  
		Last Modified: Wed, 17 Nov 2021 09:13:08 GMT  
		Size: 351.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f886d7f25bf1d3e5164054de008592d645d12c6b8c7e8046304ac3271379d893`  
		Last Modified: Wed, 17 Nov 2021 09:13:08 GMT  
		Size: 294.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ced9a75a566e4589e4973141f9de7e687f32d617e6a47a3222b9f1c7c49ac17`  
		Last Modified: Wed, 17 Nov 2021 09:13:51 GMT  
		Size: 408.6 MB (408561839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
