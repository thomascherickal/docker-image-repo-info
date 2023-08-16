## `perl:5-buster`

```console
$ docker pull perl@sha256:8e139a42d358750497d8e7b12c7f8ab6685298b4b87152b98679c89a57ad3e1e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `perl:5-buster` - linux; amd64

```console
$ docker pull perl@sha256:2c93068865eb7349be632bfe10e521c045d320472799704902da72b18e2fba1d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **327.5 MB (327509907 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a43d2893d147dc2fd5fe24ead169fb6571467f799f99aa4114324c7117c43f35`
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
# Mon, 31 Jul 2023 23:36:50 GMT
RUN true     && curl -fL https://www.cpan.org/src/5.0/perl-5.38.0.tar.xz -o perl-5.38.0.tar.xz     && echo 'eca551caec3bc549a4e590c0015003790bdd1a604ffe19cc78ee631d51f7072e *perl-5.38.0.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.38.0.tar.xz -C /usr/src/perl     && rm perl-5.38.0.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && true     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Fri, 04 Aug 2023 00:40:26 GMT
WORKDIR /usr/src/app
# Fri, 04 Aug 2023 00:40:26 GMT
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
	-	`sha256:fda2abeb146d5dd062fbe8237be983644ab1d536f25af54c51a599f282b6a374`  
		Last Modified: Tue, 01 Aug 2023 03:14:10 GMT  
		Size: 15.7 MB (15663486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fd5132eb21bdca850359fccac2d01bc38b6a7c70938d341b73e57379abeff61`  
		Last Modified: Fri, 04 Aug 2023 00:43:52 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:5-buster` - linux; arm variant v7

```console
$ docker pull perl@sha256:94a5bd156f5c57ec51900b0e48a1b69fecf5770f8f1fb3a5d9ce2497c6b54de4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **292.4 MB (292423704 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf1a9d89c0e5ffd150b6ecfbbec067e27a6a792a03ad9189bd9b904aa59338b4`
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
# Wed, 16 Aug 2023 08:13:07 GMT
RUN true     && curl -fL https://www.cpan.org/src/5.0/perl-5.38.0.tar.xz -o perl-5.38.0.tar.xz     && echo 'eca551caec3bc549a4e590c0015003790bdd1a604ffe19cc78ee631d51f7072e *perl-5.38.0.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.38.0.tar.xz -C /usr/src/perl     && rm perl-5.38.0.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && true     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Wed, 16 Aug 2023 08:13:07 GMT
WORKDIR /usr/src/app
# Wed, 16 Aug 2023 08:13:07 GMT
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
	-	`sha256:38595010925bf470fd5cf4bb271f6a31937961405fbbd69a4fadb33d3eef238a`  
		Last Modified: Wed, 16 Aug 2023 11:56:00 GMT  
		Size: 14.8 MB (14775164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bb275d15ba77b00c6a3368babd805dd46865d2d588c42820a73963b9ee3d3ec`  
		Last Modified: Wed, 16 Aug 2023 11:55:55 GMT  
		Size: 165.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:5-buster` - linux; arm64 variant v8

```console
$ docker pull perl@sha256:10b6f9c2a8d1dd77972a78f9b8aa45f2ef21131c3f588e8de745de5f7a630aaf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **318.0 MB (318017261 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f87f740202bc360cf262d4ba88f60a6a1e69491a9bef02130ccf2d3ec2f53c2`
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
# Wed, 16 Aug 2023 10:52:17 GMT
RUN true     && curl -fL https://www.cpan.org/src/5.0/perl-5.38.0.tar.xz -o perl-5.38.0.tar.xz     && echo 'eca551caec3bc549a4e590c0015003790bdd1a604ffe19cc78ee631d51f7072e *perl-5.38.0.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.38.0.tar.xz -C /usr/src/perl     && rm perl-5.38.0.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && true     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Wed, 16 Aug 2023 10:52:17 GMT
WORKDIR /usr/src/app
# Wed, 16 Aug 2023 10:52:17 GMT
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
	-	`sha256:904113149b7463c8da436d6367a53d48fc16cf8dab033926779c23f6c38d564d`  
		Last Modified: Wed, 16 Aug 2023 13:48:01 GMT  
		Size: 15.6 MB (15592960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d17da4da6d95060aed7a172da722a9253e8e577bc5adfbc895676d57e3cc2e94`  
		Last Modified: Wed, 16 Aug 2023 13:47:59 GMT  
		Size: 165.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:5-buster` - linux; 386

```console
$ docker pull perl@sha256:899a6f5048d38f93168c0a6db3745af3851916a3ab2c12bc3de6924443451d4c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **336.4 MB (336444108 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d84c0ab1dbc6e8da1d189961e3f816bd26fc1a37d5e7f463601c831e80445b20`
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
# Tue, 01 Aug 2023 00:06:05 GMT
RUN true     && curl -fL https://www.cpan.org/src/5.0/perl-5.38.0.tar.xz -o perl-5.38.0.tar.xz     && echo 'eca551caec3bc549a4e590c0015003790bdd1a604ffe19cc78ee631d51f7072e *perl-5.38.0.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.38.0.tar.xz -C /usr/src/perl     && rm perl-5.38.0.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local  -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7047.tar.gz     && echo '963e63c6e1a8725ff2f624e9086396ae150db51dd0a337c3781d09a994af05a5 *App-cpanminus-1.7047.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7047.tar.gz && cd App-cpanminus-1.7047 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && true     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7047* /tmp/*     && cpanm --version && cpm --version
# Thu, 03 Aug 2023 23:38:36 GMT
WORKDIR /usr/src/app
# Thu, 03 Aug 2023 23:38:36 GMT
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
	-	`sha256:86d842f9326af455ffa24e79fd04eb5f4901b5786add2ca93e94912bc1efe618`  
		Last Modified: Tue, 01 Aug 2023 06:23:40 GMT  
		Size: 15.2 MB (15165016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30aaddbface32fd9977b7455e9f22fd9d4c0efcf928ef04adec27dd753fbb0eb`  
		Last Modified: Thu, 03 Aug 2023 23:41:58 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
