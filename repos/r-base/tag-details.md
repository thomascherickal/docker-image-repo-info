<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `r-base`

-	[`r-base:4.3.1`](#r-base431)
-	[`r-base:latest`](#r-baselatest)

## `r-base:4.3.1`

```console
$ docker pull r-base@sha256:ddb42db9ee38db1938567e18e83f6e8e5781ae33595735fe130339c56635c21c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; ppc64le

### `r-base:4.3.1` - linux; ppc64le

```console
$ docker pull r-base@sha256:20b9ee3f6ca171833cb3f181e13c3bd8e9d9e1217fb97383fe4fed335fdd52c0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **339.6 MB (339627090 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99c7dac40d82e0dfec54b074f580f0dea9a0f84357b48e893a81f5ffdf3a7329`
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
# Tue, 20 Jun 2023 22:17:36 GMT
ENV R_BASE_VERSION=4.3.1
# Tue, 20 Jun 2023 22:21:59 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-docopt                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& chown root:staff "/usr/local/lib/R/site-library" 	&& chmod g+ws "/usr/local/lib/R/site-library" 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Tue, 20 Jun 2023 22:22:12 GMT
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
	-	`sha256:440ef8655cf83730c53a4341be03a450079d6625702dcad71a6019fa253f3433`  
		Last Modified: Tue, 20 Jun 2023 22:23:15 GMT  
		Size: 259.6 MB (259642305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `r-base:latest`

```console
$ docker pull r-base@sha256:11fdec71b25ef271e3309f056310fc3475b2693aba74c36ae0502cb7208cab20
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
$ docker pull r-base@sha256:20b9ee3f6ca171833cb3f181e13c3bd8e9d9e1217fb97383fe4fed335fdd52c0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **339.6 MB (339627090 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99c7dac40d82e0dfec54b074f580f0dea9a0f84357b48e893a81f5ffdf3a7329`
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
# Tue, 20 Jun 2023 22:17:36 GMT
ENV R_BASE_VERSION=4.3.1
# Tue, 20 Jun 2023 22:21:59 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-docopt                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& chown root:staff "/usr/local/lib/R/site-library" 	&& chmod g+ws "/usr/local/lib/R/site-library" 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Tue, 20 Jun 2023 22:22:12 GMT
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
	-	`sha256:440ef8655cf83730c53a4341be03a450079d6625702dcad71a6019fa253f3433`  
		Last Modified: Tue, 20 Jun 2023 22:23:15 GMT  
		Size: 259.6 MB (259642305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:latest` - linux; s390x

```console
$ docker pull r-base@sha256:47fcb52681cdc2a85dd364e3ff692e53ff2d4ba03324c81739b26ebddf717159
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **297.9 MB (297850943 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:21d75f9199b2088e7b386bc7324817cfec5d30232272ba30b6afeb82df97d0f0`
-	Default Command: `["R"]`

```dockerfile
# Tue, 13 Jun 2023 04:31:54 GMT
ADD file:db470514d90937dab99540062bd1d63a3d21f955b13492e99665e3081e72ebac in / 
# Tue, 13 Jun 2023 04:31:58 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 18:48:35 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Tue, 13 Jun 2023 18:48:36 GMT
RUN useradd -s /bin/bash -m docker 	&& usermod -a -G staff docker
# Tue, 13 Jun 2023 18:48:44 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 18:48:46 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Tue, 13 Jun 2023 18:48:46 GMT
ENV LC_ALL=en_US.UTF-8
# Tue, 13 Jun 2023 18:48:46 GMT
ENV LANG=en_US.UTF-8
# Tue, 13 Jun 2023 18:48:46 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Tue, 13 Jun 2023 18:48:47 GMT
ENV R_BASE_VERSION=4.3.0
# Tue, 13 Jun 2023 18:48:47 GMT
RUN echo "deb http://deb.debian.org/debian experimental main" > /etc/apt/sources.list.d/experimental.list     && echo "deb [trusted=yes] https://eddelbuettel.github.io/ppaR400 ./" > /etc/apt/sources.list.d/edd-r4.list
# Tue, 13 Jun 2023 18:50:06 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-docopt                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& chown root:staff "/usr/local/lib/R/site-library" 	&& chmod g+ws "/usr/local/lib/R/site-library" 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 18:50:15 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:6fc736e25918c8d44a93a09b96e2f37f7bcca7f1aac4e82dff1e4ad58dec740c`  
		Last Modified: Tue, 13 Jun 2023 04:36:10 GMT  
		Size: 47.9 MB (47921599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7969331660315bcea8060a75c0a805da6394b81fe84682f77e5b26a6aced966`  
		Last Modified: Tue, 13 Jun 2023 18:50:29 GMT  
		Size: 3.4 KB (3357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d8a3b69438ea6a4491eb277be4fcc02eeead0a8c13568bf9b549e2e85a1eb8d`  
		Last Modified: Tue, 13 Jun 2023 18:50:30 GMT  
		Size: 24.8 MB (24846048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae040574d66ee422683866f43810e3745236b92dd4e074eabe2a4d1d3f19bf72`  
		Last Modified: Tue, 13 Jun 2023 18:50:28 GMT  
		Size: 921.0 KB (921005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:273192fa9216dde130ec7282018ae1c0916cb05ff07ea4097c313ab16a7aec9a`  
		Last Modified: Tue, 13 Jun 2023 18:50:28 GMT  
		Size: 347.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d89a6044d15f052e70f9d294045d2c668835693b889b0751dde6b7b64215c414`  
		Last Modified: Tue, 13 Jun 2023 18:50:28 GMT  
		Size: 291.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d852c65ec8a260b07df2b767a3a663ffc6d6cf6bfac3476e473f9e5aabdebf8f`  
		Last Modified: Tue, 13 Jun 2023 18:50:51 GMT  
		Size: 224.2 MB (224158296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
