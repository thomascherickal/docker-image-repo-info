## `perl:devel-slim-threaded`

```console
$ docker pull perl@sha256:e2612ecfceb6581d03d38b8bd6ab4f6eb0e1b39b275f5399cb2d778ba271e658
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

### `perl:devel-slim-threaded` - linux; amd64

```console
$ docker pull perl@sha256:96feb84a67ecd851b42d19ba769756e386d136649070988dd23db1d56a8fd898
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.9 MB (55948426 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f70005d2d127909ff1a4a437ecb8d06cb26650616d8e82c2d4e5d83c4a027b3`
-	Default Command: `["perl5.37.8","-de0"]`

```dockerfile
# Wed, 11 Jan 2023 02:34:44 GMT
ADD file:e2398d0bf516084b2b37ba1bb76b86d56e66999831df692461679fbd6a5d8eb6 in / 
# Wed, 11 Jan 2023 02:34:44 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 10:49:36 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Tue, 24 Jan 2023 19:08:22 GMT
WORKDIR /usr/src/perl
# Tue, 24 Jan 2023 21:54:21 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        zlib1g-dev        xz-utils        libssl-dev     && curl -fL https://www.cpan.org/src/5.0/perl-5.37.8.tar.xz -o perl-5.37.8.tar.xz     && echo 'eca6396a4b1aa7a38ef467ce54ed897cc84ba948fad0f90aeb210e57b04daf3c *perl-5.37.8.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.37.8.tar.xz -C /usr/src/perl     && rm perl-5.37.8.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local -Dusedevel -Dversiononly=undef -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7046.tar.gz     && echo '3e8c9d9b44a7348f9acc917163dbfc15bd5ea72501492cea3a35b346440ff862 *App-cpanminus-1.7046.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7046.tar.gz && cd App-cpanminus-1.7046 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && savedPackages="ca-certificates make netbase zlib1g-dev libssl-dev"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7046* /tmp/*     && cpanm --version && cpm --version
# Tue, 24 Jan 2023 21:54:21 GMT
WORKDIR /
# Tue, 24 Jan 2023 21:54:21 GMT
CMD ["perl5.37.8" "-de0"]
```

-	Layers:
	-	`sha256:8740c948ffd4c816ea7ca963f99ca52f4788baa23f228da9581a9ea2edd3fcd7`  
		Last Modified: Wed, 11 Jan 2023 02:39:07 GMT  
		Size: 31.4 MB (31396972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:565612b070b898dfcb0c5e1ec36e88f1d681c94c9b757eeba21c49cc36da6a24`  
		Last Modified: Tue, 24 Jan 2023 22:03:39 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31f42e574d3203e4fbb22fcd5a8f71fcca03605fb8b5552cfbd44a9648096cbf`  
		Last Modified: Tue, 24 Jan 2023 22:11:37 GMT  
		Size: 24.6 MB (24551284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:devel-slim-threaded` - linux; arm variant v5

```console
$ docker pull perl@sha256:d54b9518fd9915078d3ceb2e0fce1cb720acba440fa7a544b166a51c88fd581f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.4 MB (51440639 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8703a8b4c02ca6fa16e231bc5e2588d545d1dc605eea473990cdb7a6b76cab5`
-	Default Command: `["perl5.37.8","-de0"]`

```dockerfile
# Sat, 04 Feb 2023 02:46:38 GMT
ADD file:ce468627e54d8d1c839cea8ab62e505f612298fd97d50e189293fcfcc6af03a5 in / 
# Sat, 04 Feb 2023 02:46:38 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 04:36:27 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Sat, 04 Feb 2023 04:36:27 GMT
WORKDIR /usr/src/perl
# Sat, 04 Feb 2023 06:26:00 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        zlib1g-dev        xz-utils        libssl-dev     && curl -fL https://www.cpan.org/src/5.0/perl-5.37.8.tar.xz -o perl-5.37.8.tar.xz     && echo 'eca6396a4b1aa7a38ef467ce54ed897cc84ba948fad0f90aeb210e57b04daf3c *perl-5.37.8.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.37.8.tar.xz -C /usr/src/perl     && rm perl-5.37.8.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local -Dusedevel -Dversiononly=undef -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7046.tar.gz     && echo '3e8c9d9b44a7348f9acc917163dbfc15bd5ea72501492cea3a35b346440ff862 *App-cpanminus-1.7046.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7046.tar.gz && cd App-cpanminus-1.7046 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && savedPackages="ca-certificates make netbase zlib1g-dev libssl-dev"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7046* /tmp/*     && cpanm --version && cpm --version
# Sat, 04 Feb 2023 06:26:01 GMT
WORKDIR /
# Sat, 04 Feb 2023 06:26:01 GMT
CMD ["perl5.37.8" "-de0"]
```

-	Layers:
	-	`sha256:83735a64f458d40820e4310d632e8bb1dc888f6c25114496be3ce431b5f21d5d`  
		Last Modified: Sat, 04 Feb 2023 02:51:43 GMT  
		Size: 28.9 MB (28898637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb60e40db7b48db175ff31c7c68e43f35e65503c9c11991b85693c20cf137f5f`  
		Last Modified: Sat, 04 Feb 2023 06:31:01 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7066b1ee3881bd8eba06b840c83159b2abeb17024e5b3f2deb12025a9f17e7d`  
		Last Modified: Sat, 04 Feb 2023 06:37:33 GMT  
		Size: 22.5 MB (22541868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:devel-slim-threaded` - linux; arm variant v7

```console
$ docker pull perl@sha256:9e6228cb2e89036fe19f5b8287a6b0759d6e570c6d722e7c646215ce6dbdcdf0
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.5 MB (48499907 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f6637e13807d3529e3f41186ddc783178f0d5b6aa2c0d60d417f69e141050852`
-	Default Command: `["perl5.37.8","-de0"]`

```dockerfile
# Wed, 11 Jan 2023 04:00:36 GMT
ADD file:3fb94bfd628f3ebd91db74501bd297a817977cc066664f0fa342442b3352e0be in / 
# Wed, 11 Jan 2023 04:00:37 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 08:07:37 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Tue, 24 Jan 2023 18:49:29 GMT
WORKDIR /usr/src/perl
# Tue, 24 Jan 2023 21:45:13 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        zlib1g-dev        xz-utils        libssl-dev     && curl -fL https://www.cpan.org/src/5.0/perl-5.37.8.tar.xz -o perl-5.37.8.tar.xz     && echo 'eca6396a4b1aa7a38ef467ce54ed897cc84ba948fad0f90aeb210e57b04daf3c *perl-5.37.8.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.37.8.tar.xz -C /usr/src/perl     && rm perl-5.37.8.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local -Dusedevel -Dversiononly=undef -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7046.tar.gz     && echo '3e8c9d9b44a7348f9acc917163dbfc15bd5ea72501492cea3a35b346440ff862 *App-cpanminus-1.7046.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7046.tar.gz && cd App-cpanminus-1.7046 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && savedPackages="ca-certificates make netbase zlib1g-dev libssl-dev"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7046* /tmp/*     && cpanm --version && cpm --version
# Tue, 24 Jan 2023 21:45:13 GMT
WORKDIR /
# Tue, 24 Jan 2023 21:45:13 GMT
CMD ["perl5.37.8" "-de0"]
```

-	Layers:
	-	`sha256:330ad28688ae3fa5f3b241fef3efd076299bec9874e0597b1c16dcf8a165a53d`  
		Last Modified: Wed, 11 Jan 2023 04:07:49 GMT  
		Size: 26.6 MB (26559488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:974bdc792ce864b03a61bccac62e3d7ff20ff77a88e902d7974df5072e59573a`  
		Last Modified: Tue, 24 Jan 2023 21:58:52 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b777114f30b103d70a43ff841b809130f0e190efbd1d84df3f9325b7e7a12b7a`  
		Last Modified: Tue, 24 Jan 2023 22:09:45 GMT  
		Size: 21.9 MB (21940285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:devel-slim-threaded` - linux; arm64 variant v8

```console
$ docker pull perl@sha256:e86cc08aa78b9269a7818b03bcb866d8c9f7b7c04dd626a9e83c9cc850c789a5
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.7 MB (53708890 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95091caa21c1bf5de9d1e07b8a8c820f803988a2fcc1bdace9263106fbecf11d`
-	Default Command: `["perl5.37.8","-de0"]`

```dockerfile
# Sat, 04 Feb 2023 06:17:37 GMT
ADD file:f613775c59ebd3ca219dc6bbad83115eb74bbbc1980ca4b63e7cb8ab3fa364e4 in / 
# Sat, 04 Feb 2023 06:17:37 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 09:36:20 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Sat, 04 Feb 2023 09:36:20 GMT
WORKDIR /usr/src/perl
# Sat, 04 Feb 2023 11:49:41 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        zlib1g-dev        xz-utils        libssl-dev     && curl -fL https://www.cpan.org/src/5.0/perl-5.37.8.tar.xz -o perl-5.37.8.tar.xz     && echo 'eca6396a4b1aa7a38ef467ce54ed897cc84ba948fad0f90aeb210e57b04daf3c *perl-5.37.8.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.37.8.tar.xz -C /usr/src/perl     && rm perl-5.37.8.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local -Dusedevel -Dversiononly=undef -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7046.tar.gz     && echo '3e8c9d9b44a7348f9acc917163dbfc15bd5ea72501492cea3a35b346440ff862 *App-cpanminus-1.7046.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7046.tar.gz && cd App-cpanminus-1.7046 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && savedPackages="ca-certificates make netbase zlib1g-dev libssl-dev"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7046* /tmp/*     && cpanm --version && cpm --version
# Sat, 04 Feb 2023 11:49:42 GMT
WORKDIR /
# Sat, 04 Feb 2023 11:49:42 GMT
CMD ["perl5.37.8" "-de0"]
```

-	Layers:
	-	`sha256:f79f8cc5c20d534298dd6317333f38b7691da6d66e063ff10699727982c852be`  
		Last Modified: Sat, 04 Feb 2023 06:21:25 GMT  
		Size: 30.0 MB (30044792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c507d23ed65647b7119b52fc539e5cc4591a4f579f075159206d5b1460a00f9c`  
		Last Modified: Sat, 04 Feb 2023 11:57:45 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:216033d93d2e4e276cac2109c8e9579afc736feb6ab0e9e1e9bb9009975e7735`  
		Last Modified: Sat, 04 Feb 2023 12:05:27 GMT  
		Size: 23.7 MB (23663930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:devel-slim-threaded` - linux; 386

```console
$ docker pull perl@sha256:3853041839954d92f241ab8b9d0b6d458625ce501eb2b84372e1464a3ec94dda
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.4 MB (58382127 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43692815750ad315fc99d27f1e8054e045938e5a5968e19563e079f596c1b50c`
-	Default Command: `["perl5.37.8","-de0"]`

```dockerfile
# Sat, 04 Feb 2023 07:49:22 GMT
ADD file:82af884aad6a87f5b309a7418aa1df69f92180a39818ae6d77d37d072cb6fecb in / 
# Sat, 04 Feb 2023 07:49:22 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 10:46:13 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Sat, 04 Feb 2023 10:46:14 GMT
WORKDIR /usr/src/perl
# Sat, 04 Feb 2023 13:53:38 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        zlib1g-dev        xz-utils        libssl-dev     && curl -fL https://www.cpan.org/src/5.0/perl-5.37.8.tar.xz -o perl-5.37.8.tar.xz     && echo 'eca6396a4b1aa7a38ef467ce54ed897cc84ba948fad0f90aeb210e57b04daf3c *perl-5.37.8.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.37.8.tar.xz -C /usr/src/perl     && rm perl-5.37.8.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local -Dusedevel -Dversiononly=undef -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7046.tar.gz     && echo '3e8c9d9b44a7348f9acc917163dbfc15bd5ea72501492cea3a35b346440ff862 *App-cpanminus-1.7046.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7046.tar.gz && cd App-cpanminus-1.7046 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && savedPackages="ca-certificates make netbase zlib1g-dev libssl-dev"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7046* /tmp/*     && cpanm --version && cpm --version
# Sat, 04 Feb 2023 13:53:38 GMT
WORKDIR /
# Sat, 04 Feb 2023 13:53:39 GMT
CMD ["perl5.37.8" "-de0"]
```

-	Layers:
	-	`sha256:fb99e0a97d653ef9acb2bdac0d1d10a8655b789bd4e8924c4a1c4a2af8adbb4a`  
		Last Modified: Sat, 04 Feb 2023 07:55:04 GMT  
		Size: 32.4 MB (32375772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3c894016f2cdcabba737a57123c4d5cd4937dfb5caa3c293f4aa5432f22a6fb`  
		Last Modified: Sat, 04 Feb 2023 14:06:12 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e47d83cb3feae70839098978f578e2139b8494d29abb8cfd18c031b1929baee5`  
		Last Modified: Sat, 04 Feb 2023 14:15:37 GMT  
		Size: 26.0 MB (26006221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:devel-slim-threaded` - linux; mips64le

```console
$ docker pull perl@sha256:2c14ff00265637401acb5c7c35a902b76cf1e3f21325f36961abea3eb685158b
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.1 MB (53087131 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c926ea6b4b4265312cd19d417b9c0df5df821e8c776a3d2b4801155d835c682c`
-	Default Command: `["perl5.37.8","-de0"]`

```dockerfile
# Wed, 11 Jan 2023 16:34:24 GMT
ADD file:295faaf493f6a8d3e2a3eecb28c8f5ac765a1281656221d0a3ab482312a5ee28 in / 
# Wed, 11 Jan 2023 16:34:29 GMT
CMD ["bash"]
# Thu, 12 Jan 2023 02:59:55 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Tue, 24 Jan 2023 19:33:06 GMT
WORKDIR /usr/src/perl
# Wed, 25 Jan 2023 01:24:48 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        zlib1g-dev        xz-utils        libssl-dev     && curl -fL https://www.cpan.org/src/5.0/perl-5.37.8.tar.xz -o perl-5.37.8.tar.xz     && echo 'eca6396a4b1aa7a38ef467ce54ed897cc84ba948fad0f90aeb210e57b04daf3c *perl-5.37.8.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.37.8.tar.xz -C /usr/src/perl     && rm perl-5.37.8.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local -Dusedevel -Dversiononly=undef -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7046.tar.gz     && echo '3e8c9d9b44a7348f9acc917163dbfc15bd5ea72501492cea3a35b346440ff862 *App-cpanminus-1.7046.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7046.tar.gz && cd App-cpanminus-1.7046 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && savedPackages="ca-certificates make netbase zlib1g-dev libssl-dev"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7046* /tmp/*     && cpanm --version && cpm --version
# Wed, 25 Jan 2023 01:24:51 GMT
WORKDIR /
# Wed, 25 Jan 2023 01:24:55 GMT
CMD ["perl5.37.8" "-de0"]
```

-	Layers:
	-	`sha256:9d653aeb7081a0b221d1160bd67b030696ca49b7ca91912bf298835f8f75ac7b`  
		Last Modified: Wed, 11 Jan 2023 16:43:17 GMT  
		Size: 29.6 MB (29619870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:963f7617737f0f06ad5fb2faf8d3e953d47d2ebc9d0149fb1a1b3930be8b210a`  
		Last Modified: Wed, 25 Jan 2023 01:27:01 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:608f53a6c07f698625ca158b67685b966a2283b63b8462be98f2c672f1670ea7`  
		Last Modified: Wed, 25 Jan 2023 01:35:13 GMT  
		Size: 23.5 MB (23467126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:devel-slim-threaded` - linux; ppc64le

```console
$ docker pull perl@sha256:c700516f42959c10857de4e297292613442b0f4ec87763b7b9f21132e12f89f3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.1 MB (60110504 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca6976a2af444712c555a0ee6b8c512de9e7665ffbcb303bfe7add1824847f99`
-	Default Command: `["perl5.37.8","-de0"]`

```dockerfile
# Sat, 04 Feb 2023 12:25:55 GMT
ADD file:2c82cc89d7ac2efeaf54e7589e28644e3e8436d66f6909bf295a2b030116ac58 in / 
# Sat, 04 Feb 2023 12:25:58 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 14:15:05 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Sat, 04 Feb 2023 14:15:06 GMT
WORKDIR /usr/src/perl
# Sat, 04 Feb 2023 15:28:11 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        zlib1g-dev        xz-utils        libssl-dev     && curl -fL https://www.cpan.org/src/5.0/perl-5.37.8.tar.xz -o perl-5.37.8.tar.xz     && echo 'eca6396a4b1aa7a38ef467ce54ed897cc84ba948fad0f90aeb210e57b04daf3c *perl-5.37.8.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.37.8.tar.xz -C /usr/src/perl     && rm perl-5.37.8.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local -Dusedevel -Dversiononly=undef -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7046.tar.gz     && echo '3e8c9d9b44a7348f9acc917163dbfc15bd5ea72501492cea3a35b346440ff862 *App-cpanminus-1.7046.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7046.tar.gz && cd App-cpanminus-1.7046 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && savedPackages="ca-certificates make netbase zlib1g-dev libssl-dev"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7046* /tmp/*     && cpanm --version && cpm --version
# Sat, 04 Feb 2023 15:28:13 GMT
WORKDIR /
# Sat, 04 Feb 2023 15:28:14 GMT
CMD ["perl5.37.8" "-de0"]
```

-	Layers:
	-	`sha256:0604364135762a6c4b3503dd7f0396a51396443bf6052b34b8df7f67679b42c0`  
		Last Modified: Sat, 04 Feb 2023 12:32:12 GMT  
		Size: 35.3 MB (35268795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:078e729cf5c5b819a53e4e9e330ddb2c5256a4c45cd842bcd42373e4cf895bf6`  
		Last Modified: Sat, 04 Feb 2023 15:32:16 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:524875a86bc59af2b750a4e09d9f87bbd1ace888d8c7737faf8b640a992714ab`  
		Last Modified: Sat, 04 Feb 2023 15:36:40 GMT  
		Size: 24.8 MB (24841541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:devel-slim-threaded` - linux; s390x

```console
$ docker pull perl@sha256:fabfaf871db95b6aee5ea587c502f6825dd74a4aa21ee3d79319a22c8836f758
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.4 MB (53396398 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13ab1a1d472142c2d13ce734421e8644b7e8c8537e9c0a8a3100a999dd9eb550`
-	Default Command: `["perl5.37.8","-de0"]`

```dockerfile
# Sat, 04 Feb 2023 04:06:15 GMT
ADD file:29a3ecb38611dbbb6f45b2d10ad3cee60c0198429376f999e9a397f9c405820e in / 
# Sat, 04 Feb 2023 04:06:17 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 05:48:39 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Sat, 04 Feb 2023 05:48:39 GMT
WORKDIR /usr/src/perl
# Sat, 04 Feb 2023 07:19:45 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        zlib1g-dev        xz-utils        libssl-dev     && curl -fL https://www.cpan.org/src/5.0/perl-5.37.8.tar.xz -o perl-5.37.8.tar.xz     && echo 'eca6396a4b1aa7a38ef467ce54ed897cc84ba948fad0f90aeb210e57b04daf3c *perl-5.37.8.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.37.8.tar.xz -C /usr/src/perl     && rm perl-5.37.8.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local -Dusedevel -Dversiononly=undef -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7046.tar.gz     && echo '3e8c9d9b44a7348f9acc917163dbfc15bd5ea72501492cea3a35b346440ff862 *App-cpanminus-1.7046.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7046.tar.gz && cd App-cpanminus-1.7046 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && savedPackages="ca-certificates make netbase zlib1g-dev libssl-dev"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7046* /tmp/*     && cpanm --version && cpm --version
# Sat, 04 Feb 2023 07:19:48 GMT
WORKDIR /
# Sat, 04 Feb 2023 07:19:48 GMT
CMD ["perl5.37.8" "-de0"]
```

-	Layers:
	-	`sha256:7c6fe4d1ef15da79055e0a71952e1a38f799d4f36e9acebdb1ec1512651b39f1`  
		Last Modified: Sat, 04 Feb 2023 04:10:27 GMT  
		Size: 29.6 MB (29629678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e758424023403d8e58948b21d40dc4a758b3011db94e66abee0fd7c0081cd50e`  
		Last Modified: Sat, 04 Feb 2023 07:23:24 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67b3e88f1bb8df67494e5134deeaab19753a753c13f6e059abbea302faf666a7`  
		Last Modified: Sat, 04 Feb 2023 07:27:12 GMT  
		Size: 23.8 MB (23766552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
