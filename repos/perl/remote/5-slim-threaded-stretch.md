## `perl:5-slim-threaded-stretch`

```console
$ docker pull perl@sha256:45a5c300cf5a0de1ed0047a3a30a43c6c134876385ad59f125c3cb19bfea3ef7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `perl:5-slim-threaded-stretch` - linux; amd64

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

### `perl:5-slim-threaded-stretch` - linux; arm variant v7

```console
$ docker pull perl@sha256:5f2f37cc928a0dd954b74fc212bccf90588e63303ab649a6376bd2c4aa82f9a8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.1 MB (33076602 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7596aa3e35b3c03b489261aafee80c1459f8c77a50ec012644f057592062873`
-	Default Command: `["perl5.32.1","-de0"]`

```dockerfile
# Wed, 12 May 2021 01:13:00 GMT
ADD file:3a0c44e2f78c31814d76ce91706cea345d424f8b49631a1e01dbfe768d244d48 in / 
# Wed, 12 May 2021 01:13:05 GMT
CMD ["bash"]
# Wed, 12 May 2021 07:02:16 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Wed, 12 May 2021 07:02:23 GMT
COPY file:3744c5cc39cdbdcae10db09a1f0f399005a79f93c237b387a72ff5710cdd458c in /usr/src/perl/ 
# Wed, 12 May 2021 07:02:30 GMT
WORKDIR /usr/src/perl
# Wed, 12 May 2021 07:54:36 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        xz-utils     && curl -SL https://www.cpan.org/src/5.0/perl-5.32.1.tar.xz -o perl-5.32.1.tar.xz     && echo '57cc47c735c8300a8ce2fa0643507b44c4ae59012bfdad0121313db639e02309 *perl-5.32.1.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.32.1.tar.xz -C /usr/src/perl     && rm perl-5.32.1.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && savedPackages="make netbase"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Wed, 12 May 2021 07:54:46 GMT
WORKDIR /
# Wed, 12 May 2021 07:54:54 GMT
CMD ["perl5.32.1" "-de0"]
```

-	Layers:
	-	`sha256:ce2b35672977ffba9f48ce0726706cd15d926482c1008f69213433c61ba44966`  
		Last Modified: Wed, 12 May 2021 01:21:44 GMT  
		Size: 19.3 MB (19315154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d3ee51572170eb8d3d7e28917aeebb7aca61bf41cad1aec8494e54da3e8b28e`  
		Last Modified: Wed, 12 May 2021 10:48:58 GMT  
		Size: 205.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a09f3333125fa32eb5a599a51b3faa027b0b93968d9efd0adde8f36e2d93cf87`  
		Last Modified: Wed, 12 May 2021 10:50:52 GMT  
		Size: 13.8 MB (13761243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:5-slim-threaded-stretch` - linux; arm64 variant v8

```console
$ docker pull perl@sha256:fb32f27fc36991a7246de4a56af303e579e3dc3212346caf8d76658975863075
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34824086 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4dd89376e69cfd57dace04ceb9272e399451f688ca24ef4c3040e3a883f1e7be`
-	Default Command: `["perl5.32.1","-de0"]`

```dockerfile
# Wed, 12 May 2021 00:56:51 GMT
ADD file:eb2bf800fab313cdab37eb6f5b5c82b2d95ca00628862c99520f3189748737ec in / 
# Wed, 12 May 2021 00:56:54 GMT
CMD ["bash"]
# Wed, 12 May 2021 08:29:26 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Wed, 12 May 2021 08:29:27 GMT
COPY file:3744c5cc39cdbdcae10db09a1f0f399005a79f93c237b387a72ff5710cdd458c in /usr/src/perl/ 
# Wed, 12 May 2021 08:29:27 GMT
WORKDIR /usr/src/perl
# Wed, 12 May 2021 09:20:22 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends        bzip2        ca-certificates        curl        dpkg-dev        gcc        libc6-dev        make        netbase        patch        xz-utils     && curl -SL https://www.cpan.org/src/5.0/perl-5.32.1.tar.xz -o perl-5.32.1.tar.xz     && echo '57cc47c735c8300a8ce2fa0643507b44c4ae59012bfdad0121313db639e02309 *perl-5.32.1.tar.xz' | sha256sum -c -     && tar --strip-components=1 -xaf perl-5.32.1.tar.xz -C /usr/src/perl     && rm perl-5.32.1.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -LO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7044.tar.gz     && echo '9b60767fe40752ef7a9d3f13f19060a63389a5c23acc3e9827e19b75500f81f3 *App-cpanminus-1.7044.tar.gz' | sha256sum -c -     && tar -xzf App-cpanminus-1.7044.tar.gz && cd App-cpanminus-1.7044 && perl bin/cpanm . && cd /root     && savedPackages="make netbase"     && apt-mark auto '.*' > /dev/null     && apt-mark manual $savedPackages     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && rm -fr /var/cache/apt/* /var/lib/apt/lists/*     && rm -fr ./cpanm /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7044* /tmp/*
# Wed, 12 May 2021 09:20:23 GMT
WORKDIR /
# Wed, 12 May 2021 09:20:24 GMT
CMD ["perl5.32.1" "-de0"]
```

-	Layers:
	-	`sha256:773a656fe22a8f8eb2899cb7975915653ef0213cc26c0dad998984433b56d5f5`  
		Last Modified: Wed, 12 May 2021 01:04:44 GMT  
		Size: 20.4 MB (20389317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50135dd28abf19a4e55bfe243e2027f7467a61b87b12a499270b6760c8138c47`  
		Last Modified: Wed, 12 May 2021 12:09:26 GMT  
		Size: 202.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61bb9cbd95d53fb4b2575fdcb5a59a8b3999649c0c29b2ebe90032cc774f10fb`  
		Last Modified: Wed, 12 May 2021 12:12:42 GMT  
		Size: 14.4 MB (14434567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:5-slim-threaded-stretch` - linux; 386

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
