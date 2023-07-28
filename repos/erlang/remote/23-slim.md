## `erlang:23-slim`

```console
$ docker pull erlang@sha256:5b0effd2faa6e7e493b1d607dd725a1494cd120e924df3b4d6927d089a78c0ab
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `erlang:23-slim` - linux; amd64

```console
$ docker pull erlang@sha256:50b81608b9d6e1231b2ea0ddc62731ab7d168ea44cf45337d88892f99a100063
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.4 MB (112357483 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:adfc09af8daf099ee13ddfcd45a3b245b5849d30dd8ec39f115ff5ccbff515ea`
-	Default Command: `["erl"]`

```dockerfile
# Thu, 27 Jul 2023 23:25:17 GMT
ADD file:46b31c893ada083f38702e21d80e5ea4b674cbc78bddd3d80020d7b8e8beb467 in / 
# Thu, 27 Jul 2023 23:25:18 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 01:16:20 GMT
ENV OTP_VERSION=23.3.4.19 REBAR3_VERSION=3.20.0
# Fri, 28 Jul 2023 01:16:20 GMT
LABEL org.opencontainers.image.version=23.3.4.19
# Fri, 28 Jul 2023 01:21:11 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="2b3b5ad2942c7f643cdf7e5b7af57f007e404f44caaa0a8ab288f4c3de23552f" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& REBAR3_DOWNLOAD_URL="https://github.com/erlang/rebar3/archive/${REBAR3_VERSION}.tar.gz" 	&& REBAR3_DOWNLOAD_SHA256="53ed7f294a8b8fb4d7d75988c69194943831c104d39832a1fa30307b1a8593de" 	&& mkdir -p /usr/src/rebar3-src 	&& curl -fSL -o rebar3-src.tar.gz "$REBAR3_DOWNLOAD_URL" 	&& echo "$REBAR3_DOWNLOAD_SHA256 rebar3-src.tar.gz" | sha256sum -c - 	&& tar -xzf rebar3-src.tar.gz -C /usr/src/rebar3-src --strip-components=1 	&& rm rebar3-src.tar.gz 	&& cd /usr/src/rebar3-src 	&& HOME=$PWD ./bootstrap 	&& install -v ./rebar3 /usr/local/bin/ 	&& rm -rf /usr/src/rebar3-src 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Fri, 28 Jul 2023 01:21:11 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:9918064ebccea7fc961fe71dad46105b217763b4b1b3a9dfa7bee2ab29d2039b`  
		Last Modified: Thu, 27 Jul 2023 23:30:27 GMT  
		Size: 50.5 MB (50497996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0066370640ec360902ab684d1ee17cd32fb556177d136b830287b3cb6209a4a`  
		Last Modified: Fri, 28 Jul 2023 01:44:08 GMT  
		Size: 61.9 MB (61859487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `erlang:23-slim` - linux; arm variant v7

```console
$ docker pull erlang@sha256:a4b8f11b5a13df7d96c45d3f471afa40536b11dbb50f18b3418f75eb314dc7c1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.3 MB (106301398 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc173e67d19be0ebf1fcad6587d4f54ed0d9163769671e45f18198f98aae166a`
-	Default Command: `["erl"]`

```dockerfile
# Thu, 27 Jul 2023 23:58:31 GMT
ADD file:234aa079d01de7f7d69cc8831073e3937debd44f772b3a29bbc3d9cac070812c in / 
# Thu, 27 Jul 2023 23:58:31 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 02:57:39 GMT
ENV OTP_VERSION=23.3.4.19 REBAR3_VERSION=3.20.0
# Fri, 28 Jul 2023 02:57:39 GMT
LABEL org.opencontainers.image.version=23.3.4.19
# Fri, 28 Jul 2023 03:02:17 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="2b3b5ad2942c7f643cdf7e5b7af57f007e404f44caaa0a8ab288f4c3de23552f" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& REBAR3_DOWNLOAD_URL="https://github.com/erlang/rebar3/archive/${REBAR3_VERSION}.tar.gz" 	&& REBAR3_DOWNLOAD_SHA256="53ed7f294a8b8fb4d7d75988c69194943831c104d39832a1fa30307b1a8593de" 	&& mkdir -p /usr/src/rebar3-src 	&& curl -fSL -o rebar3-src.tar.gz "$REBAR3_DOWNLOAD_URL" 	&& echo "$REBAR3_DOWNLOAD_SHA256 rebar3-src.tar.gz" | sha256sum -c - 	&& tar -xzf rebar3-src.tar.gz -C /usr/src/rebar3-src --strip-components=1 	&& rm rebar3-src.tar.gz 	&& cd /usr/src/rebar3-src 	&& HOME=$PWD ./bootstrap 	&& install -v ./rebar3 /usr/local/bin/ 	&& rm -rf /usr/src/rebar3-src 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Fri, 28 Jul 2023 03:02:17 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:3d63dc62bf43740491cd4bcda82a28e35ed3655623dd102a9fd80eec2889986c`  
		Last Modified: Fri, 28 Jul 2023 00:04:15 GMT  
		Size: 46.0 MB (45966204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86522066ddb3c50dc739f1947d8efe674511783cf7b807a983c482a59cc89074`  
		Last Modified: Fri, 28 Jul 2023 03:38:09 GMT  
		Size: 60.3 MB (60335194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `erlang:23-slim` - linux; arm64 variant v8

```console
$ docker pull erlang@sha256:bd8c658e7e974dea2ca61abaf667258af90ae07748673f8ade04ef42e019beb8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.0 MB (108045345 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9ec88c79777992501dd33783fc3eeb5597d94fa2b2405b7fa3ff0a5a049bc05`
-	Default Command: `["erl"]`

```dockerfile
# Thu, 27 Jul 2023 23:43:21 GMT
ADD file:7472c3a6e583fa549b0fdf510b32407a4ed40f255a30199cdd2c5fb367794d45 in / 
# Thu, 27 Jul 2023 23:43:21 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 02:55:20 GMT
ENV OTP_VERSION=23.3.4.19 REBAR3_VERSION=3.20.0
# Fri, 28 Jul 2023 02:55:21 GMT
LABEL org.opencontainers.image.version=23.3.4.19
# Fri, 28 Jul 2023 02:58:33 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="2b3b5ad2942c7f643cdf7e5b7af57f007e404f44caaa0a8ab288f4c3de23552f" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& REBAR3_DOWNLOAD_URL="https://github.com/erlang/rebar3/archive/${REBAR3_VERSION}.tar.gz" 	&& REBAR3_DOWNLOAD_SHA256="53ed7f294a8b8fb4d7d75988c69194943831c104d39832a1fa30307b1a8593de" 	&& mkdir -p /usr/src/rebar3-src 	&& curl -fSL -o rebar3-src.tar.gz "$REBAR3_DOWNLOAD_URL" 	&& echo "$REBAR3_DOWNLOAD_SHA256 rebar3-src.tar.gz" | sha256sum -c - 	&& tar -xzf rebar3-src.tar.gz -C /usr/src/rebar3-src --strip-components=1 	&& rm rebar3-src.tar.gz 	&& cd /usr/src/rebar3-src 	&& HOME=$PWD ./bootstrap 	&& install -v ./rebar3 /usr/local/bin/ 	&& rm -rf /usr/src/rebar3-src 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Fri, 28 Jul 2023 02:58:34 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:89b61c8397133d3e1d24ef0453eec8370033046cc0fc0854b595eb1e3c6d73e7`  
		Last Modified: Thu, 27 Jul 2023 23:47:32 GMT  
		Size: 49.3 MB (49290895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd7b3f4db88bb840d50577017abd939e6a202fbec1175c7bd6749f7a8b83e185`  
		Last Modified: Fri, 28 Jul 2023 03:29:01 GMT  
		Size: 58.8 MB (58754450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `erlang:23-slim` - linux; 386

```console
$ docker pull erlang@sha256:add358c9550e30677dcd9ed3c6924640f0ac94921da05778448e5dc9843bc2c4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.5 MB (112465371 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5fe76fa99838349d5dc13ac7ae4b8a65256c278c58602d8b90ddbe935e1d029`
-	Default Command: `["erl"]`

```dockerfile
# Thu, 27 Jul 2023 23:39:29 GMT
ADD file:a4caa39d69b463e1f2628cb32f33763655fd873129cf98dd26c431183c53b6d6 in / 
# Thu, 27 Jul 2023 23:39:29 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 19:47:06 GMT
ENV OTP_VERSION=23.3.4.19 REBAR3_VERSION=3.20.0
# Fri, 28 Jul 2023 19:47:06 GMT
LABEL org.opencontainers.image.version=23.3.4.19
# Fri, 28 Jul 2023 19:55:16 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="2b3b5ad2942c7f643cdf7e5b7af57f007e404f44caaa0a8ab288f4c3de23552f" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& REBAR3_DOWNLOAD_URL="https://github.com/erlang/rebar3/archive/${REBAR3_VERSION}.tar.gz" 	&& REBAR3_DOWNLOAD_SHA256="53ed7f294a8b8fb4d7d75988c69194943831c104d39832a1fa30307b1a8593de" 	&& mkdir -p /usr/src/rebar3-src 	&& curl -fSL -o rebar3-src.tar.gz "$REBAR3_DOWNLOAD_URL" 	&& echo "$REBAR3_DOWNLOAD_SHA256 rebar3-src.tar.gz" | sha256sum -c - 	&& tar -xzf rebar3-src.tar.gz -C /usr/src/rebar3-src --strip-components=1 	&& rm rebar3-src.tar.gz 	&& cd /usr/src/rebar3-src 	&& HOME=$PWD ./bootstrap 	&& install -v ./rebar3 /usr/local/bin/ 	&& rm -rf /usr/src/rebar3-src 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Fri, 28 Jul 2023 19:55:17 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:4b5eb5e3691ae17e5aaa83c175523a7a17d58c9c61698ed6bba826d9acc809ec`  
		Last Modified: Thu, 27 Jul 2023 23:44:34 GMT  
		Size: 51.3 MB (51255427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad893a3fb9314983d8cbd1faa75dcd2734021a6ef43af43990535ab891ba8f24`  
		Last Modified: Fri, 28 Jul 2023 21:20:06 GMT  
		Size: 61.2 MB (61209944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
