## `perl:devel-slim-bullseye`

```console
$ docker pull perl@sha256:5d37ac5a68e3698ca6ecb11a98eaa6199d724be05753f28b78696971f36e9538
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 10
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	unknown; unknown
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `perl:devel-slim-bullseye` - linux; amd64

```console
$ docker pull perl@sha256:93b550d1f1e4068f2af6a7dec9bedca0617014911e474c0bf3ccf3c071f5c528
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.0 MB (55952568 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a625579bb511c947b1cd0d58e5b39d4f917bce178673e7115187f84ddabef71c`
-	Default Command: `["perl5.39.5","-de0"]`

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
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        zlib1g-dev        xz-utils        libssl-dev     && curl -fL https://www.cpan.org/src/5.0/perl-5.39.5.tar.xz -o perl-5.39.5.tar.xz     && echo '4048cf0065f347a03ec85e989631a64e03ba9c9ccbc8f2a35153cad07fe21930 *perl-5.39.5.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.39.5.tar.xz -C /usr/src/perl     && rm perl-5.39.5.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local -Dusedevel -Dversiononly=undef -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && savedPackages="ca-certificates make netbase zlib1g-dev libssl-dev"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version # buildkit
# Thu, 30 Nov 2023 02:54:02 GMT
WORKDIR /usr/src/app
# Thu, 30 Nov 2023 02:54:02 GMT
CMD ["perl5.39.5" "-de0"]
```

-	Layers:
	-	`sha256:b5a0d5c14ba9ece1eecd5137c468d9a123372b0af2ed2c8c4446137730c90e5b`  
		Last Modified: Tue, 19 Dec 2023 01:25:40 GMT  
		Size: 31.4 MB (31417873 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:eefcdf50595e4db0997009fa85e46c15d8976b7499cbcfb16defd7f10abbaa9f`  
		Last Modified: Wed, 20 Dec 2023 20:23:41 GMT  
		Size: 136.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4ce83d3a8e3b53d4aaed28464d27d89d6096c6cbde227988474bb2633b785bf2`  
		Last Modified: Wed, 20 Dec 2023 20:23:42 GMT  
		Size: 24.5 MB (24534427 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:838a540ec921b6189600efd9429460e63742904781fb312b773a03085a31980f`  
		Last Modified: Wed, 20 Dec 2023 20:23:41 GMT  
		Size: 132.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `perl:devel-slim-bullseye` - unknown; unknown

```console
$ docker pull perl@sha256:3e2dcaeab65fff4ac5268b4559a22d5a8202aab07b1ff897c7e99218f0518912
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.3 MB (3311351 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab4585162c209a6602d8b8dc8b1adf1b1ff5b5f7dca468c09cc0ddc2e9bec0d1`

```dockerfile
```

-	Layers:
	-	`sha256:a9538d1723bfd064566cbb36c1797c5f793a0ebef1135ba8e96f4edddf6cef42`  
		Last Modified: Wed, 20 Dec 2023 20:23:42 GMT  
		Size: 3.3 MB (3295457 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:781a767a20fc37717504e604da9650a870fc35efd292a58a5ff3c973eb4863ba`  
		Last Modified: Wed, 20 Dec 2023 20:23:41 GMT  
		Size: 15.9 KB (15894 bytes)  
		MIME: application/vnd.in-toto+json

### `perl:devel-slim-bullseye` - linux; arm variant v5

```console
$ docker pull perl@sha256:c35ec599d247299b87f8ff759b09681be4662622cce996c422aba841494fb0c9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.7 MB (51687986 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0cc069863404323dc2569f55eb1978da50b177b2583a6f8d02f414ac3718d2c8`
-	Default Command: `["perl5.39.5","-de0"]`

```dockerfile
# Tue, 19 Dec 2023 01:55:38 GMT
ADD file:831966ecbc1ad85566dda1f3580cd9306cc099069cd418506e8befd03c296d1c in / 
# Tue, 19 Dec 2023 01:55:38 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 05:57:25 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Tue, 19 Dec 2023 05:57:25 GMT
WORKDIR /usr/src/perl
# Tue, 19 Dec 2023 08:09:41 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        zlib1g-dev        xz-utils        libssl-dev     && curl -fL https://www.cpan.org/src/5.0/perl-5.39.5.tar.xz -o perl-5.39.5.tar.xz     && echo '4048cf0065f347a03ec85e989631a64e03ba9c9ccbc8f2a35153cad07fe21930 *perl-5.39.5.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.39.5.tar.xz -C /usr/src/perl     && rm perl-5.39.5.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local -Dusedevel -Dversiononly=undef -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && savedPackages="ca-certificates make netbase zlib1g-dev libssl-dev"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Tue, 19 Dec 2023 08:09:41 GMT
WORKDIR /usr/src/app
# Tue, 19 Dec 2023 08:09:41 GMT
CMD ["perl5.39.5" "-de0"]
```

-	Layers:
	-	`sha256:fdebea600ba5b47ddd94c41d9d687679a030fdad563a3490945a5433dae01d54`  
		Last Modified: Tue, 19 Dec 2023 01:59:22 GMT  
		Size: 28.9 MB (28921283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55634b1b9ec91a98daf6acd7ab7671c4045f8bb9a30c22c1fbef3fc9bc2564ae`  
		Last Modified: Tue, 19 Dec 2023 08:37:49 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:636947247d3087d8ef820f4e6aeba507043fd5bf38de478af38ab9d7d2e27bd4`  
		Last Modified: Tue, 19 Dec 2023 08:44:25 GMT  
		Size: 22.8 MB (22766370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1172b5a7700bc58f39aca21e7e92fe2a9243b9c70fba0051f7f71a1b287b2a7`  
		Last Modified: Tue, 19 Dec 2023 08:44:17 GMT  
		Size: 164.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:devel-slim-bullseye` - linux; arm variant v7

```console
$ docker pull perl@sha256:18e641e6b6b2348b37af65e63c2dde2cb200737ef87ec1f2330771565cf690cb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.7 MB (48741271 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:991e4bd46eec13dd742eb07a1a00acafde73abd3fcef8809c29e751c081a3449`
-	Default Command: `["perl5.39.5","-de0"]`

```dockerfile
# Tue, 19 Dec 2023 02:08:09 GMT
ADD file:496e70a34ff4dabb4eefdf40e4e2f0563bea0c120bb43206f8f52ab5a887b637 in / 
# Tue, 19 Dec 2023 02:08:09 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 03:01:23 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Tue, 19 Dec 2023 03:01:24 GMT
WORKDIR /usr/src/perl
# Tue, 19 Dec 2023 04:49:07 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        zlib1g-dev        xz-utils        libssl-dev     && curl -fL https://www.cpan.org/src/5.0/perl-5.39.5.tar.xz -o perl-5.39.5.tar.xz     && echo '4048cf0065f347a03ec85e989631a64e03ba9c9ccbc8f2a35153cad07fe21930 *perl-5.39.5.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.39.5.tar.xz -C /usr/src/perl     && rm perl-5.39.5.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local -Dusedevel -Dversiononly=undef -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && savedPackages="ca-certificates make netbase zlib1g-dev libssl-dev"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Tue, 19 Dec 2023 04:49:08 GMT
WORKDIR /usr/src/app
# Tue, 19 Dec 2023 04:49:08 GMT
CMD ["perl5.39.5" "-de0"]
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
	-	`sha256:0e37eaa9f6c0c76e049ce3cfdd4c447abd021e69fee7390211a681ac1b148d97`  
		Last Modified: Tue, 19 Dec 2023 05:08:53 GMT  
		Size: 22.2 MB (22161964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de41618e5219e6442b49ee80c4d5f7085fa51d9d3c2b957f06f48ff89c861c37`  
		Last Modified: Tue, 19 Dec 2023 05:08:49 GMT  
		Size: 165.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:devel-slim-bullseye` - linux; arm64 variant v8

```console
$ docker pull perl@sha256:4a72bdbc66d658b47b4fda9f6d4f33b3d226763c8e7ad2fc1be5375501438a05
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.9 MB (53949950 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c0784b2e73b4e42cc3154230223d6b20cadcdb62189b580b1244bf113dda708`
-	Default Command: `["perl5.39.5","-de0"]`

```dockerfile
# Tue, 19 Dec 2023 01:41:25 GMT
ADD file:4dd1c5e17a5e57644787f37e8ad290baef6c93f4f112b976f19136480a293713 in / 
# Tue, 19 Dec 2023 01:41:25 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 07:54:33 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Tue, 19 Dec 2023 07:54:33 GMT
WORKDIR /usr/src/perl
# Tue, 19 Dec 2023 09:16:59 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        zlib1g-dev        xz-utils        libssl-dev     && curl -fL https://www.cpan.org/src/5.0/perl-5.39.5.tar.xz -o perl-5.39.5.tar.xz     && echo '4048cf0065f347a03ec85e989631a64e03ba9c9ccbc8f2a35153cad07fe21930 *perl-5.39.5.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.39.5.tar.xz -C /usr/src/perl     && rm perl-5.39.5.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local -Dusedevel -Dversiononly=undef -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && savedPackages="ca-certificates make netbase zlib1g-dev libssl-dev"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Tue, 19 Dec 2023 09:17:00 GMT
WORKDIR /usr/src/app
# Tue, 19 Dec 2023 09:17:00 GMT
CMD ["perl5.39.5" "-de0"]
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
	-	`sha256:4ece6d89d2a1a60893f0caf3dc6d94c91f65d04759281c5a8f6fa11e26792e9f`  
		Last Modified: Tue, 19 Dec 2023 09:33:33 GMT  
		Size: 23.9 MB (23885563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4839f28cd00bb30477cf57ca6a7096200edbf6444ff29942c8684b78a1180b5e`  
		Last Modified: Tue, 19 Dec 2023 09:33:29 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:devel-slim-bullseye` - linux; 386

```console
$ docker pull perl@sha256:4b052566f4849db0382cd76088d1b4d8688abdfaf4dbfe9fc7dbd6ffd16ffe20
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.4 MB (58369760 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:390ad4fa89411027b1b9c7c524d597ed9170cc5e695b6af40a277d3851908e9a`
-	Default Command: `["perl5.39.5","-de0"]`

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
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        zlib1g-dev        xz-utils        libssl-dev     && curl -fL https://www.cpan.org/src/5.0/perl-5.39.5.tar.xz -o perl-5.39.5.tar.xz     && echo '4048cf0065f347a03ec85e989631a64e03ba9c9ccbc8f2a35153cad07fe21930 *perl-5.39.5.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.39.5.tar.xz -C /usr/src/perl     && rm perl-5.39.5.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local -Dusedevel -Dversiononly=undef -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && savedPackages="ca-certificates make netbase zlib1g-dev libssl-dev"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version # buildkit
# Thu, 30 Nov 2023 02:54:02 GMT
WORKDIR /usr/src/app
# Thu, 30 Nov 2023 02:54:02 GMT
CMD ["perl5.39.5" "-de0"]
```

-	Layers:
	-	`sha256:e5808d881ded1b1deb8675903e6776c5a725d22c8a5c1061a96c74338f07591f`  
		Last Modified: Tue, 19 Dec 2023 01:44:31 GMT  
		Size: 32.4 MB (32402688 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2cc8115c85fda6dbf7d430ce10e20eace5e757511ccf4515780a67c904104ae3`  
		Last Modified: Wed, 20 Dec 2023 20:24:29 GMT  
		Size: 136.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:199a1aa72a1e89a34af9d0ad5d953fe5a92482f6dda1d884f4fcaeb3308de567`  
		Last Modified: Wed, 20 Dec 2023 20:24:30 GMT  
		Size: 26.0 MB (25966804 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fb8afdbbf23c6effa9e26e236324cf680b829d7eb5726df1113ea7056d00c4c1`  
		Last Modified: Wed, 20 Dec 2023 20:24:29 GMT  
		Size: 132.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `perl:devel-slim-bullseye` - unknown; unknown

```console
$ docker pull perl@sha256:4b1b104d4dead50e158d018747103a331d14ea323194a76531b75830ca2a9e66
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.7 KB (15656 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9bf1560b9bde55c6a0e5748906e377e703fa6a11874fdd5d63cccbd062b60cce`

```dockerfile
```

-	Layers:
	-	`sha256:98d2e960ee8de5e000eb4ef26a25614b8dddd72026187d7d597b716fcc54b95a`  
		Last Modified: Wed, 20 Dec 2023 20:24:29 GMT  
		Size: 15.7 KB (15656 bytes)  
		MIME: application/vnd.in-toto+json

### `perl:devel-slim-bullseye` - linux; mips64le

```console
$ docker pull perl@sha256:d1c6996f80d16c65adb774d787f1eb6721447d814826e0a35ac078594319d70e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.1 MB (53084289 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6ca210dce66bb4155577eff2b86cda5538194494843ff253f978ef3013b1246`
-	Default Command: `["perl5.39.5","-de0"]`

```dockerfile
# Tue, 19 Dec 2023 02:14:50 GMT
ADD file:dcc77071aa6c677714230fd845d154c00ba6ba34a78f8f1073c224e90f17f543 in / 
# Tue, 19 Dec 2023 02:14:54 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 08:38:29 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Tue, 19 Dec 2023 08:38:32 GMT
WORKDIR /usr/src/perl
# Tue, 19 Dec 2023 17:29:32 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        zlib1g-dev        xz-utils        libssl-dev     && curl -fL https://www.cpan.org/src/5.0/perl-5.39.5.tar.xz -o perl-5.39.5.tar.xz     && echo '4048cf0065f347a03ec85e989631a64e03ba9c9ccbc8f2a35153cad07fe21930 *perl-5.39.5.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.39.5.tar.xz -C /usr/src/perl     && rm perl-5.39.5.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local -Dusedevel -Dversiononly=undef -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && savedPackages="ca-certificates make netbase zlib1g-dev libssl-dev"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Tue, 19 Dec 2023 17:29:36 GMT
WORKDIR /usr/src/app
# Tue, 19 Dec 2023 17:29:39 GMT
CMD ["perl5.39.5" "-de0"]
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
	-	`sha256:dd45a53d1b711a456c4a735d95fd0331ccba8345717630ed6dcd001302c7fc95`  
		Last Modified: Tue, 19 Dec 2023 19:27:52 GMT  
		Size: 23.4 MB (23448041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dbd859fc98bd45084800670b467ccff39dd58f98eddb49d4009e1b3835ff3d4`  
		Last Modified: Tue, 19 Dec 2023 19:27:33 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:devel-slim-bullseye` - linux; ppc64le

```console
$ docker pull perl@sha256:4732177e77e228544d0b3df3b1612bea24ac07dd883bcf38644394b6456665e1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.3 MB (60295954 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07fa4c4af9bc82bbe5b486623aaf06be98a9a5198d5066df8bc57a43eb421a64`
-	Default Command: `["perl5.39.5","-de0"]`

```dockerfile
# Tue, 19 Dec 2023 01:22:19 GMT
ADD file:1cb772a6ad8ca6301624db3141029490564de7673bc0f2d4bedb5a1578ea85bd in / 
# Tue, 19 Dec 2023 01:22:21 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 02:09:28 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Tue, 19 Dec 2023 02:09:30 GMT
WORKDIR /usr/src/perl
# Tue, 19 Dec 2023 03:26:43 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        zlib1g-dev        xz-utils        libssl-dev     && curl -fL https://www.cpan.org/src/5.0/perl-5.39.5.tar.xz -o perl-5.39.5.tar.xz     && echo '4048cf0065f347a03ec85e989631a64e03ba9c9ccbc8f2a35153cad07fe21930 *perl-5.39.5.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.39.5.tar.xz -C /usr/src/perl     && rm perl-5.39.5.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local -Dusedevel -Dversiononly=undef -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && savedPackages="ca-certificates make netbase zlib1g-dev libssl-dev"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Tue, 19 Dec 2023 03:26:45 GMT
WORKDIR /usr/src/app
# Tue, 19 Dec 2023 03:26:45 GMT
CMD ["perl5.39.5" "-de0"]
```

-	Layers:
	-	`sha256:c9f6fac7f65cfc65b7f8de8bc377b135ca95e45a3246cf2bd1bb90922679553e`  
		Last Modified: Tue, 19 Dec 2023 01:27:11 GMT  
		Size: 35.3 MB (35293807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59fc559dcbd9cd3b3e1b0e1b2c2223b923951f3599845e6c5237585cca0def46`  
		Last Modified: Tue, 19 Dec 2023 03:42:39 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c22110a91118c2f567b9063c567f258db2f99e7a19783088f7d465e8fa9d7d52`  
		Last Modified: Tue, 19 Dec 2023 03:46:24 GMT  
		Size: 25.0 MB (25001813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd35e9136ed7a9b34aa5d3cf8fa529a0592d3d76bae58bea3765e1ba940bbc77`  
		Last Modified: Tue, 19 Dec 2023 03:46:19 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:devel-slim-bullseye` - linux; s390x

```console
$ docker pull perl@sha256:db99be13ec3bd4dd71d9fdaa90447c4ace36f7ebe84a2167571b234c1bac767b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.6 MB (53625917 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1fc21250a141eede98a91c0c9db908a53638f39e8784dd6bd62eacd8cef1d9e0`
-	Default Command: `["perl5.39.5","-de0"]`

```dockerfile
# Tue, 19 Dec 2023 01:43:11 GMT
ADD file:36a070457acddafcd6cdda22a3c41efcbd4e2b1694831eb74c8143520ebf1cf2 in / 
# Tue, 19 Dec 2023 01:43:14 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 02:14:43 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Tue, 19 Dec 2023 02:14:44 GMT
WORKDIR /usr/src/perl
# Tue, 19 Dec 2023 03:28:01 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        zlib1g-dev        xz-utils        libssl-dev     && curl -fL https://www.cpan.org/src/5.0/perl-5.39.5.tar.xz -o perl-5.39.5.tar.xz     && echo '4048cf0065f347a03ec85e989631a64e03ba9c9ccbc8f2a35153cad07fe21930 *perl-5.39.5.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.39.5.tar.xz -C /usr/src/perl     && rm perl-5.39.5.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local -Dusedevel -Dversiononly=undef -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && savedPackages="ca-certificates make netbase zlib1g-dev libssl-dev"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Tue, 19 Dec 2023 03:28:03 GMT
WORKDIR /usr/src/app
# Tue, 19 Dec 2023 03:28:03 GMT
CMD ["perl5.39.5" "-de0"]
```

-	Layers:
	-	`sha256:eff2a4367cf88d5103011eba9299da2b4d173b0bde5dc0455020febf72b9b1c4`  
		Last Modified: Tue, 19 Dec 2023 01:48:08 GMT  
		Size: 29.7 MB (29657006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ab4c45eadd0c841ede4473cd53fababdb1ba62c17b0d007909d0bcc2942960a`  
		Last Modified: Tue, 19 Dec 2023 03:43:57 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3409945de3c04e634bf5c2cd0115219e6bd7a7d79e785b66a000cd80ea260f30`  
		Last Modified: Tue, 19 Dec 2023 03:46:33 GMT  
		Size: 24.0 MB (23968576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:694afc95a4b70992ac33c9f0f45498462a6ce99a025557c96658ab8b670c9bab`  
		Last Modified: Tue, 19 Dec 2023 03:46:28 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
