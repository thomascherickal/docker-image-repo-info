<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `r-base`

-	[`r-base:4.2.3`](#r-base423)
-	[`r-base:latest`](#r-baselatest)

## `r-base:4.2.3`

```console
$ docker pull r-base@sha256:7112f97ff67880d4c5517c5429a61b5cac1ba5aad6d8ec337d56e5733a3ed6ea
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `r-base:4.2.3` - linux; amd64

```console
$ docker pull r-base@sha256:c79844fdc8bfcd92d4557fadcae3712259baabcc70433b98a5befcdb057003da
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **338.2 MB (338196915 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9af9051ce66400b983d100f7aba3c2fff73e59822728d32945f61f0a1a4bc747`
-	Default Command: `["R"]`

```dockerfile
# Wed, 01 Mar 2023 04:11:42 GMT
ADD file:74681cecd762b2ba7998f4db71254724112eeeb0a1801289e92e9be9986fab3e in / 
# Wed, 01 Mar 2023 04:11:43 GMT
CMD ["bash"]
# Wed, 15 Mar 2023 23:07:39 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Wed, 15 Mar 2023 23:07:40 GMT
RUN useradd -s /bin/bash -m docker 	&& usermod -a -G staff docker
# Wed, 15 Mar 2023 23:07:53 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Wed, 15 Mar 2023 23:07:55 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Wed, 15 Mar 2023 23:07:55 GMT
ENV LC_ALL=en_US.UTF-8
# Wed, 15 Mar 2023 23:07:55 GMT
ENV LANG=en_US.UTF-8
# Wed, 15 Mar 2023 23:07:56 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Wed, 15 Mar 2023 23:07:56 GMT
ENV R_BASE_VERSION=4.2.3
# Wed, 15 Mar 2023 23:07:56 GMT
RUN echo "deb http://deb.debian.org/debian experimental main" > /etc/apt/sources.list.d/experimental.list     && echo "deb [trusted=yes] https://eddelbuettel.github.io/ppaR400 ./" > /etc/apt/sources.list.d/edd-r4.list
# Wed, 15 Mar 2023 23:09:49 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-docopt                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& chown root:staff "/usr/local/lib/R/site-library" 	&& chmod g+ws "/usr/local/lib/R/site-library" 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Wed, 15 Mar 2023 23:09:51 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:bbf0dc8a79b520e97bfc1897d4020969033cda033c141208013b60015a6334e5`  
		Last Modified: Wed, 01 Mar 2023 04:16:58 GMT  
		Size: 49.2 MB (49237268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1bc0f45ebb23c8eb4010742705a54946ee078f9a2cb4c820cc59fbf11591ceb`  
		Last Modified: Wed, 15 Mar 2023 23:10:10 GMT  
		Size: 3.4 KB (3365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a774c8a7797545685aeaffbd3942dbb68558ff4bc8b2fa188fc76d9fd2d3d62`  
		Last Modified: Wed, 15 Mar 2023 23:10:15 GMT  
		Size: 25.1 MB (25111955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9041e14cd651d64159da5dc34102d1fbbbb1ffb18cb50f9060c1755241593ab`  
		Last Modified: Wed, 15 Mar 2023 23:10:08 GMT  
		Size: 865.9 KB (865852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0b90e55cf6c065a8f00ec8bb5ed42f7d2be8eaa0593d9cbb66fc4004ac5809a`  
		Last Modified: Wed, 15 Mar 2023 23:10:08 GMT  
		Size: 353.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8146bb0258390a77b9bcf31ed59d9de0ab0221b66dd2029ef3e1d6274e8836a`  
		Last Modified: Wed, 15 Mar 2023 23:10:08 GMT  
		Size: 293.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dbaea0691e6fb2570baf94bd3f77c5ddf9e47bacf2551b42daa9de35a1a5951`  
		Last Modified: Wed, 15 Mar 2023 23:10:39 GMT  
		Size: 263.0 MB (262977829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:4.2.3` - linux; arm64 variant v8

```console
$ docker pull r-base@sha256:cc3c6419bf93afa2e58087f2c0853cf5f4fcd4f2619e9248eb47203a9250177f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **324.2 MB (324172722 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bba11a4adc577688f5e9b57bd788f57749cc1fd5cc7c2e8bf157ca40a814f11b`
-	Default Command: `["R"]`

```dockerfile
# Wed, 01 Mar 2023 02:21:51 GMT
ADD file:c47730325f9bfe6686c928d0c7c46f6bd75a614ac9bb8bdffdcfef69b5cab2ff in / 
# Wed, 01 Mar 2023 02:21:51 GMT
CMD ["bash"]
# Wed, 15 Mar 2023 22:59:59 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Wed, 15 Mar 2023 22:59:59 GMT
RUN useradd -s /bin/bash -m docker 	&& usermod -a -G staff docker
# Wed, 15 Mar 2023 23:00:09 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Wed, 15 Mar 2023 23:00:11 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Wed, 15 Mar 2023 23:00:11 GMT
ENV LC_ALL=en_US.UTF-8
# Wed, 15 Mar 2023 23:00:11 GMT
ENV LANG=en_US.UTF-8
# Wed, 15 Mar 2023 23:00:12 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Wed, 15 Mar 2023 23:00:12 GMT
ENV R_BASE_VERSION=4.2.3
# Wed, 15 Mar 2023 23:00:12 GMT
RUN echo "deb http://deb.debian.org/debian experimental main" > /etc/apt/sources.list.d/experimental.list     && echo "deb [trusted=yes] https://eddelbuettel.github.io/ppaR400 ./" > /etc/apt/sources.list.d/edd-r4.list
# Wed, 15 Mar 2023 23:02:09 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-docopt                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& chown root:staff "/usr/local/lib/R/site-library" 	&& chmod g+ws "/usr/local/lib/R/site-library" 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Wed, 15 Mar 2023 23:02:14 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:bd5a6f14a1228f25359ec5248195de6f015069b0c74dc6be8e415fc08ed74f38`  
		Last Modified: Wed, 01 Mar 2023 02:26:44 GMT  
		Size: 49.3 MB (49273951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6d23d5508f4eb170ba8857ecdf71feb2941087ed8ba1d1ae43098dd4f85fd01`  
		Last Modified: Wed, 15 Mar 2023 23:02:29 GMT  
		Size: 3.4 KB (3366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96d1512b8721edbd32b77d4845e3582b6da3526c111aef8ebec00050f1292a3c`  
		Last Modified: Wed, 15 Mar 2023 23:02:30 GMT  
		Size: 24.9 MB (24939732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58db9db467209a79c8e159d029d9318a69925dab9e61534c201f8af53d432eaa`  
		Last Modified: Wed, 15 Mar 2023 23:02:28 GMT  
		Size: 865.9 KB (865855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:848cd30e54fd551349b2801118c70247cdb35a771eddec0e7c0261668bbd0ecd`  
		Last Modified: Wed, 15 Mar 2023 23:02:27 GMT  
		Size: 352.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd3ede8ea4be7582195f60745562142ae2ce22af57fdf5c26b3a5f4df8316b73`  
		Last Modified: Wed, 15 Mar 2023 23:02:28 GMT  
		Size: 294.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b68ea117aeb9db550d6512b550771acfcbda75ca4d9e2b72e6d684383ea663b`  
		Last Modified: Wed, 15 Mar 2023 23:02:48 GMT  
		Size: 249.1 MB (249089172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:4.2.3` - linux; ppc64le

```console
$ docker pull r-base@sha256:5bbba68a87fde58385c91321cc39b88138378f3d55e4d350c04366470464355c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **340.9 MB (340890392 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82694c6cb1cf9d8dda0357e098bc13ef5a648b0f6aaf51792f8f56b78932598f`
-	Default Command: `["R"]`

```dockerfile
# Wed, 01 Mar 2023 04:49:21 GMT
ADD file:802564bd8f691b73ccc068cc3c339c6a4c178bcf8383008e4f87a3774cb308b9 in / 
# Wed, 01 Mar 2023 04:49:24 GMT
CMD ["bash"]
# Wed, 15 Mar 2023 22:34:41 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Wed, 15 Mar 2023 22:34:43 GMT
RUN useradd -s /bin/bash -m docker 	&& usermod -a -G staff docker
# Wed, 15 Mar 2023 22:35:12 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Wed, 15 Mar 2023 22:35:17 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Wed, 15 Mar 2023 22:35:18 GMT
ENV LC_ALL=en_US.UTF-8
# Wed, 15 Mar 2023 22:35:19 GMT
ENV LANG=en_US.UTF-8
# Wed, 15 Mar 2023 22:35:21 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Wed, 15 Mar 2023 22:35:22 GMT
ENV R_BASE_VERSION=4.2.3
# Wed, 15 Mar 2023 22:35:23 GMT
RUN echo "deb http://deb.debian.org/debian experimental main" > /etc/apt/sources.list.d/experimental.list     && echo "deb [trusted=yes] https://eddelbuettel.github.io/ppaR400 ./" > /etc/apt/sources.list.d/edd-r4.list
# Wed, 15 Mar 2023 22:39:13 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-docopt                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& chown root:staff "/usr/local/lib/R/site-library" 	&& chmod g+ws "/usr/local/lib/R/site-library" 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Wed, 15 Mar 2023 22:39:16 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:adcb4bfc20e2eddc047aac97edc102514767c0f2b64f4f281f2e71651d1a97a9`  
		Last Modified: Wed, 01 Mar 2023 04:56:03 GMT  
		Size: 53.3 MB (53250177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fedfba3727b0e2481a72b4c5aaa6a213881ba512ff6a1d028af1e8b3f81dfc30`  
		Last Modified: Wed, 15 Mar 2023 22:39:30 GMT  
		Size: 3.4 KB (3368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cb5fcec2a4c12bb7a3877120fbcbd43e02d93c579b4ec23a7c0e3c24d034fc1`  
		Last Modified: Wed, 15 Mar 2023 22:39:33 GMT  
		Size: 25.5 MB (25513339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96945dc0c5c32df80886b134ea7800be68cdb966b65a2bc3082c7ab0e155c3f8`  
		Last Modified: Wed, 15 Mar 2023 22:39:29 GMT  
		Size: 865.9 KB (865853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4ade3cdc38a2299b70a9d6872515835e21db995a3e780b27e520208c7fc83d0`  
		Last Modified: Wed, 15 Mar 2023 22:39:28 GMT  
		Size: 352.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:530812c100b22df2c2bbe4d721158af28a0dc4bc9713f90be312024ed5adf3ae`  
		Last Modified: Wed, 15 Mar 2023 22:39:28 GMT  
		Size: 294.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb1f24e1acd62e26949c7606c065ef3e61fb4117829f8b9cccbeedef4fad83c7`  
		Last Modified: Wed, 15 Mar 2023 22:40:21 GMT  
		Size: 261.3 MB (261257009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:4.2.3` - linux; s390x

```console
$ docker pull r-base@sha256:9d08660a5c6806a0cb9bc535943885edaf403a99b4d55d030a0aa9500225ff55
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **299.2 MB (299203382 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22a0f59e2816acb42904f7f52c8dfb37994f6f12ed2274b3d9ac3e970b2acff8`
-	Default Command: `["R"]`

```dockerfile
# Wed, 01 Mar 2023 02:51:38 GMT
ADD file:8439a18edae9de92ebeb6ca0b69fbd74a02cc73bd2ca22601f8258fa87e9d69a in / 
# Wed, 01 Mar 2023 02:51:41 GMT
CMD ["bash"]
# Wed, 15 Mar 2023 22:42:36 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Wed, 15 Mar 2023 22:42:36 GMT
RUN useradd -s /bin/bash -m docker 	&& usermod -a -G staff docker
# Wed, 15 Mar 2023 22:42:45 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Wed, 15 Mar 2023 22:42:48 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Wed, 15 Mar 2023 22:42:48 GMT
ENV LC_ALL=en_US.UTF-8
# Wed, 15 Mar 2023 22:42:48 GMT
ENV LANG=en_US.UTF-8
# Wed, 15 Mar 2023 22:42:48 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Wed, 15 Mar 2023 22:42:49 GMT
ENV R_BASE_VERSION=4.2.3
# Wed, 15 Mar 2023 22:42:49 GMT
RUN echo "deb http://deb.debian.org/debian experimental main" > /etc/apt/sources.list.d/experimental.list     && echo "deb [trusted=yes] https://eddelbuettel.github.io/ppaR400 ./" > /etc/apt/sources.list.d/edd-r4.list
# Wed, 15 Mar 2023 22:44:25 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-docopt                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& chown root:staff "/usr/local/lib/R/site-library" 	&& chmod g+ws "/usr/local/lib/R/site-library" 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Wed, 15 Mar 2023 22:44:35 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:5cd18bb803f30053fbd73f7ae3e9f9955611d476d1cc5d8cd575f473f69eb5d3`  
		Last Modified: Wed, 01 Mar 2023 02:55:53 GMT  
		Size: 47.6 MB (47608038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:680efcad21632d35c872b57948a44685d8a9d7b983ba6917992706a4bf6a84c5`  
		Last Modified: Wed, 15 Mar 2023 22:45:02 GMT  
		Size: 3.4 KB (3365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50a0dfcc27ba3c93f7520a00297b82dad2bc844fd563f40091ee7eef8406fab0`  
		Last Modified: Wed, 15 Mar 2023 22:45:04 GMT  
		Size: 24.8 MB (24789740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:124ebae5b83e501536f499bc8a1d26293206d62e587472d9d07e12027e7289c3`  
		Last Modified: Wed, 15 Mar 2023 22:45:01 GMT  
		Size: 921.0 KB (921016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dea54bc49cb7b3d17a0237fba4a7cca1f3b4d7f80f179e70c913823d34c7343`  
		Last Modified: Wed, 15 Mar 2023 22:45:01 GMT  
		Size: 349.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c140b31dbc74c454d0f44cc8be5957d4289965a92082d37cf51473ce2b0dc147`  
		Last Modified: Wed, 15 Mar 2023 22:45:01 GMT  
		Size: 294.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c8dc6c0b2348146af4e68d7dde3dd8d4972afde117c8a29823218b6fadbe612`  
		Last Modified: Wed, 15 Mar 2023 22:45:25 GMT  
		Size: 225.9 MB (225880580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `r-base:latest`

```console
$ docker pull r-base@sha256:7112f97ff67880d4c5517c5429a61b5cac1ba5aad6d8ec337d56e5733a3ed6ea
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `r-base:latest` - linux; amd64

```console
$ docker pull r-base@sha256:c79844fdc8bfcd92d4557fadcae3712259baabcc70433b98a5befcdb057003da
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **338.2 MB (338196915 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9af9051ce66400b983d100f7aba3c2fff73e59822728d32945f61f0a1a4bc747`
-	Default Command: `["R"]`

```dockerfile
# Wed, 01 Mar 2023 04:11:42 GMT
ADD file:74681cecd762b2ba7998f4db71254724112eeeb0a1801289e92e9be9986fab3e in / 
# Wed, 01 Mar 2023 04:11:43 GMT
CMD ["bash"]
# Wed, 15 Mar 2023 23:07:39 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Wed, 15 Mar 2023 23:07:40 GMT
RUN useradd -s /bin/bash -m docker 	&& usermod -a -G staff docker
# Wed, 15 Mar 2023 23:07:53 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Wed, 15 Mar 2023 23:07:55 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Wed, 15 Mar 2023 23:07:55 GMT
ENV LC_ALL=en_US.UTF-8
# Wed, 15 Mar 2023 23:07:55 GMT
ENV LANG=en_US.UTF-8
# Wed, 15 Mar 2023 23:07:56 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Wed, 15 Mar 2023 23:07:56 GMT
ENV R_BASE_VERSION=4.2.3
# Wed, 15 Mar 2023 23:07:56 GMT
RUN echo "deb http://deb.debian.org/debian experimental main" > /etc/apt/sources.list.d/experimental.list     && echo "deb [trusted=yes] https://eddelbuettel.github.io/ppaR400 ./" > /etc/apt/sources.list.d/edd-r4.list
# Wed, 15 Mar 2023 23:09:49 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-docopt                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& chown root:staff "/usr/local/lib/R/site-library" 	&& chmod g+ws "/usr/local/lib/R/site-library" 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Wed, 15 Mar 2023 23:09:51 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:bbf0dc8a79b520e97bfc1897d4020969033cda033c141208013b60015a6334e5`  
		Last Modified: Wed, 01 Mar 2023 04:16:58 GMT  
		Size: 49.2 MB (49237268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1bc0f45ebb23c8eb4010742705a54946ee078f9a2cb4c820cc59fbf11591ceb`  
		Last Modified: Wed, 15 Mar 2023 23:10:10 GMT  
		Size: 3.4 KB (3365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a774c8a7797545685aeaffbd3942dbb68558ff4bc8b2fa188fc76d9fd2d3d62`  
		Last Modified: Wed, 15 Mar 2023 23:10:15 GMT  
		Size: 25.1 MB (25111955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9041e14cd651d64159da5dc34102d1fbbbb1ffb18cb50f9060c1755241593ab`  
		Last Modified: Wed, 15 Mar 2023 23:10:08 GMT  
		Size: 865.9 KB (865852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0b90e55cf6c065a8f00ec8bb5ed42f7d2be8eaa0593d9cbb66fc4004ac5809a`  
		Last Modified: Wed, 15 Mar 2023 23:10:08 GMT  
		Size: 353.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8146bb0258390a77b9bcf31ed59d9de0ab0221b66dd2029ef3e1d6274e8836a`  
		Last Modified: Wed, 15 Mar 2023 23:10:08 GMT  
		Size: 293.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dbaea0691e6fb2570baf94bd3f77c5ddf9e47bacf2551b42daa9de35a1a5951`  
		Last Modified: Wed, 15 Mar 2023 23:10:39 GMT  
		Size: 263.0 MB (262977829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:latest` - linux; arm64 variant v8

```console
$ docker pull r-base@sha256:cc3c6419bf93afa2e58087f2c0853cf5f4fcd4f2619e9248eb47203a9250177f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **324.2 MB (324172722 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bba11a4adc577688f5e9b57bd788f57749cc1fd5cc7c2e8bf157ca40a814f11b`
-	Default Command: `["R"]`

```dockerfile
# Wed, 01 Mar 2023 02:21:51 GMT
ADD file:c47730325f9bfe6686c928d0c7c46f6bd75a614ac9bb8bdffdcfef69b5cab2ff in / 
# Wed, 01 Mar 2023 02:21:51 GMT
CMD ["bash"]
# Wed, 15 Mar 2023 22:59:59 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Wed, 15 Mar 2023 22:59:59 GMT
RUN useradd -s /bin/bash -m docker 	&& usermod -a -G staff docker
# Wed, 15 Mar 2023 23:00:09 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Wed, 15 Mar 2023 23:00:11 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Wed, 15 Mar 2023 23:00:11 GMT
ENV LC_ALL=en_US.UTF-8
# Wed, 15 Mar 2023 23:00:11 GMT
ENV LANG=en_US.UTF-8
# Wed, 15 Mar 2023 23:00:12 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Wed, 15 Mar 2023 23:00:12 GMT
ENV R_BASE_VERSION=4.2.3
# Wed, 15 Mar 2023 23:00:12 GMT
RUN echo "deb http://deb.debian.org/debian experimental main" > /etc/apt/sources.list.d/experimental.list     && echo "deb [trusted=yes] https://eddelbuettel.github.io/ppaR400 ./" > /etc/apt/sources.list.d/edd-r4.list
# Wed, 15 Mar 2023 23:02:09 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-docopt                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& chown root:staff "/usr/local/lib/R/site-library" 	&& chmod g+ws "/usr/local/lib/R/site-library" 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Wed, 15 Mar 2023 23:02:14 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:bd5a6f14a1228f25359ec5248195de6f015069b0c74dc6be8e415fc08ed74f38`  
		Last Modified: Wed, 01 Mar 2023 02:26:44 GMT  
		Size: 49.3 MB (49273951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6d23d5508f4eb170ba8857ecdf71feb2941087ed8ba1d1ae43098dd4f85fd01`  
		Last Modified: Wed, 15 Mar 2023 23:02:29 GMT  
		Size: 3.4 KB (3366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96d1512b8721edbd32b77d4845e3582b6da3526c111aef8ebec00050f1292a3c`  
		Last Modified: Wed, 15 Mar 2023 23:02:30 GMT  
		Size: 24.9 MB (24939732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58db9db467209a79c8e159d029d9318a69925dab9e61534c201f8af53d432eaa`  
		Last Modified: Wed, 15 Mar 2023 23:02:28 GMT  
		Size: 865.9 KB (865855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:848cd30e54fd551349b2801118c70247cdb35a771eddec0e7c0261668bbd0ecd`  
		Last Modified: Wed, 15 Mar 2023 23:02:27 GMT  
		Size: 352.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd3ede8ea4be7582195f60745562142ae2ce22af57fdf5c26b3a5f4df8316b73`  
		Last Modified: Wed, 15 Mar 2023 23:02:28 GMT  
		Size: 294.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b68ea117aeb9db550d6512b550771acfcbda75ca4d9e2b72e6d684383ea663b`  
		Last Modified: Wed, 15 Mar 2023 23:02:48 GMT  
		Size: 249.1 MB (249089172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:latest` - linux; ppc64le

```console
$ docker pull r-base@sha256:5bbba68a87fde58385c91321cc39b88138378f3d55e4d350c04366470464355c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **340.9 MB (340890392 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82694c6cb1cf9d8dda0357e098bc13ef5a648b0f6aaf51792f8f56b78932598f`
-	Default Command: `["R"]`

```dockerfile
# Wed, 01 Mar 2023 04:49:21 GMT
ADD file:802564bd8f691b73ccc068cc3c339c6a4c178bcf8383008e4f87a3774cb308b9 in / 
# Wed, 01 Mar 2023 04:49:24 GMT
CMD ["bash"]
# Wed, 15 Mar 2023 22:34:41 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Wed, 15 Mar 2023 22:34:43 GMT
RUN useradd -s /bin/bash -m docker 	&& usermod -a -G staff docker
# Wed, 15 Mar 2023 22:35:12 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Wed, 15 Mar 2023 22:35:17 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Wed, 15 Mar 2023 22:35:18 GMT
ENV LC_ALL=en_US.UTF-8
# Wed, 15 Mar 2023 22:35:19 GMT
ENV LANG=en_US.UTF-8
# Wed, 15 Mar 2023 22:35:21 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Wed, 15 Mar 2023 22:35:22 GMT
ENV R_BASE_VERSION=4.2.3
# Wed, 15 Mar 2023 22:35:23 GMT
RUN echo "deb http://deb.debian.org/debian experimental main" > /etc/apt/sources.list.d/experimental.list     && echo "deb [trusted=yes] https://eddelbuettel.github.io/ppaR400 ./" > /etc/apt/sources.list.d/edd-r4.list
# Wed, 15 Mar 2023 22:39:13 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-docopt                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& chown root:staff "/usr/local/lib/R/site-library" 	&& chmod g+ws "/usr/local/lib/R/site-library" 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Wed, 15 Mar 2023 22:39:16 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:adcb4bfc20e2eddc047aac97edc102514767c0f2b64f4f281f2e71651d1a97a9`  
		Last Modified: Wed, 01 Mar 2023 04:56:03 GMT  
		Size: 53.3 MB (53250177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fedfba3727b0e2481a72b4c5aaa6a213881ba512ff6a1d028af1e8b3f81dfc30`  
		Last Modified: Wed, 15 Mar 2023 22:39:30 GMT  
		Size: 3.4 KB (3368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cb5fcec2a4c12bb7a3877120fbcbd43e02d93c579b4ec23a7c0e3c24d034fc1`  
		Last Modified: Wed, 15 Mar 2023 22:39:33 GMT  
		Size: 25.5 MB (25513339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96945dc0c5c32df80886b134ea7800be68cdb966b65a2bc3082c7ab0e155c3f8`  
		Last Modified: Wed, 15 Mar 2023 22:39:29 GMT  
		Size: 865.9 KB (865853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4ade3cdc38a2299b70a9d6872515835e21db995a3e780b27e520208c7fc83d0`  
		Last Modified: Wed, 15 Mar 2023 22:39:28 GMT  
		Size: 352.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:530812c100b22df2c2bbe4d721158af28a0dc4bc9713f90be312024ed5adf3ae`  
		Last Modified: Wed, 15 Mar 2023 22:39:28 GMT  
		Size: 294.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb1f24e1acd62e26949c7606c065ef3e61fb4117829f8b9cccbeedef4fad83c7`  
		Last Modified: Wed, 15 Mar 2023 22:40:21 GMT  
		Size: 261.3 MB (261257009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:latest` - linux; s390x

```console
$ docker pull r-base@sha256:9d08660a5c6806a0cb9bc535943885edaf403a99b4d55d030a0aa9500225ff55
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **299.2 MB (299203382 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22a0f59e2816acb42904f7f52c8dfb37994f6f12ed2274b3d9ac3e970b2acff8`
-	Default Command: `["R"]`

```dockerfile
# Wed, 01 Mar 2023 02:51:38 GMT
ADD file:8439a18edae9de92ebeb6ca0b69fbd74a02cc73bd2ca22601f8258fa87e9d69a in / 
# Wed, 01 Mar 2023 02:51:41 GMT
CMD ["bash"]
# Wed, 15 Mar 2023 22:42:36 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Wed, 15 Mar 2023 22:42:36 GMT
RUN useradd -s /bin/bash -m docker 	&& usermod -a -G staff docker
# Wed, 15 Mar 2023 22:42:45 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Wed, 15 Mar 2023 22:42:48 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Wed, 15 Mar 2023 22:42:48 GMT
ENV LC_ALL=en_US.UTF-8
# Wed, 15 Mar 2023 22:42:48 GMT
ENV LANG=en_US.UTF-8
# Wed, 15 Mar 2023 22:42:48 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Wed, 15 Mar 2023 22:42:49 GMT
ENV R_BASE_VERSION=4.2.3
# Wed, 15 Mar 2023 22:42:49 GMT
RUN echo "deb http://deb.debian.org/debian experimental main" > /etc/apt/sources.list.d/experimental.list     && echo "deb [trusted=yes] https://eddelbuettel.github.io/ppaR400 ./" > /etc/apt/sources.list.d/edd-r4.list
# Wed, 15 Mar 2023 22:44:25 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-docopt                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& chown root:staff "/usr/local/lib/R/site-library" 	&& chmod g+ws "/usr/local/lib/R/site-library" 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Wed, 15 Mar 2023 22:44:35 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:5cd18bb803f30053fbd73f7ae3e9f9955611d476d1cc5d8cd575f473f69eb5d3`  
		Last Modified: Wed, 01 Mar 2023 02:55:53 GMT  
		Size: 47.6 MB (47608038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:680efcad21632d35c872b57948a44685d8a9d7b983ba6917992706a4bf6a84c5`  
		Last Modified: Wed, 15 Mar 2023 22:45:02 GMT  
		Size: 3.4 KB (3365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50a0dfcc27ba3c93f7520a00297b82dad2bc844fd563f40091ee7eef8406fab0`  
		Last Modified: Wed, 15 Mar 2023 22:45:04 GMT  
		Size: 24.8 MB (24789740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:124ebae5b83e501536f499bc8a1d26293206d62e587472d9d07e12027e7289c3`  
		Last Modified: Wed, 15 Mar 2023 22:45:01 GMT  
		Size: 921.0 KB (921016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dea54bc49cb7b3d17a0237fba4a7cca1f3b4d7f80f179e70c913823d34c7343`  
		Last Modified: Wed, 15 Mar 2023 22:45:01 GMT  
		Size: 349.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c140b31dbc74c454d0f44cc8be5957d4289965a92082d37cf51473ce2b0dc147`  
		Last Modified: Wed, 15 Mar 2023 22:45:01 GMT  
		Size: 294.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c8dc6c0b2348146af4e68d7dde3dd8d4972afde117c8a29823218b6fadbe612`  
		Last Modified: Wed, 15 Mar 2023 22:45:25 GMT  
		Size: 225.9 MB (225880580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
