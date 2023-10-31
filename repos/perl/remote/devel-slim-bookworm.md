## `perl:devel-slim-bookworm`

```console
$ docker pull perl@sha256:c6949e3db9734efabc354a6b539c274c3bc003d5a321c1d5b71637f883f1c37b
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

### `perl:devel-slim-bookworm` - linux; amd64

```console
$ docker pull perl@sha256:78ff5818ffff4e612355cc8fe342fb83c01ce0af3be0d83922a4ad5db0f181b0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.8 MB (57818687 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ae5203ee6c72711be15075bc6059dbfc30d5727a146757ea987a80c28d470e2`
-	Default Command: `["perl5.39.4","-de0"]`

```dockerfile
# Wed, 11 Oct 2023 18:34:50 GMT
ADD file:55ad846fa191e603f48090eae0e4a7149c4066b94406593ec1898ad2c3347937 in / 
# Wed, 11 Oct 2023 18:34:51 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 00:31:42 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Thu, 12 Oct 2023 00:31:42 GMT
WORKDIR /usr/src/perl
# Mon, 30 Oct 2023 23:59:59 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        zlib1g-dev        xz-utils        libssl-dev     && curl -fL https://www.cpan.org/src/5.0/perl-5.39.4.tar.xz -o perl-5.39.4.tar.xz     && echo '73c5e1eb3f125206e82c23e2d03df2c62184d1acc330f99ab7624a3ade19b587 *perl-5.39.4.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.39.4.tar.xz -C /usr/src/perl     && rm perl-5.39.4.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local -Dusedevel -Dversiononly=undef -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && savedPackages="ca-certificates make netbase zlib1g-dev libssl-dev"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Tue, 31 Oct 2023 00:00:00 GMT
WORKDIR /usr/src/app
# Tue, 31 Oct 2023 00:00:00 GMT
CMD ["perl5.39.4" "-de0"]
```

-	Layers:
	-	`sha256:a378f10b321842c3042cdeff4f6997f34f4cb21f2eff27704b7f6193ab7b5fea`  
		Last Modified: Wed, 11 Oct 2023 18:39:34 GMT  
		Size: 29.1 MB (29149874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04ea81aa221f48138364cb21b22f167023c578f29a9243c495eaf70039887bf7`  
		Last Modified: Thu, 12 Oct 2023 02:39:59 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53758f63394bab8b52246d1a083e8b92b462fc07e6f2fe0065da981096a2ac1e`  
		Last Modified: Tue, 31 Oct 2023 00:33:46 GMT  
		Size: 28.7 MB (28668480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d144b901b2c9ff98f26be2ba9dc13039f4bf939ae53c18211e28d6a9744397ac`  
		Last Modified: Tue, 31 Oct 2023 00:33:41 GMT  
		Size: 164.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:devel-slim-bookworm` - linux; arm variant v5

```console
$ docker pull perl@sha256:2f7ace8151c727372dedb9eb5fd994a139803fc7dfb147a0c57fab925d4c62ba
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.7 MB (52697565 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c8f3e895371ffefe43b4a694efaa5dabf25c9cbcd197d6f82611631c20559e6`
-	Default Command: `["perl5.39.4","-de0"]`

```dockerfile
# Wed, 11 Oct 2023 17:37:43 GMT
ADD file:8c43adb3245fc6f2b10aa5a86c850db5dcf3515eaf7e46630922fe21f806bd2a in / 
# Wed, 11 Oct 2023 17:37:43 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 00:36:36 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Thu, 12 Oct 2023 00:36:36 GMT
WORKDIR /usr/src/perl
# Tue, 31 Oct 2023 00:06:08 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        zlib1g-dev        xz-utils        libssl-dev     && curl -fL https://www.cpan.org/src/5.0/perl-5.39.4.tar.xz -o perl-5.39.4.tar.xz     && echo '73c5e1eb3f125206e82c23e2d03df2c62184d1acc330f99ab7624a3ade19b587 *perl-5.39.4.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.39.4.tar.xz -C /usr/src/perl     && rm perl-5.39.4.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local -Dusedevel -Dversiononly=undef -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && savedPackages="ca-certificates make netbase zlib1g-dev libssl-dev"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Tue, 31 Oct 2023 00:06:08 GMT
WORKDIR /usr/src/app
# Tue, 31 Oct 2023 00:06:08 GMT
CMD ["perl5.39.4" "-de0"]
```

-	Layers:
	-	`sha256:904e6393ef1ee28b37171369eb4f7cb04714631c711799819fccb83886bd212b`  
		Last Modified: Wed, 11 Oct 2023 17:40:47 GMT  
		Size: 26.9 MB (26922150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e660dac65a2bc2fb01a31445619d7453a1affe8d18f84bdf32b6e46c503c9b1b`  
		Last Modified: Thu, 12 Oct 2023 03:25:34 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a8585f64879d6b653cc94b555e4b6e5aa77dd435f6348ceffe9f79c7a57a9ed`  
		Last Modified: Tue, 31 Oct 2023 00:39:19 GMT  
		Size: 25.8 MB (25775082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2443672b2ee2ba50795d8df48bab940a9262b044ce1ddf6718c573556868a978`  
		Last Modified: Tue, 31 Oct 2023 00:39:12 GMT  
		Size: 165.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:devel-slim-bookworm` - linux; arm variant v7

```console
$ docker pull perl@sha256:f595cfd5e8d81a1d6d759af3e79d4b78e2e235b970d63ae1a10e58c7e553339f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.7 MB (49741435 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c650aef76849dd78614e355ade6dc59f21cdcaaba4743fdc22b4c4c7e7d6294e`
-	Default Command: `["perl5.39.4","-de0"]`

```dockerfile
# Wed, 11 Oct 2023 17:42:11 GMT
ADD file:da08fed31a161a2210fd920a1b5e43aa3f4199985cdeaa0d5d24c0a0f19044aa in / 
# Wed, 11 Oct 2023 17:42:11 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 00:42:00 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Thu, 12 Oct 2023 00:42:00 GMT
WORKDIR /usr/src/perl
# Mon, 30 Oct 2023 23:22:44 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        zlib1g-dev        xz-utils        libssl-dev     && curl -fL https://www.cpan.org/src/5.0/perl-5.39.4.tar.xz -o perl-5.39.4.tar.xz     && echo '73c5e1eb3f125206e82c23e2d03df2c62184d1acc330f99ab7624a3ade19b587 *perl-5.39.4.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.39.4.tar.xz -C /usr/src/perl     && rm perl-5.39.4.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local -Dusedevel -Dversiononly=undef -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && savedPackages="ca-certificates make netbase zlib1g-dev libssl-dev"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Mon, 30 Oct 2023 23:22:44 GMT
WORKDIR /usr/src/app
# Mon, 30 Oct 2023 23:22:44 GMT
CMD ["perl5.39.4" "-de0"]
```

-	Layers:
	-	`sha256:2f11c34abc7b59f09b58bb6e2cf54f260f4b4142ecf8023a114e281ea4b532d1`  
		Last Modified: Wed, 11 Oct 2023 17:46:22 GMT  
		Size: 24.7 MB (24748925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69d4157690300bfb148958cfe6691586fafc553fe972120b3aae9ab6afacbc65`  
		Last Modified: Thu, 12 Oct 2023 02:49:52 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2020f08636a66b2317414d2c1f31b757ea21a83ff69288b1a2ba31f166d823a6`  
		Last Modified: Mon, 30 Oct 2023 23:55:06 GMT  
		Size: 25.0 MB (24992178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68f4416a7c06cb0d803bf70dc5279b9590ad23cb3e9d9eb0b00ae3454ec11bfa`  
		Last Modified: Mon, 30 Oct 2023 23:55:00 GMT  
		Size: 165.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:devel-slim-bookworm` - linux; arm64 variant v8

```console
$ docker pull perl@sha256:106f096f861d89046c284bd1c7299f836aca3f13ab1639269241026e93dd7e6c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.6 MB (56632667 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77016a1d6971a8969b793447869b3103d044247920c21ec9478c51c6a6a5eb65`
-	Default Command: `["perl5.39.4","-de0"]`

```dockerfile
# Wed, 11 Oct 2023 18:24:51 GMT
ADD file:5c81bfc00a28feb4079c0daa743f829a6a5bbc1a9d40a890cb49e420539a7f15 in / 
# Wed, 11 Oct 2023 18:24:51 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 04:57:08 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Thu, 12 Oct 2023 04:57:08 GMT
WORKDIR /usr/src/perl
# Tue, 31 Oct 2023 00:09:53 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        zlib1g-dev        xz-utils        libssl-dev     && curl -fL https://www.cpan.org/src/5.0/perl-5.39.4.tar.xz -o perl-5.39.4.tar.xz     && echo '73c5e1eb3f125206e82c23e2d03df2c62184d1acc330f99ab7624a3ade19b587 *perl-5.39.4.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.39.4.tar.xz -C /usr/src/perl     && rm perl-5.39.4.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local -Dusedevel -Dversiononly=undef -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && savedPackages="ca-certificates make netbase zlib1g-dev libssl-dev"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Tue, 31 Oct 2023 00:09:53 GMT
WORKDIR /usr/src/app
# Tue, 31 Oct 2023 00:09:54 GMT
CMD ["perl5.39.4" "-de0"]
```

-	Layers:
	-	`sha256:1bc163a14ea6a886d1d0f9a9be878b1ffd08a9311e15861137ccd85bb87190f9`  
		Last Modified: Wed, 11 Oct 2023 18:28:28 GMT  
		Size: 29.2 MB (29179284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d5a2f237160641ae7d08a395c8978bb0f6f0fbf3800ddf6b5e2d34541800cf8`  
		Last Modified: Thu, 12 Oct 2023 07:58:35 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51b680f28ef269b0116529508b345c67281a6b4eb94d4b806034b05b167a3f89`  
		Last Modified: Tue, 31 Oct 2023 00:37:57 GMT  
		Size: 27.5 MB (27453051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75ce909bb20ad399bf3c1bbf0673f90f25bf276a86c666479840e96d498fe477`  
		Last Modified: Tue, 31 Oct 2023 00:37:53 GMT  
		Size: 165.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:devel-slim-bookworm` - linux; 386

```console
$ docker pull perl@sha256:8c12832f56aae91e4e273037a5fa872dfe4de66ae9678640569052bd0f01cea3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.8 MB (57824682 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:234ceaeba6dfc5c0d18de731a1770a21f816512b18cee01e5414e63ce3b24445`
-	Default Command: `["perl5.39.4","-de0"]`

```dockerfile
# Wed, 11 Oct 2023 17:40:42 GMT
ADD file:31318c1b1f05d559cce42f5b12eef97d916932217e0b987fb07c0fc11bf0a14a in / 
# Wed, 11 Oct 2023 17:40:42 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 22:33:56 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Wed, 11 Oct 2023 22:33:56 GMT
WORKDIR /usr/src/perl
# Tue, 31 Oct 2023 00:09:13 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        zlib1g-dev        xz-utils        libssl-dev     && curl -fL https://www.cpan.org/src/5.0/perl-5.39.4.tar.xz -o perl-5.39.4.tar.xz     && echo '73c5e1eb3f125206e82c23e2d03df2c62184d1acc330f99ab7624a3ade19b587 *perl-5.39.4.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.39.4.tar.xz -C /usr/src/perl     && rm perl-5.39.4.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local -Dusedevel -Dversiononly=undef -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && savedPackages="ca-certificates make netbase zlib1g-dev libssl-dev"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Tue, 31 Oct 2023 00:09:13 GMT
WORKDIR /usr/src/app
# Tue, 31 Oct 2023 00:09:13 GMT
CMD ["perl5.39.4" "-de0"]
```

-	Layers:
	-	`sha256:b27d0f1369837277a82877763487cdd2535037988fc27e16f11cf74e103ae4cd`  
		Last Modified: Wed, 11 Oct 2023 17:45:31 GMT  
		Size: 30.2 MB (30164118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4485771d5f695f38d9604d6a6646edf79162d09d78affb7155277d86ad8d315e`  
		Last Modified: Thu, 12 Oct 2023 05:09:03 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64d70b8463fa9215294cabcddd2c713a3ebf64e90560c5ae6b5616c9054b1fe4`  
		Last Modified: Tue, 31 Oct 2023 01:05:38 GMT  
		Size: 27.7 MB (27660231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e35fa0ce1eb3b1ccefc056adfceb3a08edd4874825518f4205555f6eef8d2653`  
		Last Modified: Tue, 31 Oct 2023 01:05:31 GMT  
		Size: 165.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:devel-slim-bookworm` - linux; mips64le

```console
$ docker pull perl@sha256:33eda2024043a322f980251cf663a7555341e55d5249ee7a10126fdeb7686fa8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.8 MB (55767382 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7bdce414cc486bc55bb84ff67f34978c890aa1c6dcfcebfa2d634a979b2d4e0`
-	Default Command: `["perl5.39.4","-de0"]`

```dockerfile
# Wed, 11 Oct 2023 17:49:32 GMT
ADD file:2abda0a72972a417d4f7f530ca8fa1ee7e85e25d4015fd4e70acf903cfd96d3d in / 
# Wed, 11 Oct 2023 17:49:36 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 00:55:56 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Thu, 12 Oct 2023 00:55:58 GMT
WORKDIR /usr/src/perl
# Tue, 31 Oct 2023 00:20:54 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        zlib1g-dev        xz-utils        libssl-dev     && curl -fL https://www.cpan.org/src/5.0/perl-5.39.4.tar.xz -o perl-5.39.4.tar.xz     && echo '73c5e1eb3f125206e82c23e2d03df2c62184d1acc330f99ab7624a3ade19b587 *perl-5.39.4.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.39.4.tar.xz -C /usr/src/perl     && rm perl-5.39.4.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local -Dusedevel -Dversiononly=undef -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && savedPackages="ca-certificates make netbase zlib1g-dev libssl-dev"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Tue, 31 Oct 2023 00:20:58 GMT
WORKDIR /usr/src/app
# Tue, 31 Oct 2023 00:21:01 GMT
CMD ["perl5.39.4" "-de0"]
```

-	Layers:
	-	`sha256:f11870ec99d788b4b160d9f3f4c0a79904290083d8930b26e5d13579226e07f0`  
		Last Modified: Wed, 11 Oct 2023 18:00:43 GMT  
		Size: 29.1 MB (29142026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaa8822b22fbebdc20b374011b742f2cedfdc1fd72923b2743b4d91df26db16d`  
		Last Modified: Thu, 12 Oct 2023 11:37:58 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8451454e23d09a9ce5e990a7d921aa07ad993d15e3ecd8f6f199d1f98137bba`  
		Last Modified: Tue, 31 Oct 2023 02:32:35 GMT  
		Size: 26.6 MB (26625089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2bc1020a421bfabaacbea85843b4b8b4a029a1d609b4ba408908be30b22e5ea`  
		Last Modified: Tue, 31 Oct 2023 02:32:13 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:devel-slim-bookworm` - linux; ppc64le

```console
$ docker pull perl@sha256:0c7c0173222142fc8cb693c449d506a69b1f1027fbbabafdd791f0b1bded2941
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62359171 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29472ef02120603ea71e32c3cf66d7842b0e6dc031c817a6c019fa51580530e4`
-	Default Command: `["perl5.39.4","-de0"]`

```dockerfile
# Wed, 11 Oct 2023 17:44:19 GMT
ADD file:53c83bdd58e7c4003ae769596cc2f8e6b72c0bbb854dbe7f006a39f273848b1b in / 
# Wed, 11 Oct 2023 17:44:21 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 01:26:42 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Thu, 12 Oct 2023 01:26:43 GMT
WORKDIR /usr/src/perl
# Mon, 30 Oct 2023 23:57:05 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        zlib1g-dev        xz-utils        libssl-dev     && curl -fL https://www.cpan.org/src/5.0/perl-5.39.4.tar.xz -o perl-5.39.4.tar.xz     && echo '73c5e1eb3f125206e82c23e2d03df2c62184d1acc330f99ab7624a3ade19b587 *perl-5.39.4.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.39.4.tar.xz -C /usr/src/perl     && rm perl-5.39.4.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local -Dusedevel -Dversiononly=undef -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && savedPackages="ca-certificates make netbase zlib1g-dev libssl-dev"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Mon, 30 Oct 2023 23:57:07 GMT
WORKDIR /usr/src/app
# Mon, 30 Oct 2023 23:57:07 GMT
CMD ["perl5.39.4" "-de0"]
```

-	Layers:
	-	`sha256:54813908ce8a5d8a81f2db88ad0366eb5266484c7c402e5e93ef26e764f7a0e2`  
		Last Modified: Wed, 11 Oct 2023 17:49:58 GMT  
		Size: 33.1 MB (33141653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e0cbf2dd03640382d2eff026d4c96c2b045ee12474041d4e8302051daffc65f`  
		Last Modified: Thu, 12 Oct 2023 05:25:58 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30b2ce442339e368e8f918d07f4179c31cb50916271f063d49e0cac719d6f480`  
		Last Modified: Tue, 31 Oct 2023 00:30:18 GMT  
		Size: 29.2 MB (29217186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c50dbe7feca2fe4e7a9aa14d12c6fab16f514f6d622a95abde4f9e5fc34095b2`  
		Last Modified: Tue, 31 Oct 2023 00:30:12 GMT  
		Size: 165.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:devel-slim-bookworm` - linux; s390x

```console
$ docker pull perl@sha256:f7012cf2312006c9e6b12fbc4c536a9cf17b352e17f96046a35412d68f2f701b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.7 MB (54716789 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:616fd32ebe778e52f3549699d62625c8e3176c080c6298c101948a338eb63aa1`
-	Default Command: `["perl5.39.4","-de0"]`

```dockerfile
# Wed, 11 Oct 2023 17:50:28 GMT
ADD file:b85ed0ed01200dd3626d66cf5205d989fc48e61b3dd3498f777ee72d91e64870 in / 
# Wed, 11 Oct 2023 17:50:30 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 04:49:41 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Thu, 12 Oct 2023 04:49:41 GMT
WORKDIR /usr/src/perl
# Mon, 30 Oct 2023 23:52:26 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        zlib1g-dev        xz-utils        libssl-dev     && curl -fL https://www.cpan.org/src/5.0/perl-5.39.4.tar.xz -o perl-5.39.4.tar.xz     && echo '73c5e1eb3f125206e82c23e2d03df2c62184d1acc330f99ab7624a3ade19b587 *perl-5.39.4.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.39.4.tar.xz -C /usr/src/perl     && rm perl-5.39.4.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local -Dusedevel -Dversiononly=undef -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && savedPackages="ca-certificates make netbase zlib1g-dev libssl-dev"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Mon, 30 Oct 2023 23:52:28 GMT
WORKDIR /usr/src/app
# Mon, 30 Oct 2023 23:52:28 GMT
CMD ["perl5.39.4" "-de0"]
```

-	Layers:
	-	`sha256:f270c1bb05fa46b165ce3680225dc9fa5bbfe4d69420a467350e80f692c78eb2`  
		Last Modified: Wed, 11 Oct 2023 17:56:03 GMT  
		Size: 27.5 MB (27512850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e383dbbb0b924a308acef84b290bb5250bb4da98853b896e93aa3721719978c`  
		Last Modified: Thu, 12 Oct 2023 09:23:26 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:823129766e1e58d0db8c8648ccf7beec7530d7f52887eba066d99766389ab4a2`  
		Last Modified: Tue, 31 Oct 2023 00:28:20 GMT  
		Size: 27.2 MB (27203606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:396b27787f891191cea13bd6f5cba546a1844f22f865655ebfa03414ce9863a8`  
		Last Modified: Tue, 31 Oct 2023 00:28:15 GMT  
		Size: 164.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
