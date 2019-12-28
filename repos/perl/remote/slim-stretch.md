## `perl:slim-stretch`

```console
$ docker pull perl@sha256:0fd0dd4722b40e61068703660aac7b03ecc294f1c0d957a3cfadf820008681d6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `perl:slim-stretch` - linux; amd64

```console
$ docker pull perl@sha256:479dbf5d5a1582dd0994bafa9fd3b0537053a731fcf1f6baba81785bb195b1f7
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.9 MB (36854153 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ed641e5b57d396101cae892d210420719527c840d985019ae147e1622c9e039`
-	Default Command: `["perl5.30.1","-de0"]`

```dockerfile
# Fri, 22 Nov 2019 14:59:24 GMT
ADD file:2c1f5e08834f13ccb9c2326204eb2556e03239d00171e75755c7195289374c61 in / 
# Fri, 22 Nov 2019 14:59:25 GMT
CMD ["bash"]
# Sat, 23 Nov 2019 08:49:23 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Sat, 23 Nov 2019 08:49:24 GMT
COPY file:15650064fd29deac721f0aa084ddb3d41db77b78e2907775e257bd67e116ade4 in /usr/src/perl/ 
# Sat, 23 Nov 2019 08:49:24 GMT
WORKDIR /usr/src/perl
# Sat, 23 Nov 2019 09:00:38 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        xz-utils     && curl -SL https://www.cpan.org/src/5.0/perl-5.30.1.tar.xz -o perl-5.30.1.tar.xz     && echo '7336cd3ed0535eb61b76a71350effcfa7c88b44faf37d64d70952ced5d38cd35 *perl-5.30.1.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.30.1.tar.xz -C /usr/src/perl     && rm perl-5.30.1.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && savedPackages="make netbase"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Tue, 26 Nov 2019 01:22:15 GMT
WORKDIR /
# Tue, 26 Nov 2019 01:22:15 GMT
CMD ["perl5.30.1" "-de0"]
```

-	Layers:
	-	`sha256:d599a449871ee73b960e80d176b989365dfecb4c8f337bf21e8853862403ee9b`  
		Last Modified: Fri, 22 Nov 2019 15:06:36 GMT  
		Size: 22.5 MB (22524572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66b256b52d233b80b1aa8b4b61bf927ab3b0e9f0b2ed114b1fc3acd25708e7b7`  
		Last Modified: Sat, 23 Nov 2019 12:39:41 GMT  
		Size: 416.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8c5b2462458e4558d504389b03e14af1c0b9d6202f7bbfe1179e47f34df7718`  
		Last Modified: Sat, 23 Nov 2019 12:39:47 GMT  
		Size: 14.3 MB (14329165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:slim-stretch` - linux; arm variant v7

```console
$ docker pull perl@sha256:de649bcd7ee98094ecb36e12ecfe389474fe1e19e3a4727d0d78c3d403f8c20c
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.8 MB (32784714 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6a8c4df5b7e5bf5d78caadc1e0e7701decb9d3b4f29e937eab9f3b7c0b87de5`
-	Default Command: `["perl5.30.1","-de0"]`

```dockerfile
# Sat, 28 Dec 2019 05:03:51 GMT
ADD file:2002ba672e32ae75369830ed6a4734ce62e0118e42390b4d657f0985d6b7fd6a in / 
# Sat, 28 Dec 2019 05:03:53 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 08:25:46 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Sat, 28 Dec 2019 08:25:47 GMT
COPY file:15650064fd29deac721f0aa084ddb3d41db77b78e2907775e257bd67e116ade4 in /usr/src/perl/ 
# Sat, 28 Dec 2019 08:25:49 GMT
WORKDIR /usr/src/perl
# Sat, 28 Dec 2019 08:36:58 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        xz-utils     && curl -SL https://www.cpan.org/src/5.0/perl-5.30.1.tar.xz -o perl-5.30.1.tar.xz     && echo '7336cd3ed0535eb61b76a71350effcfa7c88b44faf37d64d70952ced5d38cd35 *perl-5.30.1.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.30.1.tar.xz -C /usr/src/perl     && rm perl-5.30.1.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && savedPackages="make netbase"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Sat, 28 Dec 2019 08:36:59 GMT
WORKDIR /
# Sat, 28 Dec 2019 08:37:00 GMT
CMD ["perl5.30.1" "-de0"]
```

-	Layers:
	-	`sha256:77cf262539006c8df77496f500f74a8c1edd158062440fd94d43d5b1292cefee`  
		Last Modified: Sat, 28 Dec 2019 05:11:13 GMT  
		Size: 19.3 MB (19311587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:143bf04aa299c977ac57ab86e5b4c42fb1cc5c8a8fd33cacf8a084ee4562cd18`  
		Last Modified: Sat, 28 Dec 2019 12:05:52 GMT  
		Size: 441.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d92a9bde745cc224f7afcd3ad754e1456e18b35dcb122f2601f5170d1e919766`  
		Last Modified: Sat, 28 Dec 2019 12:05:57 GMT  
		Size: 13.5 MB (13472686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:slim-stretch` - linux; arm64 variant v8

```console
$ docker pull perl@sha256:b44a54b8e68651804671a7a24e403b5195ca9fecb2456bb9617765c7b71595cb
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.5 MB (34537205 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da2f0b9735385a505efb74865718c30c89138b23307287a929135072b216b2b6`
-	Default Command: `["perl5.30.1","-de0"]`

```dockerfile
# Fri, 22 Nov 2019 13:45:50 GMT
ADD file:8e4d0a1e6805c641fc9d18ebad82e4b01d85c6cb9f87d1ef47d75d150212a392 in / 
# Fri, 22 Nov 2019 13:45:53 GMT
CMD ["bash"]
# Sat, 23 Nov 2019 00:02:57 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Sat, 23 Nov 2019 00:02:58 GMT
COPY file:15650064fd29deac721f0aa084ddb3d41db77b78e2907775e257bd67e116ade4 in /usr/src/perl/ 
# Sat, 23 Nov 2019 00:02:59 GMT
WORKDIR /usr/src/perl
# Sat, 23 Nov 2019 00:14:32 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        xz-utils     && curl -SL https://www.cpan.org/src/5.0/perl-5.30.1.tar.xz -o perl-5.30.1.tar.xz     && echo '7336cd3ed0535eb61b76a71350effcfa7c88b44faf37d64d70952ced5d38cd35 *perl-5.30.1.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.30.1.tar.xz -C /usr/src/perl     && rm perl-5.30.1.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && savedPackages="make netbase"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Tue, 26 Nov 2019 01:04:25 GMT
WORKDIR /
# Tue, 26 Nov 2019 01:04:42 GMT
CMD ["perl5.30.1" "-de0"]
```

-	Layers:
	-	`sha256:98a64bf4db7d2219b4fdd8182188d9422810dee890e997095bfb564a0482eed6`  
		Last Modified: Fri, 22 Nov 2019 13:52:17 GMT  
		Size: 20.4 MB (20385759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c7387377d125db2c901eedf8f0c5fc84e93d3b4df71914e04c6cbb92f8086c3`  
		Last Modified: Sat, 23 Nov 2019 04:09:06 GMT  
		Size: 441.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc0da07dae98e3a951a5c6b390de51a02bc4e54dc4d3316c4deebb162e7fb46d`  
		Last Modified: Sat, 23 Nov 2019 04:09:13 GMT  
		Size: 14.2 MB (14151005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:slim-stretch` - linux; 386

```console
$ docker pull perl@sha256:33ad19d7952a7e73005a165e32a49961ce8a81cbf4639aaf0f4987f415d45c8a
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.0 MB (36973000 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:365f26a0126453f32519e00a3f6222d3dcbdd47f9a051c0234b4c53a840d351a`
-	Default Command: `["perl5.30.1","-de0"]`

```dockerfile
# Fri, 22 Nov 2019 16:54:44 GMT
ADD file:19d04f738434c76e2dbd14b48de2f0f03afa883b15f638c6ecbbf382df03567c in / 
# Fri, 22 Nov 2019 16:54:44 GMT
CMD ["bash"]
# Sat, 23 Nov 2019 02:12:29 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Sat, 23 Nov 2019 02:12:29 GMT
COPY file:15650064fd29deac721f0aa084ddb3d41db77b78e2907775e257bd67e116ade4 in /usr/src/perl/ 
# Sat, 23 Nov 2019 02:12:30 GMT
WORKDIR /usr/src/perl
# Sat, 23 Nov 2019 02:27:27 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        xz-utils     && curl -SL https://www.cpan.org/src/5.0/perl-5.30.1.tar.xz -o perl-5.30.1.tar.xz     && echo '7336cd3ed0535eb61b76a71350effcfa7c88b44faf37d64d70952ced5d38cd35 *perl-5.30.1.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.30.1.tar.xz -C /usr/src/perl     && rm perl-5.30.1.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && savedPackages="make netbase"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Tue, 26 Nov 2019 00:38:59 GMT
WORKDIR /
# Tue, 26 Nov 2019 00:38:59 GMT
CMD ["perl5.30.1" "-de0"]
```

-	Layers:
	-	`sha256:f26c9a85c76e393c9f2313b30e82d09f933d2dd4883620de242c7d21f8812e91`  
		Last Modified: Fri, 22 Nov 2019 17:03:03 GMT  
		Size: 23.2 MB (23152070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fd36bff35a231ad00cfbde5b53295be3ecec56005de837e515cb3a2dbe13a03`  
		Last Modified: Sat, 23 Nov 2019 06:44:49 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3da0e46a1d0f1cdf28a30a39f9bdddb6b7fdff6ebd6e434b051322b7d64bfe1`  
		Last Modified: Sat, 23 Nov 2019 06:44:57 GMT  
		Size: 13.8 MB (13820517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:slim-stretch` - linux; ppc64le

```console
$ docker pull perl@sha256:fc0a248d768596efe1e2ae69ac35c47e3438f84a9b2ed7440c5f94129ce77853
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.0 MB (36982810 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:473ce0621e102aabdffb221e5ce444461aa5b03afc7cac77d42472a8d105f62a`
-	Default Command: `["perl5.30.1","-de0"]`

```dockerfile
# Sat, 28 Dec 2019 04:23:21 GMT
ADD file:a1ee5955ff3ede8df9558f4bec0c7962d54c43374f857e1da7e2639ddf82a9f1 in / 
# Sat, 28 Dec 2019 04:23:24 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 10:00:33 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Sat, 28 Dec 2019 10:00:34 GMT
COPY file:15650064fd29deac721f0aa084ddb3d41db77b78e2907775e257bd67e116ade4 in /usr/src/perl/ 
# Sat, 28 Dec 2019 10:00:36 GMT
WORKDIR /usr/src/perl
# Sat, 28 Dec 2019 10:09:33 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        xz-utils     && curl -SL https://www.cpan.org/src/5.0/perl-5.30.1.tar.xz -o perl-5.30.1.tar.xz     && echo '7336cd3ed0535eb61b76a71350effcfa7c88b44faf37d64d70952ced5d38cd35 *perl-5.30.1.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.30.1.tar.xz -C /usr/src/perl     && rm perl-5.30.1.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && savedPackages="make netbase"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Sat, 28 Dec 2019 10:09:40 GMT
WORKDIR /
# Sat, 28 Dec 2019 10:09:43 GMT
CMD ["perl5.30.1" "-de0"]
```

-	Layers:
	-	`sha256:af52e7ef6e83efadeae17be91daa6ecf61b7dfb39709c29be9b24876e60c0e36`  
		Last Modified: Sat, 28 Dec 2019 04:33:19 GMT  
		Size: 22.8 MB (22800791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5818177722de90eb0ea1eba11644272b46d315db5ba90292951d1d35bfc09b6`  
		Last Modified: Sat, 28 Dec 2019 12:51:43 GMT  
		Size: 444.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78c491122f961d2465de205d6e670e0e658768bd7314e2ec7342aeb9a867817d`  
		Last Modified: Sat, 28 Dec 2019 12:51:56 GMT  
		Size: 14.2 MB (14181575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:slim-stretch` - linux; s390x

```console
$ docker pull perl@sha256:c1d5474ba1a1696b8c760243fa118edb9d27dce5c2bbe3c37d602539c8bbf303
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.2 MB (37176610 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:082b6d925ff1bfaaebd70760147174399114f6d68c0bb58b14e7883043d63934`
-	Default Command: `["perl5.30.1","-de0"]`

```dockerfile
# Sat, 28 Dec 2019 04:43:21 GMT
ADD file:f5d0e8fb7b76fc65fc5a0951e7d647f26d110f5c92d4effe2ada348f661c87af in / 
# Sat, 28 Dec 2019 04:43:21 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 07:19:16 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Sat, 28 Dec 2019 07:19:17 GMT
COPY file:15650064fd29deac721f0aa084ddb3d41db77b78e2907775e257bd67e116ade4 in /usr/src/perl/ 
# Sat, 28 Dec 2019 07:19:17 GMT
WORKDIR /usr/src/perl
# Sat, 28 Dec 2019 07:23:43 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        xz-utils     && curl -SL https://www.cpan.org/src/5.0/perl-5.30.1.tar.xz -o perl-5.30.1.tar.xz     && echo '7336cd3ed0535eb61b76a71350effcfa7c88b44faf37d64d70952ced5d38cd35 *perl-5.30.1.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.30.1.tar.xz -C /usr/src/perl     && rm perl-5.30.1.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && savedPackages="make netbase"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Sat, 28 Dec 2019 07:23:43 GMT
WORKDIR /
# Sat, 28 Dec 2019 07:23:44 GMT
CMD ["perl5.30.1" "-de0"]
```

-	Layers:
	-	`sha256:9498763e47873a85a1a6b3ba1f12b6936fcd769bb6b0d094c36c0dd6435bb902`  
		Last Modified: Sat, 28 Dec 2019 04:46:38 GMT  
		Size: 22.4 MB (22380154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c53537d56be40007ba4306f74906ebb06a1125a227357daa5db10d236fad31e`  
		Last Modified: Sat, 28 Dec 2019 08:56:34 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c8d3e2e89dcd0122774abd61b47215b53ed8f836d14460e711559d4e694ccc8`  
		Last Modified: Sat, 28 Dec 2019 08:56:37 GMT  
		Size: 14.8 MB (14796044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
