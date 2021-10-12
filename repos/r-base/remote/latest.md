## `r-base:latest`

```console
$ docker pull r-base@sha256:02ed1988c1e7de0a70ea5a74fa4814cab5cc7008c779eba856af7d194336ffd9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `r-base:latest` - linux; amd64

```console
$ docker pull r-base@sha256:967b9d2c0474c63761305f8f1abec4a3a9426ceff98497dd7a3ba44d468711f3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **325.7 MB (325670166 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85d4d9dc4d6e23927b3c5c7daa208aa99e52c4239b401ea45ae323d3b8ebfd4e`
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
# Tue, 12 Oct 2021 04:19:58 GMT
ENV R_BASE_VERSION=4.1.1
# Tue, 12 Oct 2021 04:19:59 GMT
RUN echo "deb http://deb.debian.org/debian experimental main" > /etc/apt/sources.list.d/experimental.list     && echo "deb [trusted=yes] https://eddelbuettel.github.io/ppaR400 ./" > /etc/apt/sources.list.d/edd-r4.list
# Tue, 12 Oct 2021 04:21:02 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 04:21:04 GMT
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
	-	`sha256:02111200925ff787552c783fdea72a70c6369ddc71d03496eeab67bb01c0595b`  
		Last Modified: Tue, 12 Oct 2021 04:21:14 GMT  
		Size: 296.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1d156550b41c2e1480c9bc3d8ce7f923ae98039b5162b3aa5511add7dd77367`  
		Last Modified: Tue, 12 Oct 2021 04:21:52 GMT  
		Size: 243.7 MB (243682715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:latest` - linux; arm64 variant v8

```console
$ docker pull r-base@sha256:063ba124bdd92a89cf3a351310fa5742c0d74a549bc388a41936c4ec4a0d8ea9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **313.1 MB (313090907 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ca33888415fd2e0069ce26e75eef1224da73a874ffe8aea66272c8c67da49b8`
-	Default Command: `["R"]`

```dockerfile
# Tue, 12 Oct 2021 01:43:39 GMT
ADD file:0d2781f09dc7fd32dad3f41e34a91046910847a56bf128bb53a7cad6c06c1f26 in / 
# Tue, 12 Oct 2021 01:43:40 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 16:10:09 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Tue, 12 Oct 2021 16:10:10 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Tue, 12 Oct 2021 16:10:18 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 16:10:21 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Tue, 12 Oct 2021 16:10:21 GMT
ENV LC_ALL=en_US.UTF-8
# Tue, 12 Oct 2021 16:10:21 GMT
ENV LANG=en_US.UTF-8
# Tue, 12 Oct 2021 16:10:22 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Tue, 12 Oct 2021 16:10:22 GMT
ENV R_BASE_VERSION=4.1.1
# Tue, 12 Oct 2021 16:10:22 GMT
RUN echo "deb http://deb.debian.org/debian experimental main" > /etc/apt/sources.list.d/experimental.list     && echo "deb [trusted=yes] https://eddelbuettel.github.io/ppaR400 ./" > /etc/apt/sources.list.d/edd-r4.list
# Tue, 12 Oct 2021 16:11:08 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 16:11:09 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:0a75495c66c5fc986e1fa178fa94fe24ac603e1ee8a61ff4b344624e0b8b030e`  
		Last Modified: Tue, 12 Oct 2021 01:52:57 GMT  
		Size: 54.5 MB (54465025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a739ac24a0cd2004556208bc3ac6c5b71f88e963f0e3fa5dfac3ef8086b16b2`  
		Last Modified: Tue, 12 Oct 2021 16:11:29 GMT  
		Size: 1.9 KB (1878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8aca33f1839ce6af2591355ac9fb4ce58339b2f441675283e9f16c627bee0cd8`  
		Last Modified: Tue, 12 Oct 2021 16:11:30 GMT  
		Size: 25.7 MB (25668650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d09fe657412f8dbc739ad63b8de4b7e60934338f7038de685ce65c208f0112cb`  
		Last Modified: Tue, 12 Oct 2021 16:11:27 GMT  
		Size: 864.6 KB (864603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3cc0c3b4b4cb40836415234a2cf4e996a0a5852d297431097ac6d69e6d5fbb2`  
		Last Modified: Tue, 12 Oct 2021 16:11:27 GMT  
		Size: 348.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91f5df83b03429358cd38e241a80e22a6044e9753ba207cfbfc39b9efeeabb77`  
		Last Modified: Tue, 12 Oct 2021 16:11:27 GMT  
		Size: 294.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eb80eb5b61cae7883e70e06978728856613108fa4ce7004b0595f8365192340`  
		Last Modified: Tue, 12 Oct 2021 16:11:56 GMT  
		Size: 232.1 MB (232090109 bytes)  
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
