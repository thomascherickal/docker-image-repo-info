## `perl:slim-threaded`

```console
$ docker pull perl@sha256:a73293f7314ae295ac5adb75907404e6fd318bc3d3fef2bb99ac31a11166d40a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `perl:slim-threaded` - linux; amd64

```console
$ docker pull perl@sha256:669619f209904d948eeab2eab19935e59924152d4147b164671bdffd6e9ad506
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.7 MB (41743649 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:829ac92dd11d494e70734f0e2d542aad8d8f64e8c8862ed2ff8ca57531e90023`
-	Default Command: `["perl5.32.0","-de0"]`

```dockerfile
# Tue, 13 Oct 2020 01:39:05 GMT
ADD file:0dc53e7886c35bc21ae6c4f6cedda54d56ae9c9e9cd367678f1a72e68b3c43d4 in / 
# Tue, 13 Oct 2020 01:39:05 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 13:06:39 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Tue, 13 Oct 2020 13:06:39 GMT
COPY file:3744c5cc39cdbdcae10db09a1f0f399005a79f93c237b387a72ff5710cdd458c in /usr/src/perl/ 
# Tue, 13 Oct 2020 13:06:39 GMT
WORKDIR /usr/src/perl
# Tue, 13 Oct 2020 14:18:09 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        xz-utils     && curl -SL https://www.cpan.org/src/5.0/perl-5.32.0.tar.xz -o perl-5.32.0.tar.xz     && echo '6f436b447cf56d22464f980fac1916e707a040e96d52172984c5d184c09b859b *perl-5.32.0.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.32.0.tar.xz -C /usr/src/perl     && rm perl-5.32.0.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && savedPackages="make netbase"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Tue, 13 Oct 2020 14:18:09 GMT
WORKDIR /
# Tue, 13 Oct 2020 14:18:09 GMT
CMD ["perl5.32.0" "-de0"]
```

-	Layers:
	-	`sha256:bb79b6b2107fea8e8a47133a660b78e3a546998fcf0427be39ac9a0af4a97e90`  
		Last Modified: Tue, 13 Oct 2020 01:48:17 GMT  
		Size: 27.1 MB (27092228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c24787a9f8faf672e4ed74e156c1cd261d4482846dc53d139c3034e9aa2a98e`  
		Last Modified: Tue, 13 Oct 2020 17:44:11 GMT  
		Size: 180.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a2e0cc2e74a3d92cbf1ea77bac1ba79fb3d1923b2033d676400fea9ed808843`  
		Last Modified: Tue, 13 Oct 2020 17:45:35 GMT  
		Size: 14.7 MB (14651241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:slim-threaded` - linux; arm variant v7

```console
$ docker pull perl@sha256:7c149603816a9b2cfc40de5995b04b8f251a76486cb69513df2c4a17d611637d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.4 MB (36442719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a1469db52c73b19fe416c072486a0d857b3ae3f90fc09d287b94cd87db334af`
-	Default Command: `["perl5.32.0","-de0"]`

```dockerfile
# Tue, 13 Oct 2020 00:59:29 GMT
ADD file:e423f30ca19eb205a98de21b0545d0a764cfc4f832a9a9631542354d914d98d9 in / 
# Tue, 13 Oct 2020 00:59:31 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 09:25:27 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Tue, 13 Oct 2020 09:25:28 GMT
COPY file:3744c5cc39cdbdcae10db09a1f0f399005a79f93c237b387a72ff5710cdd458c in /usr/src/perl/ 
# Tue, 13 Oct 2020 09:25:29 GMT
WORKDIR /usr/src/perl
# Tue, 13 Oct 2020 10:19:43 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        xz-utils     && curl -SL https://www.cpan.org/src/5.0/perl-5.32.0.tar.xz -o perl-5.32.0.tar.xz     && echo '6f436b447cf56d22464f980fac1916e707a040e96d52172984c5d184c09b859b *perl-5.32.0.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.32.0.tar.xz -C /usr/src/perl     && rm perl-5.32.0.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && savedPackages="make netbase"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Tue, 13 Oct 2020 10:19:49 GMT
WORKDIR /
# Tue, 13 Oct 2020 10:19:54 GMT
CMD ["perl5.32.0" "-de0"]
```

-	Layers:
	-	`sha256:d6d8411ad43db0022fa0fce094cd2e8b1dd2f8a09d6880ed9beb6b4204867027`  
		Last Modified: Tue, 13 Oct 2020 01:08:28 GMT  
		Size: 22.7 MB (22699849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0edae30840220cb7babf673ffd0314cd1166a4317cd0a7d99469ac8af35fa22f`  
		Last Modified: Tue, 13 Oct 2020 13:38:29 GMT  
		Size: 206.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96be21a5db67879c92015f6b541185afbbc628e1aa6a0f1ff2c247c7d0fdabfb`  
		Last Modified: Tue, 13 Oct 2020 13:40:24 GMT  
		Size: 13.7 MB (13742664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:slim-threaded` - linux; arm64 variant v8

```console
$ docker pull perl@sha256:5035694541194a8a5f052db5149e620e68708e47e51fb2af967b551196dc971e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.4 MB (40427932 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ffed2675e4ad1a081015bf49c2fa8397edc6a552ad6dfc550dbd9e5a9e63cc22`
-	Default Command: `["perl5.32.0","-de0"]`

```dockerfile
# Tue, 13 Oct 2020 01:41:09 GMT
ADD file:3488b1423094a75be5bb5956e9187827b8dd35d7a1f2b14081f8e74a1629e7d0 in / 
# Tue, 13 Oct 2020 01:41:11 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 13:26:42 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Tue, 13 Oct 2020 13:26:45 GMT
COPY file:3744c5cc39cdbdcae10db09a1f0f399005a79f93c237b387a72ff5710cdd458c in /usr/src/perl/ 
# Tue, 13 Oct 2020 13:26:46 GMT
WORKDIR /usr/src/perl
# Tue, 13 Oct 2020 14:36:30 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        xz-utils     && curl -SL https://www.cpan.org/src/5.0/perl-5.32.0.tar.xz -o perl-5.32.0.tar.xz     && echo '6f436b447cf56d22464f980fac1916e707a040e96d52172984c5d184c09b859b *perl-5.32.0.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.32.0.tar.xz -C /usr/src/perl     && rm perl-5.32.0.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && savedPackages="make netbase"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Tue, 13 Oct 2020 14:36:33 GMT
WORKDIR /
# Tue, 13 Oct 2020 14:36:34 GMT
CMD ["perl5.32.0" "-de0"]
```

-	Layers:
	-	`sha256:4e6164a63b7b4cf981546947e191644c122214975d40b51ede0536791ebec3d4`  
		Last Modified: Tue, 13 Oct 2020 01:48:17 GMT  
		Size: 25.8 MB (25849329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d593250737fcbd4c2e0888d93d145bd9b8188b50a2940877e810e3c2ddd6af31`  
		Last Modified: Tue, 13 Oct 2020 17:56:08 GMT  
		Size: 205.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb95569c99c464ec15771cfb68d0438ddae76f8a388b0e679b5f73c47505410d`  
		Last Modified: Tue, 13 Oct 2020 17:58:06 GMT  
		Size: 14.6 MB (14578398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:slim-threaded` - linux; 386

```console
$ docker pull perl@sha256:117a43f946265c3810ca6589f103b7b0bbd0968b721365f21e866b755fda4c49
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.9 MB (41934493 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:438c3487aca23bbdd1bec320f9721347637eb91a9271dbf2588e1862114b9388`
-	Default Command: `["perl5.32.0","-de0"]`

```dockerfile
# Tue, 13 Oct 2020 01:41:03 GMT
ADD file:51108b89c70ce0773c897be520c84454660f38b84ba556da49c7fe77e5d52416 in / 
# Tue, 13 Oct 2020 01:41:03 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 11:18:15 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Tue, 13 Oct 2020 11:18:16 GMT
COPY file:3744c5cc39cdbdcae10db09a1f0f399005a79f93c237b387a72ff5710cdd458c in /usr/src/perl/ 
# Tue, 13 Oct 2020 11:18:16 GMT
WORKDIR /usr/src/perl
# Tue, 13 Oct 2020 12:32:10 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        xz-utils     && curl -SL https://www.cpan.org/src/5.0/perl-5.32.0.tar.xz -o perl-5.32.0.tar.xz     && echo '6f436b447cf56d22464f980fac1916e707a040e96d52172984c5d184c09b859b *perl-5.32.0.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.32.0.tar.xz -C /usr/src/perl     && rm perl-5.32.0.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && savedPackages="make netbase"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Tue, 13 Oct 2020 12:32:10 GMT
WORKDIR /
# Tue, 13 Oct 2020 12:32:11 GMT
CMD ["perl5.32.0" "-de0"]
```

-	Layers:
	-	`sha256:97e4efec21eea92209464547d0f52a0f773c505cf4ea9d8090cef667bde145b8`  
		Last Modified: Tue, 13 Oct 2020 01:48:54 GMT  
		Size: 27.8 MB (27750243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e4c3ebea056b8a11c2f22a22c440884b91f305dfe7ea857d54e51e1b1633f0f`  
		Last Modified: Tue, 13 Oct 2020 16:35:44 GMT  
		Size: 179.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce67ae6388cb83642fba0968de99dc343aadde3ad8797396811aca17b58fce9c`  
		Last Modified: Tue, 13 Oct 2020 16:36:49 GMT  
		Size: 14.2 MB (14184071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:slim-threaded` - linux; ppc64le

```console
$ docker pull perl@sha256:fc0b936e82570b691786936030e4b12dea2b3e28967c61703e9aa5f682ea95e9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.3 MB (45258097 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a395e383db3c17e23143b494b35057a8e0731f194860caee2a1aa6f8c289861`
-	Default Command: `["perl5.32.0","-de0"]`

```dockerfile
# Tue, 13 Oct 2020 01:38:54 GMT
ADD file:9992867f855c9bed54df6d26f3d8076689aff8a51e808fefba7d3b66dab250e5 in / 
# Tue, 13 Oct 2020 01:38:59 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 03:52:21 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Tue, 13 Oct 2020 03:52:23 GMT
COPY file:3744c5cc39cdbdcae10db09a1f0f399005a79f93c237b387a72ff5710cdd458c in /usr/src/perl/ 
# Tue, 13 Oct 2020 03:52:26 GMT
WORKDIR /usr/src/perl
# Tue, 13 Oct 2020 04:16:22 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        xz-utils     && curl -SL https://www.cpan.org/src/5.0/perl-5.32.0.tar.xz -o perl-5.32.0.tar.xz     && echo '6f436b447cf56d22464f980fac1916e707a040e96d52172984c5d184c09b859b *perl-5.32.0.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.32.0.tar.xz -C /usr/src/perl     && rm perl-5.32.0.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && savedPackages="make netbase"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Tue, 13 Oct 2020 04:16:31 GMT
WORKDIR /
# Tue, 13 Oct 2020 04:16:34 GMT
CMD ["perl5.32.0" "-de0"]
```

-	Layers:
	-	`sha256:523555c6877c72cfcdec912b4d0053c298b1c97835efc7c6b0211585a06bd563`  
		Last Modified: Tue, 13 Oct 2020 01:50:10 GMT  
		Size: 30.5 MB (30517878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:138a17a5113444f89a75af642dee2fb91e8d05d0df88757fd962a985c7c60427`  
		Last Modified: Tue, 13 Oct 2020 05:01:18 GMT  
		Size: 204.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74c38a589df8d0ddbcc7b11d8e5e86c963457fc989c17116962f20dec51fc874`  
		Last Modified: Tue, 13 Oct 2020 05:01:56 GMT  
		Size: 14.7 MB (14740015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:slim-threaded` - linux; s390x

```console
$ docker pull perl@sha256:f0e4dd627cc198105da26f81a967f35a1f6bbdcd29cc65ca573c46d8edb82f0c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.7 MB (40691621 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b864924b6d76956b9289392608c80115e6b0084a9dac3187eb164c2c13418efe`
-	Default Command: `["perl5.32.0","-de0"]`

```dockerfile
# Tue, 13 Oct 2020 01:42:26 GMT
ADD file:f932c1176fdc9bf45ced816290f83e6231df3dffa3b7f8de1a3bb0adcff1588b in / 
# Tue, 13 Oct 2020 01:42:27 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 03:17:18 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Tue, 13 Oct 2020 03:17:18 GMT
COPY file:3744c5cc39cdbdcae10db09a1f0f399005a79f93c237b387a72ff5710cdd458c in /usr/src/perl/ 
# Tue, 13 Oct 2020 03:17:18 GMT
WORKDIR /usr/src/perl
# Tue, 13 Oct 2020 03:33:23 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        xz-utils     && curl -SL https://www.cpan.org/src/5.0/perl-5.32.0.tar.xz -o perl-5.32.0.tar.xz     && echo '6f436b447cf56d22464f980fac1916e707a040e96d52172984c5d184c09b859b *perl-5.32.0.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.32.0.tar.xz -C /usr/src/perl     && rm perl-5.32.0.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && savedPackages="make netbase"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Tue, 13 Oct 2020 03:33:24 GMT
WORKDIR /
# Tue, 13 Oct 2020 03:33:24 GMT
CMD ["perl5.32.0" "-de0"]
```

-	Layers:
	-	`sha256:2a4f9dc00d797c86c4ffce3b50bea9037c2eb4637f045ad3fd68cf151577b639`  
		Last Modified: Tue, 13 Oct 2020 01:45:45 GMT  
		Size: 25.7 MB (25707519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eebd49218a898d75a29501f6e12a1ba06b9914854cc4ead9767ac26e95edad37`  
		Last Modified: Tue, 13 Oct 2020 04:13:48 GMT  
		Size: 202.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0e23d83e79b93d7c949274b6bae1a92924dbdc7b90096d2332315e3c24c16cc`  
		Last Modified: Tue, 13 Oct 2020 04:14:20 GMT  
		Size: 15.0 MB (14983900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
