<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `r-base`

-	[`r-base:4.0.3`](#r-base403)
-	[`r-base:latest`](#r-baselatest)

## `r-base:4.0.3`

**does not exist** (yet?)

## `r-base:latest`

```console
$ docker pull r-base@sha256:837898ed6a0dc6f9cb0f3d1fa0e801f01673797cdfd3e21c8cd2ad60f2dbe2da
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `r-base:latest` - linux; amd64

```console
$ docker pull r-base@sha256:1c4e181b5dbeef804a4bf1f2c6b888b0d2da333b1a5d99f0e1a3ced46b1cdaef
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **312.5 MB (312452725 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:673e45d6ffe13b98601b5e19ec2bfbd4ec1b1c135ed9d9e911f6c83c7b9cef1e`
-	Default Command: `["R"]`

```dockerfile
# Thu, 10 Sep 2020 00:30:59 GMT
ADD file:9b259b9d58cb55d3126a7ca20eeb5e20e8b26291fc1b738051ff61c8ec22bd95 in / 
# Thu, 10 Sep 2020 00:30:59 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 19:19:45 GMT
LABEL org.label-schema.license=GPL-2.0 org.label-schema.vcs-url=https://github.com/rocker-org/r-base org.label-schema.vendor=Rocker Project maintainer=Dirk Eddelbuettel <edd@debian.org>
# Thu, 10 Sep 2020 19:19:46 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Thu, 10 Sep 2020 19:19:57 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		ed 		fonts-texgyre 		less 		locales 		vim-tiny 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 19:20:00 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Thu, 10 Sep 2020 19:20:00 GMT
ENV LC_ALL=en_US.UTF-8
# Thu, 10 Sep 2020 19:20:00 GMT
ENV LANG=en_US.UTF-8
# Thu, 10 Sep 2020 19:20:01 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default
# Thu, 10 Sep 2020 19:20:01 GMT
ENV R_BASE_VERSION=4.0.2
# Thu, 10 Sep 2020 19:20:50 GMT
RUN apt-get update         && apt-get install -t unstable -y --no-install-recommends                 gcc-9-base                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/build.r /usr/local/bin/build.r 	&& ln -s /usr/lib/R/site-library/littler/examples/check.r /usr/local/bin/check.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 19:20:51 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:4363cc52203477cd66948034ae4a1db71cbfd27fddb648dd9c590161de1f8634`  
		Last Modified: Thu, 10 Sep 2020 00:37:58 GMT  
		Size: 51.9 MB (51906560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa432a30f21d0c64a0d61cf4c70613a6688d7cce4e504320ae34acca4446d784`  
		Last Modified: Thu, 10 Sep 2020 19:21:06 GMT  
		Size: 1.8 KB (1845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:052b8b887e975dd932da84fc5d0ac5d8e8da9d2b06ff214b8550c5071bd86f69`  
		Last Modified: Thu, 10 Sep 2020 19:21:10 GMT  
		Size: 27.4 MB (27387940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cdedc0b6b14d543e587173286437c5a39d4b33d262212bbdbba8eab5937acca`  
		Last Modified: Thu, 10 Sep 2020 19:21:06 GMT  
		Size: 863.6 KB (863572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a3db8e977220af707e98f578694fad645a7e00134d58bdf270e9acfe676e5ef`  
		Last Modified: Thu, 10 Sep 2020 19:21:06 GMT  
		Size: 295.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7670dfe48abb5f960fdebd2755c3191aeb882fc47fe52a12be80715c6f2ea85`  
		Last Modified: Thu, 10 Sep 2020 19:21:44 GMT  
		Size: 232.3 MB (232292513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:latest` - linux; arm64 variant v8

```console
$ docker pull r-base@sha256:155e1f6d579a67e53211fcadaa9169ee06cf5cb417e7fcd0f49ec71bb7eef251
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **298.4 MB (298441317 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7bc5f588fb10cbfe808c81edcc940723c82b9d63f32f81516c192a2c2c06d859`
-	Default Command: `["R"]`

```dockerfile
# Wed, 09 Sep 2020 23:55:28 GMT
ADD file:5dde8e807b0c71ebc7645a34be11d591e22056828b80451cd10b4e9e43d50f22 in / 
# Wed, 09 Sep 2020 23:55:29 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 17:42:24 GMT
LABEL org.label-schema.license=GPL-2.0 org.label-schema.vcs-url=https://github.com/rocker-org/r-base org.label-schema.vendor=Rocker Project maintainer=Dirk Eddelbuettel <edd@debian.org>
# Thu, 10 Sep 2020 17:42:29 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Thu, 10 Sep 2020 17:42:53 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		ed 		fonts-texgyre 		less 		locales 		vim-tiny 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 17:43:00 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Thu, 10 Sep 2020 17:43:01 GMT
ENV LC_ALL=en_US.UTF-8
# Thu, 10 Sep 2020 17:43:01 GMT
ENV LANG=en_US.UTF-8
# Thu, 10 Sep 2020 17:43:04 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default
# Thu, 10 Sep 2020 17:43:05 GMT
ENV R_BASE_VERSION=4.0.2
# Thu, 10 Sep 2020 17:44:40 GMT
RUN apt-get update         && apt-get install -t unstable -y --no-install-recommends                 gcc-9-base                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/build.r /usr/local/bin/build.r 	&& ln -s /usr/lib/R/site-library/littler/examples/check.r /usr/local/bin/check.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 17:44:47 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:c3a3b210b20418d18407956d6d337463c452a063f31e10abcc972012479278c3`  
		Last Modified: Thu, 10 Sep 2020 00:02:26 GMT  
		Size: 50.8 MB (50825396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:968fc21bcc0fd6889bb8e690e3bfa3a5c6b4cee6dcf8646f7f89746c2faedefe`  
		Last Modified: Thu, 10 Sep 2020 17:45:01 GMT  
		Size: 1.9 KB (1879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:693e2c06de2948d93a326b6f97e1aa23514f1214772be8062fc2d4fcfa75d538`  
		Last Modified: Thu, 10 Sep 2020 17:45:08 GMT  
		Size: 27.2 MB (27247676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acb24ec0bfb0c1170f8b3fc8ada4ac06e45decb5cd3b79fd00b338587a322b29`  
		Last Modified: Thu, 10 Sep 2020 17:45:01 GMT  
		Size: 863.6 KB (863571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3497c908e5472c628d9cb7e838f1685437f2797f836d7b08db86d4b34137e370`  
		Last Modified: Thu, 10 Sep 2020 17:45:01 GMT  
		Size: 296.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9d3541e7fe79470903d454a772e8900293ca1ee90ba601dcdb69eced43ad3fc`  
		Last Modified: Thu, 10 Sep 2020 17:45:50 GMT  
		Size: 219.5 MB (219502499 bytes)  
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
