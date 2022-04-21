## `r-base:latest`

```console
$ docker pull r-base@sha256:ae07a4e0092793330c23857922792250b898c4aad11f7dc3390c43f24576c58a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `r-base:latest` - linux; amd64

```console
$ docker pull r-base@sha256:567cb8968827c97e1fb788e23e9a3acf8a5d95c6dbeeb88a48ae438e05fe2da0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **333.8 MB (333807683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f987362a590dd6659467713d5f78324a8965c8c2a6abc464f5613da3e969aa96`
-	Default Command: `["R"]`

```dockerfile
# Wed, 20 Apr 2022 04:45:35 GMT
ADD file:fb66d619557384a14385fa7b5371be954594c4aff1700edcbd9cff422c3498f0 in / 
# Wed, 20 Apr 2022 04:45:35 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 13:25:30 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Wed, 20 Apr 2022 13:25:31 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Wed, 20 Apr 2022 13:25:41 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 13:25:43 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Wed, 20 Apr 2022 13:25:43 GMT
ENV LC_ALL=en_US.UTF-8
# Wed, 20 Apr 2022 13:25:43 GMT
ENV LANG=en_US.UTF-8
# Wed, 20 Apr 2022 13:25:44 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Wed, 20 Apr 2022 13:25:44 GMT
ENV R_BASE_VERSION=4.1.3
# Wed, 20 Apr 2022 13:26:52 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-docopt                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 13:26:54 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:536039adbcd59ca1bf50e1393d4c116319d1f29168898c56d21c192d219c4832`  
		Last Modified: Wed, 20 Apr 2022 04:52:49 GMT  
		Size: 55.6 MB (55578869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b1da36bf8d2a06d8166a24f3477fb5137ed10b2e31479a8c502fb0011af0bc9`  
		Last Modified: Wed, 20 Apr 2022 13:27:14 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4afe378696fd472844089373e7b153a0f0a0d8293e12fa57f18cb850e2c4fe37`  
		Last Modified: Wed, 20 Apr 2022 13:27:17 GMT  
		Size: 25.9 MB (25851696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61b0b85413db82c6a0f17b355291dfd6bc4c1e251d67aa85b15a568f579c0655`  
		Last Modified: Wed, 20 Apr 2022 13:27:14 GMT  
		Size: 864.6 KB (864607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bf4cc3b4afb9b51cb673c32c8d3101da067c78e42701b7b84de52cf52c4f3a0`  
		Last Modified: Wed, 20 Apr 2022 13:27:14 GMT  
		Size: 348.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11f32de4c0e37f0cceca24bc8e6d29ee2ec0eb02a91f6f329586fbd342d22da6`  
		Last Modified: Wed, 20 Apr 2022 13:27:43 GMT  
		Size: 251.5 MB (251510282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:latest` - linux; arm64 variant v8

```console
$ docker pull r-base@sha256:6511b580c48b285bef5082c7f17ac57edb7af926f5168985056952c08c4bd401
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **322.9 MB (322935119 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:587012b8220aa1be4c1ab670688e3ce7f4edd639863764982dbdf4aae0e72226`
-	Default Command: `["R"]`

```dockerfile
# Wed, 20 Apr 2022 04:31:45 GMT
ADD file:273f985806cb79b6f6b619ba5b9db50ba151174fde33bffc81c25187b0999170 in / 
# Wed, 20 Apr 2022 04:31:45 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 11:59:40 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Wed, 20 Apr 2022 11:59:41 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Wed, 20 Apr 2022 11:59:50 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 11:59:52 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Wed, 20 Apr 2022 11:59:53 GMT
ENV LC_ALL=en_US.UTF-8
# Wed, 20 Apr 2022 11:59:54 GMT
ENV LANG=en_US.UTF-8
# Wed, 20 Apr 2022 11:59:55 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Wed, 20 Apr 2022 11:59:56 GMT
ENV R_BASE_VERSION=4.1.3
# Wed, 20 Apr 2022 12:00:45 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-docopt                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 12:00:46 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:3124af2dc12fec2edfce6b676869cb7dbcea85f39bf473efd3b5674765b68351`  
		Last Modified: Wed, 20 Apr 2022 04:40:29 GMT  
		Size: 54.5 MB (54493338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86e730a7adab655457f2a985872a4b9bc5d0af23359a084ba069c602452f97f1`  
		Last Modified: Wed, 20 Apr 2022 12:00:59 GMT  
		Size: 1.8 KB (1823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f40c6eb1bebd6d176cdb1c752acf4612cdf94053b91410b654ca3a643443154`  
		Last Modified: Wed, 20 Apr 2022 12:01:02 GMT  
		Size: 25.8 MB (25841038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23547edafe1d3dec48a3eb14cac16816223e38e500ec3b14a1d4f9e7719b1d4e`  
		Last Modified: Wed, 20 Apr 2022 12:01:00 GMT  
		Size: 864.6 KB (864610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:232373586c238520cd70bb4f78a1cf585963b867f6d80f3ad76ef18d9256dadb`  
		Last Modified: Wed, 20 Apr 2022 12:00:59 GMT  
		Size: 348.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdff729dc60f243bf9bb3df1a95e763076dc3e078bae4c2c1968117716bcc946`  
		Last Modified: Wed, 20 Apr 2022 12:01:27 GMT  
		Size: 241.7 MB (241733962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:latest` - linux; ppc64le

```console
$ docker pull r-base@sha256:3a391c5c5465c4c011eb6df90fa7a72fb801fc4928aee5108ff8907a69c6f146
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **332.6 MB (332620120 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a74eb9e820a949adbdf2bd80ca4a3d4e2c4bc8f75cfd61f99441e826903813c5`
-	Default Command: `["R"]`

```dockerfile
# Wed, 20 Apr 2022 09:51:07 GMT
ADD file:0441cbd5b80c3154a95cf5f152472d9f238a42a1d874898b18c876944e830675 in / 
# Wed, 20 Apr 2022 09:51:19 GMT
CMD ["bash"]
# Thu, 21 Apr 2022 04:02:06 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Thu, 21 Apr 2022 04:02:20 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Thu, 21 Apr 2022 04:03:05 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Thu, 21 Apr 2022 04:03:15 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Thu, 21 Apr 2022 04:03:18 GMT
ENV LC_ALL=en_US.UTF-8
# Thu, 21 Apr 2022 04:03:20 GMT
ENV LANG=en_US.UTF-8
# Thu, 21 Apr 2022 04:03:26 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Thu, 21 Apr 2022 04:03:28 GMT
ENV R_BASE_VERSION=4.1.3
# Thu, 21 Apr 2022 04:09:06 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-docopt                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Thu, 21 Apr 2022 04:09:09 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:6a660090735cb86ef009831259b3363aa899b4b1f765ffad3047dd93f2146807`  
		Last Modified: Wed, 20 Apr 2022 10:01:09 GMT  
		Size: 60.0 MB (59982556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19c9dc198aaad9e3f0283974fe76f6cc66736e51428532246129be73569e59f0`  
		Last Modified: Thu, 21 Apr 2022 04:09:37 GMT  
		Size: 1.9 KB (1893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2323301907f7fc97eca9b564588154984a274701b2e4129357c99a10d1abd04`  
		Last Modified: Thu, 21 Apr 2022 04:09:41 GMT  
		Size: 26.1 MB (26079746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a539f4d83414d06c5ccb60e61f74bf0366bb2c762d7a26b72b7ad83b7754f32f`  
		Last Modified: Thu, 21 Apr 2022 04:09:37 GMT  
		Size: 864.6 KB (864604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cba10dc04e6060fe4fb45889e20b51d7d9dc4189f086075dbef9a6df080334e9`  
		Last Modified: Thu, 21 Apr 2022 04:09:37 GMT  
		Size: 351.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8fcc168060407ed4268a03dc4d2e8e190e1c165d9525f3fe79dbfef4bf992dd`  
		Last Modified: Thu, 21 Apr 2022 04:10:14 GMT  
		Size: 245.7 MB (245690970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `r-base:latest` - linux; s390x

```console
$ docker pull r-base@sha256:3d11494acba1c9d2383b94a81e2448f6df0144a1e82d2f836b6a566c5755a336
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **298.4 MB (298352704 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af80ce35cb4eec5fafec3f7f46e1b4e2743dbe65977d67d02b7b0dcfbfa6c250`
-	Default Command: `["R"]`

```dockerfile
# Wed, 20 Apr 2022 08:44:07 GMT
ADD file:23684e7af9a096cf83a114c361e7879ed97ef5fbf7cb9607e40ffaf19dd0bed7 in / 
# Wed, 20 Apr 2022 08:44:14 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 16:03:35 GMT
LABEL org.opencontainers.image.licenses=GPL-2.0-or-later org.opencontainers.image.source=https://github.com/rocker-org/rocker org.opencontainers.image.vendor=Rocker Project org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>
# Wed, 20 Apr 2022 16:03:37 GMT
RUN useradd docker 	&& mkdir /home/docker 	&& chown docker:docker /home/docker 	&& addgroup docker staff
# Wed, 20 Apr 2022 16:04:04 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ed 		less 		locales 		vim-tiny 		wget 		ca-certificates 		fonts-texgyre 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 16:04:10 GMT
RUN echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen 	&& locale-gen en_US.utf8 	&& /usr/sbin/update-locale LANG=en_US.UTF-8
# Wed, 20 Apr 2022 16:04:11 GMT
ENV LC_ALL=en_US.UTF-8
# Wed, 20 Apr 2022 16:04:12 GMT
ENV LANG=en_US.UTF-8
# Wed, 20 Apr 2022 16:04:14 GMT
RUN echo "deb http://http.debian.net/debian sid main" > /etc/apt/sources.list.d/debian-unstable.list         && echo 'APT::Default-Release "testing";' > /etc/apt/apt.conf.d/default         && echo 'APT::Install-Recommends "false";' > /etc/apt/apt.conf.d/90local-no-recommends
# Wed, 20 Apr 2022 16:04:15 GMT
ENV R_BASE_VERSION=4.1.3
# Wed, 20 Apr 2022 16:06:16 GMT
RUN apt-get update         && apt-get install -y --no-install-recommends                 libopenblas0-pthread 		littler                 r-cran-docopt                 r-cran-littler 		r-base=${R_BASE_VERSION}-* 		r-base-dev=${R_BASE_VERSION}-*                 r-base-core=${R_BASE_VERSION}-* 		r-recommended=${R_BASE_VERSION}-* 	&& ln -s /usr/lib/R/site-library/littler/examples/install.r /usr/local/bin/install.r 	&& ln -s /usr/lib/R/site-library/littler/examples/install2.r /usr/local/bin/install2.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installBioc.r /usr/local/bin/installBioc.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installDeps.r /usr/local/bin/installDeps.r 	&& ln -s /usr/lib/R/site-library/littler/examples/installGithub.r /usr/local/bin/installGithub.r 	&& ln -s /usr/lib/R/site-library/littler/examples/testInstalled.r /usr/local/bin/testInstalled.r 	&& rm -rf /tmp/downloaded_packages/ /tmp/*.rds 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 16:06:38 GMT
CMD ["R"]
```

-	Layers:
	-	`sha256:362ce0a85fc3f682e0adac2df3a00133068c959c8dbf9d7872eb24b1b68f55a3`  
		Last Modified: Wed, 20 Apr 2022 08:52:12 GMT  
		Size: 53.8 MB (53813515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2d4c28aba12d4bb2ceb61042334706fd64afbf057777f6a85df8415801c4cb0`  
		Last Modified: Wed, 20 Apr 2022 16:07:38 GMT  
		Size: 1.9 KB (1884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf874736dd9bc2cbadd95f849168168927b6a65a00d071db95f2557f21e0e5a2`  
		Last Modified: Wed, 20 Apr 2022 16:07:35 GMT  
		Size: 25.9 MB (25864057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baab6b33b8fb34f72a25d67297e7488a42a69874c74b647c63094365dbdcae3c`  
		Last Modified: Wed, 20 Apr 2022 16:07:28 GMT  
		Size: 920.2 KB (920190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d02a7efd41932b75e4ec636c8073ddfdb99f915f7ff69c8ed0f0448e5eb9de5a`  
		Last Modified: Wed, 20 Apr 2022 16:07:38 GMT  
		Size: 351.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b9628e0d42c0dfdf290d06299b8174cf8368a670a2bbc8e8afc9ad6941a6812`  
		Last Modified: Wed, 20 Apr 2022 16:07:54 GMT  
		Size: 217.8 MB (217752707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
