## `r-base:latest`

```console
$ docker pull r-base@sha256:4f8079455d39e66e3b2ebfe494bfd412c146dcb28931477466b1dbe5a1f01de3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `r-base:latest` - linux; amd64

```console
$ docker pull r-base@sha256:6389af5f9cf5c3c3268ed83fc9d9993e1321a7d9735bff43a44e026f4f6a0589
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **324.9 MB (324896043 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:062d8418ba77d109875505c295d28600ade9642f3d3828eb5240a3d4dc0af380`
-	Default Command: `["R"]`

```dockerfile
# Thu, 22 Jul 2021 00:47:30 GMT
ADD file:aefd1b2aad4a1d98fd82d86cab1e66f8f172c748e69090a4938ded7681a5fcfe in / 
# Thu, 22 Jul 2021 00:47:30 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 14:25:02 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Thu, 22 Jul 2021 14:25:03 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Thu, 22 Jul 2021 14:25:13 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 14:25:15 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Thu, 22 Jul 2021 14:25:15 GMT
ENV LC_ALL=en_US.UTF-8
# Thu, 22 Jul 2021 14:25:16 GMT
ENV LANG=en_US.UTF-8
# Thu, 22 Jul 2021 14:25:16 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Thu, 22 Jul 2021 14:25:17 GMT
ENV R_BASE_VERSION=4.1.0
# Thu, 22 Jul 2021 14:25:17 GMT
RUN echo "deb http://deb.debian.org/debian experimental main" > /etc/apt/sources.list.d/experimental.list     && echo "deb [trusted=yes] https://eddelbuettel.github.io/ppaR400 ./" > /etc/apt/sources.list.d/edd-r4.list
# Thu, 22 Jul 2021 14:26:07 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 14:26:09 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:7b303595d9b321a9020d0ddbf1dea4c83237e2367117606a8d5466c446714ba1`  
		Last Modified: Thu, 22 Jul 2021 00:53:44 GMT  
		Size: 54.9 MB (54904726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:269a52eb0491fa8f50f18f968e9a26e2c3f139332e157f2af3eaaa4ad8fbdab5`  
		Last Modified: Thu, 22 Jul 2021 14:26:23 GMT  
		Size: 1.9 KB (1878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ded859387bdafb915ae926a385218acb88202f871dab977fc1f53237dfb4a079`  
		Last Modified: Thu, 22 Jul 2021 14:26:23 GMT  
		Size: 25.6 MB (25629332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e9a9ca14ab54b7dcc64efd3dd1e59caa23457c62f787811a6dd14e73aeb8421`  
		Last Modified: Thu, 22 Jul 2021 14:26:21 GMT  
		Size: 864.6 KB (864588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2833e2a4a5cdc17504b1c82018201d1ab11fd9561b5f6b53a380150c056f80f`  
		Last Modified: Thu, 22 Jul 2021 14:26:20 GMT  
		Size: 349.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69b7b0952253024702757260108e530df6c9ae666d502264c710da8fec1cfb2b`  
		Last Modified: Thu, 22 Jul 2021 14:26:20 GMT  
		Size: 292.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13ddaffde5f2fd497225a2dd814720ed94058b4b8b663074160e4cea4b12c89e`  
		Last Modified: Thu, 22 Jul 2021 14:26:50 GMT  
		Size: 243.5 MB (243494878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:latest` - linux; arm64 variant v8

```console
$ docker pull r-base@sha256:d61c5c0c116010f15891b8c0f013d6cf1e2487890c0edb8bcb88bf73b84ec0cc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **312.4 MB (312362637 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b8f6116270d9204b7b3e518635f4e7d08de49d5982b08a62a2c80bd8ead0378`
-	Default Command: `["R"]`

```dockerfile
# Thu, 22 Jul 2021 00:41:51 GMT
ADD file:e33f1c12a015f577adbcae333030de59322c78d065b6a9bc023ebbe8137f3884 in / 
# Thu, 22 Jul 2021 00:41:51 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 12:13:23 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Thu, 22 Jul 2021 12:13:24 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Thu, 22 Jul 2021 12:13:34 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 12:13:36 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Thu, 22 Jul 2021 12:13:37 GMT
ENV LC_ALL=en_US.UTF-8
# Thu, 22 Jul 2021 12:13:37 GMT
ENV LANG=en_US.UTF-8
# Thu, 22 Jul 2021 12:13:37 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Thu, 22 Jul 2021 12:13:38 GMT
ENV R_BASE_VERSION=4.1.0
# Thu, 22 Jul 2021 12:13:38 GMT
RUN echo "deb http://deb.debian.org/debian experimental main" > /etc/apt/sources.list.d/experimental.list     && echo "deb [trusted=yes] https://eddelbuettel.github.io/ppaR400 ./" > /etc/apt/sources.list.d/edd-r4.list
# Thu, 22 Jul 2021 12:14:31 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 12:14:33 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:219bbd9a92d615a2d512d8204c52d9cba7f032064387678c47123983ca063289`  
		Last Modified: Thu, 22 Jul 2021 00:49:16 GMT  
		Size: 53.6 MB (53590205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ab128d1f5ec46f03af996322b9683b862542c96ddef5fd573885c7db8014ed9`  
		Last Modified: Thu, 22 Jul 2021 12:15:00 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fccac96ce4f126515968851094204c465e8bfc6ee6f2f8889eee8848fd5d485`  
		Last Modified: Thu, 22 Jul 2021 12:15:01 GMT  
		Size: 25.6 MB (25632060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5778bb4352a8fc91a9b7bd6c35112a000b3fc67ca354f9697d473f494158e75`  
		Last Modified: Thu, 22 Jul 2021 12:14:58 GMT  
		Size: 864.6 KB (864588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccf8c5d799739c59f3dee54e610ab1201d15cd13daff7e40cb800204a6b6c595`  
		Last Modified: Thu, 22 Jul 2021 12:14:57 GMT  
		Size: 349.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:231140f92441342bf0acd056d11d264715a9b733b57ac6ec32c2f57df389983b`  
		Last Modified: Thu, 22 Jul 2021 12:14:58 GMT  
		Size: 293.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97882368289ce686d45b910f3884a1a64a4ffd1f2ff0676ff61a742096031000`  
		Last Modified: Thu, 22 Jul 2021 12:15:26 GMT  
		Size: 232.3 MB (232273261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:latest` - linux; ppc64le

```console
$ docker pull r-base@sha256:4409a49802cb68dbb5135c26e7408f0ba6bc9713951620f2247c830c5de7f394
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **322.6 MB (322598908 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b88152f390f9fd6cc3bd37783d1c9bee76a231aa4fae1d8bbeb62dc3520e4f76`
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
# Fri, 23 Jul 2021 00:10:50 GMT
ENV R_BASE_VERSION=4.1.0
# Fri, 23 Jul 2021 00:11:22 GMT
RUN echo "deb http://deb.debian.org/debian experimental main" > /etc/apt/sources.list.d/experimental.list     && echo "deb [trusted=yes] https://eddelbuettel.github.io/ppaR400 ./" > /etc/apt/sources.list.d/edd-r4.list
# Fri, 23 Jul 2021 00:24:36 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Fri, 23 Jul 2021 00:24:44 GMT
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
	-	`sha256:4d3e2cf0069f646bfe571113cccfe62672988a5f36818c1b5111928c16e0daf6`  
		Last Modified: Fri, 23 Jul 2021 00:25:13 GMT  
		Size: 296.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:600cad0e6a7223178bf3f7b1cbeeefd5bf9d505d67d14e222b9c8317934326a9`  
		Last Modified: Fri, 23 Jul 2021 00:25:50 GMT  
		Size: 237.1 MB (237065304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:latest` - linux; s390x

```console
$ docker pull r-base@sha256:6ee58fcf95f73f262cfdd59673abe9b2b85639b7c61b575f38a3c5cfe702e40f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **291.1 MB (291088464 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:293550768279b765372e3483ce1c705bb5089f9a29e6b3bd15be7857925dfd96`
-	Default Command: `["R"]`

```dockerfile
# Thu, 22 Jul 2021 00:44:05 GMT
ADD file:21b5f07587901992012f9aba1a8fea81bde8e4d0178a7b01221b7a6070bec5c9 in / 
# Thu, 22 Jul 2021 00:44:09 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 06:27:54 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Thu, 22 Jul 2021 06:27:56 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Thu, 22 Jul 2021 06:28:12 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 06:28:16 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Thu, 22 Jul 2021 06:28:16 GMT
ENV LC_ALL=en_US.UTF-8
# Thu, 22 Jul 2021 06:28:16 GMT
ENV LANG=en_US.UTF-8
# Thu, 22 Jul 2021 06:28:18 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Thu, 22 Jul 2021 06:28:18 GMT
ENV R_BASE_VERSION=4.1.0
# Thu, 22 Jul 2021 06:28:19 GMT
RUN echo "deb http://deb.debian.org/debian experimental main" > /etc/apt/sources.list.d/experimental.list     && echo "deb [trusted=yes] https://eddelbuettel.github.io/ppaR400 ./" > /etc/apt/sources.list.d/edd-r4.list
# Thu, 22 Jul 2021 06:29:35 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 06:29:47 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:e3700ef60bb30345145fe56d1d43ec09db7b1a70ff7852b92d2431cc9cb59352`  
		Last Modified: Thu, 22 Jul 2021 00:49:37 GMT  
		Size: 53.2 MB (53183480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db6493a32457ba4c2a4d12fd05e24b15b0e52892e141503003ecf8a1efac03da`  
		Last Modified: Thu, 22 Jul 2021 06:30:08 GMT  
		Size: 1.9 KB (1889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74548a6452ad87b63b5cf8a0e1d51fc60039258d14e5c58aad95b47e4762ebe5`  
		Last Modified: Thu, 22 Jul 2021 06:30:09 GMT  
		Size: 25.6 MB (25632677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baf8c1226497d314511830e477645eaa45d6ee64def55d8a14e69c2522b7c8e2`  
		Last Modified: Thu, 22 Jul 2021 06:30:06 GMT  
		Size: 920.2 KB (920161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94d01cc79a56520493896d5bece03f2d44c526cc9a2de90982095eb600e8b1f6`  
		Last Modified: Thu, 22 Jul 2021 06:30:06 GMT  
		Size: 348.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:516d299b28d2cb1ab630cde4a763cbfc7be6f2863235a2a3dbfa4d9144bb1450`  
		Last Modified: Thu, 22 Jul 2021 06:30:06 GMT  
		Size: 294.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96077293611e1d84c5dedc398d9e3a86a42d5f9078f836055b3cb1b87e4be320`  
		Last Modified: Thu, 22 Jul 2021 06:30:28 GMT  
		Size: 211.3 MB (211349615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
