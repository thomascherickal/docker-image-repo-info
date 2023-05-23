## `perl:devel-slim-threaded-bullseye`

```console
$ docker pull perl@sha256:43cbbd8b685535ca2dd6c451c5f0bebafe99a4860b8b4326e52082ead06b005c
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

### `perl:devel-slim-threaded-bullseye` - linux; amd64

```console
$ docker pull perl@sha256:c6c8d9d60d26279f1801796e373376f22eca6fd92e82300d61c169d1d2814e31
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.0 MB (56022207 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12b52001fd71c47a988ebb94aae0ec0eb5aa312d518b446dad90f9dd95771f2a`
-	Default Command: `["perl5.37.11","-de0"]`

```dockerfile
# Tue, 02 May 2023 23:46:59 GMT
ADD file:a2378c1b12e95db69e24b9d347441678c6f23239292cce3c822b1524992b6ec4 in / 
# Tue, 02 May 2023 23:47:00 GMT
CMD ["bash"]
# Wed, 03 May 2023 13:09:34 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Wed, 03 May 2023 13:09:34 GMT
WORKDIR /usr/src/perl
# Wed, 03 May 2023 15:53:05 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        zlib1g-dev        xz-utils        libssl-dev     && curl -fL https://www.cpan.org/src/5.0/perl-5.37.11.tar.xz -o perl-5.37.11.tar.xz     && echo '3946b00266595ccc44df28275e2fbb7b86c1482934cbeab2780db304a75ffd58 *perl-5.37.11.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.37.11.tar.xz -C /usr/src/perl     && rm perl-5.37.11.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local -Dusedevel -Dversiononly=undef -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7046.tar.gz     && echo '3e8c9d9b44a7348f9acc917163dbfc15bd5ea72501492cea3a35b346440ff862 *App-cpanminus-1.7046.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7046.tar.gz && cd App-cpanminus-1.7046 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && savedPackages="ca-certificates make netbase zlib1g-dev libssl-dev"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7046* /tmp/*     && cpanm --version && cpm --version
# Wed, 03 May 2023 15:53:05 GMT
WORKDIR /
# Wed, 03 May 2023 15:53:06 GMT
CMD ["perl5.37.11" "-de0"]
```

-	Layers:
	-	`sha256:9e3ea8720c6de96cc9ad544dddc695a3ab73f5581c5d954e0504cc4f80fb5e5c`  
		Last Modified: Tue, 02 May 2023 23:50:22 GMT  
		Size: 31.4 MB (31403516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef0c2867dc1afb5dd4c1512fe4ba7830312e2a924a985bdef103eacea1224aa8`  
		Last Modified: Wed, 03 May 2023 16:01:06 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc627eddb62a602a20a487838e54f5863790ff56a80af0f35d9c6e4377c9b293`  
		Last Modified: Wed, 03 May 2023 16:08:39 GMT  
		Size: 24.6 MB (24618525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:devel-slim-threaded-bullseye` - linux; arm variant v5

```console
$ docker pull perl@sha256:b717cea1a94f359c76b1302ca99e997fd454b42dfc9a5e7474a6cb4f85777967
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.5 MB (51507157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:632fbb41d82a30704ead2a5821ea7a4829826622ac621d0a53e9a842d2ee2a37`
-	Default Command: `["perl5.37.11","-de0"]`

```dockerfile
# Tue, 23 May 2023 00:48:41 GMT
ADD file:868f634f5ddb80ed9e9c719ccaf5d564d96fe819f0b000ecc734311baf5da99b in / 
# Tue, 23 May 2023 00:48:42 GMT
CMD ["bash"]
# Tue, 23 May 2023 02:30:56 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Tue, 23 May 2023 02:30:56 GMT
WORKDIR /usr/src/perl
# Tue, 23 May 2023 03:58:47 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        zlib1g-dev        xz-utils        libssl-dev     && curl -fL https://www.cpan.org/src/5.0/perl-5.37.11.tar.xz -o perl-5.37.11.tar.xz     && echo '3946b00266595ccc44df28275e2fbb7b86c1482934cbeab2780db304a75ffd58 *perl-5.37.11.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.37.11.tar.xz -C /usr/src/perl     && rm perl-5.37.11.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local -Dusedevel -Dversiononly=undef -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7046.tar.gz     && echo '3e8c9d9b44a7348f9acc917163dbfc15bd5ea72501492cea3a35b346440ff862 *App-cpanminus-1.7046.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7046.tar.gz && cd App-cpanminus-1.7046 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && savedPackages="ca-certificates make netbase zlib1g-dev libssl-dev"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7046* /tmp/*     && cpanm --version && cpm --version
# Tue, 23 May 2023 03:58:48 GMT
WORKDIR /
# Tue, 23 May 2023 03:58:48 GMT
CMD ["perl5.37.11" "-de0"]
```

-	Layers:
	-	`sha256:812967ccba449e7a96044b2d48ffc62816b22eb17641844c4dfffbe3b3ec6f21`  
		Last Modified: Tue, 23 May 2023 00:51:19 GMT  
		Size: 28.9 MB (28903411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6442c0dd0ab32e6621ec679ac224362fc987d2a5f5efda8962d6c7bfd3761df`  
		Last Modified: Tue, 23 May 2023 03:59:52 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33934438455fccb678c33f3376a28290530750d733dbf62c231710c3b33822be`  
		Last Modified: Tue, 23 May 2023 04:04:36 GMT  
		Size: 22.6 MB (22603579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:devel-slim-threaded-bullseye` - linux; arm variant v7

```console
$ docker pull perl@sha256:7595d74eb7c03083e48103180178dd0eac1bdbbf276988d5b513724066fef625
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.6 MB (48559271 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e4d9e4a09126f2fecc4c929d652e2c298ddbbca7165e0d7e887862ce4ba3438`
-	Default Command: `["perl5.37.11","-de0"]`

```dockerfile
# Tue, 23 May 2023 00:57:55 GMT
ADD file:dbb95e676c7a9806b1883ebcf4259345159caf22ff7194ba7556ea0b1f78099a in / 
# Tue, 23 May 2023 00:57:56 GMT
CMD ["bash"]
# Tue, 23 May 2023 01:59:35 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Tue, 23 May 2023 01:59:36 GMT
WORKDIR /usr/src/perl
# Tue, 23 May 2023 03:26:38 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        zlib1g-dev        xz-utils        libssl-dev     && curl -fL https://www.cpan.org/src/5.0/perl-5.37.11.tar.xz -o perl-5.37.11.tar.xz     && echo '3946b00266595ccc44df28275e2fbb7b86c1482934cbeab2780db304a75ffd58 *perl-5.37.11.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.37.11.tar.xz -C /usr/src/perl     && rm perl-5.37.11.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local -Dusedevel -Dversiononly=undef -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7046.tar.gz     && echo '3e8c9d9b44a7348f9acc917163dbfc15bd5ea72501492cea3a35b346440ff862 *App-cpanminus-1.7046.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7046.tar.gz && cd App-cpanminus-1.7046 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && savedPackages="ca-certificates make netbase zlib1g-dev libssl-dev"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7046* /tmp/*     && cpanm --version && cpm --version
# Tue, 23 May 2023 03:26:39 GMT
WORKDIR /
# Tue, 23 May 2023 03:26:39 GMT
CMD ["perl5.37.11" "-de0"]
```

-	Layers:
	-	`sha256:a27027e97f260d9b7aac9bae941b44639374700dc4c32cc2e378b189a4ffda88`  
		Last Modified: Tue, 23 May 2023 01:01:46 GMT  
		Size: 26.6 MB (26564635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:149145aeb9bc97fa49ecb2c5e80a056c06737fcb033c53d8a2130ffe849f4c7d`  
		Last Modified: Tue, 23 May 2023 03:33:49 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff6244a66314a2cdb391f68a6d71b38d7eec1de1b7bbda4d512d37e355236eb4`  
		Last Modified: Tue, 23 May 2023 03:38:14 GMT  
		Size: 22.0 MB (21994468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:devel-slim-threaded-bullseye` - linux; arm64 variant v8

```console
$ docker pull perl@sha256:d1f60de705632c49603867523e5cf30c763a76b1b58ab52df770ec547eae8217
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.8 MB (53775751 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c955f614e6a375d3835c6b6eda3e5ea7816042557138b76d6a39a5ad099e444a`
-	Default Command: `["perl5.37.11","-de0"]`

```dockerfile
# Tue, 23 May 2023 00:43:15 GMT
ADD file:0fee550e337f1bd111a7ef785a9553674f25649f37deffa4aa8107ef6445d259 in / 
# Tue, 23 May 2023 00:43:15 GMT
CMD ["bash"]
# Tue, 23 May 2023 02:48:32 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Tue, 23 May 2023 02:48:33 GMT
WORKDIR /usr/src/perl
# Tue, 23 May 2023 03:59:29 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        zlib1g-dev        xz-utils        libssl-dev     && curl -fL https://www.cpan.org/src/5.0/perl-5.37.11.tar.xz -o perl-5.37.11.tar.xz     && echo '3946b00266595ccc44df28275e2fbb7b86c1482934cbeab2780db304a75ffd58 *perl-5.37.11.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.37.11.tar.xz -C /usr/src/perl     && rm perl-5.37.11.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local -Dusedevel -Dversiononly=undef -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7046.tar.gz     && echo '3e8c9d9b44a7348f9acc917163dbfc15bd5ea72501492cea3a35b346440ff862 *App-cpanminus-1.7046.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7046.tar.gz && cd App-cpanminus-1.7046 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && savedPackages="ca-certificates make netbase zlib1g-dev libssl-dev"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7046* /tmp/*     && cpanm --version && cpm --version
# Tue, 23 May 2023 03:59:30 GMT
WORKDIR /
# Tue, 23 May 2023 03:59:30 GMT
CMD ["perl5.37.11" "-de0"]
```

-	Layers:
	-	`sha256:d981f2c20c93e1c57a46cd87bc5b9a554be5323072a0d0ab4b354aabd237bbcf`  
		Last Modified: Tue, 23 May 2023 00:46:07 GMT  
		Size: 30.1 MB (30052747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7533f6f322a9d9de0cc36ca2b656235887578cf1d166c0614763e4cb6b1542cd`  
		Last Modified: Tue, 23 May 2023 04:05:28 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb5ffad5cdddae0b46662dae3434cc6e87e46edbe2b81fe7350f3e2e381fc3ed`  
		Last Modified: Tue, 23 May 2023 04:09:25 GMT  
		Size: 23.7 MB (23722835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:devel-slim-threaded-bullseye` - linux; 386

```console
$ docker pull perl@sha256:541a3a449b9b3f95e99158e173f87cafeaa8f1765f626cb91d58f08b5bfc672f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.5 MB (58463796 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a3a02ad43fc682ea07019b4061b95342150cda47e5737e73fe4c5377150c398`
-	Default Command: `["perl5.37.11","-de0"]`

```dockerfile
# Wed, 03 May 2023 00:00:58 GMT
ADD file:caea439e2dbe0148904e3b9a0c5a843d2d0b7c196725d2b41790594e64dcdce8 in / 
# Wed, 03 May 2023 00:00:58 GMT
CMD ["bash"]
# Wed, 03 May 2023 13:02:38 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Wed, 03 May 2023 13:02:39 GMT
WORKDIR /usr/src/perl
# Wed, 03 May 2023 17:39:22 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        zlib1g-dev        xz-utils        libssl-dev     && curl -fL https://www.cpan.org/src/5.0/perl-5.37.11.tar.xz -o perl-5.37.11.tar.xz     && echo '3946b00266595ccc44df28275e2fbb7b86c1482934cbeab2780db304a75ffd58 *perl-5.37.11.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.37.11.tar.xz -C /usr/src/perl     && rm perl-5.37.11.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local -Dusedevel -Dversiononly=undef -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7046.tar.gz     && echo '3e8c9d9b44a7348f9acc917163dbfc15bd5ea72501492cea3a35b346440ff862 *App-cpanminus-1.7046.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7046.tar.gz && cd App-cpanminus-1.7046 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && savedPackages="ca-certificates make netbase zlib1g-dev libssl-dev"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7046* /tmp/*     && cpanm --version && cpm --version
# Wed, 03 May 2023 17:39:22 GMT
WORKDIR /
# Wed, 03 May 2023 17:39:22 GMT
CMD ["perl5.37.11" "-de0"]
```

-	Layers:
	-	`sha256:10b34014bd1c165cc57a10e7492f17dce658513b7329319fe6c193c85bf752db`  
		Last Modified: Wed, 03 May 2023 00:05:12 GMT  
		Size: 32.4 MB (32388208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:471b75db11723b5d4a070ca65d02fa08242be5256657401ed362173aaefb6fd2`  
		Last Modified: Wed, 03 May 2023 17:51:21 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7058f995515a979ed24c328e81eb5142d7500f40841bb3a9fe95573e75a17b1a`  
		Last Modified: Wed, 03 May 2023 17:59:41 GMT  
		Size: 26.1 MB (26075421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:devel-slim-threaded-bullseye` - linux; mips64le

```console
$ docker pull perl@sha256:f7a4525986c17e978df156fa342ddb4753597db44ce3be1761146359b6dab49a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.2 MB (53156156 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14dee243817bb63685242939753c3fc977501d61184d1899cb25ce17c0e74816`
-	Default Command: `["perl5.37.11","-de0"]`

```dockerfile
# Tue, 02 May 2023 23:49:45 GMT
ADD file:c3427ec4e3a2c988fdd372b529660d45ee105e317d6a964ce96f8f9009a3c21e in / 
# Tue, 02 May 2023 23:49:49 GMT
CMD ["bash"]
# Wed, 03 May 2023 16:40:13 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Wed, 03 May 2023 16:40:15 GMT
WORKDIR /usr/src/perl
# Wed, 03 May 2023 22:33:43 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        zlib1g-dev        xz-utils        libssl-dev     && curl -fL https://www.cpan.org/src/5.0/perl-5.37.11.tar.xz -o perl-5.37.11.tar.xz     && echo '3946b00266595ccc44df28275e2fbb7b86c1482934cbeab2780db304a75ffd58 *perl-5.37.11.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.37.11.tar.xz -C /usr/src/perl     && rm perl-5.37.11.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local -Dusedevel -Dversiononly=undef -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7046.tar.gz     && echo '3e8c9d9b44a7348f9acc917163dbfc15bd5ea72501492cea3a35b346440ff862 *App-cpanminus-1.7046.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7046.tar.gz && cd App-cpanminus-1.7046 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && savedPackages="ca-certificates make netbase zlib1g-dev libssl-dev"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7046* /tmp/*     && cpanm --version && cpm --version
# Wed, 03 May 2023 22:33:46 GMT
WORKDIR /
# Wed, 03 May 2023 22:33:50 GMT
CMD ["perl5.37.11" "-de0"]
```

-	Layers:
	-	`sha256:498edd615f8781385e0d5246e189d80b5caceb207fe26608a12605d0a823d4df`  
		Last Modified: Tue, 02 May 2023 23:58:10 GMT  
		Size: 29.6 MB (29623482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aeab0b5e53c168509b8500954c33452a297d667979a5768726c141788e72339`  
		Last Modified: Wed, 03 May 2023 22:35:38 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37447e2e9d6c9215d146a20c3f18cd3b82a7340e86562eb7547b3e9cf2bf9163`  
		Last Modified: Wed, 03 May 2023 22:43:32 GMT  
		Size: 23.5 MB (23532541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:devel-slim-threaded-bullseye` - linux; ppc64le

```console
$ docker pull perl@sha256:eda09dcce6f1e89f98cbc8970151da3d40a3d4ec3f35878fdf3b0e6e05dceb26
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.2 MB (60178040 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a3443458915e7a574fe1abc52027acf2c9df2c627567047d35aab27b21ccf5f`
-	Default Command: `["perl5.37.11","-de0"]`

```dockerfile
# Wed, 03 May 2023 00:31:50 GMT
ADD file:ee3b3c43add645e1a2078f2a6e8544d223abf2754eb8039cbbc2cbdb911b49bb in / 
# Wed, 03 May 2023 00:31:52 GMT
CMD ["bash"]
# Wed, 03 May 2023 18:26:39 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Wed, 03 May 2023 18:26:40 GMT
WORKDIR /usr/src/perl
# Wed, 03 May 2023 20:46:30 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        zlib1g-dev        xz-utils        libssl-dev     && curl -fL https://www.cpan.org/src/5.0/perl-5.37.11.tar.xz -o perl-5.37.11.tar.xz     && echo '3946b00266595ccc44df28275e2fbb7b86c1482934cbeab2780db304a75ffd58 *perl-5.37.11.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.37.11.tar.xz -C /usr/src/perl     && rm perl-5.37.11.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local -Dusedevel -Dversiononly=undef -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7046.tar.gz     && echo '3e8c9d9b44a7348f9acc917163dbfc15bd5ea72501492cea3a35b346440ff862 *App-cpanminus-1.7046.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7046.tar.gz && cd App-cpanminus-1.7046 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && savedPackages="ca-certificates make netbase zlib1g-dev libssl-dev"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7046* /tmp/*     && cpanm --version && cpm --version
# Wed, 03 May 2023 20:46:32 GMT
WORKDIR /
# Wed, 03 May 2023 20:46:33 GMT
CMD ["perl5.37.11" "-de0"]
```

-	Layers:
	-	`sha256:e39c6de44f96d2720b144cbaa9e763eac60a69222a96279f3962e8a701fb17ac`  
		Last Modified: Wed, 03 May 2023 00:36:56 GMT  
		Size: 35.3 MB (35280910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aacc3708f3c9104e0b0fce9d52935b72c8636b637bc73b45909fca9071dc013`  
		Last Modified: Wed, 03 May 2023 20:48:14 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f41eb4a419892e52a84fcae8d7a8e763ad691d7d5eabbfc931453b458b9554ce`  
		Last Modified: Wed, 03 May 2023 20:53:54 GMT  
		Size: 24.9 MB (24896964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:devel-slim-threaded-bullseye` - linux; s390x

```console
$ docker pull perl@sha256:5022db153766f759c942a4e32177aa8a1630903748c7072f1331dd773cc060c7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.5 MB (53475872 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:110840b528d300b1736fc71bc4f42a17ea2619f6229a71e595383c12f49af0b9`
-	Default Command: `["perl5.37.11","-de0"]`

```dockerfile
# Wed, 03 May 2023 03:41:57 GMT
ADD file:7dcdb7d695d9510a1a7e1623776d63d56f7025bdd1702a13a3acd52af825b9c3 in / 
# Wed, 03 May 2023 03:41:59 GMT
CMD ["bash"]
# Wed, 03 May 2023 19:52:56 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Wed, 03 May 2023 19:52:56 GMT
WORKDIR /usr/src/perl
# Wed, 03 May 2023 21:35:03 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        zlib1g-dev        xz-utils        libssl-dev     && curl -fL https://www.cpan.org/src/5.0/perl-5.37.11.tar.xz -o perl-5.37.11.tar.xz     && echo '3946b00266595ccc44df28275e2fbb7b86c1482934cbeab2780db304a75ffd58 *perl-5.37.11.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.37.11.tar.xz -C /usr/src/perl     && rm perl-5.37.11.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local -Dusedevel -Dversiononly=undef -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7046.tar.gz     && echo '3e8c9d9b44a7348f9acc917163dbfc15bd5ea72501492cea3a35b346440ff862 *App-cpanminus-1.7046.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7046.tar.gz && cd App-cpanminus-1.7046 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && savedPackages="ca-certificates make netbase zlib1g-dev libssl-dev"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7046* /tmp/*     && cpanm --version && cpm --version
# Wed, 03 May 2023 21:35:05 GMT
WORKDIR /
# Wed, 03 May 2023 21:35:05 GMT
CMD ["perl5.37.11" "-de0"]
```

-	Layers:
	-	`sha256:8e4cb8eb5d7a86a02dfc1d3645e982def0fc1c20e1fd14d9c6736177d3887dfa`  
		Last Modified: Wed, 03 May 2023 03:44:59 GMT  
		Size: 29.6 MB (29642157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:579316470b896a113902037afcba6b6f8e35cfe96203ea94818e62994606199c`  
		Last Modified: Wed, 03 May 2023 21:36:15 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b698d566be501e2032313536a50761e278ff00e330a792b965941a9d6acdadf8`  
		Last Modified: Wed, 03 May 2023 21:39:03 GMT  
		Size: 23.8 MB (23833549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
