## `r-base:latest`

```console
$ docker pull r-base@sha256:eec9d9acf2cf232616682de330e0af0e66ee87cb5a2a8f339df9043cb2c9695b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `r-base:latest` - linux; amd64

```console
$ docker pull r-base@sha256:8c5f13cb4700e18460efca2d4a6339b82f5cbae5a53efde0c0621dfe800086a4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **340.3 MB (340330906 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05eb7a258125d7864dea5cd048e017107696ddb4e46e583502087c0107532b08`
-	Default Command: `["R"]`

```dockerfile
# Tue, 12 Jul 2022 01:21:51 GMT
ADD file:242a7253146210771956ed1bda9124125835ad9e76a50d745d06b34fbf5e50df in / 
# Tue, 12 Jul 2022 01:21:51 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 13:22:43 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Tue, 12 Jul 2022 13:22:44 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Tue, 12 Jul 2022 13:22:54 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 13:22:56 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Tue, 12 Jul 2022 13:22:56 GMT
ENV LC_ALL=en_US.UTF-8
# Tue, 12 Jul 2022 13:22:56 GMT
ENV LANG=en_US.UTF-8
# Tue, 12 Jul 2022 13:22:57 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Tue, 12 Jul 2022 13:22:57 GMT
ENV R_BASE_VERSION=4.2.1
# Tue, 12 Jul 2022 13:23:41 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-docopt                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 13:23:43 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:df98203a8b21cb36e308dd353908ed338642491ef167d757bebb3297146a77a4`  
		Last Modified: Tue, 12 Jul 2022 01:27:27 GMT  
		Size: 53.0 MB (53022316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a226d216a62319dc0bd33f9f2ab068e10914c1ea87f26a9af2a505fb3407c92a`  
		Last Modified: Tue, 12 Jul 2022 13:23:58 GMT  
		Size: 1.9 KB (1878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d06267fca963eae8a21b9c01db4027c0fce62c50c1b2af7e1b64ee3831395be9`  
		Last Modified: Tue, 12 Jul 2022 13:24:02 GMT  
		Size: 29.1 MB (29095840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aff5dbd7edf267d009f7431ab32808362abb6d08b12d8e2b754e28f178bdb02`  
		Last Modified: Tue, 12 Jul 2022 13:23:59 GMT  
		Size: 864.6 KB (864610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05f509fe31e626b0bb83a3c72375959cb5bead186d6743a524ae5ba3f7ab35d0`  
		Last Modified: Tue, 12 Jul 2022 13:23:58 GMT  
		Size: 351.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cbc1ba94271ad07911f284bcda964616faab47cbcab0c3aab7a25ca65d35a86`  
		Last Modified: Tue, 12 Jul 2022 13:24:29 GMT  
		Size: 257.3 MB (257345911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:latest` - linux; arm64 variant v8

```console
$ docker pull r-base@sha256:73b2225b46c24a9946810e3806d517f1ea56efed7dd96e6950fe37164a8a75f0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **329.6 MB (329563928 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bbcf7f59685085aa8a9b00e89a1f4ddee6213db929743e5d3eff1e7da29ad7bf`
-	Default Command: `["R"]`

```dockerfile
# Tue, 12 Jul 2022 00:42:26 GMT
ADD file:52b0a411bbddbc5a40d2288e5189606bd2fb03bdba9ab2dfa0b29ee90195a43b in / 
# Tue, 12 Jul 2022 00:42:26 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 12:56:21 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Tue, 12 Jul 2022 12:56:22 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Tue, 12 Jul 2022 12:56:33 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 12:56:35 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Tue, 12 Jul 2022 12:56:36 GMT
ENV LC_ALL=en_US.UTF-8
# Tue, 12 Jul 2022 12:56:37 GMT
ENV LANG=en_US.UTF-8
# Tue, 12 Jul 2022 12:56:38 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Tue, 12 Jul 2022 12:56:39 GMT
ENV R_BASE_VERSION=4.2.1
# Tue, 12 Jul 2022 12:57:38 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-docopt                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 12:57:39 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:370af700e1ed84d7809745357ae1357e57448bf6e682ad1ff1a41f20c19fe232`  
		Last Modified: Tue, 12 Jul 2022 00:49:31 GMT  
		Size: 52.1 MB (52128630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76e0503232cefb48c17cd3ec0bf77b8af8d657c40fe798a76613a1e006bc782c`  
		Last Modified: Tue, 12 Jul 2022 12:57:55 GMT  
		Size: 1.8 KB (1828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:311e48a7138a5ae6011c273a586f7c769f0d7af33668ce2e5a796ba2c722b73d`  
		Last Modified: Tue, 12 Jul 2022 12:57:58 GMT  
		Size: 28.9 MB (28927889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7efd61bb74bd6091d62d90398ce43ec0b82958e7dc7415e7d0b2b58b323649a`  
		Last Modified: Tue, 12 Jul 2022 12:57:55 GMT  
		Size: 864.6 KB (864612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24e3bf773dc950db2099b5feda63d9ba2aacad7d39afb3ef3e43ab14ecb4ee54`  
		Last Modified: Tue, 12 Jul 2022 12:57:54 GMT  
		Size: 348.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3ce92fcfcd656f3277ed2137f5689b99f35d54cc449cd2da4707eb8b8a1a773`  
		Last Modified: Tue, 12 Jul 2022 12:58:23 GMT  
		Size: 247.6 MB (247640621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:latest` - linux; ppc64le

```console
$ docker pull r-base@sha256:b1862f043edd8372656f6c20fc7d3962d0e20651ca6131bc2a429effc7d3ec45
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **339.5 MB (339462470 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:586738a4e8eb1f47b7cb97bfbc457b67eafba12df0b70d2fbc9752c5d84c9fc3`
-	Default Command: `["R"]`

```dockerfile
# Tue, 12 Jul 2022 01:29:05 GMT
ADD file:50749df5dfe83d67bf06b74c10d8d4c0b6c50902fb0b3fd4b1e944bb4d04d838 in / 
# Tue, 12 Jul 2022 01:29:12 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 11:19:10 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Tue, 12 Jul 2022 11:19:33 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Tue, 12 Jul 2022 11:20:40 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 11:20:56 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Tue, 12 Jul 2022 11:21:00 GMT
ENV LC_ALL=en_US.UTF-8
# Tue, 12 Jul 2022 11:21:08 GMT
ENV LANG=en_US.UTF-8
# Tue, 12 Jul 2022 11:21:19 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Tue, 12 Jul 2022 11:21:26 GMT
ENV R_BASE_VERSION=4.2.1
# Tue, 12 Jul 2022 11:28:15 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-docopt                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 11:28:20 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:0a914d717e21264ea59989c5b8ee06609e61159738242df44dc331a1146b94b4`  
		Last Modified: Tue, 12 Jul 2022 01:43:45 GMT  
		Size: 57.2 MB (57237602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d15fe2fdb00b606a3cbb96330cbc2cb4134cd935ccce98b46f822d1e83c2406d`  
		Last Modified: Tue, 12 Jul 2022 11:28:40 GMT  
		Size: 1.9 KB (1889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7da599f257f5d308622b338fce0a69bb44f8bb21237fe9e4260cd81f156396e7`  
		Last Modified: Tue, 12 Jul 2022 11:28:44 GMT  
		Size: 29.5 MB (29505876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79554b0040269bf6cfb3be3fc610e79906f4f0e4358fa6b9d391f0aeddb18a93`  
		Last Modified: Tue, 12 Jul 2022 11:28:40 GMT  
		Size: 864.6 KB (864615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c417b6d73c179f38145997c00ed8267c7e30637ae230487925281025ea0e901`  
		Last Modified: Tue, 12 Jul 2022 11:28:40 GMT  
		Size: 353.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb190937ede455359a79d1e34b6b30ec19a2e4336ef1e109a84bbbd64e10593e`  
		Last Modified: Tue, 12 Jul 2022 11:29:17 GMT  
		Size: 251.9 MB (251852135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:latest` - linux; s390x

```console
$ docker pull r-base@sha256:cb202636235fca16e8830c3e44bda1688a76d0c04e14945ecc29490098c9fd57
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **304.6 MB (304618798 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b9b2c4823d89f80dfc99b41e2f51d0c91151438406e10cf5b798ad79ddbf481`
-	Default Command: `["R"]`

```dockerfile
# Thu, 23 Jun 2022 00:46:56 GMT
ADD file:c00b81c115a6c1391868dbe0ec890701d2f39e6559e809c5bb3713590bd1108e in / 
# Thu, 23 Jun 2022 00:47:03 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 13:49:08 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Thu, 23 Jun 2022 13:49:09 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Thu, 23 Jun 2022 13:49:18 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 13:49:20 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Thu, 23 Jun 2022 13:49:20 GMT
ENV LC_ALL=en_US.UTF-8
# Thu, 23 Jun 2022 13:49:20 GMT
ENV LANG=en_US.UTF-8
# Thu, 23 Jun 2022 13:49:21 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Fri, 24 Jun 2022 17:41:54 GMT
ENV R_BASE_VERSION=4.2.1
# Fri, 24 Jun 2022 17:42:42 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-docopt                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Fri, 24 Jun 2022 17:42:49 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:a020494a73fce189d7327ea16251dde415c3d854a3d9f6bd50af5d239febdb9f`  
		Last Modified: Thu, 23 Jun 2022 00:54:13 GMT  
		Size: 51.5 MB (51530646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cea57e10bd8d4665428fdcfb6a8b7c3e88aba94cbecb59de4d41618d26420617`  
		Last Modified: Thu, 23 Jun 2022 13:50:24 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7814e02cdc3f73b040f2b3629e7215f655d070bc3306596058249a7435dce9e`  
		Last Modified: Thu, 23 Jun 2022 13:50:28 GMT  
		Size: 28.8 MB (28777608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adc9712944b06164d8744a457d83e36d30024a2c7b76f05cbc242fa6ce3e2817`  
		Last Modified: Thu, 23 Jun 2022 13:50:24 GMT  
		Size: 920.2 KB (920184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6c7f8787bb3e0aae12953f0753d16eedf45a5bcebc135ff0fef3d1fb9500443`  
		Last Modified: Thu, 23 Jun 2022 13:50:24 GMT  
		Size: 348.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd770905aa4e2f0529cca5bc1a71bdad4c8a56b47c966b4c0741801a3b18ad73`  
		Last Modified: Fri, 24 Jun 2022 17:43:30 GMT  
		Size: 223.4 MB (223388130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
