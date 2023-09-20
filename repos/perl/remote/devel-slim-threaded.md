## `perl:devel-slim-threaded`

```console
$ docker pull perl@sha256:1cc8959b779e40babcf6a271340ad6b5dba72a611329ed814b6b90ddf7e5b49c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `perl:devel-slim-threaded` - linux; amd64

```console
$ docker pull perl@sha256:dd1c7b1d96e124d932275b2f8d6d3a402ca51ed7e14a1322788ca9e278494099
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.6 MB (57640960 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8352f8fcc50ec4932708d8c4b9b441f2b171520db2f0e60e55c65bcd137ff31b`
-	Default Command: `["perl5.39.2","-de0"]`

```dockerfile
# Wed, 20 Sep 2023 04:55:40 GMT
ADD file:a1398394375faab8dd9e1e8d584eea96c750fb57ae4ffd2b14624f1cf263561b in / 
# Wed, 20 Sep 2023 04:55:41 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 12:42:23 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Wed, 20 Sep 2023 12:42:23 GMT
WORKDIR /usr/src/perl
# Wed, 20 Sep 2023 16:17:17 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        zlib1g-dev        xz-utils        libssl-dev     && curl -fL https://www.cpan.org/src/5.0/perl-5.39.2.tar.xz -o perl-5.39.2.tar.xz     && echo 'b7ae33d3c6ff80107d14c92dfb3d8d4944fec926b11bcc40c8764b73c710694f *perl-5.39.2.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.39.2.tar.xz -C /usr/src/perl     && rm perl-5.39.2.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local -Dusedevel -Dversiononly=undef -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && savedPackages="ca-certificates make netbase zlib1g-dev libssl-dev"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Wed, 20 Sep 2023 16:17:17 GMT
WORKDIR /usr/src/app
# Wed, 20 Sep 2023 16:17:17 GMT
CMD ["perl5.39.2" "-de0"]
```

-	Layers:
	-	`sha256:a803e7c4b030119420574a882a52b6431e160fceb7620f61b525d49bc2d58886`  
		Last Modified: Wed, 20 Sep 2023 05:00:22 GMT  
		Size: 29.1 MB (29124705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a3560abcc24c5fe182570a2ea91b265e938187ed9616e20d64470b931e5a5db`  
		Last Modified: Wed, 20 Sep 2023 16:26:36 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80330cd7559851c19ced18907c9cd65dd356c6b9fe295ac5a9f59174738893ac`  
		Last Modified: Wed, 20 Sep 2023 16:36:14 GMT  
		Size: 28.5 MB (28515922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:722ea4b5915bb7df2110a9dcd6894a11f243bf211c179d01cfba6b9932ba7613`  
		Last Modified: Wed, 20 Sep 2023 16:36:09 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:devel-slim-threaded` - linux; arm variant v7

```console
$ docker pull perl@sha256:8ddbf9b7cd99269f6c07cdafaf83ad228ef09d5e4f38616b1b488e5cacae924a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.6 MB (49623042 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41c56ec41d5d26fff9a7786062b3a82e77e4e6b39e878a7308652f7cdf2fe205`
-	Default Command: `["perl5.39.2","-de0"]`

```dockerfile
# Thu, 07 Sep 2023 00:57:48 GMT
ADD file:5775cb975a13a9e48198190564cd469f115a433dabc5c3406c45e1ef0b1ccdf0 in / 
# Thu, 07 Sep 2023 00:57:49 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 07:19:05 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Thu, 07 Sep 2023 07:19:05 GMT
WORKDIR /usr/src/perl
# Thu, 07 Sep 2023 11:03:24 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        zlib1g-dev        xz-utils        libssl-dev     && curl -fL https://www.cpan.org/src/5.0/perl-5.39.2.tar.xz -o perl-5.39.2.tar.xz     && echo 'b7ae33d3c6ff80107d14c92dfb3d8d4944fec926b11bcc40c8764b73c710694f *perl-5.39.2.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.39.2.tar.xz -C /usr/src/perl     && rm perl-5.39.2.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local -Dusedevel -Dversiononly=undef -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && savedPackages="ca-certificates make netbase zlib1g-dev libssl-dev"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Thu, 07 Sep 2023 11:03:25 GMT
WORKDIR /usr/src/app
# Thu, 07 Sep 2023 11:03:25 GMT
CMD ["perl5.39.2" "-de0"]
```

-	Layers:
	-	`sha256:6a9fec8868f77cdcda1bf847be168c1d104031ca6c8edc961bc7f76e3a4bf54b`  
		Last Modified: Thu, 07 Sep 2023 01:02:31 GMT  
		Size: 24.8 MB (24805221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e8a424767f96867ecabba2dda067f03f1418b2befb594931ec3574015ad1800`  
		Last Modified: Thu, 07 Sep 2023 11:13:32 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ffc89ad362765d3d54a825f7556cf7ce271babb113fe9dabff09bcde52a285f`  
		Last Modified: Thu, 07 Sep 2023 11:24:14 GMT  
		Size: 24.8 MB (24817488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ef3564a021a51b8630d6bd54cc441a4f83c537676895ddf179a4d5b89de6cf5`  
		Last Modified: Thu, 07 Sep 2023 11:24:08 GMT  
		Size: 165.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:devel-slim-threaded` - linux; arm64 variant v8

```console
$ docker pull perl@sha256:7d2f5f007efa93dc42d683808d6a9876099ca115653c1d9e4043aba19c5ae998
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.5 MB (56458269 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f260d91144f0fcd3ca126acf060f035ec92a95a01e5292fc462382660860a092`
-	Default Command: `["perl5.39.2","-de0"]`

```dockerfile
# Wed, 20 Sep 2023 02:44:13 GMT
ADD file:ec1a6e0aedd76c8fdc8544775f8b553f58950e9435f5cfe919f39374e222cfbb in / 
# Wed, 20 Sep 2023 02:44:14 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 12:59:00 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Wed, 20 Sep 2023 12:59:00 GMT
WORKDIR /usr/src/perl
# Wed, 20 Sep 2023 15:50:48 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        zlib1g-dev        xz-utils        libssl-dev     && curl -fL https://www.cpan.org/src/5.0/perl-5.39.2.tar.xz -o perl-5.39.2.tar.xz     && echo 'b7ae33d3c6ff80107d14c92dfb3d8d4944fec926b11bcc40c8764b73c710694f *perl-5.39.2.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.39.2.tar.xz -C /usr/src/perl     && rm perl-5.39.2.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local -Dusedevel -Dversiononly=undef -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && savedPackages="ca-certificates make netbase zlib1g-dev libssl-dev"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Wed, 20 Sep 2023 15:50:49 GMT
WORKDIR /usr/src/app
# Wed, 20 Sep 2023 15:50:49 GMT
CMD ["perl5.39.2" "-de0"]
```

-	Layers:
	-	`sha256:e886f0f47ef56fcadb6ecaf2116056bbdb273e0afe07ed034498b198d386c04e`  
		Last Modified: Wed, 20 Sep 2023 02:47:36 GMT  
		Size: 29.2 MB (29157221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28df2d6e8a54f41a441bc58a8b0c3af462f3295840661d2313d20a4acc8eadb5`  
		Last Modified: Wed, 20 Sep 2023 15:58:49 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1091ca753167edeed8dd4de5fb0b2d1772a8ec457d9ecf6280d795b1cc511dde`  
		Last Modified: Wed, 20 Sep 2023 16:08:23 GMT  
		Size: 27.3 MB (27300716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69f01fddb8541cd4693bb868b429736bc8408e4b359019f170247cf8bf30a8e0`  
		Last Modified: Wed, 20 Sep 2023 16:08:19 GMT  
		Size: 164.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:devel-slim-threaded` - linux; 386

```console
$ docker pull perl@sha256:cc90d54fd97f998d6f0f30ba4a0162c5e01a6ae15cf17c02ca9991503d25f7bf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.7 MB (57713734 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c547d1c1d61dd18b2e70273ad9e16f1933cbe8a7f1008fd26e3e6e20772d7e75`
-	Default Command: `["perl5.39.2","-de0"]`

```dockerfile
# Thu, 07 Sep 2023 00:39:00 GMT
ADD file:0952a54f5474629ed000e89bfd1b8827e49b63270932e45ed8d953a2676ac79c in / 
# Thu, 07 Sep 2023 00:39:00 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 12:41:35 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Thu, 07 Sep 2023 12:41:35 GMT
WORKDIR /usr/src/perl
# Thu, 07 Sep 2023 19:00:27 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        zlib1g-dev        xz-utils        libssl-dev     && curl -fL https://www.cpan.org/src/5.0/perl-5.39.2.tar.xz -o perl-5.39.2.tar.xz     && echo 'b7ae33d3c6ff80107d14c92dfb3d8d4944fec926b11bcc40c8764b73c710694f *perl-5.39.2.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.39.2.tar.xz -C /usr/src/perl     && rm perl-5.39.2.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local -Dusedevel -Dversiononly=undef -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && savedPackages="ca-certificates make netbase zlib1g-dev libssl-dev"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Thu, 07 Sep 2023 19:00:28 GMT
WORKDIR /usr/src/app
# Thu, 07 Sep 2023 19:00:28 GMT
CMD ["perl5.39.2" "-de0"]
```

-	Layers:
	-	`sha256:30ae0f429560d1effd0839849ab7780512b72d9fbc09a6cec67e03092a85a1d1`  
		Last Modified: Thu, 07 Sep 2023 00:43:48 GMT  
		Size: 30.1 MB (30141753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbee828d46eedcea4146d51da2e0167edf432406c789e46f7409b98fd558926d`  
		Last Modified: Thu, 07 Sep 2023 19:14:48 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:743dfd3e1f8023b922a4e0976337f09d3d06a30e6a4ebaf087c0096d50e8747e`  
		Last Modified: Thu, 07 Sep 2023 19:26:22 GMT  
		Size: 27.6 MB (27571649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7568a64ca0186a532a0a33bc6b09f47b831d66e2be19bd8a73f352dcc673bd8`  
		Last Modified: Thu, 07 Sep 2023 19:26:14 GMT  
		Size: 164.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
