## `r-base:latest`

```console
$ docker pull r-base@sha256:3663986441166edb4c8c8cfdc9258471c199a9f4f7acf264b027cc0db11711ea
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `r-base:latest` - linux; amd64

```console
$ docker pull r-base@sha256:2aad7f2fcc87e7f31f7851c89f1081c0933fa381945eceeecdb4a5eb56f8ea07
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **318.2 MB (318218145 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14e2ae5effa6ff9af0f494ad4d3f3a4d6ea03dfa43b49f4dc6421acae4ef92c0`
-	Default Command: `["R"]`

```dockerfile
# Tue, 04 Aug 2020 15:46:04 GMT
ADD file:d3c3063a4966a61da8d68be58dc2f4ebf0dfb1836272c5bd9d6365b79c62d8df in / 
# Tue, 04 Aug 2020 15:46:05 GMT
CMD ["bash"]
# Wed, 05 Aug 2020 06:33:02 GMT
LABEL org.label-schema.license=GPL-2.0 org.label-schema.vcs-url=https://github.com/rocker-org/r-base org.label-schema.vendor=Rocker Project maintainer=Dirk Eddelbuettel <edd@debian.org>
# Wed, 05 Aug 2020 06:33:03 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Wed, 05 Aug 2020 06:33:13 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		ed 		fonts-texgyre 		less 		locales 		vim-tiny 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Aug 2020 06:33:16 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Wed, 05 Aug 2020 06:33:16 GMT
ENV LC_ALL=en_US.UTF-8
# Wed, 05 Aug 2020 06:33:16 GMT
ENV LANG=en_US.UTF-8
# Wed, 05 Aug 2020 06:33:17 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default
# Wed, 05 Aug 2020 06:33:17 GMT
ENV R_BASE_VERSION=4.0.2
# Wed, 05 Aug 2020 06:34:18 GMT
RUN apt-get update         && apt-get install -t unstable -y --no-install-recommends                 gcc-9-base                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/build.r /usr/local/bin/build.r 	&& ln -s /usr/lib/R/site-library/littler/examples/check.r /usr/local/bin/check.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Aug 2020 06:34:18 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:c124bdc7383acd90535c8bdb4b95fa747c8497c6ea51caac97138303198f7b57`  
		Last Modified: Tue, 04 Aug 2020 15:52:32 GMT  
		Size: 51.8 MB (51838176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b76e8bb2fc6cf37b68c2020d927e358a9b1eebb366b0355e890273f083cb3c4`  
		Last Modified: Wed, 05 Aug 2020 06:34:35 GMT  
		Size: 1.9 KB (1858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35e9b4f342ba8b80f52e6283ab700b0e7956ab82cc929d6d14d3cf621e40c5a2`  
		Last Modified: Wed, 05 Aug 2020 06:34:39 GMT  
		Size: 27.4 MB (27387620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb00b22ae63c001139b608bbc1de9f98c8cd2569e052957dfd76da4d3b0273e6`  
		Last Modified: Wed, 05 Aug 2020 06:34:36 GMT  
		Size: 863.6 KB (863576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f89094b6d60c7bd19d508cdf3fac342cdc3eed93105454373971214daeccb85`  
		Last Modified: Wed, 05 Aug 2020 06:34:36 GMT  
		Size: 296.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c16e04fd79a4c0ae486527976cafbbf00105192d70f939f24fc409fc6029225f`  
		Last Modified: Wed, 05 Aug 2020 06:35:08 GMT  
		Size: 238.1 MB (238126619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:latest` - linux; arm64 variant v8

```console
$ docker pull r-base@sha256:df3948b77b984098321acfd1cf230795b3b51d364ebdf5a08942962fb6e88c03
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **298.8 MB (298819904 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b807fc20bc395fa96eb22d07e7d208a7c9966fdfd7eba25ac237bcbd9a6bab2`
-	Default Command: `["R"]`

```dockerfile
# Tue, 04 Aug 2020 07:00:45 GMT
ADD file:725f94f7e6e800981fa8f39228f0ef03900a97a621fb2415173496995bc2de4b in / 
# Tue, 04 Aug 2020 07:00:53 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 14:27:18 GMT
LABEL org.label-schema.license=GPL-2.0 org.label-schema.vcs-url=https://github.com/rocker-org/r-base org.label-schema.vendor=Rocker Project maintainer=Dirk Eddelbuettel <edd@debian.org>
# Tue, 04 Aug 2020 14:27:21 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Tue, 04 Aug 2020 14:27:44 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		ed 		fonts-texgyre 		less 		locales 		vim-tiny 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 14:27:49 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Tue, 04 Aug 2020 14:27:50 GMT
ENV LC_ALL=en_US.UTF-8
# Tue, 04 Aug 2020 14:27:51 GMT
ENV LANG=en_US.UTF-8
# Tue, 04 Aug 2020 14:27:52 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default
# Tue, 04 Aug 2020 14:27:53 GMT
ENV R_BASE_VERSION=4.0.2
# Tue, 04 Aug 2020 14:29:24 GMT
RUN apt-get update         && apt-get install -t unstable -y --no-install-recommends                 gcc-9-base                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/build.r /usr/local/bin/build.r 	&& ln -s /usr/lib/R/site-library/littler/examples/check.r /usr/local/bin/check.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 14:29:28 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:059d2624bd4cbe096feccc25cf0f53c2c9f670f108be6124ea6aeb3b78724b69`  
		Last Modified: Tue, 04 Aug 2020 07:06:56 GMT  
		Size: 50.8 MB (50751849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c68475034381fe7a90e788d7d940d600cdc107c63c75617e0bc2faf544a118f`  
		Last Modified: Tue, 04 Aug 2020 14:29:40 GMT  
		Size: 1.9 KB (1884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62472c910c33df0ee421bb3936f2f9183a7b68ef0567b5ae47232a3c563b1b4f`  
		Last Modified: Tue, 04 Aug 2020 14:29:46 GMT  
		Size: 27.2 MB (27246974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df7c0cf8e71be0cd547aa072898f9cc7b71039709be0f14129c1c52dd0483896`  
		Last Modified: Tue, 04 Aug 2020 14:29:41 GMT  
		Size: 863.6 KB (863575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fea8325a784dd759e5e2685c9cc1f9abe2afc496d5ecbd46679bfc8783f22b2a`  
		Last Modified: Tue, 04 Aug 2020 14:29:40 GMT  
		Size: 297.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41bc631ca52e813d492b710bfb4ad6f78ce072371750e4e92e3dba29a98c21ba`  
		Last Modified: Tue, 04 Aug 2020 14:30:28 GMT  
		Size: 220.0 MB (219955325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:latest` - linux; ppc64le

```console
$ docker pull r-base@sha256:9ce01ec9c95fcd1eeccbd9c66638fb656b56ed7ec6592b42ada5b945a2d99a1f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **315.7 MB (315738177 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b96464c941ad1a3c15c868537fe3ddfcd6d49cd38f74eb3ad7da15202cce0ec7`
-	Default Command: `["R"]`

```dockerfile
# Thu, 10 Sep 2020 01:14:15 GMT
ADD file:1ff1c751892adb35acbc76e9c216d58059214a72e719e3789fb186911933fe1b in / 
# Thu, 10 Sep 2020 01:14:26 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 11:05:02 GMT
LABEL org.label-schema.license=GPL-2.0 org.label-schema.vcs-url=https://github.com/rocker-org/r-base org.label-schema.vendor=Rocker Project maintainer=Dirk Eddelbuettel <edd@debian.org>
# Thu, 10 Sep 2020 11:05:35 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Thu, 10 Sep 2020 11:07:27 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		ed 		fonts-texgyre 		less 		locales 		vim-tiny 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 11:07:45 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Thu, 10 Sep 2020 11:07:52 GMT
ENV LC_ALL=en_US.UTF-8
# Thu, 10 Sep 2020 11:07:59 GMT
ENV LANG=en_US.UTF-8
# Thu, 10 Sep 2020 11:08:09 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default
# Thu, 10 Sep 2020 11:08:13 GMT
ENV R_BASE_VERSION=4.0.2
# Thu, 10 Sep 2020 11:20:53 GMT
RUN apt-get update         && apt-get install -t unstable -y --no-install-recommends                 gcc-9-base                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/build.r /usr/local/bin/build.r 	&& ln -s /usr/lib/R/site-library/littler/examples/check.r /usr/local/bin/check.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 11:21:08 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:4f06950a568456590fe3afbc7dc70475d0e9ea33f4901b4085b036db8288648c`  
		Last Modified: Thu, 10 Sep 2020 01:37:32 GMT  
		Size: 55.8 MB (55774415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4dba42cbd72ea76ebdfdf4d25b40ba35c5f5de1a292409364ed5f2c264cf377`  
		Last Modified: Thu, 10 Sep 2020 11:21:30 GMT  
		Size: 1.9 KB (1893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f352b64e887f6ee0f80ccff79b56078e041b0e9702f7166e5e74f92b0e2be91c`  
		Last Modified: Thu, 10 Sep 2020 11:21:45 GMT  
		Size: 27.7 MB (27656658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13aa724d28495233a8023f94f16edfb0b1169161c602426711e4589e7f721d33`  
		Last Modified: Thu, 10 Sep 2020 11:21:29 GMT  
		Size: 863.6 KB (863577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab640c7a0015fec3a4f7949000d41dc03a85056e9a9b0c08d6f64a1b9350c7de`  
		Last Modified: Thu, 10 Sep 2020 11:21:30 GMT  
		Size: 297.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eac68ae3042d61e264f3fe16042ff97758a8b6a3f556b1b6313972620ad8dc9e`  
		Last Modified: Thu, 10 Sep 2020 11:22:14 GMT  
		Size: 231.4 MB (231441337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
