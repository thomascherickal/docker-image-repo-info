<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `r-base`

-	[`r-base:4.1.1`](#r-base411)
-	[`r-base:latest`](#r-baselatest)

## `r-base:4.1.1`

```console
$ docker pull r-base@sha256:3c0bda6cad11e1498daa62c13bd5c19ac9d322d1dbb460f7ecf26f25c2559ef6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `r-base:4.1.1` - linux; amd64

```console
$ docker pull r-base@sha256:c7361b639c83d25cfa3d869dfb4608b9445e9da96b0b13a97c396e286b2fda63
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **330.2 MB (330235437 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e83ee6a20d40957a08ebe836619d888259b4897c9e0e800ad952f5633a8cdb92`
-	Default Command: `["R"]`

```dockerfile
# Thu, 22 Jul 2021 00:47:30 GMT
ADD file:aefd1b2aad4a1d98fd82d86cab1e66f8f172c748e69090a4938ded7681a5fcfe in / 
# Thu, 22 Jul 2021 00:47:30 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 14:25:02 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Thu, 22 Jul 2021 14:25:03 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Thu, 22 Jul 2021 14:25:13 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 14:25:15 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Thu, 22 Jul 2021 14:25:15 GMT
ENV LC_ALL=en_US.UTF-8
# Thu, 22 Jul 2021 14:25:16 GMT
ENV LANG=en_US.UTF-8
# Thu, 22 Jul 2021 14:25:16 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Tue, 10 Aug 2021 20:32:35 GMT
ENV R_BASE_VERSION=4.1.1
# Tue, 10 Aug 2021 20:32:36 GMT
RUN echo "deb http://deb.debian.org/debian experimental main" > /etc/apt/sources.list.d/experimental.list     && echo "deb [trusted=yes] https://eddelbuettel.github.io/ppaR400 ./" > /etc/apt/sources.list.d/edd-r4.list
# Tue, 10 Aug 2021 20:33:27 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Tue, 10 Aug 2021 20:33:29 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:7b303595d9b321a9020d0ddbf1dea4c83237e2367117606a8d5466c446714ba1`  
		Last Modified: Thu, 22 Jul 2021 00:53:44 GMT  
		Size: 54.9 MB (54904726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:269a52eb0491fa8f50f18f968e9a26e2c3f139332e157f2af3eaaa4ad8fbdab5`  
		Last Modified: Thu, 22 Jul 2021 14:26:23 GMT  
		Size: 1.9 KB (1878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ded859387bdafb915ae926a385218acb88202f871dab977fc1f53237dfb4a079`  
		Last Modified: Thu, 22 Jul 2021 14:26:23 GMT  
		Size: 25.6 MB (25629332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e9a9ca14ab54b7dcc64efd3dd1e59caa23457c62f787811a6dd14e73aeb8421`  
		Last Modified: Thu, 22 Jul 2021 14:26:21 GMT  
		Size: 864.6 KB (864588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2833e2a4a5cdc17504b1c82018201d1ab11fd9561b5f6b53a380150c056f80f`  
		Last Modified: Thu, 22 Jul 2021 14:26:20 GMT  
		Size: 349.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1a5465a8d4cda5658398f72d4f6457963e87134ab528e8b85290052426edebf`  
		Last Modified: Tue, 10 Aug 2021 20:33:42 GMT  
		Size: 297.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f80170cdc1529cd3405628fe4d2cf9551838ea19dd0878401a648fb547577f47`  
		Last Modified: Tue, 10 Aug 2021 20:34:10 GMT  
		Size: 248.8 MB (248834267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:4.1.1` - linux; arm64 variant v8

```console
$ docker pull r-base@sha256:679cf53883c00279b771519f41ca013eab405531ad6165dde18d7dd28735e1cd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **311.2 MB (311213242 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67a98d91c624eb33fa56c2b57145a2388ab2b953ac42f2eb0d348e4e9b99733c`
-	Default Command: `["R"]`

```dockerfile
# Tue, 17 Aug 2021 01:48:44 GMT
ADD file:3893bd6ddc225c2b660af0396860193305baef444ab5aeb369ea28b0679c3a14 in / 
# Tue, 17 Aug 2021 01:48:44 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 11:46:00 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Tue, 17 Aug 2021 11:46:01 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Tue, 17 Aug 2021 11:46:09 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 11:46:12 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Tue, 17 Aug 2021 11:46:12 GMT
ENV LC_ALL=en_US.UTF-8
# Tue, 17 Aug 2021 11:46:13 GMT
ENV LANG=en_US.UTF-8
# Tue, 17 Aug 2021 11:46:13 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Tue, 17 Aug 2021 11:46:13 GMT
ENV R_BASE_VERSION=4.1.1
# Tue, 17 Aug 2021 11:46:14 GMT
RUN echo "deb http://deb.debian.org/debian experimental main" > /etc/apt/sources.list.d/experimental.list     && echo "deb [trusted=yes] https://eddelbuettel.github.io/ppaR400 ./" > /etc/apt/sources.list.d/edd-r4.list
# Tue, 17 Aug 2021 11:46:59 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 11:47:01 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:20341cea39b7b052e8fa46c85b6e6d17dbd3830a13c140eb6d72f4dd6ec5b8e6`  
		Last Modified: Tue, 17 Aug 2021 01:58:25 GMT  
		Size: 53.6 MB (53595238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d037b018b43733167395523bdbb299306664767079cc9a989ef5135870cf8c69`  
		Last Modified: Tue, 17 Aug 2021 11:47:24 GMT  
		Size: 1.9 KB (1878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bb43f2d04b40904a1a96073154eec86259d17631ae2830fdf99353dd152b7e4`  
		Last Modified: Tue, 17 Aug 2021 11:47:25 GMT  
		Size: 25.6 MB (25632791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55477b466c6bed3955a5b74780ade5336a26f29a1dcb64c25770af9c61e4c438`  
		Last Modified: Tue, 17 Aug 2021 11:47:22 GMT  
		Size: 864.6 KB (864593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b41b3fb56558348cd5487cadbfcc1a49eb66d6930e6a2796d4cd74be2b56c45`  
		Last Modified: Tue, 17 Aug 2021 11:47:22 GMT  
		Size: 349.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0da01b3ed82dc66c3ec450a010ee2a05457729da5a15797d6766a93bab5d0152`  
		Last Modified: Tue, 17 Aug 2021 11:47:22 GMT  
		Size: 294.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3071f1c57dd21ec88ee4baec1631678d84306d7a97fe0ee99200fdd75fdc87f1`  
		Last Modified: Tue, 17 Aug 2021 11:47:52 GMT  
		Size: 231.1 MB (231118099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:4.1.1` - linux; ppc64le

```console
$ docker pull r-base@sha256:f9b2f99b1b4bd99c232eb973ac719384c9d9b37c1664f82587320397da366583
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **328.7 MB (328722936 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f0c2947da572eb28cfa944fab76b9f3595d79864885cc23a1fb4054d0966b4d`
-	Default Command: `["R"]`

```dockerfile
# Thu, 22 Jul 2021 00:21:17 GMT
ADD file:609f34b74745c6e0ad3453b3e7043b6aa9a8bd1f08450e5dacc435f2e02cfdc1 in / 
# Thu, 22 Jul 2021 00:21:28 GMT
CMD ["bash"]
# Fri, 23 Jul 2021 00:06:03 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Fri, 23 Jul 2021 00:06:45 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Fri, 23 Jul 2021 00:09:26 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Fri, 23 Jul 2021 00:09:52 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Fri, 23 Jul 2021 00:10:05 GMT
ENV LC_ALL=en_US.UTF-8
# Fri, 23 Jul 2021 00:10:14 GMT
ENV LANG=en_US.UTF-8
# Fri, 23 Jul 2021 00:10:38 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Tue, 10 Aug 2021 21:20:29 GMT
ENV R_BASE_VERSION=4.1.1
# Tue, 10 Aug 2021 21:20:43 GMT
RUN echo "deb http://deb.debian.org/debian experimental main" > /etc/apt/sources.list.d/experimental.list     && echo "deb [trusted=yes] https://eddelbuettel.github.io/ppaR400 ./" > /etc/apt/sources.list.d/edd-r4.list
# Tue, 10 Aug 2021 21:30:56 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Tue, 10 Aug 2021 21:31:02 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:a9effce78a0f7eaff718bcd66572e6000ce0a0c44f2947bbc1908696da72910b`  
		Last Modified: Thu, 22 Jul 2021 00:29:51 GMT  
		Size: 58.8 MB (58813298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00357bf8a668e7e05cde7ec787f1f104c8f855f63110ecc5dac594438e939bf7`  
		Last Modified: Fri, 23 Jul 2021 00:25:17 GMT  
		Size: 1.9 KB (1894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8e79949ae6e203ea970da1b5dfcf5667ed2cc0aebe2352b67598d2783f33749`  
		Last Modified: Fri, 23 Jul 2021 00:25:17 GMT  
		Size: 25.9 MB (25853169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d23b10c241150db5f0fe5cde642895c56b94ff685777d5c13009e5366731f617`  
		Last Modified: Fri, 23 Jul 2021 00:25:14 GMT  
		Size: 864.6 KB (864595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fe8ae5a47eccc707e40c77b69770477b5d8459036f3bbc9ab25ea5c740f8ecc`  
		Last Modified: Fri, 23 Jul 2021 00:25:13 GMT  
		Size: 352.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a43fd2a24008e5302acee98f25a8b8479af11be28f50ceea55bdbef18587c816`  
		Last Modified: Tue, 10 Aug 2021 21:31:21 GMT  
		Size: 296.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fcfb2eddd6b7eee474971037c087a154febcbf605dba0cdd3ea8cb7c2e3399d`  
		Last Modified: Tue, 10 Aug 2021 21:31:57 GMT  
		Size: 243.2 MB (243189332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:4.1.1` - linux; s390x

```console
$ docker pull r-base@sha256:9531e79d85c52e35cd30050cdb5835ed7c61648eb7d992bd051ec8bc56895b88
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.9 MB (289918237 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7a2c2d3b945b5e882cb49c29c854badf43ab362c11acceeb76b098341427bf8`
-	Default Command: `["R"]`

```dockerfile
# Tue, 17 Aug 2021 01:52:42 GMT
ADD file:b26674f4981f5db4384da9469d05dea7bdf6bca5c09c954606849d005794f331 in / 
# Tue, 17 Aug 2021 01:52:50 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 09:55:39 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Tue, 17 Aug 2021 09:55:40 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Tue, 17 Aug 2021 09:55:53 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:55:56 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Tue, 17 Aug 2021 09:55:57 GMT
ENV LC_ALL=en_US.UTF-8
# Tue, 17 Aug 2021 09:55:57 GMT
ENV LANG=en_US.UTF-8
# Tue, 17 Aug 2021 09:55:58 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Tue, 17 Aug 2021 09:55:58 GMT
ENV R_BASE_VERSION=4.1.1
# Tue, 17 Aug 2021 09:55:59 GMT
RUN echo "deb http://deb.debian.org/debian experimental main" > /etc/apt/sources.list.d/experimental.list     && echo "deb [trusted=yes] https://eddelbuettel.github.io/ppaR400 ./" > /etc/apt/sources.list.d/edd-r4.list
# Tue, 17 Aug 2021 09:57:15 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:57:30 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:9cb7e265bbdb4667aca5ec3384874eca1b6494c42d2489f1d0221adfd706bf9b`  
		Last Modified: Tue, 17 Aug 2021 02:00:01 GMT  
		Size: 53.2 MB (53188554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:956e1f8ca2f48c8f49701b3e67f321ce8096e21303628ca69c38bdb960bb6130`  
		Last Modified: Tue, 17 Aug 2021 09:57:53 GMT  
		Size: 1.9 KB (1877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbd5cd8a59c1527cd6e56fe903fdadb4f9a825477ca3b3b4c5d50ce35361b4ab`  
		Last Modified: Tue, 17 Aug 2021 09:57:54 GMT  
		Size: 25.6 MB (25632976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d16c21f4626d3b63a3cee5413eb09bf1b185eec41e31afe34db30c04b0cb12c8`  
		Last Modified: Tue, 17 Aug 2021 09:57:52 GMT  
		Size: 920.2 KB (920157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc5bae5f780c5ac96baa803ccaeed1d34f41df12abf4591dad73db495a9a93fd`  
		Last Modified: Tue, 17 Aug 2021 09:57:51 GMT  
		Size: 347.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ca83f7ac03bd9d33909868795bca8d3ba713387d0344f7673951082674de207`  
		Last Modified: Tue, 17 Aug 2021 09:57:51 GMT  
		Size: 291.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42ab8131b422b49ca4cc8d6215393a725082b279534bd1bbbb3a20880290c4fd`  
		Last Modified: Tue, 17 Aug 2021 09:58:12 GMT  
		Size: 210.2 MB (210174035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `r-base:latest`

```console
$ docker pull r-base@sha256:3c0bda6cad11e1498daa62c13bd5c19ac9d322d1dbb460f7ecf26f25c2559ef6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `r-base:latest` - linux; amd64

```console
$ docker pull r-base@sha256:c7361b639c83d25cfa3d869dfb4608b9445e9da96b0b13a97c396e286b2fda63
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **330.2 MB (330235437 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e83ee6a20d40957a08ebe836619d888259b4897c9e0e800ad952f5633a8cdb92`
-	Default Command: `["R"]`

```dockerfile
# Thu, 22 Jul 2021 00:47:30 GMT
ADD file:aefd1b2aad4a1d98fd82d86cab1e66f8f172c748e69090a4938ded7681a5fcfe in / 
# Thu, 22 Jul 2021 00:47:30 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 14:25:02 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Thu, 22 Jul 2021 14:25:03 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Thu, 22 Jul 2021 14:25:13 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 14:25:15 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Thu, 22 Jul 2021 14:25:15 GMT
ENV LC_ALL=en_US.UTF-8
# Thu, 22 Jul 2021 14:25:16 GMT
ENV LANG=en_US.UTF-8
# Thu, 22 Jul 2021 14:25:16 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Tue, 10 Aug 2021 20:32:35 GMT
ENV R_BASE_VERSION=4.1.1
# Tue, 10 Aug 2021 20:32:36 GMT
RUN echo "deb http://deb.debian.org/debian experimental main" > /etc/apt/sources.list.d/experimental.list     && echo "deb [trusted=yes] https://eddelbuettel.github.io/ppaR400 ./" > /etc/apt/sources.list.d/edd-r4.list
# Tue, 10 Aug 2021 20:33:27 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Tue, 10 Aug 2021 20:33:29 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:7b303595d9b321a9020d0ddbf1dea4c83237e2367117606a8d5466c446714ba1`  
		Last Modified: Thu, 22 Jul 2021 00:53:44 GMT  
		Size: 54.9 MB (54904726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:269a52eb0491fa8f50f18f968e9a26e2c3f139332e157f2af3eaaa4ad8fbdab5`  
		Last Modified: Thu, 22 Jul 2021 14:26:23 GMT  
		Size: 1.9 KB (1878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ded859387bdafb915ae926a385218acb88202f871dab977fc1f53237dfb4a079`  
		Last Modified: Thu, 22 Jul 2021 14:26:23 GMT  
		Size: 25.6 MB (25629332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e9a9ca14ab54b7dcc64efd3dd1e59caa23457c62f787811a6dd14e73aeb8421`  
		Last Modified: Thu, 22 Jul 2021 14:26:21 GMT  
		Size: 864.6 KB (864588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2833e2a4a5cdc17504b1c82018201d1ab11fd9561b5f6b53a380150c056f80f`  
		Last Modified: Thu, 22 Jul 2021 14:26:20 GMT  
		Size: 349.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1a5465a8d4cda5658398f72d4f6457963e87134ab528e8b85290052426edebf`  
		Last Modified: Tue, 10 Aug 2021 20:33:42 GMT  
		Size: 297.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f80170cdc1529cd3405628fe4d2cf9551838ea19dd0878401a648fb547577f47`  
		Last Modified: Tue, 10 Aug 2021 20:34:10 GMT  
		Size: 248.8 MB (248834267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:latest` - linux; arm64 variant v8

```console
$ docker pull r-base@sha256:679cf53883c00279b771519f41ca013eab405531ad6165dde18d7dd28735e1cd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **311.2 MB (311213242 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67a98d91c624eb33fa56c2b57145a2388ab2b953ac42f2eb0d348e4e9b99733c`
-	Default Command: `["R"]`

```dockerfile
# Tue, 17 Aug 2021 01:48:44 GMT
ADD file:3893bd6ddc225c2b660af0396860193305baef444ab5aeb369ea28b0679c3a14 in / 
# Tue, 17 Aug 2021 01:48:44 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 11:46:00 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Tue, 17 Aug 2021 11:46:01 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Tue, 17 Aug 2021 11:46:09 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 11:46:12 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Tue, 17 Aug 2021 11:46:12 GMT
ENV LC_ALL=en_US.UTF-8
# Tue, 17 Aug 2021 11:46:13 GMT
ENV LANG=en_US.UTF-8
# Tue, 17 Aug 2021 11:46:13 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Tue, 17 Aug 2021 11:46:13 GMT
ENV R_BASE_VERSION=4.1.1
# Tue, 17 Aug 2021 11:46:14 GMT
RUN echo "deb http://deb.debian.org/debian experimental main" > /etc/apt/sources.list.d/experimental.list     && echo "deb [trusted=yes] https://eddelbuettel.github.io/ppaR400 ./" > /etc/apt/sources.list.d/edd-r4.list
# Tue, 17 Aug 2021 11:46:59 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 11:47:01 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:20341cea39b7b052e8fa46c85b6e6d17dbd3830a13c140eb6d72f4dd6ec5b8e6`  
		Last Modified: Tue, 17 Aug 2021 01:58:25 GMT  
		Size: 53.6 MB (53595238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d037b018b43733167395523bdbb299306664767079cc9a989ef5135870cf8c69`  
		Last Modified: Tue, 17 Aug 2021 11:47:24 GMT  
		Size: 1.9 KB (1878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bb43f2d04b40904a1a96073154eec86259d17631ae2830fdf99353dd152b7e4`  
		Last Modified: Tue, 17 Aug 2021 11:47:25 GMT  
		Size: 25.6 MB (25632791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55477b466c6bed3955a5b74780ade5336a26f29a1dcb64c25770af9c61e4c438`  
		Last Modified: Tue, 17 Aug 2021 11:47:22 GMT  
		Size: 864.6 KB (864593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b41b3fb56558348cd5487cadbfcc1a49eb66d6930e6a2796d4cd74be2b56c45`  
		Last Modified: Tue, 17 Aug 2021 11:47:22 GMT  
		Size: 349.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0da01b3ed82dc66c3ec450a010ee2a05457729da5a15797d6766a93bab5d0152`  
		Last Modified: Tue, 17 Aug 2021 11:47:22 GMT  
		Size: 294.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3071f1c57dd21ec88ee4baec1631678d84306d7a97fe0ee99200fdd75fdc87f1`  
		Last Modified: Tue, 17 Aug 2021 11:47:52 GMT  
		Size: 231.1 MB (231118099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:latest` - linux; ppc64le

```console
$ docker pull r-base@sha256:f9b2f99b1b4bd99c232eb973ac719384c9d9b37c1664f82587320397da366583
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **328.7 MB (328722936 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f0c2947da572eb28cfa944fab76b9f3595d79864885cc23a1fb4054d0966b4d`
-	Default Command: `["R"]`

```dockerfile
# Thu, 22 Jul 2021 00:21:17 GMT
ADD file:609f34b74745c6e0ad3453b3e7043b6aa9a8bd1f08450e5dacc435f2e02cfdc1 in / 
# Thu, 22 Jul 2021 00:21:28 GMT
CMD ["bash"]
# Fri, 23 Jul 2021 00:06:03 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Fri, 23 Jul 2021 00:06:45 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Fri, 23 Jul 2021 00:09:26 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Fri, 23 Jul 2021 00:09:52 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Fri, 23 Jul 2021 00:10:05 GMT
ENV LC_ALL=en_US.UTF-8
# Fri, 23 Jul 2021 00:10:14 GMT
ENV LANG=en_US.UTF-8
# Fri, 23 Jul 2021 00:10:38 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Tue, 10 Aug 2021 21:20:29 GMT
ENV R_BASE_VERSION=4.1.1
# Tue, 10 Aug 2021 21:20:43 GMT
RUN echo "deb http://deb.debian.org/debian experimental main" > /etc/apt/sources.list.d/experimental.list     && echo "deb [trusted=yes] https://eddelbuettel.github.io/ppaR400 ./" > /etc/apt/sources.list.d/edd-r4.list
# Tue, 10 Aug 2021 21:30:56 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Tue, 10 Aug 2021 21:31:02 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:a9effce78a0f7eaff718bcd66572e6000ce0a0c44f2947bbc1908696da72910b`  
		Last Modified: Thu, 22 Jul 2021 00:29:51 GMT  
		Size: 58.8 MB (58813298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00357bf8a668e7e05cde7ec787f1f104c8f855f63110ecc5dac594438e939bf7`  
		Last Modified: Fri, 23 Jul 2021 00:25:17 GMT  
		Size: 1.9 KB (1894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8e79949ae6e203ea970da1b5dfcf5667ed2cc0aebe2352b67598d2783f33749`  
		Last Modified: Fri, 23 Jul 2021 00:25:17 GMT  
		Size: 25.9 MB (25853169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d23b10c241150db5f0fe5cde642895c56b94ff685777d5c13009e5366731f617`  
		Last Modified: Fri, 23 Jul 2021 00:25:14 GMT  
		Size: 864.6 KB (864595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fe8ae5a47eccc707e40c77b69770477b5d8459036f3bbc9ab25ea5c740f8ecc`  
		Last Modified: Fri, 23 Jul 2021 00:25:13 GMT  
		Size: 352.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a43fd2a24008e5302acee98f25a8b8479af11be28f50ceea55bdbef18587c816`  
		Last Modified: Tue, 10 Aug 2021 21:31:21 GMT  
		Size: 296.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fcfb2eddd6b7eee474971037c087a154febcbf605dba0cdd3ea8cb7c2e3399d`  
		Last Modified: Tue, 10 Aug 2021 21:31:57 GMT  
		Size: 243.2 MB (243189332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:latest` - linux; s390x

```console
$ docker pull r-base@sha256:9531e79d85c52e35cd30050cdb5835ed7c61648eb7d992bd051ec8bc56895b88
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.9 MB (289918237 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7a2c2d3b945b5e882cb49c29c854badf43ab362c11acceeb76b098341427bf8`
-	Default Command: `["R"]`

```dockerfile
# Tue, 17 Aug 2021 01:52:42 GMT
ADD file:b26674f4981f5db4384da9469d05dea7bdf6bca5c09c954606849d005794f331 in / 
# Tue, 17 Aug 2021 01:52:50 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 09:55:39 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Tue, 17 Aug 2021 09:55:40 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Tue, 17 Aug 2021 09:55:53 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:55:56 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Tue, 17 Aug 2021 09:55:57 GMT
ENV LC_ALL=en_US.UTF-8
# Tue, 17 Aug 2021 09:55:57 GMT
ENV LANG=en_US.UTF-8
# Tue, 17 Aug 2021 09:55:58 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Tue, 17 Aug 2021 09:55:58 GMT
ENV R_BASE_VERSION=4.1.1
# Tue, 17 Aug 2021 09:55:59 GMT
RUN echo "deb http://deb.debian.org/debian experimental main" > /etc/apt/sources.list.d/experimental.list     && echo "deb [trusted=yes] https://eddelbuettel.github.io/ppaR400 ./" > /etc/apt/sources.list.d/edd-r4.list
# Tue, 17 Aug 2021 09:57:15 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:57:30 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:9cb7e265bbdb4667aca5ec3384874eca1b6494c42d2489f1d0221adfd706bf9b`  
		Last Modified: Tue, 17 Aug 2021 02:00:01 GMT  
		Size: 53.2 MB (53188554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:956e1f8ca2f48c8f49701b3e67f321ce8096e21303628ca69c38bdb960bb6130`  
		Last Modified: Tue, 17 Aug 2021 09:57:53 GMT  
		Size: 1.9 KB (1877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbd5cd8a59c1527cd6e56fe903fdadb4f9a825477ca3b3b4c5d50ce35361b4ab`  
		Last Modified: Tue, 17 Aug 2021 09:57:54 GMT  
		Size: 25.6 MB (25632976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d16c21f4626d3b63a3cee5413eb09bf1b185eec41e31afe34db30c04b0cb12c8`  
		Last Modified: Tue, 17 Aug 2021 09:57:52 GMT  
		Size: 920.2 KB (920157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc5bae5f780c5ac96baa803ccaeed1d34f41df12abf4591dad73db495a9a93fd`  
		Last Modified: Tue, 17 Aug 2021 09:57:51 GMT  
		Size: 347.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ca83f7ac03bd9d33909868795bca8d3ba713387d0344f7673951082674de207`  
		Last Modified: Tue, 17 Aug 2021 09:57:51 GMT  
		Size: 291.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42ab8131b422b49ca4cc8d6215393a725082b279534bd1bbbb3a20880290c4fd`  
		Last Modified: Tue, 17 Aug 2021 09:58:12 GMT  
		Size: 210.2 MB (210174035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
