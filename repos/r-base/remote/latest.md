## `r-base:latest`

```console
$ docker pull r-base@sha256:ea5e7539ff0cc747365977d166b8533556f91f5028fcfc615ee1a0217f58652f
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
$ docker pull r-base@sha256:9fd04ddef4edbadad9019c09ca64a6df4b8a29779f906ee4512bdf9e3fe98ea0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **304.4 MB (304436975 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:add2935d9a645d9e001a4a1edb22c621ee41d9472ae72440f774b576776e924c`
-	Default Command: `["R"]`

```dockerfile
# Wed, 09 Sep 2020 23:55:28 GMT
ADD file:5dde8e807b0c71ebc7645a34be11d591e22056828b80451cd10b4e9e43d50f22 in / 
# Wed, 09 Sep 2020 23:55:29 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 17:42:24 GMT
LABEL org.label-schema.license=GPL-2.0 org.label-schema.vcs-url=https://github.com/rocker-org/r-base org.label-schema.vendor=Rocker Project maintainer=Dirk Eddelbuettel <edd@debian.org>
# Thu, 10 Sep 2020 17:42:29 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Mon, 12 Oct 2020 23:46:05 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Mon, 12 Oct 2020 23:46:10 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Mon, 12 Oct 2020 23:46:10 GMT
ENV LC_ALL=en_US.UTF-8
# Mon, 12 Oct 2020 23:46:11 GMT
ENV LANG=en_US.UTF-8
# Mon, 12 Oct 2020 23:46:13 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Mon, 12 Oct 2020 23:46:13 GMT
ENV R_BASE_VERSION=4.0.3
# Mon, 12 Oct 2020 23:47:55 GMT
RUN apt-get update         && apt-get install -t unstable -y --no-install-recommends                 gcc-9-base                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Mon, 12 Oct 2020 23:48:00 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:c3a3b210b20418d18407956d6d337463c452a063f31e10abcc972012479278c3`  
		Last Modified: Thu, 10 Sep 2020 00:02:26 GMT  
		Size: 50.8 MB (50825396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:968fc21bcc0fd6889bb8e690e3bfa3a5c6b4cee6dcf8646f7f89746c2faedefe`  
		Last Modified: Thu, 10 Sep 2020 17:45:01 GMT  
		Size: 1.9 KB (1879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f699fd286148e4b747ded2fb81c3f07ff122b7e7604eb2c8ed5aa8c7845c36e`  
		Last Modified: Mon, 12 Oct 2020 23:48:17 GMT  
		Size: 27.2 MB (27247663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb2cb93ef5009363aac8c57050fba00541855894c93fac940925ead1bf9dd9b1`  
		Last Modified: Mon, 12 Oct 2020 23:48:12 GMT  
		Size: 863.6 KB (863576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a28912b660cb9b336e9d9df35db905be756099817e2cf8355d1db9a4c93b631`  
		Last Modified: Mon, 12 Oct 2020 23:48:11 GMT  
		Size: 353.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a59fd1683f80330f2aaeab36c5b015cef5e866cf06774a5a6b34e4aff666aba`  
		Last Modified: Mon, 12 Oct 2020 23:52:10 GMT  
		Size: 225.5 MB (225498108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:latest` - linux; ppc64le

```console
$ docker pull r-base@sha256:b93fd19e8fc8ca405974b6cb3597a9e5769d5b98fa9b0f1c4fae6aa3a96b52b0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **323.6 MB (323640451 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc5f7828e3f1f62e3669a44edc1d6fd63675834df231d50ea8446510f5e203df`
-	Default Command: `["R"]`

```dockerfile
# Thu, 10 Sep 2020 01:14:15 GMT
ADD file:1ff1c751892adb35acbc76e9c216d58059214a72e719e3789fb186911933fe1b in / 
# Thu, 10 Sep 2020 01:14:26 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 11:05:02 GMT
LABEL org.label-schema.license=GPL-2.0 org.label-schema.vcs-url=https://github.com/rocker-org/r-base org.label-schema.vendor=Rocker Project maintainer=Dirk Eddelbuettel <edd@debian.org>
# Thu, 10 Sep 2020 11:05:35 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Mon, 12 Oct 2020 23:23:50 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Mon, 12 Oct 2020 23:24:03 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Mon, 12 Oct 2020 23:24:09 GMT
ENV LC_ALL=en_US.UTF-8
# Mon, 12 Oct 2020 23:24:13 GMT
ENV LANG=en_US.UTF-8
# Mon, 12 Oct 2020 23:24:22 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Mon, 12 Oct 2020 23:24:27 GMT
ENV R_BASE_VERSION=4.0.3
# Mon, 12 Oct 2020 23:32:21 GMT
RUN apt-get update         && apt-get install -t unstable -y --no-install-recommends                 gcc-9-base                 libopenblas0-pthread 		littler                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& install.r docopt 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Mon, 12 Oct 2020 23:32:28 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:4f06950a568456590fe3afbc7dc70475d0e9ea33f4901b4085b036db8288648c`  
		Last Modified: Thu, 10 Sep 2020 01:37:32 GMT  
		Size: 55.8 MB (55774415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4dba42cbd72ea76ebdfdf4d25b40ba35c5f5de1a292409364ed5f2c264cf377`  
		Last Modified: Thu, 10 Sep 2020 11:21:30 GMT  
		Size: 1.9 KB (1893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79808a81d992d709ac006d3265f14e3d928cb3dc4e4ee4d2e51bcc22a7f8f6c5`  
		Last Modified: Mon, 12 Oct 2020 23:32:54 GMT  
		Size: 27.7 MB (27656738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3d5c0b593ab0cd2b345695fdc15cb2714eddb6883f253daafacfb0f465465cb`  
		Last Modified: Mon, 12 Oct 2020 23:32:48 GMT  
		Size: 863.6 KB (863575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a315d7981f3c43e62cc7a708fd1d5db8225fd3a21083008998edbdefeeac133`  
		Last Modified: Mon, 12 Oct 2020 23:32:48 GMT  
		Size: 353.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:640d330a56085e86f871242f5746d1277e2f1c2112304d55856cb377e8ae3a1a`  
		Last Modified: Mon, 12 Oct 2020 23:33:30 GMT  
		Size: 239.3 MB (239343477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
