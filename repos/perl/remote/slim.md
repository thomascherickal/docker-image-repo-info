## `perl:slim`

```console
$ docker pull perl@sha256:3eca8820f48c63bc52760ac2e5ba4560f6c805cb4ead153349cfcdbde1257dae
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `perl:slim` - linux; amd64

```console
$ docker pull perl@sha256:948844de9e032e6b3997ec779a7549ab9238e567fa1a0e1d695f1f541a175ccd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.0 MB (41994795 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b19cd7670ac4f9696692b9c863f7a37ffd53eead7624cb8f4fa7a221d14d062`
-	Default Command: `["perl5.34.0","-de0"]`

```dockerfile
# Tue, 12 Oct 2021 01:21:05 GMT
ADD file:910392427fdf089bc26b64d6dc450ff3d020c7c1a474d85b2f9298134d0007bd in / 
# Tue, 12 Oct 2021 01:21:05 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 12:46:02 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Tue, 12 Oct 2021 12:46:02 GMT
COPY file:3744c5cc39cdbdcae10db09a1f0f399005a79f93c237b387a72ff5710cdd458c in /usr/src/perl/ 
# Tue, 12 Oct 2021 12:46:02 GMT
WORKDIR /usr/src/perl
# Tue, 12 Oct 2021 12:54:55 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        xz-utils     && curl -SL https://www.cpan.org/src/5.0/perl-5.34.0.tar.xz -o perl-5.34.0.tar.xz     && echo '82c2e5e5c71b0e10487a80d79140469ab1f8056349ca8545140a224dbbed7ded *perl-5.34.0.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.34.0.tar.xz -C /usr/src/perl     && rm perl-5.34.0.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && savedPackages="make netbase"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Tue, 12 Oct 2021 12:54:55 GMT
WORKDIR /
# Tue, 12 Oct 2021 12:54:56 GMT
CMD ["perl5.34.0" "-de0"]
```

-	Layers:
	-	`sha256:b380bbd43752f83945df8b5d1074fef8dd044820e7d3aef33b655a2483e030c7`  
		Last Modified: Tue, 12 Oct 2021 01:26:51 GMT  
		Size: 27.1 MB (27139510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4567231533a0e25f697e4a77bc07a5169e6a61777392e52f5813637087295990`  
		Last Modified: Tue, 12 Oct 2021 14:25:21 GMT  
		Size: 202.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7d577cc518d7221756c4e449787a732014f717b49242ce1b5f2e5885f555d66`  
		Last Modified: Tue, 12 Oct 2021 14:25:24 GMT  
		Size: 14.9 MB (14855083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:slim` - linux; arm variant v7

```console
$ docker pull perl@sha256:64e986de8a355569e503a9af916639ffb0ae991deebbb9dd5c38409d70259d7d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.7 MB (36716529 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53f09b257009d17633e1d8d8b6038f3c0956fe35070a0346f4129761f3b02f39`
-	Default Command: `["perl5.34.0","-de0"]`

```dockerfile
# Tue, 12 Oct 2021 01:29:42 GMT
ADD file:fe1eaa1b1d760b3d250cb4ac331d26a261fc569f1694bd34e146f00874dc87e5 in / 
# Tue, 12 Oct 2021 01:29:43 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 07:56:04 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Tue, 12 Oct 2021 07:56:04 GMT
COPY file:3744c5cc39cdbdcae10db09a1f0f399005a79f93c237b387a72ff5710cdd458c in /usr/src/perl/ 
# Tue, 12 Oct 2021 07:56:05 GMT
WORKDIR /usr/src/perl
# Tue, 12 Oct 2021 08:07:51 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        xz-utils     && curl -SL https://www.cpan.org/src/5.0/perl-5.34.0.tar.xz -o perl-5.34.0.tar.xz     && echo '82c2e5e5c71b0e10487a80d79140469ab1f8056349ca8545140a224dbbed7ded *perl-5.34.0.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.34.0.tar.xz -C /usr/src/perl     && rm perl-5.34.0.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && savedPackages="make netbase"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Tue, 12 Oct 2021 08:07:52 GMT
WORKDIR /
# Tue, 12 Oct 2021 08:07:52 GMT
CMD ["perl5.34.0" "-de0"]
```

-	Layers:
	-	`sha256:c0b5ba470cac8cfdae4633f5cddb3ba9350fe1d1b1507c4965a8224eb40e52c5`  
		Last Modified: Tue, 12 Oct 2021 01:45:52 GMT  
		Size: 22.7 MB (22739698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:214ca94bd1c298df274fb11c742323a10ee96cb83bbe145947f45cdfae8018e2`  
		Last Modified: Tue, 12 Oct 2021 10:02:32 GMT  
		Size: 202.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6850abc078a1b48797d76b71dd2f908a12e6d4bc966ca0a4ed551823481f96d2`  
		Last Modified: Tue, 12 Oct 2021 10:02:44 GMT  
		Size: 14.0 MB (13976629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:slim` - linux; arm64 variant v8

```console
$ docker pull perl@sha256:7794002f903da360e5ec8872f999e5a1e72174fbe75862955df3d365eb0a80a7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.7 MB (40710948 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:270c471f8f9f3874be829d7b499a1a6a789dc884b00d8de78443add18d05d390`
-	Default Command: `["perl5.34.0","-de0"]`

```dockerfile
# Tue, 12 Oct 2021 01:41:42 GMT
ADD file:f0d53027a7ba594477674127971aa477af3a2bc6bcddef6c0aa174953a5f2db0 in / 
# Tue, 12 Oct 2021 01:41:42 GMT
CMD ["bash"]
# Wed, 13 Oct 2021 11:53:54 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Wed, 13 Oct 2021 11:53:56 GMT
COPY file:3744c5cc39cdbdcae10db09a1f0f399005a79f93c237b387a72ff5710cdd458c in /usr/src/perl/ 
# Wed, 13 Oct 2021 11:53:56 GMT
WORKDIR /usr/src/perl
# Wed, 13 Oct 2021 11:57:46 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        xz-utils     && curl -SL https://www.cpan.org/src/5.0/perl-5.34.0.tar.xz -o perl-5.34.0.tar.xz     && echo '82c2e5e5c71b0e10487a80d79140469ab1f8056349ca8545140a224dbbed7ded *perl-5.34.0.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.34.0.tar.xz -C /usr/src/perl     && rm perl-5.34.0.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && savedPackages="make netbase"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Wed, 13 Oct 2021 11:57:46 GMT
WORKDIR /
# Wed, 13 Oct 2021 11:57:47 GMT
CMD ["perl5.34.0" "-de0"]
```

-	Layers:
	-	`sha256:02b45931a436a68cadb742684148ed6aacbbf9aa21447b467c11bac97f92eb46`  
		Last Modified: Tue, 12 Oct 2021 01:49:07 GMT  
		Size: 25.9 MB (25908479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6836adfdeee224a05bfda73269ca9b2e7b6fd9ca210ac24a3cf66623aedd5840`  
		Last Modified: Wed, 13 Oct 2021 13:15:10 GMT  
		Size: 180.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69a0912e3263f8a93a4fc3dc22e86dd8609470e947def764918607e6fde3a1eb`  
		Last Modified: Wed, 13 Oct 2021 13:15:13 GMT  
		Size: 14.8 MB (14802289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:slim` - linux; 386

```console
$ docker pull perl@sha256:d3b19e767d5e51599f1b07f7547df5f65bfb0f32739538c2e10fe0baf8116ae9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.2 MB (42152682 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ced3d55101a2ffed1a748f99093aa9a878cd1c302f09194ae57e9f3dd62025f9`
-	Default Command: `["perl5.34.0","-de0"]`

```dockerfile
# Tue, 12 Oct 2021 01:40:17 GMT
ADD file:1b432d2306b487c59442b30c65ddabd08b45484c6ce09b0c25112c29f4a98f17 in / 
# Tue, 12 Oct 2021 01:40:17 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 02:43:46 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Tue, 12 Oct 2021 02:43:46 GMT
COPY file:3744c5cc39cdbdcae10db09a1f0f399005a79f93c237b387a72ff5710cdd458c in /usr/src/perl/ 
# Tue, 12 Oct 2021 02:43:47 GMT
WORKDIR /usr/src/perl
# Tue, 12 Oct 2021 02:53:53 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        xz-utils     && curl -SL https://www.cpan.org/src/5.0/perl-5.34.0.tar.xz -o perl-5.34.0.tar.xz     && echo '82c2e5e5c71b0e10487a80d79140469ab1f8056349ca8545140a224dbbed7ded *perl-5.34.0.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.34.0.tar.xz -C /usr/src/perl     && rm perl-5.34.0.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && savedPackages="make netbase"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Tue, 12 Oct 2021 02:53:54 GMT
WORKDIR /
# Tue, 12 Oct 2021 02:53:55 GMT
CMD ["perl5.34.0" "-de0"]
```

-	Layers:
	-	`sha256:860d012fe46ce39c3737ace24d10d8ad65ae9c78abde6891ca6e97b0d7f271dd`  
		Last Modified: Tue, 12 Oct 2021 01:48:37 GMT  
		Size: 27.8 MB (27791445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3887e9067d342f3f073184072564d4e93e59131ccf022cd4e5d792ca6631c400`  
		Last Modified: Tue, 12 Oct 2021 04:31:15 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c592258585ff2100d16e9926d3dac5d043a8d91c1ca044d096bb5d89aefb767`  
		Last Modified: Tue, 12 Oct 2021 04:31:19 GMT  
		Size: 14.4 MB (14361036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:slim` - linux; ppc64le

```console
$ docker pull perl@sha256:c6cb9cb5a7725d22eb77816403db2ffe4fecfa00f0cafb72c5b70e43b7ff9e8e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.2 MB (50161635 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6aba71138ebb915e1f847a4f8c60cf6837724b0dfd56195bd07a4786a0bf20ef`
-	Default Command: `["perl5.34.0","-de0"]`

```dockerfile
# Tue, 12 Oct 2021 01:25:45 GMT
ADD file:d8794fadf16c9948c3574ba28740d08393eca57766340333ad91f9c2a33eb719 in / 
# Tue, 12 Oct 2021 01:25:53 GMT
CMD ["bash"]
# Fri, 12 Nov 2021 23:16:51 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Fri, 12 Nov 2021 23:16:53 GMT
COPY file:3744c5cc39cdbdcae10db09a1f0f399005a79f93c237b387a72ff5710cdd458c in /usr/src/perl/ 
# Fri, 12 Nov 2021 23:16:55 GMT
WORKDIR /usr/src/perl
# Fri, 12 Nov 2021 23:27:32 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        xz-utils     && curl -SL https://www.cpan.org/src/5.0/perl-5.34.0.tar.xz -o perl-5.34.0.tar.xz     && echo '82c2e5e5c71b0e10487a80d79140469ab1f8056349ca8545140a224dbbed7ded *perl-5.34.0.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.34.0.tar.xz -C /usr/src/perl     && rm perl-5.34.0.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && savedPackages="make netbase"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Fri, 12 Nov 2021 23:27:39 GMT
WORKDIR /
# Fri, 12 Nov 2021 23:27:43 GMT
CMD ["perl5.34.0" "-de0"]
```

-	Layers:
	-	`sha256:6c28c1405c677dd809094d06190225b38cee3d24f18da38d287ef5bcc67884d6`  
		Last Modified: Tue, 12 Oct 2021 01:37:00 GMT  
		Size: 35.3 MB (35258729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2b1371965ee604f32c7ad3a1fd03776c4c61a5060e0c4d3a2086de51645e838`  
		Last Modified: Sat, 13 Nov 2021 00:59:52 GMT  
		Size: 205.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9596733db9b9d3c9ef7169d6382a386fe6063a1ce163997a81667765fbc37425`  
		Last Modified: Sat, 13 Nov 2021 00:59:55 GMT  
		Size: 14.9 MB (14902701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:slim` - linux; s390x

```console
$ docker pull perl@sha256:5dbad78889e85b8656cbed65d6e5ade6ca426ae5e633dde940d0d3d166552a71
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.9 MB (40943308 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9864365cc4354c72b5cc761e6ddd97a1cba4dee3e3d618f8ea794a6611719803`
-	Default Command: `["perl5.34.0","-de0"]`

```dockerfile
# Tue, 12 Oct 2021 00:42:56 GMT
ADD file:39da9acd4d06d69f3ca8d25ef5c097ae741972d6b15a6a057bc7487380157b61 in / 
# Tue, 12 Oct 2021 00:42:57 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 01:06:59 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Tue, 12 Oct 2021 01:06:59 GMT
COPY file:3744c5cc39cdbdcae10db09a1f0f399005a79f93c237b387a72ff5710cdd458c in /usr/src/perl/ 
# Tue, 12 Oct 2021 01:07:00 GMT
WORKDIR /usr/src/perl
# Tue, 12 Oct 2021 01:11:28 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        xz-utils     && curl -SL https://www.cpan.org/src/5.0/perl-5.34.0.tar.xz -o perl-5.34.0.tar.xz     && echo '82c2e5e5c71b0e10487a80d79140469ab1f8056349ca8545140a224dbbed7ded *perl-5.34.0.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.34.0.tar.xz -C /usr/src/perl     && rm perl-5.34.0.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && savedPackages="make netbase"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Tue, 12 Oct 2021 01:11:29 GMT
WORKDIR /
# Tue, 12 Oct 2021 01:11:29 GMT
CMD ["perl5.34.0" "-de0"]
```

-	Layers:
	-	`sha256:78a640c6bb4733e5156ce97c5ec773cf97b357c3a07244348384da5060788a61`  
		Last Modified: Tue, 12 Oct 2021 00:48:41 GMT  
		Size: 25.8 MB (25754252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:075c451d7bf4fd5a4674680be83dd5f1f0b11125b8275b931ede795d682e924b`  
		Last Modified: Tue, 12 Oct 2021 01:40:03 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e75982b9f65dbfd4537f98534fb976bbc88f63a50635be45acad69a81404229`  
		Last Modified: Tue, 12 Oct 2021 01:40:05 GMT  
		Size: 15.2 MB (15188857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
