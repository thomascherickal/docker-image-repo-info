## `r-base:latest`

```console
$ docker pull r-base@sha256:0add182011e6f7ba655f6a242f683086f56ad7340e0d7e67d8f5d9a71176ab8e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `r-base:latest` - linux; amd64

```console
$ docker pull r-base@sha256:4f0c3a5f1681e03af47991a48d5f8c9db4d8e141a5b77b8a33526a3223a2ea6c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **336.6 MB (336631108 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4982dbf8881545eed81a3ebf73f32baf929a8c050f056f3dc55ab7debbe5f29a`
-	Default Command: `["R"]`

```dockerfile
# Mon, 12 Jun 2023 23:23:22 GMT
ADD file:418560b5057bb018516c119e87b040f82c7dce4d4961e8bf73268adb278e1635 in / 
# Mon, 12 Jun 2023 23:23:23 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 12:55:08 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Tue, 13 Jun 2023 12:55:09 GMT
RUN useradd -s /bin/bash -m docker 	&& usermod -a -G staff docker
# Tue, 13 Jun 2023 12:55:22 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 12:55:24 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Tue, 13 Jun 2023 12:55:25 GMT
ENV LC_ALL=en_US.UTF-8
# Tue, 13 Jun 2023 12:55:25 GMT
ENV LANG=en_US.UTF-8
# Tue, 13 Jun 2023 12:55:25 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Tue, 13 Jun 2023 12:55:25 GMT
ENV R_BASE_VERSION=4.3.0
# Tue, 13 Jun 2023 12:55:26 GMT
RUN echo "deb http://deb.debian.org/debian experimental main" > /etc/apt/sources.list.d/experimental.list     && echo "deb [trusted=yes] https://eddelbuettel.github.io/ppaR400 ./" > /etc/apt/sources.list.d/edd-r4.list
# Tue, 13 Jun 2023 12:56:53 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-docopt                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& chown root:staff "/usr/local/lib/R/site-library" 	&& chmod g+ws "/usr/local/lib/R/site-library" 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 12:56:55 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:dfaac2cc63fd541e1c2e3738569929f032b19fa4217d0885ba3920b8a4e9e69d`  
		Last Modified: Mon, 12 Jun 2023 23:29:32 GMT  
		Size: 49.6 MB (49552114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5a99ed878076590ed625922a37845fe8715ac4f91658998602947b554858887`  
		Last Modified: Tue, 13 Jun 2023 12:57:08 GMT  
		Size: 3.4 KB (3356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d70dc2acb54225de8cce21ee53fcefd2dd306ddff0d9b3a273a2c083e748308`  
		Last Modified: Tue, 13 Jun 2023 12:57:10 GMT  
		Size: 25.2 MB (25178219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e86bd4237083e5794b6a89917d77032894210779d2ae9dfdc5ea2413c93b4f3a`  
		Last Modified: Tue, 13 Jun 2023 12:57:07 GMT  
		Size: 865.9 KB (865852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3abea49891a27763d6c54bcd5a6f46854a0890532c82209a26624eadc442fbad`  
		Last Modified: Tue, 13 Jun 2023 12:57:06 GMT  
		Size: 347.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01cd65c0aa293bee82af92f221f63ef02e3d520b0542b7b394f95c5afe3a9904`  
		Last Modified: Tue, 13 Jun 2023 12:57:06 GMT  
		Size: 293.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de58c0ddf9dc5e91a25e8e7d1c09d81b8db84a8f1ef9c1be6752e078c8ab48f2`  
		Last Modified: Tue, 13 Jun 2023 12:57:35 GMT  
		Size: 261.0 MB (261030927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:latest` - linux; arm64 variant v8

```console
$ docker pull r-base@sha256:36524e8c48da3809fbdbbe9450d3fbb8930a11c2fa2b31195668001bd2dfac45
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **322.8 MB (322771935 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:acd385396e14111d534f9aae41b4d7b76e836b77fed62c87f3c78c89482f3cb2`
-	Default Command: `["R"]`

```dockerfile
# Mon, 12 Jun 2023 23:42:15 GMT
ADD file:9538b10221306d569a3379a42ad14f6a04e3400effaf2e6093c219ad3ed820ff in / 
# Mon, 12 Jun 2023 23:42:16 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 12:56:23 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Tue, 13 Jun 2023 12:56:24 GMT
RUN useradd -s /bin/bash -m docker 	&& usermod -a -G staff docker
# Tue, 13 Jun 2023 12:56:38 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 12:56:39 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Tue, 13 Jun 2023 12:56:40 GMT
ENV LC_ALL=en_US.UTF-8
# Tue, 13 Jun 2023 12:56:40 GMT
ENV LANG=en_US.UTF-8
# Tue, 13 Jun 2023 12:56:40 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Tue, 13 Jun 2023 12:56:40 GMT
ENV R_BASE_VERSION=4.3.0
# Tue, 13 Jun 2023 12:56:41 GMT
RUN echo "deb http://deb.debian.org/debian experimental main" > /etc/apt/sources.list.d/experimental.list     && echo "deb [trusted=yes] https://eddelbuettel.github.io/ppaR400 ./" > /etc/apt/sources.list.d/edd-r4.list
# Tue, 13 Jun 2023 12:58:16 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-docopt                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& chown root:staff "/usr/local/lib/R/site-library" 	&& chmod g+ws "/usr/local/lib/R/site-library" 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 12:58:18 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:7f36dd606efeffdc09debbf5d2f9a2a9f9cc7b769ef21cc6ade380d05fc0bc8e`  
		Last Modified: Mon, 12 Jun 2023 23:47:29 GMT  
		Size: 49.6 MB (49573160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c949a74ea55a5fb51fae0d50ac0fc8eddc26b6a1dbec18b1cff9a6ea2df0d2e`  
		Last Modified: Tue, 13 Jun 2023 12:58:39 GMT  
		Size: 3.4 KB (3358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc8cda884da2f6db927e776047ae256c89a6d90eb9a1a0e44cb86e996be5cfbd`  
		Last Modified: Tue, 13 Jun 2023 12:58:39 GMT  
		Size: 25.0 MB (25000923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a34e7b1070c2f43dc102bbfcd1535255c48c635a2cd0b9a0661b5dd5e6633717`  
		Last Modified: Tue, 13 Jun 2023 12:58:38 GMT  
		Size: 865.8 KB (865843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63b9b3056649afc986207be02188180eb815e7fa0456d7ecc1ca6549357ebdd6`  
		Last Modified: Tue, 13 Jun 2023 12:58:37 GMT  
		Size: 347.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a763461a4e6bf1eea37906ba2a6fe955c99e7d0c5564193275bbdbe27173f61`  
		Last Modified: Tue, 13 Jun 2023 12:58:37 GMT  
		Size: 290.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ee980f2e55c9808ad72c79f2a9cdcff2e85d5b8d0b83cf08a9dce7cb5c36115`  
		Last Modified: Tue, 13 Jun 2023 12:58:57 GMT  
		Size: 247.3 MB (247328014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:latest` - linux; ppc64le

```console
$ docker pull r-base@sha256:ef829cbbae72bd2206db7f5558f3c10521892fb5ea56e9292143eff41ce4dd6e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **339.4 MB (339392415 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef1b4e129a9c9dc69aa8dfc6edc40a9369aed587d24b223b73264d009884163b`
-	Default Command: `["R"]`

```dockerfile
# Mon, 12 Jun 2023 23:20:50 GMT
ADD file:c800eebe5b5256d5f3eb9d436f7401634618c397b30f31d8beee6daa24772dee in / 
# Mon, 12 Jun 2023 23:20:54 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 07:01:26 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Tue, 13 Jun 2023 07:01:27 GMT
RUN useradd -s /bin/bash -m docker 	&& usermod -a -G staff docker
# Tue, 13 Jun 2023 07:01:47 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 07:01:51 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Tue, 13 Jun 2023 07:01:52 GMT
ENV LC_ALL=en_US.UTF-8
# Tue, 13 Jun 2023 07:01:52 GMT
ENV LANG=en_US.UTF-8
# Tue, 13 Jun 2023 07:01:53 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Tue, 13 Jun 2023 07:01:54 GMT
ENV R_BASE_VERSION=4.3.0
# Tue, 13 Jun 2023 07:01:55 GMT
RUN echo "deb http://deb.debian.org/debian experimental main" > /etc/apt/sources.list.d/experimental.list     && echo "deb [trusted=yes] https://eddelbuettel.github.io/ppaR400 ./" > /etc/apt/sources.list.d/edd-r4.list
# Tue, 13 Jun 2023 07:04:43 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-docopt                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& chown root:staff "/usr/local/lib/R/site-library" 	&& chmod g+ws "/usr/local/lib/R/site-library" 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 07:04:51 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:da363b5a528e02b2ccc2452bd956ac683fa34d495ffdfd1407ffd0bd41cb001a`  
		Last Modified: Mon, 12 Jun 2023 23:27:36 GMT  
		Size: 53.5 MB (53536756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c48b63dbc8203e931d84f41ad09099a3028f74e0de284398a50d4212b5a1b2b`  
		Last Modified: Tue, 13 Jun 2023 07:05:13 GMT  
		Size: 3.4 KB (3358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2ccb7cfd103d968b0337507ee49bb5171fe8b8c5c74adb5af8cb3dcc6e568fe`  
		Last Modified: Tue, 13 Jun 2023 07:05:16 GMT  
		Size: 25.6 MB (25578470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37b8cc93cc8be20745d9070e877ae867c2b15547fa7160e151bff57c3417b557`  
		Last Modified: Tue, 13 Jun 2023 07:05:12 GMT  
		Size: 865.9 KB (865852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73c8bc99811dbe6a83892b6b4f56a01256b59b9dc439bc7d8342767b3f3795dc`  
		Last Modified: Tue, 13 Jun 2023 07:05:11 GMT  
		Size: 349.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e476441b15561442564f98ee4e908884c9c1a58fc4ab86c5c4dc28f1cdef3a6`  
		Last Modified: Tue, 13 Jun 2023 07:05:11 GMT  
		Size: 291.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:673849be497f45b195ab40705053bb83ac7e0c012eeab154a00481ba140448b9`  
		Last Modified: Tue, 13 Jun 2023 07:06:04 GMT  
		Size: 259.4 MB (259407339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:latest` - linux; s390x

```console
$ docker pull r-base@sha256:7beab94b8d15d4e89924a423f9a921dd85462cd0c3a83593005447dc94f811f0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **297.5 MB (297547859 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89cf3dfb21fa6695f7f5a2f308b669c5260ce6e1a3fc8e95f32eaf6b334be263`
-	Default Command: `["R"]`

```dockerfile
# Tue, 23 May 2023 00:43:47 GMT
ADD file:6dfd7d21cdfe9dee2a7cad47d8e2e22e6e56bd924f036cb45c183fe31efe66cc in / 
# Tue, 23 May 2023 00:43:49 GMT
CMD ["bash"]
# Tue, 23 May 2023 02:28:29 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Tue, 23 May 2023 02:28:29 GMT
RUN useradd -s /bin/bash -m docker 	&& usermod -a -G staff docker
# Tue, 23 May 2023 02:28:36 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 02:28:39 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Tue, 23 May 2023 02:28:39 GMT
ENV LC_ALL=en_US.UTF-8
# Tue, 23 May 2023 02:28:39 GMT
ENV LANG=en_US.UTF-8
# Tue, 23 May 2023 02:28:39 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Tue, 23 May 2023 02:28:39 GMT
ENV R_BASE_VERSION=4.3.0
# Tue, 23 May 2023 02:28:40 GMT
RUN echo "deb http://deb.debian.org/debian experimental main" > /etc/apt/sources.list.d/experimental.list     && echo "deb [trusted=yes] https://eddelbuettel.github.io/ppaR400 ./" > /etc/apt/sources.list.d/edd-r4.list
# Tue, 23 May 2023 02:30:10 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-docopt                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& chown root:staff "/usr/local/lib/R/site-library" 	&& chmod g+ws "/usr/local/lib/R/site-library" 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 02:30:17 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:af4d11b0c6366f32a980344976c0622adf11030b727c114fcc65377cb3f44688`  
		Last Modified: Tue, 23 May 2023 00:46:43 GMT  
		Size: 47.7 MB (47673474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c3ba3a415d79670199ec98260e42e6b72cc5eea4a1ab6c615b4caacf1cafe4c`  
		Last Modified: Tue, 23 May 2023 02:30:38 GMT  
		Size: 3.4 KB (3364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4d6d4d9b862bc7cad32b844052a1006db830fa9c3583c57182e5fa222cf18f9`  
		Last Modified: Tue, 23 May 2023 02:30:40 GMT  
		Size: 24.8 MB (24833563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83952e1da18fa0309b148dc5f654137f85a9f36300cd3f162c4bb15174507944`  
		Last Modified: Tue, 23 May 2023 02:30:37 GMT  
		Size: 921.0 KB (921007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca68baa69c6585bf823bfe9b5d023333f08dc5970cf017131d3645e4476ab2df`  
		Last Modified: Tue, 23 May 2023 02:30:37 GMT  
		Size: 349.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:128fbc66c9a8965d790c4a7a0b54f7805a39755af051c3c2454a02de3dbb1d58`  
		Last Modified: Tue, 23 May 2023 02:30:37 GMT  
		Size: 293.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97acb00df28ae2a5ef9bb1f50c3d0e0c0c9cb2a433ad2176afaa424016685779`  
		Last Modified: Tue, 23 May 2023 02:31:01 GMT  
		Size: 224.1 MB (224115809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
