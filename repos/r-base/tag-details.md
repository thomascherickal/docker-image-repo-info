<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `r-base`

-	[`r-base:4.1.1`](#r-base411)
-	[`r-base:latest`](#r-baselatest)

## `r-base:4.1.1`

```console
$ docker pull r-base@sha256:a76739d794710967a4b4d7123f4397986906d87b2291787646db6fb07c927c8e
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
$ docker pull r-base@sha256:679cf53883c00279b771519f41ca013eab405531ad6165dde18d7dd28735e1cd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **311.2 MB (311213242 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67a98d91c624eb33fa56c2b57145a2388ab2b953ac42f2eb0d348e4e9b99733c`
-	Default Command: `["R"]`

```dockerfile
# Tue, 17 Aug 2021 01:48:44 GMT
ADD file:3893bd6ddc225c2b660af0396860193305baef444ab5aeb369ea28b0679c3a14 in / 
# Tue, 17 Aug 2021 01:48:44 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 11:46:00 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Tue, 17 Aug 2021 11:46:01 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Tue, 17 Aug 2021 11:46:09 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 11:46:12 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Tue, 17 Aug 2021 11:46:12 GMT
ENV LC_ALL=en_US.UTF-8
# Tue, 17 Aug 2021 11:46:13 GMT
ENV LANG=en_US.UTF-8
# Tue, 17 Aug 2021 11:46:13 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Tue, 17 Aug 2021 11:46:13 GMT
ENV R_BASE_VERSION=4.1.1
# Tue, 17 Aug 2021 11:46:14 GMT
RUN echo "deb http://deb.debian.org/debian experimental main" > /etc/apt/sources.list.d/experimental.list     && echo "deb [trusted=yes] https://eddelbuettel.github.io/ppaR400 ./" > /etc/apt/sources.list.d/edd-r4.list
# Tue, 17 Aug 2021 11:46:59 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 11:47:01 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:20341cea39b7b052e8fa46c85b6e6d17dbd3830a13c140eb6d72f4dd6ec5b8e6`  
		Last Modified: Tue, 17 Aug 2021 01:58:25 GMT  
		Size: 53.6 MB (53595238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d037b018b43733167395523bdbb299306664767079cc9a989ef5135870cf8c69`  
		Last Modified: Tue, 17 Aug 2021 11:47:24 GMT  
		Size: 1.9 KB (1878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bb43f2d04b40904a1a96073154eec86259d17631ae2830fdf99353dd152b7e4`  
		Last Modified: Tue, 17 Aug 2021 11:47:25 GMT  
		Size: 25.6 MB (25632791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55477b466c6bed3955a5b74780ade5336a26f29a1dcb64c25770af9c61e4c438`  
		Last Modified: Tue, 17 Aug 2021 11:47:22 GMT  
		Size: 864.6 KB (864593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b41b3fb56558348cd5487cadbfcc1a49eb66d6930e6a2796d4cd74be2b56c45`  
		Last Modified: Tue, 17 Aug 2021 11:47:22 GMT  
		Size: 349.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0da01b3ed82dc66c3ec450a010ee2a05457729da5a15797d6766a93bab5d0152`  
		Last Modified: Tue, 17 Aug 2021 11:47:22 GMT  
		Size: 294.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3071f1c57dd21ec88ee4baec1631678d84306d7a97fe0ee99200fdd75fdc87f1`  
		Last Modified: Tue, 17 Aug 2021 11:47:52 GMT  
		Size: 231.1 MB (231118099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:4.1.1` - linux; ppc64le

```console
$ docker pull r-base@sha256:f9b2f99b1b4bd99c232eb973ac719384c9d9b37c1664f82587320397da366583
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **328.7 MB (328722936 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f0c2947da572eb28cfa944fab76b9f3595d79864885cc23a1fb4054d0966b4d`
-	Default Command: `["R"]`

```dockerfile
# Thu, 22 Jul 2021 00:21:17 GMT
ADD file:609f34b74745c6e0ad3453b3e7043b6aa9a8bd1f08450e5dacc435f2e02cfdc1 in / 
# Thu, 22 Jul 2021 00:21:28 GMT
CMD ["bash"]
# Fri, 23 Jul 2021 00:06:03 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Fri, 23 Jul 2021 00:06:45 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Fri, 23 Jul 2021 00:09:26 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Fri, 23 Jul 2021 00:09:52 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Fri, 23 Jul 2021 00:10:05 GMT
ENV LC_ALL=en_US.UTF-8
# Fri, 23 Jul 2021 00:10:14 GMT
ENV LANG=en_US.UTF-8
# Fri, 23 Jul 2021 00:10:38 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Tue, 10 Aug 2021 21:20:29 GMT
ENV R_BASE_VERSION=4.1.1
# Tue, 10 Aug 2021 21:20:43 GMT
RUN echo "deb http://deb.debian.org/debian experimental main" > /etc/apt/sources.list.d/experimental.list     && echo "deb [trusted=yes] https://eddelbuettel.github.io/ppaR400 ./" > /etc/apt/sources.list.d/edd-r4.list
# Tue, 10 Aug 2021 21:30:56 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Tue, 10 Aug 2021 21:31:02 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:a9effce78a0f7eaff718bcd66572e6000ce0a0c44f2947bbc1908696da72910b`  
		Last Modified: Thu, 22 Jul 2021 00:29:51 GMT  
		Size: 58.8 MB (58813298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00357bf8a668e7e05cde7ec787f1f104c8f855f63110ecc5dac594438e939bf7`  
		Last Modified: Fri, 23 Jul 2021 00:25:17 GMT  
		Size: 1.9 KB (1894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8e79949ae6e203ea970da1b5dfcf5667ed2cc0aebe2352b67598d2783f33749`  
		Last Modified: Fri, 23 Jul 2021 00:25:17 GMT  
		Size: 25.9 MB (25853169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d23b10c241150db5f0fe5cde642895c56b94ff685777d5c13009e5366731f617`  
		Last Modified: Fri, 23 Jul 2021 00:25:14 GMT  
		Size: 864.6 KB (864595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fe8ae5a47eccc707e40c77b69770477b5d8459036f3bbc9ab25ea5c740f8ecc`  
		Last Modified: Fri, 23 Jul 2021 00:25:13 GMT  
		Size: 352.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a43fd2a24008e5302acee98f25a8b8479af11be28f50ceea55bdbef18587c816`  
		Last Modified: Tue, 10 Aug 2021 21:31:21 GMT  
		Size: 296.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fcfb2eddd6b7eee474971037c087a154febcbf605dba0cdd3ea8cb7c2e3399d`  
		Last Modified: Tue, 10 Aug 2021 21:31:57 GMT  
		Size: 243.2 MB (243189332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:4.1.1` - linux; s390x

```console
$ docker pull r-base@sha256:9531e79d85c52e35cd30050cdb5835ed7c61648eb7d992bd051ec8bc56895b88
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.9 MB (289918237 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7a2c2d3b945b5e882cb49c29c854badf43ab362c11acceeb76b098341427bf8`
-	Default Command: `["R"]`

```dockerfile
# Tue, 17 Aug 2021 01:52:42 GMT
ADD file:b26674f4981f5db4384da9469d05dea7bdf6bca5c09c954606849d005794f331 in / 
# Tue, 17 Aug 2021 01:52:50 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 09:55:39 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Tue, 17 Aug 2021 09:55:40 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Tue, 17 Aug 2021 09:55:53 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:55:56 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Tue, 17 Aug 2021 09:55:57 GMT
ENV LC_ALL=en_US.UTF-8
# Tue, 17 Aug 2021 09:55:57 GMT
ENV LANG=en_US.UTF-8
# Tue, 17 Aug 2021 09:55:58 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Tue, 17 Aug 2021 09:55:58 GMT
ENV R_BASE_VERSION=4.1.1
# Tue, 17 Aug 2021 09:55:59 GMT
RUN echo "deb http://deb.debian.org/debian experimental main" > /etc/apt/sources.list.d/experimental.list     && echo "deb [trusted=yes] https://eddelbuettel.github.io/ppaR400 ./" > /etc/apt/sources.list.d/edd-r4.list
# Tue, 17 Aug 2021 09:57:15 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:57:30 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:9cb7e265bbdb4667aca5ec3384874eca1b6494c42d2489f1d0221adfd706bf9b`  
		Last Modified: Tue, 17 Aug 2021 02:00:01 GMT  
		Size: 53.2 MB (53188554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:956e1f8ca2f48c8f49701b3e67f321ce8096e21303628ca69c38bdb960bb6130`  
		Last Modified: Tue, 17 Aug 2021 09:57:53 GMT  
		Size: 1.9 KB (1877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbd5cd8a59c1527cd6e56fe903fdadb4f9a825477ca3b3b4c5d50ce35361b4ab`  
		Last Modified: Tue, 17 Aug 2021 09:57:54 GMT  
		Size: 25.6 MB (25632976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d16c21f4626d3b63a3cee5413eb09bf1b185eec41e31afe34db30c04b0cb12c8`  
		Last Modified: Tue, 17 Aug 2021 09:57:52 GMT  
		Size: 920.2 KB (920157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc5bae5f780c5ac96baa803ccaeed1d34f41df12abf4591dad73db495a9a93fd`  
		Last Modified: Tue, 17 Aug 2021 09:57:51 GMT  
		Size: 347.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ca83f7ac03bd9d33909868795bca8d3ba713387d0344f7673951082674de207`  
		Last Modified: Tue, 17 Aug 2021 09:57:51 GMT  
		Size: 291.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42ab8131b422b49ca4cc8d6215393a725082b279534bd1bbbb3a20880290c4fd`  
		Last Modified: Tue, 17 Aug 2021 09:58:12 GMT  
		Size: 210.2 MB (210174035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `r-base:latest`

```console
$ docker pull r-base@sha256:a76739d794710967a4b4d7123f4397986906d87b2291787646db6fb07c927c8e
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
$ docker pull r-base@sha256:679cf53883c00279b771519f41ca013eab405531ad6165dde18d7dd28735e1cd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **311.2 MB (311213242 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67a98d91c624eb33fa56c2b57145a2388ab2b953ac42f2eb0d348e4e9b99733c`
-	Default Command: `["R"]`

```dockerfile
# Tue, 17 Aug 2021 01:48:44 GMT
ADD file:3893bd6ddc225c2b660af0396860193305baef444ab5aeb369ea28b0679c3a14 in / 
# Tue, 17 Aug 2021 01:48:44 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 11:46:00 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Tue, 17 Aug 2021 11:46:01 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Tue, 17 Aug 2021 11:46:09 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 11:46:12 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Tue, 17 Aug 2021 11:46:12 GMT
ENV LC_ALL=en_US.UTF-8
# Tue, 17 Aug 2021 11:46:13 GMT
ENV LANG=en_US.UTF-8
# Tue, 17 Aug 2021 11:46:13 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Tue, 17 Aug 2021 11:46:13 GMT
ENV R_BASE_VERSION=4.1.1
# Tue, 17 Aug 2021 11:46:14 GMT
RUN echo "deb http://deb.debian.org/debian experimental main" > /etc/apt/sources.list.d/experimental.list     && echo "deb [trusted=yes] https://eddelbuettel.github.io/ppaR400 ./" > /etc/apt/sources.list.d/edd-r4.list
# Tue, 17 Aug 2021 11:46:59 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 11:47:01 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:20341cea39b7b052e8fa46c85b6e6d17dbd3830a13c140eb6d72f4dd6ec5b8e6`  
		Last Modified: Tue, 17 Aug 2021 01:58:25 GMT  
		Size: 53.6 MB (53595238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d037b018b43733167395523bdbb299306664767079cc9a989ef5135870cf8c69`  
		Last Modified: Tue, 17 Aug 2021 11:47:24 GMT  
		Size: 1.9 KB (1878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bb43f2d04b40904a1a96073154eec86259d17631ae2830fdf99353dd152b7e4`  
		Last Modified: Tue, 17 Aug 2021 11:47:25 GMT  
		Size: 25.6 MB (25632791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55477b466c6bed3955a5b74780ade5336a26f29a1dcb64c25770af9c61e4c438`  
		Last Modified: Tue, 17 Aug 2021 11:47:22 GMT  
		Size: 864.6 KB (864593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b41b3fb56558348cd5487cadbfcc1a49eb66d6930e6a2796d4cd74be2b56c45`  
		Last Modified: Tue, 17 Aug 2021 11:47:22 GMT  
		Size: 349.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0da01b3ed82dc66c3ec450a010ee2a05457729da5a15797d6766a93bab5d0152`  
		Last Modified: Tue, 17 Aug 2021 11:47:22 GMT  
		Size: 294.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3071f1c57dd21ec88ee4baec1631678d84306d7a97fe0ee99200fdd75fdc87f1`  
		Last Modified: Tue, 17 Aug 2021 11:47:52 GMT  
		Size: 231.1 MB (231118099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:latest` - linux; ppc64le

```console
$ docker pull r-base@sha256:f9b2f99b1b4bd99c232eb973ac719384c9d9b37c1664f82587320397da366583
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **328.7 MB (328722936 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f0c2947da572eb28cfa944fab76b9f3595d79864885cc23a1fb4054d0966b4d`
-	Default Command: `["R"]`

```dockerfile
# Thu, 22 Jul 2021 00:21:17 GMT
ADD file:609f34b74745c6e0ad3453b3e7043b6aa9a8bd1f08450e5dacc435f2e02cfdc1 in / 
# Thu, 22 Jul 2021 00:21:28 GMT
CMD ["bash"]
# Fri, 23 Jul 2021 00:06:03 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Fri, 23 Jul 2021 00:06:45 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Fri, 23 Jul 2021 00:09:26 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Fri, 23 Jul 2021 00:09:52 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Fri, 23 Jul 2021 00:10:05 GMT
ENV LC_ALL=en_US.UTF-8
# Fri, 23 Jul 2021 00:10:14 GMT
ENV LANG=en_US.UTF-8
# Fri, 23 Jul 2021 00:10:38 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Tue, 10 Aug 2021 21:20:29 GMT
ENV R_BASE_VERSION=4.1.1
# Tue, 10 Aug 2021 21:20:43 GMT
RUN echo "deb http://deb.debian.org/debian experimental main" > /etc/apt/sources.list.d/experimental.list     && echo "deb [trusted=yes] https://eddelbuettel.github.io/ppaR400 ./" > /etc/apt/sources.list.d/edd-r4.list
# Tue, 10 Aug 2021 21:30:56 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Tue, 10 Aug 2021 21:31:02 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:a9effce78a0f7eaff718bcd66572e6000ce0a0c44f2947bbc1908696da72910b`  
		Last Modified: Thu, 22 Jul 2021 00:29:51 GMT  
		Size: 58.8 MB (58813298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00357bf8a668e7e05cde7ec787f1f104c8f855f63110ecc5dac594438e939bf7`  
		Last Modified: Fri, 23 Jul 2021 00:25:17 GMT  
		Size: 1.9 KB (1894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8e79949ae6e203ea970da1b5dfcf5667ed2cc0aebe2352b67598d2783f33749`  
		Last Modified: Fri, 23 Jul 2021 00:25:17 GMT  
		Size: 25.9 MB (25853169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d23b10c241150db5f0fe5cde642895c56b94ff685777d5c13009e5366731f617`  
		Last Modified: Fri, 23 Jul 2021 00:25:14 GMT  
		Size: 864.6 KB (864595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fe8ae5a47eccc707e40c77b69770477b5d8459036f3bbc9ab25ea5c740f8ecc`  
		Last Modified: Fri, 23 Jul 2021 00:25:13 GMT  
		Size: 352.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a43fd2a24008e5302acee98f25a8b8479af11be28f50ceea55bdbef18587c816`  
		Last Modified: Tue, 10 Aug 2021 21:31:21 GMT  
		Size: 296.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fcfb2eddd6b7eee474971037c087a154febcbf605dba0cdd3ea8cb7c2e3399d`  
		Last Modified: Tue, 10 Aug 2021 21:31:57 GMT  
		Size: 243.2 MB (243189332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:latest` - linux; s390x

```console
$ docker pull r-base@sha256:9531e79d85c52e35cd30050cdb5835ed7c61648eb7d992bd051ec8bc56895b88
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.9 MB (289918237 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7a2c2d3b945b5e882cb49c29c854badf43ab362c11acceeb76b098341427bf8`
-	Default Command: `["R"]`

```dockerfile
# Tue, 17 Aug 2021 01:52:42 GMT
ADD file:b26674f4981f5db4384da9469d05dea7bdf6bca5c09c954606849d005794f331 in / 
# Tue, 17 Aug 2021 01:52:50 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 09:55:39 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Tue, 17 Aug 2021 09:55:40 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Tue, 17 Aug 2021 09:55:53 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:55:56 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Tue, 17 Aug 2021 09:55:57 GMT
ENV LC_ALL=en_US.UTF-8
# Tue, 17 Aug 2021 09:55:57 GMT
ENV LANG=en_US.UTF-8
# Tue, 17 Aug 2021 09:55:58 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Tue, 17 Aug 2021 09:55:58 GMT
ENV R_BASE_VERSION=4.1.1
# Tue, 17 Aug 2021 09:55:59 GMT
RUN echo "deb http://deb.debian.org/debian experimental main" > /etc/apt/sources.list.d/experimental.list     && echo "deb [trusted=yes] https://eddelbuettel.github.io/ppaR400 ./" > /etc/apt/sources.list.d/edd-r4.list
# Tue, 17 Aug 2021 09:57:15 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:57:30 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:9cb7e265bbdb4667aca5ec3384874eca1b6494c42d2489f1d0221adfd706bf9b`  
		Last Modified: Tue, 17 Aug 2021 02:00:01 GMT  
		Size: 53.2 MB (53188554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:956e1f8ca2f48c8f49701b3e67f321ce8096e21303628ca69c38bdb960bb6130`  
		Last Modified: Tue, 17 Aug 2021 09:57:53 GMT  
		Size: 1.9 KB (1877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbd5cd8a59c1527cd6e56fe903fdadb4f9a825477ca3b3b4c5d50ce35361b4ab`  
		Last Modified: Tue, 17 Aug 2021 09:57:54 GMT  
		Size: 25.6 MB (25632976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d16c21f4626d3b63a3cee5413eb09bf1b185eec41e31afe34db30c04b0cb12c8`  
		Last Modified: Tue, 17 Aug 2021 09:57:52 GMT  
		Size: 920.2 KB (920157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc5bae5f780c5ac96baa803ccaeed1d34f41df12abf4591dad73db495a9a93fd`  
		Last Modified: Tue, 17 Aug 2021 09:57:51 GMT  
		Size: 347.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ca83f7ac03bd9d33909868795bca8d3ba713387d0344f7673951082674de207`  
		Last Modified: Tue, 17 Aug 2021 09:57:51 GMT  
		Size: 291.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42ab8131b422b49ca4cc8d6215393a725082b279534bd1bbbb3a20880290c4fd`  
		Last Modified: Tue, 17 Aug 2021 09:58:12 GMT  
		Size: 210.2 MB (210174035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
