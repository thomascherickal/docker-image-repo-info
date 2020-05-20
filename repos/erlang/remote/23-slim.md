## `erlang:23-slim`

```console
$ docker pull erlang@sha256:77d8eeee1c49a42187eaeaa7dd412db8073deb10f9e0d8aa93c181c6d486f7df
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
$ docker pull erlang@sha256:6ab4d69b761c364d0239ac399413ba76b8064093be95f7ee472dc78e77b73a4f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.8 MB (110823796 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f7bfc896994b2b3f66e9f131b3de38d2144a516bcb0fb04eacb6ce6691181f6`
-	Default Command: `["erl"]`

```dockerfile
# Fri, 15 May 2020 06:28:12 GMT
ADD file:fb54c709daa205bf9d04eb3d90ba068db4c34dfe3b6ec0d7691f677286120903 in / 
# Fri, 15 May 2020 06:28:13 GMT
CMD ["bash"]
# Wed, 20 May 2020 17:32:07 GMT
ENV OTP_VERSION=23.0.1
# Wed, 20 May 2020 17:32:07 GMT
LABEL org.opencontainers.image.version=23.0.1
# Wed, 20 May 2020 17:41:45 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="25e9d9d4903701e4b86c60b68ac34b4a85f5a5bccfd55fa6a2345f70d84f3de8" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Wed, 20 May 2020 17:41:46 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:376057ac6fa17f65688c56977118e2e764b27c348b3f70637fa829cd2a12b200`  
		Last Modified: Fri, 15 May 2020 06:37:20 GMT  
		Size: 50.4 MB (50391294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad84b68fbfaab9782b73a15258359cbbbc2c1283f4dc646ddb97ee5932e8c202`  
		Last Modified: Wed, 20 May 2020 20:01:22 GMT  
		Size: 60.4 MB (60432502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `erlang:23-slim` - linux; arm variant v7

```console
$ docker pull erlang@sha256:3b57bfaab41aa6851bc6e4ebc2ecd9c3a30618b484124ca428b5fc6232eefcb3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.1 MB (102106980 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:548d793b308ac9390e279a00eeead0f2f1e4cc588a4892e81710d50716e36dd6`
-	Default Command: `["erl"]`

```dockerfile
# Fri, 15 May 2020 00:59:31 GMT
ADD file:d3b126babe4f145c735dff1d1a8828e523967279b9f25d547fce6f4d5422d0a4 in / 
# Fri, 15 May 2020 00:59:33 GMT
CMD ["bash"]
# Wed, 20 May 2020 17:08:06 GMT
ENV OTP_VERSION=23.0.1
# Wed, 20 May 2020 17:08:06 GMT
LABEL org.opencontainers.image.version=23.0.1
# Wed, 20 May 2020 17:14:33 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="25e9d9d4903701e4b86c60b68ac34b4a85f5a5bccfd55fa6a2345f70d84f3de8" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Wed, 20 May 2020 17:14:36 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:33f1e205e6f963868048d05375e218b5a53592240c265ac49b4860e141d25c66`  
		Last Modified: Fri, 15 May 2020 01:11:01 GMT  
		Size: 45.9 MB (45868629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ec2cb7f6ce541ab31f5fac148630f36a5ef3c7d86e358433a98b927f996e67c`  
		Last Modified: Wed, 20 May 2020 18:10:38 GMT  
		Size: 56.2 MB (56238351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `erlang:23-slim` - linux; arm64 variant v8

```console
$ docker pull erlang@sha256:2ad6ae735f2998192d0be1c9424a85c6a0224de6bcd9bd8d8aa129a6a7befefd
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.5 MB (106526939 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:956fcd721d8d30341f433cade8a56b30e40e73e782d83cbbd316f5e22fa3676f`
-	Default Command: `["erl"]`

```dockerfile
# Fri, 15 May 2020 12:43:21 GMT
ADD file:be06dd722febf4e72f7e626f70029986a5c75880941cabd553f695dd66bcbaff in / 
# Fri, 15 May 2020 12:43:25 GMT
CMD ["bash"]
# Wed, 20 May 2020 17:52:35 GMT
ENV OTP_VERSION=23.0.1
# Wed, 20 May 2020 17:52:37 GMT
LABEL org.opencontainers.image.version=23.0.1
# Wed, 20 May 2020 17:59:48 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="25e9d9d4903701e4b86c60b68ac34b4a85f5a5bccfd55fa6a2345f70d84f3de8" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Wed, 20 May 2020 17:59:51 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:d23bf71de5e1fea32788576972e233e80db7c51d831ed7edb269102dab298bf1`  
		Last Modified: Fri, 15 May 2020 12:53:11 GMT  
		Size: 49.2 MB (49170530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68c07142e0806b653e7b4f8e68e5489273590f57b11de0345e3a78b130eba31a`  
		Last Modified: Wed, 20 May 2020 19:01:25 GMT  
		Size: 57.4 MB (57356409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `erlang:23-slim` - linux; 386

```console
$ docker pull erlang@sha256:5cf403c7b80381cce9d91e0096c160be949c38305d23bce37f6f9d8646de3528
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.9 MB (110941525 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bda797b19b365cf53dc5cef20815615a0c2e9ce2b2be4105cec9670b06656d39`
-	Default Command: `["erl"]`

```dockerfile
# Fri, 15 May 2020 07:07:17 GMT
ADD file:8e3b513586e9ff0d65f88b3b2978986693585177fae673aa5432e2934e212cf1 in / 
# Fri, 15 May 2020 07:07:17 GMT
CMD ["bash"]
# Wed, 20 May 2020 17:56:51 GMT
ENV OTP_VERSION=23.0.1
# Wed, 20 May 2020 17:56:51 GMT
LABEL org.opencontainers.image.version=23.0.1
# Wed, 20 May 2020 18:13:49 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="25e9d9d4903701e4b86c60b68ac34b4a85f5a5bccfd55fa6a2345f70d84f3de8" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Wed, 20 May 2020 18:13:50 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:8f68852a383b581a180c01bf6d2f7039194fed91451d0686630c59cb80d321c3`  
		Last Modified: Fri, 15 May 2020 07:17:49 GMT  
		Size: 51.2 MB (51157846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6956d5f90b70204fc3e1565f9f98df0b6d6ce2142406089957600c22ac3dc7b9`  
		Last Modified: Wed, 20 May 2020 20:40:36 GMT  
		Size: 59.8 MB (59783679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `erlang:23-slim` - linux; ppc64le

```console
$ docker pull erlang@sha256:829a3cd5255d4eb6fb765f91e9097cd2c244c32830d31127d252393865e086ef
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.4 MB (112426521 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aff708da1abcc7415be0f97ef53356d4b7227fd8c0c0f489fbce1aa8fe771639`
-	Default Command: `["erl"]`

```dockerfile
# Sat, 16 May 2020 17:05:45 GMT
ADD file:cbc72fbbd9297b44feea736c6c3446962657f02799b5f7d66e5d755efce35b9d in / 
# Sat, 16 May 2020 17:05:47 GMT
CMD ["bash"]
# Wed, 20 May 2020 18:07:22 GMT
ENV OTP_VERSION=23.0.1
# Wed, 20 May 2020 18:07:25 GMT
LABEL org.opencontainers.image.version=23.0.1
# Wed, 20 May 2020 18:19:14 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="25e9d9d4903701e4b86c60b68ac34b4a85f5a5bccfd55fa6a2345f70d84f3de8" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Wed, 20 May 2020 18:19:30 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:62a37f23871399015330cfc44332ec26c08885d47ad5e20874fe1e3172922176`  
		Last Modified: Sat, 16 May 2020 18:30:59 GMT  
		Size: 54.1 MB (54144242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27c04ce8c384004176c9f0a3bd02e8237f0bc1a3fe048363068dc2fc55d371ce`  
		Last Modified: Wed, 20 May 2020 19:45:48 GMT  
		Size: 58.3 MB (58282279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `erlang:23-slim` - linux; s390x

```console
$ docker pull erlang@sha256:f0a271c7d7eefd8100f4b2091db5f786be7bf91cab5cf4bac0543e790437cacb
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.3 MB (106343786 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:717bd58fc06e2286e7e4fe10dc96ffb56cf4608dc0586c53fa5f655630dc7556`
-	Default Command: `["erl"]`

```dockerfile
# Thu, 14 May 2020 23:06:22 GMT
ADD file:3b65bac2545f5751eaa8e9967febbe18955f63efa32d5ca3f8bc209e1a8602de in / 
# Thu, 14 May 2020 23:06:24 GMT
CMD ["bash"]
# Wed, 20 May 2020 17:49:04 GMT
ENV OTP_VERSION=23.0.1
# Wed, 20 May 2020 17:49:04 GMT
LABEL org.opencontainers.image.version=23.0.1
# Wed, 20 May 2020 17:54:42 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="25e9d9d4903701e4b86c60b68ac34b4a85f5a5bccfd55fa6a2345f70d84f3de8" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Wed, 20 May 2020 17:54:44 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:070f0b30acfe8cf53f3aeaae5982c911acd4c4a652a456c849a94c66117d4067`  
		Last Modified: Thu, 14 May 2020 23:11:09 GMT  
		Size: 49.0 MB (48966486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:473c7ccef3949dea884e5dd8e7c847e8499b180be5f04fc82d4015a1f669a52d`  
		Last Modified: Wed, 20 May 2020 18:31:42 GMT  
		Size: 57.4 MB (57377300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
