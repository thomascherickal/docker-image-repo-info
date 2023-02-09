## `perl:devel`

```console
$ docker pull perl@sha256:7e0b9623cfabe927f34a5d905f9e2fdc4e1bdbb48e5f43a5488f059563ff712c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `perl:devel` - linux; amd64

```console
$ docker pull perl@sha256:6a432250d7bf0b736c58772a6a50e2bf9d1485cd70ac3af10eff6cfccde3957b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **338.1 MB (338138722 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba4174065cb2347e56571f5817c809301d70d145da3a7da854dd75562f136615`
-	Default Command: `["perl5.37.8","-de0"]`

```dockerfile
# Thu, 09 Feb 2023 03:20:05 GMT
ADD file:b03d13d345c29f69557f410c8504e748226756d1f48e5abdb63cd40179b2640c in / 
# Thu, 09 Feb 2023 03:20:05 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:10:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 09:10:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 09 Feb 2023 09:11:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 09:12:08 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 11:29:15 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Thu, 09 Feb 2023 11:29:15 GMT
WORKDIR /usr/src/perl
# Thu, 09 Feb 2023 13:48:51 GMT
RUN true     && curl -fL https://www.cpan.org/src/5.0/perl-5.37.8.tar.xz -o perl-5.37.8.tar.xz     && echo 'eca6396a4b1aa7a38ef467ce54ed897cc84ba948fad0f90aeb210e57b04daf3c *perl-5.37.8.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.37.8.tar.xz -C /usr/src/perl     && rm perl-5.37.8.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local -Dusedevel -Dversiononly=undef -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7046.tar.gz     && echo '3e8c9d9b44a7348f9acc917163dbfc15bd5ea72501492cea3a35b346440ff862 *App-cpanminus-1.7046.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7046.tar.gz && cd App-cpanminus-1.7046 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && true     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7046* /tmp/*     && cpanm --version && cpm --version
# Thu, 09 Feb 2023 13:48:52 GMT
WORKDIR /
# Thu, 09 Feb 2023 13:48:52 GMT
CMD ["perl5.37.8" "-de0"]
```

-	Layers:
	-	`sha256:1e4aec178e0864db93a6f97a20bde3445871a4562c1801185eca1238d3a0e80d`  
		Last Modified: Thu, 09 Feb 2023 03:24:47 GMT  
		Size: 55.0 MB (55046771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c1024729feeb2893dad43684fe7679c4d866c3640dfc3912bbd93c5a51f32d2`  
		Last Modified: Thu, 09 Feb 2023 09:17:56 GMT  
		Size: 5.2 MB (5165984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3aa11fbc85a2a9660c98cfb4d0a2db8cde983ce3c87565c356cfdf1ddf2654c`  
		Last Modified: Thu, 09 Feb 2023 09:17:56 GMT  
		Size: 10.9 MB (10876805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa54add66b3a47555c8b761f60b15f818236cc928109a30032111efc98c6fcd4`  
		Last Modified: Thu, 09 Feb 2023 09:18:15 GMT  
		Size: 54.6 MB (54587652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e3a60c2bce7eed21ed40f067f9b3491ae3e0b7a6edbc8ed5d9dc7dd9e4a0f92`  
		Last Modified: Thu, 09 Feb 2023 09:18:52 GMT  
		Size: 196.9 MB (196895515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ec67b0bdf0c51fd2f861c551f048ed6984f28757ee462dee8b9ae960fe94b3a`  
		Last Modified: Thu, 09 Feb 2023 14:31:57 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cd4fcdcea452a87862856694b47c9bef9b17850466ace24704a7103c780f58a`  
		Last Modified: Thu, 09 Feb 2023 14:38:57 GMT  
		Size: 15.6 MB (15565826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:devel` - linux; arm variant v5

```console
$ docker pull perl@sha256:86580492326d5719d1da3f69ea07105438d93a57134d26ec9c404268376d8457
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **310.4 MB (310446583 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84daffb7aeacad9a6e141c56e1db22a751feb72a7f86b27e5189adac6718673a`
-	Default Command: `["perl5.37.8","-de0"]`

```dockerfile
# Thu, 09 Feb 2023 02:00:16 GMT
ADD file:f5b31ee6dfb50a99818c1a4b3aba7c6ba1557b1547aa730e4230600017520691 in / 
# Thu, 09 Feb 2023 02:00:17 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 02:31:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 02:31:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 09 Feb 2023 02:31:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 02:32:52 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 07:45:03 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Thu, 09 Feb 2023 07:45:03 GMT
WORKDIR /usr/src/perl
# Thu, 09 Feb 2023 09:08:08 GMT
RUN true     && curl -fL https://www.cpan.org/src/5.0/perl-5.37.8.tar.xz -o perl-5.37.8.tar.xz     && echo 'eca6396a4b1aa7a38ef467ce54ed897cc84ba948fad0f90aeb210e57b04daf3c *perl-5.37.8.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.37.8.tar.xz -C /usr/src/perl     && rm perl-5.37.8.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local -Dusedevel -Dversiononly=undef -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7046.tar.gz     && echo '3e8c9d9b44a7348f9acc917163dbfc15bd5ea72501492cea3a35b346440ff862 *App-cpanminus-1.7046.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7046.tar.gz && cd App-cpanminus-1.7046 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && true     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7046* /tmp/*     && cpanm --version && cpm --version
# Thu, 09 Feb 2023 09:08:08 GMT
WORKDIR /
# Thu, 09 Feb 2023 09:08:08 GMT
CMD ["perl5.37.8" "-de0"]
```

-	Layers:
	-	`sha256:f316396b5265978a8de9d493acdc7cda735a1fae190efbd5359650183ab7271f`  
		Last Modified: Thu, 09 Feb 2023 02:05:10 GMT  
		Size: 52.6 MB (52551796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e2355e17d09850c64d649a557a5480aa67d5780f54692d771fe1c9c1a91982d`  
		Last Modified: Thu, 09 Feb 2023 02:37:33 GMT  
		Size: 5.1 MB (5072358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:033683e85ebf7bf5988c5e89fb437d067288a5d39c937e111cc7aba783033475`  
		Last Modified: Thu, 09 Feb 2023 02:37:33 GMT  
		Size: 10.6 MB (10573870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa14f2dc5a9add2b52e16a85353e1efb812f11515fa52fed1fe30ddcbd6ad55a`  
		Last Modified: Thu, 09 Feb 2023 02:37:58 GMT  
		Size: 52.3 MB (52334301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4824023e728f96a9a7331e53139208d3054c8a30e39c9e58f4b6399ef16d76f8`  
		Last Modified: Thu, 09 Feb 2023 02:38:42 GMT  
		Size: 175.1 MB (175058379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcd1a241f1d5d20e1f9ba7ec5e5148158c2cb8967a5c0af26acd2ed6c135306b`  
		Last Modified: Thu, 09 Feb 2023 09:34:03 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:152aabea0846ca6d0e145d56450f8f2a3fc2a83c265552a3ef2de047b0525821`  
		Last Modified: Thu, 09 Feb 2023 09:39:44 GMT  
		Size: 14.9 MB (14855744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:devel` - linux; arm variant v7

```console
$ docker pull perl@sha256:ca1cdb39fd32eedd081ac416ee575726011af23468118b1708408d5b517a8bdd
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **297.7 MB (297712618 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35bb2ac532981b6e65566428b1dbbd2552356346ffbebd8a5dffdc6f66a243e5`
-	Default Command: `["perl5.37.8","-de0"]`

```dockerfile
# Sat, 04 Feb 2023 09:59:19 GMT
ADD file:239b5255d05e0742f381f82fb7cd586fcc6d9a427263238a2be3372c494ae933 in / 
# Sat, 04 Feb 2023 09:59:20 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 10:49:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 10:49:12 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 04 Feb 2023 10:49:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 10:50:25 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 14:04:07 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Sat, 04 Feb 2023 14:04:07 GMT
WORKDIR /usr/src/perl
# Sat, 04 Feb 2023 16:32:37 GMT
RUN true     && curl -fL https://www.cpan.org/src/5.0/perl-5.37.8.tar.xz -o perl-5.37.8.tar.xz     && echo 'eca6396a4b1aa7a38ef467ce54ed897cc84ba948fad0f90aeb210e57b04daf3c *perl-5.37.8.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.37.8.tar.xz -C /usr/src/perl     && rm perl-5.37.8.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local -Dusedevel -Dversiononly=undef -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7046.tar.gz     && echo '3e8c9d9b44a7348f9acc917163dbfc15bd5ea72501492cea3a35b346440ff862 *App-cpanminus-1.7046.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7046.tar.gz && cd App-cpanminus-1.7046 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && true     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7046* /tmp/*     && cpanm --version && cpm --version
# Sat, 04 Feb 2023 16:32:38 GMT
WORKDIR /
# Sat, 04 Feb 2023 16:32:38 GMT
CMD ["perl5.37.8" "-de0"]
```

-	Layers:
	-	`sha256:7a21a86b3957d8c99250334cfb78c55af4f8c9277f2f1d4abd53d0362f96323d`  
		Last Modified: Sat, 04 Feb 2023 10:05:53 GMT  
		Size: 50.2 MB (50190828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aacc3c746ca1bd99005f184b00ee418e015c2090c72bda638766d9fb93d3f065`  
		Last Modified: Sat, 04 Feb 2023 10:59:08 GMT  
		Size: 4.9 MB (4933374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1b393b343e4fb3b92027c4741418a04d6475259ee243fbf036c1be41df98212`  
		Last Modified: Sat, 04 Feb 2023 10:59:09 GMT  
		Size: 10.2 MB (10217742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3e55fdd5f0aba51b2504973439b1c887364b84bc0d7b211da07aba072b81520`  
		Last Modified: Sat, 04 Feb 2023 10:59:32 GMT  
		Size: 50.4 MB (50356141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be64cd32ab1dd00c018103a465973562bcd243bfa513190390e3fc8043b7b9d0`  
		Last Modified: Sat, 04 Feb 2023 11:00:11 GMT  
		Size: 167.4 MB (167360700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7fceeaff241ee9d761952855ea07990fc069e6b1477ce423c1c7c4eda3cf477`  
		Last Modified: Sat, 04 Feb 2023 17:20:35 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d279ca1a096a831cd26370ae9f69c0ebf4319b71665c572834f03ae595b9cb92`  
		Last Modified: Sat, 04 Feb 2023 17:30:11 GMT  
		Size: 14.7 MB (14653697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:devel` - linux; arm64 variant v8

```console
$ docker pull perl@sha256:497d9f21100a055c9e8b5a4e323b1fdb34f2ed7ff728241d09481a00b178b4de
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **329.7 MB (329716617 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:680da896deea0713754ecdda6fdec636b81d134d6785c77484a557cd68c24d6e`
-	Default Command: `["perl5.37.8","-de0"]`

```dockerfile
# Thu, 09 Feb 2023 03:58:29 GMT
ADD file:5cf2de182dac36d99ec41918889c9755f9c49c56fa0a8d0ca14040c1d8c04541 in / 
# Thu, 09 Feb 2023 03:58:30 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:08:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 09:08:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 09 Feb 2023 09:08:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 09:09:11 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 10:22:00 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Thu, 09 Feb 2023 10:22:00 GMT
WORKDIR /usr/src/perl
# Thu, 09 Feb 2023 12:16:04 GMT
RUN true     && curl -fL https://www.cpan.org/src/5.0/perl-5.37.8.tar.xz -o perl-5.37.8.tar.xz     && echo 'eca6396a4b1aa7a38ef467ce54ed897cc84ba948fad0f90aeb210e57b04daf3c *perl-5.37.8.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.37.8.tar.xz -C /usr/src/perl     && rm perl-5.37.8.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local -Dusedevel -Dversiononly=undef -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7046.tar.gz     && echo '3e8c9d9b44a7348f9acc917163dbfc15bd5ea72501492cea3a35b346440ff862 *App-cpanminus-1.7046.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7046.tar.gz && cd App-cpanminus-1.7046 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && true     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7046* /tmp/*     && cpanm --version && cpm --version
# Thu, 09 Feb 2023 12:16:04 GMT
WORKDIR /
# Thu, 09 Feb 2023 12:16:04 GMT
CMD ["perl5.37.8" "-de0"]
```

-	Layers:
	-	`sha256:80dae1b9d879348c210c40024c6e90ef92677ac3515456375fcbb70bdf07b104`  
		Last Modified: Thu, 09 Feb 2023 04:02:11 GMT  
		Size: 53.7 MB (53703368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13ae98695cf4875b92116a031bcf51736705c39b105be5f240a143935d8370f6`  
		Last Modified: Thu, 09 Feb 2023 09:14:20 GMT  
		Size: 5.2 MB (5152064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09a74e69230a5d5ee55fb6baca6fb52404417efd177a2cb03c418d2d0cf599b5`  
		Last Modified: Thu, 09 Feb 2023 09:14:21 GMT  
		Size: 10.9 MB (10873498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e04cd4cd2ee5f2d53ea296fb22e3875a699f2ee5426c8908bfc38728acfb10a`  
		Last Modified: Thu, 09 Feb 2023 09:14:38 GMT  
		Size: 54.7 MB (54679990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9ce95a1e837843e3199407383cedc9261eeff413df03a3719b887cfcba7d2b2`  
		Last Modified: Thu, 09 Feb 2023 09:15:08 GMT  
		Size: 189.8 MB (189807741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cde7e6460fa9693256f02d8e700499bbc5e0893c33940406f6eb3395eb68f5f`  
		Last Modified: Thu, 09 Feb 2023 12:51:16 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6968b39c529fe43bbce561c814ca4cae9bcc2832de55650b7384353e662556ff`  
		Last Modified: Thu, 09 Feb 2023 12:58:01 GMT  
		Size: 15.5 MB (15499788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:devel` - linux; 386

```console
$ docker pull perl@sha256:99dd5d82792c236d904b5a402bad82de90b0b418a7c9b1d87e67c35e3015a9c4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **343.1 MB (343103417 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02c7125944bb020bb85b9c6934ea2fe2ad7e6f8480ccc078584259148cde4d3a`
-	Default Command: `["perl5.37.8","-de0"]`

```dockerfile
# Sat, 04 Feb 2023 07:49:07 GMT
ADD file:d610d24eb19fe7e275924d58b6dad6b9f3dce21359a4ef81d04298e94382f102 in / 
# Sat, 04 Feb 2023 07:49:07 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 08:19:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 08:19:42 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 04 Feb 2023 08:20:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 08:20:53 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 10:33:32 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Sat, 04 Feb 2023 10:33:33 GMT
WORKDIR /usr/src/perl
# Sat, 04 Feb 2023 13:14:42 GMT
RUN true     && curl -fL https://www.cpan.org/src/5.0/perl-5.37.8.tar.xz -o perl-5.37.8.tar.xz     && echo 'eca6396a4b1aa7a38ef467ce54ed897cc84ba948fad0f90aeb210e57b04daf3c *perl-5.37.8.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.37.8.tar.xz -C /usr/src/perl     && rm perl-5.37.8.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local -Dusedevel -Dversiononly=undef -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7046.tar.gz     && echo '3e8c9d9b44a7348f9acc917163dbfc15bd5ea72501492cea3a35b346440ff862 *App-cpanminus-1.7046.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7046.tar.gz && cd App-cpanminus-1.7046 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && true     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7046* /tmp/*     && cpanm --version && cpm --version
# Sat, 04 Feb 2023 13:14:43 GMT
WORKDIR /
# Sat, 04 Feb 2023 13:14:44 GMT
CMD ["perl5.37.8" "-de0"]
```

-	Layers:
	-	`sha256:082bfbf393a7a28cd82d531b1903cc5d788ac6af1b972045ad1d0deeff1aa6ab`  
		Last Modified: Sat, 04 Feb 2023 07:54:34 GMT  
		Size: 56.0 MB (56005478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feebdf79aa6d9b2be45c2a0949ac3677ad52629968a8cf44b6973890003395dd`  
		Last Modified: Sat, 04 Feb 2023 08:27:01 GMT  
		Size: 5.3 MB (5291983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:222ad836118a1e95a24ffd64386a98d933a2a2f96eacc3e3a3c13804a31d7008`  
		Last Modified: Sat, 04 Feb 2023 08:27:02 GMT  
		Size: 11.0 MB (11032558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4459f9c17c2fe68d4543c8bea4ebd0380fce63ced96500238f73aa94d3458202`  
		Last Modified: Sat, 04 Feb 2023 08:27:22 GMT  
		Size: 55.9 MB (55921584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50d6291b382a9d327a45b720e533c2a1d181957a26b6295caab87463543c9555`  
		Last Modified: Sat, 04 Feb 2023 08:28:00 GMT  
		Size: 199.8 MB (199796392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a76a4b4342b818cdc10bb689e7b40bf42f6ab85182826f866932c0ff0e206980`  
		Last Modified: Sat, 04 Feb 2023 14:05:05 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d08ec5a33ef3e4bf0354933f251cc62334b6dd3e5804892d50ea5f89f0ad4b5`  
		Last Modified: Sat, 04 Feb 2023 14:13:32 GMT  
		Size: 15.1 MB (15055287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:devel` - linux; mips64le

```console
$ docker pull perl@sha256:3b7e4c39ba28860898c1f6d3c4b26b0e3179048a1bbbda93a652fec6e26e26cf
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **316.1 MB (316108907 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:baae684d6d4059f2cbd3404b2e3cecfb8e642878d0834513750055ad9491a981`
-	Default Command: `["perl5.37.8","-de0"]`

```dockerfile
# Sat, 04 Feb 2023 06:19:34 GMT
ADD file:6ce59568f971e1c72981ffb01f3c6b67b20b5b055edec122273990ec1c36f042 in / 
# Sat, 04 Feb 2023 06:19:40 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 18:38:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 18:38:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 04 Feb 2023 18:40:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 18:46:03 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 20:03:25 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Sat, 04 Feb 2023 20:03:31 GMT
WORKDIR /usr/src/perl
# Sun, 05 Feb 2023 01:06:54 GMT
RUN true     && curl -fL https://www.cpan.org/src/5.0/perl-5.37.8.tar.xz -o perl-5.37.8.tar.xz     && echo 'eca6396a4b1aa7a38ef467ce54ed897cc84ba948fad0f90aeb210e57b04daf3c *perl-5.37.8.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.37.8.tar.xz -C /usr/src/perl     && rm perl-5.37.8.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local -Dusedevel -Dversiononly=undef -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7046.tar.gz     && echo '3e8c9d9b44a7348f9acc917163dbfc15bd5ea72501492cea3a35b346440ff862 *App-cpanminus-1.7046.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7046.tar.gz && cd App-cpanminus-1.7046 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && true     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7046* /tmp/*     && cpanm --version && cpm --version
# Sun, 05 Feb 2023 01:07:01 GMT
WORKDIR /
# Sun, 05 Feb 2023 01:07:07 GMT
CMD ["perl5.37.8" "-de0"]
```

-	Layers:
	-	`sha256:c1dc6b83fd5771c0e7c97ea21324a2c2a31849a9f2b37f7f4cf80645847ed538`  
		Last Modified: Sat, 04 Feb 2023 06:27:44 GMT  
		Size: 53.2 MB (53245135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f624d6f693356db43029a8b8962db53b8c3d6cbc3b5f85384e4fd4da7659697d`  
		Last Modified: Sat, 04 Feb 2023 18:58:52 GMT  
		Size: 5.1 MB (5125958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dd777b6a18c499deb0f24173e9393e1e84727364945534cfc2747aaa2dfb6f4`  
		Last Modified: Sat, 04 Feb 2023 18:58:54 GMT  
		Size: 10.7 MB (10662061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b908c1d639ab484cee804b8cf3515bf00fadb5effb63d57cfa59ede5a21bc22e`  
		Last Modified: Sat, 04 Feb 2023 18:59:41 GMT  
		Size: 53.3 MB (53307674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0f12ade5ebc92a87ba081f5dd680455496b9fe505d99b68336dd8c7e7c07cf7`  
		Last Modified: Sat, 04 Feb 2023 19:01:46 GMT  
		Size: 179.0 MB (178996312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2124d80553fd5b64695532dd895a7399dbac294b71ce1849f1df49abf32aa31f`  
		Last Modified: Sun, 05 Feb 2023 02:21:27 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c99766ca0fd26ea4181f407812ca57a9119ec2abd1ff2d1a011561970c3513ab`  
		Last Modified: Sun, 05 Feb 2023 02:28:27 GMT  
		Size: 14.8 MB (14771631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:devel` - linux; ppc64le

```console
$ docker pull perl@sha256:07cf61febb02751b279845cb2c409c414269e359e860917511038baab518b66d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **346.6 MB (346593283 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f6687bfba49de8a5678a80de8ce7a0641ce772a049b4d4c472fae2511cabedd`
-	Default Command: `["perl5.37.8","-de0"]`

```dockerfile
# Sat, 04 Feb 2023 12:25:27 GMT
ADD file:724a2ac3b6190353442c93dce0ad4b3ab5c60144fc8204131767af6760e11980 in / 
# Sat, 04 Feb 2023 12:25:30 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 18:02:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 18:02:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 04 Feb 2023 18:03:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 18:05:31 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 05 Feb 2023 05:58:22 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Sun, 05 Feb 2023 05:58:23 GMT
WORKDIR /usr/src/perl
# Sun, 05 Feb 2023 06:59:42 GMT
RUN true     && curl -fL https://www.cpan.org/src/5.0/perl-5.37.8.tar.xz -o perl-5.37.8.tar.xz     && echo 'eca6396a4b1aa7a38ef467ce54ed897cc84ba948fad0f90aeb210e57b04daf3c *perl-5.37.8.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.37.8.tar.xz -C /usr/src/perl     && rm perl-5.37.8.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local -Dusedevel -Dversiononly=undef -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7046.tar.gz     && echo '3e8c9d9b44a7348f9acc917163dbfc15bd5ea72501492cea3a35b346440ff862 *App-cpanminus-1.7046.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7046.tar.gz && cd App-cpanminus-1.7046 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && true     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7046* /tmp/*     && cpanm --version && cpm --version
# Sun, 05 Feb 2023 06:59:44 GMT
WORKDIR /
# Sun, 05 Feb 2023 06:59:44 GMT
CMD ["perl5.37.8" "-de0"]
```

-	Layers:
	-	`sha256:c14c296a64e0f557b40f88759a913c28d0b28c646e5ec0cf0ceb49457156a792`  
		Last Modified: Sat, 04 Feb 2023 12:31:37 GMT  
		Size: 58.9 MB (58897064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e01c913909aa7f93cc6ab033f1f6e61f49370709ea387f35a2022e742cd5d42b`  
		Last Modified: Sat, 04 Feb 2023 18:14:41 GMT  
		Size: 5.4 MB (5414184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edacbd3dc421aaeb6108d87b4dc4870994392f896c53946184172b80601b6659`  
		Last Modified: Sat, 04 Feb 2023 18:14:42 GMT  
		Size: 11.6 MB (11629731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1badae69b651e1239c1b3e0309989a6660df959409d4597bba0d594f9423abab`  
		Last Modified: Sat, 04 Feb 2023 18:15:14 GMT  
		Size: 58.9 MB (58862783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f991c2e009547b6a192e5ccb54de2e8bd2006a02250ef972285ac55591457b2`  
		Last Modified: Sat, 04 Feb 2023 18:16:18 GMT  
		Size: 196.2 MB (196229844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5355488edeaacfe14ed114911adb38d00e608d0052c59483f14e48efb254a5b7`  
		Last Modified: Sun, 05 Feb 2023 07:12:16 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e22f74b3106fcedce2453b4bccbe0b2786901b7520f53bfe069f21673fd6936c`  
		Last Modified: Sun, 05 Feb 2023 07:15:44 GMT  
		Size: 15.6 MB (15559510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `perl:devel` - linux; s390x

```console
$ docker pull perl@sha256:c308e63be20b0a41f94ec4bd22086b02fce293abccea2616f4844947ab07595a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **312.1 MB (312056630 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4cf7b73018f680292466c6cc99801bc2c87b3b9f6bf2602c3068af35f4d93878`
-	Default Command: `["perl5.37.8","-de0"]`

```dockerfile
# Thu, 09 Feb 2023 02:41:26 GMT
ADD file:952595f2a554945ef740fa7b1fbc617a9ce3e1c3b90ddf1e7c0ac6018e6a98f9 in / 
# Thu, 09 Feb 2023 02:41:30 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 07:27:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 07:27:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 09 Feb 2023 07:28:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 07:31:46 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 07:55:22 GMT
LABEL maintainer=Peter Martini <PeterCMartini@GMail.com>, Zak B. Elep <zakame@cpan.org>
# Thu, 09 Feb 2023 07:55:23 GMT
WORKDIR /usr/src/perl
# Thu, 09 Feb 2023 09:44:35 GMT
RUN true     && curl -fL https://www.cpan.org/src/5.0/perl-5.37.8.tar.xz -o perl-5.37.8.tar.xz     && echo 'eca6396a4b1aa7a38ef467ce54ed897cc84ba948fad0f90aeb210e57b04daf3c *perl-5.37.8.tar.xz' | sha256sum --strict --check -     && tar --strip-components=1 -xaf perl-5.37.8.tar.xz -C /usr/src/perl     && rm perl-5.37.8.tar.xz     && cat *.patch | patch -p1     && gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"     && archBits="$(dpkg-architecture --query DEB_BUILD_ARCH_BITS)"     && archFlag="$([ "$archBits" = '64' ] && echo '-Duse64bitall' || echo '-Duse64bitint')"     && ./Configure -Darchname="$gnuArch" "$archFlag" -Duseshrplib -Dvendorprefix=/usr/local -Dusedevel -Dversiononly=undef -des     && make -j$(nproc)     && TEST_JOBS=$(nproc) make test_harness     && make install     && cd /usr/src     && curl -fLO https://www.cpan.org/authors/id/M/MI/MIYAGAWA/App-cpanminus-1.7046.tar.gz     && echo '3e8c9d9b44a7348f9acc917163dbfc15bd5ea72501492cea3a35b346440ff862 *App-cpanminus-1.7046.tar.gz' | sha256sum --strict --check -     && tar -xzf App-cpanminus-1.7046.tar.gz && cd App-cpanminus-1.7046 && perl bin/cpanm . && cd /root     && cpanm IO::Socket::SSL     && curl -fL https://raw.githubusercontent.com/skaji/cpm/0.997011/cpm -o /usr/local/bin/cpm     && echo '7dee2176a450a8be3a6b9b91dac603a0c3a7e807042626d3fe6c93d843f75610 */usr/local/bin/cpm' | sha256sum --strict --check -     && chmod +x /usr/local/bin/cpm     && true     && rm -fr /root/.cpanm /usr/src/perl /usr/src/App-cpanminus-1.7046* /tmp/*     && cpanm --version && cpm --version
# Thu, 09 Feb 2023 09:44:39 GMT
WORKDIR /
# Thu, 09 Feb 2023 09:44:40 GMT
CMD ["perl5.37.8" "-de0"]
```

-	Layers:
	-	`sha256:83809ebda0c421fc95029bc6775e0a0c1eba6916a58b115dcb6a14885dae2028`  
		Last Modified: Thu, 09 Feb 2023 02:45:46 GMT  
		Size: 53.3 MB (53278896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b6c93cabdf59ed2ae0e16b55f3f3c261e3d470a151aafaebfb14841492c699e`  
		Last Modified: Thu, 09 Feb 2023 07:40:29 GMT  
		Size: 5.1 MB (5148933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c89bee0eba54958a826e0c254b818763de9882b96810e4be6ef4f388284b68db`  
		Last Modified: Thu, 09 Feb 2023 07:40:30 GMT  
		Size: 10.8 MB (10766263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd1905c0799757faa648df321bb0d6546b0674bafa27f5efd6aaf1e12f6802f2`  
		Last Modified: Thu, 09 Feb 2023 07:40:46 GMT  
		Size: 54.1 MB (54052598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddba8954d1958adea75458548afe196915ab7c43c468daff07fbafa4109e0888`  
		Last Modified: Thu, 09 Feb 2023 07:41:14 GMT  
		Size: 172.9 MB (172898861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9185b50fb63c7791265f3cd5183b92b367c50675a83e80b98d0d2fbd0ef24980`  
		Last Modified: Thu, 09 Feb 2023 10:15:07 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:499a937d7c5956501bd3f0495a6c8e63b8a57cabecc226ee246ec30101ec0844`  
		Last Modified: Thu, 09 Feb 2023 10:19:30 GMT  
		Size: 15.9 MB (15910911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
