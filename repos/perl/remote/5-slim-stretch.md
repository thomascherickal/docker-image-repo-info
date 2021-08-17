## `perl:5-slim-stretch`

```console
$ docker pull perl@sha256:a1fa427a5933baa7ca7054d8bf11ea9753958aaec55d706ebe57ddd5224ab025
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `perl:5-slim-stretch` - linux; amd64

```console
$ docker pull perl@sha256:78a0e748d5fbe9923e3e3ac203b11336e710caff5693f9de4f096e8dfa39c53d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.1 MB (37119264 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b2d236fd5ef514ddbf97c0a30e854fb7a02d52df6e60665b31e2cde34e0158e`
-	Default Command: `["perl5.32.1","-de0"]`

```dockerfile
# Tue, 17 Aug 2021 01:26:09 GMT
ADD file:f6c4487fa1f7a4e17f5d88fd0c91031a6efc7fa210d363a1d43d8b0f3a8d1d03 in / 
# Tue, 17 Aug 2021 01:26:09 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 07:35:37 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Tue, 17 Aug 2021 07:35:37 GMT
COPY file:3744c5cc39cdbdcae10db09a1f0f399005a79f93c237b387a72ff5710cdd458c in /usr/src/perl/ 
# Tue, 17 Aug 2021 07:35:37 GMT
WORKDIR /usr/src/perl
# Tue, 17 Aug 2021 07:46:05 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        xz-utils     && curl -SL https://www.cpan.org/src/5.0/perl-5.32.1.tar.xz -o perl-5.32.1.tar.xz     && echo '57cc47c735c8300a8ce2fa0643507b44c4ae59012bfdad0121313db639e02309 *perl-5.32.1.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.32.1.tar.xz -C /usr/src/perl     && rm perl-5.32.1.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && savedPackages="make netbase"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Tue, 17 Aug 2021 07:46:06 GMT
WORKDIR /
# Tue, 17 Aug 2021 07:46:06 GMT
CMD ["perl5.32.1" "-de0"]
```

-	Layers:
	-	`sha256:33f99cea3b7da8c6e0143c9fd7590c6d56f7d310ddd59b11be4ad485ae4cab2a`  
		Last Modified: Tue, 17 Aug 2021 01:33:27 GMT  
		Size: 22.5 MB (22527748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:592c8623822118f8fb64fc3d5fb321633e4533621c4a07545f92fea712bf4663`  
		Last Modified: Tue, 17 Aug 2021 08:47:39 GMT  
		Size: 202.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:341521087085531e0091aa7e831880848c0a118d5bc6ae4f79659e4c5dd3f79b`  
		Last Modified: Tue, 17 Aug 2021 08:47:42 GMT  
		Size: 14.6 MB (14591314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:5-slim-stretch` - linux; arm variant v7

```console
$ docker pull perl@sha256:b1902e48a36214a35b1fee67dff33c75a4570ba56c33ca0e94c0d5608f55d926
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.0 MB (33047585 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53ab1e71d9957f45f36324f21fbc98cf8bfb70b6dee16f5f1235e21b5e12cc85`
-	Default Command: `["perl5.32.1","-de0"]`

```dockerfile
# Tue, 17 Aug 2021 02:19:36 GMT
ADD file:1719cfa11cf0f895b82719a2c082abb9f2d9b6dd6efc9e610e9732b97b31f56d in / 
# Tue, 17 Aug 2021 02:19:36 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 13:39:09 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Tue, 17 Aug 2021 13:39:10 GMT
COPY file:3744c5cc39cdbdcae10db09a1f0f399005a79f93c237b387a72ff5710cdd458c in /usr/src/perl/ 
# Tue, 17 Aug 2021 13:39:10 GMT
WORKDIR /usr/src/perl
# Tue, 17 Aug 2021 13:51:11 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        xz-utils     && curl -SL https://www.cpan.org/src/5.0/perl-5.32.1.tar.xz -o perl-5.32.1.tar.xz     && echo '57cc47c735c8300a8ce2fa0643507b44c4ae59012bfdad0121313db639e02309 *perl-5.32.1.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.32.1.tar.xz -C /usr/src/perl     && rm perl-5.32.1.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && savedPackages="make netbase"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Tue, 17 Aug 2021 13:51:12 GMT
WORKDIR /
# Tue, 17 Aug 2021 13:51:12 GMT
CMD ["perl5.32.1" "-de0"]
```

-	Layers:
	-	`sha256:d1f994b3d26e717ce6c4ff9f7b5af7dbc4a4c831977d207f3ab47f213a8287e4`  
		Last Modified: Tue, 17 Aug 2021 02:36:57 GMT  
		Size: 19.3 MB (19316532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c17bf3a7e0442e2511baf025734f44fd5411cb3be483868b3de30dfc15163b14`  
		Last Modified: Tue, 17 Aug 2021 15:11:34 GMT  
		Size: 204.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9192a67f19c28f1263fa4e353ad33e3ab0e42bb43f1f50e021592c2c11ee97cc`  
		Last Modified: Tue, 17 Aug 2021 15:11:46 GMT  
		Size: 13.7 MB (13730849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:5-slim-stretch` - linux; arm64 variant v8

```console
$ docker pull perl@sha256:e5d0fdc9ab5fb5fec4a64391674bb715bd0bf39a10495f0aef4f1d9297d2304d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34793567 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3697cde7c8a77e1553603cb4e91e54788a600dd50ed482366864cb59c798d358`
-	Default Command: `["perl5.32.1","-de0"]`

```dockerfile
# Tue, 17 Aug 2021 01:48:32 GMT
ADD file:5cd26935234cc0540158a144066c0341b46a0caeb0a80db0355eeb8cfaf4fc0d in / 
# Tue, 17 Aug 2021 01:48:32 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 06:42:41 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Tue, 17 Aug 2021 06:42:41 GMT
COPY file:3744c5cc39cdbdcae10db09a1f0f399005a79f93c237b387a72ff5710cdd458c in /usr/src/perl/ 
# Tue, 17 Aug 2021 06:42:41 GMT
WORKDIR /usr/src/perl
# Tue, 17 Aug 2021 06:48:49 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        xz-utils     && curl -SL https://www.cpan.org/src/5.0/perl-5.32.1.tar.xz -o perl-5.32.1.tar.xz     && echo '57cc47c735c8300a8ce2fa0643507b44c4ae59012bfdad0121313db639e02309 *perl-5.32.1.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.32.1.tar.xz -C /usr/src/perl     && rm perl-5.32.1.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && savedPackages="make netbase"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Tue, 17 Aug 2021 06:48:49 GMT
WORKDIR /
# Tue, 17 Aug 2021 06:48:49 GMT
CMD ["perl5.32.1" "-de0"]
```

-	Layers:
	-	`sha256:f862659192cd149f96ede75854bd3ebf59937831d3e4103087ae62df34ef1a29`  
		Last Modified: Tue, 17 Aug 2021 01:58:00 GMT  
		Size: 20.4 MB (20389447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f022682a09a1a1b7dd8ae32b4afcdb0c8e7d7e06e54179ff87e5661f1b6537f`  
		Last Modified: Tue, 17 Aug 2021 07:32:56 GMT  
		Size: 202.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24c0fcc785d342fa2f06a871c13309072a0e02944556c45db5e1bc907e04ad6f`  
		Last Modified: Tue, 17 Aug 2021 07:32:59 GMT  
		Size: 14.4 MB (14403918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:5-slim-stretch` - linux; 386

```console
$ docker pull perl@sha256:d749ae62d9f73fd0253fd41d2e4800556edba286564ee7fd861fda2067b2f725
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.2 MB (37244803 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38386c06789e145a3366641806f49f1571a49eba83d0e9bb05ac2bbb7ae97a4a`
-	Default Command: `["perl5.32.1","-de0"]`

```dockerfile
# Tue, 17 Aug 2021 01:44:04 GMT
ADD file:c25cbb547d8495c7a68777f385b60687a1999dbc12ccac3313d2611ac5bd4eac in / 
# Tue, 17 Aug 2021 01:44:05 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 14:36:15 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Tue, 17 Aug 2021 14:36:16 GMT
COPY file:3744c5cc39cdbdcae10db09a1f0f399005a79f93c237b387a72ff5710cdd458c in /usr/src/perl/ 
# Tue, 17 Aug 2021 14:36:16 GMT
WORKDIR /usr/src/perl
# Tue, 17 Aug 2021 14:44:45 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        xz-utils     && curl -SL https://www.cpan.org/src/5.0/perl-5.32.1.tar.xz -o perl-5.32.1.tar.xz     && echo '57cc47c735c8300a8ce2fa0643507b44c4ae59012bfdad0121313db639e02309 *perl-5.32.1.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.32.1.tar.xz -C /usr/src/perl     && rm perl-5.32.1.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && savedPackages="make netbase"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Tue, 17 Aug 2021 14:44:45 GMT
WORKDIR /
# Tue, 17 Aug 2021 14:44:45 GMT
CMD ["perl5.32.1" "-de0"]
```

-	Layers:
	-	`sha256:4b870a82a4c75e96837d71f0160a6a128bf17b0ef8630f8a78c1a713ecbe8e92`  
		Last Modified: Tue, 17 Aug 2021 01:55:08 GMT  
		Size: 23.2 MB (23156808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39b3ad02cfad0720f0f9ba14c9483b87d83f67cffddd61f95479f1927e265649`  
		Last Modified: Tue, 17 Aug 2021 16:55:24 GMT  
		Size: 202.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e710cdf29ff784ee008a3b1d147f465ccc3396d007c596094dc8cb4c5852dde`  
		Last Modified: Tue, 17 Aug 2021 16:55:30 GMT  
		Size: 14.1 MB (14087793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
