## `elixir:otp-25-slim`

```console
$ docker pull elixir@sha256:d97a2579e51d2550e9c4d2b601ba725cb3dd07dbf9904d6023b92e08f5f514db
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `elixir:otp-25-slim` - linux; amd64

```console
$ docker pull elixir@sha256:407b7b291e698ea2aaa420834f03518630c3d44bdff7ee3ba24a440a41181ae1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.8 MB (127774331 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be45d34922e16934dd814daf79d4222149674a7fc9a425ef8d541eac5bfc8639`
-	Default Command: `["iex"]`

```dockerfile
# Mon, 12 Jun 2023 23:20:54 GMT
ADD file:e530b0563ea53d97b2f28e62149a665900196f86611df99a88c7a8ab2097b95d in / 
# Mon, 12 Jun 2023 23:20:54 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 04:30:00 GMT
ENV OTP_VERSION=25.3.2.2 REBAR3_VERSION=3.20.0
# Tue, 13 Jun 2023 04:30:00 GMT
LABEL org.opencontainers.image.version=25.3.2.2
# Tue, 13 Jun 2023 04:34:40 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="eeaa9e388fbfad90751fd75bf9207d87d7372b0a1a3266ff693c8015be91d634" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& REBAR3_DOWNLOAD_URL="https://github.com/erlang/rebar3/archive/${REBAR3_VERSION}.tar.gz" 	&& REBAR3_DOWNLOAD_SHA256="53ed7f294a8b8fb4d7d75988c69194943831c104d39832a1fa30307b1a8593de" 	&& mkdir -p /usr/src/rebar3-src 	&& curl -fSL -o rebar3-src.tar.gz "$REBAR3_DOWNLOAD_URL" 	&& echo "$REBAR3_DOWNLOAD_SHA256 rebar3-src.tar.gz" | sha256sum -c - 	&& tar -xzf rebar3-src.tar.gz -C /usr/src/rebar3-src --strip-components=1 	&& rm rebar3-src.tar.gz 	&& cd /usr/src/rebar3-src 	&& HOME=$PWD ./bootstrap 	&& install -v ./rebar3 /usr/local/bin/ 	&& rm -rf /usr/src/rebar3-src 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Tue, 13 Jun 2023 04:34:41 GMT
CMD ["erl"]
# Mon, 03 Jul 2023 17:26:34 GMT
ENV ELIXIR_VERSION=v1.15.1 LANG=C.UTF-8
# Mon, 03 Jul 2023 17:27:20 GMT
RUN set -xe 	&& ELIXIR_DOWNLOAD_URL="https://github.com/elixir-lang/elixir/archive/${ELIXIR_VERSION}.tar.gz" 	&& ELIXIR_DOWNLOAD_SHA256="cf89434f4cf7477b929c56e16ae22bf08e64101a144911d2834a2f3c9b3ae40f" 	&& buildDeps=' 		ca-certificates 		curl 		make 	' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $buildDeps 	&& curl -fSL -o elixir-src.tar.gz $ELIXIR_DOWNLOAD_URL 	&& echo "$ELIXIR_DOWNLOAD_SHA256  elixir-src.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/local/src/elixir 	&& tar -xzC /usr/local/src/elixir --strip-components=1 -f elixir-src.tar.gz 	&& rm elixir-src.tar.gz 	&& cd /usr/local/src/elixir 	&& make install clean 	&& find /usr/local/src/elixir/ -type f -not -regex "/usr/local/src/elixir/lib/[^\/]*/lib.*" -exec rm -rf {} + 	&& find /usr/local/src/elixir/ -type d -depth -empty -delete 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /var/lib/apt/lists/*
# Mon, 03 Jul 2023 17:27:20 GMT
CMD ["iex"]
```

-	Layers:
	-	`sha256:93c2d578e4211e82e47e7ada9ed05d1869a2362c6f7509f2ee8d91ccebfb7fbd`  
		Last Modified: Mon, 12 Jun 2023 23:26:08 GMT  
		Size: 55.1 MB (55055162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b4f26d8bbd0a4ecd1a223f6ec1946d67a141be17da0028a259e9f1881fcb90e`  
		Last Modified: Tue, 13 Jun 2023 05:48:53 GMT  
		Size: 65.8 MB (65824521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a7330afd9a638430a03a3fb01f816e2a4e70f4583920d5e143dda3186d0d509`  
		Last Modified: Mon, 03 Jul 2023 17:31:00 GMT  
		Size: 6.9 MB (6894648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `elixir:otp-25-slim` - linux; arm variant v7

```console
$ docker pull elixir@sha256:93b18a70190a854291108170adbde5931b117b42178b46676f7b9cfee4bc214f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.2 MB (114214781 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6f096bcf655c8d9ee54013ae2509d9c461fbdebf39f8f390dedff3c87646d34`
-	Default Command: `["iex"]`

```dockerfile
# Mon, 12 Jun 2023 23:58:34 GMT
ADD file:6edc8f94d2ebc83d6081e1c4567963d0060a842c767eaff959a6e5c6d09247b5 in / 
# Mon, 12 Jun 2023 23:58:34 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 16:03:43 GMT
ENV OTP_VERSION=25.3.2.2 REBAR3_VERSION=3.20.0
# Tue, 13 Jun 2023 16:03:44 GMT
LABEL org.opencontainers.image.version=25.3.2.2
# Tue, 13 Jun 2023 16:08:03 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="eeaa9e388fbfad90751fd75bf9207d87d7372b0a1a3266ff693c8015be91d634" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& REBAR3_DOWNLOAD_URL="https://github.com/erlang/rebar3/archive/${REBAR3_VERSION}.tar.gz" 	&& REBAR3_DOWNLOAD_SHA256="53ed7f294a8b8fb4d7d75988c69194943831c104d39832a1fa30307b1a8593de" 	&& mkdir -p /usr/src/rebar3-src 	&& curl -fSL -o rebar3-src.tar.gz "$REBAR3_DOWNLOAD_URL" 	&& echo "$REBAR3_DOWNLOAD_SHA256 rebar3-src.tar.gz" | sha256sum -c - 	&& tar -xzf rebar3-src.tar.gz -C /usr/src/rebar3-src --strip-components=1 	&& rm rebar3-src.tar.gz 	&& cd /usr/src/rebar3-src 	&& HOME=$PWD ./bootstrap 	&& install -v ./rebar3 /usr/local/bin/ 	&& rm -rf /usr/src/rebar3-src 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Tue, 13 Jun 2023 16:08:03 GMT
CMD ["erl"]
# Wed, 21 Jun 2023 00:04:35 GMT
ENV ELIXIR_VERSION=v1.15.0 LANG=C.UTF-8
# Wed, 21 Jun 2023 00:05:27 GMT
RUN set -xe 	&& ELIXIR_DOWNLOAD_URL="https://github.com/elixir-lang/elixir/archive/${ELIXIR_VERSION}.tar.gz" 	&& ELIXIR_DOWNLOAD_SHA256="0f4df7574a5f300b5c66f54906222cd46dac0df7233ded165bc8e80fd9ffeb7a" 	&& buildDeps=' 		ca-certificates 		curl 		make 	' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $buildDeps 	&& curl -fSL -o elixir-src.tar.gz $ELIXIR_DOWNLOAD_URL 	&& echo "$ELIXIR_DOWNLOAD_SHA256  elixir-src.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/local/src/elixir 	&& tar -xzC /usr/local/src/elixir --strip-components=1 -f elixir-src.tar.gz 	&& rm elixir-src.tar.gz 	&& cd /usr/local/src/elixir 	&& make install clean 	&& find /usr/local/src/elixir/ -type f -not -regex "/usr/local/src/elixir/lib/[^\/]*/lib.*" -exec rm -rf {} + 	&& find /usr/local/src/elixir/ -type d -depth -empty -delete 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 21 Jun 2023 00:05:27 GMT
CMD ["iex"]
```

-	Layers:
	-	`sha256:23807bbf2a5fd14b7975a9e82f4a5530bbba520f31b382cc4b4ce2e77e075ace`  
		Last Modified: Tue, 13 Jun 2023 00:04:02 GMT  
		Size: 50.2 MB (50218141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a1a31fe817ec99a7afad65092fd52ae097e820d04fd07f0e641974e5d2e7fe0`  
		Last Modified: Tue, 13 Jun 2023 17:03:56 GMT  
		Size: 57.1 MB (57105375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb69472960a3fba769b0dc75f0606ef0e42b7abd82359e1f75d5927475d760d0`  
		Last Modified: Wed, 21 Jun 2023 00:08:42 GMT  
		Size: 6.9 MB (6891265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `elixir:otp-25-slim` - linux; arm64 variant v8

```console
$ docker pull elixir@sha256:c1a513fa3141ae3d92aa7b5e4242d46ce6477541b3e34df883ae204e8271aed6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.8 MB (124803769 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23f41bc71143566f57afb0d6027a235a3b13dee771a71b1129ded5ad3a680e65`
-	Default Command: `["iex"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:22 GMT
ADD file:caddd2f40296ec5c1bf7487617ca8694cfff9a1d9b7484159e203b6514cb5f5f in / 
# Mon, 12 Jun 2023 23:40:23 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 03:30:30 GMT
ENV OTP_VERSION=25.3.2.2 REBAR3_VERSION=3.20.0
# Tue, 13 Jun 2023 03:30:31 GMT
LABEL org.opencontainers.image.version=25.3.2.2
# Tue, 13 Jun 2023 03:33:37 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="eeaa9e388fbfad90751fd75bf9207d87d7372b0a1a3266ff693c8015be91d634" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& REBAR3_DOWNLOAD_URL="https://github.com/erlang/rebar3/archive/${REBAR3_VERSION}.tar.gz" 	&& REBAR3_DOWNLOAD_SHA256="53ed7f294a8b8fb4d7d75988c69194943831c104d39832a1fa30307b1a8593de" 	&& mkdir -p /usr/src/rebar3-src 	&& curl -fSL -o rebar3-src.tar.gz "$REBAR3_DOWNLOAD_URL" 	&& echo "$REBAR3_DOWNLOAD_SHA256 rebar3-src.tar.gz" | sha256sum -c - 	&& tar -xzf rebar3-src.tar.gz -C /usr/src/rebar3-src --strip-components=1 	&& rm rebar3-src.tar.gz 	&& cd /usr/src/rebar3-src 	&& HOME=$PWD ./bootstrap 	&& install -v ./rebar3 /usr/local/bin/ 	&& rm -rf /usr/src/rebar3-src 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Tue, 13 Jun 2023 03:33:38 GMT
CMD ["erl"]
# Mon, 03 Jul 2023 17:44:38 GMT
ENV ELIXIR_VERSION=v1.15.1 LANG=C.UTF-8
# Mon, 03 Jul 2023 17:45:11 GMT
RUN set -xe 	&& ELIXIR_DOWNLOAD_URL="https://github.com/elixir-lang/elixir/archive/${ELIXIR_VERSION}.tar.gz" 	&& ELIXIR_DOWNLOAD_SHA256="cf89434f4cf7477b929c56e16ae22bf08e64101a144911d2834a2f3c9b3ae40f" 	&& buildDeps=' 		ca-certificates 		curl 		make 	' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $buildDeps 	&& curl -fSL -o elixir-src.tar.gz $ELIXIR_DOWNLOAD_URL 	&& echo "$ELIXIR_DOWNLOAD_SHA256  elixir-src.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/local/src/elixir 	&& tar -xzC /usr/local/src/elixir --strip-components=1 -f elixir-src.tar.gz 	&& rm elixir-src.tar.gz 	&& cd /usr/local/src/elixir 	&& make install clean 	&& find /usr/local/src/elixir/ -type f -not -regex "/usr/local/src/elixir/lib/[^\/]*/lib.*" -exec rm -rf {} + 	&& find /usr/local/src/elixir/ -type d -depth -empty -delete 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /var/lib/apt/lists/*
# Mon, 03 Jul 2023 17:45:12 GMT
CMD ["iex"]
```

-	Layers:
	-	`sha256:663ccfaf62a5d7b997bca03d1dc6d5dfff01b9e0de08d86dbea8957ea92d7d16`  
		Last Modified: Mon, 12 Jun 2023 23:44:25 GMT  
		Size: 53.7 MB (53704136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2972e0f89026f9c076b49c0b662bcbc26731b86de99e654c4556031c78e2b9a`  
		Last Modified: Tue, 13 Jun 2023 04:18:39 GMT  
		Size: 64.2 MB (64205175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03521092f8772456c5f0806102fdf559e3d65b50cb0529d511f535835dc04274`  
		Last Modified: Mon, 03 Jul 2023 17:48:28 GMT  
		Size: 6.9 MB (6894458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `elixir:otp-25-slim` - linux; 386

```console
$ docker pull elixir@sha256:77fe1c99cc3107c4568f6a5a5ecf2405d9a24fa8dd518aa6f54ba265c5cee083
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.4 MB (120429495 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe248e60afd3fbb44773c89a314a0d1745761043c57dd370548287872a8ea3d9`
-	Default Command: `["iex"]`

```dockerfile
# Mon, 12 Jun 2023 23:39:39 GMT
ADD file:4b1f447e0b75fbe493bd68bb77b74f4ba1c61ac8e14226e3c511b3a1c3d5721a in / 
# Mon, 12 Jun 2023 23:39:40 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 01:53:49 GMT
ENV OTP_VERSION=25.3.2.2 REBAR3_VERSION=3.20.0
# Tue, 13 Jun 2023 01:53:49 GMT
LABEL org.opencontainers.image.version=25.3.2.2
# Tue, 13 Jun 2023 02:01:48 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="eeaa9e388fbfad90751fd75bf9207d87d7372b0a1a3266ff693c8015be91d634" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& REBAR3_DOWNLOAD_URL="https://github.com/erlang/rebar3/archive/${REBAR3_VERSION}.tar.gz" 	&& REBAR3_DOWNLOAD_SHA256="53ed7f294a8b8fb4d7d75988c69194943831c104d39832a1fa30307b1a8593de" 	&& mkdir -p /usr/src/rebar3-src 	&& curl -fSL -o rebar3-src.tar.gz "$REBAR3_DOWNLOAD_URL" 	&& echo "$REBAR3_DOWNLOAD_SHA256 rebar3-src.tar.gz" | sha256sum -c - 	&& tar -xzf rebar3-src.tar.gz -C /usr/src/rebar3-src --strip-components=1 	&& rm rebar3-src.tar.gz 	&& cd /usr/src/rebar3-src 	&& HOME=$PWD ./bootstrap 	&& install -v ./rebar3 /usr/local/bin/ 	&& rm -rf /usr/src/rebar3-src 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Tue, 13 Jun 2023 02:01:49 GMT
CMD ["erl"]
# Tue, 20 Jun 2023 23:48:45 GMT
ENV ELIXIR_VERSION=v1.15.0 LANG=C.UTF-8
# Tue, 20 Jun 2023 23:49:55 GMT
RUN set -xe 	&& ELIXIR_DOWNLOAD_URL="https://github.com/elixir-lang/elixir/archive/${ELIXIR_VERSION}.tar.gz" 	&& ELIXIR_DOWNLOAD_SHA256="0f4df7574a5f300b5c66f54906222cd46dac0df7233ded165bc8e80fd9ffeb7a" 	&& buildDeps=' 		ca-certificates 		curl 		make 	' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $buildDeps 	&& curl -fSL -o elixir-src.tar.gz $ELIXIR_DOWNLOAD_URL 	&& echo "$ELIXIR_DOWNLOAD_SHA256  elixir-src.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/local/src/elixir 	&& tar -xzC /usr/local/src/elixir --strip-components=1 -f elixir-src.tar.gz 	&& rm elixir-src.tar.gz 	&& cd /usr/local/src/elixir 	&& make install clean 	&& find /usr/local/src/elixir/ -type f -not -regex "/usr/local/src/elixir/lib/[^\/]*/lib.*" -exec rm -rf {} + 	&& find /usr/local/src/elixir/ -type d -depth -empty -delete 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 20 Jun 2023 23:49:55 GMT
CMD ["iex"]
```

-	Layers:
	-	`sha256:0997ae72d27731326552ad4699d630b4932f3d31abc07a62105a0eb16b54173a`  
		Last Modified: Mon, 12 Jun 2023 23:46:43 GMT  
		Size: 56.0 MB (56040665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81b3154ca85ac953e4e58262f5581a82a007ddabd07121edfcc58d26ddbb9c2d`  
		Last Modified: Tue, 13 Jun 2023 04:08:26 GMT  
		Size: 57.5 MB (57497403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5198213ae3aae5bb87d415eecc2ee572959871d7c96718e4626d92138a55a203`  
		Last Modified: Tue, 20 Jun 2023 23:53:13 GMT  
		Size: 6.9 MB (6891427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `elixir:otp-25-slim` - linux; ppc64le

```console
$ docker pull elixir@sha256:d688845538c94b8a170606b1397d1fb57e1c5bf41ec2daa139b116c49ad6ea3c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.3 MB (124274255 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0471dd4d804520ba3466c28a2882b4c8967a37f4f75a2274c833f6e6c9e106a`
-	Default Command: `["iex"]`

```dockerfile
# Mon, 12 Jun 2023 23:17:54 GMT
ADD file:93fa83ca9c503a09001edab8e277ae6c67636f805f8bb49986e0ed2ad3ea8360 in / 
# Mon, 12 Jun 2023 23:17:57 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 08:16:30 GMT
ENV OTP_VERSION=25.3.2.2 REBAR3_VERSION=3.20.0
# Tue, 13 Jun 2023 08:16:31 GMT
LABEL org.opencontainers.image.version=25.3.2.2
# Tue, 13 Jun 2023 08:23:49 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="eeaa9e388fbfad90751fd75bf9207d87d7372b0a1a3266ff693c8015be91d634" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& REBAR3_DOWNLOAD_URL="https://github.com/erlang/rebar3/archive/${REBAR3_VERSION}.tar.gz" 	&& REBAR3_DOWNLOAD_SHA256="53ed7f294a8b8fb4d7d75988c69194943831c104d39832a1fa30307b1a8593de" 	&& mkdir -p /usr/src/rebar3-src 	&& curl -fSL -o rebar3-src.tar.gz "$REBAR3_DOWNLOAD_URL" 	&& echo "$REBAR3_DOWNLOAD_SHA256 rebar3-src.tar.gz" | sha256sum -c - 	&& tar -xzf rebar3-src.tar.gz -C /usr/src/rebar3-src --strip-components=1 	&& rm rebar3-src.tar.gz 	&& cd /usr/src/rebar3-src 	&& HOME=$PWD ./bootstrap 	&& install -v ./rebar3 /usr/local/bin/ 	&& rm -rf /usr/src/rebar3-src 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Tue, 13 Jun 2023 08:23:52 GMT
CMD ["erl"]
# Mon, 03 Jul 2023 17:35:51 GMT
ENV ELIXIR_VERSION=v1.15.1 LANG=C.UTF-8
# Mon, 03 Jul 2023 17:38:03 GMT
RUN set -xe 	&& ELIXIR_DOWNLOAD_URL="https://github.com/elixir-lang/elixir/archive/${ELIXIR_VERSION}.tar.gz" 	&& ELIXIR_DOWNLOAD_SHA256="cf89434f4cf7477b929c56e16ae22bf08e64101a144911d2834a2f3c9b3ae40f" 	&& buildDeps=' 		ca-certificates 		curl 		make 	' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $buildDeps 	&& curl -fSL -o elixir-src.tar.gz $ELIXIR_DOWNLOAD_URL 	&& echo "$ELIXIR_DOWNLOAD_SHA256  elixir-src.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/local/src/elixir 	&& tar -xzC /usr/local/src/elixir --strip-components=1 -f elixir-src.tar.gz 	&& rm elixir-src.tar.gz 	&& cd /usr/local/src/elixir 	&& make install clean 	&& find /usr/local/src/elixir/ -type f -not -regex "/usr/local/src/elixir/lib/[^\/]*/lib.*" -exec rm -rf {} + 	&& find /usr/local/src/elixir/ -type d -depth -empty -delete 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /var/lib/apt/lists/*
# Mon, 03 Jul 2023 17:38:04 GMT
CMD ["iex"]
```

-	Layers:
	-	`sha256:ebc829b9a845100e0e82d2b659a5cd374121460e523a23fa55a97ac0ddb14460`  
		Last Modified: Mon, 12 Jun 2023 23:24:35 GMT  
		Size: 58.9 MB (58927438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24d6451c6425afb753e732228730706c3eb15a40849010df4c4b35528d3f3423`  
		Last Modified: Tue, 13 Jun 2023 08:44:42 GMT  
		Size: 58.5 MB (58451978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f99285a69e4f72eea1f64869a1c1f030e3fcdf690f8ef5a3bf00161552872766`  
		Last Modified: Mon, 03 Jul 2023 17:42:31 GMT  
		Size: 6.9 MB (6894839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `elixir:otp-25-slim` - linux; s390x

```console
$ docker pull elixir@sha256:2aacaf76032795906ca3c646b4efa88d6d29532dd70fb82b746de4764dd81c88
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.2 MB (118211560 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0431f6edac7997b26c9920e034718cc3059d1d59027e1d01eac4580bc58628eb`
-	Default Command: `["iex"]`

```dockerfile
# Tue, 13 Jun 2023 04:29:54 GMT
ADD file:fa60f19da2df43542549a5dd89b364d30fff981d1655f9cce8900778a7b841b9 in / 
# Tue, 13 Jun 2023 04:29:57 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 19:11:56 GMT
ENV OTP_VERSION=25.3.2.2 REBAR3_VERSION=3.20.0
# Tue, 13 Jun 2023 19:11:56 GMT
LABEL org.opencontainers.image.version=25.3.2.2
# Tue, 13 Jun 2023 19:16:14 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="eeaa9e388fbfad90751fd75bf9207d87d7372b0a1a3266ff693c8015be91d634" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& REBAR3_DOWNLOAD_URL="https://github.com/erlang/rebar3/archive/${REBAR3_VERSION}.tar.gz" 	&& REBAR3_DOWNLOAD_SHA256="53ed7f294a8b8fb4d7d75988c69194943831c104d39832a1fa30307b1a8593de" 	&& mkdir -p /usr/src/rebar3-src 	&& curl -fSL -o rebar3-src.tar.gz "$REBAR3_DOWNLOAD_URL" 	&& echo "$REBAR3_DOWNLOAD_SHA256 rebar3-src.tar.gz" | sha256sum -c - 	&& tar -xzf rebar3-src.tar.gz -C /usr/src/rebar3-src --strip-components=1 	&& rm rebar3-src.tar.gz 	&& cd /usr/src/rebar3-src 	&& HOME=$PWD ./bootstrap 	&& install -v ./rebar3 /usr/local/bin/ 	&& rm -rf /usr/src/rebar3-src 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Tue, 13 Jun 2023 19:16:17 GMT
CMD ["erl"]
# Tue, 20 Jun 2023 23:49:00 GMT
ENV ELIXIR_VERSION=v1.15.0 LANG=C.UTF-8
# Tue, 20 Jun 2023 23:49:47 GMT
RUN set -xe 	&& ELIXIR_DOWNLOAD_URL="https://github.com/elixir-lang/elixir/archive/${ELIXIR_VERSION}.tar.gz" 	&& ELIXIR_DOWNLOAD_SHA256="0f4df7574a5f300b5c66f54906222cd46dac0df7233ded165bc8e80fd9ffeb7a" 	&& buildDeps=' 		ca-certificates 		curl 		make 	' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $buildDeps 	&& curl -fSL -o elixir-src.tar.gz $ELIXIR_DOWNLOAD_URL 	&& echo "$ELIXIR_DOWNLOAD_SHA256  elixir-src.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/local/src/elixir 	&& tar -xzC /usr/local/src/elixir --strip-components=1 -f elixir-src.tar.gz 	&& rm elixir-src.tar.gz 	&& cd /usr/local/src/elixir 	&& make install clean 	&& find /usr/local/src/elixir/ -type f -not -regex "/usr/local/src/elixir/lib/[^\/]*/lib.*" -exec rm -rf {} + 	&& find /usr/local/src/elixir/ -type d -depth -empty -delete 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 20 Jun 2023 23:49:47 GMT
CMD ["iex"]
```

-	Layers:
	-	`sha256:2bef9d7959742dda03e39c77232808f6559cd696f21fab76fc714bdd24cae18d`  
		Last Modified: Tue, 13 Jun 2023 04:34:33 GMT  
		Size: 53.3 MB (53288042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1836f49908b05144595b7535f2ea2ab1b66d810d7cbbb3ce6f8b75ec758eceb5`  
		Last Modified: Tue, 13 Jun 2023 19:29:43 GMT  
		Size: 58.0 MB (58032102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:699c042597d131ff1d94a931db73b5e91141aab46c2a843e84ed57fe4767ef9b`  
		Last Modified: Tue, 20 Jun 2023 23:53:22 GMT  
		Size: 6.9 MB (6891416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
