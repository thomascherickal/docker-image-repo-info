## `erlang:23-slim`

```console
$ docker pull erlang@sha256:15a88473670c6627773f85d716be8b66951f42336e7b9e70485e39dd2774fa1f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `erlang:23-slim` - linux; amd64

```console
$ docker pull erlang@sha256:e5aed9470c706e21d77ff3c5ffb456986301ab887400c085aa3c1dbacb513a16
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.7 MB (109712281 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:398b427b449f2e20192d01e209f61587eb0ac95e25501151f3c6dae5e54f0378`
-	Default Command: `["erl"]`

```dockerfile
# Wed, 26 Feb 2020 00:37:07 GMT
ADD file:e05e45c33042db4ec7f71a5952d65ee8cb3786dcd76fa7a990f48a2def1344e2 in / 
# Wed, 26 Feb 2020 00:37:07 GMT
CMD ["bash"]
# Fri, 06 Mar 2020 00:46:03 GMT
ENV OTP_VERSION=23.0-rc1
# Fri, 06 Mar 2020 00:46:03 GMT
LABEL org.opencontainers.image.version=23.0-rc1
# Fri, 06 Mar 2020 01:05:27 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="eca3c0cff83b536c5b96bff3d3b689b9fc25146a544d219aa5eee4c2a3c6d904" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Fri, 06 Mar 2020 01:05:28 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:50e431f790939a2f924af65084cc9d39c3d3fb9ad2d57d183b7eadf86ea46992`  
		Last Modified: Wed, 26 Feb 2020 00:44:04 GMT  
		Size: 50.4 MB (50381971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1be6b6baa9e3dfa96cdd80a4596561dfd487ab232b07c746453faa48e165579a`  
		Last Modified: Fri, 06 Mar 2020 02:19:55 GMT  
		Size: 59.3 MB (59330310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `erlang:23-slim` - linux; arm variant v7

```console
$ docker pull erlang@sha256:6ff5072e4410b6811e56fa98fc1f41639d60ddc8c23bc5fc51a412991797658c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.1 MB (101054951 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:550a24d1f4e080e01c02af109696a2a25f0242900fe72cd475d22cd93924abdd`
-	Default Command: `["erl"]`

```dockerfile
# Wed, 26 Feb 2020 00:50:58 GMT
ADD file:38fdfcc3155e437ce162aa0ed9dcdc5893b8145e2f3ede2858ed2187d79bf718 in / 
# Wed, 26 Feb 2020 00:51:08 GMT
CMD ["bash"]
# Fri, 06 Mar 2020 00:10:54 GMT
ENV OTP_VERSION=23.0-rc1
# Fri, 06 Mar 2020 00:10:54 GMT
LABEL org.opencontainers.image.version=23.0-rc1
# Fri, 06 Mar 2020 00:17:41 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="eca3c0cff83b536c5b96bff3d3b689b9fc25146a544d219aa5eee4c2a3c6d904" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Fri, 06 Mar 2020 00:17:42 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:3182cf45068cd9734abd8e38dedbb9930ede35ee8c11376ca2684e86f9a1aa85`  
		Last Modified: Wed, 26 Feb 2020 01:07:03 GMT  
		Size: 45.9 MB (45862691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8695b1a727d83ceb100e236c2bfef24f1023fdcb1318dbcec6bfc6238fd1a77d`  
		Last Modified: Fri, 06 Mar 2020 00:50:14 GMT  
		Size: 55.2 MB (55192260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `erlang:23-slim` - linux; arm64 variant v8

```console
$ docker pull erlang@sha256:b60042cefa49235743102b44f374ba1ebc3442eef6e9f69c3304eaa89e461a71
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.4 MB (105418118 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64df5c2beab217c5ee44993bed3d4f5184a35e94ea98aa65a11f6e092a441e04`
-	Default Command: `["erl"]`

```dockerfile
# Wed, 26 Feb 2020 00:46:17 GMT
ADD file:e3320653f0d517a6181aa46fb47407790018e2d8dee590005ffdbee3d04f72d4 in / 
# Wed, 26 Feb 2020 00:46:19 GMT
CMD ["bash"]
# Fri, 06 Mar 2020 00:53:45 GMT
ENV OTP_VERSION=23.0-rc1
# Fri, 06 Mar 2020 00:53:47 GMT
LABEL org.opencontainers.image.version=23.0-rc1
# Fri, 06 Mar 2020 01:01:34 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="eca3c0cff83b536c5b96bff3d3b689b9fc25146a544d219aa5eee4c2a3c6d904" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Fri, 06 Mar 2020 01:01:37 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:77b067f4ec14d48dbc8cd83b7a46fbb5f21fe01ea8911db256cc0168a30c1f5b`  
		Last Modified: Wed, 26 Feb 2020 00:55:50 GMT  
		Size: 49.2 MB (49169974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:882a74ddb477be761fc8b86945fdba20cb3879d53cc57b5719c32c39fbc816f4`  
		Last Modified: Fri, 06 Mar 2020 01:34:20 GMT  
		Size: 56.2 MB (56248144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `erlang:23-slim` - linux; 386

```console
$ docker pull erlang@sha256:f1db9ea1b339095f39fae82193e29eeb9bdb56d4a0f76e362b972968151d619e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.9 MB (109885312 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24233e16a7ed531ca2b299f29c7f44da56d55e135c37b6da78ba5343fe0aa18e`
-	Default Command: `["erl"]`

```dockerfile
# Wed, 26 Feb 2020 00:31:58 GMT
ADD file:1deff975480520310bf2c8d3708554d98c696f82689f0b67f9a834217c861803 in / 
# Wed, 26 Feb 2020 00:31:59 GMT
CMD ["bash"]
# Fri, 06 Mar 2020 01:45:39 GMT
ENV OTP_VERSION=23.0-rc1
# Fri, 06 Mar 2020 01:45:40 GMT
LABEL org.opencontainers.image.version=23.0-rc1
# Fri, 06 Mar 2020 02:02:39 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="eca3c0cff83b536c5b96bff3d3b689b9fc25146a544d219aa5eee4c2a3c6d904" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Fri, 06 Mar 2020 02:02:39 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:9450e7c48681b3ba36935d4e7d891b4b180d4d223a6c938faacb41402857ebd3`  
		Last Modified: Wed, 26 Feb 2020 00:38:12 GMT  
		Size: 51.1 MB (51146129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d754569feafd79de5618240795b6de80db87e160c6c7b54aec630a6a74cb4bcf`  
		Last Modified: Fri, 06 Mar 2020 03:09:10 GMT  
		Size: 58.7 MB (58739183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `erlang:23-slim` - linux; ppc64le

```console
$ docker pull erlang@sha256:43aca684e784b905013a8c8b9214acaabcc95e2323cf40dfab376dc99e11cf2d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.3 MB (111258541 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a214988870064d0413e11563ec3e8762086a8a3fe21e7f028c4418cbd3fe21bd`
-	Default Command: `["erl"]`

```dockerfile
# Wed, 26 Feb 2020 01:30:27 GMT
ADD file:b58865b3fd36d440998ef82e567179a9cd6b9ce0343d5e5a15a0b4f856f211c7 in / 
# Wed, 26 Feb 2020 01:30:35 GMT
CMD ["bash"]
# Fri, 06 Mar 2020 00:38:08 GMT
ENV OTP_VERSION=23.0-rc1
# Fri, 06 Mar 2020 00:38:11 GMT
LABEL org.opencontainers.image.version=23.0-rc1
# Fri, 06 Mar 2020 00:47:56 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="eca3c0cff83b536c5b96bff3d3b689b9fc25146a544d219aa5eee4c2a3c6d904" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Fri, 06 Mar 2020 00:48:04 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:928614537d6dedbdf79cc24c5c56bf98c3ed88f9d91a9ec1105d2a133611b0fd`  
		Last Modified: Wed, 26 Feb 2020 01:49:54 GMT  
		Size: 54.1 MB (54138444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0be593cd7b43732ecac1ccac6a6e8d1608c41cd102b541129993dcc53b99a4d1`  
		Last Modified: Fri, 06 Mar 2020 01:29:24 GMT  
		Size: 57.1 MB (57120097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `erlang:23-slim` - linux; s390x

```console
$ docker pull erlang@sha256:97eca453d2569b985c58098ea3686529522a2487e390c3e88f33cf3a80433555
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.2 MB (105242920 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d77f4734716079fe282c21fda3095cd6db6fb4cc272a2cd49fc6acb1ede563d5`
-	Default Command: `["erl"]`

```dockerfile
# Wed, 26 Feb 2020 00:42:32 GMT
ADD file:80536bfff518f6b425ad359b86a124f79ccdc82deb3e648f1746a7c87a1fcad0 in / 
# Wed, 26 Feb 2020 00:42:35 GMT
CMD ["bash"]
# Fri, 06 Mar 2020 01:01:04 GMT
ENV OTP_VERSION=23.0-rc1
# Fri, 06 Mar 2020 01:01:04 GMT
LABEL org.opencontainers.image.version=23.0-rc1
# Fri, 06 Mar 2020 01:09:11 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="eca3c0cff83b536c5b96bff3d3b689b9fc25146a544d219aa5eee4c2a3c6d904" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Fri, 06 Mar 2020 01:09:19 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:0a3603da42bb9e22573006a7f894b198954caeab529e2e041660e12c4fe62462`  
		Last Modified: Wed, 26 Feb 2020 00:47:26 GMT  
		Size: 49.0 MB (48958029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ff3e95262fce596f8b95181c5da5a155d5cec0a504bfafb5ea08ee92d439ef5`  
		Last Modified: Fri, 06 Mar 2020 01:43:55 GMT  
		Size: 56.3 MB (56284891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
