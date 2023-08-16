## `perl:stable-threaded-buster`

```console
$ docker pull perl@sha256:6b4773d9f6aafd85d2b61f707c8c091427679924780ce814ce899656fee57a4a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `perl:stable-threaded-buster` - linux; amd64

```console
$ docker pull perl@sha256:82b8c2c519b8d73abd2dc87c0703a52a60244f3d6ff33338631024bf2804a7af
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **327.6 MB (327568839 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d72f688a0b314f72e62be49c6609258e9c53b80b58216369afd2c591399ed6d`
-	Default Command: `["perl5.38.0","-de0"]`

```dockerfile
# Thu, 27 Jul 2023 23:25:17 GMT
ADD file:46b31c893ada083f38702e21d80e5ea4b674cbc78bddd3d80020d7b8e8beb467 in / 
# Thu, 27 Jul 2023 23:25:18 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 03:03:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 03:04:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 03:05:04 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 06:55:22 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Fri, 28 Jul 2023 06:55:22 GMT
WORKDIR /usr/src/perl
# Tue, 01 Aug 2023 00:12:25 GMT
RUN true     && curl -fL https://www.cpan.org/src/5.0/perl-5.38.0.tar.xz -o perl-5.38.0.tar.xz     && echo 'eca551caec3bc549a4e590c0015003790bdd1a604ffe19cc78ee631d51f7072e *perl-5.38.0.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.38.0.tar.xz -C /usr/src/perl     && rm perl-5.38.0.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && true     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Fri, 04 Aug 2023 00:40:42 GMT
WORKDIR /usr/src/app
# Fri, 04 Aug 2023 00:40:42 GMT
CMD ["perl5.38.0" "-de0"]
```

-	Layers:
	-	`sha256:9918064ebccea7fc961fe71dad46105b217763b4b1b3a9dfa7bee2ab29d2039b`  
		Last Modified: Thu, 27 Jul 2023 23:30:27 GMT  
		Size: 50.5 MB (50497996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2345e1e5f82d8963240db3c8e8ccfd431d0962d14219e24bbcc756ef217bba48`  
		Last Modified: Fri, 28 Jul 2023 03:09:21 GMT  
		Size: 17.6 MB (17579504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:947969e624beff93eed664f9f52a08712f3d1e12cadbdf929ff928f93d2c383c`  
		Last Modified: Fri, 28 Jul 2023 03:09:36 GMT  
		Size: 51.9 MB (51872820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87da2254b9de06a71bc1828dec0a28f6a16af7cade75310533cf5cff9ac7e669`  
		Last Modified: Fri, 28 Jul 2023 03:10:06 GMT  
		Size: 191.9 MB (191895767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f52bd830833c41101843f61fc2ff200672a8cbf126df8e26936f48a48ee1fba2`  
		Last Modified: Fri, 28 Jul 2023 10:35:08 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a7c45c8ea4386d207a13b73e611bf25080a2cade4e6aa55246aa3df7fbe882d`  
		Last Modified: Tue, 01 Aug 2023 03:16:21 GMT  
		Size: 15.7 MB (15722418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a24fc975eccc39c76e4f5db32532d4b9c2822026d290fc8145894c6ad65ed9cc`  
		Last Modified: Fri, 04 Aug 2023 00:45:33 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:stable-threaded-buster` - linux; arm variant v7

```console
$ docker pull perl@sha256:a06fd429f98b12a1c4f6d986e66b31244d96f46432af9e83b3d0ad53155ec97f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **292.4 MB (292445079 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:afea1e74fd643a132d3706fbe199109c2e2ba6f34d21f046b52fd2b1bfeb9c28`
-	Default Command: `["perl5.38.0","-de0"]`

```dockerfile
# Wed, 16 Aug 2023 00:17:42 GMT
ADD file:9ad3ed36bade2e2cd71bd8f66dc47946e90d205f1846692ae9c240560758b4f4 in / 
# Wed, 16 Aug 2023 00:17:43 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 05:31:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 05:32:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 05:33:49 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 08:07:52 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Wed, 16 Aug 2023 08:07:52 GMT
WORKDIR /usr/src/perl
# Wed, 16 Aug 2023 08:49:11 GMT
RUN true     && curl -fL https://www.cpan.org/src/5.0/perl-5.38.0.tar.xz -o perl-5.38.0.tar.xz     && echo 'eca551caec3bc549a4e590c0015003790bdd1a604ffe19cc78ee631d51f7072e *perl-5.38.0.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.38.0.tar.xz -C /usr/src/perl     && rm perl-5.38.0.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && true     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Wed, 16 Aug 2023 08:49:11 GMT
WORKDIR /usr/src/app
# Wed, 16 Aug 2023 08:49:11 GMT
CMD ["perl5.38.0" "-de0"]
```

-	Layers:
	-	`sha256:ed63aeb0ff951576d398ae0e8de7a2dc582157c60523055321f47ef26ce88e00`  
		Last Modified: Wed, 16 Aug 2023 00:22:28 GMT  
		Size: 46.0 MB (45966229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee91fed073f248f84b680e14ae33a93203a05d62cf51fef886cd7ce0b3ac7d45`  
		Last Modified: Wed, 16 Aug 2023 05:49:50 GMT  
		Size: 16.2 MB (16211917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fed6203f3da20d3e0f8ea7d7ec6e4fdd2cafd582b494e1e9fda0ddf4f9a1a2f5`  
		Last Modified: Wed, 16 Aug 2023 05:50:05 GMT  
		Size: 47.4 MB (47370312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e36d2cb1f3e23c88fb017f1bb7af1d240169a419bc5190369b10152b8b8255ef`  
		Last Modified: Wed, 16 Aug 2023 05:50:34 GMT  
		Size: 168.1 MB (168099748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:676620fccb0bc72360ab9273d09c6555036ecd7172c47b317d6c016a10138e01`  
		Last Modified: Wed, 16 Aug 2023 11:55:55 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abb0c70e9bd2b202feda38471f29d53a83bf0f71a942d06d18fef0dbdec6a571`  
		Last Modified: Wed, 16 Aug 2023 11:58:10 GMT  
		Size: 14.8 MB (14796539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f1673380ad08786b1afbb5a7a2274919238f31083f67699b0ff3c2d96e29338`  
		Last Modified: Wed, 16 Aug 2023 11:58:06 GMT  
		Size: 165.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:stable-threaded-buster` - linux; arm64 variant v8

```console
$ docker pull perl@sha256:00a3cfa101ffa17fc3159966e2c0e04f4cb7d761981bfa90c69706959f0f7a6e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **318.1 MB (318051376 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66cb30bbbb8cf57b0330420a0e432aa96546ec70b00f0363b030012f2e18d80e`
-	Default Command: `["perl5.38.0","-de0"]`

```dockerfile
# Tue, 15 Aug 2023 23:40:18 GMT
ADD file:366546a703fa234d38591d2a54f10fbced83cc0e407775ad31751f0111c348c8 in / 
# Tue, 15 Aug 2023 23:40:18 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:24:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:24:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:25:49 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 10:48:08 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Wed, 16 Aug 2023 10:48:08 GMT
WORKDIR /usr/src/perl
# Wed, 16 Aug 2023 11:20:02 GMT
RUN true     && curl -fL https://www.cpan.org/src/5.0/perl-5.38.0.tar.xz -o perl-5.38.0.tar.xz     && echo 'eca551caec3bc549a4e590c0015003790bdd1a604ffe19cc78ee631d51f7072e *perl-5.38.0.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.38.0.tar.xz -C /usr/src/perl     && rm perl-5.38.0.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && true     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Wed, 16 Aug 2023 11:20:03 GMT
WORKDIR /usr/src/app
# Wed, 16 Aug 2023 11:20:03 GMT
CMD ["perl5.38.0" "-de0"]
```

-	Layers:
	-	`sha256:745797452665e0b4d6f5d0f9b05ae67a86bccfea4ec3a2cf7c6dd89cbfafdd37`  
		Last Modified: Tue, 15 Aug 2023 23:44:16 GMT  
		Size: 49.3 MB (49290964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0d4e21e88dbd3e72136906f1d37cb7c9b29c4a4c107fbe1c8b0385f5e663d2e`  
		Last Modified: Wed, 16 Aug 2023 01:40:15 GMT  
		Size: 17.5 MB (17450999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed6dff3c26e414861add902b18ad78500d9300d96e33af1ad4d3795dc9cf10cd`  
		Last Modified: Wed, 16 Aug 2023 01:40:28 GMT  
		Size: 52.2 MB (52218377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e89467a67e13dedd46298880cc34cb6a78d65e3f4c66175ee80f87892403a46`  
		Last Modified: Wed, 16 Aug 2023 01:40:52 GMT  
		Size: 183.5 MB (183463629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dc750704645a351c4fbf14d9dbf035b612dc136e2788ca0c16f132942fa127b`  
		Last Modified: Wed, 16 Aug 2023 13:47:59 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69aa7d5c710964c4b22a7f5e4039baf603284bacf79bb2cd8f71a634525618c4`  
		Last Modified: Wed, 16 Aug 2023 13:50:05 GMT  
		Size: 15.6 MB (15627075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99914d754bd1456ef802711bdb214b334bdf08cfc52a291ad7706af76bc7ae05`  
		Last Modified: Wed, 16 Aug 2023 13:50:01 GMT  
		Size: 165.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:stable-threaded-buster` - linux; 386

```console
$ docker pull perl@sha256:71b83feceb158bfe8cf806ae6f3968cb789600e58e09d2e3bbf6e2f32c6e287c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **336.5 MB (336545725 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1448c78dc7411fe27403a37c32baa69fc1ba0eef462c2562ca083aac292039a1`
-	Default Command: `["perl5.38.0","-de0"]`

```dockerfile
# Thu, 27 Jul 2023 23:39:29 GMT
ADD file:a4caa39d69b463e1f2628cb32f33763655fd873129cf98dd26c431183c53b6d6 in / 
# Thu, 27 Jul 2023 23:39:29 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 09:06:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 09:07:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 09:09:13 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 29 Jul 2023 00:44:24 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Sat, 29 Jul 2023 00:44:24 GMT
WORKDIR /usr/src/perl
# Tue, 01 Aug 2023 01:05:14 GMT
RUN true     && curl -fL https://www.cpan.org/src/5.0/perl-5.38.0.tar.xz -o perl-5.38.0.tar.xz     && echo 'eca551caec3bc549a4e590c0015003790bdd1a604ffe19cc78ee631d51f7072e *perl-5.38.0.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.38.0.tar.xz -C /usr/src/perl     && rm perl-5.38.0.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Dusethreads -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && true     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Thu, 03 Aug 2023 23:38:47 GMT
WORKDIR /usr/src/app
# Thu, 03 Aug 2023 23:38:47 GMT
CMD ["perl5.38.0" "-de0"]
```

-	Layers:
	-	`sha256:4b5eb5e3691ae17e5aaa83c175523a7a17d58c9c61698ed6bba826d9acc809ec`  
		Last Modified: Thu, 27 Jul 2023 23:44:34 GMT  
		Size: 51.3 MB (51255427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b5fa9e12702be5eb86cf811e1d9eb57dd1e12b8e78f486b34d0db5316aba76a`  
		Last Modified: Fri, 28 Jul 2023 09:13:35 GMT  
		Size: 18.1 MB (18095720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82def7be0b44871538e1d9ce871e50fdcfe67a2b50c5c5a0be050ff28e4dd86e`  
		Last Modified: Fri, 28 Jul 2023 09:13:54 GMT  
		Size: 53.5 MB (53486237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4f916c8a05f9e0bad65e551e5b8af8437f43ce16ed73a1d5d390b3c5f1c5ad3`  
		Last Modified: Fri, 28 Jul 2023 09:14:36 GMT  
		Size: 198.4 MB (198441374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfb7b07bb206df3eea7d3a6781445698dbf0dc008b265d101297f21de8a1fecd`  
		Last Modified: Sat, 29 Jul 2023 03:40:25 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45058cf9c6474816471ffd51ae33c9ea03465a875ad014cfe4ef2babeba91df0`  
		Last Modified: Tue, 01 Aug 2023 06:25:57 GMT  
		Size: 15.3 MB (15266634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a7a2157c7e4638eafa7e8a682c3131c234a6e446f815c0e3327d32cd2ef71ae`  
		Last Modified: Thu, 03 Aug 2023 23:43:40 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
