<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `r-base`

-	[`r-base:4.0.5`](#r-base405)
-	[`r-base:latest`](#r-baselatest)

## `r-base:4.0.5`

```console
$ docker pull r-base@sha256:41d22a7a9dd54150433bdf5d5055877fa64e0fbdff752b6cd826bcf3315f81d5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `r-base:4.0.5` - linux; amd64

```console
$ docker pull r-base@sha256:af1b9007d8c81d0cc3cf8d11eed912537623b08a0bf8697ddba18f091bed64ec
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **323.9 MB (323897200 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f8020514dfa2784462c2ab3d5a1d402ae370067dfd4065c36de0c8ba09ab56b`
-	Default Command: `["R"]`

```dockerfile
# Tue, 30 Mar 2021 21:51:05 GMT
ADD file:43e0ccd9ab01bd6f5c0a9aef5f2ea7c9ee9af30fdf11c8a9c591587a4d089c08 in / 
# Tue, 30 Mar 2021 21:51:06 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 13:59:48 GMT
LABEL org.label-schema.license=GPL-2.0 org.label-schema.vcs-url=https://github.com/rocker-org/r-base org.label-schema.vendor=Rocker Project maintainer=Dirk Eddelbuettel <edd@debian.org>
# Wed, 31 Mar 2021 13:59:50 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Wed, 31 Mar 2021 14:00:07 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 14:00:10 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Wed, 31 Mar 2021 14:00:10 GMT
ENV LC_ALL=en_US.UTF-8
# Wed, 31 Mar 2021 14:00:10 GMT
ENV LANG=en_US.UTF-8
# Wed, 31 Mar 2021 14:00:12 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Fri, 02 Apr 2021 18:38:49 GMT
ENV R_BASE_VERSION=4.0.5
# Fri, 02 Apr 2021 18:38:50 GMT
RUN echo "deb http://deb.debian.org/debian experimental main" > /etc/apt/sources.list.d/experimental.list     && echo "deb [trusted=yes] https://eddelbuettel.github.io/ppaR400 ./" > /etc/apt/sources.list.d/edd-r4.list
# Fri, 02 Apr 2021 18:39:56 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 gcc-9-base                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Fri, 02 Apr 2021 18:39:58 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:225ef05ef5535d13824643cc5f8d3e28d2d9fb76b074b6ec850f2d382becdd39`  
		Last Modified: Tue, 30 Mar 2021 21:57:29 GMT  
		Size: 54.9 MB (54868148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bd07a5385f181125214dab9f13824e95ff6d85e268411e3e8d44aec5b74e3d0`  
		Last Modified: Wed, 31 Mar 2021 14:01:52 GMT  
		Size: 1.9 KB (1877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eebb54f13df4909a223c89a1b2008237b1f18f13314eb9ee909794f43b61173f`  
		Last Modified: Wed, 31 Mar 2021 14:01:59 GMT  
		Size: 25.6 MB (25627788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ddc18d0a329020dbc8130e1377241e6c79fa9f4621595e207cff4bf58313f96`  
		Last Modified: Wed, 31 Mar 2021 14:01:54 GMT  
		Size: 864.6 KB (864592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:758c7a4df06a1983be6c311c6ce5ddd02e39b2f8081f0afbccc15dd748a34690`  
		Last Modified: Wed, 31 Mar 2021 14:01:53 GMT  
		Size: 351.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf4aad63e756385206bdfa2a4730ead3d2ed716f1fd74169adb4c0690080534c`  
		Last Modified: Fri, 02 Apr 2021 18:40:21 GMT  
		Size: 293.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dacc3d4038d7a8e85d8e39f0d96ad8648830ccb99c32e9f62170981433ae0ff2`  
		Last Modified: Fri, 02 Apr 2021 18:41:04 GMT  
		Size: 242.5 MB (242534151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:4.0.5` - linux; arm64 variant v8

```console
$ docker pull r-base@sha256:04ee057922d716542df86dee50448cec991b9e8d875671cecf2e591ec69f89f0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **311.5 MB (311476289 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:917fbf45f92c3a87dee003685ab1979ab729995d6ae9b4fa3dbb917f283bd55a`
-	Default Command: `["R"]`

```dockerfile
# Tue, 30 Mar 2021 21:50:33 GMT
ADD file:f973554eedc62f5f46e9f38329e793a03f86e59390a1556f79308a27e73077cb in / 
# Tue, 30 Mar 2021 21:50:42 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 14:21:36 GMT
LABEL org.label-schema.license=GPL-2.0 org.label-schema.vcs-url=https://github.com/rocker-org/r-base org.label-schema.vendor=Rocker Project maintainer=Dirk Eddelbuettel <edd@debian.org>
# Wed, 31 Mar 2021 14:21:40 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Wed, 31 Mar 2021 14:22:02 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 14:22:11 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Wed, 31 Mar 2021 14:22:12 GMT
ENV LC_ALL=en_US.UTF-8
# Wed, 31 Mar 2021 14:22:13 GMT
ENV LANG=en_US.UTF-8
# Wed, 31 Mar 2021 14:22:15 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Fri, 02 Apr 2021 19:25:14 GMT
ENV R_BASE_VERSION=4.0.5
# Fri, 02 Apr 2021 19:25:17 GMT
RUN echo "deb http://deb.debian.org/debian experimental main" > /etc/apt/sources.list.d/experimental.list     && echo "deb [trusted=yes] https://eddelbuettel.github.io/ppaR400 ./" > /etc/apt/sources.list.d/edd-r4.list
# Fri, 02 Apr 2021 19:27:01 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 gcc-9-base                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Fri, 02 Apr 2021 19:27:06 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:6c5abdff1282a06d2e6071056f94730d9de00eed3f6e167672759eb8fc9eb6e6`  
		Last Modified: Tue, 30 Mar 2021 21:57:31 GMT  
		Size: 53.6 MB (53555204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:206f37d68995d36705e4f0d305852785158e659b5543570040b4fd8117c7ab42`  
		Last Modified: Wed, 31 Mar 2021 14:24:28 GMT  
		Size: 1.9 KB (1878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5932c12088ccba0fa70a51b7e2892bbd1ba7b6c90498dc185fad40b526b96bc3`  
		Last Modified: Wed, 31 Mar 2021 14:24:33 GMT  
		Size: 25.6 MB (25628300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53c6782189f1d92288d4bbfb6c1163badb6c20f80364b69bc80729faca2e0dc3`  
		Last Modified: Wed, 31 Mar 2021 14:24:28 GMT  
		Size: 864.6 KB (864597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aafe8b6bb42f6fc8b04a61c3ad571e686e1ad0f08b6699c19d69d23bc5678846`  
		Last Modified: Wed, 31 Mar 2021 14:24:28 GMT  
		Size: 351.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7deb90318bb05ae2bafb8f5f89905821bbcdfa7e0cd51ef970821d275c5fb6e8`  
		Last Modified: Fri, 02 Apr 2021 19:27:23 GMT  
		Size: 296.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b694158ddafd8f34e2523c4936f239f1bcca716d6ff449c65d1a438b946ccffd`  
		Last Modified: Fri, 02 Apr 2021 19:28:13 GMT  
		Size: 231.4 MB (231425663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:4.0.5` - linux; ppc64le

```console
$ docker pull r-base@sha256:95d0fa7b1456ccbd1a8a210b813fe59b70a713083313a80953746c6d710a2878
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **321.7 MB (321717753 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a03a067e1f4c4a1cf934cf453918a85bc96e7bca346eef202dae379bf18c7135`
-	Default Command: `["R"]`

```dockerfile
# Tue, 30 Mar 2021 22:38:18 GMT
ADD file:edfcf9830c92f6132c01327ed8606a0f69870c393e5c0c7df42b6a56f64ed7d8 in / 
# Tue, 30 Mar 2021 22:38:25 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 16:33:43 GMT
LABEL org.label-schema.license=GPL-2.0 org.label-schema.vcs-url=https://github.com/rocker-org/r-base org.label-schema.vendor=Rocker Project maintainer=Dirk Eddelbuettel <edd@debian.org>
# Wed, 31 Mar 2021 16:33:59 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Wed, 31 Mar 2021 16:35:42 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 16:36:08 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Wed, 31 Mar 2021 16:36:15 GMT
ENV LC_ALL=en_US.UTF-8
# Wed, 31 Mar 2021 16:36:19 GMT
ENV LANG=en_US.UTF-8
# Wed, 31 Mar 2021 16:36:30 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Fri, 02 Apr 2021 18:47:39 GMT
ENV R_BASE_VERSION=4.0.5
# Fri, 02 Apr 2021 18:48:58 GMT
RUN echo "deb http://deb.debian.org/debian experimental main" > /etc/apt/sources.list.d/experimental.list     && echo "deb [trusted=yes] https://eddelbuettel.github.io/ppaR400 ./" > /etc/apt/sources.list.d/edd-r4.list
# Fri, 02 Apr 2021 19:21:12 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 gcc-9-base                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Fri, 02 Apr 2021 19:21:38 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:4f44d41ee258a066a0c0b50b69d17bc36cebed954d5b1b5450cde5e7e38b6adc`  
		Last Modified: Tue, 30 Mar 2021 22:44:44 GMT  
		Size: 58.8 MB (58783345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1167c53c0bfd631e4e48cd0c2d406117f3a5744523b691e6a805bb565b36bfcc`  
		Last Modified: Wed, 31 Mar 2021 16:48:19 GMT  
		Size: 1.9 KB (1889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37b9eccbf4f4bfb7743d559571fe285f192b419219725f7e82d52d0f69ebe4f6`  
		Last Modified: Wed, 31 Mar 2021 16:48:24 GMT  
		Size: 25.9 MB (25850460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7fb9ebcf49646bba04e9867a706faa0e1106d08c81f9cbb33478463e8a26416`  
		Last Modified: Wed, 31 Mar 2021 16:48:20 GMT  
		Size: 864.6 KB (864597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7fea0f6b1edbea02a58a4bc1ced3906453a77dc78ab8394fb0140375d92ca9b`  
		Last Modified: Wed, 31 Mar 2021 16:48:19 GMT  
		Size: 351.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdb9547c29c72e68fff1cda0a3c5edf3367fe7b57cfbf9aec3f04d9a6894fb52`  
		Last Modified: Fri, 02 Apr 2021 19:22:22 GMT  
		Size: 294.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d290a46527a6d907edf0271ad2ea036291dc04cb492591e5a1df471696a128d`  
		Last Modified: Fri, 02 Apr 2021 19:23:07 GMT  
		Size: 236.2 MB (236216817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:4.0.5` - linux; s390x

```console
$ docker pull r-base@sha256:544017496bd01a6b9d6156904e809ec40814cd5d625421de2cfd332ead4cf702
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **290.2 MB (290207311 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d21c702728f58b3c680b21fec71269eab0fbb0048cfb8f05635bb9df031e4d66`
-	Default Command: `["R"]`

```dockerfile
# Tue, 30 Mar 2021 21:43:44 GMT
ADD file:8e1fa69c0f021a22f6b57a9caba4481a9da0cf39f239442db53eb11eacfbb45c in / 
# Tue, 30 Mar 2021 21:43:47 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 02:15:37 GMT
LABEL org.label-schema.license=GPL-2.0 org.label-schema.vcs-url=https://github.com/rocker-org/r-base org.label-schema.vendor=Rocker Project maintainer=Dirk Eddelbuettel <edd@debian.org>
# Wed, 31 Mar 2021 02:15:39 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Wed, 31 Mar 2021 02:15:50 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 02:15:53 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Wed, 31 Mar 2021 02:15:54 GMT
ENV LC_ALL=en_US.UTF-8
# Wed, 31 Mar 2021 02:15:54 GMT
ENV LANG=en_US.UTF-8
# Wed, 31 Mar 2021 02:15:55 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Fri, 02 Apr 2021 18:48:00 GMT
ENV R_BASE_VERSION=4.0.5
# Fri, 02 Apr 2021 18:48:01 GMT
RUN echo "deb http://deb.debian.org/debian experimental main" > /etc/apt/sources.list.d/experimental.list     && echo "deb [trusted=yes] https://eddelbuettel.github.io/ppaR400 ./" > /etc/apt/sources.list.d/edd-r4.list
# Fri, 02 Apr 2021 18:49:16 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 gcc-9-base                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Fri, 02 Apr 2021 18:49:35 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:ca6391c3ba05dc203d2d8e0b8b0b4b2351b46f0ac20ce212409979a3060a7c71`  
		Last Modified: Tue, 30 Mar 2021 21:47:45 GMT  
		Size: 53.1 MB (53148482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:749ce88b09f7367764e7639c47eab569213a01677050d4df02c1ea6909df17b8`  
		Last Modified: Wed, 31 Mar 2021 02:17:46 GMT  
		Size: 1.9 KB (1876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce8ba913a43f80e8e393cd3e31ad5f98e515cbf6b39ca9c2a0b049f8c0c5ec06`  
		Last Modified: Wed, 31 Mar 2021 02:17:49 GMT  
		Size: 25.6 MB (25632738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09e977b3e3c3ec5d5e311ebecc068758159efe7d2d567aa7b5d9a0d3e3186b2f`  
		Last Modified: Wed, 31 Mar 2021 02:17:47 GMT  
		Size: 920.2 KB (920155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c805fcdb14d2e6cf6df0bd8025d91f9d381b0457729e620d366c577689db71f`  
		Last Modified: Wed, 31 Mar 2021 02:17:46 GMT  
		Size: 348.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61ec789f1b83aaf9ef65bd0b6f97c786306fc2d219c156e466ae093bf4d54122`  
		Last Modified: Fri, 02 Apr 2021 18:49:53 GMT  
		Size: 291.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dd214d4f8233671cbbb1285589b9b1635ade670a46981e3f888669ba4364748`  
		Last Modified: Fri, 02 Apr 2021 18:50:17 GMT  
		Size: 210.5 MB (210503421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `r-base:latest`

```console
$ docker pull r-base@sha256:41d22a7a9dd54150433bdf5d5055877fa64e0fbdff752b6cd826bcf3315f81d5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `r-base:latest` - linux; amd64

```console
$ docker pull r-base@sha256:af1b9007d8c81d0cc3cf8d11eed912537623b08a0bf8697ddba18f091bed64ec
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **323.9 MB (323897200 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f8020514dfa2784462c2ab3d5a1d402ae370067dfd4065c36de0c8ba09ab56b`
-	Default Command: `["R"]`

```dockerfile
# Tue, 30 Mar 2021 21:51:05 GMT
ADD file:43e0ccd9ab01bd6f5c0a9aef5f2ea7c9ee9af30fdf11c8a9c591587a4d089c08 in / 
# Tue, 30 Mar 2021 21:51:06 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 13:59:48 GMT
LABEL org.label-schema.license=GPL-2.0 org.label-schema.vcs-url=https://github.com/rocker-org/r-base org.label-schema.vendor=Rocker Project maintainer=Dirk Eddelbuettel <edd@debian.org>
# Wed, 31 Mar 2021 13:59:50 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Wed, 31 Mar 2021 14:00:07 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 14:00:10 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Wed, 31 Mar 2021 14:00:10 GMT
ENV LC_ALL=en_US.UTF-8
# Wed, 31 Mar 2021 14:00:10 GMT
ENV LANG=en_US.UTF-8
# Wed, 31 Mar 2021 14:00:12 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Fri, 02 Apr 2021 18:38:49 GMT
ENV R_BASE_VERSION=4.0.5
# Fri, 02 Apr 2021 18:38:50 GMT
RUN echo "deb http://deb.debian.org/debian experimental main" > /etc/apt/sources.list.d/experimental.list     && echo "deb [trusted=yes] https://eddelbuettel.github.io/ppaR400 ./" > /etc/apt/sources.list.d/edd-r4.list
# Fri, 02 Apr 2021 18:39:56 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 gcc-9-base                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Fri, 02 Apr 2021 18:39:58 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:225ef05ef5535d13824643cc5f8d3e28d2d9fb76b074b6ec850f2d382becdd39`  
		Last Modified: Tue, 30 Mar 2021 21:57:29 GMT  
		Size: 54.9 MB (54868148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bd07a5385f181125214dab9f13824e95ff6d85e268411e3e8d44aec5b74e3d0`  
		Last Modified: Wed, 31 Mar 2021 14:01:52 GMT  
		Size: 1.9 KB (1877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eebb54f13df4909a223c89a1b2008237b1f18f13314eb9ee909794f43b61173f`  
		Last Modified: Wed, 31 Mar 2021 14:01:59 GMT  
		Size: 25.6 MB (25627788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ddc18d0a329020dbc8130e1377241e6c79fa9f4621595e207cff4bf58313f96`  
		Last Modified: Wed, 31 Mar 2021 14:01:54 GMT  
		Size: 864.6 KB (864592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:758c7a4df06a1983be6c311c6ce5ddd02e39b2f8081f0afbccc15dd748a34690`  
		Last Modified: Wed, 31 Mar 2021 14:01:53 GMT  
		Size: 351.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf4aad63e756385206bdfa2a4730ead3d2ed716f1fd74169adb4c0690080534c`  
		Last Modified: Fri, 02 Apr 2021 18:40:21 GMT  
		Size: 293.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dacc3d4038d7a8e85d8e39f0d96ad8648830ccb99c32e9f62170981433ae0ff2`  
		Last Modified: Fri, 02 Apr 2021 18:41:04 GMT  
		Size: 242.5 MB (242534151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:latest` - linux; arm64 variant v8

```console
$ docker pull r-base@sha256:04ee057922d716542df86dee50448cec991b9e8d875671cecf2e591ec69f89f0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **311.5 MB (311476289 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:917fbf45f92c3a87dee003685ab1979ab729995d6ae9b4fa3dbb917f283bd55a`
-	Default Command: `["R"]`

```dockerfile
# Tue, 30 Mar 2021 21:50:33 GMT
ADD file:f973554eedc62f5f46e9f38329e793a03f86e59390a1556f79308a27e73077cb in / 
# Tue, 30 Mar 2021 21:50:42 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 14:21:36 GMT
LABEL org.label-schema.license=GPL-2.0 org.label-schema.vcs-url=https://github.com/rocker-org/r-base org.label-schema.vendor=Rocker Project maintainer=Dirk Eddelbuettel <edd@debian.org>
# Wed, 31 Mar 2021 14:21:40 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Wed, 31 Mar 2021 14:22:02 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 14:22:11 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Wed, 31 Mar 2021 14:22:12 GMT
ENV LC_ALL=en_US.UTF-8
# Wed, 31 Mar 2021 14:22:13 GMT
ENV LANG=en_US.UTF-8
# Wed, 31 Mar 2021 14:22:15 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Fri, 02 Apr 2021 19:25:14 GMT
ENV R_BASE_VERSION=4.0.5
# Fri, 02 Apr 2021 19:25:17 GMT
RUN echo "deb http://deb.debian.org/debian experimental main" > /etc/apt/sources.list.d/experimental.list     && echo "deb [trusted=yes] https://eddelbuettel.github.io/ppaR400 ./" > /etc/apt/sources.list.d/edd-r4.list
# Fri, 02 Apr 2021 19:27:01 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 gcc-9-base                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Fri, 02 Apr 2021 19:27:06 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:6c5abdff1282a06d2e6071056f94730d9de00eed3f6e167672759eb8fc9eb6e6`  
		Last Modified: Tue, 30 Mar 2021 21:57:31 GMT  
		Size: 53.6 MB (53555204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:206f37d68995d36705e4f0d305852785158e659b5543570040b4fd8117c7ab42`  
		Last Modified: Wed, 31 Mar 2021 14:24:28 GMT  
		Size: 1.9 KB (1878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5932c12088ccba0fa70a51b7e2892bbd1ba7b6c90498dc185fad40b526b96bc3`  
		Last Modified: Wed, 31 Mar 2021 14:24:33 GMT  
		Size: 25.6 MB (25628300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53c6782189f1d92288d4bbfb6c1163badb6c20f80364b69bc80729faca2e0dc3`  
		Last Modified: Wed, 31 Mar 2021 14:24:28 GMT  
		Size: 864.6 KB (864597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aafe8b6bb42f6fc8b04a61c3ad571e686e1ad0f08b6699c19d69d23bc5678846`  
		Last Modified: Wed, 31 Mar 2021 14:24:28 GMT  
		Size: 351.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7deb90318bb05ae2bafb8f5f89905821bbcdfa7e0cd51ef970821d275c5fb6e8`  
		Last Modified: Fri, 02 Apr 2021 19:27:23 GMT  
		Size: 296.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b694158ddafd8f34e2523c4936f239f1bcca716d6ff449c65d1a438b946ccffd`  
		Last Modified: Fri, 02 Apr 2021 19:28:13 GMT  
		Size: 231.4 MB (231425663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:latest` - linux; ppc64le

```console
$ docker pull r-base@sha256:95d0fa7b1456ccbd1a8a210b813fe59b70a713083313a80953746c6d710a2878
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **321.7 MB (321717753 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a03a067e1f4c4a1cf934cf453918a85bc96e7bca346eef202dae379bf18c7135`
-	Default Command: `["R"]`

```dockerfile
# Tue, 30 Mar 2021 22:38:18 GMT
ADD file:edfcf9830c92f6132c01327ed8606a0f69870c393e5c0c7df42b6a56f64ed7d8 in / 
# Tue, 30 Mar 2021 22:38:25 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 16:33:43 GMT
LABEL org.label-schema.license=GPL-2.0 org.label-schema.vcs-url=https://github.com/rocker-org/r-base org.label-schema.vendor=Rocker Project maintainer=Dirk Eddelbuettel <edd@debian.org>
# Wed, 31 Mar 2021 16:33:59 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Wed, 31 Mar 2021 16:35:42 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 16:36:08 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Wed, 31 Mar 2021 16:36:15 GMT
ENV LC_ALL=en_US.UTF-8
# Wed, 31 Mar 2021 16:36:19 GMT
ENV LANG=en_US.UTF-8
# Wed, 31 Mar 2021 16:36:30 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Fri, 02 Apr 2021 18:47:39 GMT
ENV R_BASE_VERSION=4.0.5
# Fri, 02 Apr 2021 18:48:58 GMT
RUN echo "deb http://deb.debian.org/debian experimental main" > /etc/apt/sources.list.d/experimental.list     && echo "deb [trusted=yes] https://eddelbuettel.github.io/ppaR400 ./" > /etc/apt/sources.list.d/edd-r4.list
# Fri, 02 Apr 2021 19:21:12 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 gcc-9-base                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Fri, 02 Apr 2021 19:21:38 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:4f44d41ee258a066a0c0b50b69d17bc36cebed954d5b1b5450cde5e7e38b6adc`  
		Last Modified: Tue, 30 Mar 2021 22:44:44 GMT  
		Size: 58.8 MB (58783345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1167c53c0bfd631e4e48cd0c2d406117f3a5744523b691e6a805bb565b36bfcc`  
		Last Modified: Wed, 31 Mar 2021 16:48:19 GMT  
		Size: 1.9 KB (1889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37b9eccbf4f4bfb7743d559571fe285f192b419219725f7e82d52d0f69ebe4f6`  
		Last Modified: Wed, 31 Mar 2021 16:48:24 GMT  
		Size: 25.9 MB (25850460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7fb9ebcf49646bba04e9867a706faa0e1106d08c81f9cbb33478463e8a26416`  
		Last Modified: Wed, 31 Mar 2021 16:48:20 GMT  
		Size: 864.6 KB (864597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7fea0f6b1edbea02a58a4bc1ced3906453a77dc78ab8394fb0140375d92ca9b`  
		Last Modified: Wed, 31 Mar 2021 16:48:19 GMT  
		Size: 351.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdb9547c29c72e68fff1cda0a3c5edf3367fe7b57cfbf9aec3f04d9a6894fb52`  
		Last Modified: Fri, 02 Apr 2021 19:22:22 GMT  
		Size: 294.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d290a46527a6d907edf0271ad2ea036291dc04cb492591e5a1df471696a128d`  
		Last Modified: Fri, 02 Apr 2021 19:23:07 GMT  
		Size: 236.2 MB (236216817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:latest` - linux; s390x

```console
$ docker pull r-base@sha256:544017496bd01a6b9d6156904e809ec40814cd5d625421de2cfd332ead4cf702
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **290.2 MB (290207311 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d21c702728f58b3c680b21fec71269eab0fbb0048cfb8f05635bb9df031e4d66`
-	Default Command: `["R"]`

```dockerfile
# Tue, 30 Mar 2021 21:43:44 GMT
ADD file:8e1fa69c0f021a22f6b57a9caba4481a9da0cf39f239442db53eb11eacfbb45c in / 
# Tue, 30 Mar 2021 21:43:47 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 02:15:37 GMT
LABEL org.label-schema.license=GPL-2.0 org.label-schema.vcs-url=https://github.com/rocker-org/r-base org.label-schema.vendor=Rocker Project maintainer=Dirk Eddelbuettel <edd@debian.org>
# Wed, 31 Mar 2021 02:15:39 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Wed, 31 Mar 2021 02:15:50 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 02:15:53 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Wed, 31 Mar 2021 02:15:54 GMT
ENV LC_ALL=en_US.UTF-8
# Wed, 31 Mar 2021 02:15:54 GMT
ENV LANG=en_US.UTF-8
# Wed, 31 Mar 2021 02:15:55 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Fri, 02 Apr 2021 18:48:00 GMT
ENV R_BASE_VERSION=4.0.5
# Fri, 02 Apr 2021 18:48:01 GMT
RUN echo "deb http://deb.debian.org/debian experimental main" > /etc/apt/sources.list.d/experimental.list     && echo "deb [trusted=yes] https://eddelbuettel.github.io/ppaR400 ./" > /etc/apt/sources.list.d/edd-r4.list
# Fri, 02 Apr 2021 18:49:16 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 gcc-9-base                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Fri, 02 Apr 2021 18:49:35 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:ca6391c3ba05dc203d2d8e0b8b0b4b2351b46f0ac20ce212409979a3060a7c71`  
		Last Modified: Tue, 30 Mar 2021 21:47:45 GMT  
		Size: 53.1 MB (53148482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:749ce88b09f7367764e7639c47eab569213a01677050d4df02c1ea6909df17b8`  
		Last Modified: Wed, 31 Mar 2021 02:17:46 GMT  
		Size: 1.9 KB (1876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce8ba913a43f80e8e393cd3e31ad5f98e515cbf6b39ca9c2a0b049f8c0c5ec06`  
		Last Modified: Wed, 31 Mar 2021 02:17:49 GMT  
		Size: 25.6 MB (25632738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09e977b3e3c3ec5d5e311ebecc068758159efe7d2d567aa7b5d9a0d3e3186b2f`  
		Last Modified: Wed, 31 Mar 2021 02:17:47 GMT  
		Size: 920.2 KB (920155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c805fcdb14d2e6cf6df0bd8025d91f9d381b0457729e620d366c577689db71f`  
		Last Modified: Wed, 31 Mar 2021 02:17:46 GMT  
		Size: 348.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61ec789f1b83aaf9ef65bd0b6f97c786306fc2d219c156e466ae093bf4d54122`  
		Last Modified: Fri, 02 Apr 2021 18:49:53 GMT  
		Size: 291.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dd214d4f8233671cbbb1285589b9b1635ade670a46981e3f888669ba4364748`  
		Last Modified: Fri, 02 Apr 2021 18:50:17 GMT  
		Size: 210.5 MB (210503421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
