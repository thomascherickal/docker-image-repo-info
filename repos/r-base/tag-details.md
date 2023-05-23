<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `r-base`

-	[`r-base:4.3.0`](#r-base430)
-	[`r-base:latest`](#r-baselatest)

## `r-base:4.3.0`

```console
$ docker pull r-base@sha256:a9a0c1e77621470c5cf7567e4c4f9e6247f397a0f8472afa2851f460d3fe9070
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `r-base:4.3.0` - linux; amd64

```console
$ docker pull r-base@sha256:157acbe58cb30e19974c438622faac2391e6c6e59394b7d80eb62334a3e1a962
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **336.3 MB (336293440 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2fcb907f9de40b8457c40acee0b68c40c9b1615e972cb790dbc9837f5ece1d73`
-	Default Command: `["R"]`

```dockerfile
# Tue, 02 May 2023 23:48:15 GMT
ADD file:27b4229d808812579f1eb7609d08a5bb2177380a480279009a4ea17e05193323 in / 
# Tue, 02 May 2023 23:48:16 GMT
CMD ["bash"]
# Wed, 03 May 2023 22:21:45 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Wed, 03 May 2023 22:21:46 GMT
RUN useradd -s /bin/bash -m docker 	&& usermod -a -G staff docker
# Wed, 03 May 2023 22:22:00 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 22:22:03 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Wed, 03 May 2023 22:22:03 GMT
ENV LC_ALL=en_US.UTF-8
# Wed, 03 May 2023 22:22:03 GMT
ENV LANG=en_US.UTF-8
# Wed, 03 May 2023 22:22:03 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Wed, 03 May 2023 22:22:04 GMT
ENV R_BASE_VERSION=4.3.0
# Wed, 03 May 2023 22:22:04 GMT
RUN echo "deb http://deb.debian.org/debian experimental main" > /etc/apt/sources.list.d/experimental.list     && echo "deb [trusted=yes] https://eddelbuettel.github.io/ppaR400 ./" > /etc/apt/sources.list.d/edd-r4.list
# Wed, 03 May 2023 22:24:00 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-docopt                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& chown root:staff "/usr/local/lib/R/site-library" 	&& chmod g+ws "/usr/local/lib/R/site-library" 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 22:24:02 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:56c7136ddbfad3eea4cd5c38c0703e58fd25630219d5462a9099387c4b3a4160`  
		Last Modified: Tue, 02 May 2023 23:52:53 GMT  
		Size: 49.3 MB (49299248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37fcdcc91a6decc4daaa550a314607547d473fced34fdf8fa11ff5d186a989fe`  
		Last Modified: Wed, 03 May 2023 22:24:15 GMT  
		Size: 3.4 KB (3360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d61cab462a3f50000df4d96522d023f43218662709e10cbadc1c5a3cf8f2fbe`  
		Last Modified: Wed, 03 May 2023 22:24:16 GMT  
		Size: 25.2 MB (25165628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45fc804098ddade4ca07b4a75d441073309e272796dede6c657a0e1ff37e38b2`  
		Last Modified: Wed, 03 May 2023 22:24:13 GMT  
		Size: 865.9 KB (865851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5be6f23be5f8d3623373487b0e2249a630c173aa58bf25d712a714cc66dd6c2c`  
		Last Modified: Wed, 03 May 2023 22:24:13 GMT  
		Size: 348.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31631317ae9296807ef359039e524151b249e5e4cdd9dace5bc1e62f2d7b7f7e`  
		Last Modified: Wed, 03 May 2023 22:24:14 GMT  
		Size: 292.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8cea77e9be3236da8a7eaef187017822ec2b0c0189c6628247c11fdee613877`  
		Last Modified: Wed, 03 May 2023 22:24:42 GMT  
		Size: 261.0 MB (260958713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:4.3.0` - linux; arm64 variant v8

```console
$ docker pull r-base@sha256:91861e8aba13c60c6071d9679c48247cccd86cb8e7ab1ef07e183b94e6b0ead9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **322.5 MB (322487127 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce1761f714141bd97405c4836c52f793b192b238b8c97f7ea3429afb155a32fc`
-	Default Command: `["R"]`

```dockerfile
# Tue, 23 May 2023 00:44:13 GMT
ADD file:f5e81f28718d3bd832678fa284dcfc626b1a1bd4811a8912a05b9fcefd40d358 in / 
# Tue, 23 May 2023 00:44:14 GMT
CMD ["bash"]
# Tue, 23 May 2023 05:34:15 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Tue, 23 May 2023 05:34:16 GMT
RUN useradd -s /bin/bash -m docker 	&& usermod -a -G staff docker
# Tue, 23 May 2023 05:34:29 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 05:34:31 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Tue, 23 May 2023 05:34:31 GMT
ENV LC_ALL=en_US.UTF-8
# Tue, 23 May 2023 05:34:31 GMT
ENV LANG=en_US.UTF-8
# Tue, 23 May 2023 05:34:31 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Tue, 23 May 2023 05:34:31 GMT
ENV R_BASE_VERSION=4.3.0
# Tue, 23 May 2023 05:34:32 GMT
RUN echo "deb http://deb.debian.org/debian experimental main" > /etc/apt/sources.list.d/experimental.list     && echo "deb [trusted=yes] https://eddelbuettel.github.io/ppaR400 ./" > /etc/apt/sources.list.d/edd-r4.list
# Tue, 23 May 2023 05:36:27 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-docopt                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& chown root:staff "/usr/local/lib/R/site-library" 	&& chmod g+ws "/usr/local/lib/R/site-library" 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 05:36:31 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:93ff152152cfe9dc0fb257b029c2b1838408f3bee982bb891d1f5b4212469796`  
		Last Modified: Tue, 23 May 2023 00:48:27 GMT  
		Size: 49.3 MB (49347786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ee3d7f40578e3aa1c72affc9600f568297c4045a6925af45232026d55516685`  
		Last Modified: Tue, 23 May 2023 05:36:45 GMT  
		Size: 3.4 KB (3362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd1c5782d3c65a19f169d1b47f5f545fbe321d58f4226d46ea40087bd90ba305`  
		Last Modified: Tue, 23 May 2023 05:36:45 GMT  
		Size: 25.0 MB (24984469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de35ff8e5bf38bb95030252e0612bdc9df69a5aef2f74674c144066ca81a0dc7`  
		Last Modified: Tue, 23 May 2023 05:36:43 GMT  
		Size: 865.9 KB (865850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0a413c3a535e4ae71fb940eaaa1e480976dfe7126df21fc52439ac1a5955a26`  
		Last Modified: Tue, 23 May 2023 05:36:43 GMT  
		Size: 350.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c45f1c51f6e65f6533a9bfb08620464c7668b632c3f3b581b32e0e8ab8feae0`  
		Last Modified: Tue, 23 May 2023 05:36:43 GMT  
		Size: 295.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a9c686e72fdc6d6894d54302928d7edd14f4af5aaf1c1e0709a78dfaab70d59`  
		Last Modified: Tue, 23 May 2023 05:37:03 GMT  
		Size: 247.3 MB (247285015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:4.3.0` - linux; ppc64le

```console
$ docker pull r-base@sha256:f84334040c57a42c4424a421fc20f673799e4b568f7a1bd74f5028a159bdb127
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **339.1 MB (339086471 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8bedcbbf2eb9328077bfcd8e3efa357ec3cd674f00b27e3d7bd7dffd8d0a88ba`
-	Default Command: `["R"]`

```dockerfile
# Wed, 03 May 2023 00:33:35 GMT
ADD file:f54f5308138566009df9867a9e17d06810cb24a49786ebfdb8f2d83aa44bd004 in / 
# Wed, 03 May 2023 00:33:38 GMT
CMD ["bash"]
# Thu, 04 May 2023 00:52:09 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Thu, 04 May 2023 00:52:11 GMT
RUN useradd -s /bin/bash -m docker 	&& usermod -a -G staff docker
# Thu, 04 May 2023 00:52:37 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Thu, 04 May 2023 00:52:42 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Thu, 04 May 2023 00:52:43 GMT
ENV LC_ALL=en_US.UTF-8
# Thu, 04 May 2023 00:52:43 GMT
ENV LANG=en_US.UTF-8
# Thu, 04 May 2023 00:52:45 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Thu, 04 May 2023 00:52:46 GMT
ENV R_BASE_VERSION=4.3.0
# Thu, 04 May 2023 00:52:48 GMT
RUN echo "deb http://deb.debian.org/debian experimental main" > /etc/apt/sources.list.d/experimental.list     && echo "deb [trusted=yes] https://eddelbuettel.github.io/ppaR400 ./" > /etc/apt/sources.list.d/edd-r4.list
# Thu, 04 May 2023 00:56:26 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-docopt                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& chown root:staff "/usr/local/lib/R/site-library" 	&& chmod g+ws "/usr/local/lib/R/site-library" 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Thu, 04 May 2023 00:56:30 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:c7778701ecf3e4c7947d5854ffadbfcc47a1bea59eeede267cc1563d0c205014`  
		Last Modified: Wed, 03 May 2023 00:38:50 GMT  
		Size: 53.3 MB (53307302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f66bde9f479501a388f0b05d077e44d65524bbba1ee00f0dcbe703bad4534989`  
		Last Modified: Thu, 04 May 2023 00:56:41 GMT  
		Size: 3.4 KB (3358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5e618648d81125407cb42fcf36722736651dd097ba30c339a03bf4e9a8eb480`  
		Last Modified: Thu, 04 May 2023 00:56:43 GMT  
		Size: 25.6 MB (25560947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfe19135c5349f7250145ae537652ad2d7773f5c17b239681c8e8d715b80f179`  
		Last Modified: Thu, 04 May 2023 00:56:39 GMT  
		Size: 865.9 KB (865852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2b0b041784b86a1a06053e7950eaa748db7f632097dae4d8cc8cd14a8f90861`  
		Last Modified: Thu, 04 May 2023 00:56:38 GMT  
		Size: 351.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6e7ee8a60f067de2ef718e7cb15b003582717cfdd918f4c54cd0ceaeac3e4a5`  
		Last Modified: Thu, 04 May 2023 00:56:38 GMT  
		Size: 293.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d31d894101d3b038b49d338d7b2b136e522ad6078faf61b1460f8af4b087e93d`  
		Last Modified: Thu, 04 May 2023 00:57:33 GMT  
		Size: 259.3 MB (259348368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:4.3.0` - linux; s390x

```console
$ docker pull r-base@sha256:7beab94b8d15d4e89924a423f9a921dd85462cd0c3a83593005447dc94f811f0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **297.5 MB (297547859 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89cf3dfb21fa6695f7f5a2f308b669c5260ce6e1a3fc8e95f32eaf6b334be263`
-	Default Command: `["R"]`

```dockerfile
# Tue, 23 May 2023 00:43:47 GMT
ADD file:6dfd7d21cdfe9dee2a7cad47d8e2e22e6e56bd924f036cb45c183fe31efe66cc in / 
# Tue, 23 May 2023 00:43:49 GMT
CMD ["bash"]
# Tue, 23 May 2023 02:28:29 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Tue, 23 May 2023 02:28:29 GMT
RUN useradd -s /bin/bash -m docker 	&& usermod -a -G staff docker
# Tue, 23 May 2023 02:28:36 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 02:28:39 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Tue, 23 May 2023 02:28:39 GMT
ENV LC_ALL=en_US.UTF-8
# Tue, 23 May 2023 02:28:39 GMT
ENV LANG=en_US.UTF-8
# Tue, 23 May 2023 02:28:39 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Tue, 23 May 2023 02:28:39 GMT
ENV R_BASE_VERSION=4.3.0
# Tue, 23 May 2023 02:28:40 GMT
RUN echo "deb http://deb.debian.org/debian experimental main" > /etc/apt/sources.list.d/experimental.list     && echo "deb [trusted=yes] https://eddelbuettel.github.io/ppaR400 ./" > /etc/apt/sources.list.d/edd-r4.list
# Tue, 23 May 2023 02:30:10 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-docopt                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& chown root:staff "/usr/local/lib/R/site-library" 	&& chmod g+ws "/usr/local/lib/R/site-library" 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 02:30:17 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:af4d11b0c6366f32a980344976c0622adf11030b727c114fcc65377cb3f44688`  
		Last Modified: Tue, 23 May 2023 00:46:43 GMT  
		Size: 47.7 MB (47673474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c3ba3a415d79670199ec98260e42e6b72cc5eea4a1ab6c615b4caacf1cafe4c`  
		Last Modified: Tue, 23 May 2023 02:30:38 GMT  
		Size: 3.4 KB (3364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4d6d4d9b862bc7cad32b844052a1006db830fa9c3583c57182e5fa222cf18f9`  
		Last Modified: Tue, 23 May 2023 02:30:40 GMT  
		Size: 24.8 MB (24833563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83952e1da18fa0309b148dc5f654137f85a9f36300cd3f162c4bb15174507944`  
		Last Modified: Tue, 23 May 2023 02:30:37 GMT  
		Size: 921.0 KB (921007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca68baa69c6585bf823bfe9b5d023333f08dc5970cf017131d3645e4476ab2df`  
		Last Modified: Tue, 23 May 2023 02:30:37 GMT  
		Size: 349.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:128fbc66c9a8965d790c4a7a0b54f7805a39755af051c3c2454a02de3dbb1d58`  
		Last Modified: Tue, 23 May 2023 02:30:37 GMT  
		Size: 293.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97acb00df28ae2a5ef9bb1f50c3d0e0c0c9cb2a433ad2176afaa424016685779`  
		Last Modified: Tue, 23 May 2023 02:31:01 GMT  
		Size: 224.1 MB (224115809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `r-base:latest`

```console
$ docker pull r-base@sha256:a9a0c1e77621470c5cf7567e4c4f9e6247f397a0f8472afa2851f460d3fe9070
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `r-base:latest` - linux; amd64

```console
$ docker pull r-base@sha256:157acbe58cb30e19974c438622faac2391e6c6e59394b7d80eb62334a3e1a962
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **336.3 MB (336293440 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2fcb907f9de40b8457c40acee0b68c40c9b1615e972cb790dbc9837f5ece1d73`
-	Default Command: `["R"]`

```dockerfile
# Tue, 02 May 2023 23:48:15 GMT
ADD file:27b4229d808812579f1eb7609d08a5bb2177380a480279009a4ea17e05193323 in / 
# Tue, 02 May 2023 23:48:16 GMT
CMD ["bash"]
# Wed, 03 May 2023 22:21:45 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Wed, 03 May 2023 22:21:46 GMT
RUN useradd -s /bin/bash -m docker 	&& usermod -a -G staff docker
# Wed, 03 May 2023 22:22:00 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 22:22:03 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Wed, 03 May 2023 22:22:03 GMT
ENV LC_ALL=en_US.UTF-8
# Wed, 03 May 2023 22:22:03 GMT
ENV LANG=en_US.UTF-8
# Wed, 03 May 2023 22:22:03 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Wed, 03 May 2023 22:22:04 GMT
ENV R_BASE_VERSION=4.3.0
# Wed, 03 May 2023 22:22:04 GMT
RUN echo "deb http://deb.debian.org/debian experimental main" > /etc/apt/sources.list.d/experimental.list     && echo "deb [trusted=yes] https://eddelbuettel.github.io/ppaR400 ./" > /etc/apt/sources.list.d/edd-r4.list
# Wed, 03 May 2023 22:24:00 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-docopt                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& chown root:staff "/usr/local/lib/R/site-library" 	&& chmod g+ws "/usr/local/lib/R/site-library" 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 22:24:02 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:56c7136ddbfad3eea4cd5c38c0703e58fd25630219d5462a9099387c4b3a4160`  
		Last Modified: Tue, 02 May 2023 23:52:53 GMT  
		Size: 49.3 MB (49299248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37fcdcc91a6decc4daaa550a314607547d473fced34fdf8fa11ff5d186a989fe`  
		Last Modified: Wed, 03 May 2023 22:24:15 GMT  
		Size: 3.4 KB (3360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d61cab462a3f50000df4d96522d023f43218662709e10cbadc1c5a3cf8f2fbe`  
		Last Modified: Wed, 03 May 2023 22:24:16 GMT  
		Size: 25.2 MB (25165628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45fc804098ddade4ca07b4a75d441073309e272796dede6c657a0e1ff37e38b2`  
		Last Modified: Wed, 03 May 2023 22:24:13 GMT  
		Size: 865.9 KB (865851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5be6f23be5f8d3623373487b0e2249a630c173aa58bf25d712a714cc66dd6c2c`  
		Last Modified: Wed, 03 May 2023 22:24:13 GMT  
		Size: 348.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31631317ae9296807ef359039e524151b249e5e4cdd9dace5bc1e62f2d7b7f7e`  
		Last Modified: Wed, 03 May 2023 22:24:14 GMT  
		Size: 292.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8cea77e9be3236da8a7eaef187017822ec2b0c0189c6628247c11fdee613877`  
		Last Modified: Wed, 03 May 2023 22:24:42 GMT  
		Size: 261.0 MB (260958713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:latest` - linux; arm64 variant v8

```console
$ docker pull r-base@sha256:91861e8aba13c60c6071d9679c48247cccd86cb8e7ab1ef07e183b94e6b0ead9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **322.5 MB (322487127 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce1761f714141bd97405c4836c52f793b192b238b8c97f7ea3429afb155a32fc`
-	Default Command: `["R"]`

```dockerfile
# Tue, 23 May 2023 00:44:13 GMT
ADD file:f5e81f28718d3bd832678fa284dcfc626b1a1bd4811a8912a05b9fcefd40d358 in / 
# Tue, 23 May 2023 00:44:14 GMT
CMD ["bash"]
# Tue, 23 May 2023 05:34:15 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Tue, 23 May 2023 05:34:16 GMT
RUN useradd -s /bin/bash -m docker 	&& usermod -a -G staff docker
# Tue, 23 May 2023 05:34:29 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 05:34:31 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Tue, 23 May 2023 05:34:31 GMT
ENV LC_ALL=en_US.UTF-8
# Tue, 23 May 2023 05:34:31 GMT
ENV LANG=en_US.UTF-8
# Tue, 23 May 2023 05:34:31 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Tue, 23 May 2023 05:34:31 GMT
ENV R_BASE_VERSION=4.3.0
# Tue, 23 May 2023 05:34:32 GMT
RUN echo "deb http://deb.debian.org/debian experimental main" > /etc/apt/sources.list.d/experimental.list     && echo "deb [trusted=yes] https://eddelbuettel.github.io/ppaR400 ./" > /etc/apt/sources.list.d/edd-r4.list
# Tue, 23 May 2023 05:36:27 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-docopt                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& chown root:staff "/usr/local/lib/R/site-library" 	&& chmod g+ws "/usr/local/lib/R/site-library" 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 05:36:31 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:93ff152152cfe9dc0fb257b029c2b1838408f3bee982bb891d1f5b4212469796`  
		Last Modified: Tue, 23 May 2023 00:48:27 GMT  
		Size: 49.3 MB (49347786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ee3d7f40578e3aa1c72affc9600f568297c4045a6925af45232026d55516685`  
		Last Modified: Tue, 23 May 2023 05:36:45 GMT  
		Size: 3.4 KB (3362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd1c5782d3c65a19f169d1b47f5f545fbe321d58f4226d46ea40087bd90ba305`  
		Last Modified: Tue, 23 May 2023 05:36:45 GMT  
		Size: 25.0 MB (24984469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de35ff8e5bf38bb95030252e0612bdc9df69a5aef2f74674c144066ca81a0dc7`  
		Last Modified: Tue, 23 May 2023 05:36:43 GMT  
		Size: 865.9 KB (865850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0a413c3a535e4ae71fb940eaaa1e480976dfe7126df21fc52439ac1a5955a26`  
		Last Modified: Tue, 23 May 2023 05:36:43 GMT  
		Size: 350.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c45f1c51f6e65f6533a9bfb08620464c7668b632c3f3b581b32e0e8ab8feae0`  
		Last Modified: Tue, 23 May 2023 05:36:43 GMT  
		Size: 295.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a9c686e72fdc6d6894d54302928d7edd14f4af5aaf1c1e0709a78dfaab70d59`  
		Last Modified: Tue, 23 May 2023 05:37:03 GMT  
		Size: 247.3 MB (247285015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:latest` - linux; ppc64le

```console
$ docker pull r-base@sha256:f84334040c57a42c4424a421fc20f673799e4b568f7a1bd74f5028a159bdb127
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **339.1 MB (339086471 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8bedcbbf2eb9328077bfcd8e3efa357ec3cd674f00b27e3d7bd7dffd8d0a88ba`
-	Default Command: `["R"]`

```dockerfile
# Wed, 03 May 2023 00:33:35 GMT
ADD file:f54f5308138566009df9867a9e17d06810cb24a49786ebfdb8f2d83aa44bd004 in / 
# Wed, 03 May 2023 00:33:38 GMT
CMD ["bash"]
# Thu, 04 May 2023 00:52:09 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Thu, 04 May 2023 00:52:11 GMT
RUN useradd -s /bin/bash -m docker 	&& usermod -a -G staff docker
# Thu, 04 May 2023 00:52:37 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Thu, 04 May 2023 00:52:42 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Thu, 04 May 2023 00:52:43 GMT
ENV LC_ALL=en_US.UTF-8
# Thu, 04 May 2023 00:52:43 GMT
ENV LANG=en_US.UTF-8
# Thu, 04 May 2023 00:52:45 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Thu, 04 May 2023 00:52:46 GMT
ENV R_BASE_VERSION=4.3.0
# Thu, 04 May 2023 00:52:48 GMT
RUN echo "deb http://deb.debian.org/debian experimental main" > /etc/apt/sources.list.d/experimental.list     && echo "deb [trusted=yes] https://eddelbuettel.github.io/ppaR400 ./" > /etc/apt/sources.list.d/edd-r4.list
# Thu, 04 May 2023 00:56:26 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-docopt                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& chown root:staff "/usr/local/lib/R/site-library" 	&& chmod g+ws "/usr/local/lib/R/site-library" 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Thu, 04 May 2023 00:56:30 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:c7778701ecf3e4c7947d5854ffadbfcc47a1bea59eeede267cc1563d0c205014`  
		Last Modified: Wed, 03 May 2023 00:38:50 GMT  
		Size: 53.3 MB (53307302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f66bde9f479501a388f0b05d077e44d65524bbba1ee00f0dcbe703bad4534989`  
		Last Modified: Thu, 04 May 2023 00:56:41 GMT  
		Size: 3.4 KB (3358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5e618648d81125407cb42fcf36722736651dd097ba30c339a03bf4e9a8eb480`  
		Last Modified: Thu, 04 May 2023 00:56:43 GMT  
		Size: 25.6 MB (25560947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfe19135c5349f7250145ae537652ad2d7773f5c17b239681c8e8d715b80f179`  
		Last Modified: Thu, 04 May 2023 00:56:39 GMT  
		Size: 865.9 KB (865852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2b0b041784b86a1a06053e7950eaa748db7f632097dae4d8cc8cd14a8f90861`  
		Last Modified: Thu, 04 May 2023 00:56:38 GMT  
		Size: 351.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6e7ee8a60f067de2ef718e7cb15b003582717cfdd918f4c54cd0ceaeac3e4a5`  
		Last Modified: Thu, 04 May 2023 00:56:38 GMT  
		Size: 293.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d31d894101d3b038b49d338d7b2b136e522ad6078faf61b1460f8af4b087e93d`  
		Last Modified: Thu, 04 May 2023 00:57:33 GMT  
		Size: 259.3 MB (259348368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:latest` - linux; s390x

```console
$ docker pull r-base@sha256:7beab94b8d15d4e89924a423f9a921dd85462cd0c3a83593005447dc94f811f0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **297.5 MB (297547859 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89cf3dfb21fa6695f7f5a2f308b669c5260ce6e1a3fc8e95f32eaf6b334be263`
-	Default Command: `["R"]`

```dockerfile
# Tue, 23 May 2023 00:43:47 GMT
ADD file:6dfd7d21cdfe9dee2a7cad47d8e2e22e6e56bd924f036cb45c183fe31efe66cc in / 
# Tue, 23 May 2023 00:43:49 GMT
CMD ["bash"]
# Tue, 23 May 2023 02:28:29 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Tue, 23 May 2023 02:28:29 GMT
RUN useradd -s /bin/bash -m docker 	&& usermod -a -G staff docker
# Tue, 23 May 2023 02:28:36 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 02:28:39 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Tue, 23 May 2023 02:28:39 GMT
ENV LC_ALL=en_US.UTF-8
# Tue, 23 May 2023 02:28:39 GMT
ENV LANG=en_US.UTF-8
# Tue, 23 May 2023 02:28:39 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Tue, 23 May 2023 02:28:39 GMT
ENV R_BASE_VERSION=4.3.0
# Tue, 23 May 2023 02:28:40 GMT
RUN echo "deb http://deb.debian.org/debian experimental main" > /etc/apt/sources.list.d/experimental.list     && echo "deb [trusted=yes] https://eddelbuettel.github.io/ppaR400 ./" > /etc/apt/sources.list.d/edd-r4.list
# Tue, 23 May 2023 02:30:10 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-docopt                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& chown root:staff "/usr/local/lib/R/site-library" 	&& chmod g+ws "/usr/local/lib/R/site-library" 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 02:30:17 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:af4d11b0c6366f32a980344976c0622adf11030b727c114fcc65377cb3f44688`  
		Last Modified: Tue, 23 May 2023 00:46:43 GMT  
		Size: 47.7 MB (47673474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c3ba3a415d79670199ec98260e42e6b72cc5eea4a1ab6c615b4caacf1cafe4c`  
		Last Modified: Tue, 23 May 2023 02:30:38 GMT  
		Size: 3.4 KB (3364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4d6d4d9b862bc7cad32b844052a1006db830fa9c3583c57182e5fa222cf18f9`  
		Last Modified: Tue, 23 May 2023 02:30:40 GMT  
		Size: 24.8 MB (24833563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83952e1da18fa0309b148dc5f654137f85a9f36300cd3f162c4bb15174507944`  
		Last Modified: Tue, 23 May 2023 02:30:37 GMT  
		Size: 921.0 KB (921007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca68baa69c6585bf823bfe9b5d023333f08dc5970cf017131d3645e4476ab2df`  
		Last Modified: Tue, 23 May 2023 02:30:37 GMT  
		Size: 349.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:128fbc66c9a8965d790c4a7a0b54f7805a39755af051c3c2454a02de3dbb1d58`  
		Last Modified: Tue, 23 May 2023 02:30:37 GMT  
		Size: 293.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97acb00df28ae2a5ef9bb1f50c3d0e0c0c9cb2a433ad2176afaa424016685779`  
		Last Modified: Tue, 23 May 2023 02:31:01 GMT  
		Size: 224.1 MB (224115809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
