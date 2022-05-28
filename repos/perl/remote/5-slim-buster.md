## `perl:5-slim-buster`

```console
$ docker pull perl@sha256:e20f383e0829a01fa1f2f5288cd42cfebb90a39647198e6733bc2620d359385c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `perl:5-slim-buster` - linux; amd64

```console
$ docker pull perl@sha256:192192b3c38e3f48392da59c13f72125012b5eb3288c42c6f83f0b86d655acd0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.0 MB (41986550 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c7945c445994322b2fda897156f1680ab491a0d1fe4f8ff6b3f3a88e7c9c723`
-	Default Command: `["perl5.34.1","-de0"]`

```dockerfile
# Sat, 28 May 2022 01:20:43 GMT
ADD file:0513eda9512e010cb9459591b62e0c9d9319750923df091b64250ad6e98c2878 in / 
# Sat, 28 May 2022 01:20:43 GMT
CMD ["bash"]
# Sat, 28 May 2022 06:24:32 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Sat, 28 May 2022 06:24:32 GMT
COPY file:3744c5cc39cdbdcae10db09a1f0f399005a79f93c237b387a72ff5710cdd458c in /usr/src/perl/ 
# Sat, 28 May 2022 06:24:32 GMT
WORKDIR /usr/src/perl
# Sat, 28 May 2022 06:28:55 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        xz-utils     && curl -SL https://www.cpan.org/src/5.0/perl-5.34.1.tar.xz -o perl-5.34.1.tar.xz     && echo '6d52cf833ff1af27bb5e986870a2c30cec73c044b41e3458cd991f94374039f7 *perl-5.34.1.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.34.1.tar.xz -C /usr/src/perl     && rm perl-5.34.1.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && savedPackages="make netbase"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Sat, 28 May 2022 06:28:55 GMT
WORKDIR /
# Sat, 28 May 2022 06:28:55 GMT
CMD ["perl5.34.1" "-de0"]
```

-	Layers:
	-	`sha256:c1ad9731b2c7bf7fddea67f2f3f553515179a375c489e591e2372700fcaca766`  
		Last Modified: Sat, 28 May 2022 01:26:05 GMT  
		Size: 27.1 MB (27140144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8729058f5920be556d7d5a93ebcbfcc26d6ae006c81c2f430bec1b1094e23533`  
		Last Modified: Sat, 28 May 2022 08:02:30 GMT  
		Size: 202.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca89b17385d76d35450a3b6ccdb6a52f3a076e5931a718a5f3bab74d6907d935`  
		Last Modified: Sat, 28 May 2022 08:02:33 GMT  
		Size: 14.8 MB (14846204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:5-slim-buster` - linux; arm variant v5

```console
$ docker pull perl@sha256:bd893f3ae6a1d9a7a7d1f1d4104ad754026e1a4d3618ee32e2b790bedc67652d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.1 MB (39061645 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:482944a5c252c89fe0e08b3d05c8398995e347e8e48c881cd47f42f9884c72b9`
-	Default Command: `["perl5.34.1","-de0"]`

```dockerfile
# Wed, 11 May 2022 00:51:34 GMT
ADD file:c4087f224dff43064778eac76e711d30ca4882a1d3b571b1cd509089166abc0d in / 
# Wed, 11 May 2022 00:51:35 GMT
CMD ["bash"]
# Wed, 11 May 2022 03:59:24 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Wed, 11 May 2022 03:59:25 GMT
COPY file:3744c5cc39cdbdcae10db09a1f0f399005a79f93c237b387a72ff5710cdd458c in /usr/src/perl/ 
# Wed, 11 May 2022 03:59:25 GMT
WORKDIR /usr/src/perl
# Wed, 11 May 2022 04:12:25 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        xz-utils     && curl -SL https://www.cpan.org/src/5.0/perl-5.34.1.tar.xz -o perl-5.34.1.tar.xz     && echo '6d52cf833ff1af27bb5e986870a2c30cec73c044b41e3458cd991f94374039f7 *perl-5.34.1.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.34.1.tar.xz -C /usr/src/perl     && rm perl-5.34.1.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && savedPackages="make netbase"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Wed, 11 May 2022 04:12:26 GMT
WORKDIR /
# Wed, 11 May 2022 04:12:26 GMT
CMD ["perl5.34.1" "-de0"]
```

-	Layers:
	-	`sha256:69d6138017be389335ab570ff643096d0ea914f563d41f238e7ff3520fe8e93f`  
		Last Modified: Wed, 11 May 2022 01:07:20 GMT  
		Size: 24.9 MB (24889917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:013004d0f6bda05537cb74101dd6d9357de2daacde57c2a7661c12f981d6bda4`  
		Last Modified: Wed, 11 May 2022 08:32:56 GMT  
		Size: 202.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d83cb6a4942cb1b013c7655d82b28ba778af45e3816db372986abf5a0b91fb94`  
		Last Modified: Wed, 11 May 2022 08:33:09 GMT  
		Size: 14.2 MB (14171526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:5-slim-buster` - linux; arm variant v7

```console
$ docker pull perl@sha256:a98ff747b929806181fd2b98e2f24c5060b1153ac41be58ee8a3c5de2cdb1370
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.7 MB (36719864 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1ad5fe9a0116b8036e81d60b3d91f5913497eae9fdb1414f9e0e3464ffca284`
-	Default Command: `["perl5.34.1","-de0"]`

```dockerfile
# Wed, 11 May 2022 01:50:13 GMT
ADD file:bccd1898e72cc79621c20ba59061d318521fbd2a8f10806cc3a1561fcbc9daad in / 
# Wed, 11 May 2022 01:50:14 GMT
CMD ["bash"]
# Wed, 11 May 2022 09:09:40 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Wed, 11 May 2022 09:09:40 GMT
COPY file:3744c5cc39cdbdcae10db09a1f0f399005a79f93c237b387a72ff5710cdd458c in /usr/src/perl/ 
# Wed, 11 May 2022 09:09:41 GMT
WORKDIR /usr/src/perl
# Wed, 11 May 2022 09:21:49 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        xz-utils     && curl -SL https://www.cpan.org/src/5.0/perl-5.34.1.tar.xz -o perl-5.34.1.tar.xz     && echo '6d52cf833ff1af27bb5e986870a2c30cec73c044b41e3458cd991f94374039f7 *perl-5.34.1.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.34.1.tar.xz -C /usr/src/perl     && rm perl-5.34.1.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && savedPackages="make netbase"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Wed, 11 May 2022 09:21:50 GMT
WORKDIR /
# Wed, 11 May 2022 09:21:51 GMT
CMD ["perl5.34.1" "-de0"]
```

-	Layers:
	-	`sha256:8f4c08df22a944142862818447616fff8b15d3a7ba383d4eeab678af698c2c43`  
		Last Modified: Wed, 11 May 2022 02:06:00 GMT  
		Size: 22.7 MB (22747864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83bd84033e4ffbf2c4e350578c05e70c06208f3db9e535df27fc2fe455c9321b`  
		Last Modified: Wed, 11 May 2022 13:24:14 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac72a3ca3f44bbd2f22c6cca3e40b0914d13e1e94fe5a8cc4a0c8f2e241a3f47`  
		Last Modified: Wed, 11 May 2022 13:24:27 GMT  
		Size: 14.0 MB (13971799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:5-slim-buster` - linux; arm64 variant v8

```console
$ docker pull perl@sha256:36cf23f4d50ab38843fc4821d8705cc21846e432a280d6113d58263b766fff38
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.7 MB (40710474 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a78a14f7d39de076d34f140ec928ff0e59c797e7505f2d75d266225524e016f`
-	Default Command: `["perl5.34.1","-de0"]`

```dockerfile
# Sat, 28 May 2022 00:41:05 GMT
ADD file:d0e42d603f275c040783ec7b6c051200815492fc35b73110234dfcd584e6cdec in / 
# Sat, 28 May 2022 00:41:05 GMT
CMD ["bash"]
# Sat, 28 May 2022 03:31:42 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Sat, 28 May 2022 03:31:44 GMT
COPY file:3744c5cc39cdbdcae10db09a1f0f399005a79f93c237b387a72ff5710cdd458c in /usr/src/perl/ 
# Sat, 28 May 2022 03:31:44 GMT
WORKDIR /usr/src/perl
# Sat, 28 May 2022 03:37:34 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        xz-utils     && curl -SL https://www.cpan.org/src/5.0/perl-5.34.1.tar.xz -o perl-5.34.1.tar.xz     && echo '6d52cf833ff1af27bb5e986870a2c30cec73c044b41e3458cd991f94374039f7 *perl-5.34.1.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.34.1.tar.xz -C /usr/src/perl     && rm perl-5.34.1.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && savedPackages="make netbase"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Sat, 28 May 2022 03:37:35 GMT
WORKDIR /
# Sat, 28 May 2022 03:37:35 GMT
CMD ["perl5.34.1" "-de0"]
```

-	Layers:
	-	`sha256:4931fb8ba4223cb35034141162105ee5482122692b2931eb69eec912ce64606d`  
		Last Modified: Sat, 28 May 2022 00:48:26 GMT  
		Size: 25.9 MB (25914033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6e011944e8b02e9f088c22bd7fe2014f667954d88a1f95147d9c66beece0f3b`  
		Last Modified: Sat, 28 May 2022 04:36:01 GMT  
		Size: 179.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70405a25de6108bd548aa64570b7b16723816074c8def9e950fad260d3d2f316`  
		Last Modified: Sat, 28 May 2022 04:36:04 GMT  
		Size: 14.8 MB (14796262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:5-slim-buster` - linux; 386

```console
$ docker pull perl@sha256:715cd02065a5a1f39da053e76e10d3be5babf471648ddca71df4d9cc17826ebb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.1 MB (42148597 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7428902a3844cb61714cdcaddabe7c862f25e0bb8f2df60230cbcaa673daf8d`
-	Default Command: `["perl5.34.1","-de0"]`

```dockerfile
# Sat, 28 May 2022 00:40:01 GMT
ADD file:9aea7a35c215cdd778adec1dd5213973ef9b4830110e4550f2ead85679551ee5 in / 
# Sat, 28 May 2022 00:40:01 GMT
CMD ["bash"]
# Sat, 28 May 2022 04:19:14 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Sat, 28 May 2022 04:19:16 GMT
COPY file:3744c5cc39cdbdcae10db09a1f0f399005a79f93c237b387a72ff5710cdd458c in /usr/src/perl/ 
# Sat, 28 May 2022 04:19:16 GMT
WORKDIR /usr/src/perl
# Sat, 28 May 2022 04:24:20 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        xz-utils     && curl -SL https://www.cpan.org/src/5.0/perl-5.34.1.tar.xz -o perl-5.34.1.tar.xz     && echo '6d52cf833ff1af27bb5e986870a2c30cec73c044b41e3458cd991f94374039f7 *perl-5.34.1.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.34.1.tar.xz -C /usr/src/perl     && rm perl-5.34.1.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && savedPackages="make netbase"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Sat, 28 May 2022 04:24:20 GMT
WORKDIR /
# Sat, 28 May 2022 04:24:21 GMT
CMD ["perl5.34.1" "-de0"]
```

-	Layers:
	-	`sha256:40837b3d848885c0b0c031d6d950b38e6a26962a5ee49704cb3ca2d2db535617`  
		Last Modified: Sat, 28 May 2022 00:47:36 GMT  
		Size: 27.8 MB (27799572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4df56743e83452488d5118fbf98a6ca3b9db025bedd9acb66553fb521037d0b`  
		Last Modified: Sat, 28 May 2022 06:12:55 GMT  
		Size: 178.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f581f250df26ce75cb32e4f51faa66779c6c9402eb47bb86975d9e366b17de5b`  
		Last Modified: Sat, 28 May 2022 06:12:58 GMT  
		Size: 14.3 MB (14348847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:5-slim-buster` - linux; mips64le

```console
$ docker pull perl@sha256:b08f76258cd1e1cd47b88000aaaaed9c9216d2df05f4d255617c67f4fb3a4f89
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.9 MB (39904651 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e1ea9aa21e2731e57c6658e3d8f555b5b4b7643df820f652e3c5b8369a32f35`
-	Default Command: `["perl5.34.1","-de0"]`

```dockerfile
# Wed, 11 May 2022 02:24:43 GMT
ADD file:caccabd8a6e13c6bee91558efc76401078239e82c1a4a939aaf89520fab347fd in / 
# Wed, 11 May 2022 02:24:48 GMT
CMD ["bash"]
# Wed, 11 May 2022 06:42:10 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Wed, 11 May 2022 06:42:12 GMT
COPY file:3744c5cc39cdbdcae10db09a1f0f399005a79f93c237b387a72ff5710cdd458c in /usr/src/perl/ 
# Wed, 11 May 2022 06:42:14 GMT
WORKDIR /usr/src/perl
# Wed, 11 May 2022 07:02:11 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        xz-utils     && curl -SL https://www.cpan.org/src/5.0/perl-5.34.1.tar.xz -o perl-5.34.1.tar.xz     && echo '6d52cf833ff1af27bb5e986870a2c30cec73c044b41e3458cd991f94374039f7 *perl-5.34.1.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.34.1.tar.xz -C /usr/src/perl     && rm perl-5.34.1.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && savedPackages="make netbase"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Wed, 11 May 2022 07:02:14 GMT
WORKDIR /
# Wed, 11 May 2022 07:02:17 GMT
CMD ["perl5.34.1" "-de0"]
```

-	Layers:
	-	`sha256:04988468cf482e6d371e4ebf5a6fb630cd38493fcc79fe45f15650a319a1a0a5`  
		Last Modified: Wed, 11 May 2022 02:35:04 GMT  
		Size: 25.8 MB (25814525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5677f8a662455f2f7f434a5578b9ddba6fa1940df5a0c15d2e5cda183d8f3689`  
		Last Modified: Wed, 11 May 2022 13:49:53 GMT  
		Size: 182.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54910aec927d3053399023246b90df1e23fe7351ad557b23bd0fd840c666a76d`  
		Last Modified: Wed, 11 May 2022 13:50:05 GMT  
		Size: 14.1 MB (14089944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:5-slim-buster` - linux; ppc64le

```console
$ docker pull perl@sha256:9ad8db7735ca41bb6e86033fe77687b8f61836a963a23e9673bc77bfa1b2984a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.5 MB (45461941 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d12a0d6d6417ce5ce2e3c18d2b8412f267238b91a9b9f5ce7fc4b4d31ef7d9ca`
-	Default Command: `["perl5.34.1","-de0"]`

```dockerfile
# Wed, 11 May 2022 01:33:31 GMT
ADD file:57fcc3eadd20c2481e373ef3b56a194006f65b3c7ae29bd1747e625efcd89124 in / 
# Wed, 11 May 2022 01:33:37 GMT
CMD ["bash"]
# Wed, 11 May 2022 10:37:13 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Wed, 11 May 2022 10:37:16 GMT
COPY file:3744c5cc39cdbdcae10db09a1f0f399005a79f93c237b387a72ff5710cdd458c in /usr/src/perl/ 
# Wed, 11 May 2022 10:37:19 GMT
WORKDIR /usr/src/perl
# Wed, 11 May 2022 10:47:08 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        xz-utils     && curl -SL https://www.cpan.org/src/5.0/perl-5.34.1.tar.xz -o perl-5.34.1.tar.xz     && echo '6d52cf833ff1af27bb5e986870a2c30cec73c044b41e3458cd991f94374039f7 *perl-5.34.1.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.34.1.tar.xz -C /usr/src/perl     && rm perl-5.34.1.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && savedPackages="make netbase"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Wed, 11 May 2022 10:47:15 GMT
WORKDIR /
# Wed, 11 May 2022 10:47:17 GMT
CMD ["perl5.34.1" "-de0"]
```

-	Layers:
	-	`sha256:97c4e3bbd0d14c4a194ce9c48b362e1649c341b249c2ad560738b06fe8576dc3`  
		Last Modified: Wed, 11 May 2022 01:44:06 GMT  
		Size: 30.6 MB (30560544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0f5d58695b75a1cdfd8830d297f5c5184bb5f89d646e8d4c584e9ff06f5e666`  
		Last Modified: Wed, 11 May 2022 13:33:26 GMT  
		Size: 202.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a951f0da7b72c729b293e35e09b39ae7f581a9316e91acab44603061cb656b02`  
		Last Modified: Wed, 11 May 2022 13:33:30 GMT  
		Size: 14.9 MB (14901195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:5-slim-buster` - linux; s390x

```console
$ docker pull perl@sha256:c842c279ac0025632919cb5eea5c91082c1f5fee990612db8f6aa5caf5d176d3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.9 MB (40947851 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fccebdeea4f8ed52c271b599d44dacc6af9e0ce7bda428158f1cdfe94e0929f6`
-	Default Command: `["perl5.34.1","-de0"]`

```dockerfile
# Sat, 28 May 2022 00:43:43 GMT
ADD file:eb7d389650b193828480416ddc8257a8dc05bcaba9be79ef2b931e7bbae39bdc in / 
# Sat, 28 May 2022 00:43:45 GMT
CMD ["bash"]
# Sat, 28 May 2022 06:03:31 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Sat, 28 May 2022 06:03:31 GMT
COPY file:3744c5cc39cdbdcae10db09a1f0f399005a79f93c237b387a72ff5710cdd458c in /usr/src/perl/ 
# Sat, 28 May 2022 06:03:32 GMT
WORKDIR /usr/src/perl
# Sat, 28 May 2022 06:13:52 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        xz-utils     && curl -SL https://www.cpan.org/src/5.0/perl-5.34.1.tar.xz -o perl-5.34.1.tar.xz     && echo '6d52cf833ff1af27bb5e986870a2c30cec73c044b41e3458cd991f94374039f7 *perl-5.34.1.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.34.1.tar.xz -C /usr/src/perl     && rm perl-5.34.1.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && savedPackages="make netbase"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Sat, 28 May 2022 06:13:57 GMT
WORKDIR /
# Sat, 28 May 2022 06:13:57 GMT
CMD ["perl5.34.1" "-de0"]
```

-	Layers:
	-	`sha256:94516ab12915ac684a13a2161b8bcaa315b01708a424f29d321971d81ac29a93`  
		Last Modified: Sat, 28 May 2022 00:50:20 GMT  
		Size: 25.8 MB (25758660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:483de1e463ebae2adcf49842189a50523ef242dcbde07c9df355217cf8b16376`  
		Last Modified: Sat, 28 May 2022 09:00:41 GMT  
		Size: 204.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ad6b92ddf3de90c6fc31902579557ba33c74e8b1c5cbc5e260a2efd89b3ff2c`  
		Last Modified: Sat, 28 May 2022 09:00:44 GMT  
		Size: 15.2 MB (15188987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
