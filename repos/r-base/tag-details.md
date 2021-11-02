<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `r-base`

-	[`r-base:4.1.2`](#r-base412)
-	[`r-base:latest`](#r-baselatest)

## `r-base:4.1.2`

```console
$ docker pull r-base@sha256:9c5da04fae579ed7e8116a2c8f762bdadd290ae957ac6cce6f73d0b58dd298b0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
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
$ docker pull r-base@sha256:5c69200687c28a683189fd3cbb1911c292e82a80529873cc560118df197321e2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **314.4 MB (314382781 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09c6154f3d7c7c85f20fb58dca775998b14d881fea9127f63f1d637875d50b7e`
-	Default Command: `["R"]`

```dockerfile
# Tue, 12 Oct 2021 01:43:39 GMT
ADD file:0d2781f09dc7fd32dad3f41e34a91046910847a56bf128bb53a7cad6c06c1f26 in / 
# Tue, 12 Oct 2021 01:43:40 GMT
CMD ["bash"]
# Mon, 01 Nov 2021 22:18:58 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Mon, 01 Nov 2021 22:18:59 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Mon, 01 Nov 2021 22:19:10 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Mon, 01 Nov 2021 22:19:13 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Mon, 01 Nov 2021 22:19:13 GMT
ENV LC_ALL=en_US.UTF-8
# Mon, 01 Nov 2021 22:19:14 GMT
ENV LANG=en_US.UTF-8
# Mon, 01 Nov 2021 22:19:15 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Mon, 01 Nov 2021 22:19:16 GMT
ENV R_BASE_VERSION=4.1.2
# Mon, 01 Nov 2021 22:19:17 GMT
RUN echo "deb http://deb.debian.org/debian experimental main" > /etc/apt/sources.list.d/experimental.list     && echo "deb [trusted=yes] https://eddelbuettel.github.io/ppaR400 ./" > /etc/apt/sources.list.d/edd-r4.list
# Mon, 01 Nov 2021 22:20:17 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Mon, 01 Nov 2021 22:20:18 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:0a75495c66c5fc986e1fa178fa94fe24ac603e1ee8a61ff4b344624e0b8b030e`  
		Last Modified: Tue, 12 Oct 2021 01:52:57 GMT  
		Size: 54.5 MB (54465025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63c8d7fee44c549b526333f2fa675bcda3739b1b0a9913bccd27242c0d449036`  
		Last Modified: Mon, 01 Nov 2021 22:20:33 GMT  
		Size: 1.8 KB (1761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6043930ad0b89b70492c2933bb4b1ac26fc3c329a4f09b4efade34559d2a6064`  
		Last Modified: Mon, 01 Nov 2021 22:20:35 GMT  
		Size: 25.7 MB (25709011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:244ca69eb7bf6342f079b34a713ea95f9404a810ea387c9e6b3202f216f28035`  
		Last Modified: Mon, 01 Nov 2021 22:20:31 GMT  
		Size: 864.6 KB (864603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:664e83e6514dcb43e83f7fa0c20175c6f4f3383b793de2d6feea2ebbd5984934`  
		Last Modified: Mon, 01 Nov 2021 22:20:32 GMT  
		Size: 349.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45081130fa47f08935130d2a1f04061cad24e8221b2e98cee068e803ea2b43c2`  
		Last Modified: Mon, 01 Nov 2021 22:20:31 GMT  
		Size: 293.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b184dc1e127a2cebfd993a8091b0e730ef497df9d3e1e76972a2bae86741e0a`  
		Last Modified: Mon, 01 Nov 2021 22:20:59 GMT  
		Size: 233.3 MB (233341739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:4.1.2` - linux; s390x

```console
$ docker pull r-base@sha256:dcaeb2be1d58d90350dabf435f608122746feb78a4079280f00b32ef9cd0ec71
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **292.5 MB (292492241 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d9c7a61a54af603941d8c5a1f13eba03191cbcf27295f4c1adb87bd2ad9c8ff`
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
# Mon, 01 Nov 2021 22:20:32 GMT
ENV R_BASE_VERSION=4.1.2
# Mon, 01 Nov 2021 22:20:32 GMT
RUN echo "deb http://deb.debian.org/debian experimental main" > /etc/apt/sources.list.d/experimental.list     && echo "deb [trusted=yes] https://eddelbuettel.github.io/ppaR400 ./" > /etc/apt/sources.list.d/edd-r4.list
# Mon, 01 Nov 2021 22:21:27 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Mon, 01 Nov 2021 22:21:32 GMT
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
	-	`sha256:80fe35488d21277fb4073fd95f1da6874301b6726774e6f595046efb9fa28c9e`  
		Last Modified: Mon, 01 Nov 2021 22:21:48 GMT  
		Size: 290.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fc108576b3ef210b94d427a42f6710acbcbb68e04dba999035336c20ab4c470`  
		Last Modified: Mon, 01 Nov 2021 22:22:08 GMT  
		Size: 212.2 MB (212187366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `r-base:latest`

```console
$ docker pull r-base@sha256:cb12d91dbbb65b5cb657ee6666083e196496b2b8d381cee097bd744dd7d7414e
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
$ docker pull r-base@sha256:5c69200687c28a683189fd3cbb1911c292e82a80529873cc560118df197321e2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **314.4 MB (314382781 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09c6154f3d7c7c85f20fb58dca775998b14d881fea9127f63f1d637875d50b7e`
-	Default Command: `["R"]`

```dockerfile
# Tue, 12 Oct 2021 01:43:39 GMT
ADD file:0d2781f09dc7fd32dad3f41e34a91046910847a56bf128bb53a7cad6c06c1f26 in / 
# Tue, 12 Oct 2021 01:43:40 GMT
CMD ["bash"]
# Mon, 01 Nov 2021 22:18:58 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Mon, 01 Nov 2021 22:18:59 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Mon, 01 Nov 2021 22:19:10 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Mon, 01 Nov 2021 22:19:13 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Mon, 01 Nov 2021 22:19:13 GMT
ENV LC_ALL=en_US.UTF-8
# Mon, 01 Nov 2021 22:19:14 GMT
ENV LANG=en_US.UTF-8
# Mon, 01 Nov 2021 22:19:15 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Mon, 01 Nov 2021 22:19:16 GMT
ENV R_BASE_VERSION=4.1.2
# Mon, 01 Nov 2021 22:19:17 GMT
RUN echo "deb http://deb.debian.org/debian experimental main" > /etc/apt/sources.list.d/experimental.list     && echo "deb [trusted=yes] https://eddelbuettel.github.io/ppaR400 ./" > /etc/apt/sources.list.d/edd-r4.list
# Mon, 01 Nov 2021 22:20:17 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Mon, 01 Nov 2021 22:20:18 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:0a75495c66c5fc986e1fa178fa94fe24ac603e1ee8a61ff4b344624e0b8b030e`  
		Last Modified: Tue, 12 Oct 2021 01:52:57 GMT  
		Size: 54.5 MB (54465025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63c8d7fee44c549b526333f2fa675bcda3739b1b0a9913bccd27242c0d449036`  
		Last Modified: Mon, 01 Nov 2021 22:20:33 GMT  
		Size: 1.8 KB (1761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6043930ad0b89b70492c2933bb4b1ac26fc3c329a4f09b4efade34559d2a6064`  
		Last Modified: Mon, 01 Nov 2021 22:20:35 GMT  
		Size: 25.7 MB (25709011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:244ca69eb7bf6342f079b34a713ea95f9404a810ea387c9e6b3202f216f28035`  
		Last Modified: Mon, 01 Nov 2021 22:20:31 GMT  
		Size: 864.6 KB (864603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:664e83e6514dcb43e83f7fa0c20175c6f4f3383b793de2d6feea2ebbd5984934`  
		Last Modified: Mon, 01 Nov 2021 22:20:32 GMT  
		Size: 349.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45081130fa47f08935130d2a1f04061cad24e8221b2e98cee068e803ea2b43c2`  
		Last Modified: Mon, 01 Nov 2021 22:20:31 GMT  
		Size: 293.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b184dc1e127a2cebfd993a8091b0e730ef497df9d3e1e76972a2bae86741e0a`  
		Last Modified: Mon, 01 Nov 2021 22:20:59 GMT  
		Size: 233.3 MB (233341739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:latest` - linux; ppc64le

```console
$ docker pull r-base@sha256:638b06c42d007f28aa4b7fed8da1e0014145ab34b42a722301082b647bb12f15
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **323.1 MB (323096135 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:50b6280464d767b85fd83ee29c3db02eacdbfeeef6c815c46879fceaa7eddeca`
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
# Tue, 12 Oct 2021 17:34:18 GMT
ENV R_BASE_VERSION=4.1.1
# Tue, 12 Oct 2021 17:34:26 GMT
RUN echo "deb http://deb.debian.org/debian experimental main" > /etc/apt/sources.list.d/experimental.list     && echo "deb [trusted=yes] https://eddelbuettel.github.io/ppaR400 ./" > /etc/apt/sources.list.d/edd-r4.list
# Tue, 12 Oct 2021 17:39:17 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 17:39:22 GMT
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
	-	`sha256:fd9d61c392e58a19af006c7d94d67d4b99ff143d8b80c2b0df601842d14706e4`  
		Last Modified: Tue, 12 Oct 2021 17:39:41 GMT  
		Size: 295.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5af26b2299628ac45f6d8f88c4de6f247078dc20364582978724d77ded6539f3`  
		Last Modified: Tue, 12 Oct 2021 17:40:18 GMT  
		Size: 236.7 MB (236678395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:latest` - linux; s390x

```console
$ docker pull r-base@sha256:dcaeb2be1d58d90350dabf435f608122746feb78a4079280f00b32ef9cd0ec71
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **292.5 MB (292492241 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d9c7a61a54af603941d8c5a1f13eba03191cbcf27295f4c1adb87bd2ad9c8ff`
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
# Mon, 01 Nov 2021 22:20:32 GMT
ENV R_BASE_VERSION=4.1.2
# Mon, 01 Nov 2021 22:20:32 GMT
RUN echo "deb http://deb.debian.org/debian experimental main" > /etc/apt/sources.list.d/experimental.list     && echo "deb [trusted=yes] https://eddelbuettel.github.io/ppaR400 ./" > /etc/apt/sources.list.d/edd-r4.list
# Mon, 01 Nov 2021 22:21:27 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Mon, 01 Nov 2021 22:21:32 GMT
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
	-	`sha256:80fe35488d21277fb4073fd95f1da6874301b6726774e6f595046efb9fa28c9e`  
		Last Modified: Mon, 01 Nov 2021 22:21:48 GMT  
		Size: 290.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fc108576b3ef210b94d427a42f6710acbcbb68e04dba999035336c20ab4c470`  
		Last Modified: Mon, 01 Nov 2021 22:22:08 GMT  
		Size: 212.2 MB (212187366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
