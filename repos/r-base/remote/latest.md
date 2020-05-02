## `r-base:latest`

```console
$ docker pull r-base@sha256:004edd4e02d913d7163ee32a3afc506769a73db4da76f62e22cad302da429a32
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `r-base:latest` - linux; amd64

```console
$ docker pull r-base@sha256:de8a79168b303ffa816ea8414e0487e6fc73dceb96470bdb06b5316b12ffe664
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **327.9 MB (327916846 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5bfe2234bf4a4cd4a2181d65f3c9c73bd96a5dd776917d9e17b124888b763e3`
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
# Sat, 02 May 2020 01:36:43 GMT
ENV R_BASE_VERSION=4.0.0
# Sat, 02 May 2020 01:36:44 GMT
RUN echo "deb http://deb.debian.org/debian experimental main" > /etc/apt/sources.list.d/experimental.list     && echo "deb [trusted=yes] https://eddelbuettel.github.io/ppaR400 ./" > /etc/apt/sources.list.d/edd-r4.list     && rm /etc/apt/apt.conf.d/default
# Sat, 02 May 2020 01:37:40 GMT
RUN apt-get update 	&& apt-get install -t experimental -y --no-install-recommends 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Sat, 02 May 2020 01:37:41 GMT
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
	-	`sha256:be75024a75f77e145abd3fd3a2ba45ec0fc1d5b5033478d483c3933f77fed8a9`  
		Last Modified: Sat, 02 May 2020 01:37:50 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:562371e1464be08981e9d62a69d6ec891cd374501f8b9434eca22f3ff78124aa`  
		Last Modified: Sat, 02 May 2020 01:38:38 GMT  
		Size: 247.8 MB (247760567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
