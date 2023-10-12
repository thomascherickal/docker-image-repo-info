## `perl:devel-slim-threaded-bullseye`

```console
$ docker pull perl@sha256:8c661af27786d6955d70ad6809ebbda6b93903226d8fec48cc753c69ddc85cca
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
$ docker pull perl@sha256:a4285cde3c8d9aed50c854891c34e2ed01ee76a7e4653ddfb8dffe3d807a1a95
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.0 MB (56037334 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e48bee3305d85071ad1079a944554fc9e570a11631f1fd2dea4f5ebb2962fa7`
-	Default Command: `["perl5.39.3","-de0"]`

```dockerfile
# Wed, 11 Oct 2023 18:35:13 GMT
ADD file:cb13581b8e7a9de4396639e5ca2f3817763435c0563232f85e3d899f6388a1b3 in / 
# Wed, 11 Oct 2023 18:35:13 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 00:37:51 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Thu, 12 Oct 2023 00:37:51 GMT
WORKDIR /usr/src/perl
# Thu, 12 Oct 2023 02:38:07 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        zlib1g-dev        xz-utils        libssl-dev     && curl -fL https://www.cpan.org/src/5.0/perl-5.39.3.tar.xz -o perl-5.39.3.tar.xz     && echo '93c38a6ff969e3930d7eb08e69a883204a4d835c7122df47c4903950e6fc758a *perl-5.39.3.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.39.3.tar.xz -C /usr/src/perl     && rm perl-5.39.3.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local -Dusedevel -Dversiononly=undef -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && savedPackages="ca-certificates make netbase zlib1g-dev libssl-dev"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Thu, 12 Oct 2023 02:38:08 GMT
WORKDIR /usr/src/app
# Thu, 12 Oct 2023 02:38:08 GMT
CMD ["perl5.39.3" "-de0"]
```

