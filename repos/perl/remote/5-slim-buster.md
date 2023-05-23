## `perl:5-slim-buster`

```console
$ docker pull perl@sha256:13f260f52abb82f66d4badde2afd792b54da7e624e63104b788d8aad1c09c22e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `perl:5-slim-buster` - linux; amd64

```console
$ docker pull perl@sha256:4554558b1cbdcbdc6e525606d256d098a900fb09288e7d9960c2e8b7ba5e3834
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.1 MB (54066406 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd5f7f89a7a31eae509e12aa647ad2262d90a59b78f9edc7b436f0261359f8c2`
-	Default Command: `["perl5.36.1","-de0"]`

```dockerfile
# Tue, 02 May 2023 23:47:16 GMT
ADD file:00bc0eda6d2eb0f8ad4abc654f762ffb9ec7e8d1c95d0cc0e7d0cba176d33e27 in / 
# Tue, 02 May 2023 23:47:17 GMT
CMD ["bash"]
# Wed, 03 May 2023 13:15:12 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Wed, 03 May 2023 13:15:12 GMT
WORKDIR /usr/src/perl
# Wed, 03 May 2023 13:20:44 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        zlib1g-dev        xz-utils        libssl-dev     && curl -fL https://www.cpan.org/src/5.0/perl-5.36.1.tar.xz -o perl-5.36.1.tar.xz     && echo 'bd91217ea8a8c8b81f21ebbb6cefdf0d13ae532013f944cdece2cd51aef4b6a7 *perl-5.36.1.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.36.1.tar.xz -C /usr/src/perl     && rm perl-5.36.1.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7046.tar.gz     && echo '3e8c9d9b44a7348f9acc917163dbfc15bd5ea72501492cea3a35b346440ff862 *App-cpanminus-1.7046.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7046.tar.gz && cd App-cpanminus-1.7046 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && savedPackages="ca-certificates make netbase zlib1g-dev libssl-dev"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7046* /tmp/*     && cpanm --version && cpm --version
# Wed, 03 May 2023 13:20:44 GMT
WORKDIR /
# Wed, 03 May 2023 13:20:45 GMT
CMD ["perl5.36.1" "-de0"]
```

-	Layers:
	-	`sha256:25ff99d195814e98b7ef4708519299d9f177def504f9b718c61eb82c7f0b34be`  
		Last Modified: Tue, 02 May 2023 23:51:01 GMT  
		Size: 27.1 MB (27138959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b5da4d06a774e401b02ab6c29f076a92be1484ec5c1fc9f2aef885a186e15aa`  
		Last Modified: Wed, 03 May 2023 16:01:31 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5b0779e0bd733cb9aaace9681d7c3b44eea137ae3bec2ee32853479e0633000`  
		Last Modified: Wed, 03 May 2023 16:01:36 GMT  
		Size: 26.9 MB (26927281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:5-slim-buster` - linux; arm variant v7

```console
$ docker pull perl@sha256:ed8b1755e101428ab1dc6cece068d4bfda720eecf3f00751f42bc8d3b2a47ddb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.2 MB (46244381 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c8da9ecbd2ed9776082e0d012f056874e2f65da7797854111c727d726bf9ca98`
-	Default Command: `["perl5.36.1","-de0"]`

```dockerfile
# Tue, 23 May 2023 00:58:17 GMT
ADD file:fc75413703cf08c1fc3b981ebbde07494b7ad8176aadd5f3a8fb891f0c48e7b9 in / 
# Tue, 23 May 2023 00:58:17 GMT
CMD ["bash"]
# Tue, 23 May 2023 02:05:13 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Tue, 23 May 2023 02:05:13 GMT
WORKDIR /usr/src/perl
# Tue, 23 May 2023 02:11:03 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        zlib1g-dev        xz-utils        libssl-dev     && curl -fL https://www.cpan.org/src/5.0/perl-5.36.1.tar.xz -o perl-5.36.1.tar.xz     && echo 'bd91217ea8a8c8b81f21ebbb6cefdf0d13ae532013f944cdece2cd51aef4b6a7 *perl-5.36.1.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.36.1.tar.xz -C /usr/src/perl     && rm perl-5.36.1.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7046.tar.gz     && echo '3e8c9d9b44a7348f9acc917163dbfc15bd5ea72501492cea3a35b346440ff862 *App-cpanminus-1.7046.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7046.tar.gz && cd App-cpanminus-1.7046 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && savedPackages="ca-certificates make netbase zlib1g-dev libssl-dev"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7046* /tmp/*     && cpanm --version && cpm --version
# Tue, 23 May 2023 02:11:04 GMT
WORKDIR /
# Tue, 23 May 2023 02:11:04 GMT
CMD ["perl5.36.1" "-de0"]
```

-	Layers:
	-	`sha256:0265ca860f8350954d0667b45b48728e992970f63232c58e18fac59852acd8f2`  
		Last Modified: Tue, 23 May 2023 01:02:24 GMT  
		Size: 22.7 MB (22747412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1921d8365ec324266d45aa9485e81d38b5adcdc92afa1e92b8cde2298e8ec076`  
		Last Modified: Tue, 23 May 2023 03:34:15 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eca7537a59d6d6fc03794cbf00d9e1e532d42f7dd680362864c6960a7e0e4cba`  
		Last Modified: Tue, 23 May 2023 03:34:20 GMT  
		Size: 23.5 MB (23496800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:5-slim-buster` - linux; arm64 variant v8

```console
$ docker pull perl@sha256:af0a67f84fcf25575e14ae2b8e9d376c94291843dd5042084910f6cb2a5d323d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.5 MB (51482139 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca26c51c999e66dfd3018b73a52571ef598af28f2da1aeb098fe6e6899cfab7f`
-	Default Command: `["perl5.36.1","-de0"]`

```dockerfile
# Tue, 23 May 2023 00:43:28 GMT
ADD file:55a469039df0bf0e94ef7cd2d6fd355ad0c69e0e23e7921194445dd1fe281e3b in / 
# Tue, 23 May 2023 00:43:28 GMT
CMD ["bash"]
# Tue, 23 May 2023 02:53:10 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Tue, 23 May 2023 02:53:10 GMT
WORKDIR /usr/src/perl
# Tue, 23 May 2023 02:57:38 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        zlib1g-dev        xz-utils        libssl-dev     && curl -fL https://www.cpan.org/src/5.0/perl-5.36.1.tar.xz -o perl-5.36.1.tar.xz     && echo 'bd91217ea8a8c8b81f21ebbb6cefdf0d13ae532013f944cdece2cd51aef4b6a7 *perl-5.36.1.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.36.1.tar.xz -C /usr/src/perl     && rm perl-5.36.1.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7046.tar.gz     && echo '3e8c9d9b44a7348f9acc917163dbfc15bd5ea72501492cea3a35b346440ff862 *App-cpanminus-1.7046.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7046.tar.gz && cd App-cpanminus-1.7046 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && savedPackages="ca-certificates make netbase zlib1g-dev libssl-dev"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7046* /tmp/*     && cpanm --version && cpm --version
# Tue, 23 May 2023 02:57:38 GMT
WORKDIR /
# Tue, 23 May 2023 02:57:39 GMT
CMD ["perl5.36.1" "-de0"]
```

-	Layers:
	-	`sha256:3ca7b6c7180eac66b9c4301084a16319f41eb7f7365bdf91bcc272bd24cb4149`  
		Last Modified: Tue, 23 May 2023 00:46:44 GMT  
		Size: 25.9 MB (25921744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6bdb081e9d81649e4b473c649c91e68dd1799dc56558a5b1059f7db252f0de7`  
		Last Modified: Tue, 23 May 2023 04:05:52 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:348b7130b5def396677e3c1799274c85f6905a787739cadf815bc3f3ebeeacc2`  
		Last Modified: Tue, 23 May 2023 04:05:56 GMT  
		Size: 25.6 MB (25560228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:5-slim-buster` - linux; 386

```console
$ docker pull perl@sha256:dd4ce0ec46a9ca21f90bb0a2aa083136ed0732fcf524a51ec7f82737b1d7a67d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.9 MB (58853129 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03c2ae01953d80dde177c90c1a788c51d19e74ce09a2a9d5d45506afeacbed5a`
-	Default Command: `["perl5.36.1","-de0"]`

```dockerfile
# Wed, 03 May 2023 00:01:23 GMT
ADD file:b7d2995d8b654298ee7120d8293ac370802e2fda8c311516a581edef93d9e19f in / 
# Wed, 03 May 2023 00:01:24 GMT
CMD ["bash"]
# Wed, 03 May 2023 13:12:16 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Wed, 03 May 2023 13:12:16 GMT
WORKDIR /usr/src/perl
# Wed, 03 May 2023 13:21:38 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        zlib1g-dev        xz-utils        libssl-dev     && curl -fL https://www.cpan.org/src/5.0/perl-5.36.1.tar.xz -o perl-5.36.1.tar.xz     && echo 'bd91217ea8a8c8b81f21ebbb6cefdf0d13ae532013f944cdece2cd51aef4b6a7 *perl-5.36.1.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.36.1.tar.xz -C /usr/src/perl     && rm perl-5.36.1.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7046.tar.gz     && echo '3e8c9d9b44a7348f9acc917163dbfc15bd5ea72501492cea3a35b346440ff862 *App-cpanminus-1.7046.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7046.tar.gz && cd App-cpanminus-1.7046 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && savedPackages="ca-certificates make netbase zlib1g-dev libssl-dev"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7046* /tmp/*     && cpanm --version && cpm --version
# Wed, 03 May 2023 13:21:38 GMT
WORKDIR /
# Wed, 03 May 2023 13:21:39 GMT
CMD ["perl5.36.1" "-de0"]
```

-	Layers:
	-	`sha256:f1fd7e2201a19e853151f73eb8915b83c7c87b3dae495eef72019fecfbc76b3e`  
		Last Modified: Wed, 03 May 2023 00:05:57 GMT  
		Size: 27.8 MB (27797590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d2a5c7d5dcdbe8247c49e028f90b1cfe668a49bb0526e26553b77f1e704a437`  
		Last Modified: Wed, 03 May 2023 17:51:49 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6281890be492de1dfa3dfcc97c63b73fd8f4d5aab6d250869fc28498e572b9c8`  
		Last Modified: Wed, 03 May 2023 17:51:57 GMT  
		Size: 31.1 MB (31055373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
