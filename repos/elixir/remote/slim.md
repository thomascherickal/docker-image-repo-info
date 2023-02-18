## `elixir:slim`

```console
$ docker pull elixir@sha256:187e1ea2d033c635acdf365d1eb2955d48b01a2a7018fabb705da146bba0e225
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `elixir:slim` - linux; amd64

```console
$ docker pull elixir@sha256:b8521c156b7d5a60b88c5fb0c4281741874b606789188e5e57132d3bdfe0ec36
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.7 MB (127669400 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ea919861d6dfcf2dc181c56053dd3863d37455a7e7849ab285ce568ce7fe76a`
-	Default Command: `["iex"]`

```dockerfile
# Thu, 09 Feb 2023 03:20:05 GMT
ADD file:b03d13d345c29f69557f410c8504e748226756d1f48e5abdb63cd40179b2640c in / 
# Thu, 09 Feb 2023 03:20:05 GMT
CMD ["bash"]
# Fri, 17 Feb 2023 20:50:18 GMT
ENV OTP_VERSION=25.2.3 REBAR3_VERSION=3.19.0
# Fri, 17 Feb 2023 20:50:18 GMT
LABEL org.opencontainers.image.version=25.2.3
# Fri, 17 Feb 2023 20:54:56 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="637bc5cf68dd229fd3c3fe889a6f84dd32c4a827488550a0a98123b00c2d78b5" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& REBAR3_DOWNLOAD_URL="https://github.com/erlang/rebar3/archive/${REBAR3_VERSION}.tar.gz" 	&& REBAR3_DOWNLOAD_SHA256="ff9ef42c737480477ebdf0dd9d95ece534a14c96f05edafbf32e9af973280bc3" 	&& mkdir -p /usr/src/rebar3-src 	&& curl -fSL -o rebar3-src.tar.gz "$REBAR3_DOWNLOAD_URL" 	&& echo "$REBAR3_DOWNLOAD_SHA256 rebar3-src.tar.gz" | sha256sum -c - 	&& tar -xzf rebar3-src.tar.gz -C /usr/src/rebar3-src --strip-components=1 	&& rm rebar3-src.tar.gz 	&& cd /usr/src/rebar3-src 	&& HOME=$PWD ./bootstrap 	&& install -v ./rebar3 /usr/local/bin/ 	&& rm -rf /usr/src/rebar3-src 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Fri, 17 Feb 2023 20:54:57 GMT
CMD ["erl"]
# Fri, 17 Feb 2023 21:21:27 GMT
ENV ELIXIR_VERSION=v1.14.3 LANG=C.UTF-8
# Fri, 17 Feb 2023 21:22:13 GMT
RUN set -xe 	&& ELIXIR_DOWNLOAD_URL="https://github.com/elixir-lang/elixir/archive/${ELIXIR_VERSION}.tar.gz" 	&& ELIXIR_DOWNLOAD_SHA256="bd464145257f36bd64f7ba8bed93b6499c50571b415c491b20267d27d7035707" 	&& buildDeps=' 		ca-certificates 		curl 		make 	' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $buildDeps 	&& curl -fSL -o elixir-src.tar.gz $ELIXIR_DOWNLOAD_URL 	&& echo "$ELIXIR_DOWNLOAD_SHA256  elixir-src.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/local/src/elixir 	&& tar -xzC /usr/local/src/elixir --strip-components=1 -f elixir-src.tar.gz 	&& rm elixir-src.tar.gz 	&& cd /usr/local/src/elixir 	&& make install clean 	&& find /usr/local/src/elixir/ -type f -not -regex "/usr/local/src/elixir/lib/[^\/]*/lib.*" -exec rm -rf {} + 	&& find /usr/local/src/elixir/ -type d -depth -empty -delete 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 17 Feb 2023 21:22:13 GMT
CMD ["iex"]
```

-	Layers:
	-	`sha256:1e4aec178e0864db93a6f97a20bde3445871a4562c1801185eca1238d3a0e80d`  
		Last Modified: Thu, 09 Feb 2023 03:24:47 GMT  
		Size: 55.0 MB (55046771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a30ee0533ebb8f6351c31e27ec7812c42832ce3c96be2f5bf3d52caeba71bee4`  
		Last Modified: Fri, 17 Feb 2023 21:04:09 GMT  
		Size: 65.9 MB (65927359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0da83fefe84db886aa2e5b8e3c614709fc50bc3eab940dd0101bfa749572e790`  
		Last Modified: Fri, 17 Feb 2023 21:27:42 GMT  
		Size: 6.7 MB (6695270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `elixir:slim` - linux; arm variant v7

```console
$ docker pull elixir@sha256:d1d9578bd6cb2c06cd84e3f8f1fd74205a1e886c9e0a7d467cd07b2bf135b503
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.1 MB (114148425 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97dd6be7d63b22a6e2efd0d28426ee0513bedcdf41c4b50ff0d8cce9df7dcfda`
-	Default Command: `["iex"]`

```dockerfile
# Thu, 09 Feb 2023 06:11:50 GMT
ADD file:dec7deb02352cdd1425e3138d7352582848ea2b4bb65c69ea313e52e02e33f1b in / 
# Thu, 09 Feb 2023 06:11:51 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 06:56:33 GMT
ENV OTP_VERSION=25.2.2 REBAR3_VERSION=3.19.0
# Thu, 09 Feb 2023 06:56:33 GMT
LABEL org.opencontainers.image.version=25.2.2
# Thu, 09 Feb 2023 07:00:48 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="535e535b2e90e71deca96c53f19710e6ebf3d4289b0a3116e7cf83b7e2c4bb7e" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& REBAR3_DOWNLOAD_URL="https://github.com/erlang/rebar3/archive/${REBAR3_VERSION}.tar.gz" 	&& REBAR3_DOWNLOAD_SHA256="ff9ef42c737480477ebdf0dd9d95ece534a14c96f05edafbf32e9af973280bc3" 	&& mkdir -p /usr/src/rebar3-src 	&& curl -fSL -o rebar3-src.tar.gz "$REBAR3_DOWNLOAD_URL" 	&& echo "$REBAR3_DOWNLOAD_SHA256 rebar3-src.tar.gz" | sha256sum -c - 	&& tar -xzf rebar3-src.tar.gz -C /usr/src/rebar3-src --strip-components=1 	&& rm rebar3-src.tar.gz 	&& cd /usr/src/rebar3-src 	&& HOME=$PWD ./bootstrap 	&& install -v ./rebar3 /usr/local/bin/ 	&& rm -rf /usr/src/rebar3-src 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Thu, 09 Feb 2023 07:00:48 GMT
CMD ["erl"]
# Thu, 09 Feb 2023 17:53:03 GMT
ENV ELIXIR_VERSION=v1.14.3 LANG=C.UTF-8
# Thu, 09 Feb 2023 17:54:00 GMT
RUN set -xe 	&& ELIXIR_DOWNLOAD_URL="https://github.com/elixir-lang/elixir/archive/${ELIXIR_VERSION}.tar.gz" 	&& ELIXIR_DOWNLOAD_SHA256="bd464145257f36bd64f7ba8bed93b6499c50571b415c491b20267d27d7035707" 	&& buildDeps=' 		ca-certificates 		curl 		make 	' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $buildDeps 	&& curl -fSL -o elixir-src.tar.gz $ELIXIR_DOWNLOAD_URL 	&& echo "$ELIXIR_DOWNLOAD_SHA256  elixir-src.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/local/src/elixir 	&& tar -xzC /usr/local/src/elixir --strip-components=1 -f elixir-src.tar.gz 	&& rm elixir-src.tar.gz 	&& cd /usr/local/src/elixir 	&& make install clean 	&& find /usr/local/src/elixir/ -type f -not -regex "/usr/local/src/elixir/lib/[^\/]*/lib.*" -exec rm -rf {} + 	&& find /usr/local/src/elixir/ -type d -depth -empty -delete 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 17:54:00 GMT
CMD ["iex"]
```

-	Layers:
	-	`sha256:7c2a4bcf178ec94fc012530fd1bfd4b70c9838e2776f9790691fce0d2dac0ff1`  
		Last Modified: Thu, 09 Feb 2023 06:18:48 GMT  
		Size: 50.2 MB (50213699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8a3c36f130b6faab1c81ee7116c5c880ab438ed4ba67f5ada43180a83e3690a`  
		Last Modified: Thu, 09 Feb 2023 07:32:02 GMT  
		Size: 57.2 MB (57239955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a60399fb269bafd32854872845a09f1a30eef1f90fe86f1a0833a439797c854e`  
		Last Modified: Thu, 09 Feb 2023 18:09:37 GMT  
		Size: 6.7 MB (6694771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `elixir:slim` - linux; arm64 variant v8

```console
$ docker pull elixir@sha256:b224dcff0be42a53581355722cd8da9cfd230072a9f34788055ea1aeff2e9d18
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.7 MB (124716900 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22c2932ece299db0c2104907985263d10e7c5a011898bc2e02e7fd2b31ab8432`
-	Default Command: `["iex"]`

```dockerfile
# Thu, 09 Feb 2023 03:58:29 GMT
ADD file:5cf2de182dac36d99ec41918889c9755f9c49c56fa0a8d0ca14040c1d8c04541 in / 
# Thu, 09 Feb 2023 03:58:30 GMT
CMD ["bash"]
# Fri, 17 Feb 2023 22:51:53 GMT
ENV OTP_VERSION=25.2.3 REBAR3_VERSION=3.19.0
# Fri, 17 Feb 2023 22:51:53 GMT
LABEL org.opencontainers.image.version=25.2.3
# Fri, 17 Feb 2023 22:55:01 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="637bc5cf68dd229fd3c3fe889a6f84dd32c4a827488550a0a98123b00c2d78b5" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& REBAR3_DOWNLOAD_URL="https://github.com/erlang/rebar3/archive/${REBAR3_VERSION}.tar.gz" 	&& REBAR3_DOWNLOAD_SHA256="ff9ef42c737480477ebdf0dd9d95ece534a14c96f05edafbf32e9af973280bc3" 	&& mkdir -p /usr/src/rebar3-src 	&& curl -fSL -o rebar3-src.tar.gz "$REBAR3_DOWNLOAD_URL" 	&& echo "$REBAR3_DOWNLOAD_SHA256 rebar3-src.tar.gz" | sha256sum -c - 	&& tar -xzf rebar3-src.tar.gz -C /usr/src/rebar3-src --strip-components=1 	&& rm rebar3-src.tar.gz 	&& cd /usr/src/rebar3-src 	&& HOME=$PWD ./bootstrap 	&& install -v ./rebar3 /usr/local/bin/ 	&& rm -rf /usr/src/rebar3-src 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Fri, 17 Feb 2023 22:55:02 GMT
CMD ["erl"]
# Fri, 17 Feb 2023 23:22:47 GMT
ENV ELIXIR_VERSION=v1.14.3 LANG=C.UTF-8
# Fri, 17 Feb 2023 23:23:21 GMT
RUN set -xe 	&& ELIXIR_DOWNLOAD_URL="https://github.com/elixir-lang/elixir/archive/${ELIXIR_VERSION}.tar.gz" 	&& ELIXIR_DOWNLOAD_SHA256="bd464145257f36bd64f7ba8bed93b6499c50571b415c491b20267d27d7035707" 	&& buildDeps=' 		ca-certificates 		curl 		make 	' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $buildDeps 	&& curl -fSL -o elixir-src.tar.gz $ELIXIR_DOWNLOAD_URL 	&& echo "$ELIXIR_DOWNLOAD_SHA256  elixir-src.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/local/src/elixir 	&& tar -xzC /usr/local/src/elixir --strip-components=1 -f elixir-src.tar.gz 	&& rm elixir-src.tar.gz 	&& cd /usr/local/src/elixir 	&& make install clean 	&& find /usr/local/src/elixir/ -type f -not -regex "/usr/local/src/elixir/lib/[^\/]*/lib.*" -exec rm -rf {} + 	&& find /usr/local/src/elixir/ -type d -depth -empty -delete 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 17 Feb 2023 23:23:21 GMT
CMD ["iex"]
```

-	Layers:
	-	`sha256:80dae1b9d879348c210c40024c6e90ef92677ac3515456375fcbb70bdf07b104`  
		Last Modified: Thu, 09 Feb 2023 04:02:11 GMT  
		Size: 53.7 MB (53703368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51ae53aa8c9762c8d2aaf060864a7100b2d3874620078e863dfbd9b452675bc4`  
		Last Modified: Fri, 17 Feb 2023 23:02:49 GMT  
		Size: 64.3 MB (64318472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4397f5d4ac246c52effb58185fd2a092c56162c611bc168a7f8ac26eed56ccff`  
		Last Modified: Fri, 17 Feb 2023 23:27:58 GMT  
		Size: 6.7 MB (6695060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `elixir:slim` - linux; 386

```console
$ docker pull elixir@sha256:61864890f2fb011683715264af694cb7108d1d99a2fad9ec4abe7fd835c32585
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.4 MB (120369201 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28ca00082ac997aba7218ebf7b85e6acb565c8025eef24055799caa540a6b77b`
-	Default Command: `["iex"]`

```dockerfile
# Thu, 09 Feb 2023 05:12:37 GMT
ADD file:feaff299d3310c04952143a422f0d0bdd292cd174513c54b1f50765cdbcfd401 in / 
# Thu, 09 Feb 2023 05:12:38 GMT
CMD ["bash"]
# Fri, 17 Feb 2023 21:10:11 GMT
ENV OTP_VERSION=25.2.3 REBAR3_VERSION=3.19.0
# Fri, 17 Feb 2023 21:10:11 GMT
LABEL org.opencontainers.image.version=25.2.3
# Fri, 17 Feb 2023 21:15:09 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="637bc5cf68dd229fd3c3fe889a6f84dd32c4a827488550a0a98123b00c2d78b5" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& REBAR3_DOWNLOAD_URL="https://github.com/erlang/rebar3/archive/${REBAR3_VERSION}.tar.gz" 	&& REBAR3_DOWNLOAD_SHA256="ff9ef42c737480477ebdf0dd9d95ece534a14c96f05edafbf32e9af973280bc3" 	&& mkdir -p /usr/src/rebar3-src 	&& curl -fSL -o rebar3-src.tar.gz "$REBAR3_DOWNLOAD_URL" 	&& echo "$REBAR3_DOWNLOAD_SHA256 rebar3-src.tar.gz" | sha256sum -c - 	&& tar -xzf rebar3-src.tar.gz -C /usr/src/rebar3-src --strip-components=1 	&& rm rebar3-src.tar.gz 	&& cd /usr/src/rebar3-src 	&& HOME=$PWD ./bootstrap 	&& install -v ./rebar3 /usr/local/bin/ 	&& rm -rf /usr/src/rebar3-src 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Fri, 17 Feb 2023 21:15:09 GMT
CMD ["erl"]
# Fri, 17 Feb 2023 21:44:59 GMT
ENV ELIXIR_VERSION=v1.14.3 LANG=C.UTF-8
# Fri, 17 Feb 2023 21:46:06 GMT
RUN set -xe 	&& ELIXIR_DOWNLOAD_URL="https://github.com/elixir-lang/elixir/archive/${ELIXIR_VERSION}.tar.gz" 	&& ELIXIR_DOWNLOAD_SHA256="bd464145257f36bd64f7ba8bed93b6499c50571b415c491b20267d27d7035707" 	&& buildDeps=' 		ca-certificates 		curl 		make 	' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $buildDeps 	&& curl -fSL -o elixir-src.tar.gz $ELIXIR_DOWNLOAD_URL 	&& echo "$ELIXIR_DOWNLOAD_SHA256  elixir-src.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/local/src/elixir 	&& tar -xzC /usr/local/src/elixir --strip-components=1 -f elixir-src.tar.gz 	&& rm elixir-src.tar.gz 	&& cd /usr/local/src/elixir 	&& make install clean 	&& find /usr/local/src/elixir/ -type f -not -regex "/usr/local/src/elixir/lib/[^\/]*/lib.*" -exec rm -rf {} + 	&& find /usr/local/src/elixir/ -type d -depth -empty -delete 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 17 Feb 2023 21:46:07 GMT
CMD ["iex"]
```

-	Layers:
	-	`sha256:9708eacca143ba8fa6c7e9a5b05456412b7b16629c20015a43f3ca391e066162`  
		Last Modified: Thu, 09 Feb 2023 05:18:13 GMT  
		Size: 56.0 MB (56030197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea84556f3c18b9b5bd9d3949282d5885425f0da25053b47a2f729350c5934c22`  
		Last Modified: Fri, 17 Feb 2023 21:26:44 GMT  
		Size: 57.6 MB (57644612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d912c473bbf2c3e2a1f20a767531c05b42fd9704dae9e3c55a5a6217baca087`  
		Last Modified: Fri, 17 Feb 2023 21:55:35 GMT  
		Size: 6.7 MB (6694392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `elixir:slim` - linux; ppc64le

```console
$ docker pull elixir@sha256:c1cfecc1e5dd622bc4d4328c282da455da14355e22e8de332fcfe0c1f8a8d00c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.2 MB (124195958 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04089d8b89446976fb29939e64b299324b42aaee5b6f50899d0ea5becb9e2fee`
-	Default Command: `["iex"]`

```dockerfile
# Thu, 09 Feb 2023 06:21:21 GMT
ADD file:0cbfdb018ccae985f6d364f1de7d39fa004cbc966374ba83727c34aa39f946d4 in / 
# Thu, 09 Feb 2023 06:21:24 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 06:44:40 GMT
ENV OTP_VERSION=25.2.2 REBAR3_VERSION=3.19.0
# Thu, 09 Feb 2023 06:44:40 GMT
LABEL org.opencontainers.image.version=25.2.2
# Thu, 09 Feb 2023 06:52:09 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="535e535b2e90e71deca96c53f19710e6ebf3d4289b0a3116e7cf83b7e2c4bb7e" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& REBAR3_DOWNLOAD_URL="https://github.com/erlang/rebar3/archive/${REBAR3_VERSION}.tar.gz" 	&& REBAR3_DOWNLOAD_SHA256="ff9ef42c737480477ebdf0dd9d95ece534a14c96f05edafbf32e9af973280bc3" 	&& mkdir -p /usr/src/rebar3-src 	&& curl -fSL -o rebar3-src.tar.gz "$REBAR3_DOWNLOAD_URL" 	&& echo "$REBAR3_DOWNLOAD_SHA256 rebar3-src.tar.gz" | sha256sum -c - 	&& tar -xzf rebar3-src.tar.gz -C /usr/src/rebar3-src --strip-components=1 	&& rm rebar3-src.tar.gz 	&& cd /usr/src/rebar3-src 	&& HOME=$PWD ./bootstrap 	&& install -v ./rebar3 /usr/local/bin/ 	&& rm -rf /usr/src/rebar3-src 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Thu, 09 Feb 2023 06:52:11 GMT
CMD ["erl"]
# Thu, 09 Feb 2023 15:33:30 GMT
ENV ELIXIR_VERSION=v1.14.3 LANG=C.UTF-8
# Thu, 09 Feb 2023 15:35:25 GMT
RUN set -xe 	&& ELIXIR_DOWNLOAD_URL="https://github.com/elixir-lang/elixir/archive/${ELIXIR_VERSION}.tar.gz" 	&& ELIXIR_DOWNLOAD_SHA256="bd464145257f36bd64f7ba8bed93b6499c50571b415c491b20267d27d7035707" 	&& buildDeps=' 		ca-certificates 		curl 		make 	' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $buildDeps 	&& curl -fSL -o elixir-src.tar.gz $ELIXIR_DOWNLOAD_URL 	&& echo "$ELIXIR_DOWNLOAD_SHA256  elixir-src.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/local/src/elixir 	&& tar -xzC /usr/local/src/elixir --strip-components=1 -f elixir-src.tar.gz 	&& rm elixir-src.tar.gz 	&& cd /usr/local/src/elixir 	&& make install clean 	&& find /usr/local/src/elixir/ -type f -not -regex "/usr/local/src/elixir/lib/[^\/]*/lib.*" -exec rm -rf {} + 	&& find /usr/local/src/elixir/ -type d -depth -empty -delete 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 15:35:26 GMT
CMD ["iex"]
```

-	Layers:
	-	`sha256:219f4ac08f8026026673d3212473b774749e609a07e734f5812912239893f829`  
		Last Modified: Thu, 09 Feb 2023 06:27:52 GMT  
		Size: 58.9 MB (58923468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5291c96e7a501d88d8582c3532f3131835f8be2c1b82f939075483565ed7b46`  
		Last Modified: Thu, 09 Feb 2023 07:01:12 GMT  
		Size: 58.6 MB (58577082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1537e736a6fafb21f7db513f425cef713dc5168147757b1764dc40eccaa274ea`  
		Last Modified: Thu, 09 Feb 2023 15:47:05 GMT  
		Size: 6.7 MB (6695408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `elixir:slim` - linux; s390x

```console
$ docker pull elixir@sha256:9e6845a6b57a4516c268d5aa775830367931f13b8807675f90a6337440bc59fb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.1 MB (118139246 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:edcd0486e7ef6b939618f907dfb7a1e5acb24fc9799a7d45e4cec1e4240f4b54`
-	Default Command: `["iex"]`

```dockerfile
# Thu, 09 Feb 2023 02:41:26 GMT
ADD file:952595f2a554945ef740fa7b1fbc617a9ce3e1c3b90ddf1e7c0ac6018e6a98f9 in / 
# Thu, 09 Feb 2023 02:41:30 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 04:44:00 GMT
ENV OTP_VERSION=25.2.2 REBAR3_VERSION=3.19.0
# Thu, 09 Feb 2023 04:44:01 GMT
LABEL org.opencontainers.image.version=25.2.2
# Thu, 09 Feb 2023 04:50:54 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="535e535b2e90e71deca96c53f19710e6ebf3d4289b0a3116e7cf83b7e2c4bb7e" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& REBAR3_DOWNLOAD_URL="https://github.com/erlang/rebar3/archive/${REBAR3_VERSION}.tar.gz" 	&& REBAR3_DOWNLOAD_SHA256="ff9ef42c737480477ebdf0dd9d95ece534a14c96f05edafbf32e9af973280bc3" 	&& mkdir -p /usr/src/rebar3-src 	&& curl -fSL -o rebar3-src.tar.gz "$REBAR3_DOWNLOAD_URL" 	&& echo "$REBAR3_DOWNLOAD_SHA256 rebar3-src.tar.gz" | sha256sum -c - 	&& tar -xzf rebar3-src.tar.gz -C /usr/src/rebar3-src --strip-components=1 	&& rm rebar3-src.tar.gz 	&& cd /usr/src/rebar3-src 	&& HOME=$PWD ./bootstrap 	&& install -v ./rebar3 /usr/local/bin/ 	&& rm -rf /usr/src/rebar3-src 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Thu, 09 Feb 2023 04:50:57 GMT
CMD ["erl"]
# Thu, 09 Feb 2023 10:38:40 GMT
ENV ELIXIR_VERSION=v1.14.3 LANG=C.UTF-8
# Thu, 09 Feb 2023 10:39:56 GMT
RUN set -xe 	&& ELIXIR_DOWNLOAD_URL="https://github.com/elixir-lang/elixir/archive/${ELIXIR_VERSION}.tar.gz" 	&& ELIXIR_DOWNLOAD_SHA256="bd464145257f36bd64f7ba8bed93b6499c50571b415c491b20267d27d7035707" 	&& buildDeps=' 		ca-certificates 		curl 		make 	' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $buildDeps 	&& curl -fSL -o elixir-src.tar.gz $ELIXIR_DOWNLOAD_URL 	&& echo "$ELIXIR_DOWNLOAD_SHA256  elixir-src.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/local/src/elixir 	&& tar -xzC /usr/local/src/elixir --strip-components=1 -f elixir-src.tar.gz 	&& rm elixir-src.tar.gz 	&& cd /usr/local/src/elixir 	&& make install clean 	&& find /usr/local/src/elixir/ -type f -not -regex "/usr/local/src/elixir/lib/[^\/]*/lib.*" -exec rm -rf {} + 	&& find /usr/local/src/elixir/ -type d -depth -empty -delete 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 10:39:56 GMT
CMD ["iex"]
```

-	Layers:
	-	`sha256:83809ebda0c421fc95029bc6775e0a0c1eba6916a58b115dcb6a14885dae2028`  
		Last Modified: Thu, 09 Feb 2023 02:45:46 GMT  
		Size: 53.3 MB (53278896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15e0f18fdeeae8fc395d19486a276c2110949f9c8f897da07416fb591b1eae61`  
		Last Modified: Thu, 09 Feb 2023 05:00:26 GMT  
		Size: 58.2 MB (58165304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79f6c7b5c5a2563f929f9bbbb0b7e404e104815db562cd4e87cd3c31c772e7a3`  
		Last Modified: Thu, 09 Feb 2023 10:50:35 GMT  
		Size: 6.7 MB (6695046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
