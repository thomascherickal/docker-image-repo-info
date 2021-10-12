<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `r-base`

-	[`r-base:4.1.1`](#r-base411)
-	[`r-base:latest`](#r-baselatest)

## `r-base:4.1.1`

```console
$ docker pull r-base@sha256:73b9989359e99ff333081f681ead845bd0a655fdce7881edcb31f00e3cb20b08
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `r-base:4.1.1` - linux; amd64

```console
$ docker pull r-base@sha256:393a8527b6c2d9a1611f47d3632e2217294f0de07fe34ea23ad41e19c91f4880
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **327.4 MB (327445996 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4734d8463a2a9c4c1beab180bac06698fd44543e7a396d1c9a614e3ff1673a6`
-	Default Command: `["R"]`

```dockerfile
# Tue, 28 Sep 2021 01:25:43 GMT
ADD file:296666bd4e40daac711ea6d013efc43f7c50e58222b69b3d7116e4f5aa2c9e91 in / 
# Tue, 28 Sep 2021 01:25:44 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 20:51:30 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Tue, 28 Sep 2021 20:51:31 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Tue, 28 Sep 2021 20:51:55 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 20:51:59 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Tue, 28 Sep 2021 20:51:59 GMT
ENV LC_ALL=en_US.UTF-8
# Tue, 28 Sep 2021 20:52:00 GMT
ENV LANG=en_US.UTF-8
# Tue, 28 Sep 2021 20:52:01 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Tue, 28 Sep 2021 20:52:01 GMT
ENV R_BASE_VERSION=4.1.1
# Tue, 28 Sep 2021 20:52:02 GMT
RUN echo "deb http://deb.debian.org/debian experimental main" > /etc/apt/sources.list.d/experimental.list     && echo "deb [trusted=yes] https://eddelbuettel.github.io/ppaR400 ./" > /etc/apt/sources.list.d/edd-r4.list
# Tue, 28 Sep 2021 20:52:57 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 20:52:59 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:8cbc26cedebcd0983d6a6ef269bc8a686ef391b21a05f40917e03b8bc050f5f8`  
		Last Modified: Tue, 28 Sep 2021 01:33:13 GMT  
		Size: 55.4 MB (55449438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af2d070bb092134231905833ee228b059cf033c60d8da938dcf9944494b56c00`  
		Last Modified: Tue, 28 Sep 2021 20:53:18 GMT  
		Size: 1.9 KB (1875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a503e21d994c7cd2dbd87d3aa98afae29ff512edfe4ada36bda1c31652d012bf`  
		Last Modified: Tue, 28 Sep 2021 20:53:20 GMT  
		Size: 25.6 MB (25590367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22034b2cea6d05a16ab2938346475ee7217589865e4aac9d81c79afad68650d5`  
		Last Modified: Tue, 28 Sep 2021 20:53:17 GMT  
		Size: 864.6 KB (864613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cccc7912287e313be39a347097477cbb24f6b4372be61cada2b53baab0c0589`  
		Last Modified: Tue, 28 Sep 2021 20:53:16 GMT  
		Size: 346.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5a6a3142fe7ea68f1ad364050a158aaa3425f4c61f414ba5baed3825cb9fda4`  
		Last Modified: Tue, 28 Sep 2021 20:53:16 GMT  
		Size: 294.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9490c9cd4280f18d762dd0389dbe1f017b5dd55332a52f9e733de4fbe3f9fe60`  
		Last Modified: Tue, 28 Sep 2021 20:53:47 GMT  
		Size: 245.5 MB (245539063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:4.1.1` - linux; arm64 variant v8

```console
$ docker pull r-base@sha256:7ff20f200fd93a183172cc5d93507905616716761ece241ce7bdc6c58053badf
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **315.2 MB (315169992 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43004d0e92e411698b6433ac491de990ab6dac85081ecfffbefd47ddf753744b`
-	Default Command: `["R"]`

```dockerfile
# Tue, 28 Sep 2021 01:43:39 GMT
ADD file:df28df42dbd83dc9e69cbc59efab23a55fd0a6252480edbc355435be4e55acf0 in / 
# Tue, 28 Sep 2021 01:43:40 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 15:49:32 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Tue, 28 Sep 2021 15:49:33 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Tue, 28 Sep 2021 15:49:42 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 15:49:45 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Tue, 28 Sep 2021 15:49:45 GMT
ENV LC_ALL=en_US.UTF-8
# Tue, 28 Sep 2021 15:49:45 GMT
ENV LANG=en_US.UTF-8
# Tue, 28 Sep 2021 15:49:46 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Tue, 28 Sep 2021 15:49:46 GMT
ENV R_BASE_VERSION=4.1.1
# Tue, 28 Sep 2021 15:49:47 GMT
RUN echo "deb http://deb.debian.org/debian experimental main" > /etc/apt/sources.list.d/experimental.list     && echo "deb [trusted=yes] https://eddelbuettel.github.io/ppaR400 ./" > /etc/apt/sources.list.d/edd-r4.list
# Tue, 28 Sep 2021 15:50:37 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 15:50:39 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:5fd04373f6dc4ec57b4af01b70782245fdb26a426888b8d0fe9169590ef679b7`  
		Last Modified: Tue, 28 Sep 2021 01:53:17 GMT  
		Size: 54.5 MB (54460337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e418464f49f41ba43443d77e90ee257ef0a60fe422389cdafa9171100bc6f12`  
		Last Modified: Tue, 28 Sep 2021 15:50:55 GMT  
		Size: 1.9 KB (1876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eda43c359b84724a6c7d59c423387ac97b8239a3baaf96b2ad044d38da7a7690`  
		Last Modified: Tue, 28 Sep 2021 15:50:56 GMT  
		Size: 25.6 MB (25578065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e5391d63d29be63b22f7c888d0bb3e63b310b48bdfdef14c73b0d51e306fcbf`  
		Last Modified: Tue, 28 Sep 2021 15:50:53 GMT  
		Size: 864.6 KB (864613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd4ad37830882347e1b2d1d2239d283be294c35899483487b278ea18e5cf8e86`  
		Last Modified: Tue, 28 Sep 2021 15:50:53 GMT  
		Size: 348.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebba437b4f1d5d81167585c32a6dbab9cebda1f1d2bae7ac44600c4fcfd74e6c`  
		Last Modified: Tue, 28 Sep 2021 15:50:53 GMT  
		Size: 292.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54c9f61c3faaebe463cb4b6be3f6204e78a5639450d8a2380ce64fc8fac2da5e`  
		Last Modified: Tue, 28 Sep 2021 15:51:22 GMT  
		Size: 234.3 MB (234264461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:4.1.1` - linux; ppc64le

```console
$ docker pull r-base@sha256:108a285e97c8daf6739e305e9144b541f156f7096c4111c7089ab80e2d6395ca
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **326.8 MB (326834781 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3b1f95041cbafb9534bd01d9a6de3d6bf53cf9e964db3b0d47da069560b0e67`
-	Default Command: `["R"]`

```dockerfile
# Mon, 04 Oct 2021 17:59:57 GMT
ADD file:860aa6ad37b72de17204c9725c5b6bf1dec8db9354823aaa30ecfb615a55a95d in / 
# Mon, 04 Oct 2021 18:00:16 GMT
CMD ["bash"]
# Wed, 06 Oct 2021 04:07:57 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Wed, 06 Oct 2021 04:08:08 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Wed, 06 Oct 2021 04:08:47 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Wed, 06 Oct 2021 04:08:58 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Wed, 06 Oct 2021 04:09:00 GMT
ENV LC_ALL=en_US.UTF-8
# Wed, 06 Oct 2021 04:09:02 GMT
ENV LANG=en_US.UTF-8
# Wed, 06 Oct 2021 04:09:06 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Wed, 06 Oct 2021 04:09:09 GMT
ENV R_BASE_VERSION=4.1.1
# Wed, 06 Oct 2021 04:09:13 GMT
RUN echo "deb http://deb.debian.org/debian experimental main" > /etc/apt/sources.list.d/experimental.list     && echo "deb [trusted=yes] https://eddelbuettel.github.io/ppaR400 ./" > /etc/apt/sources.list.d/edd-r4.list
# Wed, 06 Oct 2021 04:14:19 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Wed, 06 Oct 2021 04:14:24 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:853d7acee2fa27387849744262847f6771f124451c1663f073c0e2c41a263a08`  
		Last Modified: Mon, 04 Oct 2021 18:11:22 GMT  
		Size: 59.6 MB (59638250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:651bf5ce47445913f99b1613948b3b17de8f68097d43fdd10e466d17a0fcd07d`  
		Last Modified: Wed, 06 Oct 2021 04:14:49 GMT  
		Size: 1.9 KB (1892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94dd96247a17aaebc6192130b2ac7ebeb140942978b81f84c662fce837ee2adb`  
		Last Modified: Wed, 06 Oct 2021 04:14:52 GMT  
		Size: 25.9 MB (25890662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c189aeb3b9a08395e364d17dca1eea60f6149b126ec61531fa9f633ccdb569cf`  
		Last Modified: Wed, 06 Oct 2021 04:14:47 GMT  
		Size: 864.6 KB (864616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05c5ae11d837acbfded16ba4d6c8325d7329331c795e6eb21dbbcecbd4aeb8a4`  
		Last Modified: Wed, 06 Oct 2021 04:14:47 GMT  
		Size: 351.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9bda0c3a0c954c250da3baba078cee1245e637f8effe7c89a6c7f1da70609e9`  
		Last Modified: Wed, 06 Oct 2021 04:14:47 GMT  
		Size: 295.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:241342fb7890d174cbb0c5cf5f4e456aa7c885a911afba147b053b2c66b2602a`  
		Last Modified: Wed, 06 Oct 2021 04:15:25 GMT  
		Size: 240.4 MB (240438715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:4.1.1` - linux; s390x

```console
$ docker pull r-base@sha256:d48eb276898d6214b3299db215a8d449bb969d31afa0e710c21c8f6595fce2b6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **291.2 MB (291181086 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7bcf5b35b3235de3e1f0b0f051a16cbe60d954f3f31ad2e3edea611ec9fefb52`
-	Default Command: `["R"]`

```dockerfile
# Tue, 12 Oct 2021 00:44:24 GMT
ADD file:6bdd28da982bbaaa3e5fd43949b430a741f7441a3423aea45476b602884003fb in / 
# Tue, 12 Oct 2021 00:44:27 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 03:55:15 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Tue, 12 Oct 2021 03:55:15 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Tue, 12 Oct 2021 03:55:24 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 03:55:26 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Tue, 12 Oct 2021 03:55:26 GMT
ENV LC_ALL=en_US.UTF-8
# Tue, 12 Oct 2021 03:55:26 GMT
ENV LANG=en_US.UTF-8
# Tue, 12 Oct 2021 03:55:27 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Tue, 12 Oct 2021 03:55:27 GMT
ENV R_BASE_VERSION=4.1.1
# Tue, 12 Oct 2021 03:55:27 GMT
RUN echo "deb http://deb.debian.org/debian experimental main" > /etc/apt/sources.list.d/experimental.list     && echo "deb [trusted=yes] https://eddelbuettel.github.io/ppaR400 ./" > /etc/apt/sources.list.d/edd-r4.list
# Tue, 12 Oct 2021 03:56:20 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 03:56:27 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:16455b9c3f308b090e540412543381f2981a94842cb89496c8f0d1636c7ad1da`  
		Last Modified: Tue, 12 Oct 2021 00:50:24 GMT  
		Size: 53.7 MB (53700056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66820cf6e7ced7ad3ac27a4b228a9ca7103ab45d324da00389cc635fd47000eb`  
		Last Modified: Tue, 12 Oct 2021 03:56:41 GMT  
		Size: 1.9 KB (1878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc12fcbdd62d39e938a41b846683ed945db78f64839cd7675068c0d888caf6e0`  
		Last Modified: Tue, 12 Oct 2021 03:56:42 GMT  
		Size: 25.7 MB (25682113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c24b3fac5234b68eef44919f692d1c7ccad29dd64834bbcf9507d97d7c31a1a4`  
		Last Modified: Tue, 12 Oct 2021 03:56:40 GMT  
		Size: 920.2 KB (920189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fabacf418fbbc1661e5d053c1bd36686a83ec085ea0aea52cba734045d5fd5c`  
		Last Modified: Tue, 12 Oct 2021 03:56:40 GMT  
		Size: 349.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07367af9be3475873d31613b5dac5c8d00d3e12e662baf229e1bab8f5285eaf8`  
		Last Modified: Tue, 12 Oct 2021 03:56:40 GMT  
		Size: 293.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2be81bf02a0c12602cd899edd23ef7f402240f848111d7a376cefbaca14130ec`  
		Last Modified: Tue, 12 Oct 2021 03:57:00 GMT  
		Size: 210.9 MB (210876208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `r-base:latest`

```console
$ docker pull r-base@sha256:73b9989359e99ff333081f681ead845bd0a655fdce7881edcb31f00e3cb20b08
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `r-base:latest` - linux; amd64

```console
$ docker pull r-base@sha256:393a8527b6c2d9a1611f47d3632e2217294f0de07fe34ea23ad41e19c91f4880
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **327.4 MB (327445996 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4734d8463a2a9c4c1beab180bac06698fd44543e7a396d1c9a614e3ff1673a6`
-	Default Command: `["R"]`

```dockerfile
# Tue, 28 Sep 2021 01:25:43 GMT
ADD file:296666bd4e40daac711ea6d013efc43f7c50e58222b69b3d7116e4f5aa2c9e91 in / 
# Tue, 28 Sep 2021 01:25:44 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 20:51:30 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Tue, 28 Sep 2021 20:51:31 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Tue, 28 Sep 2021 20:51:55 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 20:51:59 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Tue, 28 Sep 2021 20:51:59 GMT
ENV LC_ALL=en_US.UTF-8
# Tue, 28 Sep 2021 20:52:00 GMT
ENV LANG=en_US.UTF-8
# Tue, 28 Sep 2021 20:52:01 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Tue, 28 Sep 2021 20:52:01 GMT
ENV R_BASE_VERSION=4.1.1
# Tue, 28 Sep 2021 20:52:02 GMT
RUN echo "deb http://deb.debian.org/debian experimental main" > /etc/apt/sources.list.d/experimental.list     && echo "deb [trusted=yes] https://eddelbuettel.github.io/ppaR400 ./" > /etc/apt/sources.list.d/edd-r4.list
# Tue, 28 Sep 2021 20:52:57 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 20:52:59 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:8cbc26cedebcd0983d6a6ef269bc8a686ef391b21a05f40917e03b8bc050f5f8`  
		Last Modified: Tue, 28 Sep 2021 01:33:13 GMT  
		Size: 55.4 MB (55449438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af2d070bb092134231905833ee228b059cf033c60d8da938dcf9944494b56c00`  
		Last Modified: Tue, 28 Sep 2021 20:53:18 GMT  
		Size: 1.9 KB (1875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a503e21d994c7cd2dbd87d3aa98afae29ff512edfe4ada36bda1c31652d012bf`  
		Last Modified: Tue, 28 Sep 2021 20:53:20 GMT  
		Size: 25.6 MB (25590367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22034b2cea6d05a16ab2938346475ee7217589865e4aac9d81c79afad68650d5`  
		Last Modified: Tue, 28 Sep 2021 20:53:17 GMT  
		Size: 864.6 KB (864613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cccc7912287e313be39a347097477cbb24f6b4372be61cada2b53baab0c0589`  
		Last Modified: Tue, 28 Sep 2021 20:53:16 GMT  
		Size: 346.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5a6a3142fe7ea68f1ad364050a158aaa3425f4c61f414ba5baed3825cb9fda4`  
		Last Modified: Tue, 28 Sep 2021 20:53:16 GMT  
		Size: 294.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9490c9cd4280f18d762dd0389dbe1f017b5dd55332a52f9e733de4fbe3f9fe60`  
		Last Modified: Tue, 28 Sep 2021 20:53:47 GMT  
		Size: 245.5 MB (245539063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:latest` - linux; arm64 variant v8

```console
$ docker pull r-base@sha256:7ff20f200fd93a183172cc5d93507905616716761ece241ce7bdc6c58053badf
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **315.2 MB (315169992 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43004d0e92e411698b6433ac491de990ab6dac85081ecfffbefd47ddf753744b`
-	Default Command: `["R"]`

```dockerfile
# Tue, 28 Sep 2021 01:43:39 GMT
ADD file:df28df42dbd83dc9e69cbc59efab23a55fd0a6252480edbc355435be4e55acf0 in / 
# Tue, 28 Sep 2021 01:43:40 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 15:49:32 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Tue, 28 Sep 2021 15:49:33 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Tue, 28 Sep 2021 15:49:42 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 15:49:45 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Tue, 28 Sep 2021 15:49:45 GMT
ENV LC_ALL=en_US.UTF-8
# Tue, 28 Sep 2021 15:49:45 GMT
ENV LANG=en_US.UTF-8
# Tue, 28 Sep 2021 15:49:46 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Tue, 28 Sep 2021 15:49:46 GMT
ENV R_BASE_VERSION=4.1.1
# Tue, 28 Sep 2021 15:49:47 GMT
RUN echo "deb http://deb.debian.org/debian experimental main" > /etc/apt/sources.list.d/experimental.list     && echo "deb [trusted=yes] https://eddelbuettel.github.io/ppaR400 ./" > /etc/apt/sources.list.d/edd-r4.list
# Tue, 28 Sep 2021 15:50:37 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 15:50:39 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:5fd04373f6dc4ec57b4af01b70782245fdb26a426888b8d0fe9169590ef679b7`  
		Last Modified: Tue, 28 Sep 2021 01:53:17 GMT  
		Size: 54.5 MB (54460337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e418464f49f41ba43443d77e90ee257ef0a60fe422389cdafa9171100bc6f12`  
		Last Modified: Tue, 28 Sep 2021 15:50:55 GMT  
		Size: 1.9 KB (1876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eda43c359b84724a6c7d59c423387ac97b8239a3baaf96b2ad044d38da7a7690`  
		Last Modified: Tue, 28 Sep 2021 15:50:56 GMT  
		Size: 25.6 MB (25578065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e5391d63d29be63b22f7c888d0bb3e63b310b48bdfdef14c73b0d51e306fcbf`  
		Last Modified: Tue, 28 Sep 2021 15:50:53 GMT  
		Size: 864.6 KB (864613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd4ad37830882347e1b2d1d2239d283be294c35899483487b278ea18e5cf8e86`  
		Last Modified: Tue, 28 Sep 2021 15:50:53 GMT  
		Size: 348.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebba437b4f1d5d81167585c32a6dbab9cebda1f1d2bae7ac44600c4fcfd74e6c`  
		Last Modified: Tue, 28 Sep 2021 15:50:53 GMT  
		Size: 292.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54c9f61c3faaebe463cb4b6be3f6204e78a5639450d8a2380ce64fc8fac2da5e`  
		Last Modified: Tue, 28 Sep 2021 15:51:22 GMT  
		Size: 234.3 MB (234264461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:latest` - linux; ppc64le

```console
$ docker pull r-base@sha256:108a285e97c8daf6739e305e9144b541f156f7096c4111c7089ab80e2d6395ca
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **326.8 MB (326834781 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3b1f95041cbafb9534bd01d9a6de3d6bf53cf9e964db3b0d47da069560b0e67`
-	Default Command: `["R"]`

```dockerfile
# Mon, 04 Oct 2021 17:59:57 GMT
ADD file:860aa6ad37b72de17204c9725c5b6bf1dec8db9354823aaa30ecfb615a55a95d in / 
# Mon, 04 Oct 2021 18:00:16 GMT
CMD ["bash"]
# Wed, 06 Oct 2021 04:07:57 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Wed, 06 Oct 2021 04:08:08 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Wed, 06 Oct 2021 04:08:47 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Wed, 06 Oct 2021 04:08:58 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Wed, 06 Oct 2021 04:09:00 GMT
ENV LC_ALL=en_US.UTF-8
# Wed, 06 Oct 2021 04:09:02 GMT
ENV LANG=en_US.UTF-8
# Wed, 06 Oct 2021 04:09:06 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Wed, 06 Oct 2021 04:09:09 GMT
ENV R_BASE_VERSION=4.1.1
# Wed, 06 Oct 2021 04:09:13 GMT
RUN echo "deb http://deb.debian.org/debian experimental main" > /etc/apt/sources.list.d/experimental.list     && echo "deb [trusted=yes] https://eddelbuettel.github.io/ppaR400 ./" > /etc/apt/sources.list.d/edd-r4.list
# Wed, 06 Oct 2021 04:14:19 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Wed, 06 Oct 2021 04:14:24 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:853d7acee2fa27387849744262847f6771f124451c1663f073c0e2c41a263a08`  
		Last Modified: Mon, 04 Oct 2021 18:11:22 GMT  
		Size: 59.6 MB (59638250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:651bf5ce47445913f99b1613948b3b17de8f68097d43fdd10e466d17a0fcd07d`  
		Last Modified: Wed, 06 Oct 2021 04:14:49 GMT  
		Size: 1.9 KB (1892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94dd96247a17aaebc6192130b2ac7ebeb140942978b81f84c662fce837ee2adb`  
		Last Modified: Wed, 06 Oct 2021 04:14:52 GMT  
		Size: 25.9 MB (25890662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c189aeb3b9a08395e364d17dca1eea60f6149b126ec61531fa9f633ccdb569cf`  
		Last Modified: Wed, 06 Oct 2021 04:14:47 GMT  
		Size: 864.6 KB (864616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05c5ae11d837acbfded16ba4d6c8325d7329331c795e6eb21dbbcecbd4aeb8a4`  
		Last Modified: Wed, 06 Oct 2021 04:14:47 GMT  
		Size: 351.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9bda0c3a0c954c250da3baba078cee1245e637f8effe7c89a6c7f1da70609e9`  
		Last Modified: Wed, 06 Oct 2021 04:14:47 GMT  
		Size: 295.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:241342fb7890d174cbb0c5cf5f4e456aa7c885a911afba147b053b2c66b2602a`  
		Last Modified: Wed, 06 Oct 2021 04:15:25 GMT  
		Size: 240.4 MB (240438715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:latest` - linux; s390x

```console
$ docker pull r-base@sha256:d48eb276898d6214b3299db215a8d449bb969d31afa0e710c21c8f6595fce2b6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **291.2 MB (291181086 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7bcf5b35b3235de3e1f0b0f051a16cbe60d954f3f31ad2e3edea611ec9fefb52`
-	Default Command: `["R"]`

```dockerfile
# Tue, 12 Oct 2021 00:44:24 GMT
ADD file:6bdd28da982bbaaa3e5fd43949b430a741f7441a3423aea45476b602884003fb in / 
# Tue, 12 Oct 2021 00:44:27 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 03:55:15 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Tue, 12 Oct 2021 03:55:15 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Tue, 12 Oct 2021 03:55:24 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 03:55:26 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Tue, 12 Oct 2021 03:55:26 GMT
ENV LC_ALL=en_US.UTF-8
# Tue, 12 Oct 2021 03:55:26 GMT
ENV LANG=en_US.UTF-8
# Tue, 12 Oct 2021 03:55:27 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Tue, 12 Oct 2021 03:55:27 GMT
ENV R_BASE_VERSION=4.1.1
# Tue, 12 Oct 2021 03:55:27 GMT
RUN echo "deb http://deb.debian.org/debian experimental main" > /etc/apt/sources.list.d/experimental.list     && echo "deb [trusted=yes] https://eddelbuettel.github.io/ppaR400 ./" > /etc/apt/sources.list.d/edd-r4.list
# Tue, 12 Oct 2021 03:56:20 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 03:56:27 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:16455b9c3f308b090e540412543381f2981a94842cb89496c8f0d1636c7ad1da`  
		Last Modified: Tue, 12 Oct 2021 00:50:24 GMT  
		Size: 53.7 MB (53700056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66820cf6e7ced7ad3ac27a4b228a9ca7103ab45d324da00389cc635fd47000eb`  
		Last Modified: Tue, 12 Oct 2021 03:56:41 GMT  
		Size: 1.9 KB (1878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc12fcbdd62d39e938a41b846683ed945db78f64839cd7675068c0d888caf6e0`  
		Last Modified: Tue, 12 Oct 2021 03:56:42 GMT  
		Size: 25.7 MB (25682113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c24b3fac5234b68eef44919f692d1c7ccad29dd64834bbcf9507d97d7c31a1a4`  
		Last Modified: Tue, 12 Oct 2021 03:56:40 GMT  
		Size: 920.2 KB (920189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fabacf418fbbc1661e5d053c1bd36686a83ec085ea0aea52cba734045d5fd5c`  
		Last Modified: Tue, 12 Oct 2021 03:56:40 GMT  
		Size: 349.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07367af9be3475873d31613b5dac5c8d00d3e12e662baf229e1bab8f5285eaf8`  
		Last Modified: Tue, 12 Oct 2021 03:56:40 GMT  
		Size: 293.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2be81bf02a0c12602cd899edd23ef7f402240f848111d7a376cefbaca14130ec`  
		Last Modified: Tue, 12 Oct 2021 03:57:00 GMT  
		Size: 210.9 MB (210876208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
