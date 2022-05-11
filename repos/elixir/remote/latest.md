## `elixir:latest`

```console
$ docker pull elixir@sha256:f160e6dd752596df62e4b0a8c38e62e923f11da163bed4fc9e64a06e4fb4b45f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `elixir:latest` - linux; amd64

```console
$ docker pull elixir@sha256:17b9db8e4061d76acb5bc6a8860508f9d985fdcd03353118d7f4cd4d284cffaa
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **506.5 MB (506464384 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95e128f7b668420eb02f0bc12c718a102b208a3660d3832be1aadf79dbdff29a`
-	Default Command: `["iex"]`

```dockerfile
# Wed, 11 May 2022 01:20:05 GMT
ADD file:68a5d7d0db592625159865110c1b7dcb15cf70ecf71b5fd541ef89584cd734ba in / 
# Wed, 11 May 2022 01:20:05 GMT
CMD ["bash"]
# Wed, 11 May 2022 01:49:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 01:49:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 May 2022 01:49:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 01:50:11 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 02:24:48 GMT
ENV OTP_VERSION=24.3.4 REBAR3_VERSION=3.18.0
# Wed, 11 May 2022 02:24:48 GMT
LABEL org.opencontainers.image.version=24.3.4
# Wed, 11 May 2022 02:31:34 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="e59bedbb871af52244ca5284fd0a572d52128abd4decf4347fe2aef047b65c58" 	&& runtimeDeps='libodbc1 			libsctp1 			libwxgtk3.0' 	&& buildDeps='unixodbc-dev 			libsctp-dev 			libwxgtk-webview3.0-gtk3-dev' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make -j$(nproc) docs DOC_TARGETS=chunks 	  && make install install-docs DOC_TARGETS=chunks ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Wed, 11 May 2022 02:31:35 GMT
CMD ["erl"]
# Wed, 11 May 2022 02:31:35 GMT
ENV REBAR_VERSION=2.6.4
# Wed, 11 May 2022 02:31:38 GMT
RUN set -xe 	&& REBAR_DOWNLOAD_URL="https://github.com/rebar/rebar/archive/${REBAR_VERSION}.tar.gz" 	&& REBAR_DOWNLOAD_SHA256="577246bafa2eb2b2c3f1d0c157408650446884555bf87901508ce71d5cc0bd07" 	&& mkdir -p /usr/src/rebar-src 	&& curl -fSL -o rebar-src.tar.gz "$REBAR_DOWNLOAD_URL" 	&& echo "$REBAR_DOWNLOAD_SHA256 rebar-src.tar.gz" | sha256sum -c - 	&& tar -xzf rebar-src.tar.gz -C /usr/src/rebar-src --strip-components=1 	&& rm rebar-src.tar.gz 	&& cd /usr/src/rebar-src 	&& ./bootstrap 	&& install -v ./rebar /usr/local/bin/ 	&& rm -rf /usr/src/rebar-src
# Wed, 11 May 2022 02:31:53 GMT
RUN set -xe 	&& REBAR3_DOWNLOAD_URL="https://github.com/erlang/rebar3/archive/${REBAR3_VERSION}.tar.gz" 	&& REBAR3_DOWNLOAD_SHA256="cce1925d33240d81d0e4d2de2eef3616d4c17b0532ed004274f875e6607d25d2" 	&& mkdir -p /usr/src/rebar3-src 	&& curl -fSL -o rebar3-src.tar.gz "$REBAR3_DOWNLOAD_URL" 	&& echo "$REBAR3_DOWNLOAD_SHA256 rebar3-src.tar.gz" | sha256sum -c - 	&& tar -xzf rebar3-src.tar.gz -C /usr/src/rebar3-src --strip-components=1 	&& rm rebar3-src.tar.gz 	&& cd /usr/src/rebar3-src 	&& HOME=$PWD ./bootstrap 	&& install -v ./rebar3 /usr/local/bin/ 	&& rm -rf /usr/src/rebar3-src
# Wed, 11 May 2022 20:47:43 GMT
ENV ELIXIR_VERSION=v1.13.4 LANG=C.UTF-8
# Wed, 11 May 2022 20:48:24 GMT
RUN set -xe 	&& ELIXIR_DOWNLOAD_URL="https://github.com/elixir-lang/elixir/archive/${ELIXIR_VERSION}.tar.gz" 	&& ELIXIR_DOWNLOAD_SHA256="95daf2dd3052e6ca7d4d849457eaaba09de52d65ca38d6933c65bc1cdf6b8579" 	&& curl -fSL -o elixir-src.tar.gz $ELIXIR_DOWNLOAD_URL 	&& echo "$ELIXIR_DOWNLOAD_SHA256  elixir-src.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/local/src/elixir 	&& tar -xzC /usr/local/src/elixir --strip-components=1 -f elixir-src.tar.gz 	&& rm elixir-src.tar.gz 	&& cd /usr/local/src/elixir 	&& make install clean 	&& find /usr/local/src/elixir/ -type f -not -regex "/usr/local/src/elixir/lib/[^\/]*/lib.*" -exec rm -rf {} + 	&& find /usr/local/src/elixir/ -type d -depth -empty -delete
# Wed, 11 May 2022 20:48:24 GMT
CMD ["iex"]
```

-	Layers:
	-	`sha256:67e8aa6c8bbc76b1f2bccb3864b0887671833b8667dc1f6c965fcb0eac7e6402`  
		Last Modified: Wed, 11 May 2022 01:24:45 GMT  
		Size: 54.9 MB (54945622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:627e6c1e105548ea4a08354eea581f137cf368d91aeb0ad47dcb706fca54fd8b`  
		Last Modified: Wed, 11 May 2022 01:57:17 GMT  
		Size: 5.2 MB (5155721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0670968926f6461e3135c82ba2c0ad3ebdedc0d0f41b18bda4a1e41104b8be8a`  
		Last Modified: Wed, 11 May 2022 01:57:18 GMT  
		Size: 10.9 MB (10875052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a8b0e20be4b4a332bc3d90b9903a5f3c0664b440fd9f1d2a1db0d4b7e6e826b`  
		Last Modified: Wed, 11 May 2022 01:57:38 GMT  
		Size: 54.6 MB (54578468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0b10a3a2784b06bfe0af1493ea2a0fa957ae5e0dc30fcfd1166d2558ba74e4d`  
		Last Modified: Wed, 11 May 2022 01:58:14 GMT  
		Size: 196.6 MB (196562669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbc56586252fe871d988e13f9839a92a690f7ef814ccf5022edcadc61a6d6a14`  
		Last Modified: Wed, 11 May 2022 04:09:09 GMT  
		Size: 177.2 MB (177238702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42d5499926e582173f4eb67d608c91aa1259da76b526befbd0a03de9751f4beb`  
		Last Modified: Wed, 11 May 2022 04:08:47 GMT  
		Size: 196.5 KB (196529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6bede41ebadddab2f72f740a8aa5e8977fe02d73f79336e420f0b51abe47aa9`  
		Last Modified: Wed, 11 May 2022 04:08:47 GMT  
		Size: 966.7 KB (966728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:493223d4f0abc8b02120c55881303f2554c8cebc9403f47fa529413debecd06f`  
		Last Modified: Wed, 11 May 2022 21:06:59 GMT  
		Size: 5.9 MB (5944893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `elixir:latest` - linux; arm variant v7

```console
$ docker pull elixir@sha256:07e2f4712c173dae55c3b9fe523c7ddcb384110c2dd420b616f1a91b6ac8b91a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **447.0 MB (446981826 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57615d7db87b4849e6d15d8e2930bfc28acabebdaf98a71f1544e470013ca352`
-	Default Command: `["iex"]`

```dockerfile
# Wed, 20 Apr 2022 13:26:39 GMT
ADD file:1c05c50014bbd32a4cf1edd085996a8c62abc3c8969b64d2355475827a07475e in / 
# Wed, 20 Apr 2022 13:26:40 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 20:06:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 20:07:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 20 Apr 2022 20:07:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 20:09:53 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 09 May 2022 17:58:59 GMT
ENV OTP_VERSION=24.3.4 REBAR3_VERSION=3.18.0
# Mon, 09 May 2022 17:58:59 GMT
LABEL org.opencontainers.image.version=24.3.4
# Mon, 09 May 2022 18:10:20 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="e59bedbb871af52244ca5284fd0a572d52128abd4decf4347fe2aef047b65c58" 	&& runtimeDeps='libodbc1 			libsctp1 			libwxgtk3.0' 	&& buildDeps='unixodbc-dev 			libsctp-dev 			libwxgtk-webview3.0-gtk3-dev' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make -j$(nproc) docs DOC_TARGETS=chunks 	  && make install install-docs DOC_TARGETS=chunks ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Mon, 09 May 2022 18:10:21 GMT
CMD ["erl"]
# Mon, 09 May 2022 18:10:22 GMT
ENV REBAR_VERSION=2.6.4
# Mon, 09 May 2022 18:10:31 GMT
RUN set -xe 	&& REBAR_DOWNLOAD_URL="https://github.com/rebar/rebar/archive/${REBAR_VERSION}.tar.gz" 	&& REBAR_DOWNLOAD_SHA256="577246bafa2eb2b2c3f1d0c157408650446884555bf87901508ce71d5cc0bd07" 	&& mkdir -p /usr/src/rebar-src 	&& curl -fSL -o rebar-src.tar.gz "$REBAR_DOWNLOAD_URL" 	&& echo "$REBAR_DOWNLOAD_SHA256 rebar-src.tar.gz" | sha256sum -c - 	&& tar -xzf rebar-src.tar.gz -C /usr/src/rebar-src --strip-components=1 	&& rm rebar-src.tar.gz 	&& cd /usr/src/rebar-src 	&& ./bootstrap 	&& install -v ./rebar /usr/local/bin/ 	&& rm -rf /usr/src/rebar-src
# Mon, 09 May 2022 18:11:15 GMT
RUN set -xe 	&& REBAR3_DOWNLOAD_URL="https://github.com/erlang/rebar3/archive/${REBAR3_VERSION}.tar.gz" 	&& REBAR3_DOWNLOAD_SHA256="cce1925d33240d81d0e4d2de2eef3616d4c17b0532ed004274f875e6607d25d2" 	&& mkdir -p /usr/src/rebar3-src 	&& curl -fSL -o rebar3-src.tar.gz "$REBAR3_DOWNLOAD_URL" 	&& echo "$REBAR3_DOWNLOAD_SHA256 rebar3-src.tar.gz" | sha256sum -c - 	&& tar -xzf rebar3-src.tar.gz -C /usr/src/rebar3-src --strip-components=1 	&& rm rebar3-src.tar.gz 	&& cd /usr/src/rebar3-src 	&& HOME=$PWD ./bootstrap 	&& install -v ./rebar3 /usr/local/bin/ 	&& rm -rf /usr/src/rebar3-src
# Tue, 10 May 2022 01:21:00 GMT
ENV ELIXIR_VERSION=v1.13.4 LANG=C.UTF-8
# Tue, 10 May 2022 01:23:12 GMT
RUN set -xe 	&& ELIXIR_DOWNLOAD_URL="https://github.com/elixir-lang/elixir/archive/${ELIXIR_VERSION}.tar.gz" 	&& ELIXIR_DOWNLOAD_SHA256="95daf2dd3052e6ca7d4d849457eaaba09de52d65ca38d6933c65bc1cdf6b8579" 	&& curl -fSL -o elixir-src.tar.gz $ELIXIR_DOWNLOAD_URL 	&& echo "$ELIXIR_DOWNLOAD_SHA256  elixir-src.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/local/src/elixir 	&& tar -xzC /usr/local/src/elixir --strip-components=1 -f elixir-src.tar.gz 	&& rm elixir-src.tar.gz 	&& cd /usr/local/src/elixir 	&& make install clean 	&& find /usr/local/src/elixir/ -type f -not -regex "/usr/local/src/elixir/lib/[^\/]*/lib.*" -exec rm -rf {} + 	&& find /usr/local/src/elixir/ -type d -depth -empty -delete
# Tue, 10 May 2022 01:23:12 GMT
CMD ["iex"]
```

-	Layers:
	-	`sha256:0a2c02101ee4340d4a9ebb962e9331486e417a3835c9adefb9badd2f0c116ab6`  
		Last Modified: Wed, 20 Apr 2022 13:42:55 GMT  
		Size: 50.1 MB (50133696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:301394875428f05a3ac7068600f0d729f8c7df313e7c9574aec8362194fb4e56`  
		Last Modified: Wed, 20 Apr 2022 20:30:57 GMT  
		Size: 4.9 MB (4924850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44f80b9e8049b2a4b26cc100bccded1ae7d0bc8ff2e1fa9fc7e255631328f0af`  
		Last Modified: Wed, 20 Apr 2022 20:30:59 GMT  
		Size: 10.2 MB (10218007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08bb57ee492f81d7ea44b47b65fd9782dfb9241e2f5c66bd60aaba1aa5d4fcb2`  
		Last Modified: Wed, 20 Apr 2022 20:31:49 GMT  
		Size: 50.3 MB (50327803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0de27a4f4528de43d948c6d64536df939f8a738ff32df51880108c21021e59cd`  
		Last Modified: Wed, 20 Apr 2022 20:33:42 GMT  
		Size: 167.2 MB (167226095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17720168c5c22320ef6a02eb990cdee09aa4ac9d3aa54699b262145a8ac1c42d`  
		Last Modified: Mon, 09 May 2022 19:43:45 GMT  
		Size: 157.0 MB (157043203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cf9c8cd35b2c7bc896d61e64c3210d52ed8e0b79d2a6d3ca3b3d7d09d4bb14c`  
		Last Modified: Mon, 09 May 2022 19:42:57 GMT  
		Size: 196.5 KB (196508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e2d0bf42d836d001cbc0c51fe143734a9fc074cfd93f163d278f35e64ecdd60`  
		Last Modified: Mon, 09 May 2022 19:42:57 GMT  
		Size: 966.7 KB (966730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd62f9becf4a3b7d0afe9ac27c98b253ce6ffec4d81aa0bfc92ae89e7b898541`  
		Last Modified: Tue, 10 May 2022 02:19:08 GMT  
		Size: 5.9 MB (5944934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `elixir:latest` - linux; arm64 variant v8

```console
$ docker pull elixir@sha256:a3259ec9a9c8baf06dbb4255c9287c61dd9b185d91691c751f701e79170272d7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **483.1 MB (483140869 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc26f85d148492a232d8dbb8b2f6a56948f243a96731f4e7d0fc56a88a86adcf`
-	Default Command: `["iex"]`

```dockerfile
# Wed, 20 Apr 2022 04:28:55 GMT
ADD file:ece192802cbdaf1a141d04f0c2e90cfd3479e5e3e82c6a00206970684494cf48 in / 
# Wed, 20 Apr 2022 04:28:56 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 06:44:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 06:44:12 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 20 Apr 2022 06:44:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 06:45:15 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 09 May 2022 20:31:31 GMT
ENV OTP_VERSION=24.3.4 REBAR3_VERSION=3.18.0
# Mon, 09 May 2022 20:31:32 GMT
LABEL org.opencontainers.image.version=24.3.4
# Mon, 09 May 2022 20:36:56 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="e59bedbb871af52244ca5284fd0a572d52128abd4decf4347fe2aef047b65c58" 	&& runtimeDeps='libodbc1 			libsctp1 			libwxgtk3.0' 	&& buildDeps='unixodbc-dev 			libsctp-dev 			libwxgtk-webview3.0-gtk3-dev' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make -j$(nproc) docs DOC_TARGETS=chunks 	  && make install install-docs DOC_TARGETS=chunks ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Mon, 09 May 2022 20:36:57 GMT
CMD ["erl"]
# Mon, 09 May 2022 20:36:58 GMT
ENV REBAR_VERSION=2.6.4
# Mon, 09 May 2022 20:37:04 GMT
RUN set -xe 	&& REBAR_DOWNLOAD_URL="https://github.com/rebar/rebar/archive/${REBAR_VERSION}.tar.gz" 	&& REBAR_DOWNLOAD_SHA256="577246bafa2eb2b2c3f1d0c157408650446884555bf87901508ce71d5cc0bd07" 	&& mkdir -p /usr/src/rebar-src 	&& curl -fSL -o rebar-src.tar.gz "$REBAR_DOWNLOAD_URL" 	&& echo "$REBAR_DOWNLOAD_SHA256 rebar-src.tar.gz" | sha256sum -c - 	&& tar -xzf rebar-src.tar.gz -C /usr/src/rebar-src --strip-components=1 	&& rm rebar-src.tar.gz 	&& cd /usr/src/rebar-src 	&& ./bootstrap 	&& install -v ./rebar /usr/local/bin/ 	&& rm -rf /usr/src/rebar-src
# Mon, 09 May 2022 20:37:23 GMT
RUN set -xe 	&& REBAR3_DOWNLOAD_URL="https://github.com/erlang/rebar3/archive/${REBAR3_VERSION}.tar.gz" 	&& REBAR3_DOWNLOAD_SHA256="cce1925d33240d81d0e4d2de2eef3616d4c17b0532ed004274f875e6607d25d2" 	&& mkdir -p /usr/src/rebar3-src 	&& curl -fSL -o rebar3-src.tar.gz "$REBAR3_DOWNLOAD_URL" 	&& echo "$REBAR3_DOWNLOAD_SHA256 rebar3-src.tar.gz" | sha256sum -c - 	&& tar -xzf rebar3-src.tar.gz -C /usr/src/rebar3-src --strip-components=1 	&& rm rebar3-src.tar.gz 	&& cd /usr/src/rebar3-src 	&& HOME=$PWD ./bootstrap 	&& install -v ./rebar3 /usr/local/bin/ 	&& rm -rf /usr/src/rebar3-src
# Mon, 09 May 2022 21:39:19 GMT
ENV ELIXIR_VERSION=v1.13.4 LANG=C.UTF-8
# Mon, 09 May 2022 21:40:11 GMT
RUN set -xe 	&& ELIXIR_DOWNLOAD_URL="https://github.com/elixir-lang/elixir/archive/${ELIXIR_VERSION}.tar.gz" 	&& ELIXIR_DOWNLOAD_SHA256="95daf2dd3052e6ca7d4d849457eaaba09de52d65ca38d6933c65bc1cdf6b8579" 	&& curl -fSL -o elixir-src.tar.gz $ELIXIR_DOWNLOAD_URL 	&& echo "$ELIXIR_DOWNLOAD_SHA256  elixir-src.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/local/src/elixir 	&& tar -xzC /usr/local/src/elixir --strip-components=1 -f elixir-src.tar.gz 	&& rm elixir-src.tar.gz 	&& cd /usr/local/src/elixir 	&& make install clean 	&& find /usr/local/src/elixir/ -type f -not -regex "/usr/local/src/elixir/lib/[^\/]*/lib.*" -exec rm -rf {} + 	&& find /usr/local/src/elixir/ -type d -depth -empty -delete
# Mon, 09 May 2022 21:40:12 GMT
CMD ["iex"]
```

-	Layers:
	-	`sha256:83d5dcfea08e6927083bc886bf182fc39d87bb04b54b63002ac0c4c0b9aab682`  
		Last Modified: Wed, 20 Apr 2022 04:35:19 GMT  
		Size: 53.6 MB (53633096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45cfa86b7b1aca6d694057e4d42ee1440527f41c00b9e577df729244380c9eba`  
		Last Modified: Wed, 20 Apr 2022 06:54:10 GMT  
		Size: 4.9 MB (4938663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c79b19335f27cc78840bf9159e875322f3252ac06113c73756f9d4fba905f9b`  
		Last Modified: Wed, 20 Apr 2022 06:54:10 GMT  
		Size: 10.7 MB (10656971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:350ecaf08eac09037b05465ab97a1b8f7bc9b7a9b1fcef900dedd7dba9bbcf4d`  
		Last Modified: Wed, 20 Apr 2022 06:54:32 GMT  
		Size: 54.7 MB (54672934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:360771a6f68b528d0cf1b5534f58aaff178b78ec0fafb483b1ef47b7ae2b2d3e`  
		Last Modified: Wed, 20 Apr 2022 06:55:10 GMT  
		Size: 189.6 MB (189580023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7793cd3fd718efb9d4b773bc5d56e293ceba2bbd7f10fbc3bb3212927ed09be3`  
		Last Modified: Mon, 09 May 2022 21:19:09 GMT  
		Size: 162.6 MB (162550343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b20f5c777d63d95c28b80d86f807249861c7f5d67e8a006d191cd09f7a14675`  
		Last Modified: Mon, 09 May 2022 21:18:48 GMT  
		Size: 196.4 KB (196446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1c354b3c0101a5bbad11d18901136e4ecf91ae5dffc5e14d1a15a01ecf2ad1c`  
		Last Modified: Mon, 09 May 2022 21:18:48 GMT  
		Size: 966.6 KB (966640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cc55075fcbde210e1606ea9bebfcaaaaa4c684d1c9481ee2adb7facc82d5f9a`  
		Last Modified: Mon, 09 May 2022 22:02:32 GMT  
		Size: 5.9 MB (5945753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `elixir:latest` - linux; 386

```console
$ docker pull elixir@sha256:7fb4379dd8a7cb307d68dbb18cb2c43360b8eeb5cf466258a6348ca0a86e213b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **506.0 MB (506014704 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b38736fb3846dfe89934c6d993f11a1e11778e0146412252bb9c1008b959e3e`
-	Default Command: `["iex"]`

```dockerfile
# Wed, 11 May 2022 01:38:57 GMT
ADD file:dae3dc662d1327f461e95b84f6f9282f3c4fb51f16ac8f20a5f141951d8436a9 in / 
# Wed, 11 May 2022 01:38:58 GMT
CMD ["bash"]
# Wed, 11 May 2022 02:10:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 02:10:56 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 May 2022 02:11:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 02:12:18 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 02:40:23 GMT
ENV OTP_VERSION=24.3.4 REBAR3_VERSION=3.18.0
# Wed, 11 May 2022 02:40:24 GMT
LABEL org.opencontainers.image.version=24.3.4
# Wed, 11 May 2022 02:47:06 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="e59bedbb871af52244ca5284fd0a572d52128abd4decf4347fe2aef047b65c58" 	&& runtimeDeps='libodbc1 			libsctp1 			libwxgtk3.0' 	&& buildDeps='unixodbc-dev 			libsctp-dev 			libwxgtk-webview3.0-gtk3-dev' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make -j$(nproc) docs DOC_TARGETS=chunks 	  && make install install-docs DOC_TARGETS=chunks ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Wed, 11 May 2022 02:47:07 GMT
CMD ["erl"]
# Wed, 11 May 2022 02:47:08 GMT
ENV REBAR_VERSION=2.6.4
# Wed, 11 May 2022 02:47:14 GMT
RUN set -xe 	&& REBAR_DOWNLOAD_URL="https://github.com/rebar/rebar/archive/${REBAR_VERSION}.tar.gz" 	&& REBAR_DOWNLOAD_SHA256="577246bafa2eb2b2c3f1d0c157408650446884555bf87901508ce71d5cc0bd07" 	&& mkdir -p /usr/src/rebar-src 	&& curl -fSL -o rebar-src.tar.gz "$REBAR_DOWNLOAD_URL" 	&& echo "$REBAR_DOWNLOAD_SHA256 rebar-src.tar.gz" | sha256sum -c - 	&& tar -xzf rebar-src.tar.gz -C /usr/src/rebar-src --strip-components=1 	&& rm rebar-src.tar.gz 	&& cd /usr/src/rebar-src 	&& ./bootstrap 	&& install -v ./rebar /usr/local/bin/ 	&& rm -rf /usr/src/rebar-src
# Wed, 11 May 2022 02:47:39 GMT
RUN set -xe 	&& REBAR3_DOWNLOAD_URL="https://github.com/erlang/rebar3/archive/${REBAR3_VERSION}.tar.gz" 	&& REBAR3_DOWNLOAD_SHA256="cce1925d33240d81d0e4d2de2eef3616d4c17b0532ed004274f875e6607d25d2" 	&& mkdir -p /usr/src/rebar3-src 	&& curl -fSL -o rebar3-src.tar.gz "$REBAR3_DOWNLOAD_URL" 	&& echo "$REBAR3_DOWNLOAD_SHA256 rebar3-src.tar.gz" | sha256sum -c - 	&& tar -xzf rebar3-src.tar.gz -C /usr/src/rebar3-src --strip-components=1 	&& rm rebar3-src.tar.gz 	&& cd /usr/src/rebar3-src 	&& HOME=$PWD ./bootstrap 	&& install -v ./rebar3 /usr/local/bin/ 	&& rm -rf /usr/src/rebar3-src
# Wed, 11 May 2022 16:26:36 GMT
ENV ELIXIR_VERSION=v1.13.4 LANG=C.UTF-8
# Wed, 11 May 2022 16:27:42 GMT
RUN set -xe 	&& ELIXIR_DOWNLOAD_URL="https://github.com/elixir-lang/elixir/archive/${ELIXIR_VERSION}.tar.gz" 	&& ELIXIR_DOWNLOAD_SHA256="95daf2dd3052e6ca7d4d849457eaaba09de52d65ca38d6933c65bc1cdf6b8579" 	&& curl -fSL -o elixir-src.tar.gz $ELIXIR_DOWNLOAD_URL 	&& echo "$ELIXIR_DOWNLOAD_SHA256  elixir-src.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/local/src/elixir 	&& tar -xzC /usr/local/src/elixir --strip-components=1 -f elixir-src.tar.gz 	&& rm elixir-src.tar.gz 	&& cd /usr/local/src/elixir 	&& make install clean 	&& find /usr/local/src/elixir/ -type f -not -regex "/usr/local/src/elixir/lib/[^\/]*/lib.*" -exec rm -rf {} + 	&& find /usr/local/src/elixir/ -type d -depth -empty -delete
# Wed, 11 May 2022 16:27:43 GMT
CMD ["iex"]
```

-	Layers:
	-	`sha256:5ad4f92623738998bc77103ff64344255f842f6e5fe4a846df656351b3c4852f`  
		Last Modified: Wed, 11 May 2022 01:45:53 GMT  
		Size: 55.9 MB (55942833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:026e99ab0e4b1d3aec936d04cdf9c04ddc8074f2917b86c02e66d88fcae1e42f`  
		Last Modified: Wed, 11 May 2022 02:21:42 GMT  
		Size: 5.1 MB (5080245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66dba083f619f2a2c8cfef4a4e844cf6819c306e225029e62cf7c31c17b0d344`  
		Last Modified: Wed, 11 May 2022 02:21:43 GMT  
		Size: 11.0 MB (11033702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a5333a48696af9b52c4219f20b87c5cf9b05764b7c58cd19880e6c5730d1b75`  
		Last Modified: Wed, 11 May 2022 02:22:10 GMT  
		Size: 55.9 MB (55914622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:899f353e6896a6f03a5af06a01cea44badeac7062481c294a9d7c1da1859b823`  
		Last Modified: Wed, 11 May 2022 02:22:52 GMT  
		Size: 199.5 MB (199502725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf7983cd427bd8c4625f51e3c110ac884233bca60d129e2f3bab89198fa87a87`  
		Last Modified: Wed, 11 May 2022 04:08:14 GMT  
		Size: 171.4 MB (171431709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb440b28a1e704fc8efcab491324863408a43f28cf8a78934058133ea73671ad`  
		Last Modified: Wed, 11 May 2022 04:07:54 GMT  
		Size: 196.4 KB (196436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fa9ce3dee521b8d4765eba50e31fd8b3383ccb8285a6649096e3002558ded22`  
		Last Modified: Wed, 11 May 2022 04:07:54 GMT  
		Size: 966.6 KB (966636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:202d9175896b267a2180a9dca76af74a5d60b7dd85a0da9afd18089b9f5a37f1`  
		Last Modified: Wed, 11 May 2022 16:49:14 GMT  
		Size: 5.9 MB (5945796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `elixir:latest` - linux; ppc64le

```console
$ docker pull elixir@sha256:c5c3d3255ed87173b8c318c09a71202f0f99b6c433d3e19d71eb1b5e9c4bc471
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **509.9 MB (509876441 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11e84d71dc88f59db82a2a52a8945ce9d586d7a9f1ed329d4f46f01388229845`
-	Default Command: `["iex"]`

```dockerfile
# Wed, 20 Apr 2022 09:45:51 GMT
ADD file:2fff7021563ff08bee97c626d3c91410f8f8dc3213b548a7e8b0c351557c7f1d in / 
# Wed, 20 Apr 2022 09:46:01 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 16:46:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 16:47:42 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 20 Apr 2022 16:49:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 16:56:15 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 09 May 2022 23:20:55 GMT
ENV OTP_VERSION=24.3.4 REBAR3_VERSION=3.18.0
# Mon, 09 May 2022 23:20:57 GMT
LABEL org.opencontainers.image.version=24.3.4
# Mon, 09 May 2022 23:33:58 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="e59bedbb871af52244ca5284fd0a572d52128abd4decf4347fe2aef047b65c58" 	&& runtimeDeps='libodbc1 			libsctp1 			libwxgtk3.0' 	&& buildDeps='unixodbc-dev 			libsctp-dev 			libwxgtk-webview3.0-gtk3-dev' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make -j$(nproc) docs DOC_TARGETS=chunks 	  && make install install-docs DOC_TARGETS=chunks ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Mon, 09 May 2022 23:34:11 GMT
CMD ["erl"]
# Mon, 09 May 2022 23:34:13 GMT
ENV REBAR_VERSION=2.6.4
# Mon, 09 May 2022 23:34:25 GMT
RUN set -xe 	&& REBAR_DOWNLOAD_URL="https://github.com/rebar/rebar/archive/${REBAR_VERSION}.tar.gz" 	&& REBAR_DOWNLOAD_SHA256="577246bafa2eb2b2c3f1d0c157408650446884555bf87901508ce71d5cc0bd07" 	&& mkdir -p /usr/src/rebar-src 	&& curl -fSL -o rebar-src.tar.gz "$REBAR_DOWNLOAD_URL" 	&& echo "$REBAR_DOWNLOAD_SHA256 rebar-src.tar.gz" | sha256sum -c - 	&& tar -xzf rebar-src.tar.gz -C /usr/src/rebar-src --strip-components=1 	&& rm rebar-src.tar.gz 	&& cd /usr/src/rebar-src 	&& ./bootstrap 	&& install -v ./rebar /usr/local/bin/ 	&& rm -rf /usr/src/rebar-src
# Mon, 09 May 2022 23:35:09 GMT
RUN set -xe 	&& REBAR3_DOWNLOAD_URL="https://github.com/erlang/rebar3/archive/${REBAR3_VERSION}.tar.gz" 	&& REBAR3_DOWNLOAD_SHA256="cce1925d33240d81d0e4d2de2eef3616d4c17b0532ed004274f875e6607d25d2" 	&& mkdir -p /usr/src/rebar3-src 	&& curl -fSL -o rebar3-src.tar.gz "$REBAR3_DOWNLOAD_URL" 	&& echo "$REBAR3_DOWNLOAD_SHA256 rebar3-src.tar.gz" | sha256sum -c - 	&& tar -xzf rebar3-src.tar.gz -C /usr/src/rebar3-src --strip-components=1 	&& rm rebar3-src.tar.gz 	&& cd /usr/src/rebar3-src 	&& HOME=$PWD ./bootstrap 	&& install -v ./rebar3 /usr/local/bin/ 	&& rm -rf /usr/src/rebar3-src
# Tue, 10 May 2022 01:20:56 GMT
ENV ELIXIR_VERSION=v1.13.4 LANG=C.UTF-8
# Tue, 10 May 2022 01:22:58 GMT
RUN set -xe 	&& ELIXIR_DOWNLOAD_URL="https://github.com/elixir-lang/elixir/archive/${ELIXIR_VERSION}.tar.gz" 	&& ELIXIR_DOWNLOAD_SHA256="95daf2dd3052e6ca7d4d849457eaaba09de52d65ca38d6933c65bc1cdf6b8579" 	&& curl -fSL -o elixir-src.tar.gz $ELIXIR_DOWNLOAD_URL 	&& echo "$ELIXIR_DOWNLOAD_SHA256  elixir-src.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/local/src/elixir 	&& tar -xzC /usr/local/src/elixir --strip-components=1 -f elixir-src.tar.gz 	&& rm elixir-src.tar.gz 	&& cd /usr/local/src/elixir 	&& make install clean 	&& find /usr/local/src/elixir/ -type f -not -regex "/usr/local/src/elixir/lib/[^\/]*/lib.*" -exec rm -rf {} + 	&& find /usr/local/src/elixir/ -type d -depth -empty -delete
# Tue, 10 May 2022 01:23:02 GMT
CMD ["iex"]
```

-	Layers:
	-	`sha256:09c77622a2c385ed83fadca4a945b0065fdeaaac427ce2b1a9e795ce2007f8c3`  
		Last Modified: Wed, 20 Apr 2022 09:56:19 GMT  
		Size: 58.8 MB (58835334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40ca809b2ea695f0799b00d20783f98ba01ff0027cda46173ed27695cab4b285`  
		Last Modified: Wed, 20 Apr 2022 17:25:52 GMT  
		Size: 5.4 MB (5405282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6df07c738b32af886b9ac59e4c9e9fdf67b4fec93e92eacbcae05a6c9d2c758`  
		Last Modified: Wed, 20 Apr 2022 17:25:53 GMT  
		Size: 11.6 MB (11627614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a2b022e0dbff39b4cebc15bf43d0c74ad5bc802ccab05dc1cb6968abbcf844c`  
		Last Modified: Wed, 20 Apr 2022 17:27:05 GMT  
		Size: 58.9 MB (58855216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40187f7892789769600c273492f290474dc51bdbcf1f42676c5988db32f43aec`  
		Last Modified: Wed, 20 Apr 2022 17:29:37 GMT  
		Size: 196.1 MB (196108793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:565b233602f67b6fad57d1a738eea51fbf61ed8c5731c0c0d086b4afb8eee0f6`  
		Last Modified: Tue, 10 May 2022 01:00:16 GMT  
		Size: 171.9 MB (171936048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c8c7ee2fb7d3e2512395f0ab94ee79d3e321ed8324dfdd18c9f9c3f3402eed3`  
		Last Modified: Tue, 10 May 2022 00:59:48 GMT  
		Size: 196.5 KB (196527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c40366853de42f483d9dd255816b9716f0f710f25ea3f7582d8a5f2d743c8c26`  
		Last Modified: Tue, 10 May 2022 00:59:49 GMT  
		Size: 966.7 KB (966727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5b1a05dcc197e74a4ff1135d64f52bb201aa3edd8f632f66a678e4bec83b783`  
		Last Modified: Tue, 10 May 2022 02:06:39 GMT  
		Size: 5.9 MB (5944900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `elixir:latest` - linux; s390x

```console
$ docker pull elixir@sha256:7bc9d64315b9de528442459f47349885aad1783acc5f92cad8b7caf98c166544
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **471.8 MB (471834653 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ff332ca19eb8fc2c1180eaa28eaac1a0539ddcbb7c00b2a5c2782112dba3c58`
-	Default Command: `["iex"]`

```dockerfile
# Wed, 11 May 2022 00:43:58 GMT
ADD file:8b9cfb1e16e1c11cdc1f936ccd3dfdd2104ab85b0b9078b1fe3bca89f53e0682 in / 
# Wed, 11 May 2022 00:44:00 GMT
CMD ["bash"]
# Wed, 11 May 2022 01:15:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 01:15:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 May 2022 01:15:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 01:16:34 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 01:51:56 GMT
ENV OTP_VERSION=24.3.4 REBAR3_VERSION=3.18.0
# Wed, 11 May 2022 01:51:57 GMT
LABEL org.opencontainers.image.version=24.3.4
# Wed, 11 May 2022 01:57:49 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="e59bedbb871af52244ca5284fd0a572d52128abd4decf4347fe2aef047b65c58" 	&& runtimeDeps='libodbc1 			libsctp1 			libwxgtk3.0' 	&& buildDeps='unixodbc-dev 			libsctp-dev 			libwxgtk-webview3.0-gtk3-dev' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make -j$(nproc) docs DOC_TARGETS=chunks 	  && make install install-docs DOC_TARGETS=chunks ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Wed, 11 May 2022 01:57:56 GMT
CMD ["erl"]
# Wed, 11 May 2022 01:57:56 GMT
ENV REBAR_VERSION=2.6.4
# Wed, 11 May 2022 01:58:00 GMT
RUN set -xe 	&& REBAR_DOWNLOAD_URL="https://github.com/rebar/rebar/archive/${REBAR_VERSION}.tar.gz" 	&& REBAR_DOWNLOAD_SHA256="577246bafa2eb2b2c3f1d0c157408650446884555bf87901508ce71d5cc0bd07" 	&& mkdir -p /usr/src/rebar-src 	&& curl -fSL -o rebar-src.tar.gz "$REBAR_DOWNLOAD_URL" 	&& echo "$REBAR_DOWNLOAD_SHA256 rebar-src.tar.gz" | sha256sum -c - 	&& tar -xzf rebar-src.tar.gz -C /usr/src/rebar-src --strip-components=1 	&& rm rebar-src.tar.gz 	&& cd /usr/src/rebar-src 	&& ./bootstrap 	&& install -v ./rebar /usr/local/bin/ 	&& rm -rf /usr/src/rebar-src
# Wed, 11 May 2022 01:58:16 GMT
RUN set -xe 	&& REBAR3_DOWNLOAD_URL="https://github.com/erlang/rebar3/archive/${REBAR3_VERSION}.tar.gz" 	&& REBAR3_DOWNLOAD_SHA256="cce1925d33240d81d0e4d2de2eef3616d4c17b0532ed004274f875e6607d25d2" 	&& mkdir -p /usr/src/rebar3-src 	&& curl -fSL -o rebar3-src.tar.gz "$REBAR3_DOWNLOAD_URL" 	&& echo "$REBAR3_DOWNLOAD_SHA256 rebar3-src.tar.gz" | sha256sum -c - 	&& tar -xzf rebar3-src.tar.gz -C /usr/src/rebar3-src --strip-components=1 	&& rm rebar3-src.tar.gz 	&& cd /usr/src/rebar3-src 	&& HOME=$PWD ./bootstrap 	&& install -v ./rebar3 /usr/local/bin/ 	&& rm -rf /usr/src/rebar3-src
# Wed, 11 May 2022 16:47:38 GMT
ENV ELIXIR_VERSION=v1.13.4 LANG=C.UTF-8
# Wed, 11 May 2022 16:48:24 GMT
RUN set -xe 	&& ELIXIR_DOWNLOAD_URL="https://github.com/elixir-lang/elixir/archive/${ELIXIR_VERSION}.tar.gz" 	&& ELIXIR_DOWNLOAD_SHA256="95daf2dd3052e6ca7d4d849457eaaba09de52d65ca38d6933c65bc1cdf6b8579" 	&& curl -fSL -o elixir-src.tar.gz $ELIXIR_DOWNLOAD_URL 	&& echo "$ELIXIR_DOWNLOAD_SHA256  elixir-src.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/local/src/elixir 	&& tar -xzC /usr/local/src/elixir --strip-components=1 -f elixir-src.tar.gz 	&& rm elixir-src.tar.gz 	&& cd /usr/local/src/elixir 	&& make install clean 	&& find /usr/local/src/elixir/ -type f -not -regex "/usr/local/src/elixir/lib/[^\/]*/lib.*" -exec rm -rf {} + 	&& find /usr/local/src/elixir/ -type d -depth -empty -delete
# Wed, 11 May 2022 16:48:25 GMT
CMD ["iex"]
```

-	Layers:
	-	`sha256:f8313f715dc1cdd9f8a3da73eafca06dcb30dff4c078bee35a162247cae99c4d`  
		Last Modified: Wed, 11 May 2022 00:49:41 GMT  
		Size: 53.2 MB (53208696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c99502d0a4c52d58c73f967ad2c52204db08f01c6512da3a6dfd8d8ea18b3ae6`  
		Last Modified: Wed, 11 May 2022 01:24:43 GMT  
		Size: 5.1 MB (5140503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33ef0d35554dad3cfdd15fa175311fb6c20c545c9b04632039378e90a1666435`  
		Last Modified: Wed, 11 May 2022 01:24:43 GMT  
		Size: 10.8 MB (10765296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c36704bf1413eb96906c58893a7d4c74f7d88490eed870be03fe531302614745`  
		Last Modified: Wed, 11 May 2022 01:25:00 GMT  
		Size: 54.0 MB (54045195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9b12d26f79096a8ccb3b94ad468c2ae17af08aa0226a5de33c5292b25ae24d4`  
		Last Modified: Wed, 11 May 2022 01:25:31 GMT  
		Size: 172.6 MB (172581996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffe156bae6385ce1b51fd3173a381a343150993ff15f95716f389a9b2f7e9704`  
		Last Modified: Wed, 11 May 2022 02:27:20 GMT  
		Size: 169.0 MB (168984866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed7b77a2f0ebd42b9469ac6b187f0b81bd3d4555b953e20acb74565585e10a08`  
		Last Modified: Wed, 11 May 2022 02:27:02 GMT  
		Size: 196.5 KB (196519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27f9878e399ceb1d3116eb75599f1ada4b5a0e9b4c40693ee3d0d07179871e56`  
		Last Modified: Wed, 11 May 2022 02:27:02 GMT  
		Size: 966.7 KB (966723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caffec794479045e77540aa47d7bf6fa038d7e2a795b5fbf4138ad9909c2cc31`  
		Last Modified: Wed, 11 May 2022 17:02:30 GMT  
		Size: 5.9 MB (5944859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
