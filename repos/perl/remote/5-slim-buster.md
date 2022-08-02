## `perl:5-slim-buster`

```console
$ docker pull perl@sha256:d644fb4f9e8346e15ba6fdcd4bc85f1a36c626c0041caed62aef187dae2f2c88
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

### `perl:5-slim-buster` - linux; amd64

```console
$ docker pull perl@sha256:41729765885d1c7d12a9839383b72732f4b34335d1b832ffa94ce93221227947
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.1 MB (54054521 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea8b91c644f4a9fdbcf1dcf2f59d68fc18c13763a9417d1d1d5dd090d20113ab`
-	Default Command: `["perl5.36.0","-de0"]`

```dockerfile
# Tue, 12 Jul 2022 01:20:32 GMT
ADD file:7f2320197e75c5169402827ce0c47d93629331875d76b9f0ddd389244747eccd in / 
# Tue, 12 Jul 2022 01:20:33 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 05:34:14 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Tue, 12 Jul 2022 05:34:14 GMT
COPY file:3744c5cc39cdbdcae10db09a1f0f399005a79f93c237b387a72ff5710cdd458c in /usr/src/perl/ 
# Tue, 12 Jul 2022 05:34:14 GMT
WORKDIR /usr/src/perl
# Tue, 12 Jul 2022 05:40:05 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        zlib1g-dev        xz-utils        libssl-dev     && curl -fL https://www.cpan.org/src/5.0/perl-5.36.0.tar.xz -o perl-5.36.0.tar.xz     && echo '0f386dccbee8e26286404b2cca144e1005be65477979beb9b1ba272d4819bcf0 *perl-5.36.0.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.36.0.tar.xz -C /usr/src/perl     && rm perl-5.36.0.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7046.tar.gz     && echo '3e8c9d9b44a7348f9acc917163dbfc15bd5ea72501492cea3a35b346440ff862 *App-cpanminus-1.7046.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7046.tar.gz && cd App-cpanminus-1.7046 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && savedPackages="ca-certificates make netbase zlib1g-dev libssl-dev"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7046* /tmp/*     && cpanm --version && cpm --version
# Tue, 12 Jul 2022 05:40:05 GMT
WORKDIR /
# Tue, 12 Jul 2022 05:40:05 GMT
CMD ["perl5.36.0" "-de0"]
```

-	Layers:
	-	`sha256:ac2fb615420c18b61e0693f2569a3d38e3b9b58456b691bac44405e08389a591`  
		Last Modified: Tue, 12 Jul 2022 01:25:22 GMT  
		Size: 27.1 MB (27139850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9ff3d84e12f75d6433aef603baa258a636d3aed02ea3b14062ac55c4a992fa1`  
		Last Modified: Tue, 12 Jul 2022 07:44:08 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:803560d6e29e356d5cb8e2c1d0d32c36d5fba3ac132f17f48c74411f3cccb3c6`  
		Last Modified: Tue, 12 Jul 2022 07:44:13 GMT  
		Size: 26.9 MB (26914472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:5-slim-buster` - linux; arm variant v5

```console
$ docker pull perl@sha256:fb8816febe969520c684133f73e93b8ba9cab4f7e01f1814da87bbb8d0e09968
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (48984438 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9769641b5894cf189633069dc30646ac7b3a852914f9c324878f36e1a252cbd`
-	Default Command: `["perl5.36.0","-de0"]`

```dockerfile
# Tue, 12 Jul 2022 00:51:40 GMT
ADD file:ae02bb368b4b8ce35a4d250031394d4c6d9e5be3b02168f34922bd87dd2bc726 in / 
# Tue, 12 Jul 2022 00:51:40 GMT
CMD ["bash"]
# Wed, 27 Jul 2022 21:51:36 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Wed, 27 Jul 2022 21:51:36 GMT
COPY file:3744c5cc39cdbdcae10db09a1f0f399005a79f93c237b387a72ff5710cdd458c in /usr/src/perl/ 
# Wed, 27 Jul 2022 21:51:36 GMT
WORKDIR /usr/src/perl
# Wed, 27 Jul 2022 22:18:43 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        zlib1g-dev        xz-utils        libssl-dev     && curl -fL https://www.cpan.org/src/5.0/perl-5.36.0.tar.xz -o perl-5.36.0.tar.xz     && echo '0f386dccbee8e26286404b2cca144e1005be65477979beb9b1ba272d4819bcf0 *perl-5.36.0.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.36.0.tar.xz -C /usr/src/perl     && rm perl-5.36.0.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7046.tar.gz     && echo '3e8c9d9b44a7348f9acc917163dbfc15bd5ea72501492cea3a35b346440ff862 *App-cpanminus-1.7046.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7046.tar.gz && cd App-cpanminus-1.7046 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && savedPackages="ca-certificates make netbase zlib1g-dev libssl-dev"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7046* /tmp/*     && cpanm --version && cpm --version
# Wed, 27 Jul 2022 22:18:44 GMT
WORKDIR /
# Wed, 27 Jul 2022 22:18:44 GMT
CMD ["perl5.36.0" "-de0"]
```

-	Layers:
	-	`sha256:e0c9a5e64041e18deb764eddbdc6c3d20b76797d8c2e2eb4c60d4cba21dc486e`  
		Last Modified: Tue, 12 Jul 2022 01:04:31 GMT  
		Size: 24.9 MB (24889765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cf809ad288642b0e3fff8b27b2b4df7dd0698d32b4463288203f4597b49aac7`  
		Last Modified: Thu, 28 Jul 2022 07:33:42 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c1d2921509b92719181d72f5fb9c361f85e45b7ac3d8fabf03bddb220c57a1d`  
		Last Modified: Thu, 28 Jul 2022 07:33:53 GMT  
		Size: 24.1 MB (24094472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:5-slim-buster` - linux; arm variant v7

```console
$ docker pull perl@sha256:e249a291f544e35e3b1c408234115f67cc8ae450692ea785c9b3f5d8e2bd9500
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.2 MB (46243672 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0d5810cd747da80bd3d7ef1ecfb7ce31c875f9446067aae6dddc49742345e66`
-	Default Command: `["perl5.36.0","-de0"]`

```dockerfile
# Tue, 12 Jul 2022 01:01:01 GMT
ADD file:973159cf2de6d7890ce8caf5c207ff8c15c19c5b6ea8dff5ff223a1cf75e3f60 in / 
# Tue, 12 Jul 2022 01:01:02 GMT
CMD ["bash"]
# Fri, 29 Jul 2022 22:22:55 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Fri, 29 Jul 2022 22:22:55 GMT
COPY file:3744c5cc39cdbdcae10db09a1f0f399005a79f93c237b387a72ff5710cdd458c in /usr/src/perl/ 
# Fri, 29 Jul 2022 22:22:55 GMT
WORKDIR /usr/src/perl
# Fri, 29 Jul 2022 22:34:24 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        zlib1g-dev        xz-utils        libssl-dev     && curl -fL https://www.cpan.org/src/5.0/perl-5.36.0.tar.xz -o perl-5.36.0.tar.xz     && echo '0f386dccbee8e26286404b2cca144e1005be65477979beb9b1ba272d4819bcf0 *perl-5.36.0.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.36.0.tar.xz -C /usr/src/perl     && rm perl-5.36.0.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7046.tar.gz     && echo '3e8c9d9b44a7348f9acc917163dbfc15bd5ea72501492cea3a35b346440ff862 *App-cpanminus-1.7046.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7046.tar.gz && cd App-cpanminus-1.7046 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && savedPackages="ca-certificates make netbase zlib1g-dev libssl-dev"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7046* /tmp/*     && cpanm --version && cpm --version
# Fri, 29 Jul 2022 22:34:25 GMT
WORKDIR /
# Fri, 29 Jul 2022 22:34:25 GMT
CMD ["perl5.36.0" "-de0"]
```

-	Layers:
	-	`sha256:8031e2dc59e1b5a08ece8056d69de81b33dd5912c374507a775965a83ce367a8`  
		Last Modified: Tue, 12 Jul 2022 01:14:01 GMT  
		Size: 22.7 MB (22748029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:512851eed406353b71591ba4fe4c963c2acbf9d041a43c0bfe718642acce47a7`  
		Last Modified: Sat, 30 Jul 2022 02:41:37 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be1fb5778a174aa2feb56f51f639edf054fe48bd927e512206d96db2e79bd2ca`  
		Last Modified: Sat, 30 Jul 2022 02:41:43 GMT  
		Size: 23.5 MB (23495442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:5-slim-buster` - linux; arm64 variant v8

```console
$ docker pull perl@sha256:b7be7d5e49a955dfae33c1888c1deb01f9610ed0c43a05f949dbcc5e4fa87dda
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.5 MB (51467168 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1d3dc380a057e8224278db8fbdf0a3bf811183752bbe7b76e974258de1e3b52`
-	Default Command: `["perl5.36.0","-de0"]`

```dockerfile
# Tue, 02 Aug 2022 00:41:03 GMT
ADD file:d973e057fdca9166fb9f39e73d7d5d4ca8ac2af6a55813580bf14a13cef4c159 in / 
# Tue, 02 Aug 2022 00:41:04 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 05:38:33 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Tue, 02 Aug 2022 05:38:35 GMT
COPY file:3744c5cc39cdbdcae10db09a1f0f399005a79f93c237b387a72ff5710cdd458c in /usr/src/perl/ 
# Tue, 02 Aug 2022 05:38:35 GMT
WORKDIR /usr/src/perl
# Tue, 02 Aug 2022 05:44:03 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        zlib1g-dev        xz-utils        libssl-dev     && curl -fL https://www.cpan.org/src/5.0/perl-5.36.0.tar.xz -o perl-5.36.0.tar.xz     && echo '0f386dccbee8e26286404b2cca144e1005be65477979beb9b1ba272d4819bcf0 *perl-5.36.0.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.36.0.tar.xz -C /usr/src/perl     && rm perl-5.36.0.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7046.tar.gz     && echo '3e8c9d9b44a7348f9acc917163dbfc15bd5ea72501492cea3a35b346440ff862 *App-cpanminus-1.7046.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7046.tar.gz && cd App-cpanminus-1.7046 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && savedPackages="ca-certificates make netbase zlib1g-dev libssl-dev"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7046* /tmp/*     && cpanm --version && cpm --version
# Tue, 02 Aug 2022 05:44:04 GMT
WORKDIR /
# Tue, 02 Aug 2022 05:44:04 GMT
CMD ["perl5.36.0" "-de0"]
```

-	Layers:
	-	`sha256:6d588874b4737b02fc84169cf7d3d1d70f20c7f5dbd1ddfe27de4aff25e23314`  
		Last Modified: Tue, 02 Aug 2022 00:46:56 GMT  
		Size: 25.9 MB (25914363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5721374050dd485a154f968423e85d508ecd1a91bfe36044a9c556861728914f`  
		Last Modified: Tue, 02 Aug 2022 07:40:18 GMT  
		Size: 180.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f480e631de77ad2b6c8483347b0b743d4138d8679511af5b507e5e5e5d72ad6`  
		Last Modified: Tue, 02 Aug 2022 07:40:23 GMT  
		Size: 25.6 MB (25552625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:5-slim-buster` - linux; 386

```console
$ docker pull perl@sha256:709c6a737107b7561e399b2d47fa8c95a4c50b081fd51ee60b0fb5a489596976
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.8 MB (58822730 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86122bb12f7cc48f3f59dac7cb25933d4c7d790ab8f837205382ff53464f78f1`
-	Default Command: `["perl5.36.0","-de0"]`

```dockerfile
# Tue, 02 Aug 2022 00:39:47 GMT
ADD file:e8057ee44359188db14ad06a6f8e9cab7a301b479e0f7e0e61810abb0ecf48dd in / 
# Tue, 02 Aug 2022 00:39:47 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 03:42:56 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Tue, 02 Aug 2022 03:42:58 GMT
COPY file:3744c5cc39cdbdcae10db09a1f0f399005a79f93c237b387a72ff5710cdd458c in /usr/src/perl/ 
# Tue, 02 Aug 2022 03:42:58 GMT
WORKDIR /usr/src/perl
# Tue, 02 Aug 2022 03:49:24 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        zlib1g-dev        xz-utils        libssl-dev     && curl -fL https://www.cpan.org/src/5.0/perl-5.36.0.tar.xz -o perl-5.36.0.tar.xz     && echo '0f386dccbee8e26286404b2cca144e1005be65477979beb9b1ba272d4819bcf0 *perl-5.36.0.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.36.0.tar.xz -C /usr/src/perl     && rm perl-5.36.0.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7046.tar.gz     && echo '3e8c9d9b44a7348f9acc917163dbfc15bd5ea72501492cea3a35b346440ff862 *App-cpanminus-1.7046.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7046.tar.gz && cd App-cpanminus-1.7046 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && savedPackages="ca-certificates make netbase zlib1g-dev libssl-dev"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7046* /tmp/*     && cpanm --version && cpm --version
# Tue, 02 Aug 2022 03:49:25 GMT
WORKDIR /
# Tue, 02 Aug 2022 03:49:26 GMT
CMD ["perl5.36.0" "-de0"]
```

-	Layers:
	-	`sha256:0481fdd8148a195a336acc1d5b3d6b0f7fe46395e01c9b674e3ff6974b6ac5a7`  
		Last Modified: Tue, 02 Aug 2022 00:46:14 GMT  
		Size: 27.8 MB (27799555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70f47f439786b3d0eb303656f95b45a6d94d14a1d117f334369fd33c74f9fa76`  
		Last Modified: Tue, 02 Aug 2022 06:05:49 GMT  
		Size: 178.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72ce5f223849db6203368fe5c20ccf7d701eb80acbb7383e9d57004acbe51f6d`  
		Last Modified: Tue, 02 Aug 2022 06:05:55 GMT  
		Size: 31.0 MB (31022997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:5-slim-buster` - linux; mips64le

```console
$ docker pull perl@sha256:f4c9f54057fd87eb3e2f02106495e7a7ac2410816d22b55ca34ae7fffa1aa43b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.9 MB (50874729 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b27da4c6996feeb6ada9c1f66c181d8bae11a526fe6684d03ed056dbdaac9062`
-	Default Command: `["perl5.36.0","-de0"]`

```dockerfile
# Tue, 12 Jul 2022 04:42:11 GMT
ADD file:7cc67dd9da4d585d8bdaed90523c7a817bb92aac2bb1f83554f2b46a49e0e392 in / 
# Tue, 12 Jul 2022 04:42:16 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 08:28:11 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Tue, 12 Jul 2022 08:28:13 GMT
COPY file:3744c5cc39cdbdcae10db09a1f0f399005a79f93c237b387a72ff5710cdd458c in /usr/src/perl/ 
# Tue, 12 Jul 2022 08:28:16 GMT
WORKDIR /usr/src/perl
# Tue, 12 Jul 2022 08:52:15 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        zlib1g-dev        xz-utils        libssl-dev     && curl -fL https://www.cpan.org/src/5.0/perl-5.36.0.tar.xz -o perl-5.36.0.tar.xz     && echo '0f386dccbee8e26286404b2cca144e1005be65477979beb9b1ba272d4819bcf0 *perl-5.36.0.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.36.0.tar.xz -C /usr/src/perl     && rm perl-5.36.0.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7046.tar.gz     && echo '3e8c9d9b44a7348f9acc917163dbfc15bd5ea72501492cea3a35b346440ff862 *App-cpanminus-1.7046.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7046.tar.gz && cd App-cpanminus-1.7046 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && savedPackages="ca-certificates make netbase zlib1g-dev libssl-dev"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7046* /tmp/*     && cpanm --version && cpm --version
# Tue, 12 Jul 2022 08:52:19 GMT
WORKDIR /
# Tue, 12 Jul 2022 08:52:22 GMT
CMD ["perl5.36.0" "-de0"]
```

-	Layers:
	-	`sha256:33fe211fd200b2017da34e0864d2aff58d6963435c4b3b7d15083f6860c2fe1e`  
		Last Modified: Tue, 12 Jul 2022 04:53:03 GMT  
		Size: 25.8 MB (25814577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecfa2efe0ffeea984b3dadcc49f32a60dd3ae1f898de4eef0408b6a64146df24`  
		Last Modified: Tue, 12 Jul 2022 16:47:32 GMT  
		Size: 178.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:984ff5c747d2f6eb23af0aa0a36d2008a4d744420c166d6e29b73e238272d5c4`  
		Last Modified: Tue, 12 Jul 2022 16:47:55 GMT  
		Size: 25.1 MB (25059974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:5-slim-buster` - linux; ppc64le

```console
$ docker pull perl@sha256:165250c2b4bc59b4f24747ed04510c2bf61b5312d07997b6bb5da743b76d0dcc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.6 MB (57554831 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aad5502a9bece058ddc9f64403465a29ae2da7b1d0aa322036bf7b37eb80690b`
-	Default Command: `["perl5.36.0","-de0"]`

```dockerfile
# Tue, 02 Aug 2022 01:18:04 GMT
ADD file:6d33ba25d3625e5f445fc2183b60c64e2cbc780cb541d7f8ac76ce193b311d13 in / 
# Tue, 02 Aug 2022 01:18:06 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 04:58:49 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Tue, 02 Aug 2022 04:58:49 GMT
COPY file:3744c5cc39cdbdcae10db09a1f0f399005a79f93c237b387a72ff5710cdd458c in /usr/src/perl/ 
# Tue, 02 Aug 2022 04:58:49 GMT
WORKDIR /usr/src/perl
# Tue, 02 Aug 2022 05:07:29 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        zlib1g-dev        xz-utils        libssl-dev     && curl -fL https://www.cpan.org/src/5.0/perl-5.36.0.tar.xz -o perl-5.36.0.tar.xz     && echo '0f386dccbee8e26286404b2cca144e1005be65477979beb9b1ba272d4819bcf0 *perl-5.36.0.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.36.0.tar.xz -C /usr/src/perl     && rm perl-5.36.0.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7046.tar.gz     && echo '3e8c9d9b44a7348f9acc917163dbfc15bd5ea72501492cea3a35b346440ff862 *App-cpanminus-1.7046.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7046.tar.gz && cd App-cpanminus-1.7046 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && savedPackages="ca-certificates make netbase zlib1g-dev libssl-dev"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7046* /tmp/*     && cpanm --version && cpm --version
# Tue, 02 Aug 2022 05:07:31 GMT
WORKDIR /
# Tue, 02 Aug 2022 05:07:31 GMT
CMD ["perl5.36.0" "-de0"]
```

-	Layers:
	-	`sha256:fc8842eebb7ccaf249b2bb2d6a3878fffdae26c9db8f23b393c7f76a6249d2f6`  
		Last Modified: Tue, 02 Aug 2022 01:25:45 GMT  
		Size: 30.6 MB (30560308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11bde3d86787a0c5a1ea0e79e2e0db3b01430d3c5b77da15af10ddb7df611eb8`  
		Last Modified: Tue, 02 Aug 2022 07:58:48 GMT  
		Size: 202.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6bbe4129dcf1d55a6fd8ac29245a52491ef811dff31cd241bff86a8564c2cf4`  
		Last Modified: Tue, 02 Aug 2022 07:58:57 GMT  
		Size: 27.0 MB (26994321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:5-slim-buster` - linux; s390x

```console
$ docker pull perl@sha256:b950d2737a755406a3e602857849300ad4e7990a939b969431b4cf75a063ec60
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.3 MB (51276400 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a635d0b5e61b0ad5516a0aacfc4af59242dc5d62bdb668153c875c2c253f220`
-	Default Command: `["perl5.36.0","-de0"]`

```dockerfile
# Tue, 02 Aug 2022 00:42:56 GMT
ADD file:e455828726a550da92d8fc424a6d7694b6be24a8ca52a6152e2ee89d4f7269d0 in / 
# Tue, 02 Aug 2022 00:42:58 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 03:27:02 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Tue, 02 Aug 2022 03:27:02 GMT
COPY file:3744c5cc39cdbdcae10db09a1f0f399005a79f93c237b387a72ff5710cdd458c in /usr/src/perl/ 
# Tue, 02 Aug 2022 03:27:02 GMT
WORKDIR /usr/src/perl
# Tue, 02 Aug 2022 03:32:49 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        zlib1g-dev        xz-utils        libssl-dev     && curl -fL https://www.cpan.org/src/5.0/perl-5.36.0.tar.xz -o perl-5.36.0.tar.xz     && echo '0f386dccbee8e26286404b2cca144e1005be65477979beb9b1ba272d4819bcf0 *perl-5.36.0.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.36.0.tar.xz -C /usr/src/perl     && rm perl-5.36.0.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7046.tar.gz     && echo '3e8c9d9b44a7348f9acc917163dbfc15bd5ea72501492cea3a35b346440ff862 *App-cpanminus-1.7046.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7046.tar.gz && cd App-cpanminus-1.7046 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && savedPackages="ca-certificates make netbase zlib1g-dev libssl-dev"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7046* /tmp/*     && cpanm --version && cpm --version
# Tue, 02 Aug 2022 03:32:51 GMT
WORKDIR /
# Tue, 02 Aug 2022 03:32:51 GMT
CMD ["perl5.36.0" "-de0"]
```

-	Layers:
	-	`sha256:42614a0fa81c110340e6a5a5db155f27bbb6fa8c1e2421b2c2c5f148ea18f35d`  
		Last Modified: Tue, 02 Aug 2022 00:48:34 GMT  
		Size: 25.8 MB (25758761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aeaddbf6b6a3fdbb37ca1f948fb5174ea31a3e500917857030d0c78b763603d`  
		Last Modified: Tue, 02 Aug 2022 05:44:20 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d84ba8d91249d80cb34a127d6cf444649e8ea3f3b9e9bdfe0c6f5a885e7d83f`  
		Last Modified: Tue, 02 Aug 2022 05:44:25 GMT  
		Size: 25.5 MB (25517440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
