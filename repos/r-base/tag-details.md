<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `r-base`

-	[`r-base:4.0.2`](#r-base402)
-	[`r-base:latest`](#r-baselatest)

## `r-base:4.0.2`

```console
$ docker pull r-base@sha256:c057468f17115adc0a0e93fffb871c95ce5f4eccf420803ea43c23bdb3df0aea
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `r-base:4.0.2` - linux; amd64

```console
$ docker pull r-base@sha256:8751b59dc7966aa6c7c355c6b07252aa12f5636c8d5db37fad21fd45624203dd
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **340.9 MB (340906923 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:194fa228510e6d248a25ddcbb2b2b543f611fa70468d3e789c2084eb09bb7a75`
-	Default Command: `["R"]`

```dockerfile
# Tue, 09 Jun 2020 01:23:49 GMT
ADD file:63ef8f38bb25d9c0e944d04e91b6d6c6eb32289709829d3bb80998e94ff2a506 in / 
# Tue, 09 Jun 2020 01:23:49 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 16:53:26 GMT
LABEL org.label-schema.license=GPL-2.0 org.label-schema.vcs-url=https://github.com/rocker-org/r-base org.label-schema.vendor=Rocker Project maintainer=Dirk Eddelbuettel <edd@debian.org>
# Tue, 09 Jun 2020 16:53:26 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Wed, 15 Jul 2020 23:47:34 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		ed 		fonts-texgyre 		less 		locales 		vim-tiny 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 15 Jul 2020 23:47:37 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Wed, 15 Jul 2020 23:47:37 GMT
ENV LC_ALL=en_US.UTF-8
# Wed, 15 Jul 2020 23:47:37 GMT
ENV LANG=en_US.UTF-8
# Wed, 15 Jul 2020 23:47:38 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default
# Wed, 15 Jul 2020 23:47:38 GMT
ENV R_BASE_VERSION=4.0.2
# Wed, 15 Jul 2020 23:48:36 GMT
RUN apt-get update         && apt-get install -t unstable -y --no-install-recommends                 gcc-9-base                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/build.r /usr/local/bin/build.r 	&& ln -s /usr/lib/R/site-library/littler/examples/check.r /usr/local/bin/check.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Wed, 15 Jul 2020 23:48:37 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:0ab9185ddfe50c951de582032c5e29e21a851a328056e6bee6299e0ff55ec807`  
		Last Modified: Tue, 09 Jun 2020 01:28:27 GMT  
		Size: 51.4 MB (51413498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abe522cb8773f50b648207a771978f0815a06186e0161550134a9f1d0de90b7c`  
		Last Modified: Tue, 09 Jun 2020 16:54:45 GMT  
		Size: 1.8 KB (1843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:069212e018184ddd5b74b2137ab23d302e83c725182c1da2955dee62680d3c78`  
		Last Modified: Wed, 15 Jul 2020 23:48:47 GMT  
		Size: 27.3 MB (27340271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db88dffe9e04558a8fb5898d95e78f81df8390947e51fda7a116ef982417a6dc`  
		Last Modified: Wed, 15 Jul 2020 23:48:44 GMT  
		Size: 863.4 KB (863395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15b1afaf74edb234aeae4223811bf0b68bad024d564a6935f22308360db58da1`  
		Last Modified: Wed, 15 Jul 2020 23:48:44 GMT  
		Size: 296.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1deb4ced7b0ad435119b70aa777081647a76588e5b2074f03d3c52adb8cca3f6`  
		Last Modified: Wed, 15 Jul 2020 23:49:19 GMT  
		Size: 261.3 MB (261287620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:4.0.2` - linux; arm64 variant v8

```console
$ docker pull r-base@sha256:956edd2e7edf713f023775e2707025db06556410996d7debb7b9acce1d2304c9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **311.8 MB (311799691 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b9cecb44eeb8e9decfdbd36e89c22bc4f9d1934ff5e8bd863a71bc4cf77e181b`
-	Default Command: `["R"]`

```dockerfile
# Wed, 22 Jul 2020 00:44:29 GMT
ADD file:a9b119b35a33d56fcb58f91ca0224992754db12e0d3b07747c62963bc14659c8 in / 
# Wed, 22 Jul 2020 00:44:32 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 18:19:51 GMT
LABEL org.label-schema.license=GPL-2.0 org.label-schema.vcs-url=https://github.com/rocker-org/r-base org.label-schema.vendor=Rocker Project maintainer=Dirk Eddelbuettel <edd@debian.org>
# Wed, 22 Jul 2020 18:20:06 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Wed, 22 Jul 2020 18:21:26 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		ed 		fonts-texgyre 		less 		locales 		vim-tiny 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 18:21:52 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Wed, 22 Jul 2020 18:22:00 GMT
ENV LC_ALL=en_US.UTF-8
# Wed, 22 Jul 2020 18:22:05 GMT
ENV LANG=en_US.UTF-8
# Wed, 22 Jul 2020 18:22:11 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default
# Wed, 22 Jul 2020 18:22:12 GMT
ENV R_BASE_VERSION=4.0.2
# Wed, 22 Jul 2020 18:24:09 GMT
RUN apt-get update         && apt-get install -t unstable -y --no-install-recommends                 gcc-9-base                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/build.r /usr/local/bin/build.r 	&& ln -s /usr/lib/R/site-library/littler/examples/check.r /usr/local/bin/check.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 18:24:16 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:3bd06a7da77e986d495b6461507cdfdd810e88d105914958d9602ec1c748e59c`  
		Last Modified: Wed, 22 Jul 2020 00:50:38 GMT  
		Size: 52.9 MB (52886390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31fd899cc707d5e31d413ecf9244e96b6df4cd08d368c5a1073357064a989497`  
		Last Modified: Wed, 22 Jul 2020 18:24:28 GMT  
		Size: 1.9 KB (1889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:753a01faf8cb37ede96c30ca8bd066325e7fa69ccecf842cf2949238514d814e`  
		Last Modified: Wed, 22 Jul 2020 18:24:38 GMT  
		Size: 31.8 MB (31810242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93f65e5f40237135eb0dc1ecbca05b0ad9e996547a54645dbf2c1f224e177ee2`  
		Last Modified: Wed, 22 Jul 2020 18:24:28 GMT  
		Size: 863.6 KB (863577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2b461ec2eec3b5affd95277495804497a9d37e03a8561572308599999416d5f`  
		Last Modified: Wed, 22 Jul 2020 18:24:28 GMT  
		Size: 297.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4935880f04a2f54a0851bb9c16a7b44807a6f0238e199a0eac80ab6575eee24`  
		Last Modified: Wed, 22 Jul 2020 18:25:28 GMT  
		Size: 226.2 MB (226237296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:4.0.2` - linux; ppc64le

```console
$ docker pull r-base@sha256:8053db17f111e35f91dc18fa95ed7a9e90d8cf75798367009a2f0ca9c1ba125c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **328.7 MB (328668535 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2050051c720747171cdd515df23ce0d8352c44f3b8d9469f6e2df0407f309b96`
-	Default Command: `["R"]`

```dockerfile
# Wed, 22 Jul 2020 02:18:37 GMT
ADD file:d6f4416408e160284a3c90cab6e53a951dbbc7c1dfa4811f000212296eba31d7 in / 
# Wed, 22 Jul 2020 02:18:43 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 16:36:54 GMT
LABEL org.label-schema.license=GPL-2.0 org.label-schema.vcs-url=https://github.com/rocker-org/r-base org.label-schema.vendor=Rocker Project maintainer=Dirk Eddelbuettel <edd@debian.org>
# Wed, 22 Jul 2020 16:37:04 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Wed, 22 Jul 2020 16:40:06 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		ed 		fonts-texgyre 		less 		locales 		vim-tiny 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 16:40:19 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Wed, 22 Jul 2020 16:40:23 GMT
ENV LC_ALL=en_US.UTF-8
# Wed, 22 Jul 2020 16:40:27 GMT
ENV LANG=en_US.UTF-8
# Wed, 22 Jul 2020 16:40:45 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default
# Wed, 22 Jul 2020 16:40:52 GMT
ENV R_BASE_VERSION=4.0.2
# Wed, 22 Jul 2020 16:49:08 GMT
RUN apt-get update         && apt-get install -t unstable -y --no-install-recommends                 gcc-9-base                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/build.r /usr/local/bin/build.r 	&& ln -s /usr/lib/R/site-library/littler/examples/check.r /usr/local/bin/check.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 16:49:25 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:1e364755122e5010d03f3981d981af0aa16507fb01fdd2c15d80db1a963b580f`  
		Last Modified: Wed, 22 Jul 2020 02:31:33 GMT  
		Size: 58.0 MB (57953376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feef8a33b4b62328cdb97c472c74451134599e5d747e71a852c4a8de0efb9c0d`  
		Last Modified: Wed, 22 Jul 2020 16:49:49 GMT  
		Size: 1.9 KB (1884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf961d0022aa866c60a9f344c7471db43ffc2be326be68fa7dc4485340e0cdcf`  
		Last Modified: Wed, 22 Jul 2020 16:49:54 GMT  
		Size: 33.8 MB (33769704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fbbb5f2890145f505886efac8b220b1bc027cdcc2209919c53965e75af5cd11`  
		Last Modified: Wed, 22 Jul 2020 16:49:49 GMT  
		Size: 863.6 KB (863574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce397ad821652ca80c5024156ab489bb9be2c3c4d44a687d92a5401f890dc8d1`  
		Last Modified: Wed, 22 Jul 2020 16:49:49 GMT  
		Size: 299.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2f5f384a1a66f8977f3f739478739be2d29317f8b4f9435cffa8f241c9c95f0`  
		Last Modified: Wed, 22 Jul 2020 16:50:34 GMT  
		Size: 236.1 MB (236079698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `r-base:latest`

```console
$ docker pull r-base@sha256:c057468f17115adc0a0e93fffb871c95ce5f4eccf420803ea43c23bdb3df0aea
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `r-base:latest` - linux; amd64

```console
$ docker pull r-base@sha256:8751b59dc7966aa6c7c355c6b07252aa12f5636c8d5db37fad21fd45624203dd
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **340.9 MB (340906923 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:194fa228510e6d248a25ddcbb2b2b543f611fa70468d3e789c2084eb09bb7a75`
-	Default Command: `["R"]`

```dockerfile
# Tue, 09 Jun 2020 01:23:49 GMT
ADD file:63ef8f38bb25d9c0e944d04e91b6d6c6eb32289709829d3bb80998e94ff2a506 in / 
# Tue, 09 Jun 2020 01:23:49 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 16:53:26 GMT
LABEL org.label-schema.license=GPL-2.0 org.label-schema.vcs-url=https://github.com/rocker-org/r-base org.label-schema.vendor=Rocker Project maintainer=Dirk Eddelbuettel <edd@debian.org>
# Tue, 09 Jun 2020 16:53:26 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Wed, 15 Jul 2020 23:47:34 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		ed 		fonts-texgyre 		less 		locales 		vim-tiny 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 15 Jul 2020 23:47:37 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Wed, 15 Jul 2020 23:47:37 GMT
ENV LC_ALL=en_US.UTF-8
# Wed, 15 Jul 2020 23:47:37 GMT
ENV LANG=en_US.UTF-8
# Wed, 15 Jul 2020 23:47:38 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default
# Wed, 15 Jul 2020 23:47:38 GMT
ENV R_BASE_VERSION=4.0.2
# Wed, 15 Jul 2020 23:48:36 GMT
RUN apt-get update         && apt-get install -t unstable -y --no-install-recommends                 gcc-9-base                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/build.r /usr/local/bin/build.r 	&& ln -s /usr/lib/R/site-library/littler/examples/check.r /usr/local/bin/check.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Wed, 15 Jul 2020 23:48:37 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:0ab9185ddfe50c951de582032c5e29e21a851a328056e6bee6299e0ff55ec807`  
		Last Modified: Tue, 09 Jun 2020 01:28:27 GMT  
		Size: 51.4 MB (51413498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abe522cb8773f50b648207a771978f0815a06186e0161550134a9f1d0de90b7c`  
		Last Modified: Tue, 09 Jun 2020 16:54:45 GMT  
		Size: 1.8 KB (1843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:069212e018184ddd5b74b2137ab23d302e83c725182c1da2955dee62680d3c78`  
		Last Modified: Wed, 15 Jul 2020 23:48:47 GMT  
		Size: 27.3 MB (27340271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db88dffe9e04558a8fb5898d95e78f81df8390947e51fda7a116ef982417a6dc`  
		Last Modified: Wed, 15 Jul 2020 23:48:44 GMT  
		Size: 863.4 KB (863395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15b1afaf74edb234aeae4223811bf0b68bad024d564a6935f22308360db58da1`  
		Last Modified: Wed, 15 Jul 2020 23:48:44 GMT  
		Size: 296.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1deb4ced7b0ad435119b70aa777081647a76588e5b2074f03d3c52adb8cca3f6`  
		Last Modified: Wed, 15 Jul 2020 23:49:19 GMT  
		Size: 261.3 MB (261287620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:latest` - linux; arm64 variant v8

```console
$ docker pull r-base@sha256:956edd2e7edf713f023775e2707025db06556410996d7debb7b9acce1d2304c9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **311.8 MB (311799691 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b9cecb44eeb8e9decfdbd36e89c22bc4f9d1934ff5e8bd863a71bc4cf77e181b`
-	Default Command: `["R"]`

```dockerfile
# Wed, 22 Jul 2020 00:44:29 GMT
ADD file:a9b119b35a33d56fcb58f91ca0224992754db12e0d3b07747c62963bc14659c8 in / 
# Wed, 22 Jul 2020 00:44:32 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 18:19:51 GMT
LABEL org.label-schema.license=GPL-2.0 org.label-schema.vcs-url=https://github.com/rocker-org/r-base org.label-schema.vendor=Rocker Project maintainer=Dirk Eddelbuettel <edd@debian.org>
# Wed, 22 Jul 2020 18:20:06 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Wed, 22 Jul 2020 18:21:26 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		ed 		fonts-texgyre 		less 		locales 		vim-tiny 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 18:21:52 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Wed, 22 Jul 2020 18:22:00 GMT
ENV LC_ALL=en_US.UTF-8
# Wed, 22 Jul 2020 18:22:05 GMT
ENV LANG=en_US.UTF-8
# Wed, 22 Jul 2020 18:22:11 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default
# Wed, 22 Jul 2020 18:22:12 GMT
ENV R_BASE_VERSION=4.0.2
# Wed, 22 Jul 2020 18:24:09 GMT
RUN apt-get update         && apt-get install -t unstable -y --no-install-recommends                 gcc-9-base                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/build.r /usr/local/bin/build.r 	&& ln -s /usr/lib/R/site-library/littler/examples/check.r /usr/local/bin/check.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 18:24:16 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:3bd06a7da77e986d495b6461507cdfdd810e88d105914958d9602ec1c748e59c`  
		Last Modified: Wed, 22 Jul 2020 00:50:38 GMT  
		Size: 52.9 MB (52886390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31fd899cc707d5e31d413ecf9244e96b6df4cd08d368c5a1073357064a989497`  
		Last Modified: Wed, 22 Jul 2020 18:24:28 GMT  
		Size: 1.9 KB (1889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:753a01faf8cb37ede96c30ca8bd066325e7fa69ccecf842cf2949238514d814e`  
		Last Modified: Wed, 22 Jul 2020 18:24:38 GMT  
		Size: 31.8 MB (31810242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93f65e5f40237135eb0dc1ecbca05b0ad9e996547a54645dbf2c1f224e177ee2`  
		Last Modified: Wed, 22 Jul 2020 18:24:28 GMT  
		Size: 863.6 KB (863577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2b461ec2eec3b5affd95277495804497a9d37e03a8561572308599999416d5f`  
		Last Modified: Wed, 22 Jul 2020 18:24:28 GMT  
		Size: 297.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4935880f04a2f54a0851bb9c16a7b44807a6f0238e199a0eac80ab6575eee24`  
		Last Modified: Wed, 22 Jul 2020 18:25:28 GMT  
		Size: 226.2 MB (226237296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:latest` - linux; ppc64le

```console
$ docker pull r-base@sha256:8053db17f111e35f91dc18fa95ed7a9e90d8cf75798367009a2f0ca9c1ba125c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **328.7 MB (328668535 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2050051c720747171cdd515df23ce0d8352c44f3b8d9469f6e2df0407f309b96`
-	Default Command: `["R"]`

```dockerfile
# Wed, 22 Jul 2020 02:18:37 GMT
ADD file:d6f4416408e160284a3c90cab6e53a951dbbc7c1dfa4811f000212296eba31d7 in / 
# Wed, 22 Jul 2020 02:18:43 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 16:36:54 GMT
LABEL org.label-schema.license=GPL-2.0 org.label-schema.vcs-url=https://github.com/rocker-org/r-base org.label-schema.vendor=Rocker Project maintainer=Dirk Eddelbuettel <edd@debian.org>
# Wed, 22 Jul 2020 16:37:04 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Wed, 22 Jul 2020 16:40:06 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		ed 		fonts-texgyre 		less 		locales 		vim-tiny 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 16:40:19 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Wed, 22 Jul 2020 16:40:23 GMT
ENV LC_ALL=en_US.UTF-8
# Wed, 22 Jul 2020 16:40:27 GMT
ENV LANG=en_US.UTF-8
# Wed, 22 Jul 2020 16:40:45 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default
# Wed, 22 Jul 2020 16:40:52 GMT
ENV R_BASE_VERSION=4.0.2
# Wed, 22 Jul 2020 16:49:08 GMT
RUN apt-get update         && apt-get install -t unstable -y --no-install-recommends                 gcc-9-base                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/build.r /usr/local/bin/build.r 	&& ln -s /usr/lib/R/site-library/littler/examples/check.r /usr/local/bin/check.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 16:49:25 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:1e364755122e5010d03f3981d981af0aa16507fb01fdd2c15d80db1a963b580f`  
		Last Modified: Wed, 22 Jul 2020 02:31:33 GMT  
		Size: 58.0 MB (57953376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feef8a33b4b62328cdb97c472c74451134599e5d747e71a852c4a8de0efb9c0d`  
		Last Modified: Wed, 22 Jul 2020 16:49:49 GMT  
		Size: 1.9 KB (1884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf961d0022aa866c60a9f344c7471db43ffc2be326be68fa7dc4485340e0cdcf`  
		Last Modified: Wed, 22 Jul 2020 16:49:54 GMT  
		Size: 33.8 MB (33769704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fbbb5f2890145f505886efac8b220b1bc027cdcc2209919c53965e75af5cd11`  
		Last Modified: Wed, 22 Jul 2020 16:49:49 GMT  
		Size: 863.6 KB (863574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce397ad821652ca80c5024156ab489bb9be2c3c4d44a687d92a5401f890dc8d1`  
		Last Modified: Wed, 22 Jul 2020 16:49:49 GMT  
		Size: 299.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2f5f384a1a66f8977f3f739478739be2d29317f8b4f9435cffa8f241c9c95f0`  
		Last Modified: Wed, 22 Jul 2020 16:50:34 GMT  
		Size: 236.1 MB (236079698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
