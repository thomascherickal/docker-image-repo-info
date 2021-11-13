## `perl:slim-bullseye`

```console
$ docker pull perl@sha256:ce0b00ff6ee29d91afefa692284a659c8cca1692c996bedc26ea4c2451072dea
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; ppc64le

### `perl:slim-bullseye` - linux; ppc64le

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
