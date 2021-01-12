## `r-base:latest`

```console
$ docker pull r-base@sha256:e4ab10fc1531a59e92c50e0e80f0f9de9c54d79162e9a88bcc1da0635d717e1d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `r-base:latest` - linux; amd64

```console
$ docker pull r-base@sha256:fd192ac4edc4e94bdd7d4d62b6dd8c83f6a1303eb48d93ef9a4685fd0a9513f2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **519.8 MB (519758360 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b4fd0403f8f8106887bb5ea107613015f7e25e54f1f787970bd242dfd50230c`
-	Default Command: `["R"]`

```dockerfile
# Fri, 11 Dec 2020 02:09:13 GMT
ADD file:6293ddf53588d819bfa272e4dbeb8a0b72de03092414e598350b6c9ce5b08ac1 in / 
# Fri, 11 Dec 2020 02:09:13 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 21:25:00 GMT
LABEL org.label-schema.license=GPL-2.0 org.label-schema.vcs-url=https://github.com/rocker-org/r-base org.label-schema.vendor=Rocker Project maintainer=Dirk Eddelbuettel <edd@debian.org>
# Fri, 11 Dec 2020 21:25:02 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Fri, 11 Dec 2020 21:25:16 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 21:25:21 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Fri, 11 Dec 2020 21:25:21 GMT
ENV LC_ALL=en_US.UTF-8
# Fri, 11 Dec 2020 21:25:21 GMT
ENV LANG=en_US.UTF-8
# Fri, 11 Dec 2020 21:25:23 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Fri, 11 Dec 2020 21:25:23 GMT
ENV R_BASE_VERSION=4.0.3
# Fri, 11 Dec 2020 21:27:14 GMT
RUN apt-get update         && apt-get install -t unstable -y --no-install-recommends                 gcc-9-base                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 21:27:16 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:ecd924c7226f314c16de965258f37da4aa990c07e494be1116af512706138401`  
		Last Modified: Fri, 11 Dec 2020 02:16:00 GMT  
		Size: 53.1 MB (53113573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fec22ce03e6be2d27efb3e9a90be68b14183859abf0864518e2581aa49fb8f5`  
		Last Modified: Fri, 11 Dec 2020 21:27:45 GMT  
		Size: 1.8 KB (1841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69d900227a8f4d4d2647927b9fa8da77f0f535ca497bc771c5f8a72b0cc971df`  
		Last Modified: Fri, 11 Dec 2020 21:27:52 GMT  
		Size: 27.4 MB (27441203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45c9ad96a035ae2a5bda28a6e666ed7e1bbe5d945180faafd1c2ed611473e728`  
		Last Modified: Fri, 11 Dec 2020 21:27:46 GMT  
		Size: 863.6 KB (863572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6f2416c67056dd5c3a5948858ab4578631e13cc36ee43bd8d44dea4ec4693f7`  
		Last Modified: Fri, 11 Dec 2020 21:27:44 GMT  
		Size: 351.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0079bdf52f600362737f2c00e7e7ae11458844ef1d06265caf24115be990c4ab`  
		Last Modified: Fri, 11 Dec 2020 21:29:26 GMT  
		Size: 438.3 MB (438337820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:latest` - linux; arm64 variant v8

```console
$ docker pull r-base@sha256:6ba94de9e7adb0f7cd759594a90b025a8782dbd032c72dabc9bd8d33c6f2f648
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **507.1 MB (507072736 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad039ec4a4b4b25d8b7955589ea37ca166ad971f2fb85bd0a3c1dfa576dc3d20`
-	Default Command: `["R"]`

```dockerfile
# Fri, 11 Dec 2020 02:49:00 GMT
ADD file:68734186568fd3a803d44d4f42065373a0200929b1ff39d104a24dfe14316ae0 in / 
# Fri, 11 Dec 2020 02:49:04 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 17:02:39 GMT
LABEL org.label-schema.license=GPL-2.0 org.label-schema.vcs-url=https://github.com/rocker-org/r-base org.label-schema.vendor=Rocker Project maintainer=Dirk Eddelbuettel <edd@debian.org>
# Fri, 11 Dec 2020 17:02:41 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Fri, 11 Dec 2020 17:03:04 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 17:03:10 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Fri, 11 Dec 2020 17:03:13 GMT
ENV LC_ALL=en_US.UTF-8
# Fri, 11 Dec 2020 17:03:14 GMT
ENV LANG=en_US.UTF-8
# Fri, 11 Dec 2020 17:03:18 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Fri, 11 Dec 2020 17:03:20 GMT
ENV R_BASE_VERSION=4.0.3
# Fri, 11 Dec 2020 17:05:40 GMT
RUN apt-get update         && apt-get install -t unstable -y --no-install-recommends                 gcc-9-base                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 17:05:52 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:37ba54a7ad02aab7f88ab28bf1de79bd2861de26af6a6998d9b8dab9cc58b2f9`  
		Last Modified: Fri, 11 Dec 2020 02:56:23 GMT  
		Size: 52.0 MB (51961789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08fc484ab337728ab0a3c81b0016c1b7d0042e4dc5881e2bee0f37111cc38000`  
		Last Modified: Fri, 11 Dec 2020 17:06:04 GMT  
		Size: 1.9 KB (1875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1353e5265e09e606d78cfdd681b7dc846953a304e13bf818911949895b3b9353`  
		Last Modified: Fri, 11 Dec 2020 17:06:12 GMT  
		Size: 27.3 MB (27309206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:617418dda951dc7cf53cd4c56893d986d78219ef8422a487fbf414e3dfd6a4a2`  
		Last Modified: Fri, 11 Dec 2020 17:06:05 GMT  
		Size: 863.6 KB (863571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6073a1e61d66d2451b5f7149251cdbf6de1483ea3bceded8d786dfb5f9bd85bf`  
		Last Modified: Fri, 11 Dec 2020 17:06:04 GMT  
		Size: 350.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab79f74827b044a430446d69c7439babb4bfb3a8e2c11a19ac582bf4f230849a`  
		Last Modified: Fri, 11 Dec 2020 17:07:39 GMT  
		Size: 426.9 MB (426935945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:latest` - linux; ppc64le

```console
$ docker pull r-base@sha256:139d4698204b39dd9f33be02e2dac63a5bc88dffc679357d3a5c457c929de863
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **324.5 MB (324529438 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31a24688a5bbb3249b725ca6d38eb2329c1c2d8e89f301b09763e020635734c1`
-	Default Command: `["R"]`

```dockerfile
# Tue, 12 Jan 2021 00:28:12 GMT
ADD file:7c5aef981ec69d203ed3041958d604b3c221d38286982325e933a4aea004fd00 in / 
# Tue, 12 Jan 2021 00:28:23 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 12:54:51 GMT
LABEL org.label-schema.license=GPL-2.0 org.label-schema.vcs-url=https://github.com/rocker-org/r-base org.label-schema.vendor=Rocker Project maintainer=Dirk Eddelbuettel <edd@debian.org>
# Tue, 12 Jan 2021 12:55:22 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Tue, 12 Jan 2021 12:56:58 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 12:57:17 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Tue, 12 Jan 2021 12:57:24 GMT
ENV LC_ALL=en_US.UTF-8
# Tue, 12 Jan 2021 12:57:30 GMT
ENV LANG=en_US.UTF-8
# Tue, 12 Jan 2021 12:57:43 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Tue, 12 Jan 2021 12:57:49 GMT
ENV R_BASE_VERSION=4.0.3
# Tue, 12 Jan 2021 13:09:41 GMT
RUN apt-get update         && apt-get install -t unstable -y --no-install-recommends                 gcc-9-base                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 13:09:52 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:6168374c1cd1389f3d510ecd4c9bd0520534b68b8f0f32d0479e4fa2e3e9d69e`  
		Last Modified: Tue, 12 Jan 2021 00:36:39 GMT  
		Size: 57.6 MB (57562274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94a18c049e4f1d3122ce4fcc8aa472880ed62bdb9c30004e3220a381156bafb4`  
		Last Modified: Tue, 12 Jan 2021 13:10:13 GMT  
		Size: 1.9 KB (1903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b15505cef7e245a6456323c3f6293294160de098922762dfca14350f289538bb`  
		Last Modified: Tue, 12 Jan 2021 13:10:17 GMT  
		Size: 27.8 MB (27794114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:231bf04f1dee3c8e578421445abca648fa407871cac53d09b21d11f112f165f3`  
		Last Modified: Tue, 12 Jan 2021 13:10:13 GMT  
		Size: 864.6 KB (864592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:333fae2e7ae74eb979d942af51c586744886d092384d423f8ab90339254a73d0`  
		Last Modified: Tue, 12 Jan 2021 13:10:13 GMT  
		Size: 353.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9c678d06179ba47f5b8e2aa668d8498f0b99941c3cc2f44f215f76a415575d5`  
		Last Modified: Tue, 12 Jan 2021 13:10:52 GMT  
		Size: 238.3 MB (238306202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:latest` - linux; s390x

```console
$ docker pull r-base@sha256:fa199886bedfdb7388dd4f993b9c2365937bc62a6a704084c30d2051ec81d68b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **291.8 MB (291817775 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce25e85e3805bebfa4d2ef0e687b732eec3d60c87d6211be5ec49126d59e377b`
-	Default Command: `["R"]`

```dockerfile
# Tue, 12 Jan 2021 00:43:20 GMT
ADD file:79d77ce0e127a883c7393aaca5f89cab2b36703e9d08104596c40e09674d59f1 in / 
# Tue, 12 Jan 2021 00:43:23 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 02:58:19 GMT
LABEL org.label-schema.license=GPL-2.0 org.label-schema.vcs-url=https://github.com/rocker-org/r-base org.label-schema.vendor=Rocker Project maintainer=Dirk Eddelbuettel <edd@debian.org>
# Tue, 12 Jan 2021 02:58:20 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Tue, 12 Jan 2021 02:58:32 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 02:58:35 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Tue, 12 Jan 2021 02:58:35 GMT
ENV LC_ALL=en_US.UTF-8
# Tue, 12 Jan 2021 02:58:35 GMT
ENV LANG=en_US.UTF-8
# Tue, 12 Jan 2021 02:58:36 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Tue, 12 Jan 2021 02:58:37 GMT
ENV R_BASE_VERSION=4.0.3
# Tue, 12 Jan 2021 03:00:10 GMT
RUN apt-get update         && apt-get install -t unstable -y --no-install-recommends                 gcc-9-base                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 03:00:33 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:deacf9aa62ade6e1002e481ea38b97d12b800eae2cb010989bdf011c18c51650`  
		Last Modified: Tue, 12 Jan 2021 01:01:15 GMT  
		Size: 52.1 MB (52108018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4beb7061eb3cbd983566deb7ffcce8dfdee9d022ba267c60e74d01d1c07906f2`  
		Last Modified: Tue, 12 Jan 2021 03:01:08 GMT  
		Size: 1.9 KB (1878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cc4dd911ad9cd61fcfa326a909b3d2c7b7bc5d0cd09b5be9a12606b3cd28df2`  
		Last Modified: Tue, 12 Jan 2021 03:01:09 GMT  
		Size: 27.2 MB (27202505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a38cfc05f022a4702289843696fe5120b243eca1cc6db91dfe4e2f23f0cedd7f`  
		Last Modified: Tue, 12 Jan 2021 03:01:09 GMT  
		Size: 920.2 KB (920163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84133159b6c7664a09dc38a73f778bddcf71f8da27f6462c4780fe9a73a37669`  
		Last Modified: Tue, 12 Jan 2021 03:01:08 GMT  
		Size: 351.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34a5d757409c836febb87e4a55b9c3e34af980cc36dd4726503c943f9c7ab18c`  
		Last Modified: Tue, 12 Jan 2021 03:01:32 GMT  
		Size: 211.6 MB (211584860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
