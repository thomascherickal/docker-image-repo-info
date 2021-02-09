## `r-base:latest`

```console
$ docker pull r-base@sha256:497d5e9fcd96981b07da6c118bc97a6998a67e3d67c14b4df0332c0e5d7662f8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `r-base:latest` - linux; amd64

```console
$ docker pull r-base@sha256:9737d0c00160f483c09415336e34cb9bad01571c1feac93c0a5e5eb40ed84268
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **323.8 MB (323787075 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab694d121fd77e4f9abf6b19c8e46306ca842b3be1d218e775befd9e31c6e6cf`
-	Default Command: `["R"]`

```dockerfile
# Tue, 09 Feb 2021 02:23:42 GMT
ADD file:82b8788c604afb731f2703bfae955205d5f6f72d5294fd0f4867dac49640e1b4 in / 
# Tue, 09 Feb 2021 02:23:42 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 09:54:17 GMT
LABEL org.label-schema.license=GPL-2.0 org.label-schema.vcs-url=https://github.com/rocker-org/r-base org.label-schema.vendor=Rocker Project maintainer=Dirk Eddelbuettel <edd@debian.org>
# Tue, 09 Feb 2021 09:54:18 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Tue, 09 Feb 2021 09:54:29 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 09:54:32 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Tue, 09 Feb 2021 09:54:33 GMT
ENV LC_ALL=en_US.UTF-8
# Tue, 09 Feb 2021 09:54:33 GMT
ENV LANG=en_US.UTF-8
# Tue, 09 Feb 2021 09:54:34 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Tue, 09 Feb 2021 09:54:34 GMT
ENV R_BASE_VERSION=4.0.3
# Tue, 09 Feb 2021 09:55:41 GMT
RUN apt-get update         && apt-get install -t unstable -y --no-install-recommends                 gcc-9-base                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 09:55:42 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:159b898d862319846f1877e5fae72b393710e31b7cfc6406fe856ded8dac3a55`  
		Last Modified: Tue, 09 Feb 2021 02:29:52 GMT  
		Size: 54.8 MB (54757731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ab79e2223b072d16a78ae62040f573111dbb2fe25063a8964f9a6c3d71fe099`  
		Last Modified: Tue, 09 Feb 2021 09:55:53 GMT  
		Size: 1.9 KB (1855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:860eda86c9b7f0af1e065a0857a6512adf8fcf6e9ae247b6ebb1fb4c77d44fe6`  
		Last Modified: Tue, 09 Feb 2021 09:56:00 GMT  
		Size: 25.6 MB (25623535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70fdb5e53c53ae3da98312f4529de40508f87ba484a0ebcd6cca3ef09f0f3982`  
		Last Modified: Tue, 09 Feb 2021 09:55:53 GMT  
		Size: 864.6 KB (864593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b53c137bdbe8c7d19665096ed361ae4b0df0a121bbff3f8f6d8da3c3d0d09e5`  
		Last Modified: Tue, 09 Feb 2021 09:55:53 GMT  
		Size: 351.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c6ef537a6dd44243e14a5e244a0e22ee53aa9b8f801613ef8bb397d97931257`  
		Last Modified: Tue, 09 Feb 2021 09:56:48 GMT  
		Size: 242.5 MB (242539010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:latest` - linux; arm64 variant v8

```console
$ docker pull r-base@sha256:6187381a137b751960df4d4b2d2504ca1867de9285035b098e0511bc79d9da71
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **311.4 MB (311407092 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f516b6996414f3e6dde0ac7354f40990c3e37e26c7e940c54734a4fc90b87f4`
-	Default Command: `["R"]`

```dockerfile
# Tue, 09 Feb 2021 02:43:54 GMT
ADD file:409b68622e71f79b15ce6f8c2ba229eae8804eae96c108909904c9262ac92813 in / 
# Tue, 09 Feb 2021 02:43:57 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 17:31:26 GMT
LABEL org.label-schema.license=GPL-2.0 org.label-schema.vcs-url=https://github.com/rocker-org/r-base org.label-schema.vendor=Rocker Project maintainer=Dirk Eddelbuettel <edd@debian.org>
# Tue, 09 Feb 2021 17:31:29 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Tue, 09 Feb 2021 17:31:48 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 17:31:54 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Tue, 09 Feb 2021 17:31:54 GMT
ENV LC_ALL=en_US.UTF-8
# Tue, 09 Feb 2021 17:31:55 GMT
ENV LANG=en_US.UTF-8
# Tue, 09 Feb 2021 17:31:57 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Tue, 09 Feb 2021 17:31:58 GMT
ENV R_BASE_VERSION=4.0.3
# Tue, 09 Feb 2021 17:33:35 GMT
RUN apt-get update         && apt-get install -t unstable -y --no-install-recommends                 gcc-9-base                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 17:33:40 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:96558920c85c4f4f52587e2769e7ae3827f29ff19f346cfb913b61e696a9287a`  
		Last Modified: Tue, 09 Feb 2021 02:50:32 GMT  
		Size: 53.4 MB (53428409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b6ab6587c7798b572a801e60224c0f03380078950473a85aab90e65e69cfa13`  
		Last Modified: Tue, 09 Feb 2021 17:34:06 GMT  
		Size: 1.9 KB (1885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a204add6d8185cf59f7ff59b85adeb9c628de078ee4b4441713c13cbefb7f563`  
		Last Modified: Tue, 09 Feb 2021 17:34:12 GMT  
		Size: 25.6 MB (25620624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8bf43358bc1cc73f526872792c2b1518ece24742fc56472f619aec592b86be4`  
		Last Modified: Tue, 09 Feb 2021 17:34:06 GMT  
		Size: 864.6 KB (864592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f17e1327c3fce9f0476a25e7e0e577749961cfffab7d29633172c2cd3032dee4`  
		Last Modified: Tue, 09 Feb 2021 17:34:06 GMT  
		Size: 350.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a086b7c19d6169e69613931be3343f4b7ad9e888361a6d8ddbae396e9a277b77`  
		Last Modified: Tue, 09 Feb 2021 17:34:55 GMT  
		Size: 231.5 MB (231491232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:latest` - linux; ppc64le

```console
$ docker pull r-base@sha256:803cd460dd7a7cd659abe49874effe49565bcd7f43150d6332afd6ee18cdd223
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **321.6 MB (321616695 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d94730e92c8682bf12cf0a9fbeaf1c133ca2c2b937640427bb408651bdc801ac`
-	Default Command: `["R"]`

```dockerfile
# Tue, 09 Feb 2021 02:22:01 GMT
ADD file:b966d8a0637e4f8617405797940aae2bfca8fa7c2741dff346c04a7d2e46c711 in / 
# Tue, 09 Feb 2021 02:22:09 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 21:49:02 GMT
LABEL org.label-schema.license=GPL-2.0 org.label-schema.vcs-url=https://github.com/rocker-org/r-base org.label-schema.vendor=Rocker Project maintainer=Dirk Eddelbuettel <edd@debian.org>
# Tue, 09 Feb 2021 21:49:36 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Tue, 09 Feb 2021 21:51:22 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 21:51:40 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Tue, 09 Feb 2021 21:51:45 GMT
ENV LC_ALL=en_US.UTF-8
# Tue, 09 Feb 2021 21:51:51 GMT
ENV LANG=en_US.UTF-8
# Tue, 09 Feb 2021 21:52:04 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Tue, 09 Feb 2021 21:52:10 GMT
ENV R_BASE_VERSION=4.0.3
# Tue, 09 Feb 2021 22:03:09 GMT
RUN apt-get update         && apt-get install -t unstable -y --no-install-recommends                 gcc-9-base                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 22:03:17 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:c275bc88cf56a84204812c723aba51d584876a2c5cd58e37411fd1716dfb5602`  
		Last Modified: Tue, 09 Feb 2021 02:30:02 GMT  
		Size: 58.6 MB (58639014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66df3657f5e9fc36f6d822990b58589c8f0f697b5dc8ae3aede7e526854b8365`  
		Last Modified: Tue, 09 Feb 2021 22:03:45 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0219723e9ff09315c3555d4c0c1c814378e31bc6df586b63f540c71958845900`  
		Last Modified: Tue, 09 Feb 2021 22:03:49 GMT  
		Size: 25.8 MB (25840062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ddfcabf1e509d7ffeea6641f7c62ce6db86d0e9eb845d747cfe7f63f486da45`  
		Last Modified: Tue, 09 Feb 2021 22:03:45 GMT  
		Size: 864.6 KB (864594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ddf81373fbbe536e9283f40a32b7d14abc6955e3ea28de8282bf0944a23772b`  
		Last Modified: Tue, 09 Feb 2021 22:03:45 GMT  
		Size: 348.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0e8c240bf047ef7037995212858044ade5231debeaab5506ee8a6a3dc115726`  
		Last Modified: Tue, 09 Feb 2021 22:04:25 GMT  
		Size: 236.3 MB (236270795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:latest` - linux; s390x

```console
$ docker pull r-base@sha256:fa2bf03af0b48ca27a3057b4e01f74110fb3a4afabc444ccbdc509589a535622
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **290.1 MB (290136202 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7651a1724a18a2fcd54364dcad173afb1d6f54f1032833d065df82cdfd792cdd`
-	Default Command: `["R"]`

```dockerfile
# Tue, 09 Feb 2021 02:43:07 GMT
ADD file:a36ce31c894f715acdcc50e3f12103ad3a46c33a3dc3902cfab9145392f7ac0d in / 
# Tue, 09 Feb 2021 02:43:09 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 07:31:44 GMT
LABEL org.label-schema.license=GPL-2.0 org.label-schema.vcs-url=https://github.com/rocker-org/r-base org.label-schema.vendor=Rocker Project maintainer=Dirk Eddelbuettel <edd@debian.org>
# Tue, 09 Feb 2021 07:31:45 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Tue, 09 Feb 2021 07:31:55 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 07:31:57 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Tue, 09 Feb 2021 07:31:57 GMT
ENV LC_ALL=en_US.UTF-8
# Tue, 09 Feb 2021 07:31:57 GMT
ENV LANG=en_US.UTF-8
# Tue, 09 Feb 2021 07:31:58 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Tue, 09 Feb 2021 07:31:58 GMT
ENV R_BASE_VERSION=4.0.3
# Tue, 09 Feb 2021 07:32:53 GMT
RUN apt-get update         && apt-get install -t unstable -y --no-install-recommends                 gcc-9-base                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 07:33:00 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:304b8a99f74f95db1eef52b755fcfcaf4c2d5f8146606537034ad2f6cd1612eb`  
		Last Modified: Tue, 09 Feb 2021 02:46:36 GMT  
		Size: 53.0 MB (53006875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfbb5febe9760088b6b37eb86b6de4b894671d73ff434f08a065c4be75f5f15b`  
		Last Modified: Tue, 09 Feb 2021 07:33:23 GMT  
		Size: 1.9 KB (1875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80a1726a27e85bea832b50adc91a723c2674060721d6412a437bdca9c9486dc6`  
		Last Modified: Tue, 09 Feb 2021 07:33:27 GMT  
		Size: 25.6 MB (25629516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7f8775c81edbabfa12ec803b372c8803ec14befe3abea7fe59f4a9a123c1f41`  
		Last Modified: Tue, 09 Feb 2021 07:33:23 GMT  
		Size: 920.2 KB (920164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfe74f4b2a29100ecc661592714fe6a4e18e5357dc9e972ea872f9e23be99b28`  
		Last Modified: Tue, 09 Feb 2021 07:33:23 GMT  
		Size: 349.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:240919189f1d1674070089d041386a8f37831032c68e7386517ec600b18474f6`  
		Last Modified: Tue, 09 Feb 2021 07:33:44 GMT  
		Size: 210.6 MB (210577423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
