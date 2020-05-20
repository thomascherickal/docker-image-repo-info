## `erlang:21-slim`

```console
$ docker pull erlang@sha256:e29cf1ecfda285f750717e6d379d62a65604acc4fa2801e2230cfaf3829b4b6c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `erlang:21-slim` - linux; amd64

```console
$ docker pull erlang@sha256:fa9fccae19392f0a43fb0036a0fa4b7e2e55d36c5a1754de1a2e06b6fe75cb96
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.6 MB (107592147 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a9dc3a77d81c3c33239583ec890fd26a8fa30a189b605a88d5c208c05f6a88d`
-	Default Command: `["erl"]`

```dockerfile
# Fri, 15 May 2020 06:33:25 GMT
ADD file:13031623172f5c5857e27de93553adedf17d955fa370882f850bb6ed6fb8cee7 in / 
# Fri, 15 May 2020 06:33:25 GMT
CMD ["bash"]
# Wed, 20 May 2020 19:19:50 GMT
ENV OTP_VERSION=21.3.8.16
# Wed, 20 May 2020 19:19:50 GMT
LABEL org.opencontainers.image.version=21.3.8.16
# Wed, 20 May 2020 19:40:03 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="c0a5b680d33d2c58bc16ce10ab9f4c37695b3d5b5a42ca880067e19c26ce4a44" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Wed, 20 May 2020 19:40:03 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:1c6172af85ee14a8db5a3a51d406b768dfa94d196c06d0d06d591507cf8199f0`  
		Last Modified: Fri, 15 May 2020 06:40:31 GMT  
		Size: 45.4 MB (45375207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbd6ae8a5f9e3a4811f7b9b24e94bcf8b87c0e11da34d800774b6597a73b442b`  
		Last Modified: Wed, 20 May 2020 20:03:46 GMT  
		Size: 62.2 MB (62216940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `erlang:21-slim` - linux; arm variant v7

```console
$ docker pull erlang@sha256:57a9319d5a9c1b90b3b1b8d4ab9476a6163cb604367b2b3f18356b558fd24358
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.2 MB (99174982 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d6b908046bce1d8d76ad8ad520c0e5050fdf811074c9f9bbb0600014f9c8b81`
-	Default Command: `["erl"]`

```dockerfile
# Fri, 15 May 2020 01:06:22 GMT
ADD file:89db8453485648b09e63411b6e2ad84f08844ee55cb115e59cdc8c8cb1c29a1f in / 
# Fri, 15 May 2020 01:06:23 GMT
CMD ["bash"]
# Wed, 20 May 2020 17:54:29 GMT
ENV OTP_VERSION=21.3.8.16
# Wed, 20 May 2020 17:54:30 GMT
LABEL org.opencontainers.image.version=21.3.8.16
# Wed, 20 May 2020 18:01:18 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="c0a5b680d33d2c58bc16ce10ab9f4c37695b3d5b5a42ca880067e19c26ce4a44" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Wed, 20 May 2020 18:01:20 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:11acdea2de14253903f5970d63a2076ff08912929430d1c33afe617c9fa6bf8f`  
		Last Modified: Fri, 15 May 2020 01:14:46 GMT  
		Size: 42.1 MB (42104346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:403f943fa9b223d1ec2c1e9e9b4cb918b00be6101d4ee9245b359d4d2b93440e`  
		Last Modified: Wed, 20 May 2020 18:13:32 GMT  
		Size: 57.1 MB (57070636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `erlang:21-slim` - linux; arm64 variant v8

```console
$ docker pull erlang@sha256:463d1d0d65c8d25edb7c601b379a0a623001bf51fd6584d024173dfe5bf7f20b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.4 MB (101449760 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2dfe5f4121406eb63a7d7c69b7d6365d979781d91becd1514ec49d54f54f4916`
-	Default Command: `["erl"]`

```dockerfile
# Fri, 15 May 2020 12:48:07 GMT
ADD file:251053dbd1ce0b3744de3eecf53a3ef8ccf92ea509678e59800952c3dbd1b32c in / 
# Fri, 15 May 2020 12:48:09 GMT
CMD ["bash"]
# Wed, 20 May 2020 18:43:34 GMT
ENV OTP_VERSION=21.3.8.16
# Wed, 20 May 2020 18:43:35 GMT
LABEL org.opencontainers.image.version=21.3.8.16
# Wed, 20 May 2020 18:51:31 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="c0a5b680d33d2c58bc16ce10ab9f4c37695b3d5b5a42ca880067e19c26ce4a44" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Wed, 20 May 2020 18:51:36 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:8e144e997aec62ed9c3bb1ff83ae2a62cbea252858abfb48ac60bb2078817a6c`  
		Last Modified: Fri, 15 May 2020 12:55:43 GMT  
		Size: 43.2 MB (43163052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd46deaf11289949c3facf7af430362a5e0727eab4f50c4b785b6e52c9f160c5`  
		Last Modified: Wed, 20 May 2020 19:04:24 GMT  
		Size: 58.3 MB (58286708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `erlang:21-slim` - linux; 386

```console
$ docker pull erlang@sha256:396973dc57aa6cde3ffb735622a73bf7d77efd454eba6a7c511bc5a3646d9786
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.3 MB (111307587 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e13079db163d83a330d859d8afc277adf69f93317294a167d3fa0824bf29e47c`
-	Default Command: `["erl"]`

```dockerfile
# Fri, 15 May 2020 07:12:19 GMT
ADD file:22284e8c6e684308a95b18c7ed63ef235582dbb1890d1d02c22213e41ae47192 in / 
# Fri, 15 May 2020 07:12:19 GMT
CMD ["bash"]
# Wed, 20 May 2020 20:03:57 GMT
ENV OTP_VERSION=21.3.8.16
# Wed, 20 May 2020 20:03:57 GMT
LABEL org.opencontainers.image.version=21.3.8.16
# Wed, 20 May 2020 20:17:15 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="c0a5b680d33d2c58bc16ce10ab9f4c37695b3d5b5a42ca880067e19c26ce4a44" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Wed, 20 May 2020 20:17:16 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:ddf311fc69760572da5334a35e5a0e9fa15690ee1e40ed4b06e9a65213bc7223`  
		Last Modified: Fri, 15 May 2020 07:22:51 GMT  
		Size: 46.1 MB (46094205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19b986ec3978c8e2d9c9cba27f2e9ae69301da6f3b104003c6fc1f6bc73521f2`  
		Last Modified: Wed, 20 May 2020 20:43:55 GMT  
		Size: 65.2 MB (65213382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `erlang:21-slim` - linux; ppc64le

```console
$ docker pull erlang@sha256:4e5354b1dff6833ab0d3b5a86bcf67f0733705c911e56b07a85ccf59c305181d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.8 MB (104821586 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c84950ec4f85c37c92573d74f0d0b70707e37d79a7dcd88558bc37880c7afa7f`
-	Default Command: `["erl"]`

```dockerfile
# Wed, 13 May 2020 22:39:29 GMT
ADD file:fa4c7e3ca04f092e53cc791a32c929663412df3f68de2733bb867053577bf1d1 in / 
# Wed, 13 May 2020 22:39:34 GMT
CMD ["bash"]
# Wed, 20 May 2020 19:23:01 GMT
ENV OTP_VERSION=21.3.8.16
# Wed, 20 May 2020 19:23:06 GMT
LABEL org.opencontainers.image.version=21.3.8.16
# Wed, 20 May 2020 19:35:20 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="c0a5b680d33d2c58bc16ce10ab9f4c37695b3d5b5a42ca880067e19c26ce4a44" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Wed, 20 May 2020 19:35:36 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:7732483b686efe14a1cf8add89a1568b83892e243798fba30808f1fc6287210b`  
		Last Modified: Wed, 13 May 2020 23:02:10 GMT  
		Size: 45.6 MB (45646193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40395db3ef633d9429e079796e390c699316edec0e5e9809af67ea22fb30cbe3`  
		Last Modified: Wed, 20 May 2020 19:48:46 GMT  
		Size: 59.2 MB (59175393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `erlang:21-slim` - linux; s390x

```console
$ docker pull erlang@sha256:2dbb11834acf66790a8abc29ea1e9103872d2bf37e9fc5fe4f6972e78472ae05
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.0 MB (105987848 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:25b776d760bc9eaf649a5e924620dfa36ea34665cc115c75f6e3b9605620221d`
-	Default Command: `["erl"]`

```dockerfile
# Thu, 14 May 2020 23:08:23 GMT
ADD file:32ad2f356c0ec407aa31085089417aaa9f72a5dc2757ed68a0adf7a432e4bdaa in / 
# Thu, 14 May 2020 23:08:26 GMT
CMD ["bash"]
# Wed, 20 May 2020 18:19:59 GMT
ENV OTP_VERSION=21.3.8.16
# Wed, 20 May 2020 18:19:59 GMT
LABEL org.opencontainers.image.version=21.3.8.16
# Wed, 20 May 2020 18:23:49 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="c0a5b680d33d2c58bc16ce10ab9f4c37695b3d5b5a42ca880067e19c26ce4a44" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Wed, 20 May 2020 18:23:52 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:dc69489da20ae5bdf6cefc772e7ff8420ffbd2c920a57165de6ead66d1a997e4`  
		Last Modified: Thu, 14 May 2020 23:12:48 GMT  
		Size: 45.2 MB (45232081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e2a22b25d7f51a081cdc02bc77baca28e3617fce6bfd07bf868d1d0859604de`  
		Last Modified: Wed, 20 May 2020 18:33:50 GMT  
		Size: 60.8 MB (60755767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
