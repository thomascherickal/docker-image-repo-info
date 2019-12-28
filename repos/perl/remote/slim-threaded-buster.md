## `perl:slim-threaded-buster`

```console
$ docker pull perl@sha256:5fb02f47d6ec6b25ea7e4413577fd9a1ab26b0f4662fbdf34ddf825eed1ced02
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `perl:slim-threaded-buster` - linux; amd64

```console
$ docker pull perl@sha256:6bf7632936a19938e98005b7a19ac2f126e07a3a69e00c491bf824142b47e204
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.5 MB (41481439 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40dc4ebd91105225dbb82dd097fdf836f948be07a846dfb9eaf9ccd17b40f3d8`
-	Default Command: `["perl5.30.1","-de0"]`

```dockerfile
# Fri, 22 Nov 2019 14:55:09 GMT
ADD file:bc8179c87c8dbb3d962bed1801f99e7c860ff03797cde6ad19b107d43b973ada in / 
# Fri, 22 Nov 2019 14:55:10 GMT
CMD ["bash"]
# Sat, 23 Nov 2019 08:39:17 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Sat, 23 Nov 2019 08:39:17 GMT
COPY file:15650064fd29deac721f0aa084ddb3d41db77b78e2907775e257bd67e116ade4 in /usr/src/perl/ 
# Sat, 23 Nov 2019 08:39:17 GMT
WORKDIR /usr/src/perl
# Sat, 23 Nov 2019 09:37:58 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        xz-utils     && curl -SL https://www.cpan.org/src/5.0/perl-5.30.1.tar.xz -o perl-5.30.1.tar.xz     && echo '7336cd3ed0535eb61b76a71350effcfa7c88b44faf37d64d70952ced5d38cd35 *perl-5.30.1.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.30.1.tar.xz -C /usr/src/perl     && rm perl-5.30.1.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && savedPackages="make netbase"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Tue, 26 Nov 2019 01:22:27 GMT
WORKDIR /
# Tue, 26 Nov 2019 01:22:28 GMT
CMD ["perl5.30.1" "-de0"]
```

-	Layers:
	-	`sha256:000eee12ec04cc914bf96e8f5dee7767510c2aca3816af6078bd9fbe3150920c`  
		Last Modified: Fri, 22 Nov 2019 15:02:49 GMT  
		Size: 27.1 MB (27092654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8211917f08d3ba0b9ad6372157b57525f65addee699952f5260f2967463fe98b`  
		Last Modified: Sat, 23 Nov 2019 12:39:25 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ea642c157eb254d08e4ee74d8279fdcd16a181e44d78c9758cdeadd0e578780`  
		Last Modified: Sat, 23 Nov 2019 12:40:28 GMT  
		Size: 14.4 MB (14388372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:slim-threaded-buster` - linux; arm variant v7

```console
$ docker pull perl@sha256:9237fee3406f915d8a50031456470f800066f5a98b0aa9ab7430738b8a816700
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.2 MB (36188726 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bdbf5f5f812bcb27cd8b48d504cbc766e2eea02866c8f9a1e4612327fcf19218`
-	Default Command: `["perl5.30.1","-de0"]`

```dockerfile
# Fri, 22 Nov 2019 13:22:45 GMT
ADD file:85cf6081b7d1948b250d1b3749a65e2561cddafb7cd748db6b7b7420a376a48f in / 
# Fri, 22 Nov 2019 13:22:46 GMT
CMD ["bash"]
# Fri, 22 Nov 2019 20:57:25 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Fri, 22 Nov 2019 20:57:25 GMT
COPY file:15650064fd29deac721f0aa084ddb3d41db77b78e2907775e257bd67e116ade4 in /usr/src/perl/ 
# Fri, 22 Nov 2019 20:57:26 GMT
WORKDIR /usr/src/perl
# Fri, 22 Nov 2019 21:28:42 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        xz-utils     && curl -SL https://www.cpan.org/src/5.0/perl-5.30.1.tar.xz -o perl-5.30.1.tar.xz     && echo '7336cd3ed0535eb61b76a71350effcfa7c88b44faf37d64d70952ced5d38cd35 *perl-5.30.1.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.30.1.tar.xz -C /usr/src/perl     && rm perl-5.30.1.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && savedPackages="make netbase"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Tue, 26 Nov 2019 01:15:35 GMT
WORKDIR /
# Tue, 26 Nov 2019 01:15:35 GMT
CMD ["perl5.30.1" "-de0"]
```

-	Layers:
	-	`sha256:3cf3d03fb414460b7542c20e72fe29a83f08d22fd2c7a8cab1834eec2976e4b2`  
		Last Modified: Fri, 22 Nov 2019 13:33:25 GMT  
		Size: 22.7 MB (22699053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2af07f91d532bda14eeab3986dd844a8204b25b8bbee322fc0845466ebdb037`  
		Last Modified: Fri, 22 Nov 2019 22:57:32 GMT  
		Size: 440.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92e7f55edf1a1af90ec34afa8371a4be4c3f6ae6fd2db3a85f25a1725a4a046`  
		Last Modified: Fri, 22 Nov 2019 22:58:17 GMT  
		Size: 13.5 MB (13489233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:slim-threaded-buster` - linux; arm64 variant v8

```console
$ docker pull perl@sha256:f360cf64b99cc3e3723e0a75dd2af4c72042bcbdba75f56dd53822b7e6d3b9fd
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.2 MB (40177198 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bce1fb03b03751535b5e85b617b5969a04fbfb6bd2edf2f239e104f5b7231232`
-	Default Command: `["perl5.30.1","-de0"]`

```dockerfile
# Fri, 22 Nov 2019 13:41:59 GMT
ADD file:69e0891ef62c74ec5e9bae38f8d2770ab2f0d7ea0d3cf1dc85875763be0b10b7 in / 
# Fri, 22 Nov 2019 13:42:02 GMT
CMD ["bash"]
# Fri, 22 Nov 2019 23:52:48 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Fri, 22 Nov 2019 23:52:48 GMT
COPY file:15650064fd29deac721f0aa084ddb3d41db77b78e2907775e257bd67e116ade4 in /usr/src/perl/ 
# Fri, 22 Nov 2019 23:52:49 GMT
WORKDIR /usr/src/perl
# Sat, 23 Nov 2019 00:46:19 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        xz-utils     && curl -SL https://www.cpan.org/src/5.0/perl-5.30.1.tar.xz -o perl-5.30.1.tar.xz     && echo '7336cd3ed0535eb61b76a71350effcfa7c88b44faf37d64d70952ced5d38cd35 *perl-5.30.1.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.30.1.tar.xz -C /usr/src/perl     && rm perl-5.30.1.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && savedPackages="make netbase"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Tue, 26 Nov 2019 01:05:36 GMT
WORKDIR /
# Tue, 26 Nov 2019 01:05:40 GMT
CMD ["perl5.30.1" "-de0"]
```

-	Layers:
	-	`sha256:a4f3dd4087f9309af4187e5dda90741441f057da59c2270598e16aa8019b0ca2`  
		Last Modified: Fri, 22 Nov 2019 13:49:50 GMT  
		Size: 25.9 MB (25850802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3df3ab8821bd067b66e32d25e541901446cde450215525b1e8425d1e18cfa7d1`  
		Last Modified: Sat, 23 Nov 2019 04:08:47 GMT  
		Size: 444.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8156f72d8a4fc1dd45390c4aad952f87f141abeeecdcd12cafe38a50c55456a2`  
		Last Modified: Sat, 23 Nov 2019 04:10:07 GMT  
		Size: 14.3 MB (14325952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:slim-threaded-buster` - linux; 386

```console
$ docker pull perl@sha256:4d59f84e33683cfa024e906f5966a2d514788817c4ca90acde091eb82c8f7357
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.7 MB (41671141 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e84bb7ef1b5bbb821a2301f65a35da37892a9e0248e94b9a8e51396cbd52d62`
-	Default Command: `["perl5.30.1","-de0"]`

```dockerfile
# Fri, 22 Nov 2019 16:50:19 GMT
ADD file:68f0911eb53ffc655e6a641b4acfb0670c2fd84c7dc34b0128735f0478532a6b in / 
# Fri, 22 Nov 2019 16:50:19 GMT
CMD ["bash"]
# Sat, 23 Nov 2019 01:56:19 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Sat, 23 Nov 2019 01:56:19 GMT
COPY file:15650064fd29deac721f0aa084ddb3d41db77b78e2907775e257bd67e116ade4 in /usr/src/perl/ 
# Sat, 23 Nov 2019 01:56:19 GMT
WORKDIR /usr/src/perl
# Sat, 23 Nov 2019 03:15:31 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        xz-utils     && curl -SL https://www.cpan.org/src/5.0/perl-5.30.1.tar.xz -o perl-5.30.1.tar.xz     && echo '7336cd3ed0535eb61b76a71350effcfa7c88b44faf37d64d70952ced5d38cd35 *perl-5.30.1.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.30.1.tar.xz -C /usr/src/perl     && rm perl-5.30.1.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && savedPackages="make netbase"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Tue, 26 Nov 2019 00:39:11 GMT
WORKDIR /
# Tue, 26 Nov 2019 00:39:11 GMT
CMD ["perl5.30.1" "-de0"]
```

-	Layers:
	-	`sha256:ce9b44038a207698571bb0cc0b950ee2a3608cb09b2b20712b353a54ae619111`  
		Last Modified: Fri, 22 Nov 2019 16:58:27 GMT  
		Size: 27.7 MB (27746760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccfa8989ff76ba734b1026c0f8a2ef30e80c35b5e1677a90ad731c28aa7d3d3c`  
		Last Modified: Sat, 23 Nov 2019 06:44:29 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cd8e119b8b1f713fa37b93b99084526fd9ee562a01fb8fcc153b9d2537249c1`  
		Last Modified: Sat, 23 Nov 2019 06:45:39 GMT  
		Size: 13.9 MB (13923967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:slim-threaded-buster` - linux; ppc64le

```console
$ docker pull perl@sha256:ed1d388af81b4b9a330b5dc2baaebba56db479397552bd61f27c53ad5e4a7539
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.0 MB (45017563 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df627e3a99e9a8285aa9484aeccc8f58761badeeb98dbe37ecffc59c389692b2`
-	Default Command: `["perl5.30.1","-de0"]`

```dockerfile
# Fri, 22 Nov 2019 14:55:33 GMT
ADD file:56ee7f5cc8715d22f4efb9ec5b1c24fac7fdf8f6dc9c07c45625c4f89bdccac3 in / 
# Fri, 22 Nov 2019 14:55:37 GMT
CMD ["bash"]
# Sat, 23 Nov 2019 03:39:19 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Sat, 23 Nov 2019 03:39:23 GMT
COPY file:15650064fd29deac721f0aa084ddb3d41db77b78e2907775e257bd67e116ade4 in /usr/src/perl/ 
# Sat, 23 Nov 2019 03:39:30 GMT
WORKDIR /usr/src/perl
# Sat, 23 Nov 2019 04:21:40 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        xz-utils     && curl -SL https://www.cpan.org/src/5.0/perl-5.30.1.tar.xz -o perl-5.30.1.tar.xz     && echo '7336cd3ed0535eb61b76a71350effcfa7c88b44faf37d64d70952ced5d38cd35 *perl-5.30.1.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.30.1.tar.xz -C /usr/src/perl     && rm perl-5.30.1.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && savedPackages="make netbase"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Tue, 26 Nov 2019 01:18:45 GMT
WORKDIR /
# Tue, 26 Nov 2019 01:18:49 GMT
CMD ["perl5.30.1" "-de0"]
```

-	Layers:
	-	`sha256:e190211f5678d77388755410611e5e6a755e195e7a1096473c675edc074a2389`  
		Last Modified: Fri, 22 Nov 2019 15:04:10 GMT  
		Size: 30.5 MB (30517327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35cb3313693c5859035c9f1afcd6e895e6f35704024878e09e73c8e43b2d0752`  
		Last Modified: Sat, 23 Nov 2019 06:38:08 GMT  
		Size: 444.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5d5298afd83e0d3c45ccacb3fe5e023213fb895ca56ab867eb2a5f4f5c6c0fc`  
		Last Modified: Sat, 23 Nov 2019 06:40:42 GMT  
		Size: 14.5 MB (14499792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:slim-threaded-buster` - linux; s390x

```console
$ docker pull perl@sha256:ce167225a11babfe9ef4232f81192c08cdaf83d14a2b3032fdaae917f070f18a
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.4 MB (40440169 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af2bd04902486f9b71c45aeb0593e3ea2c7b7ee94c153da85f37204263a7bf8d`
-	Default Command: `["perl5.30.1","-de0"]`

```dockerfile
# Sat, 28 Dec 2019 04:42:03 GMT
ADD file:eec6c56f8680753860198c3af0d94aabb87018ca30f6f6e346621a6bffe0e4b8 in / 
# Sat, 28 Dec 2019 04:42:04 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 07:14:42 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Sat, 28 Dec 2019 07:14:42 GMT
COPY file:15650064fd29deac721f0aa084ddb3d41db77b78e2907775e257bd67e116ade4 in /usr/src/perl/ 
# Sat, 28 Dec 2019 07:14:42 GMT
WORKDIR /usr/src/perl
# Sat, 28 Dec 2019 07:38:38 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        xz-utils     && curl -SL https://www.cpan.org/src/5.0/perl-5.30.1.tar.xz -o perl-5.30.1.tar.xz     && echo '7336cd3ed0535eb61b76a71350effcfa7c88b44faf37d64d70952ced5d38cd35 *perl-5.30.1.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.30.1.tar.xz -C /usr/src/perl     && rm perl-5.30.1.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && savedPackages="make netbase"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Sat, 28 Dec 2019 07:38:38 GMT
WORKDIR /
# Sat, 28 Dec 2019 07:38:38 GMT
CMD ["perl5.30.1" "-de0"]
```

-	Layers:
	-	`sha256:f7542f43e95fb32a870ee38d7f0e7bb23267ac8dcf709e3944311b0a30d7a479`  
		Last Modified: Sat, 28 Dec 2019 04:45:08 GMT  
		Size: 25.7 MB (25705315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ad06d0668af2fbf706d1531c2ab9b4dd67a18f871fad055640c63f5b011589`  
		Last Modified: Sat, 28 Dec 2019 08:56:23 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1b58aa0e051eca6874a9f295adc6b4e41bd487f4baab27cf0ce015c1857079a`  
		Last Modified: Sat, 28 Dec 2019 08:57:25 GMT  
		Size: 14.7 MB (14734440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
