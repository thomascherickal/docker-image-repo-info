## `perl:stable-slim-threaded-buster`

```console
$ docker pull perl@sha256:3027bd3216812685104f314d5f9097f1fc9a210e339bea6e76c60a0a47a28a1d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `perl:stable-slim-threaded-buster` - linux; amd64

```console
$ docker pull perl@sha256:767603ca305e880d30fe502b6fd42ae3a44255f3ab7ecaecada82d8b264c90e8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.6 MB (54570560 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd436ca5402bfb75c102f957b6dfc51f93dc72b255d129282770dd921e1f784f`
-	Default Command: `["perl5.38.0","-de0"]`

```dockerfile
# Wed, 16 Aug 2023 01:00:31 GMT
ADD file:d4315fd7ceb67a5501410e4392ad3fd73642d6e2490f3626ce20a29321fa3682 in / 
# Wed, 16 Aug 2023 01:00:32 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 11:12:43 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Wed, 16 Aug 2023 11:12:43 GMT
WORKDIR /usr/src/perl
# Wed, 16 Aug 2023 11:54:45 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        zlib1g-dev        xz-utils        libssl-dev     && curl -fL https://www.cpan.org/src/5.0/perl-5.38.0.tar.xz -o perl-5.38.0.tar.xz     && echo 'eca551caec3bc549a4e590c0015003790bdd1a604ffe19cc78ee631d51f7072e *perl-5.38.0.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.38.0.tar.xz -C /usr/src/perl     && rm perl-5.38.0.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && savedPackages="ca-certificates make netbase zlib1g-dev libssl-dev"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Wed, 16 Aug 2023 11:54:46 GMT
WORKDIR /usr/src/app
# Wed, 16 Aug 2023 11:54:46 GMT
CMD ["perl5.38.0" "-de0"]
```

-	Layers:
	-	`sha256:ddade83992f922bd9baa0e67dd5f7e8f518b6ed19c67e2ea076c92a8b38416c0`  
		Last Modified: Wed, 16 Aug 2023 01:05:53 GMT  
		Size: 27.2 MB (27187428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d4a1c1d3f8289afc071331f0f6f37b9688e29a8609d1278311188fa7d8d92b7`  
		Last Modified: Wed, 16 Aug 2023 14:38:23 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4453965797a115197cec5dc5fa83b102d4361a038460421161aed7ad7b26f6db`  
		Last Modified: Wed, 16 Aug 2023 14:40:33 GMT  
		Size: 27.4 MB (27382798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de9823abe9417c58fd5a76686fc63bfedebde6983617e5facf4076f2094330fa`  
		Last Modified: Wed, 16 Aug 2023 14:40:29 GMT  
		Size: 165.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:stable-slim-threaded-buster` - linux; arm variant v7

```console
$ docker pull perl@sha256:191e9ce272265ab67d8e4daaa11da0f64acbd850157d27e96c6f86c3f9a7a63d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.7 MB (46716994 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:abc305d42c65b71a121cfabff41559b769fd0e52cdafe2fe84bb63030537b056`
-	Default Command: `["perl5.38.0","-de0"]`

```dockerfile
# Wed, 16 Aug 2023 00:17:52 GMT
ADD file:c676b622e67d7e8923f6eb310001d3118e7e31af842dd82f006d8900860f1f4e in / 
# Wed, 16 Aug 2023 00:17:52 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 08:25:16 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Wed, 16 Aug 2023 08:25:16 GMT
WORKDIR /usr/src/perl
# Wed, 16 Aug 2023 09:07:46 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        zlib1g-dev        xz-utils        libssl-dev     && curl -fL https://www.cpan.org/src/5.0/perl-5.38.0.tar.xz -o perl-5.38.0.tar.xz     && echo 'eca551caec3bc549a4e590c0015003790bdd1a604ffe19cc78ee631d51f7072e *perl-5.38.0.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.38.0.tar.xz -C /usr/src/perl     && rm perl-5.38.0.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && savedPackages="ca-certificates make netbase zlib1g-dev libssl-dev"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Wed, 16 Aug 2023 09:07:46 GMT
WORKDIR /usr/src/app
# Wed, 16 Aug 2023 09:07:46 GMT
CMD ["perl5.38.0" "-de0"]
```

-	Layers:
	-	`sha256:87da7f83f545c68a0ecbfd834e0fec4078d10fbcc8f3eee04eb7d85bddf5f41a`  
		Last Modified: Wed, 16 Aug 2023 00:22:48 GMT  
		Size: 22.8 MB (22795639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be0329ed99f4ca13fe6bc30b1899dacd223600b1c568b6cac00b985bd91fc88e`  
		Last Modified: Wed, 16 Aug 2023 11:57:02 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65af57cbe20348aa322f6b1955dbd808104e8c7abfda0e422bdc88aae480b900`  
		Last Modified: Wed, 16 Aug 2023 11:59:18 GMT  
		Size: 23.9 MB (23921022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ae4af36fc34e83d5b0822b65c4cadb9af235b3609108e895eda549bef70a4e1`  
		Last Modified: Wed, 16 Aug 2023 11:59:12 GMT  
		Size: 165.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:stable-slim-threaded-buster` - linux; arm64 variant v8

```console
$ docker pull perl@sha256:7b50e1058fb649698897cc4698bbc7f38e0b906a810393410a4f58047af46ed0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.0 MB (51960762 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:885f7f1a58b397f4ef6e67d6026422cce222a04717e9e3ae05df4692813782a5`
-	Default Command: `["perl5.38.0","-de0"]`

```dockerfile
# Thu, 07 Sep 2023 00:40:08 GMT
ADD file:3521159cdea23e107a3e194ebc9b8f9a6a37ea8188236a267b6ec26e87cf498a in / 
# Thu, 07 Sep 2023 00:40:08 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 02:41:51 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Thu, 07 Sep 2023 02:41:51 GMT
WORKDIR /usr/src/perl
# Thu, 07 Sep 2023 03:01:39 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        zlib1g-dev        xz-utils        libssl-dev     && curl -fL https://www.cpan.org/src/5.0/perl-5.38.0.tar.xz -o perl-5.38.0.tar.xz     && echo 'eca551caec3bc549a4e590c0015003790bdd1a604ffe19cc78ee631d51f7072e *perl-5.38.0.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.38.0.tar.xz -C /usr/src/perl     && rm perl-5.38.0.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && savedPackages="ca-certificates make netbase zlib1g-dev libssl-dev"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Thu, 07 Sep 2023 03:01:40 GMT
WORKDIR /usr/src/app
# Thu, 07 Sep 2023 03:01:40 GMT
CMD ["perl5.38.0" "-de0"]
```

-	Layers:
	-	`sha256:d7cc66d62b738dea27e341b7322194f45ab1be2e548fe11d8ad953d9d56caaa8`  
		Last Modified: Thu, 07 Sep 2023 00:44:18 GMT  
		Size: 26.0 MB (25967748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f1c7521e41e800fe718b76f3411fc6873243216f2ad33f540b7c527748b87a0`  
		Last Modified: Thu, 07 Sep 2023 04:12:43 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eed8efbc90193f62ff4896ede9ba62ff7b767edc862484d83e078c244ad47e68`  
		Last Modified: Thu, 07 Sep 2023 04:13:54 GMT  
		Size: 26.0 MB (25992684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d3334952cba449bc6a3508e0c8b1f0c250e1480202a2e4812a8fb606cfb3d7a`  
		Last Modified: Thu, 07 Sep 2023 04:13:50 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:stable-slim-threaded-buster` - linux; 386

```console
$ docker pull perl@sha256:1e220c2f6d801651a2f369cf73ab626027f9a398ea02767bc50daa40c4a61c2b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.4 MB (59392000 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9665f80809ad81437d8047938062e6fa4fa940a8fd2c0649bb3b207f6c7c8830`
-	Default Command: `["perl5.38.0","-de0"]`

```dockerfile
# Tue, 15 Aug 2023 23:39:42 GMT
ADD file:ae6c40cc5a829da442f96b66b8f569c9d6548ee7f7b5400ff2bf7c3aebfcd24e in / 
# Tue, 15 Aug 2023 23:39:42 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 10:34:30 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Wed, 16 Aug 2023 10:34:30 GMT
WORKDIR /usr/src/perl
# Wed, 16 Aug 2023 11:46:46 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        zlib1g-dev        xz-utils        libssl-dev     && curl -fL https://www.cpan.org/src/5.0/perl-5.38.0.tar.xz -o perl-5.38.0.tar.xz     && echo 'eca551caec3bc549a4e590c0015003790bdd1a604ffe19cc78ee631d51f7072e *perl-5.38.0.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.38.0.tar.xz -C /usr/src/perl     && rm perl-5.38.0.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && savedPackages="ca-certificates make netbase zlib1g-dev libssl-dev"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Wed, 16 Aug 2023 11:46:47 GMT
WORKDIR /usr/src/app
# Wed, 16 Aug 2023 11:46:47 GMT
CMD ["perl5.38.0" "-de0"]
```

-	Layers:
	-	`sha256:d9e55579ec1f77161834b61f5695b43d7d48684ba7af581863bcae8225c19e96`  
		Last Modified: Tue, 15 Aug 2023 23:44:56 GMT  
		Size: 27.8 MB (27846956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f35a8e6f041f8c41b175391fa03bc87a87651d0dd7e72782cfdeed270fbfce3f`  
		Last Modified: Wed, 16 Aug 2023 16:30:20 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f319a0fea2b46871143868b375a2ef2a13f930a65e87c63844f529de6fdcf06a`  
		Last Modified: Wed, 16 Aug 2023 16:32:49 GMT  
		Size: 31.5 MB (31544711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49afd9bb83b27d612f511c2109f2c1b10de0adbb579762b2b287400eabed2a74`  
		Last Modified: Wed, 16 Aug 2023 16:32:41 GMT  
		Size: 165.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
