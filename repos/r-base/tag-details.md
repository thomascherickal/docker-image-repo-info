<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `r-base`

-	[`r-base:4.1.2`](#r-base412)
-	[`r-base:latest`](#r-baselatest)

## `r-base:4.1.2`

```console
$ docker pull r-base@sha256:8889be1bbf8b4a2ce988940b729ce1e095ef192b0e05054ee35554166796dd38
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `r-base:4.1.2` - linux; amd64

```console
$ docker pull r-base@sha256:c78b5d720d82617849a7f28848ab7a8e08c1e03d1014e5fb13b069df89734eb9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **327.0 MB (327021596 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b5ec1f8ef98ab0900483ee414adfd92ae37452f8715ced3be34189963154819`
-	Default Command: `["R"]`

```dockerfile
# Tue, 12 Oct 2021 01:23:03 GMT
ADD file:7a2d92b4684fdb24b1c954a390700dbb0a50ce8cc8774b959e562a3652fb0456 in / 
# Tue, 12 Oct 2021 01:23:03 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 04:19:30 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Tue, 12 Oct 2021 04:19:31 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Tue, 12 Oct 2021 04:19:51 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 04:19:55 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Tue, 12 Oct 2021 04:19:56 GMT
ENV LC_ALL=en_US.UTF-8
# Tue, 12 Oct 2021 04:19:56 GMT
ENV LANG=en_US.UTF-8
# Tue, 12 Oct 2021 04:19:57 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Mon, 01 Nov 2021 23:44:59 GMT
ENV R_BASE_VERSION=4.1.2
# Mon, 01 Nov 2021 23:45:00 GMT
RUN echo "deb http://deb.debian.org/debian experimental main" > /etc/apt/sources.list.d/experimental.list     && echo "deb [trusted=yes] https://eddelbuettel.github.io/ppaR400 ./" > /etc/apt/sources.list.d/edd-r4.list
# Mon, 01 Nov 2021 23:45:48 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Mon, 01 Nov 2021 23:45:50 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:91c31f9cd4fd949265f5532465cddce98935dcfa86015a5348b5f47c344d67e0`  
		Last Modified: Tue, 12 Oct 2021 01:30:11 GMT  
		Size: 55.4 MB (55445865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e606e54707b66ea672b99397ad0143d3321576e29b913fffe5a7bbb0b2ce7a4a`  
		Last Modified: Tue, 12 Oct 2021 04:21:17 GMT  
		Size: 1.9 KB (1884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05a9125add45a3ab1be25e31cb56edcd59a930f04a18184138bf2fdc4da1d462`  
		Last Modified: Tue, 12 Oct 2021 04:21:20 GMT  
		Size: 25.7 MB (25674439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b99aa61fe4ddc891f7c96f41a1bff57bcd70f2e4a52fcd709178ae0917d00cb`  
		Last Modified: Tue, 12 Oct 2021 04:21:14 GMT  
		Size: 864.6 KB (864615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:177f6feb522e8e889e44c05679d843328ecb88d8d21ced741f9f2b7546a1a88d`  
		Last Modified: Tue, 12 Oct 2021 04:21:14 GMT  
		Size: 352.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d88edf447b3f77344d5001e55b9a52f1b3a0495d5112be28e3da8d3d075a03bf`  
		Last Modified: Mon, 01 Nov 2021 23:46:03 GMT  
		Size: 291.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd4b2e603d1cba3741abc6da0fd9f0b1daa11abdf14af473de6e91a8e41d691a`  
		Last Modified: Mon, 01 Nov 2021 23:46:31 GMT  
		Size: 245.0 MB (245034150 bytes)  
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
$ docker pull r-base@sha256:d3dbd97484977a43770f5e49aef51f32ffd077d526773d2d9f0945fa8a879c21
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **324.7 MB (324670267 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67d3d3b6fac5f60b747723e986c69878e42f8cd071d76ad8cf8cbef37eb7bef9`
-	Default Command: `["R"]`

```dockerfile
# Tue, 12 Oct 2021 01:29:42 GMT
ADD file:2920b1ef5c61978464fc969befdade3714d84884adee006fb93d4d89bb412093 in / 
# Tue, 12 Oct 2021 01:29:48 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 17:32:25 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Tue, 12 Oct 2021 17:32:41 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Tue, 12 Oct 2021 17:33:34 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 17:33:53 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Tue, 12 Oct 2021 17:34:03 GMT
ENV LC_ALL=en_US.UTF-8
# Tue, 12 Oct 2021 17:34:06 GMT
ENV LANG=en_US.UTF-8
# Tue, 12 Oct 2021 17:34:16 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Tue, 02 Nov 2021 00:43:11 GMT
ENV R_BASE_VERSION=4.1.2
# Tue, 02 Nov 2021 00:43:17 GMT
RUN echo "deb http://deb.debian.org/debian experimental main" > /etc/apt/sources.list.d/experimental.list     && echo "deb [trusted=yes] https://eddelbuettel.github.io/ppaR400 ./" > /etc/apt/sources.list.d/edd-r4.list
# Tue, 02 Nov 2021 00:50:15 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Tue, 02 Nov 2021 00:50:20 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:7695f94c27f2511cd3e23671d32882f166a2fc1b8124ec1f9d3f769e88536556`  
		Last Modified: Tue, 12 Oct 2021 01:43:25 GMT  
		Size: 59.7 MB (59659961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cf77696e867c8b3998bd381d9de600d9e5f8669138e0a2be69958974c7c9b64`  
		Last Modified: Tue, 12 Oct 2021 17:39:44 GMT  
		Size: 1.9 KB (1889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:946a3786f7cd6e7358f93ae0ca90340b4675e1029bbb6cb784ec059222ddf611`  
		Last Modified: Tue, 12 Oct 2021 17:39:45 GMT  
		Size: 25.9 MB (25890639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e767a06850ad738e951b6569fa5b7002c705294aacec9f544a4692b2ddd2f9de`  
		Last Modified: Tue, 12 Oct 2021 17:39:42 GMT  
		Size: 864.6 KB (864604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e2f5e9c5c6db95d8c42015f2e196a91a44c58a9c188a85a0c270543b63c4002`  
		Last Modified: Tue, 12 Oct 2021 17:39:41 GMT  
		Size: 352.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67e1f95094f5fa26ef464a1f54a821a5401d9782b0bb20eacdf01afc028cb2fb`  
		Last Modified: Tue, 02 Nov 2021 00:50:43 GMT  
		Size: 293.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac50c37b9129f5603d89b37a12063fd7b0af4cc3d93213a2d578c00cf02c0255`  
		Last Modified: Tue, 02 Nov 2021 00:51:20 GMT  
		Size: 238.3 MB (238252529 bytes)  
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
$ docker pull r-base@sha256:8889be1bbf8b4a2ce988940b729ce1e095ef192b0e05054ee35554166796dd38
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `r-base:latest` - linux; amd64

```console
$ docker pull r-base@sha256:c78b5d720d82617849a7f28848ab7a8e08c1e03d1014e5fb13b069df89734eb9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **327.0 MB (327021596 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b5ec1f8ef98ab0900483ee414adfd92ae37452f8715ced3be34189963154819`
-	Default Command: `["R"]`

```dockerfile
# Tue, 12 Oct 2021 01:23:03 GMT
ADD file:7a2d92b4684fdb24b1c954a390700dbb0a50ce8cc8774b959e562a3652fb0456 in / 
# Tue, 12 Oct 2021 01:23:03 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 04:19:30 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Tue, 12 Oct 2021 04:19:31 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Tue, 12 Oct 2021 04:19:51 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 04:19:55 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Tue, 12 Oct 2021 04:19:56 GMT
ENV LC_ALL=en_US.UTF-8
# Tue, 12 Oct 2021 04:19:56 GMT
ENV LANG=en_US.UTF-8
# Tue, 12 Oct 2021 04:19:57 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Mon, 01 Nov 2021 23:44:59 GMT
ENV R_BASE_VERSION=4.1.2
# Mon, 01 Nov 2021 23:45:00 GMT
RUN echo "deb http://deb.debian.org/debian experimental main" > /etc/apt/sources.list.d/experimental.list     && echo "deb [trusted=yes] https://eddelbuettel.github.io/ppaR400 ./" > /etc/apt/sources.list.d/edd-r4.list
# Mon, 01 Nov 2021 23:45:48 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Mon, 01 Nov 2021 23:45:50 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:91c31f9cd4fd949265f5532465cddce98935dcfa86015a5348b5f47c344d67e0`  
		Last Modified: Tue, 12 Oct 2021 01:30:11 GMT  
		Size: 55.4 MB (55445865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e606e54707b66ea672b99397ad0143d3321576e29b913fffe5a7bbb0b2ce7a4a`  
		Last Modified: Tue, 12 Oct 2021 04:21:17 GMT  
		Size: 1.9 KB (1884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05a9125add45a3ab1be25e31cb56edcd59a930f04a18184138bf2fdc4da1d462`  
		Last Modified: Tue, 12 Oct 2021 04:21:20 GMT  
		Size: 25.7 MB (25674439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b99aa61fe4ddc891f7c96f41a1bff57bcd70f2e4a52fcd709178ae0917d00cb`  
		Last Modified: Tue, 12 Oct 2021 04:21:14 GMT  
		Size: 864.6 KB (864615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:177f6feb522e8e889e44c05679d843328ecb88d8d21ced741f9f2b7546a1a88d`  
		Last Modified: Tue, 12 Oct 2021 04:21:14 GMT  
		Size: 352.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d88edf447b3f77344d5001e55b9a52f1b3a0495d5112be28e3da8d3d075a03bf`  
		Last Modified: Mon, 01 Nov 2021 23:46:03 GMT  
		Size: 291.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd4b2e603d1cba3741abc6da0fd9f0b1daa11abdf14af473de6e91a8e41d691a`  
		Last Modified: Mon, 01 Nov 2021 23:46:31 GMT  
		Size: 245.0 MB (245034150 bytes)  
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
$ docker pull r-base@sha256:d3dbd97484977a43770f5e49aef51f32ffd077d526773d2d9f0945fa8a879c21
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **324.7 MB (324670267 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67d3d3b6fac5f60b747723e986c69878e42f8cd071d76ad8cf8cbef37eb7bef9`
-	Default Command: `["R"]`

```dockerfile
# Tue, 12 Oct 2021 01:29:42 GMT
ADD file:2920b1ef5c61978464fc969befdade3714d84884adee006fb93d4d89bb412093 in / 
# Tue, 12 Oct 2021 01:29:48 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 17:32:25 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Tue, 12 Oct 2021 17:32:41 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Tue, 12 Oct 2021 17:33:34 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 17:33:53 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Tue, 12 Oct 2021 17:34:03 GMT
ENV LC_ALL=en_US.UTF-8
# Tue, 12 Oct 2021 17:34:06 GMT
ENV LANG=en_US.UTF-8
# Tue, 12 Oct 2021 17:34:16 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Tue, 02 Nov 2021 00:43:11 GMT
ENV R_BASE_VERSION=4.1.2
# Tue, 02 Nov 2021 00:43:17 GMT
RUN echo "deb http://deb.debian.org/debian experimental main" > /etc/apt/sources.list.d/experimental.list     && echo "deb [trusted=yes] https://eddelbuettel.github.io/ppaR400 ./" > /etc/apt/sources.list.d/edd-r4.list
# Tue, 02 Nov 2021 00:50:15 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Tue, 02 Nov 2021 00:50:20 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:7695f94c27f2511cd3e23671d32882f166a2fc1b8124ec1f9d3f769e88536556`  
		Last Modified: Tue, 12 Oct 2021 01:43:25 GMT  
		Size: 59.7 MB (59659961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cf77696e867c8b3998bd381d9de600d9e5f8669138e0a2be69958974c7c9b64`  
		Last Modified: Tue, 12 Oct 2021 17:39:44 GMT  
		Size: 1.9 KB (1889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:946a3786f7cd6e7358f93ae0ca90340b4675e1029bbb6cb784ec059222ddf611`  
		Last Modified: Tue, 12 Oct 2021 17:39:45 GMT  
		Size: 25.9 MB (25890639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e767a06850ad738e951b6569fa5b7002c705294aacec9f544a4692b2ddd2f9de`  
		Last Modified: Tue, 12 Oct 2021 17:39:42 GMT  
		Size: 864.6 KB (864604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e2f5e9c5c6db95d8c42015f2e196a91a44c58a9c188a85a0c270543b63c4002`  
		Last Modified: Tue, 12 Oct 2021 17:39:41 GMT  
		Size: 352.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67e1f95094f5fa26ef464a1f54a821a5401d9782b0bb20eacdf01afc028cb2fb`  
		Last Modified: Tue, 02 Nov 2021 00:50:43 GMT  
		Size: 293.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac50c37b9129f5603d89b37a12063fd7b0af4cc3d93213a2d578c00cf02c0255`  
		Last Modified: Tue, 02 Nov 2021 00:51:20 GMT  
		Size: 238.3 MB (238252529 bytes)  
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
