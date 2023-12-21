## `perl:5-slim-buster`

```console
$ docker pull perl@sha256:a5e6268215e23a44bc39328376456d0cbf020f7b7cc522ac3b60522bcc6a367a
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

### `perl:5-slim-buster` - linux; amd64

```console
$ docker pull perl@sha256:94541c85f41ce3e743fdeb7dea30a45a3b960d3a35b8997f93f5711e594ada07
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.5 MB (54492877 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b327bf8a3c0b6d8aaa8067f4785d5a9b707fd0565d59dd86a8ce22c4517ed90`
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
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        zlib1g-dev        xz-utils        libssl-dev     && curl -fL https://www.cpan.org/src/5.0/perl-5.38.2.tar.xz -o perl-5.38.2.tar.xz     && echo 'd91115e90b896520e83d4de6b52f8254ef2b70a8d545ffab33200ea9f1cf29e8 *perl-5.38.2.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.38.2.tar.xz -C /usr/src/perl     && rm perl-5.38.2.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && savedPackages="ca-certificates make netbase zlib1g-dev libssl-dev"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version # buildkit
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
	-	`sha256:625997f174364226a5bc95545821b93c2f42a4e8748c79630a036a9748651d01`  
		Last Modified: Wed, 20 Dec 2023 20:15:01 GMT  
		Size: 136.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1f6a015d97124e979a82dfc39b1726524faebcb717e313353ae969260768d653`  
		Last Modified: Wed, 20 Dec 2023 20:15:02 GMT  
		Size: 27.3 MB (27304388 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b32f48569cffc8d32ef7771fb0009f2b98ea204254465fab9efe41014b606877`  
		Last Modified: Wed, 20 Dec 2023 20:15:02 GMT  
		Size: 132.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `perl:5-slim-buster` - unknown; unknown

```console
$ docker pull perl@sha256:a4fd3f1bb2c7520a2ef82da8bdfebb063b228ad83c36dc139608e3320c4c3886
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2935781 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d01989c0be57d0ed337380be90ad3506c81be6e3aa597bd8995beba68e1d0db6`

```dockerfile
```

-	Layers:
	-	`sha256:dda34e9d239e0f568ac1f002f5558a3df3b17808ae8452fca178e58ccd29a89a`  
		Last Modified: Wed, 20 Dec 2023 20:15:01 GMT  
		Size: 2.9 MB (2919368 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:a028fa4b00c706ec49caba862039597fb98811d86506e839701cbe1479623bd1`  
		Last Modified: Wed, 20 Dec 2023 20:15:01 GMT  
		Size: 16.4 KB (16413 bytes)  
		MIME: application/vnd.in-toto+json

### `perl:5-slim-buster` - linux; arm variant v7

```console
$ docker pull perl@sha256:43ed2fdc45295b760392888d902382029bffb9dabcbfe1376c09d9df664bf889
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.7 MB (46686307 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55422454e7526b745d0d4d99ed7dd2109f045e981882d35ae8a4cc5a60606835`
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
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        zlib1g-dev        xz-utils        libssl-dev     && curl -fL https://www.cpan.org/src/5.0/perl-5.38.2.tar.xz -o perl-5.38.2.tar.xz     && echo 'd91115e90b896520e83d4de6b52f8254ef2b70a8d545ffab33200ea9f1cf29e8 *perl-5.38.2.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.38.2.tar.xz -C /usr/src/perl     && rm perl-5.38.2.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && savedPackages="ca-certificates make netbase zlib1g-dev libssl-dev"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version # buildkit
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
	-	`sha256:3add16c2db6e9fc2df9f24f966f721d54038818e5ba3913c8da7b7526c525e87`  
		Last Modified: Thu, 21 Dec 2023 00:05:08 GMT  
		Size: 23.9 MB (23890237 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9f957887700ea79707034cdd3384ba7a5cc276c5c21d752086dca891acd5f657`  
		Last Modified: Thu, 21 Dec 2023 00:05:06 GMT  
		Size: 132.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `perl:5-slim-buster` - unknown; unknown

```console
$ docker pull perl@sha256:daceb93397ca431ca99ce6269a224841492ad593bd8d1fd72aa554992e148849
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2914728 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f44d2c05475084008701b33bfc1adde1444a302922e087f3afb1c8cd3515432e`

```dockerfile
```

-	Layers:
	-	`sha256:f3a132e267f14149e4d1765bf855050a4f580ba5a399530ae9dc064a73d65b5c`  
		Last Modified: Thu, 21 Dec 2023 00:05:07 GMT  
		Size: 2.9 MB (2898402 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:5bb7304b50e068dcc49b04a5150219887c44b8e28c8acaa356117f736253620f`  
		Last Modified: Thu, 21 Dec 2023 00:05:06 GMT  
		Size: 16.3 KB (16326 bytes)  
		MIME: application/vnd.in-toto+json

### `perl:5-slim-buster` - linux; arm64 variant v8

```console
$ docker pull perl@sha256:ec832fab68929b6a86c8e81dd44a132f9c6079addcab33bc4317c6a2f7b4c272
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.9 MB (51917719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1447d8126b7d55a0f5f77c1d8bd28fe09c340e71956250570287b2980101ddf0`
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
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        zlib1g-dev        xz-utils        libssl-dev     && curl -fL https://www.cpan.org/src/5.0/perl-5.38.2.tar.xz -o perl-5.38.2.tar.xz     && echo 'd91115e90b896520e83d4de6b52f8254ef2b70a8d545ffab33200ea9f1cf29e8 *perl-5.38.2.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.38.2.tar.xz -C /usr/src/perl     && rm perl-5.38.2.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && savedPackages="ca-certificates make netbase zlib1g-dev libssl-dev"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version # buildkit
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
	-	`sha256:497ed160f6858b5172521fe6b1b5108035aad308c3c65cd7b95303b85127b8b6`  
		Last Modified: Wed, 20 Dec 2023 23:41:49 GMT  
		Size: 25.9 MB (25947624 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0bc20c9d55115af1557b6352c8d6e88e655ea1c25c26fee9499d3dc35b63153c`  
		Last Modified: Wed, 20 Dec 2023 23:41:48 GMT  
		Size: 133.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `perl:5-slim-buster` - unknown; unknown

```console
$ docker pull perl@sha256:273a8ef17b02b1bca88385b8cfc0ae067e2fb17752305285711556674141dd02
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2909340 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa5a3bccd06b93b297d43496c3a0315cd7bd781103e8833f362aa0b35a997cf5`

```dockerfile
```

-	Layers:
	-	`sha256:323d2b3fc9aa5c15d2fa6fcffda0fc004c04004a35e2ab04ae681d66176106cc`  
		Last Modified: Wed, 20 Dec 2023 23:41:48 GMT  
		Size: 2.9 MB (2893080 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:a772fb440a2b68573112673c0bf254578defbc051edc85e0c432c8bcc96fd142`  
		Last Modified: Wed, 20 Dec 2023 23:41:48 GMT  
		Size: 16.3 KB (16260 bytes)  
		MIME: application/vnd.in-toto+json

### `perl:5-slim-buster` - linux; 386

```console
$ docker pull perl@sha256:8a796a4d7b1f7558ed08e2c5ff3270a658d277e0295f6ab411df7d7ea6f1a8db
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.3 MB (59281520 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67e3a5ccded5213e188c336c7a460e909d301d85265b0ed47fff0c75502d5fbf`
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
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        zlib1g-dev        xz-utils        libssl-dev     && curl -fL https://www.cpan.org/src/5.0/perl-5.38.2.tar.xz -o perl-5.38.2.tar.xz     && echo 'd91115e90b896520e83d4de6b52f8254ef2b70a8d545ffab33200ea9f1cf29e8 *perl-5.38.2.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.38.2.tar.xz -C /usr/src/perl     && rm perl-5.38.2.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && savedPackages="ca-certificates make netbase zlib1g-dev libssl-dev"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version # buildkit
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
	-	`sha256:80bc387be15bc8f69a0e3389525d6610ac71311ee0c35dd6f2d7b7a326ee3205`  
		Last Modified: Wed, 20 Dec 2023 20:15:44 GMT  
		Size: 135.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8b1bebff38ce5cc5ab78f56640f5fb6cf1a6ad4bc538bc092878457c3c161d7f`  
		Last Modified: Wed, 20 Dec 2023 20:15:45 GMT  
		Size: 31.4 MB (31434370 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:90113836f728a94d73a54a246e11f29837f830accdf552d9c5a39cf577866c84`  
		Last Modified: Wed, 20 Dec 2023 20:15:44 GMT  
		Size: 132.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `perl:5-slim-buster` - unknown; unknown

```console
$ docker pull perl@sha256:ed42adc3224269bda87b6fe3d30a8fc475099cbec6d2d899fbbe451d6da38c95
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.2 KB (16166 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18e00b57b078b0aba1007187b4918029b5c791ed60fa9f5a122f91fa6516d9b2`

```dockerfile
```

-	Layers:
	-	`sha256:25d4e2de4a508b48e6188a86bcbc28792ae0f3208614a05fbc44253d62ac0326`  
		Last Modified: Wed, 20 Dec 2023 20:15:44 GMT  
		Size: 16.2 KB (16166 bytes)  
		MIME: application/vnd.in-toto+json
