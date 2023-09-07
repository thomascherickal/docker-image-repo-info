## `erlang:25-slim`

```console
$ docker pull erlang@sha256:ce515bf121726c37d63a112ebed011ad798e27bf57a3e1c5bd85e9590ed49606
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

### `erlang:25-slim` - linux; amd64

```console
$ docker pull erlang@sha256:0e63a149f81bc994592c3150e5186a1a5261079e73acbbf0f9c95c6a9694e1ba
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.9 MB (120888070 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9bf72347d5b6d3dff16aa0c9f96cef7e3fff8bbef28abfd3fc2275a20a5cd262`
-	Default Command: `["erl"]`

```dockerfile
# Thu, 07 Sep 2023 00:21:01 GMT
ADD file:144dff349a666134b5e98a9f1c6650fd9d6e4a88a6f98857f26eb84989360b91 in / 
# Thu, 07 Sep 2023 00:21:02 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 00:53:40 GMT
ENV OTP_VERSION=25.3.2.3 REBAR3_VERSION=3.20.0
# Thu, 07 Sep 2023 00:53:40 GMT
LABEL org.opencontainers.image.version=25.3.2.3
# Thu, 07 Sep 2023 00:58:23 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="93b0b2b02b789d3b51ed1c2e56fc40e2ee5a8394bf82686f06be5458e9b85994" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& REBAR3_DOWNLOAD_URL="https://github.com/erlang/rebar3/archive/${REBAR3_VERSION}.tar.gz" 	&& REBAR3_DOWNLOAD_SHA256="53ed7f294a8b8fb4d7d75988c69194943831c104d39832a1fa30307b1a8593de" 	&& mkdir -p /usr/src/rebar3-src 	&& curl -fSL -o rebar3-src.tar.gz "$REBAR3_DOWNLOAD_URL" 	&& echo "$REBAR3_DOWNLOAD_SHA256 rebar3-src.tar.gz" | sha256sum -c - 	&& tar -xzf rebar3-src.tar.gz -C /usr/src/rebar3-src --strip-components=1 	&& rm rebar3-src.tar.gz 	&& cd /usr/src/rebar3-src 	&& HOME=$PWD ./bootstrap 	&& install -v ./rebar3 /usr/local/bin/ 	&& rm -rf /usr/src/rebar3-src 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Thu, 07 Sep 2023 00:58:24 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:5dea071bb9782209397443f024a630052ab7583e365894d414f1e39cd0f65025`  
		Last Modified: Thu, 07 Sep 2023 00:25:41 GMT  
		Size: 55.1 MB (55056245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70543439c7c51f91950b2cfebacadb4b6c06a5cd93d5f68fd845b9ad7e717167`  
		Last Modified: Thu, 07 Sep 2023 01:31:54 GMT  
		Size: 65.8 MB (65831825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `erlang:25-slim` - linux; arm variant v5

```console
$ docker pull erlang@sha256:b07e7d1cb2a76dcc692edd6f49a01fdb5c3dc79927ff3ea6a510b5826f5471b1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.9 MB (109882453 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f6047e02f36046ab03289c371ad27ead815f463d4fa013e0503f422e1d7c661a`
-	Default Command: `["erl"]`

```dockerfile
# Tue, 15 Aug 2023 23:48:40 GMT
ADD file:d044e64aab907424be649252b5ff1d9f5e8c9494db5b60c0e54f5962bfb73478 in / 
# Tue, 15 Aug 2023 23:48:40 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 00:15:32 GMT
ENV OTP_VERSION=25.3.2.3 REBAR3_VERSION=3.20.0
# Wed, 16 Aug 2023 00:15:32 GMT
LABEL org.opencontainers.image.version=25.3.2.3
# Wed, 16 Aug 2023 00:19:32 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="93b0b2b02b789d3b51ed1c2e56fc40e2ee5a8394bf82686f06be5458e9b85994" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& REBAR3_DOWNLOAD_URL="https://github.com/erlang/rebar3/archive/${REBAR3_VERSION}.tar.gz" 	&& REBAR3_DOWNLOAD_SHA256="53ed7f294a8b8fb4d7d75988c69194943831c104d39832a1fa30307b1a8593de" 	&& mkdir -p /usr/src/rebar3-src 	&& curl -fSL -o rebar3-src.tar.gz "$REBAR3_DOWNLOAD_URL" 	&& echo "$REBAR3_DOWNLOAD_SHA256 rebar3-src.tar.gz" | sha256sum -c - 	&& tar -xzf rebar3-src.tar.gz -C /usr/src/rebar3-src --strip-components=1 	&& rm rebar3-src.tar.gz 	&& cd /usr/src/rebar3-src 	&& HOME=$PWD ./bootstrap 	&& install -v ./rebar3 /usr/local/bin/ 	&& rm -rf /usr/src/rebar3-src 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Wed, 16 Aug 2023 00:19:32 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:0b63bbf2e6f6026dfaed9cbedf777472a04812b7d291501b1d416e49e3ce885e`  
		Last Modified: Tue, 15 Aug 2023 23:51:54 GMT  
		Size: 52.6 MB (52558130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:722b26b4b5492f69d4ae92f252d7fdb66515231552f5034bf353a669ee85bc02`  
		Last Modified: Wed, 16 Aug 2023 00:24:24 GMT  
		Size: 57.3 MB (57324323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `erlang:25-slim` - linux; arm variant v7

```console
$ docker pull erlang@sha256:84fb37cbee4d0344a435361710ea4b8d631d5b9dd7ac0e252037748974dcd2be
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.4 MB (107350692 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bcb0f9de9a476f9cbd36cf38f9517e799e6c717cab611965ede9bf4485b95374`
-	Default Command: `["erl"]`

```dockerfile
# Thu, 07 Sep 2023 00:57:59 GMT
ADD file:931564fb3c8ea78b763a6b98f2739bb7c6a38484122c560a87c7166b7d45c5e6 in / 
# Thu, 07 Sep 2023 00:58:00 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 02:30:06 GMT
ENV OTP_VERSION=25.3.2.3 REBAR3_VERSION=3.20.0
# Thu, 07 Sep 2023 02:30:06 GMT
LABEL org.opencontainers.image.version=25.3.2.3
# Thu, 07 Sep 2023 02:34:42 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="93b0b2b02b789d3b51ed1c2e56fc40e2ee5a8394bf82686f06be5458e9b85994" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& REBAR3_DOWNLOAD_URL="https://github.com/erlang/rebar3/archive/${REBAR3_VERSION}.tar.gz" 	&& REBAR3_DOWNLOAD_SHA256="53ed7f294a8b8fb4d7d75988c69194943831c104d39832a1fa30307b1a8593de" 	&& mkdir -p /usr/src/rebar3-src 	&& curl -fSL -o rebar3-src.tar.gz "$REBAR3_DOWNLOAD_URL" 	&& echo "$REBAR3_DOWNLOAD_SHA256 rebar3-src.tar.gz" | sha256sum -c - 	&& tar -xzf rebar3-src.tar.gz -C /usr/src/rebar3-src --strip-components=1 	&& rm rebar3-src.tar.gz 	&& cd /usr/src/rebar3-src 	&& HOME=$PWD ./bootstrap 	&& install -v ./rebar3 /usr/local/bin/ 	&& rm -rf /usr/src/rebar3-src 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Thu, 07 Sep 2023 02:34:43 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:5826e0d927336e7231f9d05ec48f075045fb51f9b3f16f1e20972f2a3634d102`  
		Last Modified: Thu, 07 Sep 2023 01:02:50 GMT  
		Size: 50.2 MB (50219233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:293d0a45c8f26675afcb8c7d6cd79db45aeef2309b7712410cf3e26b004c2e03`  
		Last Modified: Thu, 07 Sep 2023 03:35:33 GMT  
		Size: 57.1 MB (57131459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `erlang:25-slim` - linux; arm64 variant v8

```console
$ docker pull erlang@sha256:b4c03e2ac2b710d507ad11a55c24fa5679c01b236b280ed4891ff6fa01536b5c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.9 MB (117917062 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0380c19febbfde84233329df5f000676667608dc39de52575987d75f357b7e84`
-	Default Command: `["erl"]`

```dockerfile
# Tue, 15 Aug 2023 23:40:03 GMT
ADD file:8973cddb2d84a543b71001635599951bea6485a3526ae4ff916443b584864c83 in / 
# Tue, 15 Aug 2023 23:40:04 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 02:20:18 GMT
ENV OTP_VERSION=25.3.2.3 REBAR3_VERSION=3.20.0
# Wed, 16 Aug 2023 02:20:18 GMT
LABEL org.opencontainers.image.version=25.3.2.3
# Wed, 16 Aug 2023 02:23:22 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="93b0b2b02b789d3b51ed1c2e56fc40e2ee5a8394bf82686f06be5458e9b85994" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& REBAR3_DOWNLOAD_URL="https://github.com/erlang/rebar3/archive/${REBAR3_VERSION}.tar.gz" 	&& REBAR3_DOWNLOAD_SHA256="53ed7f294a8b8fb4d7d75988c69194943831c104d39832a1fa30307b1a8593de" 	&& mkdir -p /usr/src/rebar3-src 	&& curl -fSL -o rebar3-src.tar.gz "$REBAR3_DOWNLOAD_URL" 	&& echo "$REBAR3_DOWNLOAD_SHA256 rebar3-src.tar.gz" | sha256sum -c - 	&& tar -xzf rebar3-src.tar.gz -C /usr/src/rebar3-src --strip-components=1 	&& rm rebar3-src.tar.gz 	&& cd /usr/src/rebar3-src 	&& HOME=$PWD ./bootstrap 	&& install -v ./rebar3 /usr/local/bin/ 	&& rm -rf /usr/src/rebar3-src 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Wed, 16 Aug 2023 02:23:22 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:e837d9f05c625de5b814b851adbc03559ba02ea7078f57c81a01e18fc65bf42b`  
		Last Modified: Tue, 15 Aug 2023 23:43:37 GMT  
		Size: 53.7 MB (53704779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a296051d87464c23d28a4aaea63b8b992e511c77b7df6607443342721159e4c`  
		Last Modified: Wed, 16 Aug 2023 03:07:51 GMT  
		Size: 64.2 MB (64212283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `erlang:25-slim` - linux; 386

```console
$ docker pull erlang@sha256:84a90ecce7ee0a6a9f436e79369a34ab6b0988a80017d30838e84eba4d249742
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.6 MB (113567727 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d7a71954d09f3ba93f12bc60ec7742038de60cd01f57270d29ee7654dce8393`
-	Default Command: `["erl"]`

```dockerfile
# Tue, 15 Aug 2023 23:39:11 GMT
ADD file:efc88a19b31e68ca41f555bcc51338b0f135cbbd72b90637d8c73969d53addd2 in / 
# Tue, 15 Aug 2023 23:39:12 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:15:51 GMT
ENV OTP_VERSION=25.3.2.3 REBAR3_VERSION=3.20.0
# Wed, 16 Aug 2023 01:15:51 GMT
LABEL org.opencontainers.image.version=25.3.2.3
# Wed, 16 Aug 2023 01:23:39 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="93b0b2b02b789d3b51ed1c2e56fc40e2ee5a8394bf82686f06be5458e9b85994" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& REBAR3_DOWNLOAD_URL="https://github.com/erlang/rebar3/archive/${REBAR3_VERSION}.tar.gz" 	&& REBAR3_DOWNLOAD_SHA256="53ed7f294a8b8fb4d7d75988c69194943831c104d39832a1fa30307b1a8593de" 	&& mkdir -p /usr/src/rebar3-src 	&& curl -fSL -o rebar3-src.tar.gz "$REBAR3_DOWNLOAD_URL" 	&& echo "$REBAR3_DOWNLOAD_SHA256 rebar3-src.tar.gz" | sha256sum -c - 	&& tar -xzf rebar3-src.tar.gz -C /usr/src/rebar3-src --strip-components=1 	&& rm rebar3-src.tar.gz 	&& cd /usr/src/rebar3-src 	&& HOME=$PWD ./bootstrap 	&& install -v ./rebar3 /usr/local/bin/ 	&& rm -rf /usr/src/rebar3-src 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:23:39 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:822e033fa7b169545d5890de01438a9dd87774ff938ff440e823a3ec3f73996d`  
		Last Modified: Tue, 15 Aug 2023 23:43:47 GMT  
		Size: 56.0 MB (56040520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01509576ddc73b687d345d88c5cc552da3b3b7022ff94d92a1e8aa9f3652fa99`  
		Last Modified: Wed, 16 Aug 2023 03:25:41 GMT  
		Size: 57.5 MB (57527207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `erlang:25-slim` - linux; mips64le

```console
$ docker pull erlang@sha256:c66a14f4f60af5105adde9e12fe16c989ca8704845806bce7c509aaf902562cd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.4 MB (111411982 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:535d806589b7cb9b071c458f1088376163d3068e5dfeb62bb8d9eb0e52d9cc02`
-	Default Command: `["erl"]`

```dockerfile
# Thu, 07 Sep 2023 01:09:47 GMT
ADD file:fdd438b39f1dce564715691d2a092378f02bc722e29cb80216efcbaf71cff0b8 in / 
# Thu, 07 Sep 2023 01:09:53 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 02:21:24 GMT
ENV OTP_VERSION=25.3.2.3 REBAR3_VERSION=3.20.0
# Thu, 07 Sep 2023 02:21:27 GMT
LABEL org.opencontainers.image.version=25.3.2.3
# Thu, 07 Sep 2023 02:43:44 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="93b0b2b02b789d3b51ed1c2e56fc40e2ee5a8394bf82686f06be5458e9b85994" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& REBAR3_DOWNLOAD_URL="https://github.com/erlang/rebar3/archive/${REBAR3_VERSION}.tar.gz" 	&& REBAR3_DOWNLOAD_SHA256="53ed7f294a8b8fb4d7d75988c69194943831c104d39832a1fa30307b1a8593de" 	&& mkdir -p /usr/src/rebar3-src 	&& curl -fSL -o rebar3-src.tar.gz "$REBAR3_DOWNLOAD_URL" 	&& echo "$REBAR3_DOWNLOAD_SHA256 rebar3-src.tar.gz" | sha256sum -c - 	&& tar -xzf rebar3-src.tar.gz -C /usr/src/rebar3-src --strip-components=1 	&& rm rebar3-src.tar.gz 	&& cd /usr/src/rebar3-src 	&& HOME=$PWD ./bootstrap 	&& install -v ./rebar3 /usr/local/bin/ 	&& rm -rf /usr/src/rebar3-src 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Thu, 07 Sep 2023 02:43:48 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:0d1f1f4ccb1e0da4313c3ebcd521e7fa8073526c6f64ca7214ed31ae9bd0788e`  
		Last Modified: Thu, 07 Sep 2023 01:21:00 GMT  
		Size: 53.3 MB (53271469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:858e532a319dd9f4e816bfd6da29cae8c02c12a6ada6a93504dcad3d750f39b4`  
		Last Modified: Thu, 07 Sep 2023 03:06:52 GMT  
		Size: 58.1 MB (58140513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `erlang:25-slim` - linux; ppc64le

```console
$ docker pull erlang@sha256:562352a593de969648347067c0160dac7ff4c8e63b48224e8d05d48a2cccff36
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.4 MB (117389020 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aff4d4cd4f5cc0de5fd72e00ed6601c41f264f5a462bba4760a9e9c3f3ef0913`
-	Default Command: `["erl"]`

```dockerfile
# Wed, 16 Aug 2023 01:09:50 GMT
ADD file:23fe4ecb2d3d302e0df50109aee416120a138fad47d1614500f98b65fa288281 in / 
# Wed, 16 Aug 2023 01:09:54 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 02:55:28 GMT
ENV OTP_VERSION=25.3.2.3 REBAR3_VERSION=3.20.0
# Wed, 16 Aug 2023 02:55:28 GMT
LABEL org.opencontainers.image.version=25.3.2.3
# Wed, 16 Aug 2023 03:02:58 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="93b0b2b02b789d3b51ed1c2e56fc40e2ee5a8394bf82686f06be5458e9b85994" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& REBAR3_DOWNLOAD_URL="https://github.com/erlang/rebar3/archive/${REBAR3_VERSION}.tar.gz" 	&& REBAR3_DOWNLOAD_SHA256="53ed7f294a8b8fb4d7d75988c69194943831c104d39832a1fa30307b1a8593de" 	&& mkdir -p /usr/src/rebar3-src 	&& curl -fSL -o rebar3-src.tar.gz "$REBAR3_DOWNLOAD_URL" 	&& echo "$REBAR3_DOWNLOAD_SHA256 rebar3-src.tar.gz" | sha256sum -c - 	&& tar -xzf rebar3-src.tar.gz -C /usr/src/rebar3-src --strip-components=1 	&& rm rebar3-src.tar.gz 	&& cd /usr/src/rebar3-src 	&& HOME=$PWD ./bootstrap 	&& install -v ./rebar3 /usr/local/bin/ 	&& rm -rf /usr/src/rebar3-src 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Wed, 16 Aug 2023 03:03:00 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:148c97e5e41c60dd4fc440664aeee1e57ab7158b53ea7d1f9132198b3d35bc5e`  
		Last Modified: Wed, 16 Aug 2023 01:16:30 GMT  
		Size: 58.9 MB (58928436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dc89e1916d27cb12121695c9105dbd2f8d936d9f5586b9de928c35403126a98`  
		Last Modified: Wed, 16 Aug 2023 03:24:59 GMT  
		Size: 58.5 MB (58460584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `erlang:25-slim` - linux; s390x

```console
$ docker pull erlang@sha256:67a948c45c1401b58a7f9add73f17220fcf767bd42e07b7d33086bdc56361c35
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.3 MB (111333339 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2cdd75e899f673e7856325f5d13dc71a334a14895512588e6754e51a7cfe55f0`
-	Default Command: `["erl"]`

```dockerfile
# Thu, 07 Sep 2023 00:44:03 GMT
ADD file:a0582e191d0265b98e5d46c64ba9b4c46445cfa821c6e41d32db343b0e2a6fec in / 
# Thu, 07 Sep 2023 00:44:12 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 01:59:24 GMT
ENV OTP_VERSION=25.3.2.3 REBAR3_VERSION=3.20.0
# Thu, 07 Sep 2023 01:59:24 GMT
LABEL org.opencontainers.image.version=25.3.2.3
# Thu, 07 Sep 2023 02:03:49 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="93b0b2b02b789d3b51ed1c2e56fc40e2ee5a8394bf82686f06be5458e9b85994" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& REBAR3_DOWNLOAD_URL="https://github.com/erlang/rebar3/archive/${REBAR3_VERSION}.tar.gz" 	&& REBAR3_DOWNLOAD_SHA256="53ed7f294a8b8fb4d7d75988c69194943831c104d39832a1fa30307b1a8593de" 	&& mkdir -p /usr/src/rebar3-src 	&& curl -fSL -o rebar3-src.tar.gz "$REBAR3_DOWNLOAD_URL" 	&& echo "$REBAR3_DOWNLOAD_SHA256 rebar3-src.tar.gz" | sha256sum -c - 	&& tar -xzf rebar3-src.tar.gz -C /usr/src/rebar3-src --strip-components=1 	&& rm rebar3-src.tar.gz 	&& cd /usr/src/rebar3-src 	&& HOME=$PWD ./bootstrap 	&& install -v ./rebar3 /usr/local/bin/ 	&& rm -rf /usr/src/rebar3-src 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Thu, 07 Sep 2023 02:03:51 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:6dd2d41f67a6666210e1a34694b8765e945a44014b53252ec0e1b50491e08d69`  
		Last Modified: Thu, 07 Sep 2023 00:49:54 GMT  
		Size: 53.3 MB (53290217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4622190453fc7e533b301540fbfccd6b62dd6e67bc2deffad6e4849ed4f266e5`  
		Last Modified: Thu, 07 Sep 2023 02:19:16 GMT  
		Size: 58.0 MB (58043122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
