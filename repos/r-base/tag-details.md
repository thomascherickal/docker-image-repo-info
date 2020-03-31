<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `r-base`

-	[`r-base:3.6.3`](#r-base363)
-	[`r-base:latest`](#r-baselatest)

## `r-base:3.6.3`

```console
$ docker pull r-base@sha256:bf512c6747021c7445dca1029801b1009611544dfb3f8531b114a1015371ca6e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `r-base:3.6.3` - linux; amd64

```console
$ docker pull r-base@sha256:f376e70ce4ca16030025ca2948ed481dd4829fa8a5dfb64404154bf5fa4ba5e4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **298.4 MB (298357189 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9b18c25082fdd0e73ed7a9f288db58af0d8f83f108ecba3f7bd04914a56ce5d`
-	Default Command: `["R"]`

```dockerfile
# Tue, 31 Mar 2020 01:24:24 GMT
ADD file:ef6d0ed43a7e57298514883c056f9c35630c293bcd6a5189ade9a7c839492abf in / 
# Tue, 31 Mar 2020 01:24:24 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 04:32:41 GMT
LABEL org.label-schema.license=GPL-2.0 org.label-schema.vcs-url=https://github.com/rocker-org/r-base org.label-schema.vendor=Rocker Project maintainer=Dirk Eddelbuettel <edd@debian.org>
# Tue, 31 Mar 2020 04:32:42 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Tue, 31 Mar 2020 04:32:52 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 04:32:55 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Tue, 31 Mar 2020 04:32:55 GMT
ENV LC_ALL=en_US.UTF-8
# Tue, 31 Mar 2020 04:32:56 GMT
ENV LANG=en_US.UTF-8
# Tue, 31 Mar 2020 04:32:56 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default
# Tue, 31 Mar 2020 04:32:57 GMT
ENV R_BASE_VERSION=3.6.3
# Tue, 31 Mar 2020 04:34:05 GMT
RUN apt-get update 	&& apt-get install -t unstable -y --no-install-recommends 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 04:34:06 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:c551897442bae279f3dc3299b5e89627f556d06912d81bd777e18eb066414c32`  
		Last Modified: Tue, 31 Mar 2020 01:29:45 GMT  
		Size: 51.9 MB (51922694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4159dc113650861209ddf42e53425f0521f9bf4f93549e21215efeb696b8d3e5`  
		Last Modified: Tue, 31 Mar 2020 04:34:14 GMT  
		Size: 1.8 KB (1843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c34992aa62704c0b9c0cf2428a9ef639b77183a7e53a3b3768704e9585a0dd8`  
		Last Modified: Tue, 31 Mar 2020 04:34:23 GMT  
		Size: 27.3 MB (27294295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1280af9307bb541416f3f0e838ce99e07acd236c8e9ba897909caf3d3bed1f74`  
		Last Modified: Tue, 31 Mar 2020 04:34:15 GMT  
		Size: 863.4 KB (863394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5416fbde85630b1724eed292ae9d519e7123aac0bb27d54a47cd03d7080c9c0`  
		Last Modified: Tue, 31 Mar 2020 04:34:14 GMT  
		Size: 295.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58958fe491e18cb33a0551fb26186449a038987d8eba4e45c3f450239541692d`  
		Last Modified: Tue, 31 Mar 2020 04:35:04 GMT  
		Size: 218.3 MB (218274668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:3.6.3` - linux; arm64 variant v8

```console
$ docker pull r-base@sha256:dd0b586f7e1b84b0aa847e8f3d4f46f7618f2b7577103fd8fb2513172c963d38
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **287.3 MB (287331272 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc8238920874c204f0b4d240a32b900010ecd1acfc6e67a73ce0dee66482ce1b`
-	Default Command: `["R"]`

```dockerfile
# Wed, 26 Feb 2020 00:51:35 GMT
ADD file:e032e27e8935ad66dc76d8dd15bdf9fb36fcc0318c7e322fcdae2ee219c11b61 in / 
# Wed, 26 Feb 2020 00:51:42 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 14:50:40 GMT
LABEL org.label-schema.license=GPL-2.0 org.label-schema.vcs-url=https://github.com/rocker-org/r-base org.label-schema.vendor=Rocker Project maintainer=Dirk Eddelbuettel <edd@debian.org>
# Wed, 26 Feb 2020 14:50:45 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Wed, 26 Feb 2020 14:51:13 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 14:51:22 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Wed, 26 Feb 2020 14:51:24 GMT
ENV LC_ALL=en_US.UTF-8
# Wed, 26 Feb 2020 14:51:25 GMT
ENV LANG=en_US.UTF-8
# Wed, 26 Feb 2020 14:51:28 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default
# Tue, 03 Mar 2020 00:43:01 GMT
ENV R_BASE_VERSION=3.6.3
# Tue, 03 Mar 2020 00:44:58 GMT
RUN apt-get update 	&& apt-get install -t unstable -y --no-install-recommends 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Tue, 03 Mar 2020 00:45:01 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:c55f06ecbc45a6b3fd4dcd737b73d5b6baa8545548d0610d133fad7fbb7be09e`  
		Last Modified: Wed, 26 Feb 2020 00:59:19 GMT  
		Size: 50.8 MB (50808498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7aa40081a4c3acb54721ed8af71d9d8b92228a4f62dfb4f98151de81d7e11c8`  
		Last Modified: Wed, 26 Feb 2020 14:53:44 GMT  
		Size: 1.9 KB (1888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fd25a08d3e01c623cda4e3d1ef09fcd60d55ac12b8cdb6ef3b91e1965b2fb4e`  
		Last Modified: Wed, 26 Feb 2020 14:53:50 GMT  
		Size: 27.2 MB (27227086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58bcd97dd1ca4be9976e01ac68037d0e11521e394d53544c3c158e4275af2754`  
		Last Modified: Wed, 26 Feb 2020 14:53:44 GMT  
		Size: 862.9 KB (862866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:161edfc7e36fd4c7de2c2a209076952456b6a85288218f171c1b4dd7c43480a9`  
		Last Modified: Wed, 26 Feb 2020 14:53:44 GMT  
		Size: 296.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fac50520fee20a4e6dae3924bc1d109df256a0884d098538528145f6909d2c1`  
		Last Modified: Tue, 03 Mar 2020 00:46:03 GMT  
		Size: 208.4 MB (208430638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `r-base:latest`

```console
$ docker pull r-base@sha256:bf512c6747021c7445dca1029801b1009611544dfb3f8531b114a1015371ca6e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `r-base:latest` - linux; amd64

```console
$ docker pull r-base@sha256:f376e70ce4ca16030025ca2948ed481dd4829fa8a5dfb64404154bf5fa4ba5e4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **298.4 MB (298357189 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9b18c25082fdd0e73ed7a9f288db58af0d8f83f108ecba3f7bd04914a56ce5d`
-	Default Command: `["R"]`

```dockerfile
# Tue, 31 Mar 2020 01:24:24 GMT
ADD file:ef6d0ed43a7e57298514883c056f9c35630c293bcd6a5189ade9a7c839492abf in / 
# Tue, 31 Mar 2020 01:24:24 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 04:32:41 GMT
LABEL org.label-schema.license=GPL-2.0 org.label-schema.vcs-url=https://github.com/rocker-org/r-base org.label-schema.vendor=Rocker Project maintainer=Dirk Eddelbuettel <edd@debian.org>
# Tue, 31 Mar 2020 04:32:42 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Tue, 31 Mar 2020 04:32:52 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 04:32:55 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Tue, 31 Mar 2020 04:32:55 GMT
ENV LC_ALL=en_US.UTF-8
# Tue, 31 Mar 2020 04:32:56 GMT
ENV LANG=en_US.UTF-8
# Tue, 31 Mar 2020 04:32:56 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default
# Tue, 31 Mar 2020 04:32:57 GMT
ENV R_BASE_VERSION=3.6.3
# Tue, 31 Mar 2020 04:34:05 GMT
RUN apt-get update 	&& apt-get install -t unstable -y --no-install-recommends 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 04:34:06 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:c551897442bae279f3dc3299b5e89627f556d06912d81bd777e18eb066414c32`  
		Last Modified: Tue, 31 Mar 2020 01:29:45 GMT  
		Size: 51.9 MB (51922694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4159dc113650861209ddf42e53425f0521f9bf4f93549e21215efeb696b8d3e5`  
		Last Modified: Tue, 31 Mar 2020 04:34:14 GMT  
		Size: 1.8 KB (1843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c34992aa62704c0b9c0cf2428a9ef639b77183a7e53a3b3768704e9585a0dd8`  
		Last Modified: Tue, 31 Mar 2020 04:34:23 GMT  
		Size: 27.3 MB (27294295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1280af9307bb541416f3f0e838ce99e07acd236c8e9ba897909caf3d3bed1f74`  
		Last Modified: Tue, 31 Mar 2020 04:34:15 GMT  
		Size: 863.4 KB (863394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5416fbde85630b1724eed292ae9d519e7123aac0bb27d54a47cd03d7080c9c0`  
		Last Modified: Tue, 31 Mar 2020 04:34:14 GMT  
		Size: 295.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58958fe491e18cb33a0551fb26186449a038987d8eba4e45c3f450239541692d`  
		Last Modified: Tue, 31 Mar 2020 04:35:04 GMT  
		Size: 218.3 MB (218274668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:latest` - linux; arm64 variant v8

```console
$ docker pull r-base@sha256:dd0b586f7e1b84b0aa847e8f3d4f46f7618f2b7577103fd8fb2513172c963d38
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **287.3 MB (287331272 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc8238920874c204f0b4d240a32b900010ecd1acfc6e67a73ce0dee66482ce1b`
-	Default Command: `["R"]`

```dockerfile
# Wed, 26 Feb 2020 00:51:35 GMT
ADD file:e032e27e8935ad66dc76d8dd15bdf9fb36fcc0318c7e322fcdae2ee219c11b61 in / 
# Wed, 26 Feb 2020 00:51:42 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 14:50:40 GMT
LABEL org.label-schema.license=GPL-2.0 org.label-schema.vcs-url=https://github.com/rocker-org/r-base org.label-schema.vendor=Rocker Project maintainer=Dirk Eddelbuettel <edd@debian.org>
# Wed, 26 Feb 2020 14:50:45 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Wed, 26 Feb 2020 14:51:13 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 14:51:22 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Wed, 26 Feb 2020 14:51:24 GMT
ENV LC_ALL=en_US.UTF-8
# Wed, 26 Feb 2020 14:51:25 GMT
ENV LANG=en_US.UTF-8
# Wed, 26 Feb 2020 14:51:28 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default
# Tue, 03 Mar 2020 00:43:01 GMT
ENV R_BASE_VERSION=3.6.3
# Tue, 03 Mar 2020 00:44:58 GMT
RUN apt-get update 	&& apt-get install -t unstable -y --no-install-recommends 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Tue, 03 Mar 2020 00:45:01 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:c55f06ecbc45a6b3fd4dcd737b73d5b6baa8545548d0610d133fad7fbb7be09e`  
		Last Modified: Wed, 26 Feb 2020 00:59:19 GMT  
		Size: 50.8 MB (50808498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7aa40081a4c3acb54721ed8af71d9d8b92228a4f62dfb4f98151de81d7e11c8`  
		Last Modified: Wed, 26 Feb 2020 14:53:44 GMT  
		Size: 1.9 KB (1888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fd25a08d3e01c623cda4e3d1ef09fcd60d55ac12b8cdb6ef3b91e1965b2fb4e`  
		Last Modified: Wed, 26 Feb 2020 14:53:50 GMT  
		Size: 27.2 MB (27227086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58bcd97dd1ca4be9976e01ac68037d0e11521e394d53544c3c158e4275af2754`  
		Last Modified: Wed, 26 Feb 2020 14:53:44 GMT  
		Size: 862.9 KB (862866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:161edfc7e36fd4c7de2c2a209076952456b6a85288218f171c1b4dd7c43480a9`  
		Last Modified: Wed, 26 Feb 2020 14:53:44 GMT  
		Size: 296.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fac50520fee20a4e6dae3924bc1d109df256a0884d098538528145f6909d2c1`  
		Last Modified: Tue, 03 Mar 2020 00:46:03 GMT  
		Size: 208.4 MB (208430638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
