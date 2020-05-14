## `erlang:23-slim`

```console
$ docker pull erlang@sha256:90b7e50854d2182f258ba49795f166e85bd0d30b41acc1fe72d01e5b050f5c83
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
$ docker pull erlang@sha256:2eaa8384ce19ad31a851d90fa16d55d4cf939ae111e3272611be7db15c6de3a7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.3 MB (110329302 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c275d6cb2848710b86c1f09c008322d3dfd88269be5fa4730f812d1f39873917`
-	Default Command: `["erl"]`

```dockerfile
# Thu, 23 Apr 2020 00:20:17 GMT
ADD file:f086177965196842af3c15f50a7f6ad7912aaa7bf73a60b1d00e3129265eec9a in / 
# Thu, 23 Apr 2020 00:20:17 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 04:36:11 GMT
ENV OTP_VERSION=23.0-rc3
# Thu, 23 Apr 2020 04:36:11 GMT
LABEL org.opencontainers.image.version=23.0-rc3
# Thu, 23 Apr 2020 04:51:38 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="2e23ab9042743803c5b6da0a6380afdc3ed7137f52f7afe801fc022f8de8fc83" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Thu, 23 Apr 2020 04:51:39 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:90fe46dd819953eb995f9cc9c326130abe9dd0b3993a998e12c01d0218a0b831`  
		Last Modified: Thu, 23 Apr 2020 00:24:56 GMT  
		Size: 50.4 MB (50382927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a05224f987fe5d742800d0b738fe2d53d5ed70cc855b8ca8349374f622a8a040`  
		Last Modified: Thu, 23 Apr 2020 08:01:25 GMT  
		Size: 59.9 MB (59946375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `erlang:23-slim` - linux; arm variant v7

```console
$ docker pull erlang@sha256:ad0b98ca31e484b900f2df543422e2a4c565d1b68e5587ac79075cc09df8ff53
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.7 MB (101654833 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07a8e5a07adf5590fe8af03be5c0816d9e8612dd32feba3797c89005ba21b984`
-	Default Command: `["erl"]`

```dockerfile
# Wed, 13 May 2020 21:13:33 GMT
ADD file:8a00a4e8b308e132c6e665ca4e517d4f8b3ba171a2f539903029bc01271087d7 in / 
# Wed, 13 May 2020 21:13:36 GMT
CMD ["bash"]
# Wed, 13 May 2020 22:28:17 GMT
ENV OTP_VERSION=23.0-rc3
# Wed, 13 May 2020 22:28:18 GMT
LABEL org.opencontainers.image.version=23.0-rc3
# Wed, 13 May 2020 22:35:17 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="2e23ab9042743803c5b6da0a6380afdc3ed7137f52f7afe801fc022f8de8fc83" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Wed, 13 May 2020 22:35:21 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:152c1d0ea8a0c219e7a54e8b39fa0bc45d7a9e072c2388cb928448e26aed5418`  
		Last Modified: Wed, 13 May 2020 21:23:12 GMT  
		Size: 45.9 MB (45871321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f70cc2429a1a5360d824cfd6fb8d5d6dd13dd9111506cb6c0d4a0e852b045bd0`  
		Last Modified: Wed, 13 May 2020 23:17:45 GMT  
		Size: 55.8 MB (55783512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `erlang:23-slim` - linux; arm64 variant v8

```console
$ docker pull erlang@sha256:2a36c759ffad60e8e385d0772342390ed3b44cf8dc97b17708f2bea6ac74f945
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.0 MB (106042230 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a382b21be62be328e7512e0ed07a319942aab5d0d4176d29969c19a6c4b39b3`
-	Default Command: `["erl"]`

```dockerfile
# Wed, 13 May 2020 21:43:08 GMT
ADD file:685903e2621502d2f743969aaf293a5feab58680a95cd93a5ebf2b07f3b5d358 in / 
# Wed, 13 May 2020 21:43:10 GMT
CMD ["bash"]
# Wed, 13 May 2020 22:54:24 GMT
ENV OTP_VERSION=23.0-rc3
# Wed, 13 May 2020 22:54:24 GMT
LABEL org.opencontainers.image.version=23.0-rc3
# Wed, 13 May 2020 23:01:05 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="2e23ab9042743803c5b6da0a6380afdc3ed7137f52f7afe801fc022f8de8fc83" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Wed, 13 May 2020 23:01:09 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:0be831822ade5f87765ba6ff26243b12a3ecd4c379df96483549a7992c1fd35b`  
		Last Modified: Wed, 13 May 2020 21:52:50 GMT  
		Size: 49.2 MB (49168115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdac2640a1c6ee5825a7d2b8d29a3c5a1eedd867ad42c652e41fe657839d6531`  
		Last Modified: Thu, 14 May 2020 00:42:39 GMT  
		Size: 56.9 MB (56874115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `erlang:23-slim` - linux; 386

```console
$ docker pull erlang@sha256:b0df8790954619e7b4105f728dcad6611d86ca219c80084a434bc5054bfd7fef
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.5 MB (110503417 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dec535b513f1cddd9560ef3ba5d2c39815fd2c91f8b0f459c42150b17d85e395`
-	Default Command: `["erl"]`

```dockerfile
# Wed, 13 May 2020 21:39:08 GMT
ADD file:6aac8e08fe944df3eddb4f6d5754281e407717bf6c2ec1ed9b6ab6af21dd6ee8 in / 
# Wed, 13 May 2020 21:39:09 GMT
CMD ["bash"]
# Wed, 13 May 2020 22:07:00 GMT
ENV OTP_VERSION=23.0-rc3
# Wed, 13 May 2020 22:07:00 GMT
LABEL org.opencontainers.image.version=23.0-rc3
# Wed, 13 May 2020 22:18:52 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="2e23ab9042743803c5b6da0a6380afdc3ed7137f52f7afe801fc022f8de8fc83" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Wed, 13 May 2020 22:18:52 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:adf8f9afd28c61bb1494b99fd6560afa547f46892f87c9847b019ac6d551809e`  
		Last Modified: Wed, 13 May 2020 21:46:14 GMT  
		Size: 51.2 MB (51153891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee90ebacad7c9c80bcb396caf09e1c78c1bdc6b0d6b60a1d787074d72e57f4a0`  
		Last Modified: Wed, 13 May 2020 23:35:31 GMT  
		Size: 59.3 MB (59349526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `erlang:23-slim` - linux; ppc64le

```console
$ docker pull erlang@sha256:aad8c9a134cb7124a95082d960e0aa3e9a16de9598bdeff36601a13789d92581
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.9 MB (111922616 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c35fc66b6c51cb10e458ede0f6a4e3e8e05a6832a64d1cb3a1a803bd3531816e`
-	Default Command: `["erl"]`

```dockerfile
# Thu, 23 Apr 2020 00:34:50 GMT
ADD file:31369dd617691a0d7181117a065290be8cd8c32814e443ef0a7c7adf7e9d800a in / 
# Thu, 23 Apr 2020 00:34:54 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 03:13:07 GMT
ENV OTP_VERSION=23.0-rc3
# Thu, 23 Apr 2020 03:13:10 GMT
LABEL org.opencontainers.image.version=23.0-rc3
# Thu, 23 Apr 2020 03:22:12 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="2e23ab9042743803c5b6da0a6380afdc3ed7137f52f7afe801fc022f8de8fc83" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Thu, 23 Apr 2020 03:22:20 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:6bf15800932473d1ca0a2cca9bfac073da118f1172b9027f7e78394850b02d05`  
		Last Modified: Thu, 23 Apr 2020 00:49:32 GMT  
		Size: 54.1 MB (54139621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d692f150b5be3674a822dc724a2a94186d92d38a67b6628772145c1c09774f6`  
		Last Modified: Thu, 23 Apr 2020 04:34:20 GMT  
		Size: 57.8 MB (57782995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `erlang:23-slim` - linux; s390x

```console
$ docker pull erlang@sha256:cbab4e817df05e4543660c4277acf0f3256e2e7aaa54c46949b29505dfa0d636
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.9 MB (105882769 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9471b850a08e9623ac8d0f718177b3a87972e3cbc46c16568dd29d342dbdc92b`
-	Default Command: `["erl"]`

```dockerfile
# Wed, 13 May 2020 21:42:20 GMT
ADD file:8f8ce7623c9f93bb85bf3b2bb1f2515de7b053e11c2efc56feb959322aefc0a0 in / 
# Wed, 13 May 2020 21:42:22 GMT
CMD ["bash"]
# Wed, 13 May 2020 22:05:21 GMT
ENV OTP_VERSION=23.0-rc3
# Wed, 13 May 2020 22:05:21 GMT
LABEL org.opencontainers.image.version=23.0-rc3
# Wed, 13 May 2020 22:09:09 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="2e23ab9042743803c5b6da0a6380afdc3ed7137f52f7afe801fc022f8de8fc83" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Wed, 13 May 2020 22:09:11 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:6542b1e7bcc740fe79dab47cd5bcdb30fe618acd5d0d0e2583571b2ed256809c`  
		Last Modified: Wed, 13 May 2020 21:46:45 GMT  
		Size: 49.0 MB (48965117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:834e477c7cc99e9d37cce612d7e4f0d63f7c870186e1b8223d1d7b132071f403`  
		Last Modified: Wed, 13 May 2020 22:34:59 GMT  
		Size: 56.9 MB (56917652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
