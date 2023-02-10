## `elixir:latest`

```console
$ docker pull elixir@sha256:e013df17ec2036c960d50b63e46efb91f803ff9b57ddf43a7a6bdd9dde547b89
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
$ docker pull elixir@sha256:336a6736283a7fbf2d7bb825d0099d6e6c9fa18fd073ebe1f7b2f096a2a7dbd1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **573.1 MB (573145472 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:891b38bfd5ff5886cb4860293e2472ec1164bbbd11aeb2af99759cbc3b2dd178`
-	Default Command: `["iex"]`

```dockerfile
# Sat, 04 Feb 2023 06:51:26 GMT
ADD file:cc6a56676703ec7ab5db8f2f7bc18a3169c0816d38703845b6b77ae5342ab41c in / 
# Sat, 04 Feb 2023 06:51:27 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 07:22:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 07:22:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 04 Feb 2023 07:22:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 07:23:44 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 07:34:56 GMT
ENV OTP_VERSION=25.2.2 REBAR3_VERSION=3.19.0
# Sat, 04 Feb 2023 07:34:56 GMT
LABEL org.opencontainers.image.version=25.2.2
# Sat, 04 Feb 2023 07:42:29 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="535e535b2e90e71deca96c53f19710e6ebf3d4289b0a3116e7cf83b7e2c4bb7e" 	&& runtimeDeps='libodbc1 			libsctp1 			libwxgtk3.0 			libwxgtk-webview3.0-gtk3-0v5' 	&& buildDeps='unixodbc-dev 			libsctp-dev 			libwxgtk-webview3.0-gtk3-dev' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make -j$(nproc) docs DOC_TARGETS=chunks 	  && make install install-docs DOC_TARGETS=chunks ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Sat, 04 Feb 2023 07:42:31 GMT
CMD ["erl"]
# Sat, 04 Feb 2023 07:42:31 GMT
ENV REBAR_VERSION=2.6.4
# Sat, 04 Feb 2023 07:42:34 GMT
RUN set -xe 	&& REBAR_DOWNLOAD_URL="https://github.com/rebar/rebar/archive/${REBAR_VERSION}.tar.gz" 	&& REBAR_DOWNLOAD_SHA256="577246bafa2eb2b2c3f1d0c157408650446884555bf87901508ce71d5cc0bd07" 	&& mkdir -p /usr/src/rebar-src 	&& curl -fSL -o rebar-src.tar.gz "$REBAR_DOWNLOAD_URL" 	&& echo "$REBAR_DOWNLOAD_SHA256 rebar-src.tar.gz" | sha256sum -c - 	&& tar -xzf rebar-src.tar.gz -C /usr/src/rebar-src --strip-components=1 	&& rm rebar-src.tar.gz 	&& cd /usr/src/rebar-src 	&& ./bootstrap 	&& install -v ./rebar /usr/local/bin/ 	&& rm -rf /usr/src/rebar-src
# Sat, 04 Feb 2023 07:42:50 GMT
RUN set -xe 	&& REBAR3_DOWNLOAD_URL="https://github.com/erlang/rebar3/archive/${REBAR3_VERSION}.tar.gz" 	&& REBAR3_DOWNLOAD_SHA256="ff9ef42c737480477ebdf0dd9d95ece534a14c96f05edafbf32e9af973280bc3" 	&& mkdir -p /usr/src/rebar3-src 	&& curl -fSL -o rebar3-src.tar.gz "$REBAR3_DOWNLOAD_URL" 	&& echo "$REBAR3_DOWNLOAD_SHA256 rebar3-src.tar.gz" | sha256sum -c - 	&& tar -xzf rebar3-src.tar.gz -C /usr/src/rebar3-src --strip-components=1 	&& rm rebar3-src.tar.gz 	&& cd /usr/src/rebar3-src 	&& HOME=$PWD ./bootstrap 	&& install -v ./rebar3 /usr/local/bin/ 	&& rm -rf /usr/src/rebar3-src
# Sun, 05 Feb 2023 01:00:44 GMT
ENV ELIXIR_VERSION=v1.14.3 LANG=C.UTF-8
# Sun, 05 Feb 2023 01:01:23 GMT
RUN set -xe 	&& ELIXIR_DOWNLOAD_URL="https://github.com/elixir-lang/elixir/archive/${ELIXIR_VERSION}.tar.gz" 	&& ELIXIR_DOWNLOAD_SHA256="bd464145257f36bd64f7ba8bed93b6499c50571b415c491b20267d27d7035707" 	&& curl -fSL -o elixir-src.tar.gz $ELIXIR_DOWNLOAD_URL 	&& echo "$ELIXIR_DOWNLOAD_SHA256  elixir-src.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/local/src/elixir 	&& tar -xzC /usr/local/src/elixir --strip-components=1 -f elixir-src.tar.gz 	&& rm elixir-src.tar.gz 	&& cd /usr/local/src/elixir 	&& make install clean 	&& find /usr/local/src/elixir/ -type f -not -regex "/usr/local/src/elixir/lib/[^\/]*/lib.*" -exec rm -rf {} + 	&& find /usr/local/src/elixir/ -type d -depth -empty -delete
# Sun, 05 Feb 2023 01:01:23 GMT
CMD ["iex"]
```

