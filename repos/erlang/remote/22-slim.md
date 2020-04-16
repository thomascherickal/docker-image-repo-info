## `erlang:22-slim`

```console
$ docker pull erlang@sha256:bf7bb5f600e84b42b8df9ef3e92d2f742eea39e362f3904f7e77d1eb08ef0b39
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `erlang:22-slim` - linux; amd64

```console
$ docker pull erlang@sha256:2ae5a0ff2f4aa5068c049bb19602c12e56205de61e0cb62446d6743c15ad7d82
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.9 MB (109899508 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:25e2ee73acf58e46275efbcc4721cfbe2813623940457fa20978f26a31f1401d`
-	Default Command: `["erl"]`

```dockerfile
# Thu, 16 Apr 2020 03:22:03 GMT
ADD file:a0c8e81c4c7fa85b43d4a9daaed7ba25964a0bf494711b6911cd4b7f5201a17f in / 
# Thu, 16 Apr 2020 03:22:03 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 05:55:38 GMT
ENV OTP_VERSION=22.3.2
# Thu, 16 Apr 2020 05:55:38 GMT
LABEL org.opencontainers.image.version=22.3.2
# Thu, 16 Apr 2020 06:10:41 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="4a3719c71a7998e4f57e73920439b4b1606f7c045e437a0f0f9f1613594d3eaa" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Thu, 16 Apr 2020 06:10:41 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:7e2b2a5af8f65687add6d864d5841067e23bd435eb1a051be6fe1ea2384946b4`  
		Last Modified: Thu, 16 Apr 2020 03:31:27 GMT  
		Size: 50.4 MB (50382957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76123bc96619b1103c1aa2c92cd32969d7539b6cc9b45ccdc99828d44a727dce`  
		Last Modified: Thu, 16 Apr 2020 08:34:48 GMT  
		Size: 59.5 MB (59516551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `erlang:22-slim` - linux; arm variant v7

```console
$ docker pull erlang@sha256:f19903f6f4845c2253fabd0f32bbb5ed47f11afa0ea916d0ce3b6191a71d639f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.2 MB (101157521 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8da58b14275234d758986d1a2862586b7e042b7400d4756bed0cb459ba133aa`
-	Default Command: `["erl"]`

```dockerfile
# Thu, 16 Apr 2020 00:59:14 GMT
ADD file:c2369e5669e570f90abaa1fd4fcea4ae1e6654bbd81e8fa070a5b2484c03ee74 in / 
# Thu, 16 Apr 2020 00:59:15 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 02:33:48 GMT
ENV OTP_VERSION=22.3.2
# Thu, 16 Apr 2020 02:33:49 GMT
LABEL org.opencontainers.image.version=22.3.2
# Thu, 16 Apr 2020 02:40:31 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="4a3719c71a7998e4f57e73920439b4b1606f7c045e437a0f0f9f1613594d3eaa" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Thu, 16 Apr 2020 02:40:36 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:020b29c91094d59c5eb128b7bc2b0b835e2ba4414358664e467428fe8b95bf52`  
		Last Modified: Thu, 16 Apr 2020 01:08:38 GMT  
		Size: 45.9 MB (45864371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ce59bc88686c1fa29f623cb797be12f56db4face19221e87a0d7abd2386061d`  
		Last Modified: Thu, 16 Apr 2020 04:06:53 GMT  
		Size: 55.3 MB (55293150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `erlang:22-slim` - linux; arm64 variant v8

```console
$ docker pull erlang@sha256:f4136ee3e37ffb5d182e232b8f130b14f30cbc9d72770d0935a730ad6d7c7888
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.6 MB (105610308 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa2c661f5a72ca9604446ce4af2ed85aa06f2e07b9a198e0d4c5cb6b898d263c`
-	Default Command: `["erl"]`

```dockerfile
# Thu, 16 Apr 2020 02:41:20 GMT
ADD file:02afb66e938cbc67271aaf8cbee75def87458a21d961d02e86383e0ed36b0c71 in / 
# Thu, 16 Apr 2020 02:41:24 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 04:06:43 GMT
ENV OTP_VERSION=22.3.2
# Thu, 16 Apr 2020 04:06:44 GMT
LABEL org.opencontainers.image.version=22.3.2
# Thu, 16 Apr 2020 04:13:04 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="4a3719c71a7998e4f57e73920439b4b1606f7c045e437a0f0f9f1613594d3eaa" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Thu, 16 Apr 2020 04:13:06 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:d080dad46627d4103daddf54c89f2ef0a0b72ba8270066c50e95ffbf4a79362e`  
		Last Modified: Thu, 16 Apr 2020 02:48:36 GMT  
		Size: 49.2 MB (49169521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dda404492e09596a6db2622da931cef9e9faea81271b428767145ba830024827`  
		Last Modified: Thu, 16 Apr 2020 05:37:57 GMT  
		Size: 56.4 MB (56440787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `erlang:22-slim` - linux; 386

```console
$ docker pull erlang@sha256:e7f42f628b607401b139d16ea8c4823b9d8bf6b89cca829d0ba03336ad1470d4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.0 MB (110039378 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:488d3fe9b28aeafa3f6df4b8f535c4657ba03787fb4bdeadf3e9b660bce78fcb`
-	Default Command: `["erl"]`

```dockerfile
# Thu, 16 Apr 2020 01:39:37 GMT
ADD file:9a9b9c1d98dfe76e20b3ed67b866e2bdbc1095e26de13b892d07f2a3ee062c83 in / 
# Thu, 16 Apr 2020 01:39:37 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 03:20:36 GMT
ENV OTP_VERSION=22.3.2
# Thu, 16 Apr 2020 03:20:36 GMT
LABEL org.opencontainers.image.version=22.3.2
# Thu, 16 Apr 2020 03:35:54 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="4a3719c71a7998e4f57e73920439b4b1606f7c045e437a0f0f9f1613594d3eaa" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Thu, 16 Apr 2020 03:35:54 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:6a29df432ebf22a237e5e0940a65a1f908be66a5204c5ef240ead7315c27335f`  
		Last Modified: Thu, 16 Apr 2020 01:46:01 GMT  
		Size: 51.1 MB (51147069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:928b780ff36812f23401e1a0a650f230e16f944ba3929a27e3bc91793c48dd11`  
		Last Modified: Thu, 16 Apr 2020 05:49:06 GMT  
		Size: 58.9 MB (58892309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `erlang:22-slim` - linux; ppc64le

```console
$ docker pull erlang@sha256:c42d2ee83c5f666f7298c55c5f62c4df799482cbf5c4e44da9ee08723448a39d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.5 MB (111481331 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:582073ee8384f5178d1e2aee1c425e9caf573ff86941489ddf1bc56170a811db`
-	Default Command: `["erl"]`

```dockerfile
# Thu, 16 Apr 2020 01:37:39 GMT
ADD file:5ea6b62430ec58194ba5685d0b5ecbc2df83c01b4e6c7d8b70f3e96c89390cd5 in / 
# Thu, 16 Apr 2020 01:37:47 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 08:13:06 GMT
ENV OTP_VERSION=22.3.2
# Thu, 16 Apr 2020 08:13:08 GMT
LABEL org.opencontainers.image.version=22.3.2
# Thu, 16 Apr 2020 08:22:39 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="4a3719c71a7998e4f57e73920439b4b1606f7c045e437a0f0f9f1613594d3eaa" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Thu, 16 Apr 2020 08:22:45 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:219153a374347511566d1327acf4e45fd3425c20cd49110ef8041930fdb965a4`  
		Last Modified: Thu, 16 Apr 2020 01:53:24 GMT  
		Size: 54.1 MB (54139564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32f46a35dccbec3322d2d7f73725a7e1820f7b73b9744a84aef8cee2358c29d1`  
		Last Modified: Thu, 16 Apr 2020 09:18:20 GMT  
		Size: 57.3 MB (57341767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `erlang:22-slim` - linux; s390x

```console
$ docker pull erlang@sha256:38c61287bfcb41a9275504db625e587de59bb69be09e8a281c55d36ea6ac5356
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.4 MB (105424234 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8290bc73c3ab88bb14b2f68756f4399ce4bf46d859b66b38e4fada3e97c7a68`
-	Default Command: `["erl"]`

```dockerfile
# Thu, 16 Apr 2020 00:42:03 GMT
ADD file:26367817216af13dc3ba9f495303f7bee8fe138fc8fb728289781563308ce0bd in / 
# Thu, 16 Apr 2020 00:42:05 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 02:36:40 GMT
ENV OTP_VERSION=22.3.2
# Thu, 16 Apr 2020 02:36:40 GMT
LABEL org.opencontainers.image.version=22.3.2
# Thu, 16 Apr 2020 02:40:47 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="4a3719c71a7998e4f57e73920439b4b1606f7c045e437a0f0f9f1613594d3eaa" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Thu, 16 Apr 2020 02:40:50 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:54e2fb160a5d4a95ec7efe70c0045923ee557e87ee68ce03f2150b8366f26729`  
		Last Modified: Thu, 16 Apr 2020 00:46:03 GMT  
		Size: 49.0 MB (48960213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28e28ee9202769cd87310f93c8bee3ae0b072ee7a000b5b366a2bbb2b171daea`  
		Last Modified: Thu, 16 Apr 2020 03:26:31 GMT  
		Size: 56.5 MB (56464021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
