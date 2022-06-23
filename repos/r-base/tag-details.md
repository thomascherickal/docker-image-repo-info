<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `r-base`

-	[`r-base:4.2.0`](#r-base420)
-	[`r-base:latest`](#r-baselatest)

## `r-base:4.2.0`

```console
$ docker pull r-base@sha256:c96cfb8bf55d2608c53a1828ab8d7cdfd536ab66fda8146a200f84414ddfac8d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `r-base:4.2.0` - linux; amd64

```console
$ docker pull r-base@sha256:6572b9195f451ac91d7ca41d341227f7ee41ef05ac1c1b322ff86d006e6d7dab
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **340.2 MB (340222428 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:25ac49f68ec58efe86a3a36ec57cf65c48f9c48ef34febbb76ffeac5e90ebdfd`
-	Default Command: `["R"]`

```dockerfile
# Thu, 23 Jun 2022 00:22:29 GMT
ADD file:5c4e113e3abcb5aeb9438cdaf07c7d900b95e2a30e114fab835f40ea836e1ecb in / 
# Thu, 23 Jun 2022 00:22:30 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 12:27:34 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Thu, 23 Jun 2022 12:27:35 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Thu, 23 Jun 2022 12:27:44 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 12:27:46 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Thu, 23 Jun 2022 12:27:47 GMT
ENV LC_ALL=en_US.UTF-8
# Thu, 23 Jun 2022 12:27:47 GMT
ENV LANG=en_US.UTF-8
# Thu, 23 Jun 2022 12:27:47 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Thu, 23 Jun 2022 12:27:47 GMT
ENV R_BASE_VERSION=4.2.0
# Thu, 23 Jun 2022 12:28:31 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-docopt                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 12:28:33 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:d21669d6bdb9702ceaeab2d3a60e86f23e6da7994b114ec5e684413e2628cb52`  
		Last Modified: Thu, 23 Jun 2022 00:30:22 GMT  
		Size: 53.0 MB (52993978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48065b77120aac393f70211402118875dd5226c209c84b4dbe8bb82be7a7b34d`  
		Last Modified: Thu, 23 Jun 2022 12:28:50 GMT  
		Size: 1.9 KB (1879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60a29b87c3a3f39d684d32917cca608c878315b6896a6bc7ededb8094e4666ca`  
		Last Modified: Thu, 23 Jun 2022 12:28:53 GMT  
		Size: 29.1 MB (29093976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e2f17fd41f07f0335b484c9ba1ce04b9eff860ada76e2b5c38ad80d42be8b5e`  
		Last Modified: Thu, 23 Jun 2022 12:28:50 GMT  
		Size: 864.6 KB (864614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0225d37a93bd8aaf24065570f09b4bb40f3f4225b6b9f4cf1e065945b9f0476e`  
		Last Modified: Thu, 23 Jun 2022 12:28:50 GMT  
		Size: 347.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a275d2aed9458641c1b0063b85b87a5cd177266cd80cbe305ce5dfbf7c8b5762`  
		Last Modified: Thu, 23 Jun 2022 12:29:19 GMT  
		Size: 257.3 MB (257267634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:4.2.0` - linux; arm64 variant v8

```console
$ docker pull r-base@sha256:6a983779870e09d3e9d7d062ec1243373a670fdf472aa9dae4ad2a0270e16398
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **329.4 MB (329381803 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b1ed7a81a958b7977c1429512a822cebd636ca5d2199f586fdc265c45a019fc`
-	Default Command: `["R"]`

```dockerfile
# Thu, 23 Jun 2022 00:43:09 GMT
ADD file:53311373f4d1abfcaa16b8c6fdad786327061f1e5003db1d3c6bdbf5b2c73333 in / 
# Thu, 23 Jun 2022 00:43:10 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 09:55:34 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Thu, 23 Jun 2022 09:55:35 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Thu, 23 Jun 2022 09:55:47 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 09:55:50 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Thu, 23 Jun 2022 09:55:50 GMT
ENV LC_ALL=en_US.UTF-8
# Thu, 23 Jun 2022 09:55:51 GMT
ENV LANG=en_US.UTF-8
# Thu, 23 Jun 2022 09:55:52 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Thu, 23 Jun 2022 09:55:53 GMT
ENV R_BASE_VERSION=4.2.0
# Thu, 23 Jun 2022 09:57:02 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-docopt                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 09:57:03 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:04df16d59bbc997b9cf53108e57268f1beac69c21eb10fac7036d92a38799d9c`  
		Last Modified: Thu, 23 Jun 2022 00:52:10 GMT  
		Size: 52.1 MB (52074599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e44e225ee8267ff47a685e6fb7cb3e044051d38a19f78c599083ef981bd56ee0`  
		Last Modified: Thu, 23 Jun 2022 09:57:23 GMT  
		Size: 1.8 KB (1828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:862e7e0ff7609e8e099b3476c09bf2fa4645d8917ac0ce81c641a21d9b76d943`  
		Last Modified: Thu, 23 Jun 2022 09:57:27 GMT  
		Size: 28.9 MB (28924383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:045b58c869361534b4dec8cb9fd7a07aa8cd72ec3cdfc49898db1c639289a98a`  
		Last Modified: Thu, 23 Jun 2022 09:57:23 GMT  
		Size: 864.6 KB (864603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d3e03efb36a58b2e4b0fef0b6d21e4449eb66de24e494f031e78b6e2350e609`  
		Last Modified: Thu, 23 Jun 2022 09:57:23 GMT  
		Size: 348.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27e47051f85d6a605c04fce2c11d4de6b822f1be1febc1d1bc19c7c0201f9c7a`  
		Last Modified: Thu, 23 Jun 2022 09:57:51 GMT  
		Size: 247.5 MB (247516042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:4.2.0` - linux; ppc64le

```console
$ docker pull r-base@sha256:9e6e298460673240a6a1a76ecead7df84469b82223e629412b7f115ae0322838
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **337.7 MB (337662243 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:738aee963ca73d0f2ecdf52a5927e62791df25e7e4b1a5c5bcf47513e2d697a7`
-	Default Command: `["R"]`

```dockerfile
# Sat, 28 May 2022 01:26:41 GMT
ADD file:c839faac39e30677565fb631dd4f40114392a7a667b8db7f85ca4d8aaeb32ad9 in / 
# Sat, 28 May 2022 01:26:46 GMT
CMD ["bash"]
# Sat, 28 May 2022 18:13:35 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Sat, 28 May 2022 18:13:55 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Sat, 28 May 2022 18:15:13 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 18:15:22 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Sat, 28 May 2022 18:15:24 GMT
ENV LC_ALL=en_US.UTF-8
# Sat, 28 May 2022 18:15:26 GMT
ENV LANG=en_US.UTF-8
# Sat, 28 May 2022 18:15:30 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Sat, 28 May 2022 18:15:33 GMT
ENV R_BASE_VERSION=4.2.0
# Sat, 28 May 2022 18:19:59 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-docopt                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 18:20:05 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:f5e0403edf3ce1164c65241f62272268585e383702736c781adae79230ef3422`  
		Last Modified: Sat, 28 May 2022 01:36:21 GMT  
		Size: 57.2 MB (57161585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93558bc00b065b9fdfdf638afa73d518e79d21654d4fa6ac9bbcf6ae535ff29f`  
		Last Modified: Sat, 28 May 2022 18:20:30 GMT  
		Size: 1.9 KB (1899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:426e1ec607ca488db98567b783ca407dd68087a6d7e2c87853705d3aacda96eb`  
		Last Modified: Sat, 28 May 2022 18:20:34 GMT  
		Size: 28.1 MB (28116523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e2bda5aa6c71f2bcf5010b6c74c566b6b1d20f2965e51e890bac59cc040d212`  
		Last Modified: Sat, 28 May 2022 18:20:31 GMT  
		Size: 864.6 KB (864604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:245fb89f5cf42bcd0902cd81074060fd771c9f04b430c63bf7ad0f86fe52e8de`  
		Last Modified: Sat, 28 May 2022 18:20:30 GMT  
		Size: 352.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8fa9c9dd9a0c1c6447e9df11957b34124507932a8d73669d4acdd4251e71011`  
		Last Modified: Sat, 28 May 2022 18:21:08 GMT  
		Size: 251.5 MB (251517280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:4.2.0` - linux; s390x

```console
$ docker pull r-base@sha256:cc900326084158b0307dd7d75d8b6501052dbbe48e62aa67ce4274c33fa026d9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **304.6 MB (304557262 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9164651256ccfea26be0ae54e54113edd3ed15e3bb3566983c33aa7911d3124d`
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
# Thu, 23 Jun 2022 13:49:21 GMT
ENV R_BASE_VERSION=4.2.0
# Thu, 23 Jun 2022 13:50:03 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-docopt                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 13:50:10 GMT
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
	-	`sha256:77850835a848b97401ca1667e77e64c87f8a0f3f870e8854e20ce7757c08d6d9`  
		Last Modified: Thu, 23 Jun 2022 13:50:46 GMT  
		Size: 223.3 MB (223326594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `r-base:latest`

```console
$ docker pull r-base@sha256:c96cfb8bf55d2608c53a1828ab8d7cdfd536ab66fda8146a200f84414ddfac8d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `r-base:latest` - linux; amd64

```console
$ docker pull r-base@sha256:6572b9195f451ac91d7ca41d341227f7ee41ef05ac1c1b322ff86d006e6d7dab
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **340.2 MB (340222428 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:25ac49f68ec58efe86a3a36ec57cf65c48f9c48ef34febbb76ffeac5e90ebdfd`
-	Default Command: `["R"]`

```dockerfile
# Thu, 23 Jun 2022 00:22:29 GMT
ADD file:5c4e113e3abcb5aeb9438cdaf07c7d900b95e2a30e114fab835f40ea836e1ecb in / 
# Thu, 23 Jun 2022 00:22:30 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 12:27:34 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Thu, 23 Jun 2022 12:27:35 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Thu, 23 Jun 2022 12:27:44 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 12:27:46 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Thu, 23 Jun 2022 12:27:47 GMT
ENV LC_ALL=en_US.UTF-8
# Thu, 23 Jun 2022 12:27:47 GMT
ENV LANG=en_US.UTF-8
# Thu, 23 Jun 2022 12:27:47 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Thu, 23 Jun 2022 12:27:47 GMT
ENV R_BASE_VERSION=4.2.0
# Thu, 23 Jun 2022 12:28:31 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-docopt                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 12:28:33 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:d21669d6bdb9702ceaeab2d3a60e86f23e6da7994b114ec5e684413e2628cb52`  
		Last Modified: Thu, 23 Jun 2022 00:30:22 GMT  
		Size: 53.0 MB (52993978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48065b77120aac393f70211402118875dd5226c209c84b4dbe8bb82be7a7b34d`  
		Last Modified: Thu, 23 Jun 2022 12:28:50 GMT  
		Size: 1.9 KB (1879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60a29b87c3a3f39d684d32917cca608c878315b6896a6bc7ededb8094e4666ca`  
		Last Modified: Thu, 23 Jun 2022 12:28:53 GMT  
		Size: 29.1 MB (29093976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e2f17fd41f07f0335b484c9ba1ce04b9eff860ada76e2b5c38ad80d42be8b5e`  
		Last Modified: Thu, 23 Jun 2022 12:28:50 GMT  
		Size: 864.6 KB (864614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0225d37a93bd8aaf24065570f09b4bb40f3f4225b6b9f4cf1e065945b9f0476e`  
		Last Modified: Thu, 23 Jun 2022 12:28:50 GMT  
		Size: 347.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a275d2aed9458641c1b0063b85b87a5cd177266cd80cbe305ce5dfbf7c8b5762`  
		Last Modified: Thu, 23 Jun 2022 12:29:19 GMT  
		Size: 257.3 MB (257267634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:latest` - linux; arm64 variant v8

```console
$ docker pull r-base@sha256:6a983779870e09d3e9d7d062ec1243373a670fdf472aa9dae4ad2a0270e16398
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **329.4 MB (329381803 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b1ed7a81a958b7977c1429512a822cebd636ca5d2199f586fdc265c45a019fc`
-	Default Command: `["R"]`

```dockerfile
# Thu, 23 Jun 2022 00:43:09 GMT
ADD file:53311373f4d1abfcaa16b8c6fdad786327061f1e5003db1d3c6bdbf5b2c73333 in / 
# Thu, 23 Jun 2022 00:43:10 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 09:55:34 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Thu, 23 Jun 2022 09:55:35 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Thu, 23 Jun 2022 09:55:47 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 09:55:50 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Thu, 23 Jun 2022 09:55:50 GMT
ENV LC_ALL=en_US.UTF-8
# Thu, 23 Jun 2022 09:55:51 GMT
ENV LANG=en_US.UTF-8
# Thu, 23 Jun 2022 09:55:52 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Thu, 23 Jun 2022 09:55:53 GMT
ENV R_BASE_VERSION=4.2.0
# Thu, 23 Jun 2022 09:57:02 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-docopt                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 09:57:03 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:04df16d59bbc997b9cf53108e57268f1beac69c21eb10fac7036d92a38799d9c`  
		Last Modified: Thu, 23 Jun 2022 00:52:10 GMT  
		Size: 52.1 MB (52074599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e44e225ee8267ff47a685e6fb7cb3e044051d38a19f78c599083ef981bd56ee0`  
		Last Modified: Thu, 23 Jun 2022 09:57:23 GMT  
		Size: 1.8 KB (1828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:862e7e0ff7609e8e099b3476c09bf2fa4645d8917ac0ce81c641a21d9b76d943`  
		Last Modified: Thu, 23 Jun 2022 09:57:27 GMT  
		Size: 28.9 MB (28924383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:045b58c869361534b4dec8cb9fd7a07aa8cd72ec3cdfc49898db1c639289a98a`  
		Last Modified: Thu, 23 Jun 2022 09:57:23 GMT  
		Size: 864.6 KB (864603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d3e03efb36a58b2e4b0fef0b6d21e4449eb66de24e494f031e78b6e2350e609`  
		Last Modified: Thu, 23 Jun 2022 09:57:23 GMT  
		Size: 348.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27e47051f85d6a605c04fce2c11d4de6b822f1be1febc1d1bc19c7c0201f9c7a`  
		Last Modified: Thu, 23 Jun 2022 09:57:51 GMT  
		Size: 247.5 MB (247516042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:latest` - linux; ppc64le

```console
$ docker pull r-base@sha256:9e6e298460673240a6a1a76ecead7df84469b82223e629412b7f115ae0322838
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **337.7 MB (337662243 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:738aee963ca73d0f2ecdf52a5927e62791df25e7e4b1a5c5bcf47513e2d697a7`
-	Default Command: `["R"]`

```dockerfile
# Sat, 28 May 2022 01:26:41 GMT
ADD file:c839faac39e30677565fb631dd4f40114392a7a667b8db7f85ca4d8aaeb32ad9 in / 
# Sat, 28 May 2022 01:26:46 GMT
CMD ["bash"]
# Sat, 28 May 2022 18:13:35 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Sat, 28 May 2022 18:13:55 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Sat, 28 May 2022 18:15:13 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 18:15:22 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Sat, 28 May 2022 18:15:24 GMT
ENV LC_ALL=en_US.UTF-8
# Sat, 28 May 2022 18:15:26 GMT
ENV LANG=en_US.UTF-8
# Sat, 28 May 2022 18:15:30 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Sat, 28 May 2022 18:15:33 GMT
ENV R_BASE_VERSION=4.2.0
# Sat, 28 May 2022 18:19:59 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-docopt                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 18:20:05 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:f5e0403edf3ce1164c65241f62272268585e383702736c781adae79230ef3422`  
		Last Modified: Sat, 28 May 2022 01:36:21 GMT  
		Size: 57.2 MB (57161585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93558bc00b065b9fdfdf638afa73d518e79d21654d4fa6ac9bbcf6ae535ff29f`  
		Last Modified: Sat, 28 May 2022 18:20:30 GMT  
		Size: 1.9 KB (1899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:426e1ec607ca488db98567b783ca407dd68087a6d7e2c87853705d3aacda96eb`  
		Last Modified: Sat, 28 May 2022 18:20:34 GMT  
		Size: 28.1 MB (28116523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e2bda5aa6c71f2bcf5010b6c74c566b6b1d20f2965e51e890bac59cc040d212`  
		Last Modified: Sat, 28 May 2022 18:20:31 GMT  
		Size: 864.6 KB (864604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:245fb89f5cf42bcd0902cd81074060fd771c9f04b430c63bf7ad0f86fe52e8de`  
		Last Modified: Sat, 28 May 2022 18:20:30 GMT  
		Size: 352.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8fa9c9dd9a0c1c6447e9df11957b34124507932a8d73669d4acdd4251e71011`  
		Last Modified: Sat, 28 May 2022 18:21:08 GMT  
		Size: 251.5 MB (251517280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:latest` - linux; s390x

```console
$ docker pull r-base@sha256:cc900326084158b0307dd7d75d8b6501052dbbe48e62aa67ce4274c33fa026d9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **304.6 MB (304557262 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9164651256ccfea26be0ae54e54113edd3ed15e3bb3566983c33aa7911d3124d`
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
# Thu, 23 Jun 2022 13:49:21 GMT
ENV R_BASE_VERSION=4.2.0
# Thu, 23 Jun 2022 13:50:03 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-docopt                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 13:50:10 GMT
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
	-	`sha256:77850835a848b97401ca1667e77e64c87f8a0f3f870e8854e20ce7757c08d6d9`  
		Last Modified: Thu, 23 Jun 2022 13:50:46 GMT  
		Size: 223.3 MB (223326594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
