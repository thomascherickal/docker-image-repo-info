<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `r-base`

-	[`r-base:4.1.3`](#r-base413)
-	[`r-base:latest`](#r-baselatest)

## `r-base:4.1.3`

```console
$ docker pull r-base@sha256:8cec4c6690e46547ee54c18998c0c4a96d38c13c15b01dc5aba7c12d26b4881b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `r-base:4.1.3` - linux; amd64

```console
$ docker pull r-base@sha256:f31be416fec8e0ad8092a68861f208275879f601f48fdbf2fb7333a7793b4bb1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **335.0 MB (335013408 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:188c9ab3c80d4777f718205d3b5de1ddf100a563fabb522cac85f3aa8157d8bf`
-	Default Command: `["R"]`

```dockerfile
# Thu, 17 Mar 2022 04:06:58 GMT
ADD file:b73203ff651eb3f27ab9c4a7c28a6755505d1cf75a460d3d0a00e1d77e6efc0e in / 
# Thu, 17 Mar 2022 04:06:59 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 08:52:26 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Fri, 18 Mar 2022 08:52:27 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Fri, 18 Mar 2022 08:52:35 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 08:52:37 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Fri, 18 Mar 2022 08:52:38 GMT
ENV LC_ALL=en_US.UTF-8
# Fri, 18 Mar 2022 08:52:38 GMT
ENV LANG=en_US.UTF-8
# Fri, 18 Mar 2022 08:52:38 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Fri, 18 Mar 2022 08:52:38 GMT
ENV R_BASE_VERSION=4.1.3
# Fri, 18 Mar 2022 08:53:21 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-docopt                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 08:53:23 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:be551d0f976eb440c1b93a9408e36752142151abf4d1a1c0972a21f347227b74`  
		Last Modified: Thu, 17 Mar 2022 04:14:26 GMT  
		Size: 55.8 MB (55754204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eda1b39b8463fd703b41a369812d03ee7e9dc5fe296a9a871ee7b1e38990869b`  
		Last Modified: Fri, 18 Mar 2022 08:53:41 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f45a3f5e9d148539552b985aeb2ddbb6265553c415d20d9415d1c9d8ed696894`  
		Last Modified: Fri, 18 Mar 2022 08:53:44 GMT  
		Size: 25.8 MB (25839518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d324cdf95d4300d9a89af48002fc2f51253bf1ed57888f324e6e6b69f864cf4`  
		Last Modified: Fri, 18 Mar 2022 08:53:41 GMT  
		Size: 864.6 KB (864603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c86e9499b23e80c08ed4e6434bcd79891425f7b1fd6a9440e61103558972ccd6`  
		Last Modified: Fri, 18 Mar 2022 08:53:41 GMT  
		Size: 349.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e9927c4838f24596f01d6e3fa43fc387a42b2a29037073cd8d76fb2e829dd0a`  
		Last Modified: Fri, 18 Mar 2022 08:54:09 GMT  
		Size: 252.6 MB (252552852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:4.1.3` - linux; arm64 variant v8

```console
$ docker pull r-base@sha256:86363c12674f41c1727f09c23f3c7982b19578c96d70ed34fb4f96664f26382c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **324.1 MB (324063831 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c2fa8004fb4624422cd215e17280d0cb6adb7cf8d7024dddfef6d46474359ed`
-	Default Command: `["R"]`

```dockerfile
# Thu, 17 Mar 2022 03:24:27 GMT
ADD file:80ce6b59df4a0234aef0fab1a3d5dce8227ac2503bf797cce72cd3991380b16f in / 
# Thu, 17 Mar 2022 03:24:29 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 00:32:34 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Fri, 18 Mar 2022 00:32:35 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Fri, 18 Mar 2022 00:32:47 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 00:32:50 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Fri, 18 Mar 2022 00:32:51 GMT
ENV LC_ALL=en_US.UTF-8
# Fri, 18 Mar 2022 00:32:52 GMT
ENV LANG=en_US.UTF-8
# Fri, 18 Mar 2022 00:32:53 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Fri, 18 Mar 2022 00:32:54 GMT
ENV R_BASE_VERSION=4.1.3
# Fri, 18 Mar 2022 00:33:53 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-docopt                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 00:33:54 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:a5f8037aec3dd841314901f25fb22b57dab74f5428d97a5eb6b6c1c3f5c189ba`  
		Last Modified: Thu, 17 Mar 2022 03:33:23 GMT  
		Size: 54.7 MB (54667996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:748dcfb3315861e490160ddeef1bdb19cadfd9c15e5716f549aafd1c821f02d0`  
		Last Modified: Fri, 18 Mar 2022 00:34:08 GMT  
		Size: 1.8 KB (1828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b24ce6a6e4de6dacc1335e77ac6fc2991c4d7c010d56fd92d4f536ad9ca7b68`  
		Last Modified: Fri, 18 Mar 2022 00:34:10 GMT  
		Size: 25.8 MB (25830013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0239c8b799c03a41f1252edab9147183ba90267fd0586b4b38f30a9ac4c01ed`  
		Last Modified: Fri, 18 Mar 2022 00:34:08 GMT  
		Size: 864.6 KB (864603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44e0558e27814ffd4af58227aab2c54e05966c24dbfde1326e65722ad7d27c50`  
		Last Modified: Fri, 18 Mar 2022 00:34:07 GMT  
		Size: 348.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd2b0ec4d29f1dd04a2ae3974f500b2e27559e9b6746675266e7db270b44bc9d`  
		Last Modified: Fri, 18 Mar 2022 00:34:36 GMT  
		Size: 242.7 MB (242699043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:4.1.3` - linux; ppc64le

```console
$ docker pull r-base@sha256:e34fd6e773541f667b79501196c3bd942b931709b200abc4bee5979d5134b7b3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **334.1 MB (334063100 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:591d01fb44cb67ea28cccbe383d8e898e1694feb0fbf930f0797071fc0ea5acb`
-	Default Command: `["R"]`

```dockerfile
# Thu, 17 Mar 2022 11:21:57 GMT
ADD file:546d1044d23d29494775e813e460e314ebb95ac4be225652e9fbf8ef7c0494ae in / 
# Thu, 17 Mar 2022 11:22:02 GMT
CMD ["bash"]
# Sat, 19 Mar 2022 07:48:29 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Sat, 19 Mar 2022 07:48:38 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Sat, 19 Mar 2022 07:49:25 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Sat, 19 Mar 2022 07:49:38 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Sat, 19 Mar 2022 07:49:42 GMT
ENV LC_ALL=en_US.UTF-8
# Sat, 19 Mar 2022 07:49:45 GMT
ENV LANG=en_US.UTF-8
# Sat, 19 Mar 2022 07:49:50 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Sat, 19 Mar 2022 07:49:53 GMT
ENV R_BASE_VERSION=4.1.3
# Sat, 19 Mar 2022 07:53:56 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-docopt                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Sat, 19 Mar 2022 07:54:01 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:2d60d151e814979276dae722a0620b58f96f365262f40d49f695e1f5d31d9da9`  
		Last Modified: Thu, 17 Mar 2022 11:32:11 GMT  
		Size: 60.2 MB (60181850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cff9496c30d856333d2ae753f2d800f8323da48aa6bf37098c97f2aa54ca3589`  
		Last Modified: Sat, 19 Mar 2022 07:54:29 GMT  
		Size: 1.9 KB (1889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e01870c0445939b9a2ee58d98c97472daf667c2683168b03bb0fb4c176b4ef7`  
		Last Modified: Sat, 19 Mar 2022 07:54:33 GMT  
		Size: 26.1 MB (26070667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2909ac02ecde7dbba8e109855afd3214c0a6a4844aad0d5b99a4b1f78f0a62a6`  
		Last Modified: Sat, 19 Mar 2022 07:54:29 GMT  
		Size: 864.6 KB (864613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dd6ee2245d877223ad851f7553ca1d67c21ccea2c62475fc712b928ec00e271`  
		Last Modified: Sat, 19 Mar 2022 07:54:29 GMT  
		Size: 351.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52e85f36f47a3fc9a263026a92e1bd88d0a898f5f5384c45ab3e1d78ee2e481c`  
		Last Modified: Sat, 19 Mar 2022 07:55:06 GMT  
		Size: 246.9 MB (246943730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:4.1.3` - linux; s390x

```console
$ docker pull r-base@sha256:9f288e5ee98709119a2e440ee2eeb17b92a51d4f213890ba23a3dc2c25acd2d9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **299.6 MB (299643425 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:561d6e0a8ff4b7d285e7c75d14e89a9570d411a9c2b54dcf38a6f9fdd04c8d3d`
-	Default Command: `["R"]`

```dockerfile
# Thu, 17 Mar 2022 03:09:05 GMT
ADD file:6eb397f5eedde7035cdb2bf9111259ff2e90682463e5019a0378e8a1f429ffee in / 
# Thu, 17 Mar 2022 03:09:09 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 18:14:26 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Thu, 17 Mar 2022 18:14:26 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Thu, 17 Mar 2022 18:14:35 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 18:14:38 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Thu, 17 Mar 2022 18:14:38 GMT
ENV LC_ALL=en_US.UTF-8
# Thu, 17 Mar 2022 18:14:38 GMT
ENV LANG=en_US.UTF-8
# Thu, 17 Mar 2022 18:14:38 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Thu, 17 Mar 2022 18:14:38 GMT
ENV R_BASE_VERSION=4.1.3
# Thu, 17 Mar 2022 18:15:26 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-docopt                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 18:15:34 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:373c0d1a4ca5b7de38c634b77e4e81cc2544d5d8d1dc697e268a5329abbb6fbe`  
		Last Modified: Thu, 17 Mar 2022 03:14:49 GMT  
		Size: 54.0 MB (54000700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2213d77020ddc562ee616141f4d156077487dc36bde0375707711c5bf144f3b`  
		Last Modified: Thu, 17 Mar 2022 18:15:53 GMT  
		Size: 1.9 KB (1880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3b4e7adb01757ef702e1ebd7bcc3215259be79c83459f283fd2d160551cbe49`  
		Last Modified: Thu, 17 Mar 2022 18:15:56 GMT  
		Size: 25.9 MB (25852166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edc2405cdce4b9605f8e7e83eed907de084fe2834698bc6bc7971a7f78ebb1a6`  
		Last Modified: Thu, 17 Mar 2022 18:15:54 GMT  
		Size: 920.2 KB (920184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b805edd27cc52c71d3c65ef4b1d52efa4c80b39e7ed1ec9e1d5d07e5357bace`  
		Last Modified: Thu, 17 Mar 2022 18:15:54 GMT  
		Size: 348.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feafd19216de5f91d125f4ac55f79422798153bb62c02b60756980703c230fc4`  
		Last Modified: Thu, 17 Mar 2022 18:16:16 GMT  
		Size: 218.9 MB (218868147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `r-base:latest`

```console
$ docker pull r-base@sha256:8cec4c6690e46547ee54c18998c0c4a96d38c13c15b01dc5aba7c12d26b4881b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `r-base:latest` - linux; amd64

```console
$ docker pull r-base@sha256:f31be416fec8e0ad8092a68861f208275879f601f48fdbf2fb7333a7793b4bb1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **335.0 MB (335013408 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:188c9ab3c80d4777f718205d3b5de1ddf100a563fabb522cac85f3aa8157d8bf`
-	Default Command: `["R"]`

```dockerfile
# Thu, 17 Mar 2022 04:06:58 GMT
ADD file:b73203ff651eb3f27ab9c4a7c28a6755505d1cf75a460d3d0a00e1d77e6efc0e in / 
# Thu, 17 Mar 2022 04:06:59 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 08:52:26 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Fri, 18 Mar 2022 08:52:27 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Fri, 18 Mar 2022 08:52:35 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 08:52:37 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Fri, 18 Mar 2022 08:52:38 GMT
ENV LC_ALL=en_US.UTF-8
# Fri, 18 Mar 2022 08:52:38 GMT
ENV LANG=en_US.UTF-8
# Fri, 18 Mar 2022 08:52:38 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Fri, 18 Mar 2022 08:52:38 GMT
ENV R_BASE_VERSION=4.1.3
# Fri, 18 Mar 2022 08:53:21 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-docopt                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 08:53:23 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:be551d0f976eb440c1b93a9408e36752142151abf4d1a1c0972a21f347227b74`  
		Last Modified: Thu, 17 Mar 2022 04:14:26 GMT  
		Size: 55.8 MB (55754204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eda1b39b8463fd703b41a369812d03ee7e9dc5fe296a9a871ee7b1e38990869b`  
		Last Modified: Fri, 18 Mar 2022 08:53:41 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f45a3f5e9d148539552b985aeb2ddbb6265553c415d20d9415d1c9d8ed696894`  
		Last Modified: Fri, 18 Mar 2022 08:53:44 GMT  
		Size: 25.8 MB (25839518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d324cdf95d4300d9a89af48002fc2f51253bf1ed57888f324e6e6b69f864cf4`  
		Last Modified: Fri, 18 Mar 2022 08:53:41 GMT  
		Size: 864.6 KB (864603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c86e9499b23e80c08ed4e6434bcd79891425f7b1fd6a9440e61103558972ccd6`  
		Last Modified: Fri, 18 Mar 2022 08:53:41 GMT  
		Size: 349.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e9927c4838f24596f01d6e3fa43fc387a42b2a29037073cd8d76fb2e829dd0a`  
		Last Modified: Fri, 18 Mar 2022 08:54:09 GMT  
		Size: 252.6 MB (252552852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:latest` - linux; arm64 variant v8

```console
$ docker pull r-base@sha256:86363c12674f41c1727f09c23f3c7982b19578c96d70ed34fb4f96664f26382c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **324.1 MB (324063831 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c2fa8004fb4624422cd215e17280d0cb6adb7cf8d7024dddfef6d46474359ed`
-	Default Command: `["R"]`

```dockerfile
# Thu, 17 Mar 2022 03:24:27 GMT
ADD file:80ce6b59df4a0234aef0fab1a3d5dce8227ac2503bf797cce72cd3991380b16f in / 
# Thu, 17 Mar 2022 03:24:29 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 00:32:34 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Fri, 18 Mar 2022 00:32:35 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Fri, 18 Mar 2022 00:32:47 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 00:32:50 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Fri, 18 Mar 2022 00:32:51 GMT
ENV LC_ALL=en_US.UTF-8
# Fri, 18 Mar 2022 00:32:52 GMT
ENV LANG=en_US.UTF-8
# Fri, 18 Mar 2022 00:32:53 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Fri, 18 Mar 2022 00:32:54 GMT
ENV R_BASE_VERSION=4.1.3
# Fri, 18 Mar 2022 00:33:53 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-docopt                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 00:33:54 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:a5f8037aec3dd841314901f25fb22b57dab74f5428d97a5eb6b6c1c3f5c189ba`  
		Last Modified: Thu, 17 Mar 2022 03:33:23 GMT  
		Size: 54.7 MB (54667996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:748dcfb3315861e490160ddeef1bdb19cadfd9c15e5716f549aafd1c821f02d0`  
		Last Modified: Fri, 18 Mar 2022 00:34:08 GMT  
		Size: 1.8 KB (1828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b24ce6a6e4de6dacc1335e77ac6fc2991c4d7c010d56fd92d4f536ad9ca7b68`  
		Last Modified: Fri, 18 Mar 2022 00:34:10 GMT  
		Size: 25.8 MB (25830013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0239c8b799c03a41f1252edab9147183ba90267fd0586b4b38f30a9ac4c01ed`  
		Last Modified: Fri, 18 Mar 2022 00:34:08 GMT  
		Size: 864.6 KB (864603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44e0558e27814ffd4af58227aab2c54e05966c24dbfde1326e65722ad7d27c50`  
		Last Modified: Fri, 18 Mar 2022 00:34:07 GMT  
		Size: 348.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd2b0ec4d29f1dd04a2ae3974f500b2e27559e9b6746675266e7db270b44bc9d`  
		Last Modified: Fri, 18 Mar 2022 00:34:36 GMT  
		Size: 242.7 MB (242699043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:latest` - linux; ppc64le

```console
$ docker pull r-base@sha256:e34fd6e773541f667b79501196c3bd942b931709b200abc4bee5979d5134b7b3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **334.1 MB (334063100 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:591d01fb44cb67ea28cccbe383d8e898e1694feb0fbf930f0797071fc0ea5acb`
-	Default Command: `["R"]`

```dockerfile
# Thu, 17 Mar 2022 11:21:57 GMT
ADD file:546d1044d23d29494775e813e460e314ebb95ac4be225652e9fbf8ef7c0494ae in / 
# Thu, 17 Mar 2022 11:22:02 GMT
CMD ["bash"]
# Sat, 19 Mar 2022 07:48:29 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Sat, 19 Mar 2022 07:48:38 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Sat, 19 Mar 2022 07:49:25 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Sat, 19 Mar 2022 07:49:38 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Sat, 19 Mar 2022 07:49:42 GMT
ENV LC_ALL=en_US.UTF-8
# Sat, 19 Mar 2022 07:49:45 GMT
ENV LANG=en_US.UTF-8
# Sat, 19 Mar 2022 07:49:50 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Sat, 19 Mar 2022 07:49:53 GMT
ENV R_BASE_VERSION=4.1.3
# Sat, 19 Mar 2022 07:53:56 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-docopt                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Sat, 19 Mar 2022 07:54:01 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:2d60d151e814979276dae722a0620b58f96f365262f40d49f695e1f5d31d9da9`  
		Last Modified: Thu, 17 Mar 2022 11:32:11 GMT  
		Size: 60.2 MB (60181850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cff9496c30d856333d2ae753f2d800f8323da48aa6bf37098c97f2aa54ca3589`  
		Last Modified: Sat, 19 Mar 2022 07:54:29 GMT  
		Size: 1.9 KB (1889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e01870c0445939b9a2ee58d98c97472daf667c2683168b03bb0fb4c176b4ef7`  
		Last Modified: Sat, 19 Mar 2022 07:54:33 GMT  
		Size: 26.1 MB (26070667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2909ac02ecde7dbba8e109855afd3214c0a6a4844aad0d5b99a4b1f78f0a62a6`  
		Last Modified: Sat, 19 Mar 2022 07:54:29 GMT  
		Size: 864.6 KB (864613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dd6ee2245d877223ad851f7553ca1d67c21ccea2c62475fc712b928ec00e271`  
		Last Modified: Sat, 19 Mar 2022 07:54:29 GMT  
		Size: 351.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52e85f36f47a3fc9a263026a92e1bd88d0a898f5f5384c45ab3e1d78ee2e481c`  
		Last Modified: Sat, 19 Mar 2022 07:55:06 GMT  
		Size: 246.9 MB (246943730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:latest` - linux; s390x

```console
$ docker pull r-base@sha256:9f288e5ee98709119a2e440ee2eeb17b92a51d4f213890ba23a3dc2c25acd2d9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **299.6 MB (299643425 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:561d6e0a8ff4b7d285e7c75d14e89a9570d411a9c2b54dcf38a6f9fdd04c8d3d`
-	Default Command: `["R"]`

```dockerfile
# Thu, 17 Mar 2022 03:09:05 GMT
ADD file:6eb397f5eedde7035cdb2bf9111259ff2e90682463e5019a0378e8a1f429ffee in / 
# Thu, 17 Mar 2022 03:09:09 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 18:14:26 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Thu, 17 Mar 2022 18:14:26 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Thu, 17 Mar 2022 18:14:35 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 18:14:38 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Thu, 17 Mar 2022 18:14:38 GMT
ENV LC_ALL=en_US.UTF-8
# Thu, 17 Mar 2022 18:14:38 GMT
ENV LANG=en_US.UTF-8
# Thu, 17 Mar 2022 18:14:38 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Thu, 17 Mar 2022 18:14:38 GMT
ENV R_BASE_VERSION=4.1.3
# Thu, 17 Mar 2022 18:15:26 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-docopt                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 18:15:34 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:373c0d1a4ca5b7de38c634b77e4e81cc2544d5d8d1dc697e268a5329abbb6fbe`  
		Last Modified: Thu, 17 Mar 2022 03:14:49 GMT  
		Size: 54.0 MB (54000700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2213d77020ddc562ee616141f4d156077487dc36bde0375707711c5bf144f3b`  
		Last Modified: Thu, 17 Mar 2022 18:15:53 GMT  
		Size: 1.9 KB (1880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3b4e7adb01757ef702e1ebd7bcc3215259be79c83459f283fd2d160551cbe49`  
		Last Modified: Thu, 17 Mar 2022 18:15:56 GMT  
		Size: 25.9 MB (25852166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edc2405cdce4b9605f8e7e83eed907de084fe2834698bc6bc7971a7f78ebb1a6`  
		Last Modified: Thu, 17 Mar 2022 18:15:54 GMT  
		Size: 920.2 KB (920184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b805edd27cc52c71d3c65ef4b1d52efa4c80b39e7ed1ec9e1d5d07e5357bace`  
		Last Modified: Thu, 17 Mar 2022 18:15:54 GMT  
		Size: 348.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feafd19216de5f91d125f4ac55f79422798153bb62c02b60756980703c230fc4`  
		Last Modified: Thu, 17 Mar 2022 18:16:16 GMT  
		Size: 218.9 MB (218868147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
