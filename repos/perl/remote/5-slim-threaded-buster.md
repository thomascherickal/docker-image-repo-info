## `perl:5-slim-threaded-buster`

```console
$ docker pull perl@sha256:50edbe92cf83104d5fb9aa368acd7f55a70ebd61dd518b9c2e8e5793978a7828
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 8
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm variant v7
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown
	-	linux; 386
	-	unknown; unknown

### `perl:5-slim-threaded-buster` - linux; amd64

```console
$ docker pull perl@sha256:535783f03cd25b01fc326427f6abd8628db48430b0e7880a6997b3bfb2ea6bfa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.6 MB (54557171 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5dd35b2488d16e37150d2b65b6ca613364e5a128e3156bb4ecc28c431c2e272`
-	Default Command: `["perl5.38.2","-de0"]`

```dockerfile
# Thu, 30 Nov 2023 02:54:02 GMT
ADD file:ae5c65eea20f7ddcf93a0aa255b6a08a906ac1a1a65cd2c4b5d1529bf9f6eaf8 in / 
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
	-	`sha256:faac0b3889808c27af96e662a1082eef35772c35dcee1c7334f5f5a22b4149d7`  
		Last Modified: Tue, 19 Dec 2023 01:26:21 GMT  
		Size: 27.2 MB (27188221 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:08195084f4c01bfbbb435a839bbc3d8c1f1edd27226fdbbcdb1adf2d66b0222c`  
		Last Modified: Wed, 20 Dec 2023 20:16:04 GMT  
		Size: 136.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:40dad487b3aaae3d857c45b3a2305620ecc5f43c1aa440ec78acecd5b15b7870`  
		Last Modified: Wed, 20 Dec 2023 20:16:21 GMT  
		Size: 27.4 MB (27368682 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:772c82db0babbfb52ac6fdc5c578c88590257e92aabfcf828a31ff08aa4fa34b`  
		Last Modified: Wed, 20 Dec 2023 20:16:21 GMT  
		Size: 132.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `perl:5-slim-threaded-buster` - unknown; unknown

```console
$ docker pull perl@sha256:6fec1a4b0c5cf53cbcb220656df98946504c92e7e002c3bfe21c5f960271bab2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2936010 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b674959adae29cafb817331fd18ae1b2b3268d0570bcb84ca35efc78bb8307b7`

```dockerfile
```

-	Layers:
	-	`sha256:e0dd43f00269917955d97fa1cd43e7a0906ddb0d701aba82c641b88b02f2ab11`  
		Last Modified: Wed, 20 Dec 2023 20:16:21 GMT  
		Size: 2.9 MB (2919458 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:75c97b70cc876f62c807312901a11a6c4101e10bb640a471b12f771b6c920dcf`  
		Last Modified: Wed, 20 Dec 2023 20:16:20 GMT  
		Size: 16.6 KB (16552 bytes)  
		MIME: application/vnd.in-toto+json

### `perl:5-slim-threaded-buster` - linux; arm variant v7

```console
$ docker pull perl@sha256:b340e6653b5eb97045f20dad5e118d28cbe28dbf2ddfed62352a788b15e6f157
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.7 MB (46709352 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13ced222c127d1eda262af3bd4211dbea34a6fd0da9d0397f3a393d0be4c72e6`
-	Default Command: `["perl5.38.2","-de0"]`

```dockerfile
# Thu, 30 Nov 2023 02:54:02 GMT
ADD file:24df0653e55efc5ba9ec22911758d187c26dbe6bda2d417ff56bc3d9a9072dd4 in / 
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
	-	`sha256:99a10db9a1b078c63980e0e4fc7242bdb6d9ba7c91dd8e0883a55756584bea0f`  
		Last Modified: Tue, 19 Dec 2023 02:13:13 GMT  
		Size: 22.8 MB (22795803 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:110a77920c4e8e13d75a747c4dd1291a9052ca8a68c2510f25052f407938ed13`  
		Last Modified: Thu, 21 Dec 2023 00:05:06 GMT  
		Size: 135.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7f20f1a23cb80854967cbf49acd2ec7b87dd26197fbd5fb603d07d3be2b6cb23`  
		Last Modified: Thu, 21 Dec 2023 01:39:06 GMT  
		Size: 23.9 MB (23913282 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c8d42e0de962fe280eed7d148634ff2bb2c720cc694b27c122ea3a5388e3bf48`  
		Last Modified: Thu, 21 Dec 2023 01:39:04 GMT  
		Size: 132.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `perl:5-slim-threaded-buster` - unknown; unknown

```console
$ docker pull perl@sha256:a281c02c15e122ccc23ea62d1f909862671e1c5f4b415f03d5144205b76c84e4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2914955 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a589c38840bd1e579002b34eaba47ae9b540f56d14d5dd985652e023d807302`

```dockerfile
```

-	Layers:
	-	`sha256:19b5510b429f369f8e4ea0148652bc2de915ec815d5e3bb41b3ec6ac9c79d6a6`  
		Last Modified: Thu, 21 Dec 2023 01:39:04 GMT  
		Size: 2.9 MB (2898492 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:972c90b92e32ce40002de97c545e30eed7e897ddf101a29f470e65390c928171`  
		Last Modified: Thu, 21 Dec 2023 01:39:04 GMT  
		Size: 16.5 KB (16463 bytes)  
		MIME: application/vnd.in-toto+json

### `perl:5-slim-threaded-buster` - linux; arm64 variant v8

```console
$ docker pull perl@sha256:7ff1c19fa474931507027bae5f3699363c5f704a218a31e159b398853e43bf65
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.9 MB (51948676 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:240025bceeb2f3f3348b0d8e6bffa2b0bf70c61d92be267b2bb4e19fc55690ed`
-	Default Command: `["perl5.38.2","-de0"]`

```dockerfile
# Thu, 30 Nov 2023 02:54:02 GMT
ADD file:f60673c303a98b4e4c676e3403bc1b7cb316335aba1202205188176810494c07 in / 
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
	-	`sha256:c0b0171eefd1c6d7f85c54d4a609269c9b5e19a0fd8cd787a49c808c6b73cf74`  
		Last Modified: Tue, 19 Dec 2023 01:46:01 GMT  
		Size: 26.0 MB (25969827 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:aebfc54de46ad36fcab29cdbc04981513a721d37dc92d20c5069470b64cd4698`  
		Last Modified: Wed, 20 Dec 2023 23:41:48 GMT  
		Size: 135.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5ebbdcacd9b3f33f1838938b569555cd34f2469c018566e831bc3685ab97d3dc`  
		Last Modified: Thu, 21 Dec 2023 01:50:35 GMT  
		Size: 26.0 MB (25978582 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:111b029792581c93f96b2cdf3093eef8c0d35eab9bc2a29d75f76c55c6ac3ae9`  
		Last Modified: Thu, 21 Dec 2023 01:50:33 GMT  
		Size: 132.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `perl:5-slim-threaded-buster` - unknown; unknown

```console
$ docker pull perl@sha256:578ec492bc7d66a5d61c3ff04b482e2db6f7f8c93218844a4d5d587efc5acb8d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2909567 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cdaa264f071b70e07b0e4349673b8dec38e300afab53aa3c14ea4ae3b8259b36`

```dockerfile
```

-	Layers:
	-	`sha256:ba9330ed073a17582aeb52f5e831a03b87818074890bdd24b0cccbd1e024cd98`  
		Last Modified: Thu, 21 Dec 2023 01:50:34 GMT  
		Size: 2.9 MB (2893170 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:3553f025029e7a588d1c6cfb86b738f65cca82a088eec1f25dddad511b837ee3`  
		Last Modified: Thu, 21 Dec 2023 01:50:34 GMT  
		Size: 16.4 KB (16397 bytes)  
		MIME: application/vnd.in-toto+json

### `perl:5-slim-threaded-buster` - linux; 386

```console
$ docker pull perl@sha256:6efa3a56f6a043abda3915c01c0f8f246c107e59bd5607a24ca36d6adfe6ce46
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.4 MB (59390020 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d0d5cf857ce6c12209cdf7295a2362aa98fcce42acefd16f41a8a1f8b24768a`
-	Default Command: `["perl5.38.2","-de0"]`

```dockerfile
# Thu, 30 Nov 2023 02:54:02 GMT
ADD file:334e70a7f093f24a0d8e3b87a26edb95d1a12e2dc805ddbcf4e75e3e406803a0 in / 
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
	-	`sha256:92f20691effe39d2fd17b271760acef5ac648490cb2e2d292d69ce7f39589f17`  
		Last Modified: Tue, 19 Dec 2023 01:45:18 GMT  
		Size: 27.8 MB (27846883 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9289e31a6e39d946fc25f97a0ee36366244eaaf2874074f645c6aab34a88aa1f`  
		Last Modified: Wed, 20 Dec 2023 20:16:51 GMT  
		Size: 135.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e5646c528318135c2d7acf92e12b6dd251516ca359a468db3f61c159b99cf4d7`  
		Last Modified: Wed, 20 Dec 2023 20:16:52 GMT  
		Size: 31.5 MB (31542870 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:22e57a7129505dce866bc23f9c7b1ed4f8e72fd7f431ad2e37ee4389cdb9d766`  
		Last Modified: Wed, 20 Dec 2023 20:16:51 GMT  
		Size: 132.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `perl:5-slim-threaded-buster` - unknown; unknown

```console
$ docker pull perl@sha256:8fdbefc13e9bbe5dfdbf1773a05194522fd2f586ee85fa8a8eb99ba272a6b13c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.3 KB (16303 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e93d10930918952a2f92809aa3ab44f0658ef9ead26d956aa0c105473d4b530d`

```dockerfile
```

-	Layers:
	-	`sha256:a4a452a11aa2612c68535524b22b9f7719a6474d0917910259ed01d955a10938`  
		Last Modified: Wed, 20 Dec 2023 20:16:51 GMT  
		Size: 16.3 KB (16303 bytes)  
		MIME: application/vnd.in-toto+json