-	Layers:
	-	`sha256:e67fdae3559346105027c63e7fb032bba57e62b1fe9f2da23e6fdfb56384e00b`  
		Last Modified: Wed, 11 Oct 2023 18:40:17 GMT  
		Size: 31.4 MB (31417862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10417c58313d252fdf76963ec59393bc668665ebe29ec3cb68d5632eb7f69bf6`  
		Last Modified: Thu, 12 Oct 2023 02:40:30 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a25b41085966f3cdce867b8c154be3aa4b37ea63f9b0dd3aa9ee7318e261841`  
		Last Modified: Thu, 12 Oct 2023 02:48:09 GMT  
		Size: 24.6 MB (24619140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8ec1f46887df7388d120b74438159b296fc1448813e2f7261287dc6e72fdc60`  
		Last Modified: Thu, 12 Oct 2023 02:48:04 GMT  
		Size: 164.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:devel-slim-threaded-bullseye` - linux; arm variant v5

```console
$ docker pull perl@sha256:daa2c61aa1c911ed4aa067cce0db31462fe28fdb893cbc5179433014a28ce0c3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.5 MB (51526552 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a0e2e268be9b77a32cf33d468f11329363d49e11e7a30afc0f2f040dce11b445`
-	Default Command: `["perl5.39.3","-de0"]`

```dockerfile
# Wed, 11 Oct 2023 17:37:59 GMT
ADD file:01d6efe5a08019fcf00cfd0af4d6d61c6d4e43fd98cbb0054e82e8a78275573f in / 
# Wed, 11 Oct 2023 17:37:59 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 00:42:44 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Thu, 12 Oct 2023 00:42:44 GMT
WORKDIR /usr/src/perl
# Thu, 12 Oct 2023 03:23:24 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        zlib1g-dev        xz-utils        libssl-dev     && curl -fL https://www.cpan.org/src/5.0/perl-5.39.3.tar.xz -o perl-5.39.3.tar.xz     && echo '93c38a6ff969e3930d7eb08e69a883204a4d835c7122df47c4903950e6fc758a *perl-5.39.3.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.39.3.tar.xz -C /usr/src/perl     && rm perl-5.39.3.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local -Dusedevel -Dversiononly=undef -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && savedPackages="ca-certificates make netbase zlib1g-dev libssl-dev"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Thu, 12 Oct 2023 03:23:24 GMT
WORKDIR /usr/src/app
# Thu, 12 Oct 2023 03:23:24 GMT
CMD ["perl5.39.3" "-de0"]
```

-	Layers:
	-	`sha256:5419c984dacdb9784c03bde904accd013b4e056c627102949c262726f4cae135`  
		Last Modified: Wed, 11 Oct 2023 17:41:31 GMT  
		Size: 28.9 MB (28921245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21b1a80256c606828acfb0aa0855e1166548776bd41e1f95942e43bea7f14fc0`  
		Last Modified: Thu, 12 Oct 2023 03:26:09 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97ddf3bc2ac8dcff82d0029d23b04aa37644a84cf823604b505263de581f455c`  
		Last Modified: Thu, 12 Oct 2023 03:34:02 GMT  
		Size: 22.6 MB (22604975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a5d2aa837edde1a53ddad7d5fc6f3a99a9b1f9749d735af49c6874c91583653`  
		Last Modified: Thu, 12 Oct 2023 03:33:57 GMT  
		Size: 165.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:devel-slim-threaded-bullseye` - linux; arm variant v7

```console
$ docker pull perl@sha256:8fffd9d6475e9b0a263510539e52ec47848c0a0e540378e3410888255cde2525
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.6 MB (48583690 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06de7a24bda7c92d47ed9970d9f9d0d675d0745786c3e726f227dbeb7910633c`
-	Default Command: `["perl5.39.3","-de0"]`

```dockerfile
# Wed, 11 Oct 2023 17:42:29 GMT
ADD file:0d1753bfedd7193184780166819d0407867a22d82804c0045274f1f13afecac0 in / 
# Wed, 11 Oct 2023 17:42:29 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 00:48:23 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Thu, 12 Oct 2023 00:48:23 GMT
WORKDIR /usr/src/perl
# Thu, 12 Oct 2023 02:48:18 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        zlib1g-dev        xz-utils        libssl-dev     && curl -fL https://www.cpan.org/src/5.0/perl-5.39.3.tar.xz -o perl-5.39.3.tar.xz     && echo '93c38a6ff969e3930d7eb08e69a883204a4d835c7122df47c4903950e6fc758a *perl-5.39.3.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.39.3.tar.xz -C /usr/src/perl     && rm perl-5.39.3.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local -Dusedevel -Dversiononly=undef -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && savedPackages="ca-certificates make netbase zlib1g-dev libssl-dev"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Thu, 12 Oct 2023 02:48:18 GMT
WORKDIR /usr/src/app
# Thu, 12 Oct 2023 02:48:18 GMT
CMD ["perl5.39.3" "-de0"]
```

-	Layers:
	-	`sha256:bb9c59b28e9fb9c31ffdb002ca9a6656677eee093c8093fcbea8818e927df70a`  
		Last Modified: Wed, 11 Oct 2023 17:47:06 GMT  
		Size: 26.6 MB (26579008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbcad4f7d79ff099c49d8bcb4b81c89da95684268758159ef7965977dba818ef`  
		Last Modified: Thu, 12 Oct 2023 02:50:23 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f3bf623ef33391264a1529422727aefccc061a6c1f0e0b0f37ada186c808ffa`  
		Last Modified: Thu, 12 Oct 2023 02:56:20 GMT  
		Size: 22.0 MB (22004351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eca8d3845722447b25f924d06671f4fc3cc130a4ca87ae287c13e1445458798e`  
		Last Modified: Thu, 12 Oct 2023 02:56:15 GMT  
		Size: 165.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:devel-slim-threaded-bullseye` - linux; arm64 variant v8

```console
$ docker pull perl@sha256:8cfa446fab4c40a654442fa2046893a6d6cdaac76f455e90101e6810f6aebd0e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.8 MB (53791181 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34126bb614de6deaea860d54705b33d43f977ec1d332798a3869e482465eae3b`
-	Default Command: `["perl5.39.3","-de0"]`

```dockerfile
# Wed, 20 Sep 2023 02:44:28 GMT
ADD file:024479be439b4ecb37c939e68673adc72955f3345ca0e809bd13e897709e59e4 in / 
# Wed, 20 Sep 2023 02:44:28 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 13:03:53 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Wed, 20 Sep 2023 13:03:53 GMT
WORKDIR /usr/src/perl
# Mon, 25 Sep 2023 20:30:50 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        zlib1g-dev        xz-utils        libssl-dev     && curl -fL https://www.cpan.org/src/5.0/perl-5.39.3.tar.xz -o perl-5.39.3.tar.xz     && echo '93c38a6ff969e3930d7eb08e69a883204a4d835c7122df47c4903950e6fc758a *perl-5.39.3.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.39.3.tar.xz -C /usr/src/perl     && rm perl-5.39.3.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local -Dusedevel -Dversiononly=undef -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && savedPackages="ca-certificates make netbase zlib1g-dev libssl-dev"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Mon, 25 Sep 2023 20:30:51 GMT
WORKDIR /usr/src/app
# Mon, 25 Sep 2023 20:30:51 GMT
CMD ["perl5.39.3" "-de0"]
```

-	Layers:
	-	`sha256:fc521c5b98350f6fd8c72ace1e48558bb7b53cb3db201a2a3b42095401cd02f1`  
		Last Modified: Wed, 20 Sep 2023 02:48:13 GMT  
		Size: 30.1 MB (30062869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:726b322dd1609c1116890332b50b0a9926436b1677427142424605e114d05f5f`  
		Last Modified: Wed, 20 Sep 2023 15:59:17 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2662906d0363286358a73d7b74ec8f7a08567610c61137f7ee4c18028f08611a`  
		Last Modified: Mon, 25 Sep 2023 20:35:41 GMT  
		Size: 23.7 MB (23727981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5eeca622e7c44a104c4aadb750509d2fadf1a4f449900d85957b22ead1ce8037`  
		Last Modified: Mon, 25 Sep 2023 20:35:37 GMT  
		Size: 165.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:devel-slim-threaded-bullseye` - linux; 386

```console
$ docker pull perl@sha256:d03c2aae310549bb008cdc7a45320259e9f725ecf6dea509ac113065ead638ba
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.5 MB (58472490 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10342a54e6e0b1c53eb11fee04886a706928d29a572ebb9baecdea428e7db3c6`
-	Default Command: `["perl5.39.3","-de0"]`

```dockerfile
# Wed, 20 Sep 2023 00:42:18 GMT
ADD file:51db29acb4893b446fcf8a93f7fa809201b49d6ea62a009ab14002cafd3ac4a8 in / 
# Wed, 20 Sep 2023 00:42:18 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 18:26:37 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Wed, 20 Sep 2023 18:26:37 GMT
WORKDIR /usr/src/perl
# Mon, 25 Sep 2023 21:04:51 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        zlib1g-dev        xz-utils        libssl-dev     && curl -fL https://www.cpan.org/src/5.0/perl-5.39.3.tar.xz -o perl-5.39.3.tar.xz     && echo '93c38a6ff969e3930d7eb08e69a883204a4d835c7122df47c4903950e6fc758a *perl-5.39.3.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.39.3.tar.xz -C /usr/src/perl     && rm perl-5.39.3.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local -Dusedevel -Dversiononly=undef -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && savedPackages="ca-certificates make netbase zlib1g-dev libssl-dev"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Mon, 25 Sep 2023 21:04:52 GMT
WORKDIR /usr/src/app
# Mon, 25 Sep 2023 21:04:52 GMT
CMD ["perl5.39.3" "-de0"]
```

-	Layers:
	-	`sha256:091eb56f13f4be91ea9416e1b67e2c1f228b5e023f447dda2d3f5c56e57ff871`  
		Last Modified: Wed, 20 Sep 2023 00:47:36 GMT  
		Size: 32.4 MB (32397092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d6016d9f565e3ec043635c786f8bc583e26abef633c71c4fe74da52bc5193e5`  
		Last Modified: Thu, 21 Sep 2023 00:47:58 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4609b3677be125f04cb43ce9edcf301e78c70d278913a8dd4f13b7cc7df0ef44`  
		Last Modified: Mon, 25 Sep 2023 21:10:07 GMT  
		Size: 26.1 MB (26075066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18b61a313734111e62826f92ce0edeaf0d4db0c264dfc8b46a0306edbaaa0a6e`  
		Last Modified: Mon, 25 Sep 2023 21:09:59 GMT  
		Size: 164.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:devel-slim-threaded-bullseye` - linux; mips64le

```console
$ docker pull perl@sha256:781601a4e20dc4df49721d438d8166b37611eb3e840c53dcb971695e0e78f3db
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.0 MB (52964641 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4f31de76c0c3a0d5219b9b06ff2a0fd3e99f56a42cd9476fb9745a021965415`
-	Default Command: `["perl5.39.3","-de0"]`

```dockerfile
# Wed, 20 Sep 2023 03:11:15 GMT
ADD file:28a15ec61fcc8eb66f514312583089fecc600fe3b84fdbe3bf5692f05d946bff in / 
# Wed, 20 Sep 2023 03:11:20 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 06:45:15 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Wed, 20 Sep 2023 06:45:18 GMT
WORKDIR /usr/src/perl
# Mon, 25 Sep 2023 21:43:59 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        zlib1g-dev        xz-utils        libssl-dev     && curl -fL https://www.cpan.org/src/5.0/perl-5.39.3.tar.xz -o perl-5.39.3.tar.xz     && echo '93c38a6ff969e3930d7eb08e69a883204a4d835c7122df47c4903950e6fc758a *perl-5.39.3.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.39.3.tar.xz -C /usr/src/perl     && rm perl-5.39.3.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local -Dusedevel -Dversiononly=undef -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && savedPackages="ca-certificates make netbase zlib1g-dev libssl-dev"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Mon, 25 Sep 2023 21:44:03 GMT
WORKDIR /usr/src/app
# Mon, 25 Sep 2023 21:44:06 GMT
CMD ["perl5.39.3" "-de0"]
```

-	Layers:
	-	`sha256:191c4163c9a486a5811472bd51ed6737ccd2265795539d3f557712be2f3a2742`  
		Last Modified: Wed, 20 Sep 2023 03:22:25 GMT  
		Size: 29.6 MB (29634617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c14300f7cee7ba2e0b33907569f05efe5a8f1e3b15189d73f90dcf6f909a98a`  
		Last Modified: Wed, 20 Sep 2023 10:02:12 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea185e7ec2980df09381ba08ecea91288c03c6d72c6b7a796bd06e808837a322`  
		Last Modified: Mon, 25 Sep 2023 21:46:55 GMT  
		Size: 23.3 MB (23329757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f2cd10aaf0681e2d65ce5f1244097b95dc02b138c7049557851cdd853ca644d`  
		Last Modified: Mon, 25 Sep 2023 21:46:36 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:devel-slim-threaded-bullseye` - linux; ppc64le

```console
$ docker pull perl@sha256:722451c819775843cb6f3c1f41d617018d01dc891da8df8986035d48142f1ba5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.2 MB (60182982 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4cb11fe6b59e6947606ac6adbcb2d47e852ad4dea7a5040182caa54326da05ac`
-	Default Command: `["perl5.39.3","-de0"]`

```dockerfile
# Wed, 20 Sep 2023 07:53:28 GMT
ADD file:906774443118f59963ef3b425ff702af4588c1cf1d7c32f6f72fff8b1af50339 in / 
# Wed, 20 Sep 2023 07:53:30 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 18:46:18 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Wed, 20 Sep 2023 18:46:18 GMT
WORKDIR /usr/src/perl
# Mon, 25 Sep 2023 20:53:15 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        zlib1g-dev        xz-utils        libssl-dev     && curl -fL https://www.cpan.org/src/5.0/perl-5.39.3.tar.xz -o perl-5.39.3.tar.xz     && echo '93c38a6ff969e3930d7eb08e69a883204a4d835c7122df47c4903950e6fc758a *perl-5.39.3.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.39.3.tar.xz -C /usr/src/perl     && rm perl-5.39.3.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local -Dusedevel -Dversiononly=undef -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && savedPackages="ca-certificates make netbase zlib1g-dev libssl-dev"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Mon, 25 Sep 2023 20:53:17 GMT
WORKDIR /usr/src/app
# Mon, 25 Sep 2023 20:53:18 GMT
CMD ["perl5.39.3" "-de0"]
```

-	Layers:
	-	`sha256:e64bfb4d4b8bfd61a4dccfc651ce802e40087cdf6029b3cbf1710fa529e70fcb`  
		Last Modified: Wed, 20 Sep 2023 08:50:44 GMT  
		Size: 35.3 MB (35291079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a07ada23eeb8c504d83ffc35e49dfac9020a406e4ab99a76e574eb361460fcee`  
		Last Modified: Wed, 20 Sep 2023 20:53:30 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6a063f05fc5a86d534e7ffcfa3a8632df27a3d0ad06320822e16dfb4534af97`  
		Last Modified: Mon, 25 Sep 2023 20:55:15 GMT  
		Size: 24.9 MB (24891572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eda683602483ac62080ca1b2b8472f812e3e52ae07bed927094c6a8480ed536f`  
		Last Modified: Mon, 25 Sep 2023 20:55:07 GMT  
		Size: 165.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:devel-slim-threaded-bullseye` - linux; s390x

```console
$ docker pull perl@sha256:b1f7b612c43839f981087a5134482732fe4fb0fdef436ebf503982ed6109eab0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.5 MB (53484089 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30977343f02f29226a63b9e98558300319c14dccd138f07212943028b69c33e0`
-	Default Command: `["perl5.39.3","-de0"]`

```dockerfile
# Wed, 20 Sep 2023 02:54:54 GMT
ADD file:02a97e0d5f41f84ac0284849646284fa41b5e324d24f4d95bb1e2419899da811 in / 
# Wed, 20 Sep 2023 02:54:57 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 10:57:36 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Wed, 20 Sep 2023 10:57:36 GMT
WORKDIR /usr/src/perl
# Mon, 25 Sep 2023 20:08:23 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        zlib1g-dev        xz-utils        libssl-dev     && curl -fL https://www.cpan.org/src/5.0/perl-5.39.3.tar.xz -o perl-5.39.3.tar.xz     && echo '93c38a6ff969e3930d7eb08e69a883204a4d835c7122df47c4903950e6fc758a *perl-5.39.3.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.39.3.tar.xz -C /usr/src/perl     && rm perl-5.39.3.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local -Dusedevel -Dversiononly=undef -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && savedPackages="ca-certificates make netbase zlib1g-dev libssl-dev"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Mon, 25 Sep 2023 20:08:25 GMT
WORKDIR /usr/src/app
# Mon, 25 Sep 2023 20:08:26 GMT
CMD ["perl5.39.3" "-de0"]
```

-	Layers:
	-	`sha256:d2d51167e651784cce0bd658d0c2caa328adef8ccf264d8c09860a95bc2a2fc6`  
		Last Modified: Wed, 20 Sep 2023 03:00:22 GMT  
		Size: 29.7 MB (29653129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de66e90e53e474082243fc37a3967eb683bc1d5b2cbd8b0cbddb8a2838c8d6ed`  
		Last Modified: Wed, 20 Sep 2023 12:30:56 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e44160dbf382c17f77f1efe43923a033db95ae0801a1ab5d2366041dc6e4da9`  
		Last Modified: Mon, 25 Sep 2023 20:10:21 GMT  
		Size: 23.8 MB (23830628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26c2e24a5fa64e3a7dd6e38a0cab230846624f18ae8a31946a81f830ef6598c5`  
		Last Modified: Mon, 25 Sep 2023 20:10:16 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
