<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `r-base`

-	[`r-base:3.6.3`](#r-base363)
-	[`r-base:latest`](#r-baselatest)

## `r-base:3.6.3`

**does not exist** (yet?)

## `r-base:latest`

```console
$ docker pull r-base@sha256:1e10ff2cb64a5129ed4b23b0bb720854739dd31d677bcf2d289c897373fc2bf7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `r-base:latest` - linux; amd64

```console
$ docker pull r-base@sha256:15ce6ce530ed183970d2409c262dacc3169ad6375676eda607935f0a8c71c01e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **295.8 MB (295789081 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46edce0e80af6bbf7ea93306dfc96aebd26b17a09270ce4318bdb1a6c59e63e2`
-	Default Command: `["R"]`

```dockerfile
# Wed, 26 Feb 2020 00:41:54 GMT
ADD file:bf9b71c3da178fa1ba282c110853082e94e9f8a90773b43b6104bdb8c9e54f5a in / 
# Wed, 26 Feb 2020 00:41:54 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 17:58:31 GMT
LABEL org.label-schema.license=GPL-2.0 org.label-schema.vcs-url=https://github.com/rocker-org/r-base org.label-schema.vendor=Rocker Project maintainer=Dirk Eddelbuettel <edd@debian.org>
# Wed, 26 Feb 2020 17:58:33 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Wed, 26 Feb 2020 17:58:55 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 17:59:00 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Wed, 26 Feb 2020 17:59:00 GMT
ENV LC_ALL=en_US.UTF-8
# Wed, 26 Feb 2020 17:59:00 GMT
ENV LANG=en_US.UTF-8
# Wed, 26 Feb 2020 17:59:02 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default
# Wed, 26 Feb 2020 17:59:02 GMT
ENV R_BASE_VERSION=3.6.2
# Wed, 26 Feb 2020 18:00:10 GMT
RUN apt-get update 	&& apt-get install -t unstable -y --no-install-recommends 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 18:00:11 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:1fcd5305bc72cb154c6bf3d1a204b8bcfc0d91d4811e6681dd2b7aafdaaa8669`  
		Last Modified: Wed, 26 Feb 2020 00:47:41 GMT  
		Size: 51.9 MB (51852708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11dae79a979ed78d9ab050337efd0a70e97e541a58aca4a9ef4decd0f444bd26`  
		Last Modified: Wed, 26 Feb 2020 18:00:18 GMT  
		Size: 1.8 KB (1844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bb692405f4d99a70dcd1dd32a1e0f61045fa501ed9a1bc7c42ca1ee1273f52b`  
		Last Modified: Wed, 26 Feb 2020 18:00:23 GMT  
		Size: 27.4 MB (27351738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9280d4f7544d4a121297722e320f2a93e71a8d793194a81be9578fd9e1452383`  
		Last Modified: Wed, 26 Feb 2020 18:00:19 GMT  
		Size: 862.9 KB (862861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab66f892f181dfa4664981ea04e0c6d793050629bf32a7aa1b9426cdec37458d`  
		Last Modified: Wed, 26 Feb 2020 18:00:19 GMT  
		Size: 295.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4c9c0b1c815a5dd3917751a96bbba8a0c7c164e1910b7e2f67261c6b8372fe8`  
		Last Modified: Wed, 26 Feb 2020 18:00:52 GMT  
		Size: 215.7 MB (215719635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:latest` - linux; arm64 variant v8

```console
$ docker pull r-base@sha256:a52d90f395cc0a06fa58dc29cab796b9dbf77cf7ac02327805e6fc866c06ef2a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **286.3 MB (286284608 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5539466a3046cce5ff87feb750088e4ff7a9e466b2cf998507db5ae4d87802fb`
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
# Wed, 26 Feb 2020 14:51:29 GMT
ENV R_BASE_VERSION=3.6.2
# Wed, 26 Feb 2020 14:53:27 GMT
RUN apt-get update 	&& apt-get install -t unstable -y --no-install-recommends 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 14:53:32 GMT
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
	-	`sha256:19dc28d0921b9d508d58a3b2f664df7810e92631e2795fe82964055f1eb6009e`  
		Last Modified: Wed, 26 Feb 2020 14:54:35 GMT  
		Size: 207.4 MB (207383974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
