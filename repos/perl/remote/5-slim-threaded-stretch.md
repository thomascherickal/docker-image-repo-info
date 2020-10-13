## `perl:5-slim-threaded-stretch`

```console
$ docker pull perl@sha256:15115656e72bcffd232da3e56722c9594cf51fd2581e92550526f07c79c16fb5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `perl:5-slim-threaded-stretch` - linux; amd64

```console
$ docker pull perl@sha256:bc3a6e77cbfc855277ee038f4a2b0bc7d06933bb45bc0b2ab2e7b9e0305b536f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.2 MB (37166174 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:640b7751a060ef2d491c74c83c4beafab3a2c0c32b6dce2eb618b71e8845ef2f`
-	Default Command: `["perl5.32.0","-de0"]`

```dockerfile
# Tue, 13 Oct 2020 01:44:45 GMT
ADD file:4453535d387fcb17ead2026c72c05444e7558aa4736e3c0cdfb87cf20eaa5a9f in / 
# Tue, 13 Oct 2020 01:44:45 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 13:20:22 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Tue, 13 Oct 2020 13:20:22 GMT
COPY file:3744c5cc39cdbdcae10db09a1f0f399005a79f93c237b387a72ff5710cdd458c in /usr/src/perl/ 
# Tue, 13 Oct 2020 13:20:22 GMT
WORKDIR /usr/src/perl
# Tue, 13 Oct 2020 14:32:48 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        xz-utils     && curl -SL https://www.cpan.org/src/5.0/perl-5.32.0.tar.xz -o perl-5.32.0.tar.xz     && echo '6f436b447cf56d22464f980fac1916e707a040e96d52172984c5d184c09b859b *perl-5.32.0.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.32.0.tar.xz -C /usr/src/perl     && rm perl-5.32.0.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && savedPackages="make netbase"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Tue, 13 Oct 2020 14:32:48 GMT
WORKDIR /
# Tue, 13 Oct 2020 14:32:49 GMT
CMD ["perl5.32.0" "-de0"]
```

-	Layers:
	-	`sha256:babf97a3f00ae0a4d59c1a0f88918d8f7aa0f0758380258b2016f0cd17e97202`  
		Last Modified: Tue, 13 Oct 2020 01:51:03 GMT  
		Size: 22.5 MB (22522093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7a3afe6c775d40924f8bc4367143a5655d18d785d64e08677accada76b7d8f3`  
		Last Modified: Tue, 13 Oct 2020 17:44:39 GMT  
		Size: 179.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e7400d94285b03f17aade10a6ecf2ac6b8814ac2cd84cc27389026ecb969a2b`  
		Last Modified: Tue, 13 Oct 2020 17:45:47 GMT  
		Size: 14.6 MB (14643902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:5-slim-threaded-stretch` - linux; arm variant v7

```console
$ docker pull perl@sha256:63c03335714971c2b882012ace6839303dd69d67668ea9f8517bcd2da07ac828
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.1 MB (33064450 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5276cc2625ffc29f0268526e9418506c188c7eecd71450b6e45a0a76fb568276`
-	Default Command: `["perl5.32.0","-de0"]`

```dockerfile
# Tue, 13 Oct 2020 01:04:30 GMT
ADD file:d204a257433edcd6f9ddd2c769b9e187c408eb4972203a5daab60214b5b576bc in / 
# Tue, 13 Oct 2020 01:04:31 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 09:36:44 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Tue, 13 Oct 2020 09:36:45 GMT
COPY file:3744c5cc39cdbdcae10db09a1f0f399005a79f93c237b387a72ff5710cdd458c in /usr/src/perl/ 
# Tue, 13 Oct 2020 09:36:46 GMT
WORKDIR /usr/src/perl
# Tue, 13 Oct 2020 10:30:46 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        xz-utils     && curl -SL https://www.cpan.org/src/5.0/perl-5.32.0.tar.xz -o perl-5.32.0.tar.xz     && echo '6f436b447cf56d22464f980fac1916e707a040e96d52172984c5d184c09b859b *perl-5.32.0.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.32.0.tar.xz -C /usr/src/perl     && rm perl-5.32.0.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && savedPackages="make netbase"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Tue, 13 Oct 2020 10:30:55 GMT
WORKDIR /
# Tue, 13 Oct 2020 10:31:02 GMT
CMD ["perl5.32.0" "-de0"]
```

-	Layers:
	-	`sha256:cc11be355171b10881b3ed16be16ceb2d7787cd459c6489d83bac55ee5824b35`  
		Last Modified: Tue, 13 Oct 2020 01:12:46 GMT  
		Size: 19.3 MB (19304540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6650d5bcf9880ee0f3e27efed1879308198cb31e9de65eb4a2247f4dd4a4237b`  
		Last Modified: Tue, 13 Oct 2020 13:38:54 GMT  
		Size: 203.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d39f29372b02dd0c79421e94352a8b61e813b0d0df2678634e76a304cd172761`  
		Last Modified: Tue, 13 Oct 2020 13:40:58 GMT  
		Size: 13.8 MB (13759707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:5-slim-threaded-stretch` - linux; arm64 variant v8

```console
$ docker pull perl@sha256:71aca4a858d2b290adbfe39f36c0051d5c3aa413bbf872d90d3ca2d9d9052e8d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34815022 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d41c8d60bdc2fbdfb2dac820b773db64d89b00a42deb3427679727e590a81473`
-	Default Command: `["perl5.32.0","-de0"]`

```dockerfile
# Tue, 13 Oct 2020 01:44:21 GMT
ADD file:1783101ec41dba711940487fb45a9287f74a0639658051ad8bc9b2618a15be61 in / 
# Tue, 13 Oct 2020 01:44:22 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 13:39:12 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Tue, 13 Oct 2020 13:39:14 GMT
COPY file:3744c5cc39cdbdcae10db09a1f0f399005a79f93c237b387a72ff5710cdd458c in /usr/src/perl/ 
# Tue, 13 Oct 2020 13:39:15 GMT
WORKDIR /usr/src/perl
# Tue, 13 Oct 2020 14:48:24 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        xz-utils     && curl -SL https://www.cpan.org/src/5.0/perl-5.32.0.tar.xz -o perl-5.32.0.tar.xz     && echo '6f436b447cf56d22464f980fac1916e707a040e96d52172984c5d184c09b859b *perl-5.32.0.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.32.0.tar.xz -C /usr/src/perl     && rm perl-5.32.0.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && savedPackages="make netbase"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Tue, 13 Oct 2020 14:48:32 GMT
WORKDIR /
# Tue, 13 Oct 2020 14:48:43 GMT
CMD ["perl5.32.0" "-de0"]
```

-	Layers:
	-	`sha256:f4bec48cdb322f1180477bdd362bcd92d70a1ab628fc36319017bf4e8058d9ee`  
		Last Modified: Tue, 13 Oct 2020 01:51:12 GMT  
		Size: 20.4 MB (20376997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d67197f45e2fed0b30c2105e7835ab2836c57d4aac180719a7f64c4446e8e16`  
		Last Modified: Tue, 13 Oct 2020 17:56:32 GMT  
		Size: 205.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e663bc1d816c072feb82a17331dc00802fbb0488303d0fc460d7baa37bc92b3`  
		Last Modified: Tue, 13 Oct 2020 17:58:29 GMT  
		Size: 14.4 MB (14437820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:5-slim-threaded-stretch` - linux; 386

```console
$ docker pull perl@sha256:883df11f0e8a2413a4ea51787e7f4f2844519323c8204dd77ae4954229735d94
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.3 MB (37329028 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66f5d7dd1f14ada62bd62ed73c51060d60820924af29e6b772ad5a1bf62e7c32`
-	Default Command: `["perl5.32.0","-de0"]`

```dockerfile
# Tue, 13 Oct 2020 01:45:31 GMT
ADD file:f09276bb607e6d68dcb997c1e8b4d004b91548964306d6a803286ba851484579 in / 
# Tue, 13 Oct 2020 01:45:31 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 11:33:00 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Tue, 13 Oct 2020 11:33:00 GMT
COPY file:3744c5cc39cdbdcae10db09a1f0f399005a79f93c237b387a72ff5710cdd458c in /usr/src/perl/ 
# Tue, 13 Oct 2020 11:33:01 GMT
WORKDIR /usr/src/perl
# Tue, 13 Oct 2020 12:45:36 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        xz-utils     && curl -SL https://www.cpan.org/src/5.0/perl-5.32.0.tar.xz -o perl-5.32.0.tar.xz     && echo '6f436b447cf56d22464f980fac1916e707a040e96d52172984c5d184c09b859b *perl-5.32.0.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.32.0.tar.xz -C /usr/src/perl     && rm perl-5.32.0.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && savedPackages="make netbase"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Tue, 13 Oct 2020 12:45:36 GMT
WORKDIR /
# Tue, 13 Oct 2020 12:45:36 GMT
CMD ["perl5.32.0" "-de0"]
```

-	Layers:
	-	`sha256:02448e4a5fa68035acff67a00ba04305cbad42b25ffeb4b141c5f1f0b9d63a2a`  
		Last Modified: Tue, 13 Oct 2020 01:52:11 GMT  
		Size: 23.1 MB (23148149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc3c8e2f1ec36d4c7ffd2f268b6fc8331830018c341ac9b09dec7aa75643b91f`  
		Last Modified: Tue, 13 Oct 2020 16:35:58 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21afe2aa2ebc2e45fc589da97058845aebdf51c6c1b1bc733fb1ae7e275ae6d6`  
		Last Modified: Tue, 13 Oct 2020 16:37:02 GMT  
		Size: 14.2 MB (14180703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:5-slim-threaded-stretch` - linux; ppc64le

```console
$ docker pull perl@sha256:ed838b5ba0d336ae7657072a7b368e39d9f14b7cbaba7cd65cb780a8354306ed
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.3 MB (37285960 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1d567c8a931f2c9827d039e646a088137232b6abc263be773e58fbc9ce43836`
-	Default Command: `["perl5.32.0","-de0"]`

```dockerfile
# Tue, 09 Jun 2020 01:25:38 GMT
ADD file:41ec53d65aa183c2835f73989c9e4922f818e59774811eaa6e7395e5a36d5eab in / 
# Tue, 09 Jun 2020 01:25:42 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 14:27:23 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Mon, 22 Jun 2020 15:40:21 GMT
COPY file:3744c5cc39cdbdcae10db09a1f0f399005a79f93c237b387a72ff5710cdd458c in /usr/src/perl/ 
# Mon, 22 Jun 2020 15:40:24 GMT
WORKDIR /usr/src/perl
# Mon, 22 Jun 2020 16:24:37 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        xz-utils     && curl -SL https://www.cpan.org/src/5.0/perl-5.32.0.tar.xz -o perl-5.32.0.tar.xz     && echo '6f436b447cf56d22464f980fac1916e707a040e96d52172984c5d184c09b859b *perl-5.32.0.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.32.0.tar.xz -C /usr/src/perl     && rm perl-5.32.0.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && savedPackages="make netbase"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Mon, 22 Jun 2020 16:24:45 GMT
WORKDIR /
# Mon, 22 Jun 2020 16:24:52 GMT
CMD ["perl5.32.0" "-de0"]
```

-	Layers:
	-	`sha256:a29e28607c9b96acae7ff89e56214e4339a87c59e40a6f030fa4cbcaab753f2c`  
		Last Modified: Tue, 09 Jun 2020 01:37:25 GMT  
		Size: 22.8 MB (22791269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0789a92ac122eecdf7b0bd168e70ec21062493b4fa3617f62eb7fd387e9d6780`  
		Last Modified: Mon, 22 Jun 2020 16:28:33 GMT  
		Size: 202.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4d7ba7b7c07cb6f09319ea14813baab5326372ecb8fd67bfd424327ce455702`  
		Last Modified: Mon, 22 Jun 2020 16:30:13 GMT  
		Size: 14.5 MB (14494489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:5-slim-threaded-stretch` - linux; s390x

```console
$ docker pull perl@sha256:40dcab1cfa0c3b1658202513214d3ec668cf1390b6f2bab0cd724da1c706e16c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.4 MB (37438418 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15576b3500996cffcf93c301c2ae3ae412296044f7c915799aab6e409c425937`
-	Default Command: `["perl5.32.0","-de0"]`

```dockerfile
# Tue, 09 Jun 2020 01:44:20 GMT
ADD file:b3e01a52177029e9c3ba14a708f5dd33a38777f05d0e43656aca742b2991b13c in / 
# Tue, 09 Jun 2020 01:44:22 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 04:04:12 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Mon, 22 Jun 2020 16:00:38 GMT
COPY file:3744c5cc39cdbdcae10db09a1f0f399005a79f93c237b387a72ff5710cdd458c in /usr/src/perl/ 
# Mon, 22 Jun 2020 16:00:39 GMT
WORKDIR /usr/src/perl
# Mon, 22 Jun 2020 16:30:35 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        xz-utils     && curl -SL https://www.cpan.org/src/5.0/perl-5.32.0.tar.xz -o perl-5.32.0.tar.xz     && echo '6f436b447cf56d22464f980fac1916e707a040e96d52172984c5d184c09b859b *perl-5.32.0.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.32.0.tar.xz -C /usr/src/perl     && rm perl-5.32.0.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && savedPackages="make netbase"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Mon, 22 Jun 2020 16:30:36 GMT
WORKDIR /
# Mon, 22 Jun 2020 16:30:36 GMT
CMD ["perl5.32.0" "-de0"]
```

-	Layers:
	-	`sha256:428ea12d5f095d89f941ce335d5f799da515abfd0c161e7ee85e12cd3d97fd4e`  
		Last Modified: Tue, 09 Jun 2020 01:48:04 GMT  
		Size: 22.4 MB (22371004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bda422b0ebe5506ce35e51f433e6f95412877201e00691a90070ae6509418a6`  
		Last Modified: Mon, 22 Jun 2020 16:32:54 GMT  
		Size: 202.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2e50c8552baae55789e5e7fc5d1eaa5e79dbec78de1e65b87414ded46cce779`  
		Last Modified: Mon, 22 Jun 2020 16:33:41 GMT  
		Size: 15.1 MB (15067212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
