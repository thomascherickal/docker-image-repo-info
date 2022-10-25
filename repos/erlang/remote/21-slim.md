## `erlang:21-slim`

```console
$ docker pull erlang@sha256:1e7a6a6d7d1c4413344c8715508f942faa18fdbbd6b64957ca078b33aa365ab2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `erlang:21-slim` - linux; amd64

```console
$ docker pull erlang@sha256:3ec8682eed625ea72990d88616c5f8c7d86e94a9baec128da3f0d388d20f7d97
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.0 MB (109006615 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01d5686f233159b0af8128aea674e5da502823fe7018aa7500837dc16d4c0bc7`
-	Default Command: `["erl"]`

```dockerfile
# Tue, 25 Oct 2022 01:44:02 GMT
ADD file:259be79d94a2549a667ad08a093fe18f15a6c93d66a0723292f49294e31fc7a1 in / 
# Tue, 25 Oct 2022 01:44:02 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 03:23:41 GMT
ENV OTP_VERSION=21.3.8.24 REBAR3_VERSION=3.15.2
# Tue, 25 Oct 2022 03:23:41 GMT
LABEL org.opencontainers.image.version=21.3.8.24
# Tue, 25 Oct 2022 03:30:40 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="90017fe0b844cf3ba7dc9faf7f6f690050f3138f3d3f7532a9343174f5f9febc" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& REBAR3_DOWNLOAD_URL="https://github.com/erlang/rebar3/archive/${REBAR3_VERSION}.tar.gz" 	&& REBAR3_DOWNLOAD_SHA256="11b6bead835421a276e287562588580b63ac1c8dcb0e3c51f674887e4ab395cd" 	&& mkdir -p /usr/src/rebar3-src 	&& curl -fSL -o rebar3-src.tar.gz "$REBAR3_DOWNLOAD_URL" 	&& echo "$REBAR3_DOWNLOAD_SHA256 rebar3-src.tar.gz" | sha256sum -c - 	&& tar -xzf rebar3-src.tar.gz -C /usr/src/rebar3-src --strip-components=1 	&& rm rebar3-src.tar.gz 	&& cd /usr/src/rebar3-src 	&& HOME=$PWD ./bootstrap 	&& install -v ./rebar3 /usr/local/bin/ 	&& rm -rf /usr/src/rebar3-src 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Tue, 25 Oct 2022 03:30:40 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:fd31ec14dccdcda8f2472547f1a94ef0a23b8dabb764cd7b1d48aeee0afea7c8`  
		Last Modified: Tue, 25 Oct 2022 01:48:15 GMT  
		Size: 50.4 MB (50447742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dc45093fb0527aac52fc5ad492f81c0917d99544b023de5cfdb9a8b71d0ac4c`  
		Last Modified: Tue, 25 Oct 2022 03:41:27 GMT  
		Size: 58.6 MB (58558873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `erlang:21-slim` - linux; arm variant v7

```console
$ docker pull erlang@sha256:c40fdb9a1c4a90b7fdfb78254aa608e5d56e57f3a57109b6e1fad99fbb031866
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.3 MB (100309363 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3644c93c2dac46ba964930b12de7e00e580c395a5ee0baaedf896512315655ef`
-	Default Command: `["erl"]`

```dockerfile
# Tue, 04 Oct 2022 23:59:00 GMT
ADD file:b16f07fda9b8beecd7c275565d0ed135fb298c712482766c8f0e40fac932130c in / 
# Tue, 04 Oct 2022 23:59:01 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 03:45:43 GMT
ENV OTP_VERSION=21.3.8.24 REBAR3_VERSION=3.15.2
# Wed, 05 Oct 2022 03:45:43 GMT
LABEL org.opencontainers.image.version=21.3.8.24
# Wed, 05 Oct 2022 03:59:54 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="90017fe0b844cf3ba7dc9faf7f6f690050f3138f3d3f7532a9343174f5f9febc" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& REBAR3_DOWNLOAD_URL="https://github.com/erlang/rebar3/archive/${REBAR3_VERSION}.tar.gz" 	&& REBAR3_DOWNLOAD_SHA256="11b6bead835421a276e287562588580b63ac1c8dcb0e3c51f674887e4ab395cd" 	&& mkdir -p /usr/src/rebar3-src 	&& curl -fSL -o rebar3-src.tar.gz "$REBAR3_DOWNLOAD_URL" 	&& echo "$REBAR3_DOWNLOAD_SHA256 rebar3-src.tar.gz" | sha256sum -c - 	&& tar -xzf rebar3-src.tar.gz -C /usr/src/rebar3-src --strip-components=1 	&& rm rebar3-src.tar.gz 	&& cd /usr/src/rebar3-src 	&& HOME=$PWD ./bootstrap 	&& install -v ./rebar3 /usr/local/bin/ 	&& rm -rf /usr/src/rebar3-src 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:59:55 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:bba3a5db4dfa403d6e1db947629616e80fb4514e2190e6aa1fb6a2c828c32491`  
		Last Modified: Wed, 05 Oct 2022 00:05:35 GMT  
		Size: 45.9 MB (45914973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3388ae5359676dbfe2220db292a933fd4bcea06ff59b4c36d4b3f9a960350a2`  
		Last Modified: Wed, 05 Oct 2022 04:42:35 GMT  
		Size: 54.4 MB (54394390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `erlang:21-slim` - linux; arm64 variant v8

```console
$ docker pull erlang@sha256:9c32aa4f22f58c65c52a065bd31f808e78b3c262f7c390cd59cbe802f122d84a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.7 MB (104660598 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa750e4dcff0c415b9e9cfe4d75d1f212a3bfb4e7d46e0228d6669875478f683`
-	Default Command: `["erl"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:07 GMT
ADD file:21afa32c0395cc5046d09741d6821d21cfd9b77bce46ebcfc8fd9aca57c73648 in / 
# Tue, 25 Oct 2022 05:46:08 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 09:24:47 GMT
ENV OTP_VERSION=21.3.8.24 REBAR3_VERSION=3.15.2
# Tue, 25 Oct 2022 09:24:47 GMT
LABEL org.opencontainers.image.version=21.3.8.24
# Tue, 25 Oct 2022 09:28:06 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="90017fe0b844cf3ba7dc9faf7f6f690050f3138f3d3f7532a9343174f5f9febc" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& REBAR3_DOWNLOAD_URL="https://github.com/erlang/rebar3/archive/${REBAR3_VERSION}.tar.gz" 	&& REBAR3_DOWNLOAD_SHA256="11b6bead835421a276e287562588580b63ac1c8dcb0e3c51f674887e4ab395cd" 	&& mkdir -p /usr/src/rebar3-src 	&& curl -fSL -o rebar3-src.tar.gz "$REBAR3_DOWNLOAD_URL" 	&& echo "$REBAR3_DOWNLOAD_SHA256 rebar3-src.tar.gz" | sha256sum -c - 	&& tar -xzf rebar3-src.tar.gz -C /usr/src/rebar3-src --strip-components=1 	&& rm rebar3-src.tar.gz 	&& cd /usr/src/rebar3-src 	&& HOME=$PWD ./bootstrap 	&& install -v ./rebar3 /usr/local/bin/ 	&& rm -rf /usr/src/rebar3-src 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Tue, 25 Oct 2022 09:28:06 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:3ba81f4c3c21f92780061ee116827d64ac4edbcd02b056845c2aaa3097b730ed`  
		Last Modified: Tue, 25 Oct 2022 05:49:24 GMT  
		Size: 49.2 MB (49233280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:240d0c3eb60ecc2be03e36788c9e47b901a38bd1a5d2bb53a31447b0c04bdee8`  
		Last Modified: Tue, 25 Oct 2022 09:42:27 GMT  
		Size: 55.4 MB (55427318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `erlang:21-slim` - linux; 386

```console
$ docker pull erlang@sha256:d62eccd6e0aa5ee7a2e6a3ca449e9f3d2d9593ce44a71d2836cfca319a6ed98b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.2 MB (109245095 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02f35ba869a459d5eb5da77928875b91215df7906856acf452158daf681d7711`
-	Default Command: `["erl"]`

```dockerfile
# Tue, 25 Oct 2022 02:22:47 GMT
ADD file:7e14d4afa5499129c959c5ae5dc270e2fa04659c2c9b0527094cda3494c02d0f in / 
# Tue, 25 Oct 2022 02:22:47 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 06:29:55 GMT
ENV OTP_VERSION=21.3.8.24 REBAR3_VERSION=3.15.2
# Tue, 25 Oct 2022 06:29:56 GMT
LABEL org.opencontainers.image.version=21.3.8.24
# Tue, 25 Oct 2022 06:34:31 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="90017fe0b844cf3ba7dc9faf7f6f690050f3138f3d3f7532a9343174f5f9febc" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& REBAR3_DOWNLOAD_URL="https://github.com/erlang/rebar3/archive/${REBAR3_VERSION}.tar.gz" 	&& REBAR3_DOWNLOAD_SHA256="11b6bead835421a276e287562588580b63ac1c8dcb0e3c51f674887e4ab395cd" 	&& mkdir -p /usr/src/rebar3-src 	&& curl -fSL -o rebar3-src.tar.gz "$REBAR3_DOWNLOAD_URL" 	&& echo "$REBAR3_DOWNLOAD_SHA256 rebar3-src.tar.gz" | sha256sum -c - 	&& tar -xzf rebar3-src.tar.gz -C /usr/src/rebar3-src --strip-components=1 	&& rm rebar3-src.tar.gz 	&& cd /usr/src/rebar3-src 	&& HOME=$PWD ./bootstrap 	&& install -v ./rebar3 /usr/local/bin/ 	&& rm -rf /usr/src/rebar3-src 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:34:32 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:76a731c42f665e7334a622f65117ef9389e97a878b7c74bb4a10dfe9cdb296c6`  
		Last Modified: Tue, 25 Oct 2022 02:28:50 GMT  
		Size: 51.2 MB (51207943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e10e7221d76fe9b333700c18cfe4ef6165706ead2cbe36e30b299df6656b059`  
		Last Modified: Tue, 25 Oct 2022 06:53:16 GMT  
		Size: 58.0 MB (58037152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
