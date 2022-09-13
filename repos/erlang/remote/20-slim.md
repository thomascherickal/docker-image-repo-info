## `erlang:20-slim`

```console
$ docker pull erlang@sha256:59a93e54b2b362c829061d4429f46210ddb5ddd0a88ffd546e1ba11cba74a7eb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `erlang:20-slim` - linux; amd64

```console
$ docker pull erlang@sha256:f34e84b7775cc1a2ea01ac610b441cf900cb79ddc32f71fa886c34cc263ef94a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.9 MB (111905979 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28b248a36b81cb7bc0b7e6b8681ade2ec66b7f6f09c74ba96061ae5ad633a250`
-	Default Command: `["erl"]`

```dockerfile
# Tue, 13 Sep 2022 00:56:38 GMT
ADD file:4649a893b2859f2ff51182a13c9c8eeaeaea866161b3f4a1c4f0bb48bc01d007 in / 
# Tue, 13 Sep 2022 00:56:38 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 05:19:09 GMT
ENV OTP_VERSION=20.3.8.26 REBAR3_VERSION=3.15.2
# Tue, 13 Sep 2022 05:26:23 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="dce78b60938a48b887317e5222cff946fd4af36666153ab2f0f022aa91755813" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& REBAR3_DOWNLOAD_URL="https://github.com/erlang/rebar3/archive/${REBAR3_VERSION}.tar.gz" 	&& REBAR3_DOWNLOAD_SHA256="11b6bead835421a276e287562588580b63ac1c8dcb0e3c51f674887e4ab395cd" 	&& mkdir -p /usr/src/rebar3-src 	&& curl -fSL -o rebar3-src.tar.gz "$REBAR3_DOWNLOAD_URL" 	&& echo "$REBAR3_DOWNLOAD_SHA256 rebar3-src.tar.gz" | sha256sum -c - 	&& tar -xzf rebar3-src.tar.gz -C /usr/src/rebar3-src --strip-components=1 	&& rm rebar3-src.tar.gz 	&& cd /usr/src/rebar3-src 	&& HOME=$PWD ./bootstrap 	&& install -v ./rebar3 /usr/local/bin/ 	&& rm -rf /usr/src/rebar3-src 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Tue, 13 Sep 2022 05:26:24 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:86467c57892b6bb48d563cb5940c68b69c431b2e79c3547df60d1c761c21c156`  
		Last Modified: Tue, 13 Sep 2022 01:00:51 GMT  
		Size: 50.4 MB (50440374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f62f3145b112a07846c7da367b6f6ba18636ce26c138e0ac24dfa3e896ff3bc`  
		Last Modified: Tue, 13 Sep 2022 05:34:16 GMT  
		Size: 61.5 MB (61465605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `erlang:20-slim` - linux; arm variant v7

```console
$ docker pull erlang@sha256:55dc2b5311a3a9c205fd6867df56928128c57efa8c3cdc01e8a2155549424bdb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **103.3 MB (103335082 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d3cad9b55092d5d2d4815ca794ff7b903334eb4df1185b001bb2179eeb512a1`
-	Default Command: `["erl"]`

```dockerfile
# Tue, 13 Sep 2022 03:42:55 GMT
ADD file:28e8fbd48a4aa7f5294aa6046899d5d5cbbd70ba28f7c6d3570d4f92dab36103 in / 
# Tue, 13 Sep 2022 03:42:55 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 11:02:27 GMT
ENV OTP_VERSION=20.3.8.26 REBAR3_VERSION=3.15.2
# Tue, 13 Sep 2022 11:16:36 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="dce78b60938a48b887317e5222cff946fd4af36666153ab2f0f022aa91755813" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& REBAR3_DOWNLOAD_URL="https://github.com/erlang/rebar3/archive/${REBAR3_VERSION}.tar.gz" 	&& REBAR3_DOWNLOAD_SHA256="11b6bead835421a276e287562588580b63ac1c8dcb0e3c51f674887e4ab395cd" 	&& mkdir -p /usr/src/rebar3-src 	&& curl -fSL -o rebar3-src.tar.gz "$REBAR3_DOWNLOAD_URL" 	&& echo "$REBAR3_DOWNLOAD_SHA256 rebar3-src.tar.gz" | sha256sum -c - 	&& tar -xzf rebar3-src.tar.gz -C /usr/src/rebar3-src --strip-components=1 	&& rm rebar3-src.tar.gz 	&& cd /usr/src/rebar3-src 	&& HOME=$PWD ./bootstrap 	&& install -v ./rebar3 /usr/local/bin/ 	&& rm -rf /usr/src/rebar3-src 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Tue, 13 Sep 2022 11:16:37 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:03c0a108fceb58ca60977e45057eccb02892db7412dc4da52f05ebeacf68951d`  
		Last Modified: Tue, 13 Sep 2022 03:50:16 GMT  
		Size: 45.9 MB (45914887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:019420c56f237a35e9f0724fe06bc6db99dc0437c0352aeccb3662bc82a17759`  
		Last Modified: Tue, 13 Sep 2022 11:28:33 GMT  
		Size: 57.4 MB (57420195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `erlang:20-slim` - linux; arm64 variant v8

```console
$ docker pull erlang@sha256:5f20f075d6a43f92974fcde0a338513203f405730d380c13261317f2b2d2560d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.6 MB (107647632 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cdeaf76003ca89cf1285cbb0a5eb7775bd8847c426e4bb7147bd45c2d0cbd0ed`
-	Default Command: `["erl"]`

```dockerfile
# Tue, 13 Sep 2022 02:11:06 GMT
ADD file:304a544562f139d7ab96511b7f1e059966cf90169117e835072f132468bf91c8 in / 
# Tue, 13 Sep 2022 02:11:07 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 06:18:32 GMT
ENV OTP_VERSION=20.3.8.26 REBAR3_VERSION=3.15.2
# Tue, 13 Sep 2022 06:22:41 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="dce78b60938a48b887317e5222cff946fd4af36666153ab2f0f022aa91755813" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& REBAR3_DOWNLOAD_URL="https://github.com/erlang/rebar3/archive/${REBAR3_VERSION}.tar.gz" 	&& REBAR3_DOWNLOAD_SHA256="11b6bead835421a276e287562588580b63ac1c8dcb0e3c51f674887e4ab395cd" 	&& mkdir -p /usr/src/rebar3-src 	&& curl -fSL -o rebar3-src.tar.gz "$REBAR3_DOWNLOAD_URL" 	&& echo "$REBAR3_DOWNLOAD_SHA256 rebar3-src.tar.gz" | sha256sum -c - 	&& tar -xzf rebar3-src.tar.gz -C /usr/src/rebar3-src --strip-components=1 	&& rm rebar3-src.tar.gz 	&& cd /usr/src/rebar3-src 	&& HOME=$PWD ./bootstrap 	&& install -v ./rebar3 /usr/local/bin/ 	&& rm -rf /usr/src/rebar3-src 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Tue, 13 Sep 2022 06:22:41 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:e2406a452ad23ba9085e0708f5e15309206a618eb828aa307becbb239414392f`  
		Last Modified: Tue, 13 Sep 2022 02:16:42 GMT  
		Size: 49.2 MB (49228261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed3c4ef69d435ce9401cd197cb3ad43792407fc81002582efbb1a0a45e0d147f`  
		Last Modified: Tue, 13 Sep 2022 06:31:39 GMT  
		Size: 58.4 MB (58419371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `erlang:20-slim` - linux; 386

```console
$ docker pull erlang@sha256:b5de46231116e85c27c649d19505a4510ff99c3c258fc828a72f749bb6eb58e9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.2 MB (112198369 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a76533a96148a1c9e02597f0edfb8fd0cf593bf505a574d4cf12ce730b1fab5`
-	Default Command: `["erl"]`

```dockerfile
# Tue, 13 Sep 2022 01:39:56 GMT
ADD file:abd47beae46939f6ebc8cc566b1f23f170bd1b9318b1ef10dd16ea4209140bd0 in / 
# Tue, 13 Sep 2022 01:39:57 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 06:10:17 GMT
ENV OTP_VERSION=20.3.8.26 REBAR3_VERSION=3.15.2
# Tue, 13 Sep 2022 06:14:43 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="dce78b60938a48b887317e5222cff946fd4af36666153ab2f0f022aa91755813" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& REBAR3_DOWNLOAD_URL="https://github.com/erlang/rebar3/archive/${REBAR3_VERSION}.tar.gz" 	&& REBAR3_DOWNLOAD_SHA256="11b6bead835421a276e287562588580b63ac1c8dcb0e3c51f674887e4ab395cd" 	&& mkdir -p /usr/src/rebar3-src 	&& curl -fSL -o rebar3-src.tar.gz "$REBAR3_DOWNLOAD_URL" 	&& echo "$REBAR3_DOWNLOAD_SHA256 rebar3-src.tar.gz" | sha256sum -c - 	&& tar -xzf rebar3-src.tar.gz -C /usr/src/rebar3-src --strip-components=1 	&& rm rebar3-src.tar.gz 	&& cd /usr/src/rebar3-src 	&& HOME=$PWD ./bootstrap 	&& install -v ./rebar3 /usr/local/bin/ 	&& rm -rf /usr/src/rebar3-src 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Tue, 13 Sep 2022 06:14:44 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:a0702c36e95be838f5e174ceb286969e8527f17111141f2c8a8ecda44d0a14d4`  
		Last Modified: Tue, 13 Sep 2022 01:45:44 GMT  
		Size: 51.2 MB (51202973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9a643bbb141d30e5da3e1f513220be51fdd075234f3c0f4593c3f16038610b0`  
		Last Modified: Tue, 13 Sep 2022 06:23:50 GMT  
		Size: 61.0 MB (60995396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
