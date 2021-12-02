<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `r-base`

-	[`r-base:4.1.2`](#r-base412)
-	[`r-base:latest`](#r-baselatest)

## `r-base:4.1.2`

```console
$ docker pull r-base@sha256:7a365f1f040a1694eb5d209b3b29faa444cf80f43545d6ac2f3cfc8c92fe67d2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `r-base:4.1.2` - linux; amd64

```console
$ docker pull r-base@sha256:38fe01d6b4744fcaae5609ad5e7f7dfa147da3706954b856666f85e7748d389f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **549.3 MB (549289155 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0bf3dc12c02b68144fa631ee01d1ed7a639639b5e47484f44d40e38324f411bd`
-	Default Command: `["R"]`

```dockerfile
# Thu, 02 Dec 2021 02:50:41 GMT
ADD file:31a3d405e7e9d997819ea8e6e3988121b5abaa06c8bbfcc777bf3564aded3f21 in / 
# Thu, 02 Dec 2021 02:50:42 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 16:04:27 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Thu, 02 Dec 2021 16:04:28 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Thu, 02 Dec 2021 16:04:44 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 16:04:48 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Thu, 02 Dec 2021 16:04:48 GMT
ENV LC_ALL=en_US.UTF-8
# Thu, 02 Dec 2021 16:04:49 GMT
ENV LANG=en_US.UTF-8
# Thu, 02 Dec 2021 16:04:50 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Thu, 02 Dec 2021 16:04:50 GMT
ENV R_BASE_VERSION=4.1.2
# Thu, 02 Dec 2021 16:04:51 GMT
RUN echo "deb http://deb.debian.org/debian experimental main" > /etc/apt/sources.list.d/experimental.list     && echo "deb [trusted=yes] https://eddelbuettel.github.io/ppaR400 ./" > /etc/apt/sources.list.d/edd-r4.list
# Thu, 02 Dec 2021 16:06:27 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 16:06:31 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:e3875f34eeed9a22ac1e5f2fe94e6fe0cd72a84f25c5a217f38aab0504154634`  
		Last Modified: Thu, 02 Dec 2021 02:58:02 GMT  
		Size: 55.6 MB (55567156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b973382c633e00629bda37f8b69a5a093051372acb470b49e9eaed298cd4f61`  
		Last Modified: Thu, 02 Dec 2021 16:06:42 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f86a94c1a1561006a76eaf44a8e977c7d1a4eb758443f2ddac12da1a407362e`  
		Last Modified: Thu, 02 Dec 2021 16:06:43 GMT  
		Size: 25.7 MB (25734194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:634f985f6d276c16d279c6fb5dd7a0af5757ff02f09895c4fba1c60aefca263b`  
		Last Modified: Thu, 02 Dec 2021 16:06:40 GMT  
		Size: 864.6 KB (864617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16935eacd317b1e913edff6a0d14dab57b1989d41f6e453ffa322fa66612ae67`  
		Last Modified: Thu, 02 Dec 2021 16:06:40 GMT  
		Size: 349.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b669150fea75e868971494ffdd28e248d93d5b6ae27e0f8fbc5e7beed694d2b`  
		Last Modified: Thu, 02 Dec 2021 16:06:40 GMT  
		Size: 296.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16edd4f3c1682ea2c1420e2ef6929cdde3ff987481c36f93003d2ced97ceb505`  
		Last Modified: Thu, 02 Dec 2021 16:07:38 GMT  
		Size: 467.1 MB (467120662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:4.1.2` - linux; arm64 variant v8

```console
$ docker pull r-base@sha256:96f97b2394aa9427b2e267a0923260c72c53b923a4a7f7f95385753588b0cac2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **537.8 MB (537845813 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8db25e6538797cf684141e8c8bd68947e1299e5a9ea2b27318a60cba942bbe78`
-	Default Command: `["R"]`

```dockerfile
# Wed, 17 Nov 2021 02:42:59 GMT
ADD file:c4d68bcae684e69a17ac01569a16c332bc925c4359383dbf3f27066f3abb295c in / 
# Wed, 17 Nov 2021 02:43:01 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 09:24:11 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Wed, 17 Nov 2021 09:24:12 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Wed, 17 Nov 2021 09:24:22 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:24:25 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Wed, 17 Nov 2021 09:24:26 GMT
ENV LC_ALL=en_US.UTF-8
# Wed, 17 Nov 2021 09:24:27 GMT
ENV LANG=en_US.UTF-8
# Wed, 17 Nov 2021 09:24:28 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Wed, 17 Nov 2021 09:24:29 GMT
ENV R_BASE_VERSION=4.1.2
# Wed, 17 Nov 2021 09:24:30 GMT
RUN echo "deb http://deb.debian.org/debian experimental main" > /etc/apt/sources.list.d/experimental.list     && echo "deb [trusted=yes] https://eddelbuettel.github.io/ppaR400 ./" > /etc/apt/sources.list.d/edd-r4.list
# Wed, 17 Nov 2021 09:25:55 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:25:56 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:3306c77e3ba6c6431765bbac6b0bbfb35079cfb5d567c3db405aad7687a02603`  
		Last Modified: Wed, 17 Nov 2021 02:52:02 GMT  
		Size: 54.5 MB (54464394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88850b877e844f037a3b637d162846c422434fc9ac156475fbc4491818d3800e`  
		Last Modified: Wed, 17 Nov 2021 09:26:17 GMT  
		Size: 1.8 KB (1760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16bab85edfcf4887dc348fb329c664aaa73da6fca768498ae1ef4c18143410f0`  
		Last Modified: Wed, 17 Nov 2021 09:26:18 GMT  
		Size: 25.7 MB (25725458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:214d9090f79499ab89198766182c5ea16e6e66a4329acefe66c98d33bbff5993`  
		Last Modified: Wed, 17 Nov 2021 09:26:15 GMT  
		Size: 864.6 KB (864612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ba744f38b2c9cdd8eb1afe1e0a05269894dd4bb3835a814ad1067186dec7302`  
		Last Modified: Wed, 17 Nov 2021 09:26:15 GMT  
		Size: 348.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb1c2c8ed5135dfb9531de18cbb591aea65d1388706d68211e447f00ffe1aa6a`  
		Last Modified: Wed, 17 Nov 2021 09:26:14 GMT  
		Size: 291.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45e32ec19a0ecdb3e2ef10e6be0e11af03c5850e4fc303c093370d6afa686f3b`  
		Last Modified: Wed, 17 Nov 2021 09:27:12 GMT  
		Size: 456.8 MB (456788950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:4.1.2` - linux; ppc64le

```console
$ docker pull r-base@sha256:1319918fb43d8e1ae8209ea7dc9117bd49a8d5f39af8fd042fe231b3cce28521
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **532.3 MB (532262775 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d534e51f0b28de723c5d3758c46efa4eb8ab1de46ea26dcc05b007c6b8e296dc`
-	Default Command: `["R"]`

```dockerfile
# Wed, 17 Nov 2021 03:35:47 GMT
ADD file:6ec33732a5ce54ae880804c7d4ce9bbc89ad76007b04d23e694d60679162abdc in / 
# Wed, 17 Nov 2021 03:36:09 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 14:36:04 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Wed, 17 Nov 2021 14:36:13 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Wed, 17 Nov 2021 14:37:04 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 14:37:12 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Wed, 17 Nov 2021 14:37:15 GMT
ENV LC_ALL=en_US.UTF-8
# Wed, 17 Nov 2021 14:37:17 GMT
ENV LANG=en_US.UTF-8
# Wed, 17 Nov 2021 14:37:23 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Wed, 17 Nov 2021 14:37:26 GMT
ENV R_BASE_VERSION=4.1.2
# Wed, 17 Nov 2021 14:37:31 GMT
RUN echo "deb http://deb.debian.org/debian experimental main" > /etc/apt/sources.list.d/experimental.list     && echo "deb [trusted=yes] https://eddelbuettel.github.io/ppaR400 ./" > /etc/apt/sources.list.d/edd-r4.list
# Wed, 17 Nov 2021 14:42:46 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 14:42:54 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:1c92bc8c2e6cbcb9f02ae352b98981f7632bf82483d2ab5a0394f4a3139b3c5b`  
		Last Modified: Wed, 17 Nov 2021 04:12:49 GMT  
		Size: 59.7 MB (59706108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a41091a6c5466c5f119f349015272ea5d9f60e438df65a19eec29aed40a748aa`  
		Last Modified: Wed, 17 Nov 2021 14:43:19 GMT  
		Size: 1.9 KB (1886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ee9788fbadb1fcccd7993a3740b96cf4b5df64a276961ad6b63e70e957c1d7e`  
		Last Modified: Wed, 17 Nov 2021 14:43:20 GMT  
		Size: 26.0 MB (25958946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:848fe08e27f2d543ede8fefd36f42933772911ba2b7f0e923743c37b030b134c`  
		Last Modified: Wed, 17 Nov 2021 14:43:17 GMT  
		Size: 864.6 KB (864617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6429b9ed205043e375a354efa42a61c9eab91c5212f97ca7d6e10729c094977a`  
		Last Modified: Wed, 17 Nov 2021 14:43:16 GMT  
		Size: 351.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ebbf6b1480dbd78c5fe8b0564e79d14f161cc3c5299d33b9e25780f013f2920`  
		Last Modified: Wed, 17 Nov 2021 14:43:17 GMT  
		Size: 295.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d88faad6b04ed2fcec177b3b962494c18eb2fcf4108e5b934c564aae3fe6327`  
		Last Modified: Wed, 17 Nov 2021 14:44:26 GMT  
		Size: 445.7 MB (445730572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:4.1.2` - linux; s390x

```console
$ docker pull r-base@sha256:758a98c272597d4266d4340f12ea2227e5478bb915eab9a63bec6b8e845f007a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **489.6 MB (489557555 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b28903f8cb3cb94b99e2608376791487e368bcbff35b0e03def902eee3e3026f`
-	Default Command: `["R"]`

```dockerfile
# Thu, 02 Dec 2021 07:21:22 GMT
ADD file:6a348f1b2d54149be6cf0ba3d61716a2dcc60830baaf5b96fbcf071b49b2299c in / 
# Thu, 02 Dec 2021 07:21:25 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 12:03:58 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Thu, 02 Dec 2021 12:03:59 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Thu, 02 Dec 2021 12:04:07 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 12:04:09 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Thu, 02 Dec 2021 12:04:10 GMT
ENV LC_ALL=en_US.UTF-8
# Thu, 02 Dec 2021 12:04:10 GMT
ENV LANG=en_US.UTF-8
# Thu, 02 Dec 2021 12:04:10 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Thu, 02 Dec 2021 12:04:11 GMT
ENV R_BASE_VERSION=4.1.2
# Thu, 02 Dec 2021 12:04:11 GMT
RUN echo "deb http://deb.debian.org/debian experimental main" > /etc/apt/sources.list.d/experimental.list     && echo "deb [trusted=yes] https://eddelbuettel.github.io/ppaR400 ./" > /etc/apt/sources.list.d/edd-r4.list
# Thu, 02 Dec 2021 12:05:21 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 12:05:35 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:c913837051836292f57261b37a6bad47f00975da0878d1c5c435a411dceaab93`  
		Last Modified: Thu, 02 Dec 2021 07:27:16 GMT  
		Size: 53.9 MB (53866716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b73d85e266ed3b3c6b7a0c9d83864786aa6b59aeefa3a5a5b53c7fc38b4d713`  
		Last Modified: Thu, 02 Dec 2021 12:05:57 GMT  
		Size: 1.9 KB (1885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b208cd25b6150c0cd5d209567d58ed7ffe8261a8a232d2a7c030c2a8a28aad0d`  
		Last Modified: Thu, 02 Dec 2021 12:05:58 GMT  
		Size: 25.7 MB (25730437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7095a3657f336366cbf2465efde2ce16968823c941e401dda0466e2640036efc`  
		Last Modified: Thu, 02 Dec 2021 12:05:56 GMT  
		Size: 920.2 KB (920187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5038114dd50e18c8dd6526e5091b0e1ad2f1068248b789418dcf7ffb926829dc`  
		Last Modified: Thu, 02 Dec 2021 12:05:56 GMT  
		Size: 349.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:025f268a0e9d503b5286f5557607bf2e83a1b970cdbedc49bb87cc77c052788f`  
		Last Modified: Thu, 02 Dec 2021 12:05:56 GMT  
		Size: 292.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88b913ebe3478969ff134790cf90c82174202a70583854cfaebbba49728a07cf`  
		Last Modified: Thu, 02 Dec 2021 12:06:38 GMT  
		Size: 409.0 MB (409037689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `r-base:latest`

```console
$ docker pull r-base@sha256:7a365f1f040a1694eb5d209b3b29faa444cf80f43545d6ac2f3cfc8c92fe67d2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `r-base:latest` - linux; amd64

```console
$ docker pull r-base@sha256:38fe01d6b4744fcaae5609ad5e7f7dfa147da3706954b856666f85e7748d389f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **549.3 MB (549289155 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0bf3dc12c02b68144fa631ee01d1ed7a639639b5e47484f44d40e38324f411bd`
-	Default Command: `["R"]`

```dockerfile
# Thu, 02 Dec 2021 02:50:41 GMT
ADD file:31a3d405e7e9d997819ea8e6e3988121b5abaa06c8bbfcc777bf3564aded3f21 in / 
# Thu, 02 Dec 2021 02:50:42 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 16:04:27 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Thu, 02 Dec 2021 16:04:28 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Thu, 02 Dec 2021 16:04:44 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 16:04:48 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Thu, 02 Dec 2021 16:04:48 GMT
ENV LC_ALL=en_US.UTF-8
# Thu, 02 Dec 2021 16:04:49 GMT
ENV LANG=en_US.UTF-8
# Thu, 02 Dec 2021 16:04:50 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Thu, 02 Dec 2021 16:04:50 GMT
ENV R_BASE_VERSION=4.1.2
# Thu, 02 Dec 2021 16:04:51 GMT
RUN echo "deb http://deb.debian.org/debian experimental main" > /etc/apt/sources.list.d/experimental.list     && echo "deb [trusted=yes] https://eddelbuettel.github.io/ppaR400 ./" > /etc/apt/sources.list.d/edd-r4.list
# Thu, 02 Dec 2021 16:06:27 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 16:06:31 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:e3875f34eeed9a22ac1e5f2fe94e6fe0cd72a84f25c5a217f38aab0504154634`  
		Last Modified: Thu, 02 Dec 2021 02:58:02 GMT  
		Size: 55.6 MB (55567156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b973382c633e00629bda37f8b69a5a093051372acb470b49e9eaed298cd4f61`  
		Last Modified: Thu, 02 Dec 2021 16:06:42 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f86a94c1a1561006a76eaf44a8e977c7d1a4eb758443f2ddac12da1a407362e`  
		Last Modified: Thu, 02 Dec 2021 16:06:43 GMT  
		Size: 25.7 MB (25734194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:634f985f6d276c16d279c6fb5dd7a0af5757ff02f09895c4fba1c60aefca263b`  
		Last Modified: Thu, 02 Dec 2021 16:06:40 GMT  
		Size: 864.6 KB (864617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16935eacd317b1e913edff6a0d14dab57b1989d41f6e453ffa322fa66612ae67`  
		Last Modified: Thu, 02 Dec 2021 16:06:40 GMT  
		Size: 349.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b669150fea75e868971494ffdd28e248d93d5b6ae27e0f8fbc5e7beed694d2b`  
		Last Modified: Thu, 02 Dec 2021 16:06:40 GMT  
		Size: 296.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16edd4f3c1682ea2c1420e2ef6929cdde3ff987481c36f93003d2ced97ceb505`  
		Last Modified: Thu, 02 Dec 2021 16:07:38 GMT  
		Size: 467.1 MB (467120662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:latest` - linux; arm64 variant v8

```console
$ docker pull r-base@sha256:96f97b2394aa9427b2e267a0923260c72c53b923a4a7f7f95385753588b0cac2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **537.8 MB (537845813 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8db25e6538797cf684141e8c8bd68947e1299e5a9ea2b27318a60cba942bbe78`
-	Default Command: `["R"]`

```dockerfile
# Wed, 17 Nov 2021 02:42:59 GMT
ADD file:c4d68bcae684e69a17ac01569a16c332bc925c4359383dbf3f27066f3abb295c in / 
# Wed, 17 Nov 2021 02:43:01 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 09:24:11 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Wed, 17 Nov 2021 09:24:12 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Wed, 17 Nov 2021 09:24:22 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:24:25 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Wed, 17 Nov 2021 09:24:26 GMT
ENV LC_ALL=en_US.UTF-8
# Wed, 17 Nov 2021 09:24:27 GMT
ENV LANG=en_US.UTF-8
# Wed, 17 Nov 2021 09:24:28 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Wed, 17 Nov 2021 09:24:29 GMT
ENV R_BASE_VERSION=4.1.2
# Wed, 17 Nov 2021 09:24:30 GMT
RUN echo "deb http://deb.debian.org/debian experimental main" > /etc/apt/sources.list.d/experimental.list     && echo "deb [trusted=yes] https://eddelbuettel.github.io/ppaR400 ./" > /etc/apt/sources.list.d/edd-r4.list
# Wed, 17 Nov 2021 09:25:55 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:25:56 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:3306c77e3ba6c6431765bbac6b0bbfb35079cfb5d567c3db405aad7687a02603`  
		Last Modified: Wed, 17 Nov 2021 02:52:02 GMT  
		Size: 54.5 MB (54464394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88850b877e844f037a3b637d162846c422434fc9ac156475fbc4491818d3800e`  
		Last Modified: Wed, 17 Nov 2021 09:26:17 GMT  
		Size: 1.8 KB (1760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16bab85edfcf4887dc348fb329c664aaa73da6fca768498ae1ef4c18143410f0`  
		Last Modified: Wed, 17 Nov 2021 09:26:18 GMT  
		Size: 25.7 MB (25725458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:214d9090f79499ab89198766182c5ea16e6e66a4329acefe66c98d33bbff5993`  
		Last Modified: Wed, 17 Nov 2021 09:26:15 GMT  
		Size: 864.6 KB (864612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ba744f38b2c9cdd8eb1afe1e0a05269894dd4bb3835a814ad1067186dec7302`  
		Last Modified: Wed, 17 Nov 2021 09:26:15 GMT  
		Size: 348.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb1c2c8ed5135dfb9531de18cbb591aea65d1388706d68211e447f00ffe1aa6a`  
		Last Modified: Wed, 17 Nov 2021 09:26:14 GMT  
		Size: 291.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45e32ec19a0ecdb3e2ef10e6be0e11af03c5850e4fc303c093370d6afa686f3b`  
		Last Modified: Wed, 17 Nov 2021 09:27:12 GMT  
		Size: 456.8 MB (456788950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:latest` - linux; ppc64le

```console
$ docker pull r-base@sha256:1319918fb43d8e1ae8209ea7dc9117bd49a8d5f39af8fd042fe231b3cce28521
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **532.3 MB (532262775 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d534e51f0b28de723c5d3758c46efa4eb8ab1de46ea26dcc05b007c6b8e296dc`
-	Default Command: `["R"]`

```dockerfile
# Wed, 17 Nov 2021 03:35:47 GMT
ADD file:6ec33732a5ce54ae880804c7d4ce9bbc89ad76007b04d23e694d60679162abdc in / 
# Wed, 17 Nov 2021 03:36:09 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 14:36:04 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Wed, 17 Nov 2021 14:36:13 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Wed, 17 Nov 2021 14:37:04 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 14:37:12 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Wed, 17 Nov 2021 14:37:15 GMT
ENV LC_ALL=en_US.UTF-8
# Wed, 17 Nov 2021 14:37:17 GMT
ENV LANG=en_US.UTF-8
# Wed, 17 Nov 2021 14:37:23 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Wed, 17 Nov 2021 14:37:26 GMT
ENV R_BASE_VERSION=4.1.2
# Wed, 17 Nov 2021 14:37:31 GMT
RUN echo "deb http://deb.debian.org/debian experimental main" > /etc/apt/sources.list.d/experimental.list     && echo "deb [trusted=yes] https://eddelbuettel.github.io/ppaR400 ./" > /etc/apt/sources.list.d/edd-r4.list
# Wed, 17 Nov 2021 14:42:46 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 14:42:54 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:1c92bc8c2e6cbcb9f02ae352b98981f7632bf82483d2ab5a0394f4a3139b3c5b`  
		Last Modified: Wed, 17 Nov 2021 04:12:49 GMT  
		Size: 59.7 MB (59706108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a41091a6c5466c5f119f349015272ea5d9f60e438df65a19eec29aed40a748aa`  
		Last Modified: Wed, 17 Nov 2021 14:43:19 GMT  
		Size: 1.9 KB (1886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ee9788fbadb1fcccd7993a3740b96cf4b5df64a276961ad6b63e70e957c1d7e`  
		Last Modified: Wed, 17 Nov 2021 14:43:20 GMT  
		Size: 26.0 MB (25958946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:848fe08e27f2d543ede8fefd36f42933772911ba2b7f0e923743c37b030b134c`  
		Last Modified: Wed, 17 Nov 2021 14:43:17 GMT  
		Size: 864.6 KB (864617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6429b9ed205043e375a354efa42a61c9eab91c5212f97ca7d6e10729c094977a`  
		Last Modified: Wed, 17 Nov 2021 14:43:16 GMT  
		Size: 351.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ebbf6b1480dbd78c5fe8b0564e79d14f161cc3c5299d33b9e25780f013f2920`  
		Last Modified: Wed, 17 Nov 2021 14:43:17 GMT  
		Size: 295.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d88faad6b04ed2fcec177b3b962494c18eb2fcf4108e5b934c564aae3fe6327`  
		Last Modified: Wed, 17 Nov 2021 14:44:26 GMT  
		Size: 445.7 MB (445730572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:latest` - linux; s390x

```console
$ docker pull r-base@sha256:758a98c272597d4266d4340f12ea2227e5478bb915eab9a63bec6b8e845f007a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **489.6 MB (489557555 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b28903f8cb3cb94b99e2608376791487e368bcbff35b0e03def902eee3e3026f`
-	Default Command: `["R"]`

```dockerfile
# Thu, 02 Dec 2021 07:21:22 GMT
ADD file:6a348f1b2d54149be6cf0ba3d61716a2dcc60830baaf5b96fbcf071b49b2299c in / 
# Thu, 02 Dec 2021 07:21:25 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 12:03:58 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Thu, 02 Dec 2021 12:03:59 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Thu, 02 Dec 2021 12:04:07 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 12:04:09 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Thu, 02 Dec 2021 12:04:10 GMT
ENV LC_ALL=en_US.UTF-8
# Thu, 02 Dec 2021 12:04:10 GMT
ENV LANG=en_US.UTF-8
# Thu, 02 Dec 2021 12:04:10 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Thu, 02 Dec 2021 12:04:11 GMT
ENV R_BASE_VERSION=4.1.2
# Thu, 02 Dec 2021 12:04:11 GMT
RUN echo "deb http://deb.debian.org/debian experimental main" > /etc/apt/sources.list.d/experimental.list     && echo "deb [trusted=yes] https://eddelbuettel.github.io/ppaR400 ./" > /etc/apt/sources.list.d/edd-r4.list
# Thu, 02 Dec 2021 12:05:21 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 12:05:35 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:c913837051836292f57261b37a6bad47f00975da0878d1c5c435a411dceaab93`  
		Last Modified: Thu, 02 Dec 2021 07:27:16 GMT  
		Size: 53.9 MB (53866716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b73d85e266ed3b3c6b7a0c9d83864786aa6b59aeefa3a5a5b53c7fc38b4d713`  
		Last Modified: Thu, 02 Dec 2021 12:05:57 GMT  
		Size: 1.9 KB (1885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b208cd25b6150c0cd5d209567d58ed7ffe8261a8a232d2a7c030c2a8a28aad0d`  
		Last Modified: Thu, 02 Dec 2021 12:05:58 GMT  
		Size: 25.7 MB (25730437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7095a3657f336366cbf2465efde2ce16968823c941e401dda0466e2640036efc`  
		Last Modified: Thu, 02 Dec 2021 12:05:56 GMT  
		Size: 920.2 KB (920187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5038114dd50e18c8dd6526e5091b0e1ad2f1068248b789418dcf7ffb926829dc`  
		Last Modified: Thu, 02 Dec 2021 12:05:56 GMT  
		Size: 349.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:025f268a0e9d503b5286f5557607bf2e83a1b970cdbedc49bb87cc77c052788f`  
		Last Modified: Thu, 02 Dec 2021 12:05:56 GMT  
		Size: 292.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88b913ebe3478969ff134790cf90c82174202a70583854cfaebbba49728a07cf`  
		Last Modified: Thu, 02 Dec 2021 12:06:38 GMT  
		Size: 409.0 MB (409037689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
