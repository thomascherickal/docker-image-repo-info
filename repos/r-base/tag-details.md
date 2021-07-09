<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `r-base`

-	[`r-base:4.1.0`](#r-base410)
-	[`r-base:latest`](#r-baselatest)

## `r-base:4.1.0`

```console
$ docker pull r-base@sha256:5f0ec1c795178fdcc89c8e69515dafbccf5dcdfca15d516dcb24298c2ca99523
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `r-base:4.1.0` - linux; amd64

```console
$ docker pull r-base@sha256:7f183f8dfb2335437e2509d43b1fa2561ba64b12c00f5936dfcafbf551ece8b6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **324.9 MB (324879129 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:27db47940ea4cefa1b2ec051d442290954260a1602c3a75916d309cb10673b1c`
-	Default Command: `["R"]`

```dockerfile
# Wed, 23 Jun 2021 00:22:26 GMT
ADD file:11d79229fbf81be2e84ec81659988987938f28988fef7b98793d53f36f1210ae in / 
# Wed, 23 Jun 2021 00:22:27 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 14:31:48 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Wed, 23 Jun 2021 14:31:51 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Wed, 23 Jun 2021 14:32:17 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 14:32:22 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Wed, 23 Jun 2021 14:32:22 GMT
ENV LC_ALL=en_US.UTF-8
# Wed, 23 Jun 2021 14:32:22 GMT
ENV LANG=en_US.UTF-8
# Wed, 23 Jun 2021 14:32:25 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Wed, 23 Jun 2021 14:32:25 GMT
ENV R_BASE_VERSION=4.1.0
# Wed, 23 Jun 2021 14:32:28 GMT
RUN echo "deb http://deb.debian.org/debian experimental main" > /etc/apt/sources.list.d/experimental.list     && echo "deb [trusted=yes] https://eddelbuettel.github.io/ppaR400 ./" > /etc/apt/sources.list.d/edd-r4.list
# Wed, 23 Jun 2021 14:33:44 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 14:33:45 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:e767ccb423aefb5241f61d2fd04a45363ff299f39c6474bbbb5a95ef4daace9f`  
		Last Modified: Wed, 23 Jun 2021 00:28:54 GMT  
		Size: 54.9 MB (54898130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c63c5328d0b617dd46ce7e4ec2b6ee5333d9972b786cedfb59f5fc6f213b164`  
		Last Modified: Wed, 23 Jun 2021 14:34:09 GMT  
		Size: 1.9 KB (1876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8c042150f8191e8bab3e76c171f584b3e76f94cd878a1e1b3466b98d6540f7d`  
		Last Modified: Wed, 23 Jun 2021 14:34:10 GMT  
		Size: 25.6 MB (25628090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d94290a7c04f9ce6cc6f441723937dd5e25d6ebb989b74d8dfedce56c2eab9f`  
		Last Modified: Wed, 23 Jun 2021 14:34:07 GMT  
		Size: 864.6 KB (864588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aeea435c0602304139d80ef36841b147d7d9ea71c3b2d804e0c6da5170663f3`  
		Last Modified: Wed, 23 Jun 2021 14:34:06 GMT  
		Size: 352.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed826a662be77d3b6519b85b11da187ca67edd3935eac70c0e94570cab9086cb`  
		Last Modified: Wed, 23 Jun 2021 14:34:06 GMT  
		Size: 295.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:573831cfb5cfa5e85ba7723b9ccdffb4066ab39de353d0adcef1797d705f4491`  
		Last Modified: Wed, 23 Jun 2021 14:34:38 GMT  
		Size: 243.5 MB (243485798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:4.1.0` - linux; arm64 variant v8

```console
$ docker pull r-base@sha256:c4ed93854f686fb0ec2f21e5ba793a6e53a9d95b184bb582701c434104ce91ae
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **312.3 MB (312346537 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b2716b67370d2f8a47922f4975a47fcc555945ba7b0f9bb8ecfc8ba96544b0b5`
-	Default Command: `["R"]`

```dockerfile
# Tue, 22 Jun 2021 23:51:21 GMT
ADD file:8b33a86eaea1ccad9ad34b736951d7b1fc6ad3dfe7fb2a6b433c966b551ec8f8 in / 
# Tue, 22 Jun 2021 23:51:22 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 12:31:08 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Wed, 23 Jun 2021 12:31:09 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Wed, 23 Jun 2021 12:31:19 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 12:31:22 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Wed, 23 Jun 2021 12:31:22 GMT
ENV LC_ALL=en_US.UTF-8
# Wed, 23 Jun 2021 12:31:22 GMT
ENV LANG=en_US.UTF-8
# Wed, 23 Jun 2021 12:31:23 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Wed, 23 Jun 2021 12:31:23 GMT
ENV R_BASE_VERSION=4.1.0
# Wed, 23 Jun 2021 12:31:24 GMT
RUN echo "deb http://deb.debian.org/debian experimental main" > /etc/apt/sources.list.d/experimental.list     && echo "deb [trusted=yes] https://eddelbuettel.github.io/ppaR400 ./" > /etc/apt/sources.list.d/edd-r4.list
# Wed, 23 Jun 2021 12:32:17 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 12:32:19 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:ebccb1b0cca36e353580d8c119fa9002e5804d4069c1f1c0f2fd0e41fc820a79`  
		Last Modified: Tue, 22 Jun 2021 23:58:47 GMT  
		Size: 53.6 MB (53581906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b4a1d2316257aff6fb13df61bf9aa39ad48d27c1d23208a466d3d148b962303`  
		Last Modified: Wed, 23 Jun 2021 12:32:44 GMT  
		Size: 1.9 KB (1877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc0a6eed952e2d30fb0ba9fae1c7d53aa883a6fddaf2a0f957aa33b03acfb2e9`  
		Last Modified: Wed, 23 Jun 2021 12:32:45 GMT  
		Size: 25.6 MB (25631135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b302a3135f6e267164a011340d9077b4296f42b4ca0023b2b2240ac8beef0951`  
		Last Modified: Wed, 23 Jun 2021 12:32:42 GMT  
		Size: 864.6 KB (864590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee6f6dbf87d40d9df6830802a40c398b040c0c7a8db380e69d445a03a8e5de4f`  
		Last Modified: Wed, 23 Jun 2021 12:32:41 GMT  
		Size: 351.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b346c36dc5a9b2d3798c908273d5fe1fd689c0fe5034f9091d50cc985ed2be6`  
		Last Modified: Wed, 23 Jun 2021 12:32:42 GMT  
		Size: 295.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c512b6cddc2ef85c46b75d59e8f850911146ecd2e3faf2955e182d162d819c44`  
		Last Modified: Wed, 23 Jun 2021 12:33:13 GMT  
		Size: 232.3 MB (232266383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:4.1.0` - linux; ppc64le

```console
$ docker pull r-base@sha256:2f418f29b5f45475dd037c88230d7b6e183065b1eb0b4a965c23ca56d7ed7a6f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **322.6 MB (322583225 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92ac411a77daa0f183b9a859752a220c47880bb6b0dcdb5be63f6dab1600ca31`
-	Default Command: `["R"]`

```dockerfile
# Wed, 23 Jun 2021 00:32:46 GMT
ADD file:28656f702990628f6d707772374ea01524be92a90a4933972d4d211cb573d675 in / 
# Wed, 23 Jun 2021 00:32:55 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 15:26:13 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Wed, 23 Jun 2021 15:26:36 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Wed, 23 Jun 2021 15:28:14 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 15:28:31 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Wed, 23 Jun 2021 15:28:36 GMT
ENV LC_ALL=en_US.UTF-8
# Wed, 23 Jun 2021 15:28:47 GMT
ENV LANG=en_US.UTF-8
# Wed, 23 Jun 2021 15:29:11 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Wed, 23 Jun 2021 15:29:24 GMT
ENV R_BASE_VERSION=4.1.0
# Wed, 23 Jun 2021 15:29:36 GMT
RUN echo "deb http://deb.debian.org/debian experimental main" > /etc/apt/sources.list.d/experimental.list     && echo "deb [trusted=yes] https://eddelbuettel.github.io/ppaR400 ./" > /etc/apt/sources.list.d/edd-r4.list
# Wed, 23 Jun 2021 15:38:13 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 15:38:37 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:7e3a7c042d8a7a01b6075e7fecff62a88da28cdebf0fd80952fc3d6159d785b4`  
		Last Modified: Wed, 23 Jun 2021 00:38:58 GMT  
		Size: 58.8 MB (58810879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68fb776660b0f301d0929cd4dd8c3ef6dca69731e59eb02da01a72de8d572d51`  
		Last Modified: Wed, 23 Jun 2021 15:39:05 GMT  
		Size: 1.9 KB (1890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d971946b3968661f0f08d1975536783bc3fe3823d58a1fe8e75dffcdbebc7adc`  
		Last Modified: Wed, 23 Jun 2021 15:39:06 GMT  
		Size: 25.9 MB (25852546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6caaddf9decb218a122dca999845b120203b8bcbe5b50cf45cb2dbca146c2692`  
		Last Modified: Wed, 23 Jun 2021 15:39:01 GMT  
		Size: 864.6 KB (864596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1be0673fc9487eb39277a17ba14f6798104344212d3b4ee5af4b8f4adf1441ad`  
		Last Modified: Wed, 23 Jun 2021 15:39:01 GMT  
		Size: 351.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f0d073677d022f65434e5b600ea300d596f7832ce097187a7dbdcc58f17339e`  
		Last Modified: Wed, 23 Jun 2021 15:39:01 GMT  
		Size: 295.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a33f0f3765090bfebc4ffe3b2ba49de68c3ba17bf11339772548ee27cace4153`  
		Last Modified: Wed, 23 Jun 2021 15:39:40 GMT  
		Size: 237.1 MB (237052668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:4.1.0` - linux; s390x

```console
$ docker pull r-base@sha256:4b651c210d4dc81c31f55cf29bdc1ccd89d6dcd5a9800d2916fd19e2ebb275a8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **291.1 MB (291087036 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41662975e6bf2f4a8bbae0436a31b16fc8e299aafc74a3d2c9763ac62929cc47`
-	Default Command: `["R"]`

```dockerfile
# Fri, 09 Jul 2021 02:51:46 GMT
ADD file:facd85bf99201bf801c84cbad25dd5ea3044aa2a35468e8238d75094a32b5f00 in / 
# Fri, 09 Jul 2021 02:51:49 GMT
CMD ["bash"]
# Fri, 09 Jul 2021 13:10:38 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Fri, 09 Jul 2021 13:10:41 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Fri, 09 Jul 2021 13:11:14 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Fri, 09 Jul 2021 13:11:20 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Fri, 09 Jul 2021 13:11:21 GMT
ENV LC_ALL=en_US.UTF-8
# Fri, 09 Jul 2021 13:11:22 GMT
ENV LANG=en_US.UTF-8
# Fri, 09 Jul 2021 13:11:24 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Fri, 09 Jul 2021 13:11:25 GMT
ENV R_BASE_VERSION=4.1.0
# Fri, 09 Jul 2021 13:11:27 GMT
RUN echo "deb http://deb.debian.org/debian experimental main" > /etc/apt/sources.list.d/experimental.list     && echo "deb [trusted=yes] https://eddelbuettel.github.io/ppaR400 ./" > /etc/apt/sources.list.d/edd-r4.list
# Fri, 09 Jul 2021 13:14:24 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Fri, 09 Jul 2021 13:14:44 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:57de50423b857ec03e5f5da3355e55ed7303841fa03258a82be273a6f2046de9`  
		Last Modified: Tue, 22 Jun 2021 23:46:48 GMT  
		Size: 53.2 MB (53183178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8b7636808066c10a27b9f7b2e001b1203c07c05d262848c870456b1bb83600a`  
		Last Modified: Fri, 09 Jul 2021 13:15:12 GMT  
		Size: 1.9 KB (1888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce74a817dff2523b782a96ed020ae5055f14c0a4ee9eac09b0f3976243aa0868`  
		Last Modified: Fri, 09 Jul 2021 13:15:13 GMT  
		Size: 25.6 MB (25631764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d027473a7fec7d34926830e2a5784e22915fefa1a91900138ed5d12675c4f08`  
		Last Modified: Fri, 09 Jul 2021 13:15:11 GMT  
		Size: 920.2 KB (920166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7150e17de2729fa905bb066784484feef83c7a33653c90908b733d44a602f9f6`  
		Last Modified: Fri, 09 Jul 2021 13:15:10 GMT  
		Size: 352.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10ff76a0f527f13e1abaff37156237998f97b9e5e6ff3d70685a40f5eab300d4`  
		Last Modified: Fri, 09 Jul 2021 13:15:10 GMT  
		Size: 296.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27f03005b49484fff8d8f963046fced68a640997dd88c37a1f77bd255596b0a0`  
		Last Modified: Fri, 09 Jul 2021 13:15:34 GMT  
		Size: 211.3 MB (211349392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `r-base:latest`

```console
$ docker pull r-base@sha256:5f0ec1c795178fdcc89c8e69515dafbccf5dcdfca15d516dcb24298c2ca99523
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `r-base:latest` - linux; amd64

```console
$ docker pull r-base@sha256:7f183f8dfb2335437e2509d43b1fa2561ba64b12c00f5936dfcafbf551ece8b6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **324.9 MB (324879129 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:27db47940ea4cefa1b2ec051d442290954260a1602c3a75916d309cb10673b1c`
-	Default Command: `["R"]`

```dockerfile
# Wed, 23 Jun 2021 00:22:26 GMT
ADD file:11d79229fbf81be2e84ec81659988987938f28988fef7b98793d53f36f1210ae in / 
# Wed, 23 Jun 2021 00:22:27 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 14:31:48 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Wed, 23 Jun 2021 14:31:51 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Wed, 23 Jun 2021 14:32:17 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 14:32:22 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Wed, 23 Jun 2021 14:32:22 GMT
ENV LC_ALL=en_US.UTF-8
# Wed, 23 Jun 2021 14:32:22 GMT
ENV LANG=en_US.UTF-8
# Wed, 23 Jun 2021 14:32:25 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Wed, 23 Jun 2021 14:32:25 GMT
ENV R_BASE_VERSION=4.1.0
# Wed, 23 Jun 2021 14:32:28 GMT
RUN echo "deb http://deb.debian.org/debian experimental main" > /etc/apt/sources.list.d/experimental.list     && echo "deb [trusted=yes] https://eddelbuettel.github.io/ppaR400 ./" > /etc/apt/sources.list.d/edd-r4.list
# Wed, 23 Jun 2021 14:33:44 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 14:33:45 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:e767ccb423aefb5241f61d2fd04a45363ff299f39c6474bbbb5a95ef4daace9f`  
		Last Modified: Wed, 23 Jun 2021 00:28:54 GMT  
		Size: 54.9 MB (54898130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c63c5328d0b617dd46ce7e4ec2b6ee5333d9972b786cedfb59f5fc6f213b164`  
		Last Modified: Wed, 23 Jun 2021 14:34:09 GMT  
		Size: 1.9 KB (1876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8c042150f8191e8bab3e76c171f584b3e76f94cd878a1e1b3466b98d6540f7d`  
		Last Modified: Wed, 23 Jun 2021 14:34:10 GMT  
		Size: 25.6 MB (25628090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d94290a7c04f9ce6cc6f441723937dd5e25d6ebb989b74d8dfedce56c2eab9f`  
		Last Modified: Wed, 23 Jun 2021 14:34:07 GMT  
		Size: 864.6 KB (864588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aeea435c0602304139d80ef36841b147d7d9ea71c3b2d804e0c6da5170663f3`  
		Last Modified: Wed, 23 Jun 2021 14:34:06 GMT  
		Size: 352.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed826a662be77d3b6519b85b11da187ca67edd3935eac70c0e94570cab9086cb`  
		Last Modified: Wed, 23 Jun 2021 14:34:06 GMT  
		Size: 295.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:573831cfb5cfa5e85ba7723b9ccdffb4066ab39de353d0adcef1797d705f4491`  
		Last Modified: Wed, 23 Jun 2021 14:34:38 GMT  
		Size: 243.5 MB (243485798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:latest` - linux; arm64 variant v8

```console
$ docker pull r-base@sha256:c4ed93854f686fb0ec2f21e5ba793a6e53a9d95b184bb582701c434104ce91ae
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **312.3 MB (312346537 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b2716b67370d2f8a47922f4975a47fcc555945ba7b0f9bb8ecfc8ba96544b0b5`
-	Default Command: `["R"]`

```dockerfile
# Tue, 22 Jun 2021 23:51:21 GMT
ADD file:8b33a86eaea1ccad9ad34b736951d7b1fc6ad3dfe7fb2a6b433c966b551ec8f8 in / 
# Tue, 22 Jun 2021 23:51:22 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 12:31:08 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Wed, 23 Jun 2021 12:31:09 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Wed, 23 Jun 2021 12:31:19 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 12:31:22 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Wed, 23 Jun 2021 12:31:22 GMT
ENV LC_ALL=en_US.UTF-8
# Wed, 23 Jun 2021 12:31:22 GMT
ENV LANG=en_US.UTF-8
# Wed, 23 Jun 2021 12:31:23 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Wed, 23 Jun 2021 12:31:23 GMT
ENV R_BASE_VERSION=4.1.0
# Wed, 23 Jun 2021 12:31:24 GMT
RUN echo "deb http://deb.debian.org/debian experimental main" > /etc/apt/sources.list.d/experimental.list     && echo "deb [trusted=yes] https://eddelbuettel.github.io/ppaR400 ./" > /etc/apt/sources.list.d/edd-r4.list
# Wed, 23 Jun 2021 12:32:17 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 12:32:19 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:ebccb1b0cca36e353580d8c119fa9002e5804d4069c1f1c0f2fd0e41fc820a79`  
		Last Modified: Tue, 22 Jun 2021 23:58:47 GMT  
		Size: 53.6 MB (53581906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b4a1d2316257aff6fb13df61bf9aa39ad48d27c1d23208a466d3d148b962303`  
		Last Modified: Wed, 23 Jun 2021 12:32:44 GMT  
		Size: 1.9 KB (1877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc0a6eed952e2d30fb0ba9fae1c7d53aa883a6fddaf2a0f957aa33b03acfb2e9`  
		Last Modified: Wed, 23 Jun 2021 12:32:45 GMT  
		Size: 25.6 MB (25631135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b302a3135f6e267164a011340d9077b4296f42b4ca0023b2b2240ac8beef0951`  
		Last Modified: Wed, 23 Jun 2021 12:32:42 GMT  
		Size: 864.6 KB (864590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee6f6dbf87d40d9df6830802a40c398b040c0c7a8db380e69d445a03a8e5de4f`  
		Last Modified: Wed, 23 Jun 2021 12:32:41 GMT  
		Size: 351.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b346c36dc5a9b2d3798c908273d5fe1fd689c0fe5034f9091d50cc985ed2be6`  
		Last Modified: Wed, 23 Jun 2021 12:32:42 GMT  
		Size: 295.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c512b6cddc2ef85c46b75d59e8f850911146ecd2e3faf2955e182d162d819c44`  
		Last Modified: Wed, 23 Jun 2021 12:33:13 GMT  
		Size: 232.3 MB (232266383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:latest` - linux; ppc64le

```console
$ docker pull r-base@sha256:2f418f29b5f45475dd037c88230d7b6e183065b1eb0b4a965c23ca56d7ed7a6f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **322.6 MB (322583225 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92ac411a77daa0f183b9a859752a220c47880bb6b0dcdb5be63f6dab1600ca31`
-	Default Command: `["R"]`

```dockerfile
# Wed, 23 Jun 2021 00:32:46 GMT
ADD file:28656f702990628f6d707772374ea01524be92a90a4933972d4d211cb573d675 in / 
# Wed, 23 Jun 2021 00:32:55 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 15:26:13 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Wed, 23 Jun 2021 15:26:36 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Wed, 23 Jun 2021 15:28:14 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 15:28:31 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Wed, 23 Jun 2021 15:28:36 GMT
ENV LC_ALL=en_US.UTF-8
# Wed, 23 Jun 2021 15:28:47 GMT
ENV LANG=en_US.UTF-8
# Wed, 23 Jun 2021 15:29:11 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Wed, 23 Jun 2021 15:29:24 GMT
ENV R_BASE_VERSION=4.1.0
# Wed, 23 Jun 2021 15:29:36 GMT
RUN echo "deb http://deb.debian.org/debian experimental main" > /etc/apt/sources.list.d/experimental.list     && echo "deb [trusted=yes] https://eddelbuettel.github.io/ppaR400 ./" > /etc/apt/sources.list.d/edd-r4.list
# Wed, 23 Jun 2021 15:38:13 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 15:38:37 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:7e3a7c042d8a7a01b6075e7fecff62a88da28cdebf0fd80952fc3d6159d785b4`  
		Last Modified: Wed, 23 Jun 2021 00:38:58 GMT  
		Size: 58.8 MB (58810879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68fb776660b0f301d0929cd4dd8c3ef6dca69731e59eb02da01a72de8d572d51`  
		Last Modified: Wed, 23 Jun 2021 15:39:05 GMT  
		Size: 1.9 KB (1890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d971946b3968661f0f08d1975536783bc3fe3823d58a1fe8e75dffcdbebc7adc`  
		Last Modified: Wed, 23 Jun 2021 15:39:06 GMT  
		Size: 25.9 MB (25852546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6caaddf9decb218a122dca999845b120203b8bcbe5b50cf45cb2dbca146c2692`  
		Last Modified: Wed, 23 Jun 2021 15:39:01 GMT  
		Size: 864.6 KB (864596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1be0673fc9487eb39277a17ba14f6798104344212d3b4ee5af4b8f4adf1441ad`  
		Last Modified: Wed, 23 Jun 2021 15:39:01 GMT  
		Size: 351.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f0d073677d022f65434e5b600ea300d596f7832ce097187a7dbdcc58f17339e`  
		Last Modified: Wed, 23 Jun 2021 15:39:01 GMT  
		Size: 295.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a33f0f3765090bfebc4ffe3b2ba49de68c3ba17bf11339772548ee27cace4153`  
		Last Modified: Wed, 23 Jun 2021 15:39:40 GMT  
		Size: 237.1 MB (237052668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:latest` - linux; s390x

```console
$ docker pull r-base@sha256:4b651c210d4dc81c31f55cf29bdc1ccd89d6dcd5a9800d2916fd19e2ebb275a8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **291.1 MB (291087036 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41662975e6bf2f4a8bbae0436a31b16fc8e299aafc74a3d2c9763ac62929cc47`
-	Default Command: `["R"]`

```dockerfile
# Fri, 09 Jul 2021 02:51:46 GMT
ADD file:facd85bf99201bf801c84cbad25dd5ea3044aa2a35468e8238d75094a32b5f00 in / 
# Fri, 09 Jul 2021 02:51:49 GMT
CMD ["bash"]
# Fri, 09 Jul 2021 13:10:38 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Fri, 09 Jul 2021 13:10:41 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Fri, 09 Jul 2021 13:11:14 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Fri, 09 Jul 2021 13:11:20 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Fri, 09 Jul 2021 13:11:21 GMT
ENV LC_ALL=en_US.UTF-8
# Fri, 09 Jul 2021 13:11:22 GMT
ENV LANG=en_US.UTF-8
# Fri, 09 Jul 2021 13:11:24 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Fri, 09 Jul 2021 13:11:25 GMT
ENV R_BASE_VERSION=4.1.0
# Fri, 09 Jul 2021 13:11:27 GMT
RUN echo "deb http://deb.debian.org/debian experimental main" > /etc/apt/sources.list.d/experimental.list     && echo "deb [trusted=yes] https://eddelbuettel.github.io/ppaR400 ./" > /etc/apt/sources.list.d/edd-r4.list
# Fri, 09 Jul 2021 13:14:24 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Fri, 09 Jul 2021 13:14:44 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:57de50423b857ec03e5f5da3355e55ed7303841fa03258a82be273a6f2046de9`  
		Last Modified: Tue, 22 Jun 2021 23:46:48 GMT  
		Size: 53.2 MB (53183178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8b7636808066c10a27b9f7b2e001b1203c07c05d262848c870456b1bb83600a`  
		Last Modified: Fri, 09 Jul 2021 13:15:12 GMT  
		Size: 1.9 KB (1888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce74a817dff2523b782a96ed020ae5055f14c0a4ee9eac09b0f3976243aa0868`  
		Last Modified: Fri, 09 Jul 2021 13:15:13 GMT  
		Size: 25.6 MB (25631764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d027473a7fec7d34926830e2a5784e22915fefa1a91900138ed5d12675c4f08`  
		Last Modified: Fri, 09 Jul 2021 13:15:11 GMT  
		Size: 920.2 KB (920166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7150e17de2729fa905bb066784484feef83c7a33653c90908b733d44a602f9f6`  
		Last Modified: Fri, 09 Jul 2021 13:15:10 GMT  
		Size: 352.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10ff76a0f527f13e1abaff37156237998f97b9e5e6ff3d70685a40f5eab300d4`  
		Last Modified: Fri, 09 Jul 2021 13:15:10 GMT  
		Size: 296.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27f03005b49484fff8d8f963046fced68a640997dd88c37a1f77bd255596b0a0`  
		Last Modified: Fri, 09 Jul 2021 13:15:34 GMT  
		Size: 211.3 MB (211349392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
