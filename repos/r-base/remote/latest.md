## `r-base:latest`

```console
$ docker pull r-base@sha256:689bf9b6c3274cafb30e657374c08e9a8bde7bca9fbec8be5053395c67b57083
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `r-base:latest` - linux; amd64

```console
$ docker pull r-base@sha256:06979524919e444f50cf01c8e37403a90c7d06daf988c206c3236049f75fe3bd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **339.7 MB (339689239 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e64c713b3583c7003979857f85f2403af438d778f02022cf780e6f380ca1abcf`
-	Default Command: `["R"]`

```dockerfile
# Wed, 11 Oct 2023 18:37:09 GMT
ADD file:21d38a28e0614f04476d0dca2e0eb55defa5f216a30c05c084c97d6d1fa90e30 in / 
# Wed, 11 Oct 2023 18:37:10 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 03:12:02 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Thu, 12 Oct 2023 03:12:03 GMT
RUN useradd -s /bin/bash -m docker 	&& usermod -a -G staff docker
# Thu, 12 Oct 2023 03:12:14 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 03:12:16 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Thu, 12 Oct 2023 03:12:16 GMT
ENV LC_ALL=en_US.UTF-8
# Thu, 12 Oct 2023 03:12:16 GMT
ENV LANG=en_US.UTF-8
# Thu, 12 Oct 2023 03:12:17 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Thu, 12 Oct 2023 03:12:17 GMT
ENV R_BASE_VERSION=4.3.1
# Thu, 12 Oct 2023 03:13:17 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-docopt                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& chown root:staff "/usr/local/lib/R/site-library" 	&& chmod g+ws "/usr/local/lib/R/site-library" 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 03:13:19 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:4b9e93079e042882107af07d114a4c10a8202361c63fbdce4fc863cd7942e65e`  
		Last Modified: Wed, 11 Oct 2023 18:43:34 GMT  
		Size: 49.5 MB (49502114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a3abc00097ca006fedf22776c231e2545fd41f2432d13fa20630f8066fb1b28`  
		Last Modified: Thu, 12 Oct 2023 03:13:31 GMT  
		Size: 3.4 KB (3361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fe8cc404d321c25adc422d19c121f41aa88609c90df0646e1d50661b0d45f64`  
		Last Modified: Thu, 12 Oct 2023 03:13:34 GMT  
		Size: 25.5 MB (25517750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aefbc40b273a0602aaff7ebf3927d359b4b35b478a0404c6f875c0642e69a632`  
		Last Modified: Thu, 12 Oct 2023 03:13:32 GMT  
		Size: 866.3 KB (866326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6de485d51833927eeffeba8297f3c9331260d41e2de8391fc3d0a37699701f3e`  
		Last Modified: Thu, 12 Oct 2023 03:13:31 GMT  
		Size: 349.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:027a08c976628a0a366eea2ab6923e995d675b63353914bbb811b55efbf0ea1a`  
		Last Modified: Thu, 12 Oct 2023 03:14:00 GMT  
		Size: 263.8 MB (263799339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:latest` - linux; arm64 variant v8

```console
$ docker pull r-base@sha256:8880164830d7cff80b95c4e5268ccccbe228ea293e88c1fceeb0c93e298d247c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **328.0 MB (328044094 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e16ff4028f486367d4102dbec06d2bfbe16e3113ed571ce15cbcf640a6780d1`
-	Default Command: `["R"]`

```dockerfile
# Wed, 11 Oct 2023 18:26:23 GMT
ADD file:c48ddb3be6db73fb74475f132903784b2239816dcf46a967c1bfb0f8a23fd0bb in / 
# Wed, 11 Oct 2023 18:26:23 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 10:09:17 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Thu, 12 Oct 2023 10:09:18 GMT
RUN useradd -s /bin/bash -m docker 	&& usermod -a -G staff docker
# Thu, 12 Oct 2023 10:09:28 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 10:09:30 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Thu, 12 Oct 2023 10:09:30 GMT
ENV LC_ALL=en_US.UTF-8
# Thu, 12 Oct 2023 10:09:30 GMT
ENV LANG=en_US.UTF-8
# Thu, 12 Oct 2023 10:09:31 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Tue, 31 Oct 2023 23:57:41 GMT
ENV R_BASE_VERSION=4.3.2
# Tue, 31 Oct 2023 23:58:50 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-docopt                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& chown root:staff "/usr/local/lib/R/site-library" 	&& chmod g+ws "/usr/local/lib/R/site-library" 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Oct 2023 23:58:54 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:484b389f95af6a0503d73ac652b29ef33a2d2fbb6e295f8bbe656d503a592a3a`  
		Last Modified: Wed, 11 Oct 2023 18:32:10 GMT  
		Size: 49.5 MB (49505546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f70272f1692c9b4f82ef47a9cf030b16fcf04ba6e41714d479d7e3bd53d1e28`  
		Last Modified: Thu, 12 Oct 2023 10:10:45 GMT  
		Size: 3.4 KB (3361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de85415d442decef501bde5fc680d6243552b2ad6415fa30678ade91a6fae187`  
		Last Modified: Thu, 12 Oct 2023 10:10:48 GMT  
		Size: 25.4 MB (25358078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71ed2dad41a93e49b56e4cac1f9350988542196eb096a932846fddb4efc6daad`  
		Last Modified: Thu, 12 Oct 2023 10:10:45 GMT  
		Size: 866.3 KB (866330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d61c476288523fd5e434fc762a49df0e3beccd99114bbdc0e9b7e8c5c1e244d`  
		Last Modified: Thu, 12 Oct 2023 10:10:45 GMT  
		Size: 351.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39f1ca7f0aaa0c47dba5df9576249cd1cf78143f079f9ddf735ec6736e19f2d0`  
		Last Modified: Tue, 31 Oct 2023 23:59:32 GMT  
		Size: 252.3 MB (252310428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:latest` - linux; ppc64le

```console
$ docker pull r-base@sha256:eec77e079184125ee915d002d2160b132881557f8dc702d90481f63cc48dc56f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **338.5 MB (338455037 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9adddf0ae88a79c1312345fd0bdd38e4a579c50991d78ea91168a50c5ac694a6`
-	Default Command: `["R"]`

```dockerfile
# Wed, 11 Oct 2023 17:46:50 GMT
ADD file:c877fccf97ee8f77aa2318c5d5fc9deea9905e038d11730ba52d9dd50217738d in / 
# Wed, 11 Oct 2023 17:46:52 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 05:35:47 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Thu, 12 Oct 2023 05:35:50 GMT
RUN useradd -s /bin/bash -m docker 	&& usermod -a -G staff docker
# Thu, 12 Oct 2023 05:36:14 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 05:36:19 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Thu, 12 Oct 2023 05:36:19 GMT
ENV LC_ALL=en_US.UTF-8
# Thu, 12 Oct 2023 05:36:19 GMT
ENV LANG=en_US.UTF-8
# Thu, 12 Oct 2023 05:36:21 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Thu, 12 Oct 2023 05:36:22 GMT
ENV R_BASE_VERSION=4.3.1
# Thu, 12 Oct 2023 05:39:01 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-docopt                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& chown root:staff "/usr/local/lib/R/site-library" 	&& chmod g+ws "/usr/local/lib/R/site-library" 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 05:39:10 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:3aaaa4d84036ee17b7ad898e0a13bebade18f92f2c7561f3d407624d1bb0da74`  
		Last Modified: Wed, 11 Oct 2023 17:53:38 GMT  
		Size: 53.4 MB (53418133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50a5aa4e8f078cf4132db1d6ba604c93b0704a9a9c4204504e1660270e1b9f79`  
		Last Modified: Thu, 12 Oct 2023 05:39:33 GMT  
		Size: 3.4 KB (3361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c6089261485c8bd6f607eb5d5b625d3a36c93e67ddbcd0000c9b8d5d8f61070`  
		Last Modified: Thu, 12 Oct 2023 05:39:38 GMT  
		Size: 25.9 MB (25910254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1345cfd388d27cade0394dfe09e741f02b2d985dce00749866652adb729759e3`  
		Last Modified: Thu, 12 Oct 2023 05:39:33 GMT  
		Size: 866.3 KB (866324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a1caf9ef78ffc13cf4a258c76afff5df590bd089c2411b6fca75413deb2bc1b`  
		Last Modified: Thu, 12 Oct 2023 05:39:33 GMT  
		Size: 351.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40c39e88e5f9c317c8f84d5e9d7b0bd7cf9b4609a661c244d1da31f407bffa94`  
		Last Modified: Thu, 12 Oct 2023 05:40:25 GMT  
		Size: 258.3 MB (258256614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:latest` - linux; s390x

```console
$ docker pull r-base@sha256:ace281f31ec194ea9c010406969f925f52d58b728fc8ecfafe114760eaa42bb0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **308.1 MB (308068983 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:58a0eb24e0cd08376db20b9128a7baf47185e02143d44f26aa1d51a327f20926`
-	Default Command: `["R"]`

```dockerfile
# Wed, 11 Oct 2023 17:52:40 GMT
ADD file:9bdb90e9fc1ff4c63bcf3d994b2211b30b462d560247548fc2e3493704b91c5b in / 
# Wed, 11 Oct 2023 17:52:43 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 09:43:09 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Thu, 12 Oct 2023 09:43:09 GMT
RUN useradd -s /bin/bash -m docker 	&& usermod -a -G staff docker
# Thu, 12 Oct 2023 09:43:33 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 09:43:36 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Thu, 12 Oct 2023 09:43:36 GMT
ENV LC_ALL=en_US.UTF-8
# Thu, 12 Oct 2023 09:43:36 GMT
ENV LANG=en_US.UTF-8
# Thu, 12 Oct 2023 09:43:37 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Tue, 31 Oct 2023 23:50:12 GMT
ENV R_BASE_VERSION=4.3.2
# Tue, 31 Oct 2023 23:50:57 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-docopt                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& chown root:staff "/usr/local/lib/R/site-library" 	&& chmod g+ws "/usr/local/lib/R/site-library" 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Oct 2023 23:51:07 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:02a6d6b749a80726477cd9a1565b54a7b73acee565b6c727afa20dc76f42a0a7`  
		Last Modified: Wed, 11 Oct 2023 18:00:50 GMT  
		Size: 48.9 MB (48924341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a64b4280bc5ee57d2e5be499e6f68994e2ec281ee9b3848500742b98c6a8ab7e`  
		Last Modified: Thu, 12 Oct 2023 09:46:51 GMT  
		Size: 3.4 KB (3357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe39616558184d901352914b72c23820f65ff261010203c387ffb587517ca126`  
		Last Modified: Thu, 12 Oct 2023 09:46:55 GMT  
		Size: 25.4 MB (25362924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cbb7527603d9af6d4a56322a084adf5845de5addbea1de7ff45b291b2872f1e`  
		Last Modified: Thu, 12 Oct 2023 09:46:52 GMT  
		Size: 922.3 KB (922277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:703815f047b55c5fc0af48b408742d44691b23d14f107203b3bc692ce04ea280`  
		Last Modified: Thu, 12 Oct 2023 09:46:51 GMT  
		Size: 350.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6471ed1b1cca464b40e9c555ff2ca8aeef66e326dc406dd552f99cd96e20daad`  
		Last Modified: Tue, 31 Oct 2023 23:51:50 GMT  
		Size: 232.9 MB (232855734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
