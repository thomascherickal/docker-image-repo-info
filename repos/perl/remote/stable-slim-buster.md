## `perl:stable-slim-buster`

```console
$ docker pull perl@sha256:2d93b1663eb6c8f0b555e36bf37675b6f31137b6bf57a9d0113b3eab042cd9f6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `perl:stable-slim-buster` - linux; amd64

```console
$ docker pull perl@sha256:31a3a47fa28675756dce64121bc059c443f693ff50753a1c4fafde29063a3c10
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.5 MB (54489801 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c6929ad1e35b46419a82d100064fad28f8d5e26b07776d9b828dda74d38b9b6`
-	Default Command: `["perl5.38.2","-de0"]`

```dockerfile
# Tue, 21 Nov 2023 05:22:20 GMT
ADD file:7672eb709be933bb0edec47b8141cd2ebff266a770dfae1278205f7cee43c71a in / 
# Tue, 21 Nov 2023 05:22:20 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 06:26:09 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Tue, 21 Nov 2023 06:26:09 GMT
WORKDIR /usr/src/perl
# Thu, 30 Nov 2023 19:55:17 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        zlib1g-dev        xz-utils        libssl-dev     && curl -fL https://www.cpan.org/src/5.0/perl-5.38.2.tar.xz -o perl-5.38.2.tar.xz     && echo 'd91115e90b896520e83d4de6b52f8254ef2b70a8d545ffab33200ea9f1cf29e8 *perl-5.38.2.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.38.2.tar.xz -C /usr/src/perl     && rm perl-5.38.2.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && savedPackages="ca-certificates make netbase zlib1g-dev libssl-dev"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Thu, 30 Nov 2023 19:55:18 GMT
WORKDIR /usr/src/app
# Thu, 30 Nov 2023 19:55:18 GMT
CMD ["perl5.38.2" "-de0"]
```

-	Layers:
	-	`sha256:0fc9206bc4affb32fe13185a20b8184271c753e9b7cb81484bf770054fc69737`  
		Last Modified: Tue, 21 Nov 2023 05:27:19 GMT  
		Size: 27.2 MB (27187457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1c9e6a0beb8102e6e4484da6fa9a020eabbf35207c975f5616538a4ac2801e0`  
		Last Modified: Tue, 21 Nov 2023 08:39:06 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62024cda86a4615febc1b6a77cf0ccee3d8fc5d0e0c1fea02d885115866dd5bd`  
		Last Modified: Thu, 30 Nov 2023 22:32:48 GMT  
		Size: 27.3 MB (27302011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f57fbe18a1e7de76db44b221238b701fde6e3aced9da794282c331bf6c348da`  
		Last Modified: Thu, 30 Nov 2023 22:32:44 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:stable-slim-buster` - linux; arm variant v7

```console
$ docker pull perl@sha256:c43ebb6b72fbcf40270fd6579c8036f30f91eab4734e78d9219fad93327f42c3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.7 MB (46684517 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd48b61cd7d87974b0b332f52d9658348c8eda4cd01ebdf60424cb0535f9445a`
-	Default Command: `["perl5.38.2","-de0"]`

```dockerfile
# Tue, 21 Nov 2023 03:58:22 GMT
ADD file:407ef80699946b8a8560ae436dfc9ca6148067b3012c02b4cb4e54d6d0aca674 in / 
# Tue, 21 Nov 2023 03:58:22 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 04:29:54 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Tue, 21 Nov 2023 04:29:54 GMT
WORKDIR /usr/src/perl
# Thu, 30 Nov 2023 19:30:07 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        zlib1g-dev        xz-utils        libssl-dev     && curl -fL https://www.cpan.org/src/5.0/perl-5.38.2.tar.xz -o perl-5.38.2.tar.xz     && echo 'd91115e90b896520e83d4de6b52f8254ef2b70a8d545ffab33200ea9f1cf29e8 *perl-5.38.2.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.38.2.tar.xz -C /usr/src/perl     && rm perl-5.38.2.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && savedPackages="ca-certificates make netbase zlib1g-dev libssl-dev"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Thu, 30 Nov 2023 19:30:08 GMT
WORKDIR /usr/src/app
# Thu, 30 Nov 2023 19:30:08 GMT
CMD ["perl5.38.2" "-de0"]
```

-	Layers:
	-	`sha256:d0b016a8027330736e9ca5c23b846a6a9c1eb0a32da6459047c95d22e9544cb7`  
		Last Modified: Tue, 21 Nov 2023 04:03:19 GMT  
		Size: 22.8 MB (22795884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2377a08a131e111c9f41f7522692d2d8f4e545680a1ae58f37f4195d9cc4ec5d`  
		Last Modified: Tue, 21 Nov 2023 06:42:55 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92d2b2014565fd5d4a882cebdd1f0643898bfe71749ab3cc75efa3c237f6bf5`  
		Last Modified: Thu, 30 Nov 2023 22:08:49 GMT  
		Size: 23.9 MB (23888299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c21bdbc371e2dd77a2b059675df97e4db18f863245867f5254c03c4304fe946a`  
		Last Modified: Thu, 30 Nov 2023 22:08:43 GMT  
		Size: 165.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:stable-slim-buster` - linux; arm64 variant v8

```console
$ docker pull perl@sha256:6ff787c8f13f543a7f62f8cef95cd67d727b936eae5ef34a5ef5661689bfcc52
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.9 MB (51914954 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7626964cc2e2e3834a10ee8325a2c6d035554f037cf6311998a16a599b4db8c4`
-	Default Command: `["perl5.38.2","-de0"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:34 GMT
ADD file:475e94b9a8f65c7cd4d4156af31e83190240ff35d8038f3fa86ad124d4d5d299 in / 
# Tue, 21 Nov 2023 06:27:35 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 10:56:31 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Tue, 21 Nov 2023 10:56:31 GMT
WORKDIR /usr/src/perl
# Thu, 30 Nov 2023 20:09:39 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        zlib1g-dev        xz-utils        libssl-dev     && curl -fL https://www.cpan.org/src/5.0/perl-5.38.2.tar.xz -o perl-5.38.2.tar.xz     && echo 'd91115e90b896520e83d4de6b52f8254ef2b70a8d545ffab33200ea9f1cf29e8 *perl-5.38.2.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.38.2.tar.xz -C /usr/src/perl     && rm perl-5.38.2.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && savedPackages="ca-certificates make netbase zlib1g-dev libssl-dev"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Thu, 30 Nov 2023 20:09:40 GMT
WORKDIR /usr/src/app
# Thu, 30 Nov 2023 20:09:40 GMT
CMD ["perl5.38.2" "-de0"]
```

-	Layers:
	-	`sha256:78b429e3efdd9f2b163abf0bca6b1462a25b1c5eddc1dd47f5d3445c6413cfa1`  
		Last Modified: Tue, 21 Nov 2023 06:31:45 GMT  
		Size: 26.0 MB (25967796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68fccf93829b001397b5136fdd9e8ef61e2d213ceff6ef312977de53aa611c06`  
		Last Modified: Tue, 21 Nov 2023 13:51:02 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c5c091eb048025578eef472d791ba565f1b486f1d8530418cb8e9657503cce3`  
		Last Modified: Thu, 30 Nov 2023 22:18:20 GMT  
		Size: 25.9 MB (25946823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcc67731ec8595f833652096b6e6fb9baaff9ec997be517086621af20df19d14`  
		Last Modified: Thu, 30 Nov 2023 22:18:15 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:stable-slim-buster` - linux; 386

```console
$ docker pull perl@sha256:d8a3d1e1f1f1bac9fedeec6ac9d6e0b31166d69a09d69f80d5f19ab6580aa86d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.3 MB (59280121 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5130f0a1ea3b20d10978893d1486aef5f954568061997c176fe18e64841945d`
-	Default Command: `["perl5.38.2","-de0"]`

```dockerfile
# Tue, 21 Nov 2023 04:40:37 GMT
ADD file:a04f70df2aa61b210935e80ad2a655ad282407ef0b8e8e0acf47479c73f64f95 in / 
# Tue, 21 Nov 2023 04:40:38 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 05:11:52 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Tue, 21 Nov 2023 05:11:52 GMT
WORKDIR /usr/src/perl
# Thu, 30 Nov 2023 20:43:04 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        zlib1g-dev        xz-utils        libssl-dev     && curl -fL https://www.cpan.org/src/5.0/perl-5.38.2.tar.xz -o perl-5.38.2.tar.xz     && echo 'd91115e90b896520e83d4de6b52f8254ef2b70a8d545ffab33200ea9f1cf29e8 *perl-5.38.2.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.38.2.tar.xz -C /usr/src/perl     && rm perl-5.38.2.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && savedPackages="ca-certificates make netbase zlib1g-dev libssl-dev"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Thu, 30 Nov 2023 20:43:05 GMT
WORKDIR /usr/src/app
# Thu, 30 Nov 2023 20:43:05 GMT
CMD ["perl5.38.2" "-de0"]
```

-	Layers:
	-	`sha256:071d917b80792914c4da1ecc1adf7e2503440a8c7a2a5508542e0850d9187060`  
		Last Modified: Tue, 21 Nov 2023 04:46:12 GMT  
		Size: 27.8 MB (27846916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ec5851faef42ba0487a82ae13df788da379aa99dc37d77640f32f0f4b91caf9`  
		Last Modified: Tue, 21 Nov 2023 09:10:06 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d83da55f4da639e2717ed6819b46241115747838ee6d45cea3e927d1ff2d682c`  
		Last Modified: Fri, 01 Dec 2023 01:31:03 GMT  
		Size: 31.4 MB (31432872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fabfb743d0f7162e519a4f58a8dbc3c8c5c6f1c3725dd56287b4077e3cedd65a`  
		Last Modified: Fri, 01 Dec 2023 01:30:54 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
