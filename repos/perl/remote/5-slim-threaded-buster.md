## `perl:5-slim-threaded-buster`

```console
$ docker pull perl@sha256:d4e645080d4df975033f4558479e0c07e46eb7e9c2835e4ee2ffd32f26309b0c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `perl:5-slim-threaded-buster` - linux; amd64

```console
$ docker pull perl@sha256:96a3cb10ce9f7f186437d538a783e11e55c365080bdc737c2d0eca43c39163f4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.6 MB (54572866 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34b906e5e62386c0fc664bbada93f740dd2738b151fe047310a4f345d8a29c89`
-	Default Command: `["perl5.38.0","-de0"]`

```dockerfile
# Thu, 07 Sep 2023 00:21:35 GMT
ADD file:9c8b7c79fbbb19d308d151785d178e19bfa7b83257f38d03fa7f30cd41d58530 in / 
# Thu, 07 Sep 2023 00:21:35 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 08:00:24 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Thu, 07 Sep 2023 08:00:24 GMT
WORKDIR /usr/src/perl
# Thu, 07 Sep 2023 08:43:29 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        zlib1g-dev        xz-utils        libssl-dev     && curl -fL https://www.cpan.org/src/5.0/perl-5.38.0.tar.xz -o perl-5.38.0.tar.xz     && echo 'eca551caec3bc549a4e590c0015003790bdd1a604ffe19cc78ee631d51f7072e *perl-5.38.0.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.38.0.tar.xz -C /usr/src/perl     && rm perl-5.38.0.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && savedPackages="ca-certificates make netbase zlib1g-dev libssl-dev"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Thu, 07 Sep 2023 08:43:30 GMT
WORKDIR /usr/src/app
# Thu, 07 Sep 2023 08:43:30 GMT
CMD ["perl5.38.0" "-de0"]
```

-	Layers:
	-	`sha256:91f01557fe0da558070d4f24631c94e91a80877a24621b52b8b13009b62d8d96`  
		Last Modified: Thu, 07 Sep 2023 00:26:44 GMT  
		Size: 27.2 MB (27187385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5eb6256486f3f9f579fb5d9f35a80679d5521f94a848d91e49bef7346310c6c`  
		Last Modified: Thu, 07 Sep 2023 11:32:18 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8e553a1dc58ad3dd4ef888835b29120fa6abfcad80da6e51acd62eab4cb68d5`  
		Last Modified: Thu, 07 Sep 2023 11:34:32 GMT  
		Size: 27.4 MB (27385150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df1b0d79fef315b86cc3df523bf3da8e0b3990f5a30c5f77e386589107c8b50a`  
		Last Modified: Thu, 07 Sep 2023 11:34:26 GMT  
		Size: 164.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:5-slim-threaded-buster` - linux; arm variant v7

```console
$ docker pull perl@sha256:0a68301dcbe07562165202a2eecb12df6b60d9e681139a628c931d12606f6ac2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.7 MB (46719021 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6db8f90c3bfae724f4e5df4a7e7cbc562209f5f0a9748474f41988a7311f49f5`
-	Default Command: `["perl5.38.0","-de0"]`

```dockerfile
# Thu, 07 Sep 2023 00:58:32 GMT
ADD file:fa060a900723a2fce017a38b08be3eb2c27d4768d40c61cd1f6292a7f28a8bdc in / 
# Thu, 07 Sep 2023 00:58:33 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 07:31:21 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Thu, 07 Sep 2023 07:31:21 GMT
WORKDIR /usr/src/perl
# Thu, 07 Sep 2023 08:16:38 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        zlib1g-dev        xz-utils        libssl-dev     && curl -fL https://www.cpan.org/src/5.0/perl-5.38.0.tar.xz -o perl-5.38.0.tar.xz     && echo 'eca551caec3bc549a4e590c0015003790bdd1a604ffe19cc78ee631d51f7072e *perl-5.38.0.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.38.0.tar.xz -C /usr/src/perl     && rm perl-5.38.0.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && savedPackages="ca-certificates make netbase zlib1g-dev libssl-dev"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Thu, 07 Sep 2023 08:16:38 GMT
WORKDIR /usr/src/app
# Thu, 07 Sep 2023 08:16:38 GMT
CMD ["perl5.38.0" "-de0"]
```

-	Layers:
	-	`sha256:7e54f06c680feaf82a31a34e7453d765f332f671cfecacb622c3046561dcc572`  
		Last Modified: Thu, 07 Sep 2023 01:03:53 GMT  
		Size: 22.8 MB (22795752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:297e4deb009e4a06184d23c2d932230c5b303f8a864eb904c789b0cfea0fd735`  
		Last Modified: Thu, 07 Sep 2023 11:14:26 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9156327068582bfeb44cdecbb2a2d3edfdd26403d5646a9443c0e4c465ef84e9`  
		Last Modified: Thu, 07 Sep 2023 11:16:56 GMT  
		Size: 23.9 MB (23922937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da723a7257d1b8c07dad6450bdbb98d2f6b0db097ceca040ba7517f8770644c3`  
		Last Modified: Thu, 07 Sep 2023 11:16:49 GMT  
		Size: 165.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:5-slim-threaded-buster` - linux; arm64 variant v8

```console
$ docker pull perl@sha256:187918ad3e974fcca7c06702b143d2768197d9067f477fb1fabda553e742903b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.0 MB (51960848 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ef55c179a1f7746b8f71d3cec2fb4baec8262e9d6087c9852b4e1fcd1fb4d4e`
-	Default Command: `["perl5.38.0","-de0"]`

```dockerfile
# Wed, 20 Sep 2023 02:44:42 GMT
ADD file:22373577ebc4a88322b8e7e5a349667740deade289df65952593aa5fa355e161 in / 
# Wed, 20 Sep 2023 02:44:42 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 13:08:31 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Wed, 20 Sep 2023 13:08:31 GMT
WORKDIR /usr/src/perl
# Wed, 20 Sep 2023 13:43:09 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        zlib1g-dev        xz-utils        libssl-dev     && curl -fL https://www.cpan.org/src/5.0/perl-5.38.0.tar.xz -o perl-5.38.0.tar.xz     && echo 'eca551caec3bc549a4e590c0015003790bdd1a604ffe19cc78ee631d51f7072e *perl-5.38.0.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.38.0.tar.xz -C /usr/src/perl     && rm perl-5.38.0.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && savedPackages="ca-certificates make netbase zlib1g-dev libssl-dev"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Wed, 20 Sep 2023 13:43:09 GMT
WORKDIR /usr/src/app
# Wed, 20 Sep 2023 13:43:09 GMT
CMD ["perl5.38.0" "-de0"]
```

-	Layers:
	-	`sha256:a5329dc26fe29288aabb62184c71ef06987bd81c95d7c43a48e38a0dfaa54ff8`  
		Last Modified: Wed, 20 Sep 2023 02:48:50 GMT  
		Size: 26.0 MB (25967816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b77314c33d9a069b543242421de6d8ba5aa4ddb60b1f9726e18dacdab64f92dd`  
		Last Modified: Wed, 20 Sep 2023 15:59:36 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13fda1d8381f638cef28913ffe0fb52e69a016d33cd0ea46b52189b4233d8e9c`  
		Last Modified: Wed, 20 Sep 2023 16:01:58 GMT  
		Size: 26.0 MB (25992701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:980aae1b47e97f3690607f3c06220154f74509602f0bde3aa6356f2c6837a4cb`  
		Last Modified: Wed, 20 Sep 2023 16:01:54 GMT  
		Size: 164.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:5-slim-threaded-buster` - linux; 386

```console
$ docker pull perl@sha256:e928ebad170f012a0cc46400cb4c4109dc96c53a45cbe77268507fc8853250d7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.4 MB (59392290 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0475b3701e87510f1c0d09f3c22e1bd2dc42206480212bfe2548b3d684f1ac1`
-	Default Command: `["perl5.38.0","-de0"]`

```dockerfile
# Thu, 07 Sep 2023 00:39:46 GMT
ADD file:e5916da683bdcea27e31e6fbb29e61d1f8457a3bebe4a83278e4f0181e5ac49f in / 
# Thu, 07 Sep 2023 00:39:47 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 13:02:22 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Thu, 07 Sep 2023 13:02:22 GMT
WORKDIR /usr/src/perl
# Thu, 07 Sep 2023 14:18:09 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        zlib1g-dev        xz-utils        libssl-dev     && curl -fL https://www.cpan.org/src/5.0/perl-5.38.0.tar.xz -o perl-5.38.0.tar.xz     && echo 'eca551caec3bc549a4e590c0015003790bdd1a604ffe19cc78ee631d51f7072e *perl-5.38.0.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.38.0.tar.xz -C /usr/src/perl     && rm perl-5.38.0.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && savedPackages="ca-certificates make netbase zlib1g-dev libssl-dev"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Thu, 07 Sep 2023 14:18:10 GMT
WORKDIR /usr/src/app
# Thu, 07 Sep 2023 14:18:10 GMT
CMD ["perl5.38.0" "-de0"]
```

-	Layers:
	-	`sha256:453c610c7d8be388b9a8559dc654a2def01e71f776e0608ae46db51ae50d10a0`  
		Last Modified: Thu, 07 Sep 2023 00:45:26 GMT  
		Size: 27.8 MB (27846798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df16ce31a766099c7ed4057e3218c376d6295228e0ca18382d95d3def41a7526`  
		Last Modified: Thu, 07 Sep 2023 19:15:46 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d2374f6ac9f654a18e71ea2719e5bdbe0ba7c547862fc58020a006fbf206e75`  
		Last Modified: Thu, 07 Sep 2023 19:18:23 GMT  
		Size: 31.5 MB (31545158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7f334d0259154c9d18e489f18e7bb966101332ec61c2cb027ce804095b88a14`  
		Last Modified: Thu, 07 Sep 2023 19:18:15 GMT  
		Size: 165.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
