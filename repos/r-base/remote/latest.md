## `r-base:latest`

```console
$ docker pull r-base@sha256:ba7343f5baddcea82d5e51f8f8e70ca6a33a356ac02d1576231b301da0f241ae
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `r-base:latest` - linux; amd64

```console
$ docker pull r-base@sha256:649a9bb859a9eed1c5ec7afb015faba12924cbc0eadfa039828a4418c1e329d9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **338.6 MB (338596469 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5441619af0c00724ee7bc64395ce504ee368b23cde615d72b25df1a300db0a26`
-	Default Command: `["R"]`

```dockerfile
# Tue, 04 Jul 2023 01:22:36 GMT
ADD file:de5374a9ef9a0a868df3aca8ce7b7d50abbcf762f41fef9c58012f36d97f78ad in / 
# Tue, 04 Jul 2023 01:22:36 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 07:09:11 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Tue, 04 Jul 2023 07:09:12 GMT
RUN useradd -s /bin/bash -m docker 	&& usermod -a -G staff docker
# Tue, 04 Jul 2023 07:09:24 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 07:09:26 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Tue, 04 Jul 2023 07:09:27 GMT
ENV LC_ALL=en_US.UTF-8
# Tue, 04 Jul 2023 07:09:27 GMT
ENV LANG=en_US.UTF-8
# Tue, 04 Jul 2023 07:09:27 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Tue, 04 Jul 2023 07:09:27 GMT
ENV R_BASE_VERSION=4.3.1
# Tue, 04 Jul 2023 07:10:51 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-docopt                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& chown root:staff "/usr/local/lib/R/site-library" 	&& chmod g+ws "/usr/local/lib/R/site-library" 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 07:10:53 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:dfc7daecfaf18ac4d0f8113f6edff692b509a3dfec300e2dc347fc813f7fd887`  
		Last Modified: Tue, 04 Jul 2023 01:28:45 GMT  
		Size: 49.5 MB (49523824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:724d9d5a54683c65388b07995a649f6df0b22cac8901836d3ce0029ecd7de185`  
		Last Modified: Tue, 04 Jul 2023 07:11:11 GMT  
		Size: 3.4 KB (3360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:464a7d454ec983caa297e5b5a95b98faa11038e1d9ce9600d32d3ce35cc6a814`  
		Last Modified: Tue, 04 Jul 2023 07:11:14 GMT  
		Size: 25.2 MB (25178309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6c065bd9257e8106bcd249c68ab9c583e09c52a897c3ee556a285230778e052`  
		Last Modified: Tue, 04 Jul 2023 07:11:11 GMT  
		Size: 865.8 KB (865846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f388f2fe8b68155bac332b7e8a14b2cbe70791fb653bb18734bb097e2377f0c2`  
		Last Modified: Tue, 04 Jul 2023 07:11:11 GMT  
		Size: 348.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c31e2e824ca5623dafd5caf30d34a1e758be709b9421e5308d5e5ba01bba509`  
		Last Modified: Tue, 04 Jul 2023 07:11:40 GMT  
		Size: 263.0 MB (263024782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:latest` - linux; arm64 variant v8

```console
$ docker pull r-base@sha256:809c0de63ab078d0fa1ff91b66936c77af56cc5963c0e6a2050b3071a50247cc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **323.1 MB (323075473 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4cee65ce469b905d0d47a20181b66a058194b6f3e80cf95e845ec078ecc44e92`
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
# Tue, 20 Jun 2023 23:05:27 GMT
ENV R_BASE_VERSION=4.3.1
# Tue, 20 Jun 2023 23:06:54 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-docopt                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& chown root:staff "/usr/local/lib/R/site-library" 	&& chmod g+ws "/usr/local/lib/R/site-library" 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Tue, 20 Jun 2023 23:06:58 GMT
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
	-	`sha256:0e5354f633754c2f9482bc9de7f241ddde92c8a297a8411d3b7f359f012d0fe8`  
		Last Modified: Tue, 20 Jun 2023 23:07:31 GMT  
		Size: 247.6 MB (247631842 bytes)  
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
$ docker pull r-base@sha256:b51b85ab44ce098144255990958313a32a476cc651aabdc99bad2ee7b339b4f6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **298.1 MB (298055103 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd2d13d4aaf6714a20784bba5b05e388aab8c9dcd1a40a2fbc089aedd8555711`
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
# Tue, 20 Jun 2023 22:46:41 GMT
ENV R_BASE_VERSION=4.3.1
# Tue, 20 Jun 2023 22:47:50 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-docopt                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& chown root:staff "/usr/local/lib/R/site-library" 	&& chmod g+ws "/usr/local/lib/R/site-library" 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Tue, 20 Jun 2023 22:47:58 GMT
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
	-	`sha256:f0dbb9ad32667b95d62767ba537ec8e178d50d39ab509e7bd44463aa861b4beb`  
		Last Modified: Tue, 20 Jun 2023 22:48:43 GMT  
		Size: 224.4 MB (224362747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
