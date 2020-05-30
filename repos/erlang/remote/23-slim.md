## `erlang:23-slim`

```console
$ docker pull erlang@sha256:f2f18f54c0d26e2cc2cc0dba61787157ef1f8782395723ae9bb85e12d05a0ff4
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
$ docker pull erlang@sha256:a0027fe480c943a5460ad4106395d2863d0106aabf0464101a55f594dc972b26
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.8 MB (110824906 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db33fe7b30c6d9591a658d2484b07300a60e92e8d48924a83d97ee0c7f3ec230`
-	Default Command: `["erl"]`

```dockerfile
# Fri, 15 May 2020 06:28:12 GMT
ADD file:fb54c709daa205bf9d04eb3d90ba068db4c34dfe3b6ec0d7691f677286120903 in / 
# Fri, 15 May 2020 06:28:13 GMT
CMD ["bash"]
# Fri, 29 May 2020 19:31:53 GMT
ENV OTP_VERSION=23.0.2
# Fri, 29 May 2020 19:31:54 GMT
LABEL org.opencontainers.image.version=23.0.2
# Fri, 29 May 2020 19:41:13 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="6bab92d1a1b20cc319cd845c23db3611cc99f8c99a610d117578262e3c108af3" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Fri, 29 May 2020 19:41:13 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:376057ac6fa17f65688c56977118e2e764b27c348b3f70637fa829cd2a12b200`  
		Last Modified: Fri, 15 May 2020 06:37:20 GMT  
		Size: 50.4 MB (50391294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5808c34635b4d4be72ed42e6bd34de1940ac070ae93301e7921b61986510c851`  
		Last Modified: Fri, 29 May 2020 19:58:16 GMT  
		Size: 60.4 MB (60433612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `erlang:23-slim` - linux; arm variant v7

```console
$ docker pull erlang@sha256:735aa71fad91173b0b3bada3afac58e60e098f9347943017323616787de81fdf
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.1 MB (102108515 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c4c55824658ee871ef201e9ac3a93997c7d5e141df14568c76ae0b75f3c48ec6`
-	Default Command: `["erl"]`

```dockerfile
# Fri, 15 May 2020 00:59:31 GMT
ADD file:d3b126babe4f145c735dff1d1a8828e523967279b9f25d547fce6f4d5422d0a4 in / 
# Fri, 15 May 2020 00:59:33 GMT
CMD ["bash"]
# Fri, 29 May 2020 19:08:47 GMT
ENV OTP_VERSION=23.0.2
# Fri, 29 May 2020 19:08:48 GMT
LABEL org.opencontainers.image.version=23.0.2
# Fri, 29 May 2020 19:15:15 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="6bab92d1a1b20cc319cd845c23db3611cc99f8c99a610d117578262e3c108af3" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Fri, 29 May 2020 19:15:17 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:33f1e205e6f963868048d05375e218b5a53592240c265ac49b4860e141d25c66`  
		Last Modified: Fri, 15 May 2020 01:11:01 GMT  
		Size: 45.9 MB (45868629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10725e5dd05a5bd54f8cd4aaacafa0d679e2a7e381ba1e512a565d5a4c0cd73d`  
		Last Modified: Fri, 29 May 2020 19:23:58 GMT  
		Size: 56.2 MB (56239886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `erlang:23-slim` - linux; arm64 variant v8

```console
$ docker pull erlang@sha256:28fd030508dca0fec028bd1d000586a79309b963b4489220d5a760f49a4e34d1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.5 MB (106527217 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0be9684f375304b01ee47af48a0f8b09c524f1bfa385d87852c8191543902786`
-	Default Command: `["erl"]`

```dockerfile
# Fri, 15 May 2020 12:43:21 GMT
ADD file:be06dd722febf4e72f7e626f70029986a5c75880941cabd553f695dd66bcbaff in / 
# Fri, 15 May 2020 12:43:25 GMT
CMD ["bash"]
# Fri, 29 May 2020 19:51:49 GMT
ENV OTP_VERSION=23.0.2
# Fri, 29 May 2020 19:51:49 GMT
LABEL org.opencontainers.image.version=23.0.2
# Fri, 29 May 2020 19:58:08 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="6bab92d1a1b20cc319cd845c23db3611cc99f8c99a610d117578262e3c108af3" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Fri, 29 May 2020 19:58:10 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:d23bf71de5e1fea32788576972e233e80db7c51d831ed7edb269102dab298bf1`  
		Last Modified: Fri, 15 May 2020 12:53:11 GMT  
		Size: 49.2 MB (49170530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e9a03dd591bbeb6452abe4dd9026d3aac67ca4543213989c1d8629f9956713c`  
		Last Modified: Fri, 29 May 2020 20:07:16 GMT  
		Size: 57.4 MB (57356687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `erlang:23-slim` - linux; 386

```console
$ docker pull erlang@sha256:860108cdc6bc27838763bd107f8d211655f106492e3e924909fefa0d5cbe9f05
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.9 MB (110941850 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb20dedacdd31db56ee58863eb76f824f89c9747ef19ec17144a22adf210e6ce`
-	Default Command: `["erl"]`

```dockerfile
# Fri, 15 May 2020 07:07:17 GMT
ADD file:8e3b513586e9ff0d65f88b3b2978986693585177fae673aa5432e2934e212cf1 in / 
# Fri, 15 May 2020 07:07:17 GMT
CMD ["bash"]
# Fri, 29 May 2020 19:56:50 GMT
ENV OTP_VERSION=23.0.2
# Fri, 29 May 2020 19:56:50 GMT
LABEL org.opencontainers.image.version=23.0.2
# Fri, 29 May 2020 20:06:08 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="6bab92d1a1b20cc319cd845c23db3611cc99f8c99a610d117578262e3c108af3" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Fri, 29 May 2020 20:06:08 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:8f68852a383b581a180c01bf6d2f7039194fed91451d0686630c59cb80d321c3`  
		Last Modified: Fri, 15 May 2020 07:17:49 GMT  
		Size: 51.2 MB (51157846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eff06e09b0a5bd6570a1159c5b416b6ec7f5d33e98fd880c3d89f4c5ac6f3620`  
		Last Modified: Fri, 29 May 2020 20:17:35 GMT  
		Size: 59.8 MB (59784004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `erlang:23-slim` - linux; ppc64le

```console
$ docker pull erlang@sha256:a3a545297b53fb8d4c5ba57e34884c73d7c992004dfcc3696884e22e5a284c50
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.4 MB (112428917 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a95f02a1c1285709b5c5d5d3cb9ec2fd12ed1a3ee199fbcbc43628e37141deea`
-	Default Command: `["erl"]`

```dockerfile
# Sat, 16 May 2020 17:05:45 GMT
ADD file:cbc72fbbd9297b44feea736c6c3446962657f02799b5f7d66e5d755efce35b9d in / 
# Sat, 16 May 2020 17:05:47 GMT
CMD ["bash"]
# Fri, 29 May 2020 19:31:18 GMT
ENV OTP_VERSION=23.0.2
# Fri, 29 May 2020 19:31:24 GMT
LABEL org.opencontainers.image.version=23.0.2
# Fri, 29 May 2020 19:42:56 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="6bab92d1a1b20cc319cd845c23db3611cc99f8c99a610d117578262e3c108af3" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Fri, 29 May 2020 19:43:07 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:62a37f23871399015330cfc44332ec26c08885d47ad5e20874fe1e3172922176`  
		Last Modified: Sat, 16 May 2020 18:30:59 GMT  
		Size: 54.1 MB (54144242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea8dd970ca05a86c0f80929f27393568fe548505b95f583acb9497d10345d557`  
		Last Modified: Fri, 29 May 2020 19:53:10 GMT  
		Size: 58.3 MB (58284675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `erlang:23-slim` - linux; s390x

```console
$ docker pull erlang@sha256:916ad8b080889a279cfa16043e02feebbec0cf42e9fd281165a8da9e6590e064
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.3 MB (106343281 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d5b56089c7f322d4b2a22a63c7787050b901f0622fc135273a180c1629b958e`
-	Default Command: `["erl"]`

```dockerfile
# Thu, 14 May 2020 23:06:22 GMT
ADD file:3b65bac2545f5751eaa8e9967febbe18955f63efa32d5ca3f8bc209e1a8602de in / 
# Thu, 14 May 2020 23:06:24 GMT
CMD ["bash"]
# Fri, 29 May 2020 19:48:59 GMT
ENV OTP_VERSION=23.0.2
# Fri, 29 May 2020 19:48:59 GMT
LABEL org.opencontainers.image.version=23.0.2
# Fri, 29 May 2020 19:53:51 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="6bab92d1a1b20cc319cd845c23db3611cc99f8c99a610d117578262e3c108af3" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Fri, 29 May 2020 19:53:53 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:070f0b30acfe8cf53f3aeaae5982c911acd4c4a652a456c849a94c66117d4067`  
		Last Modified: Thu, 14 May 2020 23:11:09 GMT  
		Size: 49.0 MB (48966486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b000757f1cde1a604bfa7e6ba9763a0c76fd2c48c291e0e53e4dbba7c8a383b`  
		Last Modified: Fri, 29 May 2020 20:01:23 GMT  
		Size: 57.4 MB (57376795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
