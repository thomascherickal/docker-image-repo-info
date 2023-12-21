## `perl:slim-threaded-bullseye`

```console
$ docker pull perl@sha256:6bd0f71db87b39661d301cf5761921e85cf24d981283bb8423482d13cdcd892b
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 13
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm variant v5
	-	unknown; unknown
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	unknown; unknown
	-	linux; mips64le
	-	linux; ppc64le
	-	unknown; unknown
	-	linux; s390x
	-	unknown; unknown

### `perl:slim-threaded-bullseye` - linux; amd64

```console
$ docker pull perl@sha256:063ed075bcc73a7d5b7b40745d25cb6c9e582306ee443830b66080f7d9000827
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.8 MB (55828203 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff17f70767cfbdd064929e0b8bcf9db4d7cd29ce42ecc53b146cfbaf7b44f2b5`
-	Default Command: `["perl5.38.2","-de0"]`

```dockerfile
# Thu, 30 Nov 2023 02:54:02 GMT
ADD file:bb44d67b03db8efaeb0c4171474f441d14ff35f328f13add32b289fca062fa2f in / 
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
	-	`sha256:b5a0d5c14ba9ece1eecd5137c468d9a123372b0af2ed2c8c4446137730c90e5b`  
		Last Modified: Tue, 19 Dec 2023 01:25:40 GMT  
		Size: 31.4 MB (31417873 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b99b952c792d2f2a2d494ff8893a0c41a849d01a25f972bb859fab2688b7d7d4`  
		Last Modified: Wed, 20 Dec 2023 20:16:12 GMT  
		Size: 136.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9c88f77afae4b07576c7c0912a2dd3cb60eefc1a14cf02c2cec80885736630c9`  
		Last Modified: Wed, 20 Dec 2023 20:16:13 GMT  
		Size: 24.4 MB (24410062 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a16187fa59065cdb15c35edb67d029492cc6dd571ede974189fcd8501bc5484d`  
		Last Modified: Wed, 20 Dec 2023 20:16:12 GMT  
		Size: 132.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `perl:slim-threaded-bullseye` - unknown; unknown

```console
$ docker pull perl@sha256:bda63ee81f1aa499e35ba6d5fb2e2d0d7b95f62401997c3a5fc4e965c4e28c44
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.3 MB (3312757 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f2d378cd75b08dbd281df3a202b1d0d0fb34b486fbd4f922106f225e96eff73a`

```dockerfile
```

-	Layers:
	-	`sha256:72bc7d779217f8e9b79012f089559df919ec7cc3137e9a4b6558e5c50c480046`  
		Last Modified: Wed, 20 Dec 2023 20:16:12 GMT  
		Size: 3.3 MB (3296169 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:d085a982947a411ef10a3bb025ff9f01f573f7498ad4ca370b6405044e42f827`  
		Last Modified: Wed, 20 Dec 2023 20:16:12 GMT  
		Size: 16.6 KB (16588 bytes)  
		MIME: application/vnd.in-toto+json

### `perl:slim-threaded-bullseye` - linux; arm variant v5

```console
$ docker pull perl@sha256:f9c5aac75f861510fc83fd5568011e97c479b319f5c8fd223f1dc2066ce2ae7b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.3 MB (51317565 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:25e0b36bb5005d9fcecc27e0a26f6a092fe5d36cfb797cf3eff5e4c959947f52`
-	Default Command: `["perl5.38.2","-de0"]`

```dockerfile
# Thu, 30 Nov 2023 02:54:02 GMT
ADD file:831966ecbc1ad85566dda1f3580cd9306cc099069cd418506e8befd03c296d1c in / 
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
	-	`sha256:fdebea600ba5b47ddd94c41d9d687679a030fdad563a3490945a5433dae01d54`  
		Last Modified: Tue, 19 Dec 2023 01:59:22 GMT  
		Size: 28.9 MB (28921283 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:03d09100782a58afba16874286ee30ec7285f79cc6f039986cfc2cdccfd58f84`  
		Last Modified: Wed, 20 Dec 2023 21:16:53 GMT  
		Size: 135.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5e020999a34e93329375322e8c8d8e49837e54ccdccf115f39f2f0df53e2917c`  
		Last Modified: Wed, 20 Dec 2023 21:47:44 GMT  
		Size: 22.4 MB (22396015 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1405870eab16b04fae240078d42e468cdbfa77514156eb20a1790675ca4bc7c3`  
		Last Modified: Wed, 20 Dec 2023 21:47:43 GMT  
		Size: 132.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `perl:slim-threaded-bullseye` - unknown; unknown

```console
$ docker pull perl@sha256:706d1cbd1004b724356ffaa754900d8f74d6ca4f82f657b76ae35236445d42f5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.3 KB (16284 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c55776b90bb9e2f2c3fa1f8708075005f73efb274a28b5cc6e84ae8141b1bd5`

```dockerfile
```

-	Layers:
	-	`sha256:912123385278ebbe310aab335e77e74ffc898c3d83a00f4d054d1597e09b71e9`  
		Last Modified: Wed, 20 Dec 2023 21:47:43 GMT  
		Size: 16.3 KB (16284 bytes)  
		MIME: application/vnd.in-toto+json

### `perl:slim-threaded-bullseye` - linux; arm variant v7

```console
$ docker pull perl@sha256:e705392d176589b71d3693d80abf05afcf323314c5db49cf9d45d1272c6fa3cf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.6 MB (48574090 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aaaafdd6c98f9f4ceacc1592e0f98e4fb53fe049ea721d28d648625aac94d6b1`
-	Default Command: `["perl5.38.2","-de0"]`

```dockerfile
# Tue, 19 Dec 2023 02:08:09 GMT
ADD file:496e70a34ff4dabb4eefdf40e4e2f0563bea0c120bb43206f8f52ab5a887b637 in / 
# Tue, 19 Dec 2023 02:08:09 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 03:01:23 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Tue, 19 Dec 2023 03:01:24 GMT
WORKDIR /usr/src/perl
# Tue, 19 Dec 2023 03:27:40 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        zlib1g-dev        xz-utils        libssl-dev     && curl -fL https://www.cpan.org/src/5.0/perl-5.38.2.tar.xz -o perl-5.38.2.tar.xz     && echo 'd91115e90b896520e83d4de6b52f8254ef2b70a8d545ffab33200ea9f1cf29e8 *perl-5.38.2.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.38.2.tar.xz -C /usr/src/perl     && rm perl-5.38.2.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && savedPackages="ca-certificates make netbase zlib1g-dev libssl-dev"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Tue, 19 Dec 2023 03:27:40 GMT
WORKDIR /usr/src/app
# Tue, 19 Dec 2023 03:27:40 GMT
CMD ["perl5.38.2" "-de0"]
```

-	Layers:
	-	`sha256:19ccf4d6cc6956e4a5522352be94632923aa376a9939a4f45428a4f304c73bc8`  
		Last Modified: Tue, 19 Dec 2023 02:12:33 GMT  
		Size: 26.6 MB (26578972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26c286cb551548b19ceb8e117a918ddb8916687aa0a647c8017024092967ca62`  
		Last Modified: Tue, 19 Dec 2023 05:03:17 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7f2b701d63f8e667a0d9936bdc0ec91ded36ceb44e7053f463ad9ad71c4a9cf`  
		Last Modified: Tue, 19 Dec 2023 05:04:50 GMT  
		Size: 22.0 MB (21994782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16bb2c920fb5bb261d5c66c98e26c5db5028657242b90c7049ec9c92bb321802`  
		Last Modified: Tue, 19 Dec 2023 05:04:42 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:slim-threaded-bullseye` - linux; arm64 variant v8

```console
$ docker pull perl@sha256:1506362bdabbeba21d01a2ed5725cf3f3eecad336a155c1af3388011d98723da
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.8 MB (53789303 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10dda0388bdbfd8e8a42ba3578d90c8c2b8d5200194e37d1e11c846e12443b94`
-	Default Command: `["perl5.38.2","-de0"]`

```dockerfile
# Tue, 19 Dec 2023 01:41:25 GMT
ADD file:4dd1c5e17a5e57644787f37e8ad290baef6c93f4f112b976f19136480a293713 in / 
# Tue, 19 Dec 2023 01:41:25 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 07:54:33 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Tue, 19 Dec 2023 07:54:33 GMT
WORKDIR /usr/src/perl
# Tue, 19 Dec 2023 08:14:01 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        zlib1g-dev        xz-utils        libssl-dev     && curl -fL https://www.cpan.org/src/5.0/perl-5.38.2.tar.xz -o perl-5.38.2.tar.xz     && echo 'd91115e90b896520e83d4de6b52f8254ef2b70a8d545ffab33200ea9f1cf29e8 *perl-5.38.2.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.38.2.tar.xz -C /usr/src/perl     && rm perl-5.38.2.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && savedPackages="ca-certificates make netbase zlib1g-dev libssl-dev"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Tue, 19 Dec 2023 08:14:01 GMT
WORKDIR /usr/src/app
# Tue, 19 Dec 2023 08:14:01 GMT
CMD ["perl5.38.2" "-de0"]
```

-	Layers:
	-	`sha256:2244706f264b35566276550fbc21ada79613ddfff850e372b8f5113110a67c93`  
		Last Modified: Tue, 19 Dec 2023 01:45:22 GMT  
		Size: 30.1 MB (30064052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db9a66f10dc01a0494eaade34f1ef8ddb160d233ef7052d6b662265be71125fd`  
		Last Modified: Tue, 19 Dec 2023 09:29:00 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3704283b12aef84fee6f58dd72ad52329eae50fa1527b20e75a6093b6ba329f0`  
		Last Modified: Tue, 19 Dec 2023 09:30:12 GMT  
		Size: 23.7 MB (23724917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c937920eaf81424d7fdc7a09c7aafbbd2cbf520e2d6b801d84389e6de33be4b0`  
		Last Modified: Tue, 19 Dec 2023 09:30:09 GMT  
		Size: 165.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:slim-threaded-bullseye` - linux; 386

```console
$ docker pull perl@sha256:cfe8357706c2cf4305d2471994dac414cf6f25bd65fbf1962e992773f1e99866
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.3 MB (58268906 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f70821d30eadcfca860f0f83f0fa99ac1a4f992cde563e3925aec0962734dfa`
-	Default Command: `["perl5.38.2","-de0"]`

```dockerfile
# Thu, 30 Nov 2023 02:54:02 GMT
ADD file:e9c344f1bffba57e46b30e3c70e4247dcf2e9d3e0484b2768f83ffd789bf3686 in / 
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
	-	`sha256:e5808d881ded1b1deb8675903e6776c5a725d22c8a5c1061a96c74338f07591f`  
		Last Modified: Tue, 19 Dec 2023 01:44:31 GMT  
		Size: 32.4 MB (32402688 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:33a23b49fffe6ae27dcecb53d07913e1e61e944aec4194049fd21a0e7ec00eba`  
		Last Modified: Wed, 20 Dec 2023 20:16:37 GMT  
		Size: 136.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9a6c2acd1c13f5620b706d4a3471d7bd90e2ca852e3868daeedaa2aefa6debfa`  
		Last Modified: Wed, 20 Dec 2023 20:16:37 GMT  
		Size: 25.9 MB (25865950 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c5e82417d52c704e206ac441eed2ad083c2107093f2af218dd2298ac0ea06404`  
		Last Modified: Wed, 20 Dec 2023 20:16:37 GMT  
		Size: 132.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `perl:slim-threaded-bullseye` - unknown; unknown

```console
$ docker pull perl@sha256:6e1563e905f2a253d4bd00e76faa5b7545eda75ba692c8fd68c2402cf2e853cc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.3 KB (16339 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:344e8f21756f0bc397731777443791f1acada622345decaba24342c68f24bc0a`

```dockerfile
```

-	Layers:
	-	`sha256:6a3f3d75ccb9c3590244e8fb3b87d1a02f63bcf440a56fe68f67e65c4034c33d`  
		Last Modified: Wed, 20 Dec 2023 20:16:37 GMT  
		Size: 16.3 KB (16339 bytes)  
		MIME: application/vnd.in-toto+json

### `perl:slim-threaded-bullseye` - linux; mips64le

```console
$ docker pull perl@sha256:c441ee771eb4b9df2e70e8b809594cd43513050a90e3e083ecf4aa39407df2a6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.0 MB (52961589 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f911517fd8ef0e6a9c42e51175e90018f87bb48c7a21e798ab1163e61b32d2b1`
-	Default Command: `["perl5.38.2","-de0"]`

```dockerfile
# Tue, 19 Dec 2023 02:14:50 GMT
ADD file:dcc77071aa6c677714230fd845d154c00ba6ba34a78f8f1073c224e90f17f543 in / 
# Tue, 19 Dec 2023 02:14:54 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 08:38:29 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Tue, 19 Dec 2023 08:38:32 GMT
WORKDIR /usr/src/perl
# Tue, 19 Dec 2023 10:42:57 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        zlib1g-dev        xz-utils        libssl-dev     && curl -fL https://www.cpan.org/src/5.0/perl-5.38.2.tar.xz -o perl-5.38.2.tar.xz     && echo 'd91115e90b896520e83d4de6b52f8254ef2b70a8d545ffab33200ea9f1cf29e8 *perl-5.38.2.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.38.2.tar.xz -C /usr/src/perl     && rm perl-5.38.2.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && savedPackages="ca-certificates make netbase zlib1g-dev libssl-dev"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Tue, 19 Dec 2023 10:43:01 GMT
WORKDIR /usr/src/app
# Tue, 19 Dec 2023 10:43:04 GMT
CMD ["perl5.38.2" "-de0"]
```

-	Layers:
	-	`sha256:f9454980ac665cb2d7641130c738c2054ef7a7516386fc6742b46b5b60dd93ad`  
		Last Modified: Tue, 19 Dec 2023 02:26:03 GMT  
		Size: 29.6 MB (29635982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e77af2a7a5dfb91c67e1d5e3c335e45941699e136408d2ea94a308750b16a4ef`  
		Last Modified: Tue, 19 Dec 2023 19:16:53 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc463581405037b1a44ee461a4de1c90b22edae6db835f982877ccb36026202b`  
		Last Modified: Tue, 19 Dec 2023 19:19:59 GMT  
		Size: 23.3 MB (23325339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5f6c116de2a9d9cf652ad963497032ad25126b31f11b34062c5d19a5aa59512`  
		Last Modified: Tue, 19 Dec 2023 19:19:38 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:slim-threaded-bullseye` - linux; ppc64le

```console
$ docker pull perl@sha256:310378c76927c4f8803eaaf7f8d8ded62ff8dc2fe0c8f2a8f1e7f6255a619e5a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.0 MB (59984344 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab95d467f8c114f2dc02fb12042f483c6730b06623f7fc9c203868d4cd74e791`
-	Default Command: `["perl5.38.2","-de0"]`

```dockerfile
# Thu, 30 Nov 2023 02:54:02 GMT
ADD file:1cb772a6ad8ca6301624db3141029490564de7673bc0f2d4bedb5a1578ea85bd in / 
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
	-	`sha256:c9f6fac7f65cfc65b7f8de8bc377b135ca95e45a3246cf2bd1bb90922679553e`  
		Last Modified: Tue, 19 Dec 2023 01:27:11 GMT  
		Size: 35.3 MB (35293807 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f11036b9609acf58122ae19b79e91c30e52886036c3305dceb4d0139ce911ebd`  
		Last Modified: Wed, 20 Dec 2023 21:52:30 GMT  
		Size: 136.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:81b19a39f9b32f8de4fe96bc74763eb9b286e43c4d354829b66009ec358edb7d`  
		Last Modified: Wed, 20 Dec 2023 22:40:37 GMT  
		Size: 24.7 MB (24690268 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7735ca13710de2ff9634dd8a7fbc3a3953274cf772dd854be5971100365db127`  
		Last Modified: Wed, 20 Dec 2023 22:40:36 GMT  
		Size: 133.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `perl:slim-threaded-bullseye` - unknown; unknown

```console
$ docker pull perl@sha256:91912e3686a08b2d65e0a3cda6101606875c6629c62a91a85cc8caa9c47b5596
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.3 MB (3303840 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b10d7693d4cfcce94cf7cb0a0cdf7222dde45110077299b12dab5954698fccff`

```dockerfile
```

-	Layers:
	-	`sha256:61f8919ac6cd85e7cb02f0b767ccf2ea0c520394ed8f75260d923e9d092e9073`  
		Last Modified: Wed, 20 Dec 2023 22:40:36 GMT  
		Size: 3.3 MB (3287376 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:39611e769d8cdec48f69104da0b3a86b0171f7313a1b5f80703ec223a8374dfe`  
		Last Modified: Wed, 20 Dec 2023 22:40:36 GMT  
		Size: 16.5 KB (16464 bytes)  
		MIME: application/vnd.in-toto+json

### `perl:slim-threaded-bullseye` - linux; s390x

```console
$ docker pull perl@sha256:e8cca8d2846fffd40136c8a6f46a538baf897ab1695f562fc584d6da943793cf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.3 MB (53285779 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e9ff71472f03a70ade7bb4622d9eb711cfc70a2698e5aed94635449119c6570`
-	Default Command: `["perl5.38.2","-de0"]`

```dockerfile
# Thu, 30 Nov 2023 02:54:02 GMT
ADD file:36a070457acddafcd6cdda22a3c41efcbd4e2b1694831eb74c8143520ebf1cf2 in / 
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
	-	`sha256:eff2a4367cf88d5103011eba9299da2b4d173b0bde5dc0455020febf72b9b1c4`  
		Last Modified: Tue, 19 Dec 2023 01:48:08 GMT  
		Size: 29.7 MB (29657006 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:92d9a7afb7027beec55ffdfc75a29a35a4bb7ce6beeb518238f728fda590fddd`  
		Last Modified: Wed, 20 Dec 2023 21:57:22 GMT  
		Size: 135.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6120d20bac9294c97c05750571527e760e11fef6a857bfca29fa9a6462688bd3`  
		Last Modified: Wed, 20 Dec 2023 22:42:51 GMT  
		Size: 23.6 MB (23628508 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bf975906794f1ab378c8cfe7ed2a02c57f4c44c3556cc7cecfb405b2dc051e6c`  
		Last Modified: Wed, 20 Dec 2023 22:42:50 GMT  
		Size: 130.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `perl:slim-threaded-bullseye` - unknown; unknown

```console
$ docker pull perl@sha256:7f1f70c981884c1fdee107c2e6a882daf547c050d6359161c09b10ab0c7e07e7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.3 MB (3302672 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a896e4e5d3ad38a433f9bdcd766d57b84c04187fbb8217ce20479febddc4e990`

```dockerfile
```

-	Layers:
	-	`sha256:e08aee58d67ef9bc72722893d466cd6027b57b8d0e3969840fc51ad24a7190dd`  
		Last Modified: Wed, 20 Dec 2023 22:42:50 GMT  
		Size: 3.3 MB (3286251 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:a4d23734886b0200731a7d2a99dcde95869729fd3989101688812f1bcca58a7e`  
		Last Modified: Wed, 20 Dec 2023 22:42:50 GMT  
		Size: 16.4 KB (16421 bytes)  
		MIME: application/vnd.in-toto+json
