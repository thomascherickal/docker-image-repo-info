## `r-base:latest`

```console
$ docker pull r-base@sha256:b8b0b5e210f8c455f62ccf9731d04695f26c6085227b88053ef93f4b9f97206b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `r-base:latest` - linux; amd64

```console
$ docker pull r-base@sha256:48d80d3ceaa21534ebd5627973ab69bec3b7db00233c1f4b54d8f9d9b3f931a9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **319.2 MB (319221746 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f6f1f4182a9d5965e336dc8686611764a3e2385c9a38aa691f158569d889778f`
-	Default Command: `["R"]`

```dockerfile
# Thu, 10 Sep 2020 00:30:59 GMT
ADD file:9b259b9d58cb55d3126a7ca20eeb5e20e8b26291fc1b738051ff61c8ec22bd95 in / 
# Thu, 10 Sep 2020 00:30:59 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 19:19:45 GMT
LABEL org.label-schema.license=GPL-2.0 org.label-schema.vcs-url=https://github.com/rocker-org/r-base org.label-schema.vendor=Rocker Project maintainer=Dirk Eddelbuettel <edd@debian.org>
# Thu, 10 Sep 2020 19:19:46 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Mon, 12 Oct 2020 22:46:00 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Mon, 12 Oct 2020 22:46:04 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Mon, 12 Oct 2020 22:46:05 GMT
ENV LC_ALL=en_US.UTF-8
# Mon, 12 Oct 2020 22:46:05 GMT
ENV LANG=en_US.UTF-8
# Mon, 12 Oct 2020 22:46:07 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Mon, 12 Oct 2020 22:46:07 GMT
ENV R_BASE_VERSION=4.0.3
# Mon, 12 Oct 2020 22:47:08 GMT
RUN apt-get update         && apt-get install -t unstable -y --no-install-recommends                 gcc-9-base                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Mon, 12 Oct 2020 22:47:09 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:4363cc52203477cd66948034ae4a1db71cbfd27fddb648dd9c590161de1f8634`  
		Last Modified: Thu, 10 Sep 2020 00:37:58 GMT  
		Size: 51.9 MB (51906560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa432a30f21d0c64a0d61cf4c70613a6688d7cce4e504320ae34acca4446d784`  
		Last Modified: Thu, 10 Sep 2020 19:21:06 GMT  
		Size: 1.8 KB (1845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c31dbcd6147f1ba05b8b33fb49d5056b86618f208bbc9163053ec2b5ccaa364a`  
		Last Modified: Mon, 12 Oct 2020 22:47:23 GMT  
		Size: 27.4 MB (27387847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61013b006f9e7d97b18548893e5946a8dfaad3186037b1c651b04325c63b5615`  
		Last Modified: Mon, 12 Oct 2020 22:47:17 GMT  
		Size: 863.6 KB (863572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bc19cf046eeddc46ad7ee8e4b40daaf91bf5fe9cb9afc9108b831f690410efc`  
		Last Modified: Mon, 12 Oct 2020 22:47:16 GMT  
		Size: 351.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eecce924be9023b2392d6f6503d04fd57eb66f78dfb275111f4d9f853a3b73fa`  
		Last Modified: Mon, 12 Oct 2020 22:50:32 GMT  
		Size: 239.1 MB (239061571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:latest` - linux; arm64 variant v8

```console
$ docker pull r-base@sha256:649a78dc814c69ac06a765e6cd0780348c3b39167732c4b1d43a8f8dc6dc61a8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **304.5 MB (304528266 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b9235c79ad1aa20abbddd2a7edde4392019e1b25bcdec4f7989737ed80f2bc0e`
-	Default Command: `["R"]`

```dockerfile
# Tue, 13 Oct 2020 01:44:43 GMT
ADD file:e1dc4f74cca26ba51ab2b0514641801b22d0f0a2eb7e8f2b4c54cc36a75494d4 in / 
# Tue, 13 Oct 2020 01:44:45 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 12:39:12 GMT
LABEL org.label-schema.license=GPL-2.0 org.label-schema.vcs-url=https://github.com/rocker-org/r-base org.label-schema.vendor=Rocker Project maintainer=Dirk Eddelbuettel <edd@debian.org>
# Tue, 13 Oct 2020 12:39:16 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Tue, 13 Oct 2020 12:39:38 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 12:39:44 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Tue, 13 Oct 2020 12:39:46 GMT
ENV LC_ALL=en_US.UTF-8
# Tue, 13 Oct 2020 12:39:47 GMT
ENV LANG=en_US.UTF-8
# Tue, 13 Oct 2020 12:39:49 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Tue, 13 Oct 2020 12:39:50 GMT
ENV R_BASE_VERSION=4.0.3
# Tue, 13 Oct 2020 12:43:16 GMT
RUN apt-get update         && apt-get install -t unstable -y --no-install-recommends                 gcc-9-base                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 12:43:27 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:c2b4ce940f2a9cdf9744b56e1bc9d370237dff1f0040d6944415cf7d5f7fb20d`  
		Last Modified: Tue, 13 Oct 2020 01:51:35 GMT  
		Size: 51.5 MB (51484285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf86b2de526df6e6d4eac882282bea3aa79a233fec1ac1e4c47643cc973b0fcc`  
		Last Modified: Tue, 13 Oct 2020 12:43:38 GMT  
		Size: 1.9 KB (1890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ed44676ad141326e62e308c5432c7ee145118db1dfdd927ac391e751e97fd76`  
		Last Modified: Tue, 13 Oct 2020 12:43:52 GMT  
		Size: 27.2 MB (27247204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ef3cacc186009187da6639f41122558383755faf1f82c5cb5247ba1910b1a51`  
		Last Modified: Tue, 13 Oct 2020 12:43:40 GMT  
		Size: 863.6 KB (863571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b44e50d52feafbd6628b02412fa4c8d766b5326e8d7f52c5c7b0e01fa179939`  
		Last Modified: Tue, 13 Oct 2020 12:43:37 GMT  
		Size: 352.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45e82596eb3a0725273dcf7b113f74d411c4f9187c6b6367d2a9624419e9927d`  
		Last Modified: Tue, 13 Oct 2020 12:44:31 GMT  
		Size: 224.9 MB (224930964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:latest` - linux; ppc64le

```console
$ docker pull r-base@sha256:088cf66f43ca2179417a068f68d20c90db417435fb076ffddfe9b98349eeea2b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **323.7 MB (323743759 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93762728762565afa398f835ed44897adec2fc2e7f83d1f6a511042115a08338`
-	Default Command: `["R"]`

```dockerfile
# Tue, 13 Oct 2020 01:41:36 GMT
ADD file:391f7beabdff070d3417ca142cf9cd5a48f50f2d865401f3fc0cafa2cd0ee9b2 in / 
# Tue, 13 Oct 2020 01:41:43 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 10:48:34 GMT
LABEL org.label-schema.license=GPL-2.0 org.label-schema.vcs-url=https://github.com/rocker-org/r-base org.label-schema.vendor=Rocker Project maintainer=Dirk Eddelbuettel <edd@debian.org>
# Tue, 13 Oct 2020 10:48:46 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Tue, 13 Oct 2020 10:50:07 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 10:50:20 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Tue, 13 Oct 2020 10:50:24 GMT
ENV LC_ALL=en_US.UTF-8
# Tue, 13 Oct 2020 10:50:28 GMT
ENV LANG=en_US.UTF-8
# Tue, 13 Oct 2020 10:50:38 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Tue, 13 Oct 2020 10:50:44 GMT
ENV R_BASE_VERSION=4.0.3
# Tue, 13 Oct 2020 10:59:44 GMT
RUN apt-get update         && apt-get install -t unstable -y --no-install-recommends                 gcc-9-base                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 10:59:49 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:a3755d6e5159d63f7070ee41c1dc98d6ba8aa63edf93e38cb36d2dff626b94b5`  
		Last Modified: Tue, 13 Oct 2020 01:55:40 GMT  
		Size: 56.5 MB (56486400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd9fc806aed0ef0f4cfa4d1f651fa01e83eafc8f13bbeb27e13cfed9292b7b3b`  
		Last Modified: Tue, 13 Oct 2020 11:00:12 GMT  
		Size: 1.9 KB (1889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d13573a1c0eae892118908b1dd9484ca1800601b4abe5372c03688e13bb45a90`  
		Last Modified: Tue, 13 Oct 2020 11:00:38 GMT  
		Size: 27.7 MB (27656553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a2f8572d20e91fc8d74a21d0863bc4acc12428e7525e2111c5b94acbb9a1234`  
		Last Modified: Tue, 13 Oct 2020 11:00:12 GMT  
		Size: 863.6 KB (863574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63f76b2dfa3fbf7c46ba3543d9455612626d9c867b4cedc568413bb5e8182f7f`  
		Last Modified: Tue, 13 Oct 2020 11:00:11 GMT  
		Size: 352.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd0dd19e6f6db5a737248162450f9a9b300fe308c08d643acccba00f680e12a6`  
		Last Modified: Tue, 13 Oct 2020 11:01:25 GMT  
		Size: 238.7 MB (238734991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
