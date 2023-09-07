## `perl:5-slim-threaded-bullseye`

```console
$ docker pull perl@sha256:14cd49cfe03829153d27015f3444adb5c544c6cc10ae65efc0536124b248b2cb
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

### `perl:5-slim-threaded-bullseye` - linux; amd64

```console
$ docker pull perl@sha256:9eb22e62c08e52d5750016159fd417cf899532ea036b76d73440fe2ca2e4d8d2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.0 MB (56037602 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56ba789a32a3b62a2bc8de05fb71fa64b55705be4b8f88e6dea48e4eff33eb97`
-	Default Command: `["perl5.38.0","-de0"]`

```dockerfile
# Wed, 16 Aug 2023 01:00:09 GMT
ADD file:2d91c2e03d02bfa16fe4f766d851b351d93d33f84751ad96c985e64ea024ec28 in / 
# Wed, 16 Aug 2023 01:00:09 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 11:07:19 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Wed, 16 Aug 2023 11:07:20 GMT
WORKDIR /usr/src/perl
# Wed, 16 Aug 2023 11:48:35 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        zlib1g-dev        xz-utils        libssl-dev     && curl -fL https://www.cpan.org/src/5.0/perl-5.38.0.tar.xz -o perl-5.38.0.tar.xz     && echo 'eca551caec3bc549a4e590c0015003790bdd1a604ffe19cc78ee631d51f7072e *perl-5.38.0.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.38.0.tar.xz -C /usr/src/perl     && rm perl-5.38.0.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && savedPackages="ca-certificates make netbase zlib1g-dev libssl-dev"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Wed, 16 Aug 2023 11:48:35 GMT
WORKDIR /usr/src/app
# Wed, 16 Aug 2023 11:48:35 GMT
CMD ["perl5.38.0" "-de0"]
```

-	Layers:
	-	`sha256:14726c8f78342865030f97a8d3492e2d1a68fbd22778f9a31dc6be4b4f12a9bc`  
		Last Modified: Wed, 16 Aug 2023 01:05:12 GMT  
		Size: 31.4 MB (31417678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:548dbb5c0b7fb4d0a2d06a37391a890125d224209c876dc6d94d8b1767134c1d`  
		Last Modified: Wed, 16 Aug 2023 14:38:04 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15b1956305fe92009702ab5a4f9de70dd8b6d7d62569bb11b782ec7314ac0ccc`  
		Last Modified: Wed, 16 Aug 2023 14:40:15 GMT  
		Size: 24.6 MB (24619590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd5fd5ed99f76a77cd7a45a83f871a8f4ed2c57e605e6e1b3b3674640e4dc569`  
		Last Modified: Wed, 16 Aug 2023 14:40:11 GMT  
		Size: 165.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:5-slim-threaded-bullseye` - linux; arm variant v5

```console
$ docker pull perl@sha256:b66cd5b62cc2760962719a1b55ae4dd41d76fe68f317c1c972f0f8a33526cca2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.5 MB (51526703 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2b50882234d8e6b3d47f31e5bd08d7b2327a7ecf4a2dad62404cfc9eb10a527`
-	Default Command: `["perl5.38.0","-de0"]`

```dockerfile
# Tue, 15 Aug 2023 23:48:48 GMT
ADD file:3b3acc24aa6c4e5b8cfc525e3f293f633aace75304eaf7d1615d63233866cd66 in / 
# Tue, 15 Aug 2023 23:48:48 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 00:57:35 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Wed, 16 Aug 2023 00:57:35 GMT
WORKDIR /usr/src/perl
# Wed, 16 Aug 2023 01:15:56 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        zlib1g-dev        xz-utils        libssl-dev     && curl -fL https://www.cpan.org/src/5.0/perl-5.38.0.tar.xz -o perl-5.38.0.tar.xz     && echo 'eca551caec3bc549a4e590c0015003790bdd1a604ffe19cc78ee631d51f7072e *perl-5.38.0.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.38.0.tar.xz -C /usr/src/perl     && rm perl-5.38.0.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && savedPackages="ca-certificates make netbase zlib1g-dev libssl-dev"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Wed, 16 Aug 2023 01:15:57 GMT
WORKDIR /usr/src/app
# Wed, 16 Aug 2023 01:15:57 GMT
CMD ["perl5.38.0" "-de0"]
```

-	Layers:
	-	`sha256:a1de04ebd80600d150cca674fb676a51a44730027c798fad7415210924b7fed2`  
		Last Modified: Tue, 15 Aug 2023 23:52:15 GMT  
		Size: 28.9 MB (28919119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8926775f7fc986a64e21012cdfd9c1840e9fb97d56c4953ca9129dc7ad9dc8c`  
		Last Modified: Wed, 16 Aug 2023 02:31:56 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8feff727b7a00a25a62ed11ad726dafa4c535a287985f501266304a94ab46f74`  
		Last Modified: Wed, 16 Aug 2023 02:32:40 GMT  
		Size: 22.6 MB (22607252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf673acc742ee8497b7df8bd753450b40ce9c181b5203b6b3653bcfa854474f4`  
		Last Modified: Wed, 16 Aug 2023 02:32:34 GMT  
		Size: 165.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:5-slim-threaded-bullseye` - linux; arm variant v7

```console
$ docker pull perl@sha256:8a511d3404e1a8c233710e849327a6ad5832478306d6cfbaf5a4b31733c8326b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.6 MB (48580458 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90db12abdeacf00779d4fbd1837ec7cd55a40dae3c302f5f58503f9357ee5228`
-	Default Command: `["perl5.38.0","-de0"]`

```dockerfile
# Wed, 16 Aug 2023 00:17:33 GMT
ADD file:d9383f6a4370dbf4af8e05edac181465a410899022cf1788f9001a976b9beecd in / 
# Wed, 16 Aug 2023 00:17:33 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 08:19:23 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Wed, 16 Aug 2023 08:19:23 GMT
WORKDIR /usr/src/perl
# Wed, 16 Aug 2023 09:01:44 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        zlib1g-dev        xz-utils        libssl-dev     && curl -fL https://www.cpan.org/src/5.0/perl-5.38.0.tar.xz -o perl-5.38.0.tar.xz     && echo 'eca551caec3bc549a4e590c0015003790bdd1a604ffe19cc78ee631d51f7072e *perl-5.38.0.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.38.0.tar.xz -C /usr/src/perl     && rm perl-5.38.0.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && savedPackages="ca-certificates make netbase zlib1g-dev libssl-dev"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Wed, 16 Aug 2023 09:01:45 GMT
WORKDIR /usr/src/app
# Wed, 16 Aug 2023 09:01:45 GMT
CMD ["perl5.38.0" "-de0"]
```

-	Layers:
	-	`sha256:66971a88ba9c0b0ac6503475f1bc4981010269bdba2638318b63c625ee44cd79`  
		Last Modified: Wed, 16 Aug 2023 00:22:09 GMT  
		Size: 26.6 MB (26578637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e938d7eac9b1a5ca7b64b214f271066d9b2ae0beb20bb63c8b3ee8137375ac21`  
		Last Modified: Wed, 16 Aug 2023 11:56:43 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80d7f4acc5add97176d862c22d238739487a1ded6a40b09d744b6ebef9d8069a`  
		Last Modified: Wed, 16 Aug 2023 11:58:58 GMT  
		Size: 22.0 MB (22001488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d27ac3cf33c6bebdbb1e58db9793f4fcb530d4df41a8469d470923565cf874f`  
		Last Modified: Wed, 16 Aug 2023 11:58:53 GMT  
		Size: 165.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:5-slim-threaded-bullseye` - linux; arm64 variant v8

```console
$ docker pull perl@sha256:08b2434f9c26cbe93faa29cfb525dcb501c980dd91e9a82f8bedb63efcbac1a7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.8 MB (53798479 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b69f3090c00e4a5c02c8b894c3aff9d468c64033ed67e0e01df35f079f1d959`
-	Default Command: `["perl5.38.0","-de0"]`

```dockerfile
# Thu, 07 Sep 2023 00:39:53 GMT
ADD file:abd1ad48ae3ebec7a6ecc8ce3016c25be2afcbaedfcb904bc89b1ce59400aef0 in / 
# Thu, 07 Sep 2023 00:39:54 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 02:37:13 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Thu, 07 Sep 2023 02:37:13 GMT
WORKDIR /usr/src/perl
# Thu, 07 Sep 2023 02:56:46 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        zlib1g-dev        xz-utils        libssl-dev     && curl -fL https://www.cpan.org/src/5.0/perl-5.38.0.tar.xz -o perl-5.38.0.tar.xz     && echo 'eca551caec3bc549a4e590c0015003790bdd1a604ffe19cc78ee631d51f7072e *perl-5.38.0.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.38.0.tar.xz -C /usr/src/perl     && rm perl-5.38.0.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && savedPackages="ca-certificates make netbase zlib1g-dev libssl-dev"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Thu, 07 Sep 2023 02:56:47 GMT
WORKDIR /usr/src/app
# Thu, 07 Sep 2023 02:56:47 GMT
CMD ["perl5.38.0" "-de0"]
```

-	Layers:
	-	`sha256:f96ab15157043879c2ff23e0556e798eba6a6ff3d7fd5d1384de223bb9f66f1d`  
		Last Modified: Thu, 07 Sep 2023 00:43:41 GMT  
		Size: 30.1 MB (30062903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fb806f7177fe03abaaba25129ae0538132fc7a37236c086784b39c9b05db0f0`  
		Last Modified: Thu, 07 Sep 2023 04:12:25 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc333b8afb0910abc4646235408f4e008127867d462137936254254bd85b662f`  
		Last Modified: Thu, 07 Sep 2023 04:13:37 GMT  
		Size: 23.7 MB (23735244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e881bb48774f5e386903c7acc4444ad58758136fa42b16c7be6c053f7b4032e1`  
		Last Modified: Thu, 07 Sep 2023 04:13:33 GMT  
		Size: 165.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:5-slim-threaded-bullseye` - linux; 386

```console
$ docker pull perl@sha256:e4f93c8f302f8c7c8671db952760eb5cdc4d8426980b25306c5d03e15102bf5d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.5 MB (58477489 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:edf98bb969152a52676891e8a808de865f4295113dd0f1a1a8c117af7f9b4f52`
-	Default Command: `["perl5.38.0","-de0"]`

```dockerfile
# Tue, 15 Aug 2023 23:39:23 GMT
ADD file:fa0abd37650f364ecdf67d446b3fe2ce58fac1ad53beb5263b4f230fad58931e in / 
# Tue, 15 Aug 2023 23:39:23 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 10:25:07 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Wed, 16 Aug 2023 10:25:07 GMT
WORKDIR /usr/src/perl
# Wed, 16 Aug 2023 11:36:22 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        zlib1g-dev        xz-utils        libssl-dev     && curl -fL https://www.cpan.org/src/5.0/perl-5.38.0.tar.xz -o perl-5.38.0.tar.xz     && echo 'eca551caec3bc549a4e590c0015003790bdd1a604ffe19cc78ee631d51f7072e *perl-5.38.0.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.38.0.tar.xz -C /usr/src/perl     && rm perl-5.38.0.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && savedPackages="ca-certificates make netbase zlib1g-dev libssl-dev"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Wed, 16 Aug 2023 11:36:23 GMT
WORKDIR /usr/src/app
# Wed, 16 Aug 2023 11:36:23 GMT
CMD ["perl5.38.0" "-de0"]
```

-	Layers:
	-	`sha256:f6edc1df8dbb4cb778380e62ce1680ea580c1b213c048642bb7adaafa4cc6d73`  
		Last Modified: Tue, 15 Aug 2023 23:44:11 GMT  
		Size: 32.4 MB (32397200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21a60367c2cd098aad894a139009b8d345a51fb686a3abc4b1950a89ce326b3e`  
		Last Modified: Wed, 16 Aug 2023 16:29:59 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce3821a30fffc035a402c34d0ea4b925de13d4be69a66bde839faa8eee5dabdd`  
		Last Modified: Wed, 16 Aug 2023 16:32:28 GMT  
		Size: 26.1 MB (26079955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d490337ff218d22beec9cc47b39f3dcfb412433dbf8ee6c597b64cde95a2e5a`  
		Last Modified: Wed, 16 Aug 2023 16:32:21 GMT  
		Size: 165.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:5-slim-threaded-bullseye` - linux; mips64le

```console
$ docker pull perl@sha256:b92dca1d7bed2a17e3cb8b28ffab35a5c62bf0ec8b9bab593d12073aff32abb6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.0 MB (52960610 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06b123ec9dd05a31698f1a2bad744bee16261cc8422c4b758760c8a9e0c4df0a`
-	Default Command: `["perl5.38.0","-de0"]`

```dockerfile
# Wed, 16 Aug 2023 00:09:57 GMT
ADD file:55aae3aeab6425dfb2efd03d619656959a01f591b2386ab3d046a6bd69624530 in / 
# Wed, 16 Aug 2023 00:10:01 GMT
CMD ["bash"]
# Thu, 17 Aug 2023 15:51:56 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Thu, 17 Aug 2023 15:51:59 GMT
WORKDIR /usr/src/perl
# Thu, 17 Aug 2023 17:05:09 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        zlib1g-dev        xz-utils        libssl-dev     && curl -fL https://www.cpan.org/src/5.0/perl-5.38.0.tar.xz -o perl-5.38.0.tar.xz     && echo 'eca551caec3bc549a4e590c0015003790bdd1a604ffe19cc78ee631d51f7072e *perl-5.38.0.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.38.0.tar.xz -C /usr/src/perl     && rm perl-5.38.0.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && savedPackages="ca-certificates make netbase zlib1g-dev libssl-dev"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Thu, 17 Aug 2023 17:05:13 GMT
WORKDIR /usr/src/app
# Thu, 17 Aug 2023 17:05:16 GMT
CMD ["perl5.38.0" "-de0"]
```

-	Layers:
	-	`sha256:7ef62af8109683ee92b199cf210a6e6134ce588b610d2a6b93fc467d34648300`  
		Last Modified: Wed, 16 Aug 2023 00:20:59 GMT  
		Size: 29.6 MB (29634580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85134e18d02ed5aa0c99f0a513d0199c25586a72f349abfa75a4d6b5d49410e0`  
		Last Modified: Thu, 17 Aug 2023 21:51:41 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:165d374a59b95c5f479c4e349cbdb922ddf4722a69d9c74a0f1706ca2aa5c838`  
		Last Modified: Thu, 17 Aug 2023 21:53:07 GMT  
		Size: 23.3 MB (23325765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2baa8e67739d143221b9f0a3fb79bda3f4a11733c532372d8e4c25c84a9c52a8`  
		Last Modified: Thu, 17 Aug 2023 21:52:47 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:5-slim-threaded-bullseye` - linux; ppc64le

```console
$ docker pull perl@sha256:9bfb41e2f9ff4e6bd3763c8e0f212b9c7367ae1031c68b2c73bc8d052840d48e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.2 MB (60194862 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9d0b7022819f45b3e0633488c2fcebddbdc427956f16b850128d9c55a9ebb53`
-	Default Command: `["perl5.38.0","-de0"]`

```dockerfile
# Wed, 16 Aug 2023 01:10:12 GMT
ADD file:eeb766a3bb0461f0baa2425cfd43628994c064bd728f51f1b8df659a4bd2f489 in / 
# Wed, 16 Aug 2023 01:10:14 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 09:31:39 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Wed, 16 Aug 2023 09:31:39 GMT
WORKDIR /usr/src/perl
# Wed, 16 Aug 2023 09:59:53 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        zlib1g-dev        xz-utils        libssl-dev     && curl -fL https://www.cpan.org/src/5.0/perl-5.38.0.tar.xz -o perl-5.38.0.tar.xz     && echo 'eca551caec3bc549a4e590c0015003790bdd1a604ffe19cc78ee631d51f7072e *perl-5.38.0.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.38.0.tar.xz -C /usr/src/perl     && rm perl-5.38.0.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && savedPackages="ca-certificates make netbase zlib1g-dev libssl-dev"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Wed, 16 Aug 2023 09:59:56 GMT
WORKDIR /usr/src/app
# Wed, 16 Aug 2023 09:59:56 GMT
CMD ["perl5.38.0" "-de0"]
```

-	Layers:
	-	`sha256:dacf4195c8a0403fd11459739bf9dc9be427261bf5e0bedb49e18d1498cf7c2e`  
		Last Modified: Wed, 16 Aug 2023 01:17:04 GMT  
		Size: 35.3 MB (35291067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd70aeab85e64935ea308ccc6f877129765319cf8e28a942b13b9ea9be755a62`  
		Last Modified: Wed, 16 Aug 2023 11:47:28 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93f5f99e11715f11b2b45be05277a1e2f53f73e61bf69d8773e5cc2724fd4251`  
		Last Modified: Wed, 16 Aug 2023 11:48:33 GMT  
		Size: 24.9 MB (24903461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d233eb60d28cba79456cf93a14bf4d4791f35ff0701a638a35785ba2f289048`  
		Last Modified: Wed, 16 Aug 2023 11:48:25 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:5-slim-threaded-bullseye` - linux; s390x

```console
$ docker pull perl@sha256:8d5679e155f10aaf3d93f20046c0cbefbec1e2dc776d3fa7274f75e44a4a65ec
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.5 MB (53485961 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e72039cf1008a2c419e30717b3cd6ea6b4381b1edf82c650a9c21cabb78fbc9`
-	Default Command: `["perl5.38.0","-de0"]`

```dockerfile
# Thu, 07 Sep 2023 00:44:33 GMT
ADD file:fb2f216acd6d0ecaf48e8d5dd7e3cdb5d1f51d414f2011ed318cb494f96d89ca in / 
# Thu, 07 Sep 2023 00:44:37 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 02:49:15 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Thu, 07 Sep 2023 02:49:16 GMT
WORKDIR /usr/src/perl
# Thu, 07 Sep 2023 03:09:10 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        zlib1g-dev        xz-utils        libssl-dev     && curl -fL https://www.cpan.org/src/5.0/perl-5.38.0.tar.xz -o perl-5.38.0.tar.xz     && echo 'eca551caec3bc549a4e590c0015003790bdd1a604ffe19cc78ee631d51f7072e *perl-5.38.0.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.38.0.tar.xz -C /usr/src/perl     && rm perl-5.38.0.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && savedPackages="ca-certificates make netbase zlib1g-dev libssl-dev"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Thu, 07 Sep 2023 03:09:12 GMT
WORKDIR /usr/src/app
# Thu, 07 Sep 2023 03:09:12 GMT
CMD ["perl5.38.0" "-de0"]
```

-	Layers:
	-	`sha256:c9501ad9402d64e6c612fa1bb94f16df51188e681dc1f28c603a6109f06f22d7`  
		Last Modified: Thu, 07 Sep 2023 00:50:10 GMT  
		Size: 29.7 MB (29652801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9414166169c76b86f17fade3e1dc61de021cc22e4d2847b07bc1d9aeb1b0288c`  
		Last Modified: Thu, 07 Sep 2023 04:25:07 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3d5e76f165cec98fec4d64e95603edfb5be2992eea78f57b0f6f68a444e0994`  
		Last Modified: Thu, 07 Sep 2023 04:25:38 GMT  
		Size: 23.8 MB (23832829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a53b0cc06f2c8eb197198a9138189ef14afa2627049bd5f79a8195fe294575f7`  
		Last Modified: Thu, 07 Sep 2023 04:25:34 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
