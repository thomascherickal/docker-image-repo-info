<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `r-base`

-	[`r-base:4.0.4`](#r-base404)
-	[`r-base:latest`](#r-baselatest)

## `r-base:4.0.4`

```console
$ docker pull r-base@sha256:adf75d39c2972b6c3f4207fd04f6a56aa3f2616474182e8414f0e1f2fb13bb11
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `r-base:4.0.4` - linux; amd64

```console
$ docker pull r-base@sha256:b453a2948b4fdc5a07940a076bf9d187e9acff344b4e9d5dd81a657e5142a168
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **323.9 MB (323938278 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:640cb54282114b70783269b890bf8daf5c22d436238405265cab644da51eeb99`
-	Default Command: `["R"]`

```dockerfile
# Fri, 12 Mar 2021 02:22:58 GMT
ADD file:f7ba3c021cb8d4754b008c0e16ed267d3af0e2b300963191be16d6d0e46312f9 in / 
# Fri, 12 Mar 2021 02:22:58 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 12:38:35 GMT
LABEL org.label-schema.license=GPL-2.0 org.label-schema.vcs-url=https://github.com/rocker-org/r-base org.label-schema.vendor=Rocker Project maintainer=Dirk Eddelbuettel <edd@debian.org>
# Fri, 12 Mar 2021 12:38:37 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Fri, 12 Mar 2021 12:38:59 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 12:39:03 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Fri, 12 Mar 2021 12:39:04 GMT
ENV LC_ALL=en_US.UTF-8
# Fri, 12 Mar 2021 12:39:04 GMT
ENV LANG=en_US.UTF-8
# Fri, 12 Mar 2021 12:39:06 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Fri, 12 Mar 2021 12:39:06 GMT
ENV R_BASE_VERSION=4.0.4
# Fri, 12 Mar 2021 12:40:22 GMT
RUN apt-get update         && apt-get install -t unstable -y --no-install-recommends                 gcc-9-base                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 12:40:24 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:e084fead077cfeb7d41648a77bc726866fae51276550348d1337cad9637493ef`  
		Last Modified: Fri, 12 Mar 2021 02:30:52 GMT  
		Size: 54.8 MB (54835743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a9d074e876f1de697195ae20e600a47f99d2006f033fa58e712713077e52569`  
		Last Modified: Fri, 12 Mar 2021 12:40:40 GMT  
		Size: 1.9 KB (1875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:273369cade45c586edefa8279f0fc330ffb8efdd4fe7c332aace317f7e00783c`  
		Last Modified: Fri, 12 Mar 2021 12:40:45 GMT  
		Size: 25.6 MB (25615618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69a65a829f14632f9d2cd9fab1e36a57f34337d2116a1aa1ddadfce15db470af`  
		Last Modified: Fri, 12 Mar 2021 12:40:40 GMT  
		Size: 864.6 KB (864593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa721b6fbf89789e8fbc672347aac18b45b3cfb81cf1a81fd8bddb03a65654d4`  
		Last Modified: Fri, 12 Mar 2021 12:40:39 GMT  
		Size: 350.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:628c2def93fe951eebb9015aee79d08ea4ce2aa62f65a0d0287de1f073866abd`  
		Last Modified: Fri, 12 Mar 2021 12:41:30 GMT  
		Size: 242.6 MB (242620099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:4.0.4` - linux; arm64 variant v8

```console
$ docker pull r-base@sha256:64a41f53ee6ef3c2e81bcbbc096c496ddc55018b814364b147ac7ad9792562b1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **311.5 MB (311544086 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b863e4478edfe91940b81cf681015954e2318efb1fabf95154504ec5db34996`
-	Default Command: `["R"]`

```dockerfile
# Fri, 12 Mar 2021 01:57:43 GMT
ADD file:22a6957379e9e833185367bde98358ddb39fa0d834fe1ef9b10d19361a9f52e0 in / 
# Fri, 12 Mar 2021 01:57:44 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 18:59:16 GMT
LABEL org.label-schema.license=GPL-2.0 org.label-schema.vcs-url=https://github.com/rocker-org/r-base org.label-schema.vendor=Rocker Project maintainer=Dirk Eddelbuettel <edd@debian.org>
# Fri, 12 Mar 2021 18:59:20 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Fri, 12 Mar 2021 18:59:43 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 18:59:50 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Fri, 12 Mar 2021 18:59:51 GMT
ENV LC_ALL=en_US.UTF-8
# Fri, 12 Mar 2021 18:59:52 GMT
ENV LANG=en_US.UTF-8
# Fri, 12 Mar 2021 18:59:57 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Fri, 12 Mar 2021 18:59:58 GMT
ENV R_BASE_VERSION=4.0.4
# Fri, 12 Mar 2021 19:01:32 GMT
RUN apt-get update         && apt-get install -t unstable -y --no-install-recommends                 gcc-9-base                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 19:01:37 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:e1386d46900c29cd2b6bae92f6d6d5f608591bc0a86997705f2b1208414bd7cd`  
		Last Modified: Fri, 12 Mar 2021 02:04:37 GMT  
		Size: 53.5 MB (53521148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:452c8a22d66e6fce594a2d949d0808c8423eef1703ad311b35dd7cc26ac57e51`  
		Last Modified: Fri, 12 Mar 2021 19:01:55 GMT  
		Size: 1.9 KB (1877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f8aac9b045980372d68cc5cf5ddb5ab13075003559bf7d273e069801fe5b0af`  
		Last Modified: Fri, 12 Mar 2021 19:02:00 GMT  
		Size: 25.6 MB (25608783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b969f8527593e0b019264c1e4b223b6e680ec4d14fa716b6df9956a6e3d76a1a`  
		Last Modified: Fri, 12 Mar 2021 19:01:57 GMT  
		Size: 864.6 KB (864592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33761823a9844d0f66fc2810560332cde7a012db18550b659356fe25d567b7c7`  
		Last Modified: Fri, 12 Mar 2021 19:01:56 GMT  
		Size: 351.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a064031b78d06a1860ff07f6eec014fddbbe1a4f2ce434ccde09ea1525eff7fc`  
		Last Modified: Fri, 12 Mar 2021 19:02:41 GMT  
		Size: 231.5 MB (231547335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:4.0.4` - linux; ppc64le

```console
$ docker pull r-base@sha256:90b5728f2e74112824e0c494973324d1d5acf43fd8e577f29e63f071ee394ed0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **321.8 MB (321803954 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c956240ac40ab9a15dd788f0bb34bc7708c08b096d5699aca12d025130c9073`
-	Default Command: `["R"]`

```dockerfile
# Fri, 12 Mar 2021 02:35:13 GMT
ADD file:f51fc83967d32c95b96fdcd3bb01770be009f079b97ead429f2d914a4463e9af in / 
# Fri, 12 Mar 2021 02:35:25 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 15:26:17 GMT
LABEL org.label-schema.license=GPL-2.0 org.label-schema.vcs-url=https://github.com/rocker-org/r-base org.label-schema.vendor=Rocker Project maintainer=Dirk Eddelbuettel <edd@debian.org>
# Fri, 12 Mar 2021 15:26:38 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Fri, 12 Mar 2021 15:28:02 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 15:28:19 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Fri, 12 Mar 2021 15:28:21 GMT
ENV LC_ALL=en_US.UTF-8
# Fri, 12 Mar 2021 15:28:24 GMT
ENV LANG=en_US.UTF-8
# Fri, 12 Mar 2021 15:28:37 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Fri, 12 Mar 2021 15:28:47 GMT
ENV R_BASE_VERSION=4.0.4
# Fri, 12 Mar 2021 15:37:50 GMT
RUN apt-get update         && apt-get install -t unstable -y --no-install-recommends                 gcc-9-base                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 15:37:58 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:c73595d876be0af8bade8ed657ff774b66282afd5232e3d0803c40419cad1267`  
		Last Modified: Fri, 12 Mar 2021 02:53:04 GMT  
		Size: 58.7 MB (58746547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f253ae15ba7f88204ad373bfe2a9c8f1a701ae05b753c2fe0b9ede6b65bbdab`  
		Last Modified: Fri, 12 Mar 2021 15:38:24 GMT  
		Size: 1.9 KB (1890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c20756f82670a94ea97e882769b85ff13842fbf1d397a29c0f7c1ae0790defa7`  
		Last Modified: Fri, 12 Mar 2021 15:38:25 GMT  
		Size: 25.8 MB (25829875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bd481fec8805e6324166caa2df8cc4d654300fb273c94e856480d7f4fcc1bab`  
		Last Modified: Fri, 12 Mar 2021 15:38:21 GMT  
		Size: 864.6 KB (864594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:496a685a5f8c5c6f77a2595d41a455d7f830f365185c07e81014306f8a4dfd2b`  
		Last Modified: Fri, 12 Mar 2021 15:38:20 GMT  
		Size: 351.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db4e335e22dae4585e5b8a3269f8290e8ea16ebb5e43dc12601962b272e60e74`  
		Last Modified: Fri, 12 Mar 2021 15:39:01 GMT  
		Size: 236.4 MB (236360697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:4.0.4` - linux; s390x

```console
$ docker pull r-base@sha256:c35142844dbb76de262d66dbf71ba95feecd1d15fd3032cbd96f47030322a73c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.2 MB (289241488 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:775206824ecf65a42f8d28fb7ffaadf65545a1f0bb46317143df3f7d5984b882`
-	Default Command: `["R"]`

```dockerfile
# Fri, 26 Mar 2021 10:55:05 GMT
ADD file:c68277f5942da894b87824e7be5e490cdc087530373096bc568a709716c8bd7b in / 
# Fri, 26 Mar 2021 10:55:10 GMT
CMD ["bash"]
# Fri, 26 Mar 2021 16:44:07 GMT
LABEL org.label-schema.license=GPL-2.0 org.label-schema.vcs-url=https://github.com/rocker-org/r-base org.label-schema.vendor=Rocker Project maintainer=Dirk Eddelbuettel <edd@debian.org>
# Fri, 26 Mar 2021 16:44:09 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Fri, 26 Mar 2021 16:44:30 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 16:44:36 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Fri, 26 Mar 2021 16:44:36 GMT
ENV LC_ALL=en_US.UTF-8
# Fri, 26 Mar 2021 16:44:37 GMT
ENV LANG=en_US.UTF-8
# Fri, 26 Mar 2021 16:44:39 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Fri, 26 Mar 2021 16:44:39 GMT
ENV R_BASE_VERSION=4.0.4
# Fri, 26 Mar 2021 16:46:30 GMT
RUN apt-get update         && apt-get install -t unstable -y --no-install-recommends                 gcc-9-base                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 16:46:48 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:d49851850d45c1c8e424bfcbe79b41751f17923fe040a5364ea54e2ebe4dcbda`  
		Last Modified: Fri, 26 Mar 2021 10:58:54 GMT  
		Size: 53.1 MB (53147632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d46a860516c38c0e5b0c3d904d41777243d4f966da5aeb74c476c956d3d003eb`  
		Last Modified: Fri, 26 Mar 2021 16:47:01 GMT  
		Size: 1.9 KB (1874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:497852a9ea1e6ae81743fbea2cf30994fe7df72f115664a4d18908132c26cb9a`  
		Last Modified: Fri, 26 Mar 2021 16:47:04 GMT  
		Size: 25.6 MB (25634143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ed3fb0e7c6dd41b08a43dd823530059e64e9cec40446fbb31823e80c0a4e712`  
		Last Modified: Fri, 26 Mar 2021 16:47:02 GMT  
		Size: 920.2 KB (920156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7b8d3aff9b383392db8c897d4009b972893c7e6c6363156e4fd6c021017277c`  
		Last Modified: Fri, 26 Mar 2021 16:47:01 GMT  
		Size: 350.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:862e1adadda82058af42fb1ac07f26ddf15c6c4925c45ce4e4e9cd9f025bbc2a`  
		Last Modified: Fri, 26 Mar 2021 16:47:24 GMT  
		Size: 209.5 MB (209537333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `r-base:latest`

```console
$ docker pull r-base@sha256:adf75d39c2972b6c3f4207fd04f6a56aa3f2616474182e8414f0e1f2fb13bb11
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `r-base:latest` - linux; amd64

```console
$ docker pull r-base@sha256:b453a2948b4fdc5a07940a076bf9d187e9acff344b4e9d5dd81a657e5142a168
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **323.9 MB (323938278 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:640cb54282114b70783269b890bf8daf5c22d436238405265cab644da51eeb99`
-	Default Command: `["R"]`

```dockerfile
# Fri, 12 Mar 2021 02:22:58 GMT
ADD file:f7ba3c021cb8d4754b008c0e16ed267d3af0e2b300963191be16d6d0e46312f9 in / 
# Fri, 12 Mar 2021 02:22:58 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 12:38:35 GMT
LABEL org.label-schema.license=GPL-2.0 org.label-schema.vcs-url=https://github.com/rocker-org/r-base org.label-schema.vendor=Rocker Project maintainer=Dirk Eddelbuettel <edd@debian.org>
# Fri, 12 Mar 2021 12:38:37 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Fri, 12 Mar 2021 12:38:59 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 12:39:03 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Fri, 12 Mar 2021 12:39:04 GMT
ENV LC_ALL=en_US.UTF-8
# Fri, 12 Mar 2021 12:39:04 GMT
ENV LANG=en_US.UTF-8
# Fri, 12 Mar 2021 12:39:06 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Fri, 12 Mar 2021 12:39:06 GMT
ENV R_BASE_VERSION=4.0.4
# Fri, 12 Mar 2021 12:40:22 GMT
RUN apt-get update         && apt-get install -t unstable -y --no-install-recommends                 gcc-9-base                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 12:40:24 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:e084fead077cfeb7d41648a77bc726866fae51276550348d1337cad9637493ef`  
		Last Modified: Fri, 12 Mar 2021 02:30:52 GMT  
		Size: 54.8 MB (54835743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a9d074e876f1de697195ae20e600a47f99d2006f033fa58e712713077e52569`  
		Last Modified: Fri, 12 Mar 2021 12:40:40 GMT  
		Size: 1.9 KB (1875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:273369cade45c586edefa8279f0fc330ffb8efdd4fe7c332aace317f7e00783c`  
		Last Modified: Fri, 12 Mar 2021 12:40:45 GMT  
		Size: 25.6 MB (25615618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69a65a829f14632f9d2cd9fab1e36a57f34337d2116a1aa1ddadfce15db470af`  
		Last Modified: Fri, 12 Mar 2021 12:40:40 GMT  
		Size: 864.6 KB (864593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa721b6fbf89789e8fbc672347aac18b45b3cfb81cf1a81fd8bddb03a65654d4`  
		Last Modified: Fri, 12 Mar 2021 12:40:39 GMT  
		Size: 350.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:628c2def93fe951eebb9015aee79d08ea4ce2aa62f65a0d0287de1f073866abd`  
		Last Modified: Fri, 12 Mar 2021 12:41:30 GMT  
		Size: 242.6 MB (242620099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:latest` - linux; arm64 variant v8

```console
$ docker pull r-base@sha256:64a41f53ee6ef3c2e81bcbbc096c496ddc55018b814364b147ac7ad9792562b1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **311.5 MB (311544086 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b863e4478edfe91940b81cf681015954e2318efb1fabf95154504ec5db34996`
-	Default Command: `["R"]`

```dockerfile
# Fri, 12 Mar 2021 01:57:43 GMT
ADD file:22a6957379e9e833185367bde98358ddb39fa0d834fe1ef9b10d19361a9f52e0 in / 
# Fri, 12 Mar 2021 01:57:44 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 18:59:16 GMT
LABEL org.label-schema.license=GPL-2.0 org.label-schema.vcs-url=https://github.com/rocker-org/r-base org.label-schema.vendor=Rocker Project maintainer=Dirk Eddelbuettel <edd@debian.org>
# Fri, 12 Mar 2021 18:59:20 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Fri, 12 Mar 2021 18:59:43 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 18:59:50 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Fri, 12 Mar 2021 18:59:51 GMT
ENV LC_ALL=en_US.UTF-8
# Fri, 12 Mar 2021 18:59:52 GMT
ENV LANG=en_US.UTF-8
# Fri, 12 Mar 2021 18:59:57 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Fri, 12 Mar 2021 18:59:58 GMT
ENV R_BASE_VERSION=4.0.4
# Fri, 12 Mar 2021 19:01:32 GMT
RUN apt-get update         && apt-get install -t unstable -y --no-install-recommends                 gcc-9-base                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 19:01:37 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:e1386d46900c29cd2b6bae92f6d6d5f608591bc0a86997705f2b1208414bd7cd`  
		Last Modified: Fri, 12 Mar 2021 02:04:37 GMT  
		Size: 53.5 MB (53521148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:452c8a22d66e6fce594a2d949d0808c8423eef1703ad311b35dd7cc26ac57e51`  
		Last Modified: Fri, 12 Mar 2021 19:01:55 GMT  
		Size: 1.9 KB (1877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f8aac9b045980372d68cc5cf5ddb5ab13075003559bf7d273e069801fe5b0af`  
		Last Modified: Fri, 12 Mar 2021 19:02:00 GMT  
		Size: 25.6 MB (25608783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b969f8527593e0b019264c1e4b223b6e680ec4d14fa716b6df9956a6e3d76a1a`  
		Last Modified: Fri, 12 Mar 2021 19:01:57 GMT  
		Size: 864.6 KB (864592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33761823a9844d0f66fc2810560332cde7a012db18550b659356fe25d567b7c7`  
		Last Modified: Fri, 12 Mar 2021 19:01:56 GMT  
		Size: 351.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a064031b78d06a1860ff07f6eec014fddbbe1a4f2ce434ccde09ea1525eff7fc`  
		Last Modified: Fri, 12 Mar 2021 19:02:41 GMT  
		Size: 231.5 MB (231547335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:latest` - linux; ppc64le

```console
$ docker pull r-base@sha256:90b5728f2e74112824e0c494973324d1d5acf43fd8e577f29e63f071ee394ed0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **321.8 MB (321803954 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c956240ac40ab9a15dd788f0bb34bc7708c08b096d5699aca12d025130c9073`
-	Default Command: `["R"]`

```dockerfile
# Fri, 12 Mar 2021 02:35:13 GMT
ADD file:f51fc83967d32c95b96fdcd3bb01770be009f079b97ead429f2d914a4463e9af in / 
# Fri, 12 Mar 2021 02:35:25 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 15:26:17 GMT
LABEL org.label-schema.license=GPL-2.0 org.label-schema.vcs-url=https://github.com/rocker-org/r-base org.label-schema.vendor=Rocker Project maintainer=Dirk Eddelbuettel <edd@debian.org>
# Fri, 12 Mar 2021 15:26:38 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Fri, 12 Mar 2021 15:28:02 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 15:28:19 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Fri, 12 Mar 2021 15:28:21 GMT
ENV LC_ALL=en_US.UTF-8
# Fri, 12 Mar 2021 15:28:24 GMT
ENV LANG=en_US.UTF-8
# Fri, 12 Mar 2021 15:28:37 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Fri, 12 Mar 2021 15:28:47 GMT
ENV R_BASE_VERSION=4.0.4
# Fri, 12 Mar 2021 15:37:50 GMT
RUN apt-get update         && apt-get install -t unstable -y --no-install-recommends                 gcc-9-base                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 15:37:58 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:c73595d876be0af8bade8ed657ff774b66282afd5232e3d0803c40419cad1267`  
		Last Modified: Fri, 12 Mar 2021 02:53:04 GMT  
		Size: 58.7 MB (58746547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f253ae15ba7f88204ad373bfe2a9c8f1a701ae05b753c2fe0b9ede6b65bbdab`  
		Last Modified: Fri, 12 Mar 2021 15:38:24 GMT  
		Size: 1.9 KB (1890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c20756f82670a94ea97e882769b85ff13842fbf1d397a29c0f7c1ae0790defa7`  
		Last Modified: Fri, 12 Mar 2021 15:38:25 GMT  
		Size: 25.8 MB (25829875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bd481fec8805e6324166caa2df8cc4d654300fb273c94e856480d7f4fcc1bab`  
		Last Modified: Fri, 12 Mar 2021 15:38:21 GMT  
		Size: 864.6 KB (864594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:496a685a5f8c5c6f77a2595d41a455d7f830f365185c07e81014306f8a4dfd2b`  
		Last Modified: Fri, 12 Mar 2021 15:38:20 GMT  
		Size: 351.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db4e335e22dae4585e5b8a3269f8290e8ea16ebb5e43dc12601962b272e60e74`  
		Last Modified: Fri, 12 Mar 2021 15:39:01 GMT  
		Size: 236.4 MB (236360697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:latest` - linux; s390x

```console
$ docker pull r-base@sha256:c35142844dbb76de262d66dbf71ba95feecd1d15fd3032cbd96f47030322a73c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.2 MB (289241488 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:775206824ecf65a42f8d28fb7ffaadf65545a1f0bb46317143df3f7d5984b882`
-	Default Command: `["R"]`

```dockerfile
# Fri, 26 Mar 2021 10:55:05 GMT
ADD file:c68277f5942da894b87824e7be5e490cdc087530373096bc568a709716c8bd7b in / 
# Fri, 26 Mar 2021 10:55:10 GMT
CMD ["bash"]
# Fri, 26 Mar 2021 16:44:07 GMT
LABEL org.label-schema.license=GPL-2.0 org.label-schema.vcs-url=https://github.com/rocker-org/r-base org.label-schema.vendor=Rocker Project maintainer=Dirk Eddelbuettel <edd@debian.org>
# Fri, 26 Mar 2021 16:44:09 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Fri, 26 Mar 2021 16:44:30 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 16:44:36 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Fri, 26 Mar 2021 16:44:36 GMT
ENV LC_ALL=en_US.UTF-8
# Fri, 26 Mar 2021 16:44:37 GMT
ENV LANG=en_US.UTF-8
# Fri, 26 Mar 2021 16:44:39 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Fri, 26 Mar 2021 16:44:39 GMT
ENV R_BASE_VERSION=4.0.4
# Fri, 26 Mar 2021 16:46:30 GMT
RUN apt-get update         && apt-get install -t unstable -y --no-install-recommends                 gcc-9-base                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 16:46:48 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:d49851850d45c1c8e424bfcbe79b41751f17923fe040a5364ea54e2ebe4dcbda`  
		Last Modified: Fri, 26 Mar 2021 10:58:54 GMT  
		Size: 53.1 MB (53147632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d46a860516c38c0e5b0c3d904d41777243d4f966da5aeb74c476c956d3d003eb`  
		Last Modified: Fri, 26 Mar 2021 16:47:01 GMT  
		Size: 1.9 KB (1874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:497852a9ea1e6ae81743fbea2cf30994fe7df72f115664a4d18908132c26cb9a`  
		Last Modified: Fri, 26 Mar 2021 16:47:04 GMT  
		Size: 25.6 MB (25634143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ed3fb0e7c6dd41b08a43dd823530059e64e9cec40446fbb31823e80c0a4e712`  
		Last Modified: Fri, 26 Mar 2021 16:47:02 GMT  
		Size: 920.2 KB (920156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7b8d3aff9b383392db8c897d4009b972893c7e6c6363156e4fd6c021017277c`  
		Last Modified: Fri, 26 Mar 2021 16:47:01 GMT  
		Size: 350.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:862e1adadda82058af42fb1ac07f26ddf15c6c4925c45ce4e4e9cd9f025bbc2a`  
		Last Modified: Fri, 26 Mar 2021 16:47:24 GMT  
		Size: 209.5 MB (209537333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
