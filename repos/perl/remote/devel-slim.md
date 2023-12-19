## `perl:devel-slim`

```console
$ docker pull perl@sha256:f1305ff383d64d7858bc7eeec5d4c629c3af94c80d182fcd67ab4b9541c81137
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

### `perl:devel-slim` - linux; amd64

```console
$ docker pull perl@sha256:3b2dba148e60937d10a96d90a706943550fbc4967e5331ca7e8a0853ddcc9e6c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.8 MB (57794656 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d11e0412e49ae91b996119e741cbadea246b9d54892a40643eda46a7c54bfc74`
-	Default Command: `["perl5.39.5","-de0"]`

```dockerfile
# Tue, 19 Dec 2023 01:20:27 GMT
ADD file:ac3cd70031d35e46d86b876934946ffc8756de4de065fbc926dce642dac07ff3 in / 
# Tue, 19 Dec 2023 01:20:28 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 08:35:45 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Tue, 19 Dec 2023 08:35:45 GMT
WORKDIR /usr/src/perl
# Tue, 19 Dec 2023 11:49:37 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        zlib1g-dev        xz-utils        libssl-dev     && curl -fL https://www.cpan.org/src/5.0/perl-5.39.5.tar.xz -o perl-5.39.5.tar.xz     && echo '4048cf0065f347a03ec85e989631a64e03ba9c9ccbc8f2a35153cad07fe21930 *perl-5.39.5.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.39.5.tar.xz -C /usr/src/perl     && rm perl-5.39.5.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local -Dusedevel -Dversiononly=undef -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && savedPackages="ca-certificates make netbase zlib1g-dev libssl-dev"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Tue, 19 Dec 2023 11:49:37 GMT
WORKDIR /usr/src/app
# Tue, 19 Dec 2023 11:49:37 GMT
CMD ["perl5.39.5" "-de0"]
```

-	Layers:
	-	`sha256:af107e978371b6cd6339127a05502c5eacd1e6b0e9eb7b2f4aa7b6fc87e2dd81`  
		Last Modified: Tue, 19 Dec 2023 01:24:59 GMT  
		Size: 29.1 MB (29125963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a651c61b3351f670ffb3682b106f2a5bdd1760ffbc26800fb736ea1a2e33edb6`  
		Last Modified: Tue, 19 Dec 2023 12:24:22 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d51a426cdc56c553bc400350a5903a2ced90695497b749d7dfab1d3104ddd752`  
		Last Modified: Tue, 19 Dec 2023 12:32:54 GMT  
		Size: 28.7 MB (28668358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ce1b808226d97dd2803d00a583f976aebac79713f9b544068bddaeaf8f67ed2`  
		Last Modified: Tue, 19 Dec 2023 12:32:49 GMT  
		Size: 165.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:devel-slim` - linux; arm variant v5

```console
$ docker pull perl@sha256:68f48d153cc8031b535ea894406c6c238a70d606f76a1a8de85d2dcb56a099b2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.7 MB (52666389 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e82390f5f9bfc9b4edbd732a7c9b4c9a9c032c3575b7f13c265d0bffe21dab0`
-	Default Command: `["perl5.39.5","-de0"]`

```dockerfile
# Tue, 19 Dec 2023 01:55:22 GMT
ADD file:9503ab966c9dd707eeccc7c2f633bccc94c199f8714ec4ff2c8b54dde3dbabf9 in / 
# Tue, 19 Dec 2023 01:55:22 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 05:50:47 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Tue, 19 Dec 2023 05:50:47 GMT
WORKDIR /usr/src/perl
# Tue, 19 Dec 2023 08:03:52 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        zlib1g-dev        xz-utils        libssl-dev     && curl -fL https://www.cpan.org/src/5.0/perl-5.39.5.tar.xz -o perl-5.39.5.tar.xz     && echo '4048cf0065f347a03ec85e989631a64e03ba9c9ccbc8f2a35153cad07fe21930 *perl-5.39.5.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.39.5.tar.xz -C /usr/src/perl     && rm perl-5.39.5.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local -Dusedevel -Dversiononly=undef -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && savedPackages="ca-certificates make netbase zlib1g-dev libssl-dev"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Tue, 19 Dec 2023 08:03:53 GMT
WORKDIR /usr/src/app
# Tue, 19 Dec 2023 08:03:53 GMT
CMD ["perl5.39.5" "-de0"]
```

-	Layers:
	-	`sha256:1ae9a2844c8c70942d2220553689b62e841cc706d77284fbfedbd770080fd699`  
		Last Modified: Tue, 19 Dec 2023 01:58:33 GMT  
		Size: 26.9 MB (26885440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2c20f375cd28a5a079f2c448b1e36f95a8b9161466b00e5488ef27bc6016971`  
		Last Modified: Tue, 19 Dec 2023 08:37:17 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aff395844b65466cab86026384084dc0a5e66cc84b6c961ea24054329955c968`  
		Last Modified: Tue, 19 Dec 2023 08:44:02 GMT  
		Size: 25.8 MB (25780615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be7acc697200ac22e3b829a0f2737a06b92a58616d5c8ce989aad1587d743d9b`  
		Last Modified: Tue, 19 Dec 2023 08:43:55 GMT  
		Size: 165.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:devel-slim` - linux; arm variant v7

```console
$ docker pull perl@sha256:ea99df69dcc670696b2fb59b408bed2a9b4d7e7e7549edb0eb66ef94b559a56d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.7 MB (49712505 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fbb10ea4d06129e61f7873c282526ff31e353c830cb2b54c1f7d358d24076588`
-	Default Command: `["perl5.39.5","-de0"]`

```dockerfile
# Tue, 19 Dec 2023 02:07:50 GMT
ADD file:aef112919e7924ad6da32181b1df5099cd692680c104118da3a24cd4dfe55a1d in / 
# Tue, 19 Dec 2023 02:07:50 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 02:55:02 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Tue, 19 Dec 2023 02:55:02 GMT
WORKDIR /usr/src/perl
# Tue, 19 Dec 2023 04:43:23 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        zlib1g-dev        xz-utils        libssl-dev     && curl -fL https://www.cpan.org/src/5.0/perl-5.39.5.tar.xz -o perl-5.39.5.tar.xz     && echo '4048cf0065f347a03ec85e989631a64e03ba9c9ccbc8f2a35153cad07fe21930 *perl-5.39.5.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.39.5.tar.xz -C /usr/src/perl     && rm perl-5.39.5.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local -Dusedevel -Dversiononly=undef -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && savedPackages="ca-certificates make netbase zlib1g-dev libssl-dev"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Tue, 19 Dec 2023 04:43:24 GMT
WORKDIR /usr/src/app
# Tue, 19 Dec 2023 04:43:24 GMT
CMD ["perl5.39.5" "-de0"]
```

-	Layers:
	-	`sha256:65ab19615c01a3b542f77fadb3bd27872b6a20cba3e9269fb951de36d8fa6805`  
		Last Modified: Tue, 19 Dec 2023 02:11:52 GMT  
		Size: 24.7 MB (24718157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37e75ffb7946479869c2df865c49429612111a6f8a18627575152f960da33e2c`  
		Last Modified: Tue, 19 Dec 2023 05:02:46 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6247337b39ab61adc896a11ab5ae9026138c06e6b6ca593c0ec3af1f0f391a33`  
		Last Modified: Tue, 19 Dec 2023 05:08:33 GMT  
		Size: 25.0 MB (24994015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f89abefe644a5d17fc39fb3e42b2c7158146ee524333aa9f6fcc4099a248a87c`  
		Last Modified: Tue, 19 Dec 2023 05:08:27 GMT  
		Size: 165.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:devel-slim` - linux; arm64 variant v8

```console
$ docker pull perl@sha256:d0be35f10d3a5dc13e4171503e23f8dd0a863e8676387d0c2c0293e2448b40f9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.6 MB (56612703 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d17f11dfce1d58bbdd3faff849cdf0695a93fb41104cc7be9fab04284bae566`
-	Default Command: `["perl5.39.5","-de0"]`

```dockerfile
# Tue, 19 Dec 2023 01:41:11 GMT
ADD file:262fd7bf0bc26e5d2a229fba52626e22b8a93beac29733acfc60e716c26e689d in / 
# Tue, 19 Dec 2023 01:41:11 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 07:49:40 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Tue, 19 Dec 2023 07:49:40 GMT
WORKDIR /usr/src/perl
# Tue, 19 Dec 2023 09:12:30 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        zlib1g-dev        xz-utils        libssl-dev     && curl -fL https://www.cpan.org/src/5.0/perl-5.39.5.tar.xz -o perl-5.39.5.tar.xz     && echo '4048cf0065f347a03ec85e989631a64e03ba9c9ccbc8f2a35153cad07fe21930 *perl-5.39.5.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.39.5.tar.xz -C /usr/src/perl     && rm perl-5.39.5.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local -Dusedevel -Dversiononly=undef -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && savedPackages="ca-certificates make netbase zlib1g-dev libssl-dev"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Tue, 19 Dec 2023 09:12:30 GMT
WORKDIR /usr/src/app
# Tue, 19 Dec 2023 09:12:30 GMT
CMD ["perl5.39.5" "-de0"]
```

-	Layers:
	-	`sha256:24e221e92a36ab5b0075dd156b4f2ff095532a9b0927946cf6070bb1bea208b8`  
		Last Modified: Tue, 19 Dec 2023 01:44:38 GMT  
		Size: 29.2 MB (29157269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e00d4f3e339e5678890c8ce5b88d61aaec1c52aedf5c1fc9fe42507c467666a`  
		Last Modified: Tue, 19 Dec 2023 09:28:33 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccfb663988c89c141a7c1326787a958b968e5ff7b6faf0c86824e883ff00c7b9`  
		Last Modified: Tue, 19 Dec 2023 09:33:13 GMT  
		Size: 27.5 MB (27455097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4055026d1c9db83ad0d2f87b18c2af590cd0c50ed83e15d5f75c9240793c0841`  
		Last Modified: Tue, 19 Dec 2023 09:33:09 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:devel-slim` - linux; 386

```console
$ docker pull perl@sha256:954f0988c2277de7b29078d3f0f110e63bcce990a08ba0700ce503843fe8208c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.8 MB (57828263 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d74724bdc662a526c233e50dfeaed236c640a0a0b9174c0bc6315a100031c1ad`
-	Default Command: `["perl5.39.5","-de0"]`

```dockerfile
# Tue, 21 Nov 2023 04:39:53 GMT
ADD file:930e1b9d85b6927c4d3046f7c75de2f3bfc6ec29100c314d0ab2b780ea30e962 in / 
# Tue, 21 Nov 2023 04:39:53 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 04:51:20 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Tue, 21 Nov 2023 04:51:20 GMT
WORKDIR /usr/src/perl
# Tue, 21 Nov 2023 08:11:34 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        zlib1g-dev        xz-utils        libssl-dev     && curl -fL https://www.cpan.org/src/5.0/perl-5.39.5.tar.xz -o perl-5.39.5.tar.xz     && echo '4048cf0065f347a03ec85e989631a64e03ba9c9ccbc8f2a35153cad07fe21930 *perl-5.39.5.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.39.5.tar.xz -C /usr/src/perl     && rm perl-5.39.5.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local -Dusedevel -Dversiononly=undef -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && savedPackages="ca-certificates make netbase zlib1g-dev libssl-dev"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Tue, 21 Nov 2023 08:11:35 GMT
WORKDIR /usr/src/app
# Tue, 21 Nov 2023 08:11:35 GMT
CMD ["perl5.39.5" "-de0"]
```

-	Layers:
	-	`sha256:c0734eabce8885d8904dbd11b77aa97c2d2b04bc8e2af9e89d47c4bda590dd8e`  
		Last Modified: Tue, 21 Nov 2023 04:44:34 GMT  
		Size: 30.2 MB (30164109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4259913184a6360dba5a8f1fed2b178b90662e8c6d557cc17e8d4e08e10dda13`  
		Last Modified: Tue, 21 Nov 2023 09:09:15 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c415278794012193d8dee543ddbcfc0ec81a041334a2dfd2a42a55ffb4a0c0bb`  
		Last Modified: Tue, 21 Nov 2023 09:15:38 GMT  
		Size: 27.7 MB (27663822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bc94500ff2ef42e4cb7ecef9aa79e766b8505a4fbaf222eb9bbb1dcb7e91b52`  
		Last Modified: Tue, 21 Nov 2023 09:15:31 GMT  
		Size: 165.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:devel-slim` - linux; mips64le

```console
$ docker pull perl@sha256:6f47fa2746bbea6cff2847c7749439ba617e8e516cad35e27a642a6771cbfe7e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.8 MB (55770345 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7072e0203b9fbe9610865dfc60a31fa3fde867f01d63e8fab90b79b066e34150`
-	Default Command: `["perl5.39.5","-de0"]`

```dockerfile
# Tue, 21 Nov 2023 04:09:50 GMT
ADD file:e093749192323dc72b60a8440ddba26c415586f618b5e107fa264ba5eb2ca7ba in / 
# Tue, 21 Nov 2023 04:09:54 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 04:30:16 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Tue, 21 Nov 2023 04:30:19 GMT
WORKDIR /usr/src/perl
# Tue, 21 Nov 2023 09:51:46 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        zlib1g-dev        xz-utils        libssl-dev     && curl -fL https://www.cpan.org/src/5.0/perl-5.39.5.tar.xz -o perl-5.39.5.tar.xz     && echo '4048cf0065f347a03ec85e989631a64e03ba9c9ccbc8f2a35153cad07fe21930 *perl-5.39.5.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.39.5.tar.xz -C /usr/src/perl     && rm perl-5.39.5.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local -Dusedevel -Dversiononly=undef -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && savedPackages="ca-certificates make netbase zlib1g-dev libssl-dev"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Tue, 21 Nov 2023 09:51:50 GMT
WORKDIR /usr/src/app
# Tue, 21 Nov 2023 09:51:53 GMT
CMD ["perl5.39.5" "-de0"]
```

-	Layers:
	-	`sha256:ebdff2138fee4a3ec27560ab1353dc51c12c2608ff721f5db3d24104872b702a`  
		Last Modified: Tue, 21 Nov 2023 04:20:35 GMT  
		Size: 29.1 MB (29141984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7fe96ade84a7d6c48a41c8eb073cdde6dc0c4d08b9b13d5bb9ca4dc9ef881a5`  
		Last Modified: Tue, 21 Nov 2023 12:00:36 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1780627303f0976f1c5c0c07cd4df6bce20b18739ebe481959ebc6f5b42e388f`  
		Last Modified: Tue, 21 Nov 2023 12:08:42 GMT  
		Size: 26.6 MB (26628094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83bbf08345fc6d28c92f9ec94c984fb63c640093959aebdac8efd211ace50dc7`  
		Last Modified: Tue, 21 Nov 2023 12:08:20 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:devel-slim` - linux; ppc64le

```console
$ docker pull perl@sha256:e4c9b0e2b7afbefc5c4ca015c23e116816c5e10403d57fbc8439fffcb94ad2a6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.3 MB (62341243 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4baaeee311f922ba20b86a27e4eaf4879857a71d772d4f5535c7116d8648b140`
-	Default Command: `["perl5.39.5","-de0"]`

```dockerfile
# Tue, 19 Dec 2023 01:21:50 GMT
ADD file:ca1db68689e0b0388337ba450ad2c8e79c159c6b78f5aa6d3ff2b89b8d7edc93 in / 
# Tue, 19 Dec 2023 01:21:51 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 02:02:17 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Tue, 19 Dec 2023 02:02:17 GMT
WORKDIR /usr/src/perl
# Tue, 19 Dec 2023 03:19:51 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        zlib1g-dev        xz-utils        libssl-dev     && curl -fL https://www.cpan.org/src/5.0/perl-5.39.5.tar.xz -o perl-5.39.5.tar.xz     && echo '4048cf0065f347a03ec85e989631a64e03ba9c9ccbc8f2a35153cad07fe21930 *perl-5.39.5.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.39.5.tar.xz -C /usr/src/perl     && rm perl-5.39.5.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local -Dusedevel -Dversiononly=undef -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && savedPackages="ca-certificates make netbase zlib1g-dev libssl-dev"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Tue, 19 Dec 2023 03:19:54 GMT
WORKDIR /usr/src/app
# Tue, 19 Dec 2023 03:19:55 GMT
CMD ["perl5.39.5" "-de0"]
```

-	Layers:
	-	`sha256:fc9b8f5eec3aa37ab3aace05165427479352f290d53904cea87dca6349633a09`  
		Last Modified: Tue, 19 Dec 2023 01:26:19 GMT  
		Size: 33.1 MB (33120558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6d2a1db67e9c3154495e7323af9c6baf9f9b922604a55dfceddcff734f1ac44`  
		Last Modified: Tue, 19 Dec 2023 03:42:08 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:057890330258d08a925154390af36311d5dbc05e4144a387bb4ab657faccd70f`  
		Last Modified: Tue, 19 Dec 2023 03:46:02 GMT  
		Size: 29.2 MB (29220351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a56f5b8ea632222d2153bf0aec5500f72fd14d9d3693a2dfebc22fcbb433593`  
		Last Modified: Tue, 19 Dec 2023 03:45:55 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:devel-slim` - linux; s390x

```console
$ docker pull perl@sha256:2a6ecd6dbecf8f94fa874cdaebfabc7225475db09c856f605737d95c0bc1953c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.7 MB (54699420 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16018c16300f177ce88e7e6307afb1353a90d57f45151489d8dad2962dc4befc`
-	Default Command: `["perl5.39.5","-de0"]`

```dockerfile
# Tue, 19 Dec 2023 01:42:37 GMT
ADD file:f06f12fa5a93afc3a79ac4371d24b0a471a5a1818cf34c1d90004c8f410914b9 in / 
# Tue, 19 Dec 2023 01:42:39 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 02:08:15 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Tue, 19 Dec 2023 02:08:15 GMT
WORKDIR /usr/src/perl
# Tue, 19 Dec 2023 03:21:53 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        zlib1g-dev        xz-utils        libssl-dev     && curl -fL https://www.cpan.org/src/5.0/perl-5.39.5.tar.xz -o perl-5.39.5.tar.xz     && echo '4048cf0065f347a03ec85e989631a64e03ba9c9ccbc8f2a35153cad07fe21930 *perl-5.39.5.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.39.5.tar.xz -C /usr/src/perl     && rm perl-5.39.5.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local -Dusedevel -Dversiononly=undef -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && savedPackages="ca-certificates make netbase zlib1g-dev libssl-dev"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Tue, 19 Dec 2023 03:21:57 GMT
WORKDIR /usr/src/app
# Tue, 19 Dec 2023 03:21:57 GMT
CMD ["perl5.39.5" "-de0"]
```

-	Layers:
	-	`sha256:bc6b1888979d3ceb063da848b2034e980e2c2613642159c1e856550b79aa620c`  
		Last Modified: Tue, 19 Dec 2023 01:47:38 GMT  
		Size: 27.5 MB (27491874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e806c55f1dec0922c7134d6527e6fc38b2b38a375f801278141bfeb4ed1582b6`  
		Last Modified: Tue, 19 Dec 2023 03:43:37 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:601f193a5d7e38d28ff9208d08355111a8e7927ccd1374d0f23f785818537a25`  
		Last Modified: Tue, 19 Dec 2023 03:46:18 GMT  
		Size: 27.2 MB (27207212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4dc3bd4606a78da34aa81b583e895689ad95d66642544b6827f6cd5cbe8b034`  
		Last Modified: Tue, 19 Dec 2023 03:46:13 GMT  
		Size: 165.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
