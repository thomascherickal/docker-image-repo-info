## `r-base:latest`

```console
$ docker pull r-base@sha256:f476d2a4850da815137f37b3de842c7fd71fa66ee8d4748ee016d5a313f46aab
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `r-base:latest` - linux; amd64

```console
$ docker pull r-base@sha256:0563681bc4b3a1ad6faaa767f8e8b0c2bfb818f921840c032fc9510058b345bb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **335.6 MB (335649989 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fdf8a3637ff60d1859246b0f25899509518f1de18f427dbc18b054b640c4081f`
-	Default Command: `["R"]`

```dockerfile
# Thu, 23 Mar 2023 01:32:10 GMT
ADD file:8d8307b9fddc1a85bdc2e0cbae7db307f7175165470e518c843af6017ba20392 in / 
# Thu, 23 Mar 2023 01:32:10 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 14:22:53 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Thu, 23 Mar 2023 14:22:54 GMT
RUN useradd -s /bin/bash -m docker 	&& usermod -a -G staff docker
# Thu, 23 Mar 2023 14:23:05 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 14:23:07 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Thu, 23 Mar 2023 14:23:07 GMT
ENV LC_ALL=en_US.UTF-8
# Thu, 23 Mar 2023 14:23:07 GMT
ENV LANG=en_US.UTF-8
# Thu, 23 Mar 2023 14:23:08 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Thu, 23 Mar 2023 14:23:08 GMT
ENV R_BASE_VERSION=4.2.3
# Thu, 23 Mar 2023 14:23:08 GMT
RUN echo "deb http://deb.debian.org/debian experimental main" > /etc/apt/sources.list.d/experimental.list     && echo "deb [trusted=yes] https://eddelbuettel.github.io/ppaR400 ./" > /etc/apt/sources.list.d/edd-r4.list
# Thu, 23 Mar 2023 14:24:58 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-docopt                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& chown root:staff "/usr/local/lib/R/site-library" 	&& chmod g+ws "/usr/local/lib/R/site-library" 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 14:25:00 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:6206d2afdcc78a73e0273edeb8fdfdbe4df15938287b733a2bbe2c7d634134cc`  
		Last Modified: Thu, 23 Mar 2023 01:36:54 GMT  
		Size: 49.3 MB (49278028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcde30a737d784ab8bbe49a3d3d40950c92f581dced4f71fdc8b35c9eab6b13f`  
		Last Modified: Thu, 23 Mar 2023 14:25:23 GMT  
		Size: 3.4 KB (3360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42693d24bae93ea6350d77b5046a19a92270e581bdfd35bc53b3127e1ef36ae5`  
		Last Modified: Thu, 23 Mar 2023 14:25:24 GMT  
		Size: 25.1 MB (25122758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c47534dbe0b2b143e29b79ea989103456e923784445aac35459f0b9e8398e45`  
		Last Modified: Thu, 23 Mar 2023 14:25:21 GMT  
		Size: 865.9 KB (865851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74267105dcfb182a1a4b0a32488a75dc9c37a94c0e6b6bf95a02ed36e8196dde`  
		Last Modified: Thu, 23 Mar 2023 14:25:21 GMT  
		Size: 348.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdc5edd4b48445ef8e62900aa9c38cb7d06fa402fdd221f6a147ef238d0371eb`  
		Last Modified: Thu, 23 Mar 2023 14:25:21 GMT  
		Size: 291.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fc5a8c5a94e9777675e61cd3765c986f9e7ec11dd2412028971c5449a291e68`  
		Last Modified: Thu, 23 Mar 2023 14:25:50 GMT  
		Size: 260.4 MB (260379353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:latest` - linux; arm64 variant v8

```console
$ docker pull r-base@sha256:6be4e05a10a22e42ca9ce12e89a3496c35de517c41345a691c7fae989ac8618c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **321.7 MB (321696075 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7eb171d7c656b07647244bdde238a2819e9dee621202aaa7cbf35ed8cf711f9e`
-	Default Command: `["R"]`

```dockerfile
# Wed, 12 Apr 2023 00:40:46 GMT
ADD file:80a4d0d891f9f28bd3948de18579583b6c11a4a8805b6230daaa0ac2a35c453d in / 
# Wed, 12 Apr 2023 00:40:46 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 03:14:34 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Wed, 12 Apr 2023 03:14:34 GMT
RUN useradd -s /bin/bash -m docker 	&& usermod -a -G staff docker
# Wed, 12 Apr 2023 03:14:44 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 03:14:46 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Wed, 12 Apr 2023 03:14:46 GMT
ENV LC_ALL=en_US.UTF-8
# Wed, 12 Apr 2023 03:14:46 GMT
ENV LANG=en_US.UTF-8
# Wed, 12 Apr 2023 03:14:47 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Wed, 12 Apr 2023 03:14:47 GMT
ENV R_BASE_VERSION=4.2.3
# Wed, 12 Apr 2023 03:14:47 GMT
RUN echo "deb http://deb.debian.org/debian experimental main" > /etc/apt/sources.list.d/experimental.list     && echo "deb [trusted=yes] https://eddelbuettel.github.io/ppaR400 ./" > /etc/apt/sources.list.d/edd-r4.list
# Wed, 12 Apr 2023 03:16:45 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-docopt                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& chown root:staff "/usr/local/lib/R/site-library" 	&& chmod g+ws "/usr/local/lib/R/site-library" 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 03:16:49 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:d1d33b0463b9cb723855fca4aff8cdc62c34a1907b920e8e626bd38d7577387f`  
		Last Modified: Wed, 12 Apr 2023 00:44:53 GMT  
		Size: 49.3 MB (49345366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14713ff22710d8236db54cc044463e0fe76c30e886891d410b14a938c637ac2e`  
		Last Modified: Wed, 12 Apr 2023 03:17:03 GMT  
		Size: 3.4 KB (3363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4c8aeb9c8fe2e295c2b3a2fea6a6498c3037b7a49a0e54376b387cdcc70af07`  
		Last Modified: Wed, 12 Apr 2023 03:17:03 GMT  
		Size: 25.0 MB (24982728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65dc3869ed093b5204a7a0a99a9e8ec1c4f4d7606b3bd9178c7bdb6b447feda1`  
		Last Modified: Wed, 12 Apr 2023 03:17:01 GMT  
		Size: 865.9 KB (865850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed6824938d3e4f2d95fd7262fa044aa52ab3114a201c9b36d95bb44e2447fe8e`  
		Last Modified: Wed, 12 Apr 2023 03:17:01 GMT  
		Size: 347.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a63c57f8e04a06247a0854efa50e538419a5e41ef1c20a87725663c2bf3f288`  
		Last Modified: Wed, 12 Apr 2023 03:17:01 GMT  
		Size: 292.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31275e575d0f0c74f798a81a94efc9cc49fae227956a2216b31cd38e953a0e5a`  
		Last Modified: Wed, 12 Apr 2023 03:17:21 GMT  
		Size: 246.5 MB (246498129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:latest` - linux; ppc64le

```console
$ docker pull r-base@sha256:ad733b9b4a87e03010934e45919108b91edda68db1af152852ff0fbebb42a081
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **338.3 MB (338307418 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9be4dafc6800be01321196dcd9ffb4fc9522bfc17143f27022d314c17451f2e`
-	Default Command: `["R"]`

```dockerfile
# Wed, 12 Apr 2023 00:10:00 GMT
ADD file:107d4f159f2bc5b04467e08852422f5c78548e0f92853bd29d5d2b05b387d3a9 in / 
# Wed, 12 Apr 2023 00:10:03 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 07:00:06 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Wed, 12 Apr 2023 07:00:09 GMT
RUN useradd -s /bin/bash -m docker 	&& usermod -a -G staff docker
# Wed, 12 Apr 2023 07:00:38 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 07:00:42 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Wed, 12 Apr 2023 07:00:43 GMT
ENV LC_ALL=en_US.UTF-8
# Wed, 12 Apr 2023 07:00:44 GMT
ENV LANG=en_US.UTF-8
# Wed, 12 Apr 2023 07:00:49 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Wed, 12 Apr 2023 07:00:50 GMT
ENV R_BASE_VERSION=4.2.3
# Wed, 12 Apr 2023 07:00:52 GMT
RUN echo "deb http://deb.debian.org/debian experimental main" > /etc/apt/sources.list.d/experimental.list     && echo "deb [trusted=yes] https://eddelbuettel.github.io/ppaR400 ./" > /etc/apt/sources.list.d/edd-r4.list
# Wed, 12 Apr 2023 07:04:52 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-docopt                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& chown root:staff "/usr/local/lib/R/site-library" 	&& chmod g+ws "/usr/local/lib/R/site-library" 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 07:05:04 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:a4fca5aa8bf3f9957686fb6705daa645629edb94592f35c71e46e52a1742ed1a`  
		Last Modified: Wed, 12 Apr 2023 00:15:06 GMT  
		Size: 53.3 MB (53299985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ccc92c826b071e57f3b9730b591c447939c384fd0951960d6e73c4821bae145`  
		Last Modified: Wed, 12 Apr 2023 07:05:22 GMT  
		Size: 3.4 KB (3366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b353e675eb05b48bb03cfd6c97c6a529edc801a1b0d92f5b66979718503acad`  
		Last Modified: Wed, 12 Apr 2023 07:05:25 GMT  
		Size: 25.6 MB (25556057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f05dceb3b5e9b5ef9cf56dd7755c08657578ca4e044b825f7b7342a468b73c1`  
		Last Modified: Wed, 12 Apr 2023 07:05:21 GMT  
		Size: 865.9 KB (865855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9da64538026eabb52f89dd3e3ead28c549abdf6db2c74f0b1907e132f41d4bb2`  
		Last Modified: Wed, 12 Apr 2023 07:05:20 GMT  
		Size: 350.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fee3887d18fba6a5e77903beb7b737cd07688f7630defc6adb1243a51c613f31`  
		Last Modified: Wed, 12 Apr 2023 07:05:20 GMT  
		Size: 294.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46af209be74a69a79b44a799b71006a0a6a130773a48e5ba48d2e90f8d0a8113`  
		Last Modified: Wed, 12 Apr 2023 07:06:12 GMT  
		Size: 258.6 MB (258581511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:latest` - linux; s390x

```console
$ docker pull r-base@sha256:52e8693051a20a597ee32b15e92010aec71ddd23f9155d2fc8179e366a90c87e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **296.7 MB (296708416 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b6c245f70a07cae74bce941333cae7299361d25fb7565b5d6af2ffa3e71ba12`
-	Default Command: `["R"]`

```dockerfile
# Thu, 23 Mar 2023 00:45:12 GMT
ADD file:a96b8cacbcadb2068e0368c020589f4d2eae9fabb0965b387d5d9fc94831a1a5 in / 
# Thu, 23 Mar 2023 00:45:16 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 10:51:36 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Thu, 23 Mar 2023 10:51:37 GMT
RUN useradd -s /bin/bash -m docker 	&& usermod -a -G staff docker
# Thu, 23 Mar 2023 10:51:46 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 10:51:48 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Thu, 23 Mar 2023 10:51:48 GMT
ENV LC_ALL=en_US.UTF-8
# Thu, 23 Mar 2023 10:51:48 GMT
ENV LANG=en_US.UTF-8
# Thu, 23 Mar 2023 10:51:49 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Thu, 23 Mar 2023 10:51:49 GMT
ENV R_BASE_VERSION=4.2.3
# Thu, 23 Mar 2023 10:51:50 GMT
RUN echo "deb http://deb.debian.org/debian experimental main" > /etc/apt/sources.list.d/experimental.list     && echo "deb [trusted=yes] https://eddelbuettel.github.io/ppaR400 ./" > /etc/apt/sources.list.d/edd-r4.list
# Thu, 23 Mar 2023 10:52:53 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-docopt                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& chown root:staff "/usr/local/lib/R/site-library" 	&& chmod g+ws "/usr/local/lib/R/site-library" 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 10:53:04 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:57560ce693355ef04b6283597b61cd71f7e8b7d7357b218eab0c8979bce7812e`  
		Last Modified: Thu, 23 Mar 2023 00:48:17 GMT  
		Size: 47.7 MB (47671021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d80793af67a69232cadace34e10b9ef46d1ba6f3755a4614ccbfb7a911f055a9`  
		Last Modified: Thu, 23 Mar 2023 10:53:16 GMT  
		Size: 3.4 KB (3357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:399fe0d57620fc4b657bb26fc130a45cf377513e271deb6fa7b2430a78ed54e3`  
		Last Modified: Thu, 23 Mar 2023 10:53:17 GMT  
		Size: 24.8 MB (24801489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a4f7d7095b671f7050cb36cce96b79401ba687ff33672f032f5bddf44ecab9b`  
		Last Modified: Thu, 23 Mar 2023 10:53:15 GMT  
		Size: 921.0 KB (921009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4593aadb093cfdef343d4697cdbe74987731c5b65b563859b94321451ccda65`  
		Last Modified: Thu, 23 Mar 2023 10:53:15 GMT  
		Size: 348.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe3069e7378cf84ce8edecd9a388442fd79d6a305de51d312c72859f4a652685`  
		Last Modified: Thu, 23 Mar 2023 10:53:15 GMT  
		Size: 292.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b341b8c60321724abfbc967e97de155e9a198bb86c525745b76bc63085e26bfd`  
		Last Modified: Thu, 23 Mar 2023 10:53:39 GMT  
		Size: 223.3 MB (223310900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
