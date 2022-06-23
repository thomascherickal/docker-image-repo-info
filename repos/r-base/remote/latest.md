## `r-base:latest`

```console
$ docker pull r-base@sha256:9734d33db3214a78dbb9d4aa3060a19e42a0a510ea3ffbb5bea36ccaa5d21fc7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `r-base:latest` - linux; amd64

```console
$ docker pull r-base@sha256:5bebae7cf805dd448f7cc41a30e7fe01361e645dff70243a5254d452330bc68c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **338.7 MB (338656865 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97b416af57eae0eaa48e1cd3ca28171c8f2eb82112d380420cbaf00aec0c90e9`
-	Default Command: `["R"]`

```dockerfile
# Sat, 28 May 2022 01:22:29 GMT
ADD file:272efeab320060153c6fd77f52b9a9922149739b8f010d93cde516421fde6ce9 in / 
# Sat, 28 May 2022 01:22:30 GMT
CMD ["bash"]
# Sat, 28 May 2022 16:20:20 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Sat, 28 May 2022 16:20:20 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Sat, 28 May 2022 16:20:29 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 16:20:32 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Sat, 28 May 2022 16:20:32 GMT
ENV LC_ALL=en_US.UTF-8
# Sat, 28 May 2022 16:20:32 GMT
ENV LANG=en_US.UTF-8
# Sat, 28 May 2022 16:20:33 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Sat, 28 May 2022 16:20:33 GMT
ENV R_BASE_VERSION=4.2.0
# Sat, 28 May 2022 16:21:17 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-docopt                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 16:21:19 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:344633e2dec142d10b6e072c2fded693fe7441d6af83d21be68657a30ac0ceaa`  
		Last Modified: Sat, 28 May 2022 01:29:25 GMT  
		Size: 52.9 MB (52947617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3534c2eeb1ed45895835ed12ccdeb205f5067b3ce17a5b188bba0bf4c4949fac`  
		Last Modified: Sat, 28 May 2022 16:21:34 GMT  
		Size: 1.9 KB (1876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc36dc8c7553ef509c9fe36539ff13ce1cbed6f234785229964905980f462c7b`  
		Last Modified: Sat, 28 May 2022 16:21:38 GMT  
		Size: 27.8 MB (27800906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a763294a707cf41ed16919594fa06b51f3ef57533daef870c45513ae3495f8f8`  
		Last Modified: Sat, 28 May 2022 16:21:35 GMT  
		Size: 864.6 KB (864611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db6688aa5e3c7633e868f7b78b2d37c0be20b046a688dd6121e89491c996b94f`  
		Last Modified: Sat, 28 May 2022 16:21:34 GMT  
		Size: 346.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:132285c4b96260e9eefc870f3589c62363cab6f4caa4d09c3489ac9ede491bca`  
		Last Modified: Sat, 28 May 2022 16:22:05 GMT  
		Size: 257.0 MB (257041509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:latest` - linux; arm64 variant v8

```console
$ docker pull r-base@sha256:6a983779870e09d3e9d7d062ec1243373a670fdf472aa9dae4ad2a0270e16398
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **329.4 MB (329381803 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b1ed7a81a958b7977c1429512a822cebd636ca5d2199f586fdc265c45a019fc`
-	Default Command: `["R"]`

```dockerfile
# Thu, 23 Jun 2022 00:43:09 GMT
ADD file:53311373f4d1abfcaa16b8c6fdad786327061f1e5003db1d3c6bdbf5b2c73333 in / 
# Thu, 23 Jun 2022 00:43:10 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 09:55:34 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Thu, 23 Jun 2022 09:55:35 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Thu, 23 Jun 2022 09:55:47 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 09:55:50 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Thu, 23 Jun 2022 09:55:50 GMT
ENV LC_ALL=en_US.UTF-8
# Thu, 23 Jun 2022 09:55:51 GMT
ENV LANG=en_US.UTF-8
# Thu, 23 Jun 2022 09:55:52 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Thu, 23 Jun 2022 09:55:53 GMT
ENV R_BASE_VERSION=4.2.0
# Thu, 23 Jun 2022 09:57:02 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-docopt                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 09:57:03 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:04df16d59bbc997b9cf53108e57268f1beac69c21eb10fac7036d92a38799d9c`  
		Last Modified: Thu, 23 Jun 2022 00:52:10 GMT  
		Size: 52.1 MB (52074599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e44e225ee8267ff47a685e6fb7cb3e044051d38a19f78c599083ef981bd56ee0`  
		Last Modified: Thu, 23 Jun 2022 09:57:23 GMT  
		Size: 1.8 KB (1828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:862e7e0ff7609e8e099b3476c09bf2fa4645d8917ac0ce81c641a21d9b76d943`  
		Last Modified: Thu, 23 Jun 2022 09:57:27 GMT  
		Size: 28.9 MB (28924383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:045b58c869361534b4dec8cb9fd7a07aa8cd72ec3cdfc49898db1c639289a98a`  
		Last Modified: Thu, 23 Jun 2022 09:57:23 GMT  
		Size: 864.6 KB (864603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d3e03efb36a58b2e4b0fef0b6d21e4449eb66de24e494f031e78b6e2350e609`  
		Last Modified: Thu, 23 Jun 2022 09:57:23 GMT  
		Size: 348.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27e47051f85d6a605c04fce2c11d4de6b822f1be1febc1d1bc19c7c0201f9c7a`  
		Last Modified: Thu, 23 Jun 2022 09:57:51 GMT  
		Size: 247.5 MB (247516042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:latest` - linux; ppc64le

```console
$ docker pull r-base@sha256:9e6e298460673240a6a1a76ecead7df84469b82223e629412b7f115ae0322838
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **337.7 MB (337662243 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:738aee963ca73d0f2ecdf52a5927e62791df25e7e4b1a5c5bcf47513e2d697a7`
-	Default Command: `["R"]`

```dockerfile
# Sat, 28 May 2022 01:26:41 GMT
ADD file:c839faac39e30677565fb631dd4f40114392a7a667b8db7f85ca4d8aaeb32ad9 in / 
# Sat, 28 May 2022 01:26:46 GMT
CMD ["bash"]
# Sat, 28 May 2022 18:13:35 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Sat, 28 May 2022 18:13:55 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Sat, 28 May 2022 18:15:13 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 18:15:22 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Sat, 28 May 2022 18:15:24 GMT
ENV LC_ALL=en_US.UTF-8
# Sat, 28 May 2022 18:15:26 GMT
ENV LANG=en_US.UTF-8
# Sat, 28 May 2022 18:15:30 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Sat, 28 May 2022 18:15:33 GMT
ENV R_BASE_VERSION=4.2.0
# Sat, 28 May 2022 18:19:59 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-docopt                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 18:20:05 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:f5e0403edf3ce1164c65241f62272268585e383702736c781adae79230ef3422`  
		Last Modified: Sat, 28 May 2022 01:36:21 GMT  
		Size: 57.2 MB (57161585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93558bc00b065b9fdfdf638afa73d518e79d21654d4fa6ac9bbcf6ae535ff29f`  
		Last Modified: Sat, 28 May 2022 18:20:30 GMT  
		Size: 1.9 KB (1899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:426e1ec607ca488db98567b783ca407dd68087a6d7e2c87853705d3aacda96eb`  
		Last Modified: Sat, 28 May 2022 18:20:34 GMT  
		Size: 28.1 MB (28116523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e2bda5aa6c71f2bcf5010b6c74c566b6b1d20f2965e51e890bac59cc040d212`  
		Last Modified: Sat, 28 May 2022 18:20:31 GMT  
		Size: 864.6 KB (864604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:245fb89f5cf42bcd0902cd81074060fd771c9f04b430c63bf7ad0f86fe52e8de`  
		Last Modified: Sat, 28 May 2022 18:20:30 GMT  
		Size: 352.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8fa9c9dd9a0c1c6447e9df11957b34124507932a8d73669d4acdd4251e71011`  
		Last Modified: Sat, 28 May 2022 18:21:08 GMT  
		Size: 251.5 MB (251517280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:latest` - linux; s390x

```console
$ docker pull r-base@sha256:ad911df2fb08e45bb78edaa2b5132acfb3c29a561f920de30f09509218117bbd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **303.2 MB (303172603 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:009a7af67a6581ac856d7b45ed7a6d339166e7e49f0931e734b15128359c4d72`
-	Default Command: `["R"]`

```dockerfile
# Sat, 28 May 2022 00:45:48 GMT
ADD file:430aae00218790907570f298b5f5c4e47453d9297090e8d006c5169e5e9ee56f in / 
# Sat, 28 May 2022 00:45:52 GMT
CMD ["bash"]
# Sat, 28 May 2022 14:09:44 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Sat, 28 May 2022 14:09:47 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Sat, 28 May 2022 14:10:16 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 14:10:22 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Sat, 28 May 2022 14:10:23 GMT
ENV LC_ALL=en_US.UTF-8
# Sat, 28 May 2022 14:10:23 GMT
ENV LANG=en_US.UTF-8
# Sat, 28 May 2022 14:10:25 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Sat, 28 May 2022 14:10:25 GMT
ENV R_BASE_VERSION=4.2.0
# Sat, 28 May 2022 14:12:29 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-docopt                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 14:12:55 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:33ada038def02ed9f3f9762c43feeaf3a66329f979154e6d3dca5e1ac4f04893`  
		Last Modified: Sat, 28 May 2022 00:51:52 GMT  
		Size: 51.5 MB (51490267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a40a861a5b04c2f9889f2481238dada12e05ef5844db1f03ea5de352d22e3de3`  
		Last Modified: Sat, 28 May 2022 14:13:14 GMT  
		Size: 1.9 KB (1886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60fed479b3faef6d091cca289e8173d1a92762ec6a1768240402b5807e63bd73`  
		Last Modified: Sat, 28 May 2022 14:13:17 GMT  
		Size: 27.5 MB (27505490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14758b183e8702560c5dce06f1b61d392a37f125018ffc195e752540236143cc`  
		Last Modified: Sat, 28 May 2022 14:13:14 GMT  
		Size: 920.2 KB (920190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1038de2e612076d08cd18dc92b28c954cfb3f1b144a68cb80632b4127c1077d3`  
		Last Modified: Sat, 28 May 2022 14:13:14 GMT  
		Size: 349.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb0e8d52a9bc82a685f859ebb220b2279417a7e47ccbb4acbaec63e528c7a869`  
		Last Modified: Sat, 28 May 2022 14:13:36 GMT  
		Size: 223.3 MB (223254421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
