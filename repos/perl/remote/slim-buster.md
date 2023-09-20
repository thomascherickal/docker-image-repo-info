## `perl:slim-buster`

```console
$ docker pull perl@sha256:03f4e657f1d0059d6bd5c5fa8db47d59bd54c585644450bc5a75d8d0063b7d4c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `perl:slim-buster` - linux; amd64

```console
$ docker pull perl@sha256:c20f4b8f0067fed742e2d40279737aed6a9a9dfa8c16a9365367e3c40677e3c7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.5 MB (54508959 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3078e353822c8f026ccf7a7e0385caafd8dee25bf7132e148f2fd430809b92db`
-	Default Command: `["perl5.38.0","-de0"]`

```dockerfile
# Wed, 20 Sep 2023 04:56:25 GMT
ADD file:a280220815a2a1eb37b2adea38333ec2f2d0c15bef81fb925d2fbb5218f0665f in / 
# Wed, 20 Sep 2023 04:56:25 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 12:54:10 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Wed, 20 Sep 2023 12:54:11 GMT
WORKDIR /usr/src/perl
# Wed, 20 Sep 2023 12:59:54 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        zlib1g-dev        xz-utils        libssl-dev     && curl -fL https://www.cpan.org/src/5.0/perl-5.38.0.tar.xz -o perl-5.38.0.tar.xz     && echo 'eca551caec3bc549a4e590c0015003790bdd1a604ffe19cc78ee631d51f7072e *perl-5.38.0.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.38.0.tar.xz -C /usr/src/perl     && rm perl-5.38.0.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && savedPackages="ca-certificates make netbase zlib1g-dev libssl-dev"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Wed, 20 Sep 2023 12:59:55 GMT
WORKDIR /usr/src/app
# Wed, 20 Sep 2023 12:59:55 GMT
CMD ["perl5.38.0" "-de0"]
```

-	Layers:
	-	`sha256:9f1ecb66bc03eb034c0c89c673def85a052c432125468c04e9aab84714aca0dd`  
		Last Modified: Wed, 20 Sep 2023 05:01:44 GMT  
		Size: 27.2 MB (27187412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:663db394295555f6cdf7a14ce395e5728a9fb239c429de79ee2e7d6602517882`  
		Last Modified: Wed, 20 Sep 2023 16:27:23 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbcc6163620cfb1a0f787422458ef051906665e3120ee3f750d96c69a5b74220`  
		Last Modified: Wed, 20 Sep 2023 16:27:28 GMT  
		Size: 27.3 MB (27321215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5ad6c057972486566d47e7dec45b9460f5dd0a933c2ee399b869ba46cf7c743`  
		Last Modified: Wed, 20 Sep 2023 16:27:23 GMT  
		Size: 164.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:slim-buster` - linux; arm variant v7

```console
$ docker pull perl@sha256:7afbe31d1179c2eb199803dad13b5ba04329bb840f6d29873d66c28554375d79
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.7 MB (46693278 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d9651fbe6a79e5a4cfa0f78a4f68ef2d012e88e1d73e624686b9813987de5eb`
-	Default Command: `["perl5.38.0","-de0"]`

```dockerfile
# Thu, 07 Sep 2023 00:58:32 GMT
ADD file:fa060a900723a2fce017a38b08be3eb2c27d4768d40c61cd1f6292a7f28a8bdc in / 
# Thu, 07 Sep 2023 00:58:33 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 07:31:21 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Thu, 07 Sep 2023 07:31:21 GMT
WORKDIR /usr/src/perl
# Thu, 07 Sep 2023 07:36:54 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        zlib1g-dev        xz-utils        libssl-dev     && curl -fL https://www.cpan.org/src/5.0/perl-5.38.0.tar.xz -o perl-5.38.0.tar.xz     && echo 'eca551caec3bc549a4e590c0015003790bdd1a604ffe19cc78ee631d51f7072e *perl-5.38.0.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.38.0.tar.xz -C /usr/src/perl     && rm perl-5.38.0.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && savedPackages="ca-certificates make netbase zlib1g-dev libssl-dev"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Thu, 07 Sep 2023 07:36:55 GMT
WORKDIR /usr/src/app
# Thu, 07 Sep 2023 07:36:55 GMT
CMD ["perl5.38.0" "-de0"]
```

-	Layers:
	-	`sha256:7e54f06c680feaf82a31a34e7453d765f332f671cfecacb622c3046561dcc572`  
		Last Modified: Thu, 07 Sep 2023 01:03:53 GMT  
		Size: 22.8 MB (22795752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:297e4deb009e4a06184d23c2d932230c5b303f8a864eb904c789b0cfea0fd735`  
		Last Modified: Thu, 07 Sep 2023 11:14:26 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6b77e6bb744203c4aba0c39bcd7e60bab706aa9ed87a3b1d11cf792a25f109c`  
		Last Modified: Thu, 07 Sep 2023 11:14:33 GMT  
		Size: 23.9 MB (23897194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dcfedb084e60908744292cef8ecfa08eb85cddaf991992cc62b8f5e2cba133d`  
		Last Modified: Thu, 07 Sep 2023 11:14:26 GMT  
		Size: 165.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:slim-buster` - linux; arm64 variant v8

```console
$ docker pull perl@sha256:6f9ab646969bb48b9775cc938d76d1171cd0493ad7821d481186915e0c0260db
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.9 MB (51925914 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f52a32b160b8777df58c9aa6a99fef95e2e59750185309646153fe553c46a19`
-	Default Command: `["perl5.38.0","-de0"]`

```dockerfile
# Wed, 20 Sep 2023 02:44:42 GMT
ADD file:22373577ebc4a88322b8e7e5a349667740deade289df65952593aa5fa355e161 in / 
# Wed, 20 Sep 2023 02:44:42 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 13:08:31 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Wed, 20 Sep 2023 13:08:31 GMT
WORKDIR /usr/src/perl
# Wed, 20 Sep 2023 13:13:01 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        zlib1g-dev        xz-utils        libssl-dev     && curl -fL https://www.cpan.org/src/5.0/perl-5.38.0.tar.xz -o perl-5.38.0.tar.xz     && echo 'eca551caec3bc549a4e590c0015003790bdd1a604ffe19cc78ee631d51f7072e *perl-5.38.0.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.38.0.tar.xz -C /usr/src/perl     && rm perl-5.38.0.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && savedPackages="ca-certificates make netbase zlib1g-dev libssl-dev"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Wed, 20 Sep 2023 13:13:01 GMT
WORKDIR /usr/src/app
# Wed, 20 Sep 2023 13:13:01 GMT
CMD ["perl5.38.0" "-de0"]
```

-	Layers:
	-	`sha256:a5329dc26fe29288aabb62184c71ef06987bd81c95d7c43a48e38a0dfaa54ff8`  
		Last Modified: Wed, 20 Sep 2023 02:48:50 GMT  
		Size: 26.0 MB (25967816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b77314c33d9a069b543242421de6d8ba5aa4ddb60b1f9726e18dacdab64f92dd`  
		Last Modified: Wed, 20 Sep 2023 15:59:36 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b755d2bfe5f334bf0643e7af64d4d74c8cdc3e9cd459b04fe855629c9bfd6285`  
		Last Modified: Wed, 20 Sep 2023 15:59:40 GMT  
		Size: 26.0 MB (25957766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11e11e7118c17f5de6e86fc21a66737a1c893e191764fb80a025b10e1a6c3181`  
		Last Modified: Wed, 20 Sep 2023 15:59:36 GMT  
		Size: 165.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:slim-buster` - linux; 386

```console
$ docker pull perl@sha256:d8d83a108d3f61341d685b023211cb0560bd2b848f43e7439c1396401fe183f9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.3 MB (59294439 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8dde48e7eb672a1e189894caaba0a4f4a4fd708f581f6efbb90e29b179154219`
-	Default Command: `["perl5.38.0","-de0"]`

```dockerfile
# Thu, 07 Sep 2023 00:39:46 GMT
ADD file:e5916da683bdcea27e31e6fbb29e61d1f8457a3bebe4a83278e4f0181e5ac49f in / 
# Thu, 07 Sep 2023 00:39:47 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 13:02:22 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Thu, 07 Sep 2023 13:02:22 GMT
WORKDIR /usr/src/perl
# Thu, 07 Sep 2023 13:11:59 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        zlib1g-dev        xz-utils        libssl-dev     && curl -fL https://www.cpan.org/src/5.0/perl-5.38.0.tar.xz -o perl-5.38.0.tar.xz     && echo 'eca551caec3bc549a4e590c0015003790bdd1a604ffe19cc78ee631d51f7072e *perl-5.38.0.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.38.0.tar.xz -C /usr/src/perl     && rm perl-5.38.0.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && savedPackages="ca-certificates make netbase zlib1g-dev libssl-dev"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Thu, 07 Sep 2023 13:11:59 GMT
WORKDIR /usr/src/app
# Thu, 07 Sep 2023 13:11:59 GMT
CMD ["perl5.38.0" "-de0"]
```

-	Layers:
	-	`sha256:453c610c7d8be388b9a8559dc654a2def01e71f776e0608ae46db51ae50d10a0`  
		Last Modified: Thu, 07 Sep 2023 00:45:26 GMT  
		Size: 27.8 MB (27846798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df16ce31a766099c7ed4057e3218c376d6295228e0ca18382d95d3def41a7526`  
		Last Modified: Thu, 07 Sep 2023 19:15:46 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b07063e429b09ef7b54bf837a4cae6b12065d590016316825e1bd152fcf6a52`  
		Last Modified: Thu, 07 Sep 2023 19:15:54 GMT  
		Size: 31.4 MB (31447308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:063dedce812d22066ccf4a685117a11ef9fd77a04db477887f3e2a36d7d0dc27`  
		Last Modified: Thu, 07 Sep 2023 19:15:46 GMT  
		Size: 164.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
