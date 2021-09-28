<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `r-base`

-	[`r-base:4.1.1`](#r-base411)
-	[`r-base:latest`](#r-baselatest)

## `r-base:4.1.1`

```console
$ docker pull r-base@sha256:814e413e570311f83999431f91ff4d6134b2d22dd19450265a36edaae9020295
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `r-base:4.1.1` - linux; amd64

```console
$ docker pull r-base@sha256:8da10a720b26d6b6c2d32cb743f90cb9bf54f4b536e471c3da23342510380fb7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **324.3 MB (324307880 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:176db8b917ff130dca4fa65bd1bc571e450cde8c2f5d71bf130394ca5579019f`
-	Default Command: `["R"]`

```dockerfile
# Fri, 03 Sep 2021 01:23:58 GMT
ADD file:34bf1f6ddafae4895f45a110a2d7ea6139557d82a9508b85d7518a54be80aa91 in / 
# Fri, 03 Sep 2021 01:23:59 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 13:34:39 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Fri, 03 Sep 2021 13:34:41 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Fri, 03 Sep 2021 13:35:03 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 13:35:07 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Fri, 03 Sep 2021 13:35:07 GMT
ENV LC_ALL=en_US.UTF-8
# Fri, 03 Sep 2021 13:35:07 GMT
ENV LANG=en_US.UTF-8
# Fri, 03 Sep 2021 13:35:08 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Fri, 03 Sep 2021 13:35:08 GMT
ENV R_BASE_VERSION=4.1.1
# Fri, 03 Sep 2021 13:35:09 GMT
RUN echo "deb http://deb.debian.org/debian experimental main" > /etc/apt/sources.list.d/experimental.list     && echo "deb [trusted=yes] https://eddelbuettel.github.io/ppaR400 ./" > /etc/apt/sources.list.d/edd-r4.list
# Fri, 03 Sep 2021 13:36:12 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 13:36:14 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:931337f74a7f142aabe368b4eb63c0e810923f0f0d4f6f018794c6213a4c07ca`  
		Last Modified: Fri, 03 Sep 2021 01:32:30 GMT  
		Size: 55.5 MB (55464641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6757576bd2e192afd6cf59dbdc918b17943ad406c681366ad3317bca84e5e2e`  
		Last Modified: Fri, 03 Sep 2021 13:36:28 GMT  
		Size: 1.9 KB (1873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8202d4b1ddd23c53d9e4245804e40b5a8e73163b20181e9cf2c02f27bb5b6f7`  
		Last Modified: Fri, 03 Sep 2021 13:36:32 GMT  
		Size: 25.6 MB (25639660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1083f8a27132de38911b25dbe58bc8a16b67fa9ee241a5a9cba37efaeccbad12`  
		Last Modified: Fri, 03 Sep 2021 13:36:26 GMT  
		Size: 864.6 KB (864587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd9b19473be7a57899c83282fb42b7a718d4f99a3f9bbe013998a8cd83751ab9`  
		Last Modified: Fri, 03 Sep 2021 13:36:27 GMT  
		Size: 350.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b650082ab77a5d9f391d6f1e1f49c6eb8d6649be477818b2b69df976bd82c8aa`  
		Last Modified: Fri, 03 Sep 2021 13:36:26 GMT  
		Size: 294.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7ef86dac7405f9734937ffde56147822f89f22b950bcff00a87c8493c3244a8`  
		Last Modified: Fri, 03 Sep 2021 13:37:08 GMT  
		Size: 242.3 MB (242336475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:4.1.1` - linux; arm64 variant v8

```console
$ docker pull r-base@sha256:7ff20f200fd93a183172cc5d93507905616716761ece241ce7bdc6c58053badf
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **315.2 MB (315169992 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43004d0e92e411698b6433ac491de990ab6dac85081ecfffbefd47ddf753744b`
-	Default Command: `["R"]`

```dockerfile
# Tue, 28 Sep 2021 01:43:39 GMT
ADD file:df28df42dbd83dc9e69cbc59efab23a55fd0a6252480edbc355435be4e55acf0 in / 
# Tue, 28 Sep 2021 01:43:40 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 15:49:32 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Tue, 28 Sep 2021 15:49:33 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Tue, 28 Sep 2021 15:49:42 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 15:49:45 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Tue, 28 Sep 2021 15:49:45 GMT
ENV LC_ALL=en_US.UTF-8
# Tue, 28 Sep 2021 15:49:45 GMT
ENV LANG=en_US.UTF-8
# Tue, 28 Sep 2021 15:49:46 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Tue, 28 Sep 2021 15:49:46 GMT
ENV R_BASE_VERSION=4.1.1
# Tue, 28 Sep 2021 15:49:47 GMT
RUN echo "deb http://deb.debian.org/debian experimental main" > /etc/apt/sources.list.d/experimental.list     && echo "deb [trusted=yes] https://eddelbuettel.github.io/ppaR400 ./" > /etc/apt/sources.list.d/edd-r4.list
# Tue, 28 Sep 2021 15:50:37 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 15:50:39 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:5fd04373f6dc4ec57b4af01b70782245fdb26a426888b8d0fe9169590ef679b7`  
		Last Modified: Tue, 28 Sep 2021 01:53:17 GMT  
		Size: 54.5 MB (54460337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e418464f49f41ba43443d77e90ee257ef0a60fe422389cdafa9171100bc6f12`  
		Last Modified: Tue, 28 Sep 2021 15:50:55 GMT  
		Size: 1.9 KB (1876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eda43c359b84724a6c7d59c423387ac97b8239a3baaf96b2ad044d38da7a7690`  
		Last Modified: Tue, 28 Sep 2021 15:50:56 GMT  
		Size: 25.6 MB (25578065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e5391d63d29be63b22f7c888d0bb3e63b310b48bdfdef14c73b0d51e306fcbf`  
		Last Modified: Tue, 28 Sep 2021 15:50:53 GMT  
		Size: 864.6 KB (864613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd4ad37830882347e1b2d1d2239d283be294c35899483487b278ea18e5cf8e86`  
		Last Modified: Tue, 28 Sep 2021 15:50:53 GMT  
		Size: 348.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebba437b4f1d5d81167585c32a6dbab9cebda1f1d2bae7ac44600c4fcfd74e6c`  
		Last Modified: Tue, 28 Sep 2021 15:50:53 GMT  
		Size: 292.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54c9f61c3faaebe463cb4b6be3f6204e78a5639450d8a2380ce64fc8fac2da5e`  
		Last Modified: Tue, 28 Sep 2021 15:51:22 GMT  
		Size: 234.3 MB (234264461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:4.1.1` - linux; ppc64le

```console
$ docker pull r-base@sha256:617559accc990c254a4ff30d43605d99c4de2a770191715667cc25a57b00fa57
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **322.6 MB (322579703 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd4059f6fd409984d90ddd1fce6ac7dc0049dc269105b326db7ab06dc42796d6`
-	Default Command: `["R"]`

```dockerfile
# Fri, 03 Sep 2021 01:28:03 GMT
ADD file:3c352e1c5b975bab6ba80213fc86e0b5836f9976e755be58fccd6f003941ca8b in / 
# Fri, 03 Sep 2021 01:28:12 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 18:07:19 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Fri, 03 Sep 2021 18:07:40 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Fri, 03 Sep 2021 18:08:48 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 18:09:03 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Fri, 03 Sep 2021 18:09:10 GMT
ENV LC_ALL=en_US.UTF-8
# Fri, 03 Sep 2021 18:09:15 GMT
ENV LANG=en_US.UTF-8
# Fri, 03 Sep 2021 18:09:24 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Fri, 03 Sep 2021 18:09:28 GMT
ENV R_BASE_VERSION=4.1.1
# Fri, 03 Sep 2021 18:09:43 GMT
RUN echo "deb http://deb.debian.org/debian experimental main" > /etc/apt/sources.list.d/experimental.list     && echo "deb [trusted=yes] https://eddelbuettel.github.io/ppaR400 ./" > /etc/apt/sources.list.d/edd-r4.list
# Fri, 03 Sep 2021 18:16:58 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 18:17:21 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:61eff2bf557a409d063c940d589dc8f98bf037655ffc94d8e30b546974554826`  
		Last Modified: Fri, 03 Sep 2021 01:47:00 GMT  
		Size: 59.5 MB (59526125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce611fbe8ab05ce2c89df4861eda9fa9a9ac574620f25260b3392fc1dbf77770`  
		Last Modified: Fri, 03 Sep 2021 18:17:44 GMT  
		Size: 1.9 KB (1897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07ebd15523833a8c3199a65b13cc3cf32a3c2519b0ffc145fe94c832b7ad527d`  
		Last Modified: Fri, 03 Sep 2021 18:17:44 GMT  
		Size: 25.8 MB (25847783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7784100ddcd38691f40bcbff901986458cd1db182a9f421257bc99102bae1a50`  
		Last Modified: Fri, 03 Sep 2021 18:17:40 GMT  
		Size: 864.6 KB (864587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00e932154d909477bfe626a1240d5f45735b0e128fdbf67a9a8f91ebdecb3772`  
		Last Modified: Fri, 03 Sep 2021 18:17:40 GMT  
		Size: 351.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85ce1c57788b3101614032507e56e512abe5141f74980255a57f6d2867a8c194`  
		Last Modified: Fri, 03 Sep 2021 18:17:40 GMT  
		Size: 294.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac7ca859214f67b7844bed90bf073802c0fa78e0e2a27926fdc9a4ac983d64d6`  
		Last Modified: Fri, 03 Sep 2021 18:22:34 GMT  
		Size: 236.3 MB (236338666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:4.1.1` - linux; s390x

```console
$ docker pull r-base@sha256:f20bfa8c68f388f3f6e71d98f6ac9ad932098ca2a34c570356029c33a294836e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **290.9 MB (290927543 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:968c5937c5239367ba52cd6cc597c904864dc5e0d347455bda95c928db3edd85`
-	Default Command: `["R"]`

```dockerfile
# Tue, 28 Sep 2021 01:45:08 GMT
ADD file:094728d97cbb14c94edb377e3d4dede62bd88e82f98ecd93bba64aebc4e7916a in / 
# Tue, 28 Sep 2021 01:45:10 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 07:23:40 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Tue, 28 Sep 2021 07:23:40 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Tue, 28 Sep 2021 07:23:49 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 07:23:51 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Tue, 28 Sep 2021 07:23:52 GMT
ENV LC_ALL=en_US.UTF-8
# Tue, 28 Sep 2021 07:23:52 GMT
ENV LANG=en_US.UTF-8
# Tue, 28 Sep 2021 07:23:52 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Tue, 28 Sep 2021 07:23:52 GMT
ENV R_BASE_VERSION=4.1.1
# Tue, 28 Sep 2021 07:23:53 GMT
RUN echo "deb http://deb.debian.org/debian experimental main" > /etc/apt/sources.list.d/experimental.list     && echo "deb [trusted=yes] https://eddelbuettel.github.io/ppaR400 ./" > /etc/apt/sources.list.d/edd-r4.list
# Tue, 28 Sep 2021 07:24:42 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 07:24:50 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:93e4733dccf8c066cccad1642f393ff63777ee8c1262cdbc961912a70203c3cb`  
		Last Modified: Tue, 28 Sep 2021 01:51:12 GMT  
		Size: 53.7 MB (53691013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a395ea0887cd48211810e3375f5b786c91bcec52da80d50b3b7c87c36ad379a`  
		Last Modified: Tue, 28 Sep 2021 07:25:07 GMT  
		Size: 1.9 KB (1876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fb981f9996bf74c927220cb62ca23a0f538a4852ceae9675b6269f3dd0664ed`  
		Last Modified: Tue, 28 Sep 2021 07:25:08 GMT  
		Size: 25.6 MB (25588352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6bfc1ca3ad281ed1acbb966e7df4c0bc7441e54d5e14d25c125ed8bdbb88266`  
		Last Modified: Tue, 28 Sep 2021 07:25:06 GMT  
		Size: 920.2 KB (920188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12174ad516d3a507e2f9681a62dfa0d98dbeee9645fc4641b005b5e32cfa05f3`  
		Last Modified: Tue, 28 Sep 2021 07:25:06 GMT  
		Size: 347.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61fe3e1e7a058b2f5343180fe46f90f388d774c223bf3b8fbbc73f058e19e763`  
		Last Modified: Tue, 28 Sep 2021 07:25:06 GMT  
		Size: 292.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f286a00e3bd2e1971e090ef242c822b502df8bcf652d44b60981902b72d62d52`  
		Last Modified: Tue, 28 Sep 2021 07:25:26 GMT  
		Size: 210.7 MB (210725475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `r-base:latest`

```console
$ docker pull r-base@sha256:814e413e570311f83999431f91ff4d6134b2d22dd19450265a36edaae9020295
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `r-base:latest` - linux; amd64

```console
$ docker pull r-base@sha256:8da10a720b26d6b6c2d32cb743f90cb9bf54f4b536e471c3da23342510380fb7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **324.3 MB (324307880 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:176db8b917ff130dca4fa65bd1bc571e450cde8c2f5d71bf130394ca5579019f`
-	Default Command: `["R"]`

```dockerfile
# Fri, 03 Sep 2021 01:23:58 GMT
ADD file:34bf1f6ddafae4895f45a110a2d7ea6139557d82a9508b85d7518a54be80aa91 in / 
# Fri, 03 Sep 2021 01:23:59 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 13:34:39 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Fri, 03 Sep 2021 13:34:41 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Fri, 03 Sep 2021 13:35:03 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 13:35:07 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Fri, 03 Sep 2021 13:35:07 GMT
ENV LC_ALL=en_US.UTF-8
# Fri, 03 Sep 2021 13:35:07 GMT
ENV LANG=en_US.UTF-8
# Fri, 03 Sep 2021 13:35:08 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Fri, 03 Sep 2021 13:35:08 GMT
ENV R_BASE_VERSION=4.1.1
# Fri, 03 Sep 2021 13:35:09 GMT
RUN echo "deb http://deb.debian.org/debian experimental main" > /etc/apt/sources.list.d/experimental.list     && echo "deb [trusted=yes] https://eddelbuettel.github.io/ppaR400 ./" > /etc/apt/sources.list.d/edd-r4.list
# Fri, 03 Sep 2021 13:36:12 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 13:36:14 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:931337f74a7f142aabe368b4eb63c0e810923f0f0d4f6f018794c6213a4c07ca`  
		Last Modified: Fri, 03 Sep 2021 01:32:30 GMT  
		Size: 55.5 MB (55464641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6757576bd2e192afd6cf59dbdc918b17943ad406c681366ad3317bca84e5e2e`  
		Last Modified: Fri, 03 Sep 2021 13:36:28 GMT  
		Size: 1.9 KB (1873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8202d4b1ddd23c53d9e4245804e40b5a8e73163b20181e9cf2c02f27bb5b6f7`  
		Last Modified: Fri, 03 Sep 2021 13:36:32 GMT  
		Size: 25.6 MB (25639660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1083f8a27132de38911b25dbe58bc8a16b67fa9ee241a5a9cba37efaeccbad12`  
		Last Modified: Fri, 03 Sep 2021 13:36:26 GMT  
		Size: 864.6 KB (864587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd9b19473be7a57899c83282fb42b7a718d4f99a3f9bbe013998a8cd83751ab9`  
		Last Modified: Fri, 03 Sep 2021 13:36:27 GMT  
		Size: 350.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b650082ab77a5d9f391d6f1e1f49c6eb8d6649be477818b2b69df976bd82c8aa`  
		Last Modified: Fri, 03 Sep 2021 13:36:26 GMT  
		Size: 294.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7ef86dac7405f9734937ffde56147822f89f22b950bcff00a87c8493c3244a8`  
		Last Modified: Fri, 03 Sep 2021 13:37:08 GMT  
		Size: 242.3 MB (242336475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:latest` - linux; arm64 variant v8

```console
$ docker pull r-base@sha256:7ff20f200fd93a183172cc5d93507905616716761ece241ce7bdc6c58053badf
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **315.2 MB (315169992 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43004d0e92e411698b6433ac491de990ab6dac85081ecfffbefd47ddf753744b`
-	Default Command: `["R"]`

```dockerfile
# Tue, 28 Sep 2021 01:43:39 GMT
ADD file:df28df42dbd83dc9e69cbc59efab23a55fd0a6252480edbc355435be4e55acf0 in / 
# Tue, 28 Sep 2021 01:43:40 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 15:49:32 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Tue, 28 Sep 2021 15:49:33 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Tue, 28 Sep 2021 15:49:42 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 15:49:45 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Tue, 28 Sep 2021 15:49:45 GMT
ENV LC_ALL=en_US.UTF-8
# Tue, 28 Sep 2021 15:49:45 GMT
ENV LANG=en_US.UTF-8
# Tue, 28 Sep 2021 15:49:46 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Tue, 28 Sep 2021 15:49:46 GMT
ENV R_BASE_VERSION=4.1.1
# Tue, 28 Sep 2021 15:49:47 GMT
RUN echo "deb http://deb.debian.org/debian experimental main" > /etc/apt/sources.list.d/experimental.list     && echo "deb [trusted=yes] https://eddelbuettel.github.io/ppaR400 ./" > /etc/apt/sources.list.d/edd-r4.list
# Tue, 28 Sep 2021 15:50:37 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 15:50:39 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:5fd04373f6dc4ec57b4af01b70782245fdb26a426888b8d0fe9169590ef679b7`  
		Last Modified: Tue, 28 Sep 2021 01:53:17 GMT  
		Size: 54.5 MB (54460337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e418464f49f41ba43443d77e90ee257ef0a60fe422389cdafa9171100bc6f12`  
		Last Modified: Tue, 28 Sep 2021 15:50:55 GMT  
		Size: 1.9 KB (1876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eda43c359b84724a6c7d59c423387ac97b8239a3baaf96b2ad044d38da7a7690`  
		Last Modified: Tue, 28 Sep 2021 15:50:56 GMT  
		Size: 25.6 MB (25578065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e5391d63d29be63b22f7c888d0bb3e63b310b48bdfdef14c73b0d51e306fcbf`  
		Last Modified: Tue, 28 Sep 2021 15:50:53 GMT  
		Size: 864.6 KB (864613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd4ad37830882347e1b2d1d2239d283be294c35899483487b278ea18e5cf8e86`  
		Last Modified: Tue, 28 Sep 2021 15:50:53 GMT  
		Size: 348.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebba437b4f1d5d81167585c32a6dbab9cebda1f1d2bae7ac44600c4fcfd74e6c`  
		Last Modified: Tue, 28 Sep 2021 15:50:53 GMT  
		Size: 292.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54c9f61c3faaebe463cb4b6be3f6204e78a5639450d8a2380ce64fc8fac2da5e`  
		Last Modified: Tue, 28 Sep 2021 15:51:22 GMT  
		Size: 234.3 MB (234264461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:latest` - linux; ppc64le

```console
$ docker pull r-base@sha256:617559accc990c254a4ff30d43605d99c4de2a770191715667cc25a57b00fa57
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **322.6 MB (322579703 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd4059f6fd409984d90ddd1fce6ac7dc0049dc269105b326db7ab06dc42796d6`
-	Default Command: `["R"]`

```dockerfile
# Fri, 03 Sep 2021 01:28:03 GMT
ADD file:3c352e1c5b975bab6ba80213fc86e0b5836f9976e755be58fccd6f003941ca8b in / 
# Fri, 03 Sep 2021 01:28:12 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 18:07:19 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Fri, 03 Sep 2021 18:07:40 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Fri, 03 Sep 2021 18:08:48 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 18:09:03 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Fri, 03 Sep 2021 18:09:10 GMT
ENV LC_ALL=en_US.UTF-8
# Fri, 03 Sep 2021 18:09:15 GMT
ENV LANG=en_US.UTF-8
# Fri, 03 Sep 2021 18:09:24 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Fri, 03 Sep 2021 18:09:28 GMT
ENV R_BASE_VERSION=4.1.1
# Fri, 03 Sep 2021 18:09:43 GMT
RUN echo "deb http://deb.debian.org/debian experimental main" > /etc/apt/sources.list.d/experimental.list     && echo "deb [trusted=yes] https://eddelbuettel.github.io/ppaR400 ./" > /etc/apt/sources.list.d/edd-r4.list
# Fri, 03 Sep 2021 18:16:58 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 18:17:21 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:61eff2bf557a409d063c940d589dc8f98bf037655ffc94d8e30b546974554826`  
		Last Modified: Fri, 03 Sep 2021 01:47:00 GMT  
		Size: 59.5 MB (59526125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce611fbe8ab05ce2c89df4861eda9fa9a9ac574620f25260b3392fc1dbf77770`  
		Last Modified: Fri, 03 Sep 2021 18:17:44 GMT  
		Size: 1.9 KB (1897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07ebd15523833a8c3199a65b13cc3cf32a3c2519b0ffc145fe94c832b7ad527d`  
		Last Modified: Fri, 03 Sep 2021 18:17:44 GMT  
		Size: 25.8 MB (25847783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7784100ddcd38691f40bcbff901986458cd1db182a9f421257bc99102bae1a50`  
		Last Modified: Fri, 03 Sep 2021 18:17:40 GMT  
		Size: 864.6 KB (864587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00e932154d909477bfe626a1240d5f45735b0e128fdbf67a9a8f91ebdecb3772`  
		Last Modified: Fri, 03 Sep 2021 18:17:40 GMT  
		Size: 351.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85ce1c57788b3101614032507e56e512abe5141f74980255a57f6d2867a8c194`  
		Last Modified: Fri, 03 Sep 2021 18:17:40 GMT  
		Size: 294.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac7ca859214f67b7844bed90bf073802c0fa78e0e2a27926fdc9a4ac983d64d6`  
		Last Modified: Fri, 03 Sep 2021 18:22:34 GMT  
		Size: 236.3 MB (236338666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:latest` - linux; s390x

```console
$ docker pull r-base@sha256:f20bfa8c68f388f3f6e71d98f6ac9ad932098ca2a34c570356029c33a294836e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **290.9 MB (290927543 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:968c5937c5239367ba52cd6cc597c904864dc5e0d347455bda95c928db3edd85`
-	Default Command: `["R"]`

```dockerfile
# Tue, 28 Sep 2021 01:45:08 GMT
ADD file:094728d97cbb14c94edb377e3d4dede62bd88e82f98ecd93bba64aebc4e7916a in / 
# Tue, 28 Sep 2021 01:45:10 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 07:23:40 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Tue, 28 Sep 2021 07:23:40 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Tue, 28 Sep 2021 07:23:49 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 07:23:51 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Tue, 28 Sep 2021 07:23:52 GMT
ENV LC_ALL=en_US.UTF-8
# Tue, 28 Sep 2021 07:23:52 GMT
ENV LANG=en_US.UTF-8
# Tue, 28 Sep 2021 07:23:52 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Tue, 28 Sep 2021 07:23:52 GMT
ENV R_BASE_VERSION=4.1.1
# Tue, 28 Sep 2021 07:23:53 GMT
RUN echo "deb http://deb.debian.org/debian experimental main" > /etc/apt/sources.list.d/experimental.list     && echo "deb [trusted=yes] https://eddelbuettel.github.io/ppaR400 ./" > /etc/apt/sources.list.d/edd-r4.list
# Tue, 28 Sep 2021 07:24:42 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 07:24:50 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:93e4733dccf8c066cccad1642f393ff63777ee8c1262cdbc961912a70203c3cb`  
		Last Modified: Tue, 28 Sep 2021 01:51:12 GMT  
		Size: 53.7 MB (53691013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a395ea0887cd48211810e3375f5b786c91bcec52da80d50b3b7c87c36ad379a`  
		Last Modified: Tue, 28 Sep 2021 07:25:07 GMT  
		Size: 1.9 KB (1876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fb981f9996bf74c927220cb62ca23a0f538a4852ceae9675b6269f3dd0664ed`  
		Last Modified: Tue, 28 Sep 2021 07:25:08 GMT  
		Size: 25.6 MB (25588352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6bfc1ca3ad281ed1acbb966e7df4c0bc7441e54d5e14d25c125ed8bdbb88266`  
		Last Modified: Tue, 28 Sep 2021 07:25:06 GMT  
		Size: 920.2 KB (920188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12174ad516d3a507e2f9681a62dfa0d98dbeee9645fc4641b005b5e32cfa05f3`  
		Last Modified: Tue, 28 Sep 2021 07:25:06 GMT  
		Size: 347.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61fe3e1e7a058b2f5343180fe46f90f388d774c223bf3b8fbbc73f058e19e763`  
		Last Modified: Tue, 28 Sep 2021 07:25:06 GMT  
		Size: 292.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f286a00e3bd2e1971e090ef242c822b502df8bcf652d44b60981902b72d62d52`  
		Last Modified: Tue, 28 Sep 2021 07:25:26 GMT  
		Size: 210.7 MB (210725475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
