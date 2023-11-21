## `perl:slim-buster`

```console
$ docker pull perl@sha256:c42d7e2508787e91d5c5f60613cc86e07e836375e56b2fc2bcb4e0606dfeac52
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `perl:slim-buster` - linux; amd64

```console
$ docker pull perl@sha256:700b89be0f0403169414ba3276b1fcb1c3f4ffb1a14fc5a5846747bf997439c4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.5 MB (54509139 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52e9340b0e5c3773e847d6ec68e096b67c4283bc4c55d2cf3023cb4dc5d21532`
-	Default Command: `["perl5.38.0","-de0"]`

```dockerfile
# Tue, 21 Nov 2023 05:22:20 GMT
ADD file:7672eb709be933bb0edec47b8141cd2ebff266a770dfae1278205f7cee43c71a in / 
# Tue, 21 Nov 2023 05:22:20 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 06:26:09 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Tue, 21 Nov 2023 06:26:09 GMT
WORKDIR /usr/src/perl
# Tue, 21 Nov 2023 06:31:37 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        zlib1g-dev        xz-utils        libssl-dev     && curl -fL https://www.cpan.org/src/5.0/perl-5.38.0.tar.xz -o perl-5.38.0.tar.xz     && echo 'eca551caec3bc549a4e590c0015003790bdd1a604ffe19cc78ee631d51f7072e *perl-5.38.0.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.38.0.tar.xz -C /usr/src/perl     && rm perl-5.38.0.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && savedPackages="ca-certificates make netbase zlib1g-dev libssl-dev"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Tue, 21 Nov 2023 06:31:38 GMT
WORKDIR /usr/src/app
# Tue, 21 Nov 2023 06:31:38 GMT
CMD ["perl5.38.0" "-de0"]
```

-	Layers:
	-	`sha256:0fc9206bc4affb32fe13185a20b8184271c753e9b7cb81484bf770054fc69737`  
		Last Modified: Tue, 21 Nov 2023 05:27:19 GMT  
		Size: 27.2 MB (27187457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1c9e6a0beb8102e6e4484da6fa9a020eabbf35207c975f5616538a4ac2801e0`  
		Last Modified: Tue, 21 Nov 2023 08:39:06 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c206c7364d9d4cbcf248638b2d44994ebd026528c23436a45bbdfbc9c7044ce`  
		Last Modified: Tue, 21 Nov 2023 08:39:11 GMT  
		Size: 27.3 MB (27321350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b87c14e8e20a264663148e2e6733453dd642dd2aba2ec86cc64f0b505385059`  
		Last Modified: Tue, 21 Nov 2023 08:39:06 GMT  
		Size: 165.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:slim-buster` - linux; arm variant v7

```console
$ docker pull perl@sha256:4fc3771f12407854184ec5bed3c63797d18493a45e7aa0e0075ad4171fd62e83
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.7 MB (46693669 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40780e54f32b70491082cff7b42462debe86b0fee1001b1260a20213db7ece60`
-	Default Command: `["perl5.38.0","-de0"]`

```dockerfile
# Tue, 21 Nov 2023 03:58:22 GMT
ADD file:407ef80699946b8a8560ae436dfc9ca6148067b3012c02b4cb4e54d6d0aca674 in / 
# Tue, 21 Nov 2023 03:58:22 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 04:29:54 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Tue, 21 Nov 2023 04:29:54 GMT
WORKDIR /usr/src/perl
# Tue, 21 Nov 2023 04:35:29 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        zlib1g-dev        xz-utils        libssl-dev     && curl -fL https://www.cpan.org/src/5.0/perl-5.38.0.tar.xz -o perl-5.38.0.tar.xz     && echo 'eca551caec3bc549a4e590c0015003790bdd1a604ffe19cc78ee631d51f7072e *perl-5.38.0.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.38.0.tar.xz -C /usr/src/perl     && rm perl-5.38.0.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && savedPackages="ca-certificates make netbase zlib1g-dev libssl-dev"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Tue, 21 Nov 2023 04:35:30 GMT
WORKDIR /usr/src/app
# Tue, 21 Nov 2023 04:35:30 GMT
CMD ["perl5.38.0" "-de0"]
```

-	Layers:
	-	`sha256:d0b016a8027330736e9ca5c23b846a6a9c1eb0a32da6459047c95d22e9544cb7`  
		Last Modified: Tue, 21 Nov 2023 04:03:19 GMT  
		Size: 22.8 MB (22795884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2377a08a131e111c9f41f7522692d2d8f4e545680a1ae58f37f4195d9cc4ec5d`  
		Last Modified: Tue, 21 Nov 2023 06:42:55 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d84ae6e9ae0e28688a6a7039c0ba50ad282c8e898511770a41dca5f29178ccd3`  
		Last Modified: Tue, 21 Nov 2023 06:43:02 GMT  
		Size: 23.9 MB (23897451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e9a4e28fd5e4c0744a61136f7602fa8f0b0456feb0a65dc2909b9e51cb98ef8`  
		Last Modified: Tue, 21 Nov 2023 06:42:55 GMT  
		Size: 165.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:slim-buster` - linux; arm64 variant v8

```console
$ docker pull perl@sha256:2e963343d4c53e6cf791257c3ec59e2a1f9aac0fe9771b0216b7c4aa0dbf4343
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.9 MB (51925914 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a21407ee28d315b1014cb51b65a6489ad5bc821b35b172e1b2ced821bbf92808`
-	Default Command: `["perl5.38.0","-de0"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:34 GMT
ADD file:475e94b9a8f65c7cd4d4156af31e83190240ff35d8038f3fa86ad124d4d5d299 in / 
# Tue, 21 Nov 2023 06:27:35 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 10:56:31 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Tue, 21 Nov 2023 10:56:31 GMT
WORKDIR /usr/src/perl
# Tue, 21 Nov 2023 11:01:01 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        zlib1g-dev        xz-utils        libssl-dev     && curl -fL https://www.cpan.org/src/5.0/perl-5.38.0.tar.xz -o perl-5.38.0.tar.xz     && echo 'eca551caec3bc549a4e590c0015003790bdd1a604ffe19cc78ee631d51f7072e *perl-5.38.0.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.38.0.tar.xz -C /usr/src/perl     && rm perl-5.38.0.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && savedPackages="ca-certificates make netbase zlib1g-dev libssl-dev"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Tue, 21 Nov 2023 11:01:02 GMT
WORKDIR /usr/src/app
# Tue, 21 Nov 2023 11:01:02 GMT
CMD ["perl5.38.0" "-de0"]
```

-	Layers:
	-	`sha256:78b429e3efdd9f2b163abf0bca6b1462a25b1c5eddc1dd47f5d3445c6413cfa1`  
		Last Modified: Tue, 21 Nov 2023 06:31:45 GMT  
		Size: 26.0 MB (25967796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68fccf93829b001397b5136fdd9e8ef61e2d213ceff6ef312977de53aa611c06`  
		Last Modified: Tue, 21 Nov 2023 13:51:02 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c9524b2b6f76b21d2a091e19c4f2f84c2491fa29d41da102f37b83da4f22076`  
		Last Modified: Tue, 21 Nov 2023 13:51:06 GMT  
		Size: 26.0 MB (25957784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f67f9417b6553ec97e40a0472440d9fc982410ec79c8113decb8cf543c8d9a62`  
		Last Modified: Tue, 21 Nov 2023 13:51:02 GMT  
		Size: 165.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:slim-buster` - linux; 386

```console
$ docker pull perl@sha256:b762c5cdceea179d20ae0bfeffb45cd562052c704383a1a2a12ca2e25aa0fe98
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.3 MB (59294490 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee27eb212a08d470b337ad936814a6b70411960b3932e6866c849c9e20d2b8ee`
-	Default Command: `["perl5.38.0","-de0"]`

```dockerfile
# Tue, 21 Nov 2023 04:40:37 GMT
ADD file:a04f70df2aa61b210935e80ad2a655ad282407ef0b8e8e0acf47479c73f64f95 in / 
# Tue, 21 Nov 2023 04:40:38 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 05:11:52 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Tue, 21 Nov 2023 05:11:52 GMT
WORKDIR /usr/src/perl
# Tue, 21 Nov 2023 05:21:41 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        zlib1g-dev        xz-utils        libssl-dev     && curl -fL https://www.cpan.org/src/5.0/perl-5.38.0.tar.xz -o perl-5.38.0.tar.xz     && echo 'eca551caec3bc549a4e590c0015003790bdd1a604ffe19cc78ee631d51f7072e *perl-5.38.0.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.38.0.tar.xz -C /usr/src/perl     && rm perl-5.38.0.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && savedPackages="ca-certificates make netbase zlib1g-dev libssl-dev"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Tue, 21 Nov 2023 05:21:42 GMT
WORKDIR /usr/src/app
# Tue, 21 Nov 2023 05:21:42 GMT
CMD ["perl5.38.0" "-de0"]
```

-	Layers:
	-	`sha256:071d917b80792914c4da1ecc1adf7e2503440a8c7a2a5508542e0850d9187060`  
		Last Modified: Tue, 21 Nov 2023 04:46:12 GMT  
		Size: 27.8 MB (27846916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ec5851faef42ba0487a82ae13df788da379aa99dc37d77640f32f0f4b91caf9`  
		Last Modified: Tue, 21 Nov 2023 09:10:06 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08dd2df578bc4f765a8f44c8ddfb162f17756ed131ab1962a1e91855c826eec1`  
		Last Modified: Tue, 21 Nov 2023 09:10:14 GMT  
		Size: 31.4 MB (31447243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3adacc2dd8c2141a70b6d00393446acd3a85532d8910ea1d72e5650bb76a8571`  
		Last Modified: Tue, 21 Nov 2023 09:10:06 GMT  
		Size: 164.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
