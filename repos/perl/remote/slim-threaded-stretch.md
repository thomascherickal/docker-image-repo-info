## `perl:slim-threaded-stretch`

```console
$ docker pull perl@sha256:58b5cf0343362740a6e632c0c56b93646a53a1e26b3b4ba7fffe5c05a1e83d13
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `perl:slim-threaded-stretch` - linux; amd64

```console
$ docker pull perl@sha256:33ace3b8e37bcd6961d0cdb970f257af79de6a8a221c3bbd642713f35235ed92
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.2 MB (37175965 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04eb19356f0e3c7867f908a8fb9950c7f5547a7706f30f81a4cd8f8ee72d5358`
-	Default Command: `["perl5.32.1","-de0"]`

```dockerfile
# Sat, 10 Apr 2021 01:21:54 GMT
ADD file:70cd6967491943999563ddd3ab9abae33791ac320cdc846dc57503cc44f25600 in / 
# Sat, 10 Apr 2021 01:21:54 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 08:25:31 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Sat, 10 Apr 2021 08:25:31 GMT
COPY file:3744c5cc39cdbdcae10db09a1f0f399005a79f93c237b387a72ff5710cdd458c in /usr/src/perl/ 
# Sat, 10 Apr 2021 08:25:31 GMT
WORKDIR /usr/src/perl
# Sat, 10 Apr 2021 09:20:08 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        xz-utils     && curl -SL https://www.cpan.org/src/5.0/perl-5.32.1.tar.xz -o perl-5.32.1.tar.xz     && echo '57cc47c735c8300a8ce2fa0643507b44c4ae59012bfdad0121313db639e02309 *perl-5.32.1.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.32.1.tar.xz -C /usr/src/perl     && rm perl-5.32.1.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && savedPackages="make netbase"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Sat, 10 Apr 2021 09:20:08 GMT
WORKDIR /
# Sat, 10 Apr 2021 09:20:08 GMT
CMD ["perl5.32.1" "-de0"]
```

-	Layers:
	-	`sha256:62deabe7a6db312ed773ccd640cd7cfbf51c22bf466886345684558f1036e358`  
		Last Modified: Sat, 10 Apr 2021 01:28:26 GMT  
		Size: 22.5 MB (22528265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f106b555f7e02a0e6315786fb4f656861806f8d417ded5022718eb5f02bc5068`  
		Last Modified: Sat, 10 Apr 2021 12:19:58 GMT  
		Size: 204.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2754e2c80a4b38d03f26b245525476f801ce1fb3ff5710361ddbeb8ed7c79595`  
		Last Modified: Sat, 10 Apr 2021 12:21:41 GMT  
		Size: 14.6 MB (14647496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:slim-threaded-stretch` - linux; arm variant v7

```console
$ docker pull perl@sha256:dfbf00f5ad338dfd7463038d5c83b1d81bada80f03d2af76190f1d0a7263bf85
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.1 MB (33075660 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:755d3e5a0ae045c7ab2362cf1733561c3fed0d4e34610a585cccd2309bbce5d5`
-	Default Command: `["perl5.32.1","-de0"]`

```dockerfile
# Sat, 10 Apr 2021 01:03:06 GMT
ADD file:52c199ce651b807d24bc90d10a436833911230c0a2e5a5e3bc404e8f60acf01f in / 
# Sat, 10 Apr 2021 01:03:08 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 10:04:37 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Sat, 10 Apr 2021 10:04:38 GMT
COPY file:3744c5cc39cdbdcae10db09a1f0f399005a79f93c237b387a72ff5710cdd458c in /usr/src/perl/ 
# Sat, 10 Apr 2021 10:04:39 GMT
WORKDIR /usr/src/perl
# Sat, 10 Apr 2021 10:54:12 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        xz-utils     && curl -SL https://www.cpan.org/src/5.0/perl-5.32.1.tar.xz -o perl-5.32.1.tar.xz     && echo '57cc47c735c8300a8ce2fa0643507b44c4ae59012bfdad0121313db639e02309 *perl-5.32.1.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.32.1.tar.xz -C /usr/src/perl     && rm perl-5.32.1.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && savedPackages="make netbase"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Sat, 10 Apr 2021 10:54:14 GMT
WORKDIR /
# Sat, 10 Apr 2021 10:54:15 GMT
CMD ["perl5.32.1" "-de0"]
```

-	Layers:
	-	`sha256:164ab14e0a3227bab5f842df5b955bd3fd592e0d78c5f19d2b1084d61e259f3a`  
		Last Modified: Sat, 10 Apr 2021 01:10:32 GMT  
		Size: 19.3 MB (19315172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50f757d4318ce717e416ae138065e5fdb90eee0fff41fb7849e60852567738af`  
		Last Modified: Sat, 10 Apr 2021 13:43:27 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83b933dbef980fe9b3dcb091a12520cf2cce4719b99bfcbe7c21faec74a93ac0`  
		Last Modified: Sat, 10 Apr 2021 13:44:56 GMT  
		Size: 13.8 MB (13760287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:slim-threaded-stretch` - linux; arm64 variant v8

```console
$ docker pull perl@sha256:15cbd99b916d96670cf413c9cba7aaa38c7024b362cca3775903db8b801562a7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34824260 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0175a871ed2600d1025cdde80da10c936bfcec35800bb9c1f2d270c29ed3aef9`
-	Default Command: `["perl5.32.1","-de0"]`

```dockerfile
# Sat, 10 Apr 2021 00:44:13 GMT
ADD file:a74d7856e70f2e18d2509edd9f0527254a69e9d1347715149c772a0d4ca7d509 in / 
# Sat, 10 Apr 2021 00:44:14 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 06:02:16 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Sat, 10 Apr 2021 06:02:17 GMT
COPY file:3744c5cc39cdbdcae10db09a1f0f399005a79f93c237b387a72ff5710cdd458c in /usr/src/perl/ 
# Sat, 10 Apr 2021 06:02:19 GMT
WORKDIR /usr/src/perl
# Sat, 10 Apr 2021 06:53:20 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        xz-utils     && curl -SL https://www.cpan.org/src/5.0/perl-5.32.1.tar.xz -o perl-5.32.1.tar.xz     && echo '57cc47c735c8300a8ce2fa0643507b44c4ae59012bfdad0121313db639e02309 *perl-5.32.1.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.32.1.tar.xz -C /usr/src/perl     && rm perl-5.32.1.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && savedPackages="make netbase"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Sat, 10 Apr 2021 06:53:23 GMT
WORKDIR /
# Sat, 10 Apr 2021 06:53:24 GMT
CMD ["perl5.32.1" "-de0"]
```

-	Layers:
	-	`sha256:bc16ed4a30c7b74efb2ba46d7df8a6591a02826832c27a5cf55cc6e06111a5a6`  
		Last Modified: Sat, 10 Apr 2021 00:50:10 GMT  
		Size: 20.4 MB (20389366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73e626338f6a4320ebadaa24418b4cc3f0092f74565ffa1c17f59fef872e8633`  
		Last Modified: Sat, 10 Apr 2021 09:30:27 GMT  
		Size: 204.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac0b804b91879c9e51f6cb1b2f6b0d3e71c15458ba7809cc9b2b60ed0c473887`  
		Last Modified: Sat, 10 Apr 2021 09:31:49 GMT  
		Size: 14.4 MB (14434690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:slim-threaded-stretch` - linux; 386

```console
$ docker pull perl@sha256:f95847401e5c52c4dc01e6f67b4ced774abbbeca729688563226f32b6881a3f4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.3 MB (37346064 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2eca2fe5caf0cf8cd7e4342752aed2d23e0d2f8a2575732bbeeadb9288bdcaea`
-	Default Command: `["perl5.32.1","-de0"]`

```dockerfile
# Sat, 10 Apr 2021 00:41:29 GMT
ADD file:9cb229e455510ee74de0debdecc6c327e9bda29ac2126c12d9a19d5ef8227d3a in / 
# Sat, 10 Apr 2021 00:41:29 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 04:41:33 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Sat, 10 Apr 2021 04:41:34 GMT
COPY file:3744c5cc39cdbdcae10db09a1f0f399005a79f93c237b387a72ff5710cdd458c in /usr/src/perl/ 
# Sat, 10 Apr 2021 04:41:34 GMT
WORKDIR /usr/src/perl
# Sat, 10 Apr 2021 05:48:49 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        xz-utils     && curl -SL https://www.cpan.org/src/5.0/perl-5.32.1.tar.xz -o perl-5.32.1.tar.xz     && echo '57cc47c735c8300a8ce2fa0643507b44c4ae59012bfdad0121313db639e02309 *perl-5.32.1.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.32.1.tar.xz -C /usr/src/perl     && rm perl-5.32.1.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && savedPackages="make netbase"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Sat, 10 Apr 2021 05:48:49 GMT
WORKDIR /
# Sat, 10 Apr 2021 05:48:49 GMT
CMD ["perl5.32.1" "-de0"]
```

-	Layers:
	-	`sha256:b18a2540ebf57cd924b9ebbf39001a2241653243e9ee3af58fa9f77a2644b7ee`  
		Last Modified: Sat, 10 Apr 2021 00:49:18 GMT  
		Size: 23.2 MB (23156271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72aeef5c93dee69da6062ba5dd20afb51d59fcfa596f954752817294d316f07e`  
		Last Modified: Sat, 10 Apr 2021 08:09:25 GMT  
		Size: 204.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff7cc17fd0c35e6fd16dfa54a455b8a79f08360719f46885d5f4f0bad10d7386`  
		Last Modified: Sat, 10 Apr 2021 08:11:50 GMT  
		Size: 14.2 MB (14189589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
