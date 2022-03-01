## `r-base:latest`

```console
$ docker pull r-base@sha256:56f2597665e9e5f37eb1cb217db70f4a11de811b66d400c75274a7cc469ccbaa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `r-base:latest` - linux; amd64

```console
$ docker pull r-base@sha256:fff003a52d076e963396876b83cfa88c4f40a8bc27e341339cd3cc0236c1db79
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **332.5 MB (332479159 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b361dfebd4fbd65e91e96956dcb1954f79b587c6b2a781b2c2cb8cc27bf9eca`
-	Default Command: `["R"]`

```dockerfile
# Wed, 26 Jan 2022 01:43:08 GMT
ADD file:0801e9051ecaf8cd32ba061e9d8b06c000f3416eecdd1b685aecf44171d2198c in / 
# Wed, 26 Jan 2022 01:43:09 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 22:38:53 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Wed, 26 Jan 2022 22:38:54 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Wed, 26 Jan 2022 22:39:06 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 22:39:09 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Wed, 26 Jan 2022 22:39:09 GMT
ENV LC_ALL=en_US.UTF-8
# Wed, 26 Jan 2022 22:39:09 GMT
ENV LANG=en_US.UTF-8
# Wed, 26 Jan 2022 22:39:10 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Wed, 26 Jan 2022 22:39:10 GMT
ENV R_BASE_VERSION=4.1.2
# Wed, 26 Jan 2022 22:39:11 GMT
RUN echo "deb http://deb.debian.org/debian experimental main" > /etc/apt/sources.list.d/experimental.list     && echo "deb [trusted=yes] https://eddelbuettel.github.io/ppaR400 ./" > /etc/apt/sources.list.d/edd-r4.list
# Wed, 26 Jan 2022 22:40:11 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 22:40:13 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:921f230b928f5947ac783609306a9da6b4f3c2fbc1347349ddf2815475c058e5`  
		Last Modified: Wed, 26 Jan 2022 01:51:33 GMT  
		Size: 55.6 MB (55560694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6e3f2821cbf850875b8d8e695f3ee7afd611ba7607593cb59a55e014c473ddd`  
		Last Modified: Wed, 26 Jan 2022 22:40:25 GMT  
		Size: 1.9 KB (1875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20de65816ba52a5a4e31f3055808c85a05feb04c124b144404eb455d4cbe4f2a`  
		Last Modified: Wed, 26 Jan 2022 22:40:26 GMT  
		Size: 25.8 MB (25843249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5682b9249ee0b4e5393da49c07c6a2c505b320feb648d1c90579b765808d0fbe`  
		Last Modified: Wed, 26 Jan 2022 22:40:23 GMT  
		Size: 864.6 KB (864597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5f65281466dbefb2c31af662723984c57fd3f6080ad9ce3fbb915b331965cf7`  
		Last Modified: Wed, 26 Jan 2022 22:40:23 GMT  
		Size: 349.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d436525a99f90922c236964ebd4eecd4f40163c28c3386e1b509151a7e0d9ea`  
		Last Modified: Wed, 26 Jan 2022 22:40:23 GMT  
		Size: 295.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84e3a4a20b3ca787bb46cd034da10c343a3605816568de5647703ff640b5d9e1`  
		Last Modified: Wed, 26 Jan 2022 22:40:54 GMT  
		Size: 250.2 MB (250208100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:latest` - linux; arm64 variant v8

```console
$ docker pull r-base@sha256:dc1cb728c1fbd3c91be2ed405c3d301da8833879433091f6e897d3dc1805cc6e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **321.2 MB (321180480 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca30608c2cc638dcc24c6cd049c8e75e491fdae6d50943a104007a13173b89e7`
-	Default Command: `["R"]`

```dockerfile
# Wed, 26 Jan 2022 01:44:58 GMT
ADD file:e2a2e74c475403cf5762c9f71f745200db9a82ef550eab75ae5846166ed389f4 in / 
# Wed, 26 Jan 2022 01:44:59 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 07:12:35 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Wed, 26 Jan 2022 07:12:36 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Wed, 26 Jan 2022 07:12:47 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 07:12:50 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Wed, 26 Jan 2022 07:12:51 GMT
ENV LC_ALL=en_US.UTF-8
# Wed, 26 Jan 2022 07:12:52 GMT
ENV LANG=en_US.UTF-8
# Wed, 26 Jan 2022 07:12:53 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Wed, 26 Jan 2022 07:12:54 GMT
ENV R_BASE_VERSION=4.1.2
# Wed, 26 Jan 2022 07:12:55 GMT
RUN echo "deb http://deb.debian.org/debian experimental main" > /etc/apt/sources.list.d/experimental.list     && echo "deb [trusted=yes] https://eddelbuettel.github.io/ppaR400 ./" > /etc/apt/sources.list.d/edd-r4.list
# Wed, 26 Jan 2022 07:14:12 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 07:14:13 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:f4e7f3fd67ab16803b5ea5353b9b4a6d7bba8d2329182eb0b5733c1178fa6b62`  
		Last Modified: Wed, 26 Jan 2022 01:53:45 GMT  
		Size: 54.5 MB (54535233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ea08b69d2197bd87b8d0ca059b9a46c882b5426261606007da8ce3156b9ea43`  
		Last Modified: Wed, 26 Jan 2022 07:14:43 GMT  
		Size: 1.8 KB (1760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1750c7f5e3bc2e2bb87c4c6f0f5344c171939cd6d6240c658f99181a732764b`  
		Last Modified: Wed, 26 Jan 2022 07:14:42 GMT  
		Size: 25.8 MB (25836814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f6fad325d1a18c861a2806d3227acc80a5e37e7adf9d8e9d4acf12af3ad5bb4`  
		Last Modified: Wed, 26 Jan 2022 07:14:39 GMT  
		Size: 864.6 KB (864614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:895b8b86845a16e1b09aa512c680e1cf5ddb64759a7f07adcf149a0b5bfbb100`  
		Last Modified: Wed, 26 Jan 2022 07:14:39 GMT  
		Size: 349.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df8337df7b87bcd000b12ba4dc508554dec455e38f0c25b581eaa4c552aff463`  
		Last Modified: Wed, 26 Jan 2022 07:14:39 GMT  
		Size: 293.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1612fb18e93bc438582e93ab09d2df37bd5c3af3b2bf628be12cab40def1ba7`  
		Last Modified: Wed, 26 Jan 2022 07:15:07 GMT  
		Size: 239.9 MB (239941417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:latest` - linux; ppc64le

```console
$ docker pull r-base@sha256:f53da4aefd8b6b071c67be5aa546a00ac18ac0f0a5fd721306cc250b47791308
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **331.3 MB (331258562 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d38c6122bf106259ac425175bbd5be321ef5cc14bd8e9c211d0c50b5790ef839`
-	Default Command: `["R"]`

```dockerfile
# Wed, 26 Jan 2022 01:50:20 GMT
ADD file:38c73ba90be6f58e3639e5d4ebbb9b3f61fb845729ac0dca30389f1f8d2c32e2 in / 
# Wed, 26 Jan 2022 01:50:26 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 19:32:00 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Wed, 26 Jan 2022 19:32:16 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Wed, 26 Jan 2022 19:33:18 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 19:33:34 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Wed, 26 Jan 2022 19:33:37 GMT
ENV LC_ALL=en_US.UTF-8
# Wed, 26 Jan 2022 19:33:41 GMT
ENV LANG=en_US.UTF-8
# Wed, 26 Jan 2022 19:33:50 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Wed, 26 Jan 2022 19:33:52 GMT
ENV R_BASE_VERSION=4.1.2
# Wed, 26 Jan 2022 19:33:56 GMT
RUN echo "deb http://deb.debian.org/debian experimental main" > /etc/apt/sources.list.d/experimental.list     && echo "deb [trusted=yes] https://eddelbuettel.github.io/ppaR400 ./" > /etc/apt/sources.list.d/edd-r4.list
# Wed, 26 Jan 2022 19:43:09 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 19:43:15 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:abb89d61badc571bdc7c4a161a7fc8463ac6b8eb973d6aeff716f76edb833ccf`  
		Last Modified: Wed, 26 Jan 2022 02:04:40 GMT  
		Size: 59.9 MB (59942294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29f98cc64611d20b5b17e209530e22cb03248662a71c794504223ead272ae0c1`  
		Last Modified: Wed, 26 Jan 2022 19:43:34 GMT  
		Size: 1.9 KB (1884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1633471432381a6ab516416379d1f7d161e5f46874e8919ff1f29d640b75e09a`  
		Last Modified: Wed, 26 Jan 2022 19:43:35 GMT  
		Size: 26.1 MB (26075299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dbce397a55206c93376b1cfff032b1e6dc6bc7f3bccd99a288a51bdb6967fbf`  
		Last Modified: Wed, 26 Jan 2022 19:43:31 GMT  
		Size: 864.6 KB (864617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dbf3d094059f2ed583df5aa6ba2ad42de8d6bde8411844bc1a4c1f6813b5b51`  
		Last Modified: Wed, 26 Jan 2022 19:43:31 GMT  
		Size: 352.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d2441e84b7966f74f2c0460540d64df9e80cacb01c10ed22a1d548fc5173be9`  
		Last Modified: Wed, 26 Jan 2022 19:43:31 GMT  
		Size: 294.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dc258d97a0498066c434f084a1e8b8174b0213328f71c9433e9b60c1a1a341a`  
		Last Modified: Wed, 26 Jan 2022 19:44:09 GMT  
		Size: 244.4 MB (244373822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:latest` - linux; s390x

```console
$ docker pull r-base@sha256:e53613fba064a29a8ae33b9c87bf7927bafc07eaa7877258a116e2e920d5b2e6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **297.9 MB (297940226 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a85192dada6cba43a8e652bd9ac5b8519890dd91d90bb70c7801f628d6be628`
-	Default Command: `["R"]`

```dockerfile
# Tue, 01 Mar 2022 02:04:00 GMT
ADD file:674969e6126779bfa143207845528923901c01711a6471c08e874b71260a2f41 in / 
# Tue, 01 Mar 2022 02:04:03 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 15:20:32 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Tue, 01 Mar 2022 15:20:33 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Tue, 01 Mar 2022 15:20:42 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 15:20:44 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Tue, 01 Mar 2022 15:20:44 GMT
ENV LC_ALL=en_US.UTF-8
# Tue, 01 Mar 2022 15:20:44 GMT
ENV LANG=en_US.UTF-8
# Tue, 01 Mar 2022 15:20:44 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Tue, 01 Mar 2022 15:20:45 GMT
ENV R_BASE_VERSION=4.1.2
# Tue, 01 Mar 2022 15:20:45 GMT
RUN echo "deb http://deb.debian.org/debian experimental main" > /etc/apt/sources.list.d/experimental.list     && echo "deb [trusted=yes] https://eddelbuettel.github.io/ppaR400 ./" > /etc/apt/sources.list.d/edd-r4.list
# Tue, 01 Mar 2022 15:21:27 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 15:21:34 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:fa3fc208bf283f64691e90f68e0932fa4d979c605b3bd3db327d9014d601764a`  
		Last Modified: Tue, 01 Mar 2022 02:09:32 GMT  
		Size: 54.0 MB (54006950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25ecddba89851dad7a6e99dfaf31da88691f9223e2c307dbcbd6729c06b81539`  
		Last Modified: Tue, 01 Mar 2022 15:21:50 GMT  
		Size: 2.0 KB (1978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:248d2141b02ddf02d31a2993cc63718b51e58331562ce9e9587870d6b197cb02`  
		Last Modified: Tue, 01 Mar 2022 15:21:51 GMT  
		Size: 25.9 MB (25860360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c34951adf2c32fb6697d4ed4cc302f3d64320f7bb32965f77ecc4b036700b1a7`  
		Last Modified: Tue, 01 Mar 2022 15:21:49 GMT  
		Size: 920.2 KB (920188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f9160918a90c4210013a7129e046edc102c751e398bdd673b056bdc6db9b7bb`  
		Last Modified: Tue, 01 Mar 2022 15:21:49 GMT  
		Size: 346.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aa78b755686ab914e647ddf9ced925687ff716035b4087f9fc794f42de06119`  
		Last Modified: Tue, 01 Mar 2022 15:21:49 GMT  
		Size: 292.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b2aa72665267257acc2eddf512a0b4ed265ff8e5998e8440fc7adc7bc1a4874`  
		Last Modified: Tue, 01 Mar 2022 15:22:09 GMT  
		Size: 217.2 MB (217150112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
