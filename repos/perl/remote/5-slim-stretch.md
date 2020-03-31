## `perl:5-slim-stretch`

```console
$ docker pull perl@sha256:35921c3bee559de3a9f174d7d5e0c281ff2510d1d3811f9b8e60ce1118470fd8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `perl:5-slim-stretch` - linux; amd64

```console
$ docker pull perl@sha256:259734a5f3bd8528a1852349b3aef6e11f04eb4ec06999e005d0bfacf32d0598
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.8 MB (36849801 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96833c532e03297c067c48b2d6d97425274933d9a2d2f05a213c5ff36e0c5a70`
-	Default Command: `["perl5.30.2","-de0"]`

```dockerfile
# Wed, 26 Feb 2020 00:41:38 GMT
ADD file:1256c62f77a54c982fdb2790d682049b2ad64c8466466e846f3d33ad1ed4035d in / 
# Wed, 26 Feb 2020 00:41:38 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 07:44:19 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Wed, 26 Feb 2020 07:44:19 GMT
COPY file:15650064fd29deac721f0aa084ddb3d41db77b78e2907775e257bd67e116ade4 in /usr/src/perl/ 
# Wed, 26 Feb 2020 07:44:20 GMT
WORKDIR /usr/src/perl
# Tue, 17 Mar 2020 18:13:44 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        xz-utils     && curl -SL https://www.cpan.org/src/5.0/perl-5.30.2.tar.xz -o perl-5.30.2.tar.xz     && echo 'a1aa88bd6fbbdc2e82938afbb76c408b0ea847317737b712dc196cc7907a5259 *perl-5.30.2.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.30.2.tar.xz -C /usr/src/perl     && rm perl-5.30.2.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && savedPackages="make netbase"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Tue, 17 Mar 2020 18:13:45 GMT
WORKDIR /
# Tue, 17 Mar 2020 18:13:45 GMT
CMD ["perl5.30.2" "-de0"]
```

-	Layers:
	-	`sha256:6d28e14ab8c85bf8a4331de0667c27d19ef4092b12531eec0334b5c2a1012668`  
		Last Modified: Wed, 26 Feb 2020 00:47:21 GMT  
		Size: 22.5 MB (22513365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffa9fabe6cfd6b6f961c4aeed770a37353a9657826e3d5d644abdf8ac9a8bd50`  
		Last Modified: Wed, 26 Feb 2020 11:43:18 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e05e8da2070325db3dcef2ff77c11dd127dc083659dd6caf0aaba146ffe35e7c`  
		Last Modified: Tue, 17 Mar 2020 22:08:12 GMT  
		Size: 14.3 MB (14336021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:5-slim-stretch` - linux; arm variant v7

```console
$ docker pull perl@sha256:fff67c25263cea8aa367dec7b09adb23c9f54d4924c87ca302dae694f1657c2e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.8 MB (32773333 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10a0186356589bf50f7c993b7b81d1cac9514ad363da5c3c602c5f0e780c9e84`
-	Default Command: `["perl5.30.2","-de0"]`

```dockerfile
# Wed, 26 Feb 2020 01:01:21 GMT
ADD file:01536f0f2d25f5114e68606280b1a495c4b930ffdd782678b7e8828aef822c14 in / 
# Wed, 26 Feb 2020 01:01:26 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 05:09:58 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Wed, 26 Feb 2020 05:09:59 GMT
COPY file:15650064fd29deac721f0aa084ddb3d41db77b78e2907775e257bd67e116ade4 in /usr/src/perl/ 
# Wed, 26 Feb 2020 05:10:00 GMT
WORKDIR /usr/src/perl
# Tue, 17 Mar 2020 17:36:54 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        xz-utils     && curl -SL https://www.cpan.org/src/5.0/perl-5.30.2.tar.xz -o perl-5.30.2.tar.xz     && echo 'a1aa88bd6fbbdc2e82938afbb76c408b0ea847317737b712dc196cc7907a5259 *perl-5.30.2.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.30.2.tar.xz -C /usr/src/perl     && rm perl-5.30.2.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && savedPackages="make netbase"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Tue, 17 Mar 2020 17:36:56 GMT
WORKDIR /
# Tue, 17 Mar 2020 17:36:57 GMT
CMD ["perl5.30.2" "-de0"]
```

-	Layers:
	-	`sha256:0e67f89df0287dbfef2de6d9322fee00ab623a93704fcb288963b8d51d7dfffe`  
		Last Modified: Wed, 26 Feb 2020 01:11:47 GMT  
		Size: 19.3 MB (19298348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63ac4cdfc390dfcde2655461c2c576e2f45649274ba8ed16acccacd0ed866401`  
		Last Modified: Wed, 26 Feb 2020 08:27:38 GMT  
		Size: 442.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64e5450bb27f465d67b6089025aee3e9081cbbf2fe618d1a9cf319e3d81575bd`  
		Last Modified: Tue, 17 Mar 2020 20:32:10 GMT  
		Size: 13.5 MB (13474543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:5-slim-stretch` - linux; arm64 variant v8

```console
$ docker pull perl@sha256:de8b92e219c4833abaeef91d529fb5c94ef1e58781869ed769195aef0c5f37d6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.5 MB (34527104 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fbd7904c8ca01818140e77dec16df6e4cc0ad736cc16e06e6925e85fc39c8732`
-	Default Command: `["perl5.30.2","-de0"]`

```dockerfile
# Wed, 26 Feb 2020 00:50:58 GMT
ADD file:9a0fcb77e697946112f14ff0a4dfe61aa0be45f648262b8e0be116e289964e4d in / 
# Wed, 26 Feb 2020 00:51:07 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 08:33:56 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Wed, 26 Feb 2020 08:33:56 GMT
COPY file:15650064fd29deac721f0aa084ddb3d41db77b78e2907775e257bd67e116ade4 in /usr/src/perl/ 
# Wed, 26 Feb 2020 08:33:57 GMT
WORKDIR /usr/src/perl
# Tue, 17 Mar 2020 17:19:16 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        xz-utils     && curl -SL https://www.cpan.org/src/5.0/perl-5.30.2.tar.xz -o perl-5.30.2.tar.xz     && echo 'a1aa88bd6fbbdc2e82938afbb76c408b0ea847317737b712dc196cc7907a5259 *perl-5.30.2.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.30.2.tar.xz -C /usr/src/perl     && rm perl-5.30.2.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && savedPackages="make netbase"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Tue, 17 Mar 2020 17:19:18 GMT
WORKDIR /
# Tue, 17 Mar 2020 17:19:18 GMT
CMD ["perl5.30.2" "-de0"]
```

-	Layers:
	-	`sha256:81610314811e98d4dba43f609b410f2d09dbcd135dc4cd4d8293fec3644dbea8`  
		Last Modified: Wed, 26 Feb 2020 00:58:54 GMT  
		Size: 20.4 MB (20369979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8e01f2c0bbce2d7a2214b0adbae3d2987024315a7af56f98640dbc4564582ab`  
		Last Modified: Wed, 26 Feb 2020 11:50:08 GMT  
		Size: 442.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0969bda1ca7fe182bd8c0dc5a6b1eaced2ea06c8504c639b5a13ccc3e9fd314`  
		Last Modified: Tue, 17 Mar 2020 20:18:24 GMT  
		Size: 14.2 MB (14156683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:5-slim-stretch` - linux; 386

```console
$ docker pull perl@sha256:46a486683660cde3ad09505edb491e80323fb90f0774ef09199472ee529750ef
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.0 MB (36964476 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a05e1bd0406272fe393c97b9b0b9a973cb7c5503f65f07be8de341f8945bc88c`
-	Default Command: `["perl5.30.2","-de0"]`

```dockerfile
# Wed, 26 Feb 2020 00:35:41 GMT
ADD file:7d77438aab7eb35501c0d27bd4350a3a9b4fd1988ce7e7fc0670a570b3112590 in / 
# Wed, 26 Feb 2020 00:35:42 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 06:14:39 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Wed, 26 Feb 2020 06:14:39 GMT
COPY file:15650064fd29deac721f0aa084ddb3d41db77b78e2907775e257bd67e116ade4 in /usr/src/perl/ 
# Wed, 26 Feb 2020 06:14:40 GMT
WORKDIR /usr/src/perl
# Tue, 17 Mar 2020 17:14:23 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        xz-utils     && curl -SL https://www.cpan.org/src/5.0/perl-5.30.2.tar.xz -o perl-5.30.2.tar.xz     && echo 'a1aa88bd6fbbdc2e82938afbb76c408b0ea847317737b712dc196cc7907a5259 *perl-5.30.2.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.30.2.tar.xz -C /usr/src/perl     && rm perl-5.30.2.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && savedPackages="make netbase"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Tue, 17 Mar 2020 17:14:23 GMT
WORKDIR /
# Tue, 17 Mar 2020 17:14:23 GMT
CMD ["perl5.30.2" "-de0"]
```

-	Layers:
	-	`sha256:5cf237473070a9ef7639307699a23bb6c32cd8321bf84c0cf61b6f9c32b44341`  
		Last Modified: Wed, 26 Feb 2020 00:42:02 GMT  
		Size: 23.1 MB (23141399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f1462d135f655a38ed8ab22e06c3942f06e9197e321bdc1c503b6aa321a11c1`  
		Last Modified: Wed, 26 Feb 2020 10:46:32 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a646d35215b251e399fe8b67ffcc7c08a93dbbf4d74c5b8630faba939552d98f`  
		Last Modified: Tue, 17 Mar 2020 21:43:45 GMT  
		Size: 13.8 MB (13822663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:5-slim-stretch` - linux; ppc64le

```console
$ docker pull perl@sha256:1d46b44be4a5a1bd46142ff22844eedae3b1abb255343a6bb833e2ea8e6c286b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.0 MB (36972973 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4e878505d2c65e4181933b29cf46b0df24ffe2c05e97027d55bb65835389ade`
-	Default Command: `["perl5.30.2","-de0"]`

```dockerfile
# Wed, 26 Feb 2020 01:37:18 GMT
ADD file:661513607cf6a4c5038d6048ea16a04dedb05c03ce6c0e33e409f51510562e11 in / 
# Wed, 26 Feb 2020 01:37:25 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 09:52:58 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Wed, 26 Feb 2020 09:53:00 GMT
COPY file:15650064fd29deac721f0aa084ddb3d41db77b78e2907775e257bd67e116ade4 in /usr/src/perl/ 
# Wed, 26 Feb 2020 09:53:03 GMT
WORKDIR /usr/src/perl
# Tue, 17 Mar 2020 17:52:48 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        xz-utils     && curl -SL https://www.cpan.org/src/5.0/perl-5.30.2.tar.xz -o perl-5.30.2.tar.xz     && echo 'a1aa88bd6fbbdc2e82938afbb76c408b0ea847317737b712dc196cc7907a5259 *perl-5.30.2.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.30.2.tar.xz -C /usr/src/perl     && rm perl-5.30.2.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && savedPackages="make netbase"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Tue, 17 Mar 2020 17:52:58 GMT
WORKDIR /
# Tue, 17 Mar 2020 17:53:02 GMT
CMD ["perl5.30.2" "-de0"]
```

-	Layers:
	-	`sha256:21d148b1dce5a6179231486bac7845a111bbaba4fcaf4232bbc39842bf6c5366`  
		Last Modified: Wed, 26 Feb 2020 02:04:13 GMT  
		Size: 22.8 MB (22785269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c3cbcbeeb2c913c59aa925fb5c941eef53fb59eeee409ae261f45c75e05ce8a`  
		Last Modified: Wed, 26 Feb 2020 12:39:55 GMT  
		Size: 441.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baef673b1cb1f0218109b73f954adaedfda1ef1fd41d96270de7d89545da3139`  
		Last Modified: Tue, 17 Mar 2020 20:45:00 GMT  
		Size: 14.2 MB (14187263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:5-slim-stretch` - linux; s390x

```console
$ docker pull perl@sha256:f687042bc1d2bcf40c2f2f786d531f01a34fbe40d8d4c1b382702c59329e4da6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.2 MB (37160696 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b66b59f7abb33b1c7e04972befe2ac82082e88620d42b189d6b7506234e1de23`
-	Default Command: `["perl5.30.2","-de0"]`

```dockerfile
# Tue, 31 Mar 2020 01:10:34 GMT
ADD file:6e9e5d781c6539464e26848fbf62d2af4e1981f3edb1c6cd7b2bbbb141593c0d in / 
# Tue, 31 Mar 2020 01:10:35 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 03:28:06 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Tue, 31 Mar 2020 03:28:06 GMT
COPY file:15650064fd29deac721f0aa084ddb3d41db77b78e2907775e257bd67e116ade4 in /usr/src/perl/ 
# Tue, 31 Mar 2020 03:28:06 GMT
WORKDIR /usr/src/perl
# Tue, 31 Mar 2020 03:32:26 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        xz-utils     && curl -SL https://www.cpan.org/src/5.0/perl-5.30.2.tar.xz -o perl-5.30.2.tar.xz     && echo 'a1aa88bd6fbbdc2e82938afbb76c408b0ea847317737b712dc196cc7907a5259 *perl-5.30.2.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.30.2.tar.xz -C /usr/src/perl     && rm perl-5.30.2.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && savedPackages="make netbase"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Tue, 31 Mar 2020 03:32:27 GMT
WORKDIR /
# Tue, 31 Mar 2020 03:32:27 GMT
CMD ["perl5.30.2" "-de0"]
```

-	Layers:
	-	`sha256:dd13cd38a69bea5bf9b51ea258a456377b153ad92cc7940735f837ffc48e3aa3`  
		Last Modified: Tue, 31 Mar 2020 01:14:18 GMT  
		Size: 22.4 MB (22365290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c8948242cb69106743f2883f51e37848f1319d9161b988ca45d666d2dff5bc2`  
		Last Modified: Tue, 31 Mar 2020 05:05:18 GMT  
		Size: 443.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f050f2aa0a8bf0274b1f75315984276d0de89fbffefabb74c0441afc84389693`  
		Last Modified: Tue, 31 Mar 2020 05:05:27 GMT  
		Size: 14.8 MB (14794963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
