## `perl:5-slim-buster`

```console
$ docker pull perl@sha256:081e9c0f9384081a68c8cdec6e784da5dda6b3d3e56a999130621981f0d7621d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `perl:5-slim-buster` - linux; amd64

```console
$ docker pull perl@sha256:daac6975a71fae10a2fec9e49e972aa219c73ea3ebc8415437d986fdf9b1ed11
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.7 MB (41692519 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:27fe7000e572d93b4a3e9d068d87e545313b7fc54f88756b3eeacaad70221859`
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
# Tue, 13 Oct 2020 13:20:12 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        xz-utils     && curl -SL https://www.cpan.org/src/5.0/perl-5.32.0.tar.xz -o perl-5.32.0.tar.xz     && echo '6f436b447cf56d22464f980fac1916e707a040e96d52172984c5d184c09b859b *perl-5.32.0.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.32.0.tar.xz -C /usr/src/perl     && rm perl-5.32.0.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && savedPackages="make netbase"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Tue, 13 Oct 2020 13:20:12 GMT
WORKDIR /
# Tue, 13 Oct 2020 13:20:13 GMT
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
	-	`sha256:e1f05e7b47d1378684af80c7cd86d38ac67608b750abdc18ff94878a98aadebb`  
		Last Modified: Tue, 13 Oct 2020 17:44:31 GMT  
		Size: 14.6 MB (14600111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:5-slim-buster` - linux; arm variant v7

```console
$ docker pull perl@sha256:899d8a230c677fe74ab8fb6b19c64be14d0efc54de55cbaf3d7091fc0865685a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.4 MB (36432492 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22d688902b77c4267b0ad40708877ac79c9397792067aac227404b88ffde6025`
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
# Tue, 13 Oct 2020 09:36:33 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        xz-utils     && curl -SL https://www.cpan.org/src/5.0/perl-5.32.0.tar.xz -o perl-5.32.0.tar.xz     && echo '6f436b447cf56d22464f980fac1916e707a040e96d52172984c5d184c09b859b *perl-5.32.0.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.32.0.tar.xz -C /usr/src/perl     && rm perl-5.32.0.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && savedPackages="make netbase"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Tue, 13 Oct 2020 09:36:35 GMT
WORKDIR /
# Tue, 13 Oct 2020 09:36:36 GMT
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
	-	`sha256:50cef945c360456c803acf12bb9cd804d958be9430460f31122c547a82d98de9`  
		Last Modified: Tue, 13 Oct 2020 13:38:37 GMT  
		Size: 13.7 MB (13732437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:5-slim-buster` - linux; arm64 variant v8

```console
$ docker pull perl@sha256:3f43646b68debb1128cc21f851f2ac90016c0f498ebe0344ced78e2597acff2e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.4 MB (40398484 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:afcc120c42588a6c78f244d888df4aad06efa7a1c35832ee1f6e504bd2b1ced9`
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
# Tue, 13 Oct 2020 13:38:47 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        xz-utils     && curl -SL https://www.cpan.org/src/5.0/perl-5.32.0.tar.xz -o perl-5.32.0.tar.xz     && echo '6f436b447cf56d22464f980fac1916e707a040e96d52172984c5d184c09b859b *perl-5.32.0.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.32.0.tar.xz -C /usr/src/perl     && rm perl-5.32.0.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && savedPackages="make netbase"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Tue, 13 Oct 2020 13:38:49 GMT
WORKDIR /
# Tue, 13 Oct 2020 13:38:49 GMT
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
	-	`sha256:06e4f04c86d8a2b1c1be03e453cf8f3495a89fc4c51d15152cf33d25281ac1bd`  
		Last Modified: Tue, 13 Oct 2020 17:56:16 GMT  
		Size: 14.5 MB (14548950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:5-slim-buster` - linux; 386

```console
$ docker pull perl@sha256:574d8009c1b401c30197d6cf7b4c299b903d3f78d577ffde03e55702de66b9c1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.9 MB (41857521 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1e483ff8b001486d3dcbdc52c5f790a358cc44e602818be655ab3a3cf3be3ea`
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
# Tue, 13 Oct 2020 11:32:49 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        xz-utils     && curl -SL https://www.cpan.org/src/5.0/perl-5.32.0.tar.xz -o perl-5.32.0.tar.xz     && echo '6f436b447cf56d22464f980fac1916e707a040e96d52172984c5d184c09b859b *perl-5.32.0.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.32.0.tar.xz -C /usr/src/perl     && rm perl-5.32.0.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && savedPackages="make netbase"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Tue, 13 Oct 2020 11:32:49 GMT
WORKDIR /
# Tue, 13 Oct 2020 11:32:50 GMT
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
	-	`sha256:d6b757ff7dc87352af939fa5fef89c1cc83e8b8611731230d38691c710ff4630`  
		Last Modified: Tue, 13 Oct 2020 16:35:50 GMT  
		Size: 14.1 MB (14107099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:5-slim-buster` - linux; ppc64le

```console
$ docker pull perl@sha256:4f501bbb87613b3635bfa413bc7cd3d69c22b2e7c966866d648fbeed2e9feb86
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.2 MB (45180161 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80bbbbb7e8821004a6a67eb992e8b8a0458291b97793fc243de68ee508a06a0f`
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
# Tue, 13 Oct 2020 04:03:57 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        xz-utils     && curl -SL https://www.cpan.org/src/5.0/perl-5.32.0.tar.xz -o perl-5.32.0.tar.xz     && echo '6f436b447cf56d22464f980fac1916e707a040e96d52172984c5d184c09b859b *perl-5.32.0.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.32.0.tar.xz -C /usr/src/perl     && rm perl-5.32.0.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && savedPackages="make netbase"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Tue, 13 Oct 2020 04:04:16 GMT
WORKDIR /
# Tue, 13 Oct 2020 04:04:23 GMT
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
	-	`sha256:3096c2c455ba3411c994f7d1f2662b456f493256d40422f1f47bfa2859330e75`  
		Last Modified: Tue, 13 Oct 2020 05:01:21 GMT  
		Size: 14.7 MB (14662079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:5-slim-buster` - linux; s390x

```console
$ docker pull perl@sha256:e94dea32f0c5101d3cd2a2d061cc9fca3625ff876f024e0dcd9fdc9bfe24970c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.6 MB (40643110 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7e35de3baa8319a5d71b20e59d6b8d4aede2504b24c9824fd3b6c7344325b9d`
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
# Tue, 13 Oct 2020 03:22:02 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        xz-utils     && curl -SL https://www.cpan.org/src/5.0/perl-5.32.0.tar.xz -o perl-5.32.0.tar.xz     && echo '6f436b447cf56d22464f980fac1916e707a040e96d52172984c5d184c09b859b *perl-5.32.0.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.32.0.tar.xz -C /usr/src/perl     && rm perl-5.32.0.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && savedPackages="make netbase"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Tue, 13 Oct 2020 03:22:03 GMT
WORKDIR /
# Tue, 13 Oct 2020 03:22:03 GMT
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
	-	`sha256:80e3e1eca0ca0e22ad009cbdb8e07c19c25fca599ce03d346476d56f6b33c2b3`  
		Last Modified: Tue, 13 Oct 2020 04:13:51 GMT  
		Size: 14.9 MB (14935389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
