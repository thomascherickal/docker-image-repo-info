## `perl:slim-threaded-buster`

```console
$ docker pull perl@sha256:d56b68f40c41f2948a95668b741b93168eb8c91f333509a04f00dd95e99f73a2
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

### `perl:slim-threaded-buster` - linux; amd64

```console
$ docker pull perl@sha256:a04942f1ed875fafff3486c479acb479aab929ac05ba96abce5319318c48dd4a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.0 MB (42035565 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf2affb6ddc930302a076667919edf12d9ef133ddfe9728dac5ca4dd1e7737f9`
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
# Sat, 28 May 2022 06:48:04 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        xz-utils     && curl -SL https://www.cpan.org/src/5.0/perl-5.34.1.tar.xz -o perl-5.34.1.tar.xz     && echo '6d52cf833ff1af27bb5e986870a2c30cec73c044b41e3458cd991f94374039f7 *perl-5.34.1.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.34.1.tar.xz -C /usr/src/perl     && rm perl-5.34.1.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && savedPackages="make netbase"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Sat, 28 May 2022 06:48:04 GMT
WORKDIR /
# Sat, 28 May 2022 06:48:04 GMT
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
	-	`sha256:1018ea3245cfdf5d4b1d5eb6e1312a68abb175d647d0a08a6c0d279b5e35d104`  
		Last Modified: Sat, 28 May 2022 08:04:03 GMT  
		Size: 14.9 MB (14895219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:slim-threaded-buster` - linux; arm variant v5

```console
$ docker pull perl@sha256:5a9c57e25eb13f5ed5296c29f8d43f5e9fe8dd07acb7e91aab47765b5f76c4a8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.1 MB (39085443 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76827c1a124413bfb19010bf74c5c3c74aeb0bc48a13e20a324e22d146f46ff6`
-	Default Command: `["perl5.34.1","-de0"]`

```dockerfile
# Sat, 28 May 2022 02:04:06 GMT
ADD file:26e9ed6c41ec12bf5fd602b7f86b924d34537bbc82442f630763f9f6c48bf3b3 in / 
# Sat, 28 May 2022 02:04:07 GMT
CMD ["bash"]
# Sat, 28 May 2022 04:57:45 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Sat, 28 May 2022 04:57:46 GMT
COPY file:3744c5cc39cdbdcae10db09a1f0f399005a79f93c237b387a72ff5710cdd458c in /usr/src/perl/ 
# Sat, 28 May 2022 04:57:46 GMT
WORKDIR /usr/src/perl
# Sat, 28 May 2022 05:59:49 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        xz-utils     && curl -SL https://www.cpan.org/src/5.0/perl-5.34.1.tar.xz -o perl-5.34.1.tar.xz     && echo '6d52cf833ff1af27bb5e986870a2c30cec73c044b41e3458cd991f94374039f7 *perl-5.34.1.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.34.1.tar.xz -C /usr/src/perl     && rm perl-5.34.1.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && savedPackages="make netbase"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Sat, 28 May 2022 05:59:49 GMT
WORKDIR /
# Sat, 28 May 2022 05:59:50 GMT
CMD ["perl5.34.1" "-de0"]
```

-	Layers:
	-	`sha256:19389fd1100abdedaa775b43242838cdd2d5c8c3388643a7e52da2b7b4399c15`  
		Last Modified: Sat, 28 May 2022 02:20:06 GMT  
		Size: 24.9 MB (24890069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb159f3a466800035e9647fbd9d66babd2ff06474591805a5453b1aa50975c17`  
		Last Modified: Sat, 28 May 2022 09:28:11 GMT  
		Size: 203.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:067bdabb3192cc2a37693288211be8851b54a0072a0a9d69cc0b1df60b35568f`  
		Last Modified: Sat, 28 May 2022 09:31:01 GMT  
		Size: 14.2 MB (14195171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:slim-threaded-buster` - linux; arm variant v7

```console
$ docker pull perl@sha256:cfe6be72f0c92dba895afc0c8522e80cf37f3cecf30446b34b8f3078bea8525e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.7 MB (36734560 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d56da4f98e7f1e9d7e5db9eb822e9dc49ebd9c900e8a9daecd9ddc4227c91ba4`
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
# Wed, 11 May 2022 10:06:57 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        xz-utils     && curl -SL https://www.cpan.org/src/5.0/perl-5.34.1.tar.xz -o perl-5.34.1.tar.xz     && echo '6d52cf833ff1af27bb5e986870a2c30cec73c044b41e3458cd991f94374039f7 *perl-5.34.1.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.34.1.tar.xz -C /usr/src/perl     && rm perl-5.34.1.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && savedPackages="make netbase"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Wed, 11 May 2022 10:06:58 GMT
WORKDIR /
# Wed, 11 May 2022 10:06:58 GMT
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
	-	`sha256:2c0eb311a6103adc68e8115584232e863aba8467e5add30d20ed165b84d408b6`  
		Last Modified: Wed, 11 May 2022 13:27:08 GMT  
		Size: 14.0 MB (13986495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:slim-threaded-buster` - linux; arm64 variant v8

```console
$ docker pull perl@sha256:01444e00bec89ab2f5331f673482d032b4eb54b726f5a53203eec60f3b5b6960
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.7 MB (40747519 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24ea128a3697de06112ad9fd034a877cfa6b45165d37f483208a529c55950f1a`
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
# Sat, 28 May 2022 03:49:52 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        xz-utils     && curl -SL https://www.cpan.org/src/5.0/perl-5.34.1.tar.xz -o perl-5.34.1.tar.xz     && echo '6d52cf833ff1af27bb5e986870a2c30cec73c044b41e3458cd991f94374039f7 *perl-5.34.1.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.34.1.tar.xz -C /usr/src/perl     && rm perl-5.34.1.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && savedPackages="make netbase"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Sat, 28 May 2022 03:49:52 GMT
WORKDIR /
# Sat, 28 May 2022 03:49:53 GMT
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
	-	`sha256:f2cfa3265a61bcf5535c24b18c01f6ad8ed0beecf0640cc449393d725f1db458`  
		Last Modified: Sat, 28 May 2022 04:37:03 GMT  
		Size: 14.8 MB (14833307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:slim-threaded-buster` - linux; 386

```console
$ docker pull perl@sha256:55cc97ab960795613971702d7937808523b78a87bc556f13e4c66f9b218293a4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.2 MB (42238064 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3244ccb8a031bae2fca9309b679c56e602e6201cf35939e6b03252190a1e01aa`
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
# Sat, 28 May 2022 04:45:38 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        xz-utils     && curl -SL https://www.cpan.org/src/5.0/perl-5.34.1.tar.xz -o perl-5.34.1.tar.xz     && echo '6d52cf833ff1af27bb5e986870a2c30cec73c044b41e3458cd991f94374039f7 *perl-5.34.1.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.34.1.tar.xz -C /usr/src/perl     && rm perl-5.34.1.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && savedPackages="make netbase"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Sat, 28 May 2022 04:45:39 GMT
WORKDIR /
# Sat, 28 May 2022 04:45:39 GMT
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
	-	`sha256:53bbe308ea6ad2a072334828a9c3679e3a8e635959dec03bf3538c926a8ac78c`  
		Last Modified: Sat, 28 May 2022 06:14:43 GMT  
		Size: 14.4 MB (14438314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:slim-threaded-buster` - linux; mips64le

```console
$ docker pull perl@sha256:b7abbef2130214ab445f9aaf11ee7357d4072be907add9dc269abc95fa398d31
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.0 MB (39966754 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dddeb56b87f815fff813933ef09887389b1949628cddc37a62b3c05396e2ba7a`
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
# Wed, 11 May 2022 08:27:44 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        xz-utils     && curl -SL https://www.cpan.org/src/5.0/perl-5.34.1.tar.xz -o perl-5.34.1.tar.xz     && echo '6d52cf833ff1af27bb5e986870a2c30cec73c044b41e3458cd991f94374039f7 *perl-5.34.1.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.34.1.tar.xz -C /usr/src/perl     && rm perl-5.34.1.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && savedPackages="make netbase"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Wed, 11 May 2022 08:27:47 GMT
WORKDIR /
# Wed, 11 May 2022 08:27:49 GMT
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
	-	`sha256:53c03821f8beaee950ace8ad05acb39376b358c64170ba805e8e83a5ba901ccf`  
		Last Modified: Wed, 11 May 2022 13:52:11 GMT  
		Size: 14.2 MB (14152047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:slim-threaded-buster` - linux; ppc64le

```console
$ docker pull perl@sha256:895587be479a8e957e9739c2784ecbe27c70b546a4f4120dc6456a51802c893a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.5 MB (45547203 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89f1d36d4f9591d9ac43833e617875b3a9ca67bb36d3afe7f73b933641932579`
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
# Wed, 11 May 2022 11:19:36 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        xz-utils     && curl -SL https://www.cpan.org/src/5.0/perl-5.34.1.tar.xz -o perl-5.34.1.tar.xz     && echo '6d52cf833ff1af27bb5e986870a2c30cec73c044b41e3458cd991f94374039f7 *perl-5.34.1.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.34.1.tar.xz -C /usr/src/perl     && rm perl-5.34.1.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && savedPackages="make netbase"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Wed, 11 May 2022 11:19:39 GMT
WORKDIR /
# Wed, 11 May 2022 11:19:42 GMT
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
	-	`sha256:add09ffc382830c6c95ac9a852f8a07000d2e3be3e8a8554227207164b344665`  
		Last Modified: Wed, 11 May 2022 13:35:38 GMT  
		Size: 15.0 MB (14986457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:slim-threaded-buster` - linux; s390x

```console
$ docker pull perl@sha256:0d95cd4803c61ba2ff87ed953e9b475d947644e354422224c24d8bbe5e171647
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.0 MB (40991718 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0be734d07dfdbe146e632f08c42d298d4a704a869dbb8d8da94dfd5b4fb3f602`
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
# Sat, 28 May 2022 07:01:28 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        xz-utils     && curl -SL https://www.cpan.org/src/5.0/perl-5.34.1.tar.xz -o perl-5.34.1.tar.xz     && echo '6d52cf833ff1af27bb5e986870a2c30cec73c044b41e3458cd991f94374039f7 *perl-5.34.1.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.34.1.tar.xz -C /usr/src/perl     && rm perl-5.34.1.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && savedPackages="make netbase"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Sat, 28 May 2022 07:01:32 GMT
WORKDIR /
# Sat, 28 May 2022 07:01:32 GMT
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
	-	`sha256:c0b71f63d475fadf5c8c785ef462f12cb65eca2517382531f89fa1b37983f9bb`  
		Last Modified: Sat, 28 May 2022 09:02:11 GMT  
		Size: 15.2 MB (15232854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
