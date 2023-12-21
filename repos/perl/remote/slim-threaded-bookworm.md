## `perl:slim-threaded-bookworm`

```console
$ docker pull perl@sha256:a58f87c66ed94c12bb0ffb003966d3958b6a91ec775fff93ab3be8fdce92840b
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 16
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm variant v5
	-	unknown; unknown
	-	linux; arm variant v7
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown
	-	linux; 386
	-	unknown; unknown
	-	linux; mips64le
	-	unknown; unknown
	-	linux; ppc64le
	-	unknown; unknown
	-	linux; s390x
	-	unknown; unknown

### `perl:slim-threaded-bookworm` - linux; amd64

```console
$ docker pull perl@sha256:a9ae3256abd4acaa260ec7f1db1c0f88750d0de32d03a80361111fd1b65d10ac
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.7 MB (57659682 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47c702062f5c23afec2b1fc43d4269c7d29b22de155ea87d8866742219b9edfd`
-	Default Command: `["perl5.38.2","-de0"]`

```dockerfile
# Thu, 30 Nov 2023 02:54:02 GMT
ADD file:ac3cd70031d35e46d86b876934946ffc8756de4de065fbc926dce642dac07ff3 in / 
# Thu, 30 Nov 2023 02:54:02 GMT
CMD ["bash"]
# Thu, 30 Nov 2023 02:54:02 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Thu, 30 Nov 2023 02:54:02 GMT
WORKDIR /usr/src/perl
# Thu, 30 Nov 2023 02:54:02 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        zlib1g-dev        xz-utils        libssl-dev     && curl -fL https://www.cpan.org/src/5.0/perl-5.38.2.tar.xz -o perl-5.38.2.tar.xz     && echo 'd91115e90b896520e83d4de6b52f8254ef2b70a8d545ffab33200ea9f1cf29e8 *perl-5.38.2.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.38.2.tar.xz -C /usr/src/perl     && rm perl-5.38.2.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && savedPackages="ca-certificates make netbase zlib1g-dev libssl-dev"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version # buildkit
# Thu, 30 Nov 2023 02:54:02 GMT
WORKDIR /usr/src/app
# Thu, 30 Nov 2023 02:54:02 GMT
CMD ["perl5.38.2" "-de0"]
```

-	Layers:
	-	`sha256:af107e978371b6cd6339127a05502c5eacd1e6b0e9eb7b2f4aa7b6fc87e2dd81`  
		Last Modified: Tue, 19 Dec 2023 01:24:59 GMT  
		Size: 29.1 MB (29125963 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b99b952c792d2f2a2d494ff8893a0c41a849d01a25f972bb859fab2688b7d7d4`  
		Last Modified: Wed, 20 Dec 2023 20:16:12 GMT  
		Size: 136.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1843e687747ae6b2c1883cefa3fc8d9622028b3f83af73a00fd75bcd5192a009`  
		Last Modified: Wed, 20 Dec 2023 20:16:47 GMT  
		Size: 28.5 MB (28533451 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:130e03968389ef9a62c34ca5e4847ab064f2e8c39b5f9f67a22d65f4c2ac4de5`  
		Last Modified: Wed, 20 Dec 2023 20:16:46 GMT  
		Size: 132.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `perl:slim-threaded-bookworm` - unknown; unknown

```console
$ docker pull perl@sha256:a66a247df2ebeb43298549085afc913d418f2d1309e44cb0745e269a5b81aa3b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.3 MB (3251160 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb5fabb3c987b42d0a671a33815dfd0d22745f3e815ae50a070a7123a8e95eda`

```dockerfile
```

-	Layers:
	-	`sha256:1f89f75c5ea710d18fa37cb02f7b1e0b069ce02828e7b3dbe8d5f6a5724e631f`  
		Last Modified: Wed, 20 Dec 2023 20:16:46 GMT  
		Size: 3.2 MB (3232990 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:e36a75db15020e5f19d14035f0fecb4518c4f73b85c995687ef255f3ca9fa3f2`  
		Last Modified: Wed, 20 Dec 2023 20:16:46 GMT  
		Size: 18.2 KB (18170 bytes)  
		MIME: application/vnd.in-toto+json

### `perl:slim-threaded-bookworm` - linux; arm variant v5

```console
$ docker pull perl@sha256:8c761d72914c902a3086145070f358edb750b36bb35e6c66719cf245126b8220
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.5 MB (52499297 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67cb111212903237012874079cf8662b7661ea11bac0308a280ad4ca9a79922f`
-	Default Command: `["perl5.38.2","-de0"]`

```dockerfile
# Thu, 30 Nov 2023 02:54:02 GMT
ADD file:9503ab966c9dd707eeccc7c2f633bccc94c199f8714ec4ff2c8b54dde3dbabf9 in / 
# Thu, 30 Nov 2023 02:54:02 GMT
CMD ["bash"]
# Thu, 30 Nov 2023 02:54:02 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Thu, 30 Nov 2023 02:54:02 GMT
WORKDIR /usr/src/perl
# Thu, 30 Nov 2023 02:54:02 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        zlib1g-dev        xz-utils        libssl-dev     && curl -fL https://www.cpan.org/src/5.0/perl-5.38.2.tar.xz -o perl-5.38.2.tar.xz     && echo 'd91115e90b896520e83d4de6b52f8254ef2b70a8d545ffab33200ea9f1cf29e8 *perl-5.38.2.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.38.2.tar.xz -C /usr/src/perl     && rm perl-5.38.2.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && savedPackages="ca-certificates make netbase zlib1g-dev libssl-dev"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version # buildkit
# Thu, 30 Nov 2023 02:54:02 GMT
WORKDIR /usr/src/app
# Thu, 30 Nov 2023 02:54:02 GMT
CMD ["perl5.38.2" "-de0"]
```

-	Layers:
	-	`sha256:1ae9a2844c8c70942d2220553689b62e841cc706d77284fbfedbd770080fd699`  
		Last Modified: Tue, 19 Dec 2023 01:58:33 GMT  
		Size: 26.9 MB (26885440 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7cb33750918ac7bd05e898c5e3298ab4f7a4be54436237b690dcdf2522fa2a84`  
		Last Modified: Wed, 20 Dec 2023 21:07:04 GMT  
		Size: 135.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0545604c81114018bc91989502ae306d3e55060ba46af4ab51e76df59d1ad5d8`  
		Last Modified: Wed, 20 Dec 2023 21:41:11 GMT  
		Size: 25.6 MB (25613589 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a34fa810b272314248dc5e28c62356c9b7ae7e917c80210f08bb80bf7ebb7dca`  
		Last Modified: Wed, 20 Dec 2023 21:41:10 GMT  
		Size: 133.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `perl:slim-threaded-bookworm` - unknown; unknown

```console
$ docker pull perl@sha256:ea5ea49b0b37e4e051354354f7faa581130d267a0f13dddd009ded8844d65c61
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.9 KB (17906 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66cf1d99db4a534a1e03bab77922c29fd1b832b1b180907bb158231722bc6b50`

```dockerfile
```

-	Layers:
	-	`sha256:d186ac9d508ece3969f4d15dcc8f0fc64b05219ff0730f74eace41543a749ad3`  
		Last Modified: Wed, 20 Dec 2023 21:41:10 GMT  
		Size: 17.9 KB (17906 bytes)  
		MIME: application/vnd.in-toto+json

### `perl:slim-threaded-bookworm` - linux; arm variant v7

```console
$ docker pull perl@sha256:dd60344beeb90ffbac54c8cdebd4a85402e5a5acd595c1f74cde25e27fde8684
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.5 MB (49537526 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e3f75345b61c181b3611598a1f5e28403847f378ff9fcd3566cd7d9521b77f0`
-	Default Command: `["perl5.38.2","-de0"]`

```dockerfile
# Thu, 30 Nov 2023 02:54:02 GMT
ADD file:aef112919e7924ad6da32181b1df5099cd692680c104118da3a24cd4dfe55a1d in / 
# Thu, 30 Nov 2023 02:54:02 GMT
CMD ["bash"]
# Thu, 30 Nov 2023 02:54:02 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Thu, 30 Nov 2023 02:54:02 GMT
WORKDIR /usr/src/perl
# Thu, 30 Nov 2023 02:54:02 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        zlib1g-dev        xz-utils        libssl-dev     && curl -fL https://www.cpan.org/src/5.0/perl-5.38.2.tar.xz -o perl-5.38.2.tar.xz     && echo 'd91115e90b896520e83d4de6b52f8254ef2b70a8d545ffab33200ea9f1cf29e8 *perl-5.38.2.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.38.2.tar.xz -C /usr/src/perl     && rm perl-5.38.2.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && savedPackages="ca-certificates make netbase zlib1g-dev libssl-dev"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version # buildkit
# Thu, 30 Nov 2023 02:54:02 GMT
WORKDIR /usr/src/app
# Thu, 30 Nov 2023 02:54:02 GMT
CMD ["perl5.38.2" "-de0"]
```

-	Layers:
	-	`sha256:65ab19615c01a3b542f77fadb3bd27872b6a20cba3e9269fb951de36d8fa6805`  
		Last Modified: Tue, 19 Dec 2023 02:11:52 GMT  
		Size: 24.7 MB (24718157 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:795fbd555a3d7b806e169b3c6883dd85433e85bf20598e85fc94b2c27f2a5b1c`  
		Last Modified: Wed, 20 Dec 2023 23:52:25 GMT  
		Size: 136.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:803210ee9b1501d3e575fe96a4f040e1c5966851131ca092b764c0bee23728df`  
		Last Modified: Thu, 21 Dec 2023 01:09:20 GMT  
		Size: 24.8 MB (24819101 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:565d692dadb28cb62cb2063a201a7d58bc3ccd02e119a7866091e37bbc2bdb6c`  
		Last Modified: Thu, 21 Dec 2023 01:09:19 GMT  
		Size: 132.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `perl:slim-threaded-bookworm` - unknown; unknown

```console
$ docker pull perl@sha256:026ebea880f379f477527d8320e6199ead44ef0ddf9eb234921f2552f5214e4e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.2 MB (3225722 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dad0408b98fd95e86eb4115ba1024e52f3537ab643b84ad5b894e44ab0e779b3`

```dockerfile
```

-	Layers:
	-	`sha256:3a3a6eb8cdb91af49f2dd725463d92f79c72e462a9cb23a6955c0fff6095d3de`  
		Last Modified: Thu, 21 Dec 2023 01:09:20 GMT  
		Size: 3.2 MB (3207601 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:4d6184645121a76bf0a4ade6f3ac68ec052df94c5edf09e06df845e13cfa52f9`  
		Last Modified: Thu, 21 Dec 2023 01:09:19 GMT  
		Size: 18.1 KB (18121 bytes)  
		MIME: application/vnd.in-toto+json

### `perl:slim-threaded-bookworm` - linux; arm64 variant v8

```console
$ docker pull perl@sha256:a6a04ee44c47cc7841ff208c70091b5507bce81f6134074f8b8b35fc9df85453
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.5 MB (56473792 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ad0a3964cc7a0ffe6b599b043d9af581079751557b62a2387b308ad1e41ee96`
-	Default Command: `["perl5.38.2","-de0"]`

```dockerfile
# Thu, 30 Nov 2023 02:54:02 GMT
ADD file:262fd7bf0bc26e5d2a229fba52626e22b8a93beac29733acfc60e716c26e689d in / 
# Thu, 30 Nov 2023 02:54:02 GMT
CMD ["bash"]
# Thu, 30 Nov 2023 02:54:02 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Thu, 30 Nov 2023 02:54:02 GMT
WORKDIR /usr/src/perl
# Thu, 30 Nov 2023 02:54:02 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        zlib1g-dev        xz-utils        libssl-dev     && curl -fL https://www.cpan.org/src/5.0/perl-5.38.2.tar.xz -o perl-5.38.2.tar.xz     && echo 'd91115e90b896520e83d4de6b52f8254ef2b70a8d545ffab33200ea9f1cf29e8 *perl-5.38.2.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.38.2.tar.xz -C /usr/src/perl     && rm perl-5.38.2.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && savedPackages="ca-certificates make netbase zlib1g-dev libssl-dev"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version # buildkit
# Thu, 30 Nov 2023 02:54:02 GMT
WORKDIR /usr/src/app
# Thu, 30 Nov 2023 02:54:02 GMT
CMD ["perl5.38.2" "-de0"]
```

-	Layers:
	-	`sha256:24e221e92a36ab5b0075dd156b4f2ff095532a9b0927946cf6070bb1bea208b8`  
		Last Modified: Tue, 19 Dec 2023 01:44:38 GMT  
		Size: 29.2 MB (29157269 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ba9c66806b05448cba83c70a91f2a4bfb5488c92b8189737967cd97934c35001`  
		Last Modified: Wed, 20 Dec 2023 23:10:48 GMT  
		Size: 134.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a998ae84203d9322f3059bcbd309b8f4ef3965292e90a16fa15890ce678c18ed`  
		Last Modified: Thu, 21 Dec 2023 01:22:52 GMT  
		Size: 27.3 MB (27316257 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:34a4507a5cc21104a031fadf4f8ed043e368f6bee96828f660aa68387ea2dedb`  
		Last Modified: Thu, 21 Dec 2023 01:22:51 GMT  
		Size: 132.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `perl:slim-threaded-bookworm` - unknown; unknown

```console
$ docker pull perl@sha256:b64a49d0742c62473faa4a2cc93e470b896542089e1bc69a0fad5f57648eadd4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.2 MB (3226209 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd9d6deb743c4413f947a8177c6b57aaf396c69eac7e4ae56086b5178ff04436`

```dockerfile
```

-	Layers:
	-	`sha256:a72a08239b7a9e6534cd935f245c193b32a402e2647599b8a5a154d703251303`  
		Last Modified: Thu, 21 Dec 2023 01:22:51 GMT  
		Size: 3.2 MB (3208184 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:c13c92820b72a9463e8dbb6cf1c21d71f05f16326a53d19b2f9de738c0ab7ae7`  
		Last Modified: Thu, 21 Dec 2023 01:22:51 GMT  
		Size: 18.0 KB (18025 bytes)  
		MIME: application/vnd.in-toto+json

### `perl:slim-threaded-bookworm` - linux; 386

```console
$ docker pull perl@sha256:3f213a2e42ed80df284823ac5e2c5b0a8122a97c8981e0ef0879ca8be0696222
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.7 MB (57718396 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5142dfcee70d4569077b0e62baef374b5544f042d1e29579d3c61d75989dfbcf`
-	Default Command: `["perl5.38.2","-de0"]`

```dockerfile
# Thu, 30 Nov 2023 02:54:02 GMT
ADD file:6f4083d57ea9644b5a827e67b0725087a15aa428272ec223ab968bf8b4623e42 in / 
# Thu, 30 Nov 2023 02:54:02 GMT
CMD ["bash"]
# Thu, 30 Nov 2023 02:54:02 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Thu, 30 Nov 2023 02:54:02 GMT
WORKDIR /usr/src/perl
# Thu, 30 Nov 2023 02:54:02 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        zlib1g-dev        xz-utils        libssl-dev     && curl -fL https://www.cpan.org/src/5.0/perl-5.38.2.tar.xz -o perl-5.38.2.tar.xz     && echo 'd91115e90b896520e83d4de6b52f8254ef2b70a8d545ffab33200ea9f1cf29e8 *perl-5.38.2.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.38.2.tar.xz -C /usr/src/perl     && rm perl-5.38.2.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && savedPackages="ca-certificates make netbase zlib1g-dev libssl-dev"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version # buildkit
# Thu, 30 Nov 2023 02:54:02 GMT
WORKDIR /usr/src/app
# Thu, 30 Nov 2023 02:54:02 GMT
CMD ["perl5.38.2" "-de0"]
```

-	Layers:
	-	`sha256:8d4aad22fb6a12b8cc7a78d338dfb9bc2bd6d621517b374e446f2915833ea883`  
		Last Modified: Tue, 19 Dec 2023 01:43:45 GMT  
		Size: 30.1 MB (30143863 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b7828572afa17988fd8b70fdf1695e965056035d2a8f82440b5e4593f7b0a001`  
		Last Modified: Wed, 20 Dec 2023 20:17:26 GMT  
		Size: 136.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1d3c3a7f4b9fafd064071f2580e33e9c3f4b92c8edba6e6a25722a1828c50bc1`  
		Last Modified: Wed, 20 Dec 2023 20:17:27 GMT  
		Size: 27.6 MB (27574265 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ac6c13b80a50e7c2499ef915aac0835201cf545886e7ab07864f97ab99624829`  
		Last Modified: Wed, 20 Dec 2023 20:17:26 GMT  
		Size: 132.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `perl:slim-threaded-bookworm` - unknown; unknown

```console
$ docker pull perl@sha256:4646c916c814a65ae19b7197a79a2e3857b8d18a7afd04dd6819926b1218f423
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.9 KB (17896 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac06aa0c73c68534f5971a6ccdd3529d7d20e24805e50650af2eb9bad969a519`

```dockerfile
```

-	Layers:
	-	`sha256:8ba9b0b222bd644b5559b2f3909f1eeb84e4851386ea048f529548f5be0c0c99`  
		Last Modified: Wed, 20 Dec 2023 20:17:26 GMT  
		Size: 17.9 KB (17896 bytes)  
		MIME: application/vnd.in-toto+json

### `perl:slim-threaded-bookworm` - linux; mips64le

```console
$ docker pull perl@sha256:6e0985ce59d0471f5d14d8f5a99b3088b21012d7f2a6764a52457425ccbdc71b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.8 MB (55821307 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7faa391e05deb8ebb60a1a3f8bd39b83f8dad739abefa6f45f4e018e3291d673`
-	Default Command: `["perl5.38.2","-de0"]`

```dockerfile
# Thu, 30 Nov 2023 02:54:02 GMT
ADD file:dcd5696ac281b24df52a518e2402c7f7a4caedfcba0d82e195b7c06cd3a38fdd in / 
# Thu, 30 Nov 2023 02:54:02 GMT
CMD ["bash"]
# Thu, 30 Nov 2023 02:54:02 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Thu, 30 Nov 2023 02:54:02 GMT
WORKDIR /usr/src/perl
# Thu, 30 Nov 2023 02:54:02 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        zlib1g-dev        xz-utils        libssl-dev     && curl -fL https://www.cpan.org/src/5.0/perl-5.38.2.tar.xz -o perl-5.38.2.tar.xz     && echo 'd91115e90b896520e83d4de6b52f8254ef2b70a8d545ffab33200ea9f1cf29e8 *perl-5.38.2.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.38.2.tar.xz -C /usr/src/perl     && rm perl-5.38.2.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && savedPackages="ca-certificates make netbase zlib1g-dev libssl-dev"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version # buildkit
# Thu, 30 Nov 2023 02:54:02 GMT
WORKDIR /usr/src/app
# Thu, 30 Nov 2023 02:54:02 GMT
CMD ["perl5.38.2" "-de0"]
```

-	Layers:
	-	`sha256:12b1322ffb17b8e81ca1c6d9d7118e2fcee0b9d971aa3c90601e6345804a60d1`  
		Last Modified: Tue, 19 Dec 2023 02:24:36 GMT  
		Size: 29.1 MB (29121427 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bab22883c3098f81a212a321bee0239ac0458d1a815b783a61fd4157928b88d8`  
		Last Modified: Thu, 21 Dec 2023 16:52:49 GMT  
		Size: 135.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b673fae1f2e7e101e6230e23353d5abda1486104d4247202aa2b7f7059cc5974`  
		Last Modified: Thu, 21 Dec 2023 18:49:07 GMT  
		Size: 26.7 MB (26699612 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a4bf864ec4cef8823b4716c2489389d864fb986d0a34eead0d189d74f09b6644`  
		Last Modified: Thu, 21 Dec 2023 18:49:03 GMT  
		Size: 133.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `perl:slim-threaded-bookworm` - unknown; unknown

```console
$ docker pull perl@sha256:96b672bdabbffd3552b807bb66ac6f041662b48ee51851fa0a9057898923510b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.9 KB (17898 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:adeea9f864fe63874967cb0d1e188e773275d134c716ceab75ff66d4eb69c349`

```dockerfile
```

-	Layers:
	-	`sha256:9d077ff6f5b559496803e625ad7f5261b376f76c8c214541b7afae25e30feacc`  
		Last Modified: Thu, 21 Dec 2023 18:49:03 GMT  
		Size: 17.9 KB (17898 bytes)  
		MIME: application/vnd.in-toto+json

### `perl:slim-threaded-bookworm` - linux; ppc64le

```console
$ docker pull perl@sha256:7418bbb7601208cdf69b82a92345c18a318e5a4227f28ad0606989eb128cf2b5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.2 MB (62243300 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:50b430838783fce526e380a13d8d2d12279fb3b3a90a3e79d1cf85e6b55c4aff`
-	Default Command: `["perl5.38.2","-de0"]`

```dockerfile
# Thu, 30 Nov 2023 02:54:02 GMT
ADD file:ca1db68689e0b0388337ba450ad2c8e79c159c6b78f5aa6d3ff2b89b8d7edc93 in / 
# Thu, 30 Nov 2023 02:54:02 GMT
CMD ["bash"]
# Thu, 30 Nov 2023 02:54:02 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Thu, 30 Nov 2023 02:54:02 GMT
WORKDIR /usr/src/perl
# Thu, 30 Nov 2023 02:54:02 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        zlib1g-dev        xz-utils        libssl-dev     && curl -fL https://www.cpan.org/src/5.0/perl-5.38.2.tar.xz -o perl-5.38.2.tar.xz     && echo 'd91115e90b896520e83d4de6b52f8254ef2b70a8d545ffab33200ea9f1cf29e8 *perl-5.38.2.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.38.2.tar.xz -C /usr/src/perl     && rm perl-5.38.2.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && savedPackages="ca-certificates make netbase zlib1g-dev libssl-dev"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version # buildkit
# Thu, 30 Nov 2023 02:54:02 GMT
WORKDIR /usr/src/app
# Thu, 30 Nov 2023 02:54:02 GMT
CMD ["perl5.38.2" "-de0"]
```

-	Layers:
	-	`sha256:fc9b8f5eec3aa37ab3aace05165427479352f290d53904cea87dca6349633a09`  
		Last Modified: Tue, 19 Dec 2023 01:26:19 GMT  
		Size: 33.1 MB (33120558 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4a1da38e97da6a26aeb168fef4c89140f2a35cfce62a3cbe9c6741c30783003d`  
		Last Modified: Wed, 20 Dec 2023 21:45:56 GMT  
		Size: 135.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a5756e9d31aceda90a5bf56e24ac3bd5ec89cc55b76f8e4e22d468f321f8a436`  
		Last Modified: Wed, 20 Dec 2023 22:13:29 GMT  
		Size: 29.1 MB (29122474 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3df800e8ff6680a2b73edbc7d27342da59a03771c5b670ab4b67e2a45ce420b2`  
		Last Modified: Wed, 20 Dec 2023 22:13:28 GMT  
		Size: 133.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `perl:slim-threaded-bookworm` - unknown; unknown

```console
$ docker pull perl@sha256:1b860f03aca53cad175b06dc36588dd080a1caf5745e7bf646070deefa2c9b2c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.2 MB (3239656 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a1e2b8f3e9a10ace87daa870d962fadaae016b182472dbd63946887b6f2105e`

```dockerfile
```

-	Layers:
	-	`sha256:562423e7a2143f349436f380d10c9afde4e8db4449e131ca2e58bb1b3754dad6`  
		Last Modified: Wed, 20 Dec 2023 22:13:28 GMT  
		Size: 3.2 MB (3221579 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:244534e344996b13607944fe7efcc39215825e8957865d7a64c3b6064e4a574d`  
		Last Modified: Wed, 20 Dec 2023 22:13:28 GMT  
		Size: 18.1 KB (18077 bytes)  
		MIME: application/vnd.in-toto+json

### `perl:slim-threaded-bookworm` - linux; s390x

```console
$ docker pull perl@sha256:44b933cd7f01577d05928b7d3b5911364db990c674aaa7a7f876b4b50bf55d97
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.6 MB (54562347 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7e775905070192818d9a66e83f5ba01a74b2f02af62fde85aa80dd225f7a34c`
-	Default Command: `["perl5.38.2","-de0"]`

```dockerfile
# Thu, 30 Nov 2023 02:54:02 GMT
ADD file:f06f12fa5a93afc3a79ac4371d24b0a471a5a1818cf34c1d90004c8f410914b9 in / 
# Thu, 30 Nov 2023 02:54:02 GMT
CMD ["bash"]
# Thu, 30 Nov 2023 02:54:02 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Thu, 30 Nov 2023 02:54:02 GMT
WORKDIR /usr/src/perl
# Thu, 30 Nov 2023 02:54:02 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        zlib1g-dev        xz-utils        libssl-dev     && curl -fL https://www.cpan.org/src/5.0/perl-5.38.2.tar.xz -o perl-5.38.2.tar.xz     && echo 'd91115e90b896520e83d4de6b52f8254ef2b70a8d545ffab33200ea9f1cf29e8 *perl-5.38.2.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.38.2.tar.xz -C /usr/src/perl     && rm perl-5.38.2.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && savedPackages="ca-certificates make netbase zlib1g-dev libssl-dev"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version # buildkit
# Thu, 30 Nov 2023 02:54:02 GMT
WORKDIR /usr/src/app
# Thu, 30 Nov 2023 02:54:02 GMT
CMD ["perl5.38.2" "-de0"]
```

-	Layers:
	-	`sha256:bc6b1888979d3ceb063da848b2034e980e2c2613642159c1e856550b79aa620c`  
		Last Modified: Tue, 19 Dec 2023 01:47:38 GMT  
		Size: 27.5 MB (27491874 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b99d0690f588c171aa5e9a610966654592952c0b2087bfa4dba439d487de7e79`  
		Last Modified: Wed, 20 Dec 2023 21:51:18 GMT  
		Size: 135.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ba20e489f1ea312f75f662aab90c65d774eeae0d2c91058ae36eee75fb7801e1`  
		Last Modified: Wed, 20 Dec 2023 22:34:09 GMT  
		Size: 27.1 MB (27070205 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f8895c4eaced4a6d1698325e983f23510f839ce5b618e65d4cb23dbd37fde364`  
		Last Modified: Wed, 20 Dec 2023 22:34:08 GMT  
		Size: 133.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `perl:slim-threaded-bookworm` - unknown; unknown

```console
$ docker pull perl@sha256:f42b3d32730fc9de52c901bbea3677664d659b8153522c518d110c7660095983
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.2 MB (3240535 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9cb79a4fe2e5b58e41e36db1329e5a111fe9347866747f2c8db05a9bc269bfb`

```dockerfile
```

-	Layers:
	-	`sha256:8f91c8956dfc9421bb503a41a5e68be0e8f50a9c26e130f244815c36ab1716bb`  
		Last Modified: Wed, 20 Dec 2023 22:34:08 GMT  
		Size: 3.2 MB (3222532 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:f25cb744cc91ff196b0453bd6f734984e19dae14b44f8cbfe6d05e6098b2fcb7`  
		Last Modified: Wed, 20 Dec 2023 22:34:08 GMT  
		Size: 18.0 KB (18003 bytes)  
		MIME: application/vnd.in-toto+json
