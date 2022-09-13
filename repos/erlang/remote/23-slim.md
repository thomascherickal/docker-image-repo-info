## `erlang:23-slim`

```console
$ docker pull erlang@sha256:490b9188e71cc81d3a27590fce1f0d63d623c5b42eff15548194e05f5d9d6b16
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `erlang:23-slim` - linux; amd64

```console
$ docker pull erlang@sha256:2d804c42f519b1e3ec1dc6df7430b8d71eb084bcf4f052e1cd8cbfa116945f2e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.4 MB (112435485 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02b76e5753ada83adfd12183736c1f4ad370cba9bd8453b3da6b793b85506ddf`
-	Default Command: `["erl"]`

```dockerfile
# Tue, 13 Sep 2022 00:56:38 GMT
ADD file:4649a893b2859f2ff51182a13c9c8eeaeaea866161b3f4a1c4f0bb48bc01d007 in / 
# Tue, 13 Sep 2022 00:56:38 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 04:33:11 GMT
ENV OTP_VERSION=23.3.4.17 REBAR3_VERSION=3.19.0
# Tue, 13 Sep 2022 04:33:12 GMT
LABEL org.opencontainers.image.version=23.3.4.17
# Tue, 13 Sep 2022 04:38:17 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="29c910f0feec751b08685f5634416ee8aa46b0a2f65dd5944694bbace2c066ed" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& REBAR3_DOWNLOAD_URL="https://github.com/erlang/rebar3/archive/${REBAR3_VERSION}.tar.gz" 	&& REBAR3_DOWNLOAD_SHA256="ff9ef42c737480477ebdf0dd9d95ece534a14c96f05edafbf32e9af973280bc3" 	&& mkdir -p /usr/src/rebar3-src 	&& curl -fSL -o rebar3-src.tar.gz "$REBAR3_DOWNLOAD_URL" 	&& echo "$REBAR3_DOWNLOAD_SHA256 rebar3-src.tar.gz" | sha256sum -c - 	&& tar -xzf rebar3-src.tar.gz -C /usr/src/rebar3-src --strip-components=1 	&& rm rebar3-src.tar.gz 	&& cd /usr/src/rebar3-src 	&& HOME=$PWD ./bootstrap 	&& install -v ./rebar3 /usr/local/bin/ 	&& rm -rf /usr/src/rebar3-src 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Tue, 13 Sep 2022 04:38:17 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:86467c57892b6bb48d563cb5940c68b69c431b2e79c3547df60d1c761c21c156`  
		Last Modified: Tue, 13 Sep 2022 01:00:51 GMT  
		Size: 50.4 MB (50440374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfc38fb79b00ca760e2034fa3a1d14e78cbbaef27482eda2dfc3e98a6822d724`  
		Last Modified: Tue, 13 Sep 2022 05:30:57 GMT  
		Size: 62.0 MB (61995111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `erlang:23-slim` - linux; arm variant v7

```console
$ docker pull erlang@sha256:c003294440ce10888777efb2561aa6772072ffd48ded955ff4badecb704e5f1e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.4 MB (106391835 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:935c960d00aaf0dad14966a941c10d47f2ff9121eaac1b0e48fefacfc00bc13b`
-	Default Command: `["erl"]`

```dockerfile
# Tue, 13 Sep 2022 03:42:55 GMT
ADD file:28e8fbd48a4aa7f5294aa6046899d5d5cbbd70ba28f7c6d3570d4f92dab36103 in / 
# Tue, 13 Sep 2022 03:42:55 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 09:25:57 GMT
ENV OTP_VERSION=23.3.4.17 REBAR3_VERSION=3.19.0
# Tue, 13 Sep 2022 09:25:57 GMT
LABEL org.opencontainers.image.version=23.3.4.17
# Tue, 13 Sep 2022 09:42:33 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="29c910f0feec751b08685f5634416ee8aa46b0a2f65dd5944694bbace2c066ed" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& REBAR3_DOWNLOAD_URL="https://github.com/erlang/rebar3/archive/${REBAR3_VERSION}.tar.gz" 	&& REBAR3_DOWNLOAD_SHA256="ff9ef42c737480477ebdf0dd9d95ece534a14c96f05edafbf32e9af973280bc3" 	&& mkdir -p /usr/src/rebar3-src 	&& curl -fSL -o rebar3-src.tar.gz "$REBAR3_DOWNLOAD_URL" 	&& echo "$REBAR3_DOWNLOAD_SHA256 rebar3-src.tar.gz" | sha256sum -c - 	&& tar -xzf rebar3-src.tar.gz -C /usr/src/rebar3-src --strip-components=1 	&& rm rebar3-src.tar.gz 	&& cd /usr/src/rebar3-src 	&& HOME=$PWD ./bootstrap 	&& install -v ./rebar3 /usr/local/bin/ 	&& rm -rf /usr/src/rebar3-src 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Tue, 13 Sep 2022 09:42:33 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:03c0a108fceb58ca60977e45057eccb02892db7412dc4da52f05ebeacf68951d`  
		Last Modified: Tue, 13 Sep 2022 03:50:16 GMT  
		Size: 45.9 MB (45914887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6065e12d063287f4a2d50bb921ffd9b1c86cfc538f21f899448313edf7c7a48`  
		Last Modified: Tue, 13 Sep 2022 11:24:23 GMT  
		Size: 60.5 MB (60476948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `erlang:23-slim` - linux; arm64 variant v8

```console
$ docker pull erlang@sha256:afc2836dc11ebb133f900517d2c9ef0a1557115412e522e0e0a2d62d74aa1d62
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.1 MB (108127456 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd900feaa7db3c3fe0021dac0ce77f059b7c825f2e8c3068218fc608e04c4660`
-	Default Command: `["erl"]`

```dockerfile
# Tue, 13 Sep 2022 02:11:06 GMT
ADD file:304a544562f139d7ab96511b7f1e059966cf90169117e835072f132468bf91c8 in / 
# Tue, 13 Sep 2022 02:11:07 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 05:46:12 GMT
ENV OTP_VERSION=23.3.4.17 REBAR3_VERSION=3.19.0
# Tue, 13 Sep 2022 05:46:13 GMT
LABEL org.opencontainers.image.version=23.3.4.17
# Tue, 13 Sep 2022 05:50:07 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="29c910f0feec751b08685f5634416ee8aa46b0a2f65dd5944694bbace2c066ed" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& REBAR3_DOWNLOAD_URL="https://github.com/erlang/rebar3/archive/${REBAR3_VERSION}.tar.gz" 	&& REBAR3_DOWNLOAD_SHA256="ff9ef42c737480477ebdf0dd9d95ece534a14c96f05edafbf32e9af973280bc3" 	&& mkdir -p /usr/src/rebar3-src 	&& curl -fSL -o rebar3-src.tar.gz "$REBAR3_DOWNLOAD_URL" 	&& echo "$REBAR3_DOWNLOAD_SHA256 rebar3-src.tar.gz" | sha256sum -c - 	&& tar -xzf rebar3-src.tar.gz -C /usr/src/rebar3-src --strip-components=1 	&& rm rebar3-src.tar.gz 	&& cd /usr/src/rebar3-src 	&& HOME=$PWD ./bootstrap 	&& install -v ./rebar3 /usr/local/bin/ 	&& rm -rf /usr/src/rebar3-src 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Tue, 13 Sep 2022 05:50:08 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:e2406a452ad23ba9085e0708f5e15309206a618eb828aa307becbb239414392f`  
		Last Modified: Tue, 13 Sep 2022 02:16:42 GMT  
		Size: 49.2 MB (49228261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6097736027934597f4f915985e8241327110e6b1bbfaf18ca68717c4323ea35`  
		Last Modified: Tue, 13 Sep 2022 06:28:23 GMT  
		Size: 58.9 MB (58899195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `erlang:23-slim` - linux; 386

```console
$ docker pull erlang@sha256:beaf76d44d151fd059b7596847bb30b86d403ff8bde62f0cdde65b0f4aa90433
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.5 MB (112546783 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2cdf7ea209a95f7780fc57a27b9d79735b5026d80bc6030da78951cbd0fd9806`
-	Default Command: `["erl"]`

```dockerfile
# Tue, 13 Sep 2022 01:39:56 GMT
ADD file:abd47beae46939f6ebc8cc566b1f23f170bd1b9318b1ef10dd16ea4209140bd0 in / 
# Tue, 13 Sep 2022 01:39:57 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 05:35:11 GMT
ENV OTP_VERSION=23.3.4.17 REBAR3_VERSION=3.19.0
# Tue, 13 Sep 2022 05:35:12 GMT
LABEL org.opencontainers.image.version=23.3.4.17
# Tue, 13 Sep 2022 05:40:20 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="29c910f0feec751b08685f5634416ee8aa46b0a2f65dd5944694bbace2c066ed" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& REBAR3_DOWNLOAD_URL="https://github.com/erlang/rebar3/archive/${REBAR3_VERSION}.tar.gz" 	&& REBAR3_DOWNLOAD_SHA256="ff9ef42c737480477ebdf0dd9d95ece534a14c96f05edafbf32e9af973280bc3" 	&& mkdir -p /usr/src/rebar3-src 	&& curl -fSL -o rebar3-src.tar.gz "$REBAR3_DOWNLOAD_URL" 	&& echo "$REBAR3_DOWNLOAD_SHA256 rebar3-src.tar.gz" | sha256sum -c - 	&& tar -xzf rebar3-src.tar.gz -C /usr/src/rebar3-src --strip-components=1 	&& rm rebar3-src.tar.gz 	&& cd /usr/src/rebar3-src 	&& HOME=$PWD ./bootstrap 	&& install -v ./rebar3 /usr/local/bin/ 	&& rm -rf /usr/src/rebar3-src 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Tue, 13 Sep 2022 05:40:21 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:a0702c36e95be838f5e174ceb286969e8527f17111141f2c8a8ecda44d0a14d4`  
		Last Modified: Tue, 13 Sep 2022 01:45:44 GMT  
		Size: 51.2 MB (51202973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9af3478691672de029f6f2154224167a654a2bfd273480ad7efe4e6fa78024b2`  
		Last Modified: Tue, 13 Sep 2022 06:20:33 GMT  
		Size: 61.3 MB (61343810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
