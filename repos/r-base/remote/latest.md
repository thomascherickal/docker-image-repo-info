## `r-base:latest`

```console
$ docker pull r-base@sha256:b86b8dc59dc9b8c41c7d92d23d80a3ad741d4fcb8ff9d878c77622faac4beefa
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
$ docker pull r-base@sha256:003c4a9630585a9104d8934e2c4e5c3cf36deaf53dce91a76309a34c711fa7e7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **316.1 MB (316094896 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:21c2346e82909e26530c61c0c3a0c73fbb9978a2e84b42d1a3870fc0dddcf0db`
-	Default Command: `["R"]`

```dockerfile
# Tue, 04 Aug 2020 04:47:25 GMT
ADD file:9716ddb36e63999f28bcc07b306d92cd35c4756a6acde3756dbea757b729c977 in / 
# Tue, 04 Aug 2020 04:47:34 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 16:09:14 GMT
LABEL org.label-schema.license=GPL-2.0 org.label-schema.vcs-url=https://github.com/rocker-org/r-base org.label-schema.vendor=Rocker Project maintainer=Dirk Eddelbuettel <edd@debian.org>
# Tue, 04 Aug 2020 16:09:29 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Tue, 04 Aug 2020 16:13:15 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		ed 		fonts-texgyre 		less 		locales 		vim-tiny 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 16:13:38 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Tue, 04 Aug 2020 16:13:46 GMT
ENV LC_ALL=en_US.UTF-8
# Tue, 04 Aug 2020 16:13:55 GMT
ENV LANG=en_US.UTF-8
# Tue, 04 Aug 2020 16:14:25 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default
# Tue, 04 Aug 2020 16:14:38 GMT
ENV R_BASE_VERSION=4.0.2
# Tue, 04 Aug 2020 16:30:38 GMT
RUN apt-get update         && apt-get install -t unstable -y --no-install-recommends                 gcc-9-base                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/build.r /usr/local/bin/build.r 	&& ln -s /usr/lib/R/site-library/littler/examples/check.r /usr/local/bin/check.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 16:30:52 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:cd5f9f7e65334c771d2f0cd8807ea5d5471b03ab32cd37132f270f6823fa6f2a`  
		Last Modified: Tue, 04 Aug 2020 04:55:20 GMT  
		Size: 55.7 MB (55655911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5ee264a174ebea6765723e13739cf6bd789dc2818510f09a8d7d910861fc1ee`  
		Last Modified: Tue, 04 Aug 2020 16:31:19 GMT  
		Size: 1.9 KB (1896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15c4a5cff8be3c83d20dfe2fe0cf0cff3753cee4e840117321ccf43eb203273f`  
		Last Modified: Tue, 04 Aug 2020 16:31:25 GMT  
		Size: 27.7 MB (27656339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8966c19eaf2734690c61f719a0ef241661a1cfde7a419c5a504d3406679b6b8d`  
		Last Modified: Tue, 04 Aug 2020 16:31:20 GMT  
		Size: 863.6 KB (863578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:305d074cbd5931b2d934cde33a6a87e4b043dffa79b5e4e679816c4e3663c2ef`  
		Last Modified: Tue, 04 Aug 2020 16:31:20 GMT  
		Size: 297.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bfadba48f2bf88e7438fcf101068a9cac7fe6a823a77a6bd09b1710db1d3d67`  
		Last Modified: Tue, 04 Aug 2020 16:32:00 GMT  
		Size: 231.9 MB (231916875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