-	Layers:
	-	`sha256:699c8a97647f5789e5850bcf1a3d5afe9730edb654e1ae0714d5bd198a67a3ed`  
		Last Modified: Sat, 04 Feb 2023 06:55:53 GMT  
		Size: 55.0 MB (55025312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86cd158b89fde67a8a4c428a844985f930eba450ec3fde1c9ef5df3884128c62`  
		Last Modified: Sat, 04 Feb 2023 07:29:25 GMT  
		Size: 5.2 MB (5165476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a226e961cfaa2d1d171e429e9db314feec6201f5cba1487b20e7aee311e4a54f`  
		Last Modified: Sat, 04 Feb 2023 07:29:25 GMT  
		Size: 10.9 MB (10876697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cec535da207f5d811fda01a346f5561fd2f77c2d09a080925b7455b84f0959e`  
		Last Modified: Sat, 04 Feb 2023 07:29:44 GMT  
		Size: 54.6 MB (54587320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:225fdd30e1a3eb664decd3c5720a9500ef3ce275075e7c61bb904f0b4d4b2f46`  
		Last Modified: Sat, 04 Feb 2023 07:30:21 GMT  
		Size: 196.9 MB (196890310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:067da9168d3974d05a3d688148ee65252b80293e9cd0edd230137156c280dbbf`  
		Last Modified: Sat, 04 Feb 2023 09:01:57 GMT  
		Size: 243.2 MB (243208757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f76a5698eff7d5a412f61370d40d3762aaa18ba839d0ae77b008ec2ef8569b5b`  
		Last Modified: Sat, 04 Feb 2023 09:01:27 GMT  
		Size: 198.6 KB (198603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae2e104cb45ff1ae8dbdd5abff661abeb3122e32e3f611823dec79c902a471c2`  
		Last Modified: Sat, 04 Feb 2023 09:01:27 GMT  
		Size: 988.3 KB (988288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43b1809b23921f7ad49f1806fdb13143999e431210e98e7f04c045a54bb502d0`  
		Last Modified: Sun, 05 Feb 2023 01:23:05 GMT  
		Size: 6.2 MB (6204709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `elixir:latest` - linux; arm variant v7

```console
$ docker pull elixir@sha256:f4f334d80b117624d8387a39c70004c6f117e1385570bb3f2de2056c303f4413
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **508.4 MB (508351689 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c822ca4c509ddb9970dc634eb4eb4f04d9309f601f5b40df06c69154d67e1164`
-	Default Command: `["iex"]`

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
# Sat, 04 Feb 2023 11:08:19 GMT
ENV OTP_VERSION=25.2.2 REBAR3_VERSION=3.19.0
# Sat, 04 Feb 2023 11:08:19 GMT
LABEL org.opencontainers.image.version=25.2.2
# Sat, 04 Feb 2023 11:14:48 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="535e535b2e90e71deca96c53f19710e6ebf3d4289b0a3116e7cf83b7e2c4bb7e" 	&& runtimeDeps='libodbc1 			libsctp1 			libwxgtk3.0 			libwxgtk-webview3.0-gtk3-0v5' 	&& buildDeps='unixodbc-dev 			libsctp-dev 			libwxgtk-webview3.0-gtk3-dev' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make -j$(nproc) docs DOC_TARGETS=chunks 	  && make install install-docs DOC_TARGETS=chunks ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Sat, 04 Feb 2023 11:14:49 GMT
CMD ["erl"]
# Sat, 04 Feb 2023 11:14:49 GMT
ENV REBAR_VERSION=2.6.4
# Sat, 04 Feb 2023 11:14:53 GMT
RUN set -xe 	&& REBAR_DOWNLOAD_URL="https://github.com/rebar/rebar/archive/${REBAR_VERSION}.tar.gz" 	&& REBAR_DOWNLOAD_SHA256="577246bafa2eb2b2c3f1d0c157408650446884555bf87901508ce71d5cc0bd07" 	&& mkdir -p /usr/src/rebar-src 	&& curl -fSL -o rebar-src.tar.gz "$REBAR_DOWNLOAD_URL" 	&& echo "$REBAR_DOWNLOAD_SHA256 rebar-src.tar.gz" | sha256sum -c - 	&& tar -xzf rebar-src.tar.gz -C /usr/src/rebar-src --strip-components=1 	&& rm rebar-src.tar.gz 	&& cd /usr/src/rebar-src 	&& ./bootstrap 	&& install -v ./rebar /usr/local/bin/ 	&& rm -rf /usr/src/rebar-src
# Sat, 04 Feb 2023 11:15:13 GMT
RUN set -xe 	&& REBAR3_DOWNLOAD_URL="https://github.com/erlang/rebar3/archive/${REBAR3_VERSION}.tar.gz" 	&& REBAR3_DOWNLOAD_SHA256="ff9ef42c737480477ebdf0dd9d95ece534a14c96f05edafbf32e9af973280bc3" 	&& mkdir -p /usr/src/rebar3-src 	&& curl -fSL -o rebar3-src.tar.gz "$REBAR3_DOWNLOAD_URL" 	&& echo "$REBAR3_DOWNLOAD_SHA256 rebar3-src.tar.gz" | sha256sum -c - 	&& tar -xzf rebar3-src.tar.gz -C /usr/src/rebar3-src --strip-components=1 	&& rm rebar3-src.tar.gz 	&& cd /usr/src/rebar3-src 	&& HOME=$PWD ./bootstrap 	&& install -v ./rebar3 /usr/local/bin/ 	&& rm -rf /usr/src/rebar3-src
# Sun, 05 Feb 2023 05:53:38 GMT
ENV ELIXIR_VERSION=v1.14.3 LANG=C.UTF-8
# Sun, 05 Feb 2023 05:54:27 GMT
RUN set -xe 	&& ELIXIR_DOWNLOAD_URL="https://github.com/elixir-lang/elixir/archive/${ELIXIR_VERSION}.tar.gz" 	&& ELIXIR_DOWNLOAD_SHA256="bd464145257f36bd64f7ba8bed93b6499c50571b415c491b20267d27d7035707" 	&& curl -fSL -o elixir-src.tar.gz $ELIXIR_DOWNLOAD_URL 	&& echo "$ELIXIR_DOWNLOAD_SHA256  elixir-src.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/local/src/elixir 	&& tar -xzC /usr/local/src/elixir --strip-components=1 -f elixir-src.tar.gz 	&& rm elixir-src.tar.gz 	&& cd /usr/local/src/elixir 	&& make install clean 	&& find /usr/local/src/elixir/ -type f -not -regex "/usr/local/src/elixir/lib/[^\/]*/lib.*" -exec rm -rf {} + 	&& find /usr/local/src/elixir/ -type d -depth -empty -delete
# Sun, 05 Feb 2023 05:54:28 GMT
CMD ["iex"]
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
	-	`sha256:a17eecd5aad341be4ea7bad9719585ac06018482d8fa545c7080254d94a89aa4`  
		Last Modified: Sat, 04 Feb 2023 12:43:03 GMT  
		Size: 217.9 MB (217901396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4bbb01bc1665401193c2ffb227d448c0a0cb702d7563f1d2ee7898cc47456be`  
		Last Modified: Sat, 04 Feb 2023 12:42:30 GMT  
		Size: 198.6 KB (198594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faae2df64d8ba2455e91abc9786a0634463ddd00bdaf43d516336cd98ab4e85c`  
		Last Modified: Sat, 04 Feb 2023 12:42:30 GMT  
		Size: 988.3 KB (988286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e60ceaf92aeb262fe3bfa10356cee897799e7c7d0e8eead52088b60c6e78264`  
		Last Modified: Sun, 05 Feb 2023 06:22:17 GMT  
		Size: 6.2 MB (6204628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `elixir:latest` - linux; arm64 variant v8

```console
$ docker pull elixir@sha256:2b1e4b64273be873c5817029de2402d11aff1f2e2dbf40e729670c29a38a8f4c
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **558.6 MB (558634724 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2aeaf6f6b19f3e66d5ab7f539507a24463ba540b6a4a0ca5964e6a29f83d8410`
-	Default Command: `["iex"]`

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
# Thu, 09 Feb 2023 21:43:18 GMT
ENV OTP_VERSION=25.2.2 REBAR3_VERSION=3.19.0
# Thu, 09 Feb 2023 21:43:18 GMT
LABEL org.opencontainers.image.version=25.2.2
# Thu, 09 Feb 2023 21:48:22 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="535e535b2e90e71deca96c53f19710e6ebf3d4289b0a3116e7cf83b7e2c4bb7e" 	&& runtimeDeps='libodbc1 			libsctp1 			libwxgtk3.0 			libwxgtk-webview3.0-gtk3-0v5' 	&& buildDeps='unixodbc-dev 			libsctp-dev 			libwxgtk-webview3.0-gtk3-dev' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make -j$(nproc) docs DOC_TARGETS=chunks 	  && make install install-docs DOC_TARGETS=chunks ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Thu, 09 Feb 2023 21:48:25 GMT
CMD ["erl"]
# Thu, 09 Feb 2023 21:48:26 GMT
ENV REBAR_VERSION=2.6.4
# Thu, 09 Feb 2023 21:48:28 GMT
RUN set -xe 	&& REBAR_DOWNLOAD_URL="https://github.com/rebar/rebar/archive/${REBAR_VERSION}.tar.gz" 	&& REBAR_DOWNLOAD_SHA256="577246bafa2eb2b2c3f1d0c157408650446884555bf87901508ce71d5cc0bd07" 	&& mkdir -p /usr/src/rebar-src 	&& curl -fSL -o rebar-src.tar.gz "$REBAR_DOWNLOAD_URL" 	&& echo "$REBAR_DOWNLOAD_SHA256 rebar-src.tar.gz" | sha256sum -c - 	&& tar -xzf rebar-src.tar.gz -C /usr/src/rebar-src --strip-components=1 	&& rm rebar-src.tar.gz 	&& cd /usr/src/rebar-src 	&& ./bootstrap 	&& install -v ./rebar /usr/local/bin/ 	&& rm -rf /usr/src/rebar-src
# Thu, 09 Feb 2023 21:48:39 GMT
RUN set -xe 	&& REBAR3_DOWNLOAD_URL="https://github.com/erlang/rebar3/archive/${REBAR3_VERSION}.tar.gz" 	&& REBAR3_DOWNLOAD_SHA256="ff9ef42c737480477ebdf0dd9d95ece534a14c96f05edafbf32e9af973280bc3" 	&& mkdir -p /usr/src/rebar3-src 	&& curl -fSL -o rebar3-src.tar.gz "$REBAR3_DOWNLOAD_URL" 	&& echo "$REBAR3_DOWNLOAD_SHA256 rebar3-src.tar.gz" | sha256sum -c - 	&& tar -xzf rebar3-src.tar.gz -C /usr/src/rebar3-src --strip-components=1 	&& rm rebar3-src.tar.gz 	&& cd /usr/src/rebar3-src 	&& HOME=$PWD ./bootstrap 	&& install -v ./rebar3 /usr/local/bin/ 	&& rm -rf /usr/src/rebar3-src
# Thu, 09 Feb 2023 22:56:48 GMT
ENV ELIXIR_VERSION=v1.14.3 LANG=C.UTF-8
# Thu, 09 Feb 2023 22:57:16 GMT
RUN set -xe 	&& ELIXIR_DOWNLOAD_URL="https://github.com/elixir-lang/elixir/archive/${ELIXIR_VERSION}.tar.gz" 	&& ELIXIR_DOWNLOAD_SHA256="bd464145257f36bd64f7ba8bed93b6499c50571b415c491b20267d27d7035707" 	&& curl -fSL -o elixir-src.tar.gz $ELIXIR_DOWNLOAD_URL 	&& echo "$ELIXIR_DOWNLOAD_SHA256  elixir-src.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/local/src/elixir 	&& tar -xzC /usr/local/src/elixir --strip-components=1 -f elixir-src.tar.gz 	&& rm elixir-src.tar.gz 	&& cd /usr/local/src/elixir 	&& make install clean 	&& find /usr/local/src/elixir/ -type f -not -regex "/usr/local/src/elixir/lib/[^\/]*/lib.*" -exec rm -rf {} + 	&& find /usr/local/src/elixir/ -type d -depth -empty -delete
# Thu, 09 Feb 2023 22:57:16 GMT
CMD ["iex"]
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
	-	`sha256:00119c189ae7f6ba599d24a0c5e16bf71080163798cf5dc212f0a5360ca366f3`  
		Last Modified: Thu, 09 Feb 2023 22:15:06 GMT  
		Size: 237.0 MB (237026442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:238fe696035b88239f527e4779896efb0fe33efa9ec15c012646ae16e672d866`  
		Last Modified: Thu, 09 Feb 2023 22:14:43 GMT  
		Size: 198.6 KB (198617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10a354392b0401381b79abeb4205c62c9bec00c858888a585271e9defdb1d46c`  
		Last Modified: Thu, 09 Feb 2023 22:14:43 GMT  
		Size: 988.3 KB (988286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee7fa38484a96ad3e62e03697049a3323b7498393b51fcbbfe881275ede0be38`  
		Last Modified: Thu, 09 Feb 2023 23:06:26 GMT  
		Size: 6.2 MB (6204718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `elixir:latest` - linux; 386

```console
$ docker pull elixir@sha256:53fe374852e05488418acd5ea3fe89cb9d86277e700c1714682d190e4714eb2d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **573.9 MB (573914576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0dce732666b5b2e5a2b5a2dac4d30cf049966c33aabfa8d1e444c5ef2344bef2`
-	Default Command: `["iex"]`

```dockerfile
# Thu, 09 Feb 2023 05:12:37 GMT
ADD file:feaff299d3310c04952143a422f0d0bdd292cd174513c54b1f50765cdbcfd401 in / 
# Thu, 09 Feb 2023 05:12:38 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 12:17:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 12:18:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 09 Feb 2023 12:18:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 12:19:14 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 20:47:14 GMT
ENV OTP_VERSION=25.2.2 REBAR3_VERSION=3.19.0
# Thu, 09 Feb 2023 20:47:15 GMT
LABEL org.opencontainers.image.version=25.2.2
# Thu, 09 Feb 2023 20:54:42 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="535e535b2e90e71deca96c53f19710e6ebf3d4289b0a3116e7cf83b7e2c4bb7e" 	&& runtimeDeps='libodbc1 			libsctp1 			libwxgtk3.0 			libwxgtk-webview3.0-gtk3-0v5' 	&& buildDeps='unixodbc-dev 			libsctp-dev 			libwxgtk-webview3.0-gtk3-dev' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make -j$(nproc) docs DOC_TARGETS=chunks 	  && make install install-docs DOC_TARGETS=chunks ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Thu, 09 Feb 2023 20:54:43 GMT
CMD ["erl"]
# Thu, 09 Feb 2023 20:54:44 GMT
ENV REBAR_VERSION=2.6.4
# Thu, 09 Feb 2023 20:54:51 GMT
RUN set -xe 	&& REBAR_DOWNLOAD_URL="https://github.com/rebar/rebar/archive/${REBAR_VERSION}.tar.gz" 	&& REBAR_DOWNLOAD_SHA256="577246bafa2eb2b2c3f1d0c157408650446884555bf87901508ce71d5cc0bd07" 	&& mkdir -p /usr/src/rebar-src 	&& curl -fSL -o rebar-src.tar.gz "$REBAR_DOWNLOAD_URL" 	&& echo "$REBAR_DOWNLOAD_SHA256 rebar-src.tar.gz" | sha256sum -c - 	&& tar -xzf rebar-src.tar.gz -C /usr/src/rebar-src --strip-components=1 	&& rm rebar-src.tar.gz 	&& cd /usr/src/rebar-src 	&& ./bootstrap 	&& install -v ./rebar /usr/local/bin/ 	&& rm -rf /usr/src/rebar-src
# Thu, 09 Feb 2023 20:55:17 GMT
RUN set -xe 	&& REBAR3_DOWNLOAD_URL="https://github.com/erlang/rebar3/archive/${REBAR3_VERSION}.tar.gz" 	&& REBAR3_DOWNLOAD_SHA256="ff9ef42c737480477ebdf0dd9d95ece534a14c96f05edafbf32e9af973280bc3" 	&& mkdir -p /usr/src/rebar3-src 	&& curl -fSL -o rebar3-src.tar.gz "$REBAR3_DOWNLOAD_URL" 	&& echo "$REBAR3_DOWNLOAD_SHA256 rebar3-src.tar.gz" | sha256sum -c - 	&& tar -xzf rebar3-src.tar.gz -C /usr/src/rebar3-src --strip-components=1 	&& rm rebar3-src.tar.gz 	&& cd /usr/src/rebar3-src 	&& HOME=$PWD ./bootstrap 	&& install -v ./rebar3 /usr/local/bin/ 	&& rm -rf /usr/src/rebar3-src
# Fri, 10 Feb 2023 00:35:01 GMT
ENV ELIXIR_VERSION=v1.14.3 LANG=C.UTF-8
# Fri, 10 Feb 2023 00:36:02 GMT
RUN set -xe 	&& ELIXIR_DOWNLOAD_URL="https://github.com/elixir-lang/elixir/archive/${ELIXIR_VERSION}.tar.gz" 	&& ELIXIR_DOWNLOAD_SHA256="bd464145257f36bd64f7ba8bed93b6499c50571b415c491b20267d27d7035707" 	&& curl -fSL -o elixir-src.tar.gz $ELIXIR_DOWNLOAD_URL 	&& echo "$ELIXIR_DOWNLOAD_SHA256  elixir-src.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/local/src/elixir 	&& tar -xzC /usr/local/src/elixir --strip-components=1 -f elixir-src.tar.gz 	&& rm elixir-src.tar.gz 	&& cd /usr/local/src/elixir 	&& make install clean 	&& find /usr/local/src/elixir/ -type f -not -regex "/usr/local/src/elixir/lib/[^\/]*/lib.*" -exec rm -rf {} + 	&& find /usr/local/src/elixir/ -type d -depth -empty -delete
# Fri, 10 Feb 2023 00:36:03 GMT
CMD ["iex"]
```

-	Layers:
	-	`sha256:9708eacca143ba8fa6c7e9a5b05456412b7b16629c20015a43f3ca391e066162`  
		Last Modified: Thu, 09 Feb 2023 05:18:13 GMT  
		Size: 56.0 MB (56030197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2436c12af0f101964f33b5c8cb58b6d5c8545be186ccfd0a63c09e496aacbd2`  
		Last Modified: Thu, 09 Feb 2023 12:25:19 GMT  
		Size: 5.1 MB (5087608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1f29511ba3bdac349af70ef81cb279b5b72aaa9cca1ef8bb69b6504ed40fecc`  
		Last Modified: Thu, 09 Feb 2023 12:25:19 GMT  
		Size: 11.0 MB (11032576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f598f483dc59afccd15236ab50153d148e29cc22c780301ab19ec1c53dda3de3`  
		Last Modified: Thu, 09 Feb 2023 12:25:41 GMT  
		Size: 55.9 MB (55922803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c14471548627c04d470672a2450dcb91a32fa0737c6d2816766ac5c688e955fd`  
		Last Modified: Thu, 09 Feb 2023 12:26:18 GMT  
		Size: 199.8 MB (199782107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9321a123df495f695ba45ae1b9a6a3378f09d87ba6c48bdf6f54ab674ae8be9`  
		Last Modified: Thu, 09 Feb 2023 21:33:21 GMT  
		Size: 238.7 MB (238667160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c652d9b4f976fc3e2ffd53146cd7f88128682b2aa4947550c8bf833c1cf74dd`  
		Last Modified: Thu, 09 Feb 2023 21:32:53 GMT  
		Size: 198.5 KB (198531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e3b6d0feded04fcff6ef50ee5fcaadea5911afd58064715d72adabf9b53d05e`  
		Last Modified: Thu, 09 Feb 2023 21:32:53 GMT  
		Size: 988.2 KB (988188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4abbd355b5e0c2d2ca5296260191c1715aef83b7ca3c51f8f32709e9cca98d5`  
		Last Modified: Fri, 10 Feb 2023 00:52:16 GMT  
		Size: 6.2 MB (6205406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `elixir:latest` - linux; ppc64le

```console
$ docker pull elixir@sha256:e0937da4f29f460948e8e467c22f6362fcaa8b3ab68eb5c6f5cec422a673f47e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **579.2 MB (579202566 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d093c2a9a9068852a893f9e5759102f209d22605f4d680e0765f5a483c5a7a52`
-	Default Command: `["iex"]`

```dockerfile
# Thu, 09 Feb 2023 06:21:21 GMT
ADD file:0cbfdb018ccae985f6d364f1de7d39fa004cbc966374ba83727c34aa39f946d4 in / 
# Thu, 09 Feb 2023 06:21:24 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 12:25:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 12:26:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 09 Feb 2023 12:26:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 12:29:31 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 20:42:19 GMT
ENV OTP_VERSION=25.2.2 REBAR3_VERSION=3.19.0
# Thu, 09 Feb 2023 20:42:20 GMT
LABEL org.opencontainers.image.version=25.2.2
# Thu, 09 Feb 2023 21:15:53 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="535e535b2e90e71deca96c53f19710e6ebf3d4289b0a3116e7cf83b7e2c4bb7e" 	&& runtimeDeps='libodbc1 			libsctp1 			libwxgtk3.0 			libwxgtk-webview3.0-gtk3-0v5' 	&& buildDeps='unixodbc-dev 			libsctp-dev 			libwxgtk-webview3.0-gtk3-dev' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make -j$(nproc) docs DOC_TARGETS=chunks 	  && make install install-docs DOC_TARGETS=chunks ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Thu, 09 Feb 2023 21:16:18 GMT
CMD ["erl"]
# Thu, 09 Feb 2023 21:16:21 GMT
ENV REBAR_VERSION=2.6.4
# Thu, 09 Feb 2023 21:16:33 GMT
RUN set -xe 	&& REBAR_DOWNLOAD_URL="https://github.com/rebar/rebar/archive/${REBAR_VERSION}.tar.gz" 	&& REBAR_DOWNLOAD_SHA256="577246bafa2eb2b2c3f1d0c157408650446884555bf87901508ce71d5cc0bd07" 	&& mkdir -p /usr/src/rebar-src 	&& curl -fSL -o rebar-src.tar.gz "$REBAR_DOWNLOAD_URL" 	&& echo "$REBAR_DOWNLOAD_SHA256 rebar-src.tar.gz" | sha256sum -c - 	&& tar -xzf rebar-src.tar.gz -C /usr/src/rebar-src --strip-components=1 	&& rm rebar-src.tar.gz 	&& cd /usr/src/rebar-src 	&& ./bootstrap 	&& install -v ./rebar /usr/local/bin/ 	&& rm -rf /usr/src/rebar-src
# Thu, 09 Feb 2023 21:17:20 GMT
RUN set -xe 	&& REBAR3_DOWNLOAD_URL="https://github.com/erlang/rebar3/archive/${REBAR3_VERSION}.tar.gz" 	&& REBAR3_DOWNLOAD_SHA256="ff9ef42c737480477ebdf0dd9d95ece534a14c96f05edafbf32e9af973280bc3" 	&& mkdir -p /usr/src/rebar3-src 	&& curl -fSL -o rebar3-src.tar.gz "$REBAR3_DOWNLOAD_URL" 	&& echo "$REBAR3_DOWNLOAD_SHA256 rebar3-src.tar.gz" | sha256sum -c - 	&& tar -xzf rebar3-src.tar.gz -C /usr/src/rebar3-src --strip-components=1 	&& rm rebar3-src.tar.gz 	&& cd /usr/src/rebar3-src 	&& HOME=$PWD ./bootstrap 	&& install -v ./rebar3 /usr/local/bin/ 	&& rm -rf /usr/src/rebar3-src
# Fri, 10 Feb 2023 02:44:54 GMT
ENV ELIXIR_VERSION=v1.14.3 LANG=C.UTF-8
# Fri, 10 Feb 2023 02:46:35 GMT
RUN set -xe 	&& ELIXIR_DOWNLOAD_URL="https://github.com/elixir-lang/elixir/archive/${ELIXIR_VERSION}.tar.gz" 	&& ELIXIR_DOWNLOAD_SHA256="bd464145257f36bd64f7ba8bed93b6499c50571b415c491b20267d27d7035707" 	&& curl -fSL -o elixir-src.tar.gz $ELIXIR_DOWNLOAD_URL 	&& echo "$ELIXIR_DOWNLOAD_SHA256  elixir-src.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/local/src/elixir 	&& tar -xzC /usr/local/src/elixir --strip-components=1 -f elixir-src.tar.gz 	&& rm elixir-src.tar.gz 	&& cd /usr/local/src/elixir 	&& make install clean 	&& find /usr/local/src/elixir/ -type f -not -regex "/usr/local/src/elixir/lib/[^\/]*/lib.*" -exec rm -rf {} + 	&& find /usr/local/src/elixir/ -type d -depth -empty -delete
# Fri, 10 Feb 2023 02:46:36 GMT
CMD ["iex"]
```

-	Layers:
	-	`sha256:219f4ac08f8026026673d3212473b774749e609a07e734f5812912239893f829`  
		Last Modified: Thu, 09 Feb 2023 06:27:52 GMT  
		Size: 58.9 MB (58923468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af05075258a7b7e3950c556c3a1feae17ac34c796aafd8beeef7f65a09814c48`  
		Last Modified: Thu, 09 Feb 2023 12:38:53 GMT  
		Size: 5.4 MB (5414780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04e56ff8ec6e7948d252089abddb1a40b844be981bbf0a052c4ec922f6b85c05`  
		Last Modified: Thu, 09 Feb 2023 12:38:53 GMT  
		Size: 11.6 MB (11630002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:716d43753f364c16df9587ba5279080353a1eeb5e6d111c50b7f24e0b75a8b7f`  
		Last Modified: Thu, 09 Feb 2023 12:39:23 GMT  
		Size: 58.9 MB (58862445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1423f5c2b50aba38458b445c1d9c8e3df16b6c9e1f677af7a56066963d4e1a3a`  
		Last Modified: Thu, 09 Feb 2023 12:40:22 GMT  
		Size: 196.2 MB (196227631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c42ef25bbf2ae5a87303a6e855db44a190ba30f208098610465ae897f7c937d`  
		Last Modified: Thu, 09 Feb 2023 21:43:21 GMT  
		Size: 240.8 MB (240752616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14c61bd17c52b846c17cabb2d966cd98155c077f0d8607659dded43cb246194a`  
		Last Modified: Thu, 09 Feb 2023 21:42:28 GMT  
		Size: 198.6 KB (198615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6836a723164367cfac6a05108bdf1fc49e8fa5ff832b70d278c358cc9c0e5b8`  
		Last Modified: Thu, 09 Feb 2023 21:42:28 GMT  
		Size: 988.3 KB (988288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:505935ca24db51aafa15d427acde584b79080cc42b1fe7620dbfab1d0fead34c`  
		Last Modified: Fri, 10 Feb 2023 02:57:17 GMT  
		Size: 6.2 MB (6204721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `elixir:latest` - linux; s390x

```console
$ docker pull elixir@sha256:78f9d47a8f0e7a7886f1ea9214c7852683d814aa5d4dc4e0e19d076008c94b3f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **534.8 MB (534755895 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28bda0bdddb83f61cd1710e97765d7a84c12a8bdadecff466f6a3c28c5400c34`
-	Default Command: `["iex"]`

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
# Thu, 09 Feb 2023 14:47:40 GMT
ENV OTP_VERSION=25.2.2 REBAR3_VERSION=3.19.0
# Thu, 09 Feb 2023 14:47:41 GMT
LABEL org.opencontainers.image.version=25.2.2
# Thu, 09 Feb 2023 15:00:23 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="535e535b2e90e71deca96c53f19710e6ebf3d4289b0a3116e7cf83b7e2c4bb7e" 	&& runtimeDeps='libodbc1 			libsctp1 			libwxgtk3.0 			libwxgtk-webview3.0-gtk3-0v5' 	&& buildDeps='unixodbc-dev 			libsctp-dev 			libwxgtk-webview3.0-gtk3-dev' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make -j$(nproc) docs DOC_TARGETS=chunks 	  && make install install-docs DOC_TARGETS=chunks ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Thu, 09 Feb 2023 15:00:33 GMT
CMD ["erl"]
# Thu, 09 Feb 2023 15:00:33 GMT
ENV REBAR_VERSION=2.6.4
# Thu, 09 Feb 2023 15:00:37 GMT
RUN set -xe 	&& REBAR_DOWNLOAD_URL="https://github.com/rebar/rebar/archive/${REBAR_VERSION}.tar.gz" 	&& REBAR_DOWNLOAD_SHA256="577246bafa2eb2b2c3f1d0c157408650446884555bf87901508ce71d5cc0bd07" 	&& mkdir -p /usr/src/rebar-src 	&& curl -fSL -o rebar-src.tar.gz "$REBAR_DOWNLOAD_URL" 	&& echo "$REBAR_DOWNLOAD_SHA256 rebar-src.tar.gz" | sha256sum -c - 	&& tar -xzf rebar-src.tar.gz -C /usr/src/rebar-src --strip-components=1 	&& rm rebar-src.tar.gz 	&& cd /usr/src/rebar-src 	&& ./bootstrap 	&& install -v ./rebar /usr/local/bin/ 	&& rm -rf /usr/src/rebar-src
# Thu, 09 Feb 2023 15:00:56 GMT
RUN set -xe 	&& REBAR3_DOWNLOAD_URL="https://github.com/erlang/rebar3/archive/${REBAR3_VERSION}.tar.gz" 	&& REBAR3_DOWNLOAD_SHA256="ff9ef42c737480477ebdf0dd9d95ece534a14c96f05edafbf32e9af973280bc3" 	&& mkdir -p /usr/src/rebar3-src 	&& curl -fSL -o rebar3-src.tar.gz "$REBAR3_DOWNLOAD_URL" 	&& echo "$REBAR3_DOWNLOAD_SHA256 rebar3-src.tar.gz" | sha256sum -c - 	&& tar -xzf rebar3-src.tar.gz -C /usr/src/rebar3-src --strip-components=1 	&& rm rebar3-src.tar.gz 	&& cd /usr/src/rebar3-src 	&& HOME=$PWD ./bootstrap 	&& install -v ./rebar3 /usr/local/bin/ 	&& rm -rf /usr/src/rebar3-src
# Thu, 09 Feb 2023 20:24:13 GMT
ENV ELIXIR_VERSION=v1.14.3 LANG=C.UTF-8
# Thu, 09 Feb 2023 20:25:57 GMT
RUN set -xe 	&& ELIXIR_DOWNLOAD_URL="https://github.com/elixir-lang/elixir/archive/${ELIXIR_VERSION}.tar.gz" 	&& ELIXIR_DOWNLOAD_SHA256="bd464145257f36bd64f7ba8bed93b6499c50571b415c491b20267d27d7035707" 	&& curl -fSL -o elixir-src.tar.gz $ELIXIR_DOWNLOAD_URL 	&& echo "$ELIXIR_DOWNLOAD_SHA256  elixir-src.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/local/src/elixir 	&& tar -xzC /usr/local/src/elixir --strip-components=1 -f elixir-src.tar.gz 	&& rm elixir-src.tar.gz 	&& cd /usr/local/src/elixir 	&& make install clean 	&& find /usr/local/src/elixir/ -type f -not -regex "/usr/local/src/elixir/lib/[^\/]*/lib.*" -exec rm -rf {} + 	&& find /usr/local/src/elixir/ -type d -depth -empty -delete
# Thu, 09 Feb 2023 20:25:59 GMT
CMD ["iex"]
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
	-	`sha256:264a553bd76ff154c2183c5e58b9e1f9becaa09ffdafd4e5956e88a0e03e88fe`  
		Last Modified: Thu, 09 Feb 2023 15:15:57 GMT  
		Size: 231.2 MB (231218840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59bec584a9ed64bb7c6876f591390d58fac1005641d84eed8c0fccdbcbd563d0`  
		Last Modified: Thu, 09 Feb 2023 15:15:31 GMT  
		Size: 198.6 KB (198593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9b56e56f5cafa493d66867a1e6da0de0dcce8453cb55dd21614473973126fe6`  
		Last Modified: Thu, 09 Feb 2023 15:15:30 GMT  
		Size: 988.3 KB (988286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03766cfd76fa74d6a49e04b12c7be939f6bda8d1150c160073bb442e289b9299`  
		Last Modified: Thu, 09 Feb 2023 20:36:37 GMT  
		Size: 6.2 MB (6204625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
