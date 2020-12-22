## `elixir:latest`

```console
$ docker pull elixir@sha256:11e027a41622a53b4a3311ae932a85da66d87118945311235976312211e1bfe1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `elixir:latest` - linux; amd64

```console
$ docker pull elixir@sha256:b2c15d27457a960a0f5ee98d4d08ddc9080d98017bd720d02732ae44cfd1f6ae
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **482.9 MB (482880564 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df50e76fe4e6ea5fbe06e6a1e6885d3cb1804ebcde1835d588e32ea759112a4a`
-	Default Command: `["iex"]`

```dockerfile
# Fri, 11 Dec 2020 02:05:52 GMT
ADD file:6014cd9d7466825f80d4a3345847efd6fd7ef600b8135811cab4f0e304f66cd7 in / 
# Fri, 11 Dec 2020 02:05:52 GMT
CMD ["bash"]
# Thu, 17 Dec 2020 16:58:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Dec 2020 16:58:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 17 Dec 2020 16:58:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 17 Dec 2020 16:59:36 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 21 Dec 2020 19:26:54 GMT
ENV OTP_VERSION=23.2.1 REBAR3_VERSION=3.14.3
# Mon, 21 Dec 2020 19:26:55 GMT
LABEL org.opencontainers.image.version=23.2.1
# Mon, 21 Dec 2020 19:40:17 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="e7034e2cfe50d7570ac8f70ea7ba69ea013f10863043e25132f0a5d3d0d8d3a7" 	&& runtimeDeps='libodbc1 			libsctp1 			libwxgtk3.0' 	&& buildDeps='unixodbc-dev 			libsctp-dev 			libwxgtk3.0-dev' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make -j$(nproc) docs DOC_TARGETS=chunks 	  && make install install-docs DOC_TARGETS=chunks ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Mon, 21 Dec 2020 19:40:17 GMT
CMD ["erl"]
# Mon, 21 Dec 2020 19:40:18 GMT
ENV REBAR_VERSION=2.6.4
# Mon, 21 Dec 2020 19:40:23 GMT
RUN set -xe 	&& REBAR_DOWNLOAD_URL="https://github.com/rebar/rebar/archive/${REBAR_VERSION}.tar.gz" 	&& REBAR_DOWNLOAD_SHA256="577246bafa2eb2b2c3f1d0c157408650446884555bf87901508ce71d5cc0bd07" 	&& mkdir -p /usr/src/rebar-src 	&& curl -fSL -o rebar-src.tar.gz "$REBAR_DOWNLOAD_URL" 	&& echo "$REBAR_DOWNLOAD_SHA256 rebar-src.tar.gz" | sha256sum -c - 	&& tar -xzf rebar-src.tar.gz -C /usr/src/rebar-src --strip-components=1 	&& rm rebar-src.tar.gz 	&& cd /usr/src/rebar-src 	&& ./bootstrap 	&& install -v ./rebar /usr/local/bin/ 	&& rm -rf /usr/src/rebar-src
# Mon, 21 Dec 2020 19:41:00 GMT
RUN set -xe 	&& REBAR3_DOWNLOAD_URL="https://github.com/erlang/rebar3/archive/${REBAR3_VERSION}.tar.gz" 	&& REBAR3_DOWNLOAD_SHA256="69024b30f17b52c61e5e0568cbf9a2db325eb646ae230c48858401507394f5c0" 	&& mkdir -p /usr/src/rebar3-src 	&& curl -fSL -o rebar3-src.tar.gz "$REBAR3_DOWNLOAD_URL" 	&& echo "$REBAR3_DOWNLOAD_SHA256 rebar3-src.tar.gz" | sha256sum -c - 	&& tar -xzf rebar3-src.tar.gz -C /usr/src/rebar3-src --strip-components=1 	&& rm rebar3-src.tar.gz 	&& cd /usr/src/rebar3-src 	&& HOME=$PWD ./bootstrap 	&& install -v ./rebar3 /usr/local/bin/ 	&& rm -rf /usr/src/rebar3-src
# Mon, 21 Dec 2020 21:52:04 GMT
ENV ELIXIR_VERSION=v1.11.2 LANG=C.UTF-8
# Mon, 21 Dec 2020 21:54:49 GMT
RUN set -xe 	&& ELIXIR_DOWNLOAD_URL="https://github.com/elixir-lang/elixir/archive/${ELIXIR_VERSION}.tar.gz" 	&& ELIXIR_DOWNLOAD_SHA256="318f0a6cb372186b0cf45d2e9c9889b4c9e941643fd67ca0ab1ec32710ab6bf5" 	&& curl -fSL -o elixir-src.tar.gz $ELIXIR_DOWNLOAD_URL 	&& echo "$ELIXIR_DOWNLOAD_SHA256  elixir-src.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/local/src/elixir 	&& tar -xzC /usr/local/src/elixir --strip-components=1 -f elixir-src.tar.gz 	&& rm elixir-src.tar.gz 	&& cd /usr/local/src/elixir 	&& make install clean
# Mon, 21 Dec 2020 21:54:49 GMT
CMD ["iex"]
```

-	Layers:
	-	`sha256:6c33745f49b41daad28b7b192c447938452ea4de9fe8c7cc3edf1433b1366946`  
		Last Modified: Fri, 11 Dec 2020 02:12:07 GMT  
		Size: 50.4 MB (50397728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef072fc32a84ef237dd4fcc7dff2c5e2a77565f24d63977d0fa654a6d8512dd8`  
		Last Modified: Thu, 17 Dec 2020 17:25:57 GMT  
		Size: 7.8 MB (7812075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0afb8e68e0bcdc1b6e05acaa713a6fe0d818086c596bd1ad99133665c4efe63`  
		Last Modified: Thu, 17 Dec 2020 17:25:58 GMT  
		Size: 10.0 MB (9996417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d599c07d28e6c920ef615f4f9b5cd0d52eb106fcd20c3a7daef389f14edd4ef5`  
		Last Modified: Thu, 17 Dec 2020 17:26:19 GMT  
		Size: 51.8 MB (51829485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2ecc74db11a2e0bc5a12395b008dc12bdbaaeeb45da34f4fa7e75b3c17ed564`  
		Last Modified: Thu, 17 Dec 2020 17:27:03 GMT  
		Size: 192.3 MB (192313866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f3d344b4bee8383280a4a91a90e577377f6992d39262c45a4162daab5698158`  
		Last Modified: Mon, 21 Dec 2020 20:12:25 GMT  
		Size: 162.4 MB (162432590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df0a42bd5765dcefb3ee64a56aeff1a78134bda3e2eb62dff2f790cfc568b1d0`  
		Last Modified: Mon, 21 Dec 2020 20:11:49 GMT  
		Size: 196.2 KB (196199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9caa3d1aa92fa1acb418510c392c2c3786a76696c8b24d3dfe24ef1721bc50ac`  
		Last Modified: Mon, 21 Dec 2020 20:11:49 GMT  
		Size: 913.0 KB (912997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dca3e70b3e07e7e20f5db27ef069acdf054e3f4f1c211771df98a2db9cede76`  
		Last Modified: Mon, 21 Dec 2020 22:01:30 GMT  
		Size: 7.0 MB (6989207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `elixir:latest` - linux; arm variant v7

```console
$ docker pull elixir@sha256:1c2fe10ebac89ddaa6ddfdd0ba0421086e58be24e05b3b5650199aa0a2ee9413
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **435.8 MB (435839218 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94ce6f867e2bb3f1b230fc81bb785196b1de81e75b523cf6fc6ce9f379d57ce3`
-	Default Command: `["iex"]`

```dockerfile
# Fri, 11 Dec 2020 02:23:08 GMT
ADD file:af46f686172bae3034ad0b34cc26081a2f8db0f5d4704ef63abb7eeaf06c75e0 in / 
# Fri, 11 Dec 2020 02:23:11 GMT
CMD ["bash"]
# Thu, 17 Dec 2020 08:16:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Dec 2020 08:16:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 17 Dec 2020 08:17:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 17 Dec 2020 08:19:31 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 21 Dec 2020 20:03:10 GMT
ENV OTP_VERSION=23.2.1 REBAR3_VERSION=3.14.3
# Mon, 21 Dec 2020 20:03:11 GMT
LABEL org.opencontainers.image.version=23.2.1
# Mon, 21 Dec 2020 20:14:34 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="e7034e2cfe50d7570ac8f70ea7ba69ea013f10863043e25132f0a5d3d0d8d3a7" 	&& runtimeDeps='libodbc1 			libsctp1 			libwxgtk3.0' 	&& buildDeps='unixodbc-dev 			libsctp-dev 			libwxgtk3.0-dev' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make -j$(nproc) docs DOC_TARGETS=chunks 	  && make install install-docs DOC_TARGETS=chunks ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Mon, 21 Dec 2020 20:14:43 GMT
CMD ["erl"]
# Mon, 21 Dec 2020 20:14:45 GMT
ENV REBAR_VERSION=2.6.4
# Mon, 21 Dec 2020 20:15:01 GMT
RUN set -xe 	&& REBAR_DOWNLOAD_URL="https://github.com/rebar/rebar/archive/${REBAR_VERSION}.tar.gz" 	&& REBAR_DOWNLOAD_SHA256="577246bafa2eb2b2c3f1d0c157408650446884555bf87901508ce71d5cc0bd07" 	&& mkdir -p /usr/src/rebar-src 	&& curl -fSL -o rebar-src.tar.gz "$REBAR_DOWNLOAD_URL" 	&& echo "$REBAR_DOWNLOAD_SHA256 rebar-src.tar.gz" | sha256sum -c - 	&& tar -xzf rebar-src.tar.gz -C /usr/src/rebar-src --strip-components=1 	&& rm rebar-src.tar.gz 	&& cd /usr/src/rebar-src 	&& ./bootstrap 	&& install -v ./rebar /usr/local/bin/ 	&& rm -rf /usr/src/rebar-src
# Mon, 21 Dec 2020 20:16:17 GMT
RUN set -xe 	&& REBAR3_DOWNLOAD_URL="https://github.com/erlang/rebar3/archive/${REBAR3_VERSION}.tar.gz" 	&& REBAR3_DOWNLOAD_SHA256="69024b30f17b52c61e5e0568cbf9a2db325eb646ae230c48858401507394f5c0" 	&& mkdir -p /usr/src/rebar3-src 	&& curl -fSL -o rebar3-src.tar.gz "$REBAR3_DOWNLOAD_URL" 	&& echo "$REBAR3_DOWNLOAD_SHA256 rebar3-src.tar.gz" | sha256sum -c - 	&& tar -xzf rebar3-src.tar.gz -C /usr/src/rebar3-src --strip-components=1 	&& rm rebar3-src.tar.gz 	&& cd /usr/src/rebar3-src 	&& HOME=$PWD ./bootstrap 	&& install -v ./rebar3 /usr/local/bin/ 	&& rm -rf /usr/src/rebar3-src
# Mon, 21 Dec 2020 22:01:03 GMT
ENV ELIXIR_VERSION=v1.11.2 LANG=C.UTF-8
# Mon, 21 Dec 2020 22:03:19 GMT
RUN set -xe 	&& ELIXIR_DOWNLOAD_URL="https://github.com/elixir-lang/elixir/archive/${ELIXIR_VERSION}.tar.gz" 	&& ELIXIR_DOWNLOAD_SHA256="318f0a6cb372186b0cf45d2e9c9889b4c9e941643fd67ca0ab1ec32710ab6bf5" 	&& curl -fSL -o elixir-src.tar.gz $ELIXIR_DOWNLOAD_URL 	&& echo "$ELIXIR_DOWNLOAD_SHA256  elixir-src.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/local/src/elixir 	&& tar -xzC /usr/local/src/elixir --strip-components=1 -f elixir-src.tar.gz 	&& rm elixir-src.tar.gz 	&& cd /usr/local/src/elixir 	&& make install clean
# Mon, 21 Dec 2020 22:03:20 GMT
CMD ["iex"]
```

-	Layers:
	-	`sha256:709549ab8c597dac59777a5a3666600f3dd986b5f05389aa7b15bd5f9281f809`  
		Last Modified: Fri, 11 Dec 2020 02:32:43 GMT  
		Size: 45.9 MB (45867902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a47835026e1df0ff27d1071162b8ee6183c6c06f3880f788d360330f95d426f3`  
		Last Modified: Thu, 17 Dec 2020 08:52:24 GMT  
		Size: 7.1 MB (7099204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9aa96a1a673a07b6f8f0936ce1fb5521c14b566ea503a69342bd56e5e115e20`  
		Last Modified: Thu, 17 Dec 2020 08:52:24 GMT  
		Size: 9.3 MB (9343453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4e19bdda1d2f3319ac9fbe5b8b2a9a62eba6a49e13e6846089d4d85f3b6d256`  
		Last Modified: Thu, 17 Dec 2020 08:52:49 GMT  
		Size: 47.4 MB (47355631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b538cd0b24d58c972e8326bf18ffc11d26c5cda4f4d245b4d6074dd970e4f4e`  
		Last Modified: Thu, 17 Dec 2020 08:53:43 GMT  
		Size: 168.5 MB (168532869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d491714b04a394903448b221a4019ffb93dc77a82edef4406fa6de191e5bb7e8`  
		Last Modified: Mon, 21 Dec 2020 20:34:13 GMT  
		Size: 149.5 MB (149541808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22d5aa1035aa0597c89b56fe45aae3b20b27eee3dd36d577d9c43263d1cb2e81`  
		Last Modified: Mon, 21 Dec 2020 20:33:33 GMT  
		Size: 196.1 KB (196133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c96958a283e87d58f7f2e6bfef8ea03b5dd8fa98aa9e628514d0d07da79141a0`  
		Last Modified: Mon, 21 Dec 2020 20:33:35 GMT  
		Size: 913.0 KB (912998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f703eb8bd60ab01da657b0e57106924e503a6ec6baf1a02e718b915bb522ea9d`  
		Last Modified: Mon, 21 Dec 2020 22:10:58 GMT  
		Size: 7.0 MB (6989220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `elixir:latest` - linux; arm64 variant v8

```console
$ docker pull elixir@sha256:1a563e6610207ea7ca179049c40ff208364b508a70f488f83e2bd7c6d7d55a99
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **466.0 MB (466045848 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a83ea0f0205009bc2ab66729f1d8472d7ce4ceda76aa442c1141b24232372a7f`
-	Default Command: `["iex"]`

```dockerfile
# Fri, 11 Dec 2020 02:45:23 GMT
ADD file:b08f373022952dba7d08b7fc02909d9e369c9727e0e4f62d6110e41e70e668cc in / 
# Fri, 11 Dec 2020 02:45:25 GMT
CMD ["bash"]
# Thu, 17 Dec 2020 10:05:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Dec 2020 10:06:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 17 Dec 2020 10:06:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 17 Dec 2020 10:08:43 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 21 Dec 2020 19:44:11 GMT
ENV OTP_VERSION=23.2.1 REBAR3_VERSION=3.14.3
# Mon, 21 Dec 2020 19:44:12 GMT
LABEL org.opencontainers.image.version=23.2.1
# Mon, 21 Dec 2020 19:54:03 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="e7034e2cfe50d7570ac8f70ea7ba69ea013f10863043e25132f0a5d3d0d8d3a7" 	&& runtimeDeps='libodbc1 			libsctp1 			libwxgtk3.0' 	&& buildDeps='unixodbc-dev 			libsctp-dev 			libwxgtk3.0-dev' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make -j$(nproc) docs DOC_TARGETS=chunks 	  && make install install-docs DOC_TARGETS=chunks ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Mon, 21 Dec 2020 19:54:20 GMT
CMD ["erl"]
# Mon, 21 Dec 2020 19:54:22 GMT
ENV REBAR_VERSION=2.6.4
# Mon, 21 Dec 2020 19:54:35 GMT
RUN set -xe 	&& REBAR_DOWNLOAD_URL="https://github.com/rebar/rebar/archive/${REBAR_VERSION}.tar.gz" 	&& REBAR_DOWNLOAD_SHA256="577246bafa2eb2b2c3f1d0c157408650446884555bf87901508ce71d5cc0bd07" 	&& mkdir -p /usr/src/rebar-src 	&& curl -fSL -o rebar-src.tar.gz "$REBAR_DOWNLOAD_URL" 	&& echo "$REBAR_DOWNLOAD_SHA256 rebar-src.tar.gz" | sha256sum -c - 	&& tar -xzf rebar-src.tar.gz -C /usr/src/rebar-src --strip-components=1 	&& rm rebar-src.tar.gz 	&& cd /usr/src/rebar-src 	&& ./bootstrap 	&& install -v ./rebar /usr/local/bin/ 	&& rm -rf /usr/src/rebar-src
# Mon, 21 Dec 2020 19:55:33 GMT
RUN set -xe 	&& REBAR3_DOWNLOAD_URL="https://github.com/erlang/rebar3/archive/${REBAR3_VERSION}.tar.gz" 	&& REBAR3_DOWNLOAD_SHA256="69024b30f17b52c61e5e0568cbf9a2db325eb646ae230c48858401507394f5c0" 	&& mkdir -p /usr/src/rebar3-src 	&& curl -fSL -o rebar3-src.tar.gz "$REBAR3_DOWNLOAD_URL" 	&& echo "$REBAR3_DOWNLOAD_SHA256 rebar3-src.tar.gz" | sha256sum -c - 	&& tar -xzf rebar3-src.tar.gz -C /usr/src/rebar3-src --strip-components=1 	&& rm rebar3-src.tar.gz 	&& cd /usr/src/rebar3-src 	&& HOME=$PWD ./bootstrap 	&& install -v ./rebar3 /usr/local/bin/ 	&& rm -rf /usr/src/rebar3-src
# Mon, 21 Dec 2020 21:33:11 GMT
ENV ELIXIR_VERSION=v1.11.2 LANG=C.UTF-8
# Mon, 21 Dec 2020 21:35:33 GMT
RUN set -xe 	&& ELIXIR_DOWNLOAD_URL="https://github.com/elixir-lang/elixir/archive/${ELIXIR_VERSION}.tar.gz" 	&& ELIXIR_DOWNLOAD_SHA256="318f0a6cb372186b0cf45d2e9c9889b4c9e941643fd67ca0ab1ec32710ab6bf5" 	&& curl -fSL -o elixir-src.tar.gz $ELIXIR_DOWNLOAD_URL 	&& echo "$ELIXIR_DOWNLOAD_SHA256  elixir-src.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/local/src/elixir 	&& tar -xzC /usr/local/src/elixir --strip-components=1 -f elixir-src.tar.gz 	&& rm elixir-src.tar.gz 	&& cd /usr/local/src/elixir 	&& make install clean
# Mon, 21 Dec 2020 21:35:34 GMT
CMD ["iex"]
```

-	Layers:
	-	`sha256:99e5136f81cd2a8cc226c42435d6f4f30584d168cc51f4d4afd2d5611e4d2215`  
		Last Modified: Fri, 11 Dec 2020 02:52:45 GMT  
		Size: 49.2 MB (49180317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4e84abcfad00e501f51bf9945429b6856c10fe31c1504e62c6520d85fff4382`  
		Last Modified: Thu, 17 Dec 2020 10:38:12 GMT  
		Size: 7.7 MB (7682276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97012cb1831f37b45ec32c7b23a4a1bbd2d92d45324067362d15f9c5ed5341b0`  
		Last Modified: Thu, 17 Dec 2020 10:38:13 GMT  
		Size: 10.0 MB (9984302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73ab763a154e0e4765c5e67269e4bb776478e2abfb52f24bae39ee817ad26bbc`  
		Last Modified: Thu, 17 Dec 2020 10:38:37 GMT  
		Size: 52.2 MB (52163991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba4c844d929512ea63e83612467e4f9da03ceeb6b1a5dafce1b077658dfe70f9`  
		Last Modified: Thu, 17 Dec 2020 10:39:25 GMT  
		Size: 183.9 MB (183870807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e08bc23d5c0df3ab26ad9098fdd992ad525e4e7d5f982fca4f51a9010cb61bc8`  
		Last Modified: Mon, 21 Dec 2020 20:12:06 GMT  
		Size: 155.1 MB (155065687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20ae3bdc5e06d55f326283a14418a33f4d1fc2118c5327df0ee4e23b8dea097a`  
		Last Modified: Mon, 21 Dec 2020 20:11:32 GMT  
		Size: 196.2 KB (196190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afcb41221ab3ee9dd1da62053ee87af01bbe4ef2c9566d26684fd528bdcb1b44`  
		Last Modified: Mon, 21 Dec 2020 20:11:33 GMT  
		Size: 913.0 KB (912995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b20f4affa9c171ca58faad348526a38c33dcc88110b6c709f4c94072fdd9bb2`  
		Last Modified: Mon, 21 Dec 2020 21:43:38 GMT  
		Size: 7.0 MB (6989283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `elixir:latest` - linux; 386

```console
$ docker pull elixir@sha256:a6ecb96064abefdcd8c5b1378c30dd7b8ddb1133a2b649295eda5c434a507e24
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **493.2 MB (493209546 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba9f6bef7c03bb61f0df96065db20f2f004fe69d14b088cef214655e1c63545b`
-	Default Command: `["iex"]`

```dockerfile
# Fri, 11 Dec 2020 02:02:51 GMT
ADD file:5131dbfe4d05a72c50b47e4ee936290486446a3a4dfe832240dd270b0f563542 in / 
# Fri, 11 Dec 2020 02:02:51 GMT
CMD ["bash"]
# Thu, 17 Dec 2020 08:08:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Dec 2020 08:08:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 17 Dec 2020 08:09:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 17 Dec 2020 08:10:11 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 21 Dec 2020 19:41:42 GMT
ENV OTP_VERSION=23.2.1 REBAR3_VERSION=3.14.3
# Mon, 21 Dec 2020 19:41:42 GMT
LABEL org.opencontainers.image.version=23.2.1
# Mon, 21 Dec 2020 20:06:39 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="e7034e2cfe50d7570ac8f70ea7ba69ea013f10863043e25132f0a5d3d0d8d3a7" 	&& runtimeDeps='libodbc1 			libsctp1 			libwxgtk3.0' 	&& buildDeps='unixodbc-dev 			libsctp-dev 			libwxgtk3.0-dev' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make -j$(nproc) docs DOC_TARGETS=chunks 	  && make install install-docs DOC_TARGETS=chunks ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Mon, 21 Dec 2020 20:06:40 GMT
CMD ["erl"]
# Mon, 21 Dec 2020 20:06:40 GMT
ENV REBAR_VERSION=2.6.4
# Mon, 21 Dec 2020 20:06:48 GMT
RUN set -xe 	&& REBAR_DOWNLOAD_URL="https://github.com/rebar/rebar/archive/${REBAR_VERSION}.tar.gz" 	&& REBAR_DOWNLOAD_SHA256="577246bafa2eb2b2c3f1d0c157408650446884555bf87901508ce71d5cc0bd07" 	&& mkdir -p /usr/src/rebar-src 	&& curl -fSL -o rebar-src.tar.gz "$REBAR_DOWNLOAD_URL" 	&& echo "$REBAR_DOWNLOAD_SHA256 rebar-src.tar.gz" | sha256sum -c - 	&& tar -xzf rebar-src.tar.gz -C /usr/src/rebar-src --strip-components=1 	&& rm rebar-src.tar.gz 	&& cd /usr/src/rebar-src 	&& ./bootstrap 	&& install -v ./rebar /usr/local/bin/ 	&& rm -rf /usr/src/rebar-src
# Mon, 21 Dec 2020 20:07:57 GMT
RUN set -xe 	&& REBAR3_DOWNLOAD_URL="https://github.com/erlang/rebar3/archive/${REBAR3_VERSION}.tar.gz" 	&& REBAR3_DOWNLOAD_SHA256="69024b30f17b52c61e5e0568cbf9a2db325eb646ae230c48858401507394f5c0" 	&& mkdir -p /usr/src/rebar3-src 	&& curl -fSL -o rebar3-src.tar.gz "$REBAR3_DOWNLOAD_URL" 	&& echo "$REBAR3_DOWNLOAD_SHA256 rebar3-src.tar.gz" | sha256sum -c - 	&& tar -xzf rebar3-src.tar.gz -C /usr/src/rebar3-src --strip-components=1 	&& rm rebar3-src.tar.gz 	&& cd /usr/src/rebar3-src 	&& HOME=$PWD ./bootstrap 	&& install -v ./rebar3 /usr/local/bin/ 	&& rm -rf /usr/src/rebar3-src
# Mon, 21 Dec 2020 22:05:41 GMT
ENV ELIXIR_VERSION=v1.11.2 LANG=C.UTF-8
# Mon, 21 Dec 2020 22:07:25 GMT
RUN set -xe 	&& ELIXIR_DOWNLOAD_URL="https://github.com/elixir-lang/elixir/archive/${ELIXIR_VERSION}.tar.gz" 	&& ELIXIR_DOWNLOAD_SHA256="318f0a6cb372186b0cf45d2e9c9889b4c9e941643fd67ca0ab1ec32710ab6bf5" 	&& curl -fSL -o elixir-src.tar.gz $ELIXIR_DOWNLOAD_URL 	&& echo "$ELIXIR_DOWNLOAD_SHA256  elixir-src.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/local/src/elixir 	&& tar -xzC /usr/local/src/elixir --strip-components=1 -f elixir-src.tar.gz 	&& rm elixir-src.tar.gz 	&& cd /usr/local/src/elixir 	&& make install clean
# Mon, 21 Dec 2020 22:07:25 GMT
CMD ["iex"]
```

-	Layers:
	-	`sha256:d18c9b676b719f51a76e9b6c9cb0781fbe5c36a18cfdcdac473acae10efbb381`  
		Last Modified: Fri, 11 Dec 2020 02:09:16 GMT  
		Size: 51.2 MB (51161209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26e3f23b521993114178224792894936dcc9b567479d0bef8aa0bf09e9184c61`  
		Last Modified: Thu, 17 Dec 2020 08:25:20 GMT  
		Size: 8.0 MB (7981625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2456a28509ee0f769d893cdf865d90b4bb8a88cd03b1a6441eba06d17550ff90`  
		Last Modified: Thu, 17 Dec 2020 08:25:20 GMT  
		Size: 10.3 MB (10338754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac4bf8443dc6c99054bcbb85570912de1784604fbf0fc8945cf010b089c05e8e`  
		Last Modified: Thu, 17 Dec 2020 08:25:45 GMT  
		Size: 53.4 MB (53432943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b2b67fa3f68359249180b1933ee6b609f92ca72c2df2edb0f85e744842edf28`  
		Last Modified: Thu, 17 Dec 2020 08:26:42 GMT  
		Size: 198.9 MB (198860928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2081f6a999ab9c745fddc6abe3fae43ab814128c7240169507e467fee0c79614`  
		Last Modified: Mon, 21 Dec 2020 20:34:47 GMT  
		Size: 163.3 MB (163335834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7843537b91458872ec4b1eaeb7a4dd500e3a96a2c152d9c52ee6e07a490688e4`  
		Last Modified: Mon, 21 Dec 2020 20:34:09 GMT  
		Size: 196.2 KB (196191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd87f6fc20e367ec8d13afabb9f64d16630c31d0dc14f2b9571afae3f66ec01d`  
		Last Modified: Mon, 21 Dec 2020 20:34:09 GMT  
		Size: 913.0 KB (912998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fee38fb9207e61fd6fa47477e5d012c8491066c4c049d0aadfa6a0b7c46171b3`  
		Last Modified: Mon, 21 Dec 2020 22:13:37 GMT  
		Size: 7.0 MB (6989064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `elixir:latest` - linux; ppc64le

```console
$ docker pull elixir@sha256:01b81ca2e4eb103e54b697e02411f83edc8cc628b50f71aff190de7097364782
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **505.1 MB (505058838 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f62304a9e4e742bb1950bdc907e28ce256c5e15a9c67ac49a44cce98d51c7f70`
-	Default Command: `["iex"]`

```dockerfile
# Fri, 11 Dec 2020 03:33:14 GMT
ADD file:3f6d74a3193dcc81fb8d9c0a830337812d5ed7618d5f16c8eb193d30f827c49d in / 
# Fri, 11 Dec 2020 03:33:24 GMT
CMD ["bash"]
# Thu, 17 Dec 2020 11:33:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Dec 2020 11:35:15 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 17 Dec 2020 11:37:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 17 Dec 2020 11:50:40 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 21 Dec 2020 19:21:29 GMT
ENV OTP_VERSION=23.2.1 REBAR3_VERSION=3.14.3
# Mon, 21 Dec 2020 19:21:38 GMT
LABEL org.opencontainers.image.version=23.2.1
# Mon, 21 Dec 2020 19:45:29 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="e7034e2cfe50d7570ac8f70ea7ba69ea013f10863043e25132f0a5d3d0d8d3a7" 	&& runtimeDeps='libodbc1 			libsctp1 			libwxgtk3.0' 	&& buildDeps='unixodbc-dev 			libsctp-dev 			libwxgtk3.0-dev' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make -j$(nproc) docs DOC_TARGETS=chunks 	  && make install install-docs DOC_TARGETS=chunks ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Mon, 21 Dec 2020 19:45:39 GMT
CMD ["erl"]
# Mon, 21 Dec 2020 19:45:45 GMT
ENV REBAR_VERSION=2.6.4
# Mon, 21 Dec 2020 19:46:07 GMT
RUN set -xe 	&& REBAR_DOWNLOAD_URL="https://github.com/rebar/rebar/archive/${REBAR_VERSION}.tar.gz" 	&& REBAR_DOWNLOAD_SHA256="577246bafa2eb2b2c3f1d0c157408650446884555bf87901508ce71d5cc0bd07" 	&& mkdir -p /usr/src/rebar-src 	&& curl -fSL -o rebar-src.tar.gz "$REBAR_DOWNLOAD_URL" 	&& echo "$REBAR_DOWNLOAD_SHA256 rebar-src.tar.gz" | sha256sum -c - 	&& tar -xzf rebar-src.tar.gz -C /usr/src/rebar-src --strip-components=1 	&& rm rebar-src.tar.gz 	&& cd /usr/src/rebar-src 	&& ./bootstrap 	&& install -v ./rebar /usr/local/bin/ 	&& rm -rf /usr/src/rebar-src
# Mon, 21 Dec 2020 19:47:11 GMT
RUN set -xe 	&& REBAR3_DOWNLOAD_URL="https://github.com/erlang/rebar3/archive/${REBAR3_VERSION}.tar.gz" 	&& REBAR3_DOWNLOAD_SHA256="69024b30f17b52c61e5e0568cbf9a2db325eb646ae230c48858401507394f5c0" 	&& mkdir -p /usr/src/rebar3-src 	&& curl -fSL -o rebar3-src.tar.gz "$REBAR3_DOWNLOAD_URL" 	&& echo "$REBAR3_DOWNLOAD_SHA256 rebar3-src.tar.gz" | sha256sum -c - 	&& tar -xzf rebar3-src.tar.gz -C /usr/src/rebar3-src --strip-components=1 	&& rm rebar3-src.tar.gz 	&& cd /usr/src/rebar3-src 	&& HOME=$PWD ./bootstrap 	&& install -v ./rebar3 /usr/local/bin/ 	&& rm -rf /usr/src/rebar3-src
# Mon, 21 Dec 2020 23:32:44 GMT
ENV ELIXIR_VERSION=v1.11.2 LANG=C.UTF-8
# Mon, 21 Dec 2020 23:35:46 GMT
RUN set -xe 	&& ELIXIR_DOWNLOAD_URL="https://github.com/elixir-lang/elixir/archive/${ELIXIR_VERSION}.tar.gz" 	&& ELIXIR_DOWNLOAD_SHA256="318f0a6cb372186b0cf45d2e9c9889b4c9e941643fd67ca0ab1ec32710ab6bf5" 	&& curl -fSL -o elixir-src.tar.gz $ELIXIR_DOWNLOAD_URL 	&& echo "$ELIXIR_DOWNLOAD_SHA256  elixir-src.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/local/src/elixir 	&& tar -xzC /usr/local/src/elixir --strip-components=1 -f elixir-src.tar.gz 	&& rm elixir-src.tar.gz 	&& cd /usr/local/src/elixir 	&& make install clean
# Mon, 21 Dec 2020 23:35:53 GMT
CMD ["iex"]
```

-	Layers:
	-	`sha256:fbe5c9ac66677a4494c2d36707222498adce02d2dcb8e08d2f8a59a0f10b2582`  
		Last Modified: Fri, 11 Dec 2020 03:41:06 GMT  
		Size: 54.1 MB (54142548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66ec43513b23f6fdf7966a25f8c07ddf163a83eecd7793ff3508c4c280091fba`  
		Last Modified: Thu, 17 Dec 2020 13:37:25 GMT  
		Size: 8.3 MB (8255775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1d8dd70933f639bb084c14461d159384654d788cec2e4c66bef8c451f55207f`  
		Last Modified: Thu, 17 Dec 2020 13:37:24 GMT  
		Size: 10.7 MB (10727587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92278c25b4d152f837c7a5038f1a925f0e92765d08e01c91c4d5b74824b37f4`  
		Last Modified: Thu, 17 Dec 2020 13:38:28 GMT  
		Size: 57.5 MB (57455306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e03cdc6497775e6b5f3dfe371ee8ede72e158d0b740f165bce00cc29adf9281f`  
		Last Modified: Thu, 17 Dec 2020 13:41:48 GMT  
		Size: 203.2 MB (203154212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a340d1b28f67662d3d054d4c5558fc8a5bede16604181d2319955d16e18dafd`  
		Last Modified: Mon, 21 Dec 2020 20:13:11 GMT  
		Size: 163.2 MB (163224980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8302f3b7227c876d4587aab25e83584cee0744385db4533a924996bd626c256d`  
		Last Modified: Mon, 21 Dec 2020 20:12:39 GMT  
		Size: 196.2 KB (196199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12b01b8978e3510227d7faf2b3170a666d77bf57a7e352aa68f7b93d9f3d614d`  
		Last Modified: Mon, 21 Dec 2020 20:12:40 GMT  
		Size: 913.0 KB (912994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39bc74482630876ac7e87474b02e93281e53d35cb0cff5144ea982e630440d41`  
		Last Modified: Mon, 21 Dec 2020 23:45:48 GMT  
		Size: 7.0 MB (6989237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `elixir:latest` - linux; s390x

```console
$ docker pull elixir@sha256:ef96247a0ec04cafc11e8ad8756fa956419949d5603b6cbaf6599aeaab31732f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **458.8 MB (458824620 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a4ade72d98eb730000e72287b093bf2135d674b169d63c6caaa086b83ecc425`
-	Default Command: `["iex"]`

```dockerfile
# Fri, 11 Dec 2020 02:11:47 GMT
ADD file:b48379f9d2c111607924e8c59c2769c735341a59df0d6819d8a4b3e44f5457b0 in / 
# Fri, 11 Dec 2020 02:11:54 GMT
CMD ["bash"]
# Thu, 17 Dec 2020 11:13:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Dec 2020 11:13:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 17 Dec 2020 11:14:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 17 Dec 2020 11:17:19 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 21 Dec 2020 19:45:18 GMT
ENV OTP_VERSION=23.2.1 REBAR3_VERSION=3.14.3
# Mon, 21 Dec 2020 19:45:18 GMT
LABEL org.opencontainers.image.version=23.2.1
# Mon, 21 Dec 2020 20:03:51 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="e7034e2cfe50d7570ac8f70ea7ba69ea013f10863043e25132f0a5d3d0d8d3a7" 	&& runtimeDeps='libodbc1 			libsctp1 			libwxgtk3.0' 	&& buildDeps='unixodbc-dev 			libsctp-dev 			libwxgtk3.0-dev' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make -j$(nproc) docs DOC_TARGETS=chunks 	  && make install install-docs DOC_TARGETS=chunks ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Mon, 21 Dec 2020 20:04:14 GMT
CMD ["erl"]
# Mon, 21 Dec 2020 20:04:14 GMT
ENV REBAR_VERSION=2.6.4
# Mon, 21 Dec 2020 20:04:24 GMT
RUN set -xe 	&& REBAR_DOWNLOAD_URL="https://github.com/rebar/rebar/archive/${REBAR_VERSION}.tar.gz" 	&& REBAR_DOWNLOAD_SHA256="577246bafa2eb2b2c3f1d0c157408650446884555bf87901508ce71d5cc0bd07" 	&& mkdir -p /usr/src/rebar-src 	&& curl -fSL -o rebar-src.tar.gz "$REBAR_DOWNLOAD_URL" 	&& echo "$REBAR_DOWNLOAD_SHA256 rebar-src.tar.gz" | sha256sum -c - 	&& tar -xzf rebar-src.tar.gz -C /usr/src/rebar-src --strip-components=1 	&& rm rebar-src.tar.gz 	&& cd /usr/src/rebar-src 	&& ./bootstrap 	&& install -v ./rebar /usr/local/bin/ 	&& rm -rf /usr/src/rebar-src
# Mon, 21 Dec 2020 20:05:16 GMT
RUN set -xe 	&& REBAR3_DOWNLOAD_URL="https://github.com/erlang/rebar3/archive/${REBAR3_VERSION}.tar.gz" 	&& REBAR3_DOWNLOAD_SHA256="69024b30f17b52c61e5e0568cbf9a2db325eb646ae230c48858401507394f5c0" 	&& mkdir -p /usr/src/rebar3-src 	&& curl -fSL -o rebar3-src.tar.gz "$REBAR3_DOWNLOAD_URL" 	&& echo "$REBAR3_DOWNLOAD_SHA256 rebar3-src.tar.gz" | sha256sum -c - 	&& tar -xzf rebar3-src.tar.gz -C /usr/src/rebar3-src --strip-components=1 	&& rm rebar3-src.tar.gz 	&& cd /usr/src/rebar3-src 	&& HOME=$PWD ./bootstrap 	&& install -v ./rebar3 /usr/local/bin/ 	&& rm -rf /usr/src/rebar3-src
# Mon, 21 Dec 2020 21:17:34 GMT
ENV ELIXIR_VERSION=v1.11.2 LANG=C.UTF-8
# Mon, 21 Dec 2020 21:19:23 GMT
RUN set -xe 	&& ELIXIR_DOWNLOAD_URL="https://github.com/elixir-lang/elixir/archive/${ELIXIR_VERSION}.tar.gz" 	&& ELIXIR_DOWNLOAD_SHA256="318f0a6cb372186b0cf45d2e9c9889b4c9e941643fd67ca0ab1ec32710ab6bf5" 	&& curl -fSL -o elixir-src.tar.gz $ELIXIR_DOWNLOAD_URL 	&& echo "$ELIXIR_DOWNLOAD_SHA256  elixir-src.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/local/src/elixir 	&& tar -xzC /usr/local/src/elixir --strip-components=1 -f elixir-src.tar.gz 	&& rm elixir-src.tar.gz 	&& cd /usr/local/src/elixir 	&& make install clean
# Mon, 21 Dec 2020 21:19:24 GMT
CMD ["iex"]
```

-	Layers:
	-	`sha256:b8cd59e115fe85cdffdb9750beb150c189e768249dc100d22cab4733fb0c7247`  
		Last Modified: Fri, 11 Dec 2020 02:16:44 GMT  
		Size: 49.0 MB (48968242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1700123a499ab3151baf0ee060bcc06b796b6407b46e7adbbd2f49d8c2db63fd`  
		Last Modified: Thu, 17 Dec 2020 11:46:18 GMT  
		Size: 7.4 MB (7386722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd656aefa64a4012ebf9ad352be8693ddcef0ff82713b7779c74d54355b38462`  
		Last Modified: Thu, 17 Dec 2020 11:46:18 GMT  
		Size: 9.9 MB (9883179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18b7c267283da311330fb132ef3dab090ca1cdd1273c31176852d7454ae16881`  
		Last Modified: Thu, 17 Dec 2020 11:46:37 GMT  
		Size: 51.4 MB (51380356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22dfc7507ea726b6fc41139d9f9fd4e69dac28229e477fb823125c9fc9606393`  
		Last Modified: Thu, 17 Dec 2020 11:47:10 GMT  
		Size: 176.8 MB (176831353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c40a5b90ba415ab84c7492d4bc6eefcf2d4b0ab07f7038dbc99caac03f6237d`  
		Last Modified: Mon, 21 Dec 2020 20:26:05 GMT  
		Size: 156.3 MB (156276343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c320ed8725ce250787c54d6ae6526dbcfc6a4d6fda0a252f052cf41b8f52dd1`  
		Last Modified: Mon, 21 Dec 2020 20:25:47 GMT  
		Size: 196.2 KB (196185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53cb76b29a4077520685cfc156ccd8424d848b08786b38c127e4363953e4ffbf`  
		Last Modified: Mon, 21 Dec 2020 20:25:46 GMT  
		Size: 913.1 KB (913055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e87e3fa70068cdc2f0e575d479921f6a15fc21a1365a598c959e4c05df602b49`  
		Last Modified: Mon, 21 Dec 2020 21:24:53 GMT  
		Size: 7.0 MB (6989185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
