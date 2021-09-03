<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `r-base`

-	[`r-base:4.1.1`](#r-base411)
-	[`r-base:latest`](#r-baselatest)

## `r-base:4.1.1`

```console
$ docker pull r-base@sha256:06ec747f404da004ee6508845d11cfa9807f150623868ede0c1201bd63bf59f9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `r-base:4.1.1` - linux; amd64

```console
$ docker pull r-base@sha256:e3db99ecd00477e755f44ebdf20eb89c0b25c7a80b0c5085d818fa60217891d4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **323.6 MB (323573190 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c27c3714f0049e58f90167840d1df16be91dc4240b2ee4e0278b869d2bd3d7ad`
-	Default Command: `["R"]`

```dockerfile
# Tue, 17 Aug 2021 01:26:21 GMT
ADD file:78a808c11f084f171360ce87535de573285eb3f06602698c86bc2007a307299e in / 
# Tue, 17 Aug 2021 01:26:21 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 14:25:49 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Tue, 17 Aug 2021 14:25:51 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Tue, 17 Aug 2021 14:26:02 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 14:26:05 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Tue, 17 Aug 2021 14:26:06 GMT
ENV LC_ALL=en_US.UTF-8
# Tue, 17 Aug 2021 14:26:06 GMT
ENV LANG=en_US.UTF-8
# Tue, 17 Aug 2021 14:26:07 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Tue, 17 Aug 2021 14:26:07 GMT
ENV R_BASE_VERSION=4.1.1
# Tue, 17 Aug 2021 14:26:08 GMT
RUN echo "deb http://deb.debian.org/debian experimental main" > /etc/apt/sources.list.d/experimental.list     && echo "deb [trusted=yes] https://eddelbuettel.github.io/ppaR400 ./" > /etc/apt/sources.list.d/edd-r4.list
# Tue, 17 Aug 2021 14:26:57 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 14:26:59 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:a42321116e438acfff1628527f7ae9e433d1ece73a19aecf4b4642d110d317fd`  
		Last Modified: Tue, 17 Aug 2021 01:33:48 GMT  
		Size: 54.9 MB (54909547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f412a7fda1e6aa9b5a01156374a3c4dcdc0e94a6596855d76138099924e0393`  
		Last Modified: Tue, 17 Aug 2021 14:27:23 GMT  
		Size: 1.9 KB (1874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fab087860f757d5a41f3d47c44c636e9035e23f37eeefd64c68d787923157043`  
		Last Modified: Tue, 17 Aug 2021 14:27:24 GMT  
		Size: 25.6 MB (25629954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25d5624c76ed18f8cd357135ed0f589838912b7c77dfff99d35eb5a93a6d4afc`  
		Last Modified: Tue, 17 Aug 2021 14:27:20 GMT  
		Size: 864.6 KB (864591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb56c0554b1798004d8fd95e6c888bb9ed6e35b9bb4ddb0b5d5020e2c90b0b7f`  
		Last Modified: Tue, 17 Aug 2021 14:27:21 GMT  
		Size: 349.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:409cf8ce22d9c250de0d27c42585f48d5154ec07fde7bc1b6b4550696e0d1dc2`  
		Last Modified: Tue, 17 Aug 2021 14:27:20 GMT  
		Size: 292.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08aa39b001b7c5244ae2171c9b8d2fcdda23c385d043fae650ff1d6c10f30578`  
		Last Modified: Tue, 17 Aug 2021 14:27:56 GMT  
		Size: 242.2 MB (242166583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:4.1.1` - linux; arm64 variant v8

```console
$ docker pull r-base@sha256:15bcdf78a283096928a79a276f3bf4b7bf8390e564df6527b79cc6634a414248
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **312.4 MB (312412401 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2b01c676c4159ccf0e5bd8fa641aec2d26e2256ab57bfcdf9344322c208896b`
-	Default Command: `["R"]`

```dockerfile
# Fri, 03 Sep 2021 00:42:59 GMT
ADD file:024a3f01f7d5ed6ce6f4ee6507a0dbb6edefe3267e1672fb07b5e5eae29a47b7 in / 
# Fri, 03 Sep 2021 00:42:59 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 01:10:42 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Fri, 03 Sep 2021 01:10:43 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Fri, 03 Sep 2021 01:10:51 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 01:10:54 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Fri, 03 Sep 2021 01:10:54 GMT
ENV LC_ALL=en_US.UTF-8
# Fri, 03 Sep 2021 01:10:54 GMT
ENV LANG=en_US.UTF-8
# Fri, 03 Sep 2021 01:10:55 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Fri, 03 Sep 2021 01:10:55 GMT
ENV R_BASE_VERSION=4.1.1
# Fri, 03 Sep 2021 01:10:56 GMT
RUN echo "deb http://deb.debian.org/debian experimental main" > /etc/apt/sources.list.d/experimental.list     && echo "deb [trusted=yes] https://eddelbuettel.github.io/ppaR400 ./" > /etc/apt/sources.list.d/edd-r4.list
# Fri, 03 Sep 2021 01:11:41 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 01:11:43 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:cb1c1f26816daf4a362d7ca0dfd432a0efc976e7a23fda91e6d7940176af45d5`  
		Last Modified: Fri, 03 Sep 2021 00:53:52 GMT  
		Size: 54.5 MB (54510227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c69dfdee9e07adfba86c978fafba78a0738db857066ab384103a0410832152b6`  
		Last Modified: Fri, 03 Sep 2021 01:12:06 GMT  
		Size: 1.9 KB (1876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8907b089dd3c59e93a8693c3c61c4bb71122ad5ded0362d201d63f710648c824`  
		Last Modified: Fri, 03 Sep 2021 01:12:09 GMT  
		Size: 25.6 MB (25628679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be0473cb5f95596271207ba1b29cf10816c4d62bd726bcf7e12fa7c371ed2b5c`  
		Last Modified: Fri, 03 Sep 2021 01:12:04 GMT  
		Size: 864.6 KB (864588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d4f43e99cba990721b85bc5659d4679c3954d763a05006fac93c32e1c45d759`  
		Last Modified: Fri, 03 Sep 2021 01:12:03 GMT  
		Size: 348.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7595359e054f4bda42eb4cc050d0e1c0761a46d6f163026e7865de86bc41d3d0`  
		Last Modified: Fri, 03 Sep 2021 01:12:03 GMT  
		Size: 292.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab5d55ad1075740960a588a8ccf04c28e59d14d82a81ba1c80e5247e644a4f64`  
		Last Modified: Fri, 03 Sep 2021 01:12:33 GMT  
		Size: 231.4 MB (231406391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:4.1.1` - linux; ppc64le

```console
$ docker pull r-base@sha256:14d2b6895d6b83099e29f797e5494bbe97e85b28540b10641415ab8f05b54bd0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **321.4 MB (321446947 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f6aba6645bfbae47c742f0df7d1e50e36db75abee4d88f958d91d3717e3d1ce3`
-	Default Command: `["R"]`

```dockerfile
# Tue, 17 Aug 2021 01:37:41 GMT
ADD file:1f0015936f61869d4be0802e8692d936b87b60ce9198abdeae9e7df07172a08f in / 
# Tue, 17 Aug 2021 01:37:49 GMT
CMD ["bash"]
# Wed, 18 Aug 2021 01:48:40 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Wed, 18 Aug 2021 01:48:59 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Wed, 18 Aug 2021 01:50:36 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Wed, 18 Aug 2021 01:51:00 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Wed, 18 Aug 2021 01:51:02 GMT
ENV LC_ALL=en_US.UTF-8
# Wed, 18 Aug 2021 01:51:07 GMT
ENV LANG=en_US.UTF-8
# Wed, 18 Aug 2021 01:51:16 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Wed, 18 Aug 2021 01:51:19 GMT
ENV R_BASE_VERSION=4.1.1
# Wed, 18 Aug 2021 01:51:32 GMT
RUN echo "deb http://deb.debian.org/debian experimental main" > /etc/apt/sources.list.d/experimental.list     && echo "deb [trusted=yes] https://eddelbuettel.github.io/ppaR400 ./" > /etc/apt/sources.list.d/edd-r4.list
# Wed, 18 Aug 2021 02:03:11 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Wed, 18 Aug 2021 02:03:17 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:2582c71fc0095399869e98ebc0072852aa8431fc7ead1a6a512085dfc17ff54f`  
		Last Modified: Tue, 17 Aug 2021 01:56:42 GMT  
		Size: 58.8 MB (58810778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e4b2c2cabd753480feda3c1ddf5e442e779b5f1030d45b1e0fef4fce678c22b`  
		Last Modified: Wed, 18 Aug 2021 02:03:46 GMT  
		Size: 1.9 KB (1895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:169df8e567c87ef41fed701a38ec07f836e37a541f40a90d84ebce47ee196a49`  
		Last Modified: Wed, 18 Aug 2021 02:03:47 GMT  
		Size: 25.9 MB (25853275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8aa3f7207216312e90497b55c9d5bf5fe8e6c20b9f718cbc539444e3d4bb038a`  
		Last Modified: Wed, 18 Aug 2021 02:03:43 GMT  
		Size: 864.6 KB (864594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc629e354395864ccf8eab0899d07f1ab5e63edb8deb82b8ada7cedcbc749f68`  
		Last Modified: Wed, 18 Aug 2021 02:03:43 GMT  
		Size: 351.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f70f5b0726ad74c663b3e033208aa66a3ac352aa268b7dfca37522d7f314543`  
		Last Modified: Wed, 18 Aug 2021 02:03:43 GMT  
		Size: 292.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1daa3ba3f262b327644bd9237e37e79ad5701a0fcdbae95e12a868ddfdc157f`  
		Last Modified: Wed, 18 Aug 2021 02:04:19 GMT  
		Size: 235.9 MB (235915762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:4.1.1` - linux; s390x

```console
$ docker pull r-base@sha256:52ccb45f6f96e9cedbb058b310dc0caacd7f9748afe480e39ecb4715b141143a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **290.6 MB (290559707 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a64d6071962e4b3e7c867f48dbb6819681f3fe1c5402a5974a427c9999f25cf`
-	Default Command: `["R"]`

```dockerfile
# Fri, 03 Sep 2021 00:47:47 GMT
ADD file:54f05be13650e2f59f5ca102e738802e756fa0f0264cf9f12db6ed40461387c8 in / 
# Fri, 03 Sep 2021 00:47:55 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 04:55:30 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Fri, 03 Sep 2021 04:55:31 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Fri, 03 Sep 2021 04:55:42 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 04:55:44 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Fri, 03 Sep 2021 04:55:44 GMT
ENV LC_ALL=en_US.UTF-8
# Fri, 03 Sep 2021 04:55:45 GMT
ENV LANG=en_US.UTF-8
# Fri, 03 Sep 2021 04:55:45 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Fri, 03 Sep 2021 04:55:46 GMT
ENV R_BASE_VERSION=4.1.1
# Fri, 03 Sep 2021 04:55:46 GMT
RUN echo "deb http://deb.debian.org/debian experimental main" > /etc/apt/sources.list.d/experimental.list     && echo "deb [trusted=yes] https://eddelbuettel.github.io/ppaR400 ./" > /etc/apt/sources.list.d/edd-r4.list
# Fri, 03 Sep 2021 04:56:48 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 04:56:58 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:09142d8bf3fde8b878e8f7bddf00b824e1f1b97647c8d5dbc3df6e87335828e7`  
		Last Modified: Fri, 03 Sep 2021 00:55:37 GMT  
		Size: 53.7 MB (53749639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4648cdd0007a319c9ba52dfc82fe89f92272e2bb31958751f2553e6cffa8c2f`  
		Last Modified: Fri, 03 Sep 2021 04:57:16 GMT  
		Size: 1.9 KB (1877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cbf8f83134375ad028e51a28afe00788a01e7fd96bda84acbcc035ba40ca613`  
		Last Modified: Fri, 03 Sep 2021 04:57:16 GMT  
		Size: 25.6 MB (25632465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:155060aa124f1134652641018462f345fd6f748b0c95993e4d34459394738769`  
		Last Modified: Fri, 03 Sep 2021 04:57:14 GMT  
		Size: 920.2 KB (920153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85edeed1a86b9b07232533e58a0cef13de02f2d2be69f48ddeed25f117ee0af9`  
		Last Modified: Fri, 03 Sep 2021 04:57:14 GMT  
		Size: 348.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:234ec4773a81fd65cbed18bc538a2a54bb2a651c184c292c08cbc1c48d813666`  
		Last Modified: Fri, 03 Sep 2021 04:57:14 GMT  
		Size: 292.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:731e213d1154e560dfc6583e424fc46f8fa42729f4ef0001759990ccb429cca3`  
		Last Modified: Fri, 03 Sep 2021 04:57:35 GMT  
		Size: 210.3 MB (210254933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `r-base:latest`

```console
$ docker pull r-base@sha256:06ec747f404da004ee6508845d11cfa9807f150623868ede0c1201bd63bf59f9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `r-base:latest` - linux; amd64

```console
$ docker pull r-base@sha256:e3db99ecd00477e755f44ebdf20eb89c0b25c7a80b0c5085d818fa60217891d4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **323.6 MB (323573190 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c27c3714f0049e58f90167840d1df16be91dc4240b2ee4e0278b869d2bd3d7ad`
-	Default Command: `["R"]`

```dockerfile
# Tue, 17 Aug 2021 01:26:21 GMT
ADD file:78a808c11f084f171360ce87535de573285eb3f06602698c86bc2007a307299e in / 
# Tue, 17 Aug 2021 01:26:21 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 14:25:49 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Tue, 17 Aug 2021 14:25:51 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Tue, 17 Aug 2021 14:26:02 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 14:26:05 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Tue, 17 Aug 2021 14:26:06 GMT
ENV LC_ALL=en_US.UTF-8
# Tue, 17 Aug 2021 14:26:06 GMT
ENV LANG=en_US.UTF-8
# Tue, 17 Aug 2021 14:26:07 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Tue, 17 Aug 2021 14:26:07 GMT
ENV R_BASE_VERSION=4.1.1
# Tue, 17 Aug 2021 14:26:08 GMT
RUN echo "deb http://deb.debian.org/debian experimental main" > /etc/apt/sources.list.d/experimental.list     && echo "deb [trusted=yes] https://eddelbuettel.github.io/ppaR400 ./" > /etc/apt/sources.list.d/edd-r4.list
# Tue, 17 Aug 2021 14:26:57 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 14:26:59 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:a42321116e438acfff1628527f7ae9e433d1ece73a19aecf4b4642d110d317fd`  
		Last Modified: Tue, 17 Aug 2021 01:33:48 GMT  
		Size: 54.9 MB (54909547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f412a7fda1e6aa9b5a01156374a3c4dcdc0e94a6596855d76138099924e0393`  
		Last Modified: Tue, 17 Aug 2021 14:27:23 GMT  
		Size: 1.9 KB (1874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fab087860f757d5a41f3d47c44c636e9035e23f37eeefd64c68d787923157043`  
		Last Modified: Tue, 17 Aug 2021 14:27:24 GMT  
		Size: 25.6 MB (25629954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25d5624c76ed18f8cd357135ed0f589838912b7c77dfff99d35eb5a93a6d4afc`  
		Last Modified: Tue, 17 Aug 2021 14:27:20 GMT  
		Size: 864.6 KB (864591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb56c0554b1798004d8fd95e6c888bb9ed6e35b9bb4ddb0b5d5020e2c90b0b7f`  
		Last Modified: Tue, 17 Aug 2021 14:27:21 GMT  
		Size: 349.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:409cf8ce22d9c250de0d27c42585f48d5154ec07fde7bc1b6b4550696e0d1dc2`  
		Last Modified: Tue, 17 Aug 2021 14:27:20 GMT  
		Size: 292.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08aa39b001b7c5244ae2171c9b8d2fcdda23c385d043fae650ff1d6c10f30578`  
		Last Modified: Tue, 17 Aug 2021 14:27:56 GMT  
		Size: 242.2 MB (242166583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:latest` - linux; arm64 variant v8

```console
$ docker pull r-base@sha256:15bcdf78a283096928a79a276f3bf4b7bf8390e564df6527b79cc6634a414248
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **312.4 MB (312412401 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2b01c676c4159ccf0e5bd8fa641aec2d26e2256ab57bfcdf9344322c208896b`
-	Default Command: `["R"]`

```dockerfile
# Fri, 03 Sep 2021 00:42:59 GMT
ADD file:024a3f01f7d5ed6ce6f4ee6507a0dbb6edefe3267e1672fb07b5e5eae29a47b7 in / 
# Fri, 03 Sep 2021 00:42:59 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 01:10:42 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Fri, 03 Sep 2021 01:10:43 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Fri, 03 Sep 2021 01:10:51 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 01:10:54 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Fri, 03 Sep 2021 01:10:54 GMT
ENV LC_ALL=en_US.UTF-8
# Fri, 03 Sep 2021 01:10:54 GMT
ENV LANG=en_US.UTF-8
# Fri, 03 Sep 2021 01:10:55 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Fri, 03 Sep 2021 01:10:55 GMT
ENV R_BASE_VERSION=4.1.1
# Fri, 03 Sep 2021 01:10:56 GMT
RUN echo "deb http://deb.debian.org/debian experimental main" > /etc/apt/sources.list.d/experimental.list     && echo "deb [trusted=yes] https://eddelbuettel.github.io/ppaR400 ./" > /etc/apt/sources.list.d/edd-r4.list
# Fri, 03 Sep 2021 01:11:41 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 01:11:43 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:cb1c1f26816daf4a362d7ca0dfd432a0efc976e7a23fda91e6d7940176af45d5`  
		Last Modified: Fri, 03 Sep 2021 00:53:52 GMT  
		Size: 54.5 MB (54510227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c69dfdee9e07adfba86c978fafba78a0738db857066ab384103a0410832152b6`  
		Last Modified: Fri, 03 Sep 2021 01:12:06 GMT  
		Size: 1.9 KB (1876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8907b089dd3c59e93a8693c3c61c4bb71122ad5ded0362d201d63f710648c824`  
		Last Modified: Fri, 03 Sep 2021 01:12:09 GMT  
		Size: 25.6 MB (25628679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be0473cb5f95596271207ba1b29cf10816c4d62bd726bcf7e12fa7c371ed2b5c`  
		Last Modified: Fri, 03 Sep 2021 01:12:04 GMT  
		Size: 864.6 KB (864588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d4f43e99cba990721b85bc5659d4679c3954d763a05006fac93c32e1c45d759`  
		Last Modified: Fri, 03 Sep 2021 01:12:03 GMT  
		Size: 348.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7595359e054f4bda42eb4cc050d0e1c0761a46d6f163026e7865de86bc41d3d0`  
		Last Modified: Fri, 03 Sep 2021 01:12:03 GMT  
		Size: 292.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab5d55ad1075740960a588a8ccf04c28e59d14d82a81ba1c80e5247e644a4f64`  
		Last Modified: Fri, 03 Sep 2021 01:12:33 GMT  
		Size: 231.4 MB (231406391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:latest` - linux; ppc64le

```console
$ docker pull r-base@sha256:14d2b6895d6b83099e29f797e5494bbe97e85b28540b10641415ab8f05b54bd0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **321.4 MB (321446947 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f6aba6645bfbae47c742f0df7d1e50e36db75abee4d88f958d91d3717e3d1ce3`
-	Default Command: `["R"]`

```dockerfile
# Tue, 17 Aug 2021 01:37:41 GMT
ADD file:1f0015936f61869d4be0802e8692d936b87b60ce9198abdeae9e7df07172a08f in / 
# Tue, 17 Aug 2021 01:37:49 GMT
CMD ["bash"]
# Wed, 18 Aug 2021 01:48:40 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Wed, 18 Aug 2021 01:48:59 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Wed, 18 Aug 2021 01:50:36 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Wed, 18 Aug 2021 01:51:00 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Wed, 18 Aug 2021 01:51:02 GMT
ENV LC_ALL=en_US.UTF-8
# Wed, 18 Aug 2021 01:51:07 GMT
ENV LANG=en_US.UTF-8
# Wed, 18 Aug 2021 01:51:16 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Wed, 18 Aug 2021 01:51:19 GMT
ENV R_BASE_VERSION=4.1.1
# Wed, 18 Aug 2021 01:51:32 GMT
RUN echo "deb http://deb.debian.org/debian experimental main" > /etc/apt/sources.list.d/experimental.list     && echo "deb [trusted=yes] https://eddelbuettel.github.io/ppaR400 ./" > /etc/apt/sources.list.d/edd-r4.list
# Wed, 18 Aug 2021 02:03:11 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Wed, 18 Aug 2021 02:03:17 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:2582c71fc0095399869e98ebc0072852aa8431fc7ead1a6a512085dfc17ff54f`  
		Last Modified: Tue, 17 Aug 2021 01:56:42 GMT  
		Size: 58.8 MB (58810778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e4b2c2cabd753480feda3c1ddf5e442e779b5f1030d45b1e0fef4fce678c22b`  
		Last Modified: Wed, 18 Aug 2021 02:03:46 GMT  
		Size: 1.9 KB (1895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:169df8e567c87ef41fed701a38ec07f836e37a541f40a90d84ebce47ee196a49`  
		Last Modified: Wed, 18 Aug 2021 02:03:47 GMT  
		Size: 25.9 MB (25853275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8aa3f7207216312e90497b55c9d5bf5fe8e6c20b9f718cbc539444e3d4bb038a`  
		Last Modified: Wed, 18 Aug 2021 02:03:43 GMT  
		Size: 864.6 KB (864594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc629e354395864ccf8eab0899d07f1ab5e63edb8deb82b8ada7cedcbc749f68`  
		Last Modified: Wed, 18 Aug 2021 02:03:43 GMT  
		Size: 351.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f70f5b0726ad74c663b3e033208aa66a3ac352aa268b7dfca37522d7f314543`  
		Last Modified: Wed, 18 Aug 2021 02:03:43 GMT  
		Size: 292.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1daa3ba3f262b327644bd9237e37e79ad5701a0fcdbae95e12a868ddfdc157f`  
		Last Modified: Wed, 18 Aug 2021 02:04:19 GMT  
		Size: 235.9 MB (235915762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:latest` - linux; s390x

```console
$ docker pull r-base@sha256:52ccb45f6f96e9cedbb058b310dc0caacd7f9748afe480e39ecb4715b141143a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **290.6 MB (290559707 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a64d6071962e4b3e7c867f48dbb6819681f3fe1c5402a5974a427c9999f25cf`
-	Default Command: `["R"]`

```dockerfile
# Fri, 03 Sep 2021 00:47:47 GMT
ADD file:54f05be13650e2f59f5ca102e738802e756fa0f0264cf9f12db6ed40461387c8 in / 
# Fri, 03 Sep 2021 00:47:55 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 04:55:30 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Fri, 03 Sep 2021 04:55:31 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Fri, 03 Sep 2021 04:55:42 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 04:55:44 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Fri, 03 Sep 2021 04:55:44 GMT
ENV LC_ALL=en_US.UTF-8
# Fri, 03 Sep 2021 04:55:45 GMT
ENV LANG=en_US.UTF-8
# Fri, 03 Sep 2021 04:55:45 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Fri, 03 Sep 2021 04:55:46 GMT
ENV R_BASE_VERSION=4.1.1
# Fri, 03 Sep 2021 04:55:46 GMT
RUN echo "deb http://deb.debian.org/debian experimental main" > /etc/apt/sources.list.d/experimental.list     && echo "deb [trusted=yes] https://eddelbuettel.github.io/ppaR400 ./" > /etc/apt/sources.list.d/edd-r4.list
# Fri, 03 Sep 2021 04:56:48 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 04:56:58 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:09142d8bf3fde8b878e8f7bddf00b824e1f1b97647c8d5dbc3df6e87335828e7`  
		Last Modified: Fri, 03 Sep 2021 00:55:37 GMT  
		Size: 53.7 MB (53749639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4648cdd0007a319c9ba52dfc82fe89f92272e2bb31958751f2553e6cffa8c2f`  
		Last Modified: Fri, 03 Sep 2021 04:57:16 GMT  
		Size: 1.9 KB (1877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cbf8f83134375ad028e51a28afe00788a01e7fd96bda84acbcc035ba40ca613`  
		Last Modified: Fri, 03 Sep 2021 04:57:16 GMT  
		Size: 25.6 MB (25632465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:155060aa124f1134652641018462f345fd6f748b0c95993e4d34459394738769`  
		Last Modified: Fri, 03 Sep 2021 04:57:14 GMT  
		Size: 920.2 KB (920153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85edeed1a86b9b07232533e58a0cef13de02f2d2be69f48ddeed25f117ee0af9`  
		Last Modified: Fri, 03 Sep 2021 04:57:14 GMT  
		Size: 348.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:234ec4773a81fd65cbed18bc538a2a54bb2a651c184c292c08cbc1c48d813666`  
		Last Modified: Fri, 03 Sep 2021 04:57:14 GMT  
		Size: 292.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:731e213d1154e560dfc6583e424fc46f8fa42729f4ef0001759990ccb429cca3`  
		Last Modified: Fri, 03 Sep 2021 04:57:35 GMT  
		Size: 210.3 MB (210254933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
