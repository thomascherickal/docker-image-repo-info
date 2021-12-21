<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `r-base`

-	[`r-base:4.1.2`](#r-base412)
-	[`r-base:latest`](#r-baselatest)

## `r-base:4.1.2`

```console
$ docker pull r-base@sha256:e43fe8509afd0714b299f3826809c3dac943b1cbb8f6e96aeece8625c10e769d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `r-base:4.1.2` - linux; amd64

```console
$ docker pull r-base@sha256:f388bbb9701e31289041e5aaf9073f9875bdbec9928d532bc130fde74ea31da5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **331.1 MB (331127316 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13f75f489d679491d9cf54abefe6b84318a6813668ce95dcaac951a19a093a63`
-	Default Command: `["R"]`

```dockerfile
# Tue, 21 Dec 2021 01:24:51 GMT
ADD file:d302405af930cc11493038d472572e46ae1d7253df1c141916634ac984b48b88 in / 
# Tue, 21 Dec 2021 01:24:52 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 12:38:55 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Tue, 21 Dec 2021 12:38:57 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Tue, 21 Dec 2021 12:39:13 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 12:39:17 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Tue, 21 Dec 2021 12:39:17 GMT
ENV LC_ALL=en_US.UTF-8
# Tue, 21 Dec 2021 12:39:17 GMT
ENV LANG=en_US.UTF-8
# Tue, 21 Dec 2021 12:39:19 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Tue, 21 Dec 2021 12:39:19 GMT
ENV R_BASE_VERSION=4.1.2
# Tue, 21 Dec 2021 12:39:20 GMT
RUN echo "deb http://deb.debian.org/debian experimental main" > /etc/apt/sources.list.d/experimental.list     && echo "deb [trusted=yes] https://eddelbuettel.github.io/ppaR400 ./" > /etc/apt/sources.list.d/edd-r4.list
# Tue, 21 Dec 2021 12:40:23 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 12:40:25 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:277c3ceb6ade1082faa3e2b17e1f8fc09ac549df797657b97f6f47253b55f4d0`  
		Last Modified: Tue, 21 Dec 2021 01:31:57 GMT  
		Size: 55.6 MB (55598781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:943eea7241a2643f7f7013ab0fc653f7ae63a0d29372ab5dc6103dbae771d7b8`  
		Last Modified: Tue, 21 Dec 2021 12:40:41 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f12182a985b31d0a699582ab4815f81bcd47dbb7d86a9e377077af37003feea6`  
		Last Modified: Tue, 21 Dec 2021 12:40:42 GMT  
		Size: 25.8 MB (25821775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f307a72a39c2bcec63ad7175dd10c30b480ff9d8745a01e70f26e690e6947463`  
		Last Modified: Tue, 21 Dec 2021 12:40:39 GMT  
		Size: 864.6 KB (864612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2386c9fd709b30e36c8a8272d646be949902ea37868ed1f28e92a9eedd2e215e`  
		Last Modified: Tue, 21 Dec 2021 12:40:38 GMT  
		Size: 351.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6475f3e8f4730d5c18e8318926f77ccded284517b25aba4d76d7646f6020eec`  
		Last Modified: Tue, 21 Dec 2021 12:40:39 GMT  
		Size: 296.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f422ee43c0213eeb78fb04e32298a67dd9a012e2011635029c05db85654ba9c9`  
		Last Modified: Tue, 21 Dec 2021 12:41:09 GMT  
		Size: 248.8 MB (248839619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:4.1.2` - linux; arm64 variant v8

```console
$ docker pull r-base@sha256:fc6f3bac82f6f732114abc019bf1558b1430adb31a3ae5bdd720973879adb554
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **319.9 MB (319888313 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:995a35b35f5471f7c6bf747f04ed341e0000453b26ee6a5ac9a3239bb9f19353`
-	Default Command: `["R"]`

```dockerfile
# Tue, 21 Dec 2021 01:44:49 GMT
ADD file:436a7cbc9b247e837b1662f418559e588633a07d97fbe015b61da9481fb8a8f0 in / 
# Tue, 21 Dec 2021 01:44:50 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 09:50:05 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Tue, 21 Dec 2021 09:50:06 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Tue, 21 Dec 2021 09:50:16 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 09:50:19 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Tue, 21 Dec 2021 09:50:19 GMT
ENV LC_ALL=en_US.UTF-8
# Tue, 21 Dec 2021 09:50:20 GMT
ENV LANG=en_US.UTF-8
# Tue, 21 Dec 2021 09:50:21 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Tue, 21 Dec 2021 09:50:22 GMT
ENV R_BASE_VERSION=4.1.2
# Tue, 21 Dec 2021 09:50:23 GMT
RUN echo "deb http://deb.debian.org/debian experimental main" > /etc/apt/sources.list.d/experimental.list     && echo "deb [trusted=yes] https://eddelbuettel.github.io/ppaR400 ./" > /etc/apt/sources.list.d/edd-r4.list
# Tue, 21 Dec 2021 09:51:31 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 09:51:32 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:ca972f55dc0f92867c66012e7edaba4ddfecaf3952bbd20e050677fdbce9fb70`  
		Last Modified: Tue, 21 Dec 2021 01:53:28 GMT  
		Size: 54.6 MB (54597836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0942aac88f7dcb4855eb45ed38d260c0f7a5c61520b4a18b65f95395dd101fbd`  
		Last Modified: Tue, 21 Dec 2021 09:51:57 GMT  
		Size: 1.8 KB (1762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:078875911a3579a92e7fb6acf917b07d1dfed5ffe75ef7ef3ab62f448bb9c2d1`  
		Last Modified: Tue, 21 Dec 2021 09:51:58 GMT  
		Size: 25.8 MB (25810048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e537596ea61fc18c65bdde583a4bba105c4779daceef81a9f88282bafc626294`  
		Last Modified: Tue, 21 Dec 2021 09:51:55 GMT  
		Size: 864.6 KB (864614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd0d6f5020075f6abaad8e50bf4a7bc81d84772d414e1ca038258f08c31f1d89`  
		Last Modified: Tue, 21 Dec 2021 09:51:54 GMT  
		Size: 349.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:656db4e7229070999c6544eb0108f26a141713cfb11618ea3ce7150a16369724`  
		Last Modified: Tue, 21 Dec 2021 09:51:54 GMT  
		Size: 294.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea17123c16709079ab9ab72cb460fb0523b454c3eb37176e8b7c7c0ede1056b3`  
		Last Modified: Tue, 21 Dec 2021 09:52:22 GMT  
		Size: 238.6 MB (238613410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:4.1.2` - linux; ppc64le

```console
$ docker pull r-base@sha256:47d464aecf9c3b8d6e9ab9d8541d7646e9bbe6e4620c2359bdd0ac2c25878388
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **329.7 MB (329651720 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71de3360191149c5093d919596ec581fce29a810f7a7777340028e7e8135ca16`
-	Default Command: `["R"]`

```dockerfile
# Tue, 21 Dec 2021 02:23:49 GMT
ADD file:42a91d93da4ddbf83627c69ff38d40590c8f8d299ec93dbedcf1faa79105a3af in / 
# Tue, 21 Dec 2021 02:23:54 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 23:10:57 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Tue, 21 Dec 2021 23:11:06 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Tue, 21 Dec 2021 23:11:53 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 23:12:09 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Tue, 21 Dec 2021 23:12:11 GMT
ENV LC_ALL=en_US.UTF-8
# Tue, 21 Dec 2021 23:12:15 GMT
ENV LANG=en_US.UTF-8
# Tue, 21 Dec 2021 23:12:23 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Tue, 21 Dec 2021 23:12:25 GMT
ENV R_BASE_VERSION=4.1.2
# Tue, 21 Dec 2021 23:12:31 GMT
RUN echo "deb http://deb.debian.org/debian experimental main" > /etc/apt/sources.list.d/experimental.list     && echo "deb [trusted=yes] https://eddelbuettel.github.io/ppaR400 ./" > /etc/apt/sources.list.d/edd-r4.list
# Tue, 21 Dec 2021 23:17:54 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 23:17:59 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:e172119311a8de31a50bf3e0fad45f9b68bf5edceb8397100d47c7833f2ac0fb`  
		Last Modified: Tue, 21 Dec 2021 02:33:13 GMT  
		Size: 60.0 MB (59991777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6b01cd3f60321f63d1a275a2d9fae1734ef413a592e085c082bb379575f818c`  
		Last Modified: Tue, 21 Dec 2021 23:18:16 GMT  
		Size: 1.9 KB (1889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d13d04733015dd0e2d9a1a5035635d45776b9e13af2eed513e2aabe2662caefb`  
		Last Modified: Tue, 21 Dec 2021 23:18:18 GMT  
		Size: 26.0 MB (26045626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7896aba092a96de7130f8d50611702cb3bb48e21d193065b6dbd13a58ebed282`  
		Last Modified: Tue, 21 Dec 2021 23:18:14 GMT  
		Size: 864.6 KB (864603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c29a33086f95c2cb9b5de568557dc0d81eec0f40b7d377034ba2224695f1c476`  
		Last Modified: Tue, 21 Dec 2021 23:18:13 GMT  
		Size: 352.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:530cbdcab69a8bc9482e211420b3952aa972fbb0460d5affaac0ee33d3b2c902`  
		Last Modified: Tue, 21 Dec 2021 23:18:13 GMT  
		Size: 297.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdf7d073d2dc131cfafb89846e02598cc1cceec77cb4409c2f434bc56cc6c6fb`  
		Last Modified: Tue, 21 Dec 2021 23:18:51 GMT  
		Size: 242.7 MB (242747176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:4.1.2` - linux; s390x

```console
$ docker pull r-base@sha256:feb3dca586aff0e9db71d96fc18cb375bc9aff0a62b3d0a862a1985f664763aa
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **295.9 MB (295923195 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f2d211b74589ac03c7098ea2b3d930d2bd9cbf6d2b4f3f3f57aaeb56898916a`
-	Default Command: `["R"]`

```dockerfile
# Tue, 21 Dec 2021 01:44:29 GMT
ADD file:fab1fb88494aec56291007be8c0c54cc9bf3f56228b1e709a070150030986221 in / 
# Tue, 21 Dec 2021 01:44:31 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 10:41:36 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Tue, 21 Dec 2021 10:41:36 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Tue, 21 Dec 2021 10:41:45 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 10:41:48 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Tue, 21 Dec 2021 10:41:48 GMT
ENV LC_ALL=en_US.UTF-8
# Tue, 21 Dec 2021 10:41:48 GMT
ENV LANG=en_US.UTF-8
# Tue, 21 Dec 2021 10:41:49 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Tue, 21 Dec 2021 10:41:49 GMT
ENV R_BASE_VERSION=4.1.2
# Tue, 21 Dec 2021 10:41:49 GMT
RUN echo "deb http://deb.debian.org/debian experimental main" > /etc/apt/sources.list.d/experimental.list     && echo "deb [trusted=yes] https://eddelbuettel.github.io/ppaR400 ./" > /etc/apt/sources.list.d/edd-r4.list
# Tue, 21 Dec 2021 10:42:29 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 10:42:38 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:38bb00702c0ff4b51b50541d1787108666c6714b6282d619229305becf8d14f8`  
		Last Modified: Tue, 21 Dec 2021 01:50:33 GMT  
		Size: 53.9 MB (53888397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:493220998c400c5fc4453f0b995e52904519cf35e543924b56e8dcebed857dc2`  
		Last Modified: Tue, 21 Dec 2021 10:43:03 GMT  
		Size: 1.9 KB (1880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a38c6c3d2c265cf1a1e8e213c5b307908de33a04d51a402097b876a57cf6dd5e`  
		Last Modified: Tue, 21 Dec 2021 10:43:04 GMT  
		Size: 25.8 MB (25824772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28ec90a0a3042c89d536ec1b8aeacc4a33bc0b3e07d7113950ae8a0485a9d8a4`  
		Last Modified: Tue, 21 Dec 2021 10:43:02 GMT  
		Size: 920.2 KB (920185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a149407a92ec9614ccf50329478bdcea835d0d114dded3d0bc39aa11060b548`  
		Last Modified: Tue, 21 Dec 2021 10:43:02 GMT  
		Size: 350.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:677b1bd875c0c817f73c13d5dfbc3fd07fffa7ef77d3ef675d020d744808a363`  
		Last Modified: Tue, 21 Dec 2021 10:43:02 GMT  
		Size: 291.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeaef226499622d4ee9328ba1fcdb9ce2d7458c3e2a55c9cf3f6e2191c89a7bb`  
		Last Modified: Tue, 21 Dec 2021 10:43:23 GMT  
		Size: 215.3 MB (215287320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `r-base:latest`

```console
$ docker pull r-base@sha256:e43fe8509afd0714b299f3826809c3dac943b1cbb8f6e96aeece8625c10e769d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `r-base:latest` - linux; amd64

```console
$ docker pull r-base@sha256:f388bbb9701e31289041e5aaf9073f9875bdbec9928d532bc130fde74ea31da5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **331.1 MB (331127316 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13f75f489d679491d9cf54abefe6b84318a6813668ce95dcaac951a19a093a63`
-	Default Command: `["R"]`

```dockerfile
# Tue, 21 Dec 2021 01:24:51 GMT
ADD file:d302405af930cc11493038d472572e46ae1d7253df1c141916634ac984b48b88 in / 
# Tue, 21 Dec 2021 01:24:52 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 12:38:55 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Tue, 21 Dec 2021 12:38:57 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Tue, 21 Dec 2021 12:39:13 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 12:39:17 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Tue, 21 Dec 2021 12:39:17 GMT
ENV LC_ALL=en_US.UTF-8
# Tue, 21 Dec 2021 12:39:17 GMT
ENV LANG=en_US.UTF-8
# Tue, 21 Dec 2021 12:39:19 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Tue, 21 Dec 2021 12:39:19 GMT
ENV R_BASE_VERSION=4.1.2
# Tue, 21 Dec 2021 12:39:20 GMT
RUN echo "deb http://deb.debian.org/debian experimental main" > /etc/apt/sources.list.d/experimental.list     && echo "deb [trusted=yes] https://eddelbuettel.github.io/ppaR400 ./" > /etc/apt/sources.list.d/edd-r4.list
# Tue, 21 Dec 2021 12:40:23 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 12:40:25 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:277c3ceb6ade1082faa3e2b17e1f8fc09ac549df797657b97f6f47253b55f4d0`  
		Last Modified: Tue, 21 Dec 2021 01:31:57 GMT  
		Size: 55.6 MB (55598781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:943eea7241a2643f7f7013ab0fc653f7ae63a0d29372ab5dc6103dbae771d7b8`  
		Last Modified: Tue, 21 Dec 2021 12:40:41 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f12182a985b31d0a699582ab4815f81bcd47dbb7d86a9e377077af37003feea6`  
		Last Modified: Tue, 21 Dec 2021 12:40:42 GMT  
		Size: 25.8 MB (25821775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f307a72a39c2bcec63ad7175dd10c30b480ff9d8745a01e70f26e690e6947463`  
		Last Modified: Tue, 21 Dec 2021 12:40:39 GMT  
		Size: 864.6 KB (864612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2386c9fd709b30e36c8a8272d646be949902ea37868ed1f28e92a9eedd2e215e`  
		Last Modified: Tue, 21 Dec 2021 12:40:38 GMT  
		Size: 351.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6475f3e8f4730d5c18e8318926f77ccded284517b25aba4d76d7646f6020eec`  
		Last Modified: Tue, 21 Dec 2021 12:40:39 GMT  
		Size: 296.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f422ee43c0213eeb78fb04e32298a67dd9a012e2011635029c05db85654ba9c9`  
		Last Modified: Tue, 21 Dec 2021 12:41:09 GMT  
		Size: 248.8 MB (248839619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:latest` - linux; arm64 variant v8

```console
$ docker pull r-base@sha256:fc6f3bac82f6f732114abc019bf1558b1430adb31a3ae5bdd720973879adb554
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **319.9 MB (319888313 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:995a35b35f5471f7c6bf747f04ed341e0000453b26ee6a5ac9a3239bb9f19353`
-	Default Command: `["R"]`

```dockerfile
# Tue, 21 Dec 2021 01:44:49 GMT
ADD file:436a7cbc9b247e837b1662f418559e588633a07d97fbe015b61da9481fb8a8f0 in / 
# Tue, 21 Dec 2021 01:44:50 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 09:50:05 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Tue, 21 Dec 2021 09:50:06 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Tue, 21 Dec 2021 09:50:16 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 09:50:19 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Tue, 21 Dec 2021 09:50:19 GMT
ENV LC_ALL=en_US.UTF-8
# Tue, 21 Dec 2021 09:50:20 GMT
ENV LANG=en_US.UTF-8
# Tue, 21 Dec 2021 09:50:21 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Tue, 21 Dec 2021 09:50:22 GMT
ENV R_BASE_VERSION=4.1.2
# Tue, 21 Dec 2021 09:50:23 GMT
RUN echo "deb http://deb.debian.org/debian experimental main" > /etc/apt/sources.list.d/experimental.list     && echo "deb [trusted=yes] https://eddelbuettel.github.io/ppaR400 ./" > /etc/apt/sources.list.d/edd-r4.list
# Tue, 21 Dec 2021 09:51:31 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 09:51:32 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:ca972f55dc0f92867c66012e7edaba4ddfecaf3952bbd20e050677fdbce9fb70`  
		Last Modified: Tue, 21 Dec 2021 01:53:28 GMT  
		Size: 54.6 MB (54597836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0942aac88f7dcb4855eb45ed38d260c0f7a5c61520b4a18b65f95395dd101fbd`  
		Last Modified: Tue, 21 Dec 2021 09:51:57 GMT  
		Size: 1.8 KB (1762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:078875911a3579a92e7fb6acf917b07d1dfed5ffe75ef7ef3ab62f448bb9c2d1`  
		Last Modified: Tue, 21 Dec 2021 09:51:58 GMT  
		Size: 25.8 MB (25810048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e537596ea61fc18c65bdde583a4bba105c4779daceef81a9f88282bafc626294`  
		Last Modified: Tue, 21 Dec 2021 09:51:55 GMT  
		Size: 864.6 KB (864614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd0d6f5020075f6abaad8e50bf4a7bc81d84772d414e1ca038258f08c31f1d89`  
		Last Modified: Tue, 21 Dec 2021 09:51:54 GMT  
		Size: 349.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:656db4e7229070999c6544eb0108f26a141713cfb11618ea3ce7150a16369724`  
		Last Modified: Tue, 21 Dec 2021 09:51:54 GMT  
		Size: 294.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea17123c16709079ab9ab72cb460fb0523b454c3eb37176e8b7c7c0ede1056b3`  
		Last Modified: Tue, 21 Dec 2021 09:52:22 GMT  
		Size: 238.6 MB (238613410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:latest` - linux; ppc64le

```console
$ docker pull r-base@sha256:47d464aecf9c3b8d6e9ab9d8541d7646e9bbe6e4620c2359bdd0ac2c25878388
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **329.7 MB (329651720 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71de3360191149c5093d919596ec581fce29a810f7a7777340028e7e8135ca16`
-	Default Command: `["R"]`

```dockerfile
# Tue, 21 Dec 2021 02:23:49 GMT
ADD file:42a91d93da4ddbf83627c69ff38d40590c8f8d299ec93dbedcf1faa79105a3af in / 
# Tue, 21 Dec 2021 02:23:54 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 23:10:57 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Tue, 21 Dec 2021 23:11:06 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Tue, 21 Dec 2021 23:11:53 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 23:12:09 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Tue, 21 Dec 2021 23:12:11 GMT
ENV LC_ALL=en_US.UTF-8
# Tue, 21 Dec 2021 23:12:15 GMT
ENV LANG=en_US.UTF-8
# Tue, 21 Dec 2021 23:12:23 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Tue, 21 Dec 2021 23:12:25 GMT
ENV R_BASE_VERSION=4.1.2
# Tue, 21 Dec 2021 23:12:31 GMT
RUN echo "deb http://deb.debian.org/debian experimental main" > /etc/apt/sources.list.d/experimental.list     && echo "deb [trusted=yes] https://eddelbuettel.github.io/ppaR400 ./" > /etc/apt/sources.list.d/edd-r4.list
# Tue, 21 Dec 2021 23:17:54 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 23:17:59 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:e172119311a8de31a50bf3e0fad45f9b68bf5edceb8397100d47c7833f2ac0fb`  
		Last Modified: Tue, 21 Dec 2021 02:33:13 GMT  
		Size: 60.0 MB (59991777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6b01cd3f60321f63d1a275a2d9fae1734ef413a592e085c082bb379575f818c`  
		Last Modified: Tue, 21 Dec 2021 23:18:16 GMT  
		Size: 1.9 KB (1889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d13d04733015dd0e2d9a1a5035635d45776b9e13af2eed513e2aabe2662caefb`  
		Last Modified: Tue, 21 Dec 2021 23:18:18 GMT  
		Size: 26.0 MB (26045626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7896aba092a96de7130f8d50611702cb3bb48e21d193065b6dbd13a58ebed282`  
		Last Modified: Tue, 21 Dec 2021 23:18:14 GMT  
		Size: 864.6 KB (864603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c29a33086f95c2cb9b5de568557dc0d81eec0f40b7d377034ba2224695f1c476`  
		Last Modified: Tue, 21 Dec 2021 23:18:13 GMT  
		Size: 352.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:530cbdcab69a8bc9482e211420b3952aa972fbb0460d5affaac0ee33d3b2c902`  
		Last Modified: Tue, 21 Dec 2021 23:18:13 GMT  
		Size: 297.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdf7d073d2dc131cfafb89846e02598cc1cceec77cb4409c2f434bc56cc6c6fb`  
		Last Modified: Tue, 21 Dec 2021 23:18:51 GMT  
		Size: 242.7 MB (242747176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:latest` - linux; s390x

```console
$ docker pull r-base@sha256:feb3dca586aff0e9db71d96fc18cb375bc9aff0a62b3d0a862a1985f664763aa
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **295.9 MB (295923195 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f2d211b74589ac03c7098ea2b3d930d2bd9cbf6d2b4f3f3f57aaeb56898916a`
-	Default Command: `["R"]`

```dockerfile
# Tue, 21 Dec 2021 01:44:29 GMT
ADD file:fab1fb88494aec56291007be8c0c54cc9bf3f56228b1e709a070150030986221 in / 
# Tue, 21 Dec 2021 01:44:31 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 10:41:36 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Tue, 21 Dec 2021 10:41:36 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Tue, 21 Dec 2021 10:41:45 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 10:41:48 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Tue, 21 Dec 2021 10:41:48 GMT
ENV LC_ALL=en_US.UTF-8
# Tue, 21 Dec 2021 10:41:48 GMT
ENV LANG=en_US.UTF-8
# Tue, 21 Dec 2021 10:41:49 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Tue, 21 Dec 2021 10:41:49 GMT
ENV R_BASE_VERSION=4.1.2
# Tue, 21 Dec 2021 10:41:49 GMT
RUN echo "deb http://deb.debian.org/debian experimental main" > /etc/apt/sources.list.d/experimental.list     && echo "deb [trusted=yes] https://eddelbuettel.github.io/ppaR400 ./" > /etc/apt/sources.list.d/edd-r4.list
# Tue, 21 Dec 2021 10:42:29 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 10:42:38 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:38bb00702c0ff4b51b50541d1787108666c6714b6282d619229305becf8d14f8`  
		Last Modified: Tue, 21 Dec 2021 01:50:33 GMT  
		Size: 53.9 MB (53888397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:493220998c400c5fc4453f0b995e52904519cf35e543924b56e8dcebed857dc2`  
		Last Modified: Tue, 21 Dec 2021 10:43:03 GMT  
		Size: 1.9 KB (1880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a38c6c3d2c265cf1a1e8e213c5b307908de33a04d51a402097b876a57cf6dd5e`  
		Last Modified: Tue, 21 Dec 2021 10:43:04 GMT  
		Size: 25.8 MB (25824772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28ec90a0a3042c89d536ec1b8aeacc4a33bc0b3e07d7113950ae8a0485a9d8a4`  
		Last Modified: Tue, 21 Dec 2021 10:43:02 GMT  
		Size: 920.2 KB (920185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a149407a92ec9614ccf50329478bdcea835d0d114dded3d0bc39aa11060b548`  
		Last Modified: Tue, 21 Dec 2021 10:43:02 GMT  
		Size: 350.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:677b1bd875c0c817f73c13d5dfbc3fd07fffa7ef77d3ef675d020d744808a363`  
		Last Modified: Tue, 21 Dec 2021 10:43:02 GMT  
		Size: 291.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeaef226499622d4ee9328ba1fcdb9ce2d7458c3e2a55c9cf3f6e2191c89a7bb`  
		Last Modified: Tue, 21 Dec 2021 10:43:23 GMT  
		Size: 215.3 MB (215287320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
