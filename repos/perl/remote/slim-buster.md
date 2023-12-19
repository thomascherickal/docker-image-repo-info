## `perl:slim-buster`

```console
$ docker pull perl@sha256:6766933601ba44415f3b48a6630fa19c61c95c8bbea909ec1f659bd71ba6d66e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `perl:slim-buster` - linux; amd64

```console
$ docker pull perl@sha256:4062a9b5a11801caec75c0a8f574f9735dc87991e07cc1de5752b435b9e58272
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.5 MB (54494446 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:21b8103d134ac56a3685a66c25edf459d5191150ca192b1864aeaeb7b37c59f4`
-	Default Command: `["perl5.38.2","-de0"]`

```dockerfile
# Tue, 19 Dec 2023 01:21:12 GMT
ADD file:ae5c65eea20f7ddcf93a0aa255b6a08a906ac1a1a65cd2c4b5d1529bf9f6eaf8 in / 
# Tue, 19 Dec 2023 01:21:13 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 08:47:48 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Tue, 19 Dec 2023 08:47:48 GMT
WORKDIR /usr/src/perl
# Tue, 19 Dec 2023 08:53:44 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        zlib1g-dev        xz-utils        libssl-dev     && curl -fL https://www.cpan.org/src/5.0/perl-5.38.2.tar.xz -o perl-5.38.2.tar.xz     && echo 'd91115e90b896520e83d4de6b52f8254ef2b70a8d545ffab33200ea9f1cf29e8 *perl-5.38.2.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.38.2.tar.xz -C /usr/src/perl     && rm perl-5.38.2.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && savedPackages="ca-certificates make netbase zlib1g-dev libssl-dev"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Tue, 19 Dec 2023 08:53:45 GMT
WORKDIR /usr/src/app
# Tue, 19 Dec 2023 08:53:45 GMT
CMD ["perl5.38.2" "-de0"]
```

-	Layers:
	-	`sha256:faac0b3889808c27af96e662a1082eef35772c35dcee1c7334f5f5a22b4149d7`  
		Last Modified: Tue, 19 Dec 2023 01:26:21 GMT  
		Size: 27.2 MB (27188221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38617e76d787f8debf4ad14e810e81bd3e329380b11565e988854493207b71ab`  
		Last Modified: Tue, 19 Dec 2023 12:25:09 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:304c099fef3e075d7537313fb7d188c32003eba5a9805d4763a29401bb2cd90b`  
		Last Modified: Tue, 19 Dec 2023 12:25:14 GMT  
		Size: 27.3 MB (27305890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34f9b444d41919ef4e4c418c1e04795f28c9b87b11bd4cd11a9939796ad6243f`  
		Last Modified: Tue, 19 Dec 2023 12:25:09 GMT  
		Size: 165.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:slim-buster` - linux; arm variant v7

```console
$ docker pull perl@sha256:9a48250119475c234e87d1612ff7ae9d353d7a1e22ce91d79c7e222a048eaded
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.7 MB (46686812 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28782bc0b1e1c73ce1084e0a64873f5330721ce1fc080adeab17d42acf9fd64a`
-	Default Command: `["perl5.38.2","-de0"]`

```dockerfile
# Tue, 19 Dec 2023 02:08:27 GMT
ADD file:24df0653e55efc5ba9ec22911758d187c26dbe6bda2d417ff56bc3d9a9072dd4 in / 
# Tue, 19 Dec 2023 02:08:27 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 03:07:47 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Tue, 19 Dec 2023 03:07:47 GMT
WORKDIR /usr/src/perl
# Tue, 19 Dec 2023 03:14:03 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        zlib1g-dev        xz-utils        libssl-dev     && curl -fL https://www.cpan.org/src/5.0/perl-5.38.2.tar.xz -o perl-5.38.2.tar.xz     && echo 'd91115e90b896520e83d4de6b52f8254ef2b70a8d545ffab33200ea9f1cf29e8 *perl-5.38.2.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.38.2.tar.xz -C /usr/src/perl     && rm perl-5.38.2.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && savedPackages="ca-certificates make netbase zlib1g-dev libssl-dev"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Tue, 19 Dec 2023 03:14:03 GMT
WORKDIR /usr/src/app
# Tue, 19 Dec 2023 03:14:04 GMT
CMD ["perl5.38.2" "-de0"]
```

-	Layers:
	-	`sha256:99a10db9a1b078c63980e0e4fc7242bdb6d9ba7c91dd8e0883a55756584bea0f`  
		Last Modified: Tue, 19 Dec 2023 02:13:13 GMT  
		Size: 22.8 MB (22795803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83000db0292fe932c776d76762ce5820480798fef2d624643423b481ea2fa46c`  
		Last Modified: Tue, 19 Dec 2023 05:03:40 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:289bb7b265a97cc732c82afaa23f28580e573af1d893b5a1a157c1ec16ef95db`  
		Last Modified: Tue, 19 Dec 2023 05:03:47 GMT  
		Size: 23.9 MB (23890675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:317b726e3aa1ea57dcbf398dfe78d6c889b2a58feec044e75d175f7c95ff2882`  
		Last Modified: Tue, 19 Dec 2023 05:03:40 GMT  
		Size: 165.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:slim-buster` - linux; arm64 variant v8

```console
$ docker pull perl@sha256:d7d997b7d10183459dedc0fa8e7dc11a73c184c568e8117af73f703341114d37
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.9 MB (51919309 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d35ada1961618a7b20845478c308d50d8a66d8d7e47a26b8daa6cae3c0c299ed`
-	Default Command: `["perl5.38.2","-de0"]`

```dockerfile
# Tue, 19 Dec 2023 01:41:39 GMT
ADD file:f60673c303a98b4e4c676e3403bc1b7cb316335aba1202205188176810494c07 in / 
# Tue, 19 Dec 2023 01:41:40 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 07:59:11 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Tue, 19 Dec 2023 07:59:11 GMT
WORKDIR /usr/src/perl
# Tue, 19 Dec 2023 08:03:42 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        zlib1g-dev        xz-utils        libssl-dev     && curl -fL https://www.cpan.org/src/5.0/perl-5.38.2.tar.xz -o perl-5.38.2.tar.xz     && echo 'd91115e90b896520e83d4de6b52f8254ef2b70a8d545ffab33200ea9f1cf29e8 *perl-5.38.2.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.38.2.tar.xz -C /usr/src/perl     && rm perl-5.38.2.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && savedPackages="ca-certificates make netbase zlib1g-dev libssl-dev"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Tue, 19 Dec 2023 08:03:42 GMT
WORKDIR /usr/src/app
# Tue, 19 Dec 2023 08:03:43 GMT
CMD ["perl5.38.2" "-de0"]
```

-	Layers:
	-	`sha256:c0b0171eefd1c6d7f85c54d4a609269c9b5e19a0fd8cd787a49c808c6b73cf74`  
		Last Modified: Tue, 19 Dec 2023 01:46:01 GMT  
		Size: 26.0 MB (25969827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4966fc0452d3af75ab6fffa0ae6d185d41fcf3b0128df28de342da625a9206e0`  
		Last Modified: Tue, 19 Dec 2023 09:29:17 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58ec6ae23efd76f8f7689e1e400f4a296b042b6ddc97d4f90c4100d661998786`  
		Last Modified: Tue, 19 Dec 2023 09:29:21 GMT  
		Size: 25.9 MB (25949146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:052f744394387f87606417b0870249871afe7b9a05f44a5a5a33191d89475e9c`  
		Last Modified: Tue, 19 Dec 2023 09:29:17 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:slim-buster` - linux; 386

```console
$ docker pull perl@sha256:f99b325c49869e037b281a0d89963bc51f49ebefe18e08f985a614114724475e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.3 MB (59283381 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ddbdb548c226e64c0eddecda43c74ec68a50aca387e30f66a454cd0bd8bad19`
-	Default Command: `["perl5.38.2","-de0"]`

```dockerfile
# Tue, 19 Dec 2023 01:39:52 GMT
ADD file:334e70a7f093f24a0d8e3b87a26edb95d1a12e2dc805ddbcf4e75e3e406803a0 in / 
# Tue, 19 Dec 2023 01:39:52 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 10:26:20 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Tue, 19 Dec 2023 10:26:20 GMT
WORKDIR /usr/src/perl
# Tue, 19 Dec 2023 10:36:02 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        zlib1g-dev        xz-utils        libssl-dev     && curl -fL https://www.cpan.org/src/5.0/perl-5.38.2.tar.xz -o perl-5.38.2.tar.xz     && echo 'd91115e90b896520e83d4de6b52f8254ef2b70a8d545ffab33200ea9f1cf29e8 *perl-5.38.2.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.38.2.tar.xz -C /usr/src/perl     && rm perl-5.38.2.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && savedPackages="ca-certificates make netbase zlib1g-dev libssl-dev"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Tue, 19 Dec 2023 10:36:02 GMT
WORKDIR /usr/src/app
# Tue, 19 Dec 2023 10:36:02 GMT
CMD ["perl5.38.2" "-de0"]
```

-	Layers:
	-	`sha256:92f20691effe39d2fd17b271760acef5ac648490cb2e2d292d69ce7f39589f17`  
		Last Modified: Tue, 19 Dec 2023 01:45:18 GMT  
		Size: 27.8 MB (27846883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10d9086831f5074bb9515f333943b300f9324b9b6748b8a80a3065c5d0914c0d`  
		Last Modified: Tue, 19 Dec 2023 16:36:45 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d401ef41b5f33dadc973e9b5549ace7e1276a804c984a2a239270e4450e3554c`  
		Last Modified: Tue, 19 Dec 2023 16:36:54 GMT  
		Size: 31.4 MB (31436162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ecbd52f910605f2a59216befa32f341b0599cfb9cf2207d35a9c28905e1909e`  
		Last Modified: Tue, 19 Dec 2023 16:36:45 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
