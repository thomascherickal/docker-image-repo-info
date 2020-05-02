<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `r-base`

-	[`r-base:4.0.0`](#r-base400)
-	[`r-base:latest`](#r-baselatest)

## `r-base:4.0.0`

**does not exist** (yet?)

## `r-base:latest`

```console
$ docker pull r-base@sha256:3a3fb1e083cbd74c4f3ad43c79ed5d7332301dc573b565e47a8c1decef9bdf36
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `r-base:latest` - linux; amd64

```console
$ docker pull r-base@sha256:5e1e1e13aaa8778e219c463a27637957404cc97bd416d4633b4b8cd9e215ff02
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **296.3 MB (296283757 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cec2502269fbb6bc1e0061249d0adf75c6e930f0ef84f062f283ab2a959ed5ab`
-	Default Command: `["R"]`

```dockerfile
# Thu, 23 Apr 2020 00:23:15 GMT
ADD file:19296a07e1c4a35ef4bd6813edc5f8402d5c77ce03f19354ec6b9b7db5286aa5 in / 
# Thu, 23 Apr 2020 00:23:15 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 01:17:07 GMT
LABEL org.label-schema.license=GPL-2.0 org.label-schema.vcs-url=https://github.com/rocker-org/r-base org.label-schema.vendor=Rocker Project maintainer=Dirk Eddelbuettel <edd@debian.org>
# Thu, 23 Apr 2020 01:17:08 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Thu, 23 Apr 2020 01:17:20 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 01:17:23 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Thu, 23 Apr 2020 01:17:23 GMT
ENV LC_ALL=en_US.UTF-8
# Thu, 23 Apr 2020 01:17:23 GMT
ENV LANG=en_US.UTF-8
# Thu, 23 Apr 2020 01:17:24 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default
# Thu, 23 Apr 2020 01:17:24 GMT
ENV R_BASE_VERSION=3.6.3
# Thu, 23 Apr 2020 01:18:14 GMT
RUN apt-get update 	&& apt-get install -t unstable -y --no-install-recommends 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 01:18:14 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:2dffa903b83a05e8f7056f2d8f378ea21af1cbc9a30f68bb9f93f103520963cb`  
		Last Modified: Thu, 23 Apr 2020 00:27:59 GMT  
		Size: 52.0 MB (51981219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10f3fdbe572d99ffe28e8e2b2fc05b92f8f8ed353c8be3704bc05d70e6f72223`  
		Last Modified: Thu, 23 Apr 2020 01:18:27 GMT  
		Size: 1.8 KB (1846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:663fe05835c5456e6e8bbe97c217642ff3d5488ea203ac725254073bf0b22a1d`  
		Last Modified: Thu, 23 Apr 2020 01:18:31 GMT  
		Size: 27.3 MB (27309197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a88b43f1097e6ec036093c7ae85f35a9cf2b5d55493e1a19f382acdaf354b1b`  
		Last Modified: Thu, 23 Apr 2020 01:18:27 GMT  
		Size: 863.4 KB (863380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff9b12da32abe2aa0c79f48998c339c246f525b5e5193b83cb2ecd121212d5cf`  
		Last Modified: Thu, 23 Apr 2020 01:18:27 GMT  
		Size: 298.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd3fedd8743fe066a3f063ffc5fbcf43ed1cba1c34443cd3a1cc28a848713b76`  
		Last Modified: Thu, 23 Apr 2020 01:19:09 GMT  
		Size: 216.1 MB (216127817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:latest` - linux; arm64 variant v8

```console
$ docker pull r-base@sha256:47c03229f5bce098616f12d8d9f3d0eee2cf6295b570e8da6cacd26249309f98
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **286.6 MB (286640480 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1fd869eaf95005ddd41f48bf5931830408a0c39869c95edd33f39e96be92d438`
-	Default Command: `["R"]`

```dockerfile
# Thu, 23 Apr 2020 00:59:29 GMT
ADD file:8d6493850808494b9c8355d7605648137017d4ab385d5f2f709e2b004ae55495 in / 
# Thu, 23 Apr 2020 00:59:37 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 09:11:44 GMT
LABEL org.label-schema.license=GPL-2.0 org.label-schema.vcs-url=https://github.com/rocker-org/r-base org.label-schema.vendor=Rocker Project maintainer=Dirk Eddelbuettel <edd@debian.org>
# Thu, 23 Apr 2020 09:11:48 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Thu, 23 Apr 2020 09:12:34 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 09:12:40 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Thu, 23 Apr 2020 09:12:41 GMT
ENV LC_ALL=en_US.UTF-8
# Thu, 23 Apr 2020 09:12:41 GMT
ENV LANG=en_US.UTF-8
# Thu, 23 Apr 2020 09:12:44 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default
# Thu, 23 Apr 2020 09:12:44 GMT
ENV R_BASE_VERSION=3.6.3
# Thu, 23 Apr 2020 09:14:41 GMT
RUN apt-get update 	&& apt-get install -t unstable -y --no-install-recommends 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 09:14:47 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:9edc88ed1cd036e1398512e49d4ca915c1b089667581f9b64036651a5c5569f8`  
		Last Modified: Thu, 23 Apr 2020 01:06:34 GMT  
		Size: 50.9 MB (50908144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4127a2cf85f285cba8b2c8607b1a93d784fde8c9c4d231b319c9e691a807c4c`  
		Last Modified: Thu, 23 Apr 2020 09:15:07 GMT  
		Size: 1.9 KB (1886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2a10dcfa11c3feca2751726cf7a0b686e0a2f55779703b02a242ed61b498c38`  
		Last Modified: Thu, 23 Apr 2020 09:15:12 GMT  
		Size: 27.2 MB (27176294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1e500848c9067a4f5dbdaf07d4ac207fbc4753e925a3703a201f47e6a6ccc9e`  
		Last Modified: Thu, 23 Apr 2020 09:15:07 GMT  
		Size: 863.4 KB (863390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1feb0b0f0f38635f33ba64df99fc1194fc2561f9152ac1fd07864d9498dd06ab`  
		Last Modified: Thu, 23 Apr 2020 09:15:07 GMT  
		Size: 299.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:908d194086f1b53439bc15f001881e7e91974241220b5714fb707c77b8b9d25c`  
		Last Modified: Thu, 23 Apr 2020 09:15:54 GMT  
		Size: 207.7 MB (207690467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
