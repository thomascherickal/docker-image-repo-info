## `erlang:24-slim`

```console
$ docker pull erlang@sha256:cef342afa2a22b3557392f63f812c02f1c77f9d72246a026cd555c91f81c4292
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

### `erlang:24-slim` - linux; amd64

```console
$ docker pull erlang@sha256:bd900743feaef879ebae5638478da434e7981195ba7ba49eb3391856eb7e1cda
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.2 MB (120244228 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97497000f881373b47865ae93943d1a50e1b0c259c943b3738b5943c9c8058ea`
-	Default Command: `["erl"]`

```dockerfile
# Wed, 12 Apr 2023 00:19:55 GMT
ADD file:f2d012660f882f319a5878a3f9ce285f488b8f90fad49ad238541cf72089e035 in / 
# Wed, 12 Apr 2023 00:19:56 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 00:54:31 GMT
ENV OTP_VERSION=24.3.4.10 REBAR3_VERSION=3.20.0
# Wed, 12 Apr 2023 00:54:32 GMT
LABEL org.opencontainers.image.version=24.3.4.10
# Wed, 12 Apr 2023 00:58:53 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="14d01d18601c1460de847ff8c4434d8e20fc322b5291766c3fe35f50907bb7a9" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& REBAR3_DOWNLOAD_URL="https://github.com/erlang/rebar3/archive/${REBAR3_VERSION}.tar.gz" 	&& REBAR3_DOWNLOAD_SHA256="53ed7f294a8b8fb4d7d75988c69194943831c104d39832a1fa30307b1a8593de" 	&& mkdir -p /usr/src/rebar3-src 	&& curl -fSL -o rebar3-src.tar.gz "$REBAR3_DOWNLOAD_URL" 	&& echo "$REBAR3_DOWNLOAD_SHA256 rebar3-src.tar.gz" | sha256sum -c - 	&& tar -xzf rebar3-src.tar.gz -C /usr/src/rebar3-src --strip-components=1 	&& rm rebar3-src.tar.gz 	&& cd /usr/src/rebar3-src 	&& HOME=$PWD ./bootstrap 	&& install -v ./rebar3 /usr/local/bin/ 	&& rm -rf /usr/src/rebar3-src 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Wed, 12 Apr 2023 00:58:54 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:b0248cf3e63c73d0e496a67807d056ca41d5e968b61087e8eca2cf4b9b4d7b99`  
		Last Modified: Wed, 12 Apr 2023 00:23:20 GMT  
		Size: 55.1 MB (55052736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cb3b47743452f54286c563cc7a7f36960cab2b0d34b3d0c4ff662019b1b4b57`  
		Last Modified: Wed, 12 Apr 2023 01:27:50 GMT  
		Size: 65.2 MB (65191492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `erlang:24-slim` - linux; arm variant v5

```console
$ docker pull erlang@sha256:ae39f921337f52af21a199ab5506a5a393dd96b2954f967d0ffa662dadfec7a2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.9 MB (109934394 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47ae564ce29915cd65f84d75ab20dc1deba6fd5ba9d10f9b2481b1804925146d`
-	Default Command: `["erl"]`

```dockerfile
# Wed, 12 Apr 2023 00:48:34 GMT
ADD file:ae13a4cbeb20b92ec29dd7409de47a964fe373bdde2a4e8880b5a4d9dc64171e in / 
# Wed, 12 Apr 2023 00:48:35 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:55:56 GMT
ENV OTP_VERSION=24.3.4.10 REBAR3_VERSION=3.20.0
# Wed, 12 Apr 2023 01:55:56 GMT
LABEL org.opencontainers.image.version=24.3.4.10
# Wed, 12 Apr 2023 02:00:17 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="14d01d18601c1460de847ff8c4434d8e20fc322b5291766c3fe35f50907bb7a9" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& REBAR3_DOWNLOAD_URL="https://github.com/erlang/rebar3/archive/${REBAR3_VERSION}.tar.gz" 	&& REBAR3_DOWNLOAD_SHA256="53ed7f294a8b8fb4d7d75988c69194943831c104d39832a1fa30307b1a8593de" 	&& mkdir -p /usr/src/rebar3-src 	&& curl -fSL -o rebar3-src.tar.gz "$REBAR3_DOWNLOAD_URL" 	&& echo "$REBAR3_DOWNLOAD_SHA256 rebar3-src.tar.gz" | sha256sum -c - 	&& tar -xzf rebar3-src.tar.gz -C /usr/src/rebar3-src --strip-components=1 	&& rm rebar3-src.tar.gz 	&& cd /usr/src/rebar3-src 	&& HOME=$PWD ./bootstrap 	&& install -v ./rebar3 /usr/local/bin/ 	&& rm -rf /usr/src/rebar3-src 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Wed, 12 Apr 2023 02:00:18 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:86cb8d774eca43d428d6a35506c172ba62358d2d5ec90c886e3b38b297f93b20`  
		Last Modified: Wed, 12 Apr 2023 00:50:46 GMT  
		Size: 52.6 MB (52555175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:380a0789284311b25fb3ef472cc8a879f05fd20dcfc05b934f77aedb0f74fcdd`  
		Last Modified: Wed, 12 Apr 2023 02:04:43 GMT  
		Size: 57.4 MB (57379219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `erlang:24-slim` - linux; arm variant v7

```console
$ docker pull erlang@sha256:87a67705154759a78d575a5806e040e8e30e6a56c39bca3069ca693702456919
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.4 MB (107379719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bce6f6f3e00318cfdfe6393b5ed904f3b758447d1a0bece5a51497b3de3d2b01`
-	Default Command: `["erl"]`

```dockerfile
# Tue, 11 Apr 2023 23:59:35 GMT
ADD file:75c57df33c95251a80549b7949853df282a42bc4e5f19176764907a54b74caa9 in / 
# Tue, 11 Apr 2023 23:59:36 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 07:44:13 GMT
ENV OTP_VERSION=24.3.4.10 REBAR3_VERSION=3.20.0
# Wed, 12 Apr 2023 07:44:13 GMT
LABEL org.opencontainers.image.version=24.3.4.10
# Wed, 12 Apr 2023 07:48:14 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="14d01d18601c1460de847ff8c4434d8e20fc322b5291766c3fe35f50907bb7a9" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& REBAR3_DOWNLOAD_URL="https://github.com/erlang/rebar3/archive/${REBAR3_VERSION}.tar.gz" 	&& REBAR3_DOWNLOAD_SHA256="53ed7f294a8b8fb4d7d75988c69194943831c104d39832a1fa30307b1a8593de" 	&& mkdir -p /usr/src/rebar3-src 	&& curl -fSL -o rebar3-src.tar.gz "$REBAR3_DOWNLOAD_URL" 	&& echo "$REBAR3_DOWNLOAD_SHA256 rebar3-src.tar.gz" | sha256sum -c - 	&& tar -xzf rebar3-src.tar.gz -C /usr/src/rebar3-src --strip-components=1 	&& rm rebar3-src.tar.gz 	&& cd /usr/src/rebar3-src 	&& HOME=$PWD ./bootstrap 	&& install -v ./rebar3 /usr/local/bin/ 	&& rm -rf /usr/src/rebar3-src 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Wed, 12 Apr 2023 07:48:14 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:4feff9b88735325634445419eaaec2ed47500b63027cfd2de34b8bc6d55ee85c`  
		Last Modified: Wed, 12 Apr 2023 00:02:57 GMT  
		Size: 50.2 MB (50216882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:439a1c8ccefc1b99e43b513a7be02514ea4f5d62d12644c6dcea1314de190263`  
		Last Modified: Wed, 12 Apr 2023 08:08:11 GMT  
		Size: 57.2 MB (57162837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `erlang:24-slim` - linux; arm64 variant v8

```console
$ docker pull erlang@sha256:1cac3f9abafb35093b2e129375b7080c46d1fd9607809d879cae3f7ab026e319
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111727892 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c793c93391cf1c48f35106b2ff4e57169f4e5f8454c930d5a41ada9112a5f406`
-	Default Command: `["erl"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:42 GMT
ADD file:dd3d4e5fe819950e7d01b44a29dbd790438cd722ba76198910e2597448ab0c6f in / 
# Wed, 12 Apr 2023 00:39:43 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 02:29:48 GMT
ENV OTP_VERSION=24.3.4.10 REBAR3_VERSION=3.20.0
# Wed, 12 Apr 2023 02:29:48 GMT
LABEL org.opencontainers.image.version=24.3.4.10
# Wed, 12 Apr 2023 02:32:51 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="14d01d18601c1460de847ff8c4434d8e20fc322b5291766c3fe35f50907bb7a9" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& REBAR3_DOWNLOAD_URL="https://github.com/erlang/rebar3/archive/${REBAR3_VERSION}.tar.gz" 	&& REBAR3_DOWNLOAD_SHA256="53ed7f294a8b8fb4d7d75988c69194943831c104d39832a1fa30307b1a8593de" 	&& mkdir -p /usr/src/rebar3-src 	&& curl -fSL -o rebar3-src.tar.gz "$REBAR3_DOWNLOAD_URL" 	&& echo "$REBAR3_DOWNLOAD_SHA256 rebar3-src.tar.gz" | sha256sum -c - 	&& tar -xzf rebar3-src.tar.gz -C /usr/src/rebar3-src --strip-components=1 	&& rm rebar3-src.tar.gz 	&& cd /usr/src/rebar3-src 	&& HOME=$PWD ./bootstrap 	&& install -v ./rebar3 /usr/local/bin/ 	&& rm -rf /usr/src/rebar3-src 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Wed, 12 Apr 2023 02:32:52 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:dc80b8cdbfd36cb20231d807a50d704945d1df4da8f6e23197ccfcb629970491`  
		Last Modified: Wed, 12 Apr 2023 00:42:14 GMT  
		Size: 53.7 MB (53705529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b85d9f0f2675097e79e59b637bb91cb8c3dca75bbf9d92d7861913e2b39341a8`  
		Last Modified: Wed, 12 Apr 2023 03:10:36 GMT  
		Size: 58.0 MB (58022363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `erlang:24-slim` - linux; 386

```console
$ docker pull erlang@sha256:b00b9bc74f7b5ae594fa90b3f69c2a447c056d7ab597c0f3d1f6cab20ae87e89
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.7 MB (113677448 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e7bae803340c1d8a28238bd0a11204a496bb91bedbfdc624e8a57fae63946c3`
-	Default Command: `["erl"]`

```dockerfile
# Wed, 12 Apr 2023 00:38:51 GMT
ADD file:4da7e6af0782b21849e5f6385de3589ac5b8d81d173721f9990d32da754df2cb in / 
# Wed, 12 Apr 2023 00:38:51 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 02:15:16 GMT
ENV OTP_VERSION=24.3.4.10 REBAR3_VERSION=3.20.0
# Wed, 12 Apr 2023 02:15:16 GMT
LABEL org.opencontainers.image.version=24.3.4.10
# Wed, 12 Apr 2023 02:22:47 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="14d01d18601c1460de847ff8c4434d8e20fc322b5291766c3fe35f50907bb7a9" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& REBAR3_DOWNLOAD_URL="https://github.com/erlang/rebar3/archive/${REBAR3_VERSION}.tar.gz" 	&& REBAR3_DOWNLOAD_SHA256="53ed7f294a8b8fb4d7d75988c69194943831c104d39832a1fa30307b1a8593de" 	&& mkdir -p /usr/src/rebar3-src 	&& curl -fSL -o rebar3-src.tar.gz "$REBAR3_DOWNLOAD_URL" 	&& echo "$REBAR3_DOWNLOAD_SHA256 rebar3-src.tar.gz" | sha256sum -c - 	&& tar -xzf rebar3-src.tar.gz -C /usr/src/rebar3-src --strip-components=1 	&& rm rebar3-src.tar.gz 	&& cd /usr/src/rebar3-src 	&& HOME=$PWD ./bootstrap 	&& install -v ./rebar3 /usr/local/bin/ 	&& rm -rf /usr/src/rebar3-src 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Wed, 12 Apr 2023 02:22:47 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:b2bef40925391866903279768b0ae1e8233ef6a1aae64509a922f4aa96fe42a6`  
		Last Modified: Wed, 12 Apr 2023 00:42:19 GMT  
		Size: 56.0 MB (56032818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10841a693a0e1c8fb0cce6dfc160eb4ee115dcec39a32aba46d45ad31ddf8f94`  
		Last Modified: Wed, 12 Apr 2023 04:09:20 GMT  
		Size: 57.6 MB (57644630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `erlang:24-slim` - linux; mips64le

```console
$ docker pull erlang@sha256:aebe4fff6e219cb816c45bd31ac6a5ac8daf1618e8ae138f7fcd424ef535a474
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.5 MB (111529401 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cbb16a077a7039f3ec3b20dd3a7603a8b2290a288b6ac4f7ed99af1ccc58dc00`
-	Default Command: `["erl"]`

```dockerfile
# Thu, 23 Mar 2023 05:17:18 GMT
ADD file:2337efa705c8772705fa8519e513f4299e72c9eb63e3a68069778ca95a1511e6 in / 
# Thu, 23 Mar 2023 05:17:24 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 16:45:43 GMT
ENV OTP_VERSION=24.3.4.10 REBAR3_VERSION=3.20.0
# Thu, 23 Mar 2023 16:45:46 GMT
LABEL org.opencontainers.image.version=24.3.4.10
# Thu, 23 Mar 2023 17:06:36 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="14d01d18601c1460de847ff8c4434d8e20fc322b5291766c3fe35f50907bb7a9" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& REBAR3_DOWNLOAD_URL="https://github.com/erlang/rebar3/archive/${REBAR3_VERSION}.tar.gz" 	&& REBAR3_DOWNLOAD_SHA256="53ed7f294a8b8fb4d7d75988c69194943831c104d39832a1fa30307b1a8593de" 	&& mkdir -p /usr/src/rebar3-src 	&& curl -fSL -o rebar3-src.tar.gz "$REBAR3_DOWNLOAD_URL" 	&& echo "$REBAR3_DOWNLOAD_SHA256 rebar3-src.tar.gz" | sha256sum -c - 	&& tar -xzf rebar3-src.tar.gz -C /usr/src/rebar3-src --strip-components=1 	&& rm rebar3-src.tar.gz 	&& cd /usr/src/rebar3-src 	&& HOME=$PWD ./bootstrap 	&& install -v ./rebar3 /usr/local/bin/ 	&& rm -rf /usr/src/rebar3-src 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Thu, 23 Mar 2023 17:06:40 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:f3951ee58695b4d906b37f2d9a07e6158f66a7328d0c70445d9607cd8367ede0`  
		Last Modified: Thu, 23 Mar 2023 05:25:08 GMT  
		Size: 53.3 MB (53264720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1521c48095585774dbaf334b00ce27e3b03f38d15997d545af3ddc6d05ed4fee`  
		Last Modified: Thu, 23 Mar 2023 17:16:07 GMT  
		Size: 58.3 MB (58264681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `erlang:24-slim` - linux; ppc64le

```console
$ docker pull erlang@sha256:cd5915f7f8c757743e845d23238093cb16e9440d12d8ea805cbdd5da7bc14e04
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.5 MB (117526589 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f3f2eb77e1b53e1650fd890525f32030b426b586b632279edfd2318c662ef20`
-	Default Command: `["erl"]`

```dockerfile
# Wed, 12 Apr 2023 00:07:58 GMT
ADD file:c3c2a10473ddaa3d8a30ca99b19ad3599d0e60d826c4e0315bdb7463352ebc09 in / 
# Wed, 12 Apr 2023 00:08:02 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:47:51 GMT
ENV OTP_VERSION=24.3.4.10 REBAR3_VERSION=3.20.0
# Wed, 12 Apr 2023 01:47:51 GMT
LABEL org.opencontainers.image.version=24.3.4.10
# Wed, 12 Apr 2023 01:57:26 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="14d01d18601c1460de847ff8c4434d8e20fc322b5291766c3fe35f50907bb7a9" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& REBAR3_DOWNLOAD_URL="https://github.com/erlang/rebar3/archive/${REBAR3_VERSION}.tar.gz" 	&& REBAR3_DOWNLOAD_SHA256="53ed7f294a8b8fb4d7d75988c69194943831c104d39832a1fa30307b1a8593de" 	&& mkdir -p /usr/src/rebar3-src 	&& curl -fSL -o rebar3-src.tar.gz "$REBAR3_DOWNLOAD_URL" 	&& echo "$REBAR3_DOWNLOAD_SHA256 rebar3-src.tar.gz" | sha256sum -c - 	&& tar -xzf rebar3-src.tar.gz -C /usr/src/rebar3-src --strip-components=1 	&& rm rebar3-src.tar.gz 	&& cd /usr/src/rebar3-src 	&& HOME=$PWD ./bootstrap 	&& install -v ./rebar3 /usr/local/bin/ 	&& rm -rf /usr/src/rebar3-src 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:57:33 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:2d3ffdd4610a019889b845cc82b3d956ad85cca78ad4bff2d5e5522bd02c17e7`  
		Last Modified: Wed, 12 Apr 2023 00:12:37 GMT  
		Size: 58.9 MB (58926600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d225fe0e6138f0d7a150dd92dcbfa2984727caa073e742e66946bb70c8e104df`  
		Last Modified: Wed, 12 Apr 2023 01:59:21 GMT  
		Size: 58.6 MB (58599989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `erlang:24-slim` - linux; s390x

```console
$ docker pull erlang@sha256:713696a0e304a04658ba5cfcb288277d3dea458961c1252f924e1cf9ef0fc375
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.4 MB (111414770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4bebed94cf67bec1598873fb77aff7126248f9d230dadf6d4dd1ad7ad9832170`
-	Default Command: `["erl"]`

```dockerfile
# Wed, 12 Apr 2023 00:00:25 GMT
ADD file:ab4e28724d04724a57e0f5bbe299d3361103f05ad1978dc3bfef243c1f9d6476 in / 
# Wed, 12 Apr 2023 00:00:38 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:23:59 GMT
ENV OTP_VERSION=24.3.4.10 REBAR3_VERSION=3.20.0
# Wed, 12 Apr 2023 01:23:59 GMT
LABEL org.opencontainers.image.version=24.3.4.10
# Wed, 12 Apr 2023 01:29:42 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="14d01d18601c1460de847ff8c4434d8e20fc322b5291766c3fe35f50907bb7a9" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& REBAR3_DOWNLOAD_URL="https://github.com/erlang/rebar3/archive/${REBAR3_VERSION}.tar.gz" 	&& REBAR3_DOWNLOAD_SHA256="53ed7f294a8b8fb4d7d75988c69194943831c104d39832a1fa30307b1a8593de" 	&& mkdir -p /usr/src/rebar3-src 	&& curl -fSL -o rebar3-src.tar.gz "$REBAR3_DOWNLOAD_URL" 	&& echo "$REBAR3_DOWNLOAD_SHA256 rebar3-src.tar.gz" | sha256sum -c - 	&& tar -xzf rebar3-src.tar.gz -C /usr/src/rebar3-src --strip-components=1 	&& rm rebar3-src.tar.gz 	&& cd /usr/src/rebar3-src 	&& HOME=$PWD ./bootstrap 	&& install -v ./rebar3 /usr/local/bin/ 	&& rm -rf /usr/src/rebar3-src 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:29:45 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:042263756d7dc47bf98a243871107aa3a2b41acda91d104d8b4e148749a43dda`  
		Last Modified: Wed, 12 Apr 2023 00:05:03 GMT  
		Size: 53.3 MB (53286682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5ab348f5af1d190336b874e41fb88bd120c9b4767b54cb03391c30fee2d2b96`  
		Last Modified: Wed, 12 Apr 2023 01:32:40 GMT  
		Size: 58.1 MB (58128088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
